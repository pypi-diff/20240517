# Comparing `tmp/RetrieverVectorDB-0.2.tar.gz` & `tmp/RetrieverVectorDB-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RetrieverVectorDB-0.2.tar", last modified: Fri May 17 09:12:02 2024, max compression
+gzip compressed data, was "RetrieverVectorDB-0.3.tar", last modified: Fri May 17 09:24:22 2024, max compression
```

## Comparing `RetrieverVectorDB-0.2.tar` & `RetrieverVectorDB-0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 09:12:02.989750 RetrieverVectorDB-0.2/
--rw-rw-rw-   0        0        0      156 2024-05-17 09:12:02.988749 RetrieverVectorDB-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-17 09:12:02.979451 RetrieverVectorDB-0.2/RetrieverVectorDB/
--rw-rw-rw-   0        0        0      281 2024-05-17 09:09:06.000000 RetrieverVectorDB-0.2/RetrieverVectorDB/RetrieverVectorDB.py
--rw-rw-rw-   0        0        0        0 2024-05-17 08:29:38.000000 RetrieverVectorDB-0.2/RetrieverVectorDB/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 09:12:02.987749 RetrieverVectorDB-0.2/RetrieverVectorDB.egg-info/
--rw-rw-rw-   0        0        0      156 2024-05-17 09:12:02.000000 RetrieverVectorDB-0.2/RetrieverVectorDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2024-05-17 09:12:02.000000 RetrieverVectorDB-0.2/RetrieverVectorDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 09:12:02.000000 RetrieverVectorDB-0.2/RetrieverVectorDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-17 09:12:02.000000 RetrieverVectorDB-0.2/RetrieverVectorDB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 09:12:02.989750 RetrieverVectorDB-0.2/setup.cfg
--rw-rw-rw-   0        0        0      248 2024-05-17 09:10:45.000000 RetrieverVectorDB-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:22.943036 RetrieverVectorDB-0.3/
+-rw-rw-rw-   0        0        0      156 2024-05-17 09:24:22.942528 RetrieverVectorDB-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:22.911292 RetrieverVectorDB-0.3/RetrieverVectorDB/
+-rw-rw-rw-   0        0        0      300 2024-05-17 09:23:41.000000 RetrieverVectorDB-0.3/RetrieverVectorDB/RetrieverVectorDB.py
+-rw-rw-rw-   0        0        0        0 2024-05-17 08:29:38.000000 RetrieverVectorDB-0.3/RetrieverVectorDB/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:22.940288 RetrieverVectorDB-0.3/RetrieverVectorDB.egg-info/
+-rw-rw-rw-   0        0        0      156 2024-05-17 09:24:22.000000 RetrieverVectorDB-0.3/RetrieverVectorDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2024-05-17 09:24:22.000000 RetrieverVectorDB-0.3/RetrieverVectorDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 09:24:22.000000 RetrieverVectorDB-0.3/RetrieverVectorDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-17 09:24:22.000000 RetrieverVectorDB-0.3/RetrieverVectorDB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 09:24:22.943036 RetrieverVectorDB-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      248 2024-05-17 09:24:06.000000 RetrieverVectorDB-0.3/setup.py
```

