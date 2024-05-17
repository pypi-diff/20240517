# Comparing `tmp/mkdocs-kroki-plugin-0.7.0.tar.gz` & `tmp/mkdocs-kroki-plugin-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-kroki-plugin-0.7.0.tar", last modified: Sun Jan  7 07:13:12 2024, max compression
+gzip compressed data, was "mkdocs-kroki-plugin-0.7.1.tar", last modified: Sun Jan 21 15:26:23 2024, max compression
```

## Comparing `mkdocs-kroki-plugin-0.7.0.tar` & `mkdocs-kroki-plugin-0.7.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 07:13:12.221202 mkdocs-kroki-plugin-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-01-07 07:13:00.000000 mkdocs-kroki-plugin-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-01-07 07:13:12.217202 mkdocs-kroki-plugin-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-01-07 07:13:00.000000 mkdocs-kroki-plugin-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 07:13:12.217202 mkdocs-kroki-plugin-0.7.0/kroki/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-07 07:13:00.000000 mkdocs-kroki-plugin-0.7.0/kroki/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-01-07 07:13:00.000000 mkdocs-kroki-plugin-0.7.0/kroki/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-01-07 07:13:00.000000 mkdocs-kroki-plugin-0.7.0/kroki/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-01-07 07:13:00.000000 mkdocs-kroki-plugin-0.7.0/kroki/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-01-07 07:13:00.000000 mkdocs-kroki-plugin-0.7.0/kroki/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 07:13:12.217202 mkdocs-kroki-plugin-0.7.0/mkdocs_kroki_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-01-07 07:13:12.000000 mkdocs-kroki-plugin-0.7.0/mkdocs_kroki_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-01-07 07:13:12.000000 mkdocs-kroki-plugin-0.7.0/mkdocs_kroki_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-07 07:13:12.000000 mkdocs-kroki-plugin-0.7.0/mkdocs_kroki_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-07 07:13:12.000000 mkdocs-kroki-plugin-0.7.0/mkdocs_kroki_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-07 07:13:12.000000 mkdocs-kroki-plugin-0.7.0/mkdocs_kroki_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-07 07:13:12.000000 mkdocs-kroki-plugin-0.7.0/mkdocs_kroki_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-07 07:13:12.221202 mkdocs-kroki-plugin-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-01-07 07:13:00.000000 mkdocs-kroki-plugin-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 15:26:23.594184 mkdocs-kroki-plugin-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-01-21 15:26:13.000000 mkdocs-kroki-plugin-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-01-21 15:26:23.590184 mkdocs-kroki-plugin-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-01-21 15:26:13.000000 mkdocs-kroki-plugin-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 15:26:23.590184 mkdocs-kroki-plugin-0.7.1/kroki/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-21 15:26:13.000000 mkdocs-kroki-plugin-0.7.1/kroki/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-01-21 15:26:13.000000 mkdocs-kroki-plugin-0.7.1/kroki/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-01-21 15:26:13.000000 mkdocs-kroki-plugin-0.7.1/kroki/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-01-21 15:26:13.000000 mkdocs-kroki-plugin-0.7.1/kroki/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-01-21 15:26:13.000000 mkdocs-kroki-plugin-0.7.1/kroki/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 15:26:23.590184 mkdocs-kroki-plugin-0.7.1/mkdocs_kroki_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-01-21 15:26:23.000000 mkdocs-kroki-plugin-0.7.1/mkdocs_kroki_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-01-21 15:26:23.000000 mkdocs-kroki-plugin-0.7.1/mkdocs_kroki_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-21 15:26:23.000000 mkdocs-kroki-plugin-0.7.1/mkdocs_kroki_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-21 15:26:23.000000 mkdocs-kroki-plugin-0.7.1/mkdocs_kroki_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-21 15:26:23.000000 mkdocs-kroki-plugin-0.7.1/mkdocs_kroki_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-21 15:26:23.000000 mkdocs-kroki-plugin-0.7.1/mkdocs_kroki_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-21 15:26:23.594184 mkdocs-kroki-plugin-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-01-21 15:26:13.000000 mkdocs-kroki-plugin-0.7.1/setup.py
```

### Comparing `mkdocs-kroki-plugin-0.7.0/LICENSE` & `mkdocs-kroki-plugin-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-kroki-plugin-0.7.0/PKG-INFO` & `mkdocs-kroki-plugin-0.7.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: mkdocs-kroki-plugin
-Version: 0.7.0
+Version: 0.7.1
 Summary: MkDocs plugin for Kroki-Diagrams
 Home-page: https://github.com/AVATEAM-IT-SYSTEMHAUS/mkdocs-kroki-plugin
 Author: Benjamin Bittner
 Author-email: benjamin.bittner@avateam.com
 License: MIT
 Keywords: mkdocs python markdown kroi diagram
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mkdocs>=1.4.0
+Requires-Dist: mkdocs>=1.5.0
 Requires-Dist: requests>=2.27.0
 
 # mkdocs-kroki-plugin
 
 This is a MkDocs plugin to embed Kroki-Diagrams into your documentation.
 
 ## Setup
