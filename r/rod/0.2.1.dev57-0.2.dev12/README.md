# Comparing `tmp/rod-0.2.1.dev57.tar.gz` & `tmp/rod-0.2.dev12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rod-0.2.1.dev57.tar", last modified: Fri May 17 20:06:40 2024, max compression
+gzip compressed data, was "rod-0.2.dev12.tar", last modified: Fri Mar  8 14:31:49 2024, max compression
```

## Comparing `rod-0.2.1.dev57.tar` & `rod-0.2.dev12.tar`

### file list

```diff
@@ -1,65 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:06:40.440779 rod-0.2.1.dev57/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:06:40.428779 rod-0.2.1.dev57/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:06:40.432779 rod-0.2.1.dev57/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/.github/workflows/ci_cd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-05-17 20:06:40.440779 rod-0.2.1.dev57/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8124 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-17 20:06:40.440779 rod-0.2.1.dev57/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:06:40.428779 rod-0.2.1.dev57/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:06:40.432779 rod-0.2.1.dev57/src/rod/
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:06:40.436779 rod-0.2.1.dev57/src/rod/builder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/builder/primitive_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/builder/primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:06:40.436779 rod-0.2.1.dev57/src/rod/kinematics/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/kinematics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13778 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/kinematics/kinematic_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/kinematics/tree_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/pretty_printer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:06:40.436779 rod-0.2.1.dev57/src/rod/sdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/sdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/sdf/collision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/sdf/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/sdf/element.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/sdf/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/sdf/joint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/sdf/link.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/sdf/material.py
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/sdf/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/sdf/physics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/sdf/scene.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/sdf/sdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/sdf/visual.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/sdf/world.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:06:40.436779 rod-0.2.1.dev57/src/rod/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/tree/directed_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/tree/tree_elements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:06:40.436779 rod-0.2.1.dev57/src/rod/urdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/urdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19726 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/urdf/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:06:40.440779 rod-0.2.1.dev57/src/rod/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12313 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/utils/frame_convention.py
--rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/utils/gazebo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/utils/resolve_frames.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/src/rod/utils/resolve_uris.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:06:40.440779 rod-0.2.1.dev57/src/rod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-05-17 20:06:40.000000 rod-0.2.1.dev57/src/rod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-17 20:06:40.000000 rod-0.2.1.dev57/src/rod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 20:06:40.000000 rod-0.2.1.dev57/src/rod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 20:06:40.000000 rod-0.2.1.dev57/src/rod.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-17 20:06:40.000000 rod-0.2.1.dev57/src/rod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-17 20:06:40.000000 rod-0.2.1.dev57/src/rod.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:06:40.440779 rod-0.2.1.dev57/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/tests/test_meshbuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/tests/test_urdf_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/tests/test_urdf_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-17 20:06:26.000000 rod-0.2.1.dev57/tests/utils_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:31:49.007024 rod-0.2.dev12/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:31:48.995023 rod-0.2.dev12/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:31:48.999024 rod-0.2.dev12/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-03-08 14:31:35.000000 rod-0.2.dev12/.github/workflows/ci_cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-03-08 14:31:35.000000 rod-0.2.dev12/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-03-08 14:31:35.000000 rod-0.2.dev12/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-03-08 14:31:35.000000 rod-0.2.dev12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-03-08 14:31:49.007024 rod-0.2.dev12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7109 2024-03-08 14:31:35.000000 rod-0.2.dev12/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-08 14:31:35.000000 rod-0.2.dev12/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-03-08 14:31:49.007024 rod-0.2.dev12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 14:31:35.000000 rod-0.2.dev12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:31:48.999024 rod-0.2.dev12/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:31:48.999024 rod-0.2.dev12/src/rod/
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:31:48.999024 rod-0.2.dev12/src/rod/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/builder/primitive_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/builder/primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:31:49.003023 rod-0.2.dev12/src/rod/kinematics/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/kinematics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13757 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/kinematics/kinematic_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/kinematics/tree_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/pretty_printer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:31:49.003023 rod-0.2.dev12/src/rod/sdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/sdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/sdf/collision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/sdf/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/sdf/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/sdf/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/sdf/joint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/sdf/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/sdf/material.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/sdf/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/sdf/physics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/sdf/scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/sdf/sdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/sdf/visual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/sdf/world.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:31:49.003023 rod-0.2.dev12/src/rod/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/tree/directed_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/tree/tree_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:31:49.003023 rod-0.2.dev12/src/rod/urdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/urdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21139 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/urdf/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:31:49.003023 rod-0.2.dev12/src/rod/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8977 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/utils/frame_convention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/utils/gazebo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/utils/resolve_frames.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-03-08 14:31:35.000000 rod-0.2.dev12/src/rod/utils/resolve_uris.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:31:49.007024 rod-0.2.dev12/src/rod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-03-08 14:31:48.000000 rod-0.2.dev12/src/rod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-08 14:31:48.000000 rod-0.2.dev12/src/rod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 14:31:48.000000 rod-0.2.dev12/src/rod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 14:31:48.000000 rod-0.2.dev12/src/rod.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-08 14:31:48.000000 rod-0.2.dev12/src/rod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-08 14:31:48.000000 rod-0.2.dev12/src/rod.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:31:49.007024 rod-0.2.dev12/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-03-08 14:31:35.000000 rod-0.2.dev12/tests/test_urdf_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-03-08 14:31:35.000000 rod-0.2.dev12/tests/utils_models.py
```

### Comparing `rod-0.2.1.dev57/.github/workflows/style.yml` & `rod-0.2.dev12/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev57/.gitignore` & `rod-0.2.dev12/.gitignore`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev57/LICENSE` & `rod-0.2.dev12/LICENSE`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev57/PKG-INFO` & `rod-0.2.dev12/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rod
-Version: 0.2.1.dev57
+Version: 0.2.dev12
 Summary: The ultimate Python tool for RObot Descriptions processing.
 Home-page: https://github.com/ami-iit/rod
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/rod/releases
 Project-URL: Source, https://github.com/ami-iit/rod
@@ -18,30 +18,30 @@
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Games/Entertainment :: Simulation
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 Requires-Dist: mashumaro
 Requires-Dist: numpy
 Requires-Dist: packaging
 Requires-Dist: resolve-robotics-uri-py
 Requires-Dist: scipy
-Requires-Dist: trimesh
 Requires-Dist: xmltodict
 Provides-Extra: style
 Requires-Dist: black; extra == "style"
 Requires-Dist: isort; extra == "style"
 Provides-Extra: pptree
 Requires-Dist: pptree; extra == "pptree"
 Provides-Extra: test
@@ -77,79 +77,47 @@
 If the URDF model is not compliant, the process errors with clear messages.
 Furthermore, modern versions of the converter produce a SDF description with standardized [pose semantics][pose_semantics],
 that greatly simplifies the life of downstream developers that do not have to guess the reference frame or pose elements.
 Last but not least, the pose semantics also makes SDF aware of the concept of _frame_ that URDF is missing.
 
 ## Features
 
-- Out-of-the-box support for SDFormat specifications [≥ 1.10][sdformat_spec_110].
-- Serialization and deserialization support for SDF files.
-- In-memory layout based on `dataclasses`.
-- Syntax highlighting and auto-completion.
-- Programmatic creation of SDF files from Python APIs.
-- Transitive support for URDF through conversion to SDF.
-- Type validation of elements and attributes.
-- Automatic check of missing required elements.
-- High-performance serialization and deserialization using [`Fatal1ty/mashumaro`][mashumaro].
-- Export in-memory model description to URDF.
+- Out-of-the-box support of SDFormat specifications [≥ 1.7][sdformat_spec_17]
+- Serialization and deserialization support of SDF files
+- In-memory layout based on `dataclasses`
+- Syntax highlighting and auto-completion
+- Support of programmatic creation of SDF files from Python APIs
+- Transitive support of URDF through conversion to SDF[^urdf_to_sdf]
+- Type validation of elements and attributes
+- Automatic check of missing required elements
+- Based on [`Fatal1ty/mashumaro`][mashumaro] for great serialization and deserialization performance
+- Support of exporting the in-memory model description to URDF
 
 [mashumaro]: https://github.com/Fatal1ty/mashumaro
 [open_robotics]: https://www.openrobotics.org/
 [pose_semantics]: http://sdformat.org/tutorials?tut=pose_frame_semantics_proposal&cat=pose_semantics_docs&
 [sdformat]: http://sdformat.org/
 [sdformat_python]: http://sdformat.org/tutorials?tut=python_bindings&cat=developers&
+[sdformat_repo]: https://github.com/gazebosim/sdformat
 [sdformat_spec]: http://sdformat.org/spec
-[sdformat_spec_110]: http://sdformat.org/spec?elem=sdf&ver=1.10
+[sdformat_spec_17]: http://sdformat.org/spec?elem=sdf&ver=1.7
 [urdf]: http://wiki.ros.org/urdf
 
-[^urdf_to_sdf]: Conversion can be done using the `gz sdf` command included in Gazebo Sim starting from Garden.
+[^urdf_to_sdf]: Conversion can be done either using `ign sdf` included in Ignition Gazebo Fortress, or `gz sdf` included in Gazebo Sim starting from Garden.
 
 ## Installation
 
-> [!TIP]
-> ROD does not support out-of-the-box URDF files.
-> URDF support is obtained by converting URDF files to SDF using the `gz sdf` command provided by [sdformat][sdformat_repo] and [gz-tools][gz-tools_repo].
-> Ensure these tools are installed on your system if URDF support is needed (more information below).
-
-[sdformat_repo]: https://github.com/gazebosim/sdformat
-[gz-tools_repo]: https://github.com/gazebosim/gz-tools
-
-<details>
-<summary>Using conda (recommended)</summary>
-
-Installing ROD using `conda` is the recommended way to obtain a complete installation with out-of-the-box support for both URDF and SDF descriptions:
+You can install the project with [`pypa/pip`][pip], preferably in a [virtual environment][venv]:
 
 ```bash
-conda install rod -c conda-forge
+pip install git+https://github.com/ami-iit/rod
 ```
 
