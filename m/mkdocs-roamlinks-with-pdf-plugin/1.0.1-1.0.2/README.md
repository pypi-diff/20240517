# Comparing `tmp/mkdocs-roamlinks-with-pdf-plugin-1.0.1.tar.gz` & `tmp/mkdocs-roamlinks-with-pdf-plugin-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-roamlinks-with-pdf-plugin-1.0.1.tar", last modified: Fri May 17 09:13:08 2024, max compression
+gzip compressed data, was "mkdocs-roamlinks-with-pdf-plugin-1.0.2.tar", last modified: Fri May 17 09:20:48 2024, max compression
```

## Comparing `mkdocs-roamlinks-with-pdf-plugin-1.0.1.tar` & `mkdocs-roamlinks-with-pdf-plugin-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 09:13:08.232968 mkdocs-roamlinks-with-pdf-plugin-1.0.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1055 2024-05-17 07:39:54.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.1/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)      870 2024-05-17 09:13:08.232968 mkdocs-roamlinks-with-pdf-plugin-1.0.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1598 2024-05-17 07:41:28.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.1/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 09:13:08.228968 mkdocs-roamlinks-with-pdf-plugin-1.0.1/mkdocs_roamlinks_with_pdf_plugin/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-17 07:37:28.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.1/mkdocs_roamlinks_with_pdf_plugin/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10672 2024-05-17 09:08:28.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.1/mkdocs_roamlinks_with_pdf_plugin/plugin.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 09:13:08.232968 mkdocs-roamlinks-with-pdf-plugin-1.0.1/mkdocs_roamlinks_with_pdf_plugin.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)      870 2024-05-17 09:13:08.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.1/mkdocs_roamlinks_with_pdf_plugin.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      491 2024-05-17 09:13:08.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.1/mkdocs_roamlinks_with_pdf_plugin.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-17 09:13:08.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.1/mkdocs_roamlinks_with_pdf_plugin.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       94 2024-05-17 09:13:08.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.1/mkdocs_roamlinks_with_pdf_plugin.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       28 2024-05-17 09:13:08.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.1/mkdocs_roamlinks_with_pdf_plugin.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       39 2024-05-17 09:13:08.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.1/mkdocs_roamlinks_with_pdf_plugin.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-17 09:13:08.232968 mkdocs-roamlinks-with-pdf-plugin-1.0.1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1181 2024-05-17 09:09:39.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.1/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 09:13:08.232968 mkdocs-roamlinks-with-pdf-plugin-1.0.1/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-17 07:37:28.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.1/tests/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5273 2024-05-17 07:37:28.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.1/tests/test_plugin.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 09:20:48.032966 mkdocs-roamlinks-with-pdf-plugin-1.0.2/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1055 2024-05-17 07:39:54.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.2/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      870 2024-05-17 09:20:48.032966 mkdocs-roamlinks-with-pdf-plugin-1.0.2/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1598 2024-05-17 07:41:28.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.2/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 09:20:48.032966 mkdocs-roamlinks-with-pdf-plugin-1.0.2/mkdocs_roamlinks_with_pdf_plugin/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-17 07:37:28.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.2/mkdocs_roamlinks_with_pdf_plugin/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10642 2024-05-17 09:19:20.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.2/mkdocs_roamlinks_with_pdf_plugin/plugin.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 09:20:48.032966 mkdocs-roamlinks-with-pdf-plugin-1.0.2/mkdocs_roamlinks_with_pdf_plugin.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      870 2024-05-17 09:20:47.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.2/mkdocs_roamlinks_with_pdf_plugin.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      491 2024-05-17 09:20:47.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.2/mkdocs_roamlinks_with_pdf_plugin.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-17 09:20:47.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.2/mkdocs_roamlinks_with_pdf_plugin.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       94 2024-05-17 09:20:47.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.2/mkdocs_roamlinks_with_pdf_plugin.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       28 2024-05-17 09:20:47.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.2/mkdocs_roamlinks_with_pdf_plugin.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       39 2024-05-17 09:20:47.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.2/mkdocs_roamlinks_with_pdf_plugin.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-17 09:20:48.032966 mkdocs-roamlinks-with-pdf-plugin-1.0.2/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1181 2024-05-17 09:20:46.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.2/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-17 09:20:48.032966 mkdocs-roamlinks-with-pdf-plugin-1.0.2/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-17 07:37:28.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.2/tests/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5273 2024-05-17 07:37:28.000000 mkdocs-roamlinks-with-pdf-plugin-1.0.2/tests/test_plugin.py
```

### Comparing `mkdocs-roamlinks-with-pdf-plugin-1.0.1/LICENSE` & `mkdocs-roamlinks-with-pdf-plugin-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-roamlinks-with-pdf-plugin-1.0.1/PKG-INFO` & `mkdocs-roamlinks-with-pdf-plugin-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-roamlinks-with-pdf-plugin
-Version: 1.0.1
+Version: 1.0.2
 Summary: An MkDocs plugin
 Home-page: https://github.com/jokulab/mkdocs-roamlinks-plugin
 Author: jokulab
 Author-email: 166611085+jokudev@users.noreply.github.com
 License: MIT
 Keywords: mkdocs
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-roamlinks-with-pdf-plugin-1.0.1/README.md` & `mkdocs-roamlinks-with-pdf-plugin-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-roamlinks-with-pdf-plugin-1.0.1/mkdocs_roamlinks_with_pdf_plugin/plugin.py` & `mkdocs-roamlinks-with-pdf-plugin-1.0.2/mkdocs_roamlinks_with_pdf_plugin/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,15 @@
                             os.path.relpath(abs_link_url, abs_linker_url), os.path.basename(rel_file))
                     if height:
                         rel_link_url = rel_link_url + height
             else:
                 for root, dirs, files in os.walk(self.base_docs_url, followlinks=True):
                     for name in files:
                         # If we have a match, create the relative path from linker to the link
