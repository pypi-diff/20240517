# Comparing `tmp/sees-0.0.8.tar.gz` & `tmp/sees-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sees-0.0.8.tar", last modified: Mon Jan 29 10:49:31 2024, max compression
+gzip compressed data, was "sees-0.0.9.tar", last modified: Fri May 17 16:12:39 2024, max compression
```

## Comparing `sees-0.0.8.tar` & `sees-0.0.9.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2024-01-29 10:49:31.206977 sees-0.0.8/
--rw-r--r--   0 claudio   (1001) claudio   (1001)     5992 2024-01-29 10:49:31.206977 sees-0.0.8/PKG-INFO
--rw-r--r--   0 claudio   (1001) claudio   (1001)     4451 2024-01-29 10:49:01.000000 sees-0.0.8/README.md
--rw-r--r--   0 claudio   (1001) claudio   (1001)     1661 2024-01-29 10:49:14.000000 sees-0.0.8/pyproject.toml
--rw-r--r--   0 claudio   (1001) claudio   (1001)       38 2024-01-29 10:49:31.206977 sees-0.0.8/setup.cfg
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2024-01-29 10:49:31.166977 sees-0.0.8/src/
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2024-01-29 10:49:31.186977 sees-0.0.8/src/sees/
--rwxr-xr-x   0 claudio   (1001) claudio   (1001)    25505 2023-10-13 05:48:39.000000 sees-0.0.8/src/sees/__init__.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     3238 2023-10-02 09:11:10.000000 sees-0.0.8/src/sees/__main__.py
--rwxr-xr-x   0 claudio   (1001) claudio   (1001)    46057 2023-07-12 02:10:35.000000 sees-0.0.8/src/sees/_render.py
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2024-01-29 10:49:31.196977 sees-0.0.8/src/sees/canvas/
--rw-r--r--   0 claudio   (1001) claudio   (1001)      714 2023-07-16 22:32:53.000000 sees-0.0.8/src/sees/canvas/canvas.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     3066 2023-10-13 07:27:00.000000 sees-0.0.8/src/sees/canvas/gltflib.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     1543 2023-07-16 22:33:08.000000 sees-0.0.8/src/sees/canvas/mpl.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     6282 2023-11-15 23:40:38.000000 sees-0.0.8/src/sees/canvas/ply.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     1458 2023-07-16 22:33:22.000000 sees-0.0.8/src/sees/canvas/tri.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     6223 2023-10-24 02:51:23.000000 sees-0.0.8/src/sees/cli.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     1390 2023-08-02 18:16:22.000000 sees-0.0.8/src/sees/config.py
--rwxr-xr-x   0 claudio   (1001) claudio   (1001)     5608 2023-07-16 22:18:49.000000 sees-0.0.8/src/sees/consolidate.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)        0 2023-07-16 06:07:59.000000 sees-0.0.8/src/sees/core.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)        1 2023-08-16 06:09:56.000000 sees-0.0.8/src/sees/schema.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     5760 2023-07-18 14:45:02.000000 sees-0.0.8/src/sees/section.py
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2024-01-29 10:49:31.196977 sees-0.0.8/src/sees/solid/
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2024-01-29 10:49:31.196977 sees-0.0.8/src/sees/solid/convert/
--rw-r--r--   0 claudio   (1001) claudio   (1001)     3303 2022-12-07 20:44:36.000000 sees-0.0.8/src/sees/solid/convert/convert.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)      383 2022-12-07 20:44:36.000000 sees-0.0.8/src/sees/solid/convert/example.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     1460 2023-03-28 16:46:02.000000 sees-0.0.8/src/sees/solid/ops.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)      265 2023-03-28 16:26:56.000000 sees-0.0.8/src/sees/solid/plt.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)        0 2023-03-27 17:30:37.000000 sees-0.0.8/src/sees/structure.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)      611 2023-10-01 21:52:01.000000 sees-0.0.8/src/sees/tcl.py
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2024-01-29 10:49:31.196977 sees-0.0.8/src/sees/utilities/
--rw-r--r--   0 claudio   (1001) claudio   (1001)     3098 2023-07-12 17:28:46.000000 sees-0.0.8/src/sees/utilities/alpha_shape.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)      202 2023-07-16 06:08:31.000000 sees-0.0.8/src/sees/views.py
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2024-01-29 10:49:31.206977 sees-0.0.8/src/sees.egg-info/
--rw-r--r--   0 claudio   (1001) claudio   (1001)     5992 2024-01-29 10:49:30.000000 sees-0.0.8/src/sees.egg-info/PKG-INFO
--rw-r--r--   0 claudio   (1001) claudio   (1001)      733 2024-01-29 10:49:31.000000 sees-0.0.8/src/sees.egg-info/SOURCES.txt
--rw-r--r--   0 claudio   (1001) claudio   (1001)        1 2024-01-29 10:49:30.000000 sees-0.0.8/src/sees.egg-info/dependency_links.txt
--rw-r--r--   0 claudio   (1001) claudio   (1001)       44 2024-01-29 10:49:30.000000 sees-0.0.8/src/sees.egg-info/entry_points.txt
--rw-r--r--   0 claudio   (1001) claudio   (1001)       69 2024-01-29 10:49:30.000000 sees-0.0.8/src/sees.egg-info/requires.txt
--rw-r--r--   0 claudio   (1001) claudio   (1001)       12 2024-01-29 10:49:30.000000 sees-0.0.8/src/sees.egg-info/top_level.txt
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2024-01-29 10:49:31.206977 sees-0.0.8/tests/
--rw-r--r--   0 claudio   (1001) claudio   (1001)      108 2022-06-20 06:36:53.000000 sees-0.0.8/tests/test.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2024-05-17 16:12:39.727245 sees-0.0.9/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     6185 2024-05-17 16:12:39.727245 sees-0.0.9/PKG-INFO
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     4644 2024-04-11 21:39:24.000000 sees-0.0.9/README.md
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     1661 2024-05-17 16:12:26.000000 sees-0.0.9/pyproject.toml
+-rw-r--r--   0 claudio   (1001) claudio   (1001)       38 2024-05-17 16:12:39.727245 sees-0.0.9/setup.cfg
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2024-05-17 16:12:39.727245 sees-0.0.9/src/
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2024-05-17 16:12:39.727245 sees-0.0.9/src/sees/
+-rwxr-xr-x   0 claudio   (1001) claudio   (1001)    26406 2024-05-04 07:17:00.000000 sees-0.0.9/src/sees/__init__.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     3238 2023-10-02 09:11:10.000000 sees-0.0.9/src/sees/__main__.py
+-rwxr-xr-x   0 claudio   (1001) claudio   (1001)    46057 2023-07-12 02:10:35.000000 sees-0.0.9/src/sees/_render.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2024-05-17 16:12:39.727245 sees-0.0.9/src/sees/canvas/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      714 2023-07-16 22:32:53.000000 sees-0.0.9/src/sees/canvas/canvas.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     3066 2023-10-13 07:27:00.000000 sees-0.0.9/src/sees/canvas/gltflib.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     1700 2024-04-19 06:57:33.000000 sees-0.0.9/src/sees/canvas/mpl.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     7210 2024-04-14 21:41:53.000000 sees-0.0.9/src/sees/canvas/ply.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     1458 2023-07-16 22:33:22.000000 sees-0.0.9/src/sees/canvas/tri.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     6208 2024-05-17 09:25:36.000000 sees-0.0.9/src/sees/cli.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     1430 2024-04-19 05:06:30.000000 sees-0.0.9/src/sees/config.py
+-rwxr-xr-x   0 claudio   (1001) claudio   (1001)     5608 2023-07-16 22:18:49.000000 sees-0.0.9/src/sees/consolidate.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)        0 2023-07-16 06:07:59.000000 sees-0.0.9/src/sees/core.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      167 2024-04-11 06:03:14.000000 sees-0.0.9/src/sees/frame.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      170 2024-04-11 06:03:00.000000 sees-0.0.9/src/sees/plane.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)        1 2023-08-16 06:09:56.000000 sees-0.0.9/src/sees/schema.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     5776 2024-05-15 19:32:10.000000 sees-0.0.9/src/sees/section.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2024-05-17 16:12:39.727245 sees-0.0.9/src/sees/solid/
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2024-05-17 16:12:39.727245 sees-0.0.9/src/sees/solid/convert/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     3303 2022-12-07 20:44:36.000000 sees-0.0.9/src/sees/solid/convert/convert.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      383 2022-12-07 20:44:36.000000 sees-0.0.9/src/sees/solid/convert/example.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     1460 2023-03-28 16:46:02.000000 sees-0.0.9/src/sees/solid/ops.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      265 2023-03-28 16:26:56.000000 sees-0.0.9/src/sees/solid/plt.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      639 2024-03-07 21:49:42.000000 sees-0.0.9/src/sees/tcl.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2024-05-17 16:12:39.727245 sees-0.0.9/src/sees/utilities/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     3098 2023-07-12 17:28:46.000000 sees-0.0.9/src/sees/utilities/alpha_shape.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      202 2024-04-19 06:11:25.000000 sees-0.0.9/src/sees/views.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2024-05-17 16:12:39.727245 sees-0.0.9/src/sees.egg-info/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     6185 2024-05-17 16:12:39.000000 sees-0.0.9/src/sees.egg-info/PKG-INFO
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      747 2024-05-17 16:12:39.000000 sees-0.0.9/src/sees.egg-info/SOURCES.txt
+-rw-r--r--   0 claudio   (1001) claudio   (1001)        1 2024-05-17 16:12:39.000000 sees-0.0.9/src/sees.egg-info/dependency_links.txt
+-rw-r--r--   0 claudio   (1001) claudio   (1001)       44 2024-05-17 16:12:39.000000 sees-0.0.9/src/sees.egg-info/entry_points.txt
+-rw-r--r--   0 claudio   (1001) claudio   (1001)       69 2024-05-17 16:12:39.000000 sees-0.0.9/src/sees.egg-info/requires.txt
+-rw-r--r--   0 claudio   (1001) claudio   (1001)       12 2024-05-17 16:12:39.000000 sees-0.0.9/src/sees.egg-info/top_level.txt
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2024-05-17 16:12:39.727245 sees-0.0.9/tests/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      108 2022-06-20 06:36:53.000000 sees-0.0.9/tests/test.py
```

### Comparing `sees-0.0.8/PKG-INFO` & `sees-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sees
-Version: 0.0.8
+Version: 0.0.9
 Summary: A modern OpenSees renderer
 Author-email: "Claudio M. Perez" <50180406+claudioperez@users.noreply.github.com>, Chrystal Chern <52893467+chrystalchern@users.noreply.github.com>
 Project-URL: repository, http://github.com/BRACE2/sees
 Keywords: seismic,post-processing,finite-element-analysis,earthquake-engineering
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -161,14 +161,23 @@
 See also
 
 - [`opensees`](https://pypi.org/project/opensees)
 - [`osmg`](https://pypi.org/project/osmg)
 - [`mdof`](https://pypi.org/project/mdof)
 - [`sdof`](https://pypi.org/project/sdof)
 
+For OpenSees rendering
+
+- [`vfo`](https://vfo.readthedocs.io/en/latest/)
+- [`opsvis`](https://opsvis.readthedocs.io/en/latest/index.html)
+
+Other
+
+- [`fapp`](https://github.com/wcfrobert/fapp)
+
 ## Support
 
 <table align="center">
 <tr>
 
   <td>
     <a href="https://peer.berkeley.edu">
```

### Comparing `sees-0.0.8/README.md` & `sees-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -123,14 +123,23 @@
 See also
 
 - [`opensees`](https://pypi.org/project/opensees)
 - [`osmg`](https://pypi.org/project/osmg)
 - [`mdof`](https://pypi.org/project/mdof)
 - [`sdof`](https://pypi.org/project/sdof)
 
+For OpenSees rendering
+
+- [`vfo`](https://vfo.readthedocs.io/en/latest/)
+- [`opsvis`](https://opsvis.readthedocs.io/en/latest/index.html)
+
+Other
+
+- [`fapp`](https://github.com/wcfrobert/fapp)
+
 ## Support
 
 <table align="center">
 <tr>
 
   <td>
     <a href="https://peer.berkeley.edu">
```

#### html2text {}

```diff
@@ -33,9 +33,12 @@
 Tcl script instead of the JSON file: ```shell python -m sees model.tcl -
 o model.html ``` To plot an elevation (`elev`) plan (`plan`) or section
 (`sect`) view, run: ```shell python -m sees model.json --view elev ``` and add
 `-o ` as appropriate. To see the help page run ```shell python -m sees --help
 ```
 See also - [`opensees`](https://pypi.org/project/opensees) - [`osmg`](https://
 pypi.org/project/osmg) - [`mdof`](https://pypi.org/project/mdof) - [`sdof`]
-(https://pypi.org/project/sdof) ## Support
+(https://pypi.org/project/sdof) For OpenSees rendering - [`vfo`](https://
+vfo.readthedocs.io/en/latest/) - [`opsvis`](https://opsvis.readthedocs.io/en/
+latest/index.html) Other - [`fapp`](https://github.com/wcfrobert/fapp) ##
+Support
                    _[_P_E_E_R_ _L_o_g_o_] _[_C_a_l_t_r_a_n_s_ _L_o_g_o_] _[_B_R_A_C_E_2_ _L_o_g_o_]
```

### Comparing `sees-0.0.8/pyproject.toml` & `sees-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sees"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   {name="Claudio M. Perez", email="50180406+claudioperez@users.noreply.github.com"},
   {name="Chrystal Chern",   email="52893467+chrystalchern@users.noreply.github.com"}
 ]
 description="A modern OpenSees renderer"
 
 readme = "README.md"
```

### Comparing `sees-0.0.8/src/sees/__init__.py` & `sees-0.0.9/src/sees/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,20 @@
 #----------------------------------------------------
 
 # The following functions are used for reshaping data
 # and carrying out other miscellaneous operations.
 
 class RenderError(Exception): pass
 
+def _is_basic_frame(el):
+    return     "beam" in el["type"].lower() \
+            or "dfrm" in el["type"].lower()
+
+#   return "zero" not in el["type"].lower()
+
 def clean_model(sam:dict, shift: Array = None, rot=None)->dict:
     """
     Process OpenSees JSON output and return dict with the form:
 
         {<elem tag>: {"crd": [<coordinates>], ...}}
     """
     try:
@@ -34,23 +40,25 @@
     except KeyError:
         pass
 
     ndm = 3
     R = np.eye(ndm) if rot is None else rot
 
     geom = sam.get("geometry", sam.get("assembly"))
+
     if shift is None:
         shift = np.zeros(ndm)
     else:
         shift = np.asarray(shift)
+
     try:
         #coord = np.array([R@n.pop("crd") for n in geom["nodes"]], dtype=FLOAT) + shift
         coord = np.array([R@n["crd"] for n in geom["nodes"]], dtype=FLOAT) + shift
     except:
-        coord = np.array([R@[*n.pop("crd"), 0.0] for n in geom["nodes"]], dtype=FLOAT) + shift
+        coord = np.array([R@[*n["crd"], 0.0] for n in geom["nodes"]], dtype=FLOAT) + shift
 
     nodes = {
             n["name"]: {**n, "crd": coord[i], "idx": i}
                 for i,n in enumerate(geom["nodes"])
     }
 
     ndm = len(next(iter(nodes.values()))["crd"])
@@ -109,15 +117,24 @@
 
 def get_section_geometries(model, config=None):
     if config is not None and "standard_section" in config:
         outline = {
             "square":  np.array([[-1., -1.],
                                  [ 1., -1.],
                                  [ 1.,  1.],
-                                 [-1.,  1.]])
+                                 [-1.,  1.]]),
+
+            "tee":     np.array([[ 6.0,  0.0],
+                                 [ 6.0,  4.0],
+                                 [-6.0,  4.0],
+                                 [-6.0,  0.0],
+                                 [-2.0,  0.0],
+                                 [-2.0, -8.0],
+                                 [ 2.0, -8.0],
+                                 [ 2.0,  0.0]])/10
         }[config["standard_section"]]
 
         config["default_section"] = outline
         return {
             elem["name"]: outline
             for elem in model["assembly"].values() if "sections" in elem
         }
@@ -195,15 +212,15 @@
     else:
         ui, vi, uj, vj = v
     xi = x/L
     M3 = 1 - xi
     M4 = 6/L*(xi-xi**2)
     M5 = 1 - 4*xi+3*xi**2
     M6 = -2*xi + 3*xi**2
-    return (ui*M3+vi*M5+uj*M4+vj*M6).flatten()
+    return (ui*M3 + vi*M5 + uj*M4 + vj*M6).flatten()
 
 def orientation(xyz, yvec=None):
     """Create a rotation matrix between local E and global e basis
     """
     dx = xyz[-1] - xyz[0]
     L = np.linalg.norm(dx)
     e1 = dx/L
@@ -278,65 +295,71 @@
     return Q.T@local_curve + coord[0][None,:].T
 
 
 class SkeletalRenderer:
     def __init__(self, model, response=None, ndf=None, loc=None, vert=2, **kwds):
         self.ndm = 3
 
-        if ndf is None: ndf = 6
+        if ndf is None:
+            ndf = 6
+
+        elif ndf == 3:
+            self.ndm = 2
 
         if vert == 3:
             R = np.eye(3)
         else:
             R = np.array(((1,0, 0),
                           (0,0,-1),
                           (0,1, 0)))
 
         self.plot_rotation = R
 
         self.model = clean_model(model, shift=loc, rot=R)
 
         # Create permutation matrix
-        if self.model["ndm"] == 2:
+#       if self.model["ndm"] == 2:
+        if ndf == 3:
             P = np.array(((1,0, 0),
                           (0,1, 0),
                           (0,0, 0),
 
                           (0,0, 0),
                           (0,0, 0),
                           (0,0, 1)))
         else:
             P = np.eye(6)
 
+
         self.dofs2plot = block_diag(*[R]*2)@P
 
 
-        self.response_layers = defaultdict(lambda : np.zeros((len(self.model["nodes"]), ndf)))
+        self.response_layers = defaultdict(lambda : np.zeros((len(self.model["nodes"]), 6)))
 
 
         config = Config()
         if "config" in kwds:
             apply_config(kwds.pop("config"), config)
         apply_config(kwds, config)
         self.config = config
 
 
         plotter = config.get("plotter", "matplotlib")
         if plotter == "matplotlib":
             import sees.canvas.mpl
-            self.canvas = sees.canvas.mpl.MatplotlibCanvas()
+            self.canvas = sees.canvas.mpl.MatplotlibCanvas(**config["canvas"])
         elif plotter == "plotly":
             import sees.canvas.ply
-            self.canvas = sees.canvas.ply.PlotlyCanvas()
+            self.canvas = sees.canvas.ply.PlotlyCanvas(**config["canvas"])
         elif plotter == "gltf":
             import sees.canvas.gltflib
-            self.canvas = sees.canvas.gltflib.GltfLibCanvas()
+            self.canvas = sees.canvas.gltflib.GltfLibCanvas(**config["canvas"])
         elif plotter == "trimesh":
             import sees.canvas.tri
-            self.canvas = sees.canvas.tri.TrimeshCanvas()
+            self.canvas = sees.canvas.tri.TrimeshCanvas(**config["canvas"])
         else:
             raise ValueError("Unknown plotter " + str(plotter))
 
         self.canvas.config = config
 
     def add_point_displacements(self, displ, scale=1.0, name=None):
         displ_array = self.response_layers[name]
@@ -383,56 +406,57 @@
             else:
                 for k, v in displ.items():
                     yield self.add_displacement_case(v, name=k, scale=scale)
         else:
             yield self.add_displacement_case(displ, scale=scale)
 
 
-    def label_nodes(self): ...
-
-
     def plot_origin(self, **kwds):
         xyz = np.zeros((3,3))
-        uvw = np.eye(3)*kwds.get("scale", 1.0)
+        uvw = self.plot_rotation.T*kwds.get("scale", 1.0)
+        off = [[0, -kwds.get("scale", 1.0)/2, 0],
+               [0]*3,
+               [0]*3] #kwds.get("scale", 1.0)/10
+#       uvw = np.eye(3)*kwds.get("scale", 1.0)
         self.canvas.plot_vectors(xyz, uvw, **kwds)
         if hasattr(self.canvas, "annotate"):
             for i,label in enumerate(kwds.get("label", [])):
-                self.canvas.annotate(label, (xyz+uvw)[i])
+                self.canvas.annotate(label, (xyz+uvw)[i]+off[i])
 
 #   def plot_frame_axes(self):
 #       for elem in self.model["assembly"].values():
 #           xyz = (elem["crd"][-1] + elem["crd"][0])/2
 #           uvw = np.eye(3)/np.linalg.norm(elem["crd"][-1] - elem["crd"][0])
 #           self.canvas.plot_vectors(xyz, uvw)
 
-    def add_elem_data(self):
-        N = 3
-        coords = np.zeros((len(self.model["assembly"])*(N+1),self.ndm))
-        coords.fill(np.nan)
-        for i,el in enumerate(self.model["assembly"].values()):
-            coords[(N+1)*i:(N+1)*i+N,:] = np.linspace(*el["crd"], N)
-
-        coords = coords.reshape(-1,4,3)[:,-3]
-
-        x,y,z = coords.T
-        keys  = ["tag",]
-        frames = np.array(list(self.model["assembly"].keys()),dtype=FLOAT)[:,None]
-        try:
-            # TODO: Make this nicer
-            self.canvas.data.append({
-                    "name": "frames",
-                    "x": x, "y": y, "z": z,
-                    "type": "scatter3d","mode": "markers",
-                    "hovertemplate": "<br>".join(f"{k}: %{{customdata[{v}]}}" for v,k in enumerate(keys)),
-                    "customdata": frames,
-                    "opacity": 0
-                    #"marker": {"opacity": 0.0,"size": 0.0, "line": {"width": 0.0}}
-            })
-        except:
-            pass
+#   def add_elem_data(self):
+#       N = 3
+#       coords = np.zeros((len(self.model["assembly"])*(N+1),self.ndm))
+#       coords.fill(np.nan)
+#       for i,el in enumerate(self.model["assembly"].values()):
+#           coords[(N+1)*i:(N+1)*i+N,:] = np.linspace(*el["crd"], N)
+
+#       coords = coords.reshape(-1,4,3)[:,-3]
+
+#       x,y,z = coords.T
+#       keys  = ["tag",]
+#       frames = np.array(list(self.model["assembly"].keys()),dtype=FLOAT)[:,None]
+#       try:
+#           # TODO: Make this nicer
+#           self.canvas.data.append({
+#                   "name": "frames",
+#                   "x": x, "y": y, "z": z,
+#                   "type": "scatter3d","mode": "markers",
+#                   "hovertemplate": "<br>".join(f"{k}: %{{customdata[{v}]}}" for v,k in enumerate(keys)),
+#                   "customdata": frames,
+#                   "opacity": 0
+#                   #"marker": {"opacity": 0.0,"size": 0.0, "line": {"width": 0.0}}
+#           })
+#       except:
+#           pass
 
     def add_elem_data(self):
         N = 3
         exclude_keys = {"type", "instances", "nodes", "crd", "crdTransformation"}
 
         if "prototypes" not in self.model:
             elem_types = defaultdict(lambda: defaultdict(list))
@@ -480,33 +504,34 @@
                 "type": "scatter3d", "mode": "markers", # "lines", #
                 "hovertemplate": "<br>".join(f"{k}: %{{customdata[{v}]}}" for v,k in enumerate(keys)),
                 "customdata": data,
                 "opacity": 0.6 if "zerolength" in name.lower() and "zerolength" in self.config["show_objects"] else 0
                 #"marker": {"opacity": 0.0,"size": 0.0, "line": {"width": 0.0}}
             })
 
+
     def plot_chords(self, assembly, displ=None, layer=None):
         frame = self.model
         nodes = self.model["nodes"]
         ndm   = self.model["ndm"]
 
         N = 2
-        coords = np.zeros((len(frame["assembly"])*(N+1),self.ndm))
+        coords = np.zeros((len(frame["assembly"])*(N+1),3))
         coords.fill(np.nan)
 
         for i,el in enumerate(frame["assembly"].values()):
             coords[(N+1)*i:(N+1)*i+N,:] = np.linspace(el["crd"][0], el["crd"][-1], N)
 
             # exclude zero-length elements
             if "zero" not in el["type"].lower() and displ is not None:
                 coords[(N+1)*i:(N+1)*i+N,:] += [
                     displ[nodes[n]["name"]][:ndm] for n in (el["nodes"][0], el["nodes"][-1])
                 ]
 
-        self.canvas.plot_lines(coords)
+        self.canvas.plot_lines(coords[:,:self.ndm])
 
 
     def plot_extruded_frames(self, displ=None, rotations=None):
         from scipy.spatial.transform import Rotation
 
         sections = get_section_geometries(self.model, self.config)
 
@@ -584,15 +609,15 @@
 
         show_edges = True
         if show_edges:
             IDX = np.array((
                 (0, 2),
                 (0, 1)
             ))
-            nan = np.zeros(self.ndm)*np.nan
+            nan = np.zeros(3)*np.nan
             coords = np.array(coords)
             tri_points = np.array([
                 coords[idx]  if (j+1)%3 else nan for j,idx in enumerate(np.array(triang).reshape(-1))
                 # coords[i]  if j%2 else nan for j,idx in enumerate(np.array(triang)) for i in idx[IDX[j%2]]
             ])
             Xe, Ye, Ze = tri_points.T
             self.canvas.data.append({
@@ -606,51 +631,51 @@
 
 
 
     def plot_displaced_assembly(self, assembly, displ=None, label=None):
         frame = self.model
         nodes = self.model["nodes"]
         N = 10 if displ is not None else 2
-        coords = np.zeros((len(frame["assembly"])*(N+1),self.ndm))
+        coords = np.zeros((len(frame["assembly"])*(N+1), 3))
         coords.fill(np.nan)
 
         for i,el in enumerate(frame["assembly"].values()):
             # exclude zero-length elements
-            if "zero" not in el["type"].lower() and displ is not None:
+            if _is_basic_frame(el) and displ is not None:
                 glob_displ = [
                     u for n in el["nodes"]
                         for u in displ[nodes[n]["idx"]]
                 ]
                 vect = None #np.array(el["trsfm"]["vecInLocXZPlane"])[axes]
                 coords[(N+1)*i:(N+1)*i+N,:] = displaced_profile(el["crd"], glob_displ, vect=vect, npoints=N).T
-            else:
+            elif len(el["crd"]) == 2:
                 coords[(N+1)*i:(N+1)*i+N,:] = np.linspace(*el["crd"], N)
 
-        self.canvas.plot_lines(coords, color="red", label=label)
+        self.canvas.plot_lines(coords[:, :self.ndm], color="red", label=label)
 
     def plot_nodes(self, displ=None, data=None):
         coord = self.model["coord"]
         if displ is not None:
-            coord = coord + displ[:, :self.ndm]
-        self.canvas.plot_nodes(coord, data=data)
+            coord = coord + displ[:, :3] #self.ndm]
+        self.canvas.plot_nodes(coord[:,:self.ndm], data=data)
 
     def add_triads(self, displ=None):
         ne = len(self.model["assembly"])
         xyz, uvw = np.nan*np.zeros((2, ne, 3, 3))
 
         for i,el in enumerate(self.model["assembly"].values()):
             scale = np.linalg.norm(el["crd"][-1] - el["crd"][0])/10
             coord = sum(i for i in el["crd"])/len(el["nodes"])
             xyz[i,:,:] = np.array([coord]*3)
             uvw[i,:,:] = scale*orientation(el["crd"], el["trsfm"]["yvec"])
 #           self.canvas.plot_vectors(np.array([coord]*3), scale*rotation(el["crd"], el["trsfm"]["yvec"]))
         self.canvas.plot_vectors(xyz.reshape(ne*3,3), uvw.reshape(ne*3,3))
 
 
-    def plot(self):
+    def draw(self):
         if "frames" in self.config["show_objects"]:
             self.plot_chords(self.model["assembly"])
             try:
                 self.add_elem_data()
             except:
                 pass
 
@@ -708,15 +733,15 @@
 
         repl.interp._interp.createcommand("plot", plot)
         # repl.interp._interp.createcommand("show", lambda *args: self.canvas.show())
         repl.repl()
 
 
 
-def render(sam_file, res_file=None, noshow=False, **opts):
+def render(sam_file, res_file=None, noshow=False, ndf=6, **opts):
     # Configuration is determined by successively layering
     # from sources with the following priorities:
     #      defaults < file configs < kwds 
 
     config = Config()
 
     if sam_file is None:
@@ -729,15 +754,15 @@
         model = sam_file
 
     if "RendererConfiguration" in model:
         apply_config(model["RendererConfiguration"], config)
 
     apply_config(opts, config)
 
-    renderer = SkeletalRenderer(model, **config)
+    renderer = SkeletalRenderer(model, ndf=ndf, **config)
 
     # Read and clean displacements 
     # TODO: 
     # - remove `cases` var, 
     # - change add_displacements from being a generator
     # rename `name` parameter
     if res_file is not None:
@@ -751,18 +776,18 @@
     if "Displacements" in model:
         cases.extend(renderer.add_displacements(model["Displacements"],scale=config["scale"],
                                                 name=config["mode_num"]))
 
 
     # write plot to file if file name provided
     if config["write_file"]:
-        renderer.plot()
+        renderer.draw()
         renderer.write(config["write_file"])
 
     else:
-        renderer.plot()
+        renderer.draw()
         if not noshow:
             renderer.canvas.show()
         # renderer.repl()
 
     return renderer
```

### Comparing `sees-0.0.8/src/sees/__main__.py` & `sees-0.0.9/src/sees/__main__.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.8/src/sees/_render.py` & `sees-0.0.9/src/sees/_render.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.8/src/sees/canvas/canvas.py` & `sees-0.0.9/src/sees/canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.8/src/sees/canvas/gltflib.py` & `sees-0.0.9/src/sees/canvas/gltflib.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.8/src/sees/canvas/mpl.py` & `sees-0.0.9/src/sees/canvas/mpl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 # Claudio Perez
 import numpy as np
 from .canvas import Canvas
 from ..views import VIEWS
 
 class MatplotlibCanvas(Canvas):
-    def __init__(self, ax=None):
+    def __init__(self, ndm=3, ax=None):
+
+        self.ndm = ndm
+
+        import matplotlib.pyplot as plt
+        self.plt = plt
         if ax is None:
-            import matplotlib.pyplot as plt
-            self.plt = plt
             _, ax = plt.subplots(1, 1, subplot_kw={"projection": "3d"})
             ax.set_autoscale_on(True)
             ax.set_axis_off()
 
         self.ax = ax
 
     def show(self):
         self.plt.show()
 
     def build(self):
         ax = self.ax
         opts = self.config
-        aspect = [ub - lb for lb, ub in (getattr(ax, f'get_{a}lim')() for a in 'xyz')]
+        aspect = [ub - lb for lb, ub in (getattr(ax, f'get_{a}lim')() for a in 'xyz'[:self.ndm])]
         aspect = [max(a,max(aspect)/8) for a in aspect]
-        ax.set_box_aspect(aspect)
-        ax.view_init(**VIEWS[opts["view"]])
+        if self.ndm == 3:
+            ax.set_box_aspect(aspect)#, zoom=3)
+            ax.view_init(**VIEWS[opts["view"]])
+        else:
+            ax.set_aspect("equal") #set_box_aspect(1)#, zoom=3)
         return ax
 
     def write(self, filename=None):
         self.ax.figure.savefig(self.config["write_file"])
 
     def plot_lines(self, coords, label=None, conf=None, color=None):
         props = conf or {"color": color or "grey", "alpha": 0.6, "linewidth": 0.5}
```

### Comparing `sees-0.0.8/src/sees/canvas/ply.py` & `sees-0.0.9/src/sees/canvas/ply.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,32 +9,45 @@
         self.annotations = []
 
     def show(self):
         self.fig.show(renderer="browser")
 
     def build(self):
         opts = self.config
-        show_axis = "axis" in opts["show_objects"]
+#       show_axis = "axis" in opts["show_objects"]
         show_grid = "grid" in opts["show_objects"]
         import plotly.graph_objects as go
         fig = go.Figure(dict(
                 data=self.data,
                 rendermode='webgl',
                 layout=go.Layout(
+#                 paper_bgcolor='white',
                   scene=dict(aspectmode="data",
-                     xaxis = {"showspikes": "tick" in opts["show_objects"],
-                              "showbackground": show_grid, "gridcolor": "gray" if show_grid else None},
-                     yaxis = {"showspikes": "tick" in opts["show_objects"],
-                              "showbackground": show_grid, "gridcolor": "gray" if show_grid else None},
-                     zaxis = {"showspikes": "tick" in opts["show_objects"],
-                              "showbackground": show_grid, "gridcolor": "gray" if show_grid else None},
-                     xaxis_title = r"$\mathbf{E}_1$",
-                     xaxis_visible = "x" in opts["show_objects"],#show_axis,
-                     yaxis_visible = "y" in opts["show_objects"],#show_axis,
-                     zaxis_visible = "z" in opts["show_objects"],#show_axis,
+                         xaxis = {"showspikes": "tick" in opts["show_objects"], "nticks": 0,
+                              "showbackground": show_grid, "backgroundcolor": "white",
+                              "showticklabels": "tick" in opts["show_objects"],
+                              "gridcolor": "gray" if show_grid else None
+                         },
+                         yaxis = {"showspikes": "tick" in opts["show_objects"], "nticks": 0,
+                              "showbackground": show_grid, "backgroundcolor": "white",
+                              "showticklabels": "tick" in opts["show_objects"],
+                              "gridcolor": "gray" if show_grid else None
+                         },
+                         zaxis = {"showspikes": "tick" in opts["show_objects"], "nticks": 0,
+                              "showbackground": show_grid, "backgroundcolor": "white",
+                              "showticklabels": "tick" in opts["show_objects"],
+                              "gridcolor": "gray" if show_grid else None
+                         },
+                     # LaTeX is not currently rendered in 3D, see:
+                     # https://github.com/plotly/plotly.js/issues/608
+#                    xaxis_title = r"$\mathbf{E}_1$",
+                     xaxis_title = "", yaxis_title="", zaxis_title="",
+                     xaxis_visible =  "x" in opts["show_objects"],#show_axis,
+                     yaxis_visible =  "y" in opts["show_objects"],#show_axis,
+                     zaxis_visible =  "z" in opts["show_objects"],#show_axis,
                      camera=dict(
                          projection={"type": opts["camera"]["projection"]}
                      ),
                      annotations=self.annotations
                   ),
 #                 showlegend=("legend" in opts["show_objects"])
                 )
@@ -45,22 +58,27 @@
                           projection=dict(
                               z=dict(show=True),
                           )
         )
         self.fig = fig
         return self
 
-    def write(self, filename=None):
+    def write(self, filename=None, format=None):
         opts = self.config
         if "html" in filename:
             import plotly
             fig = self.fig
             html = plotly.io.to_html(fig, div_id=str(id(self)), **opts["save_options"]["html"])
+            #import plotly.offline
+            #plotly.offline.plot(data, include_plotlyjs=False, output_type='div')
+
             with open(opts["write_file"],"w+") as f:
                 f.write(html)
+
+
         elif "png" in filename:
             self.fig.write_image(filename, width=1920, height=1080)
         elif "json" in opts["write_file"]:
             with open(opts["write_file"],"w+") as f:
                 self.fig.write_json(f)
 
     def make_hover_data(self, data, ln=None):
@@ -156,14 +174,14 @@
         x,y,z = zip(*vertices)
         i,j,k = zip(*triangles)
         self.data.append({
             #"name": label if label is not None else "",
             "type": "mesh3d",
             "x": x, "y": y, "z": z, "i": i, "j": j, "k": k,
             "hoverinfo":"skip",
-            "lighting": dict(ambient=0.9, roughness=0.5, specular=2),
+#           "lighting": dict(ambient=0.9, roughness=0.5, specular=2),
 #           "lighting": dict(ambient=0.4, diffuse=0.5, roughness = 0.9, specular=0.6, fresnel=0.2),
             "opacity": 1.0 if opacity is None else opacity,
             "color": color,
             # "color": "white",
             # "opacity": 0.2
         })
```

### Comparing `sees-0.0.8/src/sees/canvas/tri.py` & `sees-0.0.9/src/sees/canvas/tri.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.8/src/sees/cli.py` & `sees-0.0.9/src/sees/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import sys
 from sees import config, RenderError
 
 
 __version__ = "0.0.4"
 
 NAME = "sees"
 
@@ -118,17 +119,17 @@
                 import ast
                 k,v = next(args).split("=")
                 val = ast.literal_eval(v)
                 d = opts
                 keys = k.split(".")
                 for key in keys[:-1]:
                     d = d[key]
-                import sys
                 d[keys[-1]] = val
 
+
             elif arg[:2] == "-s":
                 opts["scale"] = float(arg[2:]) if len(arg) > 2 else float(next(args))
             elif arg == "--scale":
                 scale = next(args)
                 if "=" in scale:
                     # looks like --scale <object>=<scale>
                     k,v = scale.split("=")
```

### Comparing `sees-0.0.8/src/sees/config.py` & `sees-0.0.9/src/sees/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
   "res_file":     None,
   "write_file":   None,
   "displ":        defaultdict(list),
   "scale":        100.0,
   "vert":         2,
   "view":         "iso",
   "plotter":      "matplotlib",
+  "canvas":       {}, # kwds for canvas
 
   "camera": {
       "view": "iso",               # iso | plan| elev[ation] | sect[ion]
       "projection": "orthographic" # perspective | orthographic
   },
 
   "displacements": {"scale": 100, "color": "#660505"},
```

### Comparing `sees-0.0.8/src/sees/consolidate.py` & `sees-0.0.9/src/sees/consolidate.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.8/src/sees/section.py` & `sees-0.0.9/src/sees/section.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         show = ["fiber", "patch", "layer"]
 
     if isinstance(s, list):
         pass
 
     return MatplotlibSectionCanvas(ax=ax).plot_section(s, show=show, **kwds)
 
+
 class MatplotlibSectionCanvas:
     def __init__(self, ax=None, **kwds):
         self.ax = ax
         self.kwds = kwds
     def get_section_layers(self, section, **kwds):
         import matplotlib.lines as lines
         for layer in section.layers:
@@ -138,32 +139,33 @@
                     plt.Circle(f.coord, radius=sqrt(f.area/np.pi), linewidth=0)
                         for patch in section.patches for f in patch.fibers
                 ]
                 c = matplotlib.collections.PatchCollection(circles)
                 ax.add_collection(c)
             else:
                 # TODO: clean this up
-                try:
-                    ax.scatter(*zip(*(f.coord for patch in section.patches for f in patch.fibers)), s=0.1)
-                except:
-                    pass
+#               try:
+#                   ax.scatter(*zip(*(f.coord for patch in section.patches for f in patch.fibers)), s=0.1)
+#               except Exception as e:
+#                   print(e)
+#                   pass
 
                 try:
-                    ax.scatter(*zip(*(f.coord for patch in section.patches for f in patch.fibers)), s=0.1)
+                    ax.scatter(*zip(*(f.coord for f in section.fibers)), s=0.1)
                 except Exception as e:
-                    # print(e)
+                    print(e)
                     pass
 
 
-                try:
-                    coords, areas = zip(*((f.coord, 20*f.area) for layer in section.layers for f in layer.fibers))
-                    ax.scatter(*zip(*coords), s=areas, color="k")
-                except Exception as e:
-                    # print(e)
-                    pass
+#               try:
+#                   coords, areas = zip(*((f.coord, 20*f.area) for layer in section.layers for f in layer.fibers))
+#                   ax.scatter(*zip(*coords), s=areas, color="k")
+#               except Exception as e:
+#                   # print(e)
+#                   pass
 
         # show centroid
         #ax.scatter(*section.centroid)
         # show origin
         # ax.scatter(0, 0)
         ax.axis("equal")
         #plt.show()
```

### Comparing `sees-0.0.8/src/sees/solid/convert/convert.py` & `sees-0.0.9/src/sees/solid/convert/convert.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.8/src/sees/solid/ops.py` & `sees-0.0.9/src/sees/solid/ops.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.8/src/sees/utilities/alpha_shape.py` & `sees-0.0.9/src/sees/utilities/alpha_shape.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.8/src/sees.egg-info/PKG-INFO` & `sees-0.0.9/src/sees.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sees
-Version: 0.0.8
+Version: 0.0.9
 Summary: A modern OpenSees renderer
 Author-email: "Claudio M. Perez" <50180406+claudioperez@users.noreply.github.com>, Chrystal Chern <52893467+chrystalchern@users.noreply.github.com>
 Project-URL: repository, http://github.com/BRACE2/sees
 Keywords: seismic,post-processing,finite-element-analysis,earthquake-engineering
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -161,14 +161,23 @@
 See also
 
 - [`opensees`](https://pypi.org/project/opensees)
 - [`osmg`](https://pypi.org/project/osmg)
 - [`mdof`](https://pypi.org/project/mdof)
 - [`sdof`](https://pypi.org/project/sdof)
 
+For OpenSees rendering
+
+- [`vfo`](https://vfo.readthedocs.io/en/latest/)
+- [`opsvis`](https://opsvis.readthedocs.io/en/latest/index.html)
+
+Other
+
+- [`fapp`](https://github.com/wcfrobert/fapp)
+
 ## Support
 
 <table align="center">
 <tr>
 
   <td>
     <a href="https://peer.berkeley.edu">
```

### Comparing `sees-0.0.8/src/sees.egg-info/SOURCES.txt` & `sees-0.0.9/src/sees.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 src/sees/__init__.py
 src/sees/__main__.py
 src/sees/_render.py
 src/sees/cli.py
 src/sees/config.py
 src/sees/consolidate.py
 src/sees/core.py
+src/sees/frame.py
+src/sees/plane.py
 src/sees/schema.py
 src/sees/section.py
-src/sees/structure.py
 src/sees/tcl.py
 src/sees/views.py
 src/sees.egg-info/PKG-INFO
 src/sees.egg-info/SOURCES.txt
 src/sees.egg-info/dependency_links.txt
 src/sees.egg-info/entry_points.txt
 src/sees.egg-info/requires.txt
```

