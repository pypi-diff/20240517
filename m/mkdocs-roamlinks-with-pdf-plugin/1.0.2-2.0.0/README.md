# Comparing `tmp/mkdocs-roamlinks-with-pdf-plugin-1.0.2.tar.gz` & `tmp/mkdocs-roamlinks-with-pdf-plugin-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-roamlinks-with-pdf-plugin-1.0.2.tar", last modified: Fri May 17 09:20:48 2024, max compression
+gzip compressed data, was "mkdocs-roamlinks-with-pdf-plugin-2.0.0.tar", last modified: Fri May 17 09:23:53 2024, max compression
```

## Comparing `mkdocs-roamlinks-with-pdf-plugin-1.0.2.tar` & `mkdocs-roamlinks-with-pdf-plugin-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 09:20:48.032966 mkdocs-roamlinks-with-pdf-plugin-1.0.2/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1055 2024-05-17 07:39:54.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.2/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)      870 2024-05-17 09:20:48.032966 mkdocs-roamlinks-with-pdf-plugin-1.0.2/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1598 2024-05-17 07:41:28.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.2/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 09:20:48.032966 mkdocs-roamlinks-with-pdf-plugin-1.0.2/mkdocs_roamlinks_with_pdf_plugin/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-17 07:37:28.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.2/mkdocs_roamlinks_with_pdf_plugin/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10642 2024-05-17 09:19:20.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.2/mkdocs_roamlinks_with_pdf_plugin/plugin.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 09:20:48.032966 mkdocs-roamlinks-with-pdf-plugin-1.0.2/mkdocs_roamlinks_with_pdf_plugin.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)      870 2024-05-17 09:20:47.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.2/mkdocs_roamlinks_with_pdf_plugin.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      491 2024-05-17 09:20:47.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.2/mkdocs_roamlinks_with_pdf_plugin.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-17 09:20:47.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.2/mkdocs_roamlinks_with_pdf_plugin.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       94 2024-05-17 09:20:47.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.2/mkdocs_roamlinks_with_pdf_plugin.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       28 2024-05-17 09:20:47.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.2/mkdocs_roamlinks_with_pdf_plugin.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       39 2024-05-17 09:20:47.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.2/mkdocs_roamlinks_with_pdf_plugin.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-17 09:20:48.032966 mkdocs-roamlinks-with-pdf-plugin-1.0.2/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1181 2024-05-17 09:20:46.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.2/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 09:20:48.032966 mkdocs-roamlinks-with-pdf-plugin-1.0.2/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-17 07:37:28.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.2/tests/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5273 2024-05-17 07:37:28.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.2/tests/test_plugin.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 09:23:53.460964 mkdocs-roamlinks-with-pdf-plugin-2.0.0/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1055 2024-05-17 07:39:54.000000 mkdocs-roamlinks-with-pdf-plugin-2.0.0/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      870 2024-05-17 09:23:53.460964 mkdocs-roamlinks-with-pdf-plugin-2.0.0/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1598 2024-05-17 07:41:28.000000 mkdocs-roamlinks-with-pdf-plugin-2.0.0/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 09:23:53.456964 mkdocs-roamlinks-with-pdf-plugin-2.0.0/mkdocs_roamlinks_with_pdf_plugin/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-17 07:37:28.000000 mkdocs-roamlinks-with-pdf-plugin-2.0.0/mkdocs_roamlinks_with_pdf_plugin/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10642 2024-05-17 09:19:20.000000 mkdocs-roamlinks-with-pdf-plugin-2.0.0/mkdocs_roamlinks_with_pdf_plugin/plugin.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 09:23:53.456964 mkdocs-roamlinks-with-pdf-plugin-2.0.0/mkdocs_roamlinks_with_pdf_plugin.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      870 2024-05-17 09:23:53.000000 mkdocs-roamlinks-with-pdf-plugin-2.0.0/mkdocs_roamlinks_with_pdf_plugin.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      491 2024-05-17 09:23:53.000000 mkdocs-roamlinks-with-pdf-plugin-2.0.0/mkdocs_roamlinks_with_pdf_plugin.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-17 09:23:53.000000 mkdocs-roamlinks-with-pdf-plugin-2.0.0/mkdocs_roamlinks_with_pdf_plugin.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       94 2024-05-17 09:23:53.000000 mkdocs-roamlinks-with-pdf-plugin-2.0.0/mkdocs_roamlinks_with_pdf_plugin.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       28 2024-05-17 09:23:53.000000 mkdocs-roamlinks-with-pdf-plugin-2.0.0/mkdocs_roamlinks_with_pdf_plugin.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       39 2024-05-17 09:23:53.000000 mkdocs-roamlinks-with-pdf-plugin-2.0.0/mkdocs_roamlinks_with_pdf_plugin.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-17 09:23:53.460964 mkdocs-roamlinks-with-pdf-plugin-2.0.0/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1181 2024-05-17 09:23:46.000000 mkdocs-roamlinks-with-pdf-plugin-2.0.0/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 09:23:53.460964 mkdocs-roamlinks-with-pdf-plugin-2.0.0/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-17 07:37:28.000000 mkdocs-roamlinks-with-pdf-plugin-2.0.0/tests/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5273 2024-05-17 07:37:28.000000 mkdocs-roamlinks-with-pdf-plugin-2.0.0/tests/test_plugin.py
```

### Comparing `mkdocs-roamlinks-with-pdf-plugin-1.0.2/LICENSE` & `mkdocs-roamlinks-with-pdf-plugin-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-roamlinks-with-pdf-plugin-1.0.2/PKG-INFO` & `mkdocs-roamlinks-with-pdf-plugin-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-roamlinks-with-pdf-plugin
-Version: 1.0.2
+Version: 2.0.0
 Summary: An MkDocs plugin
 Home-page: https://github.com/jokulab/mkdocs-roamlinks-plugin
 Author: jokulab
 Author-email: 166611085+jokudev@users.noreply.github.com
 License: MIT
 Keywords: mkdocs
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-roamlinks-with-pdf-plugin-1.0.2/README.md` & `mkdocs-roamlinks-with-pdf-plugin-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-roamlinks-with-pdf-plugin-1.0.2/mkdocs_roamlinks_with_pdf_plugin/plugin.py` & `mkdocs-roamlinks-with-pdf-plugin-2.0.0/mkdocs_roamlinks_with_pdf_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-roamlinks-with-pdf-plugin-1.0.2/mkdocs_roamlinks_with_pdf_plugin.egg-info/PKG-INFO` & `mkdocs-roamlinks-with-pdf-plugin-2.0.0/mkdocs_roamlinks_with_pdf_plugin.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-roamlinks-with-pdf-plugin
-Version: 1.0.2
+Version: 2.0.0
 Summary: An MkDocs plugin
 Home-page: https://github.com/jokulab/mkdocs-roamlinks-plugin
 Author: jokulab
 Author-email: 166611085+jokudev@users.noreply.github.com
 License: MIT
 Keywords: mkdocs
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-roamlinks-with-pdf-plugin-1.0.2/setup.py` & `mkdocs-roamlinks-with-pdf-plugin-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mkdocs-roamlinks-with-pdf-plugin',
-    version='1.0.2',
+    version='2.0.0',
     description='An MkDocs plugin',
     long_description='An MkDocs plugin that automagically generates relative links and convert roamlike links for foam and obsidian between markdown pages',
     keywords='mkdocs',
     url= 'https://github.com/jokulab/mkdocs-roamlinks-plugin',
     author='jokulab',
     author_email='166611085+jokudev@users.noreply.github.com',
     license='MIT',
```

### Comparing `mkdocs-roamlinks-with-pdf-plugin-1.0.2/tests/test_plugin.py` & `mkdocs-roamlinks-with-pdf-plugin-2.0.0/tests/test_plugin.py`

 * *Files identical despite different names*

