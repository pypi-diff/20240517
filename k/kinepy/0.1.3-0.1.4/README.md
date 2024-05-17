# Comparing `tmp/kinepy-0.1.3.tar.gz` & `tmp/kinepy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kinepy-0.1.3.tar", last modified: Mon Sep  4 13:46:25 2023, max compression
+gzip compressed data, was "kinepy-0.1.4.tar", last modified: Mon Oct  9 11:59:10 2023, max compression
```

## Comparing `kinepy-0.1.3.tar` & `kinepy-0.1.4.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 13:46:25.432747 kinepy-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (999)     1075 2023-09-04 13:46:13.000000 kinepy-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     5909 2023-09-04 13:46:25.432747 kinepy-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     5490 2023-09-04 13:46:13.000000 kinepy-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 13:46:25.428746 kinepy-0.1.3/kinepy/
--rw-r--r--   0 runner    (1001) docker     (999)       44 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 13:46:25.428746 kinepy-0.1.3/kinepy/compilation/
--rw-r--r--   0 runner    (1001) docker     (999)    14094 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/compilation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     5050 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/compilation/graph_operations.py
--rw-r--r--   0 runner    (1001) docker     (999)     3499 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/compilation/graphs.py
--rw-r--r--   0 runner    (1001) docker     (999)      726 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/compilation/preparation.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 13:46:25.428746 kinepy-0.1.3/kinepy/gui/
--rw-r--r--   0 runner    (1001) docker     (999)     1048 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/gui/Rect.py
--rw-r--r--   0 runner    (1001) docker     (999)     3907 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3425 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/gui/camera.py
--rw-r--r--   0 runner    (1001) docker     (999)     4748 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/gui/drawing_tool.py
--rw-r--r--   0 runner    (1001) docker     (999)     1301 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/gui/getters.py
--rw-r--r--   0 runner    (1001) docker     (999)     3643 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/gui/grid_manager.py
--rw-r--r--   0 runner    (1001) docker     (999)     5377 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/gui/gui_class.py
--rw-r--r--   0 runner    (1001) docker     (999)     4286 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/gui/logo.ico
--rw-r--r--   0 runner    (1001) docker     (999)    11322 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/gui/system_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 13:46:25.432747 kinepy-0.1.3/kinepy/interface/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     6089 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/interface/decorators.py
--rw-r--r--   0 runner    (1001) docker     (999)     2923 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/interface/interactions.py
--rw-r--r--   0 runner    (1001) docker     (999)     2150 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/interface/joints.py
--rw-r--r--   0 runner    (1001) docker     (999)     1532 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/interface/metaclass.py
--rw-r--r--   0 runner    (1001) docker     (999)     1372 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/interface/relations.py
--rw-r--r--   0 runner    (1001) docker     (999)     1978 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/interface/solid.py
--rw-r--r--   0 runner    (1001) docker     (999)    11395 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/interface/system.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 13:46:25.432747 kinepy-0.1.3/kinepy/math/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      964 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/math/calculus.py
--rw-r--r--   0 runner    (1001) docker     (999)     6225 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/math/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (999)     1543 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/math/geometry.py
--rw-r--r--   0 runner    (1001) docker     (999)     7687 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/math/kinematic.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 13:46:25.432747 kinepy-0.1.3/kinepy/objects/
--rw-r--r--   0 runner    (1001) docker     (999)      311 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      847 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/objects/interactions.py
--rw-r--r--   0 runner    (1001) docker     (999)     9827 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/objects/joints.py
--rw-r--r--   0 runner    (1001) docker     (999)     3676 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/objects/relations.py
--rw-r--r--   0 runner    (1001) docker     (999)      856 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/objects/solid.py
--rw-r--r--   0 runner    (1001) docker     (999)     1578 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/objects/system.py
--rw-r--r--   0 runner    (1001) docker     (999)    12520 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/tools.py
--rw-r--r--   0 runner    (1001) docker     (999)     7961 2023-09-04 13:46:13.000000 kinepy-0.1.3/kinepy/units.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 13:46:25.428746 kinepy-0.1.3/kinepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     5909 2023-09-04 13:46:25.000000 kinepy-0.1.3/kinepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1065 2023-09-04 13:46:25.000000 kinepy-0.1.3/kinepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-04 13:46:25.000000 kinepy-0.1.3/kinepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)        7 2023-09-04 13:46:25.000000 kinepy-0.1.3/kinepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)       79 2023-09-04 13:46:25.432747 kinepy-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)      744 2023-09-04 13:46:13.000000 kinepy-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 11:59:10.135964 kinepy-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-10-09 11:58:59.000000 kinepy-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2023-10-09 11:59:10.135964 kinepy-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2023-10-09 11:58:59.000000 kinepy-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 11:59:10.131964 kinepy-0.1.4/kinepy/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 11:59:10.131964 kinepy-0.1.4/kinepy/compilation/
+-rw-r--r--   0 runner    (1001) docker     (127)    14275 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/compilation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5056 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/compilation/graph_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/compilation/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/compilation/preparation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 11:59:10.131964 kinepy-0.1.4/kinepy/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/gui/Rect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/gui/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/gui/drawing_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/gui/getters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/gui/grid_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/gui/gui_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/gui/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    16025 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/gui/system_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 11:59:10.135964 kinepy-0.1.4/kinepy/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6089 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/interface/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/interface/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/interface/joints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/interface/metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/interface/relations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/interface/solid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11395 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/interface/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 11:59:10.135964 kinepy-0.1.4/kinepy/math/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/math/calculus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/math/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/math/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7687 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/math/kinematic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 11:59:10.135964 kinepy-0.1.4/kinepy/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/objects/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/objects/joints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/objects/relations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/objects/solid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/objects/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12520 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7967 2023-10-09 11:58:59.000000 kinepy-0.1.4/kinepy/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 11:59:10.131964 kinepy-0.1.4/kinepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2023-10-09 11:59:10.000000 kinepy-0.1.4/kinepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2023-10-09 11:59:10.000000 kinepy-0.1.4/kinepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-09 11:59:10.000000 kinepy-0.1.4/kinepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-10-09 11:59:10.000000 kinepy-0.1.4/kinepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-09 11:59:10.000000 kinepy-0.1.4/kinepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2023-10-09 11:59:10.135964 kinepy-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2023-10-09 11:58:59.000000 kinepy-0.1.4/setup.py
```

### Comparing `kinepy-0.1.3/LICENSE` & `kinepy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kinepy-0.1.3/PKG-INFO` & `kinepy-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kinepy
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python library dedicated to plane mechanism simulation
 Home-page: https://github.com/valentin-burillier/kinepy
 Author: Loïc Chevalier - Valentin Burillier
 Keywords: robotics,simulation,dynamics,kinematics,statics,inverse-kinematics,mechanism
 Requires: numpy
 Requires: matplotlib
 Requires: pygame
