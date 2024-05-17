# Comparing `tmp/voila-materialscloud-template-0.3.9.tar.gz` & `tmp/voila_materialscloud_template-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voila-materialscloud-template-0.3.9.tar", last modified: Sat Dec 11 02:45:10 2021, max compression
+gzip compressed data, was "voila_materialscloud_template-0.4.0.tar", last modified: Fri May 17 15:56:52 2024, max compression
```

## Comparing `voila-materialscloud-template-0.3.9.tar` & `voila_materialscloud_template-0.4.0.tar`

### file list

```diff
@@ -1,66 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 02:45:10.619470 voila-materialscloud-template-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1537 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      117 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2021-12-11 02:45:10.619470 voila-materialscloud-template-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/README.md
--rwxr-xr-x   0 runner    (1001) docker     (121)     3294 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/copy_voila_template.py
--rw-r--r--   0 runner    (1001) docker     (121)       74 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/requirements_base.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)      134 2021-12-11 02:45:10.619470 voila-materialscloud-template-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2011 2021-12-11 02:45:09.000000 voila-materialscloud-template-0.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 02:45:10.607470 voila-materialscloud-template-0.3.9/share/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 02:45:10.607470 voila-materialscloud-template-0.3.9/share/jupyter/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 02:45:10.607470 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 02:45:10.607470 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 02:45:10.611470 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud/conf.json
--rw-r--r--   0 runner    (1001) docker     (121)    16909 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud/index.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 02:45:10.607470 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 02:45:10.615470 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)   546493 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud/static/css/index.css
--rw-r--r--   0 runner    (1001) docker     (121)   140563 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud/static/css/mcloud_theme.min.css
--rw-r--r--   0 runner    (1001) docker     (121)    15629 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud/static/css/theme-dark.css
--rw-r--r--   0 runner    (1001) docker     (121)    14533 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud/static/css/theme-light.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 02:45:10.615470 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud/static/images/
--rw-r--r--   0 runner    (1001) docker     (121)     2780 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud/static/images/favicon.png
--rw-r--r--   0 runner    (1001) docker     (121)     3805 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud/static/images/mcloud_logo.png
--rw-r--r--   0 runner    (1001) docker     (121)     3490 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud/static/images/mcloud_logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)     9893 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud/static/images/mcloud_spinner.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 02:45:10.615470 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud/static/js/
--rw-r--r--   0 runner    (1001) docker     (121)    17536 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud/static/js/require.min.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 02:45:10.611470 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/conf.json
--rw-r--r--   0 runner    (1001) docker     (121)    13920 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/index.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 02:45:10.607470 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 02:45:10.611470 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)   546493 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/css/index.css
--rw-r--r--   0 runner    (1001) docker     (121)   140563 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/css/mcloud_theme.min.css
--rw-r--r--   0 runner    (1001) docker     (121)    15629 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/css/theme-dark.css
--rw-r--r--   0 runner    (1001) docker     (121)    14533 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/css/theme-light.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 02:45:10.615470 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/
--rw-r--r--   0 runner    (1001) docker     (121)    18197 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/MaterialsCloud_Horizontal_White.png
--rw-r--r--   0 runner    (1001) docker     (121)     2780 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/favicon.png
--rw-r--r--   0 runner    (1001) docker     (121)     3805 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/mcloud_logo.png
--rw-r--r--   0 runner    (1001) docker     (121)     3490 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/mcloud_logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)     9893 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/mcloud_spinner.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 02:45:10.615470 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/
--rw-r--r--   0 runner    (1001) docker     (121)    53386 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/iframeResizer.contentWindow.map
--rw-r--r--   0 runner    (1001) docker     (121)    14147 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/iframeResizer.contentWindow.min.js
--rw-r--r--   0 runner    (1001) docker     (121)    17536 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/require.min.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 02:45:10.607470 voila-materialscloud-template-0.3.9/share/jupyter/voila/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 02:45:10.607470 voila-materialscloud-template-0.3.9/share/jupyter/voila/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 02:45:10.619470 voila-materialscloud-template-0.3.9/share/jupyter/voila/templates/materialscloud/
--rw-r--r--   0 runner    (1001) docker     (121)     2215 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/voila/templates/materialscloud/base.html
--rw-r--r--   0 runner    (1001) docker     (121)      876 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/voila/templates/materialscloud/index.html.j2
--rw-r--r--   0 runner    (1001) docker     (121)      678 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/voila/templates/materialscloud/spinner.macro.html.j2
--rw-r--r--   0 runner    (1001) docker     (121)      404 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/voila/templates/materialscloud/tree.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 02:45:10.619470 voila-materialscloud-template-0.3.9/share/jupyter/voila/templates/materialscloud-iframe/
--rw-r--r--   0 runner    (1001) docker     (121)      883 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/voila/templates/materialscloud-iframe/index.html.j2
--rw-r--r--   0 runner    (1001) docker     (121)      678 2021-12-11 02:45:03.000000 voila-materialscloud-template-0.3.9/share/jupyter/voila/templates/materialscloud-iframe/spinner.macro.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-11 02:45:10.619470 voila-materialscloud-template-0.3.9/voila_materialscloud_template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2021-12-11 02:45:10.000000 voila-materialscloud-template-0.3.9/voila_materialscloud_template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2779 2021-12-11 02:45:10.000000 voila-materialscloud-template-0.3.9/voila_materialscloud_template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-11 02:45:10.000000 voila-materialscloud-template-0.3.9/voila_materialscloud_template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       88 2021-12-11 02:45:10.000000 voila-materialscloud-template-0.3.9/voila_materialscloud_template.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-11 02:45:10.000000 voila-materialscloud-template-0.3.9/voila_materialscloud_template.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.120934 voila_materialscloud_template-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-17 15:56:52.120934 voila_materialscloud_template-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3294 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/copy_voila_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-17 15:56:52.120934 voila_materialscloud_template-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-17 15:56:48.000000 voila_materialscloud_template-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.096933 voila_materialscloud_template-0.4.0/share/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.100934 voila_materialscloud_template-0.4.0/share/jupyter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.096933 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.096933 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.100934 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud/conf.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16864 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud/index.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.100934 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.116933 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   546493 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud/static/css/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)   140563 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud/static/css/mcloud_theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15629 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud/static/css/theme-dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud/static/css/theme-light.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.116933 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud/static/images/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud/static/images/mcloud_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud/static/images/mcloud_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9893 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud/static/images/mcloud_spinner.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.116933 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    17536 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud/static/js/require.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.100934 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-discover/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-discover/conf.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16607 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-discover/index.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.096933 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-discover/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.104934 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-discover/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   546493 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-discover/static/css/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)   140563 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-discover/static/css/mcloud_theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15629 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-discover/static/css/theme-dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-discover/static/css/theme-light.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.104934 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-discover/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-discover/static/images/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-discover/static/images/mcloud_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-discover/static/images/mcloud_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9893 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-discover/static/images/mcloud_spinner.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.104934 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-discover/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    17536 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-discover/static/js/require.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.104934 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-iframe/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-iframe/conf.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-iframe/index.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.096933 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-iframe/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.108934 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-iframe/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   546493 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-iframe/static/css/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)   140563 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-iframe/static/css/mcloud_theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15629 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-iframe/static/css/theme-dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-iframe/static/css/theme-light.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.108934 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    18197 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/MaterialsCloud_Horizontal_White.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/mcloud_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/mcloud_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9893 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/mcloud_spinner.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.108934 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    53386 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/iframeResizer.contentWindow.map
+-rw-r--r--   0 runner    (1001) docker     (127)    14147 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/iframeResizer.contentWindow.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17536 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/require.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.108934 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-tool/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-tool/conf.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16864 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-tool/index.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.100934 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-tool/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.112933 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-tool/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   546493 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-tool/static/css/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)   140563 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-tool/static/css/mcloud_theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15629 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-tool/static/css/theme-dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-tool/static/css/theme-light.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.112933 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-tool/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-tool/static/images/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-tool/static/images/mcloud_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-tool/static/images/mcloud_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9893 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-tool/static/images/mcloud_spinner.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.112933 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-tool/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    17536 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-tool/static/js/require.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.100934 voila_materialscloud_template-0.4.0/share/jupyter/voila/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.100934 voila_materialscloud_template-0.4.0/share/jupyter/voila/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.116933 voila_materialscloud_template-0.4.0/share/jupyter/voila/templates/materialscloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/voila/templates/materialscloud/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/voila/templates/materialscloud/index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/voila/templates/materialscloud/spinner.macro.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/voila/templates/materialscloud/tree.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.116933 voila_materialscloud_template-0.4.0/share/jupyter/voila/templates/materialscloud-discover/
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/voila/templates/materialscloud-discover/index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/voila/templates/materialscloud-discover/spinner.macro.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.116933 voila_materialscloud_template-0.4.0/share/jupyter/voila/templates/materialscloud-iframe/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/voila/templates/materialscloud-iframe/index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/voila/templates/materialscloud-iframe/spinner.macro.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.116933 voila_materialscloud_template-0.4.0/share/jupyter/voila/templates/materialscloud-tool/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/voila/templates/materialscloud-tool/index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-17 15:56:39.000000 voila_materialscloud_template-0.4.0/share/jupyter/voila/templates/materialscloud-tool/spinner.macro.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:52.120934 voila_materialscloud_template-0.4.0/voila_materialscloud_template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-17 15:56:52.000000 voila_materialscloud_template-0.4.0/voila_materialscloud_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-05-17 15:56:52.000000 voila_materialscloud_template-0.4.0/voila_materialscloud_template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 15:56:52.000000 voila_materialscloud_template-0.4.0/voila_materialscloud_template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-17 15:56:52.000000 voila_materialscloud_template-0.4.0/voila_materialscloud_template.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 15:56:52.000000 voila_materialscloud_template-0.4.0/voila_materialscloud_template.egg-info/top_level.txt
```

### Comparing `voila-materialscloud-template-0.3.9/LICENSE` & `voila_materialscloud_template-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/copy_voila_template.py` & `voila_materialscloud_template-0.4.0/copy_voila_template.py`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/setup.py` & `voila_materialscloud_template-0.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup
 from setuptools.command.develop import develop
 from setuptools.command.install import install
 
 def post_install():
     """Copy materialscloud templates' files to Jupyter config location"""
-    for template in ("materialscloud", "materialscloud-iframe"):
+    for template in ("materialscloud", "materialscloud-iframe", "materialscloud-tool", "materialscloud-discover"):
         check_call(['./copy_voila_template.py', template], cwd=TOP_DIR)
 
 class ExtraInstall(install):
     """Post-installation for installation (install) mode."""
 
     def run(self):
         """Install application and copy template files to Jupyter location afterwards."""
@@ -29,33 +29,37 @@
 
 
 TOP_DIR = Path(__file__).parent.resolve()
 
 with open(TOP_DIR.joinpath("README.md")) as handle:
     README = handle.read()
 
-with open(TOP_DIR.joinpath("requirements_base.txt")) as handle:
+with open(TOP_DIR.joinpath("requirements.txt")) as handle:
     REQUIREMENTS_BASE = [f"{_.strip()}" for _ in handle.readlines() if " " not in _]
 
 with open(TOP_DIR.joinpath("requirements_dev.txt")) as handle:
     REQUIREMENTS_DEV = [f"{_.strip()}" for _ in handle.readlines() if " " not in _]
 
 
 setup(
     name='voila-materialscloud-template',
-    version='0.3.9',
+    version='0.4.0',
     packages=[],
     author='Dou Du and Casper Welzel Andersen',
     author_email='dou.du@epfl.ch',
     url='https://github.com/materialscloud-org/voila-materialscloud-template',
     license='BSD',
     description='Voilà template for Materials Cloud that implements the Materials Cloud header and CSS.',
     long_description=README,
     long_description_content_type='text/markdown',
     keywords='voila jupyter materialscloud',
     cmdclass={
         'develop': ExtraDevelop,
         'install': ExtraInstall,
     },
+    setup_requires=[
+        'setuptools>=42.0.0',
+        'jupyter-core~=5.3.1',
+    ],
     install_requires=REQUIREMENTS_BASE,
     extras_require={'dev': REQUIREMENTS_DEV}
 )
```

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud/index.html.j2` & `voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud/index.html.j2`

 * *Files 0% similar despite different names*

```diff
@@ -393,17 +393,17 @@
           <a class="navbar-brand" href="https://www.materialscloud.org/home">
             <img src="{{ resources.base_url }}voila/static/images/mcloud_logo.png">
           </a>
         </div>
 
         <div class="collapse navbar-collapse header-collapse">
           <ul class="nav navbar-nav">
