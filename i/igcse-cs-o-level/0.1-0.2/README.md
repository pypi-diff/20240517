# Comparing `tmp/igcse_cs_o_level-0.1.tar.gz` & `tmp/igcse_cs_o_level-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igcse_cs_o_level-0.1.tar", last modified: Fri May 17 11:11:55 2024, max compression
+gzip compressed data, was "igcse_cs_o_level-0.2.tar", last modified: Fri May 17 11:39:51 2024, max compression
```

## Comparing `igcse_cs_o_level-0.1.tar` & `igcse_cs_o_level-0.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 11:11:55.353813 igcse_cs_o_level-0.1/
--rw-rw-rw-   0        0        0      700 2024-05-17 11:11:55.351846 igcse_cs_o_level-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-17 11:11:55.349810 igcse_cs_o_level-0.1/igcse_cs_o_level.egg-info/
--rw-rw-rw-   0        0        0      700 2024-05-17 11:11:55.000000 igcse_cs_o_level-0.1/igcse_cs_o_level.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2024-05-17 11:11:55.000000 igcse_cs_o_level-0.1/igcse_cs_o_level.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 11:11:55.000000 igcse_cs_o_level-0.1/igcse_cs_o_level.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 11:11:55.000000 igcse_cs_o_level-0.1/igcse_cs_o_level.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 11:11:55.353813 igcse_cs_o_level-0.1/setup.cfg
--rw-rw-rw-   0        0        0      976 2024-05-17 11:09:12.000000 igcse_cs_o_level-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 11:39:51.227899 igcse_cs_o_level-0.2/
+-rw-rw-rw-   0        0        0      733 2024-05-17 11:39:51.226899 igcse_cs_o_level-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-17 11:39:51.223899 igcse_cs_o_level-0.2/igcse_cs_o_level.egg-info/
+-rw-rw-rw-   0        0        0      733 2024-05-17 11:39:51.000000 igcse_cs_o_level-0.2/igcse_cs_o_level.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2024-05-17 11:39:51.000000 igcse_cs_o_level-0.2/igcse_cs_o_level.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 11:39:51.000000 igcse_cs_o_level-0.2/igcse_cs_o_level.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-17 11:39:51.000000 igcse_cs_o_level-0.2/igcse_cs_o_level.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 11:39:51.000000 igcse_cs_o_level-0.2/igcse_cs_o_level.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 11:39:51.227899 igcse_cs_o_level-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      922 2024-05-17 11:39:04.000000 igcse_cs_o_level-0.2/setup.py
```

### Comparing `igcse_cs_o_level-0.1/PKG-INFO` & `igcse_cs_o_level-0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: igcse-cs-o-level
-Version: 0.1
+Version: 0.2
 Summary: A simple Python library for IGCSE Computer Science.
 Home-page: https://github.com/DefinetlyNotAI/IG_Python_Library
 Author: Shahm Najeeb
 Author-email: Nirt_12023@outlook.com
 Keywords: igcse computer science
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
+Requires-Dist: requests>=2.25.1
```

### Comparing `igcse_cs_o_level-0.1/igcse_cs_o_level.egg-info/PKG-INFO` & `igcse_cs_o_level-0.2/igcse_cs_o_level.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: igcse-cs-o-level
-Version: 0.1
+Version: 0.2
 Summary: A simple Python library for IGCSE Computer Science.
 Home-page: https://github.com/DefinetlyNotAI/IG_Python_Library
 Author: Shahm Najeeb
 Author-email: Nirt_12023@outlook.com
 Keywords: igcse computer science
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
+Requires-Dist: requests>=2.25.1
```

