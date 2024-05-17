# Comparing `tmp/eurmlsdk-0.1.1.tar.gz` & `tmp/eurmlsdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurmlsdk-0.1.1.tar", last modified: Fri May 17 11:41:16 2024, max compression
+gzip compressed data, was "eurmlsdk-0.1.2.tar", last modified: Fri May 17 11:43:51 2024, max compression
```

## Comparing `eurmlsdk-0.1.1.tar` & `eurmlsdk-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-17 11:41:16.557587 eurmlsdk-0.1.1/
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       16 2024-05-07 10:55:35.000000 eurmlsdk-0.1.1/LICENSE.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       38 2024-05-07 10:55:35.000000 eurmlsdk-0.1.1/MANIFEST.in
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      382 2024-05-17 11:41:16.557587 eurmlsdk-0.1.1/PKG-INFO
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       10 2024-05-07 10:55:35.000000 eurmlsdk-0.1.1/README.md
-drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-17 11:41:16.547587 eurmlsdk-0.1.1/eurmlsdk/
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       33 2024-05-15 11:40:23.000000 eurmlsdk-0.1.1/eurmlsdk/__init__.py
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)     6150 2024-05-16 10:16:43.000000 eurmlsdk-0.1.1/eurmlsdk/__main__.py
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)     9540 2024-05-17 11:35:26.000000 eurmlsdk-0.1.1/eurmlsdk/eur_sdk.py
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)     4036 2024-05-16 09:13:37.000000 eurmlsdk-0.1.1/eurmlsdk/pytorch.py
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)     1241 2024-05-17 11:32:25.000000 eurmlsdk-0.1.1/eurmlsdk/yolo.py
-drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-17 11:41:16.557587 eurmlsdk-0.1.1/eurmlsdk.egg-info/
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      382 2024-05-17 11:41:16.000000 eurmlsdk-0.1.1/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      335 2024-05-17 11:41:16.000000 eurmlsdk-0.1.1/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)        1 2024-05-17 11:41:16.000000 eurmlsdk-0.1.1/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       53 2024-05-17 11:41:16.000000 eurmlsdk-0.1.1/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      129 2024-05-17 11:41:16.000000 eurmlsdk-0.1.1/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)        9 2024-05-17 11:41:16.000000 eurmlsdk-0.1.1/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       38 2024-05-17 11:41:16.557587 eurmlsdk-0.1.1/setup.cfg
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      894 2024-05-17 11:41:06.000000 eurmlsdk-0.1.1/setup.py
+drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-17 11:43:51.097589 eurmlsdk-0.1.2/
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       16 2024-05-07 10:55:35.000000 eurmlsdk-0.1.2/LICENSE.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       38 2024-05-07 10:55:35.000000 eurmlsdk-0.1.2/MANIFEST.in
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      382 2024-05-17 11:43:51.097589 eurmlsdk-0.1.2/PKG-INFO
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       10 2024-05-07 10:55:35.000000 eurmlsdk-0.1.2/README.md
+drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-17 11:43:51.087589 eurmlsdk-0.1.2/eurmlsdk/
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       33 2024-05-15 11:40:23.000000 eurmlsdk-0.1.2/eurmlsdk/__init__.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)     6150 2024-05-16 10:16:43.000000 eurmlsdk-0.1.2/eurmlsdk/__main__.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)     9540 2024-05-17 11:35:26.000000 eurmlsdk-0.1.2/eurmlsdk/eur_sdk.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)     4036 2024-05-16 09:13:37.000000 eurmlsdk-0.1.2/eurmlsdk/pytorch.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)     1241 2024-05-17 11:32:25.000000 eurmlsdk-0.1.2/eurmlsdk/yolo.py
+drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-17 11:43:51.087589 eurmlsdk-0.1.2/eurmlsdk.egg-info/
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      382 2024-05-17 11:43:50.000000 eurmlsdk-0.1.2/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      335 2024-05-17 11:43:50.000000 eurmlsdk-0.1.2/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)        1 2024-05-17 11:43:50.000000 eurmlsdk-0.1.2/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       53 2024-05-17 11:43:50.000000 eurmlsdk-0.1.2/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      130 2024-05-17 11:43:50.000000 eurmlsdk-0.1.2/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)        9 2024-05-17 11:43:50.000000 eurmlsdk-0.1.2/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       38 2024-05-17 11:43:51.097589 eurmlsdk-0.1.2/setup.cfg
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      895 2024-05-17 11:43:12.000000 eurmlsdk-0.1.2/setup.py
```

### Comparing `eurmlsdk-0.1.1/eurmlsdk/__main__.py` & `eurmlsdk-0.1.2/eurmlsdk/__main__.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.1.1/eurmlsdk/eur_sdk.py` & `eurmlsdk-0.1.2/eurmlsdk/eur_sdk.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.1.1/eurmlsdk/pytorch.py` & `eurmlsdk-0.1.2/eurmlsdk/pytorch.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.1.1/eurmlsdk/yolo.py` & `eurmlsdk-0.1.2/eurmlsdk/yolo.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.1.1/setup.py` & `eurmlsdk-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'numpy==1.24.3',
         'python-dotenv',
         'paramiko',
         'tensorflow==2.13.1',
         'tqdm',
         'ultralytics',
         'torch',
         'timm',
-        'torchvision'
+        'torchvision',
         'menpo',
         'opencv-contrib-python'    
 ],
     author='eUR',
     author_email='aiml@embedur.com',
     license='MIT',
     entry_points={
```

