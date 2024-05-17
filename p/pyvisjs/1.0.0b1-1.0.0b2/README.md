# Comparing `tmp/pyvisjs-1.0.0b1.tar.gz` & `tmp/pyvisjs-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvisjs-1.0.0b1.tar", last modified: Wed May 15 12:34:06 2024, max compression
+gzip compressed data, was "pyvisjs-1.0.0b2.tar", last modified: Fri May 17 09:42:44 2024, max compression
```

## Comparing `pyvisjs-1.0.0b1.tar` & `pyvisjs-1.0.0b2.tar`

### file list

```diff
@@ -1,44 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:34:06.089287 pyvisjs-1.0.0b1/
--rw-rw-rw-   0 root         (0) root         (0)     1396 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      979 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     4169 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3321 2024-05-15 12:34:06.089287 pyvisjs-1.0.0b1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1394 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:34:06.082287 pyvisjs-1.0.0b1/examples/
--rw-rw-rw-   0 root         (0) root         (0)     8663 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/examples/bluor.py
--rw-rw-rw-   0 root         (0) root         (0)      289 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/examples/readme.py
--rw-rw-rw-   0 root         (0) root         (0)      959 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/folder_structure.txt
--rw-rw-rw-   0 root         (0) root         (0)      890 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:34:06.084287 pyvisjs-1.0.0b1/pyvisjs/
--rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2018 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/base_dictable.py
--rw-rw-rw-   0 root         (0) root         (0)     1274 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/edge.py
--rw-rw-rw-   0 root         (0) root         (0)     8831 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/network.py
--rw-rw-rw-   0 root         (0) root         (0)      590 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/node.py
--rw-rw-rw-   0 root         (0) root         (0)    13062 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:34:06.086287 pyvisjs-1.0.0b1/pyvisjs/templates/
--rw-rw-rw-   0 root         (0) root         (0)      792 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/templates/base.html
--rw-rw-rw-   0 root         (0) root         (0)      198 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/templates/basic.html
--rw-rw-rw-   0 root         (0) root         (0)     1193 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/templates/bs-container.html
--rw-rw-rw-   0 root         (0) root         (0)     9063 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/templates/functions.js
--rw-rw-rw-   0 root         (0) root         (0)      840 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/templates/select-edge-filter.html
--rw-rw-rw-   0 root         (0) root         (0)     1542 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/templates/tom-select.html
--rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/pyvisjs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:34:06.088287 pyvisjs-1.0.0b1/pyvisjs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3321 2024-05-15 12:34:06.000000 pyvisjs-1.0.0b1/pyvisjs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      803 2024-05-15 12:34:06.000000 pyvisjs-1.0.0b1/pyvisjs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 12:34:06.000000 pyvisjs-1.0.0b1/pyvisjs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-05-15 12:34:06.000000 pyvisjs-1.0.0b1/pyvisjs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-05-15 12:34:06.000000 pyvisjs-1.0.0b1/pyvisjs.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 12:34:06.089287 pyvisjs-1.0.0b1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 12:34:06.088287 pyvisjs-1.0.0b1/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1921 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/tests/test_base_dictable.py
--rw-rw-rw-   0 root         (0) root         (0)     1006 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/tests/test_edge.py
--rw-rw-rw-   0 root         (0) root         (0)    12014 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/tests/test_network.py
--rw-rw-rw-   0 root         (0) root         (0)     2399 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/tests/test_node.py
--rw-rw-rw-   0 root         (0) root         (0)     3863 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/tests/test_options.py
--rw-rw-rw-   0 root         (0) root         (0)     2561 2024-05-15 12:33:48.000000 pyvisjs-1.0.0b1/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 09:42:44.515450 pyvisjs-1.0.0b2/
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4169 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3331 2024-05-17 09:42:44.515450 pyvisjs-1.0.0b2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1404 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 09:42:44.508450 pyvisjs-1.0.0b2/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     8970 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/examples/bluor.py
+-rw-rw-rw-   0 root         (0) root         (0)      481 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/examples/readme.py
+-rw-rw-rw-   0 root         (0) root         (0)      959 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/folder_structure.txt
+-rw-rw-rw-   0 root         (0) root         (0)      890 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 09:42:44.509450 pyvisjs-1.0.0b2/pyvisjs/
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2018 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/base_dictable.py
+-rw-rw-rw-   0 root         (0) root         (0)     1274 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/edge.py
+-rw-rw-rw-   0 root         (0) root         (0)    10718 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/network.py
+-rw-rw-rw-   0 root         (0) root         (0)      590 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/node.py
+-rw-rw-rw-   0 root         (0) root         (0)    13394 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 09:42:44.512450 pyvisjs-1.0.0b2/pyvisjs/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      966 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/templates/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/templates/basic.html
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/templates/bs-container.html
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/templates/create_network.js
+-rw-rw-rw-   0 root         (0) root         (0)      926 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/templates/draw_title.js
+-rw-rw-rw-   0 root         (0) root         (0)     7594 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/templates/functions.js
+-rw-rw-rw-   0 root         (0) root         (0)      516 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/templates/init_tomSelect.js
+-rw-rw-rw-   0 root         (0) root         (0)      840 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/templates/select-edge-filter.html
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/templates/tom-select.html
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/pyvisjs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 09:42:44.514450 pyvisjs-1.0.0b2/pyvisjs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3331 2024-05-17 09:42:44.000000 pyvisjs-1.0.0b2/pyvisjs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      907 2024-05-17 09:42:44.000000 pyvisjs-1.0.0b2/pyvisjs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 09:42:44.000000 pyvisjs-1.0.0b2/pyvisjs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-17 09:42:44.000000 pyvisjs-1.0.0b2/pyvisjs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-17 09:42:44.000000 pyvisjs-1.0.0b2/pyvisjs.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 09:42:44.515450 pyvisjs-1.0.0b2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 09:42:44.514450 pyvisjs-1.0.0b2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1921 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/tests/test_base_dictable.py
+-rw-rw-rw-   0 root         (0) root         (0)     1006 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/tests/test_edge.py
+-rw-rw-rw-   0 root         (0) root         (0)    11958 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/tests/test_network.py
+-rw-rw-rw-   0 root         (0) root         (0)     2399 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/tests/test_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     3863 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/tests/test_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     2561 2024-05-17 09:42:28.000000 pyvisjs-1.0.0b2/tests/test_utils.py
```

### Comparing `pyvisjs-1.0.0b1/.gitignore` & `pyvisjs-1.0.0b2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b1/.gitlab-ci.yml` & `pyvisjs-1.0.0b2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b1/CONTRIBUTING.md` & `pyvisjs-1.0.0b2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b1/LICENSE` & `pyvisjs-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b1/PKG-INFO` & `pyvisjs-1.0.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisjs
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: A Python wrapper for vis.js Network
 Author-email: Andrey Morozov <andrey@morozov.lv>
 License: MIT License
         
         Copyright (c) 2024 Andrey Morozov (andrey@morozov.lv)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,16 +42,16 @@
 # pyvisjs: Python Wrapper for vis.js Network
 
 pyvisjs is a Python package designed to provide seamless interaction with [vis.js](https://visjs.org) network visualizations, allowing users to manipulate and visualize network data using Python.
 
 ## Workflow
 
 1. Create a network using python
-2. Apply standatd vis.js options such as colors, shapes or physics
-3. Apply pyvisjs specific options such as filtering or highlighting
+2. Apply standard vis.js options such as colors, shapes or physics
+3. Apply pyvisjs specific options such as node/edge filtering or highlighting
 4. Show or generate html file
 5. Enjoy network interactions in your browser
 
 ## Installation
 
 You can install PyVisjs via pip:
```

### Comparing `pyvisjs-1.0.0b1/README.md` & `pyvisjs-1.0.0b2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # pyvisjs: Python Wrapper for vis.js Network
 
 pyvisjs is a Python package designed to provide seamless interaction with [vis.js](https://visjs.org) network visualizations, allowing users to manipulate and visualize network data using Python.
 
 ## Workflow
 
 1. Create a network using python
-2. Apply standatd vis.js options such as colors, shapes or physics
-3. Apply pyvisjs specific options such as filtering or highlighting
+2. Apply standard vis.js options such as colors, shapes or physics
+3. Apply pyvisjs specific options such as node/edge filtering or highlighting
 4. Show or generate html file
 5. Enjoy network interactions in your browser
 
 ## Installation
 
 You can install PyVisjs via pip:
```

### Comparing `pyvisjs-1.0.0b1/examples/bluor.py` & `pyvisjs-1.0.0b2/examples/bluor.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,25 +74,34 @@
         color = "lime"
         shape = "dot"
         size = SMALL_SIZE
         second_line = "\n" + node[1:]
 
     return (color, shape, size, second_line)
 
-options = Options()
+####################
+try_gummy = True  
+####################
+springConstant = (0.05 if try_gummy else 0)
+damping = (0.05 if try_gummy else 0)
+
+options = Options("800px", "1300px")
 options \
     .set_configure(enabled=False) \
     .set_interaction(dragNodes=True, hideEdgesOnDrag=False, hideNodesOnDrag=False)
+options.nodes \
+    .set_font(face="JetBrains Mono")
 options.edges \
     .set_color(inherit=True) \
+    .set_font(face="JetBrains Mono") \
     .set_smooth(type="dynamic", enabled=True) \
     .set(arrows="to", arrowStrikethrough=False)
 options.physics \
     .set(enabled=True) \
-    .set_barnesHut(avoidOverlap=0, centralGravity=0.3, damping=1, gravitationalConstant=-2750, springConstant=0, springLength=250) \
+    .set_barnesHut(avoidOverlap=0, centralGravity=0.3, damping=damping, gravitationalConstant=-2750, springConstant=springConstant, springLength=250) \
     .set_stabilization(enabled=True, fit=True, iterations=1000, onlyDynamicEdges=False, updateInterval=50)
 
 net = Network(options=options)
 
 for (index, row) in df.iterrows():
     (color1, shape1, size1, second_line1) = get_color_and_shape(row["Partner1Node"], row["Countries"])
     (color2, shape2, size2, second_line2) = get_color_and_shape(row["Partner2Node"], row["Countries"])
@@ -130,15 +139,16 @@
         , partner1_name = row["Partner1Name"]
         , partner2_name = row["Partner2Name"]
         , country = row["Countries"]
     )
 
 
 
-net.render_template(open_in_browser=True, 
-                    template_filename="tom-select.html", 
+net.render_tom_template(
+                    title="035319 2023-06-01 / 2023-12-31",
+                    open_in_browser=True,
                     enable_highlighting=True, 
                     edge_filtering=["country", "category"],
                     node_filtering=["partner_name"]
                     )
 
 #net.show("example2.html")
```

### Comparing `pyvisjs-1.0.0b1/folder_structure.txt` & `pyvisjs-1.0.0b2/folder_structure.txt`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b1/pyproject.toml` & `pyvisjs-1.0.0b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b1/pyvisjs/base_dictable.py` & `pyvisjs-1.0.0b2/pyvisjs/base_dictable.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b1/pyvisjs/edge.py` & `pyvisjs-1.0.0b2/pyvisjs/edge.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b1/pyvisjs/network.py` & `pyvisjs-1.0.0b2/pyvisjs/network.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .edge import Edge
 from .options import Options
 from jinja2 import Environment, PackageLoader, select_autoescape
 from typing import List, Dict
 
 class Network(BaseDictable):
     """
-    Network is a visualization to display networks and networks consisting of nodes and edges. 
+    Network is a visualization to display networks consisting of nodes and edges. 
     The visualization is easy to use and supports custom shapes, styles, colors, sizes, images, and more. 
     The network visualization works smooth on any modern browser for up to a few thousand nodes and edges. 
     Network uses HTML canvas for rendering.
     """
     def __init__(self, name="Network", nodes:List[Node]=None, edges:List[Edge]=None, options:Options=None):
         only_use_data_attr = lambda attr: attr == "_data"
         super().__init__(attr_filter_func=only_use_data_attr)
@@ -67,100 +67,145 @@
         """
         Creates a Node with node_id and adds it to the nodes list. 
         Wont add node if the nodes list alredy contains a node with the same node_id.
 
         Parameters
         ----------
         node_id: str, default undefined
-            The id of the node. The id is mandatory for nodes and they have to be unique. Will be used as a node reference in edges
+            The id of the node. The id is mandatory for nodes and they have to be unique. 
+            Will be used as a node reference in edges
 
         label: str, default undefined
-            Will be replaced with node_id if undefined) The label is the piece of text shown in or under the node, depending on the shape.
+            Will be replaced with `str(node_id)` if undefined. 
+            The label is the piece of text shown in or under the node, depending on the shape.
         
-        color: str, default undefined
-            Could be value like '#ffffff' or 'red'
+        color: str, default undefined, but if undefined, `'#97C2FC'` will be used by vis.js
+            Could be value like `'#ffffff'` or `'red'`
         
         **kwargs: dict, optional
             Any key=value agruments could also be specified to push them into the underlying HTML template
         """
         if not [node.id for node in self.nodes if node.id == str(node_id)]:
             self.nodes.append(Node(node_id, label, color, shape, size, cid, **kwargs))
 
     def add_edge(self, from_id:str, to_id:str, **kwargs):
         """Creates an Edge which connects two nodes using from_id and to_id and adds it to the edges list.
-        If you provide node ID which is not presented in the nodes list such a node will be automatically created and added to the nodes list.
+        If you provide node ID which is not presented in the nodes list 
+        such a node will be automatically created and added to the nodes list.
         
         Parameters
         ----------
         from_id: str, default undefined
-            Edges are between two nodes, one to and one from. This is where you define the from node. You have to supply the corresponding node ID.
+            Edges are between two nodes, one to and one from. This is where you define the from node. 
+            You have to supply the corresponding node ID.
         
         to_id: str, default undefined
-            Edges are between two nodes, one to and one from. This is where you define the to node. You have to supply the corresponding node ID.
+            Edges are between two nodes, one to and one from. This is where you define the to node. 
+            You have to supply the corresponding node ID.
 
         **kwargs: dist, Optional
             Any key=value agruments could also be specified to push them into the underlying HTML template
         """
         self.add_node(from_id)
         self.add_node(to_id)
 
         if not [edge.start for edge in self.edges if edge.start == str(from_id) and edge.end == str(to_id)]:
             self.edges.append(Edge(from_id, to_id, **kwargs))
 
     def to_dict(self):
         return super().to_dict()["_data"]
 
-    def show(self, file_name, enable_highlighting=False, edge_filtering=None):
-        self.render_template(open_in_browser=True, output_filename=file_name, enable_highlighting=enable_highlighting, edge_filtering=edge_filtering)
+    def show(self, file_name):
+        self.render_default_template(open_in_browser=True, output_filename=file_name)
 
-    def render_template(self, open_in_browser=False, save_to_output=False, output_filename="default.html", template_filename="basic.html", enable_highlighting=False, edge_filtering=None, node_filtering=None) -> str:
-        """This method uses jinja to inject prepared data to a html file from the templates folder (for more info about the injected data see Notes section below).
+    def _render(self, template_filename:str, open_in_browser=False, save_to_output=False, output_filename="default.html", pyvisjs_options:Dict=None):
+        network_dict = self.to_dict()
+
+        html_output = self.env \
+            .get_template(template_filename) \
+            .render(
+                width=network_dict["options"].get("width", "100%"),
+                height=network_dict["options"].get("height", "100%"),
+                data=network_dict,
+                pyvisjs=pyvisjs_options or {},
+            )
+
+        if save_to_output or open_in_browser:
+            file_path = save_file(output_filename, html_output)
+
+        if open_in_browser:
+            open_file(file_path)
+
+        return html_output
+    
+    def render_default_template(self, open_in_browser=False, save_to_output=False, output_filename="default.html"):
+        return self._render(
+            template_filename="basic.html",
+            open_in_browser=open_in_browser,
+            save_to_output=save_to_output,
+            output_filename=output_filename)
+    
+
+    def render_tom_template(self, title:str=None, open_in_browser=False, save_to_output=False, output_filename="default.html", 
+    enable_highlighting=False, edge_filtering=None, node_filtering=None) -> str:
+        """This method uses jinja to inject prepared data to `'templates\\tom-select.html'` \n
+        (for more info about the injected data see Notes section below).
         
         Parameters
         ----------
         open_in_browser: bool, default=False
             Resolved template will be saved as the `output_filename` and opened with `os.startfile`
 
         save_to_output: bool, default=False
             Resolved template will be just saved (not opened) as the `output_filename`
 
-        output_filename: str, default="default.html"
+        output_filename: str, default=".\\default.html"
             Can be just a file name or have relative or absolute path
 
-        template_filename: str, default="basic.html"
-            Name of the jinja template file in the templates dir
-
         enable_highlighting: bool, default=False
-            Enables highlighting of the clicked node and it's neighbours which means shadowing all others. 
+            - `true` - turns highlighting mode on, which means filtering in the tom-select control will highlight a part of the network - not hide it
+            - `false` - turns highlighting mode off, which means filtering in the tom-select control will hide a part of the network - not highlight it
             This setting is not a standard vis.js option and injects to the template as the `enable_highlighting` key of the `pyvisjs` dict
         
         edge_filtering: str or list, default=None
             Enables edges filtering using predefined or dynamic edge attributes which means hiding all edges which do not satisfy filtering condition
-            So for example you can 
+            So for example you can:
             add a dynamic attribute "size" with 3 possible values ['S', 'M', 'L'] to the edges and 
-            pass `edge_filtering="size"` to the `render_template` method
+            pass `edge_filtering="size"` to the `render_tom_template` method
+            expecting resolved template to have `<select>` element with S/M/L options lookup
+            which will filter all nodes connected with edges having selected option
+            see example on `gitlab.com/22kittens/pyvisjs/examples/bluor.py`
+
+        node_filtering: str or list, default=None
+            Enables nodes filtering using predefined or dynamic node attributes which means hiding all nodes which do not satisfy filtering condition
+            So for example you can:
+            add a dynamic attribute "size" with 3 possible values ['S', 'M', 'L'] to the nodes and 
+            pass `node_filtering="size"` to the `render_tom_template` method
             expecting resolved template to have `<select>` element with S/M/L options lookup
-            which will filter all nodes connected with edges having selected option 
+            which will filter all nodes having selected option
+            see example on `gitlab.com/22kittens/pyvisjs/examples/bluor.py`
 
         Notes
         -----
         The data injected will be:
 
         >>> .render(
         >>>     width=network_dict["options"].get("width", "100%"),
         >>>     height=network_dict["options"].get("height", "100%"),
         >>>     data=network_dict,
         >>>     pyvisjs={
         >>>         "enable_highlighting": enable_highlighting,
         >>>         "edge_filtering_lookup": edge_filtering_lookup,
+        >>>         "node_filtering_lookup": node_filtering_lookup,
         >>>     },
         >>> )
 
+        you can find more details about `edge_filtering_lookup` and `node_filtering_lookup` structure here `tests\\test_network.py\\test_network_render_template_edge_filtering_list`
         """
-        network_dict = self.to_dict()
+
         edge_filtering_lookup: Dict = None
         node_filtering_lookup: Dict = None
 
         # edges
         if not edge_filtering is None:
             if not isinstance(edge_filtering, list):
                 edge_filtering = [str(edge_filtering)]
@@ -179,28 +224,21 @@
 
             node_filtering_lookup = {}
             for field_name in node_filtering:
                 unique_values = list(set([str(getattr(node, field_name)) for node in self.nodes if hasattr(node, field_name)]))
                 unique_values.sort()
                 node_filtering_lookup[field_name] = unique_values             
         
-        html_output = self.env \
-            .get_template(template_filename) \
-            .render(
-                width=network_dict["options"].get("width", "100%"),
-                height=network_dict["options"].get("height", "100%"),
-                data=network_dict,
-                pyvisjs={
+        pyvisjs_options = {
                     "enable_highlighting": enable_highlighting,
                     "edge_filtering_lookup": edge_filtering_lookup,
                     "node_filtering_lookup": node_filtering_lookup,
-                },
-            )
-
-        if save_to_output or open_in_browser:
-            file_path = save_file(output_filename, html_output)
-
-        if open_in_browser:
-            open_file(file_path)
-
-        return html_output
+                    "title": title,
+                };
+         
+        return self._render(
+            template_filename="tom-select.html",
+            open_in_browser=open_in_browser,
+            save_to_output=save_to_output,
+            output_filename=output_filename,
+            pyvisjs_options=pyvisjs_options)
```

### Comparing `pyvisjs-1.0.0b1/pyvisjs/node.py` & `pyvisjs-1.0.0b2/pyvisjs/node.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b1/pyvisjs/options.py` & `pyvisjs-1.0.0b2/pyvisjs/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,19 @@
         self._update_dict_with_locals(self.interaction, locals())
         return self
 
     class Nodes(BaseDictable):
         def __init__(self):
             super().__init__()
             self.scaling = {}
+            self.font = {}
+
+        def set_font(self, face:str=None) -> Self:
+            self._update_dict_with_locals(self.font, locals())
+            return self
 
         def set_scaling(self, min:int=None, max:int=None, label:bool=None) -> Self:
             """
             Parameters
             ----------
             min : int, default=10
                 If nodes have a value, their sizes are determined by the value, the scaling function and the min max values. The min value is the minimum allowed value.
@@ -101,17 +106,22 @@
     class Edges(BaseDictable):
         def __init__(self):
             super().__init__()
 
             self.arrows:str = None
             self.arrowStrikethrough:bool = None
 
+            self.font = {}
             self.color = {}
             self.smooth = {}
 
+        def set_font(self, face:str=None) -> Self:
+            self._update_dict_with_locals(self.font, locals())
+            return self
+
         def set(self, arrows:str=None, arrowStrikethrough:bool=None) -> Self:
             """
             Parameters
             ----------
             arrows : str, default None
                 Can be any combination with any separating symbol of `'to, from, middle'`
```

### Comparing `pyvisjs-1.0.0b1/pyvisjs/templates/base.html` & `pyvisjs-1.0.0b2/pyvisjs/templates/base.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 <html>
   <head>
     {% block head -%}
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <title>{% block title %}{% endblock %}</title>
     {% block head_scripts -%}
+    <link href='https://fonts.googleapis.com/css?family=JetBrains Mono' rel='stylesheet'>
     <script type="text/javascript" src="https://unpkg.com/vis-network/standalone/umd/vis-network.min.js"></script>
     {%- endblock %}
     <style type="text/css">
       {% block head_style -%}
+      body {
+        font-family: 'JetBrains Mono';font-size: 22px;
+      }
       #visjsnet {
           width: {{width}};
           height: {{height}};
           border: 1px solid lightgray;
       }
       {%- endblock %}
     </style>
   {%- endblock %}
   </head>
   <body>
     {% block content -%}{%- endblock %}
     <script type="text/javascript">
     {% block javascript %}
-{% include "functions.js" %}
-    {% endblock -%}
+    {% include "create_network.js" %}
+    {% endblock %}
     </script>
   </body>
 </html>
```

### Comparing `pyvisjs-1.0.0b1/pyvisjs/templates/bs-container.html` & `pyvisjs-1.0.0b2/pyvisjs/templates/bs-container.html`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b1/pyvisjs/templates/functions.js` & `pyvisjs-1.0.0b2/pyvisjs/templates/functions.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,31 +1,7 @@
-const data = create_network();
-data.network.has_hidden_nodes = false;
-//if (data.pyvisjs.enable_highlighting === true) data.network.on("click", hide_not_selected_nodes);
-
-const eventHandler = function(name) {
-    return function() {
-        const list_of_selected_values = arguments[0]
-        dict = convert_field_value_list_to_dict(list_of_selected_values)
-        hide_nodes_by_edge_attribute_values_intersect(dict)
-    };
-};
-
-new TomSelect("#select-all-fields", {
-    maxItems: 10,
-    onChange: eventHandler("onChange"),
-    //create: true,
-    //onItemAdd:function(){
-    //    this.setTextboxValue('');
-    //    this.refreshOptions();
-    //},
-    plugins: ['remove_button'],
-});
-
-
 // converts ["edge,country,LV","edge,country,GB"]
 // to
 // {country: {list: ["LV", "GB"], type="edge"}}
 function convert_field_value_list_to_dict(list) {
     dict = {}
     for (id in list) {
         const field_value_triplet = list[id].split(",")
@@ -38,63 +14,14 @@
             "list": [value],
             "type": type
         }
     }
     return dict
 }
 
-// all jinja injections should happen here because it allows to mock this function and test all the rest
-function create_network() {
-
-    // create an array with nodes
-    const ds_nodes = new vis.DataSet({
-        {
-            data["nodes"] | tojson
-        }
-    });
-
-    // create an array with edges
-    const ds_edges = new vis.DataSet({
-        {
-            data["edges"] | tojson
-        }
-    });
-
-    // create a network
-    const container = document.getElementById('visjsnet');
-
-    // provide the data in the vis format
-    const data = {
-        nodes: ds_nodes,
-        edges: ds_edges
-    };
-    const options = {
-        {
-            data["options"] | tojson
-        }
-    };
-    const pyvisjs = {
-        {
-            pyvisjs | tojson
-        }
-    };
-
-    return {
-        network: new vis.Network(container, data, options),
-        nodes: ds_nodes.get({
-            returnType: "Object"
-        }),
-        edges: ds_edges.get({
-            returnType: "Object"
-        }),
-        ds_nodes: ds_nodes,
-        pyvisjs: pyvisjs,
-    }
-}
-
 function get_nodes_by_edge_attribute_value(field, value) {
 
     const result = [];
 
     for (const key in data.edges) {
         const edge = data.edges[key];
 
@@ -269,24 +196,24 @@
         if (node.hasOwnProperty("_hidden") === false) node._hidden = false;
 
         // nodes to hide
         if (selectedNodes.includes(node_id) === false) {
             // not already hidden
             if (node._hidden === false) {
                 node._hidden = true;
-                node.hidden = true;
+                if (data.pyvisjs.enable_highlighting === false) node.hidden = true;
                 node._color = node.color;
                 node.color = "rgba(200,200,200,0.5)";
                 changed_nodes.push(node)
             }
         }
         // nodes to unhide (only if already hidden)
         else if (node._hidden === true) {
             node._hidden = false;
-            node.hidden = false;
+            if (data.pyvisjs.enable_highlighting === false) node.hidden = false;
             node.color = node._color ? node._color : "#97C2FC";
             node._color = undefined;
             changed_nodes.push(node)
         }
     }
 
     return changed_nodes
```

### Comparing `pyvisjs-1.0.0b1/pyvisjs/templates/select-edge-filter.html` & `pyvisjs-1.0.0b2/pyvisjs/templates/select-edge-filter.html`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b1/pyvisjs/utils.py` & `pyvisjs-1.0.0b2/pyvisjs/utils.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b1/pyvisjs.egg-info/PKG-INFO` & `pyvisjs-1.0.0b2/pyvisjs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisjs
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: A Python wrapper for vis.js Network
 Author-email: Andrey Morozov <andrey@morozov.lv>
 License: MIT License
         
         Copyright (c) 2024 Andrey Morozov (andrey@morozov.lv)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,16 +42,16 @@
 # pyvisjs: Python Wrapper for vis.js Network
 
 pyvisjs is a Python package designed to provide seamless interaction with [vis.js](https://visjs.org) network visualizations, allowing users to manipulate and visualize network data using Python.
 
 ## Workflow
 
 1. Create a network using python
-2. Apply standatd vis.js options such as colors, shapes or physics
-3. Apply pyvisjs specific options such as filtering or highlighting
+2. Apply standard vis.js options such as colors, shapes or physics
+3. Apply pyvisjs specific options such as node/edge filtering or highlighting
 4. Show or generate html file
 5. Enjoy network interactions in your browser
 
 ## Installation
 
 You can install PyVisjs via pip:
```

### Comparing `pyvisjs-1.0.0b1/pyvisjs.egg-info/SOURCES.txt` & `pyvisjs-1.0.0b2/pyvisjs.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,18 @@
 pyvisjs.egg-info/SOURCES.txt
 pyvisjs.egg-info/dependency_links.txt
 pyvisjs.egg-info/requires.txt
 pyvisjs.egg-info/top_level.txt
 pyvisjs/templates/base.html
 pyvisjs/templates/basic.html
 pyvisjs/templates/bs-container.html
+pyvisjs/templates/create_network.js
+pyvisjs/templates/draw_title.js
 pyvisjs/templates/functions.js
+pyvisjs/templates/init_tomSelect.js
 pyvisjs/templates/select-edge-filter.html
 pyvisjs/templates/tom-select.html
 tests/__init__.py
 tests/test_base_dictable.py
 tests/test_edge.py
 tests/test_network.py
 tests/test_node.py
```

### Comparing `pyvisjs-1.0.0b1/tests/test_base_dictable.py` & `pyvisjs-1.0.0b2/tests/test_base_dictable.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b1/tests/test_edge.py` & `pyvisjs-1.0.0b2/tests/test_edge.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b1/tests/test_network.py` & `pyvisjs-1.0.0b2/tests/test_network.py`

 * *Files 10% similar despite different names*

```diff
@@ -154,240 +154,241 @@
     n.add_edge(2, 3) # one node missing
     n.add_edge(2, 3) # duplicate edge
     
     # assert
     assert n.to_dict() == NETWORK_DICT
 
 @patch('pyvisjs.network.Environment')
-def test_network_render_template_passing_render_default_params(mock_Environment):
+def test_network_render_tom_template_passing_render_default_params(mock_Environment):
     # init
     WIDTH="100%"
     HEIGHT="100%"
     DATA={"nodes": [], "edges": [], "options": {}}
     PYVISJS={
         "enable_highlighting": False,
         "edge_filtering_lookup": None,
         "node_filtering_lookup": None,
+        "title": None,
     }
     
     # mock
     mock_render = mock_Environment.return_value.get_template.return_value.render
 
     # call
     network = Network("Test Network")
-    html_output = network.render_template() # <--------------------
+    html_output = network.render_tom_template() # <--------------------
 
     # assert
     mock_render.assert_called_once_with(width=WIDTH, height=HEIGHT, data=DATA, pyvisjs=PYVISJS)
 
 @patch('pyvisjs.network.Environment')
-def test_network_render_template_passing_render_params(mock_Environment):
+def test_network_render_tom_template_passing_render_params(mock_Environment):
     # init
     WIDTH="100%"
     HEIGHT="100%"
     DATA={"nodes": [], "edges": [], "options": {}}
-    TEMPLATE_FILENAME="another_template.html"
+    TEMPLATE_FILENAME="tom-select.html"
     ENABLE_HIGHLIGHTING=True
     EDGE_FILTERING="edge_field" # str(!) not list
     NODE_FILTERING=["field1", "field2"] # list
     PYVISJS={
         "enable_highlighting": ENABLE_HIGHLIGHTING,
         "edge_filtering_lookup": {"edge_field": []},
         "node_filtering_lookup": {"field1": [], "field2": []},
+        "title": None,
     }
     
     # mock
     mock_get_template = mock_Environment.return_value.get_template
     mock_render = mock_get_template.return_value.render
 
     # call
     network = Network("Test Network")
-    html_output = network.render_template( # <--------------------
-        template_filename=TEMPLATE_FILENAME, 
+    html_output = network.render_tom_template( # <--------------------
         enable_highlighting=ENABLE_HIGHLIGHTING, 
         edge_filtering=EDGE_FILTERING, 
         node_filtering=NODE_FILTERING)
 
     # assert
     mock_get_template.assert_called_once_with(TEMPLATE_FILENAME)
     mock_render.assert_called_once_with(width=WIDTH, height=HEIGHT, data=DATA, pyvisjs=PYVISJS)
 
 @patch('pyvisjs.network.Environment')
-def test_network_render_template_edge_filtering_list(mock_Environment):
+def test_network_render_tom_template_edge_filtering_list(mock_Environment):
     # init
     WIDTH="100%"
     HEIGHT="100%"
     DATA={
         'nodes': [
             {'id': '1', 'label': '1', 'shape': 'dot'}, 
             {'id': '2', 'label': '2', 'shape': 'dot'}, 
             {'id': '3', 'label': '3', 'shape': 'dot'}], 
         'edges': [
             {'to': '2', 'field1': 'AM', 'from': '1'}, 
             {'to': '3', 'field1': 'AM', 'from': '1'}, 
             {'to': '3', 'field1': 'JL', 'from': '2'}], 
         'options': {}
     }
-    TEMPLATE_FILENAME="another_template.html"
+    TEMPLATE_FILENAME="tom-select.html"
     ENABLE_HIGHLIGHTING=True
     EDGE_FILTERING=["field1", "field2"]
     NODE_FILTERING=["label", "shape"]
     PYVISJS={
         "enable_highlighting": ENABLE_HIGHLIGHTING,
         "edge_filtering_lookup": {"field1": ["AM", "JL"], "field2": []},
         "node_filtering_lookup": {"label": ["1", "2", "3"], "shape": ["dot"]},
+        "title": None,
     }
     
     # mock
     mock_get_template = mock_Environment.return_value.get_template
     mock_render = mock_get_template.return_value.render
 
     # call
     net = Network("Network1")
     net.add_edge(1, 2, field1="AM")
     net.add_edge(1, 3, field1="AM")
     net.add_edge(2, 3, field1="JL")
-    html_output = net.render_template( # <--------------------
-        template_filename=TEMPLATE_FILENAME, 
+    html_output = net.render_tom_template( # <--------------------
         enable_highlighting=ENABLE_HIGHLIGHTING, 
         edge_filtering=EDGE_FILTERING,
         node_filtering=NODE_FILTERING) 
 
     # assert
     mock_get_template.assert_called_once_with(TEMPLATE_FILENAME)
     mock_render.assert_called_once_with(width=WIDTH, height=HEIGHT, data=DATA, pyvisjs=PYVISJS)
 
 @patch('pyvisjs.network.Environment')
-def test_network_render_template_edge_filtering_int(mock_Environment):
+def test_network_render_tom_template_edge_filtering_int(mock_Environment):
     # init
     WIDTH="100%"
     HEIGHT="100%"
     DATA={"nodes": [], "edges": [], "options": {}}
-    TEMPLATE_FILENAME="another_template.html"
+    TEMPLATE_FILENAME="tom-select.html"
     ENABLE_HIGHLIGHTING=True
     EDGE_FILTERING=34
     NODE_FILTERING=22
     PYVISJS={
         "enable_highlighting": ENABLE_HIGHLIGHTING,
         "edge_filtering_lookup": {"34": []},
         "node_filtering_lookup": {"22": []},
+        "title": None,
     }
     
     # mock
     mock_get_template = mock_Environment.return_value.get_template
     mock_render = mock_get_template.return_value.render
 
     # call
     net = Network("Network1")
-    html_output = net.render_template(# <--------------------
-        template_filename=TEMPLATE_FILENAME, 
+    html_output = net.render_tom_template(# <--------------------
         enable_highlighting=ENABLE_HIGHLIGHTING, 
         edge_filtering=EDGE_FILTERING,
         node_filtering=NODE_FILTERING) 
 
     # assert
     mock_get_template.assert_called_once_with(TEMPLATE_FILENAME)
     mock_render.assert_called_once_with(width=WIDTH, height=HEIGHT, data=DATA, pyvisjs=PYVISJS)
 
 @patch('pyvisjs.network.open_file')
 @patch('pyvisjs.network.save_file')
 @patch('pyvisjs.network.Environment')
-def test_network_render_template_with_all_default_values(mock_Environment, mock_save_file, mock_open_file):
+def test_network_render_default_template_with_all_default_values(mock_Environment, mock_save_file, mock_open_file):
     # init
     RENDER_RESULT = "<html>template</html>"
     DEFAULT_TEMPLATE_FILENAME = "basic.html"
     
     # mock
     mock_get_template = mock_Environment.return_value.get_template
     mock_render = mock_get_template.return_value.render
     mock_render.return_value = RENDER_RESULT
 
     # call
     network = Network("Test Network")
-    html_output = network.render_template() # <--------------------
+    html_output = network.render_default_template() # <--------------------
 
     # assert
     mock_get_template.assert_called_once_with(DEFAULT_TEMPLATE_FILENAME)
     mock_save_file.assert_not_called()
     mock_open_file.assert_not_called()
     assert html_output == RENDER_RESULT
 
 
 @patch('pyvisjs.network.open_file')
 @patch('pyvisjs.network.save_file')
 @patch('pyvisjs.network.Environment')
 def test_network_render_template_with_open_in_browser(mock_Environment, mock_save_file, mock_open_file):
     # init
     RENDER_RESULT = "<html>template</html>"
-    DEFAULT_TEMPLATE_FILENAME = "basic.html"
+    TEMPLATE_FILENAME = "some-template-name.html"
     DEFAULT_OUTPUT_FILENAME = "default.html"
     
     # mock
     mock_get_template = mock_Environment.return_value.get_template
     mock_render = mock_get_template.return_value.render
     mock_render.return_value = RENDER_RESULT
     mock_save_file.return_value = DEFAULT_OUTPUT_FILENAME
 
     # call
     network = Network("Test Network")
-    html_output = network.render_template(open_in_browser=True) # <--------------------
+    html_output = network._render(TEMPLATE_FILENAME, open_in_browser=True) # <--------------------
 
     #assert
-    mock_get_template.assert_called_once_with(DEFAULT_TEMPLATE_FILENAME)
+    mock_get_template.assert_called_once_with(TEMPLATE_FILENAME)
     mock_save_file.assert_called_once_with(DEFAULT_OUTPUT_FILENAME, RENDER_RESULT)
     mock_open_file.assert_called_once_with(DEFAULT_OUTPUT_FILENAME)
     assert html_output == RENDER_RESULT
 
 
 @patch('pyvisjs.network.open_file')
 @patch('pyvisjs.network.save_file')
 @patch('pyvisjs.network.Environment')
 def test_network_render_template_with_save_to_output(mock_Environment, mock_save_file, mock_open_file):
     # init
     RENDER_RESULT = "<html>template</html>"
-    DEFAULT_TEMPLATE_FILENAME = "basic.html"
+    TEMPLATE_FILENAME = "template-1.html"
     DEFAULT_OUTPUT_FILENAME = "default.html"
     
     # mock
     mock_get_template = mock_Environment.return_value.get_template
     mock_render = mock_get_template.return_value.render
     mock_render.return_value = RENDER_RESULT
 
     # call
     network = Network("Test Network")
-    html_output = network.render_template(save_to_output=True) # <--------------------
+    html_output = network._render(TEMPLATE_FILENAME, save_to_output=True) # <--------------------
 
     #assert
-    mock_get_template.assert_called_once_with(DEFAULT_TEMPLATE_FILENAME)
+    mock_get_template.assert_called_once_with(TEMPLATE_FILENAME)
     mock_save_file.assert_called_once_with(DEFAULT_OUTPUT_FILENAME, RENDER_RESULT)
     mock_open_file.assert_not_called()
     assert html_output == RENDER_RESULT
 
 
 @patch('pyvisjs.network.open_file')
 @patch('pyvisjs.network.save_file')
 @patch('pyvisjs.network.Environment')
 def test_network_render_template_with_open_and_save_no_defaults(mock_Environment, mock_save_file, mock_open_file):
     # init
     RENDER_RESULT = "<html>template</html>"
-    CUSTOM_TEMPLATE_FILENAME = "custom_template.html"
+    TEMPLATE_FILENAME = "custom_template.html"
     CUSTOM_OUTPUT_FILENAME = "custom_output.html"
     
     # mock
     mock_get_template = mock_Environment.return_value.get_template
     mock_render = mock_get_template.return_value.render
     mock_render.return_value = RENDER_RESULT
     mock_save_file.return_value = CUSTOM_OUTPUT_FILENAME
 
     # call
     network = Network("Test Network")
-    html_output = network.render_template( # <--------------------
+    html_output = network._render( # <--------------------
+        TEMPLATE_FILENAME,
         open_in_browser=True, 
         save_to_output=True, 
-        output_filename=CUSTOM_OUTPUT_FILENAME, 
-        template_filename=CUSTOM_TEMPLATE_FILENAME)
+        output_filename=CUSTOM_OUTPUT_FILENAME)
 
     #assert
-    mock_get_template.assert_called_once_with(CUSTOM_TEMPLATE_FILENAME)
+    mock_get_template.assert_called_once_with(TEMPLATE_FILENAME)
     mock_save_file.assert_called_once_with(CUSTOM_OUTPUT_FILENAME, RENDER_RESULT)
     mock_open_file.assert_called_once_with(CUSTOM_OUTPUT_FILENAME)
     assert html_output == RENDER_RESULT
```

### Comparing `pyvisjs-1.0.0b1/tests/test_node.py` & `pyvisjs-1.0.0b2/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b1/tests/test_options.py` & `pyvisjs-1.0.0b2/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b1/tests/test_utils.py` & `pyvisjs-1.0.0b2/tests/test_utils.py`

 * *Files identical despite different names*

