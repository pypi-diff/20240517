# Comparing `tmp/TestGeneratorPluginLib-1.1.1.tar.gz` & `tmp/TestGeneratorPluginLib-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TestGeneratorPluginLib-1.1.1.tar", last modified: Thu May 16 12:38:52 2024, max compression
+gzip compressed data, was "TestGeneratorPluginLib-1.1.2.tar", last modified: Thu May 16 13:31:40 2024, max compression
```

## Comparing `TestGeneratorPluginLib-1.1.1.tar` & `TestGeneratorPluginLib-1.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 12:38:52.501874 TestGeneratorPluginLib-1.1.1/
--rw-rw-rw-   0        0        0     1090 2024-05-16 12:37:59.000000 TestGeneratorPluginLib-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     1569 2024-05-16 12:38:52.501874 TestGeneratorPluginLib-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-16 12:38:52.501874 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/
--rw-rw-rw-   0        0        0      350 2024-05-16 12:37:59.000000 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/__init__.py
--rw-rw-rw-   0        0        0     2357 2024-05-16 12:37:59.000000 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/_built_plugin.py
--rw-rw-rw-   0        0        0       19 2024-05-16 12:37:59.000000 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/_config.py
--rw-rw-rw-   0        0        0     1780 2024-05-16 12:37:59.000000 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/_language.py
--rw-rw-rw-   0        0        0     1219 2024-05-16 12:37:59.000000 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/_managers.py
--rw-rw-rw-   0        0        0      533 2024-05-16 12:37:59.000000 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/_plugin.py
--rw-rw-rw-   0        0        0     2854 2024-05-16 12:37:59.000000 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/_plugin_setup.py
--rw-rw-rw-   0        0        0     3344 2024-05-16 12:37:59.000000 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/_widgets.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:38:52.501874 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib.egg-info/
--rw-rw-rw-   0        0        0     1569 2024-05-16 12:38:52.000000 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2024-05-16 12:38:52.000000 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 12:38:52.000000 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-16 12:38:52.000000 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-16 12:38:52.000000 TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 12:38:52.501874 TestGeneratorPluginLib-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1288 2024-05-16 12:37:59.000000 TestGeneratorPluginLib-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:31:40.276308 TestGeneratorPluginLib-1.1.2/
+-rw-rw-rw-   0        0        0     1090 2024-05-16 13:30:42.000000 TestGeneratorPluginLib-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1569 2024-05-16 13:31:40.276308 TestGeneratorPluginLib-1.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 13:31:40.260684 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/
+-rw-rw-rw-   0        0        0      403 2024-05-16 13:30:42.000000 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/__init__.py
+-rw-rw-rw-   0        0        0     2357 2024-05-16 13:30:42.000000 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/_built_plugin.py
+-rw-rw-rw-   0        0        0       19 2024-05-16 13:30:42.000000 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/_config.py
+-rw-rw-rw-   0        0        0     1780 2024-05-16 13:30:42.000000 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/_language.py
+-rw-rw-rw-   0        0        0     1219 2024-05-16 13:30:42.000000 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/_managers.py
+-rw-rw-rw-   0        0        0      533 2024-05-16 13:30:42.000000 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/_plugin.py
+-rw-rw-rw-   0        0        0     2854 2024-05-16 13:30:42.000000 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/_plugin_setup.py
+-rw-rw-rw-   0        0        0     3344 2024-05-16 13:30:42.000000 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/_widgets.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:31:40.276308 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib.egg-info/
+-rw-rw-rw-   0        0        0     1569 2024-05-16 13:31:40.000000 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      535 2024-05-16 13:31:40.000000 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 13:31:40.000000 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-16 13:31:40.000000 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-16 13:31:40.000000 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 13:31:40.276308 TestGeneratorPluginLib-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1288 2024-05-16 13:30:42.000000 TestGeneratorPluginLib-1.1.2/setup.py
```

### Comparing `TestGeneratorPluginLib-1.1.1/LICENSE` & `TestGeneratorPluginLib-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.1.1/PKG-INFO` & `TestGeneratorPluginLib-1.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TestGeneratorPluginLib
-Version: 1.1.1
+Version: 1.1.2
 Summary: A TestGeneratorPluginLib package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/_built_plugin.py` & `TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/_built_plugin.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/_language.py` & `TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/_language.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/_managers.py` & `TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/_managers.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/_plugin.py` & `TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/_plugin.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/_plugin_setup.py` & `TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/_plugin_setup.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib/_widgets.py` & `TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/_widgets.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib.egg-info/PKG-INFO` & `TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TestGeneratorPluginLib
-Version: 1.1.1
+Version: 1.1.2
 Summary: A TestGeneratorPluginLib package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `TestGeneratorPluginLib-1.1.1/TestGeneratorPluginLib.egg-info/SOURCES.txt` & `TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.1.1/setup.py` & `TestGeneratorPluginLib-1.1.2/setup.py`

 * *Files identical despite different names*

