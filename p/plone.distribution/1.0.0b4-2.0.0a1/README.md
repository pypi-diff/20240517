# Comparing `tmp/plone.distribution-1.0.0b4.tar.gz` & `tmp/plone_distribution-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.distribution-1.0.0b4.tar", last modified: Wed Apr  3 10:04:16 2024, max compression
+gzip compressed data, was "plone_distribution-2.0.0a1.tar", last modified: Wed May 15 23:34:42 2024, max compression
```

## Comparing `plone.distribution-1.0.0b4.tar` & `plone_distribution-2.0.0a1.tar`

### file list

```diff
@@ -1,170 +1,178 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.773026 plone.distribution-1.0.0b4/
--rw-r--r--   0 maurits    (501) staff       (20)     1365 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/.editorconfig
--rw-r--r--   0 maurits    (501) staff       (20)      538 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/.flake8
--rw-r--r--   0 maurits    (501) staff       (20)      709 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/.gitignore
--rw-r--r--   0 maurits    (501) staff       (20)      740 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/.meta.toml
--rw-r--r--   0 maurits    (501) staff       (20)     2024 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/.pre-commit-config.yaml
--rw-r--r--   0 maurits    (501) staff       (20)     2927 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/CHANGES.md
--rw-r--r--   0 maurits    (501) staff       (20)       95 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/CONTRIBUTING.md
--rw-r--r--   0 maurits    (501) staff       (20)    18092 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/LICENSE
--rw-r--r--   0 maurits    (501) staff       (20)      299 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     5109 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/Makefile
--rw-r--r--   0 maurits    (501) staff       (20)    12950 2024-04-03 10:04:16.772569 plone.distribution-1.0.0b4/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     8816 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/README.md
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/constraints.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.740184 plone.distribution-1.0.0b4/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     7078 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/Makefile
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.741349 plone.distribution-1.0.0b4/docs/_static/
--rw-r--r--   0 maurits    (501) staff       (20)     5430 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/_static/favicon.ico
--rw-r--r--   0 maurits    (501) staff       (20)     3775 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/_static/logo.svg
--rw-r--r--   0 maurits    (501) staff       (20)       30 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/_static/print.css
--rw-r--r--   0 maurits    (501) staff       (20)     7814 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/_static/styles.css
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.742224 plone.distribution-1.0.0b4/docs/api/
--rw-r--r--   0 maurits    (501) staff       (20)      469 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/api/distribution.md
--rw-r--r--   0 maurits    (501) staff       (20)      709 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/api/index.md
--rw-r--r--   0 maurits    (501) staff       (20)      439 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/api/site.md
--rw-r--r--   0 maurits    (501) staff       (20)     2813 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/conf.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.742515 plone.distribution-1.0.0b4/docs/development/
--rw-r--r--   0 maurits    (501) staff       (20)       26 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/development/index.md
--rw-r--r--   0 maurits    (501) staff       (20)     1329 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/index.md
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.743664 plone.distribution-1.0.0b4/docs/usage/
--rw-r--r--   0 maurits    (501) staff       (20)     2560 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/usage/code-examples.md
--rw-r--r--   0 maurits    (501) staff       (20)     2528 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/usage/index.md
--rw-r--r--   0 maurits    (501) staff       (20)     5886 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/usage/package-structure.md
--rw-r--r--   0 maurits    (501) staff       (20)     2683 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/usage/zcml.md
--rw-r--r--   0 maurits    (501) staff       (20)      172 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/instance.yaml
--rw-r--r--   0 maurits    (501) staff       (20)      251 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/mx.ini
--rw-r--r--   0 maurits    (501) staff       (20)     4578 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      393 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/requirements-docs.txt
--rw-r--r--   0 maurits    (501) staff       (20)       33 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/requirements.txt
--rw-r--r--   0 maurits    (501) staff       (20)       38 2024-04-03 10:04:16.773104 plone.distribution-1.0.0b4/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2448 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.729261 plone.distribution-1.0.0b4/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.743964 plone.distribution-1.0.0b4/src/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.748906 plone.distribution-1.0.0b4/src/plone/distribution/
--rw-r--r--   0 maurits    (501) staff       (20)      221 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.749722 plone.distribution-1.0.0b4/src/plone/distribution/api/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/api/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1912 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/api/distribution.py
--rw-r--r--   0 maurits    (501) staff       (20)     6617 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/api/site.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.751053 plone.distribution-1.0.0b4/src/plone/distribution/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2547 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/browser/admin.py
--rw-r--r--   0 maurits    (501) staff       (20)      970 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1286 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/browser/image.py
--rw-r--r--   0 maurits    (501) staff       (20)     1055 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/browser/overrides.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.752952 plone.distribution-1.0.0b4/src/plone/distribution/browser/static/
--rw-r--r--   0 maurits    (501) staff       (20)     1185 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/browser/static/plone-logo.png
--rw-r--r--   0 maurits    (501) staff       (20)     2240 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/browser/static/plone-overview.min.css
--rw-r--r--   0 maurits    (501) staff       (20)   581628 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/browser/static/plone-overview.min.js
--rw-r--r--   0 maurits    (501) staff       (20)      812 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/browser/static/plone.svg
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.753240 plone.distribution-1.0.0b4/src/plone/distribution/browser/templates/
--rw-r--r--   0 maurits    (501) staff       (20)     1431 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/browser/templates/plone-overview.pt
--rw-r--r--   0 maurits    (501) staff       (20)      446 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3892 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/core.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.730780 plone.distribution-1.0.0b4/src/plone/distribution/distributions/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.754442 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.755259 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/
--rw-r--r--   0 maurits    (501) staff       (20)      336 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/defaultpages.json
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.756848 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/items/
--rw-r--r--   0 maurits    (501) staff       (20)     5166 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/items/1.json
--rw-r--r--   0 maurits    (501) staff       (20)     1324 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/items/2.json
--rw-r--r--   0 maurits    (501) staff       (20)     1885 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/items/3.json
--rw-r--r--   0 maurits    (501) staff       (20)     2261 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/items/4.json
--rw-r--r--   0 maurits    (501) staff       (20)     1881 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/items/5.json
--rw-r--r--   0 maurits    (501) staff       (20)     2256 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/items/6.json
--rw-r--r--   0 maurits    (501) staff       (20)      425 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/ordering.json
--rw-r--r--   0 maurits    (501) staff       (20)     2799 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/portlets.json
--rw-r--r--   0 maurits    (501) staff       (20)   293282 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/image.png
--rw-r--r--   0 maurits    (501) staff       (20)      148 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/profiles.json
--rw-r--r--   0 maurits    (501) staff       (20)     1280 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/schema.json
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.757941 plone.distribution-1.0.0b4/src/plone/distribution/distributions/default/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.731065 plone.distribution-1.0.0b4/src/plone/distribution/distributions/default/content/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.758191 plone.distribution-1.0.0b4/src/plone/distribution/distributions/default/content/items/
--rw-r--r--   0 maurits    (501) staff       (20)      712 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/default/content/items/1.json
--rw-r--r--   0 maurits    (501) staff       (20)   218233 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/default/image.png
--rw-r--r--   0 maurits    (501) staff       (20)      175 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/default/profiles.json
--rw-r--r--   0 maurits    (501) staff       (20)     1267 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/default/schema.json
--rw-r--r--   0 maurits    (501) staff       (20)      514 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.760076 plone.distribution-1.0.0b4/src/plone/distribution/exportimport/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/exportimport/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1415 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/exportimport/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5172 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/exportimport/dist_export.py
--rw-r--r--   0 maurits    (501) staff       (20)     4696 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/exportimport/dist_import.py
--rw-r--r--   0 maurits    (501) staff       (20)     2762 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/exportimport/helpers.py
--rw-r--r--   0 maurits    (501) staff       (20)      522 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/exportimport/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     3345 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/exportimport/serializer.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.760557 plone.distribution-1.0.0b4/src/plone/distribution/exportimport/templates/
--rw-r--r--   0 maurits    (501) staff       (20)     3756 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/exportimport/templates/export_all.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1241 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/exportimport/templates/import_all.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1457 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/handler.py
--rw-r--r--   0 maurits    (501) staff       (20)      698 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      391 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/meta.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3531 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/metaconfigure.py
--rw-r--r--   0 maurits    (501) staff       (20)     4174 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/registry.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.761435 plone.distribution-1.0.0b4/src/plone/distribution/services/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/services/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.762317 plone.distribution-1.0.0b4/src/plone/distribution/services/auth/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/services/auth/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      348 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/services/auth/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1301 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/services/auth/login.py
--rw-r--r--   0 maurits    (501) staff       (20)      412 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/services/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      582 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/services/overrides.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.763397 plone.distribution-1.0.0b4/src/plone/distribution/services/sites/
--rw-r--r--   0 maurits    (501) staff       (20)       77 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/services/sites/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2105 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/services/sites/add.py
--rw-r--r--   0 maurits    (501) staff       (20)      895 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/services/sites/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4882 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/services/sites/get.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.764201 plone.distribution-1.0.0b4/src/plone/distribution/services/system/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/services/system/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      332 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/services/system/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1112 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/services/system/get.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.765060 plone.distribution-1.0.0b4/src/plone/distribution/testing/
--rw-r--r--   0 maurits    (501) staff       (20)      149 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/testing/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3129 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/testing/layer.py
--rw-r--r--   0 maurits    (501) staff       (20)     1017 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/testing/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.766119 plone.distribution-1.0.0b4/src/plone/distribution/utils/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/utils/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      914 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/utils/request.py
--rw-r--r--   0 maurits    (501) staff       (20)     5065 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/utils/schema.py
--rw-r--r--   0 maurits    (501) staff       (20)      870 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/utils/validation.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.746327 plone.distribution-1.0.0b4/src/plone.distribution.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    12950 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone.distribution.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     5018 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone.distribution.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone.distribution.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone.distribution.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone.distribution.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone.distribution.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      365 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone.distribution.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone.distribution.egg-info/top_level.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.766553 plone.distribution-1.0.0b4/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.767027 plone.distribution-1.0.0b4/tests/api/
--rw-r--r--   0 maurits    (501) staff       (20)     1524 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/api/test_api_distribution.py
--rw-r--r--   0 maurits    (501) staff       (20)     2152 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/api/test_api_site.py
--rw-r--r--   0 maurits    (501) staff       (20)      363 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/conftest.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.768329 plone.distribution-1.0.0b4/tests/distributions/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/distributions/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      322 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/distributions/conftest.py
--rw-r--r--   0 maurits    (501) staff       (20)     1895 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/distributions/test_distributions_classic.py
--rw-r--r--   0 maurits    (501) staff       (20)     1765 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/distributions/test_distributions_default.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.769022 plone.distribution-1.0.0b4/tests/exportimport/
--rw-r--r--   0 maurits    (501) staff       (20)    12736 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/exportimport/portal.json
--rw-r--r--   0 maurits    (501) staff       (20)     2344 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/exportimport/test_exportimport_helpers.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.770071 plone.distribution-1.0.0b4/tests/services/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/services/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      243 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/services/conftest.py
--rw-r--r--   0 maurits    (501) staff       (20)     4839 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/services/test_services_site.py
--rw-r--r--   0 maurits    (501) staff       (20)     2445 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/services/test_services_system.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.771480 plone.distribution-1.0.0b4/tests/utils/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/utils/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      519 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/utils/conftest.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.772176 plone.distribution-1.0.0b4/tests/utils/data/
--rw-r--r--   0 maurits    (501) staff       (20)      969 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/utils/data/invalid.json
--rw-r--r--   0 maurits    (501) staff       (20)     1267 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/utils/data/valid.json
--rw-r--r--   0 maurits    (501) staff       (20)     1328 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/utils/data/with_default_language.json
--rw-r--r--   0 maurits    (501) staff       (20)     1205 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/utils/test_utils_request.py
--rw-r--r--   0 maurits    (501) staff       (20)     2907 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/utils/test_utils_schema.py
--rw-r--r--   0 maurits    (501) staff       (20)     1692 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/utils/test_utils_validation.py
--rw-r--r--   0 maurits    (501) staff       (20)     4885 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tox.ini
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.724026 plone_distribution-2.0.0a1/
+-rw-r--r--   0 ericof     (501) staff       (20)     1381 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/.editorconfig
+-rw-r--r--   0 ericof     (501) staff       (20)      538 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/.flake8
+-rw-r--r--   0 ericof     (501) staff       (20)      709 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/.gitignore
+-rw-r--r--   0 ericof     (501) staff       (20)      705 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/.meta.toml
+-rw-r--r--   0 ericof     (501) staff       (20)     2023 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/.pre-commit-config.yaml
+-rw-r--r--   0 ericof     (501) staff       (20)     4290 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/CHANGES.md
+-rw-r--r--   0 ericof     (501) staff       (20)       95 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/CONTRIBUTING.md
+-rw-r--r--   0 ericof     (501) staff       (20)    18092 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/LICENSE
+-rw-r--r--   0 ericof     (501) staff       (20)      320 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/MANIFEST.in
+-rw-r--r--   0 ericof     (501) staff       (20)     5109 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/Makefile
+-rw-r--r--   0 ericof     (501) staff       (20)    15461 2024-05-15 23:34:42.723714 plone_distribution-2.0.0a1/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)     9010 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/README.md
+-rw-r--r--   0 ericof     (501) staff       (20)       59 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/constraints.txt
+-rw-r--r--   0 ericof     (501) staff       (20)      322 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/dependabot.yml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.706995 plone_distribution-2.0.0a1/docs/
+-rw-r--r--   0 ericof     (501) staff       (20)     7078 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/docs/Makefile
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.707498 plone_distribution-2.0.0a1/docs/_static/
+-rw-r--r--   0 ericof     (501) staff       (20)     5430 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/docs/_static/favicon.ico
+-rw-r--r--   0 ericof     (501) staff       (20)     3775 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/docs/_static/logo.svg
+-rw-r--r--   0 ericof     (501) staff       (20)       30 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/docs/_static/print.css
+-rw-r--r--   0 ericof     (501) staff       (20)     7814 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/docs/_static/styles.css
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.707894 plone_distribution-2.0.0a1/docs/api/
+-rw-r--r--   0 ericof     (501) staff       (20)      469 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/docs/api/distribution.md
+-rw-r--r--   0 ericof     (501) staff       (20)      709 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/docs/api/index.md
+-rw-r--r--   0 ericof     (501) staff       (20)      439 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/docs/api/site.md
+-rw-r--r--   0 ericof     (501) staff       (20)     2813 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/docs/conf.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.708006 plone_distribution-2.0.0a1/docs/development/
+-rw-r--r--   0 ericof     (501) staff       (20)       26 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/docs/development/index.md
+-rw-r--r--   0 ericof     (501) staff       (20)     1329 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/docs/index.md
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.708502 plone_distribution-2.0.0a1/docs/usage/
+-rw-r--r--   0 ericof     (501) staff       (20)     2584 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/docs/usage/code-examples.md
+-rw-r--r--   0 ericof     (501) staff       (20)     2528 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/docs/usage/index.md
+-rw-r--r--   0 ericof     (501) staff       (20)     5441 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/docs/usage/package-structure.md
+-rw-r--r--   0 ericof     (501) staff       (20)     2683 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/docs/usage/zcml.md
+-rw-r--r--   0 ericof     (501) staff       (20)      158 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/instance.yaml
+-rw-r--r--   0 ericof     (501) staff       (20)      251 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/mx.ini
+-rw-r--r--   0 ericof     (501) staff       (20)     4674 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/pyproject.toml
+-rw-r--r--   0 ericof     (501) staff       (20)      393 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/requirements-docs.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       33 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/requirements.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       38 2024-05-15 23:34:42.724072 plone_distribution-2.0.0a1/setup.cfg
+-rw-r--r--   0 ericof     (501) staff       (20)     2609 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/setup.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.701760 plone_distribution-2.0.0a1/src/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.708613 plone_distribution-2.0.0a1/src/plone/
+-rw-r--r--   0 ericof     (501) staff       (20)       56 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.710837 plone_distribution-2.0.0a1/src/plone/distribution/
+-rw-r--r--   0 ericof     (501) staff       (20)      222 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.711248 plone_distribution-2.0.0a1/src/plone/distribution/api/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/api/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3061 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/api/distribution.py
+-rw-r--r--   0 ericof     (501) staff       (20)     6107 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/api/site.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.711947 plone_distribution-2.0.0a1/src/plone/distribution/browser/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/browser/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2547 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/browser/admin.py
+-rw-r--r--   0 ericof     (501) staff       (20)      970 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/browser/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     1286 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/browser/image.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1055 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/browser/overrides.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.712815 plone_distribution-2.0.0a1/src/plone/distribution/browser/static/
+-rw-r--r--   0 ericof     (501) staff       (20)     1185 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/browser/static/plone-logo.png
+-rw-r--r--   0 ericof     (501) staff       (20)     2240 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/browser/static/plone-overview.min.css
+-rw-r--r--   0 ericof     (501) staff       (20)   581612 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/browser/static/plone-overview.min.js
+-rw-r--r--   0 ericof     (501) staff       (20)      812 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/browser/static/plone.svg
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.712957 plone_distribution-2.0.0a1/src/plone/distribution/browser/templates/
+-rw-r--r--   0 ericof     (501) staff       (20)     1431 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/browser/templates/plone-overview.pt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.713095 plone_distribution-2.0.0a1/src/plone/distribution/cli/
+-rw-r--r--   0 ericof     (501) staff       (20)     1609 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/cli/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      381 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     3899 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/core.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.702935 plone_distribution-2.0.0a1/src/plone/distribution/distributions/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.713681 plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.714480 plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.714627 plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/content/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.714759 plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/content/4053ffb6901342ac991afb54da15ab77/
+-rw-r--r--   0 ericof     (501) staff       (20)     1608 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/content/4053ffb6901342ac991afb54da15ab77/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.714885 plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/content/54163be595184b4eb0a0b82a58b8def8/
+-rw-r--r--   0 ericof     (501) staff       (20)     1210 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/content/54163be595184b4eb0a0b82a58b8def8/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.715013 plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/content/61f6d382910945ea95f2e78a14ebb170/
+-rw-r--r--   0 ericof     (501) staff       (20)     2228 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/content/61f6d382910945ea95f2e78a14ebb170/data.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1700 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/content/__metadata__.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.715149 plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/content/ab584c1a6fae465da2283a0962f80114/
+-rw-r--r--   0 ericof     (501) staff       (20)     1612 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/content/ab584c1a6fae465da2283a0962f80114/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.715301 plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/content/ee556c50736a4650839e2ada6dd65454/
+-rw-r--r--   0 ericof     (501) staff       (20)     2223 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/content/ee556c50736a4650839e2ada6dd65454/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.715440 plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/content/plone_site_root/
+-rw-r--r--   0 ericof     (501) staff       (20)     5310 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/content/plone_site_root/data.json
+-rw-r--r--   0 ericof     (501) staff       (20)        2 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/discussions.json
+-rw-r--r--   0 ericof     (501) staff       (20)     3415 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/portlets.json
+-rw-r--r--   0 ericof     (501) staff       (20)      685 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/principals.json
+-rw-r--r--   0 ericof     (501) staff       (20)        2 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/redirects.json
+-rw-r--r--   0 ericof     (501) staff       (20)        2 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/relations.json
+-rw-r--r--   0 ericof     (501) staff       (20)        2 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/translations.json
+-rw-r--r--   0 ericof     (501) staff       (20)   293282 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/image.png
+-rw-r--r--   0 ericof     (501) staff       (20)      148 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/profiles.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1280 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/schema.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.716029 plone_distribution-2.0.0a1/src/plone/distribution/distributions/default/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.716726 plone_distribution-2.0.0a1/src/plone/distribution/distributions/default/content/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.716871 plone_distribution-2.0.0a1/src/plone/distribution/distributions/default/content/content/
+-rw-r--r--   0 ericof     (501) staff       (20)      299 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/distributions/default/content/content/__metadata__.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.717017 plone_distribution-2.0.0a1/src/plone/distribution/distributions/default/content/content/plone_site_root/
+-rw-r--r--   0 ericof     (501) staff       (20)      754 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/distributions/default/content/content/plone_site_root/data.json
+-rw-r--r--   0 ericof     (501) staff       (20)        2 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/distributions/default/content/discussions.json
+-rw-r--r--   0 ericof     (501) staff       (20)      685 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/distributions/default/content/principals.json
+-rw-r--r--   0 ericof     (501) staff       (20)        2 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/distributions/default/content/redirects.json
+-rw-r--r--   0 ericof     (501) staff       (20)        2 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/distributions/default/content/relations.json
+-rw-r--r--   0 ericof     (501) staff       (20)        2 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/distributions/default/content/translations.json
+-rw-r--r--   0 ericof     (501) staff       (20)   218233 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/distributions/default/image.png
+-rw-r--r--   0 ericof     (501) staff       (20)      175 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/distributions/default/profiles.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1382 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/distributions/default/schema.json
+-rw-r--r--   0 ericof     (501) staff       (20)      600 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/distributions.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     2167 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/handler.py
+-rw-r--r--   0 ericof     (501) staff       (20)      698 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/interfaces.py
+-rw-r--r--   0 ericof     (501) staff       (20)      391 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/meta.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     3531 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/metaconfigure.py
+-rw-r--r--   0 ericof     (501) staff       (20)     4174 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/registry.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.717390 plone_distribution-2.0.0a1/src/plone/distribution/services/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/services/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.717761 plone_distribution-2.0.0a1/src/plone/distribution/services/auth/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/services/auth/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      348 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/services/auth/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     1302 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/services/auth/login.py
+-rw-r--r--   0 ericof     (501) staff       (20)      412 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/services/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)      575 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/services/overrides.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.718319 plone_distribution-2.0.0a1/src/plone/distribution/services/sites/
+-rw-r--r--   0 ericof     (501) staff       (20)       77 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/services/sites/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2251 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/services/sites/add.py
+-rw-r--r--   0 ericof     (501) staff       (20)      895 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/services/sites/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     4882 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/services/sites/get.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.718727 plone_distribution-2.0.0a1/src/plone/distribution/services/system/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/services/system/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      325 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/services/system/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     1060 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/services/system/get.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.719410 plone_distribution-2.0.0a1/src/plone/distribution/testing/
+-rw-r--r--   0 ericof     (501) staff       (20)      149 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/testing/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3349 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/testing/layer.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1195 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/testing/testing.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.720061 plone_distribution-2.0.0a1/src/plone/distribution/utils/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/utils/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      489 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/utils/data.py
+-rw-r--r--   0 ericof     (501) staff       (20)      914 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/utils/request.py
+-rw-r--r--   0 ericof     (501) staff       (20)     5065 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/utils/schema.py
+-rw-r--r--   0 ericof     (501) staff       (20)      870 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone/distribution/utils/validation.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.722732 plone_distribution-2.0.0a1/src/plone.distribution.egg-info/
+-rw-r--r--   0 ericof     (501) staff       (20)    15461 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone.distribution.egg-info/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)     5537 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone.distribution.egg-info/SOURCES.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone.distribution.egg-info/dependency_links.txt
+-rw-r--r--   0 ericof     (501) staff       (20)      111 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone.distribution.egg-info/entry_points.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        6 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone.distribution.egg-info/namespace_packages.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone.distribution.egg-info/not-zip-safe
+-rw-r--r--   0 ericof     (501) staff       (20)      400 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone.distribution.egg-info/requires.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        6 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/src/plone.distribution.egg-info/top_level.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.720280 plone_distribution-2.0.0a1/tests/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/tests/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.720528 plone_distribution-2.0.0a1/tests/api/
+-rw-r--r--   0 ericof     (501) staff       (20)     1524 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/tests/api/test_api_distribution.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2212 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/tests/api/test_api_site.py
+-rw-r--r--   0 ericof     (501) staff       (20)      363 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/tests/conftest.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.720996 plone_distribution-2.0.0a1/tests/distributions/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/tests/distributions/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      322 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/tests/distributions/conftest.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2230 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/tests/distributions/test_distributions_classic.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2100 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/tests/distributions/test_distributions_default.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.721490 plone_distribution-2.0.0a1/tests/services/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/tests/services/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      243 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/tests/services/conftest.py
+-rw-r--r--   0 ericof     (501) staff       (20)     4839 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/tests/services/test_services_site.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2453 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/tests/services/test_services_system.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.722174 plone_distribution-2.0.0a1/tests/utils/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/tests/utils/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      519 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/tests/utils/conftest.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 23:34:42.722538 plone_distribution-2.0.0a1/tests/utils/data/
+-rw-r--r--   0 ericof     (501) staff       (20)      969 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/tests/utils/data/invalid.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1267 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/tests/utils/data/valid.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1328 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/tests/utils/data/with_default_language.json
+-rw-r--r--   0 ericof     (501) staff       (20)      832 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/tests/utils/test_utils_data.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1205 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/tests/utils/test_utils_request.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2907 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/tests/utils/test_utils_schema.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1692 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/tests/utils/test_utils_validation.py
+-rw-r--r--   0 ericof     (501) staff       (20)     5223 2024-05-15 23:34:42.000000 plone_distribution-2.0.0a1/tox.ini
```

### Comparing `plone.distribution-1.0.0b4/.editorconfig` & `plone_distribution-2.0.0a1/.editorconfig`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 # file types
 
 # top-most EditorConfig file:
 # Will ignore other EditorConfig files in Home directory or upper tree level.
 root = true
 
 
-[*]  # For All Files
+[*]
+# Default settings for all files.
 # Unix-style newlines with a newline ending every file
 end_of_line = lf
 insert_final_newline = true
 trim_trailing_whitespace = true
 # Set default charset
 charset = utf-8
 # Indent style default
@@ -29,15 +30,16 @@
 # 4 space indentation
 indent_size = 4
 
 [*.{yml,zpt,pt,dtml,zcml,html,xml}]
 # 2 space indentation
 indent_size = 2
 
-[*.{json,jsonl,js,jsx,ts,tsx,css,less,scss}]  # Frontend development
+[*.{json,jsonl,js,jsx,ts,tsx,css,less,scss}]
+# Frontend development
 # 2 space indentation
 indent_size = 2
 max_line_length = 80
 
 [{Makefile,.gitmodules}]
 # Tab indentation (no size specified, but view as 4 spaces)
 indent_style = tab
```

