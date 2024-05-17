# Comparing `tmp/ddeagentlib-0.3.tar.gz` & `tmp/ddeagentlib-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddeagentlib-0.3.tar", last modified: Fri May 17 04:26:34 2024, max compression
+gzip compressed data, was "ddeagentlib-1.0.2.tar", last modified: Fri May 17 05:24:08 2024, max compression
```

## Comparing `ddeagentlib-0.3.tar` & `ddeagentlib-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 04:26:34.563343 ddeagentlib-0.3/
--rw-rw-rw-   0        0        0      430 2024-05-17 04:26:34.562344 ddeagentlib-0.3/PKG-INFO
--rw-rw-rw-   0        0        0       20 2024-05-16 08:54:02.000000 ddeagentlib-0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 04:26:34.561344 ddeagentlib-0.3/ddeagentlib.egg-info/
--rw-rw-rw-   0        0        0      430 2024-05-17 04:26:34.000000 ddeagentlib-0.3/ddeagentlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      158 2024-05-17 04:26:34.000000 ddeagentlib-0.3/ddeagentlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 04:26:34.000000 ddeagentlib-0.3/ddeagentlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 04:26:34.000000 ddeagentlib-0.3/ddeagentlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 04:26:34.563343 ddeagentlib-0.3/setup.cfg
--rw-rw-rw-   0        0        0      609 2024-05-17 04:26:24.000000 ddeagentlib-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 05:24:08.645761 ddeagentlib-1.0.2/
+-rw-rw-rw-   0        0        0      199 2024-05-17 05:24:08.645761 ddeagentlib-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       20 2024-05-16 08:54:02.000000 ddeagentlib-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 05:24:08.643760 ddeagentlib-1.0.2/ddeagentlib.egg-info/
+-rw-rw-rw-   0        0        0      199 2024-05-17 05:24:08.000000 ddeagentlib-1.0.2/ddeagentlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2024-05-17 05:24:08.000000 ddeagentlib-1.0.2/ddeagentlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 05:24:08.000000 ddeagentlib-1.0.2/ddeagentlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 05:24:08.000000 ddeagentlib-1.0.2/ddeagentlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 05:24:08.645761 ddeagentlib-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      354 2024-05-17 05:23:44.000000 ddeagentlib-1.0.2/setup.py
```