-This will automatically install `sdformat` and `gz-tools`. 
-
-</details>
-
-<details>
-<summary>Using pip</summary>
-
-You can install ROD from PyPI with [`pypa/pip`][pip], preferably in a [virtual environment][venv]:
-
-```bash
-pip install rod[all]
-```
-
-If you need URDF support, follow the [official instructions][gazebo_sim_docs] to install Gazebo Sim on your operating system,
-making sure to obtain `sdformat ≥ 13.0` and `gz-tools ≥ 2.0`.
-
-You don't need to install the entire Gazebo Sim suite.
-For example, on Ubuntu, you can only install the `libsdformat13 gz-tools2` packages.
-
 [pip]: https://github.com/pypa/pip/
-[venv]: https://docs.python.org/3.10/tutorial/venv.html
-[gazebo_sim_docs]: https://gazebosim.org/docs
-
-</details>
+[venv]: https://docs.python.org/3.8/tutorial/venv.html
 
 ## Examples
 
 <details>
 <summary>Serialize and deserialize SDF files</summary>
 
 ```python
@@ -252,16 +220,18 @@
 
 ```python
 # Generate first the 'sdf' object with the collapsed code
 # of the section 'Create SDF models programmatically'.
 
 from rod.urdf.exporter import UrdfExporter
 
-urdf_string = UrdfExporter(pretty=True, gazebo_preserve_fixed_joints=True).to_urdf_string(
-    sdf=sdf
+urdf_string = UrdfExporter.sdf_to_urdf_string(
+    sdf=sdf,
+    pretty=True,
+    gazebo_preserve_fixed_joints=True,
 )
 
 print(urdf_string)
 ```
 
 ```xml
 <?xml version="1.0" encoding="utf-8"?>
```

### Comparing `rod-0.2.1.dev57/README.md` & `rod-0.2.dev12/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -17,79 +17,47 @@
 If the URDF model is not compliant, the process errors with clear messages.
 Furthermore, modern versions of the converter produce a SDF description with standardized [pose semantics][pose_semantics],
 that greatly simplifies the life of downstream developers that do not have to guess the reference frame or pose elements.
 Last but not least, the pose semantics also makes SDF aware of the concept of _frame_ that URDF is missing.
 
 ## Features
 
-- Out-of-the-box support for SDFormat specifications [≥ 1.10][sdformat_spec_110].
-- Serialization and deserialization support for SDF files.
-- In-memory layout based on `dataclasses`.
-- Syntax highlighting and auto-completion.
-- Programmatic creation of SDF files from Python APIs.
-- Transitive support for URDF through conversion to SDF.
-- Type validation of elements and attributes.
-- Automatic check of missing required elements.
-- High-performance serialization and deserialization using [`Fatal1ty/mashumaro`][mashumaro].
-- Export in-memory model description to URDF.
+- Out-of-the-box support of SDFormat specifications [≥ 1.7][sdformat_spec_17]
+- Serialization and deserialization support of SDF files
+- In-memory layout based on `dataclasses`
+- Syntax highlighting and auto-completion
+- Support of programmatic creation of SDF files from Python APIs
+- Transitive support of URDF through conversion to SDF[^urdf_to_sdf]
+- Type validation of elements and attributes
+- Automatic check of missing required elements
+- Based on [`Fatal1ty/mashumaro`][mashumaro] for great serialization and deserialization performance
+- Support of exporting the in-memory model description to URDF
 
 [mashumaro]: https://github.com/Fatal1ty/mashumaro
 [open_robotics]: https://www.openrobotics.org/
 [pose_semantics]: http://sdformat.org/tutorials?tut=pose_frame_semantics_proposal&cat=pose_semantics_docs&
 [sdformat]: http://sdformat.org/
 [sdformat_python]: http://sdformat.org/tutorials?tut=python_bindings&cat=developers&
+[sdformat_repo]: https://github.com/gazebosim/sdformat
 [sdformat_spec]: http://sdformat.org/spec
-[sdformat_spec_110]: http://sdformat.org/spec?elem=sdf&ver=1.10
+[sdformat_spec_17]: http://sdformat.org/spec?elem=sdf&ver=1.7
 [urdf]: http://wiki.ros.org/urdf
 
-[^urdf_to_sdf]: Conversion can be done using the `gz sdf` command included in Gazebo Sim starting from Garden.
+[^urdf_to_sdf]: Conversion can be done either using `ign sdf` included in Ignition Gazebo Fortress, or `gz sdf` included in Gazebo Sim starting from Garden.
 
 ## Installation
 
-> [!TIP]
-> ROD does not support out-of-the-box URDF files.
-> URDF support is obtained by converting URDF files to SDF using the `gz sdf` command provided by [sdformat][sdformat_repo] and [gz-tools][gz-tools_repo].
-> Ensure these tools are installed on your system if URDF support is needed (more information below).
-
-[sdformat_repo]: https://github.com/gazebosim/sdformat
-[gz-tools_repo]: https://github.com/gazebosim/gz-tools
-
-<details>
-<summary>Using conda (recommended)</summary>
-
-Installing ROD using `conda` is the recommended way to obtain a complete installation with out-of-the-box support for both URDF and SDF descriptions:
+You can install the project with [`pypa/pip`][pip], preferably in a [virtual environment][venv]:
 
 ```bash
-conda install rod -c conda-forge
+pip install git+https://github.com/ami-iit/rod
 ```
 
-This will automatically install `sdformat` and `gz-tools`. 
-
-</details>
-
-<details>
-<summary>Using pip</summary>
-
-You can install ROD from PyPI with [`pypa/pip`][pip], preferably in a [virtual environment][venv]:
-
-```bash
-pip install rod[all]
-```
-
-If you need URDF support, follow the [official instructions][gazebo_sim_docs] to install Gazebo Sim on your operating system,
-making sure to obtain `sdformat ≥ 13.0` and `gz-tools ≥ 2.0`.
-
-You don't need to install the entire Gazebo Sim suite.
-For example, on Ubuntu, you can only install the `libsdformat13 gz-tools2` packages.
-
 [pip]: https://github.com/pypa/pip/
-[venv]: https://docs.python.org/3.10/tutorial/venv.html
-[gazebo_sim_docs]: https://gazebosim.org/docs
-
-</details>
+[venv]: https://docs.python.org/3.8/tutorial/venv.html
 
 ## Examples
 
 <details>
 <summary>Serialize and deserialize SDF files</summary>
 
 ```python
@@ -192,16 +160,18 @@
 
 ```python
 # Generate first the 'sdf' object with the collapsed code
 # of the section 'Create SDF models programmatically'.
 
 from rod.urdf.exporter import UrdfExporter
 
-urdf_string = UrdfExporter(pretty=True, gazebo_preserve_fixed_joints=True).to_urdf_string(
-    sdf=sdf
+urdf_string = UrdfExporter.sdf_to_urdf_string(
+    sdf=sdf,
+    pretty=True,
+    gazebo_preserve_fixed_joints=True,
 )
 
 print(urdf_string)
 ```
 
 ```xml
 <?xml version="1.0" encoding="utf-8"?>
```

### Comparing `rod-0.2.1.dev57/setup.cfg` & `rod-0.2.dev12/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -33,35 +33,35 @@
 	Intended Audience :: Education
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Operating System :: POSIX :: Linux
 	Operating System :: MacOS
 	Operating System :: Microsoft :: Windows
 	Programming Language :: Python :: 3
+	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
-	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Games/Entertainment :: Simulation
 
 [options]
 zip_safe = False
 packages = find:
 package_dir = 
 	=src
-python_requires = >=3.10
+python_requires = >=3.8
 install_requires = 
 	coloredlogs
 	mashumaro
 	numpy
 	packaging
 	resolve-robotics-uri-py
 	scipy
-	trimesh
 	xmltodict
 
 [options.extras_require]
 style = 
 	black
 	isort
 pptree =
```

### Comparing `rod-0.2.1.dev57/src/rod/builder/primitive_builder.py` & `rod-0.2.dev12/src/rod/builder/primitive_builder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,32 @@
-from __future__ import annotations
-
 import abc
 import dataclasses
-from typing import Optional
+from typing import Optional, Union
 
 import numpy as np
 import numpy.typing as npt
 
 import rod
 from rod import logging
 
 
 @dataclasses.dataclass
 class PrimitiveBuilder(abc.ABC):
     name: str
     mass: float
 
-    element: rod.Model | rod.Link | rod.Inertial | rod.Collision | rod.Visual = (
+    element: Union[rod.Model, rod.Link, rod.Inertial, rod.Collision, rod.Visual] = (
         dataclasses.field(
             default=None, init=False, repr=False, hash=False, compare=False
         )
     )
 
     def build(
         self,
-    ) -> rod.Model | rod.Link | rod.Inertial | rod.Collision | rod.Visual:
+    ) -> Union[rod.Model, rod.Link, rod.Inertial, rod.Collision, rod.Visual]:
         return self.element
 
     # ================
     # Abstract methods
     # ================
 
     @abc.abstractmethod
@@ -41,90 +39,90 @@
 
     # ================
     # Element builders
     # ================
 
     def build_model(
         self,
-        name: str | None = None,
-        pose: rod.Pose | None = None,
-    ) -> PrimitiveBuilder:
+        name: Optional[str] = None,
+        pose: Optional[rod.Pose] = None,
+    ) -> "PrimitiveBuilder":
         self._check_element()
 
         self.element = self._model(name=name, pose=pose)
 
         return self
 
     def build_link(
         self,
-        name: str | None = None,
-        pose: rod.Pose | None = None,
-    ) -> PrimitiveBuilder:
+        name: Optional[str] = None,
+        pose: Optional[rod.Pose] = None,
+    ) -> "PrimitiveBuilder":
         self._check_element()
 
         self.element = self._link(name=name, pose=pose)
 
         return self
 
