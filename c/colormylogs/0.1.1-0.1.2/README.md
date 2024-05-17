# Comparing `tmp/colormylogs-0.1.1.tar.gz` & `tmp/colormylogs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colormylogs-0.1.1.tar", max compression
+gzip compressed data, was "colormylogs-0.1.2.tar", max compression
```

## Comparing `colormylogs-0.1.1.tar` & `colormylogs-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2024-05-16 07:45:24.126466 colormylogs-0.1.1/colormylogs/__init__.py
--rw-r--r--   0        0        0     1801 2024-05-16 14:42:16.371687 colormylogs-0.1.1/colormylogs/main.py
--rw-r--r--   0        0        0      346 2024-05-16 15:12:20.236661 colormylogs-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      335 1970-01-01 00:00:00.000000 colormylogs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-16 07:45:24.126466 colormylogs-0.1.2/colormylogs/__init__.py
+-rw-r--r--   0        0        0     1801 2024-05-16 14:42:16.371687 colormylogs-0.1.2/colormylogs/main.py
+-rw-r--r--   0        0        0      346 2024-05-16 15:15:39.471842 colormylogs-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      335 1970-01-01 00:00:00.000000 colormylogs-0.1.2/PKG-INFO
```

### Comparing `colormylogs-0.1.1/colormylogs/main.py` & `colormylogs-0.1.2/colormylogs/main.py`

 * *Files identical despite different names*

