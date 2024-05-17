# Comparing `tmp/pydlfmt-0.0.8.tar.gz` & `tmp/pydlfmt-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydlfmt-0.0.8.tar", last modified: Mon Jan  2 21:12:20 2023, max compression
+gzip compressed data, was "pydlfmt-0.0.9.tar", last modified: Mon Jan  2 21:15:59 2023, max compression
```

## Comparing `pydlfmt-0.0.8.tar` & `pydlfmt-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 21:12:20.666760 pydlfmt-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-02 21:12:08.000000 pydlfmt-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-01-02 21:12:20.666760 pydlfmt-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-01-02 21:12:08.000000 pydlfmt-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 21:12:20.662760 pydlfmt-0.0.8/pydlfmt/
--rw-r--r--   0 runner    (1001) docker     (123)    32855 2023-01-02 21:12:08.000000 pydlfmt-0.0.8/pydlfmt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 21:12:20.666760 pydlfmt-0.0.8/pydlfmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-01-02 21:12:20.000000 pydlfmt-0.0.8/pydlfmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-01-02 21:12:20.000000 pydlfmt-0.0.8/pydlfmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-02 21:12:20.000000 pydlfmt-0.0.8/pydlfmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-02 21:12:20.000000 pydlfmt-0.0.8/pydlfmt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-02 21:12:20.000000 pydlfmt-0.0.8/pydlfmt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-02 21:12:20.000000 pydlfmt-0.0.8/pydlfmt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-01-02 21:12:08.000000 pydlfmt-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-01-02 21:12:20.666760 pydlfmt-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-01-02 21:12:08.000000 pydlfmt-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 21:15:59.531498 pydlfmt-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-02 21:15:49.000000 pydlfmt-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-01-02 21:15:59.531498 pydlfmt-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-01-02 21:15:49.000000 pydlfmt-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 21:15:59.531498 pydlfmt-0.0.9/pydlfmt/
+-rw-r--r--   0 runner    (1001) docker     (123)    32855 2023-01-02 21:15:49.000000 pydlfmt-0.0.9/pydlfmt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 21:15:59.531498 pydlfmt-0.0.9/pydlfmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-01-02 21:15:59.000000 pydlfmt-0.0.9/pydlfmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-01-02 21:15:59.000000 pydlfmt-0.0.9/pydlfmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-02 21:15:59.000000 pydlfmt-0.0.9/pydlfmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-02 21:15:59.000000 pydlfmt-0.0.9/pydlfmt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-02 21:15:59.000000 pydlfmt-0.0.9/pydlfmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-02 21:15:59.000000 pydlfmt-0.0.9/pydlfmt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-01-02 21:15:49.000000 pydlfmt-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-01-02 21:15:59.531498 pydlfmt-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-01-02 21:15:49.000000 pydlfmt-0.0.9/setup.py
```

### Comparing `pydlfmt-0.0.8/LICENSE` & `pydlfmt-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pydlfmt-0.0.8/PKG-INFO` & `pydlfmt-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydlfmt
-Version: 0.0.8
+Version: 0.0.9
 Summary: pydlfmt will take a list of objects, dicts, etc and output them to a PDF or XLSX
 Home-page: https://github.com/jpsteil/pydlfmt
 Author: Jim Steil
 Author-email: jim@steilonline.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydlfmt-0.0.8/README.md` & `pydlfmt-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pydlfmt-0.0.8/pydlfmt/__init__.py` & `pydlfmt-0.0.9/pydlfmt/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -41,17 +41,14 @@
         self.columns = []
         self.data = data if data else []
 
         self.sections = []
 
         self.scalar_heading_column = 1
 
-        self.inch = inch
-        self.colors = colors
-
     def get_username(self):
         """
         override this method to build your username from the passed user id
         """
         return self.user_id
 
     def to_pdf(
@@ -581,14 +578,17 @@
         self.doc = None
 
         if self.orientation.upper() == "LANDSCAPE":
             self.pagesize = pagesizes.landscape(pagesizes.letter)
         else:
             self.pagesize = pagesizes.letter
 
+        self.inch = inch
+        self.colors = colors
+
         self.top_margin = 1.25 * inch + (0.5 * len(self.headings) - 1) * inch
         self.bottom_margin = 0.5 * inch
         self.left_margin = 0.5 * inch
         self.right_margin = 0.5 * inch
 
         self.date_format = date_format
```

### Comparing `pydlfmt-0.0.8/pydlfmt.egg-info/PKG-INFO` & `pydlfmt-0.0.9/pydlfmt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydlfmt
-Version: 0.0.8
+Version: 0.0.9
 Summary: pydlfmt will take a list of objects, dicts, etc and output them to a PDF or XLSX
 Home-page: https://github.com/jpsteil/pydlfmt
 Author: Jim Steil
 Author-email: jim@steilonline.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydlfmt-0.0.8/setup.cfg` & `pydlfmt-0.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pydlfmt
-version = v0.0.8
+version = v0.0.9
 author = Jim Steil
 author_email = jim@steilonline.com
 description = Quickly format lists of data as PDF or Excel
 long_description = file: README.md
 description_file = README.md
 long_description_content_type = text/markdown
 url = https://github.com/jpsteil/pydlfmt
```

### Comparing `pydlfmt-0.0.8/setup.py` & `pydlfmt-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # with open("README.md", "r", encoding="utf-8") as fh:
 #     long_description = fh.read()
 
 setup(
     name="pydlfmt",
     # package_dir={"": ""},
     packages=["pydlfmt"],
-    version="v0.0.8",  # Ideally should be same as your GitHub release tag version
+    version="v0.0.9",  # Ideally should be same as your GitHub release tag version
     description="pydlfmt will take a list of objects, dicts, etc and output them to a PDF or XLSX",
     author="Jim Steil",
     author_email="jim@steilonline.com",
     # long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jpsteil/pydlfmt",
     #     download_url="https://github.com/jpsteil/pydlfmt/archive/refs/tags/v0.0.1.tar.gz",
```

