# Comparing `tmp/grasp_planning-0.5.6.tar.gz` & `tmp/grasp_planning-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grasp_planning-0.5.6.tar", max compression
+gzip compressed data, was "grasp_planning-0.5.7.tar", max compression
```

## Comparing `grasp_planning-0.5.6.tar` & `grasp_planning-0.5.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1734 2024-05-16 09:02:48.947350 grasp_planning-0.5.6/README.md
--rw-r--r--   0        0        0      175 2024-05-15 09:11:31.290902 grasp_planning-0.5.6/grasp_planning/__init__.py
--rw-r--r--   0        0        0      888 2024-05-13 14:27:19.884831 grasp_planning-0.5.6/grasp_planning/constraints/collision_constraint.py
--rw-r--r--   0        0        0      226 2024-05-13 12:54:20.897417 grasp_planning-0.5.6/grasp_planning/constraints/constraint_template.py
--rw-r--r--   0        0        0      375 2024-05-15 09:08:01.061356 grasp_planning-0.5.6/grasp_planning/constraints/constraints.py
--rw-r--r--   0        0        0     1057 2024-05-13 12:38:19.452308 grasp_planning-0.5.6/grasp_planning/constraints/grasp_pos_constraint.py
--rw-r--r--   0        0        0     1334 2024-05-13 13:10:00.135267 grasp_planning-0.5.6/grasp_planning/constraints/grasp_rot_constraint.py
--rw-r--r--   0        0        0     1059 2024-05-09 15:55:53.313730 grasp_planning-0.5.6/grasp_planning/constraints/manipulation_constraint.py
--rw-r--r--   0        0        0     1071 2024-05-15 09:07:33.253161 grasp_planning-0.5.6/grasp_planning/constraints/orientation_constraint.py
--rw-r--r--   0        0        0     1023 2024-05-15 09:03:10.755469 grasp_planning-0.5.6/grasp_planning/constraints/position_constraint.py
--rw-r--r--   0        0        0      120 2024-05-15 08:53:23.992220 grasp_planning-0.5.6/grasp_planning/cost/costs.py
--rw-r--r--   0        0        0      424 2024-05-15 08:53:06.312040 grasp_planning-0.5.6/grasp_planning/cost/dist_to_home.py
--rw-r--r--   0        0        0     1439 2024-05-13 08:29:45.664854 grasp_planning-0.5.6/grasp_planning/cost/squared_acc_cost.py
--rw-r--r--   0        0        0     7734 2024-05-17 15:33:11.689460 grasp_planning-0.5.6/grasp_planning/solver/gomp_planner.py
--rw-r--r--   0        0        0     5326 2024-05-15 09:24:17.669132 grasp_planning-0.5.6/grasp_planning/solver/ik_optim.py
--rw-r--r--   0        0        0     1992 2024-05-15 08:35:25.352819 grasp_planning-0.5.6/grasp_planning/solver/robot_model.py
--rw-r--r--   0        0        0      555 2024-05-17 15:33:23.057539 grasp_planning-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 grasp_planning-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1734 2024-05-16 09:02:48.947350 grasp_planning-0.5.7/README.md
+-rw-r--r--   0        0        0      175 2024-05-15 09:11:31.290902 grasp_planning-0.5.7/grasp_planning/__init__.py
+-rw-r--r--   0        0        0      888 2024-05-13 14:27:19.884831 grasp_planning-0.5.7/grasp_planning/constraints/collision_constraint.py
+-rw-r--r--   0        0        0      226 2024-05-13 12:54:20.897417 grasp_planning-0.5.7/grasp_planning/constraints/constraint_template.py
+-rw-r--r--   0        0        0      375 2024-05-15 09:08:01.061356 grasp_planning-0.5.7/grasp_planning/constraints/constraints.py
+-rw-r--r--   0        0        0     1057 2024-05-13 12:38:19.452308 grasp_planning-0.5.7/grasp_planning/constraints/grasp_pos_constraint.py
+-rw-r--r--   0        0        0     1334 2024-05-13 13:10:00.135267 grasp_planning-0.5.7/grasp_planning/constraints/grasp_rot_constraint.py
+-rw-r--r--   0        0        0     1059 2024-05-09 15:55:53.313730 grasp_planning-0.5.7/grasp_planning/constraints/manipulation_constraint.py
+-rw-r--r--   0        0        0     1071 2024-05-15 09:07:33.253161 grasp_planning-0.5.7/grasp_planning/constraints/orientation_constraint.py
+-rw-r--r--   0        0        0     1023 2024-05-15 09:03:10.755469 grasp_planning-0.5.7/grasp_planning/constraints/position_constraint.py
+-rw-r--r--   0        0        0      120 2024-05-15 08:53:23.992220 grasp_planning-0.5.7/grasp_planning/cost/costs.py
+-rw-r--r--   0        0        0      424 2024-05-15 08:53:06.312040 grasp_planning-0.5.7/grasp_planning/cost/dist_to_home.py
+-rw-r--r--   0        0        0     1439 2024-05-13 08:29:45.664854 grasp_planning-0.5.7/grasp_planning/cost/squared_acc_cost.py
+-rw-r--r--   0        0        0     7732 2024-05-17 15:38:35.947749 grasp_planning-0.5.7/grasp_planning/solver/gomp_planner.py
+-rw-r--r--   0        0        0     5326 2024-05-15 09:24:17.669132 grasp_planning-0.5.7/grasp_planning/solver/ik_optim.py
+-rw-r--r--   0        0        0     1992 2024-05-15 08:35:25.352819 grasp_planning-0.5.7/grasp_planning/solver/robot_model.py
+-rw-r--r--   0        0        0      555 2024-05-17 15:38:42.943799 grasp_planning-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 grasp_planning-0.5.7/PKG-INFO
```

### Comparing `grasp_planning-0.5.6/README.md` & `grasp_planning-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.6/grasp_planning/constraints/collision_constraint.py` & `grasp_planning-0.5.7/grasp_planning/constraints/collision_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.6/grasp_planning/constraints/grasp_pos_constraint.py` & `grasp_planning-0.5.7/grasp_planning/constraints/grasp_pos_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.6/grasp_planning/constraints/grasp_rot_constraint.py` & `grasp_planning-0.5.7/grasp_planning/constraints/grasp_rot_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.6/grasp_planning/constraints/manipulation_constraint.py` & `grasp_planning-0.5.7/grasp_planning/constraints/manipulation_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.6/grasp_planning/constraints/orientation_constraint.py` & `grasp_planning-0.5.7/grasp_planning/constraints/orientation_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.6/grasp_planning/constraints/position_constraint.py` & `grasp_planning-0.5.7/grasp_planning/constraints/position_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.6/grasp_planning/cost/squared_acc_cost.py` & `grasp_planning-0.5.7/grasp_planning/cost/squared_acc_cost.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.6/grasp_planning/solver/gomp_planner.py` & `grasp_planning-0.5.7/grasp_planning/solver/gomp_planner.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,18 +40,18 @@
     def update_grasp_DOF(self, theta: float, degrees=True) -> None:
         """
         Object has to have z-axis aligned with the world frame
         """
         self.T_Obj_Grasp = np.eye(4, dtype=float)
         if degrees:
             self.theta = np.deg2rad(theta)