+            <li><a href="https://www.materialscloud.org/learn">LEARN</a></li>
             <li class="active"><a ui-sref="main.work" href="https://www.materialscloud.org/work">WORK</a></li>
             <li><a href="https://www.materialscloud.org/discover">DISCOVER</a></li>
-            <li class="active"><a ui-sref="main.discover" href="https://www.materialscloud.org/discover">DISCOVER</a></li>
             <li><a href="https://www.materialscloud.org/explore">EXPLORE</a></li>
             <li><a href="https://www.materialscloud.org/archive">ARCHIVE</a></li>
           </ul>
         </div>
       </div>
     </div>
   </header>
```

#### html2text {}

```diff
@@ -6,17 +6,17 @@
 bar_color = '#555454' %} {% else %} {% set bar_color = '#f3f700' %} {% endif %}
 {{ resources.include_css("static/css/mcloud_theme.min.css") }}
 {%- endblock html_head_css -%} {%- block body_header -%} {% if resources.theme
 == 'dark' %}
 {% else %}
 {% endif %} {{ spinner.html(resources.base_url) }}
 Toggle navigation_[_{_{_ _r_e_s_o_u_r_c_e_s_._b_a_s_e___u_r_l_ _}_}_v_o_i_l_a_/_s_t_a_t_i_c_/_i_m_a_g_e_s_/_m_c_l_o_u_d___l_o_g_o_._p_n_g_]
