# Comparing `tmp/toon3d-0.0.3.tar.gz` & `tmp/toon3d-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toon3d-0.0.3.tar", last modified: Thu May 16 20:20:55 2024, max compression
+gzip compressed data, was "toon3d-0.0.4.tar", last modified: Thu May 16 21:56:50 2024, max compression
```

## Comparing `toon3d-0.0.3.tar` & `toon3d-0.0.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 20:20:55.791628 toon3d-0.0.3/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)      906 2024-05-16 20:20:55.791628 toon3d-0.0.3/PKG-INFO
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     5271 2024-05-16 20:18:19.000000 toon3d-0.0.3/README.md
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     1296 2024-05-16 20:19:43.000000 toon3d-0.0.3/pyproject.toml
--rw-r--r--   0 ethanweber (1000282) users    (1000001)       38 2024-05-16 20:20:55.791628 toon3d-0.0.3/setup.cfg
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 20:20:55.787628 toon3d-0.0.3/toon3d/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)        0 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/__init__.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     1728 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/color_palette.py
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 20:20:55.787628 toon3d-0.0.3/toon3d/configs/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     1475 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/configs/prompts.py
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 20:20:55.787628 toon3d-0.0.3/toon3d/generative/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)    10358 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/generative/marigold.py
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 20:20:55.787628 toon3d-0.0.3/toon3d/scripts/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     4646 2024-05-10 20:12:48.000000 toon3d-0.0.3/toon3d/scripts/colmap_with_corrs.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     6596 2024-05-16 05:41:22.000000 toon3d-0.0.3/toon3d/scripts/download_data.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     8611 2024-05-10 21:53:19.000000 toon3d-0.0.3/toon3d/scripts/process_data.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)    34579 2024-05-16 20:19:04.000000 toon3d-0.0.3/toon3d/scripts/run.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     1185 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/scripts/server.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     4685 2024-05-13 05:11:25.000000 toon3d-0.0.3/toon3d/scripts/viser_vis.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     2847 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/toon3d_config.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     5939 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/toon3d_datamanager.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     1492 2024-05-16 20:15:55.000000 toon3d-0.0.3/toon3d/toon3d_dataparser.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)    12830 2024-05-16 20:15:55.000000 toon3d-0.0.3/toon3d/toon3d_model.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     3495 2024-05-16 20:15:55.000000 toon3d-0.0.3/toon3d/toon3d_pipeline.py
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 20:20:55.791628 toon3d-0.0.3/toon3d/utils/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     3376 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/utils/camera_utils.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)    12545 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/utils/colmap_database.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     1514 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/utils/convert_points.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     3008 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/utils/depth_utils.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     2699 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/utils/draw_utils.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     4322 2024-05-10 21:50:37.000000 toon3d-0.0.3/toon3d/utils/image_processing_utils.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     2108 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/utils/losses.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     1767 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/utils/novel_view_samplers.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     2675 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/utils/tsdf_utils.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     3316 2024-03-26 21:11:46.000000 toon3d-0.0.3/toon3d/utils/viser_utils.py
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 20:20:55.791628 toon3d-0.0.3/toon3d/warp/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     3415 2024-04-12 21:13:30.000000 toon3d-0.0.3/toon3d/warp/arap_utils.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)    11952 2024-05-16 20:15:55.000000 toon3d-0.0.3/toon3d/warp/warp_mesh.py
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 20:20:55.783628 toon3d-0.0.3/toon3d-labeler/
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 20:20:55.783628 toon3d-0.0.3/toon3d-labeler/node_modules/
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 20:20:55.783628 toon3d-0.0.3/toon3d-labeler/node_modules/flatted/
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 20:20:55.787628 toon3d-0.0.3/toon3d-labeler/node_modules/flatted/python/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     3879 2024-04-30 22:25:05.000000 toon3d-0.0.3/toon3d-labeler/node_modules/flatted/python/flatted.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     2129 2024-04-30 22:25:05.000000 toon3d-0.0.3/toon3d-labeler/node_modules/flatted/python/test.py
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 20:20:55.787628 toon3d-0.0.3/toon3d-spaces/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)    11016 2024-05-13 22:54:51.000000 toon3d-0.0.3/toon3d-spaces/app.py
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 20:20:55.791628 toon3d-0.0.3/toon3d.egg-info/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)      906 2024-05-16 20:20:55.000000 toon3d-0.0.3/toon3d.egg-info/PKG-INFO
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     1086 2024-05-16 20:20:55.000000 toon3d-0.0.3/toon3d.egg-info/SOURCES.txt
--rw-r--r--   0 ethanweber (1000282) users    (1000001)        1 2024-05-16 20:20:55.000000 toon3d-0.0.3/toon3d.egg-info/dependency_links.txt
--rw-r--r--   0 ethanweber (1000282) users    (1000001)      393 2024-05-16 20:20:55.000000 toon3d-0.0.3/toon3d.egg-info/entry_points.txt
--rw-r--r--   0 ethanweber (1000282) users    (1000001)      315 2024-05-16 20:20:55.000000 toon3d-0.0.3/toon3d.egg-info/requires.txt
--rw-r--r--   0 ethanweber (1000282) users    (1000001)       56 2024-05-16 20:20:55.000000 toon3d-0.0.3/toon3d.egg-info/top_level.txt
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 21:56:50.640437 toon3d-0.0.4/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)      906 2024-05-16 21:56:50.636437 toon3d-0.0.4/PKG-INFO
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     4118 2024-05-16 21:40:23.000000 toon3d-0.0.4/README.md
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     1296 2024-05-16 21:56:18.000000 toon3d-0.0.4/pyproject.toml
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)       38 2024-05-16 21:56:50.640437 toon3d-0.0.4/setup.cfg
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 21:56:50.632437 toon3d-0.0.4/toon3d/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)        0 2024-03-15 01:48:57.000000 toon3d-0.0.4/toon3d/__init__.py
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 21:56:50.636437 toon3d-0.0.4/toon3d/configs/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     1475 2024-03-15 01:48:57.000000 toon3d-0.0.4/toon3d/configs/prompts.py
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 21:56:50.636437 toon3d-0.0.4/toon3d/generative/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)    10358 2024-03-15 01:48:57.000000 toon3d-0.0.4/toon3d/generative/marigold.py
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 21:56:50.636437 toon3d-0.0.4/toon3d/scripts/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     4646 2024-05-10 20:12:48.000000 toon3d-0.0.4/toon3d/scripts/colmap_with_corrs.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     6596 2024-05-16 05:41:22.000000 toon3d-0.0.4/toon3d/scripts/download_data.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     8826 2024-05-16 21:55:20.000000 toon3d-0.0.4/toon3d/scripts/process_data.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)    30267 2024-05-16 21:56:28.000000 toon3d-0.0.4/toon3d/scripts/render.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)    25930 2024-05-16 21:09:30.000000 toon3d-0.0.4/toon3d/scripts/run.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     1185 2024-03-15 01:48:57.000000 toon3d-0.0.4/toon3d/scripts/server.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     4685 2024-05-13 05:11:25.000000 toon3d-0.0.4/toon3d/scripts/viser_vis.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     2847 2024-03-15 01:48:57.000000 toon3d-0.0.4/toon3d/toon3d_config.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)      945 2024-05-16 21:56:28.000000 toon3d-0.0.4/toon3d/toon3d_datamanager.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     1492 2024-05-16 20:15:55.000000 toon3d-0.0.4/toon3d/toon3d_dataparser.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     9292 2024-05-16 21:30:00.000000 toon3d-0.0.4/toon3d/toon3d_model.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     3077 2024-05-16 21:30:00.000000 toon3d-0.0.4/toon3d/toon3d_pipeline.py
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 21:56:50.636437 toon3d-0.0.4/toon3d/utils/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     3376 2024-03-15 01:48:57.000000 toon3d-0.0.4/toon3d/utils/camera_utils.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)    12545 2024-03-15 01:48:57.000000 toon3d-0.0.4/toon3d/utils/colmap_database.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     1514 2024-03-15 01:48:57.000000 toon3d-0.0.4/toon3d/utils/convert_points.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     3008 2024-03-15 01:48:57.000000 toon3d-0.0.4/toon3d/utils/depth_utils.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     2699 2024-03-15 01:48:57.000000 toon3d-0.0.4/toon3d/utils/draw_utils.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     4366 2024-05-16 21:53:25.000000 toon3d-0.0.4/toon3d/utils/image_processing_utils.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     7194 2024-05-16 21:30:00.000000 toon3d-0.0.4/toon3d/utils/io_utils.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     2108 2024-03-15 01:48:57.000000 toon3d-0.0.4/toon3d/utils/losses.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     1767 2024-03-15 01:48:57.000000 toon3d-0.0.4/toon3d/utils/novel_view_samplers.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     3316 2024-03-26 21:11:46.000000 toon3d-0.0.4/toon3d/utils/viser_utils.py
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 21:56:50.636437 toon3d-0.0.4/toon3d/warp/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     3415 2024-04-12 21:13:30.000000 toon3d-0.0.4/toon3d/warp/arap_utils.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)    11952 2024-05-16 20:15:55.000000 toon3d-0.0.4/toon3d/warp/warp_mesh.py
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 21:56:50.632437 toon3d-0.0.4/toon3d-labeler/
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 21:56:50.632437 toon3d-0.0.4/toon3d-labeler/node_modules/
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 21:56:50.632437 toon3d-0.0.4/toon3d-labeler/node_modules/flatted/
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 21:56:50.632437 toon3d-0.0.4/toon3d-labeler/node_modules/flatted/python/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     3879 2024-04-30 22:25:05.000000 toon3d-0.0.4/toon3d-labeler/node_modules/flatted/python/flatted.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     2129 2024-04-30 22:25:05.000000 toon3d-0.0.4/toon3d-labeler/node_modules/flatted/python/test.py
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 21:56:50.632437 toon3d-0.0.4/toon3d-spaces/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)    11077 2024-05-16 21:56:03.000000 toon3d-0.0.4/toon3d-spaces/app.py
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 21:56:50.636437 toon3d-0.0.4/toon3d.egg-info/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)      906 2024-05-16 21:56:49.000000 toon3d-0.0.4/toon3d.egg-info/PKG-INFO
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     1085 2024-05-16 21:56:50.000000 toon3d-0.0.4/toon3d.egg-info/SOURCES.txt
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)        1 2024-05-16 21:56:49.000000 toon3d-0.0.4/toon3d.egg-info/dependency_links.txt
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)      393 2024-05-16 21:56:49.000000 toon3d-0.0.4/toon3d.egg-info/entry_points.txt
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)      315 2024-05-16 21:56:49.000000 toon3d-0.0.4/toon3d.egg-info/requires.txt
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)       56 2024-05-16 21:56:49.000000 toon3d-0.0.4/toon3d.egg-info/top_level.txt
```

### Comparing `toon3d-0.0.3/PKG-INFO` & `toon3d-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toon3d
-Version: 0.0.3
+Version: 0.0.4
 Summary: toon3d package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7.3
 Requires-Dist: black
 Requires-Dist: h5py
 Requires-Dist: mediapy
