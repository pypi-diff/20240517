# Comparing `tmp/rod-0.2.1.dev33.tar.gz` & `tmp/rod-0.2.dev12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rod-0.2.1.dev33.tar", last modified: Fri May 17 12:08:29 2024, max compression
+gzip compressed data, was "rod-0.2.dev12.tar", last modified: Fri Mar  8 14:31:49 2024, max compression
```

## Comparing `rod-0.2.1.dev33.tar` & `rod-0.2.dev12.tar`

### file list

```diff
@@ -1,65 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:08:29.335558 rod-0.2.1.dev33/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:08:29.323558 rod-0.2.1.dev33/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:08:29.327558 rod-0.2.1.dev33/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/.github/workflows/ci_cd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-05-17 12:08:29.335558 rod-0.2.1.dev33/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7109 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-17 12:08:29.339558 rod-0.2.1.dev33/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:08:29.323558 rod-0.2.1.dev33/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:08:29.327558 rod-0.2.1.dev33/src/rod/
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:08:29.331558 rod-0.2.1.dev33/src/rod/builder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/builder/primitive_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/builder/primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:08:29.331558 rod-0.2.1.dev33/src/rod/kinematics/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/kinematics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13757 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/kinematics/kinematic_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/kinematics/tree_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/pretty_printer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:08:29.331558 rod-0.2.1.dev33/src/rod/sdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/sdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/sdf/collision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/sdf/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/sdf/element.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/sdf/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/sdf/joint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/sdf/link.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/sdf/material.py
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/sdf/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/sdf/physics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/sdf/scene.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/sdf/sdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/sdf/visual.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/sdf/world.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:08:29.331558 rod-0.2.1.dev33/src/rod/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/tree/directed_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/tree/tree_elements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:08:29.335558 rod-0.2.1.dev33/src/rod/urdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/urdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19757 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/urdf/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:08:29.335558 rod-0.2.1.dev33/src/rod/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11789 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/utils/frame_convention.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/utils/gazebo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/utils/resolve_frames.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/src/rod/utils/resolve_uris.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:08:29.335558 rod-0.2.1.dev33/src/rod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-05-17 12:08:29.000000 rod-0.2.1.dev33/src/rod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-17 12:08:29.000000 rod-0.2.1.dev33/src/rod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 12:08:29.000000 rod-0.2.1.dev33/src/rod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 12:08:29.000000 rod-0.2.1.dev33/src/rod.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-17 12:08:29.000000 rod-0.2.1.dev33/src/rod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-17 12:08:29.000000 rod-0.2.1.dev33/src/rod.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:08:29.335558 rod-0.2.1.dev33/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/tests/test_meshbuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/tests/test_urdf_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/tests/test_urdf_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-17 12:08:15.000000 rod-0.2.1.dev33/tests/utils_models.py
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

### Comparing `rod-0.2.1.dev33/.github/workflows/ci_cd.yml` & `rod-0.2.dev12/.github/workflows/ci_cd.yml`

 * *Files 20% similar despite different names*

```diff
@@ -100,19 +100,15 @@
           channels: conda-forge
           channel-priority: true
 
       - name: Install system dependencies
         if: matrix.type == 'apt'
         run: |
           sudo apt-get update
-          sudo apt-get install lsb-release wget gnupg
-          wget https://packages.osrfoundation.org/gazebo.gpg -O /usr/share/keyrings/pkgs-osrf-archive-keyring.gpg
-          echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/pkgs-osrf-archive-keyring.gpg] http://packages.osrfoundation.org/gazebo/ubuntu-stable $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/gazebo-stable.list > /dev/null
-          sudo apt-get update
-          sudo apt-get install --no-install-recommends libsdformat13 gz-tools2
+          sudo apt-get install -y --no-install-recommends gazebo
 
       - name: Install conda dependencies
         if: matrix.type == 'conda'
         run: |
           mamba install -y \
             coloredlogs \
             mashumaro \
@@ -122,16 +118,15 @@
             scipy \
             xmltodict \
             black \
             isort \
             pptree \
             idyntree \
             pytest \
-            robot_descriptions \
-            trimesh
+            robot_descriptions
             # pytest-icdiff \  # creates problems on macOS
           mamba install -y gz-sim7 idyntree
 
       - name: Download Python packages
         uses: actions/download-artifact@v3
         with:
           path: dist
```

