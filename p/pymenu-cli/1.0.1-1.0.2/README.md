# Comparing `tmp/pymenu_cli-1.0.1.tar.gz` & `tmp/pymenu_cli-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymenu_cli-1.0.1.tar", last modified: Fri May 17 19:15:13 2024, max compression
+gzip compressed data, was "pymenu_cli-1.0.2.tar", last modified: Fri May 17 19:24:38 2024, max compression
```

## Comparing `pymenu_cli-1.0.1.tar` & `pymenu_cli-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-17 19:15:13.442839 pymenu_cli-1.0.1/
--rw-r--r--   0 moraneus   (501) staff       (20)     2807 2024-05-17 19:15:13.442627 pymenu_cli-1.0.1/PKG-INFO
--rw-r--r--   0 moraneus   (501) staff       (20)     2587 2024-05-17 18:53:28.000000 pymenu_cli-1.0.1/README.md
-drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-17 19:15:13.441471 pymenu_cli-1.0.1/pymenu_cli/
--rw-r--r--   0 moraneus   (501) staff       (20)        0 2024-05-17 18:45:03.000000 pymenu_cli-1.0.1/pymenu_cli/__init__.py
--rw-r--r--   0 moraneus   (501) staff       (20)     5117 2024-05-17 18:51:29.000000 pymenu_cli-1.0.1/pymenu_cli/menu.py
-drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-17 19:15:13.442438 pymenu_cli-1.0.1/pymenu_cli.egg-info/
--rw-r--r--   0 moraneus   (501) staff       (20)     2807 2024-05-17 19:15:13.000000 pymenu_cli-1.0.1/pymenu_cli.egg-info/PKG-INFO
--rw-r--r--   0 moraneus   (501) staff       (20)      233 2024-05-17 19:15:13.000000 pymenu_cli-1.0.1/pymenu_cli.egg-info/SOURCES.txt
--rw-r--r--   0 moraneus   (501) staff       (20)        1 2024-05-17 19:15:13.000000 pymenu_cli-1.0.1/pymenu_cli.egg-info/dependency_links.txt
--rw-r--r--   0 moraneus   (501) staff       (20)       52 2024-05-17 19:15:13.000000 pymenu_cli-1.0.1/pymenu_cli.egg-info/entry_points.txt
--rw-r--r--   0 moraneus   (501) staff       (20)       11 2024-05-17 19:15:13.000000 pymenu_cli-1.0.1/pymenu_cli.egg-info/top_level.txt
--rw-r--r--   0 moraneus   (501) staff       (20)       38 2024-05-17 19:15:13.442878 pymenu_cli-1.0.1/setup.cfg
--rw-r--r--   0 moraneus   (501) staff       (20)      594 2024-05-17 19:15:09.000000 pymenu_cli-1.0.1/setup.py
+drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-17 19:24:38.306050 pymenu_cli-1.0.2/
+-rw-r--r--   0 moraneus   (501) staff       (20)     2867 2024-05-17 19:24:38.305857 pymenu_cli-1.0.2/PKG-INFO
+-rw-r--r--   0 moraneus   (501) staff       (20)     2587 2024-05-17 18:53:28.000000 pymenu_cli-1.0.2/README.md
+drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-17 19:24:38.304319 pymenu_cli-1.0.2/pymenu_cli/
+-rw-r--r--   0 moraneus   (501) staff       (20)        0 2024-05-17 18:45:03.000000 pymenu_cli-1.0.2/pymenu_cli/__init__.py
+-rw-r--r--   0 moraneus   (501) staff       (20)     5117 2024-05-17 18:51:29.000000 pymenu_cli-1.0.2/pymenu_cli/menu.py
+drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-17 19:24:38.305680 pymenu_cli-1.0.2/pymenu_cli.egg-info/
+-rw-r--r--   0 moraneus   (501) staff       (20)     2867 2024-05-17 19:24:38.000000 pymenu_cli-1.0.2/pymenu_cli.egg-info/PKG-INFO
+-rw-r--r--   0 moraneus   (501) staff       (20)      233 2024-05-17 19:24:38.000000 pymenu_cli-1.0.2/pymenu_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 moraneus   (501) staff       (20)        1 2024-05-17 19:24:38.000000 pymenu_cli-1.0.2/pymenu_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 moraneus   (501) staff       (20)       52 2024-05-17 19:24:38.000000 pymenu_cli-1.0.2/pymenu_cli.egg-info/entry_points.txt
+-rw-r--r--   0 moraneus   (501) staff       (20)       11 2024-05-17 19:24:38.000000 pymenu_cli-1.0.2/pymenu_cli.egg-info/top_level.txt
+-rw-r--r--   0 moraneus   (501) staff       (20)       38 2024-05-17 19:24:38.306091 pymenu_cli-1.0.2/setup.cfg
+-rw-r--r--   0 moraneus   (501) staff       (20)      654 2024-05-17 19:24:29.000000 pymenu_cli-1.0.2/setup.py
```

### Comparing `pymenu_cli-1.0.1/PKG-INFO` & `pymenu_cli-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: pymenu-cli
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python library for creating interactive CLI menus
+Home-page: https://github.com/your-username/your-repository
 Author: Moraneus
 Author-email: moraneus@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # pymenu-cli
```

### Comparing `pymenu_cli-1.0.1/README.md` & `pymenu_cli-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pymenu_cli-1.0.1/pymenu_cli/menu.py` & `pymenu_cli-1.0.2/pymenu_cli/menu.py`

 * *Files identical despite different names*

### Comparing `pymenu_cli-1.0.1/pymenu_cli.egg-info/PKG-INFO` & `pymenu_cli-1.0.2/pymenu_cli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: pymenu-cli
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python library for creating interactive CLI menus
+Home-page: https://github.com/your-username/your-repository
 Author: Moraneus
 Author-email: moraneus@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # pymenu-cli
```

### Comparing `pymenu_cli-1.0.1/setup.py` & `pymenu_cli-1.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pymenu-cli',
-    version='1.0.1',
+    version='1.0.2',
     description='A Python library for creating interactive CLI menus',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Moraneus',
     author_email='moraneus@gmail.com',
+    url='https://github.com/your-username/your-repository',
     packages=find_packages(),
     install_requires=[],
     entry_points={
         'console_scripts': [
             'pymenu-cli = pymenu_cli.menu:main'
         ]
     },
```