+    * _L_E_A_R_N
     * _W_O_R_K
     * _D_I_S_C_O_V_E_R
-    * _D_I_S_C_O_V_E_R
     * _E_X_P_L_O_R_E
     * _A_R_C_H_I_V_E
    1. _W_o_r_k
    2. _T_o_o_l_s
    3. {{nb_title}}
 {%- endblock body_header -%} {%- block body_loop -%} {% if resources.theme ==
 'dark' %}
```

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud/static/css/index.css` & `voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud/static/css/index.css`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud/static/css/mcloud_theme.min.css` & `voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud/static/css/mcloud_theme.min.css`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud/static/css/theme-dark.css` & `voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud/static/css/theme-dark.css`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud/static/css/theme-light.css` & `voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud/static/css/theme-light.css`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud/static/images/favicon.png` & `voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud/static/images/favicon.png`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud/static/images/mcloud_logo.png` & `voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud/static/images/mcloud_logo.png`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud/static/images/mcloud_logo.svg` & `voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud/static/images/mcloud_logo.svg`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud/static/images/mcloud_spinner.svg` & `voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud/static/images/mcloud_spinner.svg`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud/static/js/require.min.js` & `voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud/static/js/require.min.js`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/index.html.j2` & `voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-iframe/index.html.j2`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/css/index.css` & `voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-discover/static/css/index.css`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/css/mcloud_theme.min.css` & `voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-discover/static/css/mcloud_theme.min.css`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/css/theme-dark.css` & `voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-discover/static/css/theme-dark.css`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/css/theme-light.css` & `voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-discover/static/css/theme-light.css`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/MaterialsCloud_Horizontal_White.png` & `voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/MaterialsCloud_Horizontal_White.png`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/favicon.png` & `voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-discover/static/images/favicon.png`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/mcloud_logo.png` & `voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-discover/static/images/mcloud_logo.png`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/mcloud_logo.svg` & `voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-discover/static/images/mcloud_logo.svg`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/mcloud_spinner.svg` & `voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-discover/static/images/mcloud_spinner.svg`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/iframeResizer.contentWindow.map` & `voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/iframeResizer.contentWindow.map`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/iframeResizer.contentWindow.min.js` & `voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/iframeResizer.contentWindow.min.js`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/require.min.js` & `voila_materialscloud_template-0.4.0/share/jupyter/nbconvert/templates/materialscloud-discover/static/js/require.min.js`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/voila/templates/materialscloud/base.html` & `voila_materialscloud_template-0.4.0/share/jupyter/voila/templates/materialscloud/base.html`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/voila/templates/materialscloud/index.html.j2` & `voila_materialscloud_template-0.4.0/share/jupyter/voila/templates/materialscloud/index.html.j2`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/voila/templates/materialscloud/spinner.macro.html.j2` & `voila_materialscloud_template-0.4.0/share/jupyter/voila/templates/materialscloud/spinner.macro.html.j2`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/voila/templates/materialscloud-iframe/index.html.j2` & `voila_materialscloud_template-0.4.0/share/jupyter/voila/templates/materialscloud-iframe/index.html.j2`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/share/jupyter/voila/templates/materialscloud-iframe/spinner.macro.html.j2` & `voila_materialscloud_template-0.4.0/share/jupyter/voila/templates/materialscloud-discover/spinner.macro.html.j2`

 * *Files identical despite different names*