-    def build_inertial(self, pose: rod.Pose | None = None) -> PrimitiveBuilder:
+    def build_inertial(self, pose: Optional[rod.Pose] = None) -> "PrimitiveBuilder":
         self._check_element()
 
         self.element = self._inertial(pose=pose)
 
         return self
 
     def build_visual(
         self,
-        name: str | None = None,
-        pose: rod.Pose | None = None,
-    ) -> PrimitiveBuilder:
+        name: Optional[str] = None,
+        pose: Optional[rod.Pose] = None,
+    ) -> "PrimitiveBuilder":
         self._check_element()
 
         self.element = self._visual(name=name, pose=pose)
 
         return self
 
     def build_collision(
         self,
-        name: str | None = None,
-        pose: rod.Pose | None = None,
-    ) -> PrimitiveBuilder:
+        name: Optional[str] = None,
+        pose: Optional[rod.Pose] = None,
+    ) -> "PrimitiveBuilder":
         self._check_element()
 
         self.element = self._collision(name=name, pose=pose)
 
         return self
 
     # =================
     # Element modifiers
     # =================
 
     def add_link(
         self,
-        name: str | None = None,
-        pose: rod.Pose | None = None,
-        link: rod.Link | None = None,
-    ) -> PrimitiveBuilder:
+        name: Optional[str] = None,
+        pose: Optional[rod.Pose] = None,
+        link: Optional[rod.Link] = None,
+    ) -> "PrimitiveBuilder":
         if not isinstance(self.element, rod.Model):
             raise ValueError(type(self.element))
 
         link = link if link is not None else self._link(name=name, pose=pose)
 
         if pose is not None:
             link.pose = pose
 
         self.element.link = link
 
         return self
 
     def add_inertial(
         self,
-        pose: rod.Pose | None = None,
-        inertial: rod.Inertial | None = None,
-    ) -> PrimitiveBuilder:
+        pose: Optional[rod.Pose] = None,
+        inertial: Optional[rod.Inertial] = None,
+    ) -> "PrimitiveBuilder":
         if not isinstance(self.element, (rod.Model, rod.Link)):
             raise ValueError(type(self.element))
 
         if isinstance(self.element, rod.Model):
             link = self.element.link
 
         elif isinstance(self.element, rod.Link):
@@ -142,19 +140,19 @@
 
         link.inertial = inertial
 
         return self
 
     def add_visual(
         self,
-        name: str | None = None,
+        name: Optional[str] = None,
         use_inertial_pose: bool = True,
-        pose: rod.Pose | None = None,
-        visual: rod.Visual | None = None,
-    ) -> PrimitiveBuilder:
+        pose: Optional[rod.Pose] = None,
+        visual: Optional[rod.Visual] = None,
+    ) -> "PrimitiveBuilder":
         if not isinstance(self.element, (rod.Model, rod.Link)):
             raise ValueError(type(self.element))
 
         if isinstance(self.element, rod.Model):
             link = self.element.link
 
         elif isinstance(self.element, rod.Link):
@@ -178,19 +176,19 @@
 
         link.add_visual(visual=visual)
 
         return self
 
     def add_collision(
         self,
-        name: str | None = None,
+        name: Optional[str] = None,
         use_inertial_pose: bool = True,
-        pose: rod.Pose | None = None,
-        collision: rod.Collision | None = None,
-    ) -> PrimitiveBuilder:
+        pose: Optional[rod.Pose] = None,
+        collision: Optional[rod.Collision] = None,
+    ) -> "PrimitiveBuilder":
         if not isinstance(self.element, (rod.Model, rod.Link)):
             raise ValueError(type(self.element))
 
         if isinstance(self.element, rod.Model):
             link = self.element.link
 
         elif isinstance(self.element, rod.Link):
@@ -222,62 +220,62 @@
 
     # ====================
     # ROD element builders
     # ====================
 
     def _model(
         self,
-        name: str | None = None,
-        pose: rod.Pose | None = None,
+        name: Optional[str] = None,
+        pose: Optional[rod.Pose] = None,
     ) -> rod.Model:
         name = name if name is not None else self.name
         logging.debug(f"Building model '{name}'")
 
         if pose is not None and pose.relative_to != "world":
             raise ValueError("Model pose must be relative to 'world")
 
         return rod.Model(
             name=name,
             pose=pose,
         )
 
     def _link(
         self,
-        name: str | None = None,
-        pose: rod.Pose | None = None,
+        name: Optional[str] = None,
+        pose: Optional[rod.Pose] = None,
     ) -> rod.Link:
         return rod.Link(
             name=name if name is not None else f"{self.name}_link",
             pose=pose,
         )
 
-    def _inertial(self, pose: rod.Pose | None = None) -> rod.Inertial:
+    def _inertial(self, pose: Optional[rod.Pose] = None) -> rod.Inertial:
         return rod.Inertial(
             pose=pose,
             mass=self.mass,
             inertia=self._inertia(),
         )
 
     def _visual(
         self,
-        name: str | None = None,
-        pose: rod.Pose | None = None,
+        name: Optional[str] = None,
+        pose: Optional[rod.Pose] = None,
     ) -> rod.Visual:
         name = name if name is not None else f"{self.name}_visual"
 
         return rod.Visual(
             name=name,
             pose=pose,
             geometry=self._geometry(),
         )
 
     def _collision(
         self,
         name: Optional[str],
-        pose: rod.Pose | None = None,
+        pose: Optional[rod.Pose] = None,
     ) -> rod.Collision:
         name = name if name is not None else f"{self.name}_collision"
 
         return rod.Collision(
             name=name,
             pose=pose,
             geometry=self._geometry(),
@@ -295,15 +293,15 @@
     @staticmethod
     def build_pose(
         pos: npt.NDArray = None,
         rpy: npt.NDArray = None,
         relative_to: str = None,
         degrees: bool = None,
         rotation_format: str = None,
-    ) -> rod.Pose | None:
+    ) -> Optional[rod.Pose]:
         if pos is None and rpy is None:
             return rod.Pose.from_transform(transform=np.eye(4), relative_to=relative_to)
 
         pos = np.zeros(3) if pos is None else pos
         rpy = np.zeros(3) if rpy is None else rpy
 
         if pos.size != 3:
```

### Comparing `rod-0.2.1.dev57/src/rod/kinematics/kinematic_tree.py` & `rod-0.2.dev12/src/rod/kinematics/kinematic_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-from __future__ import annotations
-
 import copy
 import dataclasses
 import functools
-from typing import Dict, List, Sequence, Tuple
+from typing import Dict, List, Sequence, Tuple, Union
 
 import numpy as np
 
 import rod
 from rod import logging
 from rod.tree import DirectedTree, DirectedTreeNode, TreeEdge, TreeFrame
 
 
 @dataclasses.dataclass(frozen=True)
 class KinematicTree(DirectedTree):
-    model: rod.Model
+    model: "rod.Model"
 
     joints: List[TreeEdge] = dataclasses.field(default_factory=list)
     frames: List[TreeFrame] = dataclasses.field(default_factory=list)
 
     def __post_init__(self):
         # Initialize base class
         super().__post_init__()
@@ -44,15 +42,15 @@
     def frame_names(self) -> List[str]:
         return [frame.name() for frame in self.frames]
 
     def joint_names(self) -> List[str]:
         return [joint.name() for joint in self.joints]
 
     @staticmethod
-    def build(model: rod.Model, is_top_level: bool = True) -> KinematicTree:
+    def build(model: "rod.Model", is_top_level: bool = True) -> "KinematicTree":
         logging.debug(msg=f"Building kinematic tree of model '{model.name}'")
 
         if model.model is not None:
             msg = "Model composition is not yet supported. Ignoring all sub-models."
             logging.warning(msg=msg)
 
         # Copy the model and make reference frames explicit, i.e. add the pose element
@@ -197,15 +195,15 @@
             )
 
             # Produce new nodes and frames by removing the edge connecting base to world.
             # One of the additional frame will be the world frame.
             new_base_node, additional_frames = KinematicTree.remove_edge(
                 edge=world_to_base_edge, keep_parent=False
             )
-            assert any(f.name() == TreeFrame.WORLD for f in additional_frames)
+            assert any([f.name() == TreeFrame.WORLD for f in additional_frames])
 
             # Replace the former base node with the new base node
             nodes_links_dict[new_base_node.name()] = new_base_node
 
             # Add all the additional frames created by the edge removal process
             nodes_frames_dict = {
                 **nodes_frames_dict,
```

### Comparing `rod-0.2.1.dev57/src/rod/kinematics/tree_transforms.py` & `rod-0.2.dev12/src/rod/kinematics/tree_transforms.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,120 +1,83 @@
-from __future__ import annotations
-
 import copy
 import dataclasses
 
 import numpy as np
 import numpy.typing as npt
 
 import rod
 from rod.kinematics.kinematic_tree import KinematicTree
 from rod.tree import TreeFrame
 
 
 @dataclasses.dataclass
 class TreeTransforms:
     kinematic_tree: KinematicTree = dataclasses.dataclass(init=False)
-    _transform_cache: dict[str, npt.NDArray] = dataclasses.field(default_factory=dict)
 
     @staticmethod
     def build(
-        model: rod.Model,
+        model: "rod.Model",
         is_top_level: bool = True,
-    ) -> TreeTransforms:
+        prevent_switching_frame_convention: bool = False,
+    ) -> "TreeTransforms":
         model = copy.deepcopy(model)
 
-        # Make sure that all elements have a pose attribute with explicit 'relative_to'.
         model.resolve_frames(is_top_level=is_top_level, explicit_frames=True)
 
-        # Build the kinematic tree and return the TreeTransforms object.
+        if not prevent_switching_frame_convention:
+            model.switch_frame_convention(frame_convention=rod.FrameConvention.Urdf)
+
         return TreeTransforms(
             kinematic_tree=KinematicTree.build(model=model, is_top_level=is_top_level)
         )
 
     def transform(self, name: str) -> npt.NDArray:
-        if name in self._transform_cache:
-            return self._transform_cache[name]
-
-        self._transform_cache[name] = self._compute_transform(name=name)
-        return self._transform_cache[name]
-
-    def _compute_transform(self, name: str) -> npt.NDArray:
-        match name:
-            case TreeFrame.WORLD:
-
-                return np.eye(4)
-
-            case name if name in {TreeFrame.MODEL, self.kinematic_tree.model.name}:
-
-                relative_to = self.kinematic_tree.model.pose.relative_to
-                assert relative_to in {None, ""}, (relative_to, name)
-                return self.kinematic_tree.model.pose.transform()
-
-            case name if name in self.kinematic_tree.joint_names():
-
-                edge = self.kinematic_tree.joints_dict[name]
-                assert edge.name() == name
-
-                # Get the pose of the frame in which the node's pose is expressed
-                assert edge._source.pose.relative_to not in {"", None}
-                x_H_E = edge._source.pose.transform()
-                W_H_x = self.transform(name=edge._source.pose.relative_to)
-
-                # Compute the world-to-node transform
-                # TODO: this assumes all joint positions to be 0
-                W_H_E = W_H_x @ x_H_E
-
-                return W_H_E
-
-            case name if name in self.kinematic_tree.link_names():
+        if name == TreeFrame.WORLD:
+            return np.eye(4)
 
