# Comparing `tmp/aochagavia_example_lib-0.1.0.tar.gz` & `tmp/aochagavia_example_lib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aochagavia_example_lib-0.1.0.tar", last modified: Fri May 17 08:29:18 2024, max compression
+gzip compressed data, was "aochagavia_example_lib-0.1.1.tar", last modified: Fri May 17 08:45:14 2024, max compression
```

## Comparing `aochagavia_example_lib-0.1.0.tar` & `aochagavia_example_lib-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxr-xr-x   0 aochagavia  (1000) aochagavia  (1000)        0 2024-05-17 08:29:18.628404 aochagavia_example_lib-0.1.0/
--rw-r--r--   0 aochagavia  (1000) aochagavia  (1000)      374 2024-05-17 08:29:18.628404 aochagavia_example_lib-0.1.0/PKG-INFO
-drwxr-xr-x   0 aochagavia  (1000) aochagavia  (1000)        0 2024-05-17 08:29:18.628404 aochagavia_example_lib-0.1.0/aochagavia_example_lib/
-drwxr-xr-x   0 aochagavia  (1000) aochagavia  (1000)        0 2024-05-17 08:29:18.628404 aochagavia_example_lib-0.1.0/aochagavia_example_lib/aochagavia_example_lib.egg-info/
--rw-r--r--   0 aochagavia  (1000) aochagavia  (1000)      374 2024-05-17 08:29:18.000000 aochagavia_example_lib-0.1.0/aochagavia_example_lib/aochagavia_example_lib.egg-info/PKG-INFO
--rw-r--r--   0 aochagavia  (1000) aochagavia  (1000)      300 2024-05-17 08:29:18.000000 aochagavia_example_lib-0.1.0/aochagavia_example_lib/aochagavia_example_lib.egg-info/SOURCES.txt
--rw-r--r--   0 aochagavia  (1000) aochagavia  (1000)        1 2024-05-17 08:29:18.000000 aochagavia_example_lib-0.1.0/aochagavia_example_lib/aochagavia_example_lib.egg-info/dependency_links.txt
--rw-r--r--   0 aochagavia  (1000) aochagavia  (1000)        1 2024-05-17 08:29:18.000000 aochagavia_example_lib-0.1.0/aochagavia_example_lib/aochagavia_example_lib.egg-info/top_level.txt
--rw-r--r--   0 aochagavia  (1000) aochagavia  (1000)       90 2024-05-17 08:27:19.000000 aochagavia_example_lib-0.1.0/pyproject.toml
--rw-r--r--   0 aochagavia  (1000) aochagavia  (1000)      519 2024-05-17 08:29:18.628404 aochagavia_example_lib-0.1.0/setup.cfg
+drwxr-xr-x   0 aochagavia  (1000) aochagavia  (1000)        0 2024-05-17 08:45:14.566455 aochagavia_example_lib-0.1.1/
+-rw-r--r--   0 aochagavia  (1000) aochagavia  (1000)      351 2024-05-17 08:45:14.566455 aochagavia_example_lib-0.1.1/PKG-INFO
+drwxr-xr-x   0 aochagavia  (1000) aochagavia  (1000)        0 2024-05-17 08:45:14.566455 aochagavia_example_lib-0.1.1/aochagavia_example_lib/
+-rw-r--r--   0 aochagavia  (1000) aochagavia  (1000)        0 2024-05-17 08:23:59.000000 aochagavia_example_lib-0.1.1/aochagavia_example_lib/__init__.py
+drwxr-xr-x   0 aochagavia  (1000) aochagavia  (1000)        0 2024-05-17 08:45:14.566455 aochagavia_example_lib-0.1.1/aochagavia_example_lib.egg-info/
+-rw-r--r--   0 aochagavia  (1000) aochagavia  (1000)      351 2024-05-17 08:45:14.000000 aochagavia_example_lib-0.1.1/aochagavia_example_lib.egg-info/PKG-INFO
+-rw-r--r--   0 aochagavia  (1000) aochagavia  (1000)      243 2024-05-17 08:45:14.000000 aochagavia_example_lib-0.1.1/aochagavia_example_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 aochagavia  (1000) aochagavia  (1000)        1 2024-05-17 08:45:14.000000 aochagavia_example_lib-0.1.1/aochagavia_example_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 aochagavia  (1000) aochagavia  (1000)       23 2024-05-17 08:45:14.000000 aochagavia_example_lib-0.1.1/aochagavia_example_lib.egg-info/top_level.txt
+-rw-r--r--   0 aochagavia  (1000) aochagavia  (1000)       90 2024-05-17 08:27:19.000000 aochagavia_example_lib-0.1.1/pyproject.toml
+-rw-r--r--   0 aochagavia  (1000) aochagavia  (1000)      439 2024-05-17 08:45:14.566455 aochagavia_example_lib-0.1.1/setup.cfg
```

