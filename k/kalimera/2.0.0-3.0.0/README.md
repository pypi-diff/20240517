# Comparing `tmp/kalimera-2.0.0.tar.gz` & `tmp/kalimera-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalimera-2.0.0.tar", last modified: Fri May 17 12:11:54 2024, max compression
+gzip compressed data, was "kalimera-3.0.0.tar", last modified: Fri May 17 12:31:22 2024, max compression
```

## Comparing `kalimera-2.0.0.tar` & `kalimera-3.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-17 12:11:54.298626 kalimera-2.0.0/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2024-05-17 09:59:28.000000 kalimera-2.0.0/LICENSE
--rw-r--r--   0 chris     (1000) chris     (1000)      873 2024-05-17 12:11:54.294625 kalimera-2.0.0/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      313 2024-05-17 11:37:42.000000 kalimera-2.0.0/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-17 12:11:54.294625 kalimera-2.0.0/kalimera.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)      873 2024-05-17 12:11:54.000000 kalimera-2.0.0/kalimera.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      192 2024-05-17 12:11:54.000000 kalimera-2.0.0/kalimera.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2024-05-17 12:11:54.000000 kalimera-2.0.0/kalimera.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        8 2024-05-17 12:11:54.000000 kalimera-2.0.0/kalimera.egg-info/top_level.txt
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-17 12:11:54.294625 kalimera-2.0.0/libname/
--rw-rw-r--   0 chris     (1000) chris     (1000)       37 2024-05-17 09:59:10.000000 kalimera-2.0.0/libname/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)       65 2024-05-17 09:58:09.000000 kalimera-2.0.0/libname/source.py
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2024-05-17 12:11:54.298626 kalimera-2.0.0/setup.cfg
--rw-rw-r--   0 chris     (1000) chris     (1000)     1018 2024-05-17 12:10:46.000000 kalimera-2.0.0/setup.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-17 12:31:22.239894 kalimera-3.0.0/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2024-05-17 09:59:28.000000 kalimera-3.0.0/LICENSE
+-rw-r--r--   0 chris     (1000) chris     (1000)      873 2024-05-17 12:31:22.239894 kalimera-3.0.0/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      313 2024-05-17 11:37:42.000000 kalimera-3.0.0/README.md
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-17 12:31:22.235893 kalimera-3.0.0/kalimera/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2024-05-17 12:29:32.000000 kalimera-3.0.0/kalimera/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)       69 2024-05-17 12:31:07.000000 kalimera-3.0.0/kalimera/source.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-17 12:31:22.239894 kalimera-3.0.0/kalimera.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)      873 2024-05-17 12:31:22.000000 kalimera-3.0.0/kalimera.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      194 2024-05-17 12:31:22.000000 kalimera-3.0.0/kalimera.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2024-05-17 12:31:22.000000 kalimera-3.0.0/kalimera.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        9 2024-05-17 12:31:22.000000 kalimera-3.0.0/kalimera.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2024-05-17 12:31:22.239894 kalimera-3.0.0/setup.cfg
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1015 2024-05-17 12:31:12.000000 kalimera-3.0.0/setup.py
```

### Comparing `kalimera-2.0.0/LICENSE` & `kalimera-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kalimera-2.0.0/PKG-INFO` & `kalimera-3.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalimera
-Version: 2.0.0
+Version: 3.0.0
 Summary: Hello world
 Author: Chris (Christoforos Eseroglou)
 Author-email: chriseseroglou@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `kalimera-2.0.0/kalimera.egg-info/PKG-INFO` & `kalimera-3.0.0/kalimera.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalimera
-Version: 2.0.0
+Version: 3.0.0
 Summary: Hello world
 Author: Chris (Christoforos Eseroglou)
 Author-email: chriseseroglou@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `kalimera-2.0.0/setup.py` & `kalimera-3.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Read the long description from README.md
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = fh.read()
 
-VERSION = '2.0.0'
+VERSION = '3.0.0'
 DESCRIPTION = 'Hello world'
 
 # Setting up
 setup(
     name="kalimera",
     version=VERSION,
     author="Chris (Christoforos Eseroglou)",
     author_email="chriseseroglou@gmail.com",
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
-    packages=find_packages(),
+    packages=['kalimera'],
     install_requires=[],
     keywords=['python'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         'License :: OSI Approved :: MIT License',
```