```

### Comparing `kinepy-0.1.3/README.md` & `kinepy-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `kinepy-0.1.3/kinepy/compilation/__init__.py` & `kinepy-0.1.4/kinepy/compilation/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from kinepy.compilation.graph_operations import isomorph, degrees, distances, vertices_fusion, make_joint_graph, \
+from kinepy.compilation.graph_operations import isomorphic, degrees, distances, vertices_fusion, make_joint_graph, \
     make_relation_graph, match_graph
 from kinepy.compilation.graphs import GRAPHS, DEGREES, SOLVED, NAMES, EDGES, SIGNS
 from kinepy.compilation.preparation import *
 from kinepy.objects.joints import GhostRevolute, GhostPrismatic
 from kinepy.objects.relations import GearRelation
 
 
@@ -41,15 +41,15 @@
 Solved relation {}
 """
 
 # --------------------------------------------------- Constants --------------------------------------------------------
 
 DYNAMICS, KINEMATICS, BOTH = 0, 1, 2
 
-SOLVE_PILOT, SOLVE_GRAPH, SOLVE_RELATION, CSA, SET_ORIGIN, REC_GHOSTS = range(6)
+SOLVE_PILOT, SOLVE_GRAPH, SOLVE_RELATION, CONTINUOUS_SOLID_ANGLE, SET_ORIGIN, REC_GHOSTS = range(6)
 SOLVE_BLOCK, _, _, COMPUTE_MA, COMPUTE_INERTIA, _ = range(6)
 
 
 class Compiler:
     solved = eqs = sol_to_vertex = distances = joint_queue = before_pilot_mapping = delayed_gear_relations = None
 
     def __init__(self, system):
@@ -166,15 +166,15 @@
             self._manage_relations(solids, False, mode)
         return self._finish(mode)
 
     def _finish(self, mode):
         if mode:
             print("Compiling done.\n")
         system = self.system
-        self.kin_instr += [(CSA, system), (SET_ORIGIN, system), (REC_GHOSTS, system)]
+        self.kin_instr += [(CONTINUOUS_SOLID_ANGLE, system), (SET_ORIGIN, system), (REC_GHOSTS, system)]
         self.dyn_instr = [(COMPUTE_INERTIA, system), (COMPUTE_MA, system), *self.dyn_instr, (REC_GHOSTS, system)]
         return (self.dyn_instr, self.kin_instr, (self.kin_instr, self.dyn_instr))[mode]
 
     def _manage_inputs(self, solids, mode):
         if mode:
             print(INPUT_MESSAGE.format(len(self.kin_instr) + 1))
 
@@ -227,17 +227,19 @@
         self.kin_instr.append((SOLVE_GRAPH, self.system, graph_index, concerned_eqs, edges, key))
         self.dyn_instr.insert(0, (SOLVE_GRAPH, graph_index, concerned_eqs, edges, ref))
 
         vertices_fusion(self.joint_graph, sorted(vertex_map), self.eqs, self.sol_to_vertex)
         self.distances = distances(self.joint_graph)
 
     def _common_eq(self, joint1, joint2):
+        """Determines if 2 joints share exactly one eq. Returns their solids that belong to this eq.
+        Used for solving relations."""
         found = None
         for i, s_rep1 in enumerate((joint1.s1.rep, joint1.s2.rep)):
-            for j,  s_rep2 in enumerate((joint2.s1.rep, joint2.s2.rep)):
+            for j, s_rep2 in enumerate((joint2.s1.rep, joint2.s2.rep)):
                 if self.before_pilot_mapping[s_rep1] == self.before_pilot_mapping[s_rep2]:
                     if found is not None:
                         return
                     found = i, j
         return found
 
     def _get_relations(self, delay_allowed):
```

### Comparing `kinepy-0.1.3/kinepy/compilation/graph_operations.py` & `kinepy-0.1.4/kinepy/compilation/graph_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,41 +66,41 @@
     n = len(vertex_map) - 1
     for source, dest in enumerate(vertex_map[:-1]):
         if source_graph[source][n] != dest_graph[dest][vertex_map[n]][0]:
             return False
     return True
 
 
-def isomorph(src_graph, dest_graph, src_deg, dest_deg, vertex_map):
+def isomorphic(src_graph, dest_graph, src_deg, dest_deg, vertex_map):
     """
     Searches a sub-graph of dest that is isomorphic to src
     """
     if len(vertex_map) == len(src_graph):
         return vertex_map
     for vertex in range(len(dest_graph)):
         if vertex not in vertex_map and inf(src_deg[len(vertex_map)], dest_deg[vertex]) and can_match(src_graph, dest_graph, vertex_map + (vertex,)):
-            new_map = isomorph(src_graph, dest_graph, src_deg, dest_deg, vertex_map + (vertex,))
+            new_map = isomorphic(src_graph, dest_graph, src_deg, dest_deg, vertex_map + (vertex,))
             if new_map:
                 return new_map
     return ()
 
 
 def match_graph(joint_graph) -> tuple[int, tuple]:
     dest_deg = degrees(joint_graph)
     for index, (graph, src_deg) in enumerate(zip(GRAPHS, DEGREES)):
-        vertex_map = isomorph(graph, joint_graph, src_deg, dest_deg, ())
+        vertex_map = isomorphic(graph, joint_graph, src_deg, dest_deg, ())
         if vertex_map:
             return index, vertex_map
     # s = '\n'.join(map(str, joint_graph))
     # raise CompilationError(f"None of the known graphs matches the current system graph \n{s}\n"
     #                      f"Either it is hyperstatic or it is not supported")
 
 
 def vertices_fusion(joint_graph, vertices, eqs, sol_to_vertex):
-    """merges all eqs descriped in vertices, vertices is sorted"""
+    """merges all eqs described in vertices, vertices is sorted"""
     dest_vertex = vertices[0]
 
     # going in the reverse order, dest_vertiex is excluded
     for vertex in vertices[:0:-1]:
         # merging eqs
         eqs[dest_vertex] += eqs[vertex]
         # replacing the vertex with the last one