### Comparing `plone.distribution-1.0.0b4/.flake8` & `plone_distribution-2.0.0a1/.flake8`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/.gitignore` & `plone_distribution-2.0.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/.meta.toml` & `plone_distribution-2.0.0a1/.meta.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 # Generated from:
 # https://github.com/plone/meta/tree/main/config/default
 # See the inline comments on how to expand/tweak this configuration file
 [meta]
 template = "default"
-commit-id = "6e36bcc4"
+commit-id = "71d0218b"
 
 [pyproject]
 codespell_skip = "*.min.js"
 codespell_ignores = "vew"
-dependencies_ignores = "['plone.volto', 'zestreleaser.towncrier', 'zest.releaser', 'pytest', 'pytest-cov', 'pytest-plone', 'plone.testing', 'plone.app.testing']"
-dependencies_mappings = [
-    "Plone = ['Products.CMFPlone', 'Products.CMFCore', 'Products.GenericSetup']",
-    ]
+dependencies_ignores = "['plone.app.iterate', 'plone.app.upgrade', 'plone.volto', 'zestreleaser.towncrier', 'zest.releaser', 'pytest', 'pytest-cov', 'pytest-plone', 'plone.testing', 'plone.app.testing']"
 
 [tox]
 test_runner = "pytest"
 test_path = "/tests"
 use_mxdev = true
 test_deps_additional = ""
 
 [github]
+py_versions = "[\"3.11\", \"3.10\"]"
 jobs = [
     "qa",
     "test",
     "coverage",
     "dependencies",
     "release_ready",
     ]
```

### Comparing `plone.distribution-1.0.0b4/.pre-commit-config.yaml` & `plone_distribution-2.0.0a1/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # See the inline comments on how to expand/tweak this configuration file
 ci:
     autofix_prs: false
     autoupdate_schedule: monthly
 
 repos:
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.15.0
+    rev: v3.15.2
     hooks:
     -   id: pyupgrade
         args: [--py38-plus]
 -   repo: https://github.com/pycqa/isort
     rev: 5.13.2
     hooks:
     -   id: isort
 -   repo: https://github.com/psf/black
-    rev: 23.12.1
+    rev: 24.4.2
     hooks:
     -   id: black
 -   repo: https://github.com/collective/zpretty
     rev: 3.1.0
     hooks:
     -   id: zpretty
 
@@ -28,15 +28,15 @@
 # Add extra configuration options in .meta.toml:
 #  [pre_commit]
 #  zpretty_extra_lines = """
 #  _your own configuration lines_
 #  """
 ##
 -   repo: https://github.com/PyCQA/flake8
-    rev: 6.1.0
+    rev: 7.0.0
     hooks:
     -   id: flake8
 
 ##
 # Add extra configuration options in .meta.toml:
 #  [pre_commit]
 #  flake8_extra_lines = """
@@ -67,15 +67,15 @@
     -   id: pyroma
 -   repo: https://github.com/mgedmin/check-python-versions
     rev: "0.22.0"
     hooks:
     -   id: check-python-versions
         args: ['--only', 'setup.py,pyproject.toml']
 -   repo: https://github.com/collective/i18ndude
-    rev: "6.1.0"
+    rev: "6.2.0"
     hooks:
     -   id: i18ndude
 
 
 ##
 # Add extra configuration options in .meta.toml:
 #  [pre_commit]
```

### Comparing `plone.distribution-1.0.0b4/CHANGES.md` & `plone_distribution-2.0.0a1/CHANGES.md`

 * *Files 27% similar despite different names*

```diff
@@ -5,14 +5,51 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 2.0.0a1 (2024-05-16)
+
+
+### Breaking changes:
+
+- plone.distribution is now based on plone.exportimport instead of collective.exportimport.
+
+  There are some backwards-incompatible changes in the export format.
+  To convert an existing distribution to the new format, use the following steps:
+  1. Create a site from the distribution using plone.distribution 1.0.x
+  2. Install plone.distribution 2.0.x
+  3. Delete the distribution's `contents/items` folder.
+  4. Export the distribution in the new format using the `bin/export-distribution` script.
+
+  @davisagli, @ericof #61
+
+
+### New features:
+
+- Default distribution: Allow users to upload a logo during site creation [@ericof] #66
+- Classic distribution: Allow users to upload a logo during site creation [@ericof] #67
+- Remove dependency on Plone package, add dependency on Products.CMFPlone [@ericof] #70
+
+
+### Bug fixes:
+
+- Get the name of the existing distribution from the report, not the answers [@ericof] #60
+- Fix issue with payload for new site creation breaking with certain plone.rest versions [@ericof] #71
+- Read profile.json by the pathlib.Path.read_text method to avoid the unclosed file exception [@folix-01] #75
+
+
+### Internal:
+
+- Update `plone/meta` configuration [@ericof] #73
+- Log traceback when creating a site fails [@pbauer] #82
+- Bump `plone.exportimport` to 1.0.0a5 [@ericof] #83
+
 ## 1.0.0b4 (2024-04-03)
 
 
 ### Bug fixes:
 
 - Fix exporting files.
   [pbauer] #58
```

### Comparing `plone.distribution-1.0.0b4/LICENSE` & `plone_distribution-2.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/Makefile` & `plone_distribution-2.0.0a1/Makefile`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/PKG-INFO` & `plone_distribution-2.0.0a1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.distribution
-Version: 1.0.0b4
+Version: 2.0.0a1
 Summary: Plone distribution support
 Home-page: https://plone.org
 Author: Plone Foundation
 Author-email: releasemanager@plone.org
 License: GPL version 2
 Project-URL: Homepage, https://plone.org
 Project-URL: Documentation, https://6.docs.plone.org
@@ -22,57 +22,84 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: Products.CMFPlone
+Requires-Dist: Products.GenericSetup
+Requires-Dist: Zope
+Requires-Dist: setuptools
+Requires-Dist: jsonschema
+Requires-Dist: plone.api
+Requires-Dist: plone.base
+Requires-Dist: plone.dexterity
+Requires-Dist: plone.exportimport>=1.0.0a5
+Requires-Dist: plone.i18n
+Requires-Dist: plone.protect
+Requires-Dist: plone.rest
+Requires-Dist: plone.restapi
+Requires-Dist: z3c.unconfigure
+Provides-Extra: test
+Requires-Dist: plone.app.iterate; extra == "test"
+Requires-Dist: plone.app.testing; extra == "test"
+Requires-Dist: plone.app.upgrade; extra == "test"
+Requires-Dist: plone.restapi[test]; extra == "test"
+Requires-Dist: plone.volto[test]; extra == "test"
+Requires-Dist: plone.testing; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-plone>=0.5.0; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: zest.releaser[recommended]; extra == "test"
+Requires-Dist: zestreleaser.towncrier; extra == "test"
 
 
 <p align="center">
     <img alt="Plone Logo" width="200px" src="https://raw.githubusercontent.com/plone/.github/main/plone-logo.png">
 </p>
 
 <h1 align="center">
   Plone Distributions
 </h1>
 
-Package supporting the (easy) implementation of a Plone Distribution.
+Package supporting the (easy) implementation of a Plone distribution.
 
-## What is a Plone Distribution
+## What is a Plone distribution
 
-A Plone distribution is a pre-packaged version of Plone that includes specific features, themes, modules, and configurations. It is a convenient way to get a specific type of website up and running quickly, as the distribution includes everything needed to run that type of site.
+A Plone distribution is a pre-packaged version of Plone that includes specific features, themes, modules, and configurations.
+It is a convenient way to get a specific type of website up and running quickly, as the distribution includes everything needed to run that type of site.
 
 Examples of Plone distributions include:
 
-* [SENAITE](https://www.senaite.com)
-* [Quaive](https://quaivecloud.com/)
-* [Portal Modelo](https://www.interlegis.leg.br/produtos-servicos/portal-modelo/)
-* [Portal Padrão](https://identidade-digital-de-governo-plone.readthedocs.io/en/latest/)
+- [SENAITE](https://www.senaite.com)
+- [Quaive](https://quaivecloud.com/)
+- [Portal Modelo](https://www.interlegis.leg.br/produtos-servicos/portal-modelo/)
+- [Portal Padrão](https://identidade-digital-de-governo-plone.readthedocs.io/en/latest/)
 
 ### Similar Concept in Other CMS
 
-* Drupal: Drupal has distributions for blogs, e-commerce sites, and intranet portals.
+- **Drupal:** Drupal has distributions for blogs, e-commerce sites, and intranet portals.
 
-* WordPress: WordPress has a similar concept in the form of "WordPress Multisite," which allows users to run multiple websites from a single installation of WordPress.
+- **WordPress:** WordPress has a similar concept in the form of "WordPress Multisite," which allows users to run multiple websites from a single installation of WordPress.
 
-* Joomla: Joomla has a similar concept in the form of "Joomla Templates," which are pre-designed templates for Joomla websites.
+- **Joomla:** Joomla has a similar concept in the form of "Joomla Templates," which are pre-designed templates for Joomla websites.
 
-* TYPO3: TYPO3 has a similar concept in the form of "TYPO3 Distributions," which are pre-configured installations of TYPO3 for specific types of websites.
+- **TYPO3:** TYPO3 has a similar concept in the form of "TYPO3 Distributions," which are pre-configured installations of TYPO3 for specific types of websites.
 
-## Creating a new Distribution
+## Creating a new distribution
 
-First of all, a Plone Distribution is a Python Package that can be installed by `pip`.
+A Plone distribution is a Python Package that can be installed by `pip`.
 
 ### `setup.py`
+
 The package will follow some conventions, to make it "discoverable" by others.
 
-In `setup.py`, always add the correct Trove Classifiers:
+In `setup.py`, always add the correct Trove classifiers:
 
 ```python
         "Framework :: Plone",
         "Framework :: Plone :: 6.0",
         "Framework :: Plone :: Distribution",
 ```
 
@@ -84,40 +111,38 @@
         "setuptools",
         "plone.distribution",
     ],
 ```
 
 ### `configure.zcml`
 
