# Comparing `tmp/neverlib-0.0.1.tar.gz` & `tmp/neverlib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neverlib-0.0.1.tar", last modified: Fri May 17 07:46:09 2024, max compression
+gzip compressed data, was "neverlib-0.0.2.tar", last modified: Fri May 17 08:54:28 2024, max compression
```

## Comparing `neverlib-0.0.1.tar` & `neverlib-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 07:46:09.523345 neverlib-0.0.1/
--rw-rw-rw-   0        0        0      214 2024-05-17 07:46:09.521348 neverlib-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-17 07:46:09.519354 neverlib-0.0.1/neverlib.egg-info/
--rw-rw-rw-   0        0        0      214 2024-05-17 07:46:09.000000 neverlib-0.0.1/neverlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      136 2024-05-17 07:46:09.000000 neverlib-0.0.1/neverlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 07:46:09.000000 neverlib-0.0.1/neverlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 07:46:09.000000 neverlib-0.0.1/neverlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 07:46:09.523345 neverlib-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      669 2024-05-17 07:38:49.000000 neverlib-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:54:28.898128 neverlib-0.0.2/
+-rw-rw-rw-   0        0        0        0 2024-05-17 08:30:45.000000 neverlib-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      395 2024-05-17 08:54:28.897131 neverlib-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-17 08:30:32.000000 neverlib-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 08:54:28.890149 neverlib-0.0.2/neverlib.egg-info/
+-rw-rw-rw-   0        0        0      395 2024-05-17 08:54:28.000000 neverlib-0.0.2/neverlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2024-05-17 08:54:28.000000 neverlib-0.0.2/neverlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 08:54:28.000000 neverlib-0.0.2/neverlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-17 08:54:28.000000 neverlib-0.0.2/neverlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 08:54:28.898128 neverlib-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      838 2024-05-17 08:54:18.000000 neverlib-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:54:28.894139 neverlib-0.0.2/utils/
+-rw-rw-rw-   0        0        0       83 2024-05-17 08:48:24.000000 neverlib-0.0.2/utils/__init__.py
+-rw-rw-rw-   0        0        0     5087 2024-02-05 09:38:47.000000 neverlib-0.0.2/utils/utils.py
```

