# Comparing `tmp/iguana-0.1.4.tar.gz` & `tmp/iguana-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iguana-0.1.4.tar", last modified: Wed May 15 21:09:32 2024, max compression
+gzip compressed data, was "iguana-0.1.5.tar", last modified: Fri May 17 08:38:43 2024, max compression
```

## Comparing `iguana-0.1.4.tar` & `iguana-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 keksi     (1000) keksi     (1000)        0 2024-05-15 21:09:32.358583 iguana-0.1.4/
--rw-r--r--   0 keksi     (1000) keksi     (1000)     1066 2024-05-15 13:59:07.000000 iguana-0.1.4/LICENSE
--rw-r--r--   0 keksi     (1000) keksi     (1000)     7179 2024-05-15 21:09:32.358583 iguana-0.1.4/PKG-INFO
--rw-r--r--   0 keksi     (1000) keksi     (1000)     6745 2024-05-15 13:59:07.000000 iguana-0.1.4/README.md
-drwxr-xr-x   0 keksi     (1000) keksi     (1000)        0 2024-05-15 21:09:32.358583 iguana-0.1.4/iguana/
--rw-r--r--   0 keksi     (1000) keksi     (1000)        0 2024-05-15 13:59:07.000000 iguana-0.1.4/iguana/__init__.py
--rw-r--r--   0 keksi     (1000) keksi     (1000)     7405 2024-05-15 21:08:28.000000 iguana-0.1.4/iguana/iguana.py
-drwxr-xr-x   0 keksi     (1000) keksi     (1000)        0 2024-05-15 21:09:32.358583 iguana-0.1.4/iguana.egg-info/
--rw-r--r--   0 keksi     (1000) keksi     (1000)     7179 2024-05-15 21:09:32.000000 iguana-0.1.4/iguana.egg-info/PKG-INFO
--rw-r--r--   0 keksi     (1000) keksi     (1000)      244 2024-05-15 21:09:32.000000 iguana-0.1.4/iguana.egg-info/SOURCES.txt
--rw-r--r--   0 keksi     (1000) keksi     (1000)        1 2024-05-15 21:09:32.000000 iguana-0.1.4/iguana.egg-info/dependency_links.txt
--rw-r--r--   0 keksi     (1000) keksi     (1000)       46 2024-05-15 21:09:32.000000 iguana-0.1.4/iguana.egg-info/entry_points.txt
--rw-r--r--   0 keksi     (1000) keksi     (1000)       16 2024-05-15 21:09:32.000000 iguana-0.1.4/iguana.egg-info/requires.txt
--rw-r--r--   0 keksi     (1000) keksi     (1000)        7 2024-05-15 21:09:32.000000 iguana-0.1.4/iguana.egg-info/top_level.txt
--rw-r--r--   0 keksi     (1000) keksi     (1000)       38 2024-05-15 21:09:32.358583 iguana-0.1.4/setup.cfg
--rw-r--r--   0 keksi     (1000) keksi     (1000)      768 2024-05-15 21:09:18.000000 iguana-0.1.4/setup.py
+drwxr-xr-x   0 keksi     (1000) keksi     (1000)        0 2024-05-17 08:38:43.300307 iguana-0.1.5/
+-rw-r--r--   0 keksi     (1000) keksi     (1000)     1066 2024-05-15 13:59:07.000000 iguana-0.1.5/LICENSE
+-rw-r--r--   0 keksi     (1000) keksi     (1000)     7179 2024-05-17 08:38:43.300307 iguana-0.1.5/PKG-INFO
+-rw-r--r--   0 keksi     (1000) keksi     (1000)     6745 2024-05-15 13:59:07.000000 iguana-0.1.5/README.md
+drwxr-xr-x   0 keksi     (1000) keksi     (1000)        0 2024-05-17 08:38:43.300307 iguana-0.1.5/iguana/
+-rw-r--r--   0 keksi     (1000) keksi     (1000)        0 2024-05-15 13:59:07.000000 iguana-0.1.5/iguana/__init__.py
+-rw-r--r--   0 keksi     (1000) keksi     (1000)     7528 2024-05-17 08:36:55.000000 iguana-0.1.5/iguana/iguana.py
+drwxr-xr-x   0 keksi     (1000) keksi     (1000)        0 2024-05-17 08:38:43.300307 iguana-0.1.5/iguana.egg-info/
+-rw-r--r--   0 keksi     (1000) keksi     (1000)     7179 2024-05-17 08:38:43.000000 iguana-0.1.5/iguana.egg-info/PKG-INFO
+-rw-r--r--   0 keksi     (1000) keksi     (1000)      244 2024-05-17 08:38:43.000000 iguana-0.1.5/iguana.egg-info/SOURCES.txt
+-rw-r--r--   0 keksi     (1000) keksi     (1000)        1 2024-05-17 08:38:43.000000 iguana-0.1.5/iguana.egg-info/dependency_links.txt
+-rw-r--r--   0 keksi     (1000) keksi     (1000)       46 2024-05-17 08:38:43.000000 iguana-0.1.5/iguana.egg-info/entry_points.txt
+-rw-r--r--   0 keksi     (1000) keksi     (1000)       16 2024-05-17 08:38:43.000000 iguana-0.1.5/iguana.egg-info/requires.txt
+-rw-r--r--   0 keksi     (1000) keksi     (1000)        7 2024-05-17 08:38:43.000000 iguana-0.1.5/iguana.egg-info/top_level.txt
+-rw-r--r--   0 keksi     (1000) keksi     (1000)       38 2024-05-17 08:38:43.300307 iguana-0.1.5/setup.cfg
+-rw-r--r--   0 keksi     (1000) keksi     (1000)      768 2024-05-17 08:38:09.000000 iguana-0.1.5/setup.py
```

### Comparing `iguana-0.1.4/LICENSE` & `iguana-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `iguana-0.1.4/PKG-INFO` & `iguana-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iguana
-Version: 0.1.4
+Version: 0.1.5
 Summary: A network scanning tool for Kali Linux
 Home-page: https://github.com/uveissmjl/iguana
 Author: Uveis Smajli
 Author-email: smajliuveis@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iguana-0.1.4/README.md` & `iguana-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `iguana-0.1.4/iguana/iguana.py` & `iguana-0.1.5/iguana/iguana.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 import argparse
 import sys
 from scapy.all import ARP, Ether, srp, sniff
 import socket
 import dns.resolver
 import threading