```

### Comparing `toon3d-0.0.3/README.md` & `toon3d-0.0.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 For example,
 
 ```bash
 tnd-process-data initialize --dataset bobs-burgers-dining --input_path data/images/bobs-burgers-dining
 ```
 
-If you want to add more images to your dataset, run this
+If you want to add more images to your dataset after initializing it, run this
 
 ```bash
 tnd-process-data add --dataset bobs-burgers-dining --input_path data/images/more-bobs-burgers-dining-photos
 ```
 
 ## Label images
 
@@ -74,97 +74,47 @@
 
 ```bash
 tnd-server --path data/processed --port 8000
 ```
 
 Now, open your processed dataset and annotate.
 
-Navigate to https://labeler.toon3d.studio/?path=http://localhost:8000/bobs-burgers-dining in our case. Or, if you are developing locally then http://localhost:3000/?path=http://localhost:8000/bobs-burgers-dining.
+Navigate to https://labeler.toon3d.studio/?path=http://localhost:8000/bobs-burgers-dining in this case.
 
 ## Run structure from motion!
 
 Now we can run our method to get a dense 3D reconstruction for novel-view synthesis.
 
-```bash
-tnd-run --help
-```
-
 For example,
 
 ```bash
 tnd-run --dataset bobs-burgers-dining
 ```
 
