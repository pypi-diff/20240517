# Comparing `tmp/turbocase-1.2.tar.gz` & `tmp/turbocase-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbocase-1.2.tar", last modified: Wed May 15 22:54:30 2024, max compression
+gzip compressed data, was "turbocase-1.3.tar", last modified: Fri May 17 13:45:46 2024, max compression
```

## Comparing `turbocase-1.2.tar` & `turbocase-1.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 22:54:30.108217 turbocase-1.2/
--rw-r--r--   0 root         (0) root         (0)     1069 2024-05-15 14:32:06.000000 turbocase-1.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      269 2024-05-15 22:54:30.108217 turbocase-1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2443 2024-05-15 14:44:48.000000 turbocase-1.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 22:54:30.108217 turbocase-1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      438 2024-05-15 22:54:18.000000 turbocase-1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 22:54:30.108217 turbocase-1.2/turbocase/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 00:06:28.000000 turbocase-1.2/turbocase/__init__.py
--rw-r--r--   0 root         (0) root         (0)      885 2024-05-15 14:42:59.000000 turbocase-1.2/turbocase/__main__.py
--rw-r--r--   0 root         (0) root         (0)     1356 2024-05-15 14:29:21.000000 turbocase-1.2/turbocase/cases.py
--rw-r--r--   0 root         (0) root         (0)     7157 2024-05-15 22:51:03.000000 turbocase-1.2/turbocase/kicad.py
--rw-r--r--   0 root         (0) root         (0)     2855 2024-05-15 14:08:06.000000 turbocase-1.2/turbocase/scad.py
--rw-r--r--   0 root         (0) root         (0)     1279 2024-05-15 18:26:04.000000 turbocase-1.2/turbocase/vector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 22:54:30.108217 turbocase-1.2/turbocase.egg-info/
--rw-r--r--   0 root         (0) root         (0)      269 2024-05-15 22:54:30.000000 turbocase-1.2/turbocase.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      350 2024-05-15 22:54:30.000000 turbocase-1.2/turbocase.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 22:54:30.000000 turbocase-1.2/turbocase.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2024-05-15 22:54:30.000000 turbocase-1.2/turbocase.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-15 22:54:30.000000 turbocase-1.2/turbocase.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-15 22:54:30.000000 turbocase-1.2/turbocase.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 13:45:46.936815 turbocase-1.3/
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-05-15 14:32:06.000000 turbocase-1.3/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      269 2024-05-17 13:45:46.936815 turbocase-1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2443 2024-05-15 14:44:48.000000 turbocase-1.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 13:45:46.936815 turbocase-1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      438 2024-05-17 13:45:29.000000 turbocase-1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 13:45:46.933482 turbocase-1.3/turbocase/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 00:06:28.000000 turbocase-1.3/turbocase/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      885 2024-05-15 14:42:59.000000 turbocase-1.3/turbocase/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2024-05-17 12:51:54.000000 turbocase-1.3/turbocase/cases.py
+-rw-r--r--   0 root         (0) root         (0)     8225 2024-05-17 13:31:10.000000 turbocase-1.3/turbocase/kicad.py
+-rw-r--r--   0 root         (0) root         (0)      845 2024-05-17 13:19:26.000000 turbocase-1.3/turbocase/parts.py
+-rw-r--r--   0 root         (0) root         (0)     3087 2024-05-17 12:58:48.000000 turbocase-1.3/turbocase/scad.py
+-rw-r--r--   0 root         (0) root         (0)     1279 2024-05-15 18:26:04.000000 turbocase-1.3/turbocase/vector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 13:45:46.936815 turbocase-1.3/turbocase.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      269 2024-05-17 13:45:46.000000 turbocase-1.3/turbocase.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      369 2024-05-17 13:45:46.000000 turbocase-1.3/turbocase.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 13:45:46.000000 turbocase-1.3/turbocase.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2024-05-17 13:45:46.000000 turbocase-1.3/turbocase.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-17 13:45:46.000000 turbocase-1.3/turbocase.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-17 13:45:46.000000 turbocase-1.3/turbocase.egg-info/top_level.txt
```

### Comparing `turbocase-1.2/LICENSE.txt` & `turbocase-1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `turbocase-1.2/README.md` & `turbocase-1.3/README.md`

 * *Files identical despite different names*

### Comparing `turbocase-1.2/turbocase/__main__.py` & `turbocase-1.3/turbocase/__main__.py`

 * *Files identical despite different names*

### Comparing `turbocase-1.2/turbocase/cases.py` & `turbocase-1.3/turbocase/cases.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,27 +16,37 @@
     def height(self):
         return self.bounds[3] - self.bounds[1]
 
     def depth(self):
         return self.prop_height
 
 
+class Part:
+    def __init__(self):
+        self.script = None
+        self.position = None
+        self.rotation = None
+
+
 class Case:
     connectors: list[Connector]
 
     def __init__(self):
         self.inner_path = []
         self.pcb_mount = []
         self.pcb_thickness = 1.6
         self.floor_thickness = 1.2
         self.wall_thickness = 1.2
 
         self.max_connector_height = 0
         self.connectors = []
 
+        self.modules = []
+        self.parts = []
+
     def get_inner_bounds(self):
         min_x = self.inner_path[0][0]
         max_x = 0
         min_y = self.inner_path[0][1]
         max_y = 0
         for point in self.inner_path:
             min_x = min(min_x, point[0])
```

### Comparing `turbocase-1.2/turbocase/kicad.py` & `turbocase-1.3/turbocase/kicad.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import os
+import sys
 
 import sexpdata
 