-            self.R_Obj_Grasp = R.from_euler('xyz', [0, np.rad2deg(self.roll_obj_grasp), 180], degrees=True).as_matrix()
+            self.R_Obj_Grasp = R.from_euler('xyz', [0, np.rad2deg(self.roll_obj_grasp), 0.0], degrees=True).as_matrix()
         else:
             self.theta = theta
-            self.R_Obj_Grasp = R.from_euler('xyz', [0, self.roll_obj_grasp, np.pi], degrees=False).as_matrix()
+            self.R_Obj_Grasp = R.from_euler('xyz', [0, self.roll_obj_grasp, 0.0], degrees=False).as_matrix()
         self.T_Obj_Grasp[:3,:3] = self.R_Obj_Grasp
         self.T_W_Grasp = self.T_W_Obj @ self.T_Obj_Grasp
         
         # print("T_W_Grasp\n", self.T_W_Grasp)
 
 
     def update_object_pose(self, T_W_Obj: np.array) -> None:
```

### Comparing `grasp_planning-0.5.6/grasp_planning/solver/ik_optim.py` & `grasp_planning-0.5.7/grasp_planning/solver/ik_optim.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.6/grasp_planning/solver/robot_model.py` & `grasp_planning-0.5.7/grasp_planning/solver/robot_model.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.6/pyproject.toml` & `grasp_planning-0.5.7/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grasp_planning"
-version = "0.5.6"
+version = "0.5.7"
 description = "\"Grasp and Motion Planning Python Package.\""
 authors = ["Tomas Merva <tmerva7@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/TomasMerva/gomp.git"
 repository = "https://github.com/TomasMerva/gomp.git"
```

### Comparing `grasp_planning-0.5.6/PKG-INFO` & `grasp_planning-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grasp_planning
-Version: 0.5.6
+Version: 0.5.7
 Summary: "Grasp and Motion Planning Python Package."
 Home-page: https://github.com/TomasMerva/gomp.git
 License: MIT
 Author: Tomas Merva
 Author-email: tmerva7@gmail.com
 Requires-Python: >=3.8,<3.10
 Classifier: License :: OSI Approved :: MIT License
```