-# Run multi-view stereo!
+# Run dense reconstruction!
 
 For example,
 
 ```bash
 ns-train toon3d --data data/nerfstudio/bobs-burgers-dining
 ```
 
-To train a depth-nerfacto, run the following:
-
-```bash
-ns-train depth-nerfacto --data data/nerfstudio/bobs-burgers-dining \
-    --pipeline.use_visibility_loss True \
-    --pipeline.visibility_min_views 1 \
-    --pipeline.model.is_euclidean_depth True \
-    nerfstudio-data \
-    --depth_unit_scale_factor 1.0
-```
-
-<details>
-<summary><strong>(Optional) Regularize with a fine-tuned diffusion model</strong></summary>
-<br>
-
-<blockquote style="margin: 0 0 0 20px; border-left: 3px solid #4CAF50; padding: 0 10px;">
-
-We can fine-tune a diffusion model on our data, and then we can apply it while optimizing the 3D model. Check out the wandb logs to see training progress.
-
-```bash
-python toon3d/scripts/finetune.py --dataset [dataset]
-```
-
-
-For exmaple,
-
-```bash
-python toon3d/scripts/finetune.py --dataset bobs-burgers-dining
-```
-
-Now, optimize with the fine-tuned model as a prior.
-
-```bash
-TODO!
-```
-</blockquote>
-</details>
-<br>
-
 Render a camera path that you created
 
 ```bash
 tnd-render camera-path --load-config [load-config] --camera-path-filename [camera-path-filename] --output-path [output-path].mp4
 ```
 
 Render videos between training views
 
 ```bash
 tnd-render interpolate --load-config [load-config] --output-path [output-path]
-``` 
-
-# Test cases
-
-```bash
-pytest tests
 ```
 
 # Project structure
 
 The `outputs` folder is organized according to the types of experiments conducted.
 
 ```bash
 outputs/[dataset]/run/[timestamp]       # For SfM experiments
-outputs/[dataset]/finetune/[timestamp]  # For fine-tuning experiments
 outputs/[dataset]/toon3d/[timestamp]    # For MVS experiments
 ```
