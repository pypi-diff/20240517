# Comparing `tmp/clean-alchemy-0.1.tar.gz` & `tmp/clean-alchemy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean-alchemy-0.1.tar", last modified: Wed May 15 19:27:17 2024, max compression
+gzip compressed data, was "clean-alchemy-0.1.1.tar", last modified: Thu May 16 17:22:00 2024, max compression
```

## Comparing `clean-alchemy-0.1.tar` & `clean-alchemy-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,13 @@
-drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-15 19:27:17.551312 clean-alchemy-0.1/
--rw-r--r--   0 swords     (501) staff       (20)    11357 2024-05-15 18:56:06.000000 clean-alchemy-0.1/LICENSE
--rw-r--r--   0 swords     (501) staff       (20)     1479 2024-05-15 19:27:17.551204 clean-alchemy-0.1/PKG-INFO
--rw-r--r--   0 swords     (501) staff       (20)      883 2024-05-15 18:56:06.000000 clean-alchemy-0.1/README.md
--rw-r--r--   0 swords     (501) staff       (20)       38 2024-05-15 19:27:17.551365 clean-alchemy-0.1/setup.cfg
--rw-r--r--   0 swords     (501) staff       (20)     1678 2024-05-15 19:25:39.000000 clean-alchemy-0.1/setup.py
-drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-15 19:27:17.547965 clean-alchemy-0.1/src/
-drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-15 19:27:17.549079 clean-alchemy-0.1/src/clean_alchemy/
--rw-r--r--   0 swords     (501) staff       (20)        0 2024-05-15 19:05:22.000000 clean-alchemy-0.1/src/clean_alchemy/__init__.py
-drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-15 19:27:17.550069 clean-alchemy-0.1/src/clean_alchemy/base/
--rw-r--r--   0 swords     (501) staff       (20)        0 2024-05-15 19:05:40.000000 clean-alchemy-0.1/src/clean_alchemy/base/__init__.py
-drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-15 19:27:17.550450 clean-alchemy-0.1/src/clean_alchemy/base/data/
--rw-r--r--   0 swords     (501) staff       (20)        0 2024-05-15 18:56:06.000000 clean-alchemy-0.1/src/clean_alchemy/base/data/__init__.py
--rw-r--r--   0 swords     (501) staff       (20)      772 2024-05-15 18:56:06.000000 clean-alchemy-0.1/src/clean_alchemy/base/data/dao.py
--rw-r--r--   0 swords     (501) staff       (20)     3670 2024-05-15 18:56:06.000000 clean-alchemy-0.1/src/clean_alchemy/base/data/rpo.py
-drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-15 19:27:17.550989 clean-alchemy-0.1/src/clean_alchemy/base/domain/
--rw-r--r--   0 swords     (501) staff       (20)        0 2024-05-15 18:56:06.000000 clean-alchemy-0.1/src/clean_alchemy/base/domain/__init__.py
--rw-r--r--   0 swords     (501) staff       (20)      500 2024-05-15 18:56:06.000000 clean-alchemy-0.1/src/clean_alchemy/base/domain/ent.py
--rw-r--r--   0 swords     (501) staff       (20)     2050 2024-05-15 18:56:06.000000 clean-alchemy-0.1/src/clean_alchemy/base/domain/srv.py
--rw-r--r--   0 swords     (501) staff       (20)      435 2024-05-15 18:56:06.000000 clean-alchemy-0.1/src/clean_alchemy/base.py
--rw-r--r--   0 swords     (501) staff       (20)      357 2024-05-15 18:56:06.000000 clean-alchemy-0.1/src/clean_alchemy/config.py
-drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-15 19:27:17.549919 clean-alchemy-0.1/src/clean_alchemy.egg-info/
--rw-r--r--   0 swords     (501) staff       (20)     1479 2024-05-15 19:27:17.000000 clean-alchemy-0.1/src/clean_alchemy.egg-info/PKG-INFO
--rw-r--r--   0 swords     (501) staff       (20)      575 2024-05-15 19:27:17.000000 clean-alchemy-0.1/src/clean_alchemy.egg-info/SOURCES.txt
--rw-r--r--   0 swords     (501) staff       (20)        1 2024-05-15 19:27:17.000000 clean-alchemy-0.1/src/clean_alchemy.egg-info/dependency_links.txt
--rw-r--r--   0 swords     (501) staff       (20)      516 2024-05-15 19:27:17.000000 clean-alchemy-0.1/src/clean_alchemy.egg-info/requires.txt
--rw-r--r--   0 swords     (501) staff       (20)       14 2024-05-15 19:27:17.000000 clean-alchemy-0.1/src/clean_alchemy.egg-info/top_level.txt
+drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-16 17:22:00.743852 clean-alchemy-0.1.1/
+-rw-r--r--   0 swords     (501) staff       (20)    11357 2024-05-15 18:56:06.000000 clean-alchemy-0.1.1/LICENSE
+-rw-r--r--   0 swords     (501) staff       (20)     1481 2024-05-16 17:22:00.743569 clean-alchemy-0.1.1/PKG-INFO
+-rw-r--r--   0 swords     (501) staff       (20)      883 2024-05-15 18:56:06.000000 clean-alchemy-0.1.1/README.md
+drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-16 17:22:00.740869 clean-alchemy-0.1.1/clean_alchemy/
+drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-16 17:22:00.743216 clean-alchemy-0.1.1/clean_alchemy/clean_alchemy.egg-info/
+-rw-r--r--   0 swords     (501) staff       (20)     1481 2024-05-16 17:22:00.000000 clean-alchemy-0.1.1/clean_alchemy/clean_alchemy.egg-info/PKG-INFO
+-rw-r--r--   0 swords     (501) staff       (20)      280 2024-05-16 17:22:00.000000 clean-alchemy-0.1.1/clean_alchemy/clean_alchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 swords     (501) staff       (20)        1 2024-05-16 17:22:00.000000 clean-alchemy-0.1.1/clean_alchemy/clean_alchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 swords     (501) staff       (20)      516 2024-05-16 17:22:00.000000 clean-alchemy-0.1.1/clean_alchemy/clean_alchemy.egg-info/requires.txt
+-rw-r--r--   0 swords     (501) staff       (20)        1 2024-05-16 17:22:00.000000 clean-alchemy-0.1.1/clean_alchemy/clean_alchemy.egg-info/top_level.txt
+-rw-r--r--   0 swords     (501) staff       (20)       38 2024-05-16 17:22:00.743942 clean-alchemy-0.1.1/setup.cfg
+-rw-r--r--   0 swords     (501) staff       (20)     1702 2024-05-16 17:19:19.000000 clean-alchemy-0.1.1/setup.py
```

### Comparing `clean-alchemy-0.1/LICENSE` & `clean-alchemy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clean-alchemy-0.1/PKG-INFO` & `clean-alchemy-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-alchemy
-Version: 0.1
+Version: 0.1.1
 Summary: A framework for implementing Clean Architecture using SQLAlchemy, with currently only support for FastAPI.
 Home-page: https://github.com/davidswords/clean-alchemy
 Author: David Swords
 Author-email: furuer_svette.0k@icloud.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clean-alchemy-0.1/README.md` & `clean-alchemy-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `clean-alchemy-0.1/src/clean_alchemy.egg-info/PKG-INFO` & `clean-alchemy-0.1.1/clean_alchemy/clean_alchemy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-alchemy
-Version: 0.1
+Version: 0.1.1
 Summary: A framework for implementing Clean Architecture using SQLAlchemy, with currently only support for FastAPI.
 Home-page: https://github.com/davidswords/clean-alchemy
 Author: David Swords
 Author-email: furuer_svette.0k@icloud.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clean-alchemy-0.1/src/clean_alchemy.egg-info/requires.txt` & `clean-alchemy-0.1.1/clean_alchemy/clean_alchemy.egg-info/requires.txt`

 * *Files identical despite different names*

