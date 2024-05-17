# Comparing `tmp/TestGeneratorPluginLib-1.2.0.tar.gz` & `tmp/TestGeneratorPluginLib-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TestGeneratorPluginLib-1.2.0.tar", last modified: Fri May 17 15:26:49 2024, max compression
+gzip compressed data, was "TestGeneratorPluginLib-1.2.1.tar", last modified: Fri May 17 15:46:28 2024, max compression
```

## Comparing `TestGeneratorPluginLib-1.2.0.tar` & `TestGeneratorPluginLib-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 15:26:49.726081 TestGeneratorPluginLib-1.2.0/
--rw-rw-rw-   0        0        0     1090 2024-05-17 15:25:53.000000 TestGeneratorPluginLib-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     1569 2024-05-17 15:26:49.726081 TestGeneratorPluginLib-1.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-17 15:26:49.726081 TestGeneratorPluginLib-1.2.0/TestGeneratorPluginLib/
--rw-rw-rw-   0        0        0      425 2024-05-17 15:25:53.000000 TestGeneratorPluginLib-1.2.0/TestGeneratorPluginLib/__init__.py
--rw-rw-rw-   0        0        0     2357 2024-05-17 15:25:53.000000 TestGeneratorPluginLib-1.2.0/TestGeneratorPluginLib/_built_plugin.py
--rw-rw-rw-   0        0        0       19 2024-05-17 15:25:53.000000 TestGeneratorPluginLib-1.2.0/TestGeneratorPluginLib/_config.py
--rw-rw-rw-   0        0        0     1839 2024-05-17 15:25:53.000000 TestGeneratorPluginLib-1.2.0/TestGeneratorPluginLib/_language.py
--rw-rw-rw-   0        0        0     1219 2024-05-17 15:25:53.000000 TestGeneratorPluginLib-1.2.0/TestGeneratorPluginLib/_managers.py
--rw-rw-rw-   0        0        0      604 2024-05-17 15:25:53.000000 TestGeneratorPluginLib-1.2.0/TestGeneratorPluginLib/_plugin.py
--rw-rw-rw-   0        0        0     2854 2024-05-17 15:25:53.000000 TestGeneratorPluginLib-1.2.0/TestGeneratorPluginLib/_plugin_setup.py
--rw-rw-rw-   0        0        0     3344 2024-05-17 15:25:53.000000 TestGeneratorPluginLib-1.2.0/TestGeneratorPluginLib/_widgets.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:26:49.726081 TestGeneratorPluginLib-1.2.0/TestGeneratorPluginLib.egg-info/
--rw-rw-rw-   0        0        0     1569 2024-05-17 15:26:49.000000 TestGeneratorPluginLib-1.2.0/TestGeneratorPluginLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2024-05-17 15:26:49.000000 TestGeneratorPluginLib-1.2.0/TestGeneratorPluginLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 15:26:49.000000 TestGeneratorPluginLib-1.2.0/TestGeneratorPluginLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-05-17 15:26:49.000000 TestGeneratorPluginLib-1.2.0/TestGeneratorPluginLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-17 15:26:49.000000 TestGeneratorPluginLib-1.2.0/TestGeneratorPluginLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 15:26:49.726081 TestGeneratorPluginLib-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1288 2024-05-17 15:25:53.000000 TestGeneratorPluginLib-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:46:28.783635 TestGeneratorPluginLib-1.2.1/
+-rw-rw-rw-   0        0        0     1090 2024-05-17 15:45:26.000000 TestGeneratorPluginLib-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     1569 2024-05-17 15:46:28.783635 TestGeneratorPluginLib-1.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-17 15:46:28.783635 TestGeneratorPluginLib-1.2.1/TestGeneratorPluginLib/
+-rw-rw-rw-   0        0        0      425 2024-05-17 15:45:26.000000 TestGeneratorPluginLib-1.2.1/TestGeneratorPluginLib/__init__.py
+-rw-rw-rw-   0        0        0     2357 2024-05-17 15:45:26.000000 TestGeneratorPluginLib-1.2.1/TestGeneratorPluginLib/_built_plugin.py
+-rw-rw-rw-   0        0        0       19 2024-05-17 15:45:26.000000 TestGeneratorPluginLib-1.2.1/TestGeneratorPluginLib/_config.py
+-rw-rw-rw-   0        0        0     1839 2024-05-17 15:45:26.000000 TestGeneratorPluginLib-1.2.1/TestGeneratorPluginLib/_language.py
+-rw-rw-rw-   0        0        0     1219 2024-05-17 15:45:26.000000 TestGeneratorPluginLib-1.2.1/TestGeneratorPluginLib/_managers.py
+-rw-rw-rw-   0        0        0      609 2024-05-17 15:45:26.000000 TestGeneratorPluginLib-1.2.1/TestGeneratorPluginLib/_plugin.py
+-rw-rw-rw-   0        0        0     2854 2024-05-17 15:45:26.000000 TestGeneratorPluginLib-1.2.1/TestGeneratorPluginLib/_plugin_setup.py
+-rw-rw-rw-   0        0        0     3344 2024-05-17 15:45:26.000000 TestGeneratorPluginLib-1.2.1/TestGeneratorPluginLib/_widgets.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:46:28.783635 TestGeneratorPluginLib-1.2.1/TestGeneratorPluginLib.egg-info/
+-rw-rw-rw-   0        0        0     1569 2024-05-17 15:46:28.000000 TestGeneratorPluginLib-1.2.1/TestGeneratorPluginLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      535 2024-05-17 15:46:28.000000 TestGeneratorPluginLib-1.2.1/TestGeneratorPluginLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 15:46:28.000000 TestGeneratorPluginLib-1.2.1/TestGeneratorPluginLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-05-17 15:46:28.000000 TestGeneratorPluginLib-1.2.1/TestGeneratorPluginLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-17 15:46:28.000000 TestGeneratorPluginLib-1.2.1/TestGeneratorPluginLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 15:46:28.783635 TestGeneratorPluginLib-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1288 2024-05-17 15:45:26.000000 TestGeneratorPluginLib-1.2.1/setup.py
```

### Comparing `TestGeneratorPluginLib-1.2.0/LICENSE` & `TestGeneratorPluginLib-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.2.0/PKG-INFO` & `TestGeneratorPluginLib-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TestGeneratorPluginLib
-Version: 1.2.0
+Version: 1.2.1
 Summary: A TestGeneratorPluginLib package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `TestGeneratorPluginLib-1.2.0/TestGeneratorPluginLib/_built_plugin.py` & `TestGeneratorPluginLib-1.2.1/TestGeneratorPluginLib/_built_plugin.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.2.0/TestGeneratorPluginLib/_language.py` & `TestGeneratorPluginLib-1.2.1/TestGeneratorPluginLib/_language.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.2.0/TestGeneratorPluginLib/_managers.py` & `TestGeneratorPluginLib-1.2.1/TestGeneratorPluginLib/_managers.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.2.0/TestGeneratorPluginLib/_plugin.py` & `TestGeneratorPluginLib-1.2.1/TestGeneratorPluginLib/_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 
 
 class Plugin:
     def __init__(self, bm):
         self.main_tabs: dict[str: Callable[[BackendManager], MainTab]] = dict()
         self.side_tabs: dict[str: Callable[[BackendManager], SideTab]] = dict()
         self.fast_run_options: dict[str, list[_FastRunOption]] = dict()
-        self.files_context_menu_options: dict[str, tuple[Callable[[], KitForm], Callable[[list], Any]]] = dict()
+        self.files_context_menu_options: dict[str, tuple[Callable[[], KitForm], Callable[[str, list], Any]]] = dict()
```

### Comparing `TestGeneratorPluginLib-1.2.0/TestGeneratorPluginLib/_plugin_setup.py` & `TestGeneratorPluginLib-1.2.1/TestGeneratorPluginLib/_plugin_setup.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.2.0/TestGeneratorPluginLib/_widgets.py` & `TestGeneratorPluginLib-1.2.1/TestGeneratorPluginLib/_widgets.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.2.0/TestGeneratorPluginLib.egg-info/PKG-INFO` & `TestGeneratorPluginLib-1.2.1/TestGeneratorPluginLib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TestGeneratorPluginLib
-Version: 1.2.0
+Version: 1.2.1
 Summary: A TestGeneratorPluginLib package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `TestGeneratorPluginLib-1.2.0/TestGeneratorPluginLib.egg-info/SOURCES.txt` & `TestGeneratorPluginLib-1.2.1/TestGeneratorPluginLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.2.0/setup.py` & `TestGeneratorPluginLib-1.2.1/setup.py`

 * *Files identical despite different names*

