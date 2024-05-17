# Comparing `tmp/lucy01-0.2.0.tar.gz` & `tmp/lucy01-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lucy01-0.2.0.tar", last modified: Thu May 16 09:23:12 2024, max compression
+gzip compressed data, was "lucy01-0.2.1.tar", last modified: Fri May 17 12:43:28 2024, max compression
```

## Comparing `lucy01-0.2.0.tar` & `lucy01-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:23:12.252749 lucy01-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-16 09:23:12.252749 lucy01-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-16 09:23:08.000000 lucy01-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:23:12.248748 lucy01-0.2.0/lucy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:23:08.000000 lucy01-0.2.0/lucy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-16 09:23:08.000000 lucy01-0.2.0/lucy/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-16 09:23:08.000000 lucy01-0.2.0/lucy/dbx_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-16 09:23:08.000000 lucy01-0.2.0/lucy/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-05-16 09:23:08.000000 lucy01-0.2.0/lucy/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:23:12.248748 lucy01-0.2.0/lucy/parser_/
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-16 09:23:08.000000 lucy01-0.2.0/lucy/parser_/atcoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-16 09:23:08.000000 lucy01-0.2.0/lucy/parser_/contest.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-16 09:23:08.000000 lucy01-0.2.0/lucy/parser_/parser_.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-16 09:23:08.000000 lucy01-0.2.0/lucy/scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-16 09:23:08.000000 lucy01-0.2.0/lucy/tester.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-16 09:23:08.000000 lucy01-0.2.0/lucy/update_snippets.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-16 09:23:08.000000 lucy01-0.2.0/lucy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:23:12.252749 lucy01-0.2.0/lucy01.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-16 09:23:12.000000 lucy01-0.2.0/lucy01.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-16 09:23:12.000000 lucy01-0.2.0/lucy01.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:23:12.000000 lucy01-0.2.0/lucy01.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-16 09:23:12.000000 lucy01-0.2.0/lucy01.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-16 09:23:12.000000 lucy01-0.2.0/lucy01.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 09:23:12.000000 lucy01-0.2.0/lucy01.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-16 09:23:08.000000 lucy01-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 09:23:12.252749 lucy01-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:43:28.260474 lucy01-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-05-17 12:43:28.260474 lucy01-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-17 12:43:22.000000 lucy01-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:43:28.256474 lucy01-0.2.1/lucy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:43:22.000000 lucy01-0.2.1/lucy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-17 12:43:22.000000 lucy01-0.2.1/lucy/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-17 12:43:22.000000 lucy01-0.2.1/lucy/dbx_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-17 12:43:22.000000 lucy01-0.2.1/lucy/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-05-17 12:43:22.000000 lucy01-0.2.1/lucy/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:43:28.260474 lucy01-0.2.1/lucy/parser_/
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-17 12:43:22.000000 lucy01-0.2.1/lucy/parser_/atcoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-17 12:43:22.000000 lucy01-0.2.1/lucy/parser_/contest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-17 12:43:22.000000 lucy01-0.2.1/lucy/parser_/parser_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-17 12:43:22.000000 lucy01-0.2.1/lucy/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-17 12:43:22.000000 lucy01-0.2.1/lucy/tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-17 12:43:22.000000 lucy01-0.2.1/lucy/update_snippets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-17 12:43:22.000000 lucy01-0.2.1/lucy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:43:28.260474 lucy01-0.2.1/lucy01.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-05-17 12:43:28.000000 lucy01-0.2.1/lucy01.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-17 12:43:28.000000 lucy01-0.2.1/lucy01.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 12:43:28.000000 lucy01-0.2.1/lucy01.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-17 12:43:28.000000 lucy01-0.2.1/lucy01.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-17 12:43:28.000000 lucy01-0.2.1/lucy01.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-17 12:43:28.000000 lucy01-0.2.1/lucy01.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-17 12:43:22.000000 lucy01-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 12:43:28.260474 lucy01-0.2.1/setup.cfg
```

### Comparing `lucy01-0.2.0/README.md` & `lucy01-0.2.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Lucy
 
 Lucy, a CLI companion for competitive programming on AtCoder and Codeforces, frees you from tedious
 tasks. It automatically fetches sample tests, sets up directories, and lets you test your code with
 just a few commands, streamlining your workflow and letting you focus on writing brilliant
 solutions.
 
