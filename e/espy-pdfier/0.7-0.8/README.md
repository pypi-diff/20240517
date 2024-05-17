# Comparing `tmp/espy_pdfier-0.7.tar.gz` & `tmp/espy_pdfier-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espy_pdfier-0.7.tar", last modified: Tue May 14 20:34:47 2024, max compression
+gzip compressed data, was "espy_pdfier-0.8.tar", last modified: Fri May 17 20:52:23 2024, max compression
```

## Comparing `espy_pdfier-0.7.tar` & `espy_pdfier-0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-14 20:34:47.786586 espy_pdfier-0.7/
--rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-05-05 23:47:48.000000 espy_pdfier-0.7/LICENSE
--rw-r--r--   0 philipadigun   (501) staff       (20)      387 2024-05-14 20:34:47.786333 espy_pdfier-0.7/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      120 2024-05-06 00:37:08.000000 espy_pdfier-0.7/README.md
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-14 20:34:47.784001 espy_pdfier-0.7/espy_pdfier/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-06 00:00:35.000000 espy_pdfier-0.7/espy_pdfier/__init__.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-14 20:34:47.785230 espy_pdfier-0.7/espy_pdfier/service/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-05 23:40:00.000000 espy_pdfier-0.7/espy_pdfier/service/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     2497 2024-05-14 20:32:38.000000 espy_pdfier-0.7/espy_pdfier/service/img_serv.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     2855 2024-05-06 00:31:42.000000 espy_pdfier-0.7/espy_pdfier/service/service.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-14 20:34:47.785909 espy_pdfier-0.7/espy_pdfier/util/
--rw-r--r--   0 philipadigun   (501) staff       (20)     1083 2024-05-12 17:18:43.000000 espy_pdfier-0.7/espy_pdfier/util/CONSTANTS.py
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-11 23:21:45.000000 espy_pdfier-0.7/espy_pdfier/util/__init__.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-14 20:34:47.786076 espy_pdfier-0.7/espy_pdfier.egg-info/
--rw-r--r--   0 philipadigun   (501) staff       (20)      387 2024-05-14 20:34:47.000000 espy_pdfier-0.7/espy_pdfier.egg-info/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      378 2024-05-14 20:34:47.000000 espy_pdfier-0.7/espy_pdfier.egg-info/SOURCES.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-05-14 20:34:47.000000 espy_pdfier-0.7/espy_pdfier.egg-info/dependency_links.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       48 2024-05-14 20:34:47.000000 espy_pdfier-0.7/espy_pdfier.egg-info/requires.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       12 2024-05-14 20:34:47.000000 espy_pdfier-0.7/espy_pdfier.egg-info/top_level.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-05-14 20:34:47.786637 espy_pdfier-0.7/setup.cfg
--rw-r--r--   0 philipadigun   (501) staff       (20)      607 2024-05-14 20:33:02.000000 espy_pdfier-0.7/setup.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-17 20:52:23.272243 espy_pdfier-0.8/
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-05-05 23:47:48.000000 espy_pdfier-0.8/LICENSE
+-rw-r--r--   0 philipadigun   (501) staff       (20)      387 2024-05-17 20:52:23.272005 espy_pdfier-0.8/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      120 2024-05-06 00:37:08.000000 espy_pdfier-0.8/README.md
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-17 20:52:23.269681 espy_pdfier-0.8/espy_pdfier/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-06 00:00:35.000000 espy_pdfier-0.8/espy_pdfier/__init__.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-17 20:52:23.271062 espy_pdfier-0.8/espy_pdfier/service/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-05 23:40:00.000000 espy_pdfier-0.8/espy_pdfier/service/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2504 2024-05-17 20:46:22.000000 espy_pdfier-0.8/espy_pdfier/service/img_serv.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2855 2024-05-06 00:31:42.000000 espy_pdfier-0.8/espy_pdfier/service/service.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-17 20:52:23.271575 espy_pdfier-0.8/espy_pdfier/util/
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1083 2024-05-12 17:18:43.000000 espy_pdfier-0.8/espy_pdfier/util/CONSTANTS.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-11 23:21:45.000000 espy_pdfier-0.8/espy_pdfier/util/__init__.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-17 20:52:23.271751 espy_pdfier-0.8/espy_pdfier.egg-info/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      387 2024-05-17 20:52:23.000000 espy_pdfier-0.8/espy_pdfier.egg-info/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      378 2024-05-17 20:52:23.000000 espy_pdfier-0.8/espy_pdfier.egg-info/SOURCES.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-05-17 20:52:23.000000 espy_pdfier-0.8/espy_pdfier.egg-info/dependency_links.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       48 2024-05-17 20:52:23.000000 espy_pdfier-0.8/espy_pdfier.egg-info/requires.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       12 2024-05-17 20:52:23.000000 espy_pdfier-0.8/espy_pdfier.egg-info/top_level.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-05-17 20:52:23.272292 espy_pdfier-0.8/setup.cfg
+-rw-r--r--   0 philipadigun   (501) staff       (20)      607 2024-05-17 20:52:19.000000 espy_pdfier-0.8/setup.py
```

### Comparing `espy_pdfier-0.7/LICENSE` & `espy_pdfier-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `espy_pdfier-0.7/espy_pdfier/service/img_serv.py` & `espy_pdfier-0.8/espy_pdfier/service/img_serv.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import io
 
 def is_greater_than_allowed_size(image_path):
     return os.path.getsize(image_path) > CONSTANTS.IMAGE_SIZE_MB * 1024 * 1024
 
 def is_image_size_valid(file):
-    max_size_mb = CONSTANTS.IMAGE_SIZE_MB * 1024 * 1024
+    max_size_mb = float(CONSTANTS.IMAGE_SIZE_MB) * 1024 * 1024
     file_size_mb = file.file.seek(0, 2) / (1024 * 1024)  # Get file size in MB
     file.file.seek(0)  # Reset file pointer to the beginning
     return file_size_mb <= max_size_mb
     
 def resize_image(image, size):
     resized_image = image.copy()
     resized_image.thumbnail(size)
```

### Comparing `espy_pdfier-0.7/espy_pdfier/service/service.py` & `espy_pdfier-0.8/espy_pdfier/service/service.py`

 * *Files identical despite different names*

### Comparing `espy_pdfier-0.7/espy_pdfier/util/CONSTANTS.py` & `espy_pdfier-0.8/espy_pdfier/util/CONSTANTS.py`

 * *Files identical despite different names*

### Comparing `espy_pdfier-0.7/setup.py` & `espy_pdfier-0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 VERSION = '0.0.3'
 DESCRIPTION = 'ESSL assets management'
 LONG_DESCRIPTION = 'Internal helper package for ESSL assets management'
 setup(
     name='espy_pdfier',
-    version='0.7',
+    version='0.8',
     packages=find_packages(),
     install_requires=[
         'reportlab==4.2.0',
         'pillow==10.3.0',
         'boto3==1.34.103',
         ],
     author='Femi Adigun',
```

