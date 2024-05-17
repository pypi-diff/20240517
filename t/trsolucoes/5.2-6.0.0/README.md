# Comparing `tmp/trsolucoes-5.2.tar.gz` & `tmp/trsolucoes-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trsolucoes-5.2.tar", last modified: Thu May 16 23:45:23 2024, max compression
+gzip compressed data, was "trsolucoes-6.0.0.tar", last modified: Fri May 17 11:32:48 2024, max compression
```

## Comparing `trsolucoes-5.2.tar` & `trsolucoes-6.0.0.tar`

### file list

```diff
@@ -1,10 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 23:45:23.029460 trsolucoes-5.2/
--rw-rw-rw-   0        0        0      341 2024-05-16 23:45:23.028953 trsolucoes-5.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-16 23:45:23.029460 trsolucoes-5.2/setup.cfg
--rw-rw-rw-   0        0        0      701 2024-05-16 23:45:13.000000 trsolucoes-5.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 23:45:23.027953 trsolucoes-5.2/trsolucoes.egg-info/
--rw-rw-rw-   0        0        0      341 2024-05-16 23:45:22.000000 trsolucoes-5.2/trsolucoes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2024-05-16 23:45:22.000000 trsolucoes-5.2/trsolucoes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 23:45:22.000000 trsolucoes-5.2/trsolucoes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-16 23:45:22.000000 trsolucoes-5.2/trsolucoes.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 23:45:22.000000 trsolucoes-5.2/trsolucoes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 11:32:48.365868 trsolucoes-6.0.0/
+-rw-rw-rw-   0        0        0     1088 2024-05-17 11:25:36.000000 trsolucoes-6.0.0/LICENCE
+-rw-rw-rw-   0        0        0      403 2024-05-17 11:32:48.365868 trsolucoes-6.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       67 2024-05-17 11:31:58.000000 trsolucoes-6.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 11:32:48.346451 trsolucoes-6.0.0/selenium_helper/
+-rw-rw-rw-   0        0        0       43 2024-05-17 11:15:10.000000 trsolucoes-6.0.0/selenium_helper/__init__.py
+-rw-rw-rw-   0        0        0     4576 2024-05-17 11:08:04.000000 trsolucoes-6.0.0/selenium_helper/selenium_helper.py
+-rw-rw-rw-   0        0        0       42 2024-05-17 11:32:48.365868 trsolucoes-6.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      525 2024-05-17 11:32:00.000000 trsolucoes-6.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 11:32:48.364839 trsolucoes-6.0.0/trsolucoes.egg-info/
+-rw-rw-rw-   0        0        0      403 2024-05-17 11:32:48.000000 trsolucoes-6.0.0/trsolucoes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-05-17 11:32:48.000000 trsolucoes-6.0.0/trsolucoes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 11:32:48.000000 trsolucoes-6.0.0/trsolucoes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-17 11:32:48.000000 trsolucoes-6.0.0/trsolucoes.egg-info/top_level.txt
```