```

### Comparing `kinepy-0.1.3/kinepy/compilation/graphs.py` & `kinepy-0.1.4/kinepy/compilation/graphs.py`

 * *Files identical despite different names*

### Comparing `kinepy-0.1.3/kinepy/compilation/preparation.py` & `kinepy-0.1.4/kinepy/compilation/preparation.py`

 * *Files identical despite different names*

### Comparing `kinepy-0.1.3/kinepy/gui/Rect.py` & `kinepy-0.1.4/kinepy/gui/Rect.py`

 * *Files identical despite different names*

### Comparing `kinepy-0.1.3/kinepy/gui/__init__.py` & `kinepy-0.1.4/kinepy/gui/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 import kinepy.gui.gui_class as _g
 import kinepy.units as _units
 from PIL.Image import frombytes as _from_bytes
 from kinepy.interface.decorators import physics_input_function as _phy, get_object as _get_obj
 
 
 _GUI_VARIABLES = {
-    'frames_of_reference': False,
-    'grid': False,
-    'graduations': False,
+    'frames_of_reference': True,
+    'grid': True,
+    'graduations': True,
     'figure_size': (640, 480),
     'background_color': (0, 0, 0),
     'animation_time': 5.,
     'system': None,
     'points': [],
     'speeds': [],
     'forces': [],
     'torques': [],
     'joint_efforts': []
 }
 
 
 def _reset():
     for key, var in {
-        'frames_of_reference': False,
-        'grid': False,
-        'graduations': False,
-        'figure_size': (640, 480),
-        'background_color': (0, 0, 0),
-        'animation_time': 5.,
-        'system': None,
         'points': [],
         'speeds': [],
         'forces': [],
         'torques': [],
         'joint_efforts': []
     }.items():
         _GUI_VARIABLES[key] = var
@@ -47,30 +40,23 @@
     """Adds the point to the plotting list"""
     _GUI_VARIABLES['points'].append((_get_obj(solid), point * _units.SYSTEM[_units.LENGTH], trace))
     if not speed:
         return
     _GUI_VARIABLES['speeds'].append((_get_obj(solid), point * _units.SYSTEM[_units.LENGTH]))
 
 
-def add_force(solid, force, point):
-    """Behaves just like Solid.add_force but adds the point and the force to the plotting list"""
-    solid.add_force(force, point)
-    f, _, p = solid.external_actions.external[-1]
-    _GUI_VARIABLES['forces'].append((_get_obj(solid), p, f))
-
-
-def add_joint_effort(joint, reverse=False):
+def display_joint_efforts(joint, reverse=False):
     _GUI_VARIABLES['joint_efforts'].append((_get_obj(joint), reverse))
 
 
-def add_torque(solid, torque):
-    """Behaves just like Solid.add_torque but adds the torque to the plotting list"""
-    solid.add_torque(torque)
-    _, t, _ = solid.external_actions.external[-1]
-    _GUI_VARIABLES['torques'].append((_get_obj(solid), t))
+def display_mechanical_action(key):
+    """Displays the given mechanical action represented by the key returned by Solid.add_torque/Solid.add_force"""
+    solid_external, index, _type, *_ = key
+    force, torque, point = solid_external.externals[index]
+    _GUI_VARIABLES[f'{_type}s'].append((_get_obj(solid_external.solid), point, force if _type == 'force' else torque))
 
 
 def grid(value=True):
     """Set the visibility of the grid: True by default"""
     _GUI_VARIABLES['grid'] = value
```

### Comparing `kinepy-0.1.3/kinepy/gui/camera.py` & `kinepy-0.1.4/kinepy/gui/camera.py`

 * *Files identical despite different names*

### Comparing `kinepy-0.1.3/kinepy/gui/getters.py` & `kinepy-0.1.4/kinepy/gui/getters.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 def gather_points(system, points, speeds, forces):
     # points is used to determine the window
     points_ = []
     for s in system.sols:
         points_.append(s.origin)
     for s, point in speeds:
         points_.append(s.origin + rvec(s.angle, point))
-    for s, point, _ in forces + points:
+    for s, point, *_ in forces + points:
         points_.append(s.origin + rvec(s.angle, point))
 
     for joint in system.joints:
         if joint.id_ not in get_points:
             continue
         p1, p2 = get_points[joint.id_](joint)
         points_.append(joint.s1.origin + rvec(joint.s1.angle, p1))
```

### Comparing `kinepy-0.1.3/kinepy/gui/grid_manager.py` & `kinepy-0.1.4/kinepy/gui/grid_manager.py`

 * *Files identical despite different names*

### Comparing `kinepy-0.1.3/kinepy/gui/gui_class.py` & `kinepy-0.1.4/kinepy/gui/gui_class.py`

 * *Files identical despite different names*

### Comparing `kinepy-0.1.3/kinepy/gui/logo.ico` & `kinepy-0.1.4/kinepy/gui/logo.ico`

 * *Files identical despite different names*

### Comparing `kinepy-0.1.3/kinepy/gui/system_manager.py` & `kinepy-0.1.4/kinepy/gui/system_manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,86 @@
+import numpy as np
 from kinepy.gui.drawing_tool import *
-from kinepy.math.geometry import unit, z_cross, rvec, sq_mag
+from kinepy.math.geometry import unit, z_cross, rvec, sq_mag, get_point
 from kinepy.math.calculus import derivative_vec
+from kinepy.objects.joints import Joint
+from kinepy.objects.relations import LinearRelation
 
 
 class SystemManager:
-    force_scale = speed_scale = 0.
+    force_scale = speed_scale = torque_scale = 0.
 
     def __init__(self, system, scale0, points, speeds, forces, torques,  joint_efforts):
         self.scale0 = scale0
 
         # shapes, mounting points of joints
         self.solid_data_step1 = tuple([] for _ in system.sols)
         self.solid_data_step2 = tuple([] for _ in system.sols)
         self.sols = system.sols
 
+        for relation in system.relations:
+            self.get_relation_data(relation)
+
         for joint in system.joints:
-            if joint.id_ in self.get_data_dict:
-                self.get_data(joint)
+            self.get_joint_data(joint)
 
         self.traces = []
-
         for s, p, trace in points:
             self.point_data(s, p)
             if trace:
                 self.traces.append((s, s.origin + rvec(s.angle, p)))
 
         for s, p in speeds:
             self.update_speed_scale(s, p)
         for s, p in speeds:
             self.speed_data(s, p)
 
+        for s, p, f in forces:
+            self.update_force_scale(f())
+        for s, p, f in forces:
+            self.force_data(s, p, f())
+
+        for s, p, t in torques:
+            self.update_torque_scale(t())
+        for s, p, t in torques:
+            self.torque_data(s, t())
+
         for j, rev in joint_efforts:
             self.effort_scales(j)
         for j, rev in joint_efforts:
             self.effort_data(j, rev)
 
