# Comparing `tmp/mbu_dev_shared_components-0.0.2.tar.gz` & `tmp/mbu_dev_shared_components-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbu_dev_shared_components-0.0.2.tar", last modified: Thu May 16 19:19:47 2024, max compression
+gzip compressed data, was "mbu_dev_shared_components-0.0.5.tar", last modified: Thu May 16 21:04:04 2024, max compression
```

## Comparing `mbu_dev_shared_components-0.0.2.tar` & `mbu_dev_shared_components-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 19:19:47.296642 mbu_dev_shared_components-0.0.2/
--rw-rw-rw-   0        0        0     1085 2024-05-16 14:14:30.000000 mbu_dev_shared_components-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      957 2024-05-16 19:19:47.291942 mbu_dev_shared_components-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      498 2024-05-16 15:19:15.000000 mbu_dev_shared_components-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 19:19:47.240482 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components/
-drwxrwxrwx   0        0        0        0 2024-05-16 19:19:47.275358 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components/office365/
--rw-rw-rw-   0        0        0        0 2024-05-16 14:20:13.000000 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components/office365/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 19:19:47.278444 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components/office365/sharepoint_api/
--rw-rw-rw-   0        0        0        0 2024-05-16 14:20:46.000000 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components/office365/sharepoint_api/__init__.py
--rw-rw-rw-   0        0        0     8970 2024-05-16 15:09:46.000000 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components/office365/sharepoint_api/files.py
-drwxrwxrwx   0        0        0        0 2024-05-16 19:19:47.280591 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components/os2forms_api/
--rw-rw-rw-   0        0        0        0 2024-05-16 15:12:48.000000 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components/os2forms_api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 19:19:47.290229 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components.egg-info/
--rw-rw-rw-   0        0        0      957 2024-05-16 19:19:47.000000 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      498 2024-05-16 19:19:47.000000 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 19:19:47.000000 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-05-16 19:19:47.000000 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-16 19:19:47.000000 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      549 2024-05-16 19:18:30.000000 mbu_dev_shared_components-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 19:19:47.297143 mbu_dev_shared_components-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-16 21:04:04.012176 mbu_dev_shared_components-0.0.5/
+-rw-rw-rw-   0        0        0     3238 2024-05-16 14:14:30.000000 mbu_dev_shared_components-0.0.5/.gitignore
+-rw-rw-rw-   0        0        0     1085 2024-05-16 14:14:30.000000 mbu_dev_shared_components-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      989 2024-05-16 21:04:04.002896 mbu_dev_shared_components-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      498 2024-05-16 15:19:15.000000 mbu_dev_shared_components-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 21:04:03.935017 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components/
+drwxrwxrwx   0        0        0        0 2024-05-16 21:04:03.984007 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components/office365/
+-rw-rw-rw-   0        0        0        0 2024-05-16 14:20:13.000000 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components/office365/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 21:04:03.991929 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components/office365/excel/
+-rw-rw-rw-   0        0        0        0 2024-05-16 20:18:44.000000 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components/office365/excel/__init__.py
+-rw-rw-rw-   0        0        0     7176 2024-05-16 20:22:16.000000 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components/office365/excel/excel_reader.py
+drwxrwxrwx   0        0        0        0 2024-05-16 21:04:03.995526 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components/office365/sharepoint_api/
+-rw-rw-rw-   0        0        0        0 2024-05-16 14:20:46.000000 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components/office365/sharepoint_api/__init__.py
+-rw-rw-rw-   0        0        0     8970 2024-05-16 15:09:46.000000 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components/office365/sharepoint_api/files.py
+drwxrwxrwx   0        0        0        0 2024-05-16 21:04:03.997913 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components/os2forms_api/
+-rw-rw-rw-   0        0        0        0 2024-05-16 15:12:48.000000 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components/os2forms_api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 21:04:04.000888 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components.egg-info/
+-rw-rw-rw-   0        0        0      989 2024-05-16 21:04:03.000000 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      621 2024-05-16 21:04:03.000000 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 21:04:03.000000 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-16 21:04:03.000000 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-16 21:04:03.000000 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      593 2024-05-16 21:03:28.000000 mbu_dev_shared_components-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 21:04:04.012679 mbu_dev_shared_components-0.0.5/setup.cfg
```

### Comparing `mbu_dev_shared_components-0.0.2/LICENSE` & `mbu_dev_shared_components-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mbu_dev_shared_components-0.0.2/PKG-INFO` & `mbu_dev_shared_components-0.0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: mbu_dev_shared_components
-Version: 0.0.2
+Version: 0.0.5
 Summary: Shared components to use in RPA projects
 Author-email: MBU <rpa@mbu.aarhus.dk>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Office365-REST-Python-Client>=2.5.9
+Requires-Dist: openpyxl>=3.1.2
 
 # mub-dev-shared-components
 
 ## Installation
 
 ```
 pip install mbu-dev-shared-components
```

### Comparing `mbu_dev_shared_components-0.0.2/mbu_dev_shared_components/office365/sharepoint_api/files.py` & `mbu_dev_shared_components-0.0.5/mbu_dev_shared_components/office365/sharepoint_api/files.py`

 * *Files identical despite different names*

### Comparing `mbu_dev_shared_components-0.0.2/mbu_dev_shared_components.egg-info/PKG-INFO` & `mbu_dev_shared_components-0.0.5/mbu_dev_shared_components.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: mbu_dev_shared_components
-Version: 0.0.2
+Version: 0.0.5
 Summary: Shared components to use in RPA projects
 Author-email: MBU <rpa@mbu.aarhus.dk>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Office365-REST-Python-Client>=2.5.9
+Requires-Dist: openpyxl>=3.1.2
 
 # mub-dev-shared-components
 
 ## Installation
 
 ```
 pip install mbu-dev-shared-components
```

### Comparing `mbu_dev_shared_components-0.0.2/pyproject.toml` & `mbu_dev_shared_components-0.0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [build-system]
-requires = ["setuptools>=65.0"]
+requires = ["setuptools>=65.0", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mbu_dev_shared_components"
-version = "0.0.2"
+version = "0.0.5"
 authors = [
   { name="MBU", email="rpa@mbu.aarhus.dk" },
 ]
 description = "Shared components to use in RPA projects"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: Microsoft :: Windows",
 ]
 dependencies = [
-  "Office365-REST-Python-Client >= 2.5.9"
-]
+  "Office365-REST-Python-Client >= 2.5.9",
+  "openpyxl >= 3.1.2"
+]
```

