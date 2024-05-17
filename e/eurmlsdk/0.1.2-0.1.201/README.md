# Comparing `tmp/eurmlsdk-0.1.2.tar.gz` & `tmp/eurmlsdk-0.1.201.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurmlsdk-0.1.2.tar", last modified: Fri May 17 11:43:51 2024, max compression
+gzip compressed data, was "eurmlsdk-0.1.201.tar", last modified: Fri May 17 11:59:44 2024, max compression
```

## Comparing `eurmlsdk-0.1.2.tar` & `eurmlsdk-0.1.201.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-17 11:43:51.097589 eurmlsdk-0.1.2/
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       16 2024-05-07 10:55:35.000000 eurmlsdk-0.1.2/LICENSE.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       38 2024-05-07 10:55:35.000000 eurmlsdk-0.1.2/MANIFEST.in
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      382 2024-05-17 11:43:51.097589 eurmlsdk-0.1.2/PKG-INFO
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       10 2024-05-07 10:55:35.000000 eurmlsdk-0.1.2/README.md
-drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-17 11:43:51.087589 eurmlsdk-0.1.2/eurmlsdk/
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       33 2024-05-15 11:40:23.000000 eurmlsdk-0.1.2/eurmlsdk/__init__.py
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)     6150 2024-05-16 10:16:43.000000 eurmlsdk-0.1.2/eurmlsdk/__main__.py
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)     9540 2024-05-17 11:35:26.000000 eurmlsdk-0.1.2/eurmlsdk/eur_sdk.py
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)     4036 2024-05-16 09:13:37.000000 eurmlsdk-0.1.2/eurmlsdk/pytorch.py
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)     1241 2024-05-17 11:32:25.000000 eurmlsdk-0.1.2/eurmlsdk/yolo.py
-drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-17 11:43:51.087589 eurmlsdk-0.1.2/eurmlsdk.egg-info/
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      382 2024-05-17 11:43:50.000000 eurmlsdk-0.1.2/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      335 2024-05-17 11:43:50.000000 eurmlsdk-0.1.2/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)        1 2024-05-17 11:43:50.000000 eurmlsdk-0.1.2/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       53 2024-05-17 11:43:50.000000 eurmlsdk-0.1.2/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      130 2024-05-17 11:43:50.000000 eurmlsdk-0.1.2/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)        9 2024-05-17 11:43:50.000000 eurmlsdk-0.1.2/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       38 2024-05-17 11:43:51.097589 eurmlsdk-0.1.2/setup.cfg
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      895 2024-05-17 11:43:12.000000 eurmlsdk-0.1.2/setup.py
+drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-17 11:59:44.822554 eurmlsdk-0.1.201/
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       16 2024-05-07 10:55:35.000000 eurmlsdk-0.1.201/LICENSE.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       38 2024-05-07 10:55:35.000000 eurmlsdk-0.1.201/MANIFEST.in
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      384 2024-05-17 11:59:44.822554 eurmlsdk-0.1.201/PKG-INFO
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       10 2024-05-07 10:55:35.000000 eurmlsdk-0.1.201/README.md
+drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-17 11:59:44.812554 eurmlsdk-0.1.201/eurmlsdk/
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       33 2024-05-15 11:40:23.000000 eurmlsdk-0.1.201/eurmlsdk/__init__.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)     6150 2024-05-16 10:16:43.000000 eurmlsdk-0.1.201/eurmlsdk/__main__.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)     9571 2024-05-17 11:59:06.000000 eurmlsdk-0.1.201/eurmlsdk/eur_sdk.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)     4036 2024-05-16 09:13:37.000000 eurmlsdk-0.1.201/eurmlsdk/pytorch.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)     1233 2024-05-17 11:59:03.000000 eurmlsdk-0.1.201/eurmlsdk/yolo.py
+drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-17 11:59:44.822554 eurmlsdk-0.1.201/eurmlsdk.egg-info/
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      384 2024-05-17 11:59:44.000000 eurmlsdk-0.1.201/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      335 2024-05-17 11:59:44.000000 eurmlsdk-0.1.201/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)        1 2024-05-17 11:59:44.000000 eurmlsdk-0.1.201/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       53 2024-05-17 11:59:44.000000 eurmlsdk-0.1.201/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      130 2024-05-17 11:59:44.000000 eurmlsdk-0.1.201/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)        9 2024-05-17 11:59:44.000000 eurmlsdk-0.1.201/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       38 2024-05-17 11:59:44.822554 eurmlsdk-0.1.201/setup.cfg
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      897 2024-05-17 11:59:36.000000 eurmlsdk-0.1.201/setup.py
```

### Comparing `eurmlsdk-0.1.2/eurmlsdk/__main__.py` & `eurmlsdk-0.1.201/eurmlsdk/__main__.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.1.2/eurmlsdk/eur_sdk.py` & `eurmlsdk-0.1.201/eurmlsdk/eur_sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,19 +89,24 @@
                 print("Error checking the prediction results: ", err)
                 return
         except Exception as err:
             print("Error downloading file: ", err)
             ssh_client.close()
             exit(1)
 
+
+
+            
+
     def upload_to_remote(self, ssh_client, local_path, remote_path):
         print("Uploading file {} to {}".format(local_path, remote_path))
         sftp_progress_bar = SFTPWithProgressBar.from_transport(ssh_client.get_transport())
         sftp_progress_bar.put(local_path, remote_path)
-        print("File upload successful")
+        print("File upload successful"
+              )
 
     def upload_file(self, ssh_client, local_path, remote_path, home_path):
         try:
             sftp = ssh_client.open_sftp()
             # print("Checking for file in {}".format(home_path))
             sftp.stat(remote_path)
             print("File already exists")
```

### Comparing `eurmlsdk-0.1.2/eurmlsdk/pytorch.py` & `eurmlsdk-0.1.201/eurmlsdk/pytorch.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.1.2/eurmlsdk/yolo.py` & `eurmlsdk-0.1.201/eurmlsdk/yolo.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         else:
             raise ModelNotFound()
         
     def predict_model(self, pathArg, dataSet):
         try:
             model = self.load_model(pathArg)
             print("Prediction started.....")
-            model.predict(dataSet, save=True, show=True, stream=True)
+            model(dataSet, save=True, show=True, stream=True)
         except ModelNotFound as err:
             print("Error :", err)
             exit(1)
         except Exception as err:
             print("Error in Prediction :", err)
             exit(1)
```

### Comparing `eurmlsdk-0.1.2/setup.py` & `eurmlsdk-0.1.201/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.1.2',
+    version='0.1.201',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'numpy==1.24.3',
         'python-dotenv',
```

