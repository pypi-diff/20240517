# Comparing `tmp/testpackage1290-0.0.1.tar.gz` & `tmp/testpackage1290-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testpackage1290-0.0.1.tar", last modified: Fri May 17 13:07:13 2024, max compression
+gzip compressed data, was "testpackage1290-0.0.2.tar", last modified: Fri May 17 17:30:12 2024, max compression
```

## Comparing `testpackage1290-0.0.1.tar` & `testpackage1290-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxr-xr-x   0 stjansen   (503) staff       (20)        0 2024-05-17 13:07:13.025434 testpackage1290-0.0.1/
--rw-r--r--   0 stjansen   (503) staff       (20)      531 2024-05-17 13:07:13.025279 testpackage1290-0.0.1/PKG-INFO
--rw-r--r--   0 stjansen   (503) staff       (20)       38 2024-05-17 13:07:13.025505 testpackage1290-0.0.1/setup.cfg
--rw-r--r--   0 stjansen   (503) staff       (20)      985 2024-05-17 13:06:26.000000 testpackage1290-0.0.1/setup.py
-drwxr-xr-x   0 stjansen   (503) staff       (20)        0 2024-05-17 13:07:13.021347 testpackage1290-0.0.1/testpackage1290/
--rw-r--r--   0 stjansen   (503) staff       (20)       49 2024-05-17 12:57:19.000000 testpackage1290-0.0.1/testpackage1290/__init__.py
--rw-r--r--   0 stjansen   (503) staff       (20)        0 2024-05-17 12:55:23.000000 testpackage1290-0.0.1/testpackage1290/add.py
-drwxr-xr-x   0 stjansen   (503) staff       (20)        0 2024-05-17 13:07:13.025063 testpackage1290-0.0.1/testpackage1290/extras/
--rw-r--r--   0 stjansen   (503) staff       (20)       55 2024-05-17 12:58:29.000000 testpackage1290-0.0.1/testpackage1290/extras/__init__.py
--rw-r--r--   0 stjansen   (503) staff       (20)        0 2024-05-17 12:55:44.000000 testpackage1290-0.0.1/testpackage1290/extras/divide.py
--rw-r--r--   0 stjansen   (503) staff       (20)        0 2024-05-17 12:55:39.000000 testpackage1290-0.0.1/testpackage1290/extras/multiply.py
--rw-r--r--   0 stjansen   (503) staff       (20)        0 2024-05-17 12:55:30.000000 testpackage1290-0.0.1/testpackage1290/subtract.py
-drwxr-xr-x   0 stjansen   (503) staff       (20)        0 2024-05-17 13:07:13.023921 testpackage1290-0.0.1/testpackage1290.egg-info/
--rw-r--r--   0 stjansen   (503) staff       (20)      531 2024-05-17 13:07:12.000000 testpackage1290-0.0.1/testpackage1290.egg-info/PKG-INFO
--rw-r--r--   0 stjansen   (503) staff       (20)      346 2024-05-17 13:07:13.000000 testpackage1290-0.0.1/testpackage1290.egg-info/SOURCES.txt
--rw-r--r--   0 stjansen   (503) staff       (20)        1 2024-05-17 13:07:12.000000 testpackage1290-0.0.1/testpackage1290.egg-info/dependency_links.txt
--rw-r--r--   0 stjansen   (503) staff       (20)       16 2024-05-17 13:07:12.000000 testpackage1290-0.0.1/testpackage1290.egg-info/top_level.txt
+drwxr-xr-x   0 stjansen   (503) staff       (20)        0 2024-05-17 17:30:12.174663 testpackage1290-0.0.2/
+-rw-r--r--   0 stjansen   (503) staff       (20)     1070 2024-05-17 16:30:06.000000 testpackage1290-0.0.2/LICENSE
+-rw-r--r--   0 stjansen   (503) staff       (20)       17 2024-05-17 16:35:15.000000 testpackage1290-0.0.2/MANIFEST.in
+-rw-r--r--   0 stjansen   (503) staff       (20)     1373 2024-05-17 17:30:12.174055 testpackage1290-0.0.2/PKG-INFO
+-rw-r--r--   0 stjansen   (503) staff       (20)      918 2024-05-17 17:27:02.000000 testpackage1290-0.0.2/README.md
+-rw-r--r--   0 stjansen   (503) staff       (20)       38 2024-05-17 17:30:12.174851 testpackage1290-0.0.2/setup.cfg
+-rw-r--r--   0 stjansen   (503) staff       (20)      714 2024-05-17 16:35:15.000000 testpackage1290-0.0.2/setup.py
+drwxr-xr-x   0 stjansen   (503) staff       (20)        0 2024-05-17 17:30:12.168526 testpackage1290-0.0.2/testpackage1290/
+-rw-r--r--   0 stjansen   (503) staff       (20)       34 2024-05-17 16:35:15.000000 testpackage1290-0.0.2/testpackage1290/__init__.py
+-rw-r--r--   0 stjansen   (503) staff       (20)      151 2024-05-17 16:35:15.000000 testpackage1290-0.0.2/testpackage1290/math.py
+drwxr-xr-x   0 stjansen   (503) staff       (20)        0 2024-05-17 17:30:12.172783 testpackage1290-0.0.2/testpackage1290.egg-info/
+-rw-r--r--   0 stjansen   (503) staff       (20)     1373 2024-05-17 17:30:12.000000 testpackage1290-0.0.2/testpackage1290.egg-info/PKG-INFO
+-rw-r--r--   0 stjansen   (503) staff       (20)      246 2024-05-17 17:30:12.000000 testpackage1290-0.0.2/testpackage1290.egg-info/SOURCES.txt
+-rw-r--r--   0 stjansen   (503) staff       (20)        1 2024-05-17 17:30:12.000000 testpackage1290-0.0.2/testpackage1290.egg-info/dependency_links.txt
+-rw-r--r--   0 stjansen   (503) staff       (20)       16 2024-05-17 17:30:12.000000 testpackage1290-0.0.2/testpackage1290.egg-info/top_level.txt
```