-                        if self.simplify(name) == self.simplify(filename):
+                        if name == filename:
                             # Absolute path to the file we want to link to
                             abs_link_url = os.path.dirname(os.path.join(
                                 root, name))
                             # Constructing relative path from the linker to the link
                             rel_link_url = os.path.join(
                                     os.path.relpath(abs_link_url, abs_linker_url), name)
                             if height:
```

### Comparing `mkdocs-roamlinks-with-pdf-plugin-1.0.1/mkdocs_roamlinks_with_pdf_plugin.egg-info/PKG-INFO` & `mkdocs-roamlinks-with-pdf-plugin-1.0.2/mkdocs_roamlinks_with_pdf_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-roamlinks-with-pdf-plugin
-Version: 1.0.1
+Version: 1.0.2
 Summary: An MkDocs plugin
 Home-page: https://github.com/jokulab/mkdocs-roamlinks-plugin
 Author: jokulab
 Author-email: 166611085+jokudev@users.noreply.github.com
 License: MIT
 Keywords: mkdocs
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-roamlinks-with-pdf-plugin-1.0.1/setup.py` & `mkdocs-roamlinks-with-pdf-plugin-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mkdocs-roamlinks-with-pdf-plugin',
-    version='1.0.1',
+    version='1.0.2',
     description='An MkDocs plugin',
     long_description='An MkDocs plugin that automagically generates relative links and convert roamlike links for foam and obsidian between markdown pages',
     keywords='mkdocs',
     url= 'https://github.com/jokulab/mkdocs-roamlinks-plugin',
     author='jokulab',
     author_email='166611085+jokudev@users.noreply.github.com',
     license='MIT',
```

### Comparing `mkdocs-roamlinks-with-pdf-plugin-1.0.1/tests/test_plugin.py` & `mkdocs-roamlinks-with-pdf-plugin-1.0.2/tests/test_plugin.py`

 * *Files identical despite different names*

