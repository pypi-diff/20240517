# Comparing `tmp/mfu-0.0.7.tar.gz` & `tmp/mfu-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfu-0.0.7.tar", last modified: Fri May 17 08:49:44 2024, max compression
+gzip compressed data, was "mfu-0.0.8.tar", last modified: Fri May 17 08:53:45 2024, max compression
```

## Comparing `mfu-0.0.7.tar` & `mfu-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:49:44.392214 mfu-0.0.7/
--rw-r--r--   0 michael   (1000) michael   (1000)      827 2024-05-17 08:49:44.392214 mfu-0.0.7/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)      476 2024-05-17 08:49:27.000000 mfu-0.0.7/README.md
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:49:44.392214 mfu-0.0.7/mfu/
--rw-rw-r--   0 michael   (1000) michael   (1000)        0 2023-03-22 08:55:51.000000 mfu-0.0.7/mfu/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)       61 2023-03-22 08:55:56.000000 mfu-0.0.7/mfu/__main__.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      324 2024-05-17 08:42:36.000000 mfu-0.0.7/mfu/main.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:49:44.392214 mfu-0.0.7/mfu/scripts/
--rw-rw-r--   0 michael   (1000) michael   (1000)        0 2023-03-22 08:55:45.000000 mfu-0.0.7/mfu/scripts/__init__.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4159 2024-04-12 11:30:45.000000 mfu-0.0.7/mfu/scripts/cluster.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1199 2023-03-22 09:33:27.000000 mfu-0.0.7/mfu/scripts/config.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3748 2023-03-22 09:16:00.000000 mfu-0.0.7/mfu/scripts/doctor.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3709 2024-05-17 08:49:07.000000 mfu-0.0.7/mfu/scripts/sync.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:49:44.392214 mfu-0.0.7/mfu/utils/
--rwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-23 11:12:20.000000 mfu-0.0.7/mfu/utils/__init__.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2841 2022-11-23 11:15:13.000000 mfu-0.0.7/mfu/utils/forcelink.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3176 2023-06-20 13:21:08.000000 mfu-0.0.7/mfu/utils/general.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:49:44.392214 mfu-0.0.7/mfu.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)      827 2024-05-17 08:49:44.000000 mfu-0.0.7/mfu.egg-info/PKG-INFO
--rwxr-xr-x   0 michael   (1000) michael   (1000)      418 2024-05-17 08:49:44.000000 mfu-0.0.7/mfu.egg-info/SOURCES.txt
--rwxr-xr-x   0 michael   (1000) michael   (1000)        1 2024-05-17 08:49:44.000000 mfu-0.0.7/mfu.egg-info/dependency_links.txt
--rwxr-xr-x   0 michael   (1000) michael   (1000)       37 2024-05-17 08:49:44.000000 mfu-0.0.7/mfu.egg-info/entry_points.txt
--rwxr-xr-x   0 michael   (1000) michael   (1000)       83 2024-05-17 08:49:44.000000 mfu-0.0.7/mfu.egg-info/requires.txt
--rwxr-xr-x   0 michael   (1000) michael   (1000)        4 2024-05-17 08:49:44.000000 mfu-0.0.7/mfu.egg-info/top_level.txt
--rwxr-xr-x   0 michael   (1000) michael   (1000)      486 2024-05-17 08:49:37.000000 mfu-0.0.7/pyproject.toml
--rw-rw-r--   0 michael   (1000) michael   (1000)       38 2024-05-17 08:49:44.392214 mfu-0.0.7/setup.cfg
--rw-rw-r--   0 michael   (1000) michael   (1000)       68 2023-03-22 08:56:38.000000 mfu-0.0.7/setup.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:53:45.038613 mfu-0.0.8/
+-rw-r--r--   0 michael   (1000) michael   (1000)      895 2024-05-17 08:53:45.038613 mfu-0.0.8/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)      508 2024-05-17 08:53:33.000000 mfu-0.0.8/README.md
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:53:45.034613 mfu-0.0.8/mfu/
+-rw-rw-r--   0 michael   (1000) michael   (1000)        0 2023-03-22 08:55:51.000000 mfu-0.0.8/mfu/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)       61 2023-03-22 08:55:56.000000 mfu-0.0.8/mfu/__main__.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      324 2024-05-17 08:42:36.000000 mfu-0.0.8/mfu/main.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:53:45.038613 mfu-0.0.8/mfu/scripts/
+-rw-rw-r--   0 michael   (1000) michael   (1000)        0 2023-03-22 08:55:45.000000 mfu-0.0.8/mfu/scripts/__init__.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4159 2024-04-12 11:30:45.000000 mfu-0.0.8/mfu/scripts/cluster.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1199 2023-03-22 09:33:27.000000 mfu-0.0.8/mfu/scripts/config.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3748 2023-03-22 09:16:00.000000 mfu-0.0.8/mfu/scripts/doctor.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3709 2024-05-17 08:49:07.000000 mfu-0.0.8/mfu/scripts/sync.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:53:45.038613 mfu-0.0.8/mfu/utils/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-23 11:12:20.000000 mfu-0.0.8/mfu/utils/__init__.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2841 2022-11-23 11:15:13.000000 mfu-0.0.8/mfu/utils/forcelink.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3176 2023-06-20 13:21:08.000000 mfu-0.0.8/mfu/utils/general.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:53:45.038613 mfu-0.0.8/mfu.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)      895 2024-05-17 08:53:45.000000 mfu-0.0.8/mfu.egg-info/PKG-INFO
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      418 2024-05-17 08:53:45.000000 mfu-0.0.8/mfu.egg-info/SOURCES.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)        1 2024-05-17 08:53:45.000000 mfu-0.0.8/mfu.egg-info/dependency_links.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       37 2024-05-17 08:53:45.000000 mfu-0.0.8/mfu.egg-info/entry_points.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      104 2024-05-17 08:53:45.000000 mfu-0.0.8/mfu.egg-info/requires.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)        4 2024-05-17 08:53:45.000000 mfu-0.0.8/mfu.egg-info/top_level.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      516 2024-05-17 08:53:42.000000 mfu-0.0.8/pyproject.toml
+-rw-rw-r--   0 michael   (1000) michael   (1000)       38 2024-05-17 08:53:45.038613 mfu-0.0.8/setup.cfg
+-rw-rw-r--   0 michael   (1000) michael   (1000)       68 2023-03-22 08:56:38.000000 mfu-0.0.8/setup.py
```

### Comparing `mfu-0.0.7/PKG-INFO` & `mfu-0.0.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: mfu
-Version: 0.0.7
+Version: 0.0.8
 Summary: Michael's fun utilities
 Author-email: Michael Botha <michael@408.co.za>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: Click>=8.1.3
 Requires-Dist: kubernetes>=25.3.0
 Requires-Dist: watchdog>=2.1.9
 Requires-Dist: GitPython>=3.1.29
 Requires-Dist: requests>=2.28.1
