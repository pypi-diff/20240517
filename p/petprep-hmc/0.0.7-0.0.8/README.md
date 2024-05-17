# Comparing `tmp/petprep_hmc-0.0.7.tar.gz` & `tmp/petprep_hmc-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petprep_hmc-0.0.7.tar", last modified: Fri Nov 10 12:23:12 2023, max compression
+gzip compressed data, was "petprep_hmc-0.0.8.tar", last modified: Fri May 17 20:22:46 2024, max compression
```

## Comparing `petprep_hmc-0.0.7.tar` & `petprep_hmc-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-11-10 12:23:12.649015 petprep_hmc-0.0.7/
--rw-r--r--   0 martinnorgaard   (501) staff       (20)    11357 2023-04-18 08:13:25.000000 petprep_hmc-0.0.7/LICENSE
--rw-r--r--   0 martinnorgaard   (501) staff       (20)     1486 2023-11-10 12:23:12.648723 petprep_hmc-0.0.7/PKG-INFO
--rw-r--r--   0 martinnorgaard   (501) staff       (20)     4576 2023-11-10 12:21:35.000000 petprep_hmc-0.0.7/README.md
-drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-11-10 12:23:12.646894 petprep_hmc-0.0.7/petprep_hmc/
--rw-r--r--   0 martinnorgaard   (501) staff       (20)        0 2023-04-18 08:17:50.000000 petprep_hmc-0.0.7/petprep_hmc/__init__.py
--rw-r--r--   0 martinnorgaard   (501) staff       (20)    16999 2023-11-08 13:33:55.000000 petprep_hmc-0.0.7/petprep_hmc/bids.py
--rw-r--r--   0 martinnorgaard   (501) staff       (20)     2126 2023-11-07 21:02:29.000000 petprep_hmc-0.0.7/petprep_hmc/utils.py
-drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-11-10 12:23:12.647931 petprep_hmc-0.0.7/petprep_hmc.egg-info/
--rw-r--r--   0 martinnorgaard   (501) staff       (20)     1486 2023-11-10 12:23:12.000000 petprep_hmc-0.0.7/petprep_hmc.egg-info/PKG-INFO
--rw-r--r--   0 martinnorgaard   (501) staff       (20)      283 2023-11-10 12:23:12.000000 petprep_hmc-0.0.7/petprep_hmc.egg-info/SOURCES.txt
--rw-r--r--   0 martinnorgaard   (501) staff       (20)        1 2023-11-10 12:23:12.000000 petprep_hmc-0.0.7/petprep_hmc.egg-info/dependency_links.txt
--rw-r--r--   0 martinnorgaard   (501) staff       (20)      422 2023-11-10 12:23:12.000000 petprep_hmc-0.0.7/petprep_hmc.egg-info/requires.txt
--rw-r--r--   0 martinnorgaard   (501) staff       (20)       12 2023-11-10 12:23:12.000000 petprep_hmc-0.0.7/petprep_hmc.egg-info/top_level.txt
--rw-r--r--   0 martinnorgaard   (501) staff       (20)       38 2023-11-10 12:23:12.649075 petprep_hmc-0.0.7/setup.cfg
--rw-r--r--   0 martinnorgaard   (501) staff       (20)     1584 2023-11-10 09:43:07.000000 petprep_hmc-0.0.7/setup.py
-drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-11-10 12:23:12.648065 petprep_hmc-0.0.7/tests/
--rw-r--r--   0 martinnorgaard   (501) staff       (20)      510 2023-05-03 19:40:26.000000 petprep_hmc-0.0.7/tests/test_cli.py
+drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2024-05-17 20:22:46.370092 petprep_hmc-0.0.8/
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)    11357 2023-04-18 08:13:25.000000 petprep_hmc-0.0.8/LICENSE
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)     1486 2024-05-17 20:22:46.369787 petprep_hmc-0.0.8/PKG-INFO
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)     4576 2023-11-10 13:49:52.000000 petprep_hmc-0.0.8/README.md
+drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2024-05-17 20:22:46.367447 petprep_hmc-0.0.8/petprep_hmc/
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)        0 2023-04-18 08:17:50.000000 petprep_hmc-0.0.8/petprep_hmc/__init__.py
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)    16999 2023-11-08 13:33:55.000000 petprep_hmc-0.0.8/petprep_hmc/bids.py
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)     2126 2023-11-07 21:02:29.000000 petprep_hmc-0.0.8/petprep_hmc/utils.py
+drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2024-05-17 20:22:46.369272 petprep_hmc-0.0.8/petprep_hmc.egg-info/
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)     1486 2024-05-17 20:22:46.000000 petprep_hmc-0.0.8/petprep_hmc.egg-info/PKG-INFO
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)      283 2024-05-17 20:22:46.000000 petprep_hmc-0.0.8/petprep_hmc.egg-info/SOURCES.txt
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)        1 2024-05-17 20:22:46.000000 petprep_hmc-0.0.8/petprep_hmc.egg-info/dependency_links.txt
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)      422 2024-05-17 20:22:46.000000 petprep_hmc-0.0.8/petprep_hmc.egg-info/requires.txt
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)       12 2024-05-17 20:22:46.000000 petprep_hmc-0.0.8/petprep_hmc.egg-info/top_level.txt
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)       38 2024-05-17 20:22:46.370157 petprep_hmc-0.0.8/setup.cfg
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)     1584 2024-05-17 20:22:22.000000 petprep_hmc-0.0.8/setup.py
+drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2024-05-17 20:22:46.368612 petprep_hmc-0.0.8/tests/
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)      510 2023-05-03 19:40:26.000000 petprep_hmc-0.0.8/tests/test_cli.py
```

### Comparing `petprep_hmc-0.0.7/LICENSE` & `petprep_hmc-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `petprep_hmc-0.0.7/PKG-INFO` & `petprep_hmc-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petprep_hmc
-Version: 0.0.7
+Version: 0.0.8
 Summary: PETPrep Head Motion Correction Workflow
 Home-page: https://github.com/mnoergaard/petprep_hmc
 Author: Martin Norgaard
 Author-email: martin.noergaard@di.ku.dk
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `petprep_hmc-0.0.7/README.md` & `petprep_hmc-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `petprep_hmc-0.0.7/petprep_hmc/bids.py` & `petprep_hmc-0.0.8/petprep_hmc/bids.py`

 * *Files identical despite different names*

### Comparing `petprep_hmc-0.0.7/petprep_hmc/utils.py` & `petprep_hmc-0.0.8/petprep_hmc/utils.py`

 * *Files identical despite different names*

### Comparing `petprep_hmc-0.0.7/petprep_hmc.egg-info/PKG-INFO` & `petprep_hmc-0.0.8/petprep_hmc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: petprep-hmc
-Version: 0.0.7
+Name: petprep_hmc
+Version: 0.0.8
 Summary: PETPrep Head Motion Correction Workflow
 Home-page: https://github.com/mnoergaard/petprep_hmc
 Author: Martin Norgaard
 Author-email: martin.noergaard@di.ku.dk
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `petprep_hmc-0.0.7/setup.py` & `petprep_hmc-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="petprep_hmc",
-    version="0.0.7",
+    version="0.0.8",
     description='PETPrep Head Motion Correction Workflow',
     author='Martin Norgaard',
     author_email='martin.noergaard@di.ku.dk',
     url='https://github.com/mnoergaard/petprep_hmc',
     packages=find_packages(),
     install_requires=[
         "click==8.1.3",
```

