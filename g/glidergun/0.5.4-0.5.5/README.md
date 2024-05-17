# Comparing `tmp/glidergun-0.5.4.tar.gz` & `tmp/glidergun-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glidergun-0.5.4.tar", last modified: Fri May 17 02:15:41 2024, max compression
+gzip compressed data, was "glidergun-0.5.5.tar", last modified: Fri May 17 02:44:31 2024, max compression
```

## Comparing `glidergun-0.5.4.tar` & `glidergun-0.5.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 02:15:41.765731 glidergun-0.5.4/
--rw-rw-rw-   0        0        0     2832 2024-05-17 02:15:41.764395 glidergun-0.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     2148 2024-04-24 03:01:21.000000 glidergun-0.5.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 02:15:41.734629 glidergun-0.5.4/glidergun/
--rw-rw-rw-   0        0        0      438 2024-05-17 02:12:31.000000 glidergun-0.5.4/glidergun/__init__.py
--rw-rw-rw-   0        0        0    50020 2024-05-17 02:12:30.000000 glidergun-0.5.4/glidergun/_grid.py
--rw-rw-rw-   0        0        0     4099 2024-05-17 02:12:37.000000 glidergun-0.5.4/glidergun/_ipython.py
--rw-rw-rw-   0        0        0     1783 2024-04-24 03:01:21.000000 glidergun-0.5.4/glidergun/_literals.py
--rw-rw-rw-   0        0        0    10367 2024-05-17 02:12:25.000000 glidergun-0.5.4/glidergun/_stack.py
-drwxrwxrwx   0        0        0        0 2024-05-17 02:15:41.762972 glidergun-0.5.4/glidergun.egg-info/
--rw-rw-rw-   0        0        0     2832 2024-05-17 02:15:41.000000 glidergun-0.5.4/glidergun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2024-05-17 02:15:41.000000 glidergun-0.5.4/glidergun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 02:15:41.000000 glidergun-0.5.4/glidergun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-05-17 02:15:41.000000 glidergun-0.5.4/glidergun.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-17 02:15:41.000000 glidergun-0.5.4/glidergun.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      746 2024-05-17 02:11:20.000000 glidergun-0.5.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-17 02:15:41.767201 glidergun-0.5.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 02:44:31.473601 glidergun-0.5.5/
+-rw-rw-rw-   0        0        0     2832 2024-05-17 02:44:31.472300 glidergun-0.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2148 2024-04-24 03:01:21.000000 glidergun-0.5.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 02:44:31.442190 glidergun-0.5.5/glidergun/
+-rw-rw-rw-   0        0        0      438 2024-05-17 02:12:31.000000 glidergun-0.5.5/glidergun/__init__.py
+-rw-rw-rw-   0        0        0    50020 2024-05-17 02:12:30.000000 glidergun-0.5.5/glidergun/_grid.py
+-rw-rw-rw-   0        0        0     4200 2024-05-17 02:40:30.000000 glidergun-0.5.5/glidergun/_ipython.py
+-rw-rw-rw-   0        0        0     1783 2024-04-24 03:01:21.000000 glidergun-0.5.5/glidergun/_literals.py
+-rw-rw-rw-   0        0        0    10367 2024-05-17 02:12:25.000000 glidergun-0.5.5/glidergun/_stack.py
+drwxrwxrwx   0        0        0        0 2024-05-17 02:44:31.471025 glidergun-0.5.5/glidergun.egg-info/
+-rw-rw-rw-   0        0        0     2832 2024-05-17 02:44:31.000000 glidergun-0.5.5/glidergun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2024-05-17 02:44:31.000000 glidergun-0.5.5/glidergun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 02:44:31.000000 glidergun-0.5.5/glidergun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-05-17 02:44:31.000000 glidergun-0.5.5/glidergun.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-17 02:44:31.000000 glidergun-0.5.5/glidergun.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      746 2024-05-17 02:36:03.000000 glidergun-0.5.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 02:44:31.474621 glidergun-0.5.5/setup.cfg
```

### Comparing `glidergun-0.5.4/PKG-INFO` & `glidergun-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glidergun
-Version: 0.5.4
+Version: 0.5.5
 Summary: Map Algebra with NumPy
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/glidergun
 Project-URL: Bug Tracker, https://github.com/jshirota/glidergun/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `glidergun-0.5.4/README.md` & `glidergun-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `glidergun-0.5.4/glidergun/_grid.py` & `glidergun-0.5.5/glidergun/_grid.py`

 * *Files identical despite different names*

### Comparing `glidergun-0.5.4/glidergun/_ipython.py` & `glidergun-0.5.5/glidergun/_ipython.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from io import BytesIO
 from typing import Optional, Union
 
 import IPython
 import matplotlib.pyplot as plt
 import numpy as np
 
-from glidergun._grid import Grid
+from glidergun._grid import Grid, Extent
 from glidergun._stack import Stack
 
 
 def _thumbnail(obj: Union[Grid, Stack], color, figsize=None):
     with BytesIO() as buffer:
         figure = plt.figure(figsize=figsize, frameon=False)
         axes = figure.add_axes((0, 0, 1, 1))
@@ -50,17 +50,22 @@
     attribution: Optional[str],
     grayscale: bool = True,
     **kwargs,
 ):
     import folium
     import jinja2
 
-    obj = obj.project(4326)
-    obj_4326 = obj.clip((obj.xmin, max(obj.ymin, -80),
-                        obj.xmax, min(obj.ymax, 80)))
+    obj_4326 = obj.project(4326)
+
+    extent = Extent(obj_4326.xmin, max(obj_4326.ymin, -80),
+                    obj_4326.xmax, min(obj_4326.ymax, 80))
+
+    if obj_4326.extent != extent:
+        obj_4326 = obj.clip(extent)
+
     obj_3857 = obj_4326.project(3857)
 
     figure = folium.Figure(width=str(width), height=height)
     bounds = [[obj_4326.ymin, obj_4326.xmin],
               [obj_4326.ymax, obj_4326.xmax]]
 
     if folium_map is None:
```

### Comparing `glidergun-0.5.4/glidergun/_literals.py` & `glidergun-0.5.5/glidergun/_literals.py`

 * *Files identical despite different names*

### Comparing `glidergun-0.5.4/glidergun/_stack.py` & `glidergun-0.5.5/glidergun/_stack.py`

 * *Files identical despite different names*

### Comparing `glidergun-0.5.4/glidergun.egg-info/PKG-INFO` & `glidergun-0.5.5/glidergun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glidergun
-Version: 0.5.4
+Version: 0.5.5
 Summary: Map Algebra with NumPy
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/glidergun
 Project-URL: Bug Tracker, https://github.com/jshirota/glidergun/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `glidergun-0.5.4/pyproject.toml` & `glidergun-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "glidergun"
-version = "0.5.4"
+version = "0.5.5"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "Map Algebra with NumPy"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

