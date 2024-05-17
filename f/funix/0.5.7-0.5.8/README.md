# Comparing `tmp/funix-0.5.7.tar.gz` & `tmp/funix-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funix-0.5.7.tar", last modified: Sat Apr 27 10:27:29 2024, max compression
+gzip compressed data, was "funix-0.5.8.tar", last modified: Fri May 17 13:28:16 2024, max compression
```

## Comparing `funix-0.5.7.tar` & `funix-0.5.8.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.438594 funix-0.5.7/
--rw-r--r--   0 yazawazi   (501) staff       (20)     1073 2023-03-14 06:41:17.000000 funix-0.5.7/LICENSE
--rw-r--r--   0 yazawazi   (501) staff       (20)       26 2023-03-14 06:41:17.000000 funix-0.5.7/MANIFEST.in
--rw-r--r--   0 yazawazi   (501) staff       (20)    24396 2024-04-27 10:27:29.438483 funix-0.5.7/PKG-INFO
--rw-r--r--   0 yazawazi   (501) staff       (20)    21517 2024-04-21 08:51:41.000000 funix-0.5.7/README.md
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.369733 funix-0.5.7/backend/
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.371875 funix-0.5.7/backend/funix/
--rw-r--r--   0 yazawazi   (501) staff       (20)    15566 2024-04-21 08:51:41.000000 funix-0.5.7/backend/funix/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     2889 2024-04-27 10:26:28.000000 funix-0.5.7/backend/funix/__main__.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.373265 funix-0.5.7/backend/funix/app/
--rw-r--r--   0 yazawazi   (501) staff       (20)     5281 2024-03-06 15:50:54.000000 funix-0.5.7/backend/funix/app/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)      928 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/app/websocket.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.374304 funix-0.5.7/backend/funix/build/
--rw-r--r--   0 yazawazi   (501) staff       (20)      240 2024-04-27 10:27:09.000000 funix-0.5.7/backend/funix/build/asset-manifest.json
--rw-r--r--   0 yazawazi   (501) staff       (20)     3870 2024-04-27 10:26:42.000000 funix-0.5.7/backend/funix/build/favicon.ico
--rw-r--r--   0 yazawazi   (501) staff       (20)      908 2024-04-27 10:27:09.000000 funix-0.5.7/backend/funix/build/index.html
--rw-r--r--   0 yazawazi   (501) staff       (20)     5347 2024-04-27 10:26:42.000000 funix-0.5.7/backend/funix/build/logo192.png
--rw-r--r--   0 yazawazi   (501) staff       (20)     9664 2024-04-27 10:26:42.000000 funix-0.5.7/backend/funix/build/logo512.png
--rw-r--r--   0 yazawazi   (501) staff       (20)      492 2024-04-27 10:26:42.000000 funix-0.5.7/backend/funix/build/manifest.json
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.369989 funix-0.5.7/backend/funix/build/static/
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.374426 funix-0.5.7/backend/funix/build/static/css/
--rw-r--r--   0 yazawazi   (501) staff       (20)      292 2024-04-27 10:27:09.000000 funix-0.5.7/backend/funix/build/static/css/main.4efb37a3.css
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.425317 funix-0.5.7/backend/funix/build/static/js/
--rw-r--r--   0 yazawazi   (501) staff       (20)   515704 2024-04-27 10:27:09.000000 funix-0.5.7/backend/funix/build/static/js/d3.v5.js
--rw-r--r--   0 yazawazi   (501) staff       (20)    87533 2024-04-27 10:27:09.000000 funix-0.5.7/backend/funix/build/static/js/jquery-3.7.1.min.js
--rw-r--r--   0 yazawazi   (501) staff       (20)  7402218 2024-04-27 10:27:09.000000 funix-0.5.7/backend/funix/build/static/js/main.0af491b9.js
--rw-r--r--   0 yazawazi   (501) staff       (20)     3956 2024-04-27 10:27:09.000000 funix-0.5.7/backend/funix/build/static/js/main.0af491b9.js.LICENSE.txt
--rw-r--r--   0 yazawazi   (501) staff       (20)    63820 2024-04-27 10:27:09.000000 funix-0.5.7/backend/funix/build/static/js/mpld3.v0.5.8.js
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.426500 funix-0.5.7/backend/funix/config/
--rw-r--r--   0 yazawazi   (501) staff       (20)     1931 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/config/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     1348 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/config/switch.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.432939 funix-0.5.7/backend/funix/decorator/
--rw-r--r--   0 yazawazi   (501) staff       (20)    22172 2024-04-21 08:51:41.000000 funix-0.5.7/backend/funix/decorator/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)      958 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/decorator/all_of.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     4396 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/decorator/annnotation_analyzer.py
--rw-r--r--   0 yazawazi   (501) staff       (20)    12930 2024-04-21 08:51:41.000000 funix-0.5.7/backend/funix/decorator/call.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     6201 2024-04-21 08:51:41.000000 funix-0.5.7/backend/funix/decorator/file.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     3355 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/decorator/layout.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     5898 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/decorator/limit.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     3608 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/decorator/lists.py
--rw-r--r--   0 yazawazi   (501) staff       (20)    29288 2024-04-21 08:51:41.000000 funix-0.5.7/backend/funix/decorator/magic.py
--rw-r--r--   0 yazawazi   (501) staff       (20)    14042 2024-04-21 08:51:41.000000 funix-0.5.7/backend/funix/decorator/param.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     1396 2024-04-21 08:51:41.000000 funix-0.5.7/backend/funix/decorator/pre_fill.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     2814 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/decorator/reactive.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     7877 2024-03-26 05:59:46.000000 funix-0.5.7/backend/funix/decorator/runtime.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     2633 2024-04-21 08:51:41.000000 funix-0.5.7/backend/funix/decorator/secret.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     2782 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/decorator/theme.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     9228 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/decorator/widget.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.433174 funix-0.5.7/backend/funix/frontend/
--rw-r--r--   0 yazawazi   (501) staff       (20)     3462 2023-12-30 15:45:03.000000 funix-0.5.7/backend/funix/frontend/__init__.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.433697 funix-0.5.7/backend/funix/hint/
--rw-r--r--   0 yazawazi   (501) staff       (20)    14979 2024-03-26 06:15:40.000000 funix-0.5.7/backend/funix/hint/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     3842 2023-08-26 09:53:24.000000 funix-0.5.7/backend/funix/hint/layout.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.434009 funix-0.5.7/backend/funix/prep/
--rw-r--r--   0 yazawazi   (501) staff       (20)        0 2023-05-23 09:39:39.000000 funix-0.5.7/backend/funix/prep/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     5374 2024-04-21 08:51:41.000000 funix-0.5.7/backend/funix/prep/global_to_session.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.434299 funix-0.5.7/backend/funix/session/
--rw-r--r--   0 yazawazi   (501) staff       (20)     2310 2024-03-06 15:26:16.000000 funix-0.5.7/backend/funix/session/__init__.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.434523 funix-0.5.7/backend/funix/test/
--rw-r--r--   0 yazawazi   (501) staff       (20)     5415 2023-08-25 18:04:39.000000 funix-0.5.7/backend/funix/test/test_magic.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.434759 funix-0.5.7/backend/funix/theme/
--rw-r--r--   0 yazawazi   (501) staff       (20)    11239 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/theme/__init__.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.436514 funix-0.5.7/backend/funix/util/
--rw-r--r--   0 yazawazi   (501) staff       (20)        0 2023-05-23 03:43:55.000000 funix-0.5.7/backend/funix/util/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     2852 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/util/file.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     3518 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/util/module.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     4132 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/util/network.py
--rw-r--r--   0 yazawazi   (501) staff       (20)      973 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/util/secret.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     1067 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/util/text.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     1436 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/util/uri.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.436998 funix-0.5.7/backend/funix/widget/
--rw-r--r--   0 yazawazi   (501) staff       (20)     6516 2024-02-28 11:05:47.000000 funix-0.5.7/backend/funix/widget/__init__.py
--rw-r--r--   0 yazawazi   (501) staff       (20)     5067 2023-09-25 00:17:50.000000 funix-0.5.7/backend/funix/widget/builtin.py
-drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-04-27 10:27:29.437317 funix-0.5.7/backend/funix.egg-info/
--rw-r--r--   0 yazawazi   (501) staff       (20)    24396 2024-04-27 10:27:29.000000 funix-0.5.7/backend/funix.egg-info/PKG-INFO
--rw-r--r--   0 yazawazi   (501) staff       (20)     2031 2024-04-27 10:27:29.000000 funix-0.5.7/backend/funix.egg-info/SOURCES.txt
--rw-r--r--   0 yazawazi   (501) staff       (20)        1 2024-04-27 10:27:29.000000 funix-0.5.7/backend/funix.egg-info/dependency_links.txt
--rw-r--r--   0 yazawazi   (501) staff       (20)       50 2024-04-27 10:27:29.000000 funix-0.5.7/backend/funix.egg-info/entry_points.txt
--rw-r--r--   0 yazawazi   (501) staff       (20)      397 2024-04-27 10:27:29.000000 funix-0.5.7/backend/funix.egg-info/requires.txt
--rw-r--r--   0 yazawazi   (501) staff       (20)        6 2024-04-27 10:27:29.000000 funix-0.5.7/backend/funix.egg-info/top_level.txt
--rw-r--r--   0 yazawazi   (501) staff       (20)     1269 2024-04-27 10:26:28.000000 funix-0.5.7/pyproject.toml
--rw-r--r--   0 yazawazi   (501) staff       (20)      114 2024-04-27 10:27:29.438874 funix-0.5.7/setup.cfg
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-05-17 13:28:16.229767 funix-0.5.8/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     1073 2023-03-14 06:41:17.000000 funix-0.5.8/LICENSE
+-rw-r--r--   0 yazawazi   (501) staff       (20)       26 2023-03-14 06:41:17.000000 funix-0.5.8/MANIFEST.in
+-rw-r--r--   0 yazawazi   (501) staff       (20)    24874 2024-05-17 13:28:16.229692 funix-0.5.8/PKG-INFO
+-rw-r--r--   0 yazawazi   (501) staff       (20)    22291 2024-05-17 13:27:42.000000 funix-0.5.8/README.md
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-05-17 13:28:16.168527 funix-0.5.8/backend/
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-05-17 13:28:16.171175 funix-0.5.8/backend/funix/
+-rw-r--r--   0 yazawazi   (501) staff       (20)    15516 2024-05-09 05:34:44.000000 funix-0.5.8/backend/funix/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     2889 2024-05-17 13:28:05.000000 funix-0.5.8/backend/funix/__main__.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-05-17 13:28:16.173004 funix-0.5.8/backend/funix/app/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     5550 2024-05-08 21:24:29.000000 funix-0.5.8/backend/funix/app/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)      928 2024-02-28 11:05:47.000000 funix-0.5.8/backend/funix/app/websocket.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-05-17 13:28:16.174218 funix-0.5.8/backend/funix/build/
+-rw-r--r--   0 yazawazi   (501) staff       (20)      240 2024-05-17 13:25:56.000000 funix-0.5.8/backend/funix/build/asset-manifest.json
+-rw-r--r--   0 yazawazi   (501) staff       (20)     3870 2024-05-17 13:25:31.000000 funix-0.5.8/backend/funix/build/favicon.ico
+-rw-r--r--   0 yazawazi   (501) staff       (20)      908 2024-05-17 13:25:56.000000 funix-0.5.8/backend/funix/build/index.html
+-rw-r--r--   0 yazawazi   (501) staff       (20)     5347 2024-05-17 13:25:31.000000 funix-0.5.8/backend/funix/build/logo192.png
+-rw-r--r--   0 yazawazi   (501) staff       (20)     9664 2024-05-17 13:25:31.000000 funix-0.5.8/backend/funix/build/logo512.png
+-rw-r--r--   0 yazawazi   (501) staff       (20)      492 2024-05-17 13:25:31.000000 funix-0.5.8/backend/funix/build/manifest.json
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-05-17 13:28:16.168873 funix-0.5.8/backend/funix/build/static/
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-05-17 13:28:16.174378 funix-0.5.8/backend/funix/build/static/css/
+-rw-r--r--   0 yazawazi   (501) staff       (20)      292 2024-05-17 13:25:56.000000 funix-0.5.8/backend/funix/build/static/css/main.4efb37a3.css
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-05-17 13:28:16.214511 funix-0.5.8/backend/funix/build/static/js/
+-rw-r--r--   0 yazawazi   (501) staff       (20)   515704 2024-05-17 13:25:56.000000 funix-0.5.8/backend/funix/build/static/js/d3.v5.js
+-rw-r--r--   0 yazawazi   (501) staff       (20)    87533 2024-05-17 13:25:56.000000 funix-0.5.8/backend/funix/build/static/js/jquery-3.7.1.min.js
+-rw-r--r--   0 yazawazi   (501) staff       (20)  7402398 2024-05-17 13:25:56.000000 funix-0.5.8/backend/funix/build/static/js/main.279c7e85.js
+-rw-r--r--   0 yazawazi   (501) staff       (20)     3956 2024-05-17 13:25:56.000000 funix-0.5.8/backend/funix/build/static/js/main.279c7e85.js.LICENSE.txt
+-rw-r--r--   0 yazawazi   (501) staff       (20)    63820 2024-05-17 13:25:56.000000 funix-0.5.8/backend/funix/build/static/js/mpld3.v0.5.8.js
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-05-17 13:28:16.216930 funix-0.5.8/backend/funix/config/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     1931 2024-02-28 11:05:47.000000 funix-0.5.8/backend/funix/config/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     1348 2024-02-28 11:05:47.000000 funix-0.5.8/backend/funix/config/switch.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-05-17 13:28:16.224410 funix-0.5.8/backend/funix/decorator/
+-rw-r--r--   0 yazawazi   (501) staff       (20)    21852 2024-05-08 20:07:02.000000 funix-0.5.8/backend/funix/decorator/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)      958 2024-02-28 11:05:47.000000 funix-0.5.8/backend/funix/decorator/all_of.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     4396 2024-05-17 13:25:16.000000 funix-0.5.8/backend/funix/decorator/annnotation_analyzer.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)    12930 2024-05-08 20:07:02.000000 funix-0.5.8/backend/funix/decorator/call.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     6201 2024-04-21 08:51:41.000000 funix-0.5.8/backend/funix/decorator/file.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     3365 2024-05-08 20:08:10.000000 funix-0.5.8/backend/funix/decorator/layout.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     5898 2024-02-28 11:05:47.000000 funix-0.5.8/backend/funix/decorator/limit.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     3608 2024-02-28 11:05:47.000000 funix-0.5.8/backend/funix/decorator/lists.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)    29293 2024-05-08 20:08:42.000000 funix-0.5.8/backend/funix/decorator/magic.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)    14042 2024-05-08 20:07:02.000000 funix-0.5.8/backend/funix/decorator/param.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     1396 2024-04-21 08:51:41.000000 funix-0.5.8/backend/funix/decorator/pre_fill.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     2814 2024-02-28 11:05:47.000000 funix-0.5.8/backend/funix/decorator/reactive.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     7877 2024-05-08 20:07:02.000000 funix-0.5.8/backend/funix/decorator/runtime.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     2633 2024-04-21 08:51:41.000000 funix-0.5.8/backend/funix/decorator/secret.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     2782 2024-02-28 11:05:47.000000 funix-0.5.8/backend/funix/decorator/theme.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     9228 2024-02-28 11:05:47.000000 funix-0.5.8/backend/funix/decorator/widget.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-05-17 13:28:16.224813 funix-0.5.8/backend/funix/frontend/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     3462 2023-12-30 15:45:03.000000 funix-0.5.8/backend/funix/frontend/__init__.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-05-17 13:28:16.225450 funix-0.5.8/backend/funix/hint/
+-rw-r--r--   0 yazawazi   (501) staff       (20)    15084 2024-05-08 20:09:26.000000 funix-0.5.8/backend/funix/hint/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     3842 2023-08-26 09:53:24.000000 funix-0.5.8/backend/funix/hint/layout.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-05-17 13:28:16.225782 funix-0.5.8/backend/funix/prep/
+-rw-r--r--   0 yazawazi   (501) staff       (20)        0 2023-05-23 09:39:39.000000 funix-0.5.8/backend/funix/prep/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     5374 2024-04-21 08:51:41.000000 funix-0.5.8/backend/funix/prep/global_to_session.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-05-17 13:28:16.226036 funix-0.5.8/backend/funix/session/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     2310 2024-03-06 15:26:16.000000 funix-0.5.8/backend/funix/session/__init__.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-05-17 13:28:16.226297 funix-0.5.8/backend/funix/test/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     5415 2023-08-25 18:04:39.000000 funix-0.5.8/backend/funix/test/test_magic.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-05-17 13:28:16.226556 funix-0.5.8/backend/funix/theme/
+-rw-r--r--   0 yazawazi   (501) staff       (20)    11239 2024-02-28 11:05:47.000000 funix-0.5.8/backend/funix/theme/__init__.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-05-17 13:28:16.228184 funix-0.5.8/backend/funix/util/
+-rw-r--r--   0 yazawazi   (501) staff       (20)        0 2023-05-23 03:43:55.000000 funix-0.5.8/backend/funix/util/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     2964 2024-05-09 05:39:50.000000 funix-0.5.8/backend/funix/util/file.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     3518 2024-02-28 11:05:47.000000 funix-0.5.8/backend/funix/util/module.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     4120 2024-05-08 20:11:05.000000 funix-0.5.8/backend/funix/util/network.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)      973 2024-02-28 11:05:47.000000 funix-0.5.8/backend/funix/util/secret.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     1067 2024-02-28 11:05:47.000000 funix-0.5.8/backend/funix/util/text.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     1436 2024-02-28 11:05:47.000000 funix-0.5.8/backend/funix/util/uri.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-05-17 13:28:16.228671 funix-0.5.8/backend/funix/widget/
+-rw-r--r--   0 yazawazi   (501) staff       (20)     6531 2024-05-08 20:11:47.000000 funix-0.5.8/backend/funix/widget/__init__.py
+-rw-r--r--   0 yazawazi   (501) staff       (20)     5067 2023-09-25 00:17:50.000000 funix-0.5.8/backend/funix/widget/builtin.py
+drwxr-xr-x   0 yazawazi   (501) staff       (20)        0 2024-05-17 13:28:16.228950 funix-0.5.8/backend/funix.egg-info/
+-rw-r--r--   0 yazawazi   (501) staff       (20)    24874 2024-05-17 13:28:16.000000 funix-0.5.8/backend/funix.egg-info/PKG-INFO
+-rw-r--r--   0 yazawazi   (501) staff       (20)     2031 2024-05-17 13:28:16.000000 funix-0.5.8/backend/funix.egg-info/SOURCES.txt
+-rw-r--r--   0 yazawazi   (501) staff       (20)        1 2024-05-17 13:28:16.000000 funix-0.5.8/backend/funix.egg-info/dependency_links.txt
+-rw-r--r--   0 yazawazi   (501) staff       (20)       50 2024-05-17 13:28:16.000000 funix-0.5.8/backend/funix.egg-info/entry_points.txt
+-rw-r--r--   0 yazawazi   (501) staff       (20)      318 2024-05-17 13:28:16.000000 funix-0.5.8/backend/funix.egg-info/requires.txt
+-rw-r--r--   0 yazawazi   (501) staff       (20)        6 2024-05-17 13:28:16.000000 funix-0.5.8/backend/funix.egg-info/top_level.txt
+-rw-r--r--   0 yazawazi   (501) staff       (20)     1171 2024-05-17 13:28:05.000000 funix-0.5.8/pyproject.toml
+-rw-r--r--   0 yazawazi   (501) staff       (20)      114 2024-05-17 13:28:16.230023 funix-0.5.8/setup.cfg
```

### Comparing `funix-0.5.7/LICENSE` & `funix-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/PKG-INFO` & `funix-0.5.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: funix
-Version: 0.5.7
+Version: 0.5.8
 Summary: Building web apps without manually creating widgets
