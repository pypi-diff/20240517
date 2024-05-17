# Comparing `tmp/miska-0.0.1.tar.gz` & `tmp/miska-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miska-0.0.1.tar", last modified: Fri Mar  8 13:07:56 2024, max compression
+gzip compressed data, was "miska-0.0.2.tar", last modified: Fri May 17 18:14:48 2024, max compression
```

## Comparing `miska-0.0.1.tar` & `miska-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-03-08 13:07:56.355856 miska-0.0.1/
--rw-r--r--   0 cell      (1000) cell      (1000)     1289 2024-03-08 12:58:53.000000 miska-0.0.1/LICENSE
--rw-r--r--   0 cell      (1000) cell      (1000)     2728 2024-03-08 13:07:56.355856 miska-0.0.1/PKG-INFO
--rw-r--r--   0 cell      (1000) cell      (1000)      578 2024-03-08 13:07:03.000000 miska-0.0.1/README.rst
-drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-03-08 13:07:56.352856 miska-0.0.1/miska/
--rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-01-16 00:44:30.000000 miska-0.0.1/miska/__init__.py
--rw-r--r--   0 cell      (1000) cell      (1000)      222 2024-01-16 00:44:30.000000 miska-0.0.1/miska/mixins.py
--rw-r--r--   0 cell      (1000) cell      (1000)      640 2024-01-17 08:22:43.000000 miska-0.0.1/miska/registry.py
-drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-03-08 13:07:56.353856 miska-0.0.1/miska/types/
--rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-01-16 00:44:30.000000 miska-0.0.1/miska/types/__init__.py
-drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-03-08 13:07:56.354856 miska-0.0.1/miska/types/network/
--rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-01-16 00:44:30.000000 miska-0.0.1/miska/types/network/__init__.py
--rw-r--r--   0 cell      (1000) cell      (1000)     3206 2024-01-17 08:08:06.000000 miska-0.0.1/miska/types/network/bgp.py
-drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-03-08 13:07:56.354856 miska-0.0.1/miska.egg-info/
--rw-r--r--   0 cell      (1000) cell      (1000)     2728 2024-03-08 13:07:56.000000 miska-0.0.1/miska.egg-info/PKG-INFO
--rw-r--r--   0 cell      (1000) cell      (1000)      307 2024-03-08 13:07:56.000000 miska-0.0.1/miska.egg-info/SOURCES.txt
--rw-r--r--   0 cell      (1000) cell      (1000)        1 2024-03-08 13:07:56.000000 miska-0.0.1/miska.egg-info/dependency_links.txt
--rw-r--r--   0 cell      (1000) cell      (1000)        6 2024-03-08 13:07:56.000000 miska-0.0.1/miska.egg-info/top_level.txt
--rw-r--r--   0 cell      (1000) cell      (1000)      768 2024-03-08 13:06:16.000000 miska-0.0.1/pyproject.toml
--rw-r--r--   0 cell      (1000) cell      (1000)       38 2024-03-08 13:07:56.355856 miska-0.0.1/setup.cfg
-drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-03-08 13:07:56.354856 miska-0.0.1/tests/
--rw-r--r--   0 cell      (1000) cell      (1000)      209 2024-03-08 12:58:21.000000 miska-0.0.1/tests/test_registry.py
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-17 18:14:48.355019 miska-0.0.2/
+-rw-r--r--   0 cell      (1000) cell      (1000)     1289 2024-03-09 16:24:22.000000 miska-0.0.2/LICENSE
+-rw-r--r--   0 cell      (1000) cell      (1000)     2853 2024-05-17 18:14:48.354019 miska-0.0.2/PKG-INFO
+-rw-r--r--   0 cell      (1000) cell      (1000)      578 2024-03-09 16:24:22.000000 miska-0.0.2/README.rst
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-17 18:14:48.346019 miska-0.0.2/miska/
+-rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.2/miska/__init__.py
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-17 18:14:48.351019 miska-0.0.2/miska/http/
+-rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.2/miska/http/__init__.py
+-rw-r--r--   0 cell      (1000) cell      (1000)     1395 2024-03-09 16:24:22.000000 miska-0.0.2/miska/http/rs.py
+-rw-r--r--   0 cell      (1000) cell      (1000)      222 2024-03-09 16:24:22.000000 miska-0.0.2/miska/mixins.py
+-rw-r--r--   0 cell      (1000) cell      (1000)     1531 2024-05-17 13:52:44.000000 miska-0.0.2/miska/registries.py
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-17 18:14:48.351019 miska-0.0.2/miska/types/
+-rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.2/miska/types/__init__.py
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-17 18:14:48.352019 miska-0.0.2/miska/types/network/
+-rw-r--r--   0 cell      (1000) cell      (1000)        0 2024-03-09 16:24:22.000000 miska-0.0.2/miska/types/network/__init__.py
+-rw-r--r--   0 cell      (1000) cell      (1000)     3206 2024-03-09 16:24:22.000000 miska-0.0.2/miska/types/network/bgp.py
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-17 18:14:48.353019 miska-0.0.2/miska.egg-info/
+-rw-r--r--   0 cell      (1000) cell      (1000)     2853 2024-05-17 18:14:48.000000 miska-0.0.2/miska.egg-info/PKG-INFO
+-rw-r--r--   0 cell      (1000) cell      (1000)      379 2024-05-17 18:14:48.000000 miska-0.0.2/miska.egg-info/SOURCES.txt
+-rw-r--r--   0 cell      (1000) cell      (1000)        1 2024-05-17 18:14:48.000000 miska-0.0.2/miska.egg-info/dependency_links.txt
+-rw-r--r--   0 cell      (1000) cell      (1000)       36 2024-05-17 18:14:48.000000 miska-0.0.2/miska.egg-info/requires.txt
+-rw-r--r--   0 cell      (1000) cell      (1000)        6 2024-05-17 18:14:48.000000 miska-0.0.2/miska.egg-info/top_level.txt
+-rw-r--r--   0 cell      (1000) cell      (1000)      843 2024-05-17 18:11:31.000000 miska-0.0.2/pyproject.toml
+-rw-r--r--   0 cell      (1000) cell      (1000)       38 2024-05-17 18:14:48.355019 miska-0.0.2/setup.cfg
+drwxr-xr-x   0 cell      (1000) cell      (1000)        0 2024-05-17 18:14:48.353019 miska-0.0.2/tests/
+-rw-r--r--   0 cell      (1000) cell      (1000)      275 2024-05-17 18:10:11.000000 miska-0.0.2/tests/test_registries.py
```

### Comparing `miska-0.0.1/LICENSE` & `miska-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `miska-0.0.1/PKG-INFO` & `miska-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miska
-Version: 0.0.1
+Version: 0.0.2
 Summary: An exceptional library
 Author-email: Dima Burmistrov <pyctrl.dev@gmail.com>
 License: Copyright (c) 2023-2024 Dmitry Burmistrov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -35,14 +35,18 @@
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Provides-Extra: http
+Requires-Dist: requests; extra == "http"
+Provides-Extra: all
+Requires-Dist: miska[http]; extra == "all"
 
 Miska
 #####
 
 Package with **miska**-llaneous code, tools and stuff
```

### Comparing `miska-0.0.1/README.rst` & `miska-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `miska-0.0.1/miska/types/network/bgp.py` & `miska-0.0.2/miska/types/network/bgp.py`

 * *Files identical despite different names*

### Comparing `miska-0.0.1/miska.egg-info/PKG-INFO` & `miska-0.0.2/miska.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miska
-Version: 0.0.1
+Version: 0.0.2
 Summary: An exceptional library
 Author-email: Dima Burmistrov <pyctrl.dev@gmail.com>
 License: Copyright (c) 2023-2024 Dmitry Burmistrov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -35,14 +35,18 @@
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Provides-Extra: http
+Requires-Dist: requests; extra == "http"
+Provides-Extra: all
+Requires-Dist: miska[http]; extra == "all"
 
 Miska
 #####
 
 Package with **miska**-llaneous code, tools and stuff
```

