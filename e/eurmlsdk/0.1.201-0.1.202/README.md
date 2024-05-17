# Comparing `tmp/eurmlsdk-0.1.201.tar.gz` & `tmp/eurmlsdk-0.1.202.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurmlsdk-0.1.201.tar", last modified: Fri May 17 11:59:44 2024, max compression
+gzip compressed data, was "eurmlsdk-0.1.202.tar", last modified: Fri May 17 12:24:55 2024, max compression
```

## Comparing `eurmlsdk-0.1.201.tar` & `eurmlsdk-0.1.202.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-17 11:59:44.822554 eurmlsdk-0.1.201/
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       16 2024-05-07 10:55:35.000000 eurmlsdk-0.1.201/LICENSE.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       38 2024-05-07 10:55:35.000000 eurmlsdk-0.1.201/MANIFEST.in
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      384 2024-05-17 11:59:44.822554 eurmlsdk-0.1.201/PKG-INFO
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       10 2024-05-07 10:55:35.000000 eurmlsdk-0.1.201/README.md
-drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-17 11:59:44.812554 eurmlsdk-0.1.201/eurmlsdk/
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       33 2024-05-15 11:40:23.000000 eurmlsdk-0.1.201/eurmlsdk/__init__.py
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)     6150 2024-05-16 10:16:43.000000 eurmlsdk-0.1.201/eurmlsdk/__main__.py
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)     9571 2024-05-17 11:59:06.000000 eurmlsdk-0.1.201/eurmlsdk/eur_sdk.py
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)     4036 2024-05-16 09:13:37.000000 eurmlsdk-0.1.201/eurmlsdk/pytorch.py
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)     1233 2024-05-17 11:59:03.000000 eurmlsdk-0.1.201/eurmlsdk/yolo.py
-drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-17 11:59:44.822554 eurmlsdk-0.1.201/eurmlsdk.egg-info/
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      384 2024-05-17 11:59:44.000000 eurmlsdk-0.1.201/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      335 2024-05-17 11:59:44.000000 eurmlsdk-0.1.201/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)        1 2024-05-17 11:59:44.000000 eurmlsdk-0.1.201/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       53 2024-05-17 11:59:44.000000 eurmlsdk-0.1.201/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      130 2024-05-17 11:59:44.000000 eurmlsdk-0.1.201/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)        9 2024-05-17 11:59:44.000000 eurmlsdk-0.1.201/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       38 2024-05-17 11:59:44.822554 eurmlsdk-0.1.201/setup.cfg
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      897 2024-05-17 11:59:36.000000 eurmlsdk-0.1.201/setup.py
+drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-17 12:24:55.282554 eurmlsdk-0.1.202/
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       16 2024-05-07 10:55:35.000000 eurmlsdk-0.1.202/LICENSE.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       38 2024-05-07 10:55:35.000000 eurmlsdk-0.1.202/MANIFEST.in
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      384 2024-05-17 12:24:55.282554 eurmlsdk-0.1.202/PKG-INFO
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       10 2024-05-07 10:55:35.000000 eurmlsdk-0.1.202/README.md
+drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-17 12:24:55.282554 eurmlsdk-0.1.202/eurmlsdk/
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       33 2024-05-15 11:40:23.000000 eurmlsdk-0.1.202/eurmlsdk/__init__.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)     6150 2024-05-16 10:16:43.000000 eurmlsdk-0.1.202/eurmlsdk/__main__.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)     9571 2024-05-17 11:59:06.000000 eurmlsdk-0.1.202/eurmlsdk/eur_sdk.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)     4036 2024-05-16 09:13:37.000000 eurmlsdk-0.1.202/eurmlsdk/pytorch.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)     1222 2024-05-17 12:24:36.000000 eurmlsdk-0.1.202/eurmlsdk/yolo.py
+drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-17 12:24:55.282554 eurmlsdk-0.1.202/eurmlsdk.egg-info/
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      384 2024-05-17 12:24:55.000000 eurmlsdk-0.1.202/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      335 2024-05-17 12:24:55.000000 eurmlsdk-0.1.202/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)        1 2024-05-17 12:24:55.000000 eurmlsdk-0.1.202/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       53 2024-05-17 12:24:55.000000 eurmlsdk-0.1.202/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      130 2024-05-17 12:24:55.000000 eurmlsdk-0.1.202/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)        9 2024-05-17 12:24:55.000000 eurmlsdk-0.1.202/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       38 2024-05-17 12:24:55.282554 eurmlsdk-0.1.202/setup.cfg
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      897 2024-05-17 12:22:41.000000 eurmlsdk-0.1.202/setup.py
```

### Comparing `eurmlsdk-0.1.201/eurmlsdk/__main__.py` & `eurmlsdk-0.1.202/eurmlsdk/__main__.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.1.201/eurmlsdk/eur_sdk.py` & `eurmlsdk-0.1.202/eurmlsdk/eur_sdk.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.1.201/eurmlsdk/pytorch.py` & `eurmlsdk-0.1.202/eurmlsdk/pytorch.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.1.201/eurmlsdk/yolo.py` & `eurmlsdk-0.1.202/eurmlsdk/yolo.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         else:
             raise ModelNotFound()
         
     def predict_model(self, pathArg, dataSet):
         try:
             model = self.load_model(pathArg)
             print("Prediction started.....")
-            model(dataSet, save=True, show=True, stream=True)
+            model(dataSet, show=True, stream=True)
         except ModelNotFound as err:
             print("Error :", err)
             exit(1)
         except Exception as err:
             print("Error in Prediction :", err)
             exit(1)
```

### Comparing `eurmlsdk-0.1.201/setup.py` & `eurmlsdk-0.1.202/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.1.201',
+    version='0.1.202',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'numpy==1.24.3',
         'python-dotenv',
```

