# Comparing `tmp/dbSQL_connect-0.0.3.tar.gz` & `tmp/dbSQL_connect-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbSQL_connect-0.0.3.tar", last modified: Fri May 17 01:33:26 2024, max compression
+gzip compressed data, was "dbSQL_connect-0.0.4.tar", last modified: Fri May 17 05:17:16 2024, max compression
```

## Comparing `dbSQL_connect-0.0.3.tar` & `dbSQL_connect-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 01:33:26.141390 dbSQL_connect-0.0.3/
--rw-rw-rw-   0        0        0      423 2024-05-17 01:33:26.141390 dbSQL_connect-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-13 19:50:39.000000 dbSQL_connect-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 01:33:26.136403 dbSQL_connect-0.0.3/dbSQL_connect/
--rw-rw-rw-   0        0        0        0 2024-05-13 20:38:13.000000 dbSQL_connect-0.0.3/dbSQL_connect/__init__.py
--rw-rw-rw-   0        0        0     5963 2024-05-14 03:44:55.000000 dbSQL_connect-0.0.3/dbSQL_connect/_entry_points.py
--rw-rw-rw-   0        0        0     3735 2024-05-17 01:03:30.000000 dbSQL_connect-0.0.3/dbSQL_connect/_imp.py
--rw-rw-rw-   0        0        0    36807 2024-05-17 01:32:35.000000 dbSQL_connect-0.0.3/dbSQL_connect/requires.py
-drwxrwxrwx   0        0        0        0 2024-05-17 01:33:26.140394 dbSQL_connect-0.0.3/dbSQL_connect.egg-info/
--rw-rw-rw-   0        0        0      423 2024-05-17 01:33:26.000000 dbSQL_connect-0.0.3/dbSQL_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2024-05-17 01:33:26.000000 dbSQL_connect-0.0.3/dbSQL_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 01:33:26.000000 dbSQL_connect-0.0.3/dbSQL_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-17 01:33:26.000000 dbSQL_connect-0.0.3/dbSQL_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-17 01:33:26.000000 dbSQL_connect-0.0.3/dbSQL_connect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 01:33:26.142388 dbSQL_connect-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      685 2024-05-17 01:33:23.000000 dbSQL_connect-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 05:17:16.867299 dbSQL_connect-0.0.4/
+-rw-rw-rw-   0        0        0      423 2024-05-17 05:17:16.868296 dbSQL_connect-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-13 19:50:39.000000 dbSQL_connect-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 05:17:16.862312 dbSQL_connect-0.0.4/dbSQL_connect/
+-rw-rw-rw-   0        0        0        0 2024-05-13 20:38:13.000000 dbSQL_connect-0.0.4/dbSQL_connect/__init__.py
+-rw-rw-rw-   0        0        0     5963 2024-05-14 03:44:55.000000 dbSQL_connect-0.0.4/dbSQL_connect/_entry_points.py
+-rw-rw-rw-   0        0        0     3735 2024-05-17 02:10:18.000000 dbSQL_connect-0.0.4/dbSQL_connect/_imp.py
+-rw-rw-rw-   0        0        0    36807 2024-05-17 01:32:35.000000 dbSQL_connect-0.0.4/dbSQL_connect/requires.py
+drwxrwxrwx   0        0        0        0 2024-05-17 05:17:16.867299 dbSQL_connect-0.0.4/dbSQL_connect.egg-info/
+-rw-rw-rw-   0        0        0      423 2024-05-17 05:17:16.000000 dbSQL_connect-0.0.4/dbSQL_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2024-05-17 05:17:16.000000 dbSQL_connect-0.0.4/dbSQL_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 05:17:16.000000 dbSQL_connect-0.0.4/dbSQL_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-17 05:17:16.000000 dbSQL_connect-0.0.4/dbSQL_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-17 05:17:16.000000 dbSQL_connect-0.0.4/dbSQL_connect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 05:17:16.868296 dbSQL_connect-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      685 2024-05-17 05:17:10.000000 dbSQL_connect-0.0.4/setup.py
```

### Comparing `dbSQL_connect-0.0.3/dbSQL_connect/_entry_points.py` & `dbSQL_connect-0.0.4/dbSQL_connect/_entry_points.py`

 * *Files identical despite different names*

### Comparing `dbSQL_connect-0.0.3/dbSQL_connect/_imp.py` & `dbSQL_connect-0.0.4/dbSQL_connect/_imp.py`

 * *Files identical despite different names*

### Comparing `dbSQL_connect-0.0.3/dbSQL_connect/requires.py` & `dbSQL_connect-0.0.4/dbSQL_connect/requires.py`

 * *Files identical despite different names*

### Comparing `dbSQL_connect-0.0.3/setup.py` & `dbSQL_connect-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 
 setup(
   name='dbSQL_connect',
-  version='0.0.3',
+  version='0.0.4',
   author='virginxlub',
   author_email='vzlomka927@yandex.ru',
   description='This is the simplest module for quick work with files.',
   long_description=readme(),
   long_description_content_type='text/markdown',
   packages=find_packages(),
   install_requires=['requests>=2.25.1'],
```

