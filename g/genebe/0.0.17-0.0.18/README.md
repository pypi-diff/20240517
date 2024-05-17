# Comparing `tmp/genebe-0.0.17.tar.gz` & `tmp/genebe-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genebe-0.0.17.tar", last modified: Fri Mar  8 14:13:58 2024, max compression
+gzip compressed data, was "genebe-0.0.18.tar", last modified: Fri May 17 07:14:14 2024, max compression
```

## Comparing `genebe-0.0.17.tar` & `genebe-0.0.18.tar`

### file list

```diff
@@ -1,21 +1,124 @@
-drwxr-xr-x   0 pio       (1000) pio       (1000)        0 2024-03-08 14:13:58.949847 genebe-0.0.17/
--rw-r--r--   0 pio       (1000) pio       (1000)        0 2023-10-01 16:14:18.000000 genebe-0.0.17/MANIFEST.in
--rw-r--r--   0 pio       (1000) pio       (1000)     5994 2024-03-08 14:13:58.949847 genebe-0.0.17/PKG-INFO
--rw-r--r--   0 pio       (1000) pio       (1000)     5269 2024-02-22 09:17:43.000000 genebe-0.0.17/README.md
-drwxr-xr-x   0 pio       (1000) pio       (1000)        0 2024-03-08 14:13:58.949847 genebe-0.0.17/genebe/
--rw-r--r--   0 pio       (1000) pio       (1000)      375 2024-02-22 08:50:38.000000 genebe-0.0.17/genebe/__init__.py
--rw-r--r--   0 pio       (1000) pio       (1000)    22740 2024-02-22 09:10:18.000000 genebe-0.0.17/genebe/client.py
--rw-r--r--   0 pio       (1000) pio       (1000)     6929 2024-02-19 09:42:15.000000 genebe-0.0.17/genebe/entrypoint.py
--rw-r--r--   0 pio       (1000) pio       (1000)     7868 2024-03-08 14:08:23.000000 genebe-0.0.17/genebe/gbid.py
--rw-r--r--   0 pio       (1000) pio       (1000)     6742 2024-01-05 19:54:06.000000 genebe-0.0.17/genebe/json_simple_annotator.py
--rw-r--r--   0 pio       (1000) pio       (1000)     6110 2024-02-19 09:42:15.000000 genebe-0.0.17/genebe/vcf_simple_annotator.py
--rw-r--r--   0 pio       (1000) pio       (1000)       23 2024-03-08 14:13:36.000000 genebe-0.0.17/genebe/version.py
-drwxr-xr-x   0 pio       (1000) pio       (1000)        0 2024-03-08 14:13:58.949847 genebe-0.0.17/genebe.egg-info/
--rw-r--r--   0 pio       (1000) pio       (1000)     5994 2024-03-08 14:13:58.000000 genebe-0.0.17/genebe.egg-info/PKG-INFO
--rw-r--r--   0 pio       (1000) pio       (1000)      365 2024-03-08 14:13:58.000000 genebe-0.0.17/genebe.egg-info/SOURCES.txt
--rw-r--r--   0 pio       (1000) pio       (1000)        1 2024-03-08 14:13:58.000000 genebe-0.0.17/genebe.egg-info/dependency_links.txt
--rw-r--r--   0 pio       (1000) pio       (1000)       50 2024-03-08 14:13:58.000000 genebe-0.0.17/genebe.egg-info/entry_points.txt
--rw-r--r--   0 pio       (1000) pio       (1000)       67 2024-03-08 14:13:58.000000 genebe-0.0.17/genebe.egg-info/requires.txt
--rw-r--r--   0 pio       (1000) pio       (1000)        7 2024-03-08 14:13:58.000000 genebe-0.0.17/genebe.egg-info/top_level.txt
--rw-r--r--   0 pio       (1000) pio       (1000)       38 2024-03-08 14:13:58.949847 genebe-0.0.17/setup.cfg
--rw-r--r--   0 pio       (1000) pio       (1000)      962 2024-01-10 11:50:29.000000 genebe-0.0.17/setup.py
+drwxr-xr-x   0 pio       (1000) pio       (1000)        0 2024-05-17 07:14:14.225197 genebe-0.0.18/
+-rw-r--r--   0 pio       (1000) pio       (1000)       61 2024-01-09 15:54:49.000000 genebe-0.0.18/.gitignore
+-rw-r--r--   0 pio       (1000) pio       (1000)      816 2024-01-11 20:02:07.000000 genebe-0.0.18/.readthedocs.yaml
+-rw-r--r--   0 pio       (1000) pio       (1000)      391 2024-01-09 19:40:17.000000 genebe-0.0.18/Dockerfile
+-rw-r--r--   0 pio       (1000) pio       (1000)        0 2023-10-01 16:14:18.000000 genebe-0.0.18/MANIFEST.in
+-rw-r--r--   0 pio       (1000) pio       (1000)     5994 2024-05-17 07:14:14.225197 genebe-0.0.18/PKG-INFO
+-rw-r--r--   0 pio       (1000) pio       (1000)     5269 2024-02-22 09:17:43.000000 genebe-0.0.18/README.md
+drwxr-xr-x   0 pio       (1000) pio       (1000)        0 2024-05-17 07:14:14.205197 genebe-0.0.18/docs/
+-rw-r--r--   0 pio       (1000) pio       (1000)      634 2024-01-10 10:59:22.000000 genebe-0.0.18/docs/Makefile
+drwxr-xr-x   0 pio       (1000) pio       (1000)        0 2024-05-17 07:14:14.201197 genebe-0.0.18/docs/_build/
+drwxr-xr-x   0 pio       (1000) pio       (1000)        0 2024-05-17 07:14:14.209197 genebe-0.0.18/docs/_build/doctrees/
+-rw-r--r--   0 pio       (1000) pio       (1000)   594958 2024-01-11 17:59:55.000000 genebe-0.0.18/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0 pio       (1000) pio       (1000)   193739 2024-01-11 17:59:55.000000 genebe-0.0.18/docs/_build/doctrees/genebe.doctree
+-rw-r--r--   0 pio       (1000) pio       (1000)     5099 2024-01-11 17:59:55.000000 genebe-0.0.18/docs/_build/doctrees/index.doctree
+-rw-r--r--   0 pio       (1000) pio       (1000)     7125 2024-01-11 17:59:55.000000 genebe-0.0.18/docs/_build/doctrees/installation.doctree
+-rw-r--r--   0 pio       (1000) pio       (1000)     2947 2024-01-11 17:59:55.000000 genebe-0.0.18/docs/_build/doctrees/limits.doctree
+-rw-r--r--   0 pio       (1000) pio       (1000)     2766 2024-01-11 17:59:55.000000 genebe-0.0.18/docs/_build/doctrees/modules.doctree
+drwxr-xr-x   0 pio       (1000) pio       (1000)        0 2024-05-17 07:14:14.209197 genebe-0.0.18/docs/_build/doctrees/source/
+-rw-r--r--   0 pio       (1000) pio       (1000)   193753 2024-01-10 19:04:34.000000 genebe-0.0.18/docs/_build/doctrees/source/genebe.doctree
+-rw-r--r--   0 pio       (1000) pio       (1000)     2787 2024-01-10 19:04:34.000000 genebe-0.0.18/docs/_build/doctrees/source/modules.doctree
+-rw-r--r--   0 pio       (1000) pio       (1000)     9281 2024-01-11 17:59:55.000000 genebe-0.0.18/docs/_build/doctrees/usage.doctree
+drwxr-xr-x   0 pio       (1000) pio       (1000)        0 2024-05-17 07:14:14.213197 genebe-0.0.18/docs/_build/html/
+-rw-r--r--   0 pio       (1000) pio       (1000)      230 2024-01-11 17:59:55.000000 genebe-0.0.18/docs/_build/html/.buildinfo
+drwxr-xr-x   0 pio       (1000) pio       (1000)        0 2024-05-17 07:14:14.213197 genebe-0.0.18/docs/_build/html/_sources/
+-rw-r--r--   0 pio       (1000) pio       (1000)     1036 2024-01-10 19:02:50.000000 genebe-0.0.18/docs/_build/html/_sources/genebe.rst.txt
+-rw-r--r--   0 pio       (1000) pio       (1000)      485 2024-01-11 17:57:49.000000 genebe-0.0.18/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 pio       (1000) pio       (1000)     1172 2024-01-10 11:30:23.000000 genebe-0.0.18/docs/_build/html/_sources/installation.rst.txt
+-rw-r--r--   0 pio       (1000) pio       (1000)       36 2024-01-11 17:59:40.000000 genebe-0.0.18/docs/_build/html/_sources/limits.md.txt
+-rw-r--r--   0 pio       (1000) pio       (1000)       55 2024-01-10 19:02:50.000000 genebe-0.0.18/docs/_build/html/_sources/modules.rst.txt
+drwxr-xr-x   0 pio       (1000) pio       (1000)        0 2024-05-17 07:14:14.213197 genebe-0.0.18/docs/_build/html/_sources/source/
+-rw-r--r--   0 pio       (1000) pio       (1000)     1036 2024-01-10 19:02:50.000000 genebe-0.0.18/docs/_build/html/_sources/source/genebe.rst.txt
+-rw-r--r--   0 pio       (1000) pio       (1000)       55 2024-01-10 19:02:50.000000 genebe-0.0.18/docs/_build/html/_sources/source/modules.rst.txt
+-rw-r--r--   0 pio       (1000) pio       (1000)     1718 2024-01-10 18:28:15.000000 genebe-0.0.18/docs/_build/html/_sources/usage.rst.txt
+drwxr-xr-x   0 pio       (1000) pio       (1000)        0 2024-05-17 07:14:14.217197 genebe-0.0.18/docs/_build/html/_static/
+-rw-r--r--   0 pio       (1000) pio       (1000)     4289 2024-01-11 17:59:55.000000 genebe-0.0.18/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 pio       (1000) pio       (1000)    11143 2024-01-10 11:31:07.000000 genebe-0.0.18/docs/_build/html/_static/alabaster.css
+-rw-r--r--   0 pio       (1000) pio       (1000)    15094 2024-01-11 17:59:55.000000 genebe-0.0.18/docs/_build/html/_static/basic.css
+drwxr-xr-x   0 pio       (1000) pio       (1000)        0 2024-05-17 07:14:14.217197 genebe-0.0.18/docs/_build/html/_static/css/
+-rw-r--r--   0 pio       (1000) pio       (1000)     3229 2024-01-10 10:59:48.000000 genebe-0.0.18/docs/_build/html/_static/css/badge_only.css
+drwxr-xr-x   0 pio       (1000) pio       (1000)        0 2024-05-17 07:14:14.221197 genebe-0.0.18/docs/_build/html/_static/css/fonts/
+-rw-r--r--   0 pio       (1000) pio       (1000)    87624 2024-01-10 10:59:48.000000 genebe-0.0.18/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 pio       (1000) pio       (1000)    67312 2024-01-10 10:59:48.000000 genebe-0.0.18/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 pio       (1000) pio       (1000)    86288 2024-01-10 10:59:48.000000 genebe-0.0.18/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 pio       (1000) pio       (1000)    66444 2024-01-10 10:59:48.000000 genebe-0.0.18/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 pio       (1000) pio       (1000)   165742 2024-01-10 10:59:48.000000 genebe-0.0.18/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 pio       (1000) pio       (1000)   444379 2024-01-10 10:59:48.000000 genebe-0.0.18/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 pio       (1000) pio       (1000)   165548 2024-01-10 10:59:48.000000 genebe-0.0.18/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 pio       (1000) pio       (1000)    98024 2024-01-10 10:59:48.000000 genebe-0.0.18/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 pio       (1000) pio       (1000)    77160 2024-01-10 10:59:48.000000 genebe-0.0.18/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 pio       (1000) pio       (1000)   323344 2024-01-10 10:59:48.000000 genebe-0.0.18/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 pio       (1000) pio       (1000)   193308 2024-01-10 10:59:48.000000 genebe-0.0.18/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 pio       (1000) pio       (1000)   309728 2024-01-10 10:59:48.000000 genebe-0.0.18/docs/_build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 pio       (1000) pio       (1000)   184912 2024-01-10 10:59:48.000000 genebe-0.0.18/docs/_build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 pio       (1000) pio       (1000)   328412 2024-01-10 10:59:48.000000 genebe-0.0.18/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 pio       (1000) pio       (1000)   195704 2024-01-10 10:59:48.000000 genebe-0.0.18/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 pio       (1000) pio       (1000)   309192 2024-01-10 10:59:48.000000 genebe-0.0.18/docs/_build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 pio       (1000) pio       (1000)   182708 2024-01-10 10:59:48.000000 genebe-0.0.18/docs/_build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 pio       (1000) pio       (1000)   135314 2024-01-10 10:59:48.000000 genebe-0.0.18/docs/_build/html/_static/css/theme.css
+-rw-r--r--   0 pio       (1000) pio       (1000)       42 2024-01-10 10:49:43.000000 genebe-0.0.18/docs/_build/html/_static/custom.css
+-rw-r--r--   0 pio       (1000) pio       (1000)     4472 2024-01-10 10:49:44.000000 genebe-0.0.18/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 pio       (1000) pio       (1000)      329 2024-01-11 17:59:55.000000 genebe-0.0.18/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 pio       (1000) pio       (1000)      286 2024-01-10 10:49:44.000000 genebe-0.0.18/docs/_build/html/_static/file.png
+-rw-r--r--   0 pio       (1000) pio       (1000)    89501 2024-01-11 17:59:55.000000 genebe-0.0.18/docs/_build/html/_static/jquery.js
+drwxr-xr-x   0 pio       (1000) pio       (1000)        0 2024-05-17 07:14:14.221197 genebe-0.0.18/docs/_build/html/_static/js/
+-rw-r--r--   0 pio       (1000) pio       (1000)      934 2024-01-10 10:59:48.000000 genebe-0.0.18/docs/_build/html/_static/js/badge_only.js
+-rw-r--r--   0 pio       (1000) pio       (1000)     4370 2024-01-10 10:59:48.000000 genebe-0.0.18/docs/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 pio       (1000) pio       (1000)     2734 2024-01-10 10:59:48.000000 genebe-0.0.18/docs/_build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0 pio       (1000) pio       (1000)     5023 2024-01-10 10:59:48.000000 genebe-0.0.18/docs/_build/html/_static/js/theme.js
+-rw-r--r--   0 pio       (1000) pio       (1000)     4758 2024-01-11 17:59:55.000000 genebe-0.0.18/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 pio       (1000) pio       (1000)       90 2024-01-10 10:49:44.000000 genebe-0.0.18/docs/_build/html/_static/minus.png
+-rw-r--r--   0 pio       (1000) pio       (1000)       90 2024-01-10 10:49:44.000000 genebe-0.0.18/docs/_build/html/_static/plus.png
+-rw-r--r--   0 pio       (1000) pio       (1000)     4902 2024-01-11 17:59:55.000000 genebe-0.0.18/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 pio       (1000) pio       (1000)    18732 2024-01-10 10:49:44.000000 genebe-0.0.18/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 pio       (1000) pio       (1000)     5123 2024-01-10 10:49:44.000000 genebe-0.0.18/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 pio       (1000) pio       (1000)    68320 2024-01-11 17:59:55.000000 genebe-0.0.18/docs/_build/html/genebe.html
+-rw-r--r--   0 pio       (1000) pio       (1000)    13167 2024-01-11 17:59:55.000000 genebe-0.0.18/docs/_build/html/genindex.html
+-rw-r--r--   0 pio       (1000) pio       (1000)     6000 2024-01-11 17:59:55.000000 genebe-0.0.18/docs/_build/html/index.html
+-rw-r--r--   0 pio       (1000) pio       (1000)     7168 2024-01-11 17:59:55.000000 genebe-0.0.18/docs/_build/html/installation.html
+-rw-r--r--   0 pio       (1000) pio       (1000)     4673 2024-01-11 17:59:55.000000 genebe-0.0.18/docs/_build/html/limits.html
+-rw-r--r--   0 pio       (1000) pio       (1000)    13691 2024-01-11 17:59:55.000000 genebe-0.0.18/docs/_build/html/modules.html
+-rw-r--r--   0 pio       (1000) pio       (1000)      784 2024-01-11 17:59:55.000000 genebe-0.0.18/docs/_build/html/objects.inv
+-rw-r--r--   0 pio       (1000) pio       (1000)     5558 2024-01-11 17:59:55.000000 genebe-0.0.18/docs/_build/html/py-modindex.html
+-rw-r--r--   0 pio       (1000) pio       (1000)     4128 2024-01-11 17:59:55.000000 genebe-0.0.18/docs/_build/html/search.html
+-rw-r--r--   0 pio       (1000) pio       (1000)    13471 2024-01-11 17:59:55.000000 genebe-0.0.18/docs/_build/html/searchindex.js
+drwxr-xr-x   0 pio       (1000) pio       (1000)        0 2024-05-17 07:14:14.221197 genebe-0.0.18/docs/_build/html/source/
+-rw-r--r--   0 pio       (1000) pio       (1000)    64157 2024-01-10 19:04:35.000000 genebe-0.0.18/docs/_build/html/source/genebe.html
+-rw-r--r--   0 pio       (1000) pio       (1000)    12903 2024-01-10 19:04:35.000000 genebe-0.0.18/docs/_build/html/source/modules.html
+-rw-r--r--   0 pio       (1000) pio       (1000)     8089 2024-01-11 17:59:55.000000 genebe-0.0.18/docs/_build/html/usage.html
+-rw-r--r--   0 pio       (1000) pio       (1000)     1018 2024-01-11 17:59:12.000000 genebe-0.0.18/docs/conf.py
+-rw-r--r--   0 pio       (1000) pio       (1000)     1036 2024-01-10 19:02:50.000000 genebe-0.0.18/docs/genebe.rst
+-rw-r--r--   0 pio       (1000) pio       (1000)      485 2024-01-11 17:57:49.000000 genebe-0.0.18/docs/index.rst
+-rw-r--r--   0 pio       (1000) pio       (1000)     1172 2024-01-10 11:30:23.000000 genebe-0.0.18/docs/installation.rst
+-rw-r--r--   0 pio       (1000) pio       (1000)     1185 2024-01-11 18:22:53.000000 genebe-0.0.18/docs/limits.md
+-rw-r--r--   0 pio       (1000) pio       (1000)      800 2024-01-10 10:59:22.000000 genebe-0.0.18/docs/make.bat
+-rw-r--r--   0 pio       (1000) pio       (1000)       55 2024-01-10 19:02:50.000000 genebe-0.0.18/docs/modules.rst
+-rw-r--r--   0 pio       (1000) pio       (1000)       29 2024-01-11 19:59:28.000000 genebe-0.0.18/docs/requirements.txt
+-rw-r--r--   0 pio       (1000) pio       (1000)     2813 2024-02-22 09:15:03.000000 genebe-0.0.18/docs/usage.md
+drwxr-xr-x   0 pio       (1000) pio       (1000)        0 2024-05-17 07:14:14.221197 genebe-0.0.18/examples/
+-rw-r--r--   0 pio       (1000) pio       (1000)    60896 2024-01-10 19:11:19.000000 genebe-0.0.18/examples/clingen-erepo.ipynb
+-rw-r--r--   0 pio       (1000) pio       (1000)    15034 2024-01-13 11:25:38.000000 genebe-0.0.18/examples/showcase.ipynb
+drwxr-xr-x   0 pio       (1000) pio       (1000)        0 2024-05-17 07:14:14.221197 genebe-0.0.18/genebe/
+-rw-r--r--   0 pio       (1000) pio       (1000)       12 2024-01-09 15:55:17.000000 genebe-0.0.18/genebe/.gitignore
+-rw-r--r--   0 pio       (1000) pio       (1000)      375 2024-02-22 08:50:38.000000 genebe-0.0.18/genebe/__init__.py
+-rw-r--r--   0 pio       (1000) pio       (1000)    23110 2024-05-17 07:10:57.000000 genebe-0.0.18/genebe/client.py
+-rw-r--r--   0 pio       (1000) pio       (1000)     6929 2024-02-19 09:42:15.000000 genebe-0.0.18/genebe/entrypoint.py
+-rw-r--r--   0 pio       (1000) pio       (1000)     7868 2024-03-08 14:08:23.000000 genebe-0.0.18/genebe/gbid.py
+-rw-r--r--   0 pio       (1000) pio       (1000)     6742 2024-01-05 19:54:06.000000 genebe-0.0.18/genebe/json_simple_annotator.py
+-rw-r--r--   0 pio       (1000) pio       (1000)     6110 2024-02-19 09:42:15.000000 genebe-0.0.18/genebe/vcf_simple_annotator.py
+-rw-r--r--   0 pio       (1000) pio       (1000)       23 2024-05-17 07:09:26.000000 genebe-0.0.18/genebe/version.py
+drwxr-xr-x   0 pio       (1000) pio       (1000)        0 2024-05-17 07:14:14.225197 genebe-0.0.18/genebe.egg-info/
+-rw-r--r--   0 pio       (1000) pio       (1000)     5994 2024-05-17 07:14:13.000000 genebe-0.0.18/genebe.egg-info/PKG-INFO
+-rw-r--r--   0 pio       (1000) pio       (1000)     3671 2024-05-17 07:14:14.000000 genebe-0.0.18/genebe.egg-info/SOURCES.txt
+-rw-r--r--   0 pio       (1000) pio       (1000)        1 2024-05-17 07:14:13.000000 genebe-0.0.18/genebe.egg-info/dependency_links.txt
+-rw-r--r--   0 pio       (1000) pio       (1000)       50 2024-05-17 07:14:13.000000 genebe-0.0.18/genebe.egg-info/entry_points.txt
+-rw-r--r--   0 pio       (1000) pio       (1000)       67 2024-05-17 07:14:13.000000 genebe-0.0.18/genebe.egg-info/requires.txt
+-rw-r--r--   0 pio       (1000) pio       (1000)        7 2024-05-17 07:14:13.000000 genebe-0.0.18/genebe.egg-info/top_level.txt
+-rwxr-xr-x   0 pio       (1000) pio       (1000)      196 2024-02-19 09:42:15.000000 genebe-0.0.18/publish_docker.sh
+-rwxr--r--   0 pio       (1000) pio       (1000)      139 2024-01-09 19:53:02.000000 genebe-0.0.18/publish_pypi.sh
+-rw-r--r--   0 pio       (1000) pio       (1000)       38 2024-05-17 07:14:14.225197 genebe-0.0.18/setup.cfg
+-rw-r--r--   0 pio       (1000) pio       (1000)      962 2024-01-10 11:50:29.000000 genebe-0.0.18/setup.py
+-rw-r--r--   0 pio       (1000) pio       (1000)       69 2023-12-21 11:38:46.000000 genebe-0.0.18/simple_runner.py
+drwxr-xr-x   0 pio       (1000) pio       (1000)        0 2024-05-17 07:14:14.225197 genebe-0.0.18/tests/
+-rw-r--r--   0 pio       (1000) pio       (1000)      180 2023-12-01 17:22:09.000000 genebe-0.0.18/tests/unit_test.py
+-rw-r--r--   0 pio       (1000) pio       (1000)      753 2023-12-01 17:32:49.000000 genebe-0.0.18/tests/variantannotation_test.py
```

### Comparing `genebe-0.0.17/PKG-INFO` & `genebe-0.0.18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genebe
-Version: 0.0.17
+Version: 0.0.18
 Summary: GeneBe Client: A user-friendly system for annotating genetic variants
 Home-page: https://github.com/pstawinski/pygenebe
 Author: Piotr Stawinski
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `genebe-0.0.17/README.md` & `genebe-0.0.18/README.md`

 * *Files identical despite different names*

