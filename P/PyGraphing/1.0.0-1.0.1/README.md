# Comparing `tmp/PyGraphing-1.0.0.tar.gz` & `tmp/PyGraphing-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGraphing-1.0.0.tar", last modified: Fri Dec 15 16:58:20 2023, max compression
+gzip compressed data, was "PyGraphing-1.0.1.tar", last modified: Mon Mar  4 20:58:14 2024, max compression
```

## Comparing `PyGraphing-1.0.0.tar` & `PyGraphing-1.0.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-12-15 16:58:20.301406 PyGraphing-1.0.0/
--rw-rw-rw-   0        0        0    35823 2022-09-12 17:26:44.000000 PyGraphing-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    41660 2023-12-15 16:58:20.300408 PyGraphing-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      462 2023-12-15 16:45:26.000000 PyGraphing-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-12-15 16:58:20.301406 PyGraphing-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-12-15 16:58:20.260406 PyGraphing-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-12-15 16:58:20.273406 PyGraphing-1.0.0/src/PyGraphing/
--rw-rw-rw-   0        0        0      132 2022-09-26 13:37:48.000000 PyGraphing-1.0.0/src/PyGraphing/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-15 16:58:20.288408 PyGraphing-1.0.0/src/PyGraphing/accessories/
--rw-rw-rw-   0        0        0       32 2023-12-02 16:55:38.000000 PyGraphing-1.0.0/src/PyGraphing/accessories/__init__.py
--rw-rw-rw-   0        0        0     3849 2023-12-02 16:55:38.000000 PyGraphing-1.0.0/src/PyGraphing/accessories/bezier.py
-drwxrwxrwx   0        0        0        0 2023-12-15 16:58:20.291408 PyGraphing-1.0.0/src/PyGraphing/data_sturctures/
--rw-rw-rw-   0        0        0     1992 2023-12-12 14:16:15.000000 PyGraphing-1.0.0/src/PyGraphing/data_sturctures/PriorityQueue.py
--rw-rw-rw-   0        0        0     1365 2023-12-11 19:45:24.000000 PyGraphing-1.0.0/src/PyGraphing/data_sturctures/UnionFind.py
--rw-rw-rw-   0        0        0       89 2023-12-15 16:49:45.000000 PyGraphing-1.0.0/src/PyGraphing/data_sturctures/__init__.py
--rw-rw-rw-   0        0        0     2913 2023-12-15 16:57:44.000000 PyGraphing-1.0.0/src/PyGraphing/data_sturctures/tree.py
--rw-rw-rw-   0        0        0     5507 2023-12-15 16:52:15.000000 PyGraphing-1.0.0/src/PyGraphing/frame.py
--rw-rw-rw-   0        0        0     3699 2023-12-15 16:57:44.000000 PyGraphing-1.0.0/src/PyGraphing/graph.py
--rw-rw-rw-   0        0        0      632 2023-12-15 16:57:44.000000 PyGraphing-1.0.0/src/PyGraphing/icon.py
--rw-rw-rw-   0        0        0     1652 2023-12-12 20:13:05.000000 PyGraphing-1.0.0/src/PyGraphing/legend.py
--rw-rw-rw-   0        0        0     2250 2023-12-15 16:57:44.000000 PyGraphing-1.0.0/src/PyGraphing/plot.py
-drwxrwxrwx   0        0        0        0 2023-12-15 16:58:20.298407 PyGraphing-1.0.0/src/PyGraphing/series/
--rw-rw-rw-   0        0        0       29 2023-12-13 15:23:44.000000 PyGraphing-1.0.0/src/PyGraphing/series/__init__.py
--rw-rw-rw-   0        0        0        0 2023-12-13 14:55:22.000000 PyGraphing-1.0.0/src/PyGraphing/series/bars.py
--rw-rw-rw-   0        0        0        0 2023-12-15 16:47:35.000000 PyGraphing-1.0.0/src/PyGraphing/series/box.py
--rw-rw-rw-   0        0        0        0 2023-12-15 16:47:35.000000 PyGraphing-1.0.0/src/PyGraphing/series/error_bars.py
--rw-rw-rw-   0        0        0        0 2023-12-13 14:02:18.000000 PyGraphing-1.0.0/src/PyGraphing/series/line.py
--rw-rw-rw-   0        0        0     1123 2023-12-13 14:02:18.000000 PyGraphing-1.0.0/src/PyGraphing/series/pie.py
--rw-rw-rw-   0        0        0        0 2023-12-13 14:55:21.000000 PyGraphing-1.0.0/src/PyGraphing/series/scatter.py
--rw-rw-rw-   0        0        0      937 2023-12-13 16:18:35.000000 PyGraphing-1.0.0/src/PyGraphing/series/series.py
-drwxrwxrwx   0        0        0        0 2023-12-15 16:58:20.299407 PyGraphing-1.0.0/src/PyGraphing.egg-info/
--rw-rw-rw-   0        0        0    41660 2023-12-15 16:58:20.000000 PyGraphing-1.0.0/src/PyGraphing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      851 2023-12-15 16:58:20.000000 PyGraphing-1.0.0/src/PyGraphing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-15 16:58:20.000000 PyGraphing-1.0.0/src/PyGraphing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-12-15 16:58:20.000000 PyGraphing-1.0.0/src/PyGraphing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2022-09-12 17:37:59.000000 PyGraphing-1.0.0/src/__init__.py
--rw-rw-rw-   0        0        0     1822 2023-12-15 16:54:58.000000 PyGraphing-1.0.0/src/test.py
+drwxrwxrwx   0        0        0        0 2024-03-04 20:58:14.876286 PyGraphing-1.0.1/
+-rw-rw-rw-   0        0        0    35823 2022-09-12 17:26:44.000000 PyGraphing-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    41660 2024-03-04 20:58:14.875279 PyGraphing-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      462 2024-03-04 20:56:49.000000 PyGraphing-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-03-04 20:58:14.877280 PyGraphing-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-03-04 20:58:14.847279 PyGraphing-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-03-04 20:58:14.851279 PyGraphing-1.0.1/src/PyGraphing/
+-rw-rw-rw-   0        0        0      132 2023-12-15 17:02:44.000000 PyGraphing-1.0.1/src/PyGraphing/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-04 20:58:14.864278 PyGraphing-1.0.1/src/PyGraphing/accessories/
+-rw-rw-rw-   0        0        0       32 2023-12-15 17:02:44.000000 PyGraphing-1.0.1/src/PyGraphing/accessories/__init__.py
+-rw-rw-rw-   0        0        0     3849 2023-12-15 17:02:44.000000 PyGraphing-1.0.1/src/PyGraphing/accessories/bezier.py
+drwxrwxrwx   0        0        0        0 2024-03-04 20:58:14.867281 PyGraphing-1.0.1/src/PyGraphing/data_sturctures/
+-rw-rw-rw-   0        0        0     1992 2023-12-15 17:02:44.000000 PyGraphing-1.0.1/src/PyGraphing/data_sturctures/PriorityQueue.py
+-rw-rw-rw-   0        0        0     1365 2023-12-15 17:02:44.000000 PyGraphing-1.0.1/src/PyGraphing/data_sturctures/UnionFind.py
+-rw-rw-rw-   0        0        0       89 2023-12-15 17:02:44.000000 PyGraphing-1.0.1/src/PyGraphing/data_sturctures/__init__.py
+-rw-rw-rw-   0        0        0     2913 2023-12-15 17:02:44.000000 PyGraphing-1.0.1/src/PyGraphing/data_sturctures/tree.py
+-rw-rw-rw-   0        0        0     5507 2023-12-15 17:02:44.000000 PyGraphing-1.0.1/src/PyGraphing/frame.py
+-rw-rw-rw-   0        0        0     3699 2023-12-26 14:51:10.000000 PyGraphing-1.0.1/src/PyGraphing/graph.py
+-rw-rw-rw-   0        0        0      632 2023-12-15 17:02:44.000000 PyGraphing-1.0.1/src/PyGraphing/icon.py
+-rw-rw-rw-   0        0        0     1676 2024-03-04 20:51:34.000000 PyGraphing-1.0.1/src/PyGraphing/legend.py
+-rw-rw-rw-   0        0        0     2290 2024-03-04 20:48:43.000000 PyGraphing-1.0.1/src/PyGraphing/plot.py
+drwxrwxrwx   0        0        0        0 2024-03-04 20:58:14.873280 PyGraphing-1.0.1/src/PyGraphing/series/
+-rw-rw-rw-   0        0        0       35 2023-12-20 20:09:47.000000 PyGraphing-1.0.1/src/PyGraphing/series/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-12-15 17:02:44.000000 PyGraphing-1.0.1/src/PyGraphing/series/bars.py
+-rw-rw-rw-   0        0        0        0 2023-12-15 17:02:44.000000 PyGraphing-1.0.1/src/PyGraphing/series/box.py
+-rw-rw-rw-   0        0        0        0 2023-12-15 17:02:44.000000 PyGraphing-1.0.1/src/PyGraphing/series/error_bars.py
+-rw-rw-rw-   0        0        0        0 2023-12-15 17:02:44.000000 PyGraphing-1.0.1/src/PyGraphing/series/line.py
+-rw-rw-rw-   0        0        0     1123 2023-12-15 17:02:44.000000 PyGraphing-1.0.1/src/PyGraphing/series/pie.py
+-rw-rw-rw-   0        0        0        0 2023-12-15 17:02:44.000000 PyGraphing-1.0.1/src/PyGraphing/series/scatter.py
+-rw-rw-rw-   0        0        0     1353 2024-03-04 20:51:34.000000 PyGraphing-1.0.1/src/PyGraphing/series/series.py
+drwxrwxrwx   0        0        0        0 2024-03-04 20:58:14.874278 PyGraphing-1.0.1/src/PyGraphing.egg-info/
+-rw-rw-rw-   0        0        0    41660 2024-03-04 20:58:14.000000 PyGraphing-1.0.1/src/PyGraphing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      851 2024-03-04 20:58:14.000000 PyGraphing-1.0.1/src/PyGraphing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-04 20:58:14.000000 PyGraphing-1.0.1/src/PyGraphing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-03-04 20:58:14.000000 PyGraphing-1.0.1/src/PyGraphing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2022-09-12 17:37:59.000000 PyGraphing-1.0.1/src/__init__.py
+-rw-rw-rw-   0        0        0     1822 2023-12-15 16:54:58.000000 PyGraphing-1.0.1/src/test.py
```

### Comparing `PyGraphing-1.0.0/LICENSE` & `PyGraphing-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyGraphing-1.0.0/PKG-INFO` & `PyGraphing-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGraphing
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python interface for creating SVG Graphs
 Author-email: Carter Bodinger <carterallenbodinger@yahoo.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `PyGraphing-1.0.0/src/PyGraphing/accessories/bezier.py` & `PyGraphing-1.0.1/src/PyGraphing/accessories/bezier.py`

 * *Files identical despite different names*