```

### Comparing `toon3d-0.0.3/pyproject.toml` & `toon3d-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "toon3d"
-version = "0.0.3"
+version = "0.0.4"
 description = "toon3d package"
 requires-python = ">=3.7.3"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python",
 ]
 dependencies = [
```

### Comparing `toon3d-0.0.3/toon3d/configs/prompts.py` & `toon3d-0.0.4/toon3d/configs/prompts.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.3/toon3d/generative/marigold.py` & `toon3d-0.0.4/toon3d/generative/marigold.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.3/toon3d/scripts/colmap_with_corrs.py` & `toon3d-0.0.4/toon3d/scripts/colmap_with_corrs.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.3/toon3d/scripts/download_data.py` & `toon3d-0.0.4/toon3d/scripts/download_data.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.3/toon3d/scripts/process_data.py` & `toon3d-0.0.4/toon3d/scripts/process_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,26 +35,30 @@
     compute_segment_anything: bool = True
     compute_lines: bool = False
     update_segment_anything: bool = False
     update_lines: bool = False
     skip_image_resizing: bool = False
     add_to_existing: bool = False
     sam_checkpoint_prefix: str = "data/sam-checkpoints"
+    sam_points_per_side: int = 32
+    """Set to higher, e.g., 128 for higher quality but slower."""
 
 
 @dataclass
 class InitializeProcessData(ProcessData):
     """Initialize process data
     
     This will take a folder of images and process them.
     """
 
     def run(self):
         """check here"""
         device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
+        
+        self.data_prefix.mkdir(exist_ok=True, parents=True)
 
         dataset_path = self.data_prefix / self.dataset
         images_path = dataset_path / "images"
         depths_path = dataset_path / "depths"
         depth_images_path = dataset_path / "depth-images"
 
         if self.add_to_existing:
@@ -135,15 +139,15 @@
             metadata = json.loads(metadata_path.read_text())
 
         do_segment_anything = self.compute_segment_anything and (self.add_to_existing or self.update_segment_anything or compute_metadata or "masks" not in metadata["frames"][0])
         do_lines = self.compute_lines and (self.add_to_existing or self.update_lines or compute_metadata or "lines" not in metadata["frames"][0])
         
         if do_segment_anything:
             CONSOLE.log("[bold yellow]Running Segment Anything... (This may take a while)")
-            segments = generate_segments(images, device, sam_checkpoint_prefix=self.sam_checkpoint_prefix)
+            segments = generate_segments(images, device, sam_checkpoint_prefix=self.sam_checkpoint_prefix, sam_points_per_side=self.sam_points_per_side)
             CONSOLE.log("[bold green]:tada: Done Segmenting Masks.")
             for i, segment in enumerate(segments):
                 metadata["frames"][si+i]["masks"] = segment
         elif self.compute_segment_anything:
             CONSOLE.log("[bold yellow]Segment Anything Masks already exist. Use --update-segment-anything to recompute.")
         
         if do_lines:
```

### Comparing `toon3d-0.0.3/toon3d/scripts/run.py` & `toon3d-0.0.4/toon3d/scripts/run.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,211 +1,41 @@
 """
 Main script.
 """
 
 from pathlib import Path
 import json
 from datetime import datetime
-import io
+
 
 import cv2 
-import kornia
 import mediapy
 import numpy as np
 import torch
 import torch.nn as nn
 from tqdm import tqdm
 import shutil
 import cv2
 
 import tyro
 import viser
 from toon3d.utils.draw_utils import get_images_with_keypoints
 from toon3d.utils.viser_utils import view_pcs_cameras
 from toon3d.utils.camera_utils import Cameras
+from toon3d.utils.io_utils import make_transforms_json, make_dense_points_3d, make_plys, load_dataset
 from toon3d.warp.warp_mesh import WarpMesh, draw_tris, draw_points, FrameMeshes, get_simplices
 from toon3d.warp.arap_utils import face_verts_arap_loss, calc_area_loss, signed_areas
-from toon3d.utils.depth_utils import create_discontinuity_mask
 
 
-from nerfstudio.utils.colormaps import apply_depth_colormap
 from nerfstudio.utils.rich_utils import CONSOLE
 
 
-def make_transforms_json(fxs, fys, Rs, ts, widths, heights):
-    fxs, fys, Rs, ts = fxs.detach().cpu(), fys.detach().cpu(), Rs.detach().cpu(), ts.detach().cpu()
-    transforms = {
-        "camera_model": "OPENCV",
-        "ply_file_path": "plys/all.ply",
-        "points": "points/points.pt",
-        "points_mask": "points/points_mask.pt",
-        "meshes_points": "meshes/meshes_points.pt",
-        "warped_meshes_points": "meshes/warped_meshes_points.pt",
-        "simplices": "meshes/simplices.pt",
-    }
-
-    frames = []
-    for i, (R, t) in enumerate(zip(Rs, ts)):
-        flip = torch.tensor([[1, 0, 0], [0, -1, 0], [0, 0, -1]]).float()
-        R = R @ flip
-        transform_matrix = torch.cat([torch.cat([R, t[...,None]], 1), torch.tensor([[0, 0, 0, 1]])], 0)
-        width = widths[i].item()
-        height = heights[i].item()
-        fx = fxs[i] / 2 * widths[i]
-        fy = fys[i] / 2 * heights[i]
-        frame = {
-            "file_path": f"images/{i:05d}.png",
-            "fl_x": fx.item(),
-            "fl_y": fy.item(),
-            "cx": width // 2,
-            "cy": height // 2,
-            "w": int(width),
-            "h": int(height),
-            "transform_matrix": transform_matrix.tolist(),
-            "depth_file_path": f"depths/{i:05d}.npy",
-            "mask_path": f"masks/{i:05d}.png",
-        }
-        frames.append(frame)
-    transforms["frames"] = frames
-
-    return transforms
-
-def make_dense_points_3d(cameras, depths, factor=4):
-    dense_points_3d = []
-
-    for ndx, depth_map in enumerate(depths): 
-        height, width = depth_map.shape
-        xs = torch.arange(width).to(depth_map.device)
-        ys = torch.arange(height).to(depth_map.device)
-        grid_x, grid_y = torch.meshgrid(xs, ys, indexing="ij")
-
-        grid_x = (grid_x / (width - 1) * 2) - 1
-        grid_y = (grid_y / (height - 1) * 2) - 1
-
-        x = grid_x[::factor, ::factor].flatten()
-        y = grid_y[::factor, ::factor].flatten()
-        z = depth_map[::factor, ::factor].T.flatten()
-
-        dense_points_3d.append(cameras(x, y, z)[ndx])
-
-    return dense_points_3d
-
-def make_plys(images_colors, points_3d):
-    n = len(images_colors)
-    plys = []
-    for i in range(n):
-        image_colors = images_colors[i]
-        ply_points = points_3d[i]
-
-        ply = io.StringIO()
-        ply.write("ply\n")
-        ply.write("format ascii 1.0\n")
-        ply.write(f"element vertex {len(ply_points)}\n")
-        ply.write("property float x\n")
-        ply.write("property float y\n")
-        ply.write("property float z\n")
-        ply.write("property uint8 red\n")
-        ply.write("property uint8 green\n")
-        ply.write("property uint8 blue\n")
-        ply.write("end_header\n")
-
-        for point, color in zip(ply_points, image_colors):
-            x, y, z = point.to(torch.float)
-            r, g, b = (color * 255).to(torch.uint8)
-            ply.write(f"{x:8f} {y:8f} {z:8f} {r} {g} {b}\n")
-
-        plys.append(ply.getvalue())
-        ply.close()
-
-    return plys
-
-def load_dataset(data_path, device="cpu", dilate_mask_iters=4, dilate_lines_thresh=0.05, dilate_lines_iters=3, min_valid_points=3):
-    images_path = data_path / "images"
-    metadata_path = data_path / "metadata.json"
-    points_path = data_path / "points.json"
-    depths_path = data_path / "depths"
-
-    metadata_json = json.loads(metadata_path.read_text())
-
-    points_json = json.loads(points_path.read_text())
-    valid_images = points_json["validImages"]
-    points_list = [[[p["x"], p["y"]] for p in points] for points in points_json["points"]]
-    valid_points_list = points_json["validPoints"]
-    # update valid_images based on valid_points_list and min_valid_points
-    valid_images = [valid_images[i] and sum(valid_points_list[i]) >= min_valid_points for i in range(len(valid_images))]
-    valid_polygons = points_json["polygons"]
-    image_filenames = sorted(list(images_path.glob("*.png")))
-
-    # only keep the valid indices, based on valid_images
-    metadata_json["frames"] = [
-        metadata_json["frames"][i] for i in range(len(metadata_json["frames"])) if valid_images[i]
-    ]
-    points_list = [points_list[i] for i in range(len(points_list)) if valid_images[i]]
-    valid_points_list = [valid_points_list[i] for i in range(len(valid_points_list)) if valid_images[i]]
-    valid_polygons = [valid_polygons[i] for i in range(len(valid_polygons)) if valid_images[i]]
-    image_filenames = [image_filenames[i] for i in range(len(image_filenames)) if valid_images[i]]
-
-    images = [torch.from_numpy(mediapy.read_image(imf)[:, :, :3] / 255.0).float() for imf in image_filenames]
-    n = len(images)
-    heights = torch.tensor([image.shape[0] for image in images]).to(device)
-    widths = torch.tensor([image.shape[1] for image in images]).to(device)
-
-    m = max([len(p) for p in points_list])
-
-    points = torch.full([n, m, 2], -1).float().to(device)
-    for i in range(n):
-        for j in range(len(points_list[i])):
-            points[i, j, 0] = points_list[i][j][0]
-            points[i, j, 1] = points_list[i][j][1]
-
-    # points_mask padded with False
-    points_mask = torch.zeros_like(points[:, :, 0]) == 1
-    for i in range(n):
-        for j in range(len(points_list[i])):
-            points_mask[i, j] = valid_points_list[i][j]
-
-    # remove points that have no pair
-    points_mask.T[(points_mask * 1).sum(0) < 2][:] = False
-
-    depths = []
-    for i in range(len(valid_images)):
-        depths.append(torch.load(depths_path / f"{i:05d}.pt").squeeze().to(device))
-    # only keep the valid indices, based on valid_images
-    depths = [depths[i] for i in range(len(depths)) if valid_images[i]]
-    max_depth = max([torch.max(depth) for depth in depths])
-    depths = [depth / max_depth for depth in depths]
-
-    masks = []
-    for i in range(n):
-        mask_image = np.ones((heights[i], widths[i]), dtype=np.uint8) * 255
-        for j in range(len(metadata_json["frames"][i]["masks"])):
-            mask = metadata_json["frames"][i]["masks"][j]
-            for k in range(len(mask["polygons"])):
-                contour = np.array(mask["polygons"][k]).reshape(-1, 2).astype(np.int32)
-                temp_mask_image = np.zeros((heights[i], widths[i]), dtype=np.uint8)
-                if valid_polygons[i][j][k]:
-                    cv2.fillPoly(temp_mask_image, [contour], 1)
-                temp_mask_image = cv2.dilate(temp_mask_image, np.ones((5, 5), np.uint8), iterations=dilate_mask_iters)
-                mask_image[temp_mask_image == 1] = 0
-        masks.append(mask_image)
-
-    # mask out parts of the depth map where they are big discontinuities
-    for i in range(n):
-        depth_mask = 1 - create_discontinuity_mask(depths[i][None], dilate_lines_thresh, dilate_lines_iters)[0].float()
-        masks[i] *= depth_mask.cpu().numpy().astype(np.uint8)
-
-    shapes = torch.cat([widths[:, None], heights[:, None]], -1).unsqueeze(1).repeat(1, m, 1).to(device)
-    points_normed = (points / shapes) * 2 - 1
-
-    return images, heights, widths, points, points_normed, points_mask, depths, masks
-
-
 def main(
     data_prefix: Path = Path("data/processed"),
-    dataset: str = "rick-house",
+    dataset: str = "bobs-burgers-dining",
     device: str = "cpu",
     niters: int = 2000,
     lr: float = 0.01,
     affine_loss_mult: float = 1000.0,
     scale_loss_mult: float = 1e3,
     scale_loss_target: float = 1.0,
     offset_loss_mult: float = 1e3,
@@ -217,15 +47,14 @@
     arap_mult: float = 1, 
     zs_diff_mult: float = 1,
     output_prefix: Path = Path("outputs"),
     output_method: Path = Path("run"),
     nerfstudio_folder: Path = Path("data/nerfstudio"),
     ply_downscale_factor: int = 4,
     view_point_cloud: bool = True,
-    make_video: bool = False,
     save_geometry: bool = True,
     write_to_nerfstudio: bool = True,
     mask_random_points: int = 0,
     port: int = 7007,
     seed: int = None,
 ):
     """Script to run our SfM on cartoons."""
@@ -370,15 +199,14 @@
     CONSOLE.print("[bold green] Image Warping")
 
     dzs_warp = nn.Parameter(dzs.detach().clone()) # delta zs
     szs_warp = nn.Parameter(szs.detach().clone()) # scale zs
 
     # set up optimizer
     optimizer = torch.optim.Adam(list(frame_meshes.parameters()) + list(refined_cameras.parameters()) + [szs_warp, dzs_warp], lr=lr_warp)
-    video_warped_mesh_points = [[] for _ in range(n)]
 
     # optimization loop
     pbar = tqdm(range(niters_warp))
 
     tri_areas = signed_areas(face_verts_packed)
 
     for i in pbar:
@@ -435,19 +263,14 @@
             if offset_loss_mult == 0:
                 dzs_warp[:] = 0
 
             corrs_lthan_min = frame_meshes.corr_zs_padded + frame_meshes.delta_corr_zs_padded < 0.1
             if torch.any(corrs_lthan_min):
                 frame_meshes.delta_corr_zs_padded[corrs_lthan_min] = 0.1 - frame_meshes.corr_zs_padded[corrs_lthan_min]
 
-            if make_video and i % 20 == 0:
-                for ndx in range(n):
-                        video_warped_mesh_points[ndx].append(frame_meshes.warped_corr_points_list[ndx].clone())
-
-
         pbar.set_description(f"Loss: {loss:.2e}, 3D: {affine_loss:.2e}, ARAP: {arap_loss:.2e}, Z: {zs_diff_loss:.2e}", refresh=True)
 
     ### create meshes for warping ###
     all_meshes = []
 
     for ndx in range(n):
         warped_mesh_points = frame_meshes.warped_points_list[ndx]
@@ -525,38 +348,14 @@
         mediapy.write_image(output_warped_depths_dir / f"zdepth_{ndx:02d}.png", warped_depth_z.numpy())
         mediapy.write_image(output_warped_masks_dir / f"{ndx:02d}.png", warped_mask)
 
         warped_images.append(warped_image)
         warped_depths.append(warped_depth)
         warped_masks.append(warped_mask)
 
-    if make_video:
-        CONSOLE.print("[bold green] Rendering Videos")
-        pbar = tqdm(range(n))
-        for ndx in pbar:
-            warped_mesh_points_frames = video_warped_mesh_points[ndx]
-            
-            uv_points = frame_meshes.points_list[ndx]
-            simplices = frame_meshes.simplices_list[ndx]
-
-            video_frames = []
-
-            mesh = WarpMesh(warped_mesh_points, simplices, heights[ndx], widths[ndx], uv_points, device=device)
-
-            for warped_mesh_points in warped_mesh_points_frames:
-                mesh.points = warped_mesh_points.to(mesh.device).float()
-                image = images[ndx]
-
-                warped_image = mesh.apply_warp(image).cpu().detach()
-                wire_img = draw_tris(mesh, image = warped_image.numpy())
-                points_img = draw_points(mesh, image=wire_img, points=warped_mesh_points[:frame_meshes.num_corrs_per_mesh[ndx]], colors=point_colors[points_mask[ndx]].tolist())
-                video_frames.append(np.concatenate([warped_image.numpy(), points_img], axis=1))
-
-            mediapy.write_video(output_warped_images_dir / f"{ndx:02d}.mp4", video_frames)
-
 
     # rescale depths
     depths = [(depth_map * sz[...,None]) + dz[...,None] for depth_map, dz, sz in zip(depths, dzs, szs)]
     warped_depths = [(depth_map.to(device) * sz[...,None]) + dz[...,None] for depth_map, dz, sz in zip(warped_depths, dzs_warp, szs_warp)]
 
 
     #######################
@@ -566,24 +365,22 @@
     nerfstudio_dir = output_folder / "nerfstudio"
     nerfstudio_images_dir = nerfstudio_dir / "images"
     nerfstudio_depths_dir = nerfstudio_dir / "depths"
     nerfstudio_masks_dir = nerfstudio_dir / "masks"
     nerfstudio_points_dir = nerfstudio_dir / "points"
     nerfstudio_meshes_dir = nerfstudio_dir / "meshes"
     nerfstudio_plys_dir = nerfstudio_dir / "plys"
-    nerfstudio_objs_dir = nerfstudio_dir / "objs"
 
     nerfstudio_dir.mkdir(parents=True, exist_ok=True)
     nerfstudio_images_dir.mkdir(parents=True, exist_ok=True)
     nerfstudio_depths_dir.mkdir(parents=True, exist_ok=True)
     nerfstudio_masks_dir.mkdir(parents=True, exist_ok=True)
     nerfstudio_points_dir.mkdir(parents=True, exist_ok=True)
     nerfstudio_meshes_dir.mkdir(parents=True, exist_ok=True)
     nerfstudio_plys_dir.mkdir(parents=True, exist_ok=True)
-    nerfstudio_objs_dir.mkdir(parents=True, exist_ok=True)
 
     # store mesh points
     
     meshes_points_dict = {"corr_points": frame_meshes.corr_points_list, 
                     "boundary_points": [], 
                     "inner_points": [],
                     "points": frame_meshes.points_list}
@@ -736,15 +533,15 @@
                 json.dump(metrics, f, indent=4)
         CONSOLE.print(f"[bold green] Metrics: {metrics}")
     else:
         metrics = None
 
 
     if write_to_nerfstudio or save_geometry:
-        CONSOLE.print("[bold green] Writing objs and plys")
+        CONSOLE.print("[bold green] Writing plys")
 
         # create plys (point clouds)
         plys = make_plys(warped_images_colors, warped_dense_points_3d)
         for i, ply in enumerate(plys):
             with open(output_folder / "nerfstudio" / "plys" / f"{i:05d}.ply", "w") as f:
                 f.write(ply)
 
@@ -800,15 +597,14 @@
                          refined_corrs_3d, # sparse pc
                          sparse_point_colors,
                          warped_mesh_verts_list, # mesh
                          frame_meshes.simplices_list,
                          mesh_colors,
                          prefix="refined")
         