+    def do_nothing(self, *args, **kwargs):
+        """Void function"""
+
+    # relation positional data
+    # region
+    def gears_data(self, gear):
+        r1, r2 = gear.get_radii()
+        d = np.nanmax(sq_mag(get_point(gear.j1, 0) - get_point(gear.j2, 0)) ** .5)
+
+        s1, p1 = (gear.j1.s1, gear.j1.s2)[not gear.common_eq[0]], (gear.j1.p1, gear.j1.p2)[not gear.common_eq[0]]
+        self.solid_data_step1[s1.rep].append(('circle', (p1, r1 * d * self.scale0, False)))
+        self.solid_data_step1[s1.rep].append(('lines', np.array((p1, p1 + r1 * d * unit(0)))))
+
+        s2, p2 = (gear.j2.s1, gear.j2.s2)[not gear.common_eq[1]], (gear.j2.p1, gear.j2.p2)[not gear.common_eq[1]]
+        self.solid_data_step1[s2.rep].append(('circle', (p2, r2 * d * self.scale0, False)))
+        self.solid_data_step1[s2.rep].append(('lines', np.array((p2, p2 + r2 * d * unit(gear.v0)))))
+
+    relation_data = {
+        LinearRelation.GEAR: 'gears_data',
+    }
+
+    def get_relation_data(self, rel: LinearRelation):
+        getattr(self, self.relation_data.get(rel.id_, 'do_nothing'))(rel)
+
+    # endregion
+
+    # joint positional data
+    # region
     def revolute_data(self, rev):
         # Regions: GREEN, BLUE, RED, YELLOW
         offset_angles = -np.pi * .5, 0, np.pi, np.pi * .5
         for s, point in (rev.s1, rev.p1), (rev.s2, rev.p2):
             # region matching
             p = np.array(point) * self.scale0 / REVOLUTE_RADIUS
             if not s.rep or p[1] >= 2:
@@ -55,15 +97,15 @@
             self.solid_data_step1[s.rep].append(('line', shape))
             if not s.rep:
                 self.solid_data_step1[s.rep].append(('ground', m_point))
             elif region in (0, 3):
                 self.solid_data_step1[s.rep].append(('lines', np.array(((0., 0.), (m_point[0], 0), m_point))))
             else:
                 self.solid_data_step1[s.rep].append(('lines', np.array(((0., 0.), (0., m_point[1]), m_point))))
-        self.solid_data_step2[rev.s2.rep].append(('circle', (rev.p2, REVOLUTE_RADIUS)))
+        self.solid_data_step2[rev.s2.rep].append(('circle', (rev.p2, REVOLUTE_RADIUS, True)))
 
     def prismatic_data(self, pri):
         u1, u2 = unit(pri.a1), unit(pri.a2)
         v1, v2 = pri.d1 * z_cross(u1), pri.d2 * z_cross(u2)
 
         shape1 = np.einsum('ik,lk->li', rot(pri.a1 + np.pi * (pri.d1 > 0)), PRISMATIC) / self.scale0 + v1
         m_point = shape1[PRISMATIC_MOUNTING_POINT]
@@ -120,87 +162,149 @@
             self.solid_data_step1[pin.s2.rep].append(('ground', m_point))
         elif region2 in (0, 3):
             self.solid_data_step1[pin.s2.rep].append(('lines', np.array(((0., 0.), (m_point[0], 0), m_point))))
         else:
             self.solid_data_step1[pin.s2.rep].append(('lines', np.array(((0., 0.), (0., m_point[1]), m_point))))
 
     get_data_dict = {
-        1: 'revolute_data',
-        2: 'prismatic_data',
-        3: 'pin_slot_data'
+        Joint.REVOLUTE: 'revolute_data',
+        Joint.PRISMATIC: 'prismatic_data',
+        Joint.PIN_SLOT: 'pin_slot_data'
     }
 
-    def get_data(self, joint):
-        getattr(self, self.get_data_dict[joint.id_])(joint)
+    def get_joint_data(self, joint):
+        getattr(self, self.get_data_dict.get(joint.id_, 'do_nothing'))(joint)
+    # endregion
 
+    # single objects data
+    # region
     def point_data(self, solid, point):
-        self.solid_data_step2[solid.rep].append(('circle', (point, REVOLUTE_RADIUS * .5)))
+        self.solid_data_step2[solid.rep].append(('circle', (point, REVOLUTE_RADIUS * .5, True)))
         self.solid_data_step1[solid.rep].append(('lines', np.array(((0., 0.), (point[0], 0), point))))
 
     def speed_data(self, solid, point):
         self.solid_data_step1[solid.rep].append(('lines', np.array(((0., 0.), (point[0], 0), point))))
-        self.solid_data_step2[solid.rep].append(('circle', (point, REVOLUTE_RADIUS * .5)))
+        self.solid_data_step2[solid.rep].append(('circle', (point, REVOLUTE_RADIUS * .5, True)))
 
         real_point = solid.origin + rvec(solid.angle, point)
         speed = derivative_vec(real_point, 1.)
         mag = sq_mag(speed) ** .5
         angle = np.arccos(speed[0] / mag) * (2 * (speed[1] > 0) - 1)
 
         shape = np.einsum('ikn,lk->lin', rot(-angle), ARROW / self.scale0) * mag / self.speed_scale
         self.solid_data_step2[solid.rep].append(('arrow', (real_point, shape)))
 
+    def force_data(self, solid, point, force):
+        self.solid_data_step1[solid.rep].append(('lines', np.array(((0., 0.), (point[0], 0), point))))
+        self.solid_data_step2[solid.rep].append(('circle', (point, REVOLUTE_RADIUS * .5, True)))
+
+        real_point = solid.origin + rvec(solid.angle, point)
+        mag = sq_mag(force) ** .5
+        angle = np.arccos(force[0] / mag) * (2 * (force[1] > 0) - 1)
+
+        shape = np.einsum('ikn,lk->lin', rot(-angle), ARROW / self.scale0) * mag / self.speed_scale
+        self.solid_data_step2[solid.rep].append(('arrow', (real_point, shape)))
+
+    def torque_data(self, solid, torque):
+        shape = np.einsum(
+            'ikn,lk->lin',
+            rot(-solid.angle), CIRCLE_ARROW / self.scale0
+        ) * torque / self.torque_scale
+        self.solid_data_step2[solid.rep].append(('arrow', (solid.origin, shape)))
+    # endregion
+
+    # joint effort data
+    # region
     def rev_effort(self, rev, reverse):
         real_point = rev.s1.origin + rvec(rev.s1.angle, rev.p1)
         mag = sq_mag(rev.force) ** .5
         f = (1, -1)[reverse]
         angle = np.arccos(f * rev.force[0] / mag) * (2 * (f * rev.force[1] > 0) - 1)
         shape = np.einsum('ikn,lk->lin', rot(-angle), ARROW / self.scale0) * mag / self.force_scale
 
-        self.solid_data_step2[(rev.s1.rep, rev.s2.rep)[reverse]].append(('arrow', (real_point, shape)))
+        self.solid_data_step2[(rev.s2.rep, rev.s1.rep)[reverse]].append(('arrow', (real_point, shape)))
 
     def pri_effort(self, pri, reverse):
