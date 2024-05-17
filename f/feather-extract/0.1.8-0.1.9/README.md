# Comparing `tmp/feather_extract-0.1.8.tar.gz` & `tmp/feather_extract-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jonathanhofmann/Desktop/base folder/dist/.tmp-p01zcot2/feather_extract-0.1.8.tar", last modified: Fri May 17 02:14:26 2024, max compression
+gzip compressed data, was "/Users/jonathanhofmann/Desktop/base folder/dist/.tmp-dg6v10do/feather_extract-0.1.9.tar", last modified: Fri May 17 02:27:45 2024, max compression
```

## Comparing `feather_extract-0.1.8.tar` & `feather_extract-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jonathanhofmann   (501) staff       (20)        0 2024-05-17 02:14:26.023209 feather_extract-0.1.8/
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)        0 2024-05-17 02:12:14.000000 feather_extract-0.1.8/MANIFEST.in
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)     3334 2024-05-17 02:14:26.022930 feather_extract-0.1.8/PKG-INFO
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)     2694 2024-05-16 21:46:44.000000 feather_extract-0.1.8/README.md
-drwxr-xr-x   0 jonathanhofmann   (501) staff       (20)        0 2024-05-17 02:14:26.018407 feather_extract-0.1.8/feather_extract/
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)      167 2024-05-16 19:50:44.000000 feather_extract-0.1.8/feather_extract/__init__.py
-drwxr-xr-x   0 jonathanhofmann   (501) staff       (20)        0 2024-05-17 02:14:26.020816 feather_extract-0.1.8/feather_extract/data/
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)   257204 2024-05-17 01:28:12.000000 feather_extract-0.1.8/feather_extract/data/standard-form-filled-out.pdf
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)   911064 2024-05-16 19:49:23.000000 feather_extract-0.1.8/feather_extract/data/standard_form.pdf
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)      391 2024-05-17 00:45:12.000000 feather_extract-0.1.8/feather_extract/excel_writer.py
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)      703 2024-05-15 21:36:11.000000 feather_extract-0.1.8/feather_extract/extract_text.py
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)     1100 2024-05-15 21:47:36.000000 feather_extract-0.1.8/feather_extract/format_text.py
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)     1016 2024-05-17 00:41:37.000000 feather_extract-0.1.8/feather_extract/forms.py
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)      185 2024-05-15 21:36:13.000000 feather_extract-0.1.8/feather_extract/utils.py
-drwxr-xr-x   0 jonathanhofmann   (501) staff       (20)        0 2024-05-17 02:14:26.022600 feather_extract-0.1.8/feather_extract.egg-info/
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)     3334 2024-05-17 02:14:26.000000 feather_extract-0.1.8/feather_extract.egg-info/PKG-INFO
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)      492 2024-05-17 02:14:26.000000 feather_extract-0.1.8/feather_extract.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)        1 2024-05-17 02:14:26.000000 feather_extract-0.1.8/feather_extract.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)       47 2024-05-17 02:14:26.000000 feather_extract-0.1.8/feather_extract.egg-info/requires.txt
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)       16 2024-05-17 02:14:26.000000 feather_extract-0.1.8/feather_extract.egg-info/top_level.txt
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)      838 2024-05-17 02:14:14.000000 feather_extract-0.1.8/pyproject.toml
--rw-r--r--   0 jonathanhofmann   (501) staff       (20)       38 2024-05-17 02:14:26.023274 feather_extract-0.1.8/setup.cfg
+drwxr-xr-x   0 jonathanhofmann   (501) staff       (20)        0 2024-05-17 02:27:45.288064 feather_extract-0.1.9/
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)      105 2024-05-17 02:26:05.000000 feather_extract-0.1.9/MANIFEST.in
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)     3273 2024-05-17 02:27:45.287768 feather_extract-0.1.9/PKG-INFO
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)     2694 2024-05-16 21:46:44.000000 feather_extract-0.1.9/README.md
+drwxr-xr-x   0 jonathanhofmann   (501) staff       (20)        0 2024-05-17 02:27:45.283435 feather_extract-0.1.9/feather_extract/
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)      167 2024-05-16 19:50:44.000000 feather_extract-0.1.9/feather_extract/__init__.py
+drwxr-xr-x   0 jonathanhofmann   (501) staff       (20)        0 2024-05-17 02:27:45.285686 feather_extract-0.1.9/feather_extract/data/
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)   257204 2024-05-17 01:28:12.000000 feather_extract-0.1.9/feather_extract/data/standard-form-filled-out.pdf
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)   911064 2024-05-16 19:49:23.000000 feather_extract-0.1.9/feather_extract/data/standard_form.pdf
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)      391 2024-05-17 00:45:12.000000 feather_extract-0.1.9/feather_extract/excel_writer.py
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)      703 2024-05-15 21:36:11.000000 feather_extract-0.1.9/feather_extract/extract_text.py
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)     1100 2024-05-15 21:47:36.000000 feather_extract-0.1.9/feather_extract/format_text.py
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)     1016 2024-05-17 00:41:37.000000 feather_extract-0.1.9/feather_extract/forms.py
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)      185 2024-05-15 21:36:13.000000 feather_extract-0.1.9/feather_extract/utils.py
+drwxr-xr-x   0 jonathanhofmann   (501) staff       (20)        0 2024-05-17 02:27:45.287423 feather_extract-0.1.9/feather_extract.egg-info/
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)     3273 2024-05-17 02:27:45.000000 feather_extract-0.1.9/feather_extract.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)      492 2024-05-17 02:27:45.000000 feather_extract-0.1.9/feather_extract.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)        1 2024-05-17 02:27:45.000000 feather_extract-0.1.9/feather_extract.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)       47 2024-05-17 02:27:45.000000 feather_extract-0.1.9/feather_extract.egg-info/requires.txt
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)       16 2024-05-17 02:27:45.000000 feather_extract-0.1.9/feather_extract.egg-info/top_level.txt
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)      777 2024-05-17 02:27:34.000000 feather_extract-0.1.9/pyproject.toml
+-rw-r--r--   0 jonathanhofmann   (501) staff       (20)       38 2024-05-17 02:27:45.288130 feather_extract-0.1.9/setup.cfg
```

### Comparing `feather_extract-0.1.8/PKG-INFO` & `feather_extract-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: feather_extract
-Version: 0.1.8
-Summary: A package for extracting handwritten data from PDF documents, and returning an Excel workbook output. Designed for bar / restaurant industry inventory management.
+Version: 0.1.9
+Summary: A package for extracting handwritten data from PDF documents, and returning an Excel workbook output.
 Author-email: Jonathan Hofmann <awsjonathan99@gmail.com>
 License: MIT
 Project-URL: Homepage, https://www.featherdata.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `feather_extract-0.1.8/README.md` & `feather_extract-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `feather_extract-0.1.8/feather_extract/data/standard-form-filled-out.pdf` & `feather_extract-0.1.9/feather_extract/data/standard-form-filled-out.pdf`

 * *Files identical despite different names*