### Comparing `rod-0.2.1.dev33/.github/workflows/style.yml` & `rod-0.2.dev12/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev33/.gitignore` & `rod-0.2.dev12/.gitignore`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev33/LICENSE` & `rod-0.2.dev12/LICENSE`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev33/PKG-INFO` & `rod-0.2.dev12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rod
-Version: 0.2.1.dev33
+Version: 0.2.dev12
 Summary: The ultimate Python tool for RObot Descriptions processing.
 Home-page: https://github.com/ami-iit/rod
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/rod/releases
 Project-URL: Source, https://github.com/ami-iit/rod
@@ -34,15 +34,14 @@
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
```

### Comparing `rod-0.2.1.dev33/README.md` & `rod-0.2.dev12/README.md`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev33/setup.cfg` & `rod-0.2.dev12/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
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

### Comparing `rod-0.2.1.dev33/src/rod/builder/primitive_builder.py` & `rod-0.2.dev12/src/rod/builder/primitive_builder.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev33/src/rod/kinematics/kinematic_tree.py` & `rod-0.2.dev12/src/rod/kinematics/kinematic_tree.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev33/src/rod/kinematics/tree_transforms.py` & `rod-0.2.dev12/src/rod/kinematics/tree_transforms.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,23 +10,26 @@
 
 
 @dataclasses.dataclass
 class TreeTransforms:
     kinematic_tree: KinematicTree = dataclasses.dataclass(init=False)
 
     @staticmethod
