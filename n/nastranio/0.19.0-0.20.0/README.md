# Comparing `tmp/nastranio-0.19.0.tar.gz` & `tmp/nastranio-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nastranio-0.19.0.tar", max compression
+gzip compressed data, was "nastranio-0.20.0.tar", max compression
```

## Comparing `nastranio-0.19.0.tar` & `nastranio-0.20.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0        1 2020-01-22 08:16:12.114971 nastranio-0.19.0/LICENSE
--rw-r--r--   0        0        0       89 2020-01-22 08:16:12.114971 nastranio-0.19.0/README.rst
--rw-r--r--   0        0        0     1479 2024-02-27 14:19:59.853717 nastranio-0.19.0/nastranio/__init__.py
--rw-r--r--   0        0        0     3352 2024-02-27 14:19:20.085262 nastranio-0.19.0/nastranio/cards/__init__.py
--rw-r--r--   0        0        0     2030 2023-04-28 07:42:45.007054 nastranio-0.19.0/nastranio/cards/axis.py
--rw-r--r--   0        0        0    19328 2024-02-27 13:48:29.504018 nastranio-0.19.0/nastranio/cards/elements.py
--rw-r--r--   0        0        0     8367 2023-05-31 13:23:34.155937 nastranio-0.19.0/nastranio/cards/loading.py
--rw-r--r--   0        0        0     1617 2023-05-31 13:23:34.155937 nastranio-0.19.0/nastranio/cards/materials.py
--rw-r--r--   0        0        0    11518 2024-02-12 21:44:19.734640 nastranio-0.19.0/nastranio/cards/properties.py
--rw-r--r--   0        0        0     5807 2023-05-31 13:23:34.159937 nastranio-0.19.0/nastranio/cards/types.py
--rw-r--r--   0        0        0    46329 2024-02-27 13:49:33.410031 nastranio-0.19.0/nastranio/cardslib.py
--rw-r--r--   0        0        0     1253 2023-05-31 13:23:34.159937 nastranio-0.19.0/nastranio/cli.py
--rw-r--r--   0        0        0   170959 2023-04-28 07:44:07.063736 nastranio-0.19.0/nastranio/clib.c
--rwxr-xr-x   0        0        0   166416 2023-04-28 08:29:45.772902 nastranio-0.19.0/nastranio/clib.cpython-38-x86_64-linux-gnu.so
--rwxr-xr-x   0        0        0    45440 2023-04-28 07:59:47.406232 nastranio-0.19.0/nastranio/clib.cpython-39-x86_64-linux-gnu.so
--rw-r--r--   0        0        0     1522 2024-02-12 21:59:21.602773 nastranio-0.19.0/nastranio/constants.py
--rw-r--r--   0        0        0    11029 2024-02-27 14:19:20.061262 nastranio-0.19.0/nastranio/decorators.py
--rw-r--r--   0        0        0     7605 2023-05-31 13:23:34.159937 nastranio-0.19.0/nastranio/fields_writer.py
--rw-r--r--   0        0        0       27 2023-04-28 07:42:45.011054 nastranio-0.19.0/nastranio/mesh_api/__init__.py
--rw-r--r--   0        0        0    89538 2024-01-30 14:25:03.117235 nastranio-0.19.0/nastranio/mesh_api/mesh_api.py
--rw-r--r--   0        0        0    12711 2023-12-21 07:32:34.982849 nastranio-0.19.0/nastranio/mesh_api/mod.py
--rw-r--r--   0        0        0     5885 2023-07-09 09:33:40.969349 nastranio-0.19.0/nastranio/mesh_api/rtree_indexes.py
--rw-r--r--   0        0        0     1453 2023-05-31 13:23:34.163937 nastranio-0.19.0/nastranio/pylib.py
--rw-r--r--   0        0        0        0 2020-01-22 08:16:12.126971 nastranio-0.19.0/nastranio/readers/__init__.py
--rw-r--r--   0        0        0    18462 2023-05-31 13:23:34.163937 nastranio-0.19.0/nastranio/readers/bulk.py
--rw-r--r--   0        0        0       29 2023-05-31 13:23:34.167937 nastranio-0.19.0/nastranio/readers/gmsh/__init__.py
--rw-r--r--   0        0        0    12017 2024-02-08 08:27:46.605878 nastranio-0.19.0/nastranio/readers/gmsh/gmsh.py
--rw-r--r--   0        0        0     4359 2023-05-31 13:23:34.167937 nastranio-0.19.0/nastranio/readers/gmsh/mixins.py
--rw-r--r--   0        0        0    17317 2024-02-03 17:59:09.499013 nastranio-0.19.0/nastranio/readers/gmsh/study.py
--rw-r--r--   0        0        0        0 2023-05-31 13:23:34.167937 nastranio-0.19.0/nastranio/readers/gmsh/ui_versions/__init__.py
--rw-r--r--   0        0        0     4910 2023-05-31 13:23:34.167937 nastranio-0.19.0/nastranio/readers/gmsh/ui_versions/user_input_v1.py
--rw-r--r--   0        0        0     9844 2024-01-09 06:45:25.246699 nastranio-0.19.0/nastranio/readers/gmsh/ui_versions/user_input_v2.py
--rw-r--r--   0        0        0      267 2023-05-31 13:23:34.171937 nastranio-0.19.0/nastranio/readers/gmsh/user_input.py
--rw-r--r--   0        0        0     7210 2023-04-28 07:42:45.019054 nastranio-0.19.0/nastranio/readers/op2.py
--rw-r--r--   0        0        0    12642 2023-05-31 13:23:34.171937 nastranio-0.19.0/nastranio/registry.py
--rw-r--r--   0        0        0     1702 2023-04-28 07:42:45.023054 nastranio-0.19.0/nastranio/serializer.py
--rw-r--r--   0        0        0      389 2021-03-23 07:27:54.551241 nastranio-0.19.0/nastranio/types.py
--rw-r--r--   0        0        0    10920 2023-05-31 13:23:34.171937 nastranio-0.19.0/nastranio/utils.py
--rw-r--r--   0        0        0        0 2023-05-31 13:23:34.171937 nastranio-0.19.0/nastranio/writers/__init__.py
--rw-r--r--   0        0        0    15816 2023-07-31 06:05:24.324098 nastranio-0.19.0/nastranio/writers/femap_neutral.py
--rw-r--r--   0        0        0        0 2023-07-31 06:22:37.191405 nastranio-0.19.0/nastranio/writers/templates/__init__.py
--rw-r--r--   0        0        0      576 2023-05-31 13:23:34.175937 nastranio-0.19.0/nastranio/writers/templates/femap_neu.tpl
--rw-r--r--   0        0        0     1239 2024-02-27 14:19:59.853717 nastranio-0.19.0/pyproject.toml
--rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 nastranio-0.19.0/PKG-INFO
+-rw-r--r--   0        0        0        1 2020-01-22 08:16:12.114971 nastranio-0.20.0/LICENSE
+-rw-r--r--   0        0        0       89 2020-01-22 08:16:12.114971 nastranio-0.20.0/README.rst
+-rw-r--r--   0        0        0     1479 2024-05-17 07:25:06.476085 nastranio-0.20.0/nastranio/__init__.py
+-rw-r--r--   0        0        0     3352 2024-02-27 14:19:20.085262 nastranio-0.20.0/nastranio/cards/__init__.py
+-rw-r--r--   0        0        0     2030 2023-04-28 07:42:45.007054 nastranio-0.20.0/nastranio/cards/axis.py
+-rw-r--r--   0        0        0    19328 2024-02-27 13:48:29.504018 nastranio-0.20.0/nastranio/cards/elements.py
+-rw-r--r--   0        0        0     8367 2023-05-31 13:23:34.155937 nastranio-0.20.0/nastranio/cards/loading.py
+-rw-r--r--   0        0        0     1617 2023-05-31 13:23:34.155937 nastranio-0.20.0/nastranio/cards/materials.py
+-rw-r--r--   0        0        0    11518 2024-02-12 21:44:19.734640 nastranio-0.20.0/nastranio/cards/properties.py
+-rw-r--r--   0        0        0     5807 2023-05-31 13:23:34.159937 nastranio-0.20.0/nastranio/cards/types.py
+-rw-r--r--   0        0        0    46329 2024-02-27 13:49:33.410031 nastranio-0.20.0/nastranio/cardslib.py
+-rw-r--r--   0        0        0     1253 2023-05-31 13:23:34.159937 nastranio-0.20.0/nastranio/cli.py
+-rw-r--r--   0        0        0   170959 2023-04-28 07:44:07.063736 nastranio-0.20.0/nastranio/clib.c
+-rwxr-xr-x   0        0        0   166416 2023-04-28 08:29:45.772902 nastranio-0.20.0/nastranio/clib.cpython-38-x86_64-linux-gnu.so
+-rwxr-xr-x   0        0        0    45440 2023-04-28 07:59:47.406232 nastranio-0.20.0/nastranio/clib.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0     1522 2024-02-12 21:59:21.602773 nastranio-0.20.0/nastranio/constants.py
+-rw-r--r--   0        0        0    11029 2024-02-27 14:19:20.061262 nastranio-0.20.0/nastranio/decorators.py
+-rw-r--r--   0        0        0     7605 2023-05-31 13:23:34.159937 nastranio-0.20.0/nastranio/fields_writer.py
+-rw-r--r--   0        0        0       27 2023-04-28 07:42:45.011054 nastranio-0.20.0/nastranio/mesh_api/__init__.py
+-rw-r--r--   0        0        0    89538 2024-01-30 14:25:03.117235 nastranio-0.20.0/nastranio/mesh_api/mesh_api.py
+-rw-r--r--   0        0        0    12953 2024-05-16 12:57:58.823327 nastranio-0.20.0/nastranio/mesh_api/mod.py
+-rw-r--r--   0        0        0     5885 2023-07-09 09:33:40.969349 nastranio-0.20.0/nastranio/mesh_api/rtree_indexes.py
+-rw-r--r--   0        0        0     1453 2023-05-31 13:23:34.163937 nastranio-0.20.0/nastranio/pylib.py
+-rw-r--r--   0        0        0        0 2020-01-22 08:16:12.126971 nastranio-0.20.0/nastranio/readers/__init__.py
+-rw-r--r--   0        0        0    18462 2023-05-31 13:23:34.163937 nastranio-0.20.0/nastranio/readers/bulk.py
+-rw-r--r--   0        0        0       29 2023-05-31 13:23:34.167937 nastranio-0.20.0/nastranio/readers/gmsh/__init__.py
+-rw-r--r--   0        0        0    12017 2024-02-08 08:27:46.605878 nastranio-0.20.0/nastranio/readers/gmsh/gmsh.py
+-rw-r--r--   0        0        0     4359 2023-05-31 13:23:34.167937 nastranio-0.20.0/nastranio/readers/gmsh/mixins.py
+-rw-r--r--   0        0        0    17317 2024-02-03 17:59:09.499013 nastranio-0.20.0/nastranio/readers/gmsh/study.py
+-rw-r--r--   0        0        0        0 2023-05-31 13:23:34.167937 nastranio-0.20.0/nastranio/readers/gmsh/ui_versions/__init__.py
+-rw-r--r--   0        0        0     4910 2023-05-31 13:23:34.167937 nastranio-0.20.0/nastranio/readers/gmsh/ui_versions/user_input_v1.py
+-rw-r--r--   0        0        0     9844 2024-01-09 06:45:25.246699 nastranio-0.20.0/nastranio/readers/gmsh/ui_versions/user_input_v2.py
+-rw-r--r--   0        0        0      267 2023-05-31 13:23:34.171937 nastranio-0.20.0/nastranio/readers/gmsh/user_input.py
+-rw-r--r--   0        0        0     7210 2023-04-28 07:42:45.019054 nastranio-0.20.0/nastranio/readers/op2.py
+-rw-r--r--   0        0        0    12642 2023-05-31 13:23:34.171937 nastranio-0.20.0/nastranio/registry.py
+-rw-r--r--   0        0        0     1702 2023-04-28 07:42:45.023054 nastranio-0.20.0/nastranio/serializer.py
+-rw-r--r--   0        0        0      389 2021-03-23 07:27:54.551241 nastranio-0.20.0/nastranio/types.py
+-rw-r--r--   0        0        0    10920 2023-05-31 13:23:34.171937 nastranio-0.20.0/nastranio/utils.py
+-rw-r--r--   0        0        0        0 2023-05-31 13:23:34.171937 nastranio-0.20.0/nastranio/writers/__init__.py
+-rw-r--r--   0        0        0    15816 2023-07-31 06:05:24.324098 nastranio-0.20.0/nastranio/writers/femap_neutral.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:22:37.191405 nastranio-0.20.0/nastranio/writers/templates/__init__.py
+-rw-r--r--   0        0        0      576 2023-05-31 13:23:34.175937 nastranio-0.20.0/nastranio/writers/templates/femap_neu.tpl
+-rw-r--r--   0        0        0     1239 2024-05-17 07:25:06.468084 nastranio-0.20.0/pyproject.toml
+-rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 nastranio-0.20.0/PKG-INFO
```

### Comparing `nastranio-0.19.0/nastranio/__init__.py` & `nastranio-0.20.0/nastranio/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.19.0"
+__version__ = "0.20.0"
 
 import logging
 import sys
 from typing import Dict, Optional
 
 from colorama import Back, Fore, Style