-                element = self.kinematic_tree.links_dict[name]
+        if name in {TreeFrame.MODEL, self.kinematic_tree.model.name}:
+            relative_to = self.kinematic_tree.model.pose.relative_to
+            assert relative_to in {None, ""}, (relative_to, name)
+            return self.kinematic_tree.model.pose.transform()
+
+        if name in self.kinematic_tree.joint_names():
+            edge = self.kinematic_tree.joints_dict[name]
+            assert edge.name() == name
+
+            # Get the pose of the frame in which the node's pose is expressed
+            assert edge._source.pose.relative_to not in {"", None}
+            x_H_E = edge._source.pose.transform()
+            W_H_x = self.transform(name=edge._source.pose.relative_to)
+
+            # Compute the world-to-node transform
+            # TODO: this assumes all joint positions to be 0
+            W_H_E = W_H_x @ x_H_E
+
+            return W_H_E
+
+        if (
+            name in self.kinematic_tree.link_names()
+            or name in self.kinematic_tree.frame_names()
+        ):
+            element = (
+                self.kinematic_tree.links_dict[name]
+                if name in self.kinematic_tree.link_names()
+                else self.kinematic_tree.frames_dict[name]
+            )
+            assert element.name() == name
+
+            # Get the pose of the frame in which the node's pose is expressed
+            assert element._source.pose.relative_to not in {"", None}
+            x_H_N = element._source.pose.transform()
+            W_H_x = self.transform(name=element._source.pose.relative_to)
 
-                assert element.name() == name
-                assert element._source.pose.relative_to not in {"", None}
+            # Compute and cache the world-to-node transform
+            W_H_N = W_H_x @ x_H_N
 
-                # Get the pose of the frame in which the link's pose is expressed.
-                x_H_L = element._source.pose.transform()
-                W_H_x = self.transform(name=element._source.pose.relative_to)
+            return W_H_N
 
-                # Compute the world transform of the link.
-                W_H_L = W_H_x @ x_H_L
-                return W_H_L
-
-            case name if name in self.kinematic_tree.frame_names():
-
-                element = self.kinematic_tree.frames_dict[name]
-
-                assert element.name() == name
-                assert element._source.pose.relative_to not in {"", None}
-
-                # Get the pose of the frame in which the frame's pose is expressed.
-                x_H_F = element._source.pose.transform()
-                W_H_x = self.transform(name=element._source.pose.relative_to)
-
-                # Compute the world transform of the frame.
-                W_H_F = W_H_x @ x_H_F
-                return W_H_F
-
-            case _:
-                raise ValueError(name)
+        raise ValueError(name)
 
     def relative_transform(self, relative_to: str, name: str) -> npt.NDArray:
-
-        world_H_name = self.transform(name=name)
-        world_H_relative_to = self.transform(name=relative_to)
-
-        return TreeTransforms.inverse(world_H_relative_to) @ world_H_name
-
-    @staticmethod
-    def inverse(transform: npt.NDArray) -> npt.NDArray:
-
-        R = transform[0:3, 0:3]
-        p = np.vstack(transform[0:3, 3])
-
-        return np.block(
-            [
-                [R.T, -R.T @ p],
-                [0, 0, 0, 1],
-            ]
+        return np.linalg.inv(self.transform(name=relative_to)) @ self.transform(
+            name=name
         )
```

### Comparing `rod-0.2.1.dev57/src/rod/logging.py` & `rod-0.2.dev12/src/rod/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import enum
 import logging
+from typing import Union
 
 import coloredlogs
 
 LOGGER_NAME = "rod"
 
 
 class LoggingLevel(enum.IntEnum):
@@ -15,15 +16,15 @@
     CRITICAL = logging.CRITICAL
 
 
 def _logger() -> logging.Logger:
     return logging.getLogger(name=LOGGER_NAME)
 
 
-def set_logging_level(level: int | LoggingLevel = LoggingLevel.WARNING):
+def set_logging_level(level: Union[int, LoggingLevel] = LoggingLevel.WARNING):
     if isinstance(level, int):
         level = LoggingLevel(level)
 
     _logger().setLevel(level=level.value)
 
 
 def get_logging_level() -> LoggingLevel:
```

### Comparing `rod-0.2.1.dev57/src/rod/pretty_printer.py` & `rod-0.2.dev12/src/rod/pretty_printer.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,50 +26,49 @@
                 if dataclasses.is_dataclass(el)
                 else str(el)
             )
             for el in obj
         ]
 
         return (
-            "[\n"
+            f"[\n"
             + ",\n".join(f"{spacing_level}{el!s}" for el in list_str)
             + f",\n{spacing_level_up}]"
         )
 
     @staticmethod
     def dataclass_to_str(obj: Any, level: int = 1) -> str:
         if not dataclasses.is_dataclass(obj):
             raise TypeError(obj, type(obj))
 
         serialization: List[Tuple[str, str]] = []
 
         for field in dataclasses.fields(obj):
             attr = getattr(obj, field.name)
 
-            match attr:
-                case None | "":
-                    continue
-
-                case list():
-                    list_str = DataclassPrettyPrinter.list_to_string(
-                        obj=attr, level=level + 1
-                    )
-                    serialization += [(field.name, list_str)]
-                    continue
-
-                case _ if dataclasses.is_dataclass(attr):
-                    dataclass_str = DataclassPrettyPrinter.dataclass_to_str(
-                        obj=attr, level=level + 1
-                    )
-                    serialization += [(field.name, dataclass_str)]
-                    continue
-
-                case _:
-                    serialization += [(field.name, f"{attr!s}")]
-                    continue
+            if attr is None or attr == "":
+                continue
+
+            elif isinstance(attr, list):
+                list_str = DataclassPrettyPrinter.list_to_string(
+                    obj=attr, level=level + 1
+                )
+                serialization += [(field.name, list_str)]
+                continue
+
+            elif dataclasses.is_dataclass(attr):
+                dataclass_str = DataclassPrettyPrinter.dataclass_to_str(
+                    obj=attr, level=level + 1
+                )
+                serialization += [(field.name, dataclass_str)]
+                continue
+
+            else:
+                serialization += [(field.name, f"{attr!s}")]
+                continue
 
         spacing = " " * 4
         spacing_level = spacing * level
         spacing_level_up = spacing * (level - 1)
 
         self_str = ",\n".join(
             f"{spacing_level}{name}={value_str}" for name, value_str in serialization
```

### Comparing `rod-0.2.1.dev57/src/rod/sdf/common.py` & `rod-0.2.dev12/src/rod/sdf/common.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev57/src/rod/sdf/element.py` & `rod-0.2.dev12/src/rod/sdf/element.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import dataclasses
-from typing import Any, Dict, List
+from typing import Any, Dict, List, Optional
 
 import mashumaro.config
 import mashumaro.mixins.dict
 import numpy as np
 
 from rod.pretty_printer import DataclassPrettyPrinter
 
@@ -33,28 +33,28 @@
     @staticmethod
     def deserialize_bool(data: str) -> bool:
         assert isinstance(data, str)
         true_vals = {"1", "True", "true"}
         false_vals = {"0", "False", "false"}
         assert data in true_vals.union(false_vals)
 
-        return data in true_vals
+        return True if data in true_vals else False
 
     @staticmethod
     def serialize_float(data: float) -> str:
         assert isinstance(data, float)
         return str(data)
 
     @staticmethod
     def serialize_list(data: List[float]) -> str:
         assert isinstance(data, list)
         return " ".join(np.array(data, dtype=str))
 
     @staticmethod
-    def deserialize_list(data: str, length: int | None = None) -> List[float]:
+    def deserialize_list(data: str, length: Optional[int] = None) -> List[float]:
         assert isinstance(data, str)
         array = np.atleast_1d(np.array(data.split(sep=" "), dtype=float).squeeze())
 
         if length is not None:
             assert array.size == length
 
         return list(array)
```

### Comparing `rod-0.2.1.dev57/src/rod/sdf/geometry.py` & `rod-0.2.dev12/src/rod/sdf/geometry.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev57/src/rod/sdf/joint.py` & `rod-0.2.dev12/src/rod/sdf/joint.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev57/src/rod/sdf/link.py` & `rod-0.2.dev12/src/rod/sdf/link.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import dataclasses
-from typing import List, Optional
+from typing import List, Optional, Union
 
 import mashumaro
 import numpy as np
 import numpy.typing as npt
 
 from .collision import Collision
 from .common import Pose
@@ -69,17 +69,19 @@
 class Link(Element):
     name: str = dataclasses.field(metadata=mashumaro.field_options(alias="@name"))
 
     pose: Optional[Pose] = dataclasses.field(default=None)
 
     inertial: Optional[Inertial] = dataclasses.field(default=None)
 
-    visual: Optional[Visual | List[Visual]] = dataclasses.field(default=None)
+    visual: Optional[Union[Visual, List[Visual]]] = dataclasses.field(default=None)
 
-    collision: Optional[Collision | List[Collision]] = dataclasses.field(default=None)
+    collision: Optional[Union[Collision, List[Collision]]] = dataclasses.field(
+        default=None
+    )
 
     gravity: Optional[bool] = dataclasses.field(
         default=None,
         metadata=mashumaro.field_options(
             serialize=Element.serialize_bool, deserialize=Element.deserialize_bool
         ),
     )
```

### Comparing `rod-0.2.1.dev57/src/rod/sdf/material.py` & `rod-0.2.dev12/src/rod/sdf/material.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev57/src/rod/sdf/model.py` & `rod-0.2.dev12/src/rod/sdf/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-from __future__ import annotations
-
 import dataclasses
-from typing import List, Optional
+from typing import List, Optional, Union
 
 import mashumaro
 
 import rod
 from rod import logging
 
 from .common import Frame, Pose
@@ -52,21 +50,21 @@
         metadata=mashumaro.field_options(
             serialize=Element.serialize_bool, deserialize=Element.deserialize_bool
         ),
     )
 
     pose: Optional[Pose] = dataclasses.field(default=None)
 
-    model: Optional[Model | List[Model]] = dataclasses.field(default=None)
+    model: Optional[Union["Model", List["Model"]]] = dataclasses.field(default=None)
 
