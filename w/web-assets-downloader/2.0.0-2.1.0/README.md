# Comparing `tmp/web_assets_downloader-2.0.0.tar.gz` & `tmp/web_assets_downloader-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_assets_downloader-2.0.0.tar", last modified: Sat Apr 13 16:17:16 2024, max compression
+gzip compressed data, was "web_assets_downloader-2.1.0.tar", last modified: Fri May 17 09:34:09 2024, max compression
```

## Comparing `web_assets_downloader-2.0.0.tar` & `web_assets_downloader-2.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2024-04-13 16:17:16.356332 web_assets_downloader-2.0.0/
--rw-rw-r--   0 arif      (1000) arif      (1000)      957 2024-04-13 16:17:16.356332 web_assets_downloader-2.0.0/PKG-INFO
--rw-rw-r--   0 arif      (1000) arif      (1000)       38 2024-04-13 16:17:16.356332 web_assets_downloader-2.0.0/setup.cfg
--rw-rw-r--   0 arif      (1000) arif      (1000)     1543 2024-04-13 16:17:11.000000 web_assets_downloader-2.0.0/setup.py
-drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2024-04-13 16:17:16.356332 web_assets_downloader-2.0.0/web_assets_downloader/
--rw-rw-r--   0 arif      (1000) arif      (1000)      141 2024-03-03 10:53:55.000000 web_assets_downloader-2.0.0/web_assets_downloader/__init__.py
--rw-rw-r--   0 arif      (1000) arif      (1000)     2663 2024-03-03 10:42:41.000000 web_assets_downloader-2.0.0/web_assets_downloader/web_assets_downloader.py
-drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2024-04-13 16:17:16.356332 web_assets_downloader-2.0.0/web_assets_downloader.egg-info/
--rw-rw-r--   0 arif      (1000) arif      (1000)      957 2024-04-13 16:17:16.000000 web_assets_downloader-2.0.0/web_assets_downloader.egg-info/PKG-INFO
--rw-rw-r--   0 arif      (1000) arif      (1000)      361 2024-04-13 16:17:16.000000 web_assets_downloader-2.0.0/web_assets_downloader.egg-info/SOURCES.txt
--rw-rw-r--   0 arif      (1000) arif      (1000)       88 2024-04-13 16:17:16.000000 web_assets_downloader-2.0.0/web_assets_downloader.egg-info/dependency_links.txt
--rw-rw-r--   0 arif      (1000) arif      (1000)       81 2024-04-13 16:17:16.000000 web_assets_downloader-2.0.0/web_assets_downloader.egg-info/entry_points.txt
--rw-rw-r--   0 arif      (1000) arif      (1000)       59 2024-04-13 16:17:16.000000 web_assets_downloader-2.0.0/web_assets_downloader.egg-info/requires.txt
--rw-rw-r--   0 arif      (1000) arif      (1000)       22 2024-04-13 16:17:16.000000 web_assets_downloader-2.0.0/web_assets_downloader.egg-info/top_level.txt
+drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2024-05-17 09:34:09.832431 web_assets_downloader-2.1.0/
+-rw-rw-r--   0 arif      (1000) arif      (1000)      957 2024-05-17 09:34:09.832431 web_assets_downloader-2.1.0/PKG-INFO
+-rw-rw-r--   0 arif      (1000) arif      (1000)       38 2024-05-17 09:34:09.832431 web_assets_downloader-2.1.0/setup.cfg
+-rw-rw-r--   0 arif      (1000) arif      (1000)     1543 2024-05-17 09:30:22.000000 web_assets_downloader-2.1.0/setup.py
+drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2024-05-17 09:34:09.832431 web_assets_downloader-2.1.0/web_assets_downloader/
+-rw-rw-r--   0 arif      (1000) arif      (1000)      141 2024-03-03 10:53:55.000000 web_assets_downloader-2.1.0/web_assets_downloader/__init__.py
+-rw-rw-r--   0 arif      (1000) arif      (1000)     4757 2024-05-17 09:29:02.000000 web_assets_downloader-2.1.0/web_assets_downloader/web_assets_downloader.py
+drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2024-05-17 09:34:09.832431 web_assets_downloader-2.1.0/web_assets_downloader.egg-info/
+-rw-rw-r--   0 arif      (1000) arif      (1000)      957 2024-05-17 09:34:09.000000 web_assets_downloader-2.1.0/web_assets_downloader.egg-info/PKG-INFO
+-rw-rw-r--   0 arif      (1000) arif      (1000)      361 2024-05-17 09:34:09.000000 web_assets_downloader-2.1.0/web_assets_downloader.egg-info/SOURCES.txt
+-rw-rw-r--   0 arif      (1000) arif      (1000)       88 2024-05-17 09:34:09.000000 web_assets_downloader-2.1.0/web_assets_downloader.egg-info/dependency_links.txt
+-rw-rw-r--   0 arif      (1000) arif      (1000)       81 2024-05-17 09:34:09.000000 web_assets_downloader-2.1.0/web_assets_downloader.egg-info/entry_points.txt
+-rw-rw-r--   0 arif      (1000) arif      (1000)       59 2024-05-17 09:34:09.000000 web_assets_downloader-2.1.0/web_assets_downloader.egg-info/requires.txt
+-rw-rw-r--   0 arif      (1000) arif      (1000)       22 2024-05-17 09:34:09.000000 web_assets_downloader-2.1.0/web_assets_downloader.egg-info/top_level.txt
```

### Comparing `web_assets_downloader-2.0.0/PKG-INFO` & `web_assets_downloader-2.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web_assets_downloader
-Version: 2.0.0
+Version: 2.1.0
 Summary: A package for downloading web content and assets
 Home-page: https://github.com/arif-x/web-assets-downloader
 Author: Ariffudin
 Author-email: sudo.ariffudin@email.com
 License: MIT
 Project-URL: Source, https://github.com/arif-x/web-assets-downloader
 Project-URL: Source Code, https://github.com/arif-x/web-assets-downloader
```

### Comparing `web_assets_downloader-2.0.0/setup.py` & `web_assets_downloader-2.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='web_assets_downloader',
-    version='2.0.0',
+    version='2.1.0',
     packages=find_packages(),
     install_requires=[
         'requests',
         'beautifulsoup4',
         'pillow',
         'PyPDF2',
         'python-docx',
```

### Comparing `web_assets_downloader-2.0.0/web_assets_downloader.egg-info/PKG-INFO` & `web_assets_downloader-2.1.0/web_assets_downloader.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-assets-downloader
-Version: 2.0.0
+Version: 2.1.0
 Summary: A package for downloading web content and assets
 Home-page: https://github.com/arif-x/web-assets-downloader
 Author: Ariffudin
 Author-email: sudo.ariffudin@email.com
 License: MIT
 Project-URL: Source, https://github.com/arif-x/web-assets-downloader
 Project-URL: Source Code, https://github.com/arif-x/web-assets-downloader
```