-In your main `configure.zcml`, make sure to have the `plone` xml namespace declared:
+In your main `configure.zcml`, make sure to have the `plone` XML namespace declared:
 
 ```xml
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:plone="http://namespaces.plone.org/plone"
     >
 ```
 
 And also include `plone.distribution`:
 
 ```xml
-  <include package="plone.distribution" />
+<include package="plone.distribution" />
 ```
 
 Then declare the distributions included in your package:
 
 ```xml
-
   <plone:distribution
       name="blog"
       title="Personal Blog"
       description="A Plone site already configured to host a personal Blog."
       directory="distributions/blog"
       />
-
 ```
 
 The registered distribution will configure a Personal Blog, with some default content.
 
 #### distribution handlers
 
 When registering a distribution, you can provide a `pre_handler`, a `handler` and a `post_handler` which must be
@@ -133,30 +158,28 @@
 def post_handler(distribution: Distribution, site, answers: dict):
     return site
 ```
 
 Each of those handlers will be called in this way:
 
 - `pre_handler`: it will process the answers to do modifications on them before creating the site
-- `handler`: it will be run after the bare Plone site will be created but instead of the default handler that installs the required GenericSetup profiles and creates the content.
-- `post_handler`: it will be run after the site is setup.
+- `handler`: it will be run after the bare Plone site will be created, but instead of the default handler that installs the required GenericSetup profiles and creates the content.
+- `post_handler`: it will be run after the site is set up.
 
-So if you have added some extra fields in the Plone site creation form and want to do some extra configuration in the
+If you have added some extra fields in the Plone site creation form and want to do some extra configuration in the
 Plone site, you can add your own handler and register as follows:
 
 ```xml
-
   <plone:distribution
       name="blog"
       title="Personal Blog"
       description="A Plone site already configured to host a personal Blog."
       directory="distributions/blog"
       post_handler=".handlers.blog.post_handler"
       />