-    frame: Optional[Frame | List[Frame]] = dataclasses.field(default=None)
+    frame: Optional[Union[Frame, List[Frame]]] = dataclasses.field(default=None)
 
-    link: Optional[Link | List[Link]] = dataclasses.field(default=None)
+    link: Optional[Union[Link, List[Link]]] = dataclasses.field(default=None)
 
-    joint: Optional[Joint | List[Joint]] = dataclasses.field(default=None)
+    joint: Optional[Union[Joint, List[Joint]]] = dataclasses.field(default=None)
 
     def is_fixed_base(self) -> bool:
         joints_having_world_parent = [j for j in self.joints() if j.parent == "world"]
         assert len(joints_having_world_parent) in {0, 1}
 
         return len(joints_having_world_parent) > 0
 
@@ -78,15 +76,15 @@
 
         if self.canonical_link is not None:
             assert self.canonical_link in {l.name for l in self.links()}
             return self.canonical_link
 
         return self.links()[0].name
 
-    def models(self) -> List[Model]:
+    def models(self) -> List["Model"]:
         if self.model is None:
             return []
 
         if isinstance(self.model, Model):
             return [self.model]
 
         assert isinstance(self.model, list)
@@ -153,22 +151,20 @@
 
         resolve_frames.resolve_model_frames(
             model=self, is_top_level=is_top_level, explicit_frames=explicit_frames
         )
 
     def switch_frame_convention(
         self,
-        frame_convention: rod.FrameConvention,
+        frame_convention: "rod.FrameConvention",
         is_top_level: bool = True,
         explicit_frames: bool = True,
-        attach_frames_to_links: bool = True,
     ) -> None:
         from rod.utils.frame_convention import switch_frame_convention
 
         switch_frame_convention(
             model=self,
             frame_convention=frame_convention,
             is_top_level=is_top_level,
-            attach_frames_to_links=attach_frames_to_links,
         )
 
         self.resolve_frames(is_top_level=is_top_level, explicit_frames=explicit_frames)
```

### Comparing `rod-0.2.1.dev57/src/rod/sdf/physics.py` & `rod-0.2.dev12/src/rod/sdf/physics.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev57/src/rod/sdf/scene.py` & `rod-0.2.dev12/src/rod/sdf/scene.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev57/src/rod/sdf/sdf.py` & `rod-0.2.dev12/src/rod/sdf/sdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from __future__ import annotations
-
 import dataclasses
 import os
 import pathlib
-from typing import List, Optional
+from typing import List, Optional, Union
 
 import mashumaro
 import packaging.specifiers
 import packaging.version
 import xmltodict
 
 from rod.utils.gazebo import GazeboHelper
@@ -17,17 +15,17 @@
 from .world import World
 
 
 @dataclasses.dataclass
 class Sdf(Element):
     version: str = dataclasses.field(metadata=mashumaro.field_options(alias="@version"))
 
-    world: Optional[World | List[World]] = dataclasses.field(default=None)
+    world: Optional[Union[World, List[World]]] = dataclasses.field(default=None)
 
-    model: Optional[Model | List[Model]] = dataclasses.field(default=None)
+    model: Optional[Union[Model, List[Model]]] = dataclasses.field(default=None)
 
     def worlds(self) -> List[World]:
         if self.world is None:
             return []
 
         if isinstance(self.world, World):
             return [self.world]
@@ -42,15 +40,15 @@
         if isinstance(self.model, Model):
             return [self.model]
 
         assert isinstance(self.model, list), type(self.model)
         return self.model
 
     @staticmethod
-    def load(sdf: pathlib.Path | str, is_urdf: bool | None = None) -> Sdf:
+    def load(sdf: Union[pathlib.Path, str], is_urdf: Optional[bool] = None) -> "Sdf":
         """
         Load an SDF resource.
 
         The SDF resource could either be a `pathlibPath` or a `str` containing
         either the path to the SDF file or an already parsed SDF string.
 
         Args:
@@ -78,15 +76,15 @@
 
         # Then, check if it's a string with a path
         elif (
             isinstance(sdf, str)
             and len(sdf) <= MAX_PATH
             and pathlib.Path(sdf).is_file()
         ):
-            sdf_string = pathlib.Path(sdf).read_text(encoding="utf-8")
+            sdf_string = pathlib.Path(sdf).read_text()
             is_urdf = (
                 is_urdf if is_urdf is not None else pathlib.Path(sdf).suffix == ".urdf"
             )
 
         # Finally, it must be a SDF/URDF string
         else:
             sdf_string = sdf
@@ -97,16 +95,16 @@
             sdf_string = GazeboHelper.process_model_description_with_sdformat(
                 model_description=urdf_string
             )
 
         # Parse the SDF to dict
         try:
             xml_dict = xmltodict.parse(xml_input=sdf_string)
-        except Exception as exc:
-            raise exc("Failed to parse 'sdf' argument")
+        except Exception:
+            raise ValueError("Failed to parse 'sdf' argument")
 
         # Look for the top-level <sdf> element
         try:
             sdf_dict = xml_dict["sdf"]
         except KeyError:
             raise RuntimeError("Failed to find top-level '<sdf>' element")
```

### Comparing `rod-0.2.1.dev57/src/rod/sdf/world.py` & `rod-0.2.dev12/src/rod/sdf/world.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import dataclasses
-from typing import List, Optional
+from typing import List, Optional, Union
 
 import mashumaro
 
 from .common import Frame
 from .element import Element
 from .model import Model
 from .physics import Physics
@@ -30,17 +30,17 @@
         ),
     )
 
     physics: Physics = dataclasses.field(default_factory=Physics)
 
     scene: Scene = dataclasses.field(default_factory=Scene)
 
-    model: Optional[Model | List[Model]] = dataclasses.field(default=None)
+    model: Optional[Union[Model, List[Model]]] = dataclasses.field(default=None)
 
-    frame: Optional[Frame | List[Frame]] = dataclasses.field(default=None)
+    frame: Optional[Union[Frame, List[Frame]]] = dataclasses.field(default=None)
 
     def models(self) -> List[Model]:
         if self.model is None:
             return []
 
         if isinstance(self.model, Model):
             return [self.model]
```

### Comparing `rod-0.2.1.dev57/src/rod/tree/directed_tree.py` & `rod-0.2.dev12/src/rod/tree/directed_tree.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import collections.abc
 import dataclasses
 import functools
-from typing import Any, Callable, Dict, Iterable, List
+from typing import Any, Callable, Dict, Iterable, List, Optional, Union
 
 from .tree_elements import DirectedTreeNode
 
 
 @dataclasses.dataclass(frozen=True)
 class DirectedTree(collections.abc.Sequence):
     root: DirectedTreeNode
@@ -29,15 +29,15 @@
     @functools.cached_property
     def nodes_dict(self) -> Dict[str, DirectedTreeNode]:
         return {node.name(): node for node in iter(self)}
 
     @staticmethod
     def breadth_first_search(
         root: DirectedTreeNode,
-        sort_children: Callable[[Any], Any] | None = lambda node: node.name(),
+        sort_children: Optional[Callable[[Any], Any]] = lambda node: node.name(),
     ) -> Iterable[DirectedTreeNode]:
         queue = [root]
 
         # We assume that nodes have a unique name, and we mark a node as visited by
         # storing its name. This assumption speeds up considerably object comparison.
         visited = list()
         visited.append(root.name)
@@ -65,16 +65,16 @@
             current_node=self.root,
             childattr="children",
             nameattr="tree_label",
             horizontal=True,
         )
 
     def __getitem__(
-        self, key: int | slice | str
-    ) -> DirectedTreeNode | List[DirectedTreeNode]:
+        self, key: Union[int, slice, str]
+    ) -> Union[DirectedTreeNode, List[DirectedTreeNode]]:
         # Get the nodes' dictionary (already inserted in order following BFS)
         nodes_dict = self.nodes_dict
 
         if isinstance(key, str):
             if key not in nodes_dict.keys():
                 raise KeyError(key)
 
@@ -96,15 +96,15 @@
 
     def __iter__(self) -> Iterable[DirectedTreeNode]:
         yield from DirectedTree.breadth_first_search(root=self.root)
 
     def __reversed__(self) -> Iterable[DirectedTreeNode]:
         yield from reversed(self)
 
-    def __contains__(self, item: str | DirectedTreeNode) -> bool:
+    def __contains__(self, item: Union[str, DirectedTreeNode]) -> bool:
         if isinstance(item, str):
             return item in self.nodes_dict.keys()
 
         if isinstance(item, DirectedTreeNode):
             return item.name() in self.nodes_dict.keys()
 
         raise TypeError(type(item).__name__)
```

### Comparing `rod-0.2.1.dev57/src/rod/tree/tree_elements.py` & `rod-0.2.dev12/src/rod/tree/tree_elements.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-from __future__ import annotations
-
 import abc
 import dataclasses
-from typing import ClassVar, List, Optional
+from typing import ClassVar, List, Optional, Union
 
 import rod
 from rod import logging
 
 
 class TreeElement(abc.ABC):
     index: Optional[int] = dataclasses.field(default=None, init=False)
@@ -27,27 +25,27 @@
 
     def __hash__(self):
         return hash(str(type(self)) + self.name())
 
 
 @dataclasses.dataclass(eq=False)
 class DirectedTreeNode(TreeElement):
-    parent: Optional[DirectedTreeNode] = None
-    children: List[DirectedTreeNode] = dataclasses.field(default_factory=list)
+    parent: Optional["DirectedTreeNode"] = None
+    children: List["DirectedTreeNode"] = dataclasses.field(default_factory=list)
 
-    _source: Optional[rod.Link] = dataclasses.field(default=None, repr=False)
+    _source: Optional["rod.Link"] = dataclasses.field(default=None, repr=False)
 
     def name(self) -> str:
         return self._source.name
 
-    def pose(self) -> rod.Pose:
+    def pose(self) -> "rod.Pose":
         if self._source is not None and self._source.pose is not None:
             return self._source.pose
-
-        return rod.Pose(relative_to="world")
+        else:
+            return rod.Pose(relative_to="world")
 
     @property
     def tree_label(self) -> str:
         return (
             f"#{self.index}_<{self.name()}>"
             if self.index is not None
             else f"<{self.name()}>"
@@ -67,15 +65,15 @@
 @dataclasses.dataclass(eq=False)
 class TreeEdge(TreeElement):
     child: DirectedTreeNode
     parent: DirectedTreeNode
 
     _source: Optional[rod.Joint] = dataclasses.field(default=None, repr=False)
 
-    def pose(self) -> rod.Pose:
+    def pose(self) -> "rod.Pose":
         return self._source.pose
 
     def name(self) -> str:
         return self._source.name
 
     def __str__(self) -> str:
         content_string = "name={}, parent={}, child={}".format(
@@ -86,15 +84,15 @@
 
 
 @dataclasses.dataclass(eq=False)
 class TreeFrame(TreeElement):
     WORLD: ClassVar[str] = "world"
     MODEL: ClassVar[str] = "__model__"
 
-    _source: Optional[rod.Frame] = dataclasses.field(default=None, repr=False)
+    _source: Optional["rod.Frame"] = dataclasses.field(default=None, repr=False)
 
     def name(self) -> str:
         return self._source.name
 
     def attached_to(self) -> str:
         return self._source.attached_to
 
@@ -107,16 +105,16 @@
         )
 
         return f"{type(self).__name__}({content_string})"
 
     @staticmethod
     def from_node(
         node: DirectedTreeNode,
-        attached_to: DirectedTreeNode | TreeFrame | TreeEdge | None = None,
-    ) -> TreeFrame:
+        attached_to: Union[DirectedTreeNode, "TreeFrame", TreeEdge] = None,
+    ) -> "TreeFrame":
         attached_to = attached_to if attached_to is not None else node.parent
 
         logging.debug(
             msg="Node '{}' became a frame attached to '{}'".format(
                 node.name(), attached_to.name() if attached_to is not None else "None"
             )
         )
@@ -126,16 +124,16 @@
                 name=node.name(), pose=node._source.pose, attached_to=attached_to.name()
             )
         )
 
     @staticmethod
     def from_edge(
         edge: TreeEdge,
-        attached_to: DirectedTreeNode | TreeFrame | TreeEdge | None = None,
-    ) -> TreeFrame:
+        attached_to: Union[DirectedTreeNode, "TreeFrame", TreeEdge] = None,
+    ) -> "TreeFrame":
         attached_to = attached_to if attached_to is not None else edge.parent
 
         logging.debug(
             msg="Edge '{}' became a frame attached to '{}'".format(
                 edge.name(), attached_to.name() if attached_to is not None else "None"
             )
         )
```

### Comparing `rod-0.2.1.dev57/src/rod/urdf/exporter.py` & `rod-0.2.dev12/src/rod/urdf/exporter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,86 +1,61 @@
 import abc
 import copy
-import dataclasses
-from typing import Any, ClassVar, Dict, List, Set
+from typing import Any, Dict, List, Union
 
 import numpy as np
 import xmltodict
 
 import rod
 from rod import logging
 from rod.kinematics.tree_transforms import TreeTransforms
 
 
-@dataclasses.dataclass
 class UrdfExporter(abc.ABC):
-    """Resources to convert an in-memory ROD model to URDF."""
 
-    # The string to use for each indentation level.
-    indent: str = "  "
+    SupportedSdfJointTypes = {"revolute", "continuous", "prismatic", "fixed"}
 
-    # Whether to include indentation and newlines in the output.
-    pretty: bool = False
-
-    # Whether to inject additional `<gazebo>` elements in the resulting URDF
-    # to preserve fixed joints in case of re-loading into sdformat.
-    # If a list of strings is passed, only the listed fixed joints will be preserved.
-    gazebo_preserve_fixed_joints: bool | List[str] = False
-
-    SupportedSdfJointTypes: ClassVar[Set[str]] = {
-        "revolute",
-        "continuous",
-        "prismatic",
-        "fixed",
-    }
-
-    DefaultMaterial: ClassVar[Dict[str, Any]] = {
+    DefaultMaterial = {
         "@name": "default_material",
         "color": {
             "@rgba": " ".join(np.array([1, 1, 1, 1], dtype=str)),
         },
     }
 
     @staticmethod
     def sdf_to_urdf_string(
         sdf: rod.Sdf | rod.Model,
         pretty: bool = False,
         indent: str = "  ",
-        gazebo_preserve_fixed_joints: bool | List[str] = False,
+        gazebo_preserve_fixed_joints: Union[bool, List[str]] = False,
     ) -> str:
-
-        msg = "This method is deprecated, please use '{}' instead."
-        logging.warning(msg.format("UrdfExporter.to_urdf_string"))
-
-        return UrdfExporter(
-            pretty=pretty,
-            indent=indent,
-            gazebo_preserve_fixed_joints=gazebo_preserve_fixed_joints,
-        ).to_urdf_string(sdf=sdf)
-
-    def to_urdf_string(self, sdf: rod.Sdf | rod.Model) -> str:
         """
         Convert an in-memory SDF model to a URDF string.
 
         Args:
             sdf: The SDF model parsed by ROD to convert.
