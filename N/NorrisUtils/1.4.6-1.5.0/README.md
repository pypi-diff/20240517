# Comparing `tmp/NorrisUtils-1.4.6.tar.gz` & `tmp/NorrisUtils-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NorrisUtils-1.4.6.tar", last modified: Wed May  8 06:26:04 2024, max compression
+gzip compressed data, was "NorrisUtils-1.5.0.tar", last modified: Fri May 17 06:08:15 2024, max compression
```

## Comparing `NorrisUtils-1.4.6.tar` & `NorrisUtils-1.5.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 htd        (502) staff       (20)        0 2024-05-08 06:26:04.602480 NorrisUtils-1.4.6/
-drwxr-xr-x   0 htd        (502) staff       (20)        0 2024-05-08 06:26:04.599652 NorrisUtils-1.4.6/NorrisUtils/
--rw-r--r--   0 htd        (502) staff       (20)       42 2022-12-21 09:04:02.000000 NorrisUtils-1.4.6/NorrisUtils/BuildConfig.py
--rw-r--r--   0 htd        (502) staff       (20)    12658 2024-05-08 06:25:19.000000 NorrisUtils-1.4.6/NorrisUtils/DingTalkGenius.py
--rw-r--r--   0 htd        (502) staff       (20)     5581 2023-10-17 09:11:02.000000 NorrisUtils-1.4.6/NorrisUtils/FileUtil.py
--rw-r--r--   0 htd        (502) staff       (20)     1392 2022-12-21 09:04:02.000000 NorrisUtils-1.4.6/NorrisUtils/GarbageGenius.py
--rw-r--r--   0 htd        (502) staff       (20)     3351 2024-05-08 03:17:50.000000 NorrisUtils-1.4.6/NorrisUtils/ImageUploadUtils.py
--rw-r--r--   0 htd        (502) staff       (20)    10121 2022-12-21 09:04:02.000000 NorrisUtils-1.4.6/NorrisUtils/RawUtil.py
--rw-r--r--   0 htd        (502) staff       (20)     2755 2022-12-21 09:04:02.000000 NorrisUtils-1.4.6/NorrisUtils/RawUtils.py
--rw-r--r--   0 htd        (502) staff       (20)     8470 2022-12-21 09:04:02.000000 NorrisUtils-1.4.6/NorrisUtils/RequestUtils.py
--rw-r--r--   0 htd        (502) staff       (20)       20 2022-12-21 09:04:02.000000 NorrisUtils-1.4.6/NorrisUtils/__init__.py
-drwxr-xr-x   0 htd        (502) staff       (20)        0 2024-05-08 06:26:04.601548 NorrisUtils-1.4.6/NorrisUtils.egg-info/
--rw-r--r--   0 htd        (502) staff       (20)     1026 2024-05-08 06:26:04.000000 NorrisUtils-1.4.6/NorrisUtils.egg-info/PKG-INFO
--rw-r--r--   0 htd        (502) staff       (20)      433 2024-05-08 06:26:04.000000 NorrisUtils-1.4.6/NorrisUtils.egg-info/SOURCES.txt
--rw-r--r--   0 htd        (502) staff       (20)        1 2024-05-08 06:26:04.000000 NorrisUtils-1.4.6/NorrisUtils.egg-info/dependency_links.txt
--rw-r--r--   0 htd        (502) staff       (20)       17 2024-05-08 06:26:04.000000 NorrisUtils-1.4.6/NorrisUtils.egg-info/requires.txt
--rw-r--r--   0 htd        (502) staff       (20)       12 2024-05-08 06:26:04.000000 NorrisUtils-1.4.6/NorrisUtils.egg-info/top_level.txt
--rw-r--r--   0 htd        (502) staff       (20)     1026 2024-05-08 06:26:04.601956 NorrisUtils-1.4.6/PKG-INFO
--rw-r--r--   0 htd        (502) staff       (20)       60 2022-12-21 09:04:02.000000 NorrisUtils-1.4.6/README.md
--rw-r--r--   0 htd        (502) staff       (20)       38 2024-05-08 06:26:04.602710 NorrisUtils-1.4.6/setup.cfg
--rw-r--r--   0 htd        (502) staff       (20)     1256 2024-05-08 06:26:01.000000 NorrisUtils-1.4.6/setup.py
+drwxr-xr-x   0 htd        (502) staff       (20)        0 2024-05-17 06:08:15.013078 NorrisUtils-1.5.0/
+drwxr-xr-x   0 htd        (502) staff       (20)        0 2024-05-17 06:08:15.009685 NorrisUtils-1.5.0/NorrisUtils/
+-rw-r--r--   0 htd        (502) staff       (20)       42 2022-12-21 09:04:02.000000 NorrisUtils-1.5.0/NorrisUtils/BuildConfig.py
+-rw-r--r--   0 htd        (502) staff       (20)     2140 2024-05-17 04:02:47.000000 NorrisUtils-1.5.0/NorrisUtils/ConfigLoader.py
+-rw-r--r--   0 htd        (502) staff       (20)    12658 2024-05-17 05:37:51.000000 NorrisUtils-1.5.0/NorrisUtils/DingTalkGenius.py
+-rw-r--r--   0 htd        (502) staff       (20)     5581 2023-10-17 09:11:02.000000 NorrisUtils-1.5.0/NorrisUtils/FileUtil.py
+-rw-r--r--   0 htd        (502) staff       (20)     1392 2022-12-21 09:04:02.000000 NorrisUtils-1.5.0/NorrisUtils/GarbageGenius.py
+-rw-r--r--   0 htd        (502) staff       (20)     3351 2024-05-08 03:17:50.000000 NorrisUtils-1.5.0/NorrisUtils/ImageUploadUtils.py
+-rw-r--r--   0 htd        (502) staff       (20)    10121 2022-12-21 09:04:02.000000 NorrisUtils-1.5.0/NorrisUtils/RawUtil.py
+-rw-r--r--   0 htd        (502) staff       (20)     2755 2022-12-21 09:04:02.000000 NorrisUtils-1.5.0/NorrisUtils/RawUtils.py
+-rw-r--r--   0 htd        (502) staff       (20)     8470 2022-12-21 09:04:02.000000 NorrisUtils-1.5.0/NorrisUtils/RequestUtils.py
+-rw-r--r--   0 htd        (502) staff       (20)       20 2022-12-21 09:04:02.000000 NorrisUtils-1.5.0/NorrisUtils/__init__.py
+drwxr-xr-x   0 htd        (502) staff       (20)        0 2024-05-17 06:08:15.012326 NorrisUtils-1.5.0/NorrisUtils.egg-info/
+-rw-r--r--   0 htd        (502) staff       (20)      965 2024-05-17 06:08:14.000000 NorrisUtils-1.5.0/NorrisUtils.egg-info/PKG-INFO
+-rw-r--r--   0 htd        (502) staff       (20)      461 2024-05-17 06:08:14.000000 NorrisUtils-1.5.0/NorrisUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 htd        (502) staff       (20)        1 2024-05-17 06:08:14.000000 NorrisUtils-1.5.0/NorrisUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 htd        (502) staff       (20)       17 2024-05-17 06:08:14.000000 NorrisUtils-1.5.0/NorrisUtils.egg-info/requires.txt
+-rw-r--r--   0 htd        (502) staff       (20)       12 2024-05-17 06:08:14.000000 NorrisUtils-1.5.0/NorrisUtils.egg-info/top_level.txt
+-rw-r--r--   0 htd        (502) staff       (20)      965 2024-05-17 06:08:15.012722 NorrisUtils-1.5.0/PKG-INFO
+-rw-r--r--   0 htd        (502) staff       (20)       60 2022-12-21 09:04:02.000000 NorrisUtils-1.5.0/README.md
+-rw-r--r--   0 htd        (502) staff       (20)       38 2024-05-17 06:08:15.013164 NorrisUtils-1.5.0/setup.cfg
+-rw-r--r--   0 htd        (502) staff       (20)     1195 2024-05-17 06:03:48.000000 NorrisUtils-1.5.0/setup.py
```

### Comparing `NorrisUtils-1.4.6/NorrisUtils/DingTalkGenius.py` & `NorrisUtils-1.5.0/NorrisUtils/DingTalkGenius.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.4.6/NorrisUtils/FileUtil.py` & `NorrisUtils-1.5.0/NorrisUtils/FileUtil.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.4.6/NorrisUtils/GarbageGenius.py` & `NorrisUtils-1.5.0/NorrisUtils/GarbageGenius.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.4.6/NorrisUtils/ImageUploadUtils.py` & `NorrisUtils-1.5.0/NorrisUtils/ImageUploadUtils.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.4.6/NorrisUtils/RawUtil.py` & `NorrisUtils-1.5.0/NorrisUtils/RawUtil.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.4.6/NorrisUtils/RawUtils.py` & `NorrisUtils-1.5.0/NorrisUtils/RawUtils.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.4.6/NorrisUtils/RequestUtils.py` & `NorrisUtils-1.5.0/NorrisUtils/RequestUtils.py`

 * *Files identical despite different names*

### Comparing `NorrisUtils-1.4.6/NorrisUtils.egg-info/PKG-INFO` & `NorrisUtils-1.5.0/NorrisUtils.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: NorrisUtils
-Version: 1.4.6
-Summary: 图床工具包，支持上传到sm.ms图床，支持发送钉钉消息
+Version: 1.5.0
+Summary: ini.loader
 Home-page: https://www.baidu.com
 Author: AlaricNorris
 Author-email: norris.sly@gmail.com
 Maintainer: AlaricNorris
 Maintainer-email: norris.sly@gmail.com
 License: BSD License
 Platform: all
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `NorrisUtils-1.4.6/PKG-INFO` & `NorrisUtils-1.5.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: NorrisUtils
-Version: 1.4.6
-Summary: 图床工具包，支持上传到sm.ms图床，支持发送钉钉消息
+Version: 1.5.0
+Summary: ini.loader
 Home-page: https://www.baidu.com
 Author: AlaricNorris
 Author-email: norris.sly@gmail.com
 Maintainer: AlaricNorris
 Maintainer-email: norris.sly@gmail.com
 License: BSD License
 Platform: all
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

