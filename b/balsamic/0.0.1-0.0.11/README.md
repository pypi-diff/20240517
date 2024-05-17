# Comparing `tmp/balsamic-0.0.1.tar.gz` & `tmp/balsamic-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balsamic-0.0.1.tar", last modified: Fri May 17 19:45:58 2024, max compression
+gzip compressed data, was "balsamic-0.0.11.tar", last modified: Fri May 17 19:51:54 2024, max compression
```

## Comparing `balsamic-0.0.1.tar` & `balsamic-0.0.11.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 19:45:58.659171 balsamic-0.0.1/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2108 2024-05-17 19:45:58.655171 balsamic-0.0.1/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1574 2024-05-17 19:32:39.000000 balsamic-0.0.1/README.md
-drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 19:45:58.655171 balsamic-0.0.1/balsamic.egg-info/
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2108 2024-05-17 19:45:58.000000 balsamic-0.0.1/balsamic.egg-info/PKG-INFO
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      177 2024-05-17 19:45:58.000000 balsamic-0.0.1/balsamic.egg-info/SOURCES.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:45:58.000000 balsamic-0.0.1/balsamic.egg-info/dependency_links.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       39 2024-05-17 19:45:58.000000 balsamic-0.0.1/balsamic.egg-info/requires.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:45:58.000000 balsamic-0.0.1/balsamic.egg-info/top_level.txt
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-17 19:45:58.659171 balsamic-0.0.1/setup.cfg
--rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1203 2024-05-17 19:43:56.000000 balsamic-0.0.1/setup.py
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 19:51:54.699953 balsamic-0.0.11/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2109 2024-05-17 19:51:54.695953 balsamic-0.0.11/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1574 2024-05-17 19:32:39.000000 balsamic-0.0.11/README.md
+drwxr-xr-x   0 witchdoc  (1000) witchdoc  (1001)        0 2024-05-17 19:51:54.695953 balsamic-0.0.11/balsamic.egg-info/
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     2109 2024-05-17 19:51:54.000000 balsamic-0.0.11/balsamic.egg-info/PKG-INFO
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)      177 2024-05-17 19:51:54.000000 balsamic-0.0.11/balsamic.egg-info/SOURCES.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:51:54.000000 balsamic-0.0.11/balsamic.egg-info/dependency_links.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       40 2024-05-17 19:51:54.000000 balsamic-0.0.11/balsamic.egg-info/requires.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)        1 2024-05-17 19:51:54.000000 balsamic-0.0.11/balsamic.egg-info/top_level.txt
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)       38 2024-05-17 19:51:54.699953 balsamic-0.0.11/setup.cfg
+-rw-r--r--   0 witchdoc  (1000) witchdoc  (1001)     1205 2024-05-17 19:51:47.000000 balsamic-0.0.11/setup.py
```

### Comparing `balsamic-0.0.1/PKG-INFO` & `balsamic-0.0.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.0.1
+Version: 0.0.11
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.0.1/README.md` & `balsamic-0.0.11/README.md`

 * *Files identical despite different names*

### Comparing `balsamic-0.0.1/balsamic.egg-info/PKG-INFO` & `balsamic-0.0.11/balsamic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsamic
-Version: 0.0.1
+Version: 0.0.11
 Summary: Send malicious pickles via requests or sockets
 Author: Witchdoctor (malectrica)
 Keywords: python,hack,pickle,serialization,security,sockets,web
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `balsamic-0.0.1/setup.py` & `balsamic-0.0.11/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.11'
 DESCRIPTION = 'Send malicious pickles via requests or sockets'
 LONG_DESCRIPTION = 'A package that allows the user to easily send out malicious pickles, via web requests, or a malicious server or client(currently ipv4 only)'
 
 # Setting up
 setup(
     name="balsamic",
     version=VERSION,
     author="Witchdoctor (malectrica)",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['pickle', 'base64', 'requests', 'socket', 'argparse'],
+    install_requires=['pickle5', 'base64', 'requests', 'socket', 'argparse'],
     keywords=['python', 'hack', 'pickle', 'serialization', 'security', 'sockets', 'web'],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