-        # import pdb; pdb.set_trace()
         while True:
             pass
 
     return metrics
 
 
 def entrypoint():
```

### Comparing `toon3d-0.0.3/toon3d/scripts/server.py` & `toon3d-0.0.4/toon3d/scripts/server.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.3/toon3d/scripts/viser_vis.py` & `toon3d-0.0.4/toon3d/scripts/viser_vis.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.3/toon3d/toon3d_config.py` & `toon3d-0.0.4/toon3d/toon3d_config.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.3/toon3d/toon3d_dataparser.py` & `toon3d-0.0.4/toon3d/toon3d_dataparser.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.3/toon3d/toon3d_model.py` & `toon3d-0.0.4/toon3d/toon3d_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,66 +15,34 @@
 
 from toon3d.utils.losses import depth_ranking_loss
 
 import math
 from dataclasses import dataclass, field
 from typing import Dict, List, Optional, Tuple, Type, Union
 
-import numpy as np
 import torch
-import torchvision.transforms.functional as TF
-from gsplat._torch_impl import quat_to_rotmat
-
-from gsplat.project_gaussians import project_gaussians
-from gsplat.rasterize import rasterize_gaussians
-from gsplat.sh import num_sh_bases, spherical_harmonics
-from pytorch_msssim import SSIM
-from sklearn.neighbors import NearestNeighbors
-from torch.nn import Parameter
-from torchmetrics.image import PeakSignalNoiseRatio
-from torchmetrics.image.lpip import LearnedPerceptualImagePatchSimilarity
 
 from nerfstudio.cameras.cameras import Cameras
 from nerfstudio.data.scene_box import OrientedBox
 from nerfstudio.engine.callbacks import TrainingCallback, TrainingCallbackAttributes, TrainingCallbackLocation
 from nerfstudio.engine.optimizers import Optimizers
 
 # need following import for background color override