```

### Comparing `mkdocs-kroki-plugin-0.7.0/README.md` & `mkdocs-kroki-plugin-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-kroki-plugin-0.7.0/kroki/client.py` & `mkdocs-kroki-plugin-0.7.1/kroki/client.py`

 * *Files identical despite different names*

### Comparing `mkdocs-kroki-plugin-0.7.0/kroki/config.py` & `mkdocs-kroki-plugin-0.7.1/kroki/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs-kroki-plugin-0.7.0/kroki/plugin.py` & `mkdocs-kroki-plugin-0.7.1/kroki/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-kroki-plugin-0.7.0/kroki/util.py` & `mkdocs-kroki-plugin-0.7.1/kroki/util.py`

 * *Files identical despite different names*

### Comparing `mkdocs-kroki-plugin-0.7.0/mkdocs_kroki_plugin.egg-info/PKG-INFO` & `mkdocs-kroki-plugin-0.7.1/mkdocs_kroki_plugin.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: mkdocs-kroki-plugin
-Version: 0.7.0
+Version: 0.7.1
 Summary: MkDocs plugin for Kroki-Diagrams
 Home-page: https://github.com/AVATEAM-IT-SYSTEMHAUS/mkdocs-kroki-plugin
 Author: Benjamin Bittner
 Author-email: benjamin.bittner@avateam.com
 License: MIT
 Keywords: mkdocs python markdown kroi diagram
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mkdocs>=1.4.0
+Requires-Dist: mkdocs>=1.5.0
 Requires-Dist: requests>=2.27.0
 
 # mkdocs-kroki-plugin
 
 This is a MkDocs plugin to embed Kroki-Diagrams into your documentation.
 
 ## Setup
```

### Comparing `mkdocs-kroki-plugin-0.7.0/setup.py` & `mkdocs-kroki-plugin-0.7.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,36 +4,34 @@
 # read the contents of your README file
 PROJ_DIR = Path(__file__).resolve().parent
 with open(PROJ_DIR / "README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="mkdocs-kroki-plugin",
-    version="0.7.0",
+    version="0.7.1",
     description="MkDocs plugin for Kroki-Diagrams",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="mkdocs python markdown kroi diagram",
     url="https://github.com/AVATEAM-IT-SYSTEMHAUS/mkdocs-kroki-plugin",
     author="Benjamin Bittner",
     author_email="benjamin.bittner@avateam.com",
     license="MIT",
-    python_requires=">=3.6",
-    install_requires=["mkdocs>=1.4.0", "requests>=2.27.0"],
+    python_requires=">=3.10",
+    install_requires=["mkdocs>=1.5.0", "requests>=2.27.0"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+        "Programming Language :: Python :: 3.13",
     ],
     packages=find_packages(),
     entry_points={"mkdocs.plugins": ["kroki = kroki.plugin:KrokiPlugin"]},
 )
```

