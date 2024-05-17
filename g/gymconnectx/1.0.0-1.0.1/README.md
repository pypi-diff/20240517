# Comparing `tmp/gymconnectx-1.0.0.tar.gz` & `tmp/gymconnectx-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymconnectx-1.0.0.tar", last modified: Fri May 17 14:25:24 2024, max compression
+gzip compressed data, was "gymconnectx-1.0.1.tar", last modified: Fri May 17 14:46:03 2024, max compression
```

## Comparing `gymconnectx-1.0.0.tar` & `gymconnectx-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:25:24.402143 gymconnectx-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-17 14:25:20.000000 gymconnectx-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-17 14:25:24.402143 gymconnectx-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-17 14:25:20.000000 gymconnectx-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:25:24.398143 gymconnectx-1.0.0/gymconnectx/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-17 14:25:20.000000 gymconnectx-1.0.0/gymconnectx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:25:24.402143 gymconnectx-1.0.0/gymconnectx/envs/
--rw-r--r--   0 runner    (1001) docker     (127)    25493 2024-05-17 14:25:20.000000 gymconnectx-1.0.0/gymconnectx/envs/gymconnectxenv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:25:24.402143 gymconnectx-1.0.0/gymconnectx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-17 14:25:24.000000 gymconnectx-1.0.0/gymconnectx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-17 14:25:24.000000 gymconnectx-1.0.0/gymconnectx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:25:24.000000 gymconnectx-1.0.0/gymconnectx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 14:25:24.000000 gymconnectx-1.0.0/gymconnectx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-17 14:25:24.000000 gymconnectx-1.0.0/gymconnectx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-17 14:25:20.000000 gymconnectx-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 14:25:24.402143 gymconnectx-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-17 14:25:20.000000 gymconnectx-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:46:03.477001 gymconnectx-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-17 14:45:58.000000 gymconnectx-1.0.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-17 14:46:03.477001 gymconnectx-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-17 14:45:58.000000 gymconnectx-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:46:03.477001 gymconnectx-1.0.1/gymconnectx/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-17 14:45:58.000000 gymconnectx-1.0.1/gymconnectx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:46:03.477001 gymconnectx-1.0.1/gymconnectx/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-17 14:45:58.000000 gymconnectx-1.0.1/gymconnectx/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25493 2024-05-17 14:45:58.000000 gymconnectx-1.0.1/gymconnectx/envs/gymconnectxenv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:46:03.477001 gymconnectx-1.0.1/gymconnectx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-17 14:46:03.000000 gymconnectx-1.0.1/gymconnectx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-17 14:46:03.000000 gymconnectx-1.0.1/gymconnectx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:46:03.000000 gymconnectx-1.0.1/gymconnectx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 14:46:03.000000 gymconnectx-1.0.1/gymconnectx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-17 14:46:03.000000 gymconnectx-1.0.1/gymconnectx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-17 14:45:58.000000 gymconnectx-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 14:46:03.477001 gymconnectx-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-17 14:45:58.000000 gymconnectx-1.0.1/setup.py
```

### Comparing `gymconnectx-1.0.0/LICENSE.md` & `gymconnectx-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gymconnectx-1.0.0/PKG-INFO` & `gymconnectx-1.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gymconnectx
-Version: 1.0.0
+Version: 1.0.1
 Summary: An OpenAI Gym Environment Connect X Game with GUI. ConnectX is a game for two players that is based on the well-known Connect 4. The goal is to place X coins in a row, column, or diagonal on a board with dimensions M by N.
 Home-page: https://github.com/fauzisho/GymConnectX
 Author: Fauzi Sholichin
 License: MIT License
         
         Copyright (c) 2024 AI Trafic Project
         
@@ -32,8 +32,26 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: gym
 Requires-Dist: pygame
 
-GYM Connect X
+# Connect Game Environment
+
+This repository contains the implementation of a Connect Game Environment using OpenAI's Gym and Pygame for rendering. The environment supports various game modes like Connect Four and includes features like GUI display, avatar support for players, and different modes of player interaction (human, random).
+
+## Table of Contents
+
+- [Description](#description)
+- [Installation](#installation)
+
+## Description
+
+The Connect Game Environment is a customizable and interactive environment for simulating Connect-style games. It leverages the OpenAI Gym interface for standard reinforcement learning interactions and uses Pygame for graphical rendering. The environment allows for different configurations of the board size and connect length and includes support for different player types, including human players and random agents.
+
+## Installation
+
+To use this environment, you need to have Python installed. You can install the necessary packages using `pip`:
+
+```bash
+pip install gymconnectx
```

### Comparing `gymconnectx-1.0.0/gymconnectx/envs/gymconnectxenv.py` & `gymconnectx-1.0.1/gymconnectx/envs/gymconnectxenv.py`

 * *Files identical despite different names*

### Comparing `gymconnectx-1.0.0/gymconnectx.egg-info/PKG-INFO` & `gymconnectx-1.0.1/gymconnectx.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gymconnectx
-Version: 1.0.0
+Version: 1.0.1
 Summary: An OpenAI Gym Environment Connect X Game with GUI. ConnectX is a game for two players that is based on the well-known Connect 4. The goal is to place X coins in a row, column, or diagonal on a board with dimensions M by N.
 Home-page: https://github.com/fauzisho/GymConnectX
 Author: Fauzi Sholichin
 License: MIT License
         
         Copyright (c) 2024 AI Trafic Project
         
@@ -32,8 +32,26 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: gym
 Requires-Dist: pygame
 
-GYM Connect X
+# Connect Game Environment
+
+This repository contains the implementation of a Connect Game Environment using OpenAI's Gym and Pygame for rendering. The environment supports various game modes like Connect Four and includes features like GUI display, avatar support for players, and different modes of player interaction (human, random).
+
+## Table of Contents
+
+- [Description](#description)
+- [Installation](#installation)
+
+## Description
+
+The Connect Game Environment is a customizable and interactive environment for simulating Connect-style games. It leverages the OpenAI Gym interface for standard reinforcement learning interactions and uses Pygame for graphical rendering. The environment allows for different configurations of the board size and connect length and includes support for different player types, including human players and random agents.
+
+## Installation
+
+To use this environment, you need to have Python installed. You can install the necessary packages using `pip`:
+
+```bash
+pip install gymconnectx
```

### Comparing `gymconnectx-1.0.0/pyproject.toml` & `gymconnectx-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gymconnectx"
-version = "1.0.0"
+version = "1.0.1"
 description = "An OpenAI Gym Environment Connect X Game with GUI. ConnectX is a game for two players that is based on the well-known Connect 4. The goal is to place X coins in a row, column, or diagonal on a board with dimensions M by N."
 readme = "README.md"
 authors = [{ name = "Fauzi Sholichin" }]
 license = { file = "LICENSE.md" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

