# Comparing `tmp/pandisplay-1.0.0.tar.gz` & `tmp/pandisplay-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandisplay-1.0.0.tar", last modified: Mon May 13 03:00:30 2024, max compression
+gzip compressed data, was "pandisplay-2.0.0.tar", last modified: Fri May 17 18:09:00 2024, max compression
```

## Comparing `pandisplay-1.0.0.tar` & `pandisplay-2.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 artemis    (501) staff       (20)        0 2024-05-13 03:00:30.686346 pandisplay-1.0.0/
--rw-r--r--   0 artemis    (501) staff       (20)      151 2024-05-13 03:00:30.686232 pandisplay-1.0.0/PKG-INFO
-drwxr-xr-x   0 artemis    (501) staff       (20)        0 2024-05-13 03:00:30.685541 pandisplay-1.0.0/pandisplay/
--rw-r--r--   0 artemis    (501) staff       (20)     1019 2024-05-13 02:52:42.000000 pandisplay-1.0.0/pandisplay/__init__.py
-drwxr-xr-x   0 artemis    (501) staff       (20)        0 2024-05-13 03:00:30.686086 pandisplay-1.0.0/pandisplay.egg-info/
--rw-r--r--   0 artemis    (501) staff       (20)      151 2024-05-13 03:00:30.000000 pandisplay-1.0.0/pandisplay.egg-info/PKG-INFO
--rw-r--r--   0 artemis    (501) staff       (20)      200 2024-05-13 03:00:30.000000 pandisplay-1.0.0/pandisplay.egg-info/SOURCES.txt
--rw-r--r--   0 artemis    (501) staff       (20)        1 2024-05-13 03:00:30.000000 pandisplay-1.0.0/pandisplay.egg-info/dependency_links.txt
--rw-r--r--   0 artemis    (501) staff       (20)       15 2024-05-13 03:00:30.000000 pandisplay-1.0.0/pandisplay.egg-info/requires.txt
--rw-r--r--   0 artemis    (501) staff       (20)       11 2024-05-13 03:00:30.000000 pandisplay-1.0.0/pandisplay.egg-info/top_level.txt
--rw-r--r--   0 artemis    (501) staff       (20)       38 2024-05-13 03:00:30.686443 pandisplay-1.0.0/setup.cfg
--rw-r--r--   0 artemis    (501) staff       (20)      329 2024-05-13 03:00:28.000000 pandisplay-1.0.0/setup.py
+drwxr-xr-x   0 artemis    (501) staff       (20)        0 2024-05-17 18:09:00.263011 pandisplay-2.0.0/
+-rw-r--r--   0 artemis    (501) staff       (20)      151 2024-05-17 18:09:00.262897 pandisplay-2.0.0/PKG-INFO
+drwxr-xr-x   0 artemis    (501) staff       (20)        0 2024-05-17 18:09:00.262133 pandisplay-2.0.0/pandisplay/
+-rw-r--r--   0 artemis    (501) staff       (20)     1456 2024-05-17 18:04:19.000000 pandisplay-2.0.0/pandisplay/__init__.py
+drwxr-xr-x   0 artemis    (501) staff       (20)        0 2024-05-17 18:09:00.262753 pandisplay-2.0.0/pandisplay.egg-info/
+-rw-r--r--   0 artemis    (501) staff       (20)      151 2024-05-17 18:09:00.000000 pandisplay-2.0.0/pandisplay.egg-info/PKG-INFO
+-rw-r--r--   0 artemis    (501) staff       (20)      200 2024-05-17 18:09:00.000000 pandisplay-2.0.0/pandisplay.egg-info/SOURCES.txt
+-rw-r--r--   0 artemis    (501) staff       (20)        1 2024-05-17 18:09:00.000000 pandisplay-2.0.0/pandisplay.egg-info/dependency_links.txt
+-rw-r--r--   0 artemis    (501) staff       (20)       15 2024-05-17 18:09:00.000000 pandisplay-2.0.0/pandisplay.egg-info/requires.txt
+-rw-r--r--   0 artemis    (501) staff       (20)       11 2024-05-17 18:09:00.000000 pandisplay-2.0.0/pandisplay.egg-info/top_level.txt
+-rw-r--r--   0 artemis    (501) staff       (20)       38 2024-05-17 18:09:00.263051 pandisplay-2.0.0/setup.cfg
+-rw-r--r--   0 artemis    (501) staff       (20)      329 2024-05-17 17:58:37.000000 pandisplay-2.0.0/setup.py
```

