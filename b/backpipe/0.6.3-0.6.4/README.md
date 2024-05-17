# Comparing `tmp/backpipe-0.6.3.tar.gz` & `tmp/backpipe-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backpipe-0.6.3.tar", last modified: Wed May 15 20:52:58 2024, max compression
+gzip compressed data, was "backpipe-0.6.4.tar", last modified: Fri May 17 21:28:45 2024, max compression
```

## Comparing `backpipe-0.6.3.tar` & `backpipe-0.6.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-15 20:52:58.112189 backpipe-0.6.3/
--rw-r--r--   0 simon     (1000) simon     (1000)    35129 2023-11-04 20:14:40.000000 backpipe-0.6.3/LICENSE
--rw-r--r--   0 simon     (1000) simon     (1000)      176 2024-04-22 18:38:17.000000 backpipe-0.6.3/MANIFEST.in
--rw-r--r--   0 simon     (1000) simon     (1000)     3525 2024-05-15 20:52:58.111189 backpipe-0.6.3/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)     2872 2024-05-09 11:06:37.000000 backpipe-0.6.3/README.md
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-15 20:52:58.106189 backpipe-0.6.3/backpipe/
--rw-r--r--   0 simon     (1000) simon     (1000)      537 2024-05-15 20:43:50.000000 backpipe-0.6.3/backpipe/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)     5172 2024-04-26 15:29:12.000000 backpipe-0.6.3/backpipe/__main__.py
--rw-r--r--   0 simon     (1000) simon     (1000)     5682 2024-05-15 20:43:50.000000 backpipe-0.6.3/backpipe/app.py
--rw-r--r--   0 simon     (1000) simon     (1000)     3535 2024-05-14 16:10:35.000000 backpipe-0.6.3/backpipe/builder.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1027 2024-05-09 11:37:15.000000 backpipe-0.6.3/backpipe/config.py
--rw-r--r--   0 simon     (1000) simon     (1000)      364 2024-03-29 01:51:22.000000 backpipe-0.6.3/backpipe/defaults.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1916 2024-05-09 19:47:37.000000 backpipe-0.6.3/backpipe/host.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-15 20:52:58.107189 backpipe-0.6.3/backpipe/presets/
--rw-r--r--   0 simon     (1000) simon     (1000)      627 2024-05-09 14:02:28.000000 backpipe-0.6.3/backpipe/presets/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1528 2024-05-14 16:14:59.000000 backpipe-0.6.3/backpipe/presets/file.py
--rw-r--r--   0 simon     (1000) simon     (1000)      465 2024-05-14 15:59:22.000000 backpipe-0.6.3/backpipe/presets/ipaddr.py
--rw-r--r--   0 simon     (1000) simon     (1000)      870 2024-05-09 15:37:55.000000 backpipe-0.6.3/backpipe/presets/redirect.py
--rw-r--r--   0 simon     (1000) simon     (1000)      600 2024-05-14 15:54:50.000000 backpipe-0.6.3/backpipe/redirect.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1233 2024-05-09 10:28:38.000000 backpipe-0.6.3/backpipe/rq.py
--rw-r--r--   0 simon     (1000) simon     (1000)     7185 2024-05-10 12:09:45.000000 backpipe-0.6.3/backpipe/server.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-15 20:52:58.107189 backpipe-0.6.3/backpipe/tools/
--rw-r--r--   0 simon     (1000) simon     (1000)      178 2024-04-22 17:36:44.000000 backpipe-0.6.3/backpipe/tools/__init__.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-15 20:52:58.108189 backpipe-0.6.3/backpipe/tools/base64/
--rw-r--r--   0 simon     (1000) simon     (1000)       95 2024-04-15 14:45:34.000000 backpipe-0.6.3/backpipe/tools/base64/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)      177 2024-04-15 14:45:00.000000 backpipe-0.6.3/backpipe/tools/base64/decode.py
--rw-r--r--   0 simon     (1000) simon     (1000)      177 2024-04-15 14:43:40.000000 backpipe-0.6.3/backpipe/tools/base64/encode.py
--rw-r--r--   0 simon     (1000) simon     (1000)      398 2024-04-15 15:05:34.000000 backpipe-0.6.3/backpipe/tools/check_type.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-15 20:52:58.108189 backpipe-0.6.3/backpipe/tools/file/
--rw-r--r--   0 simon     (1000) simon     (1000)      181 2024-04-22 17:06:34.000000 backpipe-0.6.3/backpipe/tools/file/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)      464 2024-04-22 17:03:16.000000 backpipe-0.6.3/backpipe/tools/file/append.py
--rw-r--r--   0 simon     (1000) simon     (1000)      301 2024-04-22 16:26:18.000000 backpipe-0.6.3/backpipe/tools/file/create.py
--rw-r--r--   0 simon     (1000) simon     (1000)      388 2024-04-22 16:51:25.000000 backpipe-0.6.3/backpipe/tools/file/delete.py
--rw-r--r--   0 simon     (1000) simon     (1000)      463 2024-04-22 16:39:25.000000 backpipe-0.6.3/backpipe/tools/file/write.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-15 20:52:58.110189 backpipe-0.6.3/backpipe/tools/hash/
--rw-r--r--   0 simon     (1000) simon     (1000)      265 2024-04-22 17:45:34.000000 backpipe-0.6.3/backpipe/tools/hash/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)      284 2024-04-22 17:41:35.000000 backpipe-0.6.3/backpipe/tools/hash/md5.py
--rw-r--r--   0 simon     (1000) simon     (1000)      286 2024-04-22 17:41:54.000000 backpipe-0.6.3/backpipe/tools/hash/sha1.py
--rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:42:44.000000 backpipe-0.6.3/backpipe/tools/hash/sha224.py
--rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:42:57.000000 backpipe-0.6.3/backpipe/tools/hash/sha256.py
--rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:44:00.000000 backpipe-0.6.3/backpipe/tools/hash/sha384.py
--rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:44:07.000000 backpipe-0.6.3/backpipe/tools/hash/sha512.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-15 20:52:58.110189 backpipe-0.6.3/backpipe/tools/html/
--rw-r--r--   0 simon     (1000) simon     (1000)       41 2024-04-14 18:21:28.000000 backpipe-0.6.3/backpipe/tools/html/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)      212 2024-04-14 20:54:18.000000 backpipe-0.6.3/backpipe/tools/html/addMeta.py
--rw-r--r--   0 simon     (1000) simon     (1000)      130 2024-04-14 20:54:11.000000 backpipe-0.6.3/backpipe/tools/html/addStyle.py
--rw-r--r--   0 simon     (1000) simon     (1000)      346 2024-04-27 09:07:22.000000 backpipe-0.6.3/backpipe/tools/html/addTag.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1176 2024-04-27 09:10:21.000000 backpipe-0.6.3/backpipe/tools/html/html.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-15 20:52:58.111189 backpipe-0.6.3/backpipe/tools/json/
--rw-r--r--   0 simon     (1000) simon     (1000)      107 2024-04-14 16:06:07.000000 backpipe-0.6.3/backpipe/tools/json/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)      289 2024-05-15 20:48:24.000000 backpipe-0.6.3/backpipe/tools/json/deserialize.py
--rw-r--r--   0 simon     (1000) simon     (1000)      262 2024-04-15 14:42:48.000000 backpipe-0.6.3/backpipe/tools/json/serialize.py
--rw-r--r--   0 simon     (1000) simon     (1000)      137 2023-11-14 15:08:41.000000 backpipe-0.6.3/backpipe/uptime.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-15 20:52:58.106189 backpipe-0.6.3/backpipe.egg-info/
--rw-r--r--   0 simon     (1000) simon     (1000)     3525 2024-05-15 20:52:58.000000 backpipe-0.6.3/backpipe.egg-info/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)     1316 2024-05-15 20:52:58.000000 backpipe-0.6.3/backpipe.egg-info/SOURCES.txt
--rw-r--r--   0 simon     (1000) simon     (1000)        1 2024-05-15 20:52:58.000000 backpipe-0.6.3/backpipe.egg-info/dependency_links.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       52 2024-05-15 20:52:58.000000 backpipe-0.6.3/backpipe.egg-info/entry_points.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       19 2024-05-15 20:52:58.000000 backpipe-0.6.3/backpipe.egg-info/requires.txt
--rw-r--r--   0 simon     (1000) simon     (1000)        9 2024-05-15 20:52:58.000000 backpipe-0.6.3/backpipe.egg-info/top_level.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       38 2024-05-15 20:52:58.112189 backpipe-0.6.3/setup.cfg
--rw-r--r--   0 simon     (1000) simon     (1000)     1532 2024-04-26 16:49:47.000000 backpipe-0.6.3/setup.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-17 21:28:45.305904 backpipe-0.6.4/
+-rw-r--r--   0 simon     (1000) simon     (1000)    35129 2023-11-04 20:14:40.000000 backpipe-0.6.4/LICENSE
+-rw-r--r--   0 simon     (1000) simon     (1000)      176 2024-04-22 18:38:17.000000 backpipe-0.6.4/MANIFEST.in
+-rw-r--r--   0 simon     (1000) simon     (1000)     3456 2024-05-17 21:28:45.304904 backpipe-0.6.4/PKG-INFO
+-rw-r--r--   0 simon     (1000) simon     (1000)     2803 2024-05-17 21:26:25.000000 backpipe-0.6.4/README.md
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-17 21:28:45.300904 backpipe-0.6.4/backpipe/
+-rw-r--r--   0 simon     (1000) simon     (1000)      537 2024-05-17 21:27:59.000000 backpipe-0.6.4/backpipe/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     5172 2024-04-26 15:29:12.000000 backpipe-0.6.4/backpipe/__main__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     5682 2024-05-15 20:54:20.000000 backpipe-0.6.4/backpipe/app.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     3535 2024-05-14 16:10:35.000000 backpipe-0.6.4/backpipe/builder.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1027 2024-05-09 11:37:15.000000 backpipe-0.6.4/backpipe/config.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      364 2024-03-29 01:51:22.000000 backpipe-0.6.4/backpipe/defaults.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1916 2024-05-09 19:47:37.000000 backpipe-0.6.4/backpipe/host.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-17 21:28:45.301904 backpipe-0.6.4/backpipe/presets/
+-rw-r--r--   0 simon     (1000) simon     (1000)      627 2024-05-09 14:02:28.000000 backpipe-0.6.4/backpipe/presets/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1528 2024-05-14 16:14:59.000000 backpipe-0.6.4/backpipe/presets/file.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      465 2024-05-14 15:59:22.000000 backpipe-0.6.4/backpipe/presets/ipaddr.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      870 2024-05-09 15:37:55.000000 backpipe-0.6.4/backpipe/presets/redirect.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      600 2024-05-14 15:54:50.000000 backpipe-0.6.4/backpipe/redirect.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1233 2024-05-09 10:28:38.000000 backpipe-0.6.4/backpipe/rq.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     7185 2024-05-10 12:09:45.000000 backpipe-0.6.4/backpipe/server.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-17 21:28:45.302904 backpipe-0.6.4/backpipe/tools/
+-rw-r--r--   0 simon     (1000) simon     (1000)      178 2024-04-22 17:36:44.000000 backpipe-0.6.4/backpipe/tools/__init__.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-17 21:28:45.302904 backpipe-0.6.4/backpipe/tools/base64/
+-rw-r--r--   0 simon     (1000) simon     (1000)       95 2024-04-15 14:45:34.000000 backpipe-0.6.4/backpipe/tools/base64/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      249 2024-05-17 21:27:59.000000 backpipe-0.6.4/backpipe/tools/base64/decode.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      255 2024-05-17 21:27:59.000000 backpipe-0.6.4/backpipe/tools/base64/encode.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      398 2024-04-15 15:05:34.000000 backpipe-0.6.4/backpipe/tools/check_type.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-17 21:28:45.303904 backpipe-0.6.4/backpipe/tools/file/
+-rw-r--r--   0 simon     (1000) simon     (1000)      181 2024-04-22 17:06:34.000000 backpipe-0.6.4/backpipe/tools/file/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      464 2024-04-22 17:03:16.000000 backpipe-0.6.4/backpipe/tools/file/append.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      301 2024-04-22 16:26:18.000000 backpipe-0.6.4/backpipe/tools/file/create.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      388 2024-04-22 16:51:25.000000 backpipe-0.6.4/backpipe/tools/file/delete.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      463 2024-04-22 16:39:25.000000 backpipe-0.6.4/backpipe/tools/file/write.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-17 21:28:45.303904 backpipe-0.6.4/backpipe/tools/hash/
+-rw-r--r--   0 simon     (1000) simon     (1000)      265 2024-04-22 17:45:34.000000 backpipe-0.6.4/backpipe/tools/hash/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      284 2024-04-22 17:41:35.000000 backpipe-0.6.4/backpipe/tools/hash/md5.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      286 2024-04-22 17:41:54.000000 backpipe-0.6.4/backpipe/tools/hash/sha1.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:42:44.000000 backpipe-0.6.4/backpipe/tools/hash/sha224.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:42:57.000000 backpipe-0.6.4/backpipe/tools/hash/sha256.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:44:00.000000 backpipe-0.6.4/backpipe/tools/hash/sha384.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:44:07.000000 backpipe-0.6.4/backpipe/tools/hash/sha512.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-17 21:28:45.304904 backpipe-0.6.4/backpipe/tools/html/
+-rw-r--r--   0 simon     (1000) simon     (1000)       41 2024-04-14 18:21:28.000000 backpipe-0.6.4/backpipe/tools/html/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      212 2024-04-14 20:54:18.000000 backpipe-0.6.4/backpipe/tools/html/addMeta.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      130 2024-04-14 20:54:11.000000 backpipe-0.6.4/backpipe/tools/html/addStyle.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      346 2024-04-27 09:07:22.000000 backpipe-0.6.4/backpipe/tools/html/addTag.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1176 2024-04-27 09:10:21.000000 backpipe-0.6.4/backpipe/tools/html/html.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-17 21:28:45.304904 backpipe-0.6.4/backpipe/tools/json/
+-rw-r--r--   0 simon     (1000) simon     (1000)      107 2024-04-14 16:06:07.000000 backpipe-0.6.4/backpipe/tools/json/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      289 2024-05-15 20:54:20.000000 backpipe-0.6.4/backpipe/tools/json/deserialize.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      262 2024-04-15 14:42:48.000000 backpipe-0.6.4/backpipe/tools/json/serialize.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      137 2023-11-14 15:08:41.000000 backpipe-0.6.4/backpipe/uptime.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-17 21:28:45.301904 backpipe-0.6.4/backpipe.egg-info/
+-rw-r--r--   0 simon     (1000) simon     (1000)     3456 2024-05-17 21:28:45.000000 backpipe-0.6.4/backpipe.egg-info/PKG-INFO
+-rw-r--r--   0 simon     (1000) simon     (1000)     1316 2024-05-17 21:28:45.000000 backpipe-0.6.4/backpipe.egg-info/SOURCES.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)        1 2024-05-17 21:28:45.000000 backpipe-0.6.4/backpipe.egg-info/dependency_links.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       52 2024-05-17 21:28:45.000000 backpipe-0.6.4/backpipe.egg-info/entry_points.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       19 2024-05-17 21:28:45.000000 backpipe-0.6.4/backpipe.egg-info/requires.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)        9 2024-05-17 21:28:45.000000 backpipe-0.6.4/backpipe.egg-info/top_level.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       38 2024-05-17 21:28:45.305904 backpipe-0.6.4/setup.cfg
+-rw-r--r--   0 simon     (1000) simon     (1000)     1532 2024-04-26 16:49:47.000000 backpipe-0.6.4/setup.py
```

### Comparing `backpipe-0.6.3/LICENSE` & `backpipe-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `backpipe-0.6.3/PKG-INFO` & `backpipe-0.6.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backpipe
-Version: 0.6.3
+Version: 0.6.4
 Summary: A backend HTTP framework for Python.
 Home-page: https://github.com/Simoso68/backpipe
 Author: Simoso68
 Maintainer: Simoso68
 License: GNU GPL v3
 Keywords: framework,http,web,api,server
 Classifier: Development Status :: 4 - Beta
@@ -128,15 +128,15 @@
 When activating HTTPS, you need to sign your certificate file \
 with a key provided by a trusted authority. \
 \
 Self-signing your certificate will make tools such as \
 CURL, your Browser, etc. raise a warning, \
 that the website may be unsafe.
 
-## Documentation for dummies
+## Documentation
 
-Read through the [Documentation for Dummies](https://github.com/Simoso68/backpipe/blob/main/DOCUMENTATION_FOR_DUMMIES.md), \
+Read through the [Documentation](https://backpipe.streamlit.app), \
 to get started with backpipe
 
 ## License
 
 Backpipe is licensed under the GNU GPL v3.
```

