# Comparing `tmp/zorch-0.0.3.tar.gz` & `tmp/zorch-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zorch-0.0.3.tar", last modified: Fri May 17 05:58:28 2024, max compression
+gzip compressed data, was "zorch-0.0.4.tar", last modified: Fri May 17 06:02:44 2024, max compression
```

## Comparing `zorch-0.0.3.tar` & `zorch-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 zwhy      (1000) zwhy      (1000)        0 2024-05-17 05:58:28.647900 zorch-0.0.3/
--rw-r--r--   0 zwhy      (1000) zwhy      (1000)      162 2024-05-17 05:58:28.647900 zorch-0.0.3/PKG-INFO
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)       38 2024-05-17 05:58:28.647900 zorch-0.0.3/setup.cfg
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)     1416 2024-05-17 05:58:06.000000 zorch-0.0.3/setup.py
-drwxrwxr-x   0 zwhy      (1000) zwhy      (1000)        0 2024-05-17 05:58:28.647900 zorch-0.0.3/zorch/
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)       22 2024-05-17 05:58:28.000000 zorch-0.0.3/zorch/__init__.py
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)        0 2024-05-16 07:24:14.000000 zorch-0.0.3/zorch/postprocess.py
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)      458 2024-05-16 09:58:45.000000 zorch-0.0.3/zorch/preprocess.py
-drwxrwxr-x   0 zwhy      (1000) zwhy      (1000)        0 2024-05-17 05:58:28.647900 zorch-0.0.3/zorch.egg-info/
--rw-r--r--   0 zwhy      (1000) zwhy      (1000)      162 2024-05-17 05:58:28.000000 zorch-0.0.3/zorch.egg-info/PKG-INFO
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)      183 2024-05-17 05:58:28.000000 zorch-0.0.3/zorch.egg-info/SOURCES.txt
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)        1 2024-05-17 05:58:28.000000 zorch-0.0.3/zorch.egg-info/dependency_links.txt
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)        6 2024-05-17 05:58:28.000000 zorch-0.0.3/zorch.egg-info/top_level.txt
+drwxrwxr-x   0 zwhy      (1000) zwhy      (1000)        0 2024-05-17 06:02:44.524513 zorch-0.0.4/
+-rw-r--r--   0 zwhy      (1000) zwhy      (1000)      162 2024-05-17 06:02:44.524513 zorch-0.0.4/PKG-INFO
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)       38 2024-05-17 06:02:44.524513 zorch-0.0.4/setup.cfg
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)     1416 2024-05-17 05:58:06.000000 zorch-0.0.4/setup.py
+drwxrwxr-x   0 zwhy      (1000) zwhy      (1000)        0 2024-05-17 06:02:44.524513 zorch-0.0.4/zorch/
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)       22 2024-05-17 06:02:44.000000 zorch-0.0.4/zorch/__init__.py
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)        0 2024-05-16 07:24:14.000000 zorch-0.0.4/zorch/postprocess.py
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)      458 2024-05-16 09:58:45.000000 zorch-0.0.4/zorch/preprocess.py
+drwxrwxr-x   0 zwhy      (1000) zwhy      (1000)        0 2024-05-17 06:02:44.524513 zorch-0.0.4/zorch.egg-info/
+-rw-r--r--   0 zwhy      (1000) zwhy      (1000)      162 2024-05-17 06:02:44.000000 zorch-0.0.4/zorch.egg-info/PKG-INFO
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)      183 2024-05-17 06:02:44.000000 zorch-0.0.4/zorch.egg-info/SOURCES.txt
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)        1 2024-05-17 06:02:44.000000 zorch-0.0.4/zorch.egg-info/dependency_links.txt
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)        6 2024-05-17 06:02:44.000000 zorch-0.0.4/zorch.egg-info/top_level.txt
```

### Comparing `zorch-0.0.3/setup.py` & `zorch-0.0.4/setup.py`

 * *Files identical despite different names*