-    def build(model: "rod.Model", is_top_level: bool = True) -> "TreeTransforms":
-
-        # Operate on a deep copy of the model to avoid side effects.
+    def build(
+        model: "rod.Model",
+        is_top_level: bool = True,
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
         if name == TreeFrame.WORLD:
             return np.eye(4)
@@ -47,58 +50,34 @@
 
             # Compute the world-to-node transform
             # TODO: this assumes all joint positions to be 0
             W_H_E = W_H_x @ x_H_E
 
             return W_H_E
 
-        if name in self.kinematic_tree.link_names():
-
-            element = self.kinematic_tree.links_dict[name]
-
+        if (
+            name in self.kinematic_tree.link_names()
+            or name in self.kinematic_tree.frame_names()
+        ):
+            element = (
+                self.kinematic_tree.links_dict[name]
+                if name in self.kinematic_tree.link_names()
+                else self.kinematic_tree.frames_dict[name]
+            )
             assert element.name() == name
-            assert element._source.pose.relative_to not in {"", None}
-
-            # Get the pose of the frame in which the link's pose is expressed.
-            x_H_L = element._source.pose.transform()
-            W_H_x = self.transform(name=element._source.pose.relative_to)
-
-            # Compute the world transform of the link.
-            W_H_L = W_H_x @ x_H_L
-            return W_H_L
-
-        if name in self.kinematic_tree.frame_names():
-
-            element = self.kinematic_tree.frames_dict[name]
 
-            assert element.name() == name
+            # Get the pose of the frame in which the node's pose is expressed
             assert element._source.pose.relative_to not in {"", None}
-
-            # Get the pose of the frame in which the frame's pose is expressed.
-            x_H_F = element._source.pose.transform()
+            x_H_N = element._source.pose.transform()
             W_H_x = self.transform(name=element._source.pose.relative_to)
 
-            # Compute the world transform of the frame.
-            W_H_F = W_H_x @ x_H_F
-            return W_H_F
+            # Compute and cache the world-to-node transform
+            W_H_N = W_H_x @ x_H_N
+
+            return W_H_N
 
         raise ValueError(name)
 
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

### Comparing `rod-0.2.1.dev33/src/rod/logging.py` & `rod-0.2.dev12/src/rod/logging.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev33/src/rod/pretty_printer.py` & `rod-0.2.dev12/src/rod/pretty_printer.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev33/src/rod/sdf/common.py` & `rod-0.2.dev12/src/rod/sdf/common.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev33/src/rod/sdf/element.py` & `rod-0.2.dev12/src/rod/sdf/element.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev33/src/rod/sdf/geometry.py` & `rod-0.2.dev12/src/rod/sdf/geometry.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev33/src/rod/sdf/joint.py` & `rod-0.2.dev12/src/rod/sdf/joint.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev33/src/rod/sdf/link.py` & `rod-0.2.dev12/src/rod/sdf/link.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev33/src/rod/sdf/material.py` & `rod-0.2.dev12/src/rod/sdf/material.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev33/src/rod/sdf/model.py` & `rod-0.2.dev12/src/rod/sdf/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,19 +154,17 @@
         )
 
     def switch_frame_convention(
         self,
         frame_convention: "rod.FrameConvention",
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

### Comparing `rod-0.2.1.dev33/src/rod/sdf/physics.py` & `rod-0.2.dev12/src/rod/sdf/physics.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev33/src/rod/sdf/scene.py` & `rod-0.2.dev12/src/rod/sdf/scene.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev33/src/rod/sdf/sdf.py` & `rod-0.2.dev12/src/rod/sdf/sdf.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev33/src/rod/sdf/world.py` & `rod-0.2.dev12/src/rod/sdf/world.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev33/src/rod/tree/directed_tree.py` & `rod-0.2.dev12/src/rod/tree/directed_tree.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev33/src/rod/tree/tree_elements.py` & `rod-0.2.dev12/src/rod/tree/tree_elements.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev33/src/rod/urdf/exporter.py` & `rod-0.2.dev12/src/rod/urdf/exporter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,86 +1,61 @@
 import abc
 import copy
-import dataclasses
-from typing import Any, ClassVar, Dict, List, Set, Union
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
-    gazebo_preserve_fixed_joints: Union[bool, List[str]] = False
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
-        sdf: Union[rod.Sdf, rod.Model],
+        sdf: rod.Sdf | rod.Model,
         pretty: bool = False,
         indent: str = "  ",
         gazebo_preserve_fixed_joints: Union[bool, List[str]] = False,
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
-    def to_urdf_string(self, sdf: Union[rod.Sdf, rod.Model]) -> str:
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

### Comparing `rod-0.2.1.dev33/src/rod/utils/gazebo.py` & `rod-0.2.dev12/src/rod/utils/gazebo.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,27 +74,17 @@
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
+        with tempfile.NamedTemporaryFile(mode="w+") as fp:
+            fp.write(model_description_string)
+            fp.seek(0)
 
             cp = subprocess.run(
                 [str(gazebo_executable), "sdf", "-p", fp.name],
                 text=True,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.STDOUT,
             )
```

### Comparing `rod-0.2.1.dev33/src/rod/utils/resolve_frames.py` & `rod-0.2.dev12/src/rod/utils/resolve_frames.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,21 +65,15 @@
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

### Comparing `rod-0.2.1.dev33/src/rod/utils/resolve_uris.py` & `rod-0.2.dev12/src/rod/utils/resolve_uris.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev33/src/rod.egg-info/PKG-INFO` & `rod-0.2.dev12/src/rod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rod
-Version: 0.2.1.dev33
+Version: 0.2.dev12
 Summary: The ultimate Python tool for RObot Descriptions processing.
 Home-page: https://github.com/ami-iit/rod
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/rod/releases
 Project-URL: Source, https://github.com/ami-iit/rod
@@ -34,15 +34,14 @@
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
```

### Comparing `rod-0.2.1.dev33/src/rod.egg-info/SOURCES.txt` & `rod-0.2.dev12/src/rod.egg-info/SOURCES.txt`

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

### Comparing `rod-0.2.1.dev33/tests/test_urdf_parsing.py` & `rod-0.2.dev12/tests/test_urdf_parsing.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev33/tests/utils_models.py` & `rod-0.2.dev12/tests/utils_models.py`

 * *Files identical despite different names*