-from nerfstudio.model_components import renderers
 from nerfstudio.model_components.losses import tv_loss
-from nerfstudio.models.base_model import Model, ModelConfig
-from nerfstudio.utils.rich_utils import CONSOLE
-from nerfstudio.utils.colormaps import apply_depth_colormap
 
-import mediapy
-from toon3d.configs.prompts import get_prompts
+
 from toon3d.utils.novel_view_samplers import sample_interpolated_camera
-from toon3d.utils.depth_utils import depth_to_disparity
-from nerfstudio.viewer.viewer_elements import ViewerControl
-from nerfstudio.viewer.viewer import VISER_NERFSTUDIO_SCALE_RATIO
 
 
 @dataclass
 class Toon3DModelConfig(SplatfactoModelConfig):
     """Config for the toon3d model."""
 
     _target: Type = field(default_factory=lambda: Toon3DModel)
 
-    # color palette parameters
-    use_color_palette: bool = False
-    """Whether to use the color palette for the toon3d model."""
-    color_palette_project_before_render: bool = False
-    """Whether to project nd dim with the color palette before rendering."""
-    color_palette_use_as_colors: bool = False
-    """Whether to use the color palette as the rgb output of the model."""
-    color_palette_mult: float = 1.0
-    """Multiplier for the color palette loss, when using it as a regularizer (not rgb)."""
-    color_palette_rend_consistency_mult: float = 1.0
-    """Multiplier for the color palette rendered consistency loss, when using it as a regularizer (not rgb)."""
-
     # depth regularization parameters
     use_tv_loss: bool = True
     """Whether to use the total variation loss."""
     tv_loss_mult: float = 100.0
     """Multiplier for the total variation loss."""
     tv_loss_strides: List[int] = field(default_factory=lambda: [1])
     """Downscale strides to use for the total variation loss."""
