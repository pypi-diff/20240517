# Comparing `tmp/json24-0.0.1.tar.gz` & `tmp/json24-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "json24-0.1.0.tar", last modified: Thu May 16 22:25:21 2024, max compression
```

## Comparing `json24-0.0.1.tar` & `json24-0.1.0.tar`

### file list

```diff
@@ -1,28 +1,16 @@
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 json24-0.0.1/setup.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 json24-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 json24-0.0.1/.idea/.gitignore
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 json24-0.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 json24-0.0.1/.idea/modules.xml
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 json24-0.0.1/.idea/pjson24.iml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 json24-0.0.1/.idea/vcs.xml
--rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 json24-0.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 json24-0.0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 json24-0.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 json24-0.0.1/build/lib/json24/__init__.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 json24-0.0.1/build/lib/json24/parser.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 json24-0.0.1/example_package_yeargun.egg-info/PKG-INFO
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 json24-0.0.1/example_package_yeargun.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 json24-0.0.1/example_package_yeargun.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 json24-0.0.1/example_package_yeargun.egg-info/top_level.txt
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 json24-0.0.1/json24/__init__.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 json24-0.0.1/json24/parser.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 json24-0.0.1/json24.egg-info/PKG-INFO
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 json24-0.0.1/json24.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 json24-0.0.1/json24.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 json24-0.0.1/json24.egg-info/top_level.txt
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 json24-0.0.1/tests/test_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 json24-0.0.1/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 json24-0.0.1/LICENSE
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 json24-0.0.1/README.md
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 json24-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 json24-0.0.1/PKG-INFO
+drwxr-xr-x   0 yeargun    (501) staff       (20)        0 2024-05-16 22:25:21.576598 json24-0.1.0/
+-rw-r--r--   0 yeargun    (501) staff       (20)      412 2024-05-16 22:25:21.576031 json24-0.1.0/PKG-INFO
+-rw-r--r--   0 yeargun    (501) staff       (20)      139 2024-05-16 22:24:28.000000 json24-0.1.0/README.md
+drwxr-xr-x   0 yeargun    (501) staff       (20)        0 2024-05-16 22:25:21.573566 json24-0.1.0/json24/
+-rw-r--r--   0 yeargun    (501) staff       (20)      197 2024-05-16 22:23:36.000000 json24-0.1.0/json24/__init__.py
+-rw-r--r--   0 yeargun    (501) staff       (20)     1704 2024-05-16 22:23:28.000000 json24-0.1.0/json24/parser.py
+drwxr-xr-x   0 yeargun    (501) staff       (20)        0 2024-05-16 22:25:21.574765 json24-0.1.0/json24.egg-info/
+-rw-r--r--   0 yeargun    (501) staff       (20)      412 2024-05-16 22:25:21.000000 json24-0.1.0/json24.egg-info/PKG-INFO
+-rw-r--r--   0 yeargun    (501) staff       (20)      210 2024-05-16 22:25:21.000000 json24-0.1.0/json24.egg-info/SOURCES.txt
+-rw-r--r--   0 yeargun    (501) staff       (20)        1 2024-05-16 22:25:21.000000 json24-0.1.0/json24.egg-info/dependency_links.txt
+-rw-r--r--   0 yeargun    (501) staff       (20)        7 2024-05-16 22:25:21.000000 json24-0.1.0/json24.egg-info/top_level.txt
+-rw-r--r--   0 yeargun    (501) staff       (20)       91 2024-05-16 22:25:01.000000 json24-0.1.0/pyproject.toml
+-rw-r--r--   0 yeargun    (501) staff       (20)       38 2024-05-16 22:25:21.576656 json24-0.1.0/setup.cfg
+-rw-r--r--   0 yeargun    (501) staff       (20)      561 2024-05-16 22:24:00.000000 json24-0.1.0/setup.py
+drwxr-xr-x   0 yeargun    (501) staff       (20)        0 2024-05-16 22:25:21.575312 json24-0.1.0/tests/
+-rw-r--r--   0 yeargun    (501) staff       (20)      936 2024-05-16 22:23:47.000000 json24-0.1.0/tests/test_parser.py
```

### Comparing `json24-0.0.1/setup.py` & `json24-0.1.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='json24',
-    version='0.0.1',
+    version='0.1.0',
     packages=find_packages(),
     install_requires=[],
     description='A library to parse partial JSON strings with optional logging for faulty JSON.',
-    author='Ali Argun Sayilgan',
-    author_email='yeargun@stuf24.com',
-    url='https://github.com/yeargun/json24-python',
+    author='Your Name',
+    author_email='your.email@example.com',
+    url='https://github.com/yourusername/json24',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
 )
```

### Comparing `json24-0.0.1/build/lib/json24/parser.py` & `json24-0.1.0/json24/parser.py`

 * *Files identical despite different names*

### Comparing `json24-0.0.1/tests/test_parser.py` & `json24-0.1.0/tests/test_parser.py`

 * *Files identical despite different names*

