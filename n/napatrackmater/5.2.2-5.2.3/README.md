# Comparing `tmp/napatrackmater-5.2.2.tar.gz` & `tmp/napatrackmater-5.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napatrackmater-5.2.2.tar", last modified: Sun May 12 11:46:40 2024, max compression
+gzip compressed data, was "napatrackmater-5.2.3.tar", last modified: Fri May 17 15:00:47 2024, max compression
```

## Comparing `napatrackmater-5.2.2.tar` & `napatrackmater-5.2.3.tar`

### file list

```diff
@@ -1,281 +1,281 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.290998 napatrackmater-5.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.238998 napatrackmater-5.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.254998 napatrackmater-5.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/MASTER.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.254998 napatrackmater-5.2.2/Notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/Notebooks/Track_vector.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-12 11:46:40.290998 napatrackmater-5.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.250998 napatrackmater-5.2.2/_build/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.254998 napatrackmater-5.2.2/_build/.doctrees/
--rw-r--r--   0 runner    (1001) docker     (127)    33531 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/.doctrees/MASTER.doctree
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.254998 napatrackmater-5.2.2/_build/.doctrees/Notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    29083 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/.doctrees/Notebooks/Track_vector.doctree
--rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/.doctrees/README.doctree
--rw-r--r--   0 runner    (1001) docker     (127)    36454 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/.doctrees/environment.pickle
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.258998 napatrackmater-5.2.2/_build/html/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/.buildinfo
--rw-r--r--   0 runner    (1001) docker     (127)    29915 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/MASTER.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.258998 napatrackmater-5.2.2/_build/html/Notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    66062 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/Notebooks/Track_vector.html
--rw-r--r--   0 runner    (1001) docker     (127)    18885 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/README.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.258998 napatrackmater-5.2.2/_build/html/_images/
--rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_images/ClusterDistributionPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_images/ClusterNearnessPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)   162373 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_images/ClusterPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    61613 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_images/FeatureMatrixPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    66872 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_images/QuadrantDistributionPlot_time_point_97.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.258998 napatrackmater-5.2.2/_build/html/_sources/
--rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_sources/MASTER.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.258998 napatrackmater-5.2.2/_build/html/_sources/Notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_sources/Notebooks/Track_vector.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_sources/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.262998 napatrackmater-5.2.2/_build/html/_sphinx_design_static/
--rw-r--r--   0 runner    (1001) docker     (127)    48417 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_sphinx_design_static/design-style.4045f2051d55cab465a707391d5b2007.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_sphinx_design_static/design-tabs.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.266998 napatrackmater-5.2.2/_build/html/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    14692 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/check-solid.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/clipboard.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/copy-button.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/copybutton.css
--rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/copybutton.js
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/copybutton_funcs.js
--rw-r--r--   0 runner    (1001) docker     (127)    48417 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/design-style.4045f2051d55cab465a707391d5b2007.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/design-tabs.js
--rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/file.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.266998 napatrackmater-5.2.2/_build/html/_static/images/
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/images/logo_binder.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/images/logo_colab.png
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/images/logo_deepnote.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/images/logo_jupyterhub.svg
--rw-r--r--   0 runner    (1001) docker     (127)   287630 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/jquery-3.5.1.js
--rw-r--r--   0 runner    (1001) docker     (127)    89476 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/jquery.js
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/kapoorlablogo.png
--rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/language_data.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.250998 napatrackmater-5.2.2/_build/html/_static/locales/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.242998 napatrackmater-5.2.2/_build/html/_static/locales/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.266998 napatrackmater-5.2.2/_build/html/_static/locales/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.242998 napatrackmater-5.2.2/_build/html/_static/locales/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.266998 napatrackmater-5.2.2/_build/html/_static/locales/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.242998 napatrackmater-5.2.2/_build/html/_static/locales/bn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.266998 napatrackmater-5.2.2/_build/html/_static/locales/bn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.242998 napatrackmater-5.2.2/_build/html/_static/locales/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.266998 napatrackmater-5.2.2/_build/html/_static/locales/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.242998 napatrackmater-5.2.2/_build/html/_static/locales/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.270998 napatrackmater-5.2.2/_build/html/_static/locales/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.242998 napatrackmater-5.2.2/_build/html/_static/locales/da/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.270998 napatrackmater-5.2.2/_build/html/_static/locales/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/da/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.242998 napatrackmater-5.2.2/_build/html/_static/locales/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.270998 napatrackmater-5.2.2/_build/html/_static/locales/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/de/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.242998 napatrackmater-5.2.2/_build/html/_static/locales/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.270998 napatrackmater-5.2.2/_build/html/_static/locales/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/el/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.242998 napatrackmater-5.2.2/_build/html/_static/locales/eo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.270998 napatrackmater-5.2.2/_build/html/_static/locales/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.242998 napatrackmater-5.2.2/_build/html/_static/locales/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.270998 napatrackmater-5.2.2/_build/html/_static/locales/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/es/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.242998 napatrackmater-5.2.2/_build/html/_static/locales/et/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.270998 napatrackmater-5.2.2/_build/html/_static/locales/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/et/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.242998 napatrackmater-5.2.2/_build/html/_static/locales/fi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.270998 napatrackmater-5.2.2/_build/html/_static/locales/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.242998 napatrackmater-5.2.2/_build/html/_static/locales/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.270998 napatrackmater-5.2.2/_build/html/_static/locales/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.242998 napatrackmater-5.2.2/_build/html/_static/locales/hr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.270998 napatrackmater-5.2.2/_build/html/_static/locales/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.242998 napatrackmater-5.2.2/_build/html/_static/locales/id/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.270998 napatrackmater-5.2.2/_build/html/_static/locales/id/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/id/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.242998 napatrackmater-5.2.2/_build/html/_static/locales/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.270998 napatrackmater-5.2.2/_build/html/_static/locales/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/it/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.246998 napatrackmater-5.2.2/_build/html/_static/locales/iw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.270998 napatrackmater-5.2.2/_build/html/_static/locales/iw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.246998 napatrackmater-5.2.2/_build/html/_static/locales/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.270998 napatrackmater-5.2.2/_build/html/_static/locales/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.246998 napatrackmater-5.2.2/_build/html/_static/locales/ko/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.270998 napatrackmater-5.2.2/_build/html/_static/locales/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.246998 napatrackmater-5.2.2/_build/html/_static/locales/lt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.270998 napatrackmater-5.2.2/_build/html/_static/locales/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.246998 napatrackmater-5.2.2/_build/html/_static/locales/lv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.270998 napatrackmater-5.2.2/_build/html/_static/locales/lv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.246998 napatrackmater-5.2.2/_build/html/_static/locales/ml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.270998 napatrackmater-5.2.2/_build/html/_static/locales/ml/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.246998 napatrackmater-5.2.2/_build/html/_static/locales/mr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.270998 napatrackmater-5.2.2/_build/html/_static/locales/mr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.246998 napatrackmater-5.2.2/_build/html/_static/locales/ms/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.270998 napatrackmater-5.2.2/_build/html/_static/locales/ms/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.246998 napatrackmater-5.2.2/_build/html/_static/locales/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.270998 napatrackmater-5.2.2/_build/html/_static/locales/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.246998 napatrackmater-5.2.2/_build/html/_static/locales/no/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.270998 napatrackmater-5.2.2/_build/html/_static/locales/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/no/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.246998 napatrackmater-5.2.2/_build/html/_static/locales/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.274998 napatrackmater-5.2.2/_build/html/_static/locales/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.246998 napatrackmater-5.2.2/_build/html/_static/locales/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.274998 napatrackmater-5.2.2/_build/html/_static/locales/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.246998 napatrackmater-5.2.2/_build/html/_static/locales/ro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.274998 napatrackmater-5.2.2/_build/html/_static/locales/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.246998 napatrackmater-5.2.2/_build/html/_static/locales/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.274998 napatrackmater-5.2.2/_build/html/_static/locales/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.246998 napatrackmater-5.2.2/_build/html/_static/locales/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.274998 napatrackmater-5.2.2/_build/html/_static/locales/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.246998 napatrackmater-5.2.2/_build/html/_static/locales/sl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.274998 napatrackmater-5.2.2/_build/html/_static/locales/sl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.246998 napatrackmater-5.2.2/_build/html/_static/locales/sr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.274998 napatrackmater-5.2.2/_build/html/_static/locales/sr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.246998 napatrackmater-5.2.2/_build/html/_static/locales/sv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.274998 napatrackmater-5.2.2/_build/html/_static/locales/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.250998 napatrackmater-5.2.2/_build/html/_static/locales/ta/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.274998 napatrackmater-5.2.2/_build/html/_static/locales/ta/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.250998 napatrackmater-5.2.2/_build/html/_static/locales/te/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.274998 napatrackmater-5.2.2/_build/html/_static/locales/te/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/te/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.250998 napatrackmater-5.2.2/_build/html/_static/locales/tg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.274998 napatrackmater-5.2.2/_build/html/_static/locales/tg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.250998 napatrackmater-5.2.2/_build/html/_static/locales/th/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.274998 napatrackmater-5.2.2/_build/html/_static/locales/th/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/th/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.250998 napatrackmater-5.2.2/_build/html/_static/locales/tl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.274998 napatrackmater-5.2.2/_build/html/_static/locales/tl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.250998 napatrackmater-5.2.2/_build/html/_static/locales/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.274998 napatrackmater-5.2.2/_build/html/_static/locales/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.250998 napatrackmater-5.2.2/_build/html/_static/locales/uk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.274998 napatrackmater-5.2.2/_build/html/_static/locales/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.250998 napatrackmater-5.2.2/_build/html/_static/locales/ur/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.274998 napatrackmater-5.2.2/_build/html/_static/locales/ur/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.250998 napatrackmater-5.2.2/_build/html/_static/locales/vi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.274998 napatrackmater-5.2.2/_build/html/_static/locales/vi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.250998 napatrackmater-5.2.2/_build/html/_static/locales/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.274998 napatrackmater-5.2.2/_build/html/_static/locales/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.250998 napatrackmater-5.2.2/_build/html/_static/locales/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.274998 napatrackmater-5.2.2/_build/html/_static/locales/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (127)    39364 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)    12757 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/sbt-webpack-macros.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.278998 napatrackmater-5.2.2/_build/html/_static/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)    80813 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/scripts/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/scripts/bootstrap.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   335757 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/scripts/bootstrap.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/scripts/pydata-sphinx-theme.js
--rw-r--r--   0 runner    (1001) docker     (127)    19648 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/scripts/pydata-sphinx-theme.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/scripts/sphinx-book-theme.js
--rw-r--r--   0 runner    (1001) docker     (127)    13066 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/scripts/sphinx-book-theme.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    16634 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/sphinx-thebe.css
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/sphinx-thebe.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.278998 napatrackmater-5.2.2/_build/html/_static/styles/
--rw-r--r--   0 runner    (1001) docker     (127)   176654 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/styles/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)    63341 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/styles/pydata-sphinx-theme.css
--rw-r--r--   0 runner    (1001) docker     (127)    13841 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/styles/sphinx-book-theme.css
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/styles/theme.css
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/togglebutton.css
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/togglebutton.js
--rw-r--r--   0 runner    (1001) docker     (127)    68420 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/underscore.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.250998 napatrackmater-5.2.2/_build/html/_static/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.250998 napatrackmater-5.2.2/_build/html/_static/vendor/fontawesome/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.278998 napatrackmater-5.2.2/_build/html/_static/vendor/fontawesome/6.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.278998 napatrackmater-5.2.2/_build/html/_static/vendor/fontawesome/6.1.2/css/
--rw-r--r--   0 runner    (1001) docker     (127)   101691 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.282998 napatrackmater-5.2.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/
--rw-r--r--   0 runner    (1001) docker     (127)   181264 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   105112 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    60236 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    24028 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   389948 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   154840 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/_static/webpack-macros.html
--rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/genindex.html
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/objects.inv
--rw-r--r--   0 runner    (1001) docker     (127)    12010 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/search.html
--rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/html/searchindex.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.250998 napatrackmater-5.2.2/_build/jupyter_execute/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.282998 napatrackmater-5.2.2/_build/jupyter_execute/Notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    17500 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_build/jupyter_execute/Notebooks/Track_vector.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/_toc.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.286998 napatrackmater-5.2.2/images/
--rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/images/ClusterDistributionPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/images/ClusterNearnessPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)   162373 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/images/ClusterPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    61613 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/images/FeatureMatrixPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    66872 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/images/QuadrantDistributionPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/images/kapoorlablogo.png
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/images/kapoorlogo.png
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-12 11:46:40.290998 napatrackmater-5.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.250998 napatrackmater-5.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.286998 napatrackmater-5.2.2/src/napatrackmater/
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/src/napatrackmater/CloudAutoEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/src/napatrackmater/DeepEmbeddedClustering.py
--rw-r--r--   0 runner    (1001) docker     (127)   145682 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/src/napatrackmater/Trackmate.py
--rw-r--r--   0 runner    (1001) docker     (127)   141873 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/src/napatrackmater/Trackvector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/src/napatrackmater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/src/napatrackmater/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    24585 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/src/napatrackmater/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/src/napatrackmater/fast_radius_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    13035 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/src/napatrackmater/fate_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     6603 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/src/napatrackmater/pretrained.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:46:40.286998 napatrackmater-5.2.2/src/napatrackmater.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-12 11:46:40.000000 napatrackmater-5.2.2/src/napatrackmater.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-12 11:46:40.000000 napatrackmater-5.2.2/src/napatrackmater.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 11:46:40.000000 napatrackmater-5.2.2/src/napatrackmater.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-12 11:46:40.000000 napatrackmater-5.2.2/src/napatrackmater.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-12 11:46:40.000000 napatrackmater-5.2.2/src/napatrackmater.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-12 11:46:29.000000 napatrackmater-5.2.2/update_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.778747 napatrackmater-5.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.734747 napatrackmater-5.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.750747 napatrackmater-5.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/MASTER.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.750747 napatrackmater-5.2.3/Notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/Notebooks/Track_vector.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-17 15:00:47.778747 napatrackmater-5.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.746747 napatrackmater-5.2.3/_build/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.750747 napatrackmater-5.2.3/_build/.doctrees/
+-rw-r--r--   0 runner    (1001) docker     (127)    33531 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/.doctrees/MASTER.doctree
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.750747 napatrackmater-5.2.3/_build/.doctrees/Notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    29083 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/.doctrees/Notebooks/Track_vector.doctree
+-rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/.doctrees/README.doctree
+-rw-r--r--   0 runner    (1001) docker     (127)    36454 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/.doctrees/environment.pickle
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.750747 napatrackmater-5.2.3/_build/html/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/.buildinfo
+-rw-r--r--   0 runner    (1001) docker     (127)    29915 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/MASTER.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.750747 napatrackmater-5.2.3/_build/html/Notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    66062 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/Notebooks/Track_vector.html
+-rw-r--r--   0 runner    (1001) docker     (127)    18885 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/README.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.750747 napatrackmater-5.2.3/_build/html/_images/
+-rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_images/ClusterDistributionPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_images/ClusterNearnessPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)   162373 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_images/ClusterPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61613 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_images/FeatureMatrixPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66872 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_images/QuadrantDistributionPlot_time_point_97.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.754747 napatrackmater-5.2.3/_build/html/_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_sources/MASTER.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.754747 napatrackmater-5.2.3/_build/html/_sources/Notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_sources/Notebooks/Track_vector.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_sources/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.754747 napatrackmater-5.2.3/_build/html/_sphinx_design_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    48417 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_sphinx_design_static/design-style.4045f2051d55cab465a707391d5b2007.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_sphinx_design_static/design-tabs.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.758747 napatrackmater-5.2.3/_build/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    14692 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/basic.css
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/check-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/clipboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/copy-button.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/copybutton.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/copybutton.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/copybutton_funcs.js
+-rw-r--r--   0 runner    (1001) docker     (127)    48417 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/design-style.4045f2051d55cab465a707391d5b2007.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/design-tabs.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/file.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.758747 napatrackmater-5.2.3/_build/html/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/images/logo_binder.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/images/logo_colab.png
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/images/logo_deepnote.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/images/logo_jupyterhub.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   287630 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/jquery-3.5.1.js
+-rw-r--r--   0 runner    (1001) docker     (127)    89476 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/kapoorlablogo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/language_data.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.746747 napatrackmater-5.2.3/_build/html/_static/locales/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.738747 napatrackmater-5.2.3/_build/html/_static/locales/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.758747 napatrackmater-5.2.3/_build/html/_static/locales/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.738747 napatrackmater-5.2.3/_build/html/_static/locales/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.758747 napatrackmater-5.2.3/_build/html/_static/locales/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.738747 napatrackmater-5.2.3/_build/html/_static/locales/bn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.758747 napatrackmater-5.2.3/_build/html/_static/locales/bn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.738747 napatrackmater-5.2.3/_build/html/_static/locales/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.758747 napatrackmater-5.2.3/_build/html/_static/locales/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.738747 napatrackmater-5.2.3/_build/html/_static/locales/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.758747 napatrackmater-5.2.3/_build/html/_static/locales/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.738747 napatrackmater-5.2.3/_build/html/_static/locales/da/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.758747 napatrackmater-5.2.3/_build/html/_static/locales/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/da/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.738747 napatrackmater-5.2.3/_build/html/_static/locales/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.762747 napatrackmater-5.2.3/_build/html/_static/locales/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/de/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.738747 napatrackmater-5.2.3/_build/html/_static/locales/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.762747 napatrackmater-5.2.3/_build/html/_static/locales/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/el/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.738747 napatrackmater-5.2.3/_build/html/_static/locales/eo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.762747 napatrackmater-5.2.3/_build/html/_static/locales/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.738747 napatrackmater-5.2.3/_build/html/_static/locales/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.762747 napatrackmater-5.2.3/_build/html/_static/locales/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/es/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.738747 napatrackmater-5.2.3/_build/html/_static/locales/et/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.762747 napatrackmater-5.2.3/_build/html/_static/locales/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/et/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.738747 napatrackmater-5.2.3/_build/html/_static/locales/fi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.762747 napatrackmater-5.2.3/_build/html/_static/locales/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.738747 napatrackmater-5.2.3/_build/html/_static/locales/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.762747 napatrackmater-5.2.3/_build/html/_static/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.738747 napatrackmater-5.2.3/_build/html/_static/locales/hr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.762747 napatrackmater-5.2.3/_build/html/_static/locales/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.738747 napatrackmater-5.2.3/_build/html/_static/locales/id/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.762747 napatrackmater-5.2.3/_build/html/_static/locales/id/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/id/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.738747 napatrackmater-5.2.3/_build/html/_static/locales/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.762747 napatrackmater-5.2.3/_build/html/_static/locales/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/it/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.738747 napatrackmater-5.2.3/_build/html/_static/locales/iw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.762747 napatrackmater-5.2.3/_build/html/_static/locales/iw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.738747 napatrackmater-5.2.3/_build/html/_static/locales/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.762747 napatrackmater-5.2.3/_build/html/_static/locales/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.738747 napatrackmater-5.2.3/_build/html/_static/locales/ko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.762747 napatrackmater-5.2.3/_build/html/_static/locales/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.738747 napatrackmater-5.2.3/_build/html/_static/locales/lt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.762747 napatrackmater-5.2.3/_build/html/_static/locales/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.742747 napatrackmater-5.2.3/_build/html/_static/locales/lv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.762747 napatrackmater-5.2.3/_build/html/_static/locales/lv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.742747 napatrackmater-5.2.3/_build/html/_static/locales/ml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.762747 napatrackmater-5.2.3/_build/html/_static/locales/ml/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.742747 napatrackmater-5.2.3/_build/html/_static/locales/mr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.762747 napatrackmater-5.2.3/_build/html/_static/locales/mr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.742747 napatrackmater-5.2.3/_build/html/_static/locales/ms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.762747 napatrackmater-5.2.3/_build/html/_static/locales/ms/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.742747 napatrackmater-5.2.3/_build/html/_static/locales/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.762747 napatrackmater-5.2.3/_build/html/_static/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.742747 napatrackmater-5.2.3/_build/html/_static/locales/no/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.762747 napatrackmater-5.2.3/_build/html/_static/locales/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/no/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.742747 napatrackmater-5.2.3/_build/html/_static/locales/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.762747 napatrackmater-5.2.3/_build/html/_static/locales/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.742747 napatrackmater-5.2.3/_build/html/_static/locales/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.762747 napatrackmater-5.2.3/_build/html/_static/locales/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.742747 napatrackmater-5.2.3/_build/html/_static/locales/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.762747 napatrackmater-5.2.3/_build/html/_static/locales/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.742747 napatrackmater-5.2.3/_build/html/_static/locales/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.766747 napatrackmater-5.2.3/_build/html/_static/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.742747 napatrackmater-5.2.3/_build/html/_static/locales/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.766747 napatrackmater-5.2.3/_build/html/_static/locales/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.742747 napatrackmater-5.2.3/_build/html/_static/locales/sl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.766747 napatrackmater-5.2.3/_build/html/_static/locales/sl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.742747 napatrackmater-5.2.3/_build/html/_static/locales/sr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.766747 napatrackmater-5.2.3/_build/html/_static/locales/sr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.742747 napatrackmater-5.2.3/_build/html/_static/locales/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.766747 napatrackmater-5.2.3/_build/html/_static/locales/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.742747 napatrackmater-5.2.3/_build/html/_static/locales/ta/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.766747 napatrackmater-5.2.3/_build/html/_static/locales/ta/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.742747 napatrackmater-5.2.3/_build/html/_static/locales/te/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.766747 napatrackmater-5.2.3/_build/html/_static/locales/te/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/te/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.742747 napatrackmater-5.2.3/_build/html/_static/locales/tg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.766747 napatrackmater-5.2.3/_build/html/_static/locales/tg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.742747 napatrackmater-5.2.3/_build/html/_static/locales/th/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.766747 napatrackmater-5.2.3/_build/html/_static/locales/th/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/th/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.742747 napatrackmater-5.2.3/_build/html/_static/locales/tl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.766747 napatrackmater-5.2.3/_build/html/_static/locales/tl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.742747 napatrackmater-5.2.3/_build/html/_static/locales/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.766747 napatrackmater-5.2.3/_build/html/_static/locales/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.742747 napatrackmater-5.2.3/_build/html/_static/locales/uk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.766747 napatrackmater-5.2.3/_build/html/_static/locales/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.746747 napatrackmater-5.2.3/_build/html/_static/locales/ur/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.766747 napatrackmater-5.2.3/_build/html/_static/locales/ur/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.746747 napatrackmater-5.2.3/_build/html/_static/locales/vi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.766747 napatrackmater-5.2.3/_build/html/_static/locales/vi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.746747 napatrackmater-5.2.3/_build/html/_static/locales/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.766747 napatrackmater-5.2.3/_build/html/_static/locales/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.746747 napatrackmater-5.2.3/_build/html/_static/locales/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.766747 napatrackmater-5.2.3/_build/html/_static/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)    39364 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12757 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/sbt-webpack-macros.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.770747 napatrackmater-5.2.3/_build/html/_static/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)    80813 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/scripts/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/scripts/bootstrap.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   335757 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/scripts/bootstrap.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/scripts/pydata-sphinx-theme.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19648 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/scripts/pydata-sphinx-theme.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/scripts/sphinx-book-theme.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13066 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/scripts/sphinx-book-theme.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    16634 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/sphinx-thebe.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/sphinx-thebe.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.770747 napatrackmater-5.2.3/_build/html/_static/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)   176654 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/styles/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)    63341 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/styles/pydata-sphinx-theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)    13841 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/styles/sphinx-book-theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/styles/theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/togglebutton.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/togglebutton.js
+-rw-r--r--   0 runner    (1001) docker     (127)    68420 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/underscore.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.746747 napatrackmater-5.2.3/_build/html/_static/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.746747 napatrackmater-5.2.3/_build/html/_static/vendor/fontawesome/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.770747 napatrackmater-5.2.3/_build/html/_static/vendor/fontawesome/6.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.770747 napatrackmater-5.2.3/_build/html/_static/vendor/fontawesome/6.1.2/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   101691 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.774747 napatrackmater-5.2.3/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   181264 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   105112 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    60236 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    24028 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   389948 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   154840 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/_static/webpack-macros.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (127)    12010 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/html/searchindex.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.746747 napatrackmater-5.2.3/_build/jupyter_execute/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.774747 napatrackmater-5.2.3/_build/jupyter_execute/Notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    17500 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_build/jupyter_execute/Notebooks/Track_vector.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/_toc.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.774747 napatrackmater-5.2.3/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/images/ClusterDistributionPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/images/ClusterNearnessPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)   162373 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/images/ClusterPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61613 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/images/FeatureMatrixPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66872 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/images/QuadrantDistributionPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/images/kapoorlablogo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/images/kapoorlogo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-17 15:00:47.778747 napatrackmater-5.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.746747 napatrackmater-5.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.774747 napatrackmater-5.2.3/src/napatrackmater/
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/src/napatrackmater/CloudAutoEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/src/napatrackmater/DeepEmbeddedClustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)   145682 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/src/napatrackmater/Trackmate.py
+-rw-r--r--   0 runner    (1001) docker     (127)   125528 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/src/napatrackmater/Trackvector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/src/napatrackmater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/src/napatrackmater/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24585 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/src/napatrackmater/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/src/napatrackmater/fast_radius_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13035 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/src/napatrackmater/fate_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6603 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/src/napatrackmater/pretrained.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:47.778747 napatrackmater-5.2.3/src/napatrackmater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-17 15:00:47.000000 napatrackmater-5.2.3/src/napatrackmater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-17 15:00:47.000000 napatrackmater-5.2.3/src/napatrackmater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 15:00:47.000000 napatrackmater-5.2.3/src/napatrackmater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-17 15:00:47.000000 napatrackmater-5.2.3/src/napatrackmater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-17 15:00:47.000000 napatrackmater-5.2.3/src/napatrackmater.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-17 15:00:36.000000 napatrackmater-5.2.3/update_version.py
```

### Comparing `napatrackmater-5.2.2/.github/workflows/deploy.yml` & `napatrackmater-5.2.3/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/.github/workflows/test_and_deploy.yml` & `napatrackmater-5.2.3/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/.gitignore` & `napatrackmater-5.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/.pre-commit-config.yaml` & `napatrackmater-5.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/.travis.yml` & `napatrackmater-5.2.3/.travis.yml`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/Dockerfile` & `napatrackmater-5.2.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/LICENSE` & `napatrackmater-5.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/MASTER.md` & `napatrackmater-5.2.3/MASTER.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/Notebooks/Track_vector.ipynb` & `napatrackmater-5.2.3/Notebooks/Track_vector.ipynb`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/PKG-INFO` & `napatrackmater-5.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 5.2.2
+Version: 5.2.3
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/Kapoorlabs-CAPED/napatrackmater
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/napatrackmater/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/napatrackmater#README.md
```

### Comparing `napatrackmater-5.2.2/README.md` & `napatrackmater-5.2.3/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/.doctrees/MASTER.doctree` & `napatrackmater-5.2.3/_build/.doctrees/MASTER.doctree`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/.doctrees/Notebooks/Track_vector.doctree` & `napatrackmater-5.2.3/_build/.doctrees/Notebooks/Track_vector.doctree`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/.doctrees/README.doctree` & `napatrackmater-5.2.3/_build/.doctrees/README.doctree`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/.doctrees/environment.pickle` & `napatrackmater-5.2.3/_build/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/MASTER.html` & `napatrackmater-5.2.3/_build/html/MASTER.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/Notebooks/Track_vector.html` & `napatrackmater-5.2.3/_build/html/Notebooks/Track_vector.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/README.html` & `napatrackmater-5.2.3/_build/html/README.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_images/ClusterDistributionPlot_time_point_97.png` & `napatrackmater-5.2.3/_build/html/_images/ClusterDistributionPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_images/ClusterNearnessPlot_time_point_97.png` & `napatrackmater-5.2.3/_build/html/_images/ClusterNearnessPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_images/ClusterPlot_time_point_97.png` & `napatrackmater-5.2.3/_build/html/_images/ClusterPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_images/FeatureMatrixPlot_time_point_97.png` & `napatrackmater-5.2.3/_build/html/_images/FeatureMatrixPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_images/QuadrantDistributionPlot_time_point_97.png` & `napatrackmater-5.2.3/_build/html/_images/QuadrantDistributionPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_sources/MASTER.md` & `napatrackmater-5.2.3/_build/html/_sources/MASTER.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_sources/Notebooks/Track_vector.ipynb` & `napatrackmater-5.2.3/_build/html/_sources/Notebooks/Track_vector.ipynb`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_sources/README.md` & `napatrackmater-5.2.3/_build/html/_sources/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_sphinx_design_static/design-style.4045f2051d55cab465a707391d5b2007.min.css` & `napatrackmater-5.2.3/_build/html/_sphinx_design_static/design-style.4045f2051d55cab465a707391d5b2007.min.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_sphinx_design_static/design-tabs.js` & `napatrackmater-5.2.3/_build/html/_sphinx_design_static/design-tabs.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/basic.css` & `napatrackmater-5.2.3/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/clipboard.min.js` & `napatrackmater-5.2.3/_build/html/_static/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/copybutton.css` & `napatrackmater-5.2.3/_build/html/_static/copybutton.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/copybutton.js` & `napatrackmater-5.2.3/_build/html/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/copybutton_funcs.js` & `napatrackmater-5.2.3/_build/html/_static/copybutton_funcs.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/design-style.4045f2051d55cab465a707391d5b2007.min.css` & `napatrackmater-5.2.3/_build/html/_static/design-style.4045f2051d55cab465a707391d5b2007.min.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/design-tabs.js` & `napatrackmater-5.2.3/_build/html/_static/design-tabs.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/doctools.js` & `napatrackmater-5.2.3/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/images/logo_binder.svg` & `napatrackmater-5.2.3/_build/html/_static/images/logo_binder.svg`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/images/logo_colab.png` & `napatrackmater-5.2.3/_build/html/_static/images/logo_colab.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/images/logo_deepnote.svg` & `napatrackmater-5.2.3/_build/html/_static/images/logo_deepnote.svg`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/images/logo_jupyterhub.svg` & `napatrackmater-5.2.3/_build/html/_static/images/logo_jupyterhub.svg`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/jquery-3.5.1.js` & `napatrackmater-5.2.3/_build/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/jquery.js` & `napatrackmater-5.2.3/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/kapoorlablogo.png` & `napatrackmater-5.2.3/_build/html/_static/kapoorlablogo.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/language_data.js` & `napatrackmater-5.2.3/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/ar/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/ar/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/bg/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/bg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/bn/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/bn/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/ca/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/ca/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/cs/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/cs/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/da/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/da/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/de/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/de/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/el/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/el/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/eo/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/eo/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/es/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/es/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/et/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/et/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/fi/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/fi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/fr/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/fr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/hr/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/hr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/id/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/id/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/it/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/it/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/iw/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/iw/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/ja/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/ja/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/ko/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/ko/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/lt/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/lt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/lv/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/lv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/ml/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/ml/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/mr/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/mr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/ms/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/ms/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/nl/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/nl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/no/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/no/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/pl/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/pl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/pt/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/pt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/ro/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/ro/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/ru/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/ru/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/sk/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/sk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/sl/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/sl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/sr/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/sr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/sv/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/sv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/ta/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/ta/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/te/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/te/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/tg/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/tg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/th/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/th/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/tl/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/tl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/tr/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/tr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/uk/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/uk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/ur/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/ur/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/vi/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/vi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.3/_build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css` & `napatrackmater-5.2.3/_build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/pygments.css` & `napatrackmater-5.2.3/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/scripts/bootstrap.js` & `napatrackmater-5.2.3/_build/html/_static/scripts/bootstrap.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/scripts/bootstrap.js.map` & `napatrackmater-5.2.3/_build/html/_static/scripts/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/scripts/pydata-sphinx-theme.js` & `napatrackmater-5.2.3/_build/html/_static/scripts/pydata-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/scripts/pydata-sphinx-theme.js.map` & `napatrackmater-5.2.3/_build/html/_static/scripts/pydata-sphinx-theme.js.map`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/scripts/sphinx-book-theme.js` & `napatrackmater-5.2.3/_build/html/_static/scripts/sphinx-book-theme.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/scripts/sphinx-book-theme.js.map` & `napatrackmater-5.2.3/_build/html/_static/scripts/sphinx-book-theme.js.map`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/searchtools.js` & `napatrackmater-5.2.3/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/sphinx-thebe.css` & `napatrackmater-5.2.3/_build/html/_static/sphinx-thebe.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/sphinx-thebe.js` & `napatrackmater-5.2.3/_build/html/_static/sphinx-thebe.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/styles/bootstrap.css` & `napatrackmater-5.2.3/_build/html/_static/styles/bootstrap.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/styles/pydata-sphinx-theme.css` & `napatrackmater-5.2.3/_build/html/_static/styles/pydata-sphinx-theme.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/styles/sphinx-book-theme.css` & `napatrackmater-5.2.3/_build/html/_static/styles/sphinx-book-theme.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/togglebutton.css` & `napatrackmater-5.2.3/_build/html/_static/togglebutton.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/togglebutton.js` & `napatrackmater-5.2.3/_build/html/_static/togglebutton.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/underscore-1.13.1.js` & `napatrackmater-5.2.3/_build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/underscore.js` & `napatrackmater-5.2.3/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt` & `napatrackmater-5.2.3/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css` & `napatrackmater-5.2.3/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf` & `napatrackmater-5.2.3/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2` & `napatrackmater-5.2.3/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf` & `napatrackmater-5.2.3/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2` & `napatrackmater-5.2.3/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf` & `napatrackmater-5.2.3/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2` & `napatrackmater-5.2.3/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf` & `napatrackmater-5.2.3/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2` & `napatrackmater-5.2.3/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/_static/webpack-macros.html` & `napatrackmater-5.2.3/_build/html/_static/webpack-macros.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/genindex.html` & `napatrackmater-5.2.3/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/search.html` & `napatrackmater-5.2.3/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/html/searchindex.js` & `napatrackmater-5.2.3/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_build/jupyter_execute/Notebooks/Track_vector.ipynb` & `napatrackmater-5.2.3/_build/jupyter_execute/Notebooks/Track_vector.ipynb`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/_config.yml` & `napatrackmater-5.2.3/_config.yml`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/images/ClusterDistributionPlot_time_point_97.png` & `napatrackmater-5.2.3/images/ClusterDistributionPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/images/ClusterNearnessPlot_time_point_97.png` & `napatrackmater-5.2.3/images/ClusterNearnessPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/images/ClusterPlot_time_point_97.png` & `napatrackmater-5.2.3/images/ClusterPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/images/FeatureMatrixPlot_time_point_97.png` & `napatrackmater-5.2.3/images/FeatureMatrixPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/images/QuadrantDistributionPlot_time_point_97.png` & `napatrackmater-5.2.3/images/QuadrantDistributionPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/images/kapoorlablogo.png` & `napatrackmater-5.2.3/images/kapoorlablogo.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/images/kapoorlogo.png` & `napatrackmater-5.2.3/images/kapoorlogo.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/setup.cfg` & `napatrackmater-5.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/src/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-5.2.3/src/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/src/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-5.2.3/src/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/src/napatrackmater/Trackmate.py` & `napatrackmater-5.2.3/src/napatrackmater/Trackmate.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/src/napatrackmater/Trackvector.py` & `napatrackmater-5.2.3/src/napatrackmater/Trackvector.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,36 +6,27 @@
 import numpy as np
 import re
 import napari
 import pandas as pd
 from scipy.spatial.distance import pdist
 from scipy.cluster.hierarchy import linkage, fcluster
 from scipy.spatial import cKDTree
-from sklearn.model_selection import train_test_split
-from sklearn.neighbors import KNeighborsClassifier
-from joblib import dump
-from sklearn.ensemble import RandomForestClassifier
-from sklearn.metrics import accuracy_score
-from sklearn.metrics import silhouette_score
 import torch
-import torch.nn as nn
-import torch.optim as optim
-from torch.utils.data import DataLoader, Dataset
 import json
-from tqdm import tqdm
-from torch.optim.lr_scheduler import MultiStepLR
 import matplotlib.pyplot as plt
 from typing import List, Union
 import torch.nn.init as init
 import random
-
+from sklearn.metrics import silhouette_score
 from sklearn.preprocessing import PolynomialFeatures
 from sklearn.linear_model import LinearRegression
 from statsmodels.tsa.stattools import acf, ccf
 from scipy.stats import norm, anderson
+from kapoorlabs_lightning.lightning_trainer import MitosisInception
+
 
 SHAPE_FEATURES = [
     "Radius",
     "Eccentricity_Comp_First",
     "Eccentricity_Comp_Second",
     "Eccentricity_Comp_Third",
     "Local_Cell_Density",
@@ -1119,105 +1110,14 @@
         )
     }
     full_dataframe["Cluster"] = full_dataframe["Track ID"].map(track_id_to_cluster)
 
     return full_dataframe
 
 
-def supervised_clustering(
-    csv_file_name, gt_analysis_vectors, n_neighbors=10, n_estimators=50, method="knn"
-):
-    csv_file_name_original = csv_file_name + "_training_data"
-    data_list = []
-    track_ids = []
-    for track_id, (
-        shape_dynamic_dataframe_list,
-        gt_dataframe_list,
-        full_dataframe_list,
-    ) in gt_analysis_vectors.items():
-
-        shape_dynamic_track_array = np.array(
-            [
-                [item for item in record.values()]
-                for record in shape_dynamic_dataframe_list
-            ]
-        )
-
-        gt_track_array = np.array(
-            [[item for item in record.values()] for record in gt_dataframe_list]
-        )
-        if shape_dynamic_track_array.shape[0] > 1:
-            track_ids.append(track_id)
-        if not np.isnan(gt_track_array[0]) and shape_dynamic_track_array.shape[0] > 1:
-            (
-                shape_dynamic_covariance,
-                shape_dynamic_eigenvectors,
-            ) = compute_covariance_matrix(shape_dynamic_track_array)
-            upper_triangle_indices = np.triu_indices_from(shape_dynamic_covariance)
-
-            flattened_covariance = shape_dynamic_covariance[upper_triangle_indices]
-            data_list.append(
-                {
-                    "Flattened_Covariance": flattened_covariance,
-                    "gt_label": gt_track_array[0][0],
-                }
-            )
-    result_dataframe = pd.DataFrame(data_list)
-    if os.path.exists(csv_file_name_original):
-        os.remove(csv_file_name_original)
-    result_dataframe.to_csv(csv_file_name_original + ".csv", index=False)
-    if method == "knn":
-        X = np.vstack(result_dataframe["Flattened_Covariance"].values)
-        y = result_dataframe["gt_label"].values
-
-        X_train, X_test, y_train, y_test = train_test_split(
-            X, y, test_size=0.1, random_state=42
-        )
-        unique_train_labels, count_train_labels = np.unique(y_train, return_counts=True)
-
-        unique_test_labels, count_test_labels = np.unique(y_test, return_counts=True)
-
-        print(f"Training labels: {unique_train_labels}")
-        print(f"Training label counts: {count_train_labels}")
-        print(f"Testing labels: {unique_test_labels}")
-        print(f"Testing label counts: {count_test_labels}")
-        print(
-            f"Training data shape: {X_train.shape}, Testing data shape: {X_test.shape}"
-        )
-        model = KNeighborsClassifier(n_neighbors=n_neighbors, n_jobs=-1)
-        model.fit(X_train, y_train)
-        accuracy = model.score(X_test, y_test)
-        print(f"Model Accuracy on test: {accuracy:.2f}")
-        accuracy = model.score(X_train, y_train)
-        print(f"Model Accuracy on train: {accuracy:.2f}")
-
-        model_filename = csv_file_name + "_knn_model.joblib"
-        dump(model, model_filename)
-    else:
-        model = RandomForestClassifier(
-            n_estimators=n_estimators, n_jobs=-1, random_state=42
-        )
-
-        model.fit(X_train, y_train)
-
-        # Make predictions on the test data
-        y_pred_test = model.predict(X_test)
-        y_pred_train = model.predict(X_train)
-
-        accuracy_test = accuracy_score(y_test, y_pred_test)
-        accuracy_train = accuracy_score(y_train, y_pred_train)
-
-        print(f"Model Accuracy on test: {accuracy_test:.2f}")
-        print(f"Model Accuracy on train: {accuracy_train:.2f}")
-
-        model_filename = "random_forest_model.joblib"
-        dump(model, model_filename)
-
-    return model
-
 
 def calculate_wcss(data, labels, centroids):
     wcss = 0
     for i in range(len(data)):
         cluster_label = labels[i]
         centroid = centroids[cluster_label]
         distance = np.linalg.norm(data[i] - centroid)
@@ -2699,373 +2599,70 @@
         concatenated_eigenvectors = np.concatenate((real_part, imag_part), axis=1)
 
         return covariance_matrix, concatenated_eigenvectors
     except Exception as e:
         print(f"Covariance matric computation {e}")
 
 
-class DenseLayer(nn.Module):
-    """ """
-
-    def __init__(self, in_channels, growth_rate, bottleneck_size, kernel_size):
-        super().__init__()
-        self.use_bottleneck = bottleneck_size > 0
-        self.num_bottleneck_output_filters = growth_rate * bottleneck_size
-        if self.use_bottleneck:
-            self.bn2 = nn.GroupNorm(1, in_channels)
-            self.act2 = nn.ReLU(inplace=True)
-            self.conv2 = nn.Conv1d(
-                in_channels, self.num_bottleneck_output_filters, kernel_size=1, stride=1
-            )
-        self.bn1 = nn.GroupNorm(1, self.num_bottleneck_output_filters)
-        self.act1 = nn.ReLU(inplace=True)
-        self.conv1 = nn.Conv1d(
-            self.num_bottleneck_output_filters,
-            growth_rate,
-            kernel_size=kernel_size,
-            stride=1,
-            dilation=1,
-            padding=kernel_size // 2,
-        )
-
-    def forward(self, x):
-        if self.use_bottleneck:
-            x = self.bn2(x)
-            x = self.act2(x)
-            x = self.conv2(x)
-        x = self.bn1(x)
-        x = self.act1(x)
-        x = self.conv1(x)
-        return x
-
-
-class DenseBlock(nn.ModuleDict):
-    """ """
-
-    def __init__(
-        self, num_layers, in_channels, growth_rate, kernel_size, bottleneck_size
-    ):
-        super().__init__()
-        self.num_layers = num_layers
-        for i in range(self.num_layers):
-            self.add_module(
-                f"denselayer{i}",
-                DenseLayer(
-                    in_channels + i * growth_rate,
-                    growth_rate,
-                    bottleneck_size,
-                    kernel_size,
-                ),
-            )
-
-    def forward(self, x):
-        layer_outputs = [x]
-        for _, layer in self.items():
-            x = layer(x)
-            layer_outputs.append(x)
-            x = torch.cat(layer_outputs, dim=1)
-        return x
-
-
-class TransitionBlock(nn.Module):
-    """ """
-
-    def __init__(self, in_channels, out_channels):
-        super().__init__()
-        self.bn = nn.GroupNorm(1, in_channels)
-        self.act = nn.ReLU(inplace=True)
-        self.conv = nn.Conv1d(
-            in_channels, out_channels, kernel_size=1, stride=1, dilation=1
-        )
-        self.pool = nn.AvgPool1d(kernel_size=2, stride=2)
-
-    def forward(self, x):
-        x = self.bn(x)
-        x = self.act(x)
-        x = self.conv(x)
-        x = self.pool(x)
-        return x
-
-
-class DenseNet1d(nn.Module):
-    def __init__(
-        self,
-        growth_rate: int = 32,
-        block_config: tuple = (6, 12, 24, 16),
-        num_init_features: int = 32,
-        bottleneck_size: int = 4,
-        kernel_size: int = 3,
-        in_channels: int = 1,
-        num_classes_1: int = 1,
-    ):
-
-        super().__init__()
-        self._initialize_weights()
-
-        self.features = nn.Sequential(
-            nn.Conv1d(in_channels, num_init_features, kernel_size=1),
-            nn.GroupNorm(1, num_init_features),
-            nn.ReLU(inplace=True),
-            nn.MaxPool1d(kernel_size=1),
-        )
-
-        num_features = num_init_features
-        for i, num_layers in enumerate(block_config):
-            block = DenseBlock(
-                num_layers=num_layers,
-                in_channels=num_features,
-                growth_rate=growth_rate,
-                kernel_size=kernel_size,
-                bottleneck_size=bottleneck_size,
-            )
-            self.features.add_module(f"denseblock{i}", block)
-            num_features = num_features + num_layers * growth_rate
-            if i != len(block_config) - 1:
-                trans = TransitionBlock(
-                    in_channels=num_features, out_channels=num_features // 2
-                )
-                self.features.add_module(f"transition{i}", trans)
-                num_features = num_features // 2
-
-        self.final_bn = nn.GroupNorm(1, num_features)
-        self.final_act = nn.ReLU(inplace=True)
-        self.final_pool = nn.AdaptiveAvgPool1d(1)
-        self.classifier_1 = nn.Linear(num_features, num_classes_1)
-
-    def _initialize_weights(self):
-        for m in self.modules():
-            if isinstance(m, nn.Conv1d):
-                init.kaiming_normal_(m.weight)
-                if m.bias is not None:
-                    init.constant_(m.bias, 0)
-            elif isinstance(m, nn.BatchNorm1d) or isinstance(m, nn.GroupNorm):
-                init.constant_(m.weight, 1)
-                init.constant_(m.bias, 0)
-            elif isinstance(m, nn.Linear):
-                init.kaiming_normal_(m.weight)
-                init.constant_(m.bias, 0)
-
-    def forward_features(self, x):
-        out = self.features(x)
-        out = self.final_bn(out)
-        out = self.final_act(out)
-        out = self.final_pool(out)
-        return out
-
-    def forward(self, x):
-        features = self.forward_features(x)
-        features = features.squeeze(-1)
-        out_1 = self.classifier_1(features)
-        return out_1
-
-    def reset_classifier(self):
-        self.classifier = nn.Identity()
-
-    def get_classifier(self):
-        return self.classifier
-
-
-class MitosisNet(nn.Module):
-
-    def __init__(self, input_channels, num_classes):
-
-        super().__init__()
-        self.conv1 = nn.Conv1d(in_channels=input_channels, out_channels=32, kernel_size=3)
-        self.pool1 = nn.MaxPool1d(kernel_size=2)
-        self.conv2 = nn.Conv1d(in_channels=32, out_channels=64, kernel_size=3)
-        self.pool2 = nn.MaxPool1d(kernel_size=2)
-        
-        self.global_pooling = nn.AdaptiveAvgPool1d(1)
-        self.fc = nn.Linear(64, num_classes)  
-
-    def forward(self, x):
-        x = self.pool1(nn.functional.relu(self.conv1(x)))
-        x = self.pool2(nn.functional.relu(self.conv2(x)))
-        x = self.global_pooling(x).squeeze()  
-        x = self.fc(x)
-        return x
-
-
-class MitosisDataset(Dataset):
-    def __init__(self, arrays, labels):
-        self.arrays = arrays
-        self.labels = labels
-        self.input_channels = arrays.shape[2]
-        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-        
-    def __len__(self):
-        return len(self.arrays)
-    
-    def __getitem__(self, idx):
-        array = self.arrays[idx]
-        array = torch.tensor(array).permute(1, 0).float().to(self.device)
-        label = torch.tensor(self.labels[idx]).to(self.device)
-        return array, label
-   
 
 
 def train_mitosis_neural_net(
     npz_file,
     save_path,
     num_classes = 2,
     batch_size=64,
+    num_workers = 0,
     learning_rate=0.001,
-    weight_decay: float = 1e-5,
-    eps: float = 1e-1,
     epochs=10,
-    use_scheduler=False,
+    accelerator = 'cuda',
+    devices = 1,
+    model_type = 'simple',
+    growth_rate: int = 32,
+    block_config: tuple = (6, 12, 24, 16),
+    num_init_features: int = 32,
+    bottleneck_size: int = 4,
+    kernel_size: int = 3,
+    experiment_name = 'mitosis'
 ):
-    device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-    training_data = np.load(npz_file)
-    train_dividing_arrays = training_data['dividing_train_arrays']
-    train_dividing_labels = training_data['dividing_train_labels']
-    train_non_dividing_arrays = training_data['non_dividing_train_arrays']
-    train_non_dividing_labels = training_data['non_dividing_train_labels']
     
-    val_dividing_arrays = training_data['dividing_val_arrays']
-    val_dividing_labels = training_data['dividing_val_labels']
-    val_non_dividing_arrays = training_data['non_dividing_val_arrays']
-    val_non_dividing_labels = training_data['non_dividing_val_labels']
+   if isinstance(block_config, int):
+       block_config = (block_config,)
+   mitosis_inception = MitosisInception(
+       npz_file = npz_file,
+       num_classes=num_classes,
+       growth_rate=growth_rate,
+       block_config=block_config,
+       num_init_features=num_init_features,
+       bottleneck_size=bottleneck_size,
+       kernel_size=kernel_size,
+       num_workers=num_workers,
+       epochs = epochs,
+       log_path=save_path,
+       batch_size=batch_size,
+       accelerator=accelerator,
+       devices = devices,
+       experiment_name= experiment_name,
+       learning_rate=learning_rate
+   )
+
+   mitosis_inception.setup_datasets()
+   if model_type == 'simple':
+       mitosis_inception.setup_mitosisnet_model()
+   else:     
+       mitosis_inception.setup_densenet_model()
+
+   mitosis_inception.setup_logger()   
+   mitosis_inception.setup_checkpoint()
+   mitosis_inception.setup_adam()
+   mitosis_inception.setup_lightning_model()
+   mitosis_inception.train()
 
 
 
-
-    train_arrays = np.concatenate((train_dividing_arrays, train_non_dividing_arrays))
-    train_labels = np.concatenate((train_dividing_labels, train_non_dividing_labels))
-
-    train_dataset = MitosisDataset(train_arrays, train_labels)
-    train_loader = DataLoader(train_dataset, batch_size=batch_size, shuffle=True)
-
-    val_arrays = np.concatenate((val_dividing_arrays, val_non_dividing_arrays))
-    val_labels = np.concatenate((val_dividing_labels, val_non_dividing_labels))
-
-    val_dataset = MitosisDataset(val_arrays, val_labels)
-    val_loader = DataLoader(val_dataset, batch_size=batch_size, shuffle=False)
-     
-
-    input_channels = train_dataset.input_channels
-   
-
-    model = MitosisNet(
-        input_channels,
-        num_classes =num_classes,
-    )
-
-    model_info = {
-        'input_channels': input_channels,
-        'num_classes': num_classes
-    }
-    with open(save_path + "_model_info.json", "w") as json_file:
-        json.dump(model_info, json_file)
-
-
-    model.to(device)
-
-    criterion_class= nn.CrossEntropyLoss()
-    optimizer = optim.Adam(
-        model.parameters(), lr=learning_rate, weight_decay=weight_decay, eps=eps
-    )
-
-    if use_scheduler:
-        milestones = [int(epochs * 0.25), int(epochs * 0.5), int(epochs * 0.75)]
-        scheduler = MultiStepLR(optimizer, milestones=milestones, gamma=0.1)
-
-   
-    train_loss_class1_values = []
-    val_loss_class1_values = []
-    train_acc_class1_values = []
-    val_acc_class1_values = []
-    for epoch in range(epochs):
-        model.train()
-        running_loss_class= 0.0
-        correct_train_class= 0
-        total_train_class= 0
-
-        with tqdm(total=len(train_loader), desc=f"Epoch {epoch + 1}/{epochs}") as pbar:
-            for i, data in enumerate(train_loader):
-                inputs, labels_class = data
-                optimizer.zero_grad()
-                outputs_class = model(inputs)
-
-                loss_class= criterion_class(outputs_class, labels_class)
-                loss_class.backward()
-
-                optimizer.step()
-
-                _, predicted_class= torch.max(outputs_class.data, 1)
-
-                running_loss_class += loss_class.item()
-                correct_train_class += (predicted_class== labels_class).sum().item()
-                total_train_class+= labels_class.size(0)
-                pbar.update(1)
-                pbar.set_postfix(
-                    {
-                        "Acc Class1": correct_train_class/ total_train_class
-                        if total_train_class> 0
-                        else 0,
-                        "classLoss": running_loss_class/ (i + 1),
-                    }
-                )
-            if use_scheduler:
-                scheduler.step()
-        train_loss_class1_values.append(running_loss_class/ len(train_loader))
-        train_acc_class1_values.append(
-            correct_train_class/ total_train_class if total_train_class> 0 else 0
-        )
-
-        model.eval()
-        running_val_loss_class= 0.0
-        correct_val_class= 0
-        total_val_class= 0
-
-        with tqdm(
-            total=len(val_loader), desc=f"Validation Epoch {epoch + 1}/{epochs}"
-        ) as pbar_val:
-            with torch.no_grad():
-                for i, data in enumerate(val_loader):
-                    inputs, labels_class= data
-                    outputs_class= model(inputs)
-
-                    _, predicted_class= torch.max(outputs_class.data, 1)
-
-                    total_val_class+= labels_class.size(0)
-                    correct_val_class+= (
-                        (predicted_class== labels_class).sum().item()
-                    )
-
-                    pbar_val.update(1)
-                    accuracy_class= (
-                        correct_val_class/ total_val_class
-                        if total_val_class> 0
-                        else 0
-                    )
-                    loss_class= criterion_class(outputs_class, labels_class)
-
-                    running_val_loss_class+= loss_class.item()
-                    pbar_val.set_postfix(
-                        {
-                            "Acc Class1": accuracy_class,
-                            "classLoss": running_val_loss_class/ (i + 1),
-                        }
-                    )
-
-        val_loss_class1_values.append(running_val_loss_class/ len(val_loader))
-        val_acc_class1_values.append(
-            correct_val_class/ total_val_class if total_val_class> 0 else 0
-        )
-
-    np.savez(
-        save_path + "_metrics.npz",
-        train_loss_class1=train_loss_class1_values,
-        val_loss_class1=val_loss_class1_values,
-        train_acc_class1=train_acc_class1_values,
-        val_acc_class1=val_acc_class1_values,
-    )
-    torch.save(model.state_dict(), save_path + "_mitosis_track_model.pth")
-
+    
 
 def plot_metrics_from_npz(npz_file):
     data = np.load(npz_file)
 
     train_loss_class= data["train_loss_class1"]
     val_loss_class= data["val_loss_class1"]
     train_acc_class= data["train_acc_class1"]
@@ -3086,59 +2683,14 @@
     plt.legend(loc="upper right")
     plt.title("Accuracy for Class 1")
 
     plt.tight_layout()
     plt.show()
 
 
-def predict_with_model(
-    saved_model_path, saved_model_json, features_array, threshold=None
-):
-    device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-    with open(saved_model_json) as json_file:
-        model_info = json.load(json_file)
-
-    input_channels = model_info["input_channels"]
-    num_classes = model_info["num_classes"]
-  
-
-    model = MitosisNet(
-        input_channels,
-        num_classes_class1=num_classes,
-    )
-
-  
-    model.load_state_dict(
-        torch.load(saved_model_path, map_location=torch.device(device))
-    )
-    model.to(device)
-    model.eval()
-    predicted_classes1 = []
-    for idx in range(features_array.shape[0]):
-        feature_type = features_array[idx, :].tolist()
-        features_tensor = torch.tensor(feature_type).to(device)
-
-        with torch.no_grad():
-            outputs_class= model(features_tensor)
-            predicted_probs_class= torch.softmax(outputs_class, dim=1)
-            if threshold is not None:
-                predicted_probs_class1_numpy = (
-                    predicted_probs_class.cpu().detach().numpy()
-                )
-                predicted_class= (
-                    predicted_probs_class1_numpy[0][1] > threshold
-                ).astype(int)
-            else:
-                predicted_class= (
-                    torch.argmax(predicted_probs_class, dim=1).cpu().numpy()
-                )[0]
-
-            predicted_classes1.append(predicted_class)
-
-    return predicted_classes1
 
 
 def get_zero_gen_daughter_generations(
     unique_trackmate_track_ids,
     global_shape_dynamic_dataframe,
     zero_gen_tracklets,
     daughter_generations,
```