+[Demo](https://github.com/kid-116/Lucy/assets/75692643/1b7195f7-fcd3-4e05-b23e-48061f6ef1b1)
+
 ## Support Languages
 - [x] C++
 - [ ] Python
 
 ## Supported Platforms
 - [x] AtCoder
 - [ ] Codeforces
@@ -18,50 +20,62 @@
 - [x] Fetch Hidden Test Cases (after the contest 🤪)
 - [x] Test Solution
 - [x] Setup Snippets
 - [ ] Submit Solution
 - [ ] What else? 🤔
 
 ## Installation
+```
+pip install lucy01
+```
+
+## Environment Variables
+- `LUCY_HOME`
+
+    Specify home directory for `lucy`.
+
+- `DROPBOX_TOKEN`
+
+
+    Dropbox developer access token with `sharing.read` permission. It can be generated at
+    [DBX Platform for Developers](https://www.dropbox.com/developers). This is necessary to fetch
+    hidden AtCoder test cases releaved after the contest has ended. All AtCoder test cases may be
+    found [here](https://www.dropbox.com/sh/nx3tnilzqz7df8a/AAAYlTq2tiEHl5hsESw6-yfLa?dl=0).
 
 ## Getting Started
 1. Set the environment variable `$LUCY_HOME` as preferred. By default, it uses the `~/.lucy`.
 2. Get help!
     ```
     lucy --help
     ```
+    Check out the [documentation](https://lucy01.readthedocs.io/en/latest/).
 
 ## Directory Structure
 ```
 $LUCY_HOME
 ├── .vscode
 │   └── cp.code-snippets*
 ├── AtCoder
 │   └── {ARC177}
-│       └──{A}
-│           ├── main
-│           ├── tests
-│           │   ├── in
-│           │   │   ├── {00.txt}
-│           │   │   ├── {01.txt}
-│           │   └── out
-│           │       ├── {00.txt}
-│           │       ├── {01.txt}
-│           └── main.cpp
+│       ├──{A}
+│       │   ├── main
+│       │   ├── tests
+│       │   │   ├── in
+│       │   │   │   ├── {00.txt}
+│       │   │   │   └── ...
+│       │   │   └── out
+│       │   │       ├── {00.txt}
+│       │   │       └── ...
+│       │   └── main.cpp
+│       └──...
 ├── Codeforces
 └── common*
     ├── base.cpp*
     ├── structures
     │   ├── grid.cpp
-    │   ├── linked_list.cpp
-    │   ├── point.cpp
-    │   ├── tree.cpp
-    │   ├── trie.cpp
-    │   └── union_find.cpp
-    └── text
-        ├── is_subseq.cpp
-
+    │   └── ...
+    └── ...
 ```
 
 - Lucy organizes your competitive programming workspace with a clear directory structure. Besides folders for specific contests and their solutions with `tests`, a key element is the `common` directory. This folder stores reusable code snippets `(*.cpp)`. These snippets can be easily inserted into your solution files using filename prefixes thanks to the `cp.code-snippets` file in the `.vscode` folder. This file, automatically generated with `lucy update-snippets`,  facilitates code completion within Visual Studio Code.
 
-  [Using Snippets](https://github.com/kid-116/CP/assets/75692643/3636b6f1-ad58-4bd7-8cb1-2c700f8a5b72)
+    [Using Snippets](https://github.com/kid-116/Lucy/assets/75692643/4b747b59-9736-4185-a6ee-9aa1fc843e92)
```

### Comparing `lucy01-0.2.0/lucy/config.py` & `lucy01-0.2.1/lucy/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 
 @dataclass
 class Config:
     WEBSITE_HOST = {Website.ATCODER: 'https://atcoder.jp'}
 
     LUCY_HOME = os.getenv('LUCY_HOME') or f'{os.getenv("HOME")}/.lucy'
     LUCY_HOME = os.path.abspath(LUCY_HOME)
-    assert os.path.isdir(LUCY_HOME)
 
     SNIPPETS_DIR = f'{LUCY_HOME}/.vscode'
     SNIPPETS_FILE_NAME = 'cp.code-snippets'
     SNIPPETS_PATH = f'{SNIPPETS_DIR}/{SNIPPETS_FILE_NAME}'
 
     COMMONS_DIR = os.path.abspath(f'{LUCY_HOME}/common')
```

### Comparing `lucy01-0.2.0/lucy/filesystem.py` & `lucy01-0.2.1/lucy/filesystem.py`

 * *Files identical despite different names*

### Comparing `lucy01-0.2.0/lucy/parser_/atcoder.py` & `lucy01-0.2.1/lucy/parser_/atcoder.py`

 * *Files identical despite different names*

### Comparing `lucy01-0.2.0/lucy/scraper.py` & `lucy01-0.2.1/lucy/scraper.py`

 * *Files identical despite different names*

### Comparing `lucy01-0.2.0/lucy/tester.py` & `lucy01-0.2.1/lucy/tester.py`

 * *Files identical despite different names*

### Comparing `lucy01-0.2.0/lucy/update_snippets.py` & `lucy01-0.2.1/lucy/update_snippets.py`

 * *Files identical despite different names*

