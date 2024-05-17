# Comparing `tmp/way3-0.0.24.tar.gz` & `tmp/way3-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "way3-0.0.24.tar", last modified: Thu May 16 17:34:46 2024, max compression
+gzip compressed data, was "way3-0.0.25.tar", last modified: Fri May 17 18:52:41 2024, max compression
```

## Comparing `way3-0.0.24.tar` & `way3-0.0.25.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:34:46.816334 way3-0.0.24/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-16 17:34:43.000000 way3-0.0.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-16 17:34:46.816334 way3-0.0.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-16 17:34:43.000000 way3-0.0.24/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 17:34:46.816334 way3-0.0.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-16 17:34:43.000000 way3-0.0.24/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:34:46.816334 way3-0.0.24/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:34:43.000000 way3-0.0.24/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-16 17:34:43.000000 way3-0.0.24/tests/test_file_find.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-16 17:34:43.000000 way3-0.0.24/tests/test_file_op.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:34:46.816334 way3-0.0.24/way3/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-16 17:34:43.000000 way3-0.0.24/way3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:34:46.816334 way3-0.0.24/way3/file_find/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:34:43.000000 way3-0.0.24/way3/file_find/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-16 17:34:43.000000 way3-0.0.24/way3/file_find/current_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-16 17:34:43.000000 way3-0.0.24/way3/file_find/traverse_files_from_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:34:46.816334 way3-0.0.24/way3/file_op/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:34:43.000000 way3-0.0.24/way3/file_op/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-16 17:34:43.000000 way3-0.0.24/way3/file_op/create_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:34:46.816334 way3-0.0.24/way3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-16 17:34:46.000000 way3-0.0.24/way3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-16 17:34:46.000000 way3-0.0.24/way3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 17:34:46.000000 way3-0.0.24/way3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 17:34:46.000000 way3-0.0.24/way3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:52:41.829053 way3-0.0.25/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-17 18:52:37.000000 way3-0.0.25/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-17 18:52:41.829053 way3-0.0.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-17 18:52:37.000000 way3-0.0.25/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 18:52:41.829053 way3-0.0.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-17 18:52:37.000000 way3-0.0.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:52:41.829053 way3-0.0.25/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 18:52:37.000000 way3-0.0.25/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-17 18:52:37.000000 way3-0.0.25/tests/test_file_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-17 18:52:37.000000 way3-0.0.25/tests/test_file_op.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:52:41.829053 way3-0.0.25/way3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-17 18:52:37.000000 way3-0.0.25/way3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:52:41.829053 way3-0.0.25/way3/file_find/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 18:52:37.000000 way3-0.0.25/way3/file_find/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-17 18:52:37.000000 way3-0.0.25/way3/file_find/current_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-17 18:52:37.000000 way3-0.0.25/way3/file_find/traverse_files_from_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:52:41.829053 way3-0.0.25/way3/file_op/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 18:52:37.000000 way3-0.0.25/way3/file_op/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-17 18:52:37.000000 way3-0.0.25/way3/file_op/create_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:52:41.829053 way3-0.0.25/way3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-17 18:52:41.000000 way3-0.0.25/way3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-17 18:52:41.000000 way3-0.0.25/way3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 18:52:41.000000 way3-0.0.25/way3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 18:52:41.000000 way3-0.0.25/way3.egg-info/top_level.txt
```

### Comparing `way3-0.0.24/LICENSE` & `way3-0.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `way3-0.0.24/PKG-INFO` & `way3-0.0.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: way3
-Version: 0.0.24
+Version: 0.0.25
 Summary: Simplified file path management for Python developers
 Home-page: https://github.com/aboutmydreams/way3
 Author: aboutmydreams
 Author-email: aboutmydreams@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `way3-0.0.24/README.md` & `way3-0.0.25/README.md`

 * *Files identical despite different names*

### Comparing `way3-0.0.24/setup.py` & `way3-0.0.25/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="way3",
-    version="0.0.24",
+    version="0.0.25",
     author="aboutmydreams",
     author_email="aboutmydreams@163.com",
     description="Simplified file path management for Python developers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aboutmydreams/way3",
     packages=setuptools.find_packages(),
```

### Comparing `way3-0.0.24/tests/test_file_op.py` & `way3-0.0.25/tests/test_file_op.py`

 * *Files identical despite different names*

### Comparing `way3-0.0.24/way3/__init__.py` & `way3-0.0.25/way3/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,7 +9,16 @@
 # File Find
 from .file_find.current_dir import get_current_dir as get_current_dir  # noqa: E402
 from .file_find.traverse_files_from_folder import parse_gitignore as parse_gitignore  # noqa: E402
 from .file_find.traverse_files_from_folder import is_gitignored as is_gitignored  # noqa: E402
 from .file_find.traverse_files_from_folder import (  # noqa: E402
     get_files_in_directory as get_files_in_directory,
 )
+from .file_find.traverse_files_from_folder import (  # noqa: E402
+    get_directory_structure as get_directory_structure,
+)
+from .file_find.traverse_files_from_folder import (  # noqa: E402
+    get_directory_folder_list as get_directory_folder_list,
+)
+from .file_find.traverse_files_from_folder import (  # noqa: E402
+    get_directory_file_list as get_directory_file_list,
+)
```

### Comparing `way3-0.0.24/way3/file_op/create_file.py` & `way3-0.0.25/way3/file_op/create_file.py`

 * *Files identical despite different names*

### Comparing `way3-0.0.24/way3.egg-info/PKG-INFO` & `way3-0.0.25/way3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: way3
-Version: 0.0.24
+Version: 0.0.25
 Summary: Simplified file path management for Python developers
 Home-page: https://github.com/aboutmydreams/way3
 Author: aboutmydreams
 Author-email: aboutmydreams@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

