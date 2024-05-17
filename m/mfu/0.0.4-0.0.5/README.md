# Comparing `tmp/mfu-0.0.4.tar.gz` & `tmp/mfu-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfu-0.0.4.tar", last modified: Mon Nov 21 08:54:10 2022, max compression
+gzip compressed data, was "mfu-0.0.5.tar", last modified: Mon Nov 21 09:19:56 2022, max compression
```

## Comparing `mfu-0.0.4.tar` & `mfu-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-11-21 08:54:10.925367 mfu-0.0.4/
--rw-rw-r--   0 michael   (1000) michael   (1000)      197 2022-11-21 08:54:10.925367 mfu-0.0.4/PKG-INFO
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-11-21 08:54:10.925367 mfu-0.0.4/mfu/
--rw-rw-r--   0 michael   (1000) michael   (1000)        0 2022-11-21 04:24:21.000000 mfu-0.0.4/mfu/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)       61 2022-11-21 08:51:54.000000 mfu-0.0.4/mfu/__main__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      194 2022-11-21 04:24:21.000000 mfu-0.0.4/mfu/main.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-11-21 08:54:10.925367 mfu-0.0.4/mfu/scripts/
--rw-rw-r--   0 michael   (1000) michael   (1000)        0 2022-11-21 04:24:21.000000 mfu-0.0.4/mfu/scripts/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3651 2022-11-21 08:51:54.000000 mfu-0.0.4/mfu/scripts/doctor.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3693 2022-11-21 08:51:54.000000 mfu-0.0.4/mfu/scripts/sync.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      756 2022-11-21 04:24:21.000000 mfu-0.0.4/mfu/utils.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-11-21 08:54:10.925367 mfu-0.0.4/mfu.egg-info/
--rw-rw-r--   0 michael   (1000) michael   (1000)      197 2022-11-21 08:54:10.000000 mfu-0.0.4/mfu.egg-info/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)      305 2022-11-21 08:54:10.000000 mfu-0.0.4/mfu.egg-info/SOURCES.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2022-11-21 08:54:10.000000 mfu-0.0.4/mfu.egg-info/dependency_links.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       38 2022-11-21 08:54:10.000000 mfu-0.0.4/mfu.egg-info/entry_points.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       66 2022-11-21 08:54:10.000000 mfu-0.0.4/mfu.egg-info/requires.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        4 2022-11-21 08:54:10.000000 mfu-0.0.4/mfu.egg-info/top_level.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       79 2022-11-21 08:54:10.925367 mfu-0.0.4/setup.cfg
--rw-rw-r--   0 michael   (1000) michael   (1000)      508 2022-11-21 08:51:54.000000 mfu-0.0.4/setup.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-11-21 09:19:56.104891 mfu-0.0.5/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      514 2022-11-21 09:19:56.104891 mfu-0.0.5/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)      321 2022-11-21 08:51:54.000000 mfu-0.0.5/README.md
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-11-21 09:19:56.104891 mfu-0.0.5/mfu/
+-rw-rw-r--   0 michael   (1000) michael   (1000)        0 2022-11-21 04:24:21.000000 mfu-0.0.5/mfu/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)       61 2022-11-21 08:51:54.000000 mfu-0.0.5/mfu/__main__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      194 2022-11-21 04:24:21.000000 mfu-0.0.5/mfu/main.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-11-21 09:19:56.104891 mfu-0.0.5/mfu/scripts/
+-rw-rw-r--   0 michael   (1000) michael   (1000)        0 2022-11-21 04:24:21.000000 mfu-0.0.5/mfu/scripts/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3651 2022-11-21 08:51:54.000000 mfu-0.0.5/mfu/scripts/doctor.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3693 2022-11-21 08:51:54.000000 mfu-0.0.5/mfu/scripts/sync.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      756 2022-11-21 04:24:21.000000 mfu-0.0.5/mfu/utils.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-11-21 09:19:56.104891 mfu-0.0.5/mfu.egg-info/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      514 2022-11-21 09:19:56.000000 mfu-0.0.5/mfu.egg-info/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)      320 2022-11-21 09:19:56.000000 mfu-0.0.5/mfu.egg-info/SOURCES.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2022-11-21 09:19:56.000000 mfu-0.0.5/mfu.egg-info/dependency_links.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       37 2022-11-21 09:19:56.000000 mfu-0.0.5/mfu.egg-info/entry_points.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       66 2022-11-21 09:19:56.000000 mfu-0.0.5/mfu.egg-info/requires.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        4 2022-11-21 09:19:56.000000 mfu-0.0.5/mfu.egg-info/top_level.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)      460 2022-11-21 09:15:37.000000 mfu-0.0.5/pyproject.toml
+-rw-rw-r--   0 michael   (1000) michael   (1000)       38 2022-11-21 09:19:56.104891 mfu-0.0.5/setup.cfg
+-rw-rw-r--   0 michael   (1000) michael   (1000)       68 2022-11-21 09:07:09.000000 mfu-0.0.5/setup.py
```

### Comparing `mfu-0.0.4/mfu/scripts/doctor.py` & `mfu-0.0.5/mfu/scripts/doctor.py`

 * *Files identical despite different names*

### Comparing `mfu-0.0.4/mfu/scripts/sync.py` & `mfu-0.0.5/mfu/scripts/sync.py`

 * *Files identical despite different names*

### Comparing `mfu-0.0.4/mfu/utils.py` & `mfu-0.0.5/mfu/utils.py`

 * *Files identical despite different names*

