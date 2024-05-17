# Comparing `tmp/feather_extract-0.1.5.tar.gz` & `tmp/feather_extract-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jonathanhofmann/Desktop/base folder/dist/.tmp-qg23y2mw/feather_extract-0.1.5.tar", last modified: Fri May 17 01:08:22 2024, max compression
+gzip compressed data, was "/Users/jonathanhofmann/Desktop/base folder/dist/.tmp-kztg7eew/feather_extract-0.1.6.tar", last modified: Fri May 17 01:59:26 2024, max compression
```

## Comparing `feather_extract-0.1.5.tar` & `feather_extract-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jonathanhofmann   (501) staff       (20)        0 2024-05-17 01:08:22.295200 feather_extract-0.1.5/
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)     3339 2024-05-17 01:08:22.294914 feather_extract-0.1.5/PKG-INFO
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)     2694 2024-05-16 21:46:44.000000 feather_extract-0.1.5/README.md
-drwxr-xr-x   0 jonathanhofmann   (501) staff       (20)        0 2024-05-17 01:08:22.293588 feather_extract-0.1.5/feather_extract/
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)      167 2024-05-16 19:50:44.000000 feather_extract-0.1.5/feather_extract/__init__.py
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)      391 2024-05-17 00:45:12.000000 feather_extract-0.1.5/feather_extract/excel_writer.py
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)      703 2024-05-15 21:36:11.000000 feather_extract-0.1.5/feather_extract/extract_text.py
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)     1100 2024-05-15 21:47:36.000000 feather_extract-0.1.5/feather_extract/format_text.py
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)     1016 2024-05-17 00:41:37.000000 feather_extract-0.1.5/feather_extract/forms.py
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)      185 2024-05-15 21:36:13.000000 feather_extract-0.1.5/feather_extract/utils.py
-drwxr-xr-x   0 jonathanhofmann   (501) staff       (20)        0 2024-05-17 01:08:22.294633 feather_extract-0.1.5/feather_extract.egg-info/
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)     3339 2024-05-17 01:08:22.000000 feather_extract-0.1.5/feather_extract.egg-info/PKG-INFO
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)      391 2024-05-17 01:08:22.000000 feather_extract-0.1.5/feather_extract.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)        1 2024-05-17 01:08:22.000000 feather_extract-0.1.5/feather_extract.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)       47 2024-05-17 01:08:22.000000 feather_extract-0.1.5/feather_extract.egg-info/requires.txt
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)       16 2024-05-17 01:08:22.000000 feather_extract-0.1.5/feather_extract.egg-info/top_level.txt
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)      760 2024-05-17 01:08:15.000000 feather_extract-0.1.5/pyproject.toml
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)       38 2024-05-17 01:08:22.295270 feather_extract-0.1.5/setup.cfg
+drwxr-xr-x   0 jonathanhofmann   (501) staff       (20)        0 2024-05-17 01:59:26.452260 feather_extract-0.1.6/
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)     3334 2024-05-17 01:59:26.451961 feather_extract-0.1.6/PKG-INFO
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)     2694 2024-05-16 21:46:44.000000 feather_extract-0.1.6/README.md
+drwxr-xr-x   0 jonathanhofmann   (501) staff       (20)        0 2024-05-17 01:59:26.450312 feather_extract-0.1.6/feather_extract/
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)      167 2024-05-16 19:50:44.000000 feather_extract-0.1.6/feather_extract/__init__.py
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)      391 2024-05-17 00:45:12.000000 feather_extract-0.1.6/feather_extract/excel_writer.py
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)      703 2024-05-15 21:36:11.000000 feather_extract-0.1.6/feather_extract/extract_text.py
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)     1100 2024-05-15 21:47:36.000000 feather_extract-0.1.6/feather_extract/format_text.py
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)     1016 2024-05-17 00:41:37.000000 feather_extract-0.1.6/feather_extract/forms.py
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)      185 2024-05-15 21:36:13.000000 feather_extract-0.1.6/feather_extract/utils.py
+drwxr-xr-x   0 jonathanhofmann   (501) staff       (20)        0 2024-05-17 01:59:26.451640 feather_extract-0.1.6/feather_extract.egg-info/
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)     3334 2024-05-17 01:59:26.000000 feather_extract-0.1.6/feather_extract.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)      391 2024-05-17 01:59:26.000000 feather_extract-0.1.6/feather_extract.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)        1 2024-05-17 01:59:26.000000 feather_extract-0.1.6/feather_extract.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)       47 2024-05-17 01:59:26.000000 feather_extract-0.1.6/feather_extract.egg-info/requires.txt
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)       16 2024-05-17 01:59:26.000000 feather_extract-0.1.6/feather_extract.egg-info/top_level.txt
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)      770 2024-05-17 01:56:08.000000 feather_extract-0.1.6/pyproject.toml
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)       38 2024-05-17 01:59:26.452320 feather_extract-0.1.6/setup.cfg
```

### Comparing `feather_extract-0.1.5/PKG-INFO` & `feather_extract-0.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: feather_extract
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for extracting handwritten data from PDF documents, and returning an Excel workbook output. Designed for bar / restaurant industry inventory management.
 Author-email: Jonathan Hofmann <awsjonathan99@gmail.com>
-Project-URL: Homepage, https://github.com/hofmannj0n/feather-extract
+License: MIT
+Project-URL: Homepage, https://www.featherdata.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: azure-ai-formrecognizer==3.3.3
 Requires-Dist: openpyxl==3.1.2
```

### Comparing `feather_extract-0.1.5/README.md` & `feather_extract-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `feather_extract-0.1.5/feather_extract/extract_text.py` & `feather_extract-0.1.6/feather_extract/extract_text.py`

 * *Files identical despite different names*

### Comparing `feather_extract-0.1.5/feather_extract/format_text.py` & `feather_extract-0.1.6/feather_extract/format_text.py`

 * *Files identical despite different names*

### Comparing `feather_extract-0.1.5/feather_extract/forms.py` & `feather_extract-0.1.6/feather_extract/forms.py`

 * *Files identical despite different names*

### Comparing `feather_extract-0.1.5/feather_extract.egg-info/PKG-INFO` & `feather_extract-0.1.6/feather_extract.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: feather_extract
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for extracting handwritten data from PDF documents, and returning an Excel workbook output. Designed for bar / restaurant industry inventory management.
 Author-email: Jonathan Hofmann <awsjonathan99@gmail.com>
-Project-URL: Homepage, https://github.com/hofmannj0n/feather-extract
+License: MIT
+Project-URL: Homepage, https://www.featherdata.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: azure-ai-formrecognizer==3.3.3
 Requires-Dist: openpyxl==3.1.2
```

### Comparing `feather_extract-0.1.5/pyproject.toml` & `feather_extract-0.1.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "feather_extract"
-version = "0.1.5"
+version = "0.1.6"
 description = "A package for extracting handwritten data from PDF documents, and returning an Excel workbook output. Designed for bar / restaurant industry inventory management."
 readme = "README.md"
 authors = [
     { name = "Jonathan Hofmann", email = "awsjonathan99@gmail.com" }
 ]
 dependencies = [
     "azure-ai-formrecognizer==3.3.3",
@@ -16,12 +16,14 @@
 ]
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
-urls = { "Homepage" = "https://github.com/hofmannj0n/feather-extract" }
+license = { text = "MIT" }
+urls = { "Homepage" = "https://www.featherdata.io/" }
+
```

