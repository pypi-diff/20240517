# Comparing `tmp/rod-0.2.1.dev16.tar.gz` & `tmp/rod-0.2.dev12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rod-0.2.1.dev16.tar", last modified: Thu May 16 13:21:12 2024, max compression
+gzip compressed data, was "rod-0.2.dev12.tar", last modified: Fri Mar  8 14:31:49 2024, max compression
```

## Comparing `rod-0.2.1.dev16.tar` & `rod-0.2.dev12.tar`

### file list

```diff
@@ -1,64 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:21:12.529118 rod-0.2.1.dev16/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:21:12.517118 rod-0.2.1.dev16/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:21:12.521118 rod-0.2.1.dev16/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/.github/workflows/ci_cd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-05-16 13:21:12.529118 rod-0.2.1.dev16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7109 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-16 13:21:12.529118 rod-0.2.1.dev16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:21:12.517118 rod-0.2.1.dev16/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:21:12.521118 rod-0.2.1.dev16/src/rod/
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:21:12.521118 rod-0.2.1.dev16/src/rod/builder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/builder/primitive_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/builder/primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:21:12.521118 rod-0.2.1.dev16/src/rod/kinematics/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/kinematics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13757 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/kinematics/kinematic_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/kinematics/tree_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/pretty_printer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:21:12.525118 rod-0.2.1.dev16/src/rod/sdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/sdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/sdf/collision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/sdf/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/sdf/element.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/sdf/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/sdf/joint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/sdf/link.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/sdf/material.py
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/sdf/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/sdf/physics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/sdf/scene.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/sdf/sdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/sdf/visual.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/sdf/world.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:21:12.525118 rod-0.2.1.dev16/src/rod/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/tree/directed_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/tree/tree_elements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:21:12.525118 rod-0.2.1.dev16/src/rod/urdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/urdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21139 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/urdf/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:21:12.525118 rod-0.2.1.dev16/src/rod/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8977 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/utils/frame_convention.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/utils/gazebo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/utils/resolve_frames.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/src/rod/utils/resolve_uris.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:21:12.525118 rod-0.2.1.dev16/src/rod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-05-16 13:21:12.000000 rod-0.2.1.dev16/src/rod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-16 13:21:12.000000 rod-0.2.1.dev16/src/rod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:21:12.000000 rod-0.2.1.dev16/src/rod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:21:12.000000 rod-0.2.1.dev16/src/rod.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-16 13:21:12.000000 rod-0.2.1.dev16/src/rod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-16 13:21:12.000000 rod-0.2.1.dev16/src/rod.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:21:12.525118 rod-0.2.1.dev16/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/tests/test_meshbuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/tests/test_urdf_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-16 13:20:58.000000 rod-0.2.1.dev16/tests/utils_models.py
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

### Comparing `rod-0.2.1.dev16/.github/workflows/ci_cd.yml` & `rod-0.2.dev12/.github/workflows/ci_cd.yml`

 * *Files 1% similar despite different names*

```diff
@@ -118,16 +118,15 @@
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

### Comparing `rod-0.2.1.dev16/.github/workflows/style.yml` & `rod-0.2.dev12/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/.gitignore` & `rod-0.2.dev12/.gitignore`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/LICENSE` & `rod-0.2.dev12/LICENSE`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/PKG-INFO` & `rod-0.2.dev12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rod
-Version: 0.2.1.dev16
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

### Comparing `rod-0.2.1.dev16/README.md` & `rod-0.2.dev12/README.md`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/setup.cfg` & `rod-0.2.dev12/setup.cfg`

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

### Comparing `rod-0.2.1.dev16/src/rod/__init__.py` & `rod-0.2.dev12/src/rod/__init__.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/src/rod/builder/primitive_builder.py` & `rod-0.2.dev12/src/rod/builder/primitive_builder.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/src/rod/kinematics/kinematic_tree.py` & `rod-0.2.dev12/src/rod/kinematics/kinematic_tree.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/src/rod/kinematics/tree_transforms.py` & `rod-0.2.dev12/src/rod/kinematics/tree_transforms.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/src/rod/logging.py` & `rod-0.2.dev12/src/rod/logging.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/src/rod/pretty_printer.py` & `rod-0.2.dev12/src/rod/pretty_printer.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/src/rod/sdf/common.py` & `rod-0.2.dev12/src/rod/sdf/common.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/src/rod/sdf/element.py` & `rod-0.2.dev12/src/rod/sdf/element.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/src/rod/sdf/geometry.py` & `rod-0.2.dev12/src/rod/sdf/geometry.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/src/rod/sdf/joint.py` & `rod-0.2.dev12/src/rod/sdf/joint.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/src/rod/sdf/link.py` & `rod-0.2.dev12/src/rod/sdf/link.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/src/rod/sdf/material.py` & `rod-0.2.dev12/src/rod/sdf/material.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/src/rod/sdf/model.py` & `rod-0.2.dev12/src/rod/sdf/model.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/src/rod/sdf/physics.py` & `rod-0.2.dev12/src/rod/sdf/physics.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/src/rod/sdf/scene.py` & `rod-0.2.dev12/src/rod/sdf/scene.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/src/rod/sdf/sdf.py` & `rod-0.2.dev12/src/rod/sdf/sdf.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/src/rod/sdf/world.py` & `rod-0.2.dev12/src/rod/sdf/world.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/src/rod/tree/directed_tree.py` & `rod-0.2.dev12/src/rod/tree/directed_tree.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/src/rod/tree/tree_elements.py` & `rod-0.2.dev12/src/rod/tree/tree_elements.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/src/rod/urdf/exporter.py` & `rod-0.2.dev12/src/rod/urdf/exporter.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/src/rod/utils/frame_convention.py` & `rod-0.2.dev12/src/rod/utils/frame_convention.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/src/rod/utils/gazebo.py` & `rod-0.2.dev12/src/rod/utils/gazebo.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/src/rod/utils/resolve_frames.py` & `rod-0.2.dev12/src/rod/utils/resolve_frames.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/src/rod/utils/resolve_uris.py` & `rod-0.2.dev12/src/rod/utils/resolve_uris.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/src/rod.egg-info/PKG-INFO` & `rod-0.2.dev12/src/rod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rod
-Version: 0.2.1.dev16
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

### Comparing `rod-0.2.1.dev16/src/rod.egg-info/SOURCES.txt` & `rod-0.2.dev12/src/rod.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -41,10 +41,9 @@
 src/rod/urdf/__init__.py
 src/rod/urdf/exporter.py
 src/rod/utils/__init__.py
 src/rod/utils/frame_convention.py
 src/rod/utils/gazebo.py
 src/rod/utils/resolve_frames.py
 src/rod/utils/resolve_uris.py
-tests/test_meshbuilder.py
 tests/test_urdf_parsing.py
 tests/utils_models.py
```

### Comparing `rod-0.2.1.dev16/tests/test_urdf_parsing.py` & `rod-0.2.dev12/tests/test_urdf_parsing.py`

 * *Files identical despite different names*

### Comparing `rod-0.2.1.dev16/tests/utils_models.py` & `rod-0.2.dev12/tests/utils_models.py`

 * *Files identical despite different names*

