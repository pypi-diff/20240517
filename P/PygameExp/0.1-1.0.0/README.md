# Comparing `tmp/PygameExp-0.1.tar.gz` & `tmp/PygameExp-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PygameExp-0.1.tar", last modified: Thu May 16 11:36:20 2024, max compression
+gzip compressed data, was "PygameExp-1.0.0.tar", last modified: Thu May 16 11:40:04 2024, max compression
```

## Comparing `PygameExp-0.1.tar` & `PygameExp-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 11:36:20.638519 PygameExp-0.1/
--rw-rw-rw-   0        0        0       54 2024-05-16 11:36:20.638519 PygameExp-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-16 11:36:20.633298 PygameExp-0.1/PygameExp.egg-info/
--rw-rw-rw-   0        0        0       54 2024-05-16 11:36:20.000000 PygameExp-0.1/PygameExp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2024-05-16 11:36:20.000000 PygameExp-0.1/PygameExp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 11:36:20.000000 PygameExp-0.1/PygameExp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-16 11:36:20.000000 PygameExp-0.1/PygameExp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-16 11:36:20.000000 PygameExp-0.1/PygameExp.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-16 11:36:20.636581 PygameExp-0.1/pygame_plus/
--rw-rw-rw-   0        0        0        0 2024-05-16 10:46:39.000000 PygameExp-0.1/pygame_plus/__init__.py
--rw-rw-rw-   0        0        0      429 2024-05-16 10:46:39.000000 PygameExp-0.1/pygame_plus/game_math.py
--rw-rw-rw-   0        0        0     9468 2024-05-16 10:46:39.000000 PygameExp-0.1/pygame_plus/main.py
--rw-rw-rw-   0        0        0       42 2024-05-16 11:36:20.639523 PygameExp-0.1/setup.cfg
--rw-rw-rw-   0        0        0      166 2024-05-16 11:36:08.000000 PygameExp-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:40:04.310865 PygameExp-1.0.0/
+-rw-rw-rw-   0        0        0       56 2024-05-16 11:40:04.309864 PygameExp-1.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 11:40:04.299865 PygameExp-1.0.0/PygameExp.egg-info/
+-rw-rw-rw-   0        0        0       56 2024-05-16 11:40:01.000000 PygameExp-1.0.0/PygameExp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-16 11:40:04.000000 PygameExp-1.0.0/PygameExp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 11:40:01.000000 PygameExp-1.0.0/PygameExp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-16 11:40:01.000000 PygameExp-1.0.0/PygameExp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-16 11:40:04.000000 PygameExp-1.0.0/PygameExp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 11:40:04.305864 PygameExp-1.0.0/pygame_exp/
+-rw-rw-rw-   0        0        0        0 2024-05-16 10:46:39.000000 PygameExp-1.0.0/pygame_exp/__init__.py
+-rw-rw-rw-   0        0        0      429 2024-05-16 10:46:39.000000 PygameExp-1.0.0/pygame_exp/game_math.py
+-rw-rw-rw-   0        0        0     9468 2024-05-16 10:46:39.000000 PygameExp-1.0.0/pygame_exp/main.py
+-rw-rw-rw-   0        0        0       42 2024-05-16 11:40:04.310865 PygameExp-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      168 2024-05-16 11:39:37.000000 PygameExp-1.0.0/setup.py
```

### Comparing `PygameExp-0.1/pygame_plus/main.py` & `PygameExp-1.0.0/pygame_exp/main.py`

 * *Files identical despite different names*

