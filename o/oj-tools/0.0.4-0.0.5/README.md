# Comparing `tmp/oj_tools-0.0.4.tar.gz` & `tmp/oj_tools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oj_tools-0.0.4.tar", last modified: Wed May 15 20:28:30 2024, max compression
+gzip compressed data, was "oj_tools-0.0.5.tar", last modified: Fri May 17 06:19:38 2024, max compression
```

## Comparing `oj_tools-0.0.4.tar` & `oj_tools-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:28:30.267180 oj_tools-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-15 20:28:30.267180 oj_tools-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-15 20:28:20.000000 oj_tools-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-15 20:28:20.000000 oj_tools-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 20:28:30.267180 oj_tools-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:28:30.267180 oj_tools-0.0.4/src/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-15 20:28:20.000000 oj_tools-0.0.4/src/oj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:28:30.267180 oj_tools-0.0.4/src/oj_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-15 20:28:30.000000 oj_tools-0.0.4/src/oj_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-15 20:28:30.000000 oj_tools-0.0.4/src/oj_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:28:30.000000 oj_tools-0.0.4/src/oj_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 20:28:30.000000 oj_tools-0.0.4/src/oj_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-15 20:28:20.000000 oj_tools-0.0.4/src/problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-15 20:28:20.000000 oj_tools-0.0.4/src/testcase.py
+drwxr-xr-x   0 hepheir    (501) staff       (20)        0 2024-05-17 06:19:38.775215 oj_tools-0.0.5/
+-rw-r--r--   0 hepheir    (501) staff       (20)     2301 2024-05-17 06:19:38.775037 oj_tools-0.0.5/PKG-INFO
+-rw-r--r--   0 hepheir    (501) staff       (20)     1815 2024-05-15 20:24:23.000000 oj_tools-0.0.5/README.md
+-rw-r--r--   0 hepheir    (501) staff       (20)      489 2024-05-16 08:10:27.000000 oj_tools-0.0.5/pyproject.toml
+-rw-r--r--   0 hepheir    (501) staff       (20)       38 2024-05-17 06:19:38.775251 oj_tools-0.0.5/setup.cfg
+drwxr-xr-x   0 hepheir    (501) staff       (20)        0 2024-05-17 06:19:38.771951 oj_tools-0.0.5/src/
+drwxr-xr-x   0 hepheir    (501) staff       (20)        0 2024-05-17 06:19:38.773868 oj_tools-0.0.5/src/oj/
+-rw-r--r--   0 hepheir    (501) staff       (20)      111 2024-05-16 20:21:21.000000 oj_tools-0.0.5/src/oj/__init__.py
+-rw-r--r--   0 hepheir    (501) staff       (20)      321 2024-05-17 05:58:56.000000 oj_tools-0.0.5/src/oj/constants.py
+-rw-r--r--   0 hepheir    (501) staff       (20)     2100 2024-05-16 09:33:25.000000 oj_tools-0.0.5/src/oj/problem.py
+-rw-r--r--   0 hepheir    (501) staff       (20)     1418 2024-05-16 09:32:33.000000 oj_tools-0.0.5/src/oj/testcase.py
+-rw-r--r--   0 hepheir    (501) staff       (20)     1246 2024-05-17 06:01:33.000000 oj_tools-0.0.5/src/oj/validators.py
+-rw-r--r--   0 hepheir    (501) staff       (20)      895 2024-05-16 09:31:34.000000 oj_tools-0.0.5/src/oj_test.py
+drwxr-xr-x   0 hepheir    (501) staff       (20)        0 2024-05-17 06:19:38.774846 oj_tools-0.0.5/src/oj_tools.egg-info/
+-rw-r--r--   0 hepheir    (501) staff       (20)     2301 2024-05-17 06:19:38.000000 oj_tools-0.0.5/src/oj_tools.egg-info/PKG-INFO
+-rw-r--r--   0 hepheir    (501) staff       (20)      280 2024-05-17 06:19:38.000000 oj_tools-0.0.5/src/oj_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 hepheir    (501) staff       (20)        1 2024-05-17 06:19:38.000000 oj_tools-0.0.5/src/oj_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 hepheir    (501) staff       (20)       11 2024-05-17 06:19:38.000000 oj_tools-0.0.5/src/oj_tools.egg-info/top_level.txt
```

### Comparing `oj_tools-0.0.4/PKG-INFO` & `oj_tools-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oj-tools
-Version: 0.0.4
+Version: 0.0.5
 Summary: tools for Online Judge management
 Author-email: hepheir <hepheir@gmail.com>
 Project-URL: Homepage, https://https://github.com/hepheir/oj-tools
 Project-URL: Issues, https://https://github.com/hepheir/oj-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `oj_tools-0.0.4/README.md` & `oj_tools-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `oj_tools-0.0.4/src/oj_tools.egg-info/PKG-INFO` & `oj_tools-0.0.5/src/oj_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oj-tools
-Version: 0.0.4
+Version: 0.0.5
 Summary: tools for Online Judge management
 Author-email: hepheir <hepheir@gmail.com>
 Project-URL: Homepage, https://https://github.com/hepheir/oj-tools
 Project-URL: Issues, https://https://github.com/hepheir/oj-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