+Requires-Dist: python-gitlab>=3.7.0
 
 # MFU (Michael's Fun Utilities)
 
 A collection of utilities to make my life easier and hopefully others too.
 
 
 ## Release Notes
 
+### 0.0.8
+- Fixed dependencies
+
 ### 0.0.7
 - Fixed new acumen namespace.
 
 ### 0.0.6
 - Fixed pypi config.
 
 ### 0.0.5
```

### Comparing `mfu-0.0.7/mfu/scripts/cluster.py` & `mfu-0.0.8/mfu/scripts/cluster.py`

 * *Files identical despite different names*

### Comparing `mfu-0.0.7/mfu/scripts/config.py` & `mfu-0.0.8/mfu/scripts/config.py`

 * *Files identical despite different names*

### Comparing `mfu-0.0.7/mfu/scripts/doctor.py` & `mfu-0.0.8/mfu/scripts/doctor.py`

 * *Files identical despite different names*

### Comparing `mfu-0.0.7/mfu/scripts/sync.py` & `mfu-0.0.8/mfu/scripts/sync.py`

 * *Files identical despite different names*

### Comparing `mfu-0.0.7/mfu/utils/forcelink.py` & `mfu-0.0.8/mfu/utils/forcelink.py`

 * *Files identical despite different names*

### Comparing `mfu-0.0.7/mfu/utils/general.py` & `mfu-0.0.8/mfu/utils/general.py`

 * *Files identical despite different names*

### Comparing `mfu-0.0.7/mfu.egg-info/PKG-INFO` & `mfu-0.0.8/mfu.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: mfu
-Version: 0.0.7
+Version: 0.0.8
 Summary: Michael's fun utilities
 Author-email: Michael Botha <michael@408.co.za>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: Click>=8.1.3
 Requires-Dist: kubernetes>=25.3.0
 Requires-Dist: watchdog>=2.1.9
 Requires-Dist: GitPython>=3.1.29
 Requires-Dist: requests>=2.28.1
+Requires-Dist: python-gitlab>=3.7.0
 
 # MFU (Michael's Fun Utilities)
 
 A collection of utilities to make my life easier and hopefully others too.
 
 
 ## Release Notes
 
+### 0.0.8
+- Fixed dependencies
+
 ### 0.0.7
 - Fixed new acumen namespace.
 
 ### 0.0.6
 - Fixed pypi config.
 
 ### 0.0.5
```

