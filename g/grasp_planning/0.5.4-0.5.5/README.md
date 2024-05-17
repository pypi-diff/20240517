# Comparing `tmp/grasp_planning-0.5.4.tar.gz` & `tmp/grasp_planning-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grasp_planning-0.5.4.tar", max compression
+gzip compressed data, was "grasp_planning-0.5.5.tar", max compression
```

## Comparing `grasp_planning-0.5.4.tar` & `grasp_planning-0.5.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1677 2024-05-15 15:06:33.607404 grasp_planning-0.5.4/README.md
--rw-r--r--   0        0        0      175 2024-05-15 09:11:31.290902 grasp_planning-0.5.4/grasp_planning/__init__.py
--rw-r--r--   0        0        0      888 2024-05-13 14:27:19.884831 grasp_planning-0.5.4/grasp_planning/constraints/collision_constraint.py
--rw-r--r--   0        0        0      226 2024-05-13 12:54:20.897417 grasp_planning-0.5.4/grasp_planning/constraints/constraint_template.py
--rw-r--r--   0        0        0      375 2024-05-15 09:08:01.061356 grasp_planning-0.5.4/grasp_planning/constraints/constraints.py
--rw-r--r--   0        0        0     1057 2024-05-13 12:38:19.452308 grasp_planning-0.5.4/grasp_planning/constraints/grasp_pos_constraint.py
--rw-r--r--   0        0        0     1334 2024-05-13 13:10:00.135267 grasp_planning-0.5.4/grasp_planning/constraints/grasp_rot_constraint.py
--rw-r--r--   0        0        0     1059 2024-05-09 15:55:53.313730 grasp_planning-0.5.4/grasp_planning/constraints/manipulation_constraint.py
--rw-r--r--   0        0        0     1071 2024-05-15 09:07:33.253161 grasp_planning-0.5.4/grasp_planning/constraints/orientation_constraint.py
--rw-r--r--   0        0        0     1023 2024-05-15 09:03:10.755469 grasp_planning-0.5.4/grasp_planning/constraints/position_constraint.py
--rw-r--r--   0        0        0      120 2024-05-15 08:53:23.992220 grasp_planning-0.5.4/grasp_planning/cost/costs.py
--rw-r--r--   0        0        0      424 2024-05-15 08:53:06.312040 grasp_planning-0.5.4/grasp_planning/cost/dist_to_home.py
--rw-r--r--   0        0        0     1439 2024-05-13 08:29:45.664854 grasp_planning-0.5.4/grasp_planning/cost/squared_acc_cost.py
--rw-r--r--   0        0        0     7603 2024-05-15 08:38:17.450744 grasp_planning-0.5.4/grasp_planning/solver/gomp_planner.py
--rw-r--r--   0        0        0     5326 2024-05-15 09:24:17.669132 grasp_planning-0.5.4/grasp_planning/solver/ik_optim.py
--rw-r--r--   0        0        0     1992 2024-05-15 08:35:25.352819 grasp_planning-0.5.4/grasp_planning/solver/robot_model.py
--rw-r--r--   0        0        0      555 2024-05-16 08:41:18.559634 grasp_planning-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 grasp_planning-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1734 2024-05-16 09:02:48.947350 grasp_planning-0.5.5/README.md
+-rw-r--r--   0        0        0      175 2024-05-15 09:11:31.290902 grasp_planning-0.5.5/grasp_planning/__init__.py
+-rw-r--r--   0        0        0      888 2024-05-13 14:27:19.884831 grasp_planning-0.5.5/grasp_planning/constraints/collision_constraint.py
+-rw-r--r--   0        0        0      226 2024-05-13 12:54:20.897417 grasp_planning-0.5.5/grasp_planning/constraints/constraint_template.py
+-rw-r--r--   0        0        0      375 2024-05-15 09:08:01.061356 grasp_planning-0.5.5/grasp_planning/constraints/constraints.py
+-rw-r--r--   0        0        0     1057 2024-05-13 12:38:19.452308 grasp_planning-0.5.5/grasp_planning/constraints/grasp_pos_constraint.py
+-rw-r--r--   0        0        0     1334 2024-05-13 13:10:00.135267 grasp_planning-0.5.5/grasp_planning/constraints/grasp_rot_constraint.py
+-rw-r--r--   0        0        0     1059 2024-05-09 15:55:53.313730 grasp_planning-0.5.5/grasp_planning/constraints/manipulation_constraint.py
+-rw-r--r--   0        0        0     1071 2024-05-15 09:07:33.253161 grasp_planning-0.5.5/grasp_planning/constraints/orientation_constraint.py
+-rw-r--r--   0        0        0     1023 2024-05-15 09:03:10.755469 grasp_planning-0.5.5/grasp_planning/constraints/position_constraint.py
+-rw-r--r--   0        0        0      120 2024-05-15 08:53:23.992220 grasp_planning-0.5.5/grasp_planning/cost/costs.py
+-rw-r--r--   0        0        0      424 2024-05-15 08:53:06.312040 grasp_planning-0.5.5/grasp_planning/cost/dist_to_home.py
+-rw-r--r--   0        0        0     1439 2024-05-13 08:29:45.664854 grasp_planning-0.5.5/grasp_planning/cost/squared_acc_cost.py
+-rw-r--r--   0        0        0     7746 2024-05-17 08:13:16.425722 grasp_planning-0.5.5/grasp_planning/solver/gomp_planner.py
+-rw-r--r--   0        0        0     5326 2024-05-15 09:24:17.669132 grasp_planning-0.5.5/grasp_planning/solver/ik_optim.py
+-rw-r--r--   0        0        0     1992 2024-05-15 08:35:25.352819 grasp_planning-0.5.5/grasp_planning/solver/robot_model.py
+-rw-r--r--   0        0        0      555 2024-05-17 08:15:57.652051 grasp_planning-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 grasp_planning-0.5.5/PKG-INFO
```

### Comparing `grasp_planning-0.5.4/README.md` & `grasp_planning-0.5.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 This package provides grasp and motion planning using CasADi and IPOPT. 
 