-        pass
+        real_point = pri.s1.origin + pri.d1 * z_cross(unit(pri.s1.angle + pri.a1))
+        mag, angle = np.abs(pri.normal), pri.s1.angle + pri.a1 + np.pi * .5 * (1, -1)[reverse]
+        shape = np.einsum('ikn,lk->lin', rot(-angle), ARROW / self.scale0) * mag / self.force_scale
+        self.solid_data_step2[(pri.s2.rep, pri.s1.rep)[reverse]].append(('arrow', (real_point, shape)))
+
+        torque = pri.torque * (1, -1)[reverse]
+        shape = np.einsum(
+            'ikn,lk->lin',
+            rot(-(pri.s1.angle + pri.a1)), CIRCLE_ARROW / self.scale0
+        ) * torque / self.torque_scale + pri.d1 * z_cross(unit(pri.s1.angle + pri.a1))
+        self.solid_data_step2[(pri.s2.rep, pri.s1.rep)[reverse]].append(('arrow', (pri.s1.origin, shape)))
 
     def pin_effort(self, pin, reverse):
-        pass
+        u1 = unit(pin.s1.angle + pin.a1)
+        real_point = pin.s1.origin + pin.d1 * z_cross(u1) + pin.sliding * u1
+        mag, angle = np.abs(pin.normal) ** .5, pin.s1.angle + pin.a1 + np.pi * .5 * (1, -1)[reverse]
+        shape = np.einsum('ikn,lk->lin', rot(-angle), ARROW / self.scale0) * mag / self.force_scale
+        self.solid_data_step2[(pin.s2.rep, pin.s1.rep)[reverse]].append(('arrow', (real_point, shape)))
 
     effort_data_dict = {
-        1: 'rev_effort',
-        2: 'pri_effort',
-        3: 'pin_effort'
+        Joint.REVOLUTE: 'rev_effort',
+        Joint.PRISMATIC: 'pri_effort',
+        Joint.PIN_SLOT: 'pin_effort'
     }
 
     def effort_data(self, j, reverse):
-        getattr(self, self.effort_data_dict[j.id_])(j, reverse)
+        getattr(self, self.effort_data_dict.get(j.id_, 'do_nothing'))(j, reverse)
+    # endregion
+
+    # joint effort scales
+    # region
 
     def rev_scales(self, rev):
         mag = sq_mag(rev.force) ** .5
         self.force_scale = max(self.force_scale, np.nanmax(mag))
 
     def pri_scales(self, pri):
-        pass
+        mag = np.abs(pri.normal)
+        self.force_scale = max(self.force_scale, np.nanmax(mag))
+        mag = np.abs(pri.torque)
+        self.torque_scale = max(self.torque_scale, np.nanmax(mag))
 
     def pin_scales(self, pin):
-        pass
+        mag = np.abs(pin.normal)
+        self.force_scale = max(self.force_scale, np.nanmax(mag))
 
     effort_scales_dict = {
-        1: 'rev_scales',
-        2: 'pri_scales',
-        3: 'pin_scales'
+        Joint.REVOLUTE: 'rev_scales',
+        Joint.PRISMATIC: 'pri_scales',
+        Joint.PIN_SLOT: 'pin_scales'
     }
 
     def effort_scales(self, j):
-        getattr(self, self.effort_scales_dict[j.id_])(j)
+        getattr(self, self.effort_scales_dict.get(j.id_, 'do_nothing'))(j)
 
+    # endregion
+
+    # scale setters
+    # region
     def update_speed_scale(self, solid, point):
         real_point = solid.origin + rvec(solid.angle, point)
         speed = derivative_vec(real_point, 1.)
         mag = sq_mag(speed) ** .5
         self.speed_scale = max(self.speed_scale, np.nanmax(mag))
 
+    def update_force_scale(self, force):
+        mag = sq_mag(force) ** .5
+        self.force_scale = max(self.force_scale, np.nanmax(mag))
+
+    def update_torque_scale(self, torque):
+        mag = np.abs(torque)
+        self.torque_scale = max(self.torque_scale, np.nanmax(mag))
+    # endregion
+
+    # parts drawing
+    # region
+
     @staticmethod
     def arrow(camera, color, solid, data):
         frame = int(camera.animation_state)
         point, shape = data
         shape = camera.real_to_screen(point[:, frame]) + shape[:, :, frame] * camera.scale * camera.zoom
         pg.draw.polygon(
             camera.surface,
@@ -236,32 +340,35 @@
             False,
             shape,
             2
         )
 
     @staticmethod
     def circle(camera, color, solid, circle):
-        p, rad = circle
+        p, rad, hide_bg = circle
         frame = int(camera.animation_state)
         point = camera.real_to_screen(solid.origin[:, frame] + rot(solid.angle[frame]) @ p)
-        pg.draw.circle(
-            camera.surface,
-            camera.background,
-            point,
-            rad * camera.scale * camera.zoom / camera.scale0,
-            0
-        )
+        if hide_bg:
+            pg.draw.circle(
+                camera.surface,
+                camera.background,
+                point,
+                rad * camera.scale * camera.zoom / camera.scale0,
+                0
+            )
+
         pg.draw.circle(
             camera.surface,
             color,
             point,
             rad * camera.scale * camera.zoom / camera.scale0,
             2
         )
 