```

### Comparing `nastranio-0.19.0/nastranio/cards/__init__.py` & `nastranio-0.20.0/nastranio/cards/__init__.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/cards/axis.py` & `nastranio-0.20.0/nastranio/cards/axis.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/cards/elements.py` & `nastranio-0.20.0/nastranio/cards/elements.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/cards/loading.py` & `nastranio-0.20.0/nastranio/cards/loading.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/cards/materials.py` & `nastranio-0.20.0/nastranio/cards/materials.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/cards/properties.py` & `nastranio-0.20.0/nastranio/cards/properties.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/cards/types.py` & `nastranio-0.20.0/nastranio/cards/types.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/cardslib.py` & `nastranio-0.20.0/nastranio/cardslib.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/cli.py` & `nastranio-0.20.0/nastranio/cli.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/clib.c` & `nastranio-0.20.0/nastranio/clib.c`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/clib.cpython-38-x86_64-linux-gnu.so` & `nastranio-0.20.0/nastranio/clib.cpython-38-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/clib.cpython-39-x86_64-linux-gnu.so` & `nastranio-0.20.0/nastranio/clib.cpython-39-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/constants.py` & `nastranio-0.20.0/nastranio/constants.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/decorators.py` & `nastranio-0.20.0/nastranio/decorators.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/fields_writer.py` & `nastranio-0.20.0/nastranio/fields_writer.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/mesh_api/mesh_api.py` & `nastranio-0.20.0/nastranio/mesh_api/mesh_api.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/mesh_api/mod.py` & `nastranio-0.20.0/nastranio/mesh_api/mod.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Mesh Modification package"""
+
 import logging
 import numbers
 from collections import defaultdict
 
 import numpy as np
 from numpy.lib import recfunctions as rfn
 
@@ -233,14 +234,15 @@
         """split elements found close to each point"""
         if eids:
             rtree = self.reg.mesh.mod.rtrees.create_rtree(eids=eids)
         if not round_t_digits:
             # round `t` to number of digits of margin, therefore, defaulted to 2
             round_t_digits = len(str(float(margin)).split(".")[-1])
         _details = []
+        _historic_by_eid = defaultdict(list)
         _prev_eids = defaultdict(set)
         for i, point in enumerate(points):
             prev_eids = self.rtrees.nearest_elements(
                 point, cardname=cardname, rtree=rtree, astype=list
             )
             prev_eid = next(iter(prev_eids))
             if cardname:
@@ -280,25 +282,27 @@
                     root_eid = prev_eid
                 _prev_eids[root_eid].add(new_eid)
             else:
                 # no element split. An existing node is returned, so, let's return the
                 # existing element as mother and child element
                 root_eid = prev_eid
                 new_eid = prev_eid
-            _details.append(
-                {
-                    "prev_eid": root_eid,
-                    "eid": new_eid,
-                    "gid": new_gid,
-                    "XA": point[0],
-                    "XB": point[1],
-                    "XC": point[2],
-                    "t": round(t, round_t_digits),
-                }
-            )
+                # but maybe prev_eid comes from a previous plit...?
+            _historic_by_eid[new_eid].append(root_eid)
+            __details = {
+                "prev_eids": _historic_by_eid[new_eid],  # ths whole historic
+                "prev_eid": root_eid,  # really the last one
+                "eid": new_eid,
+                "gid": new_gid,
+                "XA": point[0],
+                "XB": point[1],
+                "XC": point[2],
+                "t": round(t, round_t_digits),
+            }
+            _details.append(__details)
         # -----------------------------------------------------------------
         # rebuild caches
         self.bulk["GRID"].clear_caches()
         card = self.reg.container["bulk"][cardname]
         card.clear_caches()
         self.reg.mesh.clear_caches()
         return _details
```