### Comparing `PyGraphing-1.0.0/src/PyGraphing/data_sturctures/PriorityQueue.py` & `PyGraphing-1.0.1/src/PyGraphing/data_sturctures/PriorityQueue.py`

 * *Files identical despite different names*

### Comparing `PyGraphing-1.0.0/src/PyGraphing/data_sturctures/UnionFind.py` & `PyGraphing-1.0.1/src/PyGraphing/data_sturctures/UnionFind.py`

 * *Files identical despite different names*

### Comparing `PyGraphing-1.0.0/src/PyGraphing/data_sturctures/tree.py` & `PyGraphing-1.0.1/src/PyGraphing/data_sturctures/tree.py`

 * *Files identical despite different names*

### Comparing `PyGraphing-1.0.0/src/PyGraphing/frame.py` & `PyGraphing-1.0.1/src/PyGraphing/frame.py`

 * *Files identical despite different names*

### Comparing `PyGraphing-1.0.0/src/PyGraphing/graph.py` & `PyGraphing-1.0.1/src/PyGraphing/graph.py`

 * *Files identical despite different names*

### Comparing `PyGraphing-1.0.0/src/PyGraphing/icon.py` & `PyGraphing-1.0.1/src/PyGraphing/icon.py`

 * *Files identical despite different names*