+
     @staticmethod
     def polygon(camera, color, solid, polygon):
         poly = SystemManager.shape_to_screen(camera, solid, polygon)
         pg.draw.polygon(
             camera.surface,
             camera.background,
             poly,
@@ -282,14 +389,15 @@
             pg.draw.line(
                 camera.surface,
                 color,
                 ground[i],
                 ground[i + 1],
                 2
             )
+    # endregion
 
     def draw(self, camera):
         cam_center, surf_center = (
             np.array(camera.camera_area.center)[:, None], np.array(camera.surface.get_rect().center)[:, None]
         )
 
         for s, trace in self.traces:
```

### Comparing `kinepy-0.1.3/kinepy/interface/decorators.py` & `kinepy-0.1.4/kinepy/interface/decorators.py`

 * *Files identical despite different names*

### Comparing `kinepy-0.1.3/kinepy/interface/interactions.py` & `kinepy-0.1.4/kinepy/interface/solid.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,89 +1,43 @@
-import kinepy.objects as obj
+import numpy as np
+
 from kinepy.interface.metaclass import *
 import kinepy.units as units
-from kinepy.math.geometry import ZERO_21, unit, get_angle, get_zero, rvec
-from kinepy.interface.decorators import get_object
-
-
-class Gravity(obj.Gravity, metaclass=MetaUnit):
-    read_write = ('g', ACCELERATION),
-
-
-class Spring(obj.Spring, metaclass=MetaUnit):
-    read_only = FORCE_,
-    read_write = P1, P2, ('k', SPRING_CONSTANT), ('l0', LENGTH)
-
-
-class SolidExternal:
-    def __init__(self, solid):
-        self.solid = solid
-        self.externals = []
-
-    def append(self, force, torque, point):
-        self.externals.append((
-            (lambda: force() * units.SYSTEM[FORCE]),
-            (lambda: torque() * units.SYSTEM[TORQUE]),
-            point
-        ))
-
-    def set_ma(self, _):
-        sol: obj.Solid = get_object(self.solid)
-        for f, t, p in self.externals:
-            sol.add_mech_action(f(), sol.origin + rvec(sol.angle, p), t())
-
-
-class RevoluteTorque:
-
-    def __init__(self, rev, t):
-        self.rev, self._torque = rev, t
-
-    torque = property(
-        (lambda self: (lambda: self._torque() / units.SYSTEM[FORCE])),
-        (lambda self, value: setattr(self, '_torque', (lambda: value() * units.SYSTEM[FORCE])))
-    )
-
-    def set_ma(self, _):
-        t = self._torque()
-        get_object(self.rev).s1.add_mech_action(ZERO_21, 0., t)
-        get_object(self.rev).s2.add_mech_action(ZERO_21, 0., -t)
-
-
-class PrismaticTangent:
-
-    def __init__(self, pri, f):
-        self.pri, self._tangent = pri, f
-
-    tangent = property(
-        (lambda self: (lambda: self._tangent() / units.SYSTEM[FORCE])),
-        (lambda self, value: setattr(self, '_tangent', (lambda: value() * units.SYSTEM[FORCE])))
-    )
-
-    def set_ma(self, _):
-        u = unit(get_angle(get_object(self.pri), 0))
-        f = self._tangent() * u
-        p = get_zero(get_object(self.pri), 0, u)
-        get_object(self.pri).s1.add_mech_action(f, p, 0.)
-        get_object(self.pri).s2.add_mech_action(-f, p, 0.)
-
-
-class PinSlotTangentTorque:
-
-    def __init__(self, pin, f, t):
-        self.pin, self._tangent, self._torque = get_object(pin), f, t
-
-    def set_ma(self, _):
-        u = unit(self.pin.s1.angle + self.pin.a1)
-        f, t = self._tangent() * u, self._torque()
-        p = self.pin.s2.origin + rvec(self.pin.s2.angle, self.pin.p2)
-        self.pin.s1.add_mech_action(f, p, t)
-        self.pin.s2.add_mech_action(-f, p, -t)
-
-    tangent = property(
-        (lambda self: (lambda: self._tangent() / units.SYSTEM[FORCE])),
-        (lambda self, value: setattr(self, '_tangent', (lambda: value() * units.SYSTEM[FORCE])))
-    )
-
-    torque = property(
-        (lambda self: (lambda: self._torque() / units.SYSTEM[FORCE])),
-        (lambda self, value: setattr(self, '_torque', (lambda: value() * units.SYSTEM[FORCE])))
-    )
+import kinepy.objects as obj
+from kinepy.math.geometry import rvec, ZERO_F, ZERO_ARRAY_F
+from kinepy.interface.decorators import physics_input_method, physics_output, FUNCTION_TYPE
+from kinepy.interface.interactions import SolidExternal
+
+
+class Solid(obj.Solid, metaclass=MetaUnit):
+    _object: obj.Solid
+    read_only = ('origin', LENGTH), ('angle', ANGLE)
+    read_write = ('m', MASS), ('g', LENGTH), ('j', INERTIA)
+
+    def __init__(self): # noqa
+        self.external_actions = SolidExternal(self)
+
+    def __repr__(self):
+        return f'{self.rep} | {self._object.name}'
+
+    @physics_output(LENGTH)
+    @physics_input_method(LENGTH)
+    def get_point(self, p):
+        return self._object.origin + rvec(self._object.angle, p)
+
+    @physics_input_method('', LENGTH)
+    def add_force(self, f, p):
+        if isinstance(f, (np.ndarray, tuple, list)) and len(f) == 2:
+            f = np.array(f)
+            if f.shape == (2,):
+                f = f.reshape((2, 1))
+            return *self.external_actions.append((lambda: f * units.SYSTEM[FORCE]), ZERO_F, p), 'force'
+        elif isinstance(f, FUNCTION_TYPE):
+            return *self.external_actions.append((lambda: f() * units.SYSTEM[FORCE]), ZERO_F, p), 'force'
+        raise TypeError("force must be either: ndarray, list, tuple of shape (2,), (2, 1) or (2, n) or a function returning one of these types")
+
+    def add_torque(self, t):
+        if isinstance(t, (int, float, np.ndarray)):
+            return *self.external_actions.append(ZERO_ARRAY_F, (lambda: t * units.SYSTEM[TORQUE]), self._object.g), 'torque'
+        elif isinstance(t, FUNCTION_TYPE):
+            return *self.external_actions.append(ZERO_ARRAY_F, (lambda: t() * units.SYSTEM[TORQUE]), self._object.g), 'torque'
+        raise TypeError("torque must be either: int, float, ndarray of shape (), (1,) or (n,)  or a function returning one of these types")
```

### Comparing `kinepy-0.1.3/kinepy/interface/joints.py` & `kinepy-0.1.4/kinepy/interface/joints.py`

 * *Files identical despite different names*

### Comparing `kinepy-0.1.3/kinepy/interface/metaclass.py` & `kinepy-0.1.4/kinepy/interface/metaclass.py`

 * *Files identical despite different names*

### Comparing `kinepy-0.1.3/kinepy/interface/relations.py` & `kinepy-0.1.4/kinepy/interface/relations.py`

 * *Files identical despite different names*

### Comparing `kinepy-0.1.3/kinepy/interface/system.py` & `kinepy-0.1.4/kinepy/interface/system.py`

 * *Files identical despite different names*

### Comparing `kinepy-0.1.3/kinepy/math/calculus.py` & `kinepy-0.1.4/kinepy/math/calculus.py`

 * *Files identical despite different names*

### Comparing `kinepy-0.1.3/kinepy/math/dynamic.py` & `kinepy-0.1.4/kinepy/math/dynamic.py`

 * *Files identical despite different names*

### Comparing `kinepy-0.1.3/kinepy/math/geometry.py` & `kinepy-0.1.4/kinepy/math/geometry.py`

 * *Files identical despite different names*

### Comparing `kinepy-0.1.3/kinepy/math/kinematic.py` & `kinepy-0.1.4/kinepy/math/kinematic.py`

 * *Files identical despite different names*

### Comparing `kinepy-0.1.3/kinepy/objects/interactions.py` & `kinepy-0.1.4/kinepy/objects/interactions.py`

 * *Files identical despite different names*

### Comparing `kinepy-0.1.3/kinepy/objects/joints.py` & `kinepy-0.1.4/kinepy/objects/joints.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from kinepy.objects.solid import Solid
 from kinepy.math.geometry import np, rotate_eq, move_eq, get_point, rvec, unit, get_angle, get_zero, det, dot, z_cross,\
     ZERO_POINT, ZERO_21
 from kinepy.math.dynamic import trd, tmd
 
 
 class Joint:
-    tag, id_, dof, interaction, inputs, rep = 'Joint', 0, None, None, (), None
+    IDS = GENERIC, REVOLUTE, PRISMATIC, PIN_SLOT, RECTANGULAR = range(5)
+    tag, id_, dof, interaction, inputs, rep = 'Joint', GENERIC, None, None, (), None
     s1: Solid
     s2: Solid
 
     def __init__(self, s1, s2, name):
         self.s1, self.s2, self.name = s1, s2, f'{self.tag}({name})'
 
     def __repr__(self):
@@ -20,15 +21,15 @@
         pass
 
     def input_mode(self):
         return tuple(f'{self.name}: {i}' for i in self.inputs)
 
 
 class RevoluteJoint(Joint):
-    id_, tag, dof, inputs = 1, 'Rev', 1, (ANGLE,)
+    id_, tag, dof, inputs = Joint.REVOLUTE, 'Rev', 1, (ANGLE,)
     force = torque = angle = None
 
     def __init__(self, s1, s2, p1, p2, name):
         Joint.__init__(self, s1, s2, name)
         self.p1, self.p2 = p1, p2
 
     def reset(self, n):
@@ -61,15 +62,15 @@
         self.s2.add_mech_action(ZERO_21, p, -value)
 
     def get_effort(self):
         return self.torque
 
 
 class PrismaticJoint(Joint):
-    id_, tag, dof, inputs = 2, 'Pri', 1, (LENGTH,)
+    id_, tag, dof, inputs = Joint.PRISMATIC, 'Pri', 1, (LENGTH,)
     normal = tangent = torque = sliding = None
 
     def __init__(self, s1, s2, a1, d1, a2, d2, name):
         Joint.__init__(self, s1, s2, name)
         self.a1, self.a2, self.d1, self.d2 = a1, a2, d1, d2
     
     def reset(self, n):
@@ -142,15 +143,15 @@
     d1 = property(lambda self: 0. if isinstance(self.master, RectangularJoint) else self.master.d1)
     a2 = property(lambda self: self.master.a2 - self.master.angle if self.index else self.master.a1)
 
     reset = PrismaticJoint.reset
 
 
 class PinSlotJoint(Joint):
-    id_, tag, dof, inputs = 3, 'PinSlot', 2, (LENGTH, ANGLE)
+    id_, tag, dof, inputs = Joint.PIN_SLOT, 'PinSlot', 2, (LENGTH, ANGLE)
     normal = tangent = torque = sliding = angle = None
 
     def __init__(self, s1, s2, a1, d1, p2, name):
         Joint.__init__(self, s1, s2, name)
         self.p2, self.a1, self.d1 = p2, a1, d1
         self.ghost_sol = Solid(0, 0, (0, 0), f'Ghost-{self.name}')
         self.ghost_j1 = GhostPrismatic(self, 0, f'{self.name}-0')
@@ -188,15 +189,15 @@
         self.sliding = self.ghost_j1.sliding
 
     def dyn_recover_ghosts(self):
         self.normal = self.ghost_j1.normal
 
 
 class RectangularJoint(Joint):
-    id_, tag, dof, inputs = 4, 'Rec', 2, (f'X ({LENGTH})', f'Y ({LENGTH})')
+    id_, tag, dof, inputs = Joint.RECTANGULAR, 'Rec', 2, (f'X ({LENGTH})', f'Y ({LENGTH})')
     torque = sliding = force_x = force_y = None
 
     def __init__(self, s1, s2, angle, a1, a2, p1, p2, name):
         Joint.__init__(self, s1, s2, name)
         self.angle, self.a1, self.a2, self.p1, self.p2 = angle, a1, a2, p1, p2
         self.ghost_sol = Solid(0, 0, (0, 0), f'Ghost-{self.name}')
         self.ghost_j1 = GhostPrismatic(self, 0, f'{self.name}-0')
```

### Comparing `kinepy-0.1.3/kinepy/objects/relations.py` & `kinepy-0.1.4/kinepy/objects/relations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,82 +1,96 @@
 from kinepy.math.dynamic import group_tmd, group_trd, set_force, set_normal
-from kinepy.math.geometry import get_point, sq_mag, z_cross, np, unit, get_angle, dot, get_zero, ZERO_21
-from kinepy.objects.joints import RevoluteJoint, PrismaticJoint
+from kinepy.math.geometry import get_point, sq_mag, z_cross, np, unit, get_angle, dot, get_zero
 
 
-class LinearRelationBase:
+class LinearRelation:
+    IDS = GENERIC, EFFORTLESS, DISTANT, GEAR, GEAR_RACK = range(5)
+    id_ = GENERIC
     v0 = r = j1 = j2 = None
 
+    def __init__(self, j1, j2, r, v0):
+        self.j1, self.j2, self.r, self.v0 = j1, j2, r, v0
+
     def rel_pilot(self, j_index, eq1, eq2):
         v = (self.j1.get_value() * self.r + self.v0) if j_index else (self.j2.get_value() - self.v0) / self.r
         (self.j1, self.j2)[j_index].set_value(v, eq1, eq2)
 
     def rel_block(self, direction, eq0, eq1, ref):
         (self.j1, self.j2)[direction].block(eq0, eq1, ref)
 
 
-class LinearRelation(LinearRelationBase):
-    def __init__(self, j1, j2, r, v0):
-        self.j1, self.j2, self.r, self.v0 = j1, j2, r, v0
-
-
 class EffortlessRelation(LinearRelation):
-    pass
+    id_ = LinearRelation.EFFORTLESS
 
 
 class DistantRelation(LinearRelation):
+    id_ = LinearRelation.DISTANT
+
     def rel_block(self, direction, eq0, eq1, ref):
-        LinearRelationBase.rel_block(self, direction, eq0, eq1, ref)
+        LinearRelation.rel_block(self, direction, eq0, eq1, ref)
         (self.j1, self.j2)[not direction].put_effort((self.j1, self.j2)[direction] * self.r ** (-1, 1)[direction])
 
 
-class GearRelation(LinearRelationBase):
+class GearRelation(LinearRelation):
     common_eq = False, False
     contact_point = contact_force = None
-    tmp = None
 
     def __init__(self, j1, j2, r, v0, pa):
-        self.j1, self.j2, self.r, self.v0 = j1, j2, r, v0
+        LinearRelation.__init__(self, j1, j2, r, v0)
         self.pressure_angle = pa
 
     def _solve_contact(self, direction, radius, vec, contact_point, t_gear):
         n_gear = np.tan(self.pressure_angle) * abs(t_gear) * (1, -1)[(radius > 0)]
         # force applied on the propagated gear
         f_gear = vec * n_gear + z_cross(vec) * t_gear
 
         # add the force to gears
         j1, j2 = ((self.j2, self.j1), (self.j1, self.j2))[direction]
         (j2.s1, j2.s2)[not self.common_eq[direction]].add_mech_action(f_gear, contact_point, 0.)
         (j1.s1, j1.s2)[not self.common_eq[not direction]].add_mech_action(-f_gear, contact_point, 0.)
 
         self.contact_force = f_gear * (1, -1)[direction]
 
+    def get_radii(self):
+        pass
+
 
 class Gear(GearRelation):
+    id_ = LinearRelation.GEAR
+
     def rel_block(self, direction, eq0, eq1, ref):
         eff_r = (self.r, -self.r)[self.common_eq[0] ^ self.common_eq[1]]
         p1, p2 = get_point(self.j1, 0), get_point(self.j2, 0)
         radius = eff_r ** (1, 0)[direction] / (eff_r - 1)
         t_gear = group_tmd((eq0, eq1), (not self.common_eq[direction],), ref, (p1, p2)[direction]) / radius
 
         vec = p2 - p1
         self.contact_point = contact_point = p1 + vec * eff_r / (eff_r - 1)
         self._solve_contact(direction, radius, vec / sq_mag(vec), contact_point, t_gear)
 
         # RevoluteJoint force
         set_force((self.j1, self.j2)[direction], True, group_trd((eq0, eq1), (0,), ref))
 
+    def get_radii(self):
+        eff_r = (self.r, -self.r)[self.common_eq[0] ^ self.common_eq[1]]
+        return abs(eff_r / (eff_r - 1)), abs(1 / (eff_r - 1))
+
 
 class GearRack(GearRelation):
+    id_ = LinearRelation.GEAR_RACK
+
     def rel_block(self, direction, eq0, eq1, ref):
         eff_r = self.r * (1, -1)[self.common_eq[0] ^ self.common_eq[1]]
         v = -z_cross(u := unit(get_angle(self.j2, 0)))
         self.contact_point = contact_point = get_point(self.j1, 0) + v * eff_r
         if not direction:
             t_gear = group_tmd((eq0, eq1), (not self.common_eq[direction],), ref, get_point(self.j1, 0)) / eff_r
             self._solve_contact(direction, eff_r, v, contact_point, t_gear)
             set_force(self.j1, True, group_trd((eq1, eq0), (0,), ref))
         else:
             t_gear = dot(group_trd((eq0, eq1), (not self.common_eq[direction],), ref), u)
             self._solve_contact(direction, -eff_r, v, contact_point, t_gear)
             n_10, m_10 = group_trd((eq0, eq1), (0,), ref), group_tmd((eq0, eq1), (0,), ref, get_zero(self.j2, 0, u))
             set_normal(self.j2, True, n_10, m_10, u)
+
+    def get_radii(self):
+        return abs(self.r), None
```

### Comparing `kinepy-0.1.3/kinepy/objects/solid.py` & `kinepy-0.1.4/kinepy/objects/solid.py`

 * *Files identical despite different names*

### Comparing `kinepy-0.1.3/kinepy/objects/system.py` & `kinepy-0.1.4/kinepy/objects/system.py`

 * *Files identical despite different names*

### Comparing `kinepy-0.1.3/kinepy/tools.py` & `kinepy-0.1.4/kinepy/tools.py`

 * *Files identical despite different names*

### Comparing `kinepy-0.1.3/kinepy/units.py` & `kinepy-0.1.4/kinepy/units.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,27 +214,30 @@
 
 
 def set_unit(phy, value, unit='Unnamed unit'):
     if isinstance(value, tuple):
         value, unit = value
     SYSTEM.set(phy, value, unit)
     
-def get_unit(phy):
-    return SYSTEM.dct[phy][1]
-
-def get_value(phy):
-    return SYSTEM.dct[phy][0]
 
 set_unit.__doc__ = f"""Changes the unit
 phy is the physical quantity among {', '.join(PHYSICAL_QUANTITIES)}
 value is hom much of the SI unit your unit is: ex. 1 mm is 0.001 m so value is 0.001
 name is the name of your unit.
 You can use units imported from units.py"""
 
 
+def get_unit(phy):
+    return SYSTEM.dct[phy][1]
+
+
+def get_value(phy):
+    return SYSTEM.dct[phy][0]
+
+
 def set_unit_system(unit_system: dict):
     """
     Replaces every unit of the global unit system with the units described in unit_system.
     Missing units will be unchanged.
     
     Available systems:
     DEFAULT_SYSTEM, SI, AMERICAN_SYSTEM, GOAT_SYSTEM
```

### Comparing `kinepy-0.1.3/kinepy.egg-info/PKG-INFO` & `kinepy-0.1.4/kinepy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kinepy
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python library dedicated to plane mechanism simulation
 Home-page: https://github.com/valentin-burillier/kinepy
 Author: Loïc Chevalier - Valentin Burillier
 Keywords: robotics,simulation,dynamics,kinematics,statics,inverse-kinematics,mechanism
 Requires: numpy
 Requires: matplotlib
 Requires: pygame
```

### Comparing `kinepy-0.1.3/kinepy.egg-info/SOURCES.txt` & `kinepy-0.1.4/kinepy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 kinepy/__init__.py
 kinepy/tools.py
 kinepy/units.py
 kinepy.egg-info/PKG-INFO
 kinepy.egg-info/SOURCES.txt
 kinepy.egg-info/dependency_links.txt
+kinepy.egg-info/requires.txt
 kinepy.egg-info/top_level.txt
 kinepy/compilation/__init__.py
 kinepy/compilation/graph_operations.py
 kinepy/compilation/graphs.py
 kinepy/compilation/preparation.py
 kinepy/gui/Rect.py
 kinepy/gui/__init__.py
```

### Comparing `kinepy-0.1.3/setup.py` & `kinepy-0.1.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 
 
 setup(
     name='kinepy',
     packages=[
         'kinepy', 'kinepy.interface', 'kinepy.gui', 'kinepy.objects', 'kinepy.math', 'kinepy.compilation'
     ],
-    version='0.1.3',
+    version='0.1.4',
     description='Python library dedicated to plane mechanism simulation',
     author='Loïc Chevalier - Valentin Burillier',
     url='https://github.com/valentin-burillier/kinepy',
     requires=['numpy', 'matplotlib', 'pygame'],
+    install_requires=['numpy', 'matplotlib', 'pygame'],
     keywords=['robotics', 'simulation', 'dynamics', 'kinematics', 'statics', 'inverse-kinematics', 'mechanism'],
     package_data={'kinepy.gui': ['logo.ico']},
     long_description=long_desc,
     long_description_content_type='text/markdown'
 )
```

