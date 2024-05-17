# Comparing `tmp/pandoc-jinja-0.2.2.tar.gz` & `tmp/pandoc_jinja-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandoc-jinja-0.2.2.tar", last modified: Thu Mar  2 17:10:20 2023, max compression
+gzip compressed data, was "pandoc_jinja-0.2.4.tar", last modified: Fri May 17 06:50:49 2024, max compression
```

## Comparing `pandoc-jinja-0.2.2.tar` & `pandoc_jinja-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:10:20.335241 pandoc-jinja-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-03-02 17:10:08.000000 pandoc-jinja-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-03-02 17:10:20.335241 pandoc-jinja-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-03-02 17:10:08.000000 pandoc-jinja-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:10:20.331241 pandoc-jinja-0.2.2/pandoc_jinja.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-03-02 17:10:20.000000 pandoc-jinja-0.2.2/pandoc_jinja.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-02 17:10:20.000000 pandoc-jinja-0.2.2/pandoc_jinja.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 17:10:20.000000 pandoc-jinja-0.2.2/pandoc_jinja.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-02 17:10:20.000000 pandoc-jinja-0.2.2/pandoc_jinja.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-02 17:10:20.000000 pandoc-jinja-0.2.2/pandoc_jinja.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-02 17:10:20.000000 pandoc-jinja-0.2.2/pandoc_jinja.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     2376 2023-03-02 17:10:08.000000 pandoc-jinja-0.2.2/pandoc_jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-03-02 17:10:08.000000 pandoc-jinja-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 17:10:20.335241 pandoc-jinja-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:50:49.785496 pandoc_jinja-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-17 06:50:43.000000 pandoc_jinja-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-17 06:50:49.785496 pandoc_jinja-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-17 06:50:43.000000 pandoc_jinja-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:50:49.785496 pandoc_jinja-0.2.4/pandoc_jinja.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-17 06:50:49.000000 pandoc_jinja-0.2.4/pandoc_jinja.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-17 06:50:49.000000 pandoc_jinja-0.2.4/pandoc_jinja.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 06:50:49.000000 pandoc_jinja-0.2.4/pandoc_jinja.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-17 06:50:49.000000 pandoc_jinja-0.2.4/pandoc_jinja.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-17 06:50:49.000000 pandoc_jinja-0.2.4/pandoc_jinja.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-17 06:50:49.000000 pandoc_jinja-0.2.4/pandoc_jinja.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2509 2024-05-17 06:50:43.000000 pandoc_jinja-0.2.4/pandoc_jinja.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-17 06:50:43.000000 pandoc_jinja-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 06:50:49.785496 pandoc_jinja-0.2.4/setup.cfg
```

### Comparing `pandoc-jinja-0.2.2/LICENSE` & `pandoc_jinja-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pandoc-jinja-0.2.2/PKG-INFO` & `pandoc_jinja-0.2.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: pandoc-jinja
-Version: 0.2.2
+Version: 0.2.4
 Summary: Render pandoc metadata variables inside the document
 Author-email: Damien Clochard <damien.clochard@dalibo.com>
-Project-URL: Homepage, https://github.com/daamien/pandoc-cover
-Project-URL: Bug Tracker, https://github.com/daamien/pandoc-cover/issues
+Project-URL: Homepage, https://github.com/daamien/pandoc-jinja
+Project-URL: Bug Tracker, https://github.com/daamien/pandoc-jinja/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: panflute
+Requires-Dist: jinja2
 
 [![PyPI version](https://badge.fury.io/py/pandoc-jinja.svg)](https://pypi.org/project/pandoc-jinja/)
 
 # pandoc-jinja
 
 Render pandoc metadata inside the document itself
```

### Comparing `pandoc-jinja-0.2.2/README.md` & `pandoc_jinja-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pandoc-jinja-0.2.2/pandoc_jinja.egg-info/PKG-INFO` & `pandoc_jinja-0.2.4/pandoc_jinja.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: pandoc-jinja
-Version: 0.2.2
+Version: 0.2.4
 Summary: Render pandoc metadata variables inside the document
 Author-email: Damien Clochard <damien.clochard@dalibo.com>
-Project-URL: Homepage, https://github.com/daamien/pandoc-cover
-Project-URL: Bug Tracker, https://github.com/daamien/pandoc-cover/issues
+Project-URL: Homepage, https://github.com/daamien/pandoc-jinja
+Project-URL: Bug Tracker, https://github.com/daamien/pandoc-jinja/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: panflute
+Requires-Dist: jinja2
 
 [![PyPI version](https://badge.fury.io/py/pandoc-jinja.svg)](https://pypi.org/project/pandoc-jinja/)
 
 # pandoc-jinja
 
 Render pandoc metadata inside the document itself
```

### Comparing `pandoc-jinja-0.2.2/pyproject.toml` & `pandoc_jinja-0.2.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pandoc-jinja"
-version = "0.2.2"
+version = "0.2.4"
 authors = [
   { name="Damien Clochard", email="damien.clochard@dalibo.com" },
 ]
 description = "Render pandoc metadata variables inside the document"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -15,15 +15,15 @@
 
 dependencies = [
     "panflute",
     "jinja2"
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/daamien/pandoc-cover"
-"Bug Tracker" = "https://github.com/daamien/pandoc-cover/issues"
+"Homepage" = "https://github.com/daamien/pandoc-jinja"
+"Bug Tracker" = "https://github.com/daamien/pandoc-jinja/issues"
 
 [project.scripts]
 pandoc-jinja = 'pandoc_jinja:main'
 
 [tool.setuptools]
 py-modules = ["pandoc_jinja"]
```