### Comparing `voila-materialscloud-template-0.3.9/voila_materialscloud_template.egg-info/SOURCES.txt` & `voila_materialscloud_template-0.4.0/voila_materialscloud_template.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,70 @@
 LICENSE
 MANIFEST.in
 README.md
 copy_voila_template.py
 requirements.txt
-requirements_base.txt
 requirements_dev.txt
 setup.cfg
 setup.py
 share/jupyter/nbconvert/templates/materialscloud/conf.json
 share/jupyter/nbconvert/templates/materialscloud/index.html.j2
+share/jupyter/nbconvert/templates/materialscloud-discover/conf.json
+share/jupyter/nbconvert/templates/materialscloud-discover/index.html.j2
+share/jupyter/nbconvert/templates/materialscloud-discover/static/css/index.css
+share/jupyter/nbconvert/templates/materialscloud-discover/static/css/mcloud_theme.min.css
+share/jupyter/nbconvert/templates/materialscloud-discover/static/css/theme-dark.css
+share/jupyter/nbconvert/templates/materialscloud-discover/static/css/theme-light.css
+share/jupyter/nbconvert/templates/materialscloud-discover/static/images/favicon.png
+share/jupyter/nbconvert/templates/materialscloud-discover/static/images/mcloud_logo.png
+share/jupyter/nbconvert/templates/materialscloud-discover/static/images/mcloud_logo.svg
+share/jupyter/nbconvert/templates/materialscloud-discover/static/images/mcloud_spinner.svg
+share/jupyter/nbconvert/templates/materialscloud-discover/static/js/require.min.js
 share/jupyter/nbconvert/templates/materialscloud-iframe/conf.json
 share/jupyter/nbconvert/templates/materialscloud-iframe/index.html.j2
 share/jupyter/nbconvert/templates/materialscloud-iframe/static/css/index.css
 share/jupyter/nbconvert/templates/materialscloud-iframe/static/css/mcloud_theme.min.css
 share/jupyter/nbconvert/templates/materialscloud-iframe/static/css/theme-dark.css
 share/jupyter/nbconvert/templates/materialscloud-iframe/static/css/theme-light.css
 share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/MaterialsCloud_Horizontal_White.png
 share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/favicon.png
 share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/mcloud_logo.png
 share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/mcloud_logo.svg
 share/jupyter/nbconvert/templates/materialscloud-iframe/static/images/mcloud_spinner.svg
 share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/iframeResizer.contentWindow.map
 share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/iframeResizer.contentWindow.min.js
 share/jupyter/nbconvert/templates/materialscloud-iframe/static/js/require.min.js
