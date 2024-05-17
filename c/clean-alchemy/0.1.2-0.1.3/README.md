# Comparing `tmp/clean-alchemy-0.1.2.tar.gz` & `tmp/clean-alchemy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean-alchemy-0.1.2.tar", last modified: Fri May 17 07:49:01 2024, max compression
+gzip compressed data, was "clean-alchemy-0.1.3.tar", last modified: Fri May 17 08:01:46 2024, max compression
```

## Comparing `clean-alchemy-0.1.2.tar` & `clean-alchemy-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,20 @@
-drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-17 07:49:01.506151 clean-alchemy-0.1.2/
--rw-r--r--   0 swords     (501) staff       (20)    11357 2024-05-15 18:56:06.000000 clean-alchemy-0.1.2/LICENSE
--rw-r--r--   0 swords     (501) staff       (20)     1481 2024-05-17 07:49:01.505927 clean-alchemy-0.1.2/PKG-INFO
--rw-r--r--   0 swords     (501) staff       (20)      883 2024-05-15 18:56:06.000000 clean-alchemy-0.1.2/README.md
-drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-17 07:49:01.503852 clean-alchemy-0.1.2/clean_alchemy/
-drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-17 07:49:01.505729 clean-alchemy-0.1.2/clean_alchemy/clean_alchemy.egg-info/
--rw-r--r--   0 swords     (501) staff       (20)     1481 2024-05-17 07:49:01.000000 clean-alchemy-0.1.2/clean_alchemy/clean_alchemy.egg-info/PKG-INFO
--rw-r--r--   0 swords     (501) staff       (20)      280 2024-05-17 07:49:01.000000 clean-alchemy-0.1.2/clean_alchemy/clean_alchemy.egg-info/SOURCES.txt
--rw-r--r--   0 swords     (501) staff       (20)        1 2024-05-17 07:49:01.000000 clean-alchemy-0.1.2/clean_alchemy/clean_alchemy.egg-info/dependency_links.txt
--rw-r--r--   0 swords     (501) staff       (20)      516 2024-05-17 07:49:01.000000 clean-alchemy-0.1.2/clean_alchemy/clean_alchemy.egg-info/requires.txt
--rw-r--r--   0 swords     (501) staff       (20)        1 2024-05-17 07:49:01.000000 clean-alchemy-0.1.2/clean_alchemy/clean_alchemy.egg-info/top_level.txt
--rw-r--r--   0 swords     (501) staff       (20)       38 2024-05-17 07:49:01.506214 clean-alchemy-0.1.2/setup.cfg
--rw-r--r--   0 swords     (501) staff       (20)     1732 2024-05-17 07:48:56.000000 clean-alchemy-0.1.2/setup.py
+drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-17 08:01:46.593613 clean-alchemy-0.1.3/
+-rw-r--r--   0 swords     (501) staff       (20)    11357 2024-05-15 18:56:06.000000 clean-alchemy-0.1.3/LICENSE
+-rw-r--r--   0 swords     (501) staff       (20)     1481 2024-05-17 08:01:46.593486 clean-alchemy-0.1.3/PKG-INFO
+-rw-r--r--   0 swords     (501) staff       (20)      883 2024-05-15 18:56:06.000000 clean-alchemy-0.1.3/README.md
+drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-17 08:01:46.592666 clean-alchemy-0.1.3/clean_alchemy/
+-rw-r--r--   0 swords     (501) staff       (20)      195 2024-05-17 07:46:14.000000 clean-alchemy-0.1.3/clean_alchemy/__init__.py
+-rw-r--r--   0 swords     (501) staff       (20)      445 2024-05-15 20:09:20.000000 clean-alchemy-0.1.3/clean_alchemy/base.py
+-rw-r--r--   0 swords     (501) staff       (20)      782 2024-05-16 17:14:56.000000 clean-alchemy-0.1.3/clean_alchemy/base_dao.py
+-rw-r--r--   0 swords     (501) staff       (20)      500 2024-05-15 18:56:06.000000 clean-alchemy-0.1.3/clean_alchemy/base_ent.py
+-rw-r--r--   0 swords     (501) staff       (20)     3645 2024-05-16 17:18:08.000000 clean-alchemy-0.1.3/clean_alchemy/base_rpo.py
+-rw-r--r--   0 swords     (501) staff       (20)     2015 2024-05-15 20:12:10.000000 clean-alchemy-0.1.3/clean_alchemy/base_srv.py
+-rw-r--r--   0 swords     (501) staff       (20)      357 2024-05-15 18:56:06.000000 clean-alchemy-0.1.3/clean_alchemy/config.py
+drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-17 08:01:46.593303 clean-alchemy-0.1.3/clean_alchemy.egg-info/
+-rw-r--r--   0 swords     (501) staff       (20)     1481 2024-05-17 08:01:46.000000 clean-alchemy-0.1.3/clean_alchemy.egg-info/PKG-INFO
+-rw-r--r--   0 swords     (501) staff       (20)      386 2024-05-17 08:01:46.000000 clean-alchemy-0.1.3/clean_alchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 swords     (501) staff       (20)        1 2024-05-17 08:01:46.000000 clean-alchemy-0.1.3/clean_alchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 swords     (501) staff       (20)      516 2024-05-17 08:01:46.000000 clean-alchemy-0.1.3/clean_alchemy.egg-info/requires.txt
+-rw-r--r--   0 swords     (501) staff       (20)       14 2024-05-17 08:01:46.000000 clean-alchemy-0.1.3/clean_alchemy.egg-info/top_level.txt
+-rw-r--r--   0 swords     (501) staff       (20)       38 2024-05-17 08:01:46.593665 clean-alchemy-0.1.3/setup.cfg
+-rw-r--r--   0 swords     (501) staff       (20)     1669 2024-05-17 08:01:34.000000 clean-alchemy-0.1.3/setup.py
```

### Comparing `clean-alchemy-0.1.2/LICENSE` & `clean-alchemy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clean-alchemy-0.1.2/PKG-INFO` & `clean-alchemy-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-alchemy
-Version: 0.1.2
+Version: 0.1.3
 Summary: A framework for implementing Clean Architecture using SQLAlchemy, with currently only support for FastAPI.
 Home-page: https://github.com/davidswords/clean-alchemy
 Author: David Swords
 Author-email: furuer_svette.0k@icloud.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clean-alchemy-0.1.2/README.md` & `clean-alchemy-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `clean-alchemy-0.1.2/clean_alchemy/clean_alchemy.egg-info/PKG-INFO` & `clean-alchemy-0.1.3/clean_alchemy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-alchemy
-Version: 0.1.2
+Version: 0.1.3
 Summary: A framework for implementing Clean Architecture using SQLAlchemy, with currently only support for FastAPI.
 Home-page: https://github.com/davidswords/clean-alchemy
 Author: David Swords
 Author-email: furuer_svette.0k@icloud.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clean-alchemy-0.1.2/clean_alchemy/clean_alchemy.egg-info/requires.txt` & `clean-alchemy-0.1.3/clean_alchemy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `clean-alchemy-0.1.2/setup.py` & `clean-alchemy-0.1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name="clean-alchemy",
-    version="0.1.2",
-    package_dir={"": "clean_alchemy"},
-    packages=find_packages(where="clean_alchemy", exclude=["tests*", "build*"]),
+    version="0.1.3",
+    packages=find_packages(exclude=["tests*", "build*"]),
     install_requires=[
         "annotated-types==0.6.0",
         "black==24.4.2",
         "click==8.1.7",
         "exceptiongroup==1.2.1",
         "factory-boy==3.3.0",
         "Faker==25.0.1",
@@ -48,8 +47,8 @@
     url="https://github.com/davidswords/clean-alchemy",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9.6",
-)
+)
```

