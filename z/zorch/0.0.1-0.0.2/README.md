# Comparing `tmp/zorch-0.0.1.tar.gz` & `tmp/zorch-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zorch-0.0.1.tar", last modified: Fri May 17 03:36:43 2024, max compression
+gzip compressed data, was "zorch-0.0.2.tar", last modified: Fri May 17 05:41:19 2024, max compression
```

## Comparing `zorch-0.0.1.tar` & `zorch-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 zwhy      (1000) zwhy      (1000)        0 2024-05-17 03:36:43.819152 zorch-0.0.1/
--rw-r--r--   0 zwhy      (1000) zwhy      (1000)      162 2024-05-17 03:36:43.819152 zorch-0.0.1/PKG-INFO
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)       38 2024-05-17 03:36:43.819152 zorch-0.0.1/setup.cfg
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)     1286 2024-05-17 03:36:31.000000 zorch-0.0.1/setup.py
-drwxrwxr-x   0 zwhy      (1000) zwhy      (1000)        0 2024-05-17 03:36:43.819152 zorch-0.0.1/zorch/
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)       23 2024-05-16 07:09:28.000000 zorch-0.0.1/zorch/__init__.py
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)        0 2024-05-16 07:24:14.000000 zorch-0.0.1/zorch/postprocess.py
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)      458 2024-05-16 09:58:45.000000 zorch-0.0.1/zorch/preprocess.py
-drwxrwxr-x   0 zwhy      (1000) zwhy      (1000)        0 2024-05-17 03:36:43.819152 zorch-0.0.1/zorch.egg-info/
--rw-r--r--   0 zwhy      (1000) zwhy      (1000)      162 2024-05-17 03:36:43.000000 zorch-0.0.1/zorch.egg-info/PKG-INFO
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)      183 2024-05-17 03:36:43.000000 zorch-0.0.1/zorch.egg-info/SOURCES.txt
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)        1 2024-05-17 03:36:43.000000 zorch-0.0.1/zorch.egg-info/dependency_links.txt
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)        6 2024-05-17 03:36:43.000000 zorch-0.0.1/zorch.egg-info/top_level.txt
+drwxrwxr-x   0 zwhy      (1000) zwhy      (1000)        0 2024-05-17 05:41:19.122623 zorch-0.0.2/
+-rw-r--r--   0 zwhy      (1000) zwhy      (1000)      162 2024-05-17 05:41:19.122623 zorch-0.0.2/PKG-INFO
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)       38 2024-05-17 05:41:19.122623 zorch-0.0.2/setup.cfg
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)     1503 2024-05-17 05:41:10.000000 zorch-0.0.2/setup.py
+drwxrwxr-x   0 zwhy      (1000) zwhy      (1000)        0 2024-05-17 05:41:19.122623 zorch-0.0.2/zorch/
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)       21 2024-05-17 05:39:34.000000 zorch-0.0.2/zorch/__init__.py
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)        0 2024-05-16 07:24:14.000000 zorch-0.0.2/zorch/postprocess.py
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)      458 2024-05-16 09:58:45.000000 zorch-0.0.2/zorch/preprocess.py
+drwxrwxr-x   0 zwhy      (1000) zwhy      (1000)        0 2024-05-17 05:41:19.122623 zorch-0.0.2/zorch.egg-info/
+-rw-r--r--   0 zwhy      (1000) zwhy      (1000)      162 2024-05-17 05:41:19.000000 zorch-0.0.2/zorch.egg-info/PKG-INFO
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)      183 2024-05-17 05:41:19.000000 zorch-0.0.2/zorch.egg-info/SOURCES.txt
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)        1 2024-05-17 05:41:19.000000 zorch-0.0.2/zorch.egg-info/dependency_links.txt
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)        6 2024-05-17 05:41:19.000000 zorch-0.0.2/zorch.egg-info/top_level.txt
```