+import os
+
+def main(
+    if os.geteuid() != 0:
+        print("This script requires root privilages")
+        sys.exit(1)
+)
 
 iguana_art = """
 ⢀⣤⠴⠖⠋⠉⠓⢦⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
 ⣿⣄⠀⠂⠀⢶⣿⣇⡙⠷⣄⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣀⣀⣀⣀⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
 ⠈⢳⡝⠢⡀⠀⠁⠀⠙⠦⣈⢻⡄⠀⠀⠀⠀⣠⢖⣶⡶⠶⠚⠛⠉⣉⠭⠝⠛⠋⠉⠉⠉⠛⠛⠓⠒⠶⠤⣤⣀⡀⠀⠀⠀⠀⠀⠀⠀⠀
 ⠀⠀⠙⣦⠈⠲⠄⣀⠀⢾⡏⠑⠿⡦⣤⣴⠞⠛⢉⣁⣀⠠⠤⠒⠉⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠉⠙⠓⠶⣤⡀⠀⠀⠀⠀
 ⠀⠀⠀⠈⠳⣄⡀⠀⠙⢓⡆⠠⢲⢾⣖⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⡔⠀⢦⠤⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠙⠳⣄⠀⠀
```

### Comparing `iguana-0.1.4/iguana.egg-info/PKG-INFO` & `iguana-0.1.5/iguana.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iguana
-Version: 0.1.4
+Version: 0.1.5
 Summary: A network scanning tool for Kali Linux
 Home-page: https://github.com/uveissmjl/iguana
 Author: Uveis Smajli
 Author-email: smajliuveis@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iguana-0.1.4/setup.py` & `iguana-0.1.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='iguana',
-    version='0.1.4',
+    version='0.1.5',
     description='A network scanning tool for Kali Linux',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Uveis Smajli',
     author_email='smajliuveis@yahoo.com',
     url='https://github.com/uveissmjl/iguana',
     packages=find_packages(),
```

