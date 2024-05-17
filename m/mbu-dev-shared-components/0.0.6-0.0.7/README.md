# Comparing `tmp/mbu_dev_shared_components-0.0.6.tar.gz` & `tmp/mbu_dev_shared_components-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbu_dev_shared_components-0.0.6.tar", last modified: Fri May 17 13:59:13 2024, max compression
+gzip compressed data, was "mbu_dev_shared_components-0.0.7.tar", last modified: Fri May 17 14:33:13 2024, max compression
```

## Comparing `mbu_dev_shared_components-0.0.6.tar` & `mbu_dev_shared_components-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 13:59:13.184469 mbu_dev_shared_components-0.0.6/
--rw-rw-rw-   0        0        0     3238 2024-05-16 14:14:30.000000 mbu_dev_shared_components-0.0.6/.gitignore
--rw-rw-rw-   0        0        0     1085 2024-05-16 14:14:30.000000 mbu_dev_shared_components-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      989 2024-05-17 13:59:13.178759 mbu_dev_shared_components-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      498 2024-05-16 15:19:15.000000 mbu_dev_shared_components-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 13:59:13.026980 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components/
-drwxrwxrwx   0        0        0        0 2024-05-17 13:59:13.119929 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components/office365/
--rw-rw-rw-   0        0        0        0 2024-05-16 14:20:13.000000 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components/office365/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:59:13.155273 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components/office365/excel/
--rw-rw-rw-   0        0        0        0 2024-05-16 20:18:44.000000 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components/office365/excel/__init__.py
--rw-rw-rw-   0        0        0     7181 2024-05-17 13:55:50.000000 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components/office365/excel/excel_reader.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:59:13.172933 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components/office365/sharepoint_api/
--rw-rw-rw-   0        0        0        0 2024-05-16 14:20:46.000000 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components/office365/sharepoint_api/__init__.py
--rw-rw-rw-   0        0        0     8970 2024-05-16 15:09:46.000000 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components/office365/sharepoint_api/files.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:59:13.172933 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components/os2forms_api/
--rw-rw-rw-   0        0        0        0 2024-05-16 15:12:48.000000 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components/os2forms_api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:59:13.178759 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components.egg-info/
--rw-rw-rw-   0        0        0      989 2024-05-17 13:59:12.000000 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      621 2024-05-17 13:59:13.000000 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 13:59:12.000000 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-05-17 13:59:12.000000 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-17 13:59:12.000000 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      593 2024-05-17 13:58:21.000000 mbu_dev_shared_components-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-17 13:59:13.187067 mbu_dev_shared_components-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 14:33:13.838200 mbu_dev_shared_components-0.0.7/
+-rw-rw-rw-   0        0        0     3238 2024-05-16 14:14:30.000000 mbu_dev_shared_components-0.0.7/.gitignore
+-rw-rw-rw-   0        0        0     1085 2024-05-16 14:14:30.000000 mbu_dev_shared_components-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      989 2024-05-17 14:33:13.836437 mbu_dev_shared_components-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      498 2024-05-16 15:19:15.000000 mbu_dev_shared_components-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 14:33:13.653942 mbu_dev_shared_components-0.0.7/mbu_dev_shared_components/
+drwxrwxrwx   0        0        0        0 2024-05-17 14:33:13.733667 mbu_dev_shared_components-0.0.7/mbu_dev_shared_components/office365/
+-rw-rw-rw-   0        0        0        0 2024-05-16 14:20:13.000000 mbu_dev_shared_components-0.0.7/mbu_dev_shared_components/office365/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 14:33:13.782520 mbu_dev_shared_components-0.0.7/mbu_dev_shared_components/office365/excel/
+-rw-rw-rw-   0        0        0        0 2024-05-16 20:18:44.000000 mbu_dev_shared_components-0.0.7/mbu_dev_shared_components/office365/excel/__init__.py
+-rw-rw-rw-   0        0        0     7181 2024-05-17 13:55:50.000000 mbu_dev_shared_components-0.0.7/mbu_dev_shared_components/office365/excel/excel_reader.py
+drwxrwxrwx   0        0        0        0 2024-05-17 14:33:13.818815 mbu_dev_shared_components-0.0.7/mbu_dev_shared_components/office365/sharepoint_api/
+-rw-rw-rw-   0        0        0        0 2024-05-16 14:20:46.000000 mbu_dev_shared_components-0.0.7/mbu_dev_shared_components/office365/sharepoint_api/__init__.py
+-rw-rw-rw-   0        0        0     8970 2024-05-16 15:09:46.000000 mbu_dev_shared_components-0.0.7/mbu_dev_shared_components/office365/sharepoint_api/files.py
+drwxrwxrwx   0        0        0        0 2024-05-17 14:33:13.818815 mbu_dev_shared_components-0.0.7/mbu_dev_shared_components/os2forms_api/
+-rw-rw-rw-   0        0        0        0 2024-05-16 15:12:48.000000 mbu_dev_shared_components-0.0.7/mbu_dev_shared_components/os2forms_api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 14:33:13.830808 mbu_dev_shared_components-0.0.7/mbu_dev_shared_components/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-17 14:24:58.000000 mbu_dev_shared_components-0.0.7/mbu_dev_shared_components/utils/__init__.py
+-rw-rw-rw-   0        0        0     1976 2024-05-17 14:30:40.000000 mbu_dev_shared_components-0.0.7/mbu_dev_shared_components/utils/json.py
+drwxrwxrwx   0        0        0        0 2024-05-17 14:33:13.832295 mbu_dev_shared_components-0.0.7/mbu_dev_shared_components.egg-info/
+-rw-rw-rw-   0        0        0      989 2024-05-17 14:33:13.000000 mbu_dev_shared_components-0.0.7/mbu_dev_shared_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2024-05-17 14:33:13.000000 mbu_dev_shared_components-0.0.7/mbu_dev_shared_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 14:33:13.000000 mbu_dev_shared_components-0.0.7/mbu_dev_shared_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-17 14:33:13.000000 mbu_dev_shared_components-0.0.7/mbu_dev_shared_components.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-17 14:33:13.000000 mbu_dev_shared_components-0.0.7/mbu_dev_shared_components.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      593 2024-05-17 14:32:17.000000 mbu_dev_shared_components-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 14:33:13.840776 mbu_dev_shared_components-0.0.7/setup.cfg
```

### Comparing `mbu_dev_shared_components-0.0.6/.gitignore` & `mbu_dev_shared_components-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `mbu_dev_shared_components-0.0.6/LICENSE` & `mbu_dev_shared_components-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mbu_dev_shared_components-0.0.6/PKG-INFO` & `mbu_dev_shared_components-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbu_dev_shared_components
-Version: 0.0.6
+Version: 0.0.7
 Summary: Shared components to use in RPA projects
 Author-email: MBU <rpa@mbu.aarhus.dk>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `mbu_dev_shared_components-0.0.6/mbu_dev_shared_components/office365/excel/excel_reader.py` & `mbu_dev_shared_components-0.0.7/mbu_dev_shared_components/office365/excel/excel_reader.py`

 * *Files identical despite different names*

### Comparing `mbu_dev_shared_components-0.0.6/mbu_dev_shared_components/office365/sharepoint_api/files.py` & `mbu_dev_shared_components-0.0.7/mbu_dev_shared_components/office365/sharepoint_api/files.py`

 * *Files identical despite different names*

### Comparing `mbu_dev_shared_components-0.0.6/mbu_dev_shared_components.egg-info/PKG-INFO` & `mbu_dev_shared_components-0.0.7/mbu_dev_shared_components.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbu_dev_shared_components
-Version: 0.0.6
+Version: 0.0.7
 Summary: Shared components to use in RPA projects
 Author-email: MBU <rpa@mbu.aarhus.dk>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `mbu_dev_shared_components-0.0.6/mbu_dev_shared_components.egg-info/SOURCES.txt` & `mbu_dev_shared_components-0.0.7/mbu_dev_shared_components.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -8,8 +8,10 @@
 mbu_dev_shared_components.egg-info/requires.txt
 mbu_dev_shared_components.egg-info/top_level.txt
 mbu_dev_shared_components/office365/__init__.py
 mbu_dev_shared_components/office365/excel/__init__.py
 mbu_dev_shared_components/office365/excel/excel_reader.py
 mbu_dev_shared_components/office365/sharepoint_api/__init__.py
 mbu_dev_shared_components/office365/sharepoint_api/files.py
-mbu_dev_shared_components/os2forms_api/__init__.py
+mbu_dev_shared_components/os2forms_api/__init__.py
+mbu_dev_shared_components/utils/__init__.py
+mbu_dev_shared_components/utils/json.py
```

### Comparing `mbu_dev_shared_components-0.0.6/pyproject.toml` & `mbu_dev_shared_components-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mbu_dev_shared_components"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="MBU", email="rpa@mbu.aarhus.dk" },
 ]
 description = "Shared components to use in RPA projects"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

