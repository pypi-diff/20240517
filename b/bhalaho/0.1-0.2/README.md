# Comparing `tmp/bhalaho-0.1.tar.gz` & `tmp/bhalaho-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhalaho-0.1.tar", last modified: Thu May 16 22:30:16 2024, max compression
+gzip compressed data, was "bhalaho-0.2.tar", last modified: Thu May 16 22:42:58 2024, max compression
```

## Comparing `bhalaho-0.1.tar` & `bhalaho-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 22:30:16.138817 bhalaho-0.1/
--rw-rw-rw-   0        0        0     1041 2024-05-16 22:19:08.000000 bhalaho-0.1/LICENSE
--rw-rw-rw-   0        0        0       72 2024-05-16 22:19:58.000000 bhalaho-0.1/MANIFEST.in
--rw-rw-rw-   0        0        0       75 2024-05-16 22:30:16.138817 bhalaho-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       21 2024-05-16 21:22:32.000000 bhalaho-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 22:30:16.112002 bhalaho-0.1/bhalaho/
--rw-rw-rw-   0        0        0        0 2024-05-16 20:58:36.000000 bhalaho-0.1/bhalaho/__init__.py
--rw-rw-rw-   0        0        0    30234 2024-05-16 22:15:13.000000 bhalaho-0.1/bhalaho/daoa.py
--rw-rw-rw-   0        0        0      756 2024-05-16 21:25:52.000000 bhalaho-0.1/bhalaho/download.py
-drwxrwxrwx   0        0        0        0 2024-05-16 22:30:16.138817 bhalaho-0.1/bhalaho.egg-info/
--rw-rw-rw-   0        0        0       75 2024-05-16 22:30:15.000000 bhalaho-0.1/bhalaho.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-05-16 22:30:15.000000 bhalaho-0.1/bhalaho.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 22:30:15.000000 bhalaho-0.1/bhalaho.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-16 22:30:15.000000 bhalaho-0.1/bhalaho.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 22:30:16.144322 bhalaho-0.1/setup.cfg
--rw-rw-rw-   0        0        0      211 2024-05-16 22:20:14.000000 bhalaho-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 22:42:58.878158 bhalaho-0.2/
+-rw-rw-rw-   0        0        0     1041 2024-05-16 22:19:08.000000 bhalaho-0.2/LICENSE
+-rw-rw-rw-   0        0        0       72 2024-05-16 22:19:58.000000 bhalaho-0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0       75 2024-05-16 22:42:58.871429 bhalaho-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       21 2024-05-16 21:22:32.000000 bhalaho-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 22:42:58.839193 bhalaho-0.2/bhalaho/
+-rw-rw-rw-   0        0        0        0 2024-05-16 20:58:36.000000 bhalaho-0.2/bhalaho/__init__.py
+-rw-rw-rw-   0        0        0    30234 2024-05-16 22:15:13.000000 bhalaho-0.2/bhalaho/daoa.py
+-rw-rw-rw-   0        0        0      756 2024-05-16 21:25:52.000000 bhalaho-0.2/bhalaho/download.py
+drwxrwxrwx   0        0        0        0 2024-05-16 22:42:58.871429 bhalaho-0.2/bhalaho.egg-info/
+-rw-rw-rw-   0        0        0       75 2024-05-16 22:42:58.000000 bhalaho-0.2/bhalaho.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-05-16 22:42:58.000000 bhalaho-0.2/bhalaho.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 22:42:58.000000 bhalaho-0.2/bhalaho.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-16 22:42:58.000000 bhalaho-0.2/bhalaho.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 22:42:58.878158 bhalaho-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      211 2024-05-16 22:42:53.000000 bhalaho-0.2/setup.py
```

### Comparing `bhalaho-0.1/LICENSE` & `bhalaho-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bhalaho-0.1/bhalaho/daoa.py` & `bhalaho-0.2/bhalaho/daoa.py`

 * *Files identical despite different names*

### Comparing `bhalaho-0.1/bhalaho/download.py` & `bhalaho-0.2/bhalaho/download.py`

 * *Files identical despite different names*

