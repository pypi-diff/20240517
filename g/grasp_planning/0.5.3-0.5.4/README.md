# Comparing `tmp/grasp_planning-0.5.3.tar.gz` & `tmp/grasp_planning-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grasp_planning-0.5.3.tar", max compression
+gzip compressed data, was "grasp_planning-0.5.4.tar", max compression
```

## Comparing `grasp_planning-0.5.3.tar` & `grasp_planning-0.5.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1940 2024-05-15 08:31:46.546248 grasp_planning-0.5.3/README.md
--rw-r--r--   0        0        0      175 2024-05-15 09:11:31.290902 grasp_planning-0.5.3/grasp_planning/__init__.py
--rw-r--r--   0        0        0      888 2024-05-13 14:27:19.884831 grasp_planning-0.5.3/grasp_planning/constraints/collision_constraint.py
--rw-r--r--   0        0        0      226 2024-05-13 12:54:20.897417 grasp_planning-0.5.3/grasp_planning/constraints/constraint_template.py
--rw-r--r--   0        0        0      375 2024-05-15 09:08:01.061356 grasp_planning-0.5.3/grasp_planning/constraints/constraints.py
--rw-r--r--   0        0        0     1057 2024-05-13 12:38:19.452308 grasp_planning-0.5.3/grasp_planning/constraints/grasp_pos_constraint.py
--rw-r--r--   0        0        0     1334 2024-05-13 13:10:00.135267 grasp_planning-0.5.3/grasp_planning/constraints/grasp_rot_constraint.py
--rw-r--r--   0        0        0     1059 2024-05-09 15:55:53.313730 grasp_planning-0.5.3/grasp_planning/constraints/manipulation_constraint.py
--rw-r--r--   0        0        0     1071 2024-05-15 09:07:33.253161 grasp_planning-0.5.3/grasp_planning/constraints/orientation_constraint.py
--rw-r--r--   0        0        0     1023 2024-05-15 09:03:10.755469 grasp_planning-0.5.3/grasp_planning/constraints/position_constraint.py
--rw-r--r--   0        0        0      120 2024-05-15 08:53:23.992220 grasp_planning-0.5.3/grasp_planning/cost/costs.py
--rw-r--r--   0        0        0      424 2024-05-15 08:53:06.312040 grasp_planning-0.5.3/grasp_planning/cost/dist_to_home.py
--rw-r--r--   0        0        0     1439 2024-05-13 08:29:45.664854 grasp_planning-0.5.3/grasp_planning/cost/squared_acc_cost.py
--rw-r--r--   0        0        0     7603 2024-05-15 08:38:17.450744 grasp_planning-0.5.3/grasp_planning/solver/gomp_planner.py
--rw-r--r--   0        0        0     5326 2024-05-15 09:24:17.669132 grasp_planning-0.5.3/grasp_planning/solver/ik_optim.py
--rw-r--r--   0        0        0     1992 2024-05-15 08:35:25.352819 grasp_planning-0.5.3/grasp_planning/solver/robot_model.py
--rw-r--r--   0        0        0      555 2024-05-15 09:29:35.627838 grasp_planning-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     2696 1970-01-01 00:00:00.000000 grasp_planning-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1677 2024-05-15 15:06:33.607404 grasp_planning-0.5.4/README.md
+-rw-r--r--   0        0        0      175 2024-05-15 09:11:31.290902 grasp_planning-0.5.4/grasp_planning/__init__.py
+-rw-r--r--   0        0        0      888 2024-05-13 14:27:19.884831 grasp_planning-0.5.4/grasp_planning/constraints/collision_constraint.py
+-rw-r--r--   0        0        0      226 2024-05-13 12:54:20.897417 grasp_planning-0.5.4/grasp_planning/constraints/constraint_template.py
+-rw-r--r--   0        0        0      375 2024-05-15 09:08:01.061356 grasp_planning-0.5.4/grasp_planning/constraints/constraints.py
+-rw-r--r--   0        0        0     1057 2024-05-13 12:38:19.452308 grasp_planning-0.5.4/grasp_planning/constraints/grasp_pos_constraint.py
+-rw-r--r--   0        0        0     1334 2024-05-13 13:10:00.135267 grasp_planning-0.5.4/grasp_planning/constraints/grasp_rot_constraint.py
+-rw-r--r--   0        0        0     1059 2024-05-09 15:55:53.313730 grasp_planning-0.5.4/grasp_planning/constraints/manipulation_constraint.py
+-rw-r--r--   0        0        0     1071 2024-05-15 09:07:33.253161 grasp_planning-0.5.4/grasp_planning/constraints/orientation_constraint.py
+-rw-r--r--   0        0        0     1023 2024-05-15 09:03:10.755469 grasp_planning-0.5.4/grasp_planning/constraints/position_constraint.py
+-rw-r--r--   0        0        0      120 2024-05-15 08:53:23.992220 grasp_planning-0.5.4/grasp_planning/cost/costs.py
+-rw-r--r--   0        0        0      424 2024-05-15 08:53:06.312040 grasp_planning-0.5.4/grasp_planning/cost/dist_to_home.py
+-rw-r--r--   0        0        0     1439 2024-05-13 08:29:45.664854 grasp_planning-0.5.4/grasp_planning/cost/squared_acc_cost.py
+-rw-r--r--   0        0        0     7603 2024-05-15 08:38:17.450744 grasp_planning-0.5.4/grasp_planning/solver/gomp_planner.py
+-rw-r--r--   0        0        0     5326 2024-05-15 09:24:17.669132 grasp_planning-0.5.4/grasp_planning/solver/ik_optim.py
+-rw-r--r--   0        0        0     1992 2024-05-15 08:35:25.352819 grasp_planning-0.5.4/grasp_planning/solver/robot_model.py
+-rw-r--r--   0        0        0      555 2024-05-16 08:41:18.559634 grasp_planning-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 grasp_planning-0.5.4/PKG-INFO
```

### Comparing `grasp_planning-0.5.3/README.md` & `grasp_planning-0.5.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -43,15 +43,7 @@
 planner.update_constraints_params(T_W_Obj, T_W_Obst)
 x, solver_flag = planner.solve()
 end = time.time()
 print(f"Computational time: {end-start}" )
 print(f"Solver status: {solver_flag}" )
 ```
 
-## ToDo
-- [ ] removing constraints
-- [ ] automatic constraints for collisions
-
-1. zacni riesit to ze nejde mi parametre
-
-- trebalo poriesit ze kazde zavolanie add collision vytvori premennu pre obstacle
-- idealne poriesit aby sa zadaval aj parent link pre koliziu
```