+## Installation
+```bash
+pip3 install grasp_planning
+```
+
 
 ## Usage
 ```python
 from grasp_planning import GOMP
 import numpy as np
 import time
 import os
```

### Comparing `grasp_planning-0.5.4/grasp_planning/constraints/collision_constraint.py` & `grasp_planning-0.5.5/grasp_planning/constraints/collision_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.4/grasp_planning/constraints/grasp_pos_constraint.py` & `grasp_planning-0.5.5/grasp_planning/constraints/grasp_pos_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.4/grasp_planning/constraints/grasp_rot_constraint.py` & `grasp_planning-0.5.5/grasp_planning/constraints/grasp_rot_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.4/grasp_planning/constraints/manipulation_constraint.py` & `grasp_planning-0.5.5/grasp_planning/constraints/manipulation_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.4/grasp_planning/constraints/orientation_constraint.py` & `grasp_planning-0.5.5/grasp_planning/constraints/orientation_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.4/grasp_planning/constraints/position_constraint.py` & `grasp_planning-0.5.5/grasp_planning/constraints/position_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.4/grasp_planning/cost/squared_acc_cost.py` & `grasp_planning-0.5.5/grasp_planning/cost/squared_acc_cost.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.4/grasp_planning/solver/gomp_planner.py` & `grasp_planning-0.5.5/grasp_planning/solver/gomp_planner.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 import spatial_casadi as sc
 from scipy.spatial.transform import Rotation as R
 from grasp_planning.solver.robot_model import RobotKinematicModel
 from grasp_planning.cost.costs import SquaredAccCost
 from grasp_planning.constraints.constraints import *
 
 class GOMP():
-    def __init__(self, n_waypoints, urdf, theta=np.pi/4, root_link='world', end_link='tool_frame') -> None:
+    def __init__(self, n_waypoints, urdf, theta=np.pi/4, roll_obj_grasp = np.pi, root_link='world', end_link='tool_frame') -> None:
         # Init variables
         self.T_W_Grasp = None
         self.T_W_Obj = None
         self.T_Obj_Grasp = np.eye(4, dtype=float)
         
         # Kinematics
         self._robot_model = RobotKinematicModel(urdf, root_link, end_link)
         self.n_dofs = self._robot_model.n_dofs
         self.manipulation_frame_dim = 6
         self.x_dim = self.n_dofs
         self.n_waypoints = n_waypoints
         self.theta = theta