### Comparing `genebe-0.0.17/genebe/client.py` & `genebe-0.0.18/genebe/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import json
 import logging
 import netrc
 from tinynetrc import Netrc
 from urllib.parse import urlparse
 from importlib import metadata
 from .version import __version__
+from pathlib import Path
+
 
 try:
     from tqdm import tqdm
 except ImportError:
 
     def tqdm(iterator, *args, **kwargs):
         return iterator
@@ -53,18 +55,27 @@
         return {"chr": chr_, "pos": pos, "ref": ref, "alt": alt}
     else:
         print(f"Error: Invalid format in [{s}]")
         return None
 
 
 def _save_credentials_to_netrc(machine, login, password):
-    netrc = Netrc()
-    netrc[machine]["login"] = login
-    netrc[machine]["password"] = password
-    netrc.save()
+    try:
+        fpath = Path().home().joinpath(".netrc")
+        fpath.touch(exist_ok=True)
+        netrc = Netrc(str(fpath))
+
+        netrc[machine]["login"] = login
+        netrc[machine]["password"] = password
+        netrc.save()
+        print(
+            "Saved credentials to .netrc, you don't need to provide username/api_key anymore."
+        )
+    except Exception as e:
+        print(f"An error occurred while saving credentials to {fpath}: {e}")
 
 
 def _get_machine_name_from_endpoint(endpoint):
     """
     Extracts the machine name from an endpoint URL.
 
     Args:
```

### Comparing `genebe-0.0.17/genebe/entrypoint.py` & `genebe-0.0.18/genebe/entrypoint.py`

 * *Files identical despite different names*

### Comparing `genebe-0.0.17/genebe/gbid.py` & `genebe-0.0.18/genebe/gbid.py`

 * *Files identical despite different names*

### Comparing `genebe-0.0.17/genebe/json_simple_annotator.py` & `genebe-0.0.18/genebe/json_simple_annotator.py`

 * *Files identical despite different names*

### Comparing `genebe-0.0.17/genebe/vcf_simple_annotator.py` & `genebe-0.0.18/genebe/vcf_simple_annotator.py`

 * *Files identical despite different names*

### Comparing `genebe-0.0.17/genebe.egg-info/PKG-INFO` & `genebe-0.0.18/genebe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genebe
-Version: 0.0.17
+Version: 0.0.18
 Summary: GeneBe Client: A user-friendly system for annotating genetic variants
 Home-page: https://github.com/pstawinski/pygenebe
 Author: Piotr Stawinski
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `genebe-0.0.17/setup.py` & `genebe-0.0.18/setup.py`

 * *Files identical despite different names*