@@ -116,29 +84,20 @@
 
 class Toon3DModel(SplatfactoModel):
     """Model for toon3d."""
 
     config: Toon3DModelConfig
 
     def __init__(self, *args, **kwargs):
-        self.color_palette = kwargs["color_palette"]
         self.cameras = kwargs["cameras"]
         super().__init__(*args, **kwargs)
 
     def populate_modules(self):
         """Required for our custom models."""
 
-        # modify the config for nd attributes
-        if self.config.use_color_palette:
-            print("Overriding nd_dim config based on color palette config")
-            if self.config.color_palette_use_as_colors:
-                self.config.nd_detach = False
-            else:
-                self.config.nd_detach = True
-
         super().populate_modules()
 
         # we toggle this on and off
         # when True, we perturb the camera
         self.perturb_camera = False
 
     def get_training_callbacks(
@@ -188,31 +147,14 @@
             camera_perturb = camera_perturb.reshape(camera.shape).to(camera.device)
             outputs = super().get_outputs(camera_perturb)
             # mediapy.write_image("novel_view.png", outputs["rgb"].detach().cpu())
         else:
             outputs = super().get_outputs(camera)
         return outputs
 
-    def get_nd_values(self):
-        if self.config.use_color_palette and self.config.color_palette_project_before_render:
-            sm = torch.softmax(self.nd_values, dim=-1)[..., None]
-            cp = self.color_palette[None]
-            nd_values = torch.sum(sm * cp, dim=-2)
-            return nd_values
-        else:
-            return self.nd_values
-
-    def get_color_palette_rgb(self, nd_value):
-        if self.config.use_color_palette and self.config.color_palette_project_before_render:
-            return nd_value
-        else:
-            sm = torch.softmax(nd_value, dim=-1)[..., None]
-            cp = self.color_palette[None, None]
-            return torch.sum(sm * cp, dim=-2)
-
     def get_metrics_dict(self, outputs, batch) -> Dict[str, torch.Tensor]:
         """Compute and returns metrics.
 
         Args:
             outputs: the output to compute loss dict to
             batch: ground truth batch corresponding to outputs
         """
@@ -256,35 +198,19 @@
         depth = batch["depth_image"] # (height, width, 1)
 
         assert self._get_downscale_factor() == 1, "downscale factor must be 1 for toon3d model"
 
         gt_img = image
 
         # rgb loss
-        if self.config.use_color_palette and self.config.color_palette_use_as_colors:
-            rgb = outputs["nd_value"] * mask[...,None].to(outputs["nd_value"].device)
-        else:
-            rgb = outputs["rgb"] * mask[...,None].to(outputs["rgb"].device)
+        rgb = outputs["rgb"] * mask[...,None].to(outputs["rgb"].device)
 
         Ll1 = torch.abs(gt_img[mask] - rgb[mask]).mean()
         loss_dict["rgb"] = Ll1
 
-        # color palette as a regularizer
-        if self.config.use_color_palette and not self.config.color_palette_use_as_colors:
-            color_palette_rgb = self.get_color_palette_rgb(outputs["nd_value"])
-            # color palette loss
-            Ll1 = torch.abs(gt_img[mask] - color_palette_rgb[mask]).mean()
-            loss_dict["rgb-cpalette"] = Ll1
-
-            # color consistency loss
-            loss_dict["rgb-cpalette-rend-consistency"] = (
-                self.config.color_palette_rend_consistency_mult
-                * torch.abs(rgb[mask] - color_palette_rgb[mask].detach()).mean()
-            )
-
         if self.config.use_tv_loss:
             pred_depth = outputs["depth"]
             for stride in self.config.tv_loss_strides:
                 loss_dict[f"depth_tv_loss_stride-{stride}"] = self.config.tv_loss_mult * tv_loss(
                     pred_depth.permute(2, 0, 1)[None, :, ::stride, ::stride]
                 )
```

### Comparing `toon3d-0.0.3/toon3d/utils/camera_utils.py` & `toon3d-0.0.4/toon3d/utils/camera_utils.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.3/toon3d/utils/colmap_database.py` & `toon3d-0.0.4/toon3d/utils/colmap_database.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.3/toon3d/utils/convert_points.py` & `toon3d-0.0.4/toon3d/utils/convert_points.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.3/toon3d/utils/depth_utils.py` & `toon3d-0.0.4/toon3d/utils/depth_utils.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.3/toon3d/utils/draw_utils.py` & `toon3d-0.0.4/toon3d/utils/draw_utils.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.3/toon3d/utils/image_processing_utils.py` & `toon3d-0.0.4/toon3d/utils/image_processing_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             depth_tensor = -depth_tensor.permute(1, 2, 0)
             depth_tensor = depth_tensor - depth_tensor.min()
         depths.append(depth_tensor)
 
     return depths
 
 
-def generate_segments(images, device="cpu", sam_checkpoint_prefix="data/sam-checkpoints"):
+def generate_segments(images, device="cpu", sam_checkpoint_prefix="data/sam-checkpoints", sam_points_per_side=32):
     sam_checkpoint = os.path.join(sam_checkpoint_prefix, "sam_vit_b_01ec64.pth")
     model_type = "vit_b"
 
     if not os.path.exists(sam_checkpoint):
         CONSOLE.log(f"[bold yellow]File not found: {sam_checkpoint}")
         CONSOLE.log(f"[bold yellow]Downloading `vit_b` from https://github.com/facebookresearch/segment-anything")
         os.system(
@@ -59,18 +59,18 @@
     try:
         sam = sam_model_registry[model_type](checkpoint=sam_checkpoint)
         sam.to(device=device)
     except FileNotFoundError as e:
         CONSOLE.log(f"[bold red]{e}")
         CONSOLE.log(f"[bold red]Problem Downloading `vit_b` from https://github.com/facebookresearch/segment-anything")
         sys.exit(1)
-
+    
     mask_generator = SamAutomaticMaskGenerator(
         model=sam,
-        points_per_side=128,
+        points_per_side=sam_points_per_side,
         pred_iou_thresh=0.85,
         stability_score_thresh=0.88,
         stability_score_offset=1,
         box_nms_thresh=0.9,
         output_mode="coco_rle",
     )
```

### Comparing `toon3d-0.0.3/toon3d/utils/losses.py` & `toon3d-0.0.4/toon3d/utils/losses.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.3/toon3d/utils/novel_view_samplers.py` & `toon3d-0.0.4/toon3d/utils/novel_view_samplers.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.3/toon3d/utils/viser_utils.py` & `toon3d-0.0.4/toon3d/utils/viser_utils.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.3/toon3d/warp/arap_utils.py` & `toon3d-0.0.4/toon3d/warp/arap_utils.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.3/toon3d/warp/warp_mesh.py` & `toon3d-0.0.4/toon3d/warp/warp_mesh.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.3/toon3d-labeler/node_modules/flatted/python/flatted.py` & `toon3d-0.0.4/toon3d-labeler/node_modules/flatted/python/flatted.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.3/toon3d-labeler/node_modules/flatted/python/test.py` & `toon3d-0.0.4/toon3d-labeler/node_modules/flatted/python/test.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.3/toon3d-spaces/app.py` & `toon3d-0.0.4/toon3d-spaces/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 viewer_thread_instance = None
 stop_event = threading.Event()
 shared_url = None
 
 _HEADER_ = '''
 <h2>Toon3D: Seeing Cartoons from a New Perspective</h2>
-Toon3D lifts cartoons into 3D via aligning and warping backprojected monocular depth predictions. The project page is at <a href='https://toon3d.studio/' target='_blank'>https://toon3d.studio/</a> and the Toon3D Labeler is at <a href='https://labeler.toon3d.studio/' target='_blank'>https://labeler.toon3d.studio/</a>. Follow the steps below to run Toon3D!
+Toon3D lifts hand-drawn images to 3D with a piecewise-rigid deformation optimization at hand-labeled keypoints and using monocular depth as a prior. The project page is at <a href='https://toon3d.studio/' target='_blank'>https://toon3d.studio/</a> and the Toon3D Labeler is at <a href='https://labeler.toon3d.studio/' target='_blank'>https://labeler.toon3d.studio/</a>. Follow the steps below to run Toon3D!
 
 <div style="margin-top: 20px; font-size: 16px; line-height: 1.6;">
     <div style="display: flex; justify-content: space-between;">
         <div style="width: 49%;">
             <ol>
                 <li><strong>Prepare and Process Data</strong>
                     <ul>
@@ -265,8 +265,8 @@
         fn=start_viewer,
         inputs=[processed_data_zip, labeled_data, toon3d_output_zip],
         outputs=[viser_link],
     )
 
 if __name__ == "__main__":
     demo.queue(max_size=10)
-    demo.launch()
+    demo.launch(share=True)
```

### Comparing `toon3d-0.0.3/toon3d.egg-info/PKG-INFO` & `toon3d-0.0.4/toon3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toon3d
-Version: 0.0.3
+Version: 0.0.4
 Summary: toon3d package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7.3
 Requires-Dist: black
 Requires-Dist: h5py
 Requires-Dist: mediapy
```

### Comparing `toon3d-0.0.3/toon3d.egg-info/SOURCES.txt` & `toon3d-0.0.4/toon3d.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 README.md
 pyproject.toml
 toon3d/__init__.py
-toon3d/color_palette.py
 toon3d/toon3d_config.py
 toon3d/toon3d_datamanager.py
 toon3d/toon3d_dataparser.py
 toon3d/toon3d_model.py
 toon3d/toon3d_pipeline.py
 toon3d-labeler/node_modules/flatted/python/flatted.py
 toon3d-labeler/node_modules/flatted/python/test.py
@@ -17,22 +16,23 @@
 toon3d.egg-info/requires.txt
 toon3d.egg-info/top_level.txt
 toon3d/configs/prompts.py
 toon3d/generative/marigold.py
 toon3d/scripts/colmap_with_corrs.py
 toon3d/scripts/download_data.py
 toon3d/scripts/process_data.py
+toon3d/scripts/render.py
 toon3d/scripts/run.py
 toon3d/scripts/server.py
 toon3d/scripts/viser_vis.py
 toon3d/utils/camera_utils.py
 toon3d/utils/colmap_database.py
 toon3d/utils/convert_points.py
 toon3d/utils/depth_utils.py
 toon3d/utils/draw_utils.py
 toon3d/utils/image_processing_utils.py
+toon3d/utils/io_utils.py
 toon3d/utils/losses.py
 toon3d/utils/novel_view_samplers.py
-toon3d/utils/tsdf_utils.py
 toon3d/utils/viser_utils.py
 toon3d/warp/arap_utils.py
 toon3d/warp/warp_mesh.py
```

