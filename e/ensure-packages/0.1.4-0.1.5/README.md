# Comparing `tmp/ensure_packages-0.1.4.tar.gz` & `tmp/ensure_packages-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensure_packages-0.1.4.tar", last modified: Thu May 16 05:19:24 2024, max compression
+gzip compressed data, was "ensure_packages-0.1.5.tar", last modified: Fri May 17 09:04:01 2024, max compression
```

## Comparing `ensure_packages-0.1.4.tar` & `ensure_packages-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 05:19:24.540071 ensure_packages-0.1.4/
--rw-rw-rw-   0        0        0      578 2024-05-16 05:19:24.223247 ensure_packages-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      126 2024-05-15 07:47:47.000000 ensure_packages-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 05:19:24.169836 ensure_packages-0.1.4/ensure_packages/
--rw-rw-rw-   0        0        0       38 2024-05-16 05:16:32.000000 ensure_packages-0.1.4/ensure_packages/__init__.py
--rw-rw-rw-   0        0        0     1196 2024-05-16 05:04:42.000000 ensure_packages-0.1.4/ensure_packages/ensure_package.py
-drwxrwxrwx   0        0        0        0 2024-05-16 05:19:24.223247 ensure_packages-0.1.4/ensure_packages.egg-info/
--rw-rw-rw-   0        0        0      578 2024-05-16 05:19:23.000000 ensure_packages-0.1.4/ensure_packages.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-05-16 05:19:23.000000 ensure_packages-0.1.4/ensure_packages.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 05:19:23.000000 ensure_packages-0.1.4/ensure_packages.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-16 05:19:23.000000 ensure_packages-0.1.4/ensure_packages.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 05:19:24.540071 ensure_packages-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      722 2024-05-16 05:17:25.000000 ensure_packages-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:04:01.623434 ensure_packages-0.1.5/
+-rw-rw-rw-   0        0        0      578 2024-05-17 09:04:01.615446 ensure_packages-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      126 2024-05-15 07:47:47.000000 ensure_packages-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 09:04:01.511425 ensure_packages-0.1.5/ensure_packages/
+-rw-rw-rw-   0        0        0       37 2024-05-17 09:03:04.000000 ensure_packages-0.1.5/ensure_packages/__init__.py
+-rw-rw-rw-   0        0        0     1196 2024-05-16 05:04:42.000000 ensure_packages-0.1.5/ensure_packages/ensure_package.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:04:01.607435 ensure_packages-0.1.5/ensure_packages.egg-info/
+-rw-rw-rw-   0        0        0      578 2024-05-17 09:03:58.000000 ensure_packages-0.1.5/ensure_packages.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-17 09:03:59.000000 ensure_packages-0.1.5/ensure_packages.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 09:03:58.000000 ensure_packages-0.1.5/ensure_packages.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-17 09:03:58.000000 ensure_packages-0.1.5/ensure_packages.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 09:04:01.623434 ensure_packages-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      722 2024-05-17 09:02:43.000000 ensure_packages-0.1.5/setup.py
```

### Comparing `ensure_packages-0.1.4/PKG-INFO` & `ensure_packages-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensure_packages
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package to ensure other packages are installed its created by vinoth cse-B. a laternate for using pip
 Author: vinothjs
 Author-email: jeyashreenarayan@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `ensure_packages-0.1.4/ensure_packages/ensure_package.py` & `ensure_packages-0.1.5/ensure_packages/ensure_package.py`

 * *Files identical despite different names*

### Comparing `ensure_packages-0.1.4/ensure_packages.egg-info/PKG-INFO` & `ensure_packages-0.1.5/ensure_packages.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensure-packages
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package to ensure other packages are installed its created by vinoth cse-B. a laternate for using pip
 Author: vinothjs
 Author-email: jeyashreenarayan@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `ensure_packages-0.1.4/setup.py` & `ensure_packages-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="ensure_packages", 
-    version="0.1.4",
+    version="0.1.5",
     author="vinothjs",
     author_email="jeyashreenarayan@gmail.com",
     description="A package to ensure other packages are installed its created by vinoth cse-B. a laternate for using pip",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
```

