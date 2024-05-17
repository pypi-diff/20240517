# Comparing `tmp/TestGeneratorPluginLib-1.1.2.tar.gz` & `tmp/TestGeneratorPluginLib-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TestGeneratorPluginLib-1.1.2.tar", last modified: Thu May 16 13:31:40 2024, max compression
+gzip compressed data, was "TestGeneratorPluginLib-1.1.3.tar", last modified: Fri May 17 10:55:13 2024, max compression
```

## Comparing `TestGeneratorPluginLib-1.1.2.tar` & `TestGeneratorPluginLib-1.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 13:31:40.276308 TestGeneratorPluginLib-1.1.2/
--rw-rw-rw-   0        0        0     1090 2024-05-16 13:30:42.000000 TestGeneratorPluginLib-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     1569 2024-05-16 13:31:40.276308 TestGeneratorPluginLib-1.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-16 13:31:40.260684 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/
--rw-rw-rw-   0        0        0      403 2024-05-16 13:30:42.000000 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/__init__.py
--rw-rw-rw-   0        0        0     2357 2024-05-16 13:30:42.000000 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/_built_plugin.py
--rw-rw-rw-   0        0        0       19 2024-05-16 13:30:42.000000 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/_config.py
--rw-rw-rw-   0        0        0     1780 2024-05-16 13:30:42.000000 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/_language.py
--rw-rw-rw-   0        0        0     1219 2024-05-16 13:30:42.000000 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/_managers.py
--rw-rw-rw-   0        0        0      533 2024-05-16 13:30:42.000000 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/_plugin.py
--rw-rw-rw-   0        0        0     2854 2024-05-16 13:30:42.000000 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/_plugin_setup.py
--rw-rw-rw-   0        0        0     3344 2024-05-16 13:30:42.000000 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/_widgets.py
-drwxrwxrwx   0        0        0        0 2024-05-16 13:31:40.276308 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib.egg-info/
--rw-rw-rw-   0        0        0     1569 2024-05-16 13:31:40.000000 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2024-05-16 13:31:40.000000 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 13:31:40.000000 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-16 13:31:40.000000 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-16 13:31:40.000000 TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 13:31:40.276308 TestGeneratorPluginLib-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1288 2024-05-16 13:30:42.000000 TestGeneratorPluginLib-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:55:13.544717 TestGeneratorPluginLib-1.1.3/
+-rw-rw-rw-   0        0        0     1090 2024-05-17 10:54:25.000000 TestGeneratorPluginLib-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1569 2024-05-17 10:55:13.544717 TestGeneratorPluginLib-1.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-17 10:55:13.529129 TestGeneratorPluginLib-1.1.3/TestGeneratorPluginLib/
+-rw-rw-rw-   0        0        0      403 2024-05-17 10:54:25.000000 TestGeneratorPluginLib-1.1.3/TestGeneratorPluginLib/__init__.py
+-rw-rw-rw-   0        0        0     2357 2024-05-17 10:54:25.000000 TestGeneratorPluginLib-1.1.3/TestGeneratorPluginLib/_built_plugin.py
+-rw-rw-rw-   0        0        0       19 2024-05-17 10:54:25.000000 TestGeneratorPluginLib-1.1.3/TestGeneratorPluginLib/_config.py
+-rw-rw-rw-   0        0        0     1839 2024-05-17 10:54:25.000000 TestGeneratorPluginLib-1.1.3/TestGeneratorPluginLib/_language.py
+-rw-rw-rw-   0        0        0     1219 2024-05-17 10:54:25.000000 TestGeneratorPluginLib-1.1.3/TestGeneratorPluginLib/_managers.py
+-rw-rw-rw-   0        0        0      533 2024-05-17 10:54:25.000000 TestGeneratorPluginLib-1.1.3/TestGeneratorPluginLib/_plugin.py
+-rw-rw-rw-   0        0        0     2854 2024-05-17 10:54:25.000000 TestGeneratorPluginLib-1.1.3/TestGeneratorPluginLib/_plugin_setup.py
+-rw-rw-rw-   0        0        0     3344 2024-05-17 10:54:25.000000 TestGeneratorPluginLib-1.1.3/TestGeneratorPluginLib/_widgets.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:55:13.544717 TestGeneratorPluginLib-1.1.3/TestGeneratorPluginLib.egg-info/
+-rw-rw-rw-   0        0        0     1569 2024-05-17 10:55:13.000000 TestGeneratorPluginLib-1.1.3/TestGeneratorPluginLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      535 2024-05-17 10:55:13.000000 TestGeneratorPluginLib-1.1.3/TestGeneratorPluginLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 10:55:13.000000 TestGeneratorPluginLib-1.1.3/TestGeneratorPluginLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-17 10:55:13.000000 TestGeneratorPluginLib-1.1.3/TestGeneratorPluginLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-17 10:55:13.000000 TestGeneratorPluginLib-1.1.3/TestGeneratorPluginLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 10:55:13.544717 TestGeneratorPluginLib-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1288 2024-05-17 10:54:25.000000 TestGeneratorPluginLib-1.1.3/setup.py
```

### Comparing `TestGeneratorPluginLib-1.1.2/LICENSE` & `TestGeneratorPluginLib-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.1.2/PKG-INFO` & `TestGeneratorPluginLib-1.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TestGeneratorPluginLib
-Version: 1.1.2
+Version: 1.1.3
 Summary: A TestGeneratorPluginLib package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/_built_plugin.py` & `TestGeneratorPluginLib-1.1.3/TestGeneratorPluginLib/_built_plugin.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/_language.py` & `TestGeneratorPluginLib-1.1.3/TestGeneratorPluginLib/_language.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,9 +57,13 @@
         return self._function(path, bm)
 
 
 class FastRunFunction(_FastRunOption):
     pass
 
 
+class FastRunAsyncFunction(_FastRunOption):
+    pass
+
+
 class FastRunCommand(_FastRunOption):
     pass
```

### Comparing `TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/_managers.py` & `TestGeneratorPluginLib-1.1.3/TestGeneratorPluginLib/_managers.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/_plugin.py` & `TestGeneratorPluginLib-1.1.3/TestGeneratorPluginLib/_plugin.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/_plugin_setup.py` & `TestGeneratorPluginLib-1.1.3/TestGeneratorPluginLib/_plugin_setup.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 import sys
 from sys import argv
 from typing import Iterable
 
 
 class PluginSetup:
     def __init__(self,
-                 plugin: str,
                  name: str,
                  description: str,
                  version: str,
                  author: str,
+                 plugin: str,
                  url='',
                  platform_specific: bool = None,
                  dependencies: Iterable[str] = tuple(),
                  conflicts: Iterable[str] = tuple(),
 
                  directories: Iterable[str] = tuple(),
                  requirements: Iterable[str] = tuple(),
```

### Comparing `TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib/_widgets.py` & `TestGeneratorPluginLib-1.1.3/TestGeneratorPluginLib/_widgets.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib.egg-info/PKG-INFO` & `TestGeneratorPluginLib-1.1.3/TestGeneratorPluginLib.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TestGeneratorPluginLib
-Version: 1.1.2
+Version: 1.1.3
 Summary: A TestGeneratorPluginLib package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `TestGeneratorPluginLib-1.1.2/TestGeneratorPluginLib.egg-info/SOURCES.txt` & `TestGeneratorPluginLib-1.1.3/TestGeneratorPluginLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.1.2/setup.py` & `TestGeneratorPluginLib-1.1.3/setup.py`

 * *Files identical despite different names*