+        self.roll_obj_grasp = roll_obj_grasp
         
         # Optimization
         self.x = ca.SX.sym("x", self.x_dim, self.n_waypoints)
         self.x_init = None
         
         self._objective = None
         self.l_joint_limits, self.u_joint_limits = None, None
@@ -39,18 +40,18 @@
     def update_grasp_DOF(self, theta: float, degrees=True) -> None:
         """
         Object has to have z-axis aligned with the world frame
         """
         self.T_Obj_Grasp = np.eye(4, dtype=float)
         if degrees:
             self.theta = np.deg2rad(theta)
-            self.R_Obj_Grasp = R.from_euler('xyz', [180, 0, self.theta], degrees=True).as_matrix()
+            self.R_Obj_Grasp = R.from_euler('xyz', [np.rad2deg(self.roll_obj_grasp), 0, self.theta], degrees=True).as_matrix()
         else:
             self.theta = theta
-            self.R_Obj_Grasp = R.from_euler('xyz', [np.pi, 0, self.theta], degrees=False).as_matrix()
+            self.R_Obj_Grasp = R.from_euler('xyz', [self.roll_obj_grasp, 0, self.theta], degrees=False).as_matrix()
         self.T_Obj_Grasp[:3,:3] = self.R_Obj_Grasp
         self.T_W_Grasp = self.T_W_Obj @ self.T_Obj_Grasp
         
         # print("T_W_Grasp\n", self.T_W_Grasp)
 
 
     def update_object_pose(self, T_W_Obj: np.array) -> None:
@@ -154,17 +155,17 @@
         self.g_list.append(GraspRotConstraint(self._robot_model, 
                                               self.x, 
                                               waypoint_ID, 
                                               self.param_grasp_ca, 
                                               self.theta, 
                                               tolerance))
 
-    def add_grasp_constraint(self, waypoint_ID, tolerance=0.0):
-        self._add_grasp_pos_constraint(waypoint_ID, tolerance)
-        self._add_grasp_rot_constraint(waypoint_ID, tolerance)
+    def add_grasp_constraint(self, waypoint_ID, pos_tolerance=0.0, rot_tolerance=0.01):
+        self._add_grasp_pos_constraint(waypoint_ID, pos_tolerance)
+        self._add_grasp_rot_constraint(waypoint_ID, rot_tolerance)
         self.param_ca_list.append(self.param_grasp_ca)
 
     def add_collision_constraint(self, waypoint_ID, child_link, r_link=0.5, r_obst=0.2, tolerance=0.01):
         self._collision_flag = True
         self.g_list.append(CollisionConstraint(robot=self._robot_model,
                                                 q_ca=self.x,
                                                 waypoint_ID=waypoint_ID,
```

### Comparing `grasp_planning-0.5.4/grasp_planning/solver/ik_optim.py` & `grasp_planning-0.5.5/grasp_planning/solver/ik_optim.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.4/grasp_planning/solver/robot_model.py` & `grasp_planning-0.5.5/grasp_planning/solver/robot_model.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.4/pyproject.toml` & `grasp_planning-0.5.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grasp_planning"
-version = "0.5.4"
+version = "0.5.5"
 description = "\"Grasp and Motion Planning Python Package.\""
 authors = ["Tomas Merva <tmerva7@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/TomasMerva/gomp.git"
 repository = "https://github.com/TomasMerva/gomp.git"
```

### Comparing `grasp_planning-0.5.4/PKG-INFO` & `grasp_planning-0.5.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grasp_planning
-Version: 0.5.4
+Version: 0.5.5
 Summary: "Grasp and Motion Planning Python Package."
 Home-page: https://github.com/TomasMerva/gomp.git
 License: MIT
 Author: Tomas Merva
 Author-email: tmerva7@gmail.com
 Requires-Python: >=3.8,<3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,19 @@
 Requires-Dist: scipy (<=1.10.1)
 Requires-Dist: spatial-casadi (>=1.1.0,<2.0.0)
 Project-URL: Repository, https://github.com/TomasMerva/gomp.git
 Description-Content-Type: text/markdown
 
 This package provides grasp and motion planning using CasADi and IPOPT. 
 
+## Installation
+```bash
+pip3 install grasp_planning
+```
+
 
 ## Usage
 ```python
 from grasp_planning import GOMP
 import numpy as np
 import time
 import os
```

