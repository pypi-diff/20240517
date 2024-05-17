# Comparing `tmp/clean-alchemy-0.1.4.tar.gz` & `tmp/clean-alchemy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean-alchemy-0.1.4.tar", last modified: Fri May 17 08:07:41 2024, max compression
+gzip compressed data, was "clean-alchemy-0.1.5.tar", last modified: Fri May 17 08:14:35 2024, max compression
```

## Comparing `clean-alchemy-0.1.4.tar` & `clean-alchemy-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-17 08:07:41.753346 clean-alchemy-0.1.4/
--rw-r--r--   0 swords     (501) staff       (20)    11357 2024-05-15 18:56:06.000000 clean-alchemy-0.1.4/LICENSE
--rw-r--r--   0 swords     (501) staff       (20)     1481 2024-05-17 08:07:41.753205 clean-alchemy-0.1.4/PKG-INFO
--rw-r--r--   0 swords     (501) staff       (20)      883 2024-05-15 18:56:06.000000 clean-alchemy-0.1.4/README.md
-drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-17 08:07:41.752167 clean-alchemy-0.1.4/clean_alchemy/
--rw-r--r--   0 swords     (501) staff       (20)      235 2024-05-17 08:06:35.000000 clean-alchemy-0.1.4/clean_alchemy/__init__.py
--rw-r--r--   0 swords     (501) staff       (20)      445 2024-05-15 20:09:20.000000 clean-alchemy-0.1.4/clean_alchemy/_base.py
--rw-r--r--   0 swords     (501) staff       (20)      777 2024-05-17 08:06:21.000000 clean-alchemy-0.1.4/clean_alchemy/_base_dao.py
--rw-r--r--   0 swords     (501) staff       (20)      500 2024-05-15 18:56:06.000000 clean-alchemy-0.1.4/clean_alchemy/_base_ent.py
--rw-r--r--   0 swords     (501) staff       (20)     3645 2024-05-16 17:18:08.000000 clean-alchemy-0.1.4/clean_alchemy/_base_rpo.py
--rw-r--r--   0 swords     (501) staff       (20)     2015 2024-05-15 20:12:10.000000 clean-alchemy-0.1.4/clean_alchemy/_base_srv.py
--rw-r--r--   0 swords     (501) staff       (20)      357 2024-05-15 18:56:06.000000 clean-alchemy-0.1.4/clean_alchemy/config.py
-drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-17 08:07:41.752980 clean-alchemy-0.1.4/clean_alchemy.egg-info/
--rw-r--r--   0 swords     (501) staff       (20)     1481 2024-05-17 08:07:41.000000 clean-alchemy-0.1.4/clean_alchemy.egg-info/PKG-INFO
--rw-r--r--   0 swords     (501) staff       (20)      391 2024-05-17 08:07:41.000000 clean-alchemy-0.1.4/clean_alchemy.egg-info/SOURCES.txt
--rw-r--r--   0 swords     (501) staff       (20)        1 2024-05-17 08:07:41.000000 clean-alchemy-0.1.4/clean_alchemy.egg-info/dependency_links.txt
--rw-r--r--   0 swords     (501) staff       (20)      516 2024-05-17 08:07:41.000000 clean-alchemy-0.1.4/clean_alchemy.egg-info/requires.txt
--rw-r--r--   0 swords     (501) staff       (20)       14 2024-05-17 08:07:41.000000 clean-alchemy-0.1.4/clean_alchemy.egg-info/top_level.txt
--rw-r--r--   0 swords     (501) staff       (20)       38 2024-05-17 08:07:41.753406 clean-alchemy-0.1.4/setup.cfg
--rw-r--r--   0 swords     (501) staff       (20)     1669 2024-05-17 08:07:18.000000 clean-alchemy-0.1.4/setup.py
+drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-17 08:14:35.418117 clean-alchemy-0.1.5/
+-rw-r--r--   0 swords     (501) staff       (20)    11357 2024-05-15 18:56:06.000000 clean-alchemy-0.1.5/LICENSE
+-rw-r--r--   0 swords     (501) staff       (20)     1481 2024-05-17 08:14:35.417976 clean-alchemy-0.1.5/PKG-INFO
+-rw-r--r--   0 swords     (501) staff       (20)      883 2024-05-15 18:56:06.000000 clean-alchemy-0.1.5/README.md
+drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-17 08:14:35.417062 clean-alchemy-0.1.5/clean_alchemy/
+-rw-r--r--   0 swords     (501) staff       (20)      195 2024-05-17 08:13:25.000000 clean-alchemy-0.1.5/clean_alchemy/__init__.py
+-rw-r--r--   0 swords     (501) staff       (20)      445 2024-05-15 20:09:20.000000 clean-alchemy-0.1.5/clean_alchemy/base.py
+-rw-r--r--   0 swords     (501) staff       (20)      777 2024-05-17 08:06:21.000000 clean-alchemy-0.1.5/clean_alchemy/base_dao.py
+-rw-r--r--   0 swords     (501) staff       (20)      500 2024-05-15 18:56:06.000000 clean-alchemy-0.1.5/clean_alchemy/base_ent.py
+-rw-r--r--   0 swords     (501) staff       (20)     3645 2024-05-16 17:18:08.000000 clean-alchemy-0.1.5/clean_alchemy/base_rpo.py
+-rw-r--r--   0 swords     (501) staff       (20)     2015 2024-05-15 20:12:10.000000 clean-alchemy-0.1.5/clean_alchemy/base_srv.py
+-rw-r--r--   0 swords     (501) staff       (20)      357 2024-05-15 18:56:06.000000 clean-alchemy-0.1.5/clean_alchemy/config.py
+drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-17 08:14:35.417762 clean-alchemy-0.1.5/clean_alchemy.egg-info/
+-rw-r--r--   0 swords     (501) staff       (20)     1481 2024-05-17 08:14:35.000000 clean-alchemy-0.1.5/clean_alchemy.egg-info/PKG-INFO
+-rw-r--r--   0 swords     (501) staff       (20)      386 2024-05-17 08:14:35.000000 clean-alchemy-0.1.5/clean_alchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 swords     (501) staff       (20)        1 2024-05-17 08:14:35.000000 clean-alchemy-0.1.5/clean_alchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 swords     (501) staff       (20)      516 2024-05-17 08:14:35.000000 clean-alchemy-0.1.5/clean_alchemy.egg-info/requires.txt
+-rw-r--r--   0 swords     (501) staff       (20)       14 2024-05-17 08:14:35.000000 clean-alchemy-0.1.5/clean_alchemy.egg-info/top_level.txt
+-rw-r--r--   0 swords     (501) staff       (20)       38 2024-05-17 08:14:35.418183 clean-alchemy-0.1.5/setup.cfg
+-rw-r--r--   0 swords     (501) staff       (20)     1669 2024-05-17 08:13:50.000000 clean-alchemy-0.1.5/setup.py
```

### Comparing `clean-alchemy-0.1.4/LICENSE` & `clean-alchemy-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `clean-alchemy-0.1.4/PKG-INFO` & `clean-alchemy-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-alchemy
-Version: 0.1.4
+Version: 0.1.5
 Summary: A framework for implementing Clean Architecture using SQLAlchemy, with currently only support for FastAPI.
 Home-page: https://github.com/davidswords/clean-alchemy
 Author: David Swords
 Author-email: furuer_svette.0k@icloud.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clean-alchemy-0.1.4/README.md` & `clean-alchemy-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `clean-alchemy-0.1.4/clean_alchemy/_base_dao.py` & `clean-alchemy-0.1.5/clean_alchemy/base_dao.py`

 * *Files identical despite different names*

### Comparing `clean-alchemy-0.1.4/clean_alchemy/_base_rpo.py` & `clean-alchemy-0.1.5/clean_alchemy/base_rpo.py`

 * *Files identical despite different names*

### Comparing `clean-alchemy-0.1.4/clean_alchemy/_base_srv.py` & `clean-alchemy-0.1.5/clean_alchemy/base_srv.py`

 * *Files identical despite different names*

### Comparing `clean-alchemy-0.1.4/clean_alchemy.egg-info/PKG-INFO` & `clean-alchemy-0.1.5/clean_alchemy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-alchemy
-Version: 0.1.4
+Version: 0.1.5
 Summary: A framework for implementing Clean Architecture using SQLAlchemy, with currently only support for FastAPI.
 Home-page: https://github.com/davidswords/clean-alchemy
 Author: David Swords
 Author-email: furuer_svette.0k@icloud.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clean-alchemy-0.1.4/clean_alchemy.egg-info/requires.txt` & `clean-alchemy-0.1.5/clean_alchemy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `clean-alchemy-0.1.4/setup.py` & `clean-alchemy-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="clean-alchemy",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(exclude=["tests*", "build*"]),
     install_requires=[
         "annotated-types==0.6.0",
         "black==24.4.2",
         "click==8.1.7",
         "exceptiongroup==1.2.1",
         "factory-boy==3.3.0",
```