### Comparing `nastranio-0.19.0/nastranio/mesh_api/rtree_indexes.py` & `nastranio-0.20.0/nastranio/mesh_api/rtree_indexes.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/pylib.py` & `nastranio-0.20.0/nastranio/pylib.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/readers/bulk.py` & `nastranio-0.20.0/nastranio/readers/bulk.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/readers/gmsh/gmsh.py` & `nastranio-0.20.0/nastranio/readers/gmsh/gmsh.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/readers/gmsh/mixins.py` & `nastranio-0.20.0/nastranio/readers/gmsh/mixins.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/readers/gmsh/study.py` & `nastranio-0.20.0/nastranio/readers/gmsh/study.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/readers/gmsh/ui_versions/user_input_v1.py` & `nastranio-0.20.0/nastranio/readers/gmsh/ui_versions/user_input_v1.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/readers/gmsh/ui_versions/user_input_v2.py` & `nastranio-0.20.0/nastranio/readers/gmsh/ui_versions/user_input_v2.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/readers/op2.py` & `nastranio-0.20.0/nastranio/readers/op2.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/registry.py` & `nastranio-0.20.0/nastranio/registry.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/serializer.py` & `nastranio-0.20.0/nastranio/serializer.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/utils.py` & `nastranio-0.20.0/nastranio/utils.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/writers/femap_neutral.py` & `nastranio-0.20.0/nastranio/writers/femap_neutral.py`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/nastranio/writers/templates/femap_neu.tpl` & `nastranio-0.20.0/nastranio/writers/templates/femap_neu.tpl`

 * *Files identical despite different names*

### Comparing `nastranio-0.19.0/pyproject.toml` & `nastranio-0.20.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nastranio"
-version = "0.19.0"
+version = "0.20.0"
 description = ""
 authors = ["Nicolas Cordier <nicolas.cordier@numeric-gmbh.ch>"]
 readme = "README.rst"
 include = [
 	{ path = "writers"},
 	]
```

### Comparing `nastranio-0.19.0/PKG-INFO` & `nastranio-0.20.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nastranio
-Version: 0.19.0
+Version: 0.20.0
 Summary: 
 Author: Nicolas Cordier
 Author-email: nicolas.cordier@numeric-gmbh.ch
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Click
```

