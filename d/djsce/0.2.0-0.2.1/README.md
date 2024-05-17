# Comparing `tmp/djsce-0.2.0.tar.gz` & `tmp/djsce-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djsce-0.2.0.tar", last modified: Sat May  4 12:51:10 2024, max compression
+gzip compressed data, was "djsce-0.2.1.tar", last modified: Fri May 17 13:10:56 2024, max compression
```

## Comparing `djsce-0.2.0.tar` & `djsce-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 12:51:10.977380 djsce-0.2.0/
--rw-rw-rw-   0        0        0     1095 2023-12-11 07:22:54.000000 djsce-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      537 2024-05-04 12:51:10.976377 djsce-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0        7 2023-12-11 08:13:47.000000 djsce-0.2.0/README.txt
-drwxrwxrwx   0        0        0        0 2024-05-04 12:51:10.911695 djsce-0.2.0/djsce/
--rw-rw-rw-   0        0        0      138 2024-05-04 12:39:01.000000 djsce-0.2.0/djsce/__init__.py
--rw-rw-rw-   0        0        0    18825 2024-05-04 12:39:25.000000 djsce-0.2.0/djsce/ai.py
--rw-rw-rw-   0        0        0    33347 2024-05-04 12:39:28.000000 djsce-0.2.0/djsce/daa.py
--rw-rw-rw-   0        0        0     2533 2024-05-04 12:39:32.000000 djsce-0.2.0/djsce/de.py
--rw-rw-rw-   0        0        0    78867 2023-12-14 11:23:53.000000 djsce-0.2.0/djsce/dsa.py
--rw-rw-rw-   0        0        0    34344 2024-05-04 12:21:50.000000 djsce-0.2.0/djsce/os.py
--rw-rw-rw-   0        0        0    25202 2024-05-04 12:38:44.000000 djsce-0.2.0/djsce/poa.py
--rw-rw-rw-   0        0        0     9690 2023-12-14 13:15:39.000000 djsce-0.2.0/djsce/python.py
-drwxrwxrwx   0        0        0        0 2024-05-04 12:51:10.975384 djsce-0.2.0/djsce.egg-info/
--rw-rw-rw-   0        0        0      537 2024-05-04 12:51:09.000000 djsce-0.2.0/djsce.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2024-05-04 12:51:09.000000 djsce-0.2.0/djsce.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 12:51:09.000000 djsce-0.2.0/djsce.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-04 12:51:09.000000 djsce-0.2.0/djsce.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 12:51:10.977380 djsce-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      648 2024-05-04 12:51:01.000000 djsce-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:10:56.331673 djsce-0.2.1/
+-rw-rw-rw-   0        0        0     1095 2023-12-11 07:22:54.000000 djsce-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      537 2024-05-17 13:10:56.330703 djsce-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2023-12-11 08:13:47.000000 djsce-0.2.1/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 13:10:56.307652 djsce-0.2.1/djsce/
+-rw-rw-rw-   0        0        0      161 2024-05-17 13:09:44.000000 djsce-0.2.1/djsce/__init__.py
+-rw-rw-rw-   0        0        0    18825 2024-05-04 12:39:25.000000 djsce-0.2.1/djsce/ai.py
+-rw-rw-rw-   0        0        0    33347 2024-05-04 12:39:28.000000 djsce-0.2.1/djsce/daa.py
+-rw-rw-rw-   0        0        0     2533 2024-05-04 12:39:32.000000 djsce-0.2.1/djsce/de.py
+-rw-rw-rw-   0        0        0    78867 2023-12-14 11:23:53.000000 djsce-0.2.1/djsce/dsa.py
+-rw-rw-rw-   0        0        0    34344 2024-05-04 12:21:50.000000 djsce-0.2.1/djsce/os.py
+-rw-rw-rw-   0        0        0    25202 2024-05-04 12:38:44.000000 djsce-0.2.1/djsce/poa.py
+-rw-rw-rw-   0        0        0     9690 2023-12-14 13:15:39.000000 djsce-0.2.1/djsce/python.py
+-rw-rw-rw-   0        0        0    42621 2024-05-17 13:09:20.000000 djsce-0.2.1/djsce/webdev.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:10:56.324714 djsce-0.2.1/djsce.egg-info/
+-rw-rw-rw-   0        0        0      537 2024-05-17 13:10:56.000000 djsce-0.2.1/djsce.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2024-05-17 13:10:56.000000 djsce-0.2.1/djsce.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 13:10:56.000000 djsce-0.2.1/djsce.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-17 13:10:56.000000 djsce-0.2.1/djsce.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 13:10:56.331673 djsce-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      648 2024-05-17 13:10:49.000000 djsce-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:10:56.329674 djsce-0.2.1/test/
+-rw-rw-rw-   0        0        0       28 2024-05-04 12:55:52.000000 djsce-0.2.1/test/test.py
```

### Comparing `djsce-0.2.0/LICENSE` & `djsce-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `djsce-0.2.0/PKG-INFO` & `djsce-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djsce
-Version: 0.2.0
+Version: 0.2.1
 Summary: DJSCE
 Home-page: UNKNOWN
 Author: Mihir Panchal
 Author-email: mihirpanchal5400@gmail.com
 License: MIT
 Keywords: djsce
 Platform: UNKNOWN
```

### Comparing `djsce-0.2.0/djsce/ai.py` & `djsce-0.2.1/djsce/ai.py`

 * *Files identical despite different names*

### Comparing `djsce-0.2.0/djsce/daa.py` & `djsce-0.2.1/djsce/daa.py`

 * *Files identical despite different names*

### Comparing `djsce-0.2.0/djsce/de.py` & `djsce-0.2.1/djsce/de.py`

 * *Files identical despite different names*

### Comparing `djsce-0.2.0/djsce/dsa.py` & `djsce-0.2.1/djsce/dsa.py`

 * *Files identical despite different names*

### Comparing `djsce-0.2.0/djsce/os.py` & `djsce-0.2.1/djsce/os.py`

 * *Files identical despite different names*

### Comparing `djsce-0.2.0/djsce/poa.py` & `djsce-0.2.1/djsce/poa.py`

 * *Files identical despite different names*

### Comparing `djsce-0.2.0/djsce/python.py` & `djsce-0.2.1/djsce/python.py`

 * *Files identical despite different names*

### Comparing `djsce-0.2.0/djsce.egg-info/PKG-INFO` & `djsce-0.2.1/djsce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djsce
-Version: 0.2.0
+Version: 0.2.1
 Summary: DJSCE
 Home-page: UNKNOWN
 Author: Mihir Panchal
 Author-email: mihirpanchal5400@gmail.com
 License: MIT
 Keywords: djsce
 Platform: UNKNOWN
```

### Comparing `djsce-0.2.0/setup.py` & `djsce-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='djsce',
-  version='0.2.0',
+  version='0.2.1',
   description='DJSCE',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Mihir Panchal',
   author_email='mihirpanchal5400@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

