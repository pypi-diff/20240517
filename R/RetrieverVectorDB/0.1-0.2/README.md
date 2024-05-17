# Comparing `tmp/RetrieverVectorDB-0.1.tar.gz` & `tmp/RetrieverVectorDB-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RetrieverVectorDB-0.1.tar", last modified: Fri May 17 08:32:49 2024, max compression
+gzip compressed data, was "RetrieverVectorDB-0.2.tar", last modified: Fri May 17 09:12:02 2024, max compression
```

## Comparing `RetrieverVectorDB-0.1.tar` & `RetrieverVectorDB-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 08:32:49.426189 RetrieverVectorDB-0.1/
--rw-rw-rw-   0        0        0      156 2024-05-17 08:32:49.424188 RetrieverVectorDB-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-17 08:32:49.331578 RetrieverVectorDB-0.1/RetrieverVectorDB/
--rw-rw-rw-   0        0        0      390 2024-05-17 08:31:42.000000 RetrieverVectorDB-0.1/RetrieverVectorDB/RetrieverVectorDB.py
--rw-rw-rw-   0        0        0        0 2024-05-17 08:29:38.000000 RetrieverVectorDB-0.1/RetrieverVectorDB/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 08:32:49.422202 RetrieverVectorDB-0.1/RetrieverVectorDB.egg-info/
--rw-rw-rw-   0        0        0      156 2024-05-17 08:32:49.000000 RetrieverVectorDB-0.1/RetrieverVectorDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2024-05-17 08:32:49.000000 RetrieverVectorDB-0.1/RetrieverVectorDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 08:32:49.000000 RetrieverVectorDB-0.1/RetrieverVectorDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-17 08:32:49.000000 RetrieverVectorDB-0.1/RetrieverVectorDB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 08:32:49.427187 RetrieverVectorDB-0.1/setup.cfg
--rw-rw-rw-   0        0        0      248 2024-05-17 08:31:25.000000 RetrieverVectorDB-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:12:02.989750 RetrieverVectorDB-0.2/
+-rw-rw-rw-   0        0        0      156 2024-05-17 09:12:02.988749 RetrieverVectorDB-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-17 09:12:02.979451 RetrieverVectorDB-0.2/RetrieverVectorDB/
+-rw-rw-rw-   0        0        0      281 2024-05-17 09:09:06.000000 RetrieverVectorDB-0.2/RetrieverVectorDB/RetrieverVectorDB.py
+-rw-rw-rw-   0        0        0        0 2024-05-17 08:29:38.000000 RetrieverVectorDB-0.2/RetrieverVectorDB/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:12:02.987749 RetrieverVectorDB-0.2/RetrieverVectorDB.egg-info/
+-rw-rw-rw-   0        0        0      156 2024-05-17 09:12:02.000000 RetrieverVectorDB-0.2/RetrieverVectorDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2024-05-17 09:12:02.000000 RetrieverVectorDB-0.2/RetrieverVectorDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 09:12:02.000000 RetrieverVectorDB-0.2/RetrieverVectorDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-17 09:12:02.000000 RetrieverVectorDB-0.2/RetrieverVectorDB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 09:12:02.989750 RetrieverVectorDB-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      248 2024-05-17 09:10:45.000000 RetrieverVectorDB-0.2/setup.py
```

