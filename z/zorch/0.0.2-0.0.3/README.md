# Comparing `tmp/zorch-0.0.2.tar.gz` & `tmp/zorch-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zorch-0.0.2.tar", last modified: Fri May 17 05:41:19 2024, max compression
+gzip compressed data, was "zorch-0.0.3.tar", last modified: Fri May 17 05:58:28 2024, max compression
```

## Comparing `zorch-0.0.2.tar` & `zorch-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 zwhy      (1000) zwhy      (1000)        0 2024-05-17 05:41:19.122623 zorch-0.0.2/
--rw-r--r--   0 zwhy      (1000) zwhy      (1000)      162 2024-05-17 05:41:19.122623 zorch-0.0.2/PKG-INFO
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)       38 2024-05-17 05:41:19.122623 zorch-0.0.2/setup.cfg
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)     1503 2024-05-17 05:41:10.000000 zorch-0.0.2/setup.py
-drwxrwxr-x   0 zwhy      (1000) zwhy      (1000)        0 2024-05-17 05:41:19.122623 zorch-0.0.2/zorch/
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)       21 2024-05-17 05:39:34.000000 zorch-0.0.2/zorch/__init__.py
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)        0 2024-05-16 07:24:14.000000 zorch-0.0.2/zorch/postprocess.py
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)      458 2024-05-16 09:58:45.000000 zorch-0.0.2/zorch/preprocess.py
-drwxrwxr-x   0 zwhy      (1000) zwhy      (1000)        0 2024-05-17 05:41:19.122623 zorch-0.0.2/zorch.egg-info/
--rw-r--r--   0 zwhy      (1000) zwhy      (1000)      162 2024-05-17 05:41:19.000000 zorch-0.0.2/zorch.egg-info/PKG-INFO
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)      183 2024-05-17 05:41:19.000000 zorch-0.0.2/zorch.egg-info/SOURCES.txt
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)        1 2024-05-17 05:41:19.000000 zorch-0.0.2/zorch.egg-info/dependency_links.txt
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)        6 2024-05-17 05:41:19.000000 zorch-0.0.2/zorch.egg-info/top_level.txt
+drwxrwxr-x   0 zwhy      (1000) zwhy      (1000)        0 2024-05-17 05:58:28.647900 zorch-0.0.3/
+-rw-r--r--   0 zwhy      (1000) zwhy      (1000)      162 2024-05-17 05:58:28.647900 zorch-0.0.3/PKG-INFO
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)       38 2024-05-17 05:58:28.647900 zorch-0.0.3/setup.cfg
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)     1416 2024-05-17 05:58:06.000000 zorch-0.0.3/setup.py
+drwxrwxr-x   0 zwhy      (1000) zwhy      (1000)        0 2024-05-17 05:58:28.647900 zorch-0.0.3/zorch/
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)       22 2024-05-17 05:58:28.000000 zorch-0.0.3/zorch/__init__.py
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)        0 2024-05-16 07:24:14.000000 zorch-0.0.3/zorch/postprocess.py
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)      458 2024-05-16 09:58:45.000000 zorch-0.0.3/zorch/preprocess.py
+drwxrwxr-x   0 zwhy      (1000) zwhy      (1000)        0 2024-05-17 05:58:28.647900 zorch-0.0.3/zorch.egg-info/
+-rw-r--r--   0 zwhy      (1000) zwhy      (1000)      162 2024-05-17 05:58:28.000000 zorch-0.0.3/zorch.egg-info/PKG-INFO
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)      183 2024-05-17 05:58:28.000000 zorch-0.0.3/zorch.egg-info/SOURCES.txt
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)        1 2024-05-17 05:58:28.000000 zorch-0.0.3/zorch.egg-info/dependency_links.txt
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)        6 2024-05-17 05:58:28.000000 zorch-0.0.3/zorch.egg-info/top_level.txt
```

