# Comparing `tmp/tdh-tcd-2.5.3.tar.gz` & `tmp/tdh_tcd-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdh-tcd-2.5.3.tar", last modified: Mon May  8 00:41:35 2023, max compression
+gzip compressed data, was "tdh_tcd-2.5.4.tar", last modified: Fri May 17 21:19:08 2024, max compression
```

## Comparing `tdh-tcd-2.5.3.tar` & `tdh_tcd-2.5.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:41:35.989564 tdh-tcd-2.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-08 00:41:22.000000 tdh-tcd-2.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-08 00:41:35.989564 tdh-tcd-2.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-08 00:41:22.000000 tdh-tcd-2.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 00:41:35.989564 tdh-tcd-2.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-08 00:41:22.000000 tdh-tcd-2.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:41:35.985564 tdh-tcd-2.5.3/tcd/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-08 00:41:22.000000 tdh-tcd-2.5.3/tcd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-08 00:41:22.000000 tdh-tcd-2.5.3/tcd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-08 00:41:22.000000 tdh-tcd-2.5.3/tcd/example.settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-05-08 00:41:22.000000 tdh-tcd-2.5.3/tcd/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-05-08 00:41:22.000000 tdh-tcd-2.5.3/tcd/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-05-08 00:41:22.000000 tdh-tcd-2.5.3/tcd/twitch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:41:35.989564 tdh-tcd-2.5.3/tdh_tcd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-08 00:41:35.000000 tdh-tcd-2.5.3/tdh_tcd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-08 00:41:35.000000 tdh-tcd-2.5.3/tdh_tcd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 00:41:35.000000 tdh-tcd-2.5.3/tdh_tcd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-08 00:41:35.000000 tdh-tcd-2.5.3/tdh_tcd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-08 00:41:35.000000 tdh-tcd-2.5.3/tdh_tcd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-08 00:41:35.000000 tdh-tcd-2.5.3/tdh_tcd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:19:08.650084 tdh_tcd-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-17 21:19:00.000000 tdh_tcd-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-05-17 21:19:08.650084 tdh_tcd-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-17 21:19:00.000000 tdh_tcd-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 21:19:08.650084 tdh_tcd-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-17 21:19:00.000000 tdh_tcd-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:19:08.646083 tdh_tcd-2.5.4/tcd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-17 21:19:00.000000 tdh_tcd-2.5.4/tcd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-17 21:19:00.000000 tdh_tcd-2.5.4/tcd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-17 21:19:00.000000 tdh_tcd-2.5.4/tcd/example.settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-05-17 21:19:00.000000 tdh_tcd-2.5.4/tcd/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-05-17 21:19:00.000000 tdh_tcd-2.5.4/tcd/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8910 2024-05-17 21:19:00.000000 tdh_tcd-2.5.4/tcd/twitch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:19:08.650084 tdh_tcd-2.5.4/tdh_tcd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-05-17 21:19:08.000000 tdh_tcd-2.5.4/tdh_tcd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-17 21:19:08.000000 tdh_tcd-2.5.4/tdh_tcd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 21:19:08.000000 tdh_tcd-2.5.4/tdh_tcd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-17 21:19:08.000000 tdh_tcd-2.5.4/tdh_tcd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-17 21:19:08.000000 tdh_tcd-2.5.4/tdh_tcd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-17 21:19:08.000000 tdh_tcd-2.5.4/tdh_tcd.egg-info/top_level.txt
```

### Comparing `tdh-tcd-2.5.3/LICENSE` & `tdh_tcd-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tdh-tcd-2.5.3/PKG-INFO` & `tdh_tcd-2.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: tdh-tcd
-Version: 2.5.3
+Version: 2.5.4
 Summary: Twitch Chat Downloader
 Home-page: https://github.com/TheDrHax/Twitch-Chat-Downloader
 Author: Dmitry Karikh
 Author-email: the.dr.hax@gmail.com
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: progressbar2
+Requires-Dist: iso8601
 
 # Twitch Chat Downloader [![PyPI version](https://badge.fury.io/py/tdh-tcd.svg)](https://badge.fury.io/py/tdh-tcd)
 
 Neat python script to download chat messages from past broadcasts
 
 ## Requirements
```

### Comparing `tdh-tcd-2.5.3/README.md` & `tdh_tcd-2.5.4/README.md`

 * *Files identical despite different names*

### Comparing `tdh-tcd-2.5.3/setup.py` & `tdh_tcd-2.5.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open('README.md', 'r') as fi:
     long_description = fi.read()
 
 
 setup(
     name='tdh-tcd',
-    version='2.5.3',
+    version='2.5.4',
 
     author='Dmitry Karikh',
     author_email='the.dr.hax@gmail.com',
 
     description='Twitch Chat Downloader',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `tdh-tcd-2.5.3/tcd/__init__.py` & `tdh_tcd-2.5.4/tcd/__init__.py`

 * *Files identical despite different names*

### Comparing `tdh-tcd-2.5.3/tcd/example.settings.json` & `tdh_tcd-2.5.4/tcd/example.settings.json`

 * *Files identical despite different names*

### Comparing `tdh-tcd-2.5.3/tcd/settings.py` & `tdh_tcd-2.5.4/tcd/settings.py`

 * *Files identical despite different names*

### Comparing `tdh-tcd-2.5.3/tcd/subtitles.py` & `tdh_tcd-2.5.4/tcd/subtitles.py`

 * *Files identical despite different names*

### Comparing `tdh-tcd-2.5.3/tcd/twitch.py` & `tdh_tcd-2.5.4/tcd/twitch.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
 class Messages(object):
     def __init__(self, video_id):
         self.video_id = video_id
 
         video = gql(f'''
             query {{
-                video(id: {video_id}) {{
+                video(id: "{video_id}") {{
                     creator {{
                         displayName
                         id
                     }}
                     createdAt
                     lengthSeconds
                     title
```

### Comparing `tdh-tcd-2.5.3/tdh_tcd.egg-info/PKG-INFO` & `tdh_tcd-2.5.4/tdh_tcd.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: tdh-tcd
-Version: 2.5.3
+Version: 2.5.4
 Summary: Twitch Chat Downloader
 Home-page: https://github.com/TheDrHax/Twitch-Chat-Downloader
 Author: Dmitry Karikh
 Author-email: the.dr.hax@gmail.com
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: progressbar2
+Requires-Dist: iso8601
 
 # Twitch Chat Downloader [![PyPI version](https://badge.fury.io/py/tdh-tcd.svg)](https://badge.fury.io/py/tdh-tcd)
 
 Neat python script to download chat messages from past broadcasts
 
 ## Requirements
```

