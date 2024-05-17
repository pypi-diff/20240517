# Comparing `tmp/iguana-0.1.5.tar.gz` & `tmp/iguana-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iguana-0.1.5.tar", last modified: Fri May 17 08:38:43 2024, max compression
+gzip compressed data, was "iguana-0.1.6.tar", last modified: Fri May 17 08:49:37 2024, max compression
```

## Comparing `iguana-0.1.5.tar` & `iguana-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 keksi     (1000) keksi     (1000)        0 2024-05-17 08:38:43.300307 iguana-0.1.5/
--rw-r--r--   0 keksi     (1000) keksi     (1000)     1066 2024-05-15 13:59:07.000000 iguana-0.1.5/LICENSE
--rw-r--r--   0 keksi     (1000) keksi     (1000)     7179 2024-05-17 08:38:43.300307 iguana-0.1.5/PKG-INFO
--rw-r--r--   0 keksi     (1000) keksi     (1000)     6745 2024-05-15 13:59:07.000000 iguana-0.1.5/README.md
-drwxr-xr-x   0 keksi     (1000) keksi     (1000)        0 2024-05-17 08:38:43.300307 iguana-0.1.5/iguana/
--rw-r--r--   0 keksi     (1000) keksi     (1000)        0 2024-05-15 13:59:07.000000 iguana-0.1.5/iguana/__init__.py
--rw-r--r--   0 keksi     (1000) keksi     (1000)     7528 2024-05-17 08:36:55.000000 iguana-0.1.5/iguana/iguana.py
-drwxr-xr-x   0 keksi     (1000) keksi     (1000)        0 2024-05-17 08:38:43.300307 iguana-0.1.5/iguana.egg-info/
--rw-r--r--   0 keksi     (1000) keksi     (1000)     7179 2024-05-17 08:38:43.000000 iguana-0.1.5/iguana.egg-info/PKG-INFO
--rw-r--r--   0 keksi     (1000) keksi     (1000)      244 2024-05-17 08:38:43.000000 iguana-0.1.5/iguana.egg-info/SOURCES.txt
--rw-r--r--   0 keksi     (1000) keksi     (1000)        1 2024-05-17 08:38:43.000000 iguana-0.1.5/iguana.egg-info/dependency_links.txt
--rw-r--r--   0 keksi     (1000) keksi     (1000)       46 2024-05-17 08:38:43.000000 iguana-0.1.5/iguana.egg-info/entry_points.txt
--rw-r--r--   0 keksi     (1000) keksi     (1000)       16 2024-05-17 08:38:43.000000 iguana-0.1.5/iguana.egg-info/requires.txt
--rw-r--r--   0 keksi     (1000) keksi     (1000)        7 2024-05-17 08:38:43.000000 iguana-0.1.5/iguana.egg-info/top_level.txt
--rw-r--r--   0 keksi     (1000) keksi     (1000)       38 2024-05-17 08:38:43.300307 iguana-0.1.5/setup.cfg
--rw-r--r--   0 keksi     (1000) keksi     (1000)      768 2024-05-17 08:38:09.000000 iguana-0.1.5/setup.py
+drwxr-xr-x   0 keksi     (1000) keksi     (1000)        0 2024-05-17 08:49:37.460844 iguana-0.1.6/
+-rw-r--r--   0 keksi     (1000) keksi     (1000)     1066 2024-05-15 13:59:07.000000 iguana-0.1.6/LICENSE
+-rw-r--r--   0 keksi     (1000) keksi     (1000)     7176 2024-05-17 08:49:37.460844 iguana-0.1.6/PKG-INFO
+-rw-r--r--   0 keksi     (1000) keksi     (1000)     6745 2024-05-15 13:59:07.000000 iguana-0.1.6/README.md
+drwxr-xr-x   0 keksi     (1000) keksi     (1000)        0 2024-05-17 08:49:37.456843 iguana-0.1.6/iguana/
+-rw-r--r--   0 keksi     (1000) keksi     (1000)        0 2024-05-15 13:59:07.000000 iguana-0.1.6/iguana/__init__.py
+-rw-r--r--   0 keksi     (1000) keksi     (1000)     7528 2024-05-17 08:36:55.000000 iguana-0.1.6/iguana/iguana.py
+drwxr-xr-x   0 keksi     (1000) keksi     (1000)        0 2024-05-17 08:49:37.460844 iguana-0.1.6/iguana.egg-info/
+-rw-r--r--   0 keksi     (1000) keksi     (1000)     7176 2024-05-17 08:49:37.000000 iguana-0.1.6/iguana.egg-info/PKG-INFO
+-rw-r--r--   0 keksi     (1000) keksi     (1000)      244 2024-05-17 08:49:37.000000 iguana-0.1.6/iguana.egg-info/SOURCES.txt
+-rw-r--r--   0 keksi     (1000) keksi     (1000)        1 2024-05-17 08:49:37.000000 iguana-0.1.6/iguana.egg-info/dependency_links.txt
+-rw-r--r--   0 keksi     (1000) keksi     (1000)       39 2024-05-17 08:49:37.000000 iguana-0.1.6/iguana.egg-info/entry_points.txt
+-rw-r--r--   0 keksi     (1000) keksi     (1000)       16 2024-05-17 08:49:37.000000 iguana-0.1.6/iguana.egg-info/requires.txt
+-rw-r--r--   0 keksi     (1000) keksi     (1000)        7 2024-05-17 08:49:37.000000 iguana-0.1.6/iguana.egg-info/top_level.txt
+-rw-r--r--   0 keksi     (1000) keksi     (1000)       38 2024-05-17 08:49:37.460844 iguana-0.1.6/setup.cfg
+-rw-r--r--   0 keksi     (1000) keksi     (1000)      758 2024-05-17 08:48:53.000000 iguana-0.1.6/setup.py
```

### Comparing `iguana-0.1.5/LICENSE` & `iguana-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `iguana-0.1.5/PKG-INFO` & `iguana-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: iguana
-Version: 0.1.5
+Version: 0.1.6
 Summary: A network scanning tool for Kali Linux
-Home-page: https://github.com/uveissmjl/iguana
+Home-page: https://pypi.org/project/iguana/
 Author: Uveis Smajli
 Author-email: smajliuveis@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `iguana-0.1.5/README.md` & `iguana-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `iguana-0.1.5/iguana/iguana.py` & `iguana-0.1.6/iguana/iguana.py`

 * *Files identical despite different names*

### Comparing `iguana-0.1.5/iguana.egg-info/PKG-INFO` & `iguana-0.1.6/iguana.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: iguana
-Version: 0.1.5
+Version: 0.1.6
 Summary: A network scanning tool for Kali Linux
-Home-page: https://github.com/uveissmjl/iguana
+Home-page: https://pypi.org/project/iguana/
 Author: Uveis Smajli
 Author-email: smajliuveis@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `iguana-0.1.5/setup.py` & `iguana-0.1.6/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='iguana',
-    version='0.1.5',
+    version='0.1.6',
     description='A network scanning tool for Kali Linux',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Uveis Smajli',
     author_email='smajliuveis@yahoo.com',
-    url='https://github.com/uveissmjl/iguana',
+    url='https://pypi.org/project/iguana/',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
-            'iguana=iguana.iguana:main',
+            'iguana=iguana:main',
         ],
     },
     install_requires=[
         'scapy',
         'dnspython',
     ],
     classifiers=[
```