-
 ```
 
 ### distribution folder
 
 A convention is to use the `distributions/<distribution_name>`folder in the root of your package to organize your distribution configuration.
 
 In that folder, you will need to provide:
@@ -167,17 +190,17 @@
 
 ### `profiles.json`
 
 A `JSON` file with the GenericSetup profiles that are used by your distribution during installation.
 
 This file needs to contain two keys:
 
-* **base**: List of profiles installed in every new site using this distribution.
+- **base**: List of profiles installed in every new site using this distribution.
 
-* **content**: List of profiles installed when the user decides to create a site with example content.
+- **content**: List of profiles installed when the user decides to create a site with example content.
 
 The configuration for a new Volto site is:
 
 ```json
 {
   "base": [
     "plone.app.contenttypes:default",
@@ -234,25 +257,25 @@
 
 ### `schema.json`
 
 In case you require additional input from the user during site creation, you can customize the form using the `schema.json` file.
 
 The file should contain two keys:
 
-* **schema**: A JSON Schema definition.
-* **uischema**: A [react-jsonschema-form](https://rjsf-team.github.io/react-jsonschema-form/docs/) configuration to modify how the form is displayed.
+- **schema**: A JSON Schema definition.
+- **uischema**: A [react-jsonschema-form](https://rjsf-team.github.io/react-jsonschema-form/docs/) configuration to modify how the form is displayed.
 
 The **schema** should have at least the following keys:
 
-* site_id
-* title
-* description
-* default_language
-* portal_timezone
-* setup_content
+- site_id
+- title
+- description
+- default_language
+- portal_timezone
+- setup_content
 
 The `schema.json` used for the default site creation is:
 
 ```json
 {
   "schema": {
     "title": "Create a Plone site",
@@ -309,55 +332,100 @@
 {"$ref": "#/definitions/timezones"}
 ```
 
 Both definitions are added in runtime by `plone.distribution` to provide a list of languages and timezones available on the installation.
 
 ### `content` folder
 
-Folder containing JSON data exported using the `@@dist_export_all` browser view of this package.
+Folder containing JSON data representing this distribution's content.
+
+To export content from a site into this folder, use the `bin/export-distribution` script.
+
+```shell
+bin/export-distribution path/to/zope.conf Plone
+```
+
+> In the example above, "Plone" is the ID of the Plone site to export.
 
 ## Advanced Usage
 
 ### Hiding Distributions
 
 By default, `plone.distribution` ships with two ready-to-use distributions:
 
-* **default**: Plone Site (Volto frontend)
-* **classic**: Plone Site (Classic UI)
+- **default**: Plone Site (Volto frontend)
+- **classic**: Plone Site (Classic UI)
 
 If you want to limit your users option to select a distribution, it is possible to set the environment variable `ALLOWED_DISTRIBUTIONS` with fewer options:
 
 ```shell
 ALLOWED_DISTRIBUTIONS=default
 ```
 
-
 ## This project is supported by
 
 <p align="left">
     <a href="https://plone.org/foundation/">
       <img alt="Plone Logo" width="200px" src="https://raw.githubusercontent.com/plone/.github/main/plone-foundation.png">
     </a>
 </p>
 
 ## License
+
 The project is licensed under the GPLv2.
 
 
 # Changelog
 
 <!--
    You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 2.0.0a1 (2024-05-16)
+
+
+### Breaking changes:
+
+- plone.distribution is now based on plone.exportimport instead of collective.exportimport.
+
+  There are some backwards-incompatible changes in the export format.
+  To convert an existing distribution to the new format, use the following steps:
+  1. Create a site from the distribution using plone.distribution 1.0.x
+  2. Install plone.distribution 2.0.x
+  3. Delete the distribution's `contents/items` folder.
+  4. Export the distribution in the new format using the `bin/export-distribution` script.
+
+  @davisagli, @ericof #61
+
+
+### New features:
+
+- Default distribution: Allow users to upload a logo during site creation [@ericof] #66
+- Classic distribution: Allow users to upload a logo during site creation [@ericof] #67
+- Remove dependency on Plone package, add dependency on Products.CMFPlone [@ericof] #70
+
+
+### Bug fixes:
+
+- Get the name of the existing distribution from the report, not the answers [@ericof] #60
+- Fix issue with payload for new site creation breaking with certain plone.rest versions [@ericof] #71
+- Read profile.json by the pathlib.Path.read_text method to avoid the unclosed file exception [@folix-01] #75
+
+
+### Internal:
+
+- Update `plone/meta` configuration [@ericof] #73
+- Log traceback when creating a site fails [@pbauer] #82
+- Bump `plone.exportimport` to 1.0.0a5 [@ericof] #83
+
 ## 1.0.0b4 (2024-04-03)
 
 
 ### Bug fixes:
 
 - Fix exporting files.
   [pbauer] #58
```

### Comparing `plone.distribution-1.0.0b4/README.md` & `plone_distribution-2.0.0a1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,45 +2,47 @@
     <img alt="Plone Logo" width="200px" src="https://raw.githubusercontent.com/plone/.github/main/plone-logo.png">
 </p>
 
 <h1 align="center">
   Plone Distributions
 </h1>
 
-Package supporting the (easy) implementation of a Plone Distribution.
+Package supporting the (easy) implementation of a Plone distribution.
 
-## What is a Plone Distribution
+## What is a Plone distribution
 
-A Plone distribution is a pre-packaged version of Plone that includes specific features, themes, modules, and configurations. It is a convenient way to get a specific type of website up and running quickly, as the distribution includes everything needed to run that type of site.
+A Plone distribution is a pre-packaged version of Plone that includes specific features, themes, modules, and configurations.
+It is a convenient way to get a specific type of website up and running quickly, as the distribution includes everything needed to run that type of site.
 
 Examples of Plone distributions include:
 
-* [SENAITE](https://www.senaite.com)
-* [Quaive](https://quaivecloud.com/)
-* [Portal Modelo](https://www.interlegis.leg.br/produtos-servicos/portal-modelo/)
-* [Portal Padrão](https://identidade-digital-de-governo-plone.readthedocs.io/en/latest/)
+- [SENAITE](https://www.senaite.com)
+- [Quaive](https://quaivecloud.com/)
+- [Portal Modelo](https://www.interlegis.leg.br/produtos-servicos/portal-modelo/)
+- [Portal Padrão](https://identidade-digital-de-governo-plone.readthedocs.io/en/latest/)
 
 ### Similar Concept in Other CMS
 
-* Drupal: Drupal has distributions for blogs, e-commerce sites, and intranet portals.
+- **Drupal:** Drupal has distributions for blogs, e-commerce sites, and intranet portals.
 
-* WordPress: WordPress has a similar concept in the form of "WordPress Multisite," which allows users to run multiple websites from a single installation of WordPress.
+- **WordPress:** WordPress has a similar concept in the form of "WordPress Multisite," which allows users to run multiple websites from a single installation of WordPress.
 
-* Joomla: Joomla has a similar concept in the form of "Joomla Templates," which are pre-designed templates for Joomla websites.
+- **Joomla:** Joomla has a similar concept in the form of "Joomla Templates," which are pre-designed templates for Joomla websites.
 
-* TYPO3: TYPO3 has a similar concept in the form of "TYPO3 Distributions," which are pre-configured installations of TYPO3 for specific types of websites.
+- **TYPO3:** TYPO3 has a similar concept in the form of "TYPO3 Distributions," which are pre-configured installations of TYPO3 for specific types of websites.
 
-## Creating a new Distribution
+## Creating a new distribution
 
-First of all, a Plone Distribution is a Python Package that can be installed by `pip`.
+A Plone distribution is a Python Package that can be installed by `pip`.
 
 ### `setup.py`
+
 The package will follow some conventions, to make it "discoverable" by others.
 
-In `setup.py`, always add the correct Trove Classifiers:
+In `setup.py`, always add the correct Trove classifiers:
 
 ```python
         "Framework :: Plone",
         "Framework :: Plone :: 6.0",
         "Framework :: Plone :: Distribution",
 ```
 
@@ -52,40 +54,38 @@
         "setuptools",
         "plone.distribution",
     ],
 ```
 
 ### `configure.zcml`
 
-In your main `configure.zcml`, make sure to have the `plone` xml namespace declared:
+In your main `configure.zcml`, make sure to have the `plone` XML namespace declared:
 
 ```xml
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:plone="http://namespaces.plone.org/plone"
     >
 ```
 
 And also include `plone.distribution`:
 
 ```xml
-  <include package="plone.distribution" />
+<include package="plone.distribution" />
 ```
 
 Then declare the distributions included in your package:
 
 ```xml
-
   <plone:distribution
       name="blog"
       title="Personal Blog"
       description="A Plone site already configured to host a personal Blog."
       directory="distributions/blog"
       />
-
 ```
 
 The registered distribution will configure a Personal Blog, with some default content.
 
 #### distribution handlers
 
 When registering a distribution, you can provide a `pre_handler`, a `handler` and a `post_handler` which must be
@@ -101,30 +101,28 @@
 def post_handler(distribution: Distribution, site, answers: dict):
     return site
 ```
 
 Each of those handlers will be called in this way:
 
 - `pre_handler`: it will process the answers to do modifications on them before creating the site
-- `handler`: it will be run after the bare Plone site will be created but instead of the default handler that installs the required GenericSetup profiles and creates the content.
-- `post_handler`: it will be run after the site is setup.
+- `handler`: it will be run after the bare Plone site will be created, but instead of the default handler that installs the required GenericSetup profiles and creates the content.
+- `post_handler`: it will be run after the site is set up.
 
-So if you have added some extra fields in the Plone site creation form and want to do some extra configuration in the
+If you have added some extra fields in the Plone site creation form and want to do some extra configuration in the
 Plone site, you can add your own handler and register as follows:
 
 ```xml
-
   <plone:distribution
       name="blog"
       title="Personal Blog"
       description="A Plone site already configured to host a personal Blog."
       directory="distributions/blog"
       post_handler=".handlers.blog.post_handler"
       />
-
 ```
 
 ### distribution folder
 
 A convention is to use the `distributions/<distribution_name>`folder in the root of your package to organize your distribution configuration.
 
 In that folder, you will need to provide:
@@ -135,17 +133,17 @@
 
 ### `profiles.json`
 
 A `JSON` file with the GenericSetup profiles that are used by your distribution during installation.
 
 This file needs to contain two keys:
 
-* **base**: List of profiles installed in every new site using this distribution.
+- **base**: List of profiles installed in every new site using this distribution.
 
-* **content**: List of profiles installed when the user decides to create a site with example content.
+- **content**: List of profiles installed when the user decides to create a site with example content.
 
 The configuration for a new Volto site is:
 
 ```json
 {
   "base": [
     "plone.app.contenttypes:default",
@@ -202,25 +200,25 @@
 
 ### `schema.json`
 
 In case you require additional input from the user during site creation, you can customize the form using the `schema.json` file.
 
 The file should contain two keys:
 
-* **schema**: A JSON Schema definition.
-* **uischema**: A [react-jsonschema-form](https://rjsf-team.github.io/react-jsonschema-form/docs/) configuration to modify how the form is displayed.
+- **schema**: A JSON Schema definition.
+- **uischema**: A [react-jsonschema-form](https://rjsf-team.github.io/react-jsonschema-form/docs/) configuration to modify how the form is displayed.
 
 The **schema** should have at least the following keys:
 
-* site_id
-* title
-* description
-* default_language
-* portal_timezone
-* setup_content
+- site_id
+- title
+- description
+- default_language
+- portal_timezone
+- setup_content
 
 The `schema.json` used for the default site creation is:
 
 ```json
 {
   "schema": {
     "title": "Create a Plone site",
@@ -277,35 +275,43 @@
 {"$ref": "#/definitions/timezones"}
 ```
 
 Both definitions are added in runtime by `plone.distribution` to provide a list of languages and timezones available on the installation.
 
 ### `content` folder
 
-Folder containing JSON data exported using the `@@dist_export_all` browser view of this package.
+Folder containing JSON data representing this distribution's content.
+
+To export content from a site into this folder, use the `bin/export-distribution` script.
+
+```shell
+bin/export-distribution path/to/zope.conf Plone
+```
+
+> In the example above, "Plone" is the ID of the Plone site to export.
 
 ## Advanced Usage
 
 ### Hiding Distributions
 
 By default, `plone.distribution` ships with two ready-to-use distributions:
 
-* **default**: Plone Site (Volto frontend)
-* **classic**: Plone Site (Classic UI)
+- **default**: Plone Site (Volto frontend)
+- **classic**: Plone Site (Classic UI)
 
 If you want to limit your users option to select a distribution, it is possible to set the environment variable `ALLOWED_DISTRIBUTIONS` with fewer options:
 
 ```shell
 ALLOWED_DISTRIBUTIONS=default
 ```
 
-
 ## This project is supported by
 
 <p align="left">
     <a href="https://plone.org/foundation/">
       <img alt="Plone Logo" width="200px" src="https://raw.githubusercontent.com/plone/.github/main/plone-foundation.png">
     </a>
 </p>
 
 ## License
+
 The project is licensed under the GPLv2.
```

### Comparing `plone.distribution-1.0.0b4/docs/Makefile` & `plone_distribution-2.0.0a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/docs/_static/favicon.ico` & `plone_distribution-2.0.0a1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/docs/_static/logo.svg` & `plone_distribution-2.0.0a1/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/docs/_static/styles.css` & `plone_distribution-2.0.0a1/docs/_static/styles.css`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/docs/api/index.md` & `plone_distribution-2.0.0a1/docs/api/index.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/docs/conf.py` & `plone_distribution-2.0.0a1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/docs/index.md` & `plone_distribution-2.0.0a1/docs/index.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/docs/usage/code-examples.md` & `plone_distribution-2.0.0a1/docs/usage/code-examples.md`

 * *Files 8% similar despite different names*

```diff
@@ -48,14 +48,28 @@
 
 distribution = dist_api.get(name="default")
 
 assert isinstance(distribution, Distribution)
 assert distribution.title == "Plone Site"
 ```
 
+(api-distribution-get_creation_report-example)=
+
+### Get creation report for a site
+
+To get a report of the creation of the site use the method {meth}`api.distribution.get_creation_report`.
+
+```python
+from plone.distribution.api import distribution as dist_api
+
+site = app.Plone
+report = dist_api.get_creation_report(site)
+```
+
+
 ## `api.site`
 
 This section describes how to interface with the `site` module.
 
 (api-site-get_sites-example)=
 
 ### Get the list of all sites
@@ -65,28 +79,14 @@
 ```python
 from plone.distribution.api import site as site_api
 
 
 sites = site_api.get_sites(app)
 ```
 
-
-(api-site-get_creation_report-example)=
-
-### Get creation report for a site
-
-To get a report of the creation of the site use the method {meth}`api.site.get_creation_report`.
-
-```python
-from plone.distribution.api import site as site_api
-
-site = app.Plone
-report = site_api.get_creation_report(site)
-```
-
 (api-site-create-example)=
 
 ### Create a new site
 
 Create a new Plone site using one of the available distributions using the method {meth}`api.site.create`.
 
 ```python
```

### Comparing `plone.distribution-1.0.0b4/docs/usage/index.md` & `plone_distribution-2.0.0a1/docs/usage/index.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/docs/usage/package-structure.md` & `plone_distribution-2.0.0a1/docs/usage/package-structure.md`

 * *Files 20% similar despite different names*

```diff
@@ -171,53 +171,34 @@
 Both definitions are added in runtime by `plone.distribution` to provide a list of languages and timezones available on the installation.
 ````
 
 ### `content`
 
 Folder containing content and settings to be imported if the user selects `setup_content` during site creation.
 
-#### `content/items`
+#### `content/content`
 
-Sub-folder with JSON files representing the content to be imported during site creation. Each JSON file represent one content item, including the site root.
-
-References to image and file blobs in each file would point to `content/blobs`.
-
-#### `content/blobs`
-
-Sub-folder with blob files used during content creation.
+Contains data representing each content item to be imported during site creation. For each content item, there is a subfolder named with the item's UID, containing data.json as well as any blobs used by the item.
 
 #### `content/discussion.json`
 
 Contains comments on content items.
 
-#### `content/ordering.json`
-
-Contains ordering information, in folderish items, of content items.
-
 #### `content/redirects.json`
 
 Contains information about redirects to be created.
 
-
 #### `content/relations.json`
 
 Information about relations between contents.
 
 #### `content/translations.json`
 
 Information about translations of contents.
 
-#### `content/members.json`
-
-Contains information about users to be created during content creation.
-
-#### `content/localroles.json`
-
-Contains information about local roles to be set during content creation.
-
-#### `content/defaultpages.json`
+#### `content/principals.json`
 
-Contains information about default pages on folderish content. **Only available for non-headless distributions**
+Contains information about users and groups to be created during content creation.
 
 #### `content/portlets.json`
 
 Contains information about portlets. **Only available for non-headless distributions**
```

### Comparing `plone.distribution-1.0.0b4/docs/usage/zcml.md` & `plone_distribution-2.0.0a1/docs/usage/zcml.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/pyproject.toml` & `plone_distribution-2.0.0a1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -117,44 +117,50 @@
   'zope.sendmail', 'Zope'
 ]
 'plone.base' = [
   'plone.batching', 'plone.registry', 'plone.schema','plone.z3cform',
   'Products.CMFCore', 'Products.CMFDynamicViewFTI',
 ]
 python-dateutil = ['dateutil']
-ignore-packages = ['plone.volto', 'zestreleaser.towncrier', 'zest.releaser', 'pytest', 'pytest-cov', 'pytest-plone', 'plone.testing', 'plone.app.testing']
-Plone = ['Products.CMFPlone', 'Products.CMFCore', 'Products.GenericSetup']
+ignore-packages = ['plone.app.iterate', 'plone.app.upgrade', 'plone.volto', 'zestreleaser.towncrier', 'zest.releaser', 'pytest', 'pytest-cov', 'pytest-plone', 'plone.testing', 'plone.app.testing']
 
 ##
 # Add extra configuration options in .meta.toml:
 #  [pyproject]
 #  dependencies_ignores = "['zestreleaser.towncrier']"
 #  dependencies_mappings = [
 #    "gitpython = ['git']",
 #    "pygithub = ['github']",
 #  ]
 ##
 
 [tool.check-manifest]
 ignore = [
     ".editorconfig",
+    ".flake8",
     ".meta.toml",
     ".pre-commit-config.yaml",
-    "tox.ini",
-    ".flake8",
+    "dependabot.yml",
     "mx.ini",
+    "tox.ini",
 
 ]
+
 ##
 # Add extra configuration options in .meta.toml:
 #  [pyproject]
 #  check_manifest_ignores = """
 #      "*.map.js",
 #      "*.pyc",
 #  """
+#  check_manifest_extra_lines = """
+#  ignore-bad-ideas = [
+#      "some/test/file/PKG-INFO",
+#  ]
+#  """
 ##
 
 
 ##
 # Add extra configuration options in .meta.toml:
 #  [pyproject]
 #  extra_lines = """
```

### Comparing `plone.distribution-1.0.0b4/setup.py` & `plone_distribution-2.0.0a1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = f"""
 {Path("README.md").read_text()}\n
 {Path("CHANGES.md").read_text()}\n
 """
 
 setup(
     name="plone.distribution",
-    version="1.0.0b4",
+    version="2.0.0a1",
     description="Plone distribution support",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Web Environment",
         "Framework :: Plone",
@@ -43,40 +43,44 @@
     },
     packages=find_packages("src"),
     namespace_packages=["plone"],
     package_dir={"": "src"},
     include_package_data=True,
     zip_safe=False,
     install_requires=[
-        "Plone",
+        "Products.CMFPlone",
+        "Products.GenericSetup",
         "Zope",
         "setuptools",
-        "collective.exportimport>=1.12",
         "jsonschema",
         "plone.api",
-        "plone.app.contentrules",
         "plone.base",
         "plone.dexterity",
+        "plone.exportimport>=1.0.0a5",
         "plone.i18n",
-        "plone.namedfile",
         "plone.protect",
         "plone.rest",
         "plone.restapi",
         "z3c.unconfigure",
     ],
     extras_require={
         "test": [
-            "zest.releaser[recommended]",
-            "zestreleaser.towncrier",
-            "plone.volto",
+            "plone.app.iterate",
             "plone.app.testing",
+            "plone.app.upgrade",
             "plone.restapi[test]",
+            "plone.volto[test]",
             "plone.testing",
-            "pytest",
             "pytest-cov",
-            "pytest-plone>=0.2.0",
+            "pytest-plone>=0.5.0",
+            "pytest",
+            "zest.releaser[recommended]",
+            "zestreleaser.towncrier",
         ]
     },
     entry_points={
         "z3c.autoinclude.plugin": ["target = plone"],
+        "console_scripts": [
+            "export-distribution = plone.distribution.cli:export",
+        ],
     },
 )
```

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/api/site.py` & `plone_distribution-2.0.0a1/src/plone/distribution/api/site.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,32 +10,28 @@
 from plone.distribution.handler import default_pre_handler
 from plone.distribution.utils.validation import validate_answers
 from plone.registry.interfaces import IRegistry
 from Products.CMFPlone.events import SiteManagerCreatedEvent
 from Products.CMFPlone.Portal import PloneSite
 from Products.GenericSetup.tool import SetupTool
 from typing import List
-from typing import Union
 from ZODB.broken import Broken
 from zope.annotation.interfaces import IAnnotations
 from zope.component import queryUtility
 from zope.component.hooks import setSite
 from zope.event import notify
 from zope.lifecycleevent import ObjectCreatedEvent
 
 import transaction
 
 
 _TOOL_ID = "portal_setup"
 _DEFAULT_PROFILE = "Products.CMFPlone:plone"
 
 
-SITE_REPORT_ANNO = "__plone_distribution_report__"
-
-
 def _handlers_for_distribution(distribution: Distribution):
     """Return pre_handler, handler and post_handler for a distribution."""
     pre_handler = (
         distribution.pre_handler if distribution.pre_handler else default_pre_handler
     )
     handler = distribution.handler if distribution.handler else default_handler
     return pre_handler, handler, distribution.post_handler
@@ -84,15 +80,15 @@
 def _add_report_to_site(site: PloneSite, distribution_name: str, answers: dict) -> None:
     """Add a report to the newly created site."""
     # Create a report of a site creation
     annotations = IAnnotations(site)
     report = SiteCreationReport(
         distribution_name, datetime.now(tz=timezone.utc), answers
     )
-    annotations[SITE_REPORT_ANNO] = report
+    annotations[dist_api.SITE_REPORT_ANNO] = report
 
 
 def _create_site(
     context,
     distribution_name: str,
     answers: dict,
     profile_id: str = _DEFAULT_PROFILE,
@@ -136,27 +132,14 @@
             if secman.checkPermission(View, obj):
                 result.append(obj)
         elif obj.getId() in getattr(context, "_mount_points", {}):
             result.extend(get_sites(context=obj))
     return result
 
 
-def get_creation_report(site: PloneSite) -> Union[SiteCreationReport, None]:
-    """Return a site creation report for a Plone site.
-
-    :param site: Plone Site.
-    :returns: SiteCreationReport with distribution name, creation date and
-              answers used to create the site.
-
-    :Example: :ref:`api-site-get_creation_report-example`
-    """
-    annotations = IAnnotations(site)
-    return annotations.get(SITE_REPORT_ANNO, None)
-
-
 def create(
     context,
     distribution_name: str,
     answers: dict,
     profile_id: str = _DEFAULT_PROFILE,
 ) -> PloneSite:
     """Create a new Plone site using one of the distributions.
```

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/browser/admin.py` & `plone_distribution-2.0.0a1/src/plone/distribution/browser/admin.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/browser/configure.zcml` & `plone_distribution-2.0.0a1/src/plone/distribution/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/browser/image.py` & `plone_distribution-2.0.0a1/src/plone/distribution/browser/image.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/browser/overrides.zcml` & `plone_distribution-2.0.0a1/src/plone/distribution/browser/overrides.zcml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/browser/static/plone-logo.png` & `plone_distribution-2.0.0a1/src/plone/distribution/browser/static/plone-logo.png`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/browser/static/plone-overview.min.css` & `plone_distribution-2.0.0a1/src/plone/distribution/browser/static/plone-overview.min.css`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/browser/static/plone-overview.min.js` & `plone_distribution-2.0.0a1/src/plone/distribution/browser/static/plone-overview.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -31139,18 +31139,18 @@
             }) {
                 i(h)
             }
             const u = () => {
                 o(""), s.reset()
             };
             async function c(h) {
-                const f = JSON.stringify({
+                const f = {
                     ...h.formData,
                     distribution: r
-                });
+                };
                 s.mutate(f)
             }
             if (s.isSuccess) {
                 const h = s.data["@id"];
                 window.location.replace(h)
             }
             if (s.isError && !a) {
```

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/browser/static/plone.svg` & `plone_distribution-2.0.0a1/src/plone/distribution/browser/static/plone.svg`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/browser/templates/plone-overview.pt` & `plone_distribution-2.0.0a1/src/plone/distribution/browser/templates/plone-overview.pt`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/core.py` & `plone_distribution-2.0.0a1/src/plone/distribution/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         schema = schema_utils.process_raw_schema(raw_schema)
         if not schema_utils.validate_jsonschema(schema["schema"]):
             raise ValueError(f"Invalid schema for {schema_file}")
         self._schema = schema
         profiles = {"base": [], "content": []}
         data_file = self.directory / "profiles.json"
         if data_file.exists():
-            profiles = json.load(open(data_file))
+            profiles = json.loads(data_file.read_text())
         self._profiles = profiles
 
     def __repr__(self) -> str:
         return f"<Distribution name='{self.name}' title='{self.title}'>"
 
     @property
     def image(self) -> Path:
```

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/items/1.json` & `plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/content/plone_site_root/data.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7191358024691359%*

 * *Differences: {"'@id'": "'/classic'",*

 * * "'UID'": "'plone_site_root'",*

 * * "'description'": "'A Plone Site with Classic UI'",*

 * * "'exportimport.constrains'": 'OrderedDict()',*

 * * "'exportimport.conversation'": '[]',*

 * * "'exportimport.versions'": 'OrderedDict()',*

 * * "'id'": "'classic'",*

 * * "'items_total'": '2',*

 * * "'language'": "'##DEFAULT##'",*

 * * "'text'": '{\'data\': \'<div class="hero"> <h1>Welcome!</h1> <p><a class="btn btn-primary" '*

 * *           'href="https://plone.org" target="_blank">Learn more about Plone</a></p> </div> <p '*

 * *         […]*

```diff
@@ -1,34 +1,38 @@
 {
-    "@id": "/Plone",
+    "@id": "/classic",
     "@type": "Plone Site",
-    "UID": "6de6fe58afb6479f870839b9bc71e9cc",
+    "UID": "plone_site_root",
     "allow_discussion": null,
     "contributors": [],
     "creators": [
         "admin"
     ],
-    "description": "Congratulations! You have successfully installed Plone.",
+    "description": "A Plone Site with Classic UI",
     "effective": null,
     "exclude_from_nav": false,
     "expires": null,
-    "id": "Plone",
+    "exportimport.constrains": {},
+    "exportimport.conversation": [],
+    "exportimport.versions": {},
+    "id": "classic",
     "is_folderish": true,
-    "items_total": 3,
-    "language": "en",
+    "items_total": 2,
+    "language": "##DEFAULT##",
     "lock": {
         "locked": false,
         "stealable": true
     },
     "parent": {},
     "review_state": null,
     "rights": "",
     "subjects": [],
     "table_of_contents": null,
     "text": {
         "content-type": "text/html",
-        "data": "<div class=\"hero\"> <h1>Welcome!</h1> <p><a class=\"btn btn-primary\" href=\"https://plone.org\" target=\"_blank\">Learn more about Plone</a></p> </div> <p class=\"discreet\"> If you're seeing this text instead of the web site you were expecting, the owner of this web site has just installed Plone. Do not contact the Plone Team or the Plone support channels about this. </p> <h2>Get started</h2> <p> Before you start exploring your newly created Plone site, please do the following: </p> <ol> <li>Make sure you are logged in as an admin/manager user. <span class=\"discreet\">You should have a Site Setup entry in the user menu.</span></li> <li><a href=\"@@mail-controlpanel\" target=\"_blank\">Set up your mail server</a>. <span class=\"discreet\">Plone needs a valid SMTP server to verify users and send out password reminders.</span></li> <li><a href=\"@@security-controlpanel\" target=\"_blank\">Decide what security level you want on your site</a>. <span class=\"discreet\">Allow self registration, password policies, and more.</span></li> </ol> <h2>Get comfortable</h2> <p>After that, we suggest you do one or more of the following:</p> <ul> <li>Get the latest <a class=\"link-plain\" href=\"https://plone.org/news\" target=\"_blank\">news</a> about Plone.</li> <li>Read the <a class=\"link-plain\" href=\"https://6.docs.plone.org\" target=\"_blank\">documentation</a>.</li> <li>Follow a <a class=\"link-plain\" href=\"https://training.plone.org\" target=\"_blank\">training</a>.</li> <li>Explore the <a class=\"link-plain\" href=\"https://plone.org/download/add-ons\" target=\"_blank\">available add-ons</a> for Plone.</li> <li>Read or subscribe to the <a class=\"link-plain\" href=\"https://plone.org/support\" target=\"_blank\">support channels</a>.</li> </ul> <h2>Make it your own</h2> <p>Plone has many settings to make it do what you want. Some examples include:</p> <ul> <li> Try out a different theme, either pick from <a href=\"@@theming-controlpanel\" target=\"_blank\">the included ones</a>, or one of the <a class=\"link-plain\" href=\"https://plone.org/download/add-ons\" target=\"_blank\">available themes from plone.org</a>. <span class=\"discreet\">Make sure the theme is compatible with the version of Plone you are currently using.</span> </li> <li> <a href=\"@@content-controlpanel\" target=\"_blank\"> Decide what kind of workflow you want in your site.</a> <span class=\"discreet\">The default is typical for a public web site; if you want to use Plone as a closed intranet or extranet, you can choose a different workflow.</span> </li> <li> By default, Plone uses a visual editor for content. <span class=\"discreet\">If you prefer text-based syntax and/or wiki syntax, you can change this in the <a href=\"@@markup-controlpanel\" target=\"_blank\">markup control panel</a></span> </li> <li>\u2026and many more settings are available in the <a href=\"@@overview-controlpanel\" target=\"_blank\">Site Setup</a>. </li> </ul> <h2>Tell us how you use it</h2> <p> Are you doing something interesting with Plone? Big site deployments, interesting use cases? Do you have a company that delivers Plone-based solutions? </p> <ul> <li>Add your company as a <a class=\"link-plain\" href=\"https://plone.org/providers/\" target=\"_blank\">Plone provider</a>.</li> <li>Add a <a class=\"link-plain\" href=\"https://plone.org/news/plone-news-by-category/success-story\" target=\"_blank\">success story</a> describing your deployed project and customer.</li> </ul> <h2>Find out more about Plone</h2> <p> Plone is a powerful content management system built on a rock-solid application stack. Read about its technology on the <a class=\"link-plain\" href=\"https://plone.org/what-is-plone\" target=\"_blank\">Plone web site</a>. </p> <h2>Support the Plone Foundation</h2> <p> Plone is made possible only through the efforts of thousands of dedicated individuals and hundreds of companies. The Plone Foundation: </p> <ul> <li>\u2026protects and promotes Plone.</li> <li>\u2026is a recognized 501(c)(3) charitable organization with the United States Internal Revenue Service.</li> <li>\u2026receives donations that may be tax-deductible.</li> <li><a href=\"https://plone.org/sponsors/be-a-hero\" target=\"_blank\">Support the Foundation and help make Plone better!</a></li> </ul> <p>Thanks for using our product. We hope you like it!</p> <p>\u2014The Plone Team</p>",
+        "data": "<div class=\"hero\"> <h1>Welcome!</h1> <p><a class=\"btn btn-primary\" href=\"https://plone.org\" target=\"_blank\">Learn more about Plone</a></p> </div> <p class=\"discreet\"> If you're seeing this text instead of the web site you were expecting, the owner of this web site has just installed Plone. Do not contact the Plone Team or the Plone support channels about this. </p> <h2>Get started</h2> <p> Before you start exploring your newly created Plone site, please do the following: </p> <ol> <li>Make sure you are logged in as an admin/manager user. <span class=\"discreet\">You should have a Site Setup entry in the user menu.</span></li> <li><a href=\"http://nohost/classic/@@mail-controlpanel\" target=\"_blank\">Set up your mail server</a>. <span class=\"discreet\">Plone needs a valid SMTP server to verify users and send out password reminders.</span></li> <li><a href=\"http://nohost/classic/@@security-controlpanel\" target=\"_blank\">Decide what security level you want on your site</a>. <span class=\"discreet\">Allow self registration, password policies, and more.</span></li> </ol> <h2>Get comfortable</h2> <p>After that, we suggest you do one or more of the following:</p> <ul> <li>Get the latest <a class=\"link-plain\" href=\"https://plone.org/news\" target=\"_blank\">news</a> about Plone.</li> <li>Read the <a class=\"link-plain\" href=\"https://6.docs.plone.org\" target=\"_blank\">documentation</a>.</li> <li>Follow a <a class=\"link-plain\" href=\"https://training.plone.org\" target=\"_blank\">training</a>.</li> <li>Explore the <a class=\"link-plain\" href=\"https://plone.org/download/add-ons\" target=\"_blank\">available add-ons</a> for Plone.</li> <li>Read or subscribe to the <a class=\"link-plain\" href=\"https://plone.org/support\" target=\"_blank\">support channels</a>.</li> </ul> <h2>Make it your own</h2> <p>Plone has many settings to make it do what you want. Some examples include:</p> <ul> <li> Try out a different theme, either pick from <a href=\"http://nohost/classic/@@theming-controlpanel\" target=\"_blank\">the included ones</a>, or one of the <a class=\"link-plain\" href=\"https://plone.org/download/add-ons\" target=\"_blank\">available themes from plone.org</a>. <span class=\"discreet\">Make sure the theme is compatible with the version of Plone you are currently using.</span> </li> <li> <a href=\"http://nohost/classic/@@content-controlpanel\" target=\"_blank\"> Decide what kind of workflow you want in your site.</a> <span class=\"discreet\">The default is typical for a public web site; if you want to use Plone as a closed intranet or extranet, you can choose a different workflow.</span> </li> <li> By default, Plone uses a visual editor for content. <span class=\"discreet\">If you prefer text-based syntax and/or wiki syntax, you can change this in the <a href=\"http://nohost/classic/@@markup-controlpanel\" target=\"_blank\">markup control panel</a></span> </li> <li>\u2026and many more settings are available in the <a href=\"http://nohost/classic/@@overview-controlpanel\" target=\"_blank\">Site Setup</a>. </li> </ul> <h2>Tell us how you use it</h2> <p> Are you doing something interesting with Plone? Big site deployments, interesting use cases? Do you have a company that delivers Plone-based solutions? </p> <ul> <li>Add your company as a <a class=\"link-plain\" href=\"https://plone.org/providers/\" target=\"_blank\">Plone provider</a>.</li> <li>Add a <a class=\"link-plain\" href=\"https://plone.org/news/plone-news-by-category/success-story\" target=\"_blank\">success story</a> describing your deployed project and customer.</li> </ul> <h2>Find out more about Plone</h2> <p> Plone is a powerful content management system built on a rock-solid application stack. Read about its technology on the <a class=\"link-plain\" href=\"https://plone.org/what-is-plone\" target=\"_blank\">Plone web site</a>. </p> <h2>Support the Plone Foundation</h2> <p> Plone is made possible only through the efforts of thousands of dedicated individuals and hundreds of companies. The Plone Foundation: </p> <ul> <li>\u2026protects and promotes Plone.</li> <li>\u2026is a recognized 501(c)(3) charitable organization with the United States Internal Revenue Service.</li> <li>\u2026receives donations that may be tax-deductible.</li> <li><a href=\"https://plone.org/sponsors/be-a-hero\" target=\"_blank\">Support the Foundation and help make Plone better!</a></li> </ul> <p>Thanks for using our product. We hope you like it!</p> <p>\u2014The Plone Team</p>",
         "encoding": "utf-8"
     },
-    "title": "Welcome to Plone",
-    "type_title": "Plone Site"
+    "title": "Plone Site",
+    "type_title": "Plone Site",
+    "workflow_history": {}
 }
```

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/items/2.json` & `plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/content/54163be595184b4eb0a0b82a58b8def8/data.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8830645161290323%*

 * *Differences: {"'exportimport.constrains'": 'OrderedDict()',*

 * * "'exportimport.conversation'": '[]',*

 * * "'exportimport.versions'": 'OrderedDict()',*

 * * "'language'": "'##DEFAULT##'",*

 * * "'parent'": "{'UID': 'plone_site_root', 'description': 'A Plone Site', 'title': 'Site'}"}*

```diff
@@ -8,27 +8,30 @@
     "creators": [
         "admin"
     ],
     "description": "Site Users",
     "effective": null,
     "exclude_from_nav": false,
     "expires": null,
+    "exportimport.constrains": {},
+    "exportimport.conversation": [],
+    "exportimport.versions": {},
     "id": "Members",
     "is_folderish": true,
-    "language": "en",
+    "language": "##DEFAULT##",
     "layout": "@@member-search",
     "lock": {},
     "modified": "2023-05-18T18:07:36+00:00",
     "nextPreviousEnabled": false,
     "parent": {
         "@id": "/",
         "@type": "Plone Site",
-        "UID": "6de6fe58afb6479f870839b9bc71e9cc",
-        "description": "Congratulations! You have successfully installed Plone.",
-        "title": "Welcome to Plone",
+        "UID": "plone_site_root",
+        "description": "A Plone Site",
+        "title": "Site",
         "type_title": "Plone Site"
     },
     "review_state": "private",
     "rights": "",
     "subjects": [],
     "title": "Users",
     "type_title": "Folder",
```

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/items/3.json` & `plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/content/ab584c1a6fae465da2283a0962f80114/data.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8991935483870968%*

 * *Differences: {"'exportimport.conversation'": '[]',*

 * * "'exportimport.versions'": 'OrderedDict()',*

 * * "'language'": "'##DEFAULT##'",*

 * * "'modified'": "'2024-04-18T18:09:42+00:00'",*

 * * "'parent'": "{'UID': 'plone_site_root', 'description': 'A Plone Site', 'title': 'Site'}"}*

```diff
@@ -23,27 +23,29 @@
             "Link",
             "File",
             "Image",
             "News Item",
             "Event"
         ]
     },
+    "exportimport.conversation": [],
+    "exportimport.versions": {},
     "id": "events",
     "is_folderish": true,
-    "language": "en",
+    "language": "##DEFAULT##",
     "layout": "listing_view",
     "lock": {},
-    "modified": "2023-10-09T22:08:50+00:00",
+    "modified": "2024-04-18T18:09:42+00:00",
     "nextPreviousEnabled": false,
     "parent": {
         "@id": "/",
         "@type": "Plone Site",
-        "UID": "6de6fe58afb6479f870839b9bc71e9cc",
-        "description": "Congratulations! You have successfully installed Plone.",
-        "title": "Welcome to Plone",
+        "UID": "plone_site_root",
+        "description": "A Plone Site",
+        "title": "Site",
         "type_title": "Plone Site"
     },
     "review_state": "published",
     "rights": "",
     "subjects": [],
     "title": "Events",
     "type_title": "Folder",
```

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/items/4.json` & `plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/content/ee556c50736a4650839e2ada6dd65454/data.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8117690058479532%*

 * *Differences: {"'@id'": "'/news/aggregator'",*

 * * "'UID'": "'ee556c50736a4650839e2ada6dd65454'",*

 * * "'customViewFields'": "[OrderedDict([('title', 'Title'), ('token', 'Title')]), "*

 * *                       "OrderedDict([('title', 'Creator'), ('token', 'Creator')]), "*

 * *                       "OrderedDict([('title', 'Type'), ('token', 'Type')]), "*

 * *                       "OrderedDict([('title', 'Last modified'), ('token', 'ModificationDate')])]",*

 * * "'description'": "'Site News'",*

 * * "'exportimport.constrains'": 'OrderedDict()',*

 * * "'exp […]*

```diff
@@ -1,73 +1,88 @@
 {
-    "@id": "/events/aggregator",
+    "@id": "/news/aggregator",
     "@type": "Collection",
-    "UID": "61f6d382910945ea95f2e78a14ebb170",
+    "UID": "ee556c50736a4650839e2ada6dd65454",
     "allow_discussion": false,
     "contributors": [],
     "created": "2023-05-18T18:07:36+00:00",
     "creators": [
         "admin"
     ],
     "customViewFields": [
-        "Title",
-        "Creator",
-        "Type",
-        "ModificationDate"
+        {
+            "title": "Title",
+            "token": "Title"
+        },
+        {
+            "title": "Creator",
+            "token": "Creator"
+        },
+        {
+            "title": "Type",
+            "token": "Type"
+        },
+        {
+            "title": "Last modified",
+            "token": "ModificationDate"
+        }
     ],
-    "description": "Site Events",
+    "description": "Site News",
     "effective": null,
     "exclude_from_nav": false,
     "expires": null,
+    "exportimport.constrains": {},
+    "exportimport.conversation": [],
+    "exportimport.versions": {},
     "id": "aggregator",
     "is_folderish": false,
     "item_count": 30,
     "items_total": 0,
-    "language": "en",
-    "layout": "event_listing",
+    "language": "##DEFAULT##",
+    "layout": "summary_view",
     "limit": 1000,
     "lock": {
         "locked": false,
         "stealable": true
     },
     "modified": "2023-05-18T18:07:36+00:00",
     "parent": {
-        "@id": "/events",
+        "@id": "/news",
         "@type": "Folder",
-        "UID": "ab584c1a6fae465da2283a0962f80114",
-        "description": "Site Events",
+        "UID": "4053ffb6901342ac991afb54da15ab77",
+        "description": "Site News",
         "image_field": null,
         "image_scales": null,
         "review_state": "published",
-        "title": "Events",
+        "title": "News",
         "type_title": "Folder"
     },
     "query": [
         {
             "i": "portal_type",
             "o": "plone.app.querystring.operation.selection.any",
             "v": [
-                "Event"
+                "News Item"
             ]
         },
         {
             "i": "review_state",
             "o": "plone.app.querystring.operation.selection.any",
             "v": [
                 "published"
             ]
         }
     ],
     "review_state": "published",
     "rights": "",
-    "sort_on": "start",
+    "sort_on": "effective",
     "sort_reversed": true,
     "subjects": [],
     "text": null,
-    "title": "Events",
+    "title": "News",
     "type_title": "Collection",
     "version": "current",
     "workflow_history": {
         "simple_publication_workflow": [
             {
                 "action": null,
                 "actor": "admin",
```

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/items/5.json` & `plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/content/4053ffb6901342ac991afb54da15ab77/data.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8991935483870968%*

 * *Differences: {"'exportimport.conversation'": '[]',*

 * * "'exportimport.versions'": 'OrderedDict()',*

 * * "'language'": "'##DEFAULT##'",*

 * * "'modified'": "'2024-04-18T18:09:43+00:00'",*

 * * "'parent'": "{'UID': 'plone_site_root', 'description': 'A Plone Site', 'title': 'Site'}"}*

```diff
@@ -23,27 +23,29 @@
             "Link",
             "File",
             "Image",
             "News Item",
             "Event"
         ]
     },
+    "exportimport.conversation": [],
+    "exportimport.versions": {},
     "id": "news",
     "is_folderish": true,
-    "language": "en",
+    "language": "##DEFAULT##",
     "layout": "listing_view",
     "lock": {},
-    "modified": "2023-10-09T22:08:50+00:00",
+    "modified": "2024-04-18T18:09:43+00:00",
     "nextPreviousEnabled": false,
     "parent": {
         "@id": "/",
         "@type": "Plone Site",
-        "UID": "6de6fe58afb6479f870839b9bc71e9cc",
-        "description": "Congratulations! You have successfully installed Plone.",
-        "title": "Welcome to Plone",
+        "UID": "plone_site_root",
+        "description": "A Plone Site",
+        "title": "Site",
         "type_title": "Plone Site"
     },
     "review_state": "published",
     "rights": "",
     "subjects": [],
     "title": "News",
     "type_title": "Folder",
```

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/items/6.json` & `plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/content/61f6d382910945ea95f2e78a14ebb170/data.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8117690058479532%*

 * *Differences: {"'@id'": "'/events/aggregator'",*

 * * "'UID'": "'61f6d382910945ea95f2e78a14ebb170'",*

 * * "'customViewFields'": "[OrderedDict([('title', 'Title'), ('token', 'Title')]), "*

 * *                       "OrderedDict([('title', 'Creator'), ('token', 'Creator')]), "*

 * *                       "OrderedDict([('title', 'Type'), ('token', 'Type')]), "*

 * *                       "OrderedDict([('title', 'Last modified'), ('token', 'ModificationDate')])]",*

 * * "'description'": "'Site Events'",*

 * * "'exportimport.constrains'": 'OrderedDict()',*

 * * " […]*

```diff
@@ -1,73 +1,88 @@
 {
-    "@id": "/news/aggregator",
+    "@id": "/events/aggregator",
     "@type": "Collection",
-    "UID": "ee556c50736a4650839e2ada6dd65454",
+    "UID": "61f6d382910945ea95f2e78a14ebb170",
     "allow_discussion": false,
     "contributors": [],
     "created": "2023-05-18T18:07:36+00:00",
     "creators": [
         "admin"
     ],
     "customViewFields": [
-        "Title",
-        "Creator",
-        "Type",
-        "ModificationDate"
+        {
+            "title": "Title",
+            "token": "Title"
+        },
+        {
+            "title": "Creator",
+            "token": "Creator"
+        },
+        {
+            "title": "Type",
+            "token": "Type"
+        },
+        {
+            "title": "Last modified",
+            "token": "ModificationDate"
+        }
     ],
-    "description": "Site News",
+    "description": "Site Events",
     "effective": null,
     "exclude_from_nav": false,
     "expires": null,
+    "exportimport.constrains": {},
+    "exportimport.conversation": [],
+    "exportimport.versions": {},
     "id": "aggregator",
     "is_folderish": false,
     "item_count": 30,
     "items_total": 0,
-    "language": "en",
-    "layout": "summary_view",
+    "language": "##DEFAULT##",
+    "layout": "event_listing",
     "limit": 1000,
     "lock": {
         "locked": false,
         "stealable": true
     },
     "modified": "2023-05-18T18:07:36+00:00",
     "parent": {
-        "@id": "/news",
+        "@id": "/events",
         "@type": "Folder",
-        "UID": "4053ffb6901342ac991afb54da15ab77",
-        "description": "Site News",
+        "UID": "ab584c1a6fae465da2283a0962f80114",
+        "description": "Site Events",
         "image_field": null,
         "image_scales": null,
         "review_state": "published",
-        "title": "News",
+        "title": "Events",
         "type_title": "Folder"
     },
     "query": [
         {
             "i": "portal_type",
             "o": "plone.app.querystring.operation.selection.any",
             "v": [
-                "News Item"
+                "Event"
             ]
         },
         {
             "i": "review_state",
             "o": "plone.app.querystring.operation.selection.any",
             "v": [
                 "published"
             ]
         }
     ],
     "review_state": "published",
     "rights": "",
-    "sort_on": "effective",
+    "sort_on": "start",
     "sort_reversed": true,
     "subjects": [],
     "text": null,
-    "title": "News",
+    "title": "Events",
     "type_title": "Collection",
     "version": "current",
     "workflow_history": {
         "simple_publication_workflow": [
             {
                 "action": null,
                 "actor": "admin",
```

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/portlets.json` & `plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/content/portlets.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.359375%*

 * *Differences: {'0': "{'@id': 'http://nohost/classic/Members', 'UID': '54163be595184b4eb0a0b82a58b8def8', delete: "*

 * *      "['uuid']}",*

 * * '1': "{'@id': 'http://nohost/classic', 'portlets': {'plone.footerportlets': {insert: [(0, "*

 * *      "OrderedDict([('assignment', OrderedDict([('macro', ''), ('template', '@@footer')])), "*

 * *      "('type', 'portlets.Classic'), ('visible', True)])), (1, OrderedDict([('assignment', "*

 * *      "OrderedDict([('category', 'site_actions'), ('default_icon', 'action_icon.png'), ('ptitle', "*

 * *      "'site […]*

```diff
@@ -1,10 +1,11 @@
 [
     {
-        "@id": "http://localhost:8080/Plone/Members",
+        "@id": "http://nohost/classic/Members",
+        "UID": "54163be595184b4eb0a0b82a58b8def8",
         "blacklist_status": [
             {
                 "category": "group",
                 "manager": "plone.rightcolumn",
                 "status": "block"
             },
             {
@@ -13,19 +14,19 @@
                 "status": "block"
             },
             {
                 "category": "context",
                 "manager": "plone.rightcolumn",
                 "status": "block"
             }
-        ],
-        "uuid": "54163be595184b4eb0a0b82a58b8def8"
+        ]
     },
     {
-        "@id": "http://localhost:8080/Plone",
+        "@id": "http://nohost/classic",
+        "UID": "plone_site_root",
         "portlets": {
             "plone.footerportlets": [
                 {
                     "assignment": {
                         "macro": "",
                         "template": "@@footer"
                     },
@@ -46,14 +47,41 @@
                 {
                     "assignment": {
                         "macro": "",
                         "template": "colophon"
                     },
                     "type": "portlets.Classic",
                     "visible": true
+                },
+                {
+                    "assignment": {
+                        "macro": "",
+                        "template": "@@footer"
+                    },
+                    "type": "portlets.Classic",
+                    "visible": true
+                },
+                {
+                    "assignment": {
+                        "category": "site_actions",
+                        "default_icon": "action_icon.png",
+                        "ptitle": "site_actions",
+                        "show_icons": false,
+                        "show_title": false
+                    },
+                    "type": "portlets.Actions",
+                    "visible": true
+                },
+                {
+                    "assignment": {
+                        "macro": "",
+                        "template": "colophon"
+                    },
+                    "type": "portlets.Classic",
+                    "visible": true
                 }
             ],
             "plone.leftcolumn": [
                 {
                     "assignment": {
                         "bottomLevel": 0,
                         "currentFolderOnly": false,
@@ -63,26 +91,51 @@
                         "no_thumbs": false,
                         "root_uid": null,
                         "thumb_scale": null,
                         "topLevel": 1
                     },
                     "type": "portlets.Navigation",
                     "visible": true
+                },
+                {
+                    "assignment": {
+                        "bottomLevel": 0,
+                        "currentFolderOnly": false,
+                        "includeTop": false,
+                        "name": "",
+                        "no_icons": false,
+                        "no_thumbs": false,
+                        "root_uid": null,
+                        "thumb_scale": null,
+                        "topLevel": 1
+                    },
+                    "type": "portlets.Navigation",
+                    "visible": true
                 }
             ],
             "plone.rightcolumn": [
                 {
                     "assignment": {
                         "count": 5,
                         "no_thumbs": false,
                         "search_base_uid": null,
                         "state": null,
                         "thumb_scale": null
                     },
                     "type": "portlets.Events",
                     "visible": true
+                },
+                {
+                    "assignment": {
+                        "count": 5,
+                        "no_thumbs": false,
+                        "search_base_uid": null,
+                        "state": null,
+                        "thumb_scale": null
+                    },
+                    "type": "portlets.Events",
+                    "visible": true
                 }
             ]
-        },
-        "uuid": "<Portal>"
+        }
     }
 ]
```

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/image.png` & `plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/image.png`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/schema.json` & `plone_distribution-2.0.0a1/src/plone/distribution/distributions/classic/schema.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/distributions/default/image.png` & `plone_distribution-2.0.0a1/src/plone/distribution/distributions/default/image.png`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/distributions/default/schema.json` & `plone_distribution-2.0.0a1/tests/utils/data/valid.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/exportimport/dist_export.py` & `plone_distribution-2.0.0a1/src/plone/distribution/services/sites/get.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,135 +1,130 @@
-from collective.exportimport import config
-from collective.exportimport.export_content import ExportContent as BaseExportView
-from pathlib import Path
-from plone import api
-from plone.dexterity.content import DexterityContent
-from plone.distribution import logger
+from AccessControl import getSecurityManager
 from plone.distribution.api import distribution as dist_api
 from plone.distribution.api import site as site_api
 from plone.distribution.core import Distribution
-from plone.distribution.exportimport import helpers
-from plone.distribution.exportimport.interfaces import IDistributionBlobsMarker
-from Products.Five import BrowserView
+from plone.distribution.utils.request import extract_browser_language
+from plone.distribution.utils.schema import should_provide_default_language_default
+from plone.restapi.services import Service
+from Products.CMFCore.permissions import ManagePortal
 from typing import List
-from zope.interface import alsoProvides
-
-
-class ExportAll(BrowserView):
-    distribution: Distribution
-    directory: Path
-    _current_content: List[Path]
-
-    def __call__(self):
-        request = self.request
-        # We do not allow exports to other distributions
-        # as that was confusing and error-prune
-        self.distribution = self.get_current_distribution()
-        self.directory = self.distribution.directory / "content"
-        self.other_exports = helpers.exports_for_distribution(self.distribution)
-        if not request.form.get("form.submitted", False):
-            return self.index()
-        # Get exports
-        all_exports = request.form.get("exports", [])
-        if all_exports:
-            # Remove contents, as it is always required
-            all_exports.remove("contents")
-
-        # To handle an issue with json_body deserialization
-        request["BODY"] = {}
-        other_exports = all_exports or self.other_exports
-        alsoProvides(self.request, IDistributionBlobsMarker)
-        config.CENTRAL_DIRECTORY = str(self.directory)
-        # pass the target-dir to blob-serializer via request
-        request.form["distribution_directory"] = config.CENTRAL_DIRECTORY
-        # Export all content
-        export_name = "dist_export_content"
-        view = api.content.get_view(export_name, self.context, request)
-        # small hack to get all exportable types from the view
-        view.portal_type = []
-        view.path = "/".join(self.context.getPhysicalPath())
-        view.depth = -1
-        portal_types = [i["value"] for i in view.portal_types()]
-        download_to_server = request.form.get("download_to_server", 2)
-        split_files = download_to_server == 2
-        filename = "items.json"
-        if not split_files:
-            portal_types.remove("Plone Site")
-            filename = "content.json"
-        request.form["filename"] = filename
-        view(
-            portal_type=portal_types,
-            include_blobs=2,
-            download_to_server=download_to_server,
-        )
-        logger.info(f"Finished {export_name}")
+from zExceptions import BadRequest
+from zope.interface import implementer
+from zope.publisher.interfaces import IPublishTraverse
+
+import json
+
+
+DEFAULT_ID = "Plone"
+
+
+def _is_outdated(site) -> bool:
+    """Check if site needs an upgrade."""
+    mig = getattr(site, "portal_migration", None) or site.get("portal_migration", None)
+    return mig.needUpgrading() if mig else False
+
+
+_no_content_marker = object()
+
+
+@implementer(IPublishTraverse)
+class SitesGet(Service):
+    def __init__(self, context, request):
+        super().__init__(context, request)
+        self.params = []
+
+    def publishTraverse(self, request, name):
+        # Consume any path segments after /@users as parameters
+        self.params.append(name)
+        return self
+
+    def check_permission(self):
+        """Ignore 'plone.restapi: Use REST API' permission on Application."""
+        pass
+
+    def render(self):
+        # Make sure we do not change the order of the keys
+        content = self.reply()
+        if content is not _no_content_marker:
+            self.request.response.setHeader("Content-Type", self.content_type)
+            return json.dumps(content, indent=2, separators=(", ", ": "))
+
+    def get_distributions(self, base_url: str) -> List[dict]:
+        """Return a list of available distributions."""
+        response = []
+        distributions = dist_api.get_distributions()
+        for dist in distributions:
+            response.append(
+                {
+                    "@id": f"{base_url}/{dist.name}",
+                    "name": dist.name,
+                    "title": dist.title,
+                    "description": dist.description,
+                    "image": f"{self.context.absolute_url()}/@@dist-image/{dist.name}",
+                }
+            )
+        return response
 
-        if not split_files:
-            portal_types = ["Plone Site"]
-            request.form["filename"] = "portal.json"
-            view(portal_type=portal_types, include_blobs=2, download_to_server=True)
-            logger.info(f"Finished {export_name}")
-
-        for export in other_exports:
-            export_view = api.content.get_view(
-                f"export_{export}", self.context, request
+    def get_sites(self) -> List[dict]:
+        """Return a list of site information."""
+        response = []
+        sites = site_api.get_sites(self.context)
+        for site in sites:
+            dist_report = dist_api.get_creation_report(site)
+            distribution_name = dist_report.name if dist_report else ""
+            response.append(
+                {
+                    "@id": site.absolute_url(),
+                    "id": site.id,
+                    "title": site.title,
+                    "description": site.description,
+                    "creation_date": site.CreationDate(),
+                    "needs_upgrade": _is_outdated(site),
+                    "distribution": distribution_name,
+                }
             )
-            request.form["form.submitted"] = True
-            request.form["filename"] = f"{export}.json"
-            export_view(download_to_server=True)
-
-        logger.info("Finished export_all")
-        return self.request.response.redirect(self.context.absolute_url())
-
-    def get_current_distribution(self) -> Distribution:
-        """Extract distribution used to create the current site."""
-        creation_report = site_api.get_creation_report(api.portal.get())
-        dist = None
-        if creation_report:
-            name = creation_report.answers.get("distribution", "")
-            dist = dist_api.get(name=name)
-        return dist
-
-    def distributions(self, name: str = "") -> List[Distribution]:
-        """Return a list of distributions."""
-        if not name:
-            name = self.get_current_distribution()
-        return helpers.filter_devel_distributions(name=name)
-
-
-class ExportContent(BaseExportView):
-    """Export content from a distribution."""
-
-    PORTAL_URL: str = ""
-
-    def __call__(
-        self,
-        portal_type=None,
-        path=None,
-        depth=-1,
-        include_blobs=1,
-        download_to_server=False,
-        migration=True,
-        include_revisions=False,
-    ):
-        self.PORTAL_URL = api.portal.get().absolute_url()
+        return response
+
+    def _populate_server_defaults(self, distribution: Distribution) -> dict:
+        """Provide default values for new Plone sites."""
+        server_defaults = {}
         request = self.request
-        if download_to_server == 2:
-            distribution_directory = request.form["distribution_directory"]
-            helpers.remove_path(distribution_directory)
-        return super().__call__(
-            portal_type,
-            path,
-            depth,
-            include_blobs,
-            download_to_server,
-            migration,
-            include_revisions,
+        # Sites with default id
+        all_sites = self.get_sites()
+        sites = [site for site in all_sites if site["id"].startswith(DEFAULT_ID)]
+        server_defaults["site_id"] = (
+            f"{DEFAULT_ID}{len(sites)}" if sites else DEFAULT_ID
         )
-
-    def global_dict_hook(self, item: dict, obj: DexterityContent) -> dict:
-        """Clean up data before export."""
-        item = helpers.remove_site_root(item, self.PORTAL_URL)
-        if item["@type"] == "Plone Site":
-            # To avoid a conflict between @id and id
-            item["@id"] = f"/{item['id']}"
-        return item
+        jsonschema = distribution.schema
+        uischema = distribution.uischema
+        if should_provide_default_language_default(uischema, jsonschema):
+            server_defaults["default_language"] = extract_browser_language(request)
+        return server_defaults
+
+    def can_manage(self) -> bool:
+        secman = getSecurityManager()
+        return True if secman.checkPermission(ManagePortal, self.context) else False
+
+    def reply(self) -> dict:
+        base_url = f"{self.context.absolute_url()}/@sites"
+        if len(self.params) == 0:
+            return {
+                "@id": base_url,
+                "can_manage": self.can_manage(),
+                "sites": self.get_sites(),
+                "distributions": self.get_distributions(base_url),
+            }
+        else:
+            name = self.params[0]
+            dist = dist_api.get(name)
+            if not dist:
+                raise BadRequest("Parameters supplied are not valid")
+            return {
+                "@id": f"{base_url}/{dist.name}",
+                "name": dist.name,
+                "title": dist.title,
+                "description": dist.description,
+                "image": f"{base_url}/@@dist-image/{dist.name}",
+                "schema": dist.schema,
+                "uischema": dist.uischema,
+                "default_values": self._populate_server_defaults(dist),
+            }
```

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/handler.py` & `plone_distribution-2.0.0a1/src/plone/distribution/handler.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from plone import api
+from plone.dexterity.schema import SCHEMA_CACHE
+from plone.distribution import logger
 from plone.distribution.core import Distribution
+from plone.distribution.utils.data import convert_data_uri_to_b64
+from plone.exportimport.importers import get_importer
 from Products.CMFPlone.Portal import PloneSite
-from zope.globalrequest import getRequest
 
 import transaction
 
 
 def default_pre_handler(answers: dict) -> dict:
     """Process answers before creating a new site."""
     return answers
@@ -30,11 +33,27 @@
         for profile_id in content_profiles:
             setup_tool.runAllImportStepsFromProfile(f"profile-{profile_id}")
         # Process content import from json
         content_json_path = contents["json"]
         if content_json_path:
             # If there is no savepoint most tests fail with a PosKeyError
             transaction.savepoint(optimistic=True)
-            request = getRequest() or site.REQUEST
-            import_all = api.content.get_view("dist_import_all", site, request)
-            import_all(content_json_path)
+            # Invalidate the schema cache to make sure we get up to date behaviors.
+            # Normally this happens on commit, but we didn't commit yet.
+            SCHEMA_CACHE.clear()
+            importer = get_importer(site)
+            importer.import_site(content_json_path)
+            transaction.commit()
+    return site
+
+
+def post_handler(
+    distribution: Distribution, site: PloneSite, answers: dict
+) -> PloneSite:
+    """After site creation, run last steps."""
+    name = distribution.name
+    raw_logo = answers.get("site_logo")
+    if raw_logo:
+        logo = convert_data_uri_to_b64(raw_logo)
+        logger.info(f"{name}: Set logo")
+        api.portal.set_registry_record("plone.site_logo", logo)
     return site
```

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/interfaces.py` & `plone_distribution-2.0.0a1/src/plone/distribution/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/metaconfigure.py` & `plone_distribution-2.0.0a1/src/plone/distribution/metaconfigure.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/registry.py` & `plone_distribution-2.0.0a1/src/plone/distribution/registry.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/services/auth/login.py` & `plone_distribution-2.0.0a1/src/plone/distribution/services/auth/login.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Authenticate a user in Zope root."""
+
 from plone.restapi.deserializer import json_body
 from plone.restapi.services import Service
 from zope.interface import alsoProvides
 
 import plone.protect.interfaces
```

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/services/overrides.zcml` & `plone_distribution-2.0.0a1/src/plone/distribution/services/overrides.zcml`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
       />
 
   <unconfigure>
 
     <plone:service
         method="GET"
         factory="plone.restapi.services.system.get.SystemGet"
-        for="Products.CMFPlone.interfaces.IPloneSiteRoot"
+        for="plone.base.interfaces.IPloneSiteRoot"
         permission="plone.app.controlpanel.Overview"
         name="@system"
         />
 
 
   </unconfigure>
```

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/services/sites/add.py` & `plone_distribution-2.0.0a1/src/plone/distribution/services/sites/add.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Service to create a Plone Site."""
+
+from plone.distribution import logger
 from plone.distribution.api import distribution as dist_api
 from plone.distribution.api import site as site_api
 from plone.distribution.utils.validation import validate_answers
 from plone.restapi.deserializer import json_body
 from plone.restapi.services import Service
 from zExceptions import BadRequest
 from zExceptions import NotFound
@@ -46,15 +48,17 @@
         try:
             site = site_api.create(
                 self.context,
                 distribution_name=distribution_name,
                 answers=data,
             )
         except KeyError:
+            logger.error("Error creating the site.", exc_info=True)
             raise BadRequest("Error creating the site.")
         site_info = {
             "@id": site.absolute_url(),
+            "@type": site.portal_type,
             "id": site.id,
             "title": site.title,
             "description": site.description,
         }
         return site_info
```

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/services/sites/configure.zcml` & `plone_distribution-2.0.0a1/src/plone/distribution/services/sites/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/services/sites/get.py` & `plone_distribution-2.0.0a1/tests/services/test_services_site.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,130 +1,136 @@
-from AccessControl import getSecurityManager
-from plone.distribution.api import distribution as dist_api
-from plone.distribution.api import site as site_api
-from plone.distribution.core import Distribution
-from plone.distribution.utils.request import extract_browser_language
-from plone.distribution.utils.schema import should_provide_default_language_default
-from plone.restapi.services import Service
-from Products.CMFCore.permissions import ManagePortal
-from typing import List
-from zExceptions import BadRequest
-from zope.interface import implementer
-from zope.publisher.interfaces import IPublishTraverse
-
-import json
-
-
-DEFAULT_ID = "Plone"
-
-
-def _is_outdated(site) -> bool:
-    """Check if site needs an upgrade."""
-    mig = getattr(site, "portal_migration", None) or site.get("portal_migration", None)
-    return mig.needUpgrading() if mig else False
-
-
-_no_content_marker = object()
-
-
-@implementer(IPublishTraverse)
-class SitesGet(Service):
-    def __init__(self, context, request):
-        super().__init__(context, request)
-        self.params = []
-
-    def publishTraverse(self, request, name):
-        # Consume any path segments after /@users as parameters
-        self.params.append(name)
-        return self
-
-    def check_permission(self):
-        """Ignore 'plone.restapi: Use REST API' permission on Application."""
-        pass
-
-    def render(self):
-        # Make sure we do not change the order of the keys
-        content = self.reply()
-        if content is not _no_content_marker:
-            self.request.response.setHeader("Content-Type", self.content_type)
-            return json.dumps(content, indent=2, separators=(", ", ": "))
-
-    def get_distributions(self, base_url: str) -> List[dict]:
-        """Return a list of available distributions."""
-        response = []
-        distributions = dist_api.get_distributions()
-        for dist in distributions:
-            response.append(
-                {
-                    "@id": f"{base_url}/{dist.name}",
-                    "name": dist.name,
-                    "title": dist.title,
-                    "description": dist.description,
-                    "image": f"{self.context.absolute_url()}/@@dist-image/{dist.name}",
-                }
-            )
-        return response
-
-    def get_sites(self) -> List[dict]:
-        """Return a list of site information."""
-        response = []
-        sites = site_api.get_sites(self.context)
-        for site in sites:
-            dist_report = site_api.get_creation_report(site)
-            distribution_name = dist_report.name if dist_report else ""
-            response.append(
-                {
-                    "@id": site.absolute_url(),
-                    "id": site.id,
-                    "title": site.title,
-                    "description": site.description,
-                    "creation_date": site.CreationDate(),
-                    "needs_upgrade": _is_outdated(site),
-                    "distribution": distribution_name,
-                }
-            )
-        return response
-
-    def _populate_server_defaults(self, distribution: Distribution) -> dict:
-        """Provide default values for new Plone sites."""
-        server_defaults = {}
-        request = self.request
-        # Sites with default id
-        all_sites = self.get_sites()
-        sites = [site for site in all_sites if site["id"].startswith(DEFAULT_ID)]
-        server_defaults["site_id"] = (
-            f"{DEFAULT_ID}{len(sites)}" if sites else DEFAULT_ID
+from copy import deepcopy
+from plone.app.testing import SITE_OWNER_NAME
+from plone.app.testing import SITE_OWNER_PASSWORD
+from plone.restapi.testing import RelativeSession
+
+import pytest
+
+
+class TestServicesSite:
+    @pytest.fixture(autouse=True)
+    def _api_session(self, app):
+        url = app.absolute_url()
+        api_session = RelativeSession(url)
+        api_session.auth = (SITE_OWNER_NAME, SITE_OWNER_PASSWORD)
+        api_session.headers.update({"Accept": "application/json"})
+        self.api_session = api_session
+
+
+class TestServicesSitesGET(TestServicesSite):
+    def test_sites_get_anonymous(self, app):
+        self.api_session.auth = None
+        response = self.api_session.get("@sites")
+        assert response.status_code == 200
+        data = response.json()
+        assert isinstance(data, dict)
+        assert data["can_manage"] is False
+
+    def test_sites_get_authenticated(self, app):
+        response = self.api_session.get("@sites")
+        assert response.status_code == 200
+        data = response.json()
+        assert isinstance(data, dict)
+        assert data["can_manage"] is True
+
+    def test_sites_get_distributions(self, app):
+        response = self.api_session.get("@sites")
+        data = response.json()
+        distributions = data["distributions"]
+        assert isinstance(distributions, list)
+        assert len(distributions) == 2
+        assert distributions[0]["name"] == "default"
+        assert distributions[0]["title"] == "Plone Site"
+
+    def test_sites_get_sites(self, app):
+        response = self.api_session.get("@sites")
+        data = response.json()
+        sites = data["sites"]
+        assert isinstance(sites, list)
+        assert len(sites) == 2
+        assert sites[0]["id"] == "plone"
+        assert sites[0]["needs_upgrade"] is False
+
+
+class TestServicesSitesPOST(TestServicesSite):
+    @pytest.fixture(autouse=True)
+    def _answers(self):
+        self.answers = {
+            "site_id": "PloneBrasil",
+            "title": "Plone site in Brazil",
+            "description": "A simple Plone Site",
+            "default_language": "pt-br",
+            "portal_timezone": "America/Sao_Paulo",
+            "setup_content": True,
+        }
+
+    @pytest.mark.parametrize(
+        "distribution_name",
+        [
+            "default",
+            "classic",
+        ],
+    )
+    def test_sites_create_success(self, app, distribution_name):
+        response = self.api_session.post(
+            f"@sites/{distribution_name}", json=self.answers
         )
-        jsonschema = distribution.schema
-        uischema = distribution.uischema
-        if should_provide_default_language_default(uischema, jsonschema):
-            server_defaults["default_language"] = extract_browser_language(request)
-        return server_defaults
-
-    def can_manage(self) -> bool:
-        secman = getSecurityManager()
-        return True if secman.checkPermission(ManagePortal, self.context) else False
-
-    def reply(self) -> dict:
-        base_url = f"{self.context.absolute_url()}/@sites"
-        if len(self.params) == 0:
-            return {
-                "@id": base_url,
-                "can_manage": self.can_manage(),
-                "sites": self.get_sites(),
-                "distributions": self.get_distributions(base_url),
-            }
-        else:
-            name = self.params[0]
-            dist = dist_api.get(name)
-            if not dist:
-                raise BadRequest("Parameters supplied are not valid")
-            return {
-                "@id": f"{base_url}/{dist.name}",
-                "name": dist.name,
-                "title": dist.title,
-                "description": dist.description,
-                "image": f"{base_url}/@@dist-image/{dist.name}",
-                "schema": dist.schema,
-                "uischema": dist.uischema,
-                "default_values": self._populate_server_defaults(dist),
-            }
+        assert response.status_code == 200
+        data = response.json()
+        assert data["id"] == "PloneBrasil"
+        assert data["@type"] == "Plone Site"
+
+    @pytest.mark.parametrize(
+        "distribution_name",
+        [
+            "someStrangeName",
+            "404",
+        ],
+    )
+    def test_sites_create_failure(self, app, distribution_name):
+        """Test POST with non-existing distribution names."""
+        response = self.api_session.post(
+            f"@sites/{distribution_name}", json=self.answers
+        )
+        assert response.status_code == 404
+        data = response.json()
+        assert data["message"].startswith("Resource not found:")
+
+    def test_sites_create_empty_site_id(self, app):
+        distribution_name = "default"
+        # Empty site_id
+        answers = {"site_id": "", "title": "Site"}
+
+        response = self.api_session.post(f"@sites/{distribution_name}", json=answers)
+        assert response.status_code == 400
+        data = response.json()
+        assert data["message"].startswith("Invalid data for site creation")
+
+    def test_sites_create_empty_title(self, app):
+        distribution_name = "default"
+        # Empty title
+        answers = {"site_id": "Site", "title": ""}
+
+        response = self.api_session.post(f"@sites/{distribution_name}", json=answers)
+        assert response.status_code == 400
+        data = response.json()
+        assert data["message"].startswith("Invalid data for site creation")
+
+    def test_sites_create_invalid_language(self, app):
+        distribution_name = "default"
+        answers = deepcopy(self.answers)
+        answers["default_language"] = "klingon"
+
+        response = self.api_session.post(f"@sites/{distribution_name}", json=answers)
+        assert response.status_code == 400
+        data = response.json()
+        assert data["message"].startswith("Invalid data for site creation")
+
+    def test_sites_create_invalid_timezone(self, app):
+        distribution_name = "default"
+        answers = deepcopy(self.answers)
+        answers["portal_timezone"] = "something"
+
+        response = self.api_session.post(f"@sites/{distribution_name}", json=answers)
+        assert response.status_code == 400
+        data = response.json()
+        assert data["message"].startswith("Invalid data for site creation")
```

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/services/system/get.py` & `plone_distribution-2.0.0a1/src/plone/distribution/services/system/get.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from plone.distribution.api import distribution as dist_api
-from plone.distribution.api import site as site_api
 from plone.restapi.services.system.get import SystemGet as BaseService
 
 import pkg_resources
 
 
 plone_distribution_version = pkg_resources.require("plone.distribution")[0].version
 
 
 class SystemGet(BaseService):
     def distribution_info(self) -> str:
         """Get distribution information if site was created with a distribution."""
         info = ""
         portal = self.context
-        report = site_api.get_creation_report(portal)
+        report = dist_api.get_creation_report(portal)
         if report:
             dist_name = report.name
             try:
                 dist_title = dist_api.get(dist_name).title
             except ValueError:
                 dist_title = "Uninstalled"
             info = f"{dist_title} ({dist_name})"
```

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/testing/layer.py` & `plone_distribution-2.0.0a1/src/plone/distribution/testing/layer.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 from plone.app.testing.interfaces import SITE_OWNER_PASSWORD
 from plone.app.testing.interfaces import TEST_USER_ID
 from plone.app.testing.interfaces import TEST_USER_NAME
 from plone.app.testing.interfaces import TEST_USER_PASSWORD
 from plone.app.testing.interfaces import TEST_USER_ROLES
 from plone.app.testing.layers import PloneFixture
 from plone.testing import zope
+from zope.globalrequest import setRequest
 
 
 DEFAULT_DISTRIBUTION = "default"
 DEFAULT_ANSWERS = {
     "site_id": PLONE_SITE_ID,
     "title": "Plone Site",
     "description": "A Plone Site",
+    "site_logo": "name=teste;data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAUAAAAFCAYAAACNbyblAAAAHElEQVQI12P4//8/w38GIAXDIBKE0DHxgljNBAAO9TXL0Y4OHwAAAABJRU5ErkJggg==",  # noQA
     "default_language": "en",
     "portal_timezone": "America/Sao_Paulo",
     "setup_content": True,
 }
 
 
 class PloneDistributionFixture(PloneFixture):
@@ -29,15 +31,14 @@
 
     PACKAGE_NAME: str = ""
     SITES: tuple = ()
 
     _distribution_products = (
         ("plone.app.contenttypes", {"loadZCML": True}),
         ("plone.restapi", {"loadZCML": True}),
-        ("collective.exportimport", {"loadZCML": True}),
         ("plone.volto", {"loadZCML": True, "silent": True}),
         ("plone.distribution", {"loadZCML": True}),
     )
 
     @property
     def products(self):
         """Merge products available on PloneFixture, with ones needed here."""
@@ -62,14 +63,15 @@
 
         # Create the owner user and "log in" so that the site object gets
         # the right ownership information
         app["acl_users"].userFolderAddUser(
             SITE_OWNER_NAME, SITE_OWNER_PASSWORD, ["Manager"], []
         )
 
+        setRequest(app.REQUEST)
         zope.login(app["acl_users"], SITE_OWNER_NAME)
         sites = self.sites
         for distribution_name, answers in sites:
             site_id = answers["site_id"]
             # Create Plone site
             site_api._create_site(
                 context=app, distribution_name=distribution_name, answers=answers
@@ -81,7 +83,8 @@
             pas = app[site_id]["acl_users"]
             pas.source_users.addUser(TEST_USER_ID, TEST_USER_NAME, TEST_USER_PASSWORD)
             for role in TEST_USER_ROLES:
                 pas.portal_role_manager.doAssignRoleToPrincipal(TEST_USER_ID, role)
 
         # Log out again
         zope.logout()
+        setRequest(None)
```

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/testing/testing.py` & `plone_distribution-2.0.0a1/src/plone/distribution/testing/testing.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from plone.testing.zope import WSGI_SERVER_FIXTURE
 
 
 CLASSIC_ANSWERS = {
     "site_id": "classic",
     "title": "Plone Site",
     "description": "A Plone Site with Classic UI",
+    "site_logo": "name=teste;data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAUAAAAFCAYAAACNbyblAAAAHElEQVQI12P4//8/w38GIAXDIBKE0DHxgljNBAAO9TXL0Y4OHwAAAABJRU5ErkJggg==",  # noQA
     "default_language": "en",
     "portal_timezone": "America/Sao_Paulo",
     "setup_content": True,
 }
 
 
 class BaseFixture(PloneDistributionFixture):
```

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/utils/request.py` & `plone_distribution-2.0.0a1/src/plone/distribution/utils/request.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/utils/schema.py` & `plone_distribution-2.0.0a1/src/plone/distribution/utils/schema.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/src/plone/distribution/utils/validation.py` & `plone_distribution-2.0.0a1/src/plone/distribution/utils/validation.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/src/plone.distribution.egg-info/PKG-INFO` & `plone_distribution-2.0.0a1/src/plone.distribution.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.distribution
-Version: 1.0.0b4
+Version: 2.0.0a1
 Summary: Plone distribution support
 Home-page: https://plone.org
 Author: Plone Foundation
 Author-email: releasemanager@plone.org
 License: GPL version 2
 Project-URL: Homepage, https://plone.org
 Project-URL: Documentation, https://6.docs.plone.org
@@ -22,57 +22,84 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: Products.CMFPlone
+Requires-Dist: Products.GenericSetup
+Requires-Dist: Zope
+Requires-Dist: setuptools
+Requires-Dist: jsonschema
+Requires-Dist: plone.api
+Requires-Dist: plone.base
+Requires-Dist: plone.dexterity
+Requires-Dist: plone.exportimport>=1.0.0a5
+Requires-Dist: plone.i18n
+Requires-Dist: plone.protect
+Requires-Dist: plone.rest
+Requires-Dist: plone.restapi
+Requires-Dist: z3c.unconfigure
+Provides-Extra: test
+Requires-Dist: plone.app.iterate; extra == "test"
+Requires-Dist: plone.app.testing; extra == "test"
+Requires-Dist: plone.app.upgrade; extra == "test"
+Requires-Dist: plone.restapi[test]; extra == "test"
+Requires-Dist: plone.volto[test]; extra == "test"
+Requires-Dist: plone.testing; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-plone>=0.5.0; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: zest.releaser[recommended]; extra == "test"
+Requires-Dist: zestreleaser.towncrier; extra == "test"
 
 
 <p align="center">
     <img alt="Plone Logo" width="200px" src="https://raw.githubusercontent.com/plone/.github/main/plone-logo.png">
 </p>
 
 <h1 align="center">
   Plone Distributions
 </h1>
 
-Package supporting the (easy) implementation of a Plone Distribution.
+Package supporting the (easy) implementation of a Plone distribution.
 
-## What is a Plone Distribution
+## What is a Plone distribution
 
-A Plone distribution is a pre-packaged version of Plone that includes specific features, themes, modules, and configurations. It is a convenient way to get a specific type of website up and running quickly, as the distribution includes everything needed to run that type of site.
+A Plone distribution is a pre-packaged version of Plone that includes specific features, themes, modules, and configurations.
+It is a convenient way to get a specific type of website up and running quickly, as the distribution includes everything needed to run that type of site.
 
 Examples of Plone distributions include:
 
-* [SENAITE](https://www.senaite.com)
-* [Quaive](https://quaivecloud.com/)
-* [Portal Modelo](https://www.interlegis.leg.br/produtos-servicos/portal-modelo/)
-* [Portal Padrão](https://identidade-digital-de-governo-plone.readthedocs.io/en/latest/)
+- [SENAITE](https://www.senaite.com)
+- [Quaive](https://quaivecloud.com/)
+- [Portal Modelo](https://www.interlegis.leg.br/produtos-servicos/portal-modelo/)
+- [Portal Padrão](https://identidade-digital-de-governo-plone.readthedocs.io/en/latest/)
 
 ### Similar Concept in Other CMS
 
-* Drupal: Drupal has distributions for blogs, e-commerce sites, and intranet portals.
+- **Drupal:** Drupal has distributions for blogs, e-commerce sites, and intranet portals.
 
-* WordPress: WordPress has a similar concept in the form of "WordPress Multisite," which allows users to run multiple websites from a single installation of WordPress.
+- **WordPress:** WordPress has a similar concept in the form of "WordPress Multisite," which allows users to run multiple websites from a single installation of WordPress.
 
-* Joomla: Joomla has a similar concept in the form of "Joomla Templates," which are pre-designed templates for Joomla websites.
+- **Joomla:** Joomla has a similar concept in the form of "Joomla Templates," which are pre-designed templates for Joomla websites.
 
-* TYPO3: TYPO3 has a similar concept in the form of "TYPO3 Distributions," which are pre-configured installations of TYPO3 for specific types of websites.
+- **TYPO3:** TYPO3 has a similar concept in the form of "TYPO3 Distributions," which are pre-configured installations of TYPO3 for specific types of websites.
 
-## Creating a new Distribution
+## Creating a new distribution
 
-First of all, a Plone Distribution is a Python Package that can be installed by `pip`.
+A Plone distribution is a Python Package that can be installed by `pip`.
 
 ### `setup.py`
+
 The package will follow some conventions, to make it "discoverable" by others.
 
-In `setup.py`, always add the correct Trove Classifiers:
+In `setup.py`, always add the correct Trove classifiers:
 
 ```python
         "Framework :: Plone",
         "Framework :: Plone :: 6.0",
         "Framework :: Plone :: Distribution",
 ```
 
@@ -84,40 +111,38 @@
         "setuptools",
         "plone.distribution",
     ],
 ```
 
 ### `configure.zcml`
 
-In your main `configure.zcml`, make sure to have the `plone` xml namespace declared:
+In your main `configure.zcml`, make sure to have the `plone` XML namespace declared:
 
 ```xml
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:plone="http://namespaces.plone.org/plone"
     >
 ```
 
 And also include `plone.distribution`:
 
 ```xml
-  <include package="plone.distribution" />
+<include package="plone.distribution" />
 ```
 
 Then declare the distributions included in your package:
 
 ```xml
-
   <plone:distribution
       name="blog"
       title="Personal Blog"
       description="A Plone site already configured to host a personal Blog."
       directory="distributions/blog"
       />
-
 ```
 
 The registered distribution will configure a Personal Blog, with some default content.
 
 #### distribution handlers
 
 When registering a distribution, you can provide a `pre_handler`, a `handler` and a `post_handler` which must be
@@ -133,30 +158,28 @@
 def post_handler(distribution: Distribution, site, answers: dict):
     return site
 ```
 
 Each of those handlers will be called in this way:
 
 - `pre_handler`: it will process the answers to do modifications on them before creating the site
-- `handler`: it will be run after the bare Plone site will be created but instead of the default handler that installs the required GenericSetup profiles and creates the content.
-- `post_handler`: it will be run after the site is setup.
+- `handler`: it will be run after the bare Plone site will be created, but instead of the default handler that installs the required GenericSetup profiles and creates the content.
+- `post_handler`: it will be run after the site is set up.
 
-So if you have added some extra fields in the Plone site creation form and want to do some extra configuration in the
+If you have added some extra fields in the Plone site creation form and want to do some extra configuration in the
 Plone site, you can add your own handler and register as follows:
 
 ```xml
-
   <plone:distribution
       name="blog"
       title="Personal Blog"
       description="A Plone site already configured to host a personal Blog."
       directory="distributions/blog"
       post_handler=".handlers.blog.post_handler"
       />
-
 ```
 
 ### distribution folder
 
 A convention is to use the `distributions/<distribution_name>`folder in the root of your package to organize your distribution configuration.
 
 In that folder, you will need to provide:
@@ -167,17 +190,17 @@
 
 ### `profiles.json`
 
 A `JSON` file with the GenericSetup profiles that are used by your distribution during installation.
 
 This file needs to contain two keys:
 
-* **base**: List of profiles installed in every new site using this distribution.
+- **base**: List of profiles installed in every new site using this distribution.
 
-* **content**: List of profiles installed when the user decides to create a site with example content.
+- **content**: List of profiles installed when the user decides to create a site with example content.
 
 The configuration for a new Volto site is:
 
 ```json
 {
   "base": [
     "plone.app.contenttypes:default",
@@ -234,25 +257,25 @@
 
 ### `schema.json`
 
 In case you require additional input from the user during site creation, you can customize the form using the `schema.json` file.
 
 The file should contain two keys:
 
-* **schema**: A JSON Schema definition.
-* **uischema**: A [react-jsonschema-form](https://rjsf-team.github.io/react-jsonschema-form/docs/) configuration to modify how the form is displayed.
+- **schema**: A JSON Schema definition.
+- **uischema**: A [react-jsonschema-form](https://rjsf-team.github.io/react-jsonschema-form/docs/) configuration to modify how the form is displayed.
 
 The **schema** should have at least the following keys:
 
-* site_id
-* title
-* description
-* default_language
-* portal_timezone
-* setup_content
+- site_id
+- title
+- description
+- default_language
+- portal_timezone
+- setup_content
 
 The `schema.json` used for the default site creation is:
 
 ```json
 {
   "schema": {
     "title": "Create a Plone site",
@@ -309,55 +332,100 @@
 {"$ref": "#/definitions/timezones"}
 ```
 
 Both definitions are added in runtime by `plone.distribution` to provide a list of languages and timezones available on the installation.
 
 ### `content` folder
 
-Folder containing JSON data exported using the `@@dist_export_all` browser view of this package.
+Folder containing JSON data representing this distribution's content.
+
+To export content from a site into this folder, use the `bin/export-distribution` script.
+
+```shell
+bin/export-distribution path/to/zope.conf Plone
+```
+
+> In the example above, "Plone" is the ID of the Plone site to export.
 
 ## Advanced Usage
 
 ### Hiding Distributions
 
 By default, `plone.distribution` ships with two ready-to-use distributions:
 
-* **default**: Plone Site (Volto frontend)
-* **classic**: Plone Site (Classic UI)
+- **default**: Plone Site (Volto frontend)
+- **classic**: Plone Site (Classic UI)
 
 If you want to limit your users option to select a distribution, it is possible to set the environment variable `ALLOWED_DISTRIBUTIONS` with fewer options:
 
 ```shell
 ALLOWED_DISTRIBUTIONS=default
 ```
 
-
 ## This project is supported by
 
 <p align="left">
     <a href="https://plone.org/foundation/">
       <img alt="Plone Logo" width="200px" src="https://raw.githubusercontent.com/plone/.github/main/plone-foundation.png">
     </a>
 </p>
 
 ## License
+
 The project is licensed under the GPLv2.
 
 
 # Changelog
 
 <!--
    You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 2.0.0a1 (2024-05-16)
+
+
+### Breaking changes:
+
+- plone.distribution is now based on plone.exportimport instead of collective.exportimport.
+
+  There are some backwards-incompatible changes in the export format.
+  To convert an existing distribution to the new format, use the following steps:
+  1. Create a site from the distribution using plone.distribution 1.0.x
+  2. Install plone.distribution 2.0.x
+  3. Delete the distribution's `contents/items` folder.
+  4. Export the distribution in the new format using the `bin/export-distribution` script.
+
+  @davisagli, @ericof #61
+
+
+### New features:
+
+- Default distribution: Allow users to upload a logo during site creation [@ericof] #66
+- Classic distribution: Allow users to upload a logo during site creation [@ericof] #67
+- Remove dependency on Plone package, add dependency on Products.CMFPlone [@ericof] #70
+
+
+### Bug fixes:
+
+- Get the name of the existing distribution from the report, not the answers [@ericof] #60
+- Fix issue with payload for new site creation breaking with certain plone.rest versions [@ericof] #71
+- Read profile.json by the pathlib.Path.read_text method to avoid the unclosed file exception [@folix-01] #75
+
+
+### Internal:
+
+- Update `plone/meta` configuration [@ericof] #73
+- Log traceback when creating a site fails [@pbauer] #82
+- Bump `plone.exportimport` to 1.0.0a5 [@ericof] #83
+
 ## 1.0.0b4 (2024-04-03)
 
 
 ### Bug fixes:
 
 - Fix exporting files.
   [pbauer] #58
```

### Comparing `plone.distribution-1.0.0b4/src/plone.distribution.egg-info/SOURCES.txt` & `plone_distribution-2.0.0a1/src/plone.distribution.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 CHANGES.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 constraints.txt
+dependabot.yml
 instance.yaml
 mx.ini
 pyproject.toml
 requirements-docs.txt
 requirements.txt
 setup.py
 tox.ini
@@ -59,39 +60,41 @@
 src/plone/distribution/browser/image.py
 src/plone/distribution/browser/overrides.zcml
 src/plone/distribution/browser/static/plone-logo.png
 src/plone/distribution/browser/static/plone-overview.min.css
 src/plone/distribution/browser/static/plone-overview.min.js
 src/plone/distribution/browser/static/plone.svg
 src/plone/distribution/browser/templates/plone-overview.pt
+src/plone/distribution/cli/__init__.py
 src/plone/distribution/distributions/classic/image.png
 src/plone/distribution/distributions/classic/profiles.json
 src/plone/distribution/distributions/classic/schema.json
-src/plone/distribution/distributions/classic/content/defaultpages.json
-src/plone/distribution/distributions/classic/content/ordering.json
+src/plone/distribution/distributions/classic/content/discussions.json
 src/plone/distribution/distributions/classic/content/portlets.json
-src/plone/distribution/distributions/classic/content/items/1.json
-src/plone/distribution/distributions/classic/content/items/2.json
-src/plone/distribution/distributions/classic/content/items/3.json
-src/plone/distribution/distributions/classic/content/items/4.json
-src/plone/distribution/distributions/classic/content/items/5.json
-src/plone/distribution/distributions/classic/content/items/6.json
+src/plone/distribution/distributions/classic/content/principals.json
+src/plone/distribution/distributions/classic/content/redirects.json
+src/plone/distribution/distributions/classic/content/relations.json
+src/plone/distribution/distributions/classic/content/translations.json
+src/plone/distribution/distributions/classic/content/content/__metadata__.json
+src/plone/distribution/distributions/classic/content/content/4053ffb6901342ac991afb54da15ab77/data.json
+src/plone/distribution/distributions/classic/content/content/54163be595184b4eb0a0b82a58b8def8/data.json
+src/plone/distribution/distributions/classic/content/content/61f6d382910945ea95f2e78a14ebb170/data.json
+src/plone/distribution/distributions/classic/content/content/ab584c1a6fae465da2283a0962f80114/data.json
+src/plone/distribution/distributions/classic/content/content/ee556c50736a4650839e2ada6dd65454/data.json
+src/plone/distribution/distributions/classic/content/content/plone_site_root/data.json
 src/plone/distribution/distributions/default/image.png
 src/plone/distribution/distributions/default/profiles.json
 src/plone/distribution/distributions/default/schema.json
-src/plone/distribution/distributions/default/content/items/1.json
-src/plone/distribution/exportimport/__init__.py
-src/plone/distribution/exportimport/configure.zcml
-src/plone/distribution/exportimport/dist_export.py
-src/plone/distribution/exportimport/dist_import.py
-src/plone/distribution/exportimport/helpers.py
-src/plone/distribution/exportimport/interfaces.py
-src/plone/distribution/exportimport/serializer.py
-src/plone/distribution/exportimport/templates/export_all.pt
-src/plone/distribution/exportimport/templates/import_all.pt
+src/plone/distribution/distributions/default/content/discussions.json
+src/plone/distribution/distributions/default/content/principals.json
+src/plone/distribution/distributions/default/content/redirects.json
+src/plone/distribution/distributions/default/content/relations.json
+src/plone/distribution/distributions/default/content/translations.json
+src/plone/distribution/distributions/default/content/content/__metadata__.json
+src/plone/distribution/distributions/default/content/content/plone_site_root/data.json
 src/plone/distribution/services/__init__.py
 src/plone/distribution/services/configure.zcml
 src/plone/distribution/services/overrides.zcml
 src/plone/distribution/services/auth/__init__.py
 src/plone/distribution/services/auth/configure.zcml
 src/plone/distribution/services/auth/login.py
 src/plone/distribution/services/sites/__init__.py
@@ -101,32 +104,32 @@
 src/plone/distribution/services/system/__init__.py
 src/plone/distribution/services/system/configure.zcml
 src/plone/distribution/services/system/get.py
 src/plone/distribution/testing/__init__.py
 src/plone/distribution/testing/layer.py
 src/plone/distribution/testing/testing.py
 src/plone/distribution/utils/__init__.py
+src/plone/distribution/utils/data.py
 src/plone/distribution/utils/request.py
 src/plone/distribution/utils/schema.py
 src/plone/distribution/utils/validation.py
 tests/__init__.py
 tests/conftest.py
 tests/api/test_api_distribution.py
 tests/api/test_api_site.py
 tests/distributions/__init__.py
 tests/distributions/conftest.py
 tests/distributions/test_distributions_classic.py
 tests/distributions/test_distributions_default.py
-tests/exportimport/portal.json
-tests/exportimport/test_exportimport_helpers.py
 tests/services/__init__.py
 tests/services/conftest.py
 tests/services/test_services_site.py
 tests/services/test_services_system.py
 tests/utils/__init__.py
 tests/utils/conftest.py
+tests/utils/test_utils_data.py
 tests/utils/test_utils_request.py
 tests/utils/test_utils_schema.py
 tests/utils/test_utils_validation.py
 tests/utils/data/invalid.json
 tests/utils/data/valid.json
 tests/utils/data/with_default_language.json
```

### Comparing `plone.distribution-1.0.0b4/tests/api/test_api_distribution.py` & `plone_distribution-2.0.0a1/tests/api/test_api_distribution.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/tests/api/test_api_site.py` & `plone_distribution-2.0.0a1/tests/api/test_api_site.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from plone import api
+from plone.distribution.api import distribution as dist_api
 from plone.distribution.api import site as site_api
 from Products.CMFPlone.Portal import PloneSite
 
 import pytest
 
 
 @pytest.fixture
@@ -54,13 +55,13 @@
         assert isinstance(site, PloneSite)
         assert site.title == new_site.title
 
     def test_get_creation_report_new_site(self, site):
         from datetime import datetime
         from plone.distribution.core import SiteCreationReport
 
-        report = site_api.get_creation_report(site)
+        report = dist_api.get_creation_report(site)
         assert isinstance(report, SiteCreationReport)
         assert report.name == "default"
         assert isinstance(report.date, datetime)
         assert isinstance(report.answers, dict)
         assert report.answers["title"] == site.title
```

### Comparing `plone.distribution-1.0.0b4/tests/distributions/test_distributions_classic.py` & `plone_distribution-2.0.0a1/tests/distributions/test_distributions_classic.py`

 * *Files 18% similar despite different names*

```diff
@@ -55,7 +55,11 @@
         assert content.portal_type == portal_type
         if review_state:
             assert api.content.get_state(content) == review_state
         else:
             with pytest.raises(WorkflowException) as exc:
                 api.content.get_state(content)
             assert "No workflow provides" in str(exc)
+
+    def test_plone_logo_applied(self, portal):
+        expected_result = b"filenameb64:dGVzdGU7ZGF0YTppbWFnZS9wbmc=;datab64:iVBORw0KGgoAAAANSUhEUgAAAAUAAAAFCAYAAACNbyblAAAAHElEQVQI12P4//8/w38GIAXDIBKE0DHxgljNBAAO9TXL0Y4OHwAAAABJRU5ErkJggg=="  # noQA
+        assert api.portal.get_registry_record("plone.site_logo") == expected_result
```

### Comparing `plone.distribution-1.0.0b4/tests/distributions/test_distributions_default.py` & `plone_distribution-2.0.0a1/tests/distributions/test_distributions_default.py`

 * *Files 25% similar despite different names*

```diff
@@ -32,14 +32,18 @@
             ("plonetheme.barceloneta", True),
             ("plone.volto", True),
         ],
     )
     def test_dependencies_installed(self, installer, package, expected):
         assert installer.is_product_installed(package) is expected
 
+    def test_plone_logo_applied(self, portal):
+        expected_result = b"filenameb64:dGVzdGU7ZGF0YTppbWFnZS9wbmc=;datab64:iVBORw0KGgoAAAANSUhEUgAAAAUAAAAFCAYAAACNbyblAAAAHElEQVQI12P4//8/w38GIAXDIBKE0DHxgljNBAAO9TXL0Y4OHwAAAABJRU5ErkJggg=="  # noQA
+        assert api.portal.get_registry_record("plone.site_logo") == expected_result
+
     @pytest.mark.parametrize(
         "path,title,portal_type,review_state",
         [
             ("/", "Plone Site", "Plone Site", ""),
         ],
     )
     def test_content_created(self, portal, path, title, portal_type, review_state):
```

### Comparing `plone.distribution-1.0.0b4/tests/services/test_services_system.py` & `plone_distribution-2.0.0a1/tests/services/test_services_system.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from plone.app.testing import SITE_OWNER_NAME
 from plone.app.testing import SITE_OWNER_PASSWORD
-from plone.distribution.api.site import SITE_REPORT_ANNO
+from plone.distribution.api.distribution import SITE_REPORT_ANNO
 from plone.restapi.testing import RelativeSession
 from zope.annotation.interfaces import IAnnotations
 
 import pytest
 
 
 @pytest.fixture
```

### Comparing `plone.distribution-1.0.0b4/tests/utils/conftest.py` & `plone_distribution-2.0.0a1/tests/utils/conftest.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/tests/utils/data/invalid.json` & `plone_distribution-2.0.0a1/tests/utils/data/invalid.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/tests/utils/data/valid.json` & `plone_distribution-2.0.0a1/tests/utils/data/with_default_language.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9979166666666667%*

 * *Differences: {"'schema'": "{'properties': {'default_language': {replace: OrderedDict([('type', 'string'), "*

 * *             "('title', 'Default language'), ('default', 'es')])}}}"}*

```diff
@@ -1,13 +1,15 @@
 {
     "schema": {
         "description": "Adds a new Plone content management system site to the underlying application server.",
         "properties": {
             "default_language": {
-                "$ref": "#/definitions/languages"
+                "default": "es",
+                "title": "Default language",
+                "type": "string"
             },
             "description": {
                 "default": "A Plone Site",
                 "title": "Site Description",
                 "type": "string"
             },
             "portal_timezone": {
```

### Comparing `plone.distribution-1.0.0b4/tests/utils/data/with_default_language.json` & `plone_distribution-2.0.0a1/src/plone/distribution/distributions/default/schema.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9946428571428572%*

 * *Differences: {"'schema'": "{'properties': {'default_language': {replace: OrderedDict([('$ref', "*

 * *             "'#/definitions/languages')])}, 'site_logo': OrderedDict([('type', 'string'), "*

 * *             "('format', 'data-url'), ('title', 'Site logo')])}}"}*

```diff
@@ -1,15 +1,13 @@
 {
     "schema": {
         "description": "Adds a new Plone content management system site to the underlying application server.",
         "properties": {
             "default_language": {
-                "default": "es",
-                "title": "Default language",
-                "type": "string"
+                "$ref": "#/definitions/languages"
             },
             "description": {
                 "default": "A Plone Site",
                 "title": "Site Description",
                 "type": "string"
             },
             "portal_timezone": {
@@ -23,14 +21,19 @@
             },
             "site_id": {
                 "default": "Plone",
                 "description": "The ID of the site. No special characters or spaces are allowed. This ends up as part of the URL unless hidden by an upstream web server.",
                 "title": "Path Identifier",
                 "type": "string"
             },
+            "site_logo": {
+                "format": "data-url",
+                "title": "Site logo",
+                "type": "string"
+            },
             "title": {
                 "default": "Site",
                 "description": "A short title for the site. This will be shown as part of the title of the browser window on each page.",
                 "title": "Title",
                 "type": "string"
             }
         },
```

### Comparing `plone.distribution-1.0.0b4/tests/utils/test_utils_request.py` & `plone_distribution-2.0.0a1/tests/utils/test_utils_request.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/tests/utils/test_utils_schema.py` & `plone_distribution-2.0.0a1/tests/utils/test_utils_schema.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/tests/utils/test_utils_validation.py` & `plone_distribution-2.0.0a1/tests/utils/test_utils_validation.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b4/tox.ini` & `plone_distribution-2.0.0a1/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -146,21 +146,28 @@
 #  test_environment_variables = """
 #      PIP_EXTRA_INDEX_URL=https://my-pypi.my-server.com/
 #  """
 #
 # Set constrain_package_deps .meta.toml:
 #  [tox]
 #  constrain_package_deps = "false"
+#
+# Explicitly set the package name .meta.toml:
+#  (For cases where the repository name is not the same of
+#   the package name)
+#  [tox]
+#  package_name = "pytest_plone"
+#
 ##
 deps =
     pytest-plone
     pytest
     coverage
     -c constraints-mxdev.txt
-    
+
 commands =
     coverage run --source plone.distribution -m pytest  {posargs} --disable-warnings {toxinidir}/tests
     coverage report -m --format markdown
     coverage xml
 extras =
     test
 
@@ -169,27 +176,30 @@
 description = ensure that the distribution is ready to release
 skip_install = true
 deps =
     twine
     build
     towncrier
     -c constraints-mxdev.txt
-    
+
 commands =
     # fake version to not have to install the package
     # we build the change log as news entries might break
     # the README that is displayed on PyPI
     towncrier build --version=100.0.0 --yes
     python -m build --sdist
     twine check dist/*
 
 [testenv:circular]
 description = ensure there are no cyclic dependencies
 use_develop = true
 skip_install = false
+# Here we must always constrain the package deps to what is already installed,
+# otherwise we simply get the latest from PyPI, which may not work.
+constrain_package_deps = true
 set_env =
 
 ##
 # Specify extra test environment variables in .meta.toml:
 #  [tox]
 #  test_environment_variables = """
 #      PIP_EXTRA_INDEX_URL=https://my-pypi.my-server.com/
@@ -197,15 +207,15 @@
 ##
 allowlist_externals =
     sh
 deps =
     pipdeptree
     pipforester
     -c constraints-mxdev.txt
-    
+
 commands =
     # Generate the full dependency tree
     sh -c 'pipdeptree -j > forest.json'
     # Generate a DOT graph with the circular dependencies, if any
     pipforester -i forest.json -o forest.dot --cycles
     # Report if there are any circular dependencies, i.e. error if there are any
     pipforester -i forest.json --check-cycles -o /dev/null
```