### Comparing `PyGraphing-1.0.0/src/PyGraphing/legend.py` & `PyGraphing-1.0.1/src/PyGraphing/legend.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,38 +26,40 @@
         return self.icon.h + self.top + self.bot
 
     def set(self):
         self.icon.x = self.x + self.left
         self.icon.y = self.y + self.top
 
         self.text.x = self.x + self.left + self.icon.w + self.midl
-        self.text.y = self.top + self.icon.y / 2 + self.y
+        self.text.y = self.icon.y + self.icon.h / 2
 
 
 class Legend(Section):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._items = []
         self.y0 = 0
 
         self.background = Rect(active=False)
         self.addChild(self.background)
 
     def addItem(self, icon: Icon, text: Text, **kwargs):
         self._items.append(Item(icon, text, **kwargs))
 
-    def _set(self):
+    def set(self):
         y = self.y0
         for item in self._items:
             item.y = y
             y += item.h
 
-            self.addChild(item.icon)
+            self.addChild(item.icon.root)
             self.addChild(item.text)
 
+            item.set()
+
     @property
     def xywh(self):
         return self.x, self.y, self.w, self.h
 
     @xywh.setter
     def xywh(self, vals: tuple[float, float, float, float]):
         self.x = vals[0]
```

### Comparing `PyGraphing-1.0.0/src/PyGraphing/plot.py` & `PyGraphing-1.0.1/src/PyGraphing/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 
 class Plot(Section):
     def __init__(self):
         super().__init__()
         self.xmin, self.ymin, self.xmax, self.ymax = 0, 0, 1, 1
         self.background = Rect()