-from turbocase.cases import Case, Connector
+from turbocase.cases import Case, Connector, Part
 from turbocase.vector import Vector
+import turbocase.parts
 
 
 class Sym:
     def __init__(self, symbol):
         self.raw = symbol
         self.name = symbol[0].value()
         self.attr = {}
         self.values = []
         self.property = {}
 
-        arrays = ['pad', 'property', 'fp_text', 'fp_line', 'fp_rect', 'xy']
+        arrays = ['pad', 'property', 'fp_text', 'fp_line', 'fp_rect', 'fp_circle', 'xy']
 
         for part in symbol:
             if isinstance(part, sexpdata.Symbol):
                 continue
             if isinstance(part, list):
                 key = part[0].value()
 
@@ -100,26 +102,36 @@
         min_x = min(min_x, point[0])
         max_x = max(max_x, point[0])
         min_y = min(min_y, point[1])
         max_y = max(max_y, point[1])
     return min_x, min_y, max_x, max_y
 
 
+def unindent(raw):
+    raw = raw.lstrip('\n')
+    indent = len(raw) - len(raw.lstrip())
+    result = []
+    for line in raw.splitlines():
+        result.append(line[indent:])
+    return '\n'.join(result)
+
+
 def load_pcb(pcb_file, outline_layer=None):
     if outline_layer is None:
         outline_layer = 'User.6'
 
     with open(pcb_file) as handle:
         pcb = sexpdata.load(handle)
 
     result = Case()
 
     outline_shapes = []
     mountingholes = []
     connectors = []
+    parts = []
 
     for symbol in pcb:
         if not isinstance(symbol, list):
             continue
         if isinstance(symbol[0], sexpdata.Symbol):
             name = symbol[0].value()
 
@@ -133,19 +145,21 @@
                         if sub[0].value() == 'layer' and sub[1] == outline_layer:
                             outline_shapes.append(Sym(symbol))
 
             if name == 'footprint':
                 footprint = Sym(symbol)
 
                 if 'MountingHole' in footprint[0]:
-                    mountingholes.append(Sym(symbol))
-
-                for prop in footprint['property']:
-                    if len(prop) == 2 and prop[0] == 'Height':
-                        connectors.append(footprint)
+                    mountingholes.append(footprint)
+                elif 'TurboCase' in footprint[0]:
+                    parts.append(footprint)
+                else:
+                    for prop in footprint['property']:
+                        if len(prop) == 2 and prop[0] == 'Height':
+                            connectors.append(footprint)
 
     outline = sort_outline(outline_shapes)
 
     path = []
     if outline[0].name == 'gr_poly':
         poly = outline[0]['pts']['xy']
         for xy in poly:
@@ -205,19 +219,25 @@
 
     result.inner_path = path
 
     for hole in mountingholes:
         center = hole['at'][:]
 
         drill = 0
-        space = 0
         for pad in hole['pad']:
             if pad['drill'][0] > drill:
                 drill = pad['drill'][0]
-                space = pad['size'][0]
+
+        space = drill + 2
+        for circle in hole['fp_circle']:
+            if circle['layer'][0] != 'F.CrtYd':
+                continue
+            diam = max(circle['end'][0], circle['end'][1]) * 2
+            if diam > space:
+                space = diam
 
         result.pcb_mount.append((center, drill, space, hole.property['Reference']))
 
     max_height = 0
     for item in connectors:
         ref = item.property['Reference']
         footprint = item.property['Footprint']
@@ -238,8 +258,26 @@
         c.footprint = footprint
         c.description = desc
         c.bounds = shape_bounds(shapes)
         c.position = item['at'][:]
         result.connectors.append(c)
     result.max_connector_height = max_height
 
+    modules = set()
+
+    for part in parts:
+        part_id = part[0].split(':')[1]
+        if not hasattr(turbocase.parts, part_id):
+            sys.stderr.write(f"Unknown part: {part.name}\n")
+            continue
+
+        func = getattr(turbocase.parts, part_id)
+        modules.add(unindent(func.__doc__))
+
+        p = Part()
+        p.script = func()
+        p.position = part.attr['at'][:]
+
+        result.parts.append(p)
+    result.modules = list(modules)
+
     return result
```

### Comparing `turbocase-1.2/turbocase/scad.py` & `turbocase-1.3/turbocase/scad.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,17 @@
 def generate(case):
     """
     :type case: Case
     """
 
     result = _template + "\n"
 
+    for m in case.modules:
+        result += m + "\n"
+
     center = case.get_center()
     result += f'translate([-{center[0]}, -{center[1]}, 0]) ' + '{\n'
 
     result += f'    standoff_height = 5;\n'
     result += f'    floor_height = {case.floor_thickness};\n'
     result += f'    pcb_thickness = {case.pcb_thickness};\n'
     result += f'    inner_height = standoff_height + pcb_thickness + {case.max_connector_height};\n'
@@ -82,9 +85,13 @@
 
     for mount in case.pcb_mount:
         result += f'    // {mount[3]}\n'
         result += f'    translate([{mount[0][0]}, {mount[0][1]}, {case.floor_thickness}])\n'
         # This currently creates correct holes for the M3 threaded metal inserts I have. Not generic
         result += f'    mount({mount[1] + 0.2}, {mount[2]}, 5);\n\n'
 
+    for part in case.parts:
+        result += f'    translate([{part.position[0]}, {part.position[1]}, {case.floor_thickness}])\n'
+        result += f'        {part.script}\n'
+
     result += '}\n'
     return result
```

### Comparing `turbocase-1.2/turbocase/vector.py` & `turbocase-1.3/turbocase/vector.py`

 * *Files identical despite different names*

