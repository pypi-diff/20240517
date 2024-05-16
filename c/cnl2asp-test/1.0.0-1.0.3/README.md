# Comparing `tmp/cnl2asp_test-1.0.0.tar.gz` & `tmp/cnl2asp_test-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnl2asp_test-1.0.0.tar", last modified: Thu May 16 21:45:33 2024, max compression
+gzip compressed data, was "cnl2asp_test-1.0.3.tar", last modified: Thu May 16 22:00:00 2024, max compression
```

## Comparing `cnl2asp_test-1.0.0.tar` & `cnl2asp_test-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:33.184359 cnl2asp_test-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-16 21:45:33.184359 cnl2asp_test-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 21:45:22.000000 cnl2asp_test-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 21:45:33.184359 cnl2asp_test-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-16 21:45:22.000000 cnl2asp_test-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:33.180359 cnl2asp_test-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:33.184359 cnl2asp_test-1.0.0/src/cnl2asp_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-16 21:45:33.000000 cnl2asp_test-1.0.0/src/cnl2asp_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-16 21:45:33.000000 cnl2asp_test-1.0.0/src/cnl2asp_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 21:45:33.000000 cnl2asp_test-1.0.0/src/cnl2asp_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 21:45:33.000000 cnl2asp_test-1.0.0/src/cnl2asp_test.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 21:45:33.000000 cnl2asp_test-1.0.0/src/cnl2asp_test.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:33.184359 cnl2asp_test-1.0.0/src/printer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:45:22.000000 cnl2asp_test-1.0.0/src/printer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-16 21:45:22.000000 cnl2asp_test-1.0.0/src/printer/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:00:00.606716 cnl2asp_test-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-16 22:00:00.606716 cnl2asp_test-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 21:59:56.000000 cnl2asp_test-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 22:00:00.606716 cnl2asp_test-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-16 21:59:56.000000 cnl2asp_test-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:00:00.606716 cnl2asp_test-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:00:00.606716 cnl2asp_test-1.0.3/src/cnl2asp_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-16 22:00:00.000000 cnl2asp_test-1.0.3/src/cnl2asp_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-16 22:00:00.000000 cnl2asp_test-1.0.3/src/cnl2asp_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 22:00:00.000000 cnl2asp_test-1.0.3/src/cnl2asp_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 22:00:00.000000 cnl2asp_test-1.0.3/src/cnl2asp_test.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 22:00:00.000000 cnl2asp_test-1.0.3/src/cnl2asp_test.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:00:00.606716 cnl2asp_test-1.0.3/src/printer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:59:56.000000 cnl2asp_test-1.0.3/src/printer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 21:59:56.000000 cnl2asp_test-1.0.3/src/printer/main.py
```

### Comparing `cnl2asp_test-1.0.0/setup.py` & `cnl2asp_test-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cnl2asp-test',
-    version='1.0.0',
+    version='1.0.3',
     description='Hello',
     long_description='World',
     url='https://github.com/simocaruso/test',
     license='Apache License',
     author='Simone Caruso',
     author_email='simone.caruso@edu.unige.it',
     maintainer='Simone Caruso',
```