+        self.background.active = False
         self.addChild(self.background)
 
     @property
     def extrema(self):
         return self.xmin, self.xmax, self.ymin, self.ymax
 
     @extrema.setter
```

### Comparing `PyGraphing-1.0.0/src/PyGraphing/series/pie.py` & `PyGraphing-1.0.1/src/PyGraphing/series/pie.py`

 * *Files identical despite different names*

### Comparing `PyGraphing-1.0.0/src/PyGraphing/series/series.py` & `PyGraphing-1.0.1/src/PyGraphing/series/series.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from ..plot import Plot
-from PySVG import G
+from PySVG import G, Path
 from numpy import ndarray
 from ..icon import Icon
 
 
 class Series(G):
     def __init__(self, plot: Plot, x: ndarray, y: ndarray):
         super().__init__()
@@ -32,7 +32,21 @@
 
     def _set_icon(self, x: float, y: float):
         icon = self.icon.copy()
         icon.x = x
         icon.y = y
 
         self.add_child(icon.root)
+
+
+class Line(Series):
+    def __init__(self, path: Path, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.path = path
+        self.add_child(self.path)
+
+    def _process(self):
+        x = self.plot.cart2pixel_x(self.X)
+        y = self.plot.cart2pixel_y(self.Y)
+        f = ['M'] + ['L'] * (len(x) - 1)
+
+        self.path.points = [(i, j, k) for i, j, k in zip(f, x, y)]
```

### Comparing `PyGraphing-1.0.0/src/PyGraphing.egg-info/PKG-INFO` & `PyGraphing-1.0.1/src/PyGraphing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGraphing
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python interface for creating SVG Graphs
 Author-email: Carter Bodinger <carterallenbodinger@yahoo.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `PyGraphing-1.0.0/src/PyGraphing.egg-info/SOURCES.txt` & `PyGraphing-1.0.1/src/PyGraphing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyGraphing-1.0.0/src/test.py` & `PyGraphing-1.0.1/src/test.py`

 * *Files identical despite different names*

