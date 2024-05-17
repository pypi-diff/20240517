# Comparing `tmp/unimore_lab_cicd_singh-0.2.tar.gz` & `tmp/unimore_lab_cicd_singh-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unimore_lab_cicd_singh-0.2.tar", last modified: Fri May 10 08:42:13 2024, max compression
+gzip compressed data, was "unimore_lab_cicd_singh-0.4.tar", last modified: Fri May 17 12:41:06 2024, max compression
```

## Comparing `unimore_lab_cicd_singh-0.2.tar` & `unimore_lab_cicd_singh-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:42:13.702496 unimore_lab_cicd_singh-0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-10 08:42:13.702496 unimore_lab_cicd_singh-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-10 08:42:09.000000 unimore_lab_cicd_singh-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:42:13.698496 unimore_lab_cicd_singh-0.2/my_math/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-10 08:42:09.000000 unimore_lab_cicd_singh-0.2/my_math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-10 08:42:09.000000 unimore_lab_cicd_singh-0.2/my_math/unimore_math.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 08:42:13.702496 unimore_lab_cicd_singh-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-10 08:42:09.000000 unimore_lab_cicd_singh-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:42:13.698496 unimore_lab_cicd_singh-0.2/unimore_lab_cicd_singh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-10 08:42:13.000000 unimore_lab_cicd_singh-0.2/unimore_lab_cicd_singh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-10 08:42:13.000000 unimore_lab_cicd_singh-0.2/unimore_lab_cicd_singh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:42:13.000000 unimore_lab_cicd_singh-0.2/unimore_lab_cicd_singh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 08:42:13.000000 unimore_lab_cicd_singh-0.2/unimore_lab_cicd_singh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 08:42:13.000000 unimore_lab_cicd_singh-0.2/unimore_lab_cicd_singh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:41:06.452464 unimore_lab_cicd_singh-0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-17 12:41:06.452464 unimore_lab_cicd_singh-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-17 12:41:01.000000 unimore_lab_cicd_singh-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:41:06.448464 unimore_lab_cicd_singh-0.4/my_math/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-17 12:41:01.000000 unimore_lab_cicd_singh-0.4/my_math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-17 12:41:01.000000 unimore_lab_cicd_singh-0.4/my_math/unimore_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 12:41:06.452464 unimore_lab_cicd_singh-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-17 12:41:01.000000 unimore_lab_cicd_singh-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:41:06.452464 unimore_lab_cicd_singh-0.4/unimore_lab_cicd_singh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-17 12:41:06.000000 unimore_lab_cicd_singh-0.4/unimore_lab_cicd_singh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-17 12:41:06.000000 unimore_lab_cicd_singh-0.4/unimore_lab_cicd_singh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 12:41:06.000000 unimore_lab_cicd_singh-0.4/unimore_lab_cicd_singh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 12:41:06.000000 unimore_lab_cicd_singh-0.4/unimore_lab_cicd_singh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-17 12:41:06.000000 unimore_lab_cicd_singh-0.4/unimore_lab_cicd_singh.egg-info/top_level.txt
```