-Author-email: "Textea Inc." <hello@funix.io>
+Author-email: "Textea Inc." <forrestbao@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 Textea Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -39,33 +39,27 @@
 Requires-Dist: flask>=2.2.2
 Requires-Dist: functions-framework==3.*
 Requires-Dist: requests>=2.28.1
 Requires-Dist: plac>=1.3.5
 Requires-Dist: gitignore-parser>=0.1.9
 Requires-Dist: flask-sock>=0.7.0
 Requires-Dist: SQLAlchemy>=2.0.23
-Provides-Extra: plot
-Requires-Dist: matplotlib>=3.4.3; extra == "plot"
-Requires-Dist: mpld3>=0.5.8; extra == "plot"
+Requires-Dist: matplotlib>=3.4.3
+Requires-Dist: mpld3>=0.5.8
+Requires-Dist: pandera>=0.17.2
+Requires-Dist: pandas>=2.0.3
 Provides-Extra: git
 Requires-Dist: GitPython>=3.1.31; extra == "git"
 Provides-Extra: ipython
 Requires-Dist: IPython>=8.14.0; extra == "ipython"
 Requires-Dist: ipywidgets>=8.0.7; extra == "ipython"
-Provides-Extra: pandas
-Requires-Dist: pandera>=0.17.2; extra == "pandas"
-Requires-Dist: pandas>=2.0.3; extra == "pandas"
 Provides-Extra: all
-Requires-Dist: matplotlib>=3.4.3; extra == "all"
-Requires-Dist: mpld3>=0.5.8; extra == "all"
 Requires-Dist: GitPython>=3.1.31; extra == "all"
 Requires-Dist: IPython>=8.14.0; extra == "all"
 Requires-Dist: ipywidgets>=8.0.7; extra == "all"
-Requires-Dist: pandera>=0.17.2; extra == "all"
-Requires-Dist: pandas>=2.0.3; extra == "all"
 
 <h1 align="center">
     <!-- <b> -->
         Funix.io<br>
     <!-- </b> -->
     The laziest way to build AI/Data apps in Python
 </h1>
@@ -78,22 +72,23 @@
 
 <h4><a href="https://youtu.be/qDkzXS270Zo">Intro video</a> | <a href="#getting-started-with-funix">Getting started</a> |  <a href="#gallery"> Gallery </a> | <a href="https://github.com/TexteaInc/funix-doc/blob/main/Reference.md">Reference Manual</a> </h4>
 
 https://github.com/TexteaInc/funix/assets/438579/86868ab5-ed6e-46e5-8dc5-9e3e4a3cdc3f
 
 </div>
 
-## What is Funix? 
+## What is Funix?
 
 * Funix automatically turns an ordinary Python function or class definition into a web app, which is accessible in a browser via a shareable link. 
 * Funix is the frontend/backend/fullstack engineer and the infra/ops engineer for AI/Data/Science solo stars like you. 
 * Funix is the no-/low-code solution for those who write the most core and innovative code. 
 * Funix is open-source and can be deployed on-premises. 
 
 ## Use cases
+
 * Startups: quickly build demos, iterate on MVPs, get user feedback and statistics, and pitch to investors or your mom. 
 * Generative AI: instantly allow people to interact your GenAI model or idea.
 * STEM research: let people run your model and/or algorithm effortlessly. 
 * Data browser: an interface to page through your data. 
 * A/B test and data labeling: collect human labeling or preference.
 
 ## Key advantages
