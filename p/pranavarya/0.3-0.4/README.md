# Comparing `tmp/pranavarya-0.3.tar.gz` & `tmp/pranavarya-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pranavarya-0.3.tar", last modified: Thu May 16 22:15:52 2024, max compression
+gzip compressed data, was "pranavarya-0.4.tar", last modified: Thu May 16 22:29:37 2024, max compression
```

## Comparing `pranavarya-0.3.tar` & `pranavarya-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 22:15:52.805029 pranavarya-0.3/
--rw-rw-rw-   0        0        0       76 2024-05-16 22:15:52.804031 pranavarya-0.3/PKG-INFO
--rw-rw-rw-   0        0        0       15 2024-05-16 20:28:55.000000 pranavarya-0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 22:15:52.786814 pranavarya-0.3/pranavarya/
--rw-rw-rw-   0        0        0       40 2024-05-16 20:22:26.000000 pranavarya-0.3/pranavarya/__init__.py
--rw-rw-rw-   0        0        0       69 2024-05-16 20:21:56.000000 pranavarya-0.3/pranavarya/main.py
-drwxrwxrwx   0        0        0        0 2024-05-16 22:15:52.803053 pranavarya-0.3/pranavarya.egg-info/
--rw-rw-rw-   0        0        0       76 2024-05-16 22:15:52.000000 pranavarya-0.3/pranavarya.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2024-05-16 22:15:52.000000 pranavarya-0.3/pranavarya.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 22:15:52.000000 pranavarya-0.3/pranavarya.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-05-16 22:15:52.000000 pranavarya-0.3/pranavarya.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2024-05-16 22:15:52.000000 pranavarya-0.3/pranavarya.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 22:15:52.805029 pranavarya-0.3/setup.cfg
--rw-rw-rw-   0        0        0      347 2024-05-16 22:15:47.000000 pranavarya-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 22:29:37.207179 pranavarya-0.4/
+-rw-rw-rw-   0        0        0       76 2024-05-16 22:29:37.205188 pranavarya-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2024-05-16 20:28:55.000000 pranavarya-0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 22:29:37.169163 pranavarya-0.4/pranavarya/
+-rw-rw-rw-   0        0        0       40 2024-05-16 20:22:26.000000 pranavarya-0.4/pranavarya/__init__.py
+-rw-rw-rw-   0        0        0       69 2024-05-16 20:21:56.000000 pranavarya-0.4/pranavarya/main.py
+drwxrwxrwx   0        0        0        0 2024-05-16 22:29:37.203187 pranavarya-0.4/pranavarya.egg-info/
+-rw-rw-rw-   0        0        0       76 2024-05-16 22:29:36.000000 pranavarya-0.4/pranavarya.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2024-05-16 22:29:36.000000 pranavarya-0.4/pranavarya.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 22:29:36.000000 pranavarya-0.4/pranavarya.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-16 22:29:36.000000 pranavarya-0.4/pranavarya.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2024-05-16 22:29:36.000000 pranavarya-0.4/pranavarya.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 22:29:37.208287 pranavarya-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      342 2024-05-16 22:29:27.000000 pranavarya-0.4/setup.py
```

