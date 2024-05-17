# Comparing `tmp/eurmlsdk-0.1.0.tar.gz` & `tmp/eurmlsdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurmlsdk-0.1.0.tar", last modified: Thu May 16 10:48:52 2024, max compression
+gzip compressed data, was "eurmlsdk-0.1.1.tar", last modified: Fri May 17 11:41:16 2024, max compression
```

## Comparing `eurmlsdk-0.1.0.tar` & `eurmlsdk-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 10:48:52.603050 eurmlsdk-0.1.0/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.1.0/LICENSE.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.1.0/MANIFEST.in
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      382 2024-05-16 10:48:52.603050 eurmlsdk-0.1.0/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.1.0/README.md
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 10:48:52.593050 eurmlsdk-0.1.0/eurmlsdk/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       33 2024-05-14 11:25:38.000000 eurmlsdk-0.1.0/eurmlsdk/__init__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     6249 2024-05-16 10:48:46.000000 eurmlsdk-0.1.0/eurmlsdk/__main__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     9540 2024-05-15 12:55:17.000000 eurmlsdk-0.1.0/eurmlsdk/eur_sdk.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     4036 2024-05-16 07:32:23.000000 eurmlsdk-0.1.0/eurmlsdk/pytorch.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     1217 2024-05-16 10:29:42.000000 eurmlsdk-0.1.0/eurmlsdk/yolo.py
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 10:48:52.603050 eurmlsdk-0.1.0/eurmlsdk.egg-info/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      382 2024-05-16 10:48:52.000000 eurmlsdk-0.1.0/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      335 2024-05-16 10:48:52.000000 eurmlsdk-0.1.0/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-16 10:48:52.000000 eurmlsdk-0.1.0/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-16 10:48:52.000000 eurmlsdk-0.1.0/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      102 2024-05-16 10:48:52.000000 eurmlsdk-0.1.0/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-16 10:48:52.000000 eurmlsdk-0.1.0/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-16 10:48:52.603050 eurmlsdk-0.1.0/setup.cfg
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      845 2024-05-16 10:48:40.000000 eurmlsdk-0.1.0/setup.py
+drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-17 11:41:16.557587 eurmlsdk-0.1.1/
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       16 2024-05-07 10:55:35.000000 eurmlsdk-0.1.1/LICENSE.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       38 2024-05-07 10:55:35.000000 eurmlsdk-0.1.1/MANIFEST.in
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      382 2024-05-17 11:41:16.557587 eurmlsdk-0.1.1/PKG-INFO
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       10 2024-05-07 10:55:35.000000 eurmlsdk-0.1.1/README.md
+drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-17 11:41:16.547587 eurmlsdk-0.1.1/eurmlsdk/
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       33 2024-05-15 11:40:23.000000 eurmlsdk-0.1.1/eurmlsdk/__init__.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)     6150 2024-05-16 10:16:43.000000 eurmlsdk-0.1.1/eurmlsdk/__main__.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)     9540 2024-05-17 11:35:26.000000 eurmlsdk-0.1.1/eurmlsdk/eur_sdk.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)     4036 2024-05-16 09:13:37.000000 eurmlsdk-0.1.1/eurmlsdk/pytorch.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)     1241 2024-05-17 11:32:25.000000 eurmlsdk-0.1.1/eurmlsdk/yolo.py
+drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-17 11:41:16.557587 eurmlsdk-0.1.1/eurmlsdk.egg-info/
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      382 2024-05-17 11:41:16.000000 eurmlsdk-0.1.1/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      335 2024-05-17 11:41:16.000000 eurmlsdk-0.1.1/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)        1 2024-05-17 11:41:16.000000 eurmlsdk-0.1.1/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       53 2024-05-17 11:41:16.000000 eurmlsdk-0.1.1/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      129 2024-05-17 11:41:16.000000 eurmlsdk-0.1.1/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)        9 2024-05-17 11:41:16.000000 eurmlsdk-0.1.1/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       38 2024-05-17 11:41:16.557587 eurmlsdk-0.1.1/setup.cfg
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      894 2024-05-17 11:41:06.000000 eurmlsdk-0.1.1/setup.py
```

### Comparing `eurmlsdk-0.1.0/eurmlsdk/__main__.py` & `eurmlsdk-0.1.1/eurmlsdk/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,35 +10,35 @@
 
 def list_commands():
     print("Available commands in eurmlsdk package are:")
     print("  deploy <model type> <model path> <hostname> <username> <password> : Uploads the model file and executes remote script")
     print("  help | --h                                           : Lists all commands available in eurmlsdk package")
     print("  predict <model path> <dataset path>                  : Predicts the labels and saves the predicted result")
     print("  validate <task> <model path>                         : Validates the model and returns the metrics using default dataset")
-    print("  pt-predict <model name>                              : Predicts the labels and prints the predicted results")
-    print("  pt-list-model                                        : Lists all the pytorch models available")
-    print("  pt-validate <model name>                             : Validates the model and prints the metrics")
     print(" ")
+    print("pytorch commands")
+    print("pt-predict <modelname>                                 : Predicts the labels and prints the predicted results")
+    print("pt-list-model                                          : list all the pytorch models available")
     print("Options:")
     print(" <dataset path> : Image or Video path")
     print(" <hostname>     : Remote Server hostname")
     print(" <model path>   : Model file path")
     print(" <model type>   : Model type - 'yolo' or 'pt'")
     print(" <password>     : Remote Server password")
     print(" <task>         : Validation task - 'seg' or 'pose' or 'detect' or 'classify'")
     print(" <username>     : Remote Server username")
 
 def main():
-    commands_list = ['deploy','help','--h','predict','validate', 'pt-predict', 'pt-validate', 'pt-list-model']
+    commands_list = ['deploy','help','--h','predict','validate', 'pt-predict', 'pt-validate']
     try:
         argLen = len(argv)
         if argLen == 1:
             print("Model Zoo SDK")
             print("Package name: eurmlsdk")
-            print("Version: 0.1.0")
+            print("Version: 0.0.902")
             print("Run 'eurmlsdk help' or eurmlsdk --h to find the list of commands.")
             exit()
 
         command = argv[1]
         if command not in commands_list:
             print("Unknown command. Please find the list of commands")
             list_commands()
```

### Comparing `eurmlsdk-0.1.0/eurmlsdk/eur_sdk.py` & `eurmlsdk-0.1.1/eurmlsdk/eur_sdk.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.1.0/eurmlsdk/pytorch.py` & `eurmlsdk-0.1.1/eurmlsdk/pytorch.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.1.0/eurmlsdk/yolo.py` & `eurmlsdk-0.1.1/eurmlsdk/yolo.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         else:
             raise ModelNotFound()
         
     def predict_model(self, pathArg, dataSet):
         try:
             model = self.load_model(pathArg)
             print("Prediction started.....")
-            model.predict(dataSet, save=True)
+            model.predict(dataSet, save=True, show=True, stream=True)
         except ModelNotFound as err:
             print("Error :", err)
             exit(1)
         except Exception as err:
             print("Error in Prediction :", err)
             exit(1)
```

### Comparing `eurmlsdk-0.1.0/setup.py` & `eurmlsdk-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.1.0',
+    version='0.1.1',
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
         'torchvision'
-    ],
+        'menpo',
+        'opencv-contrib-python'    
+],
     author='eUR',
     author_email='aiml@embedur.com',
     license='MIT',
     entry_points={
         "console_scripts": [
             "eurmlsdk = eurmlsdk.__main__:main"
         ]
```