@@ -134,19 +129,17 @@
     ![screenshots/hello.png](https://github.com/TexteaInc/funix-doc/raw/main/screenshots/hello.png)
 
 
 <!-- > **Note**: The `-l` flag stands for _"lazy"_ meaning that only default settings are used. It cannot be used when your function is decorated by the funix decorator `@funix()` which allows you to customize your app. For more details, please refer to the [reference manual]([docs/Reference.md](https://github.com/TexteaInc/funix-doc/blob/main/Reference.md)). -->
 
 ## Getting started with Funix
 
-**The Zen of Funix** is to generate widgets for function I/Os based on their types, instead of manually picking and customizing the widget for each I/O. **Funix to Python is like CSS to HTML or style class to LaTeX**. UI stuff is not intermingled with the core logic but defined separately. The type-to-widget mapping is controlled by a theme and new types can be defined on top of existing types. 
-
-
-The example below shows how common UI compoents are generated from four Python-native data types: `str`, `bool`, `Literal` and `range`, as well as types in popular packages such as `ipywidgets.Password`. The example below further maps default values to placeholders in the UI widgets. From this example, we can see that developers need to **learn nothing about Funix or do nothing to their existing code** before they can get an app. 
+**The Zen of Funix** is to generate widgets for function I/Os based on their types, instead of manually picking and customizing the widget for each I/O. **Funix to Python is like CSS to HTML or style class to LaTeX**. UI stuff is not intermingled with the core logic but defined separately. The type-to-widget mapping is controlled by a theme and new types can be defined on top of existing types.
 
+The example below shows how common UI compoents are generated from four Python-native data types: `str`, `bool`, `Literal` and `range`, as well as types in popular packages such as `ipywidgets.Password`. The example below further maps default values to placeholders in the UI widgets. From this example, we can see that developers need to **learn nothing about Funix or do nothing to their existing code** before they can get an app.
 
 ```python
 import typing # Python native 
 
 import ipywidgets  # popular UI library 
 
 def input_widgets_basic(
@@ -157,15 +150,15 @@
     openai_key: ipywidgets.Password = "1234556",
     )  -> str:
     pass
 ```
 
 ![four input types](https://raw.githubusercontent.com/TexteaInc/funix-doc/main/screenshots/input_widgets.png)
 
-The example below shows how `pandas.DataFrame` and `matplotlib.figure.Figure` that AI/data developers cannot be more familiar with are mapped to tables and charts in an app. 
+The example below shows how `pandas.DataFrame` and `matplotlib.figure.Figure` that AI/data developers cannot be more familiar with are mapped to tables and charts in an app.
 
 ```python
 import pandas, matplotlib.pyplot
 from numpy import arange, log
 from numpy.random import random
 
 def table_and_plot(
@@ -180,15 +173,15 @@
     matplotlib.pyplot.plot(df["a"], df["c"], 'r')
 
     return fig
 ```
 
 ![table and plot screenshot](https://raw.githubusercontent.com/TexteaInc/funix-doc/main/screenshots/table_plot.png)
 
-You can even continuously update a plot based on user input. 
+You can even continuously update a plot based on user input.
 
 ```python
 import funix 
 import matplotlib.pyplot, matplotlib.figure
 import numpy 
 
 @funix.funix(
@@ -200,76 +193,72 @@
     y = numpy.sin(x*omega)
     matplotlib.pyplot.plot(x, y, linewidth=5)
     return fig
 ```
 
 ![continuous sine function](https://raw.githubusercontent.com/TexteaInc/funix-doc/main/screenshots/continous_run_sine.gif)
 
- 
 ### Out-of-box support for classes and OOP
 
 Funix can turn each member method of a class into a page of an app. 
 In two additional lines, the example below turn a class definition into a multi-page app with the OOP experience where the instantiation of an object of the class is done in a page corresponding to the constructor of the class and the member values of the object can be viewed and updated in other pages. **No need to manually expose** the member methods of the class.
 
 ```python
 from funix import funix_class
 
 @funix_class()  
 class A:
     def __init__(self, a: int):
         self.a = a
         return f"`self.a` has been initialized to {self.a}"
 
-    def update_a(self, b: int) -> str:
+    def set(self, b: int) -> str:
         self.a = b
         return f"`self.a` has been updated to {self.a}"
 
-    def print_a(self) -> str:
+    def get(self) -> str:
         return f"The value of `self.a` is {self.a}"
 ```
 
 ![class demo app gif](https://raw.githubusercontent.com/TexteaInc/funix-doc/main/videos/class/class.gif)
 
-
 A more advanced example of class is the wordle game. You can find the source code in [`examples/wordle.py`](./examples/games/wordle.py). In less than 100 lines, you can build Wordle! The screenshot is as follows:
 
 ![Wordle demo](https://github.com/TexteaInc/funix-doc/blob/main/screenshots/wordle.png?raw=true)
 
 ### The quickest way to build GenAI apps
 
 You can wrap any Python function into a web app in Funix.
-For example, you can take the ChatGPT demo code from OpenAI's APi reference and wrap it into a str-to-str function: 
+For example, you can take the ChatGPT demo code from OpenAI's APi reference and wrap it into a str-to-str function:
 
 ```python
 from openai import OpenAI
 
 def ChatGPT(prompt: str) -> str:    
     client = OpenAI()
 
     completion = client.chat.completions.create(
         model="gpt-3.5-turbo",
         messages=[
             {"role": "user", "content": prompt}
         ]
     )
-return completion.choices[0].message
+    return completion.choices[0].message.content
 ```
+
 which is turned into an app by Funix like below: 
 
 ![screenshots/ChatGPT_lazy.png](https://github.com/TexteaInc/funix-doc/raw/main/screenshots/chatGPT_lazy.png)
 
+### Themes: the CSS for Python
 
+**Funix to Python is like CSS to HTML or macros to LaTeX.** It separates the core logic and the UI.
+All UI stuff is centrally defined in a JSON-based theme to avoid the repetitiveness of individually configuring widgets and keep a consistent look across apps. Consequently, a data scientist or a machine learning engineer does not need to think about anything UI. Just leave it to the UI team and Funix.
 
-
-### Themes: the CSS for Python 
-
-**Funix to Python is like CSS to HTML or macros to LaTeX.** It separates the core logic and the UI. 
-All UI stuff is centrally defined in a JSON-based theme to avoid the repetitiveness of individually configuring widgets and keep a consistent look across apps. Consequently, a data scientist or a machine learning engineer does not need to think about anything UI. Just leave it to the UI team and Funix. 
-
-Below is an example of a theme file. It defines the widget choices based on variable types and tweaks the `props` of UI components (currently only MUI ones are supported). Funix exposes frontend components and their `props` to developers, requiring them to know nothing about frontend. To know more about how to define and apply a theme, please refer to [the Themes section in the reference manual](https://github.com/TexteaInc/funix-doc/blob/main/Reference.md#themes). 
+Below is an example of a theme file. It defines the widget choices based on variable types and tweaks the `props` of UI components (currently only MUI ones are supported). Funix exposes frontend components and their `props` to developers, requiring them to know nothing about frontend. To know more about how to define and apply a theme, please refer to [the Themes section in the reference manual](https://github.com/TexteaInc/funix-doc/blob/main/Reference.md#themes).
 
 ```jsonc
 {
   "name": "test_theme",
   "widgets": {    // dict, map types to widgets
     "str": "inputbox", // using Funix' widget shorthand
     "int": "slider[0,100,2]", // using Funix' widget shorthand
@@ -283,15 +272,15 @@
         }
     }, 
     "Literal": "radio"
   },
 }
 ```
 
-To introduce a new data type, just declare a new Python class, and use a decorator to let Funix know. You can associate the type with a widget either on-the-fly (below) or via a theme file. 
+To introduce a new data type, just declare a new Python class, and use a decorator to let Funix know. You can associate the type with a widget either on-the-fly (below) or via a theme file.
 
 ```python
 from funix import funix, new_funix_type
 
 @new_funix_type(
     widget = {
         "widget": "@mui/material/TextField",
@@ -311,15 +300,15 @@
 
 if __name__ == "__main__":
     print (hoho(blackout('Fun'))) 
 ```
 
 ### Python-native to web-native
 
-Funix repurposes some Python-native features to web features. 
+Funix repurposes some Python-native features to web features.
 
 First, Funix won't let your docstring or `print()` function calls go to waste. They will appear in the input and output panels of the web app.
 
 ```python
 from funix import funix
 @funix(
     print_to_web=True
@@ -351,15 +340,15 @@
     for i in range(len(message)):
         time.sleep(0.01)
         yield message[0:i]
 ```
 
 ![Streamt text to web](https://github.com/TexteaInc/funix-doc/blob/main/screenshots/stream.gif?raw=true)
 
-## Advanced features 
+## Advanced features
 
 ### History: Keep your call logs
 
 <details>
 <summary>
 Click to expand
 </summary>
@@ -409,20 +398,23 @@
 
 A special case of passing data between functions is to use the return value of one function as the value in the widget of an argument of another function. This is called prefill. Funix support prefill by using a decorator attribute `pre_fill`. Below is an example and the corresponding GIF animation.
 
 
 ```python
 import funix
 
+@funix.funix()
 def first_action(x: int) -> int:
   return x - 1
 
+@funix.funix()
 def second_action(message: str) -> list[str]:
   return message.split(" ")
 
+@funix.funix()
 def third_action(x: int, y: int) -> dict:
   return {"x": x, "y": y}
 
 @funix.funix(
   pre_fill={
     "a": first_action,
     "b": (second_action, -1),
@@ -474,48 +466,52 @@
 
 More examples in <a href="https://github.com/TexteaInc/funix-doc/blob/main/Reference.md">Reference Manual</a> or the <code>./examples</code> folder.
 
 * [ChatPaper](https://github.com/forrestbao/ChatPaper) (It's like the popular ChatPDF. But in Funix, only 70 lines of code needed.)
 * [mFlux](https://github.com/Yazawazi/MFlux) (synthetic biology)
 
 ### ChatGPT, multi-turn
+
 <details>
   <summary><code>examples/AI/chatGPT_multi_turn.py</code> 👈 Toggle me to show source code </summary>
 
   ```python
     import os
     import IPython     
-    import openai
-    openai.api_key = os.environ.get("OPENAI_KEY")
+    from openai import OpenAI
+    import funix
+
+    client = OpenAI(api_key=os.environ.get("OPENAI_KEY"))
 
     messages  = []  # list of dicts, dict keys: role, content, system
 
+    @funix.funix(
+        disable=True,
+    )
     def print_messages_html(messages):
         printout = ""
         for message in messages:
             if message["role"] == "user":
-                align, left, name = "left", "0%", "You"
+                align, name = "left", "You"
             elif message["role"] == "assistant":
-                align, left, name = "right", "30%", "ChatGPT"
-            printout += f'<div style="position: relative; left: {left}; width: 70%"><b>{name}</b>: {message["content"]}</div>'
+                align, name = "right", "ChatGPT"
+            printout += f'<div style="width: 100%; text-align: {align}"><b>{name}</b>: {message["content"]}</div>'
         return printout
 
-    import funix
+
     @funix.funix(
         direction="column-reverse",
     )
     def ChatGPT_multi_turn(current_message: str)  -> IPython.display.HTML:
         current_message = current_message.strip()
         messages.append({"role": "user", "content": current_message})
-        completion = openai.ChatCompletion.create(
-            messages=messages,
-            model='gpt-3.5-turbo',
-            max_tokens=100,
-        )
-        chatgpt_response = completion["choices"][0]["message"]["content"]
+        completion = client.chat.completions.create(messages=messages,
+        model='gpt-3.5-turbo',
+        max_tokens=100)
+        chatgpt_response = completion.choices[0].message.content
         messages.append({"role": "assistant", "content": chatgpt_response})
 
         # return print_messages_markdown(messages)
         return print_messages_html(messages)
 
   ```
 
@@ -523,23 +519,25 @@
 
 ![Multiturn chat](https://github.com/TexteaInc/funix-doc/raw/main/screenshots/chatGPT_multiturn.png)
 
 ### Shortest Dall-E web app in Python
 
 ```python
 from funix import funix                      # add line one
-from funix.hint import Images                # add line two
-import openai  # pip install openai
+from IPython.display import Image
+from openai import OpenAI                    # pip install openai
+
+import os
+client = OpenAI(api_key=os.environ.get("OPENAI_KEY"))  
 
-openai.api_key = os.environ.get("OPENAI_KEY")
 
-@funix()                                     # add line three
+@funix()                                     # add line two
 def dalle(prompt: str = "a cat") -> Image:
-    response = openai.Image.create(prompt=prompt)
-    return response["data"][0]["url"]
+    response = client.images.generate(prompt=prompt)
+    return response.data[0].url
 ```
 
 ![Dalle demo](https://github.com/TexteaInc/funix-doc/raw/main/screenshots/dalle.jpg)
 
 <!-- Funix.io can get the same job done in half the amount of code required by Gradio, by exploiting the Python language as much as possible. Here, state/session is maintained using a global variable, while the order of the returns defines the return layout.  -->
 
 ### Bioinformatics: vector stripping
@@ -550,25 +548,26 @@
 
 ### Multimedia inputs and outputs
 
 <details>
 <summary><code>examples/multimedia/rgb2gray.py</code> 👈 Toggle me to show source code</summary>
 
 ```python
-import  io # Python's native
+import  io # Python's native 
 
 import PIL # the Python Image Library
-import funix
+import IPython 
+import funix 
 
 @funix.funix(
     title="Convert color images to grayscale images",
 )
-def gray_it(image: funix.hint.BytesImage) -> funix.hint.Image:
+def gray_it(image: funix.hint.BytesImage) -> IPython.display.Image:
     img = PIL.Image.open(io.BytesIO(image))
-    gray = PIL.ImageOps.grayscale(img)
+    gray = PIL.ImageOps.grayscale(img) 
     output = io.BytesIO()
     gray.save(output, format="PNG")
     return output.getvalue()
 ```
 </details>
 
 ![shipping example](https://raw.githubusercontent.com/TexteaInc/funix-doc/main/screenshots/rgb2gray.png)
@@ -586,41 +585,67 @@
 * From PyPI (stable, lacking the latest feature)
     ```bash
     pip install funix
     ```
 * From GitHub (latest)
 
     ```bash
-    pip -b develop install "git+https://github.com/TexteaInc/funix.git"
+    pip install "git+https://github.com/TexteaInc/funix.git@develop" # Develop version
+    pip install "git+https://github.com/TexteaInc/funix.git" # Stable version
     ```
 * Local development
 
     ```bash
     git clone -b develop https://github.com/TexteaInc/funix
     cd funix
     pip install -e .
     ```
     Add `--prefix=~/.local` if pip insists to install to system paths. See [#24](https://github.com/TexteaInc/funix/issues/24) and [#23](https://github.com/TexteaInc/funix/issues/23)
 
+### Additional type support
+
+1. If you want to use `git` related features (use project from GitHub), install funix by:
+    
+    ```bash
+    pip install funix[git]
+    ```
+
+2. If you want to use `ipython` features, install funix by:
+    
+    ```bash
+    pip install funix[ipython]
+    ```
+
+3. If you need to have more than one feature, you can try installing them together:
+    
+    ```bash
+    pip install funix[all]
+    ```
+
 ### Building the frontend
 
 In the last two cases above, you will need to compile the frontend by yourself. Suppose you are in the `funix` folder. Then run the following commands:
 
 1. `cd frontend`
-3. `yarn install`
-4. `yarn start`
+2. `yarn install` (you need install Node.JS and Yarn)
+3. `yarn funix:build`
+
+For debugging:
+
+1. `yarn funix:test` (Start development mode)
+2. `funix xxx -p 8080 -F` (Use 8080 port and no frontend mode)
 
 #### Building the frontend with MUI Pro
 
 Our table widget uses advanced features in MUI Pro. If you have a MUI Pro license, you can build the frontend with MUI Pro by following the steps below:
 
 1. Install Node.js and Yarn;
 2. Create a file called `.env` in the `frontend` folder;
 3. Add `MUI_PRO_LICENSE_KEY=[your_key]` to the file;
-4. Run `yarn funix:build` to build the frontend;
+4. Run `yarn install && yarn funix:build` to build the frontend;
 5. Done!
 
 ### Command line options
 
 Run the command below to see the command line options:
 
 ```text
@@ -650,12 +675,13 @@
 
 ## How to contribute
 
 Funix is open-sourced under the MIT License. Community contribution is not only welcomed but desired. Feel free to fork and make a pull request when you are ready. You can also report bugs, suggest new features via the [issue tracker](https://github.com/TexteaInc/funix/issues/new) or our [Discord server](https://discord.gg/JyANAMUAHM).
 
 ## Acknowledgment
 
-Funix draws inspiration from FastAPI and Python-Fire: building software interfaces by inferring from function signatures containing type hints. We port this idea from the backend (FastAPI) or the terminal (Python-Fire) to the frontend. We also thank Streamlit, Gradio, PyWebIO, and Pynecone/Reflex. They inspired us. We are just too lazy to manually define widgets imperatively. Funix’s backend is implemented in Flask and the frontend in Material UI. 
+Funix draws inspiration from FastAPI and Python-Fire: building software interfaces by inferring from function signatures containing type hints. We port this idea from the backend (FastAPI) or the terminal (Python-Fire) to the frontend. We also thank Streamlit, Gradio, PyWebIO, and Pynecone/Reflex. They inspired us. We are just too lazy to manually define widgets imperatively. Funix’s backend is implemented in Flask and the frontend in Material UI.
 
 ## Contact
 
-hello at funix dot io
+Forrest dot Bao @ Gmail 
+
```

### Comparing `funix-0.5.7/README.md` & `funix-0.5.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -13,22 +13,23 @@
 
 <h4><a href="https://youtu.be/qDkzXS270Zo">Intro video</a> | <a href="#getting-started-with-funix">Getting started</a> |  <a href="#gallery"> Gallery </a> | <a href="https://github.com/TexteaInc/funix-doc/blob/main/Reference.md">Reference Manual</a> </h4>
 
 https://github.com/TexteaInc/funix/assets/438579/86868ab5-ed6e-46e5-8dc5-9e3e4a3cdc3f
 
 </div>
 
-## What is Funix? 
+## What is Funix?
 
 * Funix automatically turns an ordinary Python function or class definition into a web app, which is accessible in a browser via a shareable link. 
 * Funix is the frontend/backend/fullstack engineer and the infra/ops engineer for AI/Data/Science solo stars like you. 
 * Funix is the no-/low-code solution for those who write the most core and innovative code. 
 * Funix is open-source and can be deployed on-premises. 
 
 ## Use cases
+
 * Startups: quickly build demos, iterate on MVPs, get user feedback and statistics, and pitch to investors or your mom. 
 * Generative AI: instantly allow people to interact your GenAI model or idea.
 * STEM research: let people run your model and/or algorithm effortlessly. 
 * Data browser: an interface to page through your data. 
 * A/B test and data labeling: collect human labeling or preference.
 
 ## Key advantages
@@ -69,19 +70,17 @@
     ![screenshots/hello.png](https://github.com/TexteaInc/funix-doc/raw/main/screenshots/hello.png)
 
 
 <!-- > **Note**: The `-l` flag stands for _"lazy"_ meaning that only default settings are used. It cannot be used when your function is decorated by the funix decorator `@funix()` which allows you to customize your app. For more details, please refer to the [reference manual]([docs/Reference.md](https://github.com/TexteaInc/funix-doc/blob/main/Reference.md)). -->
 
 ## Getting started with Funix
 
-**The Zen of Funix** is to generate widgets for function I/Os based on their types, instead of manually picking and customizing the widget for each I/O. **Funix to Python is like CSS to HTML or style class to LaTeX**. UI stuff is not intermingled with the core logic but defined separately. The type-to-widget mapping is controlled by a theme and new types can be defined on top of existing types. 
-
-
-The example below shows how common UI compoents are generated from four Python-native data types: `str`, `bool`, `Literal` and `range`, as well as types in popular packages such as `ipywidgets.Password`. The example below further maps default values to placeholders in the UI widgets. From this example, we can see that developers need to **learn nothing about Funix or do nothing to their existing code** before they can get an app. 
+**The Zen of Funix** is to generate widgets for function I/Os based on their types, instead of manually picking and customizing the widget for each I/O. **Funix to Python is like CSS to HTML or style class to LaTeX**. UI stuff is not intermingled with the core logic but defined separately. The type-to-widget mapping is controlled by a theme and new types can be defined on top of existing types.
 
+The example below shows how common UI compoents are generated from four Python-native data types: `str`, `bool`, `Literal` and `range`, as well as types in popular packages such as `ipywidgets.Password`. The example below further maps default values to placeholders in the UI widgets. From this example, we can see that developers need to **learn nothing about Funix or do nothing to their existing code** before they can get an app.
 
 ```python
 import typing # Python native 
 
 import ipywidgets  # popular UI library 
 
 def input_widgets_basic(
@@ -92,15 +91,15 @@
     openai_key: ipywidgets.Password = "1234556",
     )  -> str:
     pass
 ```
 
 ![four input types](https://raw.githubusercontent.com/TexteaInc/funix-doc/main/screenshots/input_widgets.png)
 
-The example below shows how `pandas.DataFrame` and `matplotlib.figure.Figure` that AI/data developers cannot be more familiar with are mapped to tables and charts in an app. 
+The example below shows how `pandas.DataFrame` and `matplotlib.figure.Figure` that AI/data developers cannot be more familiar with are mapped to tables and charts in an app.
 
 ```python
 import pandas, matplotlib.pyplot
 from numpy import arange, log
 from numpy.random import random
 
 def table_and_plot(
@@ -115,15 +114,15 @@
     matplotlib.pyplot.plot(df["a"], df["c"], 'r')
 
     return fig
 ```
 
 ![table and plot screenshot](https://raw.githubusercontent.com/TexteaInc/funix-doc/main/screenshots/table_plot.png)
 
-You can even continuously update a plot based on user input. 
+You can even continuously update a plot based on user input.
 
 ```python
 import funix 
 import matplotlib.pyplot, matplotlib.figure
 import numpy 
 
 @funix.funix(
@@ -135,76 +134,72 @@
     y = numpy.sin(x*omega)
     matplotlib.pyplot.plot(x, y, linewidth=5)
     return fig
 ```
 
 ![continuous sine function](https://raw.githubusercontent.com/TexteaInc/funix-doc/main/screenshots/continous_run_sine.gif)
 
- 
 ### Out-of-box support for classes and OOP
 
 Funix can turn each member method of a class into a page of an app. 
 In two additional lines, the example below turn a class definition into a multi-page app with the OOP experience where the instantiation of an object of the class is done in a page corresponding to the constructor of the class and the member values of the object can be viewed and updated in other pages. **No need to manually expose** the member methods of the class.
 
 ```python
 from funix import funix_class
 
 @funix_class()  
 class A:
     def __init__(self, a: int):
         self.a = a
         return f"`self.a` has been initialized to {self.a}"
 
-    def update_a(self, b: int) -> str:
+    def set(self, b: int) -> str:
         self.a = b
         return f"`self.a` has been updated to {self.a}"
 
-    def print_a(self) -> str:
+    def get(self) -> str:
         return f"The value of `self.a` is {self.a}"
 ```
 
 ![class demo app gif](https://raw.githubusercontent.com/TexteaInc/funix-doc/main/videos/class/class.gif)
 
-
 A more advanced example of class is the wordle game. You can find the source code in [`examples/wordle.py`](./examples/games/wordle.py). In less than 100 lines, you can build Wordle! The screenshot is as follows:
 
 ![Wordle demo](https://github.com/TexteaInc/funix-doc/blob/main/screenshots/wordle.png?raw=true)
 
 ### The quickest way to build GenAI apps
 
 You can wrap any Python function into a web app in Funix.
-For example, you can take the ChatGPT demo code from OpenAI's APi reference and wrap it into a str-to-str function: 
+For example, you can take the ChatGPT demo code from OpenAI's APi reference and wrap it into a str-to-str function:
 
 ```python
 from openai import OpenAI
 
 def ChatGPT(prompt: str) -> str:    
     client = OpenAI()
 
     completion = client.chat.completions.create(
         model="gpt-3.5-turbo",
         messages=[
             {"role": "user", "content": prompt}
         ]
     )
-return completion.choices[0].message
+    return completion.choices[0].message.content
 ```
+
 which is turned into an app by Funix like below: 
 
 ![screenshots/ChatGPT_lazy.png](https://github.com/TexteaInc/funix-doc/raw/main/screenshots/chatGPT_lazy.png)
 
+### Themes: the CSS for Python
 
+**Funix to Python is like CSS to HTML or macros to LaTeX.** It separates the core logic and the UI.
+All UI stuff is centrally defined in a JSON-based theme to avoid the repetitiveness of individually configuring widgets and keep a consistent look across apps. Consequently, a data scientist or a machine learning engineer does not need to think about anything UI. Just leave it to the UI team and Funix.
 
-
-### Themes: the CSS for Python 
-
-**Funix to Python is like CSS to HTML or macros to LaTeX.** It separates the core logic and the UI. 
-All UI stuff is centrally defined in a JSON-based theme to avoid the repetitiveness of individually configuring widgets and keep a consistent look across apps. Consequently, a data scientist or a machine learning engineer does not need to think about anything UI. Just leave it to the UI team and Funix. 
-
-Below is an example of a theme file. It defines the widget choices based on variable types and tweaks the `props` of UI components (currently only MUI ones are supported). Funix exposes frontend components and their `props` to developers, requiring them to know nothing about frontend. To know more about how to define and apply a theme, please refer to [the Themes section in the reference manual](https://github.com/TexteaInc/funix-doc/blob/main/Reference.md#themes). 
+Below is an example of a theme file. It defines the widget choices based on variable types and tweaks the `props` of UI components (currently only MUI ones are supported). Funix exposes frontend components and their `props` to developers, requiring them to know nothing about frontend. To know more about how to define and apply a theme, please refer to [the Themes section in the reference manual](https://github.com/TexteaInc/funix-doc/blob/main/Reference.md#themes).
 
 ```jsonc
 {
   "name": "test_theme",
   "widgets": {    // dict, map types to widgets
     "str": "inputbox", // using Funix' widget shorthand
     "int": "slider[0,100,2]", // using Funix' widget shorthand
@@ -218,15 +213,15 @@
         }
     }, 
     "Literal": "radio"
   },
 }
 ```
 
-To introduce a new data type, just declare a new Python class, and use a decorator to let Funix know. You can associate the type with a widget either on-the-fly (below) or via a theme file. 
+To introduce a new data type, just declare a new Python class, and use a decorator to let Funix know. You can associate the type with a widget either on-the-fly (below) or via a theme file.
 
 ```python
 from funix import funix, new_funix_type
 
 @new_funix_type(
     widget = {
         "widget": "@mui/material/TextField",
@@ -246,15 +241,15 @@
 
 if __name__ == "__main__":
     print (hoho(blackout('Fun'))) 
 ```
 
 ### Python-native to web-native
 
-Funix repurposes some Python-native features to web features. 
+Funix repurposes some Python-native features to web features.
 
 First, Funix won't let your docstring or `print()` function calls go to waste. They will appear in the input and output panels of the web app.
 
 ```python
 from funix import funix
 @funix(
     print_to_web=True
@@ -286,15 +281,15 @@
     for i in range(len(message)):
         time.sleep(0.01)
         yield message[0:i]
 ```
 
 ![Streamt text to web](https://github.com/TexteaInc/funix-doc/blob/main/screenshots/stream.gif?raw=true)
 
-## Advanced features 
+## Advanced features
 
 ### History: Keep your call logs
 
 <details>
 <summary>
 Click to expand
 </summary>
@@ -344,20 +339,23 @@
 
 A special case of passing data between functions is to use the return value of one function as the value in the widget of an argument of another function. This is called prefill. Funix support prefill by using a decorator attribute `pre_fill`. Below is an example and the corresponding GIF animation.
 
 
 ```python
 import funix
 
+@funix.funix()
 def first_action(x: int) -> int:
   return x - 1
 
+@funix.funix()
 def second_action(message: str) -> list[str]:
   return message.split(" ")
 
+@funix.funix()
 def third_action(x: int, y: int) -> dict:
   return {"x": x, "y": y}
 
 @funix.funix(
   pre_fill={
     "a": first_action,
     "b": (second_action, -1),
@@ -409,48 +407,52 @@
 
 More examples in <a href="https://github.com/TexteaInc/funix-doc/blob/main/Reference.md">Reference Manual</a> or the <code>./examples</code> folder.
 
 * [ChatPaper](https://github.com/forrestbao/ChatPaper) (It's like the popular ChatPDF. But in Funix, only 70 lines of code needed.)
 * [mFlux](https://github.com/Yazawazi/MFlux) (synthetic biology)
 
 ### ChatGPT, multi-turn
+
 <details>
   <summary><code>examples/AI/chatGPT_multi_turn.py</code> 👈 Toggle me to show source code </summary>
 
   ```python
     import os
     import IPython     
-    import openai
-    openai.api_key = os.environ.get("OPENAI_KEY")
+    from openai import OpenAI
+    import funix
+
+    client = OpenAI(api_key=os.environ.get("OPENAI_KEY"))
 
     messages  = []  # list of dicts, dict keys: role, content, system
 
+    @funix.funix(
+        disable=True,
+    )
     def print_messages_html(messages):
         printout = ""
         for message in messages:
             if message["role"] == "user":
-                align, left, name = "left", "0%", "You"
+                align, name = "left", "You"
             elif message["role"] == "assistant":
-                align, left, name = "right", "30%", "ChatGPT"
-            printout += f'<div style="position: relative; left: {left}; width: 70%"><b>{name}</b>: {message["content"]}</div>'
+                align, name = "right", "ChatGPT"
+            printout += f'<div style="width: 100%; text-align: {align}"><b>{name}</b>: {message["content"]}</div>'
         return printout
 
-    import funix
+
     @funix.funix(
         direction="column-reverse",
     )
     def ChatGPT_multi_turn(current_message: str)  -> IPython.display.HTML:
         current_message = current_message.strip()
         messages.append({"role": "user", "content": current_message})
-        completion = openai.ChatCompletion.create(
-            messages=messages,
-            model='gpt-3.5-turbo',
-            max_tokens=100,
-        )
-        chatgpt_response = completion["choices"][0]["message"]["content"]
+        completion = client.chat.completions.create(messages=messages,
+        model='gpt-3.5-turbo',
+        max_tokens=100)
+        chatgpt_response = completion.choices[0].message.content
         messages.append({"role": "assistant", "content": chatgpt_response})
 
         # return print_messages_markdown(messages)
         return print_messages_html(messages)
 
   ```
 
@@ -458,23 +460,25 @@
 
 ![Multiturn chat](https://github.com/TexteaInc/funix-doc/raw/main/screenshots/chatGPT_multiturn.png)
 
 ### Shortest Dall-E web app in Python
 
 ```python
 from funix import funix                      # add line one
-from funix.hint import Images                # add line two
-import openai  # pip install openai
+from IPython.display import Image
+from openai import OpenAI                    # pip install openai
+
+import os
+client = OpenAI(api_key=os.environ.get("OPENAI_KEY"))  
 
-openai.api_key = os.environ.get("OPENAI_KEY")
 
-@funix()                                     # add line three
+@funix()                                     # add line two
 def dalle(prompt: str = "a cat") -> Image:
-    response = openai.Image.create(prompt=prompt)
-    return response["data"][0]["url"]
+    response = client.images.generate(prompt=prompt)
+    return response.data[0].url
 ```
 
 ![Dalle demo](https://github.com/TexteaInc/funix-doc/raw/main/screenshots/dalle.jpg)
 
 <!-- Funix.io can get the same job done in half the amount of code required by Gradio, by exploiting the Python language as much as possible. Here, state/session is maintained using a global variable, while the order of the returns defines the return layout.  -->
 
 ### Bioinformatics: vector stripping
@@ -485,25 +489,26 @@
 
 ### Multimedia inputs and outputs
 
 <details>
 <summary><code>examples/multimedia/rgb2gray.py</code> 👈 Toggle me to show source code</summary>
 
 ```python
-import  io # Python's native
+import  io # Python's native 
 
 import PIL # the Python Image Library
-import funix
+import IPython 
+import funix 
 
 @funix.funix(
     title="Convert color images to grayscale images",
 )
-def gray_it(image: funix.hint.BytesImage) -> funix.hint.Image:
+def gray_it(image: funix.hint.BytesImage) -> IPython.display.Image:
     img = PIL.Image.open(io.BytesIO(image))
-    gray = PIL.ImageOps.grayscale(img)
+    gray = PIL.ImageOps.grayscale(img) 
     output = io.BytesIO()
     gray.save(output, format="PNG")
     return output.getvalue()
 ```
 </details>
 
 ![shipping example](https://raw.githubusercontent.com/TexteaInc/funix-doc/main/screenshots/rgb2gray.png)
@@ -521,41 +526,67 @@
 * From PyPI (stable, lacking the latest feature)
     ```bash
     pip install funix
     ```
 * From GitHub (latest)
 
     ```bash
-    pip -b develop install "git+https://github.com/TexteaInc/funix.git"
+    pip install "git+https://github.com/TexteaInc/funix.git@develop" # Develop version
+    pip install "git+https://github.com/TexteaInc/funix.git" # Stable version
     ```
 * Local development
 
     ```bash
     git clone -b develop https://github.com/TexteaInc/funix
     cd funix
     pip install -e .
     ```
     Add `--prefix=~/.local` if pip insists to install to system paths. See [#24](https://github.com/TexteaInc/funix/issues/24) and [#23](https://github.com/TexteaInc/funix/issues/23)
 
+### Additional type support
+
+1. If you want to use `git` related features (use project from GitHub), install funix by:
+    
+    ```bash
+    pip install funix[git]
+    ```
+
+2. If you want to use `ipython` features, install funix by:
+    
+    ```bash
+    pip install funix[ipython]
+    ```
+
+3. If you need to have more than one feature, you can try installing them together:
+    
+    ```bash
+    pip install funix[all]
+    ```
+
 ### Building the frontend
 
 In the last two cases above, you will need to compile the frontend by yourself. Suppose you are in the `funix` folder. Then run the following commands:
 
 1. `cd frontend`
-3. `yarn install`
-4. `yarn start`
+2. `yarn install` (you need install Node.JS and Yarn)
+3. `yarn funix:build`
+
+For debugging:
+
+1. `yarn funix:test` (Start development mode)
+2. `funix xxx -p 8080 -F` (Use 8080 port and no frontend mode)
 
 #### Building the frontend with MUI Pro
 
 Our table widget uses advanced features in MUI Pro. If you have a MUI Pro license, you can build the frontend with MUI Pro by following the steps below:
 
 1. Install Node.js and Yarn;
 2. Create a file called `.env` in the `frontend` folder;
 3. Add `MUI_PRO_LICENSE_KEY=[your_key]` to the file;
-4. Run `yarn funix:build` to build the frontend;
+4. Run `yarn install && yarn funix:build` to build the frontend;
 5. Done!
 
 ### Command line options
 
 Run the command below to see the command line options:
 
 ```text
@@ -585,12 +616,13 @@
 
 ## How to contribute
 
 Funix is open-sourced under the MIT License. Community contribution is not only welcomed but desired. Feel free to fork and make a pull request when you are ready. You can also report bugs, suggest new features via the [issue tracker](https://github.com/TexteaInc/funix/issues/new) or our [Discord server](https://discord.gg/JyANAMUAHM).
 
 ## Acknowledgment
 
-Funix draws inspiration from FastAPI and Python-Fire: building software interfaces by inferring from function signatures containing type hints. We port this idea from the backend (FastAPI) or the terminal (Python-Fire) to the frontend. We also thank Streamlit, Gradio, PyWebIO, and Pynecone/Reflex. They inspired us. We are just too lazy to manually define widgets imperatively. Funix’s backend is implemented in Flask and the frontend in Material UI. 
+Funix draws inspiration from FastAPI and Python-Fire: building software interfaces by inferring from function signatures containing type hints. We port this idea from the backend (FastAPI) or the terminal (Python-Fire) to the frontend. We also thank Streamlit, Gradio, PyWebIO, and Pynecone/Reflex. They inspired us. We are just too lazy to manually define widgets imperatively. Funix’s backend is implemented in Flask and the frontend in Material UI.
 
 ## Contact
 
-hello at funix dot io
+Forrest dot Bao @ Gmail 
+
```

### Comparing `funix-0.5.7/backend/funix/__init__.py` & `funix-0.5.8/backend/funix/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 import funix.decorator as decorator
 import funix.decorator.call as call
 import funix.decorator.limit as limit
 import funix.decorator.lists as lists
 import funix.decorator.secret as secret
 import funix.decorator.theme as theme
 import funix.hint as hint
-from funix.app import app, enable_funix_host_checker, privacy_policy
-from funix.frontend import OpenFrontend, run_open_frontend, start
+from funix.app import app, enable_funix_host_checker
+from funix.frontend import run_open_frontend, start
 from funix.prep.global_to_session import get_new_python_file
 from funix.util.file import (
     create_safe_tempdir,
     get_path_difference,
     get_python_files_in_dir,
 )
-from funix.util.module import getsourcefile_safe, handle_module, import_module_from_file
+from funix.util.module import handle_module, import_module_from_file
 from funix.util.network import get_compressed_ip_address_as_str, get_unused_port_from
 
 # ---- Exports ----
 # ---- Decorators ----
 funix = decorator.funix
 funix_class = decorator.funix_class
 funix_method = decorator.funix_method
```

### Comparing `funix-0.5.7/backend/funix/__main__.py` & `funix-0.5.8/backend/funix/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,12 +77,12 @@
 
 def cli_main():
     """
     The entry point for the command line interface.
 
     This function is called when you run `python -m funix` or `funix` from the command line.
     """
-    plac.call(main, version="Funix 0.5.7")
+    plac.call(main, version="Funix 0.5.8")
 
 
 if __name__ == "__main__":
     cli_main()
```

### Comparing `funix-0.5.7/backend/funix/app/__init__.py` & `funix-0.5.8/backend/funix/app/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 from funix.config.switch import GlobalSwitchOption
 from funix.hint import LogLevel
 
 app = Flask(__name__)
 app.secret_key = GlobalSwitchOption.get_session_key()
 app.config.update(
     SESSION_COOKIE_PATH="/",
-    SESSION_COOKIE_SAMESITE="Lax",
+    SESSION_COOKIE_SAMESITE="None",
+    SESSION_TYPE="filesystem",
 )
 sock = Sock(app)
 
 funix_log_level = LogLevel.get_level()
 
 privacy = """We honor your choices. For your data and freedom.
 
@@ -65,19 +66,24 @@
         message.encode() + str(funix_log_level.value).encode()
     ).hexdigest()
     privacy = message
 
 
 @app.after_request
 def funix_auto_cors(response: Response) -> Response:
-    response.headers["Access-Control-Allow-Origin"] = "*"
+    if "HTTP_ORIGIN" not in request.environ:
+        response.headers["Access-Control-Allow-Origin"] = "*"
+    else:
+        response.headers["Access-Control-Allow-Credentials"] = "true"
+        response.headers["Access-Control-Allow-Origin"] = request.environ["HTTP_ORIGIN"]
     response.headers[
         "Access-Control-Allow-Methods"
     ] = "GET, HEAD, POST, OPTIONS, PUT, PATCH, DELETE"
-    response.headers["Access-Control-Allow-Headers"] = "*"
+    response.headers["Access-Control-Allow-Headers"] = "Content-Type, *"
+    
     return response
 
 
 def __api_call_data(response: Response, dict_to_json: bool = False) -> dict | None:
     do_not_log_me = (
         request.cookies.get("DO_NOT_LOG_ME") and funix_log_level != LogLevel.MANDATORY
     )
```

### Comparing `funix-0.5.7/backend/funix/app/websocket.py` & `funix-0.5.8/backend/funix/app/websocket.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/build/favicon.ico` & `funix-0.5.8/backend/funix/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/build/index.html` & `funix-0.5.8/backend/funix/build/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="description" content="Textea Funix React Frontend"/><link rel="apple-touch-icon" href="/logo192.png"/><link rel="manifest" href="/manifest.json"/><link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Roboto:300,400,500,700&display=swap"/><script src="static/js/d3.v5.js"></script><script src="static/js/mpld3.v0.5.8.js"></script><script src="static/js/jquery-3.7.1.min.js"></script><style>.text-style{margin:0;padding:0;list-style-position:inside}</style><title>Funix</title><script defer="defer" src="/static/js/main.0af491b9.js"></script><link href="/static/css/main.4efb37a3.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
+<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="description" content="Textea Funix React Frontend"/><link rel="apple-touch-icon" href="/logo192.png"/><link rel="manifest" href="/manifest.json"/><link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Roboto:300,400,500,700&display=swap"/><script src="static/js/d3.v5.js"></script><script src="static/js/mpld3.v0.5.8.js"></script><script src="static/js/jquery-3.7.1.min.js"></script><style>.text-style{margin:0;padding:0;list-style-position:inside}</style><title>Funix</title><script defer="defer" src="/static/js/main.279c7e85.js"></script><link href="/static/css/main.4efb37a3.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
```

### Comparing `funix-0.5.7/backend/funix/build/logo192.png` & `funix-0.5.8/backend/funix/build/logo192.png`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/build/logo512.png` & `funix-0.5.8/backend/funix/build/logo512.png`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/build/static/js/d3.v5.js` & `funix-0.5.8/backend/funix/build/static/js/d3.v5.js`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/build/static/js/jquery-3.7.1.min.js` & `funix-0.5.8/backend/funix/build/static/js/jquery-3.7.1.min.js`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/build/static/js/main.0af491b9.js` & `funix-0.5.8/backend/funix/build/static/js/main.279c7e85.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.0af491b9.js.LICENSE.txt */ ! function() {
+/*! For license information please see main.279c7e85.js.LICENSE.txt */ ! function() {
     var e = {
             5296: function(e, t, n) {
                 "use strict";
                 n.d(t, {
                     Z: function() {
                         return ae
                     }
@@ -63757,15 +63757,16 @@
 
             function Kn() {
                 return Kn = en(Xt().mark((function e(t, n) {
                     return Xt().wrap((function(e) {
                         for (;;) switch (e.prev = e.next) {
                             case 0:
                                 return e.abrupt("return", Yn(t, s(s({}, n), {}, {
-                                    method: "GET"
+                                    method: "GET",
+                                    credentials: "include"
                                 })));
                             case 1:
                             case "end":
                                 return e.stop()
                         }
                     }), e)
                 }))), Kn.apply(this, arguments)
@@ -63781,15 +63782,16 @@
                         for (;;) switch (e.prev = e.next) {
                             case 0:
                                 return e.abrupt("return", fetch(t, s(s({}, r), {}, {
                                     method: "POST",
                                     body: JSON.stringify(n),
                                     headers: s(s({}, null === r || void 0 === r ? void 0 : r.headers), {}, {
                                         "Content-Type": "application/json"
-                                    })
+                                    }),
+                                    credentials: "include"
                                 })).then((function(e) {
                                     return e.text()
                                 })));
                             case 1:
                             case "end":
                                 return e.stop()
                         }
@@ -63805,15 +63807,16 @@
                                 return e.abrupt("return", Yn(t, s(s({}, r), {}, {
                                     method: "POST",
                                     body: JSON.stringify({
                                         secret: n
                                     }),
                                     headers: s(s({}, null === r || void 0 === r ? void 0 : r.headers), {}, {
                                         "Content-Type": "application/json"
-                                    })
+                                    }),
+                                    credentials: "include"
                                 })).then((function(e) {
                                     return e.success
                                 })));
                             case 1:
                             case "end":
                                 return e.stop()
                         }
@@ -113612,15 +113615,16 @@
                                     var n = t.formData;
                                     o(n), e.preview.reactive && cq().debounce((function() {
                                         fetch(new URL("/update/".concat(e.preview.id), e.backend), {
                                             method: "POST",
                                             headers: {
                                                 "Content-Type": "application/json"
                                             },
-                                            body: JSON.stringify(n)
+                                            body: JSON.stringify(n),
+                                            credentials: "include"
                                         }).then((function(e) {
                                             return e.json()
                                         })).then((function(e) {
                                             var t = e.result;
                                             if (null !== t)
                                                 for (var n = function() {
                                                         var e = (0, c.Z)(a[r], 2),
@@ -114646,24 +114650,31 @@
                                 if (Array.isArray(n) && r(n)) {
                                     var u = function(e) {
                                         if ("json" === e.selectedResponseViewType) return (0, v.jsx)(VA, {
                                             src: null !== n && void 0 !== n ? n : {}
                                         });
                                         if ("sheet" === e.selectedResponseViewType) return (0, v.jsx)(aU, {
                                             columns: [{
-                                                field: "root"
+                                                field: "id",
+                                                headerName: "ID"
+                                            }, {
+                                                field: "value",
+                                                headerName: "Root"
                                             }],
                                             rows: n.map((function(e, t) {
                                                 return {
                                                     id: t,
-                                                    root: e
+                                                    value: e
                                                 }
                                             })),
                                             components: {
                                                 Toolbar: Qq
+                                            },
+                                            sx: {
+                                                minHeight: 400
                                             }
                                         });
                                         throw new Error("Unsupported selectedResponseViewType")
                                     };
                                     return (0, v.jsxs)("div", {
                                         children: [a, (0, v.jsx)(u, {
                                             selectedResponseViewType: o
@@ -115003,15 +115014,15 @@
                         V = Z[1],
                         B = (0, r.useState)(!1),
                         j = (0, c.Z)(B, 2),
                         U = j[0],
                         G = j[1];
                     (0, r.useEffect)((function() {
                         if (t.secret) {
-                            var e = t.name in h ? h[t.path] : null !== _ ? _ : "";
+                            var e = t.path in h ? h[t.path] : null !== _ ? _ : "";
                             (function(e, t, n) {
                                 return Xn.apply(this, arguments)
                             })(new URL("/verify/".concat(t.id), n), e || "").then((function(e) {
                                 D(e)
                             })).catch((function() {
                                 D(!1)
                             }))
@@ -115053,15 +115064,17 @@
                     }), [x]), (0, r.useEffect)((function() {
                         null != i && E((function(e) {
                             return s(s({}, e), {}, {
                                 theme: i.theme
                             })
                         }))
                     }), [i]), (0, r.useEffect)((function() {
-                        P.current || (P.current = !0, fetch(new URL("/param/".concat(t.id), n).toString()).then((function(e) {
+                        P.current || (P.current = !0, fetch(new URL("/param/".concat(t.id), n).toString(), {
+                            credentials: "include"
+                        }).then((function(e) {
                             return e.json()
                         })).then((function(e) {
                             l(e), V(!1)
                         })).then((function() {
                             t.keepLast && t.id in b && N(JSON.stringify(b[t.id].output))
                         })))
                     }), [t, n, b]);
```

### Comparing `funix-0.5.7/backend/funix/build/static/js/main.0af491b9.js.LICENSE.txt` & `funix-0.5.8/backend/funix/build/static/js/main.279c7e85.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/build/static/js/mpld3.v0.5.8.js` & `funix-0.5.8/backend/funix/build/static/js/mpld3.v0.5.8.js`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/config/__init__.py` & `funix-0.5.8/backend/funix/config/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/config/switch.py` & `funix-0.5.8/backend/funix/config/switch.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/decorator/__init__.py` & `funix-0.5.8/backend/funix/decorator/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,62 +11,43 @@
 from typing import Callable, Optional, Union
 from uuid import uuid4
 
 from funix.app import app, sock
 from funix.config import banned_function_name_and_path
 from funix.config.switch import GlobalSwitchOption
 from funix.decorator.all_of import parse_all_of
-from funix.decorator.annnotation_analyzer import (
-    analyze,
-    register_ipywidgets,
-    register_pandera,
-)
+from funix.decorator.annnotation_analyzer import register_ipywidgets, register_pandera
 from funix.decorator.call import funix_call
-from funix.decorator.file import (
-    enable_file_service,
-    get_static_uri,
-    handle_ipython_audio_image_video,
-)
+from funix.decorator.file import enable_file_service
 from funix.decorator.layout import handle_input_layout, handle_output_layout
-from funix.decorator.limit import Limiter, global_rate_limiters, parse_limiter_args
+from funix.decorator.limit import Limiter, parse_limiter_args
 from funix.decorator.lists import (
     decorated_functions_list_append,
     enable_list,
     get_default_function_name,
     push_counter,
     set_default_function,
 )
-from funix.decorator.magic import (
-    anal_function_result,
-    function_param_to_widget,
-    get_type_dict,
-    get_type_widget_prop,
-    parse_function_annotation,
-)
+from funix.decorator.magic import parse_function_annotation
 from funix.decorator.param import (
     create_parse_type_metadata,
     get_param_for_funix,
     parse_param,
 )
-from funix.decorator.pre_fill import get_pre_fill_metadata, parse_pre_fill
+from funix.decorator.pre_fill import parse_pre_fill
 from funix.decorator.reactive import function_reactive_update, get_reactive_config
 from funix.decorator.runtime import RuntimeClassVisitor
 from funix.decorator.secret import (
     check_secret,
     get_app_secret,
     get_secret_by_id,
     set_function_secret,
 )
-from funix.decorator.theme import (
-    get_parsed_theme_fot_funix,
-    import_theme,
-    parsed_themes,
-    themes,
-)
-from funix.decorator.widget import parse_argument_config, parse_widget, widget_parse
+from funix.decorator.theme import get_parsed_theme_fot_funix
+from funix.decorator.widget import parse_argument_config, widget_parse
 from funix.hint import (
     ArgumentConfigType,
     ConditionalVisibleType,
     DestinationType,
     DirectionType,
     ExamplesType,
     InputLayout,
```

### Comparing `funix-0.5.7/backend/funix/decorator/all_of.py` & `funix-0.5.8/backend/funix/decorator/all_of.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/decorator/annnotation_analyzer.py` & `funix-0.5.8/backend/funix/decorator/annnotation_analyzer.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/decorator/call.py` & `funix-0.5.8/backend/funix/decorator/call.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/decorator/file.py` & `funix-0.5.8/backend/funix/decorator/file.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/decorator/layout.py` & `funix-0.5.8/backend/funix/decorator/layout.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     converted_item = row_item
     converted_item["type"] = item_type
     converted_item["content"] = row_item[item_type]
     converted_item.pop(item_type)
     return converted_item
 
 
-def handle_input_layout(input_layout: list) -> (list, dict):
+def handle_input_layout(input_layout: list) -> tuple[list, dict]:
     return_input_layout = []
     decorated_params = {}
     for row in input_layout:
         row_layout = []
         for row_item in row:
             row_item_done = row_item
             for common_row_item_key in ["markdown", "html"]:
@@ -42,15 +42,15 @@
                     row_item_done["content"] = row_item_done["divider"]
                 row_item_done.pop("divider")
             row_layout.append(row_item_done)
         return_input_layout.append(row_layout)
     return return_input_layout, decorated_params
 
 
-def handle_output_layout(output_layout: list) -> (list, list):
+def handle_output_layout(output_layout: list) -> tuple[list, list]:
     return_output_layout = []
     return_output_indexes = []
     for row in output_layout:
         row_layout = []
         for row_item in row:
             row_item_done = row_item
             for common_row_item_key in [
```

### Comparing `funix-0.5.7/backend/funix/decorator/limit.py` & `funix-0.5.8/backend/funix/decorator/limit.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/decorator/lists.py` & `funix-0.5.8/backend/funix/decorator/lists.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/decorator/magic.py` & `funix-0.5.8/backend/funix/decorator/magic.py`

 * *Files 0% similar despite different names*

```diff
@@ -581,15 +581,15 @@
                             call_result = [get_static_uri(call_result[0])]
                 return call_result
     return call_result
 
 
 def parse_function_annotation(
     function_signature: Signature, figure_to_image: bool
-) -> (bool, Any):
+) -> tuple[bool, Any]:
     cast_to_list_flag = False
     if function_signature.return_annotation is not Signature.empty:
         # TODO: Magic code, I've forgotten what it does, but it works, refactor it if you can
         # return type dict enforcement for yodas only
         try:
             if (
                 cast_to_list_flag := function_signature.return_annotation.__class__.__name__
```

### Comparing `funix-0.5.7/backend/funix/decorator/param.py` & `funix-0.5.8/backend/funix/decorator/param.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/decorator/pre_fill.py` & `funix-0.5.8/backend/funix/decorator/pre_fill.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/decorator/reactive.py` & `funix-0.5.8/backend/funix/decorator/reactive.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/decorator/runtime.py` & `funix-0.5.8/backend/funix/decorator/runtime.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/decorator/secret.py` & `funix-0.5.8/backend/funix/decorator/secret.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/decorator/theme.py` & `funix-0.5.8/backend/funix/decorator/theme.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/decorator/widget.py` & `funix-0.5.8/backend/funix/decorator/widget.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/frontend/__init__.py` & `funix-0.5.8/backend/funix/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/hint/__init__.py` & `funix-0.5.8/backend/funix/hint/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,70 +294,70 @@
 """
 Support URL, path, bytes
 
 For example: "https://example.org/imgs/1.png"
 """
 
 _Markdown = NewType("Markdown", type(Optional[str]))
-Markdown: TypeAlias = _Markdown
+Markdown: TypeAlias = _Markdown # type: ignore
 """
 Markdown type.
 For output.
 
 Support Markdown like "**bold**" and "*italic*"
 """
 
 _HTML = NewType("HTML", type(Optional[str]))
-HTML: TypeAlias = _HTML
+HTML: TypeAlias = _HTML # type: ignore
 """
 HTML type.
 For output.
 
 
 Support HTML like "<span style='color: red'>red</span>"
 """
 
 _Image = NewType("Images", type(BasicFileType))
-Image: TypeAlias = _Image
+Image: TypeAlias = _Image # type: ignore
 """
 Image type.
 For output.
 
 See `BasicFileType` for more information.
 """
 
 _Video = NewType("Videos", type(BasicFileType))
-Video: TypeAlias = _Video
+Video: TypeAlias = _Video # type: ignore
 """
 Video type.
 For output.
 
 See `BasicFileType` for more information.
 """
 
 _Audio = NewType("Audios", type(BasicFileType))
-Audio: TypeAlias = _Audio
+Audio: TypeAlias = _Audio # type: ignore
 """
 Audio type.
 For output.
 
 See `BasicFileType` for more information.
 """
 
 _File = NewType("Files", type(BasicFileType))
-File: TypeAlias = _File
+File: TypeAlias = _File # type: ignore
 """
 File type.
 For output.
 
 See `BasicFileType` for more information.
 """
 
 _Code = NewType("Code", type(Optional[str | CodeConfig]))
-Code: TypeAlias = _Code
+Code: TypeAlias = _Code # type: ignore
 """
 Code type.
 For output.
 
 
 Support Code like:
```

### Comparing `funix-0.5.7/backend/funix/hint/layout.py` & `funix-0.5.8/backend/funix/hint/layout.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/prep/global_to_session.py` & `funix-0.5.8/backend/funix/prep/global_to_session.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/session/__init__.py` & `funix-0.5.8/backend/funix/session/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/test/test_magic.py` & `funix-0.5.8/backend/funix/test/test_magic.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/theme/__init__.py` & `funix-0.5.8/backend/funix/theme/__init__.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/util/file.py` & `funix-0.5.8/backend/funix/util/file.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,14 +44,17 @@
         >>> assert get_path_difference("/abc", "/abc/de/c") == "de.c"
     """
     base_components = normpath(base_path).split(sep)
     target_components = normpath(target_path).split(sep)
 
     if not target_path.startswith(base_path):
         raise ValueError("The base directory is not a prefix of the target directory.")
+    
+    if len(base_components) == 1 and base_components[0] == ".":
+        return ".".join(target_components)
 
     path_diff = target_components
 
     for _ in range(len(base_components)):
         path_diff.pop(0)
 
     return ".".join(path_diff)
```

### Comparing `funix-0.5.7/backend/funix/util/module.py` & `funix-0.5.8/backend/funix/util/module.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/util/network.py` & `funix-0.5.8/backend/funix/util/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Network utils for funix.
 """
 
-from ipaddress import IPv4Address, IPv6Address, ip_network
+from ipaddress import IPv4Address, IPv6Address
 from socket import AF_INET, SOCK_STREAM, socket
 
 
 def get_compressed_ip_address_as_str(host: IPv4Address | IPv6Address) -> str:
     """
     Get the str ip and handle the local ip.
     Just 0.0.0.0 and :: will be formatted, others will be stringify and returned.
```

### Comparing `funix-0.5.7/backend/funix/util/secret.py` & `funix-0.5.8/backend/funix/util/secret.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/util/text.py` & `funix-0.5.8/backend/funix/util/text.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/util/uri.py` & `funix-0.5.8/backend/funix/util/uri.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix/widget/__init__.py` & `funix-0.5.8/backend/funix/widget/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         SliderConfig: The updated config of the slider widget.
     """
     new_config = SliderConfig(min=0, max=100, step=0.1)
     new_config.update(slider(*args[0])[1])
     return new_config
 
 
-def slider(*args, **kwargs) -> (str, SliderConfig):
+def slider(*args, **kwargs) -> tuple[str, SliderConfig]:
     """
     Create a slider widget config.
 
     Parameters:
         *args: The config of the slider widget. The order is `min`, `max`, `step`.
         **kwargs: The config of the slider widget. The key is `min`, `max`, `step`.
 
@@ -135,15 +135,15 @@
 
     language: str
     """
     The language of the code.
     """
 
 
-def code(language: str = "plaintext") -> (str, CodeConfig):
+def code(language: str = "plaintext") -> tuple[str, CodeConfig]:
     """
     Create a code widget config.
 
     Parameters:
         language(str): The language of the code, default is `plaintext`.
 
     Returns:
@@ -175,15 +175,15 @@
     """
     When upgrade to 3.11, use `NotRequired`
     
     The maximum number of rows of the textbox.
     """
 
 
-def textarea(*args, **kwargs) -> (str, MultilineTextboxConfig):
+def textarea(*args, **kwargs) -> tuple[str, MultilineTextboxConfig]:
     """
     Create a multiline textbox widget config.
 
     Parameters:
         *args: The config of the slider widget. The order is `min`, `max`, `step`.
         **kwargs: The config of the multiline textbox widget. The key is `rows`, `min`, `max`.
```

### Comparing `funix-0.5.7/backend/funix/widget/builtin.py` & `funix-0.5.8/backend/funix/widget/builtin.py`

 * *Files identical despite different names*

### Comparing `funix-0.5.7/backend/funix.egg-info/PKG-INFO` & `funix-0.5.8/backend/funix.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: funix
-Version: 0.5.7
+Version: 0.5.8
 Summary: Building web apps without manually creating widgets
-Author-email: "Textea Inc." <hello@funix.io>
+Author-email: "Textea Inc." <forrestbao@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 Textea Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -39,33 +39,27 @@
 Requires-Dist: flask>=2.2.2
 Requires-Dist: functions-framework==3.*
 Requires-Dist: requests>=2.28.1
 Requires-Dist: plac>=1.3.5
 Requires-Dist: gitignore-parser>=0.1.9
 Requires-Dist: flask-sock>=0.7.0
 Requires-Dist: SQLAlchemy>=2.0.23
-Provides-Extra: plot
-Requires-Dist: matplotlib>=3.4.3; extra == "plot"
-Requires-Dist: mpld3>=0.5.8; extra == "plot"
+Requires-Dist: matplotlib>=3.4.3
+Requires-Dist: mpld3>=0.5.8
+Requires-Dist: pandera>=0.17.2
+Requires-Dist: pandas>=2.0.3
 Provides-Extra: git
 Requires-Dist: GitPython>=3.1.31; extra == "git"
 Provides-Extra: ipython
 Requires-Dist: IPython>=8.14.0; extra == "ipython"
 Requires-Dist: ipywidgets>=8.0.7; extra == "ipython"
-Provides-Extra: pandas
-Requires-Dist: pandera>=0.17.2; extra == "pandas"
-Requires-Dist: pandas>=2.0.3; extra == "pandas"
 Provides-Extra: all
-Requires-Dist: matplotlib>=3.4.3; extra == "all"
-Requires-Dist: mpld3>=0.5.8; extra == "all"
 Requires-Dist: GitPython>=3.1.31; extra == "all"
 Requires-Dist: IPython>=8.14.0; extra == "all"
 Requires-Dist: ipywidgets>=8.0.7; extra == "all"
-Requires-Dist: pandera>=0.17.2; extra == "all"
-Requires-Dist: pandas>=2.0.3; extra == "all"
 
 <h1 align="center">
     <!-- <b> -->
         Funix.io<br>
     <!-- </b> -->
     The laziest way to build AI/Data apps in Python
 </h1>
@@ -78,22 +72,23 @@
 
 <h4><a href="https://youtu.be/qDkzXS270Zo">Intro video</a> | <a href="#getting-started-with-funix">Getting started</a> |  <a href="#gallery"> Gallery </a> | <a href="https://github.com/TexteaInc/funix-doc/blob/main/Reference.md">Reference Manual</a> </h4>
 
 https://github.com/TexteaInc/funix/assets/438579/86868ab5-ed6e-46e5-8dc5-9e3e4a3cdc3f
 
 </div>
 
-## What is Funix? 
+## What is Funix?
 
 * Funix automatically turns an ordinary Python function or class definition into a web app, which is accessible in a browser via a shareable link. 
 * Funix is the frontend/backend/fullstack engineer and the infra/ops engineer for AI/Data/Science solo stars like you. 
 * Funix is the no-/low-code solution for those who write the most core and innovative code. 
 * Funix is open-source and can be deployed on-premises. 
 
 ## Use cases
+
 * Startups: quickly build demos, iterate on MVPs, get user feedback and statistics, and pitch to investors or your mom. 
 * Generative AI: instantly allow people to interact your GenAI model or idea.
 * STEM research: let people run your model and/or algorithm effortlessly. 
 * Data browser: an interface to page through your data. 
 * A/B test and data labeling: collect human labeling or preference.
 
 ## Key advantages
@@ -134,19 +129,17 @@
     ![screenshots/hello.png](https://github.com/TexteaInc/funix-doc/raw/main/screenshots/hello.png)
 
 
 <!-- > **Note**: The `-l` flag stands for _"lazy"_ meaning that only default settings are used. It cannot be used when your function is decorated by the funix decorator `@funix()` which allows you to customize your app. For more details, please refer to the [reference manual]([docs/Reference.md](https://github.com/TexteaInc/funix-doc/blob/main/Reference.md)). -->
 
 ## Getting started with Funix
 
-**The Zen of Funix** is to generate widgets for function I/Os based on their types, instead of manually picking and customizing the widget for each I/O. **Funix to Python is like CSS to HTML or style class to LaTeX**. UI stuff is not intermingled with the core logic but defined separately. The type-to-widget mapping is controlled by a theme and new types can be defined on top of existing types. 
-
-
-The example below shows how common UI compoents are generated from four Python-native data types: `str`, `bool`, `Literal` and `range`, as well as types in popular packages such as `ipywidgets.Password`. The example below further maps default values to placeholders in the UI widgets. From this example, we can see that developers need to **learn nothing about Funix or do nothing to their existing code** before they can get an app. 
+**The Zen of Funix** is to generate widgets for function I/Os based on their types, instead of manually picking and customizing the widget for each I/O. **Funix to Python is like CSS to HTML or style class to LaTeX**. UI stuff is not intermingled with the core logic but defined separately. The type-to-widget mapping is controlled by a theme and new types can be defined on top of existing types.
 
+The example below shows how common UI compoents are generated from four Python-native data types: `str`, `bool`, `Literal` and `range`, as well as types in popular packages such as `ipywidgets.Password`. The example below further maps default values to placeholders in the UI widgets. From this example, we can see that developers need to **learn nothing about Funix or do nothing to their existing code** before they can get an app.
 
 ```python
 import typing # Python native 
 
 import ipywidgets  # popular UI library 
 
 def input_widgets_basic(
@@ -157,15 +150,15 @@
     openai_key: ipywidgets.Password = "1234556",
     )  -> str:
     pass
 ```
 
 ![four input types](https://raw.githubusercontent.com/TexteaInc/funix-doc/main/screenshots/input_widgets.png)
 
-The example below shows how `pandas.DataFrame` and `matplotlib.figure.Figure` that AI/data developers cannot be more familiar with are mapped to tables and charts in an app. 
+The example below shows how `pandas.DataFrame` and `matplotlib.figure.Figure` that AI/data developers cannot be more familiar with are mapped to tables and charts in an app.
 
 ```python
 import pandas, matplotlib.pyplot
 from numpy import arange, log
 from numpy.random import random
 
 def table_and_plot(
@@ -180,15 +173,15 @@
     matplotlib.pyplot.plot(df["a"], df["c"], 'r')
 
     return fig
 ```
 
 ![table and plot screenshot](https://raw.githubusercontent.com/TexteaInc/funix-doc/main/screenshots/table_plot.png)
 
-You can even continuously update a plot based on user input. 
+You can even continuously update a plot based on user input.
 
 ```python
 import funix 
 import matplotlib.pyplot, matplotlib.figure
 import numpy 
 
 @funix.funix(
@@ -200,76 +193,72 @@
     y = numpy.sin(x*omega)
     matplotlib.pyplot.plot(x, y, linewidth=5)
     return fig
 ```
 
 ![continuous sine function](https://raw.githubusercontent.com/TexteaInc/funix-doc/main/screenshots/continous_run_sine.gif)
 
- 
 ### Out-of-box support for classes and OOP
 
 Funix can turn each member method of a class into a page of an app. 
 In two additional lines, the example below turn a class definition into a multi-page app with the OOP experience where the instantiation of an object of the class is done in a page corresponding to the constructor of the class and the member values of the object can be viewed and updated in other pages. **No need to manually expose** the member methods of the class.
 
 ```python
 from funix import funix_class
 
 @funix_class()  
 class A:
     def __init__(self, a: int):
         self.a = a
         return f"`self.a` has been initialized to {self.a}"
 
-    def update_a(self, b: int) -> str:
+    def set(self, b: int) -> str:
         self.a = b
         return f"`self.a` has been updated to {self.a}"
 
-    def print_a(self) -> str:
+    def get(self) -> str:
         return f"The value of `self.a` is {self.a}"
 ```
 
 ![class demo app gif](https://raw.githubusercontent.com/TexteaInc/funix-doc/main/videos/class/class.gif)
 
-
 A more advanced example of class is the wordle game. You can find the source code in [`examples/wordle.py`](./examples/games/wordle.py). In less than 100 lines, you can build Wordle! The screenshot is as follows:
 
 ![Wordle demo](https://github.com/TexteaInc/funix-doc/blob/main/screenshots/wordle.png?raw=true)
 
 ### The quickest way to build GenAI apps
 
 You can wrap any Python function into a web app in Funix.
-For example, you can take the ChatGPT demo code from OpenAI's APi reference and wrap it into a str-to-str function: 
+For example, you can take the ChatGPT demo code from OpenAI's APi reference and wrap it into a str-to-str function:
 
 ```python
 from openai import OpenAI
 
 def ChatGPT(prompt: str) -> str:    
     client = OpenAI()
 
     completion = client.chat.completions.create(
         model="gpt-3.5-turbo",
         messages=[
             {"role": "user", "content": prompt}
         ]
     )
-return completion.choices[0].message
+    return completion.choices[0].message.content
 ```
+
 which is turned into an app by Funix like below: 
 
 ![screenshots/ChatGPT_lazy.png](https://github.com/TexteaInc/funix-doc/raw/main/screenshots/chatGPT_lazy.png)
 
+### Themes: the CSS for Python
 
+**Funix to Python is like CSS to HTML or macros to LaTeX.** It separates the core logic and the UI.
+All UI stuff is centrally defined in a JSON-based theme to avoid the repetitiveness of individually configuring widgets and keep a consistent look across apps. Consequently, a data scientist or a machine learning engineer does not need to think about anything UI. Just leave it to the UI team and Funix.
 
-
-### Themes: the CSS for Python 
-
-**Funix to Python is like CSS to HTML or macros to LaTeX.** It separates the core logic and the UI. 
-All UI stuff is centrally defined in a JSON-based theme to avoid the repetitiveness of individually configuring widgets and keep a consistent look across apps. Consequently, a data scientist or a machine learning engineer does not need to think about anything UI. Just leave it to the UI team and Funix. 
-
-Below is an example of a theme file. It defines the widget choices based on variable types and tweaks the `props` of UI components (currently only MUI ones are supported). Funix exposes frontend components and their `props` to developers, requiring them to know nothing about frontend. To know more about how to define and apply a theme, please refer to [the Themes section in the reference manual](https://github.com/TexteaInc/funix-doc/blob/main/Reference.md#themes). 
+Below is an example of a theme file. It defines the widget choices based on variable types and tweaks the `props` of UI components (currently only MUI ones are supported). Funix exposes frontend components and their `props` to developers, requiring them to know nothing about frontend. To know more about how to define and apply a theme, please refer to [the Themes section in the reference manual](https://github.com/TexteaInc/funix-doc/blob/main/Reference.md#themes).
 
 ```jsonc
 {
   "name": "test_theme",
   "widgets": {    // dict, map types to widgets
     "str": "inputbox", // using Funix' widget shorthand
     "int": "slider[0,100,2]", // using Funix' widget shorthand
@@ -283,15 +272,15 @@
         }
     }, 
     "Literal": "radio"
   },
 }
 ```
 
-To introduce a new data type, just declare a new Python class, and use a decorator to let Funix know. You can associate the type with a widget either on-the-fly (below) or via a theme file. 
+To introduce a new data type, just declare a new Python class, and use a decorator to let Funix know. You can associate the type with a widget either on-the-fly (below) or via a theme file.
 
 ```python
 from funix import funix, new_funix_type
 
 @new_funix_type(
     widget = {
         "widget": "@mui/material/TextField",
@@ -311,15 +300,15 @@
 
 if __name__ == "__main__":
     print (hoho(blackout('Fun'))) 
 ```
 
 ### Python-native to web-native
 
-Funix repurposes some Python-native features to web features. 
+Funix repurposes some Python-native features to web features.
 
 First, Funix won't let your docstring or `print()` function calls go to waste. They will appear in the input and output panels of the web app.
 
 ```python
 from funix import funix
 @funix(
     print_to_web=True
@@ -351,15 +340,15 @@
     for i in range(len(message)):
         time.sleep(0.01)
         yield message[0:i]
 ```
 
 ![Streamt text to web](https://github.com/TexteaInc/funix-doc/blob/main/screenshots/stream.gif?raw=true)
 
-## Advanced features 
+## Advanced features
 
 ### History: Keep your call logs
 
 <details>
 <summary>
 Click to expand
 </summary>
@@ -409,20 +398,23 @@
 
 A special case of passing data between functions is to use the return value of one function as the value in the widget of an argument of another function. This is called prefill. Funix support prefill by using a decorator attribute `pre_fill`. Below is an example and the corresponding GIF animation.
 
 
 ```python
 import funix
 
+@funix.funix()
 def first_action(x: int) -> int:
   return x - 1
 
+@funix.funix()
 def second_action(message: str) -> list[str]:
   return message.split(" ")
 
+@funix.funix()
 def third_action(x: int, y: int) -> dict:
   return {"x": x, "y": y}
 
 @funix.funix(
   pre_fill={
     "a": first_action,
     "b": (second_action, -1),
@@ -474,48 +466,52 @@
 
 More examples in <a href="https://github.com/TexteaInc/funix-doc/blob/main/Reference.md">Reference Manual</a> or the <code>./examples</code> folder.
 
 * [ChatPaper](https://github.com/forrestbao/ChatPaper) (It's like the popular ChatPDF. But in Funix, only 70 lines of code needed.)
 * [mFlux](https://github.com/Yazawazi/MFlux) (synthetic biology)
 
 ### ChatGPT, multi-turn
+
 <details>
   <summary><code>examples/AI/chatGPT_multi_turn.py</code> 👈 Toggle me to show source code </summary>
 
   ```python
     import os
     import IPython     
-    import openai
-    openai.api_key = os.environ.get("OPENAI_KEY")
+    from openai import OpenAI
+    import funix
+
+    client = OpenAI(api_key=os.environ.get("OPENAI_KEY"))
 
     messages  = []  # list of dicts, dict keys: role, content, system
 
+    @funix.funix(
+        disable=True,
+    )
     def print_messages_html(messages):
         printout = ""
         for message in messages:
             if message["role"] == "user":
-                align, left, name = "left", "0%", "You"
+                align, name = "left", "You"
             elif message["role"] == "assistant":
-                align, left, name = "right", "30%", "ChatGPT"
-            printout += f'<div style="position: relative; left: {left}; width: 70%"><b>{name}</b>: {message["content"]}</div>'
+                align, name = "right", "ChatGPT"
+            printout += f'<div style="width: 100%; text-align: {align}"><b>{name}</b>: {message["content"]}</div>'
         return printout
 
-    import funix
+
     @funix.funix(
         direction="column-reverse",
     )
     def ChatGPT_multi_turn(current_message: str)  -> IPython.display.HTML:
         current_message = current_message.strip()
         messages.append({"role": "user", "content": current_message})
-        completion = openai.ChatCompletion.create(
-            messages=messages,
-            model='gpt-3.5-turbo',
-            max_tokens=100,
-        )
-        chatgpt_response = completion["choices"][0]["message"]["content"]
+        completion = client.chat.completions.create(messages=messages,
+        model='gpt-3.5-turbo',
+        max_tokens=100)
+        chatgpt_response = completion.choices[0].message.content
         messages.append({"role": "assistant", "content": chatgpt_response})
 
         # return print_messages_markdown(messages)
         return print_messages_html(messages)
 
   ```
 
@@ -523,23 +519,25 @@
 
 ![Multiturn chat](https://github.com/TexteaInc/funix-doc/raw/main/screenshots/chatGPT_multiturn.png)
 
 ### Shortest Dall-E web app in Python
 
 ```python
 from funix import funix                      # add line one
-from funix.hint import Images                # add line two
-import openai  # pip install openai
+from IPython.display import Image
+from openai import OpenAI                    # pip install openai
+
+import os
+client = OpenAI(api_key=os.environ.get("OPENAI_KEY"))  
 
-openai.api_key = os.environ.get("OPENAI_KEY")
 
-@funix()                                     # add line three
+@funix()                                     # add line two
 def dalle(prompt: str = "a cat") -> Image:
-    response = openai.Image.create(prompt=prompt)
-    return response["data"][0]["url"]
+    response = client.images.generate(prompt=prompt)
+    return response.data[0].url
 ```
 
 ![Dalle demo](https://github.com/TexteaInc/funix-doc/raw/main/screenshots/dalle.jpg)
 
 <!-- Funix.io can get the same job done in half the amount of code required by Gradio, by exploiting the Python language as much as possible. Here, state/session is maintained using a global variable, while the order of the returns defines the return layout.  -->
 
 ### Bioinformatics: vector stripping
@@ -550,25 +548,26 @@
 
 ### Multimedia inputs and outputs
 
 <details>
 <summary><code>examples/multimedia/rgb2gray.py</code> 👈 Toggle me to show source code</summary>
 
 ```python
-import  io # Python's native
+import  io # Python's native 
 
 import PIL # the Python Image Library
-import funix
+import IPython 
+import funix 
 
 @funix.funix(
     title="Convert color images to grayscale images",
 )
-def gray_it(image: funix.hint.BytesImage) -> funix.hint.Image:
+def gray_it(image: funix.hint.BytesImage) -> IPython.display.Image:
     img = PIL.Image.open(io.BytesIO(image))
-    gray = PIL.ImageOps.grayscale(img)
+    gray = PIL.ImageOps.grayscale(img) 
     output = io.BytesIO()
     gray.save(output, format="PNG")
     return output.getvalue()
 ```
 </details>
 
 ![shipping example](https://raw.githubusercontent.com/TexteaInc/funix-doc/main/screenshots/rgb2gray.png)
@@ -586,41 +585,67 @@
 * From PyPI (stable, lacking the latest feature)
     ```bash
     pip install funix
     ```
 * From GitHub (latest)
 
     ```bash
-    pip -b develop install "git+https://github.com/TexteaInc/funix.git"
+    pip install "git+https://github.com/TexteaInc/funix.git@develop" # Develop version
+    pip install "git+https://github.com/TexteaInc/funix.git" # Stable version
     ```
 * Local development
 
     ```bash
     git clone -b develop https://github.com/TexteaInc/funix
     cd funix
     pip install -e .
     ```
     Add `--prefix=~/.local` if pip insists to install to system paths. See [#24](https://github.com/TexteaInc/funix/issues/24) and [#23](https://github.com/TexteaInc/funix/issues/23)
 
+### Additional type support
+
+1. If you want to use `git` related features (use project from GitHub), install funix by:
+    
+    ```bash
+    pip install funix[git]
+    ```
+
+2. If you want to use `ipython` features, install funix by:
+    
+    ```bash
+    pip install funix[ipython]
+    ```
+
+3. If you need to have more than one feature, you can try installing them together:
+    
+    ```bash
+    pip install funix[all]
+    ```
+
 ### Building the frontend
 
 In the last two cases above, you will need to compile the frontend by yourself. Suppose you are in the `funix` folder. Then run the following commands:
 
 1. `cd frontend`
-3. `yarn install`
-4. `yarn start`
+2. `yarn install` (you need install Node.JS and Yarn)
+3. `yarn funix:build`
+
+For debugging:
+
+1. `yarn funix:test` (Start development mode)
+2. `funix xxx -p 8080 -F` (Use 8080 port and no frontend mode)
 
 #### Building the frontend with MUI Pro
 
 Our table widget uses advanced features in MUI Pro. If you have a MUI Pro license, you can build the frontend with MUI Pro by following the steps below:
 
 1. Install Node.js and Yarn;
 2. Create a file called `.env` in the `frontend` folder;
 3. Add `MUI_PRO_LICENSE_KEY=[your_key]` to the file;
-4. Run `yarn funix:build` to build the frontend;
+4. Run `yarn install && yarn funix:build` to build the frontend;
 5. Done!
 
 ### Command line options
 
 Run the command below to see the command line options:
 
 ```text
@@ -650,12 +675,13 @@
 
 ## How to contribute
 
 Funix is open-sourced under the MIT License. Community contribution is not only welcomed but desired. Feel free to fork and make a pull request when you are ready. You can also report bugs, suggest new features via the [issue tracker](https://github.com/TexteaInc/funix/issues/new) or our [Discord server](https://discord.gg/JyANAMUAHM).
 
 ## Acknowledgment
 
-Funix draws inspiration from FastAPI and Python-Fire: building software interfaces by inferring from function signatures containing type hints. We port this idea from the backend (FastAPI) or the terminal (Python-Fire) to the frontend. We also thank Streamlit, Gradio, PyWebIO, and Pynecone/Reflex. They inspired us. We are just too lazy to manually define widgets imperatively. Funix’s backend is implemented in Flask and the frontend in Material UI. 
+Funix draws inspiration from FastAPI and Python-Fire: building software interfaces by inferring from function signatures containing type hints. We port this idea from the backend (FastAPI) or the terminal (Python-Fire) to the frontend. We also thank Streamlit, Gradio, PyWebIO, and Pynecone/Reflex. They inspired us. We are just too lazy to manually define widgets imperatively. Funix’s backend is implemented in Flask and the frontend in Material UI.
 
 ## Contact
 
-hello at funix dot io
+Forrest dot Bao @ Gmail 
+
```

### Comparing `funix-0.5.7/backend/funix.egg-info/SOURCES.txt` & `funix-0.5.8/backend/funix.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 backend/funix/build/index.html
 backend/funix/build/logo192.png
 backend/funix/build/logo512.png
 backend/funix/build/manifest.json
 backend/funix/build/static/css/main.4efb37a3.css
 backend/funix/build/static/js/d3.v5.js
 backend/funix/build/static/js/jquery-3.7.1.min.js
-backend/funix/build/static/js/main.0af491b9.js
-backend/funix/build/static/js/main.0af491b9.js.LICENSE.txt
+backend/funix/build/static/js/main.279c7e85.js
+backend/funix/build/static/js/main.279c7e85.js.LICENSE.txt
 backend/funix/build/static/js/mpld3.v0.5.8.js
 backend/funix/config/__init__.py
 backend/funix/config/switch.py
 backend/funix/decorator/__init__.py
 backend/funix/decorator/all_of.py
 backend/funix/decorator/annnotation_analyzer.py
 backend/funix/decorator/call.py
```

### Comparing `funix-0.5.7/pyproject.toml` & `funix-0.5.8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "funix"
-version = "0.5.7"
+version = "0.5.8"
 authors = [
-  {name = "Textea Inc.", email = "hello@funix.io"}
+  {name = "Textea Inc.", email = "forrestbao@gmail.com"}
 ]
 license = {file = "LICENSE"}
 description = "Building web apps without manually creating widgets"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
   "Development Status :: 4 - Beta",
@@ -20,41 +20,33 @@
 dependencies = [
   "flask>=2.2.2",
   "functions-framework==3.*",
   "requests>=2.28.1",
   "plac>=1.3.5",
   "gitignore-parser>=0.1.9",
   "flask-sock>=0.7.0",
-  "SQLAlchemy>=2.0.23"
-]
-
-[project.optional-dependencies]
-plot = [
+  "SQLAlchemy>=2.0.23",
   "matplotlib>=3.4.3",
   "mpld3>=0.5.8",
+  "pandera>=0.17.2",
+  "pandas>=2.0.3",
 ]
+
+[project.optional-dependencies]
 git = [
   "GitPython>=3.1.31",
 ]
 ipython = [
   "IPython>=8.14.0",
   "ipywidgets>=8.0.7",
 ]
-pandas = [
-  "pandera>=0.17.2",
-  "pandas>=2.0.3",
-]
 all = [
-  "matplotlib>=3.4.3",
-  "mpld3>=0.5.8",
   "GitPython>=3.1.31",
   "IPython>=8.14.0",
   "ipywidgets>=8.0.7",
-  "pandera>=0.17.2",
-  "pandas>=2.0.3",
 ]
 
 [project.urls]
 homepage = "https://github.com/TexteaInc/funix"
 
 [project.scripts]
 funix = "funix.__main__:cli_main"
```