+            pretty: Whether to include indentation and newlines in the output.
+            indent: The string to use for each indentation level.
+            gazebo_preserve_fixed_joints: Whether to inject additional `<gazebo>` elements in the
+                resulting URDF to preserve fixed joints in case of re-loading into sdformat.
+                If a list of strings is passed, only the listed fixed joints will be preserved.
+                If `True` is passed, all fixed joints will be preserved.
 
         Returns:
             The URDF string representing the converted SDF model.
         """
 
         # Operate on a copy of the sdf object
         sdf = copy.deepcopy(sdf)
 
         if isinstance(sdf, rod.Sdf) and len(sdf.models()) > 1:
             raise RuntimeError("URDF only supports one robot element")
 
         # Get the model
         model = sdf if isinstance(sdf, rod.Model) else sdf.models()[0]
-        logging.debug(f"Converting model '{model.name}' to URDF")
 
         # Remove all poses that could be assumed being implicit
         model.resolve_frames(is_top_level=True, explicit_frames=False)
 
         # Model composition is not supported, ignoring sub-models
         if len(model.models()) > 0:
             msg = f"Ignoring unsupported sub-models of model '{model.name}'"
@@ -99,15 +74,14 @@
             and model.pose is not None
             and not np.allclose(model.pose.pose, np.zeros(6))
         ):
             logging.warning("Ignoring non-trivial pose of fixed-base model")
             model.pose = None
 
         # Get the canonical link of the model
-        logging.debug(f"Detected '{model.get_canonical_link()}' as root link")
         canonical_link: rod.Link = {l.name: l for l in model.links()}[
             model.get_canonical_link()
         ]
 
         # If the canonical link has a custom pose, notify that it will be ignored.
         # In fact, it might happen that the canonical link has a custom pose w.r.t.
         # the __model__ frame. In SDF, the __model__frame defines the default reference
@@ -119,118 +93,121 @@
             and not np.allclose(canonical_link.pose.pose, np.zeros(6))
         ):
             msg = "Ignoring non-trivial pose of canonical link '{name}'"
             logging.warning(msg.format(name=canonical_link.name))
             canonical_link.pose = None
 
         # Convert all poses to use the Urdf frames convention.
-        # This process drastically simplifies extracting compatible kinematic transforms.
-        # Furthermore, it post-processes frames such that they get directly attached to
-        # a real link (instead of being attached to other frames).
+        # This process drastically simplifies extracting compatible kinematic trasforms.
         model.switch_frame_convention(
-            frame_convention=rod.FrameConvention.Urdf,
-            explicit_frames=True,
-            attach_frames_to_links=True,
+            frame_convention=rod.FrameConvention.Urdf, explicit_frames=True
         )
 
         # ============================================
         # Convert SDF frames to URDF equivalent chains
         # ============================================
 
         # Tree transforms helper used to process SDF frame poses, if any.
         # No need to switch frame convention to Urdf since it was already done above.
         tree_transforms = (
-            TreeTransforms.build(model=model, is_top_level=True)
+            TreeTransforms.build(
+                model=model,
+                is_top_level=True,
+                prevent_switching_frame_convention=True,
+            )
             if len(model.frames()) is not None
             else None
         )
 
         # Initialize the containers of extra links and joints
         extra_links_from_frames: List[Dict[str, Any]] = []
         extra_joints_from_frames: List[Dict[str, Any]] = []
 
         # Since URDF does not support plain frames as SDF, we convert all frames
         # to (fixed_joint->dummy_link) sequences
         for frame in model.frames():
+            # Find the name of the first parent link of a frame (since a frame could be
+            # attached to another frame). Falls back to __model__ in case of failure.
+            parent_link_name = UrdfExporter._find_parent_link(frame=frame, model=model)
+
+            # Populate a new Pose with the transform between the link to which the fixed
+            # joint will be attached and the frame that will be converted to dummy link
+            new_link_pose = rod.Pose.from_transform(
+                transform=tree_transforms.relative_transform(
+                    relative_to=parent_link_name, name=frame.name
+                ),
+                relative_to=parent_link_name,
+            )
+
+            # Smallest value not ignored by sdformat
+            epsilon = 1e-6 + 1e-9
 
             # New dummy link with same name of the frame
-            dummy_link = {
+            new_link = {
                 "@name": frame.name,
+                # If the link has no inertial properties, parsing again the exported
+                # URDF model with SDF would ignore it.
+                # We need to add a tiny fake mass greater than 1e-6.
+                # https://github.com/gazebosim/sdformat/issues/199#issuecomment-622127508
                 "inertial": {
                     "origin": {
                         "@xyz": "0 0 0",
                         "@rpy": "0 0 0",
                     },
-                    "mass": {"@value": 0.0},
+                    "mass": {"@value": str(epsilon)},
                     "inertia": {
-                        "@ixx": 0.0,
-                        "@ixy": 0.0,
-                        "@ixz": 0.0,
-                        "@iyy": 0.0,
-                        "@iyz": 0.0,
-                        "@izz": 0.0,
+                        "@ixx": str(epsilon),
+                        "@ixy": 0,
+                        "@ixz": 0,
+                        "@iyy": str(epsilon),
+                        "@iyz": 0,
+                        "@izz": str(epsilon),
+                    },
+                },
+                "visual": {
+                    "@name": f"{frame.name}_visual",
+                    "origin": {
+                        "@xyz": "0 0 0",
+                        "@rpy": "0 0 0",
                     },
+                    "geometry": UrdfExporter._rod_geometry_to_xmltodict(
+                        geometry=rod.Geometry(sphere=rod.Sphere(radius=0.0))
+                    ),
                 },
             }
 
-            # Note: the pose of the frame in FrameConvention.Urdf already
-            # refers to the parent link, so we can directly use it.
-            assert frame.pose.relative_to == frame.attached_to
-
-            # New joint connecting the link to which the frame is attached
-            # to the new dummy link.
+            # New joint connecting the detected parent link to the new link
             new_joint = {
-                "@name": f"{frame.attached_to}_to_{dummy_link['@name']}",
+                "@name": f"{parent_link_name}_to_{new_link['@name']}",
                 "@type": "fixed",
-                "parent": {"@link": frame.attached_to},
-                "child": {"@link": dummy_link["@name"]},
+                "parent": {"@link": parent_link_name},
+                "child": {"@link": new_link["@name"]},
                 "origin": {
-                    "@xyz": " ".join(np.array(frame.pose.xyz, dtype=str)),
-                    "@rpy": " ".join(np.array(frame.pose.rpy, dtype=str)),
+                    "@xyz": " ".join(np.array(new_link_pose.xyz, dtype=str)),
+                    "@rpy": " ".join(np.array(new_link_pose.rpy, dtype=str)),
                 },
             }
 
-            logging.debug(
-                "Processing frame '{}': created new dummy chain {}->({})->{}".format(
-                    frame.name,
-                    frame.attached_to,
-                    new_joint["@name"],
-                    dummy_link["@name"],
-                )
-            )
-
-            extra_links_from_frames.append(dummy_link)
+            extra_links_from_frames.append(new_link)
             extra_joints_from_frames.append(new_joint)
 
         # =====================
         # Preserve fixed joints
         # =====================
 
-        # This attribute could either be list of fixed joint names to preserve,
-        # or a boolean to preserve all fixed joints.
-        gazebo_preserve_fixed_joints = copy.copy(self.gazebo_preserve_fixed_joints)
-
-        # If it is a boolean, automatically populate the list with all fixed joints.
         if gazebo_preserve_fixed_joints is True:
             gazebo_preserve_fixed_joints = [
                 j.name for j in model.joints() if j.type == "fixed"
             ]
 
         if gazebo_preserve_fixed_joints is False:
             gazebo_preserve_fixed_joints = []
 
         assert isinstance(gazebo_preserve_fixed_joints, list)
 
-        # Check that all fixed joints to preserve are actually present in the model.
-        for fixed_joint_name in gazebo_preserve_fixed_joints:
-            logging.debug(f"Preserving fixed joint '{fixed_joint_name}'")
-            all_model_joint_names = {j.name for j in model.joints()}
-            if fixed_joint_name not in all_model_joint_names:
-                raise RuntimeError(f"Joint '{fixed_joint_name}' not found in the model")
-
         # ===================
         # Convert SDF to URDF
         # ===================
 
         # In URDF, links are directly attached to the frame of their parent joint
         for link in model.links():
             if link.pose is not None and not np.allclose(link.pose.pose, np.zeros(6)):
@@ -397,31 +374,83 @@
                 # Add the extra joints resulting from the frame->link conversion
                 + extra_joints_from_frames,
                 # Extra gazebo-related elements
                 # https://classic.gazebosim.org/tutorials?tut=ros_urdf
                 # https://github.com/gazebosim/sdformat/issues/199#issuecomment-622127508
                 "gazebo": [
                     {
+                        "@reference": extra_joint["@name"],
+                        "preserveFixedJoint": "true",
+                        "disableFixedJointLumping": "true",
+                    }
+                    for extra_joint in extra_joints_from_frames
+                ]
+                + [
+                    {
                         "@reference": fixed_joint,
                         "preserveFixedJoint": "true",
                         "disableFixedJointLumping": "true",
                     }
                     for fixed_joint in gazebo_preserve_fixed_joints
                 ],
             }
         )
 
         return xmltodict.unparse(
             input_dict=urdf_dict,
-            pretty=self.pretty,
-            indent=self.indent,
+            pretty=pretty,
+            indent=indent,
             short_empty_elements=True,
         )
 
     @staticmethod
+    def _find_parent_link(frame: rod.Frame, model: rod.Model) -> str:
+        links_dict = {l.name: l for l in model.links()}
+        frames_dict = {f.name: f for f in model.frames()}
+        joints_dict = {j.name: j for j in model.joints()}
+        sub_models_dict = {m.name: m for m in model.models()}
+
+        parent = frame
+
+        # SDF frames can be attached to links, joints, the model, or other frames.
+        # - link: consider it as parent
+        # - joint: consider its child as parent (child because is rigidly attached)
+        # - model: consider the canonical link as parent
+        # - frame: recursive call to find its parent
+        while True:
+            if isinstance(parent, rod.Frame) and not parent.name == frame.name:
+                return UrdfExporter._find_parent_link(frame=parent, model=model)
+
+            if isinstance(parent, rod.Link):
+                return parent.name
+
+            if isinstance(parent, rod.Joint):
+                return parent.child
+
+            parent_name = frame.attached_to
+
+            if parent_name in links_dict:
+                parent = links_dict[parent_name]
+
+            elif parent_name in joints_dict:
+                parent = joints_dict[parent_name]
+
+            elif parent_name in frames_dict:
+                parent = frames_dict[parent_name]
+
+            elif parent_name == model.name:
+                return "__model__"
+
+            elif parent_name in sub_models_dict:
+                raise RuntimeError("Model composition not yet supported")
+
+            else:
+                raise RuntimeError(f"Failed to find element with name '{parent_name}'")
+
+    @staticmethod
     def _rod_geometry_to_xmltodict(geometry: rod.Geometry) -> Dict[str, Any]:
         return {
             **(
                 {"box": {"@size": " ".join(np.array(geometry.box.size, dtype=str))}}
                 if geometry.box is not None
                 else dict()
             ),
```

### Comparing `rod-0.2.1.dev57/src/rod/utils/gazebo.py` & `rod-0.2.dev12/src/rod/utils/gazebo.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 import os
 import pathlib
 import shutil
 import subprocess
 import tempfile
+from typing import Union
 
 
 class GazeboHelper:
-    _cached_executable: pathlib.Path = None
-
-    @classmethod
-    def get_gazebo_executable(cls) -> pathlib.Path:
-        if cls._cached_executable is not None:
-            return cls._cached_executable
-
+    @staticmethod
+    def get_gazebo_executable() -> pathlib.Path:
         gz = shutil.which("gz")
         ign = shutil.which("ign")
 
         # Check if either Gazebo Sim or Ignition Gazebo are installed
         if gz is not None:
             executable = pathlib.Path(shutil.which("gz"))
         elif ign is not None:
@@ -25,37 +21,33 @@
             msg = "Failed to find either the 'gz' or 'ign' executables in PATH"
             raise FileNotFoundError(msg)
 
         if not executable.is_file():
             raise TypeError(executable)
 
         # Check if the sdf plugin of the simulator is installed
-        try:
-            subprocess.run(
-                [executable, "sdf", "--help"], check=True, capture_output=True
-            )
-        except subprocess.CalledProcessError as e:
-            msg = f"Failed to find 'sdf' command part of {executable} installation"
-            raise RuntimeError(msg) from e
+        cp = subprocess.run([executable, "sdf", "--help"], capture_output=True)
 
-        cls._cached_executable = executable
+        if cp.returncode != 0:
+            msg = f"Failed to find 'sdf' command part of {executable} installation"
+            raise RuntimeError(msg)
 
-        return cls._cached_executable
+        return executable
 
     @staticmethod
     def has_gazebo() -> bool:
         try:
             _ = GazeboHelper.get_gazebo_executable()
             return True
-        except Exception:
+        except:
             return False
 
     @staticmethod
     def process_model_description_with_sdformat(
-        model_description: str | pathlib.Path,
+        model_description: Union[str, pathlib.Path]
     ) -> str:
         # =============================
         # Select the correct input type
         # =============================
 
         # Handle the max path length depending on the OS
         try:
@@ -69,57 +61,41 @@
 
         # Then, check if it's a string with a path
         elif (
             isinstance(model_description, str)
             and len(model_description) <= MAX_PATH
             and pathlib.Path(model_description).is_file()
         ):
-            model_description_string = pathlib.Path(model_description).read_text(
-                encoding="utf-8"
-            )
+            model_description_string = pathlib.Path(model_description).read_text()
 
         # Finally, it must be a SDF/URDF string
         else:
             model_description_string = model_description
 
         # ================================
         # Process the string with sdformat
         # ================================
 
         # Get the Gazebo Sim executable (raises exception if not found)
         gazebo_executable = GazeboHelper.get_gazebo_executable()
 
-        # Operate on a file stored in a temporary directory.
-        # This is necessary on windows because the file has to be closed before
-        # it can be processed by the sdformat executable.
-        # As soon as 3.12 will be the minimum supported version, we can use just
-        # NamedTemporaryFile with the new delete_on_close=False parameter.
-        with tempfile.TemporaryDirectory() as tmp:
-
-            with tempfile.NamedTemporaryFile(
-                mode="w+", suffix=".xml", dir=tmp, delete=False
-            ) as fp:
-
-                fp.write(model_description_string)
-                fp.close()
-
-            try:
-                cp = subprocess.run(
-                    [str(gazebo_executable), "sdf", "-p", fp.name],
-                    text=True,
-                    stdout=subprocess.PIPE,
-                    stderr=subprocess.STDOUT,
-                    check=True,
-                )
-            except subprocess.CalledProcessError as e:
-                if e.returncode != 0:
-                    print(e.stdout)
-                    raise RuntimeError(
-                        "Failed to process the input with sdformat"
-                    ) from e
+        with tempfile.NamedTemporaryFile(mode="w+") as fp:
+            fp.write(model_description_string)
+            fp.seek(0)
+
+            cp = subprocess.run(
+                [str(gazebo_executable), "sdf", "-p", fp.name],
+                text=True,
+                stdout=subprocess.PIPE,
+                stderr=subprocess.STDOUT,
+            )
+
+        if cp.returncode != 0:
+            print(cp.stdout)
+            raise RuntimeError("Failed to process the input with sdformat")
 
         # Get the resulting SDF string
         sdf_string = cp.stdout
 
         # There might be warnings in the output, so we remove them by finding the
         # first <sdf> tag and ignoring everything before it
         sdf_string = sdf_string[sdf_string.find("<sdf") :]
```

### Comparing `rod-0.2.1.dev57/src/rod/utils/resolve_frames.py` & `rod-0.2.dev12/src/rod/utils/resolve_frames.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-from __future__ import annotations
-
 import functools
-from typing import List
+from typing import List, Union
 
 import numpy as np
 
 import rod
 from rod.sdf.element import Element
 
 
 def update_element_with_pose(
-    element: Element, default_relative_to: str | List[str], explicit_frames: bool
+    element: Element, default_relative_to: Union[str, List[str]], explicit_frames: bool
 ) -> None:
     if not hasattr(element, "pose"):
         raise ValueError("The input element has no 'pose' attribute")
 
     # If there are multiple defaults to detect (e.g. __model__ and <model_name>),
     # we select the first entry of the list as real default
     default_relative_to = (
@@ -50,15 +48,15 @@
 
             # Remove implicit reference frame
             else:
                 element.pose.relative_to = ""
 
 
 def resolve_model_frames(
-    model: rod.Model, is_top_level: bool = True, explicit_frames: bool = True
+    model: "rod.Model", is_top_level: bool = True, explicit_frames: bool = True
 ) -> None:
     # Close the helper for compactness
     update_element = functools.partial(
         update_element_with_pose, explicit_frames=explicit_frames
     )
 
     # Update the model
@@ -67,21 +65,15 @@
             model.pose = rod.Pose(pose=list(np.zeros(6)))
         else:
             assert model.pose.relative_to in {"", None}
     else:
         update_element(element=model, default_relative_to="world")
 
     for frame in model.frames():
-        update_element(
-            element=frame,
-            default_relative_to=(
-                [frame.attached_to] if frame.attached_to is not None else []
-            )
-            + [model.get_canonical_link()],
-        )
+        update_element(element=frame, default_relative_to=["__model__", model.name])
 
     # Update the links and its children elements
     for link in model.links():
         update_element(element=link, default_relative_to=["__model__", model.name])
 
         update_element(element=link.inertial, default_relative_to=link.name)
```

### Comparing `rod-0.2.1.dev57/src/rod/utils/resolve_uris.py` & `rod-0.2.dev12/src/rod/utils/resolve_uris.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from rod import Geometry, logging
 
 
 def resolve_local_uri(uri: str) -> pathlib.Path:
 
     try:
         return resolve_robotics_uri_py.resolve_robotics_uri(uri=uri)
-    except FileNotFoundError:
+    except:
         pass
 
     # Remove the prefix of the URI
     uri_no_prefix = uri.split(sep="://")[-1]
 
     paths = []
     paths += paths_from_environment_variable("GZ_SIM_RESOURCE_PATH")
```

### Comparing `rod-0.2.1.dev57/src/rod.egg-info/PKG-INFO` & `rod-0.2.dev12/src/rod.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rod
-Version: 0.2.1.dev57
+Version: 0.2.dev12
 Summary: The ultimate Python tool for RObot Descriptions processing.
 Home-page: https://github.com/ami-iit/rod
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/rod/releases
 Project-URL: Source, https://github.com/ami-iit/rod
@@ -18,30 +18,30 @@
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Games/Entertainment :: Simulation
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 Requires-Dist: mashumaro
 Requires-Dist: numpy
 Requires-Dist: packaging
 Requires-Dist: resolve-robotics-uri-py
 Requires-Dist: scipy
-Requires-Dist: trimesh
 Requires-Dist: xmltodict
 Provides-Extra: style
 Requires-Dist: black; extra == "style"
 Requires-Dist: isort; extra == "style"
 Provides-Extra: pptree
 Requires-Dist: pptree; extra == "pptree"
 Provides-Extra: test
@@ -77,79 +77,47 @@
 If the URDF model is not compliant, the process errors with clear messages.
 Furthermore, modern versions of the converter produce a SDF description with standardized [pose semantics][pose_semantics],
 that greatly simplifies the life of downstream developers that do not have to guess the reference frame or pose elements.
 Last but not least, the pose semantics also makes SDF aware of the concept of _frame_ that URDF is missing.
 
 ## Features
 
-- Out-of-the-box support for SDFormat specifications [≥ 1.10][sdformat_spec_110].
-- Serialization and deserialization support for SDF files.
-- In-memory layout based on `dataclasses`.
-- Syntax highlighting and auto-completion.
-- Programmatic creation of SDF files from Python APIs.
-- Transitive support for URDF through conversion to SDF.
-- Type validation of elements and attributes.
-- Automatic check of missing required elements.
-- High-performance serialization and deserialization using [`Fatal1ty/mashumaro`][mashumaro].
-- Export in-memory model description to URDF.
+- Out-of-the-box support of SDFormat specifications [≥ 1.7][sdformat_spec_17]
+- Serialization and deserialization support of SDF files
+- In-memory layout based on `dataclasses`
+- Syntax highlighting and auto-completion
+- Support of programmatic creation of SDF files from Python APIs
+- Transitive support of URDF through conversion to SDF[^urdf_to_sdf]
+- Type validation of elements and attributes
+- Automatic check of missing required elements
+- Based on [`Fatal1ty/mashumaro`][mashumaro] for great serialization and deserialization performance
+- Support of exporting the in-memory model description to URDF
 
 [mashumaro]: https://github.com/Fatal1ty/mashumaro
 [open_robotics]: https://www.openrobotics.org/
 [pose_semantics]: http://sdformat.org/tutorials?tut=pose_frame_semantics_proposal&cat=pose_semantics_docs&
 [sdformat]: http://sdformat.org/
 [sdformat_python]: http://sdformat.org/tutorials?tut=python_bindings&cat=developers&
+[sdformat_repo]: https://github.com/gazebosim/sdformat
 [sdformat_spec]: http://sdformat.org/spec
-[sdformat_spec_110]: http://sdformat.org/spec?elem=sdf&ver=1.10
+[sdformat_spec_17]: http://sdformat.org/spec?elem=sdf&ver=1.7
 [urdf]: http://wiki.ros.org/urdf
 
-[^urdf_to_sdf]: Conversion can be done using the `gz sdf` command included in Gazebo Sim starting from Garden.
+[^urdf_to_sdf]: Conversion can be done either using `ign sdf` included in Ignition Gazebo Fortress, or `gz sdf` included in Gazebo Sim starting from Garden.
 
 ## Installation
 
-> [!TIP]
-> ROD does not support out-of-the-box URDF files.
-> URDF support is obtained by converting URDF files to SDF using the `gz sdf` command provided by [sdformat][sdformat_repo] and [gz-tools][gz-tools_repo].
-> Ensure these tools are installed on your system if URDF support is needed (more information below).
-
-[sdformat_repo]: https://github.com/gazebosim/sdformat
-[gz-tools_repo]: https://github.com/gazebosim/gz-tools
-
-<details>
-<summary>Using conda (recommended)</summary>
-
-Installing ROD using `conda` is the recommended way to obtain a complete installation with out-of-the-box support for both URDF and SDF descriptions:
+You can install the project with [`pypa/pip`][pip], preferably in a [virtual environment][venv]:
 
 ```bash
-conda install rod -c conda-forge
+pip install git+https://github.com/ami-iit/rod
 ```
 
-This will automatically install `sdformat` and `gz-tools`. 
-
-</details>
-
-<details>
-<summary>Using pip</summary>
-
-You can install ROD from PyPI with [`pypa/pip`][pip], preferably in a [virtual environment][venv]:
-
-```bash
-pip install rod[all]
-```
-
-If you need URDF support, follow the [official instructions][gazebo_sim_docs] to install Gazebo Sim on your operating system,
-making sure to obtain `sdformat ≥ 13.0` and `gz-tools ≥ 2.0`.
-
-You don't need to install the entire Gazebo Sim suite.
-For example, on Ubuntu, you can only install the `libsdformat13 gz-tools2` packages.
-
 [pip]: https://github.com/pypa/pip/
-[venv]: https://docs.python.org/3.10/tutorial/venv.html
-[gazebo_sim_docs]: https://gazebosim.org/docs
-
-</details>
+[venv]: https://docs.python.org/3.8/tutorial/venv.html
 
 ## Examples
 
 <details>
 <summary>Serialize and deserialize SDF files</summary>
 
 ```python
@@ -252,16 +220,18 @@
 
 ```python
 # Generate first the 'sdf' object with the collapsed code
 # of the section 'Create SDF models programmatically'.
 
 from rod.urdf.exporter import UrdfExporter
 
-urdf_string = UrdfExporter(pretty=True, gazebo_preserve_fixed_joints=True).to_urdf_string(
-    sdf=sdf
+urdf_string = UrdfExporter.sdf_to_urdf_string(
+    sdf=sdf,
+    pretty=True,
+    gazebo_preserve_fixed_joints=True,
 )
 
 print(urdf_string)
 ```
 
 ```xml
 <?xml version="1.0" encoding="utf-8"?>
```

### Comparing `rod-0.2.1.dev57/src/rod.egg-info/SOURCES.txt` & `rod-0.2.dev12/src/rod.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -41,11 +41,9 @@
 src/rod/urdf/__init__.py
 src/rod/urdf/exporter.py
 src/rod/utils/__init__.py
 src/rod/utils/frame_convention.py
 src/rod/utils/gazebo.py
 src/rod/utils/resolve_frames.py
 src/rod/utils/resolve_uris.py
-tests/test_meshbuilder.py
-tests/test_urdf_exporter.py
 tests/test_urdf_parsing.py
 tests/utils_models.py
```

### Comparing `rod-0.2.1.dev57/tests/test_urdf_parsing.py` & `rod-0.2.dev12/tests/test_urdf_parsing.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev57/tests/utils_models.py` & `rod-0.2.dev12/tests/utils_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import enum
 import importlib
 import pathlib
+from typing import Union
 
 
 class Robot(enum.IntEnum):
     Hyq = enum.auto()
     iCub = enum.auto()
     Ur10 = enum.auto()
     Baxter = enum.auto()
@@ -33,15 +34,15 @@
         return f"{name_sc}_description"
 
 
 class ModelFactory:
     """Factory class providing URDF files used by the tests."""
 
     @staticmethod
-    def get_model_description(robot: Robot | str) -> pathlib.Path:
+    def get_model_description(robot: Union[Robot, str]) -> pathlib.Path:
         """
         Get the URDF file of different robots.
 
         Args:
             robot: Robot name of the desired URDF file.
 
         Returns:
```

