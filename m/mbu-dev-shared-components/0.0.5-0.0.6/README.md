# Comparing `tmp/mbu_dev_shared_components-0.0.5.tar.gz` & `tmp/mbu_dev_shared_components-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbu_dev_shared_components-0.0.5.tar", last modified: Thu May 16 21:04:04 2024, max compression
+gzip compressed data, was "mbu_dev_shared_components-0.0.6.tar", last modified: Fri May 17 13:59:13 2024, max compression
```

## Comparing `mbu_dev_shared_components-0.0.5.tar` & `mbu_dev_shared_components-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 21:04:04.012176 mbu_dev_shared_components-0.0.5/
--rw-rw-rw-   0        0        0     3238 2024-05-16 14:14:30.000000 mbu_dev_shared_components-0.0.5/.gitignore
--rw-rw-rw-   0        0        0     1085 2024-05-16 14:14:30.000000 mbu_dev_shared_components-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      989 2024-05-16 21:04:04.002896 mbu_dev_shared_components-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      498 2024-05-16 15:19:15.000000 mbu_dev_shared_components-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 21:04:03.935017 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components/
-drwxrwxrwx   0        0        0        0 2024-05-16 21:04:03.984007 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components/office365/
--rw-rw-rw-   0        0        0        0 2024-05-16 14:20:13.000000 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components/office365/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 21:04:03.991929 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components/office365/excel/
--rw-rw-rw-   0        0        0        0 2024-05-16 20:18:44.000000 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components/office365/excel/__init__.py
--rw-rw-rw-   0        0        0     7176 2024-05-16 20:22:16.000000 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components/office365/excel/excel_reader.py
-drwxrwxrwx   0        0        0        0 2024-05-16 21:04:03.995526 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components/office365/sharepoint_api/
--rw-rw-rw-   0        0        0        0 2024-05-16 14:20:46.000000 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components/office365/sharepoint_api/__init__.py
--rw-rw-rw-   0        0        0     8970 2024-05-16 15:09:46.000000 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components/office365/sharepoint_api/files.py
-drwxrwxrwx   0        0        0        0 2024-05-16 21:04:03.997913 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components/os2forms_api/
--rw-rw-rw-   0        0        0        0 2024-05-16 15:12:48.000000 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components/os2forms_api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 21:04:04.000888 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components.egg-info/
--rw-rw-rw-   0        0        0      989 2024-05-16 21:04:03.000000 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      621 2024-05-16 21:04:03.000000 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 21:04:03.000000 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-05-16 21:04:03.000000 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-16 21:04:03.000000 mbu_dev_shared_components-0.0.5/mbu_dev_shared_components.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      593 2024-05-16 21:03:28.000000 mbu_dev_shared_components-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 21:04:04.012679 mbu_dev_shared_components-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 13:59:13.184469 mbu_dev_shared_components-0.0.6/
+-rw-rw-rw-   0        0        0     3238 2024-05-16 14:14:30.000000 mbu_dev_shared_components-0.0.6/.gitignore
+-rw-rw-rw-   0        0        0     1085 2024-05-16 14:14:30.000000 mbu_dev_shared_components-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      989 2024-05-17 13:59:13.178759 mbu_dev_shared_components-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      498 2024-05-16 15:19:15.000000 mbu_dev_shared_components-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 13:59:13.026980 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components/
+drwxrwxrwx   0        0        0        0 2024-05-17 13:59:13.119929 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components/office365/
+-rw-rw-rw-   0        0        0        0 2024-05-16 14:20:13.000000 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components/office365/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:59:13.155273 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components/office365/excel/
+-rw-rw-rw-   0        0        0        0 2024-05-16 20:18:44.000000 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components/office365/excel/__init__.py
+-rw-rw-rw-   0        0        0     7181 2024-05-17 13:55:50.000000 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components/office365/excel/excel_reader.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:59:13.172933 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components/office365/sharepoint_api/
+-rw-rw-rw-   0        0        0        0 2024-05-16 14:20:46.000000 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components/office365/sharepoint_api/__init__.py
+-rw-rw-rw-   0        0        0     8970 2024-05-16 15:09:46.000000 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components/office365/sharepoint_api/files.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:59:13.172933 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components/os2forms_api/
+-rw-rw-rw-   0        0        0        0 2024-05-16 15:12:48.000000 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components/os2forms_api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:59:13.178759 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components.egg-info/
+-rw-rw-rw-   0        0        0      989 2024-05-17 13:59:12.000000 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      621 2024-05-17 13:59:13.000000 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 13:59:12.000000 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-17 13:59:12.000000 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-17 13:59:12.000000 mbu_dev_shared_components-0.0.6/mbu_dev_shared_components.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      593 2024-05-17 13:58:21.000000 mbu_dev_shared_components-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 13:59:13.187067 mbu_dev_shared_components-0.0.6/setup.cfg
```

### Comparing `mbu_dev_shared_components-0.0.5/.gitignore` & `mbu_dev_shared_components-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `mbu_dev_shared_components-0.0.5/LICENSE` & `mbu_dev_shared_components-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mbu_dev_shared_components-0.0.5/PKG-INFO` & `mbu_dev_shared_components-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbu_dev_shared_components
-Version: 0.0.5
+Version: 0.0.6
 Summary: Shared components to use in RPA projects
 Author-email: MBU <rpa@mbu.aarhus.dk>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `mbu_dev_shared_components-0.0.5/mbu_dev_shared_components/office365/excel/excel_reader.py` & `mbu_dev_shared_components-0.0.6/mbu_dev_shared_components/office365/excel/excel_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             A list of lists where each inner list contains the data from one row.
         """
         sheet = self.workbook[sheet_name]
         data = []
         for row in sheet.iter_rows(min_col=self._col_to_index(start_col),
                                    max_col=self._col_to_index(end_col),
                                    min_row=start_row):
-            row_data = [cell.value for cell in row if cell.value is not None]
+            row_data = [str(cell.value) for cell in row if cell.value is not None]
             data.append(row_data)
 
         if rows_to_remove > 0:
             data = self._remove_rows_from_end(data, rows_to_remove)
 
         return data
```

### Comparing `mbu_dev_shared_components-0.0.5/mbu_dev_shared_components/office365/sharepoint_api/files.py` & `mbu_dev_shared_components-0.0.6/mbu_dev_shared_components/office365/sharepoint_api/files.py`

 * *Files identical despite different names*

### Comparing `mbu_dev_shared_components-0.0.5/mbu_dev_shared_components.egg-info/PKG-INFO` & `mbu_dev_shared_components-0.0.6/mbu_dev_shared_components.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbu_dev_shared_components
-Version: 0.0.5
+Version: 0.0.6
 Summary: Shared components to use in RPA projects
 Author-email: MBU <rpa@mbu.aarhus.dk>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `mbu_dev_shared_components-0.0.5/mbu_dev_shared_components.egg-info/SOURCES.txt` & `mbu_dev_shared_components-0.0.6/mbu_dev_shared_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mbu_dev_shared_components-0.0.5/pyproject.toml` & `mbu_dev_shared_components-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mbu_dev_shared_components"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="MBU", email="rpa@mbu.aarhus.dk" },
 ]
 description = "Shared components to use in RPA projects"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