+share/jupyter/nbconvert/templates/materialscloud-tool/conf.json
+share/jupyter/nbconvert/templates/materialscloud-tool/index.html.j2
+share/jupyter/nbconvert/templates/materialscloud-tool/static/css/index.css
+share/jupyter/nbconvert/templates/materialscloud-tool/static/css/mcloud_theme.min.css
+share/jupyter/nbconvert/templates/materialscloud-tool/static/css/theme-dark.css
+share/jupyter/nbconvert/templates/materialscloud-tool/static/css/theme-light.css
+share/jupyter/nbconvert/templates/materialscloud-tool/static/images/favicon.png
+share/jupyter/nbconvert/templates/materialscloud-tool/static/images/mcloud_logo.png
+share/jupyter/nbconvert/templates/materialscloud-tool/static/images/mcloud_logo.svg
+share/jupyter/nbconvert/templates/materialscloud-tool/static/images/mcloud_spinner.svg
+share/jupyter/nbconvert/templates/materialscloud-tool/static/js/require.min.js
 share/jupyter/nbconvert/templates/materialscloud/static/css/index.css
 share/jupyter/nbconvert/templates/materialscloud/static/css/mcloud_theme.min.css
 share/jupyter/nbconvert/templates/materialscloud/static/css/theme-dark.css
 share/jupyter/nbconvert/templates/materialscloud/static/css/theme-light.css
 share/jupyter/nbconvert/templates/materialscloud/static/images/favicon.png
 share/jupyter/nbconvert/templates/materialscloud/static/images/mcloud_logo.png
 share/jupyter/nbconvert/templates/materialscloud/static/images/mcloud_logo.svg
 share/jupyter/nbconvert/templates/materialscloud/static/images/mcloud_spinner.svg
 share/jupyter/nbconvert/templates/materialscloud/static/js/require.min.js
 share/jupyter/voila/templates/materialscloud/base.html
 share/jupyter/voila/templates/materialscloud/index.html.j2
 share/jupyter/voila/templates/materialscloud/spinner.macro.html.j2
 share/jupyter/voila/templates/materialscloud/tree.html
+share/jupyter/voila/templates/materialscloud-discover/index.html.j2
+share/jupyter/voila/templates/materialscloud-discover/spinner.macro.html.j2
 share/jupyter/voila/templates/materialscloud-iframe/index.html.j2
 share/jupyter/voila/templates/materialscloud-iframe/spinner.macro.html.j2
+share/jupyter/voila/templates/materialscloud-tool/index.html.j2
+share/jupyter/voila/templates/materialscloud-tool/spinner.macro.html.j2
 voila_materialscloud_template.egg-info/PKG-INFO
 voila_materialscloud_template.egg-info/SOURCES.txt
 voila_materialscloud_template.egg-info/dependency_links.txt
 voila_materialscloud_template.egg-info/requires.txt
 voila_materialscloud_template.egg-info/top_level.txt
```