### Comparing `grasp_planning-0.5.3/grasp_planning/constraints/collision_constraint.py` & `grasp_planning-0.5.4/grasp_planning/constraints/collision_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.3/grasp_planning/constraints/grasp_pos_constraint.py` & `grasp_planning-0.5.4/grasp_planning/constraints/grasp_pos_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.3/grasp_planning/constraints/grasp_rot_constraint.py` & `grasp_planning-0.5.4/grasp_planning/constraints/grasp_rot_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.3/grasp_planning/constraints/manipulation_constraint.py` & `grasp_planning-0.5.4/grasp_planning/constraints/manipulation_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.3/grasp_planning/constraints/orientation_constraint.py` & `grasp_planning-0.5.4/grasp_planning/constraints/orientation_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.3/grasp_planning/constraints/position_constraint.py` & `grasp_planning-0.5.4/grasp_planning/constraints/position_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.3/grasp_planning/cost/squared_acc_cost.py` & `grasp_planning-0.5.4/grasp_planning/cost/squared_acc_cost.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.3/grasp_planning/solver/gomp_planner.py` & `grasp_planning-0.5.4/grasp_planning/solver/gomp_planner.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.3/grasp_planning/solver/ik_optim.py` & `grasp_planning-0.5.4/grasp_planning/solver/ik_optim.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.3/grasp_planning/solver/robot_model.py` & `grasp_planning-0.5.4/grasp_planning/solver/robot_model.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.3/pyproject.toml` & `grasp_planning-0.5.4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "grasp_planning"
-version = "0.5.3"
+version = "0.5.4"
 description = "\"Grasp and Motion Planning Python Package.\""
 authors = ["Tomas Merva <tmerva7@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/TomasMerva/gomp.git"
 repository = "https://github.com/TomasMerva/gomp.git"
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.10"
 casadi = "^3.6"
 numpy = "^1.15.3"
-forwardkinematics = ">=1.1.3"
+forwardkinematics = ">=1.2.0"
 spatial-casadi="^1.1.0"
 scipy="<=1.10.1"
 
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `grasp_planning-0.5.3/PKG-INFO` & `grasp_planning-0.5.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: grasp_planning
-Version: 0.5.3
+Version: 0.5.4
 Summary: "Grasp and Motion Planning Python Package."
 Home-page: https://github.com/TomasMerva/gomp.git
 License: MIT
 Author: Tomas Merva
 Author-email: tmerva7@gmail.com
 Requires-Python: >=3.8,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: casadi (>=3.6,<4.0)
-Requires-Dist: forwardkinematics (>=1.1.3)
+Requires-Dist: forwardkinematics (>=1.2.0)
 Requires-Dist: numpy (>=1.15.3,<2.0.0)
 Requires-Dist: scipy (<=1.10.1)
 Requires-Dist: spatial-casadi (>=1.1.0,<2.0.0)
 Project-URL: Repository, https://github.com/TomasMerva/gomp.git
 Description-Content-Type: text/markdown
 
 This package provides grasp and motion planning using CasADi and IPOPT. 
@@ -64,15 +64,8 @@
 planner.update_constraints_params(T_W_Obj, T_W_Obst)
 x, solver_flag = planner.solve()
 end = time.time()
 print(f"Computational time: {end-start}" )
 print(f"Solver status: {solver_flag}" )
 ```
 
-## ToDo
-- [ ] removing constraints
-- [ ] automatic constraints for collisions
 
-1. zacni riesit to ze nejde mi parametre
-
-- trebalo poriesit ze kazde zavolanie add collision vytvori premennu pre obstacle
-- idealne poriesit aby sa zadaval aj parent link pre koliziu
```