### Comparing `backpipe-0.6.3/README.md` & `backpipe-0.6.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 When activating HTTPS, you need to sign your certificate file \
 with a key provided by a trusted authority. \
 \
 Self-signing your certificate will make tools such as \
 CURL, your Browser, etc. raise a warning, \
 that the website may be unsafe.
 
-## Documentation for dummies
+## Documentation
 
-Read through the [Documentation for Dummies](https://github.com/Simoso68/backpipe/blob/main/DOCUMENTATION_FOR_DUMMIES.md), \
+Read through the [Documentation](https://backpipe.streamlit.app), \
 to get started with backpipe
 
 ## License
 
 Backpipe is licensed under the GNU GPL v3.
```

### Comparing `backpipe-0.6.3/backpipe/__init__.py` & `backpipe-0.6.4/backpipe/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 from backpipe.redirect import redirect
 from colorama import init as __init
 
 import backpipe.tools as tools
 
 __init()
 
-__version__ = "0.6.3"
+__version__ = "0.6.4"
```

### Comparing `backpipe-0.6.3/backpipe/__main__.py` & `backpipe-0.6.4/backpipe/__main__.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.6.3/backpipe/app.py` & `backpipe-0.6.4/backpipe/app.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.6.3/backpipe/builder.py` & `backpipe-0.6.4/backpipe/builder.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.6.3/backpipe/config.py` & `backpipe-0.6.4/backpipe/config.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.6.3/backpipe/host.py` & `backpipe-0.6.4/backpipe/host.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.6.3/backpipe/presets/__init__.py` & `backpipe-0.6.4/backpipe/presets/__init__.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.6.3/backpipe/presets/file.py` & `backpipe-0.6.4/backpipe/presets/file.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.6.3/backpipe/presets/redirect.py` & `backpipe-0.6.4/backpipe/presets/redirect.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.6.3/backpipe/redirect.py` & `backpipe-0.6.4/backpipe/redirect.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.6.3/backpipe/rq.py` & `backpipe-0.6.4/backpipe/rq.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.6.3/backpipe/server.py` & `backpipe-0.6.4/backpipe/server.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.6.3/backpipe/tools/html/html.py` & `backpipe-0.6.4/backpipe/tools/html/html.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.6.3/backpipe.egg-info/PKG-INFO` & `backpipe-0.6.4/backpipe.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backpipe
-Version: 0.6.3
+Version: 0.6.4
 Summary: A backend HTTP framework for Python.
 Home-page: https://github.com/Simoso68/backpipe
 Author: Simoso68
 Maintainer: Simoso68
 License: GNU GPL v3
 Keywords: framework,http,web,api,server
 Classifier: Development Status :: 4 - Beta
@@ -128,15 +128,15 @@
 When activating HTTPS, you need to sign your certificate file \
 with a key provided by a trusted authority. \
 \
 Self-signing your certificate will make tools such as \
 CURL, your Browser, etc. raise a warning, \
 that the website may be unsafe.
 
-## Documentation for dummies
+## Documentation
 
-Read through the [Documentation for Dummies](https://github.com/Simoso68/backpipe/blob/main/DOCUMENTATION_FOR_DUMMIES.md), \
+Read through the [Documentation](https://backpipe.streamlit.app), \
 to get started with backpipe
 
 ## License
 
 Backpipe is licensed under the GNU GPL v3.
```

### Comparing `backpipe-0.6.3/backpipe.egg-info/SOURCES.txt` & `backpipe-0.6.4/backpipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backpipe-0.6.3/setup.py` & `backpipe-0.6.4/setup.py`

 * *Files identical despite different names*