### Comparing `napatrackmater-5.2.2/src/napatrackmater/__init__.py` & `napatrackmater-5.2.3/src/napatrackmater/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 from .Trackmate import TrackMate, get_feature_dict
 
 from .Trackvector import (
     TrackVector,
     convert_tracks_to_arrays,
     unsupervised_clustering,
     simple_unsupervised_clustering,
-    supervised_clustering,
     create_global_gt_dataframe,
     create_gt_analysis_vectors_dict,
     train_mitosis_neural_net,
-    predict_with_model,
     plot_metrics_from_npz,
     create_analysis_tracklets,
     create_dividing_prediction_tracklets,
     convert_tracks_to_simple_arrays,
     local_track_covaraince,
     cell_fate_recipe,
     core_clustering,
```

### Comparing `napatrackmater-5.2.2/src/napatrackmater/clustering.py` & `napatrackmater-5.2.3/src/napatrackmater/clustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/src/napatrackmater/fast_radius_regression.py` & `napatrackmater-5.2.3/src/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/src/napatrackmater/fate_mapping.py` & `napatrackmater-5.2.3/src/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/src/napatrackmater/pretrained.py` & `napatrackmater-5.2.3/src/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/src/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-5.2.3/src/napatrackmater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 5.2.2
+Version: 5.2.3
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/Kapoorlabs-CAPED/napatrackmater
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/napatrackmater/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/napatrackmater#README.md
```

### Comparing `napatrackmater-5.2.2/src/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-5.2.3/src/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.2.2/update_version.py` & `napatrackmater-5.2.3/update_version.py`

 * *Files identical despite different names*

