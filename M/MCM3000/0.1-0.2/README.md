# Comparing `tmp/MCM3000-0.1.tar.gz` & `tmp/MCM3000-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MCM3000-0.1.tar", last modified: Thu May 16 23:58:28 2024, max compression
+gzip compressed data, was "dist/MCM3000-0.2.tar", last modified: Fri May 17 19:59:26 2024, max compression
```

## Comparing `MCM3000-0.1.tar` & `MCM3000-0.2.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 23:58:28.000000 MCM3000-0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 23:58:28.000000 MCM3000-0.1/MCM3000.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-16 23:58:28.000000 MCM3000-0.1/MCM3000.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-16 23:58:28.000000 MCM3000-0.1/MCM3000.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 23:58:28.000000 MCM3000-0.1/MCM3000.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 23:58:28.000000 MCM3000-0.1/MCM3000.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-16 23:58:28.000000 MCM3000-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 23:58:13.000000 MCM3000-0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 23:58:28.000000 MCM3000-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-16 23:58:13.000000 MCM3000-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:59:26.000000 MCM3000-0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:59:26.000000 MCM3000-0.2/MCM3000/
+-rw-r--r--   0 runner    (1001) docker     (127)    12755 2024-05-17 19:59:15.000000 MCM3000-0.2/MCM3000/MCM3000.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-17 19:59:15.000000 MCM3000-0.2/MCM3000/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:59:26.000000 MCM3000-0.2/MCM3000.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-17 19:59:26.000000 MCM3000-0.2/MCM3000.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-17 19:59:26.000000 MCM3000-0.2/MCM3000.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 19:59:26.000000 MCM3000-0.2/MCM3000.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-17 19:59:26.000000 MCM3000-0.2/MCM3000.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-17 19:59:26.000000 MCM3000-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-17 19:59:15.000000 MCM3000-0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 19:59:26.000000 MCM3000-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-17 19:59:15.000000 MCM3000-0.2/setup.py
```