### Comparing `feather_extract-0.1.8/feather_extract/data/standard_form.pdf` & `feather_extract-0.1.9/feather_extract/data/standard_form.pdf`

 * *Files identical despite different names*

### Comparing `feather_extract-0.1.8/feather_extract/extract_text.py` & `feather_extract-0.1.9/feather_extract/extract_text.py`

 * *Files identical despite different names*

### Comparing `feather_extract-0.1.8/feather_extract/format_text.py` & `feather_extract-0.1.9/feather_extract/format_text.py`

 * *Files identical despite different names*

### Comparing `feather_extract-0.1.8/feather_extract/forms.py` & `feather_extract-0.1.9/feather_extract/forms.py`

 * *Files identical despite different names*

### Comparing `feather_extract-0.1.8/feather_extract.egg-info/PKG-INFO` & `feather_extract-0.1.9/feather_extract.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: feather_extract
-Version: 0.1.8
-Summary: A package for extracting handwritten data from PDF documents, and returning an Excel workbook output. Designed for bar / restaurant industry inventory management.
+Version: 0.1.9
+Summary: A package for extracting handwritten data from PDF documents, and returning an Excel workbook output.
 Author-email: Jonathan Hofmann <awsjonathan99@gmail.com>
 License: MIT
 Project-URL: Homepage, https://www.featherdata.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `feather_extract-0.1.8/pyproject.toml` & `feather_extract-0.1.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "feather_extract"
-version = "0.1.8"
-description = "A package for extracting handwritten data from PDF documents, and returning an Excel workbook output. Designed for bar / restaurant industry inventory management."
+version = "0.1.9"
+description = "A package for extracting handwritten data from PDF documents, and returning an Excel workbook output."
 readme = "README.md"
 authors = [
     { name = "Jonathan Hofmann", email = "awsjonathan99@gmail.com" }
 ]
 dependencies = [
     "azure-ai-formrecognizer==3.3.3",
     "openpyxl==3.1.2"
```

