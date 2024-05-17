# Comparing `tmp/video-representations-extractor-1.0.3.tar.gz` & `tmp/video-representations-extractor-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video-representations-extractor-1.0.3.tar", last modified: Tue May 14 16:29:33 2024, max compression
+gzip compressed data, was "video-representations-extractor-1.0.4.tar", last modified: Fri May 17 08:31:30 2024, max compression
```

## Comparing `video-representations-extractor-1.0.3.tar` & `video-representations-extractor-1.0.4.tar`

### file list

```diff
@@ -1,226 +1,227 @@
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.041629 video-representations-extractor-1.0.3/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      486 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/LICENSE.TXT
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     5500 2024-05-14 16:29:33.041629 video-representations-extractor-1.0.3/PKG-INFO
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     5137 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.3/README.md
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.013629 video-representations-extractor-1.0.3/bin/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)     4253 2024-05-13 17:44:45.000000 video-representations-extractor-1.0.3/bin/vre
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)     4061 2024-05-06 11:15:40.000000 video-representations-extractor-1.0.3/bin/vre_collage
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       38 2024-05-14 16:29:33.041629 video-representations-extractor-1.0.3/setup.cfg
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1341 2024-05-14 16:29:31.000000 video-representations-extractor-1.0.3/setup.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.017629 video-representations-extractor-1.0.3/video_representations_extractor.egg-info/
--rw-r--r--   0 mihai     (1000) mihai     (1000)     5500 2024-05-14 16:29:32.000000 video-representations-extractor-1.0.3/video_representations_extractor.egg-info/PKG-INFO
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    12678 2024-05-14 16:29:32.000000 video-representations-extractor-1.0.3/video_representations_extractor.egg-info/SOURCES.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2024-05-14 16:29:32.000000 video-representations-extractor-1.0.3/video_representations_extractor.egg-info/dependency_links.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      396 2024-05-14 16:29:32.000000 video-representations-extractor-1.0.3/video_representations_extractor.egg-info/requires.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        4 2024-05-14 16:29:32.000000 video-representations-extractor-1.0.3/video_representations_extractor.egg-info/top_level.txt
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.017629 video-representations-extractor-1.0.3/vre/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      215 2024-05-06 12:14:58.000000 video-representations-extractor-1.0.3/vre/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3607 2024-05-13 17:44:45.000000 video-representations-extractor-1.0.3/vre/data_storer.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2355 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/logger.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2419 2024-05-08 19:37:37.000000 video-representations-extractor-1.0.3/vre/representation.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.017629 video-representations-extractor-1.0.3/vre/representations/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       82 2024-05-07 08:51:30.000000 video-representations-extractor-1.0.3/vre/representations/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     5474 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.3/vre/representations/build_representations.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.017629 video-representations-extractor-1.0.3/vre/representations/depth/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/depth/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.021629 video-representations-extractor-1.0.3/vre/representations/depth/dpt/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       48 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/depth/dpt/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3880 2024-05-08 19:33:51.000000 video-representations-extractor-1.0.3/vre/representations/depth/dpt/depth_dpt.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.021629 video-representations-extractor-1.0.3/vre/representations/depth/dpt/dpt_impl/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/depth/dpt/dpt_impl/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      389 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/depth/dpt/dpt_impl/base_model.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     9178 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/depth/dpt/dpt_impl/blocks.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3088 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/depth/dpt/dpt_impl/dpt_depth.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    14673 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/depth/dpt/dpt_impl/vit.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.021629 video-representations-extractor-1.0.3/vre/representations/depth/odo_flow/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       57 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/depth/odo_flow/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     5726 2024-05-08 19:28:49.000000 video-representations-extractor-1.0.3/vre/representations/depth/odo_flow/depth_odo_flow.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.021629 video-representations-extractor-1.0.3/vre/representations/depth/odo_flow/odo_flow_impl/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/depth/odo_flow/odo_flow_impl/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2485 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/depth/odo_flow/odo_flow_impl/cam.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3381 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/depth/odo_flow/odo_flow_impl/camera_info.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    27130 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/depth/odo_flow/odo_flow_impl/depth_from_flow.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2996 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/depth/odo_flow/odo_flow_impl/loss.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2552 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/depth/odo_flow/odo_flow_impl/polyfit.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    12079 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/depth/odo_flow/odo_flow_impl/utils.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    11740 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/depth/odo_flow/odo_flow_impl/utils_geometry.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1172 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/dummy_representation.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.021629 video-representations-extractor-1.0.3/vre/representations/edges/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/edges/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1620 2024-05-08 19:06:41.000000 video-representations-extractor-1.0.3/vre/representations/edges/canny.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.021629 video-representations-extractor-1.0.3/vre/representations/edges/dexined/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       45 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/edges/dexined/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3429 2024-05-09 21:06:52.000000 video-representations-extractor-1.0.3/vre/representations/edges/dexined/dexined.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    10066 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/edges/dexined/model_dexined.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      883 2024-05-07 14:46:28.000000 video-representations-extractor-1.0.3/vre/representations/hsv.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.021629 video-representations-extractor-1.0.3/vre/representations/normals/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/normals/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.021629 video-representations-extractor-1.0.3/vre/representations/normals/depth_svd/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       63 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/normals/depth_svd/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4088 2024-05-08 19:20:50.000000 video-representations-extractor-1.0.3/vre/representations/normals/depth_svd/depth_normals_svd.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.021629 video-representations-extractor-1.0.3/vre/representations/normals/depth_svd/depth_svd_impl/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/normals/depth_svd/depth_svd_impl/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2485 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/normals/depth_svd/depth_svd_impl/cam.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3125 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/normals/depth_svd/depth_svd_impl/utils.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.021629 video-representations-extractor-1.0.3/vre/representations/optical_flow/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/optical_flow/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.021629 video-representations-extractor-1.0.3/vre/representations/optical_flow/raft/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       48 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/optical_flow/raft/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4983 2024-05-09 21:06:52.000000 video-representations-extractor-1.0.3/vre/representations/optical_flow/raft/flow_raft.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.025629 video-representations-extractor-1.0.3/vre/representations/optical_flow/raft/raft_impl/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/optical_flow/raft/raft_impl/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3074 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/optical_flow/raft/raft_impl/corr.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     9267 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/optical_flow/raft/raft_impl/datasets.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     8869 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/optical_flow/raft/raft_impl/extractor.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4512 2024-05-08 18:52:36.000000 video-representations-extractor-1.0.3/vre/representations/optical_flow/raft/raft_impl/raft.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     5249 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/optical_flow/raft/raft_impl/update.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2573 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/optical_flow/raft/raft_impl/utils.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.025629 video-representations-extractor-1.0.3/vre/representations/optical_flow/rife/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       48 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/optical_flow/rife/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4698 2024-05-09 21:06:52.000000 video-representations-extractor-1.0.3/vre/representations/optical_flow/rife/flow_rife.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.025629 video-representations-extractor-1.0.3/vre/representations/optical_flow/rife/rife_impl/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4421 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/optical_flow/rife/rife_impl/IFNet_HD.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3712 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/optical_flow/rife/rife_impl/IFNet_HDv2.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     8754 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/optical_flow/rife/rife_impl/RIFE_HDv2.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/optical_flow/rife/rife_impl/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2866 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/optical_flow/rife/rife_impl/loss.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1091 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/optical_flow/rife/rife_impl/warplayer.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      804 2024-05-09 21:06:52.000000 video-representations-extractor-1.0.3/vre/representations/rgb.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.025629 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.025629 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       53 2024-04-23 19:55:41.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)    39430 2024-04-26 05:56:06.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/convert.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)     8143 2024-05-08 08:30:31.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.025629 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      138 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     7259 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/comm.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.025629 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       96 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.025629 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      318 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    52231 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_ade20k_full.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4608 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_ade20k_instance.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    19460 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_ade20k_panoptic.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     7080 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_coco_panoptic_annos_semseg.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    13576 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_coco_stuff_10k.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    13034 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_mapillary_vistas.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    16080 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_mapillary_vistas_panoptic.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.029629 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      666 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     7404 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/benchmark.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    26836 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/build.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     6991 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/catalog.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    13408 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/common.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     8129 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/dataset_mapper.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.029629 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      545 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    10183 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/builtin.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    21863 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/builtin_meta.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    11343 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/cityscapes.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     7793 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/cityscapes_panoptic.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    22788 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/coco.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     7649 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/coco_panoptic.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     8816 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)   223779 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis_v0_5_categories.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)   219199 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis_v1_categories.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    39436 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis_v1_category_image_count.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3112 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/pascal_voc.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      191 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/register_coco.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    23182 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/detection_utils.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.029629 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/samplers/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      434 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/samplers/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    12251 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/samplers/distributed_sampler.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1966 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/samplers/grouped_batch_sampler.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.029629 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      352 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    14138 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/augmentation.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    27338 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/augmentation_impl.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    12653 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/transform.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1259 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/file_io.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.033629 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      253 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3040 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/blocks.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    16657 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/deform_conv.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     9779 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/norm.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      559 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/shape_spec.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1388 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/wrappers.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    18059 2024-04-25 06:02:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/maskformer_model.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.033629 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      238 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.033629 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/backbone/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/backbone/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    27473 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/backbone/swin.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.033629 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/meta_arch/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/meta_arch/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     5262 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/meta_arch/mask_former_head.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.033629 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    11748 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/fpn.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     7811 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/ms_deform_attn.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    15168 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/msdeformattn.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    25781 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/resnet.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.033629 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      224 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    17739 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/mask2former_transformer_decoder.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     6946 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/maskformer_transformer_decoder.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2540 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/position_encoding.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    11959 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/transformer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.037629 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      410 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    14451 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/boxes.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     6697 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/image_list.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     6635 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/instances.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     9030 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/keypoints.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    19531 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/masks.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    18980 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/rotated_boxes.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    54116 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/visualizer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.037629 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/safeuav/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     5125 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/safeuav/Map2Map.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       45 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/safeuav/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4155 2024-05-08 08:31:54.000000 video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/safeuav/safeuav.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.037629 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.037629 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       67 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)     8799 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/fastsam.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.037629 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/fastsam_impl/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      312 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/fastsam_impl/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4725 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/fastsam_impl/decoder.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     8187 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/fastsam_impl/model.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    12770 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/fastsam_impl/ops.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     6949 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/fastsam_impl/predict.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    18538 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/fastsam_impl/prompt.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    35552 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/fastsam_impl/results.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    12112 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/fastsam_impl/utils.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.037629 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/ultralytics/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       22 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/ultralytics/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.037629 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/ultralytics/nn/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      102 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/ultralytics/nn/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.037629 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/ultralytics/nn/modules/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1587 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/ultralytics/nn/modules/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    11838 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/ultralytics/nn/modules/block.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    11669 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/ultralytics/nn/modules/conv.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    16428 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/ultralytics/nn/modules/head.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    15956 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/ultralytics/nn/modules/transformer.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3266 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/ultralytics/nn/modules/utils.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3722 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/ultralytics/nn/tasks.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.037629 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/ultralytics/yolo/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       22 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/ultralytics/yolo/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.037629 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/ultralytics/yolo/utils/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      786 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/ultralytics/yolo/utils/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.037629 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/generalized_boundaries/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       74 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/generalized_boundaries/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1836 2024-05-07 15:03:35.000000 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/generalized_boundaries/generalized_boundaries.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.037629 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/halftone/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       47 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/halftone/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     7704 2024-05-07 15:05:55.000000 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/halftone/halftone.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4026 2024-05-07 14:54:13.000000 video-representations-extractor-1.0.3/vre/representations/soft_segmentation/kmeans.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-14 16:29:33.041629 video-representations-extractor-1.0.3/vre/utils/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      128 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/utils/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      679 2024-05-06 09:42:54.000000 video-representations-extractor-1.0.3/vre/utils/fake_video.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1352 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.3/vre/utils/topological_sort.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     5169 2024-05-09 21:06:52.000000 video-representations-extractor-1.0.3/vre/utils/utils.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     6609 2024-05-13 17:44:45.000000 video-representations-extractor-1.0.3/vre/video_representations_extractor.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1300 2024-05-13 17:44:45.000000 video-representations-extractor-1.0.3/vre/vre_representation_mixin.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     7169 2024-05-13 17:44:45.000000 video-representations-extractor-1.0.3/vre/vre_runtime_args.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.805239 video-representations-extractor-1.0.4/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      486 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/LICENSE.TXT
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     6496 2024-05-17 08:31:30.805239 video-representations-extractor-1.0.4/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5382 2024-05-17 08:18:09.000000 video-representations-extractor-1.0.4/README.md
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.773239 video-representations-extractor-1.0.4/bin/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)     4253 2024-05-13 17:44:45.000000 video-representations-extractor-1.0.4/bin/vre
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)     4007 2024-05-17 06:00:28.000000 video-representations-extractor-1.0.4/bin/vre_collage
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       38 2024-05-17 08:31:30.805239 video-representations-extractor-1.0.4/setup.cfg
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1336 2024-05-17 08:30:51.000000 video-representations-extractor-1.0.4/setup.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.805239 video-representations-extractor-1.0.4/video_representations_extractor.egg-info/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     6496 2024-05-17 08:31:30.000000 video-representations-extractor-1.0.4/video_representations_extractor.egg-info/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    12697 2024-05-17 08:31:30.000000 video-representations-extractor-1.0.4/video_representations_extractor.egg-info/SOURCES.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2024-05-17 08:31:30.000000 video-representations-extractor-1.0.4/video_representations_extractor.egg-info/dependency_links.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      391 2024-05-17 08:31:30.000000 video-representations-extractor-1.0.4/video_representations_extractor.egg-info/requires.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        4 2024-05-17 08:31:30.000000 video-representations-extractor-1.0.4/video_representations_extractor.egg-info/top_level.txt
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.777239 video-representations-extractor-1.0.4/vre/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      215 2024-05-06 12:14:58.000000 video-representations-extractor-1.0.4/vre/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3607 2024-05-13 17:44:45.000000 video-representations-extractor-1.0.4/vre/data_storer.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2355 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/logger.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2419 2024-05-08 19:37:37.000000 video-representations-extractor-1.0.4/vre/representation.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.777239 video-representations-extractor-1.0.4/vre/representations/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       82 2024-05-07 08:51:30.000000 video-representations-extractor-1.0.4/vre/representations/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5474 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.4/vre/representations/build_representations.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.777239 video-representations-extractor-1.0.4/vre/representations/depth/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/depth/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.777239 video-representations-extractor-1.0.4/vre/representations/depth/dpt/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       48 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/depth/dpt/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3880 2024-05-08 19:33:51.000000 video-representations-extractor-1.0.4/vre/representations/depth/dpt/depth_dpt.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.781239 video-representations-extractor-1.0.4/vre/representations/depth/dpt/dpt_impl/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/depth/dpt/dpt_impl/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      389 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/depth/dpt/dpt_impl/base_model.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     9178 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/depth/dpt/dpt_impl/blocks.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3088 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/depth/dpt/dpt_impl/dpt_depth.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    14673 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/depth/dpt/dpt_impl/vit.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.781239 video-representations-extractor-1.0.4/vre/representations/depth/odo_flow/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       57 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/depth/odo_flow/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5331 2024-05-17 06:00:36.000000 video-representations-extractor-1.0.4/vre/representations/depth/odo_flow/depth_odo_flow.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.781239 video-representations-extractor-1.0.4/vre/representations/depth/odo_flow/odo_flow_impl/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/depth/odo_flow/odo_flow_impl/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2485 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/depth/odo_flow/odo_flow_impl/cam.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3381 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/depth/odo_flow/odo_flow_impl/camera_info.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    26297 2024-05-17 06:53:47.000000 video-representations-extractor-1.0.4/vre/representations/depth/odo_flow/odo_flow_impl/depth_from_flow.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2996 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/depth/odo_flow/odo_flow_impl/loss.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2552 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/depth/odo_flow/odo_flow_impl/polyfit.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    11709 2024-05-17 06:55:19.000000 video-representations-extractor-1.0.4/vre/representations/depth/odo_flow/odo_flow_impl/utils.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    11132 2024-05-17 06:56:39.000000 video-representations-extractor-1.0.4/vre/representations/depth/odo_flow/odo_flow_impl/utils_geometry.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1172 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/dummy_representation.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.781239 video-representations-extractor-1.0.4/vre/representations/edges/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/edges/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1620 2024-05-08 19:06:41.000000 video-representations-extractor-1.0.4/vre/representations/edges/canny.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.781239 video-representations-extractor-1.0.4/vre/representations/edges/dexined/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       45 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/edges/dexined/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3429 2024-05-09 21:06:52.000000 video-representations-extractor-1.0.4/vre/representations/edges/dexined/dexined.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    10066 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/edges/dexined/model_dexined.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2064 2024-05-17 06:43:15.000000 video-representations-extractor-1.0.4/vre/representations/hsv.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.781239 video-representations-extractor-1.0.4/vre/representations/normals/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/normals/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.781239 video-representations-extractor-1.0.4/vre/representations/normals/depth_svd/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       63 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/normals/depth_svd/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4088 2024-05-08 19:20:50.000000 video-representations-extractor-1.0.4/vre/representations/normals/depth_svd/depth_normals_svd.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.781239 video-representations-extractor-1.0.4/vre/representations/normals/depth_svd/depth_svd_impl/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/normals/depth_svd/depth_svd_impl/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2485 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/normals/depth_svd/depth_svd_impl/cam.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3125 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/normals/depth_svd/depth_svd_impl/utils.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.785239 video-representations-extractor-1.0.4/vre/representations/optical_flow/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/optical_flow/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.785239 video-representations-extractor-1.0.4/vre/representations/optical_flow/raft/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       48 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/optical_flow/raft/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4983 2024-05-09 21:06:52.000000 video-representations-extractor-1.0.4/vre/representations/optical_flow/raft/flow_raft.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.785239 video-representations-extractor-1.0.4/vre/representations/optical_flow/raft/raft_impl/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/optical_flow/raft/raft_impl/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3074 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/optical_flow/raft/raft_impl/corr.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     9267 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/optical_flow/raft/raft_impl/datasets.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     8869 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/optical_flow/raft/raft_impl/extractor.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4512 2024-05-08 18:52:36.000000 video-representations-extractor-1.0.4/vre/representations/optical_flow/raft/raft_impl/raft.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5249 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/optical_flow/raft/raft_impl/update.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2573 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/optical_flow/raft/raft_impl/utils.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.785239 video-representations-extractor-1.0.4/vre/representations/optical_flow/rife/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       48 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/optical_flow/rife/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4698 2024-05-09 21:06:52.000000 video-representations-extractor-1.0.4/vre/representations/optical_flow/rife/flow_rife.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.785239 video-representations-extractor-1.0.4/vre/representations/optical_flow/rife/rife_impl/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4421 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/optical_flow/rife/rife_impl/IFNet_HD.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3712 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/optical_flow/rife/rife_impl/IFNet_HDv2.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     8754 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/optical_flow/rife/rife_impl/RIFE_HDv2.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/optical_flow/rife/rife_impl/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2866 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/optical_flow/rife/rife_impl/loss.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1091 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/optical_flow/rife/rife_impl/warplayer.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      804 2024-05-09 21:06:52.000000 video-representations-extractor-1.0.4/vre/representations/rgb.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.785239 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.789239 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       53 2024-04-23 19:55:41.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)    39430 2024-04-26 05:56:06.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/convert.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)     7600 2024-05-17 08:12:54.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.789239 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      138 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     7259 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/comm.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.789239 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       96 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.789239 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      318 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    52231 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_ade20k_full.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4608 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_ade20k_instance.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    19460 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_ade20k_panoptic.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     7080 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_coco_panoptic_annos_semseg.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    13576 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_coco_stuff_10k.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    13034 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_mapillary_vistas.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    16080 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_mapillary_vistas_panoptic.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.793239 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      666 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     7404 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/benchmark.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    26836 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/build.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     6991 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/catalog.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    13273 2024-05-17 06:00:36.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/common.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     8129 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/dataset_mapper.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.793239 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      545 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    10183 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/builtin.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    21863 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/builtin_meta.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    11343 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/cityscapes.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     7793 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/cityscapes_panoptic.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    22788 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/coco.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     7649 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/coco_panoptic.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     8816 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)   223779 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis_v0_5_categories.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)   219199 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis_v1_categories.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    39436 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis_v1_category_image_count.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3112 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/pascal_voc.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      191 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/register_coco.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    23182 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/detection_utils.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.793239 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/samplers/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      434 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/samplers/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    12251 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/samplers/distributed_sampler.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1966 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/samplers/grouped_batch_sampler.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.797239 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      352 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    14138 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/augmentation.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    27338 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/augmentation_impl.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    12653 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/transform.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1259 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/file_io.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.797239 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      253 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3040 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/blocks.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    16657 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/deform_conv.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     9779 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/norm.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      559 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/shape_spec.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1388 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/wrappers.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    18059 2024-04-25 06:02:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/maskformer_model.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.797239 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      238 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.797239 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/backbone/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/backbone/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    27473 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/backbone/swin.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.797239 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/meta_arch/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/meta_arch/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5262 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/meta_arch/mask_former_head.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.797239 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    11748 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/fpn.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     7811 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/ms_deform_attn.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    15168 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/msdeformattn.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    25781 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/resnet.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.797239 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      224 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    17739 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/mask2former_transformer_decoder.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     6946 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/maskformer_transformer_decoder.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2540 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/position_encoding.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    11959 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/transformer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.801239 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      410 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    14451 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/boxes.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     6697 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/image_list.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     6635 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/instances.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     9030 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/keypoints.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    19531 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/masks.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    18980 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/rotated_boxes.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    54116 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/visualizer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.801239 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/safeuav/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5125 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/safeuav/Map2Map.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       45 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/safeuav/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4155 2024-05-08 08:31:54.000000 video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/safeuav/safeuav.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.801239 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.801239 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       67 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)     9731 2024-05-17 08:13:03.000000 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/fastsam.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.801239 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/fastsam_impl/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      200 2024-05-15 05:52:32.000000 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/fastsam_impl/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4725 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/fastsam_impl/decoder.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     8319 2024-05-15 06:21:23.000000 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/fastsam_impl/model.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    12770 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/fastsam_impl/ops.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     6949 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/fastsam_impl/predict.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    18538 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/fastsam_impl/prompt.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    35552 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/fastsam_impl/results.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    12112 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/fastsam_impl/utils.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.801239 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/ultralytics/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       22 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/ultralytics/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.805239 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/ultralytics/nn/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      102 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/ultralytics/nn/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.805239 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/ultralytics/nn/modules/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1587 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/ultralytics/nn/modules/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    11838 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/ultralytics/nn/modules/block.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    11669 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/ultralytics/nn/modules/conv.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    16428 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/ultralytics/nn/modules/head.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    15956 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/ultralytics/nn/modules/transformer.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3266 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/ultralytics/nn/modules/utils.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3722 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/ultralytics/nn/tasks.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.805239 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/ultralytics/yolo/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       22 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/ultralytics/yolo/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.805239 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/ultralytics/yolo/utils/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      786 2024-05-14 16:28:09.000000 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/ultralytics/yolo/utils/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.805239 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/generalized_boundaries/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       74 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/generalized_boundaries/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1836 2024-05-07 15:03:35.000000 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/generalized_boundaries/generalized_boundaries.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.805239 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/halftone/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       47 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/halftone/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     7685 2024-05-17 06:00:28.000000 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/halftone/halftone.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4026 2024-05-07 14:54:13.000000 video-representations-extractor-1.0.4/vre/representations/soft_segmentation/kmeans.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-17 08:31:30.805239 video-representations-extractor-1.0.4/vre/utils/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      149 2024-05-15 06:01:40.000000 video-representations-extractor-1.0.4/vre/utils/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      710 2024-05-16 05:07:27.000000 video-representations-extractor-1.0.4/vre/utils/fake_video.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    14414 2024-05-17 08:16:59.000000 video-representations-extractor-1.0.4/vre/utils/image.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1352 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.4/vre/utils/topological_sort.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3823 2024-05-17 08:15:42.000000 video-representations-extractor-1.0.4/vre/utils/utils.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     6609 2024-05-13 17:44:45.000000 video-representations-extractor-1.0.4/vre/video_representations_extractor.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1300 2024-05-13 17:44:45.000000 video-representations-extractor-1.0.4/vre/vre_representation_mixin.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     7185 2024-05-16 05:07:27.000000 video-representations-extractor-1.0.4/vre/vre_runtime_args.py
```

### Comparing `video-representations-extractor-1.0.3/PKG-INFO` & `video-representations-extractor-1.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: video-representations-extractor
-Version: 1.0.3
-Summary: Video Representations Extractor (VRE) for computing algorithmic or neural representations of each frame.
-Home-page: https://gitlab.com/meehai/video-representations-extractor
-License: WTFPL
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.TXT
-
 # Video Representation Extractor
 
 ![logo](logo.png)
 
 ## 1. Description
 
 The purpose of this repository is to export various representations starting from RGB videos only. Representations are
@@ -42,15 +32,15 @@
 ```
 git clone https://gitlab.com/meehai/video-representations-extractor [/some/dir]
 # in .bashrc
 export PYTHONPATH="$PYTHONPATH:/some/dir"
 export PATH="$PATH:/some/dir/bin"
 ```
 
-After eithrer option, you should be able to run:
+After either option, you should be able to run:
 ```bash
 vre <path/to/video.mp4> --cfg_path <path/to/cfg> -o <path/to/export_dir>
 ```
 
 The magic happens inside the config file, where we define *what* representations to extract and *what* parameters are
 used to instantiate said representations.
 
@@ -66,40 +56,42 @@
 Note: use `--cfg_path resources/cfgs/testCfg_ootb.yaml` for 'out of the box' working representations.
 
 Note2: Use `VRE_DEVICE=cuda vre...` to use cuda. For some representations, this speeds up the process by a lot.
 
 ## 3. CFG file
 
 The config file will have the hyperparameters required to instantiate each supported method as well as global
-hyperparameters for the output. This means that if a depth method is pre-traied for 0-300m, this information will be
-encoded in the CFG file and passed to the constructor of that particular depth method. There are also export level
-parameters, such as the output resolution of the representations.
+hyperparameters for the output. These parameters are sent to the constructor of each representation, so one can pass
+additional semantics to each representation, such as classes of a semantic segmentation or the maximum global depth
+value in meters.
 
 High level format:
 
 ```
 name of representation:
   type: some high level type (such as depth, semantic, edges, etc.)
   name: the implemented method's name (i.e. dexined, dpt, odoflow etc.)
   dependencies: [a list of dependencies given by their names]
-  parameters: (as defined in the constructor of the implementation)
+  parameters: # as defined in the constructor of the implementation
     param1: value1
     param2: value2
+  vre_parameters: # also known as runtime parameters (post constructor). Calls repr.vre_setup()
+    device: "cuda" # for representations that have in their vre_setup() method a model.to(device) call
 
 name of representation 2:
   type: some other type
   name: some other method
-  dependencies: [name of representation]
+  dependencies: [name of representation] # since this representation depends on the prev one, it'll be computed after
   parameters: []
 ```
 
-Example cfg file: See [out of the box supported representations](cfgs/testCfg_ootb.yaml) and the CFG defined in
-the [CI process](.gitlab-ci.yml) for an actual export that is done at every commit on a real video.
+Example cfg file: See [out of the box supported representations](resources/cfgs/testCfg_ootb.yaml) and the CFG defined
+in the [CI process](test/end_to_end/imgur/run.sh) for an actual export that is done at every commit on a real video.
 
-Note: If the topological sort fails (because cycle dependencies), an error will be thrown.
+Note: If the topological sort fails (because of cycle dependencies), an error will be thrown.
 
 ## 4. Output format
 
 All the outputs are going to be stored as [0-1] float32 npz files, one for each frame in a directory specified by
 `--output_dir/-o`. A subdirectory will be created for each representation.
 
 For the above CFG file, 2 subdirectories will be created:
@@ -123,34 +115,31 @@
 
 In `bin/` we provide a secondary tool, `vre_collage` that takes all the png files from an output_dir as above and
 stacks them together in a single image. This is useful if we want to create a single image of all representations which
 can later be turned into a video as well.
 
 Usage:
 ```
-vre_collage /path/to/output_dir -o /path/to/collae_dir [--overwrite] [--video] [--fps] [--output_resolution H W]
+vre_collage /path/to/output_dir -o /path/to/collage_dir [--overwrite] [--video] [--fps] [--output_resolution H W]
 ```
 
-Note: This requries `media-processing-lib` to be installed (via pip).
-
 Note: you can also get video from a collage dir like this (in case you forgot to set --video or want more control):
 
 ```bash
-old_path=`pwd`
 cd /path/to/collage_dir
-ffmpeg -start_number 1 -framerate 30 -i %d.png -c:v libx264 -pix_fmt yuv420p $oldPath/collage.mp4;
-cd -;
+ffmpeg -start_number 1 -framerate 30 -i %d.png -c:v libx264 -pix_fmt yuv420p /path/to/collage.mp4;
 ```
 
 ### 5. Run in docker
-- use `meehai/vre:latest` from docker hub.
+
+We don't offer a pre-pushed vre image in dockerhub. You need to build it from vre-ci (used in CI duh):
 
 ```
-mkdir example
-# move the cfg and the video in some local dir
-gdown https://drive.google.com/uc?id=158U-W-Gal6eXxYtS1ca1DAAxHvknqwAk -O example/vid.mp4
-wget https://gitlab.com/meehai/video-representations-extractor/-/raw/df15af177edf5c101bbb241428c43faac333cea4/test/end_to_end/imgur/cfg.yaml -O example/cfg.yaml
-docker run \
-  -v `pwd`/example:/app/resources \
-  meehai/vre \
-  /app/resources/vid.mp4 --cfg_path /app/resources/cfg.yaml -o /app/resources/result --start_frame 5 --end_frame 6
+git clone https://gitlab.com/meehai/video-representations-extractor
+cd video-representations-extractor
+docker build . -f Dockerfile_run -t vre
+mkdir example/
+gdown https://drive.google.com/uc?id=158U-W-Gal6eXxYtS1ca1DAAxHvknqwAk -O example/video.mp4 # you can use your video
+cp resources/cfgs/testCfg_ootb.yaml example/cfg.yaml
+docker container run -v `pwd`/example:/app/resources vre /app/resources/video.mp4 \
+  --cfg_path /app/resources/cfg.yaml -o /app/resources/output_dir --start_frame 100 --end_frame 101
 ```
```

### Comparing `video-representations-extractor-1.0.3/README.md` & `video-representations-extractor-1.0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,41 @@
+Metadata-Version: 2.1
+Name: video-representations-extractor
+Version: 1.0.4
+Summary: Video Representations Extractor (VRE) for computing algorithmic or neural representations of each frame.
+Home-page: https://gitlab.com/meehai/video-representations-extractor
+License: WTFPL
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.TXT
+Requires-Dist: numpy>=1.21.6
+Requires-Dist: PyYAML==6.0
+Requires-Dist: pims==0.6.1
+Requires-Dist: tqdm==4.66.1
+Requires-Dist: natsort==8.2.0
+Requires-Dist: gdown==4.6.0
+Requires-Dist: torch==2.2.1
+Requires-Dist: torchvision==0.17.1
+Requires-Dist: timm==0.6.13
+Requires-Dist: transforms3d==0.4.1
+Requires-Dist: pyproj>=3.2.0
+Requires-Dist: overrides==7.3.1
+Requires-Dist: pandas==2.1.3
+Requires-Dist: matplotlib==3.7.1
+Requires-Dist: flow_vis==0.1
+Requires-Dist: colorama==0.4.6
+Requires-Dist: omegaconf==2.3.0
+Requires-Dist: lovely_tensors==0.1.15
+Requires-Dist: fvcore==0.1.5.post20221221
+Requires-Dist: pycocotools==2.0.7
+Requires-Dist: moviepy==1.0.3
+Requires-Dist: opencv-python==4.7.0.68
+Requires-Dist: Pillow==10.3.0
+Requires-Dist: scipy==1.8.1
+
 # Video Representation Extractor
 
 ![logo](logo.png)
 
 ## 1. Description
 
 The purpose of this repository is to export various representations starting from RGB videos only. Representations are
@@ -32,15 +66,15 @@
 ```
 git clone https://gitlab.com/meehai/video-representations-extractor [/some/dir]
 # in .bashrc
 export PYTHONPATH="$PYTHONPATH:/some/dir"
 export PATH="$PATH:/some/dir/bin"
 ```
 
-After eithrer option, you should be able to run:
+After either option, you should be able to run:
 ```bash
 vre <path/to/video.mp4> --cfg_path <path/to/cfg> -o <path/to/export_dir>
 ```
 
 The magic happens inside the config file, where we define *what* representations to extract and *what* parameters are
 used to instantiate said representations.
 
@@ -56,40 +90,42 @@
 Note: use `--cfg_path resources/cfgs/testCfg_ootb.yaml` for 'out of the box' working representations.
 
 Note2: Use `VRE_DEVICE=cuda vre...` to use cuda. For some representations, this speeds up the process by a lot.
 
 ## 3. CFG file
 
 The config file will have the hyperparameters required to instantiate each supported method as well as global
-hyperparameters for the output. This means that if a depth method is pre-traied for 0-300m, this information will be
-encoded in the CFG file and passed to the constructor of that particular depth method. There are also export level
-parameters, such as the output resolution of the representations.
+hyperparameters for the output. These parameters are sent to the constructor of each representation, so one can pass
+additional semantics to each representation, such as classes of a semantic segmentation or the maximum global depth
+value in meters.
 
 High level format:
 
 ```
 name of representation:
   type: some high level type (such as depth, semantic, edges, etc.)
   name: the implemented method's name (i.e. dexined, dpt, odoflow etc.)
   dependencies: [a list of dependencies given by their names]
-  parameters: (as defined in the constructor of the implementation)
+  parameters: # as defined in the constructor of the implementation
     param1: value1
     param2: value2
+  vre_parameters: # also known as runtime parameters (post constructor). Calls repr.vre_setup()
+    device: "cuda" # for representations that have in their vre_setup() method a model.to(device) call
 
 name of representation 2:
   type: some other type
   name: some other method
-  dependencies: [name of representation]
+  dependencies: [name of representation] # since this representation depends on the prev one, it'll be computed after
   parameters: []
 ```
 
-Example cfg file: See [out of the box supported representations](cfgs/testCfg_ootb.yaml) and the CFG defined in
-the [CI process](.gitlab-ci.yml) for an actual export that is done at every commit on a real video.
+Example cfg file: See [out of the box supported representations](resources/cfgs/testCfg_ootb.yaml) and the CFG defined
+in the [CI process](test/end_to_end/imgur/run.sh) for an actual export that is done at every commit on a real video.
 
-Note: If the topological sort fails (because cycle dependencies), an error will be thrown.
+Note: If the topological sort fails (because of cycle dependencies), an error will be thrown.
 
 ## 4. Output format
 
 All the outputs are going to be stored as [0-1] float32 npz files, one for each frame in a directory specified by
 `--output_dir/-o`. A subdirectory will be created for each representation.
 
 For the above CFG file, 2 subdirectories will be created:
@@ -113,34 +149,31 @@
 
 In `bin/` we provide a secondary tool, `vre_collage` that takes all the png files from an output_dir as above and
 stacks them together in a single image. This is useful if we want to create a single image of all representations which
 can later be turned into a video as well.
 
 Usage:
 ```
-vre_collage /path/to/output_dir -o /path/to/collae_dir [--overwrite] [--video] [--fps] [--output_resolution H W]
+vre_collage /path/to/output_dir -o /path/to/collage_dir [--overwrite] [--video] [--fps] [--output_resolution H W]
 ```
 
-Note: This requries `media-processing-lib` to be installed (via pip).
-
 Note: you can also get video from a collage dir like this (in case you forgot to set --video or want more control):
 
 ```bash
-old_path=`pwd`
 cd /path/to/collage_dir
-ffmpeg -start_number 1 -framerate 30 -i %d.png -c:v libx264 -pix_fmt yuv420p $oldPath/collage.mp4;
-cd -;
+ffmpeg -start_number 1 -framerate 30 -i %d.png -c:v libx264 -pix_fmt yuv420p /path/to/collage.mp4;
 ```
 
 ### 5. Run in docker
-- use `meehai/vre:latest` from docker hub.
+
+We don't offer a pre-pushed vre image in dockerhub. You need to build it from vre-ci (used in CI duh):
 
 ```
-mkdir example
-# move the cfg and the video in some local dir
-gdown https://drive.google.com/uc?id=158U-W-Gal6eXxYtS1ca1DAAxHvknqwAk -O example/vid.mp4
-wget https://gitlab.com/meehai/video-representations-extractor/-/raw/df15af177edf5c101bbb241428c43faac333cea4/test/end_to_end/imgur/cfg.yaml -O example/cfg.yaml
-docker run \
-  -v `pwd`/example:/app/resources \
-  meehai/vre \
-  /app/resources/vid.mp4 --cfg_path /app/resources/cfg.yaml -o /app/resources/result --start_frame 5 --end_frame 6
+git clone https://gitlab.com/meehai/video-representations-extractor
+cd video-representations-extractor
+docker build . -f Dockerfile_run -t vre
+mkdir example/
+gdown https://drive.google.com/uc?id=158U-W-Gal6eXxYtS1ca1DAAxHvknqwAk -O example/video.mp4 # you can use your video
+cp resources/cfgs/testCfg_ootb.yaml example/cfg.yaml
+docker container run -v `pwd`/example:/app/resources vre /app/resources/video.mp4 \
+  --cfg_path /app/resources/cfg.yaml -o /app/resources/output_dir --start_frame 100 --end_frame 101
 ```
```

### Comparing `video-representations-extractor-1.0.3/bin/vre` & `video-representations-extractor-1.0.4/bin/vre`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/bin/vre_collage` & `video-representations-extractor-1.0.4/bin/vre_collage`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python3
 """vre_collage tool"""
 from argparse import ArgumentParser
 from pathlib import Path
-from media_processing_lib.image import image_add_title, image_read, image_write, image_resize
-from media_processing_lib.collage_maker import collage_fn
 from natsort import natsorted
 from tqdm import tqdm
+from moviepy.editor import ImageSequenceClip
 import numpy as np
 
+from vre.utils import image_read, image_write, image_resize, image_add_title, collage_fn
 from vre.logger import logger
 
 def get_args():
     """Cli args"""
     parser = ArgumentParser()
     parser.add_argument("vre_export_dir", type=lambda p: Path(p).absolute(), help="Path to the dir where VRE exported")
     parser.add_argument("--output_path", "-o", required=False, help="Path to the collage is stored")
@@ -22,15 +22,15 @@
     # TODO: add order of collage
     args = parser.parse_args()
 
     if args.output_path is None:
         args.output_path = args.vre_export_dir / "collage"
         logger.warning(f"--output_path not provided, defaulting to '{args.output_path}'")
     args.output_path = Path(args.output_path).absolute()
-    assert not args.output_path.exists() or args.overwrite, f"Output path '{args.output_path}' exists. Use --overwrite."
+    # assert not args.output_path.exists() or args.overwrite, f"Output path '{args.output_path}' exists. Use --overwrite."
     assert args.video is False or args.fps is not None, "If video is set, --fps must also be set."
     return args
 
 def resolve_files(vre_export_dir: Path) -> dict[str, list[Path]]:
     """Gets a list of all images that are going to be used for the collage."""
     found_dirs = [x / "png" for x in vre_export_dir.iterdir() if (x / "png").exists()]
     repr_files = {}
@@ -59,22 +59,21 @@
     args.output_path.mkdir(parents=True, exist_ok=True)
     for current_frame_paths in tqdm(values, desc="collage images"):
         # export the png with the same name as all the other png from which it is constructed
         name = current_frame_paths[0].stem
         current_frames = [image_read(x) for x in current_frame_paths]
         h, w = current_frames[0].shape[0:2]
         # keep only first 25 chars of vre representation, otherwise the title is too long
-        trimmed_keys = [k[0:25] for k in keys]
+        titles = [k[0:25] for k in keys]
         h_out, w_out = args.output_resolution if args.output_resolution is not None else (h, w)
-        titled_frames = [image_add_title(image_resize(img, height=h_out, width=w_out), title, size_px=w_out // 15)
-                         for img, title in zip(current_frames, trimmed_keys)]
+        rsz_frames = [image_resize(img, height=h_out, width=w_out) for img in current_frames]
+        titled_frames = [image_add_title(img, title, size_px=w_out // 15, top_padding=w_out // 10)
+                         for img, title in zip(rsz_frames, titles)]
         img = collage_fn(titled_frames, pad_right=w_out // 75)
         image_write(img, args.output_path / f"{name}.png")
 
     if args.video:
-        from media_processing_lib.video.backends import DiskBackend
-        from media_processing_lib.video import MPLVideo
-        video = MPLVideo(DiskBackend(list(args.output_path.iterdir())), fps=args.fps)
-        video.save(args.output_path / "collage.mp4")
+        video = ImageSequenceClip([str(x) for x in args.output_path.glob("*.png")], fps=args.fps)
+        video.write_videofile(f"{args.output_path}/collage.mp4")
 
 if __name__ == "__main__":
     main()
```

### Comparing `video-representations-extractor-1.0.3/setup.py` & `video-representations-extractor-1.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """setup.py"""
 from pathlib import Path
 from setuptools import setup, find_packages
 
 NAME = "video-representations-extractor"
-VERSION = "1.0.3"
+VERSION = "1.0.4"
 DESCRIPTION = "Video Representations Extractor (VRE) for computing algorithmic or neural representations of each frame."
 URL = "https://gitlab.com/meehai/video-representations-extractor"
 
 with open(f"{Path(__file__).absolute().parent}/README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-REQUIRED = ["numpy>=1.21.6", "PyYAML==6.0", "argparse==1.1", "pims==0.6.1", "tqdm==4.66.1", "scikit-image==0.19.3",
-            "natsort==8.2.0", "gitpython==3.1.31", "gdown==4.6.0", "torch==2.2.1", "torchvision==0.17.1",
-            "timm==0.6.13", "transforms3d==0.4.1", "pyproj>=3.2.0", "overrides==7.3.1", "pandas==2.1.3",
-            "matplotlib==3.7.1", "flow_vis==0.1", "colorama==0.4.6", "omegaconf==2.3.0", "lovely_tensors==0.1.15",
-            "fvcore==0.1.5.post20221221", "pycocotools==2.0.7", "cloudpickle==3.0.0"]
+REQUIRED = ["numpy>=1.21.6", "PyYAML==6.0", "pims==0.6.1", "tqdm==4.66.1", "natsort==8.2.0", "gdown==4.6.0",
+            "torch==2.2.1", "torchvision==0.17.1", "timm==0.6.13", "transforms3d==0.4.1", "pyproj>=3.2.0",
+            "overrides==7.3.1", "pandas==2.1.3", "matplotlib==3.7.1", "flow_vis==0.1", "colorama==0.4.6",
+            "omegaconf==2.3.0", "lovely_tensors==0.1.15", "fvcore==0.1.5.post20221221", "pycocotools==2.0.7",
+            "moviepy==1.0.3", "opencv-python==4.7.0.68", "Pillow==10.3.0", "scipy==1.8.1"]
 
 setup(
     name=NAME,
     version=VERSION,
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `video-representations-extractor-1.0.3/video_representations_extractor.egg-info/PKG-INFO` & `video-representations-extractor-1.0.4/video_representations_extractor.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,40 @@
 Metadata-Version: 2.1
 Name: video-representations-extractor
-Version: 1.0.3
+Version: 1.0.4
 Summary: Video Representations Extractor (VRE) for computing algorithmic or neural representations of each frame.
 Home-page: https://gitlab.com/meehai/video-representations-extractor
 License: WTFPL
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.TXT
+Requires-Dist: numpy>=1.21.6
+Requires-Dist: PyYAML==6.0
+Requires-Dist: pims==0.6.1
+Requires-Dist: tqdm==4.66.1
+Requires-Dist: natsort==8.2.0
+Requires-Dist: gdown==4.6.0
+Requires-Dist: torch==2.2.1
+Requires-Dist: torchvision==0.17.1
+Requires-Dist: timm==0.6.13
+Requires-Dist: transforms3d==0.4.1
+Requires-Dist: pyproj>=3.2.0
+Requires-Dist: overrides==7.3.1
+Requires-Dist: pandas==2.1.3
+Requires-Dist: matplotlib==3.7.1
+Requires-Dist: flow_vis==0.1
+Requires-Dist: colorama==0.4.6
+Requires-Dist: omegaconf==2.3.0
+Requires-Dist: lovely_tensors==0.1.15
+Requires-Dist: fvcore==0.1.5.post20221221
+Requires-Dist: pycocotools==2.0.7
+Requires-Dist: moviepy==1.0.3
+Requires-Dist: opencv-python==4.7.0.68
+Requires-Dist: Pillow==10.3.0
+Requires-Dist: scipy==1.8.1
 
 # Video Representation Extractor
 
 ![logo](logo.png)
 
 ## 1. Description
 
@@ -42,15 +66,15 @@
 ```
 git clone https://gitlab.com/meehai/video-representations-extractor [/some/dir]
 # in .bashrc
 export PYTHONPATH="$PYTHONPATH:/some/dir"
 export PATH="$PATH:/some/dir/bin"
 ```
 
-After eithrer option, you should be able to run:
+After either option, you should be able to run:
 ```bash
 vre <path/to/video.mp4> --cfg_path <path/to/cfg> -o <path/to/export_dir>
 ```
 
 The magic happens inside the config file, where we define *what* representations to extract and *what* parameters are
 used to instantiate said representations.
 
@@ -66,40 +90,42 @@
 Note: use `--cfg_path resources/cfgs/testCfg_ootb.yaml` for 'out of the box' working representations.
 
 Note2: Use `VRE_DEVICE=cuda vre...` to use cuda. For some representations, this speeds up the process by a lot.
 
 ## 3. CFG file
 
 The config file will have the hyperparameters required to instantiate each supported method as well as global
-hyperparameters for the output. This means that if a depth method is pre-traied for 0-300m, this information will be
-encoded in the CFG file and passed to the constructor of that particular depth method. There are also export level
-parameters, such as the output resolution of the representations.
+hyperparameters for the output. These parameters are sent to the constructor of each representation, so one can pass
+additional semantics to each representation, such as classes of a semantic segmentation or the maximum global depth
+value in meters.
 
 High level format:
 
 ```
 name of representation:
   type: some high level type (such as depth, semantic, edges, etc.)
   name: the implemented method's name (i.e. dexined, dpt, odoflow etc.)
   dependencies: [a list of dependencies given by their names]
-  parameters: (as defined in the constructor of the implementation)
+  parameters: # as defined in the constructor of the implementation
     param1: value1
     param2: value2
+  vre_parameters: # also known as runtime parameters (post constructor). Calls repr.vre_setup()
+    device: "cuda" # for representations that have in their vre_setup() method a model.to(device) call
 
 name of representation 2:
   type: some other type
   name: some other method
-  dependencies: [name of representation]
+  dependencies: [name of representation] # since this representation depends on the prev one, it'll be computed after
   parameters: []
 ```
 
-Example cfg file: See [out of the box supported representations](cfgs/testCfg_ootb.yaml) and the CFG defined in
-the [CI process](.gitlab-ci.yml) for an actual export that is done at every commit on a real video.
+Example cfg file: See [out of the box supported representations](resources/cfgs/testCfg_ootb.yaml) and the CFG defined
+in the [CI process](test/end_to_end/imgur/run.sh) for an actual export that is done at every commit on a real video.
 
-Note: If the topological sort fails (because cycle dependencies), an error will be thrown.
+Note: If the topological sort fails (because of cycle dependencies), an error will be thrown.
 
 ## 4. Output format
 
 All the outputs are going to be stored as [0-1] float32 npz files, one for each frame in a directory specified by
 `--output_dir/-o`. A subdirectory will be created for each representation.
 
 For the above CFG file, 2 subdirectories will be created:
@@ -123,34 +149,31 @@
 
 In `bin/` we provide a secondary tool, `vre_collage` that takes all the png files from an output_dir as above and
 stacks them together in a single image. This is useful if we want to create a single image of all representations which
 can later be turned into a video as well.
 
 Usage:
 ```
-vre_collage /path/to/output_dir -o /path/to/collae_dir [--overwrite] [--video] [--fps] [--output_resolution H W]
+vre_collage /path/to/output_dir -o /path/to/collage_dir [--overwrite] [--video] [--fps] [--output_resolution H W]
 ```
 
-Note: This requries `media-processing-lib` to be installed (via pip).
-
 Note: you can also get video from a collage dir like this (in case you forgot to set --video or want more control):
 
 ```bash
-old_path=`pwd`
 cd /path/to/collage_dir
-ffmpeg -start_number 1 -framerate 30 -i %d.png -c:v libx264 -pix_fmt yuv420p $oldPath/collage.mp4;
-cd -;
+ffmpeg -start_number 1 -framerate 30 -i %d.png -c:v libx264 -pix_fmt yuv420p /path/to/collage.mp4;
 ```
 
 ### 5. Run in docker
-- use `meehai/vre:latest` from docker hub.
+
+We don't offer a pre-pushed vre image in dockerhub. You need to build it from vre-ci (used in CI duh):
 
 ```
-mkdir example
-# move the cfg and the video in some local dir
-gdown https://drive.google.com/uc?id=158U-W-Gal6eXxYtS1ca1DAAxHvknqwAk -O example/vid.mp4
-wget https://gitlab.com/meehai/video-representations-extractor/-/raw/df15af177edf5c101bbb241428c43faac333cea4/test/end_to_end/imgur/cfg.yaml -O example/cfg.yaml
-docker run \
-  -v `pwd`/example:/app/resources \
-  meehai/vre \
-  /app/resources/vid.mp4 --cfg_path /app/resources/cfg.yaml -o /app/resources/result --start_frame 5 --end_frame 6
+git clone https://gitlab.com/meehai/video-representations-extractor
+cd video-representations-extractor
+docker build . -f Dockerfile_run -t vre
+mkdir example/
+gdown https://drive.google.com/uc?id=158U-W-Gal6eXxYtS1ca1DAAxHvknqwAk -O example/video.mp4 # you can use your video
+cp resources/cfgs/testCfg_ootb.yaml example/cfg.yaml
+docker container run -v `pwd`/example:/app/resources vre /app/resources/video.mp4 \
+  --cfg_path /app/resources/cfg.yaml -o /app/resources/output_dir --start_frame 100 --end_frame 101
 ```
```

### Comparing `video-representations-extractor-1.0.3/video_representations_extractor.egg-info/SOURCES.txt` & `video-representations-extractor-1.0.4/video_representations_extractor.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -168,9 +168,10 @@
 vre/representations/soft_segmentation/fastsam/ultralytics/yolo/utils/__init__.py
 vre/representations/soft_segmentation/generalized_boundaries/__init__.py
 vre/representations/soft_segmentation/generalized_boundaries/generalized_boundaries.py
 vre/representations/soft_segmentation/halftone/__init__.py
 vre/representations/soft_segmentation/halftone/halftone.py
 vre/utils/__init__.py
 vre/utils/fake_video.py
+vre/utils/image.py
 vre/utils/topological_sort.py
 vre/utils/utils.py
```

### Comparing `video-representations-extractor-1.0.3/vre/data_storer.py` & `video-representations-extractor-1.0.4/vre/data_storer.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/logger.py` & `video-representations-extractor-1.0.4/vre/logger.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representation.py` & `video-representations-extractor-1.0.4/vre/representation.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/build_representations.py` & `video-representations-extractor-1.0.4/vre/representations/build_representations.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/depth/dpt/depth_dpt.py` & `video-representations-extractor-1.0.4/vre/representations/depth/dpt/depth_dpt.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/depth/dpt/dpt_impl/blocks.py` & `video-representations-extractor-1.0.4/vre/representations/depth/dpt/dpt_impl/blocks.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/depth/dpt/dpt_impl/dpt_depth.py` & `video-representations-extractor-1.0.4/vre/representations/depth/dpt/dpt_impl/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/depth/dpt/dpt_impl/vit.py` & `video-representations-extractor-1.0.4/vre/representations/depth/dpt/dpt_impl/vit.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/depth/odo_flow/depth_odo_flow.py` & `video-representations-extractor-1.0.4/vre/representations/depth/odo_flow/depth_odo_flow.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,23 +8,20 @@
 from ....representation import Representation, RepresentationOutput
 from ....logger import logger
 from ....utils import image_resize_batch, VREVideo, get_weights_dir
 
 
 class DepthOdoFlow(Representation):
     """Depth from optical flow and odometry."""
-    def __init__(self, linear_ang_vel_correction: bool, focus_correction: bool,
-                 cosine_correction_scipy: bool, cosine_correction_gd: bool, sensor_fov: int, sensor_width: int,
+    def __init__(self, linear_ang_vel_correction: bool, focus_correction: bool, sensor_fov: int, sensor_width: int,
                  sensor_height: int, min_depth_meters: int, max_depth_meters: int, **kwargs):
         super().__init__(**kwargs)
 
         self.linear_ang_vel_correction = linear_ang_vel_correction
         self.focus_correction = focus_correction
-        self.cosine_correction_scipy = cosine_correction_scipy
-        self.cosine_correction_gd = cosine_correction_gd
         self.min_depth_meters = min_depth_meters
         self.max_depth_meters = max_depth_meters
         # TODO: thresholds picked for flow at 960x540; scaled correspondingly in filter function
         self.thresholds = {
             "Z": 0,
             ("Z", "around_focus_expansion_A"): 20,
             "angle (deg)": 20,
@@ -75,17 +72,15 @@
 
         if not self.camera_info.has_K():
             self.camera_info.frame_resolution = (flow_width, flow_height)
         flows = flows / self.camera_info.dt
 
         Zs, As, bs, derotating_flows, batch_ang_velc = depth_from_flow(flows, lin_vel, ang_vel, self.camera_info.K,
                                                                        self.linear_ang_vel_correction,
-                                                                       self.focus_correction,
-                                                                       self.cosine_correction_gd,
-                                                                       self.cosine_correction_scipy)
+                                                                       self.focus_correction)
         valid = filter_depth_from_flow(Zs, As, bs, derotating_flows, thresholds=self.thresholds)
 
         Zs[~valid] = np.nan
         depth = np.clip(Zs.astype(np.float32), self.min_depth_meters, self.max_depth_meters)
         depth = (depth - self.min_depth_meters) / (self.max_depth_meters - self.min_depth_meters)
         depth[~np.isfinite(depth)] = 1
```

### Comparing `video-representations-extractor-1.0.3/vre/representations/depth/odo_flow/odo_flow_impl/cam.py` & `video-representations-extractor-1.0.4/vre/representations/depth/odo_flow/odo_flow_impl/cam.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/depth/odo_flow/odo_flow_impl/camera_info.py` & `video-representations-extractor-1.0.4/vre/representations/depth/odo_flow/odo_flow_impl/camera_info.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/depth/odo_flow/odo_flow_impl/depth_from_flow.py` & `video-representations-extractor-1.0.4/vre/representations/depth/odo_flow/odo_flow_impl/depth_from_flow.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # pylint: disable=all
 import numpy as np
 import torch
-from skimage.filters import gaussian
-from scipy import optimize
-
+from scipy import ndimage as ndi
 
 from .polyfit import linear_least_squares
 
 
 def solve_delta_ang_vel_old(jacobian_z, jacobian_ang_vel, b):
     # A is 2 x W x H
     _, W, H = jacobian_z.shape
@@ -291,17 +289,16 @@
     A_norm_sq_all = np.sum(np.square(A), axis=-1)
     Ab_all = np.sum(A * b, axis=-1)
     # N_frames x N_points
     Z = Ab_all / A_norm_sq_all
     return Z
 
 
-def depth_from_flow(batched_flow, linear_velocity, angular_velocity, K,
-                    adjust_ang_vel=True, use_focus_correction=False, use_cosine_correction_gd=False,
-                    use_cosine_correction_scipy=False, mesh_grid=None, axis=("x", "y", "xy")[2]):
+def depth_from_flow(batched_flow, linear_velocity, angular_velocity, K, adjust_ang_vel=True, use_focus_correction=False,
+                    use_cosine_correction_gd=True, mesh_grid=None, axis=("x", "y", "xy")[2]):
     f_u, f_v = K[0, 0], K[1, 1]
     u0, v0 = K[0, 2], K[1, 2]
 
     H, W = batched_flow.shape[-2:]
 
     if mesh_grid is not None:
         us_bar, vs_bar = mesh_grid
@@ -354,18 +351,14 @@
         for b_ind in range(B):
             ang_vel_correction[b_ind] = focus_corection(angular_velocity[b_ind], linear_velocity[b_ind],
                                                         f_u, (int(u0), int(v0)), b[b_ind])
     if use_cosine_correction_gd:
         for b_ind in range(B):
             ang_vel_correction[b_ind] = cosine_correction_torch(b[b_ind], A[b_ind], J_w,
                                                                 initial_delta=ang_vel_correction[b_ind], b_ind=b_ind)
-    if use_cosine_correction_scipy:
-        for b_ind in range(B):
-            ang_vel_correction[b_ind] = cosine_correction_scipy(b[b_ind], A[b_ind], J_w,
-                                                                initial_delta=ang_vel_correction[b_ind], b_ind=b_ind)
 
     angular_velocity = angular_velocity - ang_vel_correction
     derotating_flow = get_derotating_flow(J_w, angular_velocity)
     b = batched_flow - derotating_flow
 
     if axis == "xy":
         norm_A_squared = np.sum(np.square(A), axis=1)
@@ -530,19 +523,44 @@
         feature_data = np.linalg.norm(As, axis=1)
     # if mask_region == "top_half":
     #     H, W, = feature_data.shape[-2:]
     #     feature_data[:, int(H // 2):] = np.nan
 
     return feature_data
 
+def gaussian(
+    image,
+    sigma=1,
+    mode='nearest',
+    cval=0,
+    preserve_range=False,
+    truncate=4.0,
+    *,
+    channel_axis=None,
+    out=None,
+):
+    """Multi-dimensional Gaussian filter."""
+    if np.any(np.asarray(sigma) < 0.0):
+        raise ValueError("Sigma values less than zero are not valid")
+    if channel_axis is not None:
+        # do not filter across channels
+        if not isinstance(sigma, (list, tuple)):
+            sigma = [sigma] * (image.ndim - 1)
+        if len(sigma) == image.ndim - 1:
+            sigma = list(sigma)
+            sigma.insert(channel_axis % image.ndim, 0)
+    assert image.dtype == np.float64, image.dtype
+    if (out is not None) and (not np.issubdtype(out.dtype, np.floating)):
+        raise ValueError(f"dtype of `out` must be float; got {out.dtype!r}.")
+    return ndi.gaussian_filter(
+        image, sigma, output=out, mode=mode, cval=cval, truncate=truncate
+    )
 
 def focus_corection(ang_vel, lin_vel, f, c, b):
     # speed check
-    low_axis_threshold = 0.1
-    low_ang_vel_threshold = 0.05
     window_size = 5
     use_real_minimum = True
     approximate_out_of_image = True
 
     # init
     dw = np.zeros(3)
     focus_correction_valid = True
@@ -579,25 +597,16 @@
 
         jw = np.array([[u * v / f, -(f ** 2 + u ** 2) / f, v],
                        [(f ** 2 + v ** 2) / f, -u * v / f, -u]])[None]
 
         jw = np.delete(jw, ang_low_idx, axis=2)
         jw = jw.reshape(jw.shape[0] * 2, 2)
 
-        # tg = np.array([-b[:, v + c[1], u + c[0]] for u, v in xy])
-        # tg = np.array([b[:, focus_real[0], focus_real[1]] - b[:, v + c[1], u + c[0]] for u, v in xy])
-        # tg = tg.mean(axis=0)
-        # tg = tg.flatten()
-
         tg = -b[:, yw[0]:yw[1], xw[0]:xw[1]]
-        # print(tg.shape)
         tg = tg.reshape(-1, tg.shape[1] * tg.shape[2]).mean(axis=1)
-        # tg = tg.flatten()
-        # print(tg.shape)
-        # print(tg)
 
         if use_real_minimum:
             norm = np.sqrt((b ** 2).sum(axis=0))
             # idx = np.argmin(norm)
             idx = np.argmin(gaussian(norm, sigma=2))
             yf, xf = np.unravel_index(idx, norm.shape)
             tg += b[:, yf, xf]
@@ -606,50 +615,14 @@
             dw = np.linalg.lstsq(jw, tg, rcond=None)[0]
             dw = np.insert(dw, ang_low_idx, 0, axis=0)
         except np.linalg.LinAlgError:
             pass
 
     return dw
 
-
-def cosine_correction_scipy(b, A, Jw, initial_delta=None, b_ind=None):
-    if initial_delta is not None:
-        dw = initial_delta
-    else:
-        dw = np.zeros(3)
-
-    A = A.transpose((1, 2, 0)).reshape(A.shape[1] * A.shape[2], 2)
-    b = b.transpose((1, 2, 0)).reshape(b.shape[1] * b.shape[2], 2)
-    Jw = Jw.transpose((2, 3, 0, 1)).reshape(Jw.shape[2] * Jw.shape[3], 2, 3)
-
-    Au, Av = A[:, :1], A[:, 1:]
-    bu, bv = b[:, :1], b[:, 1:]
-    Ju, Jv = Jw[:, 0], Jw[:, 1]
-
-    Ab = (A * b).sum(axis=1)[..., None]
-    nA2 = (A ** 2).sum(axis=1)[..., None]
-    AJ = Au * Ju + Av * Jv
-
-    def sim_loss(w):
-        w = w[..., None]
-        cos = (1 - (Ab + AJ @ w) / (np.sqrt(nA2) * np.sqrt((bu + Ju @ w) ** 2 + (bv + Jv @ w) ** 2))).mean()
-        return cos
-
-    res = optimize.minimize(sim_loss, dw, method='Nelder-Mead')
-    dw = res.x
-
-    if np.linalg.norm(dw) < 0.02:
-        dw = dw
-    else:
-        dw = np.zeros(3)
-        # print(b_ind, 'trigger norm', np.linalg.norm(dw))
-
-    return dw
-
-
 def cosine_correction_torch(b, A, Jw, initial_delta=None, b_ind=None):
     n_optim_steps = 50
     lr = 1e-4
     stop_cond = 1e-12
 
     if initial_delta is not None:
         dw = initial_delta
```

### Comparing `video-representations-extractor-1.0.3/vre/representations/depth/odo_flow/odo_flow_impl/loss.py` & `video-representations-extractor-1.0.4/vre/representations/depth/odo_flow/odo_flow_impl/loss.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/depth/odo_flow/odo_flow_impl/polyfit.py` & `video-representations-extractor-1.0.4/vre/representations/depth/odo_flow/odo_flow_impl/polyfit.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/depth/odo_flow/odo_flow_impl/utils.py` & `video-representations-extractor-1.0.4/vre/representations/depth/odo_flow/odo_flow_impl/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # pylint: disable=all
 from pathlib import Path
 import numpy as np
 import multiprocessing
-from sklearn.preprocessing import MinMaxScaler
-from matplotlib import cm
 import torch
 from tqdm import tqdm
 from collections import defaultdict
 
 import pandas as pd
 from matplotlib import pyplot as plt
 
@@ -234,22 +232,14 @@
     return np.stack((x, y, z), axis=2)
 
 
 def depth_to_pointcloud(depth, normalized_coords):
     return depth[:, :, None] * normalized_coords
 
 
-def get_colors(cmap_name='gist_rainbow', number_of_colors=10, xs=None):
-    map = cm.get_cmap(cmap_name)
-    if xs is None and number_of_colors:
-        xs = np.linspace(0, 1, number_of_colors)
-    colors = map(MinMaxScaler().fit_transform(xs.reshape(-1, 1)).flatten())
-    return colors[:, :3]
-
-
 LINE_STYLES = ('solid', 'dashed', 'dashdot', 'dotted')
 def get_linestyles(number_of_elements, styleset=LINE_STYLES):
     styles = []
     for i in range(number_of_elements):
         styles.append(styleset[i % len(styleset)])
     return styles
```

### Comparing `video-representations-extractor-1.0.3/vre/representations/depth/odo_flow/odo_flow_impl/utils_geometry.py` & `video-representations-extractor-1.0.4/vre/representations/depth/odo_flow/odo_flow_impl/utils_geometry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 # pylint: disable=all
 import pyproj
 from scipy import integrate
 from scipy.spatial.transform import Rotation, Slerp, RotationSpline
-from sklearn.base import BaseEstimator
-from sklearn.decomposition import PCA
-from sklearn.linear_model import RANSACRegressor
+from scipy.interpolate import interp1d
 import numpy as np
 from transforms3d import quaternions as quat, euler, axangles
-from scipy.interpolate import interp1d
 
-
-from .utils import closest_indexes, nn_interpolation
+from .utils import nn_interpolation
 
 
 def transform_points(camera_pose, points):
     if len(points) == 0:
         return points
     R, t = camera_pose
     points_out = (R @ points.T).T + t.reshape(1, -1)
@@ -38,26 +34,14 @@
 
 def pose_to_matrix(pose):
     T = np.zeros((4, 4))
     T[:3, :3] = pose[0]
     T[:3, 3] = pose[1]
     return T
 
-
-def fit_plane(X):
-    pca = PCA(n_components=3)
-    pca.fit(X)
-    eigenvectors, eigenvalues = pca.components_, pca.singular_values_
-    normal = eigenvectors[-1]
-    pt = np.mean(X, axis=0)
-    a, b, c, = normal
-    d = - (np.dot(normal, pt))
-    return a, b, c, d
-
-
 def get_plane_pose(plane):
     A, B, C, D = plane
     # two different points on the plane
     p1 = np.array((0, 0, -D / C))
     p2 = np.array((-D / A, 0, 0))
 
     # relative vectors defines a direction parallel to the plane
@@ -202,21 +186,14 @@
 
 def interp_vectors(source_t, vectors, target_t):
     target_t_mask = np.logical_and(source_t[0] <= target_t, source_t[-1] >= target_t)
     interp_vectors = interp1d(source_t, vectors, axis=0)(target_t[target_t_mask])
     return nn_interpolation(target_t, interp_vectors, target_t[target_t_mask])
 
 
-def get_planar_trajectory_coords(coords):
-    plane = fit_plane(coords)
-    pose = get_plane_pose(plane)
-    plane_points = transform_points(invert_pose(*pose), coords)
-    return plane_points
-
-
 def diff_rot(orientations, ts, type='central'):
     angle_vels = []
     for ind in range(len(orientations)):
         prev_ind = next_ind = ind
         if type in ['central', 'left', 'right']:
             if type in ['central', 'left']:
                 prev_ind = max(0, ind - 1)
```

### Comparing `video-representations-extractor-1.0.3/vre/representations/dummy_representation.py` & `video-representations-extractor-1.0.4/vre/representations/dummy_representation.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/edges/canny.py` & `video-representations-extractor-1.0.4/vre/representations/edges/canny.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/edges/dexined/dexined.py` & `video-representations-extractor-1.0.4/vre/representations/edges/dexined/dexined.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/edges/dexined/model_dexined.py` & `video-representations-extractor-1.0.4/vre/representations/edges/dexined/model_dexined.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/hsv.py` & `video-representations-extractor-1.0.4/vre/representations/rgb.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-"""HSV module"""
+"""RGB representation"""
 import numpy as np
 from overrides import overrides
-from skimage.color import rgb2hsv
 from ..representation import Representation, RepresentationOutput
 from ..utils import image_resize_batch
 
-class HSV(Representation):
-    """HSV representation"""
+class RGB(Representation):
+    """RGB representation"""
     @overrides
     def make(self, frames: np.ndarray) -> RepresentationOutput:
-        return rgb2hsv(frames).astype(np.float32)
+        return frames
 
     @overrides
     def make_images(self, frames: np.ndarray, repr_data: RepresentationOutput) -> np.ndarray:
-        return (repr_data * 255).astype(np.uint8)
+        return repr_data
 
     @overrides
     def size(self, repr_data: RepresentationOutput) -> tuple[int, int]:
         return repr_data.shape[1:3]
 
     @overrides
     def resize(self, repr_data: RepresentationOutput, new_size: tuple[int, int]) -> RepresentationOutput:
```

### Comparing `video-representations-extractor-1.0.3/vre/representations/normals/depth_svd/depth_normals_svd.py` & `video-representations-extractor-1.0.4/vre/representations/normals/depth_svd/depth_normals_svd.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/normals/depth_svd/depth_svd_impl/cam.py` & `video-representations-extractor-1.0.4/vre/representations/normals/depth_svd/depth_svd_impl/cam.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/normals/depth_svd/depth_svd_impl/utils.py` & `video-representations-extractor-1.0.4/vre/representations/normals/depth_svd/depth_svd_impl/utils.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/optical_flow/raft/flow_raft.py` & `video-representations-extractor-1.0.4/vre/representations/optical_flow/raft/flow_raft.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/optical_flow/raft/raft_impl/corr.py` & `video-representations-extractor-1.0.4/vre/representations/optical_flow/raft/raft_impl/corr.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/optical_flow/raft/raft_impl/datasets.py` & `video-representations-extractor-1.0.4/vre/representations/optical_flow/raft/raft_impl/datasets.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/optical_flow/raft/raft_impl/extractor.py` & `video-representations-extractor-1.0.4/vre/representations/optical_flow/raft/raft_impl/extractor.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/optical_flow/raft/raft_impl/raft.py` & `video-representations-extractor-1.0.4/vre/representations/optical_flow/raft/raft_impl/raft.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/optical_flow/raft/raft_impl/update.py` & `video-representations-extractor-1.0.4/vre/representations/optical_flow/raft/raft_impl/update.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/optical_flow/raft/raft_impl/utils.py` & `video-representations-extractor-1.0.4/vre/representations/optical_flow/raft/raft_impl/utils.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/optical_flow/rife/flow_rife.py` & `video-representations-extractor-1.0.4/vre/representations/optical_flow/rife/flow_rife.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/optical_flow/rife/rife_impl/IFNet_HD.py` & `video-representations-extractor-1.0.4/vre/representations/optical_flow/rife/rife_impl/IFNet_HD.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/optical_flow/rife/rife_impl/IFNet_HDv2.py` & `video-representations-extractor-1.0.4/vre/representations/optical_flow/rife/rife_impl/IFNet_HDv2.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/optical_flow/rife/rife_impl/RIFE_HDv2.py` & `video-representations-extractor-1.0.4/vre/representations/optical_flow/rife/rife_impl/RIFE_HDv2.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/optical_flow/rife/rife_impl/loss.py` & `video-representations-extractor-1.0.4/vre/representations/optical_flow/rife/rife_impl/loss.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/optical_flow/rife/rife_impl/warplayer.py` & `video-representations-extractor-1.0.4/vre/representations/optical_flow/rife/rife_impl/warplayer.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/convert.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/convert.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,46 @@
 """Mask2Former representation"""
 import json
+from argparse import ArgumentParser, Namespace
 from pathlib import Path
-import sys
+from datetime import datetime
 from overrides import overrides
 import torch as tr
 from torch import nn
 import numpy as np
 from lovely_tensors import monkey_patch
-from PIL import Image
 from fvcore.common.config import CfgNode
 
-monkey_patch()
+from vre.representation import Representation, RepresentationOutput
+from vre.logger import logger
+from vre.utils import gdown_mkdir, image_resize_batch, VREVideo, get_weights_dir, image_read, image_write
 
 try:
     from .mask2former_impl import MaskFormer as MaskFormerImpl
     from .mask2former_impl.det2_data import MetadataCatalog
     from .mask2former_impl.visualizer import Visualizer, ColorMode
-    from ....representation import Representation, RepresentationOutput
-    from ....logger import logger
-    from ....utils import gdown_mkdir, image_resize_batch, VREVideo, get_weights_dir
 except ImportError: # when running this script directly
     from mask2former_impl import MaskFormer as MaskFormerImpl
     from mask2former_impl.visualizer import Visualizer, ColorMode
     from mask2former_impl.det2_data import MetadataCatalog
-    from vre.representation import Representation, RepresentationOutput
-    from vre.logger import logger
-    from vre.utils import gdown_mkdir, image_resize_batch, VREVideo, get_weights_dir
+
+monkey_patch()
 
 def get_output_shape(oldh: int, oldw: int, short_edge_length: int, max_size: int):
     """
     Compute the output size given input size and target short edge length.
     """
-    h, w = oldh, oldw
-    scale = short_edge_length / min(h, w)
-    newh, neww = (short_edge_length, scale * w) if h < w else (scale * h, short_edge_length)
+    scale = short_edge_length / min(oldh, oldw)
+    newh, neww = (short_edge_length, scale * oldw) if oldh < oldw else (scale * oldh, short_edge_length)
     if max(newh, neww) > max_size:
         scale = max_size * 1.0 / max(newh, neww)
-        newh = newh * scale
-        neww = neww * scale
+        newh, neww = newh * scale, neww * scale
     neww, newh = int(neww + 0.5), int(newh + 0.5)
     return newh, neww
 
-def apply_image(img: np.ndarray, h, w, new_h, new_w):
-    """apply image transform -- see if we need the non uint8 variant"""
-    assert img.shape[:2] == (h, w)
-    assert len(img.shape) <= 4
-    interp_method = Image.BILINEAR
-    assert img.dtype == np.uint8, img.dtype
-
-    if len(img.shape) > 2 and img.shape[2] == 1:
-        pil_image = Image.fromarray(img[:, :, 0], mode="L")
-    else:
-        pil_image = Image.fromarray(img)
-    pil_image = pil_image.resize((new_w, new_h), interp_method)
-    ret = np.asarray(pil_image)
-    if len(img.shape) > 2 and img.shape[2] == 1:
-        ret = np.expand_dims(ret, -1)
-    return ret
-
 class Mask2Former(Representation):
     """Mask2Former representation implementation. Note: only semantic segmentation (not panoptic/instance) enabled."""
     def __init__(self, model_id: str, semantic_argmax_only: bool, **kwargs):
         super().__init__(**kwargs)
         weights_path = self._get_weights(model_id)
         self.model, self.cfg, self.metadata = self._build_model(weights_path)
         self.model_id = model_id
@@ -75,15 +54,15 @@
         self.device = device
 
     @tr.no_grad()
     @overrides
     def make(self, frames: np.ndarray) -> RepresentationOutput:
         height, width = frames.shape[1:3]
         _os = get_output_shape(height, width, self.cfg.INPUT.MIN_SIZE_TEST, self.cfg.INPUT.MAX_SIZE_TEST)
-        imgs = [apply_image(img, height, width, _os[0], _os[1]).astype("float32").transpose(2, 0, 1) for img in frames]
+        imgs = image_resize_batch(frames, _os[0], _os[1], "bilinear", "PIL").transpose(0, 3, 1, 2).astype("float32")
         inputs = [{"image": tr.from_numpy(img), "height": height, "width": width} for img in imgs]
         predictions = [x["sem_seg"] for x in self.model(inputs)]
         res = []
         for pred in predictions:
             _pred = pred.argmax(0).byte() if self.semantic_argmax_only else pred.half().permute(1, 2, 0)
             res.append(_pred.to("cpu").numpy())
         return np.stack(res)
@@ -129,46 +108,53 @@
     def _build_model(self, weights_path: Path | dict) -> tuple[nn.Module, CfgNode, MetadataCatalog]:
         ckpt_data = tr.load(weights_path, map_location="cpu") if isinstance(weights_path, Path) else weights_path
         cfg = CfgNode(json.loads(ckpt_data["cfg"]))
         params = MaskFormerImpl.from_config(cfg)
         params = {**params, "semantic_on": True, "panoptic_on": False, "instance_on": False}
         model = MaskFormerImpl(**params).eval()
         res = model.load_state_dict(ckpt_data["state_dict"], strict=False) # inference only: we remove criterion
-        assert res.unexpected_keys == ["criterion.empty_weight"] or res.unexpected_keys == [], res
+        assert res.unexpected_keys in (["criterion.empty_weight"], []), res
         model.to("cuda" if tr.cuda.is_available() else "cpu")
         assert len(cfg.DATASETS.TEST) == 1, cfg.DATASETS.TEST
         metadata = MetadataCatalog.get(cfg.DATASETS.TEST[0])
         logger.debug(f"Loade weights from '{weights_path}'")
         return model, cfg, metadata
 
     def __del__(self):
         del self.model
 
-def main():
+def get_args() -> Namespace:
+    """cli args"""
+    parser = ArgumentParser()
+    parser.add_argument("model_id_or_path")
+    parser.add_argument("input_image", type=Path)
+    parser.add_argument("output_path", type=Path)
+    parser.add_argument("--n_tries", type=int, default=1)
+    return parser.parse_args()
+
+def main(args: Namespace):
     """main fn. Usage: python mask2former.py 49189528_1/47429163_0/49189528_0 demo1.jpg output1.jpg"""
-    from datetime import datetime # pylint: disable=all
-    from media_processing_lib.image import image_read, image_write # pylint: disable=all
-    assert len(sys.argv) == 4
-    img = image_read(sys.argv[2])
+    img = image_read(args.input_image)
 
-    m2f = Mask2Former(sys.argv[1], semantic_argmax_only=False, name="m2f", dependencies=[])
+    m2f = Mask2Former(args.model_id_or_path, semantic_argmax_only=False, name="m2f", dependencies=[])
     m2f.model.to("cuda" if tr.cuda.is_available() else "cpu")
-    for _ in range(1):
+    for _ in range(args.n_tries):
         now = datetime.now()
         pred = m2f.make(img[None])
-        print(f"Pred took: {datetime.now() - now}")
+        logger.info(f"Pred took: {datetime.now() - now}")
         semantic_result = m2f.make_images(img[None], pred)[0]
-        image_write(semantic_result, sys.argv[3])
+        image_write(semantic_result, args.output_path)
+    logger.info(f"Written prediction to '{args.output_path}'")
 
     # Sanity checks
-    if m2f.model_id == "47429163_0" and Path(sys.argv[2]).name == "demo1.jpg":
+    if m2f.model_id == "47429163_0" and args.input_image.name == "demo1.jpg":
         assert np.allclose(mean := semantic_result.mean(), 129.41173), (mean, semantic_result.std())
         assert np.allclose(std := semantic_result.std(), 53.33731), std
-    elif m2f.model_id == "49189528_1" and Path(sys.argv[2]).name == "demo1.jpg":
+    elif m2f.model_id == "49189528_1" and args.input_image.name == "demo1.jpg":
         assert np.allclose(mean := semantic_result.mean(), 125.23281), (mean, semantic_result.std())
         assert np.allclose(std := semantic_result.std(), 48.89948), std
-    elif m2f.model_id == "49189528_0" and Path(sys.argv[2]).name == "demo1.jpg":
+    elif m2f.model_id == "49189528_0" and args.input_image.name == "demo1.jpg":
         assert np.allclose(mean := semantic_result.mean(), 118.47982), (mean, semantic_result.std())
         assert np.allclose(std := semantic_result.std(), 52.08105), std
 
 if __name__ == "__main__":
-    main()
+    main(get_args())
```

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/comm.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/comm.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_ade20k_full.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_ade20k_full.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_ade20k_instance.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_ade20k_instance.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_ade20k_panoptic.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_ade20k_panoptic.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_coco_panoptic_annos_semseg.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_coco_panoptic_annos_semseg.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_coco_stuff_10k.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_coco_stuff_10k.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_mapillary_vistas.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_mapillary_vistas.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_mapillary_vistas_panoptic.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_mapillary_vistas_panoptic.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/__init__.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/__init__.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/benchmark.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/benchmark.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/build.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/build.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/catalog.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/catalog.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/common.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,35 +8,31 @@
 import pickle
 import random
 from typing import Callable, Union
 import torch
 import torch.utils.data as data
 from torch.utils.data.sampler import Sampler
 
-import cloudpickle
-
 class PicklableWrapper:
     """
     Wrap an object to make it more picklable, note that it uses
     heavy weight serialization libraries that are slower than pickle.
     It's best to use it only on closures (which are usually not picklable).
-
-    This is a simplified version of
-    https://github.com/joblib/joblib/blob/master/joblib/externals/loky/cloudpickle_wrapper.py
     """
 
     def __init__(self, obj):
         while isinstance(obj, PicklableWrapper):
+            print("lala")
             # Wrapping an object twice is no-op
             obj = obj._obj
         self._obj = obj
 
     def __reduce__(self):
-        s = cloudpickle.dumps(self._obj)
-        return cloudpickle.loads, (s,)
+        s = pickle.dumps(self._obj)
+        return pickle.loads, (s,)
 
     def __call__(self, *args, **kwargs):
         return self._obj(*args, **kwargs)
 
     def __getattr__(self, attr):
         # Ensure that the wrapped object can be used seamlessly as the previous object.
         if attr not in ["_obj"]:
```

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/dataset_mapper.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/dataset_mapper.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/__init__.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/builtin.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/builtin.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/builtin_meta.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/builtin_meta.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/cityscapes.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/cityscapes_panoptic.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/cityscapes_panoptic.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/coco.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/coco_panoptic.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/coco_panoptic.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis_v0_5_categories.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis_v0_5_categories.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis_v1_categories.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis_v1_categories.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis_v1_category_image_count.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis_v1_category_image_count.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/pascal_voc.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/detection_utils.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/detection_utils.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/samplers/distributed_sampler.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/samplers/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/samplers/grouped_batch_sampler.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/samplers/grouped_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/augmentation.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/augmentation.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/augmentation_impl.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/augmentation_impl.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/transform.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/file_io.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/file_io.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/blocks.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/blocks.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/deform_conv.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/deform_conv.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/norm.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/norm.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/shape_spec.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/shape_spec.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/wrappers.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/wrappers.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/maskformer_model.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/maskformer_model.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/backbone/swin.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/backbone/swin.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/meta_arch/mask_former_head.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/meta_arch/mask_former_head.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/fpn.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/fpn.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/ms_deform_attn.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/ms_deform_attn.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/msdeformattn.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/msdeformattn.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/resnet.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/resnet.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/mask2former_transformer_decoder.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/mask2former_transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/maskformer_transformer_decoder.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/maskformer_transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/position_encoding.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/position_encoding.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/transformer.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/transformer.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/boxes.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/boxes.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/image_list.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/image_list.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/instances.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/instances.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/keypoints.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/keypoints.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/masks.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/masks.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/rotated_boxes.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/mask2former/mask2former_impl/visualizer.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/mask2former/mask2former_impl/visualizer.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/safeuav/Map2Map.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/safeuav/Map2Map.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/semantic_segmentation/safeuav/safeuav.py` & `video-representations-extractor-1.0.4/vre/representations/semantic_segmentation/safeuav/safeuav.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/fastsam.py` & `video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/fastsam.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """FastSAM representation."""
-from overrides import overrides
+from argparse import ArgumentParser, Namespace
+from datetime import datetime
+from pathlib import Path
 import numpy as np
 import torch as tr
+from overrides import overrides
 from torch.nn import functional as F
 
+from vre.representation import Representation, RepresentationOutput
+from vre.utils import gdown_mkdir, VREVideo, image_resize_batch, get_weights_dir, image_read, image_write
+from vre.logger import logger
+
 try:
     from .fastsam_impl import FastSAM as Model, FastSAMPredictor, FastSAMPrompt
     from .fastsam_impl.results import Results
     from .fastsam_impl.utils import bbox_iou
     from .fastsam_impl.ops import scale_boxes, non_max_suppression, process_mask_native
-    from ....representation import Representation, RepresentationOutput
-    from ....utils import gdown_mkdir, VREVideo, image_resize_batch, get_weights_dir
 except ImportError:
     from fastsam_impl import FastSAM as Model, FastSAMPredictor, FastSAMPrompt
     from fastsam_impl.results import Results
     from fastsam_impl.utils import bbox_iou
     from fastsam_impl.ops import scale_boxes, non_max_suppression, process_mask_native
-    from vre.representation import Representation, RepresentationOutput
-    from vre.utils import gdown_mkdir, VREVideo, image_resize_batch, get_weights_dir
 
 class FastSam(Representation):
     """FastSAM representation."""
     def __init__(self, variant: str, iou: float, conf: float, **kwargs):
         assert variant in ("fastsam-s", "fastsam-x"), variant
         self.variant = variant
         self.conf = conf
@@ -146,32 +149,48 @@
             new_w, new_h = desired_max, w * desired_max // h
         def _offset32(x: int) -> int:
             return ((32 - x % 32) if x < 32 or (x % 32 <= 16) else -(x % 32)) % 32 # get closest modulo 32 offset of x
         new_h, new_w = new_h + _offset32(new_h), new_w + _offset32(new_w) # needed because it throws otherwise
         tr_x = F.interpolate(tr_x, size=(new_h, new_w), mode="bilinear", align_corners=False)
         return tr_x
 
-def main():
+def get_args() -> Namespace:
+    """cli args"""
+    parser = ArgumentParser()
+    parser = ArgumentParser()
+    parser.add_argument("model_id", choices=["fastsam-x", "fastsam-s"])
+    parser.add_argument("input_image", type=Path)
+    parser.add_argument("output_path", type=Path)
+    return parser.parse_args()
+
+def main(args: Namespace):
     """main fn. Usage: python fastsam.py fastsam-x/fastsam-s demo1.jpg output1.jpg"""
-    import sys
-    from datetime import datetime # pylint: disable=all
-    from media_processing_lib.image import image_read, image_write # pylint: disable=all
-    assert len(sys.argv) == 4
-    img = image_read(sys.argv[2])
+    img = image_read(args.input_image)
 
-    fastsam = FastSam(sys.argv[1], iou=0.9, conf=0.4, name="fastsam", dependencies=[])
+    fastsam = FastSam(args.model_id, iou=0.9, conf=0.4, name="fastsam", dependencies=[])
     fastsam.predictor.model.to("cuda" if tr.cuda.is_available() else "cpu")
-    for _ in range(1):
-        now = datetime.now()
-        pred = fastsam.make(img[None])
-        print(f"Pred took: {datetime.now() - now}")
-        semantic_result = fastsam.make_images(img[None], pred)[0]
-        image_write(semantic_result, sys.argv[3])
-    print(f"Written result to '{sys.argv[3]}'")
+    now = datetime.now()
+    pred = fastsam.make(img[None])
+    logger.info(f"Pred took: {datetime.now() - now}")
+    semantic_result = fastsam.make_images(img[None], pred)[0]
+    image_write(semantic_result, args.output_path)
+    logger.info(f"Written result to '{args.output_path}'")
 
+    output_path_rsz = args.output_path.parent / f"{args.output_path.stem}_rsz.{args.output_path.suffix}"
     pred_rsz = fastsam.resize(pred, img.shape[0:2])
     semantic_result_rsz = fastsam.make_images(img[None], pred_rsz)[0]
-    image_write(semantic_result_rsz, name := f"{sys.argv[3][0:-4]}_rsz.{sys.argv[3][-3:]}")
-    print(f"Written resized result to '{name}'")
+    image_write(semantic_result_rsz, output_path_rsz)
+    logger.info(f"Written resized result to '{output_path_rsz}'")
+
+    if args.input_image.name == "demo1.jpg" and args.model_id == "fastsam-s":
+        assert np.allclose(a := pred[0].mean(), 0.8813972), a
+        assert np.allclose(b := pred[1][0]["boxes"].mean(), 46.200043), b
+        assert np.allclose(a := pred_rsz[0].mean(), 0.88434076), a
+        assert np.allclose(b := pred_rsz[1][0]["boxes"].mean(), 28.541258), b
+    elif args.input_image.name == "demo1.jpg" and args.model_id == "fastsam-x":
+        assert np.allclose(a := pred[0].mean(), 0.80122584), a
+        assert np.allclose(b := pred[1][0]["boxes"].mean(), 49.640644), b
+        assert np.allclose(a := pred_rsz[0].mean(), 0.80056435), a
+        assert np.allclose(b := pred_rsz[1][0]["boxes"].mean(), 30.688671), b
 
 if __name__ == "__main__":
-    main()
+    main(get_args())
```

### Comparing `video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/fastsam_impl/decoder.py` & `video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/fastsam_impl/decoder.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/fastsam_impl/model.py` & `video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/fastsam_impl/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     model = FastSAM('last.pt')
     results = model.predict('ultralytics/assets/bus.jpg')
 """
 
 from torch import nn
 import torch
 from pathlib import Path
+import sys
+sys.path.append(Path(__file__).parents[1].__str__()) # needed to load the weights because ultralytics must be in path...
 
 from .predict import FastSAMPredictor
 from .utils import DEFAULT_CFG_DICT, DEFAULT_CFG_KEYS
 
 def autopad(k, p=None, d=1):  # kernel, padding, dilation
     """Pad to 'same' shape outputs."""
     if d > 1:
```

### Comparing `video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/fastsam_impl/ops.py` & `video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/fastsam_impl/ops.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/fastsam_impl/predict.py` & `video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/fastsam_impl/predict.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/fastsam_impl/prompt.py` & `video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/fastsam_impl/prompt.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/fastsam_impl/results.py` & `video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/fastsam_impl/results.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/fastsam_impl/utils.py` & `video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/fastsam_impl/utils.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/ultralytics/nn/modules/__init__.py` & `video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/ultralytics/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/ultralytics/nn/modules/block.py` & `video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/ultralytics/nn/modules/block.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/ultralytics/nn/modules/conv.py` & `video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/ultralytics/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/ultralytics/nn/modules/head.py` & `video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/ultralytics/nn/modules/head.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/ultralytics/nn/modules/transformer.py` & `video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/ultralytics/nn/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/ultralytics/nn/modules/utils.py` & `video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/ultralytics/nn/modules/utils.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/ultralytics/nn/tasks.py` & `video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/ultralytics/nn/tasks.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/soft_segmentation/fastsam/ultralytics/yolo/utils/__init__.py` & `video-representations-extractor-1.0.4/vre/representations/soft_segmentation/fastsam/ultralytics/yolo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/soft_segmentation/generalized_boundaries/generalized_boundaries.py` & `video-representations-extractor-1.0.4/vre/representations/soft_segmentation/generalized_boundaries/generalized_boundaries.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/representations/soft_segmentation/halftone/halftone.py` & `video-representations-extractor-1.0.4/vre/representations/soft_segmentation/halftone/halftone.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 
             half_tone = half_tone.crop((xx1, yy1, xx2, yy2))
 
             if self.antialias is True:
                 # Scale it back down to antialias the image.
                 w = int((xx2 - xx1) / antialias_scale)
                 h = int((yy2 - yy1) / antialias_scale)
-                half_tone = half_tone.resize((w, h), resample=Image.LANCZOS)
+                half_tone = image_resize(half_tone, h, w)
 
             dots.append(half_tone)
         return dots
 
     def _make_one_image(self, frame: np.ndarray) -> np.ndarray:
         frame = image_resize(frame, height=self.resolution[0], width=self.resolution[1])
         im = Image.fromarray(frame, "RGB")
```

### Comparing `video-representations-extractor-1.0.3/vre/representations/soft_segmentation/kmeans.py` & `video-representations-extractor-1.0.4/vre/representations/soft_segmentation/kmeans.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/utils/fake_video.py` & `video-representations-extractor-1.0.4/vre/utils/fake_video.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """FakeVideo module"""
+from typing import Union
 import numpy as np
 import pims
 
 class FakeVideo:
     """FakeVideo -- class used to test representations with a given numpy array"""
     def __init__(self, data: np.ndarray, frame_rate: int):
         assert len(data) > 0, "No data provided"
@@ -18,8 +19,8 @@
 
     def __getitem__(self, ix):
         return self.data[ix]
 
     def __len__(self):
         return len(self.data)
 
-VREVideo = pims.Video | FakeVideo
+VREVideo = Union[pims.Video, FakeVideo]
```

### Comparing `video-representations-extractor-1.0.3/vre/utils/topological_sort.py` & `video-representations-extractor-1.0.4/vre/utils/topological_sort.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/utils/utils.py` & `video-representations-extractor-1.0.4/vre/utils/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 """utils for vre"""
 from typing import Any
 from pathlib import Path
 from datetime import datetime
 import os
 import gdown
 import numpy as np
-from skimage.transform import resize
-from skimage.io import imsave, imread
-from skimage.color import hsv2rgb
 
 from ..logger import logger
 from .fake_video import VREVideo
 
 RepresentationOutput = np.ndarray | tuple[np.ndarray, list[dict]]
 
 def get_project_root() -> Path:
@@ -22,39 +19,14 @@
     """gets the weights dir of this project"""
     return Path(os.getenv("VRE_WEIGHTS_DIR", get_project_root() / "weights"))
 
 def parsed_str_type(item: Any) -> str:
     """Given an object with a type of the format: <class 'A.B.C.D'>, parse it and return 'A.B.C.D'"""
     return str(type(item)).rsplit(".", maxsplit=1)[-1][0:-2]
 
-def image_resize(data: np.ndarray, height: int, width: int, interpolation: str = "bilinear", **kwargs) -> np.ndarray:
-    """Skimage image resizer"""
-    assert interpolation in ("nearest", "bilinear", "bicubic", "biquadratic", "biquartic", "biquintic")
-    assert isinstance(height, int) and isinstance(width, int) and height > 0 and width > 0, (height, width)
-    # As per: https://github.com/scikit-image/scikit-image/blob/main/skimage/transform/_warps.py#L820
-    order = {"nearest": 0, "bilinear": 1, "biquadratic": 2, "bicubic": 3, "biquartic": 4, "biquintic": 5}[interpolation]
-    img_resized = resize(data, output_shape=(height, width), order=order, preserve_range=True, **kwargs)
-    img_resized = img_resized.astype(data.dtype)
-    return img_resized
-
-def image_resize_batch(x_batch: np.ndarray, height: int, width: int, **kwargs) -> np.ndarray:
-    """resizes a bath of images to the given height and width"""
-    return np.array([image_resize(x, height, width, **kwargs) for x in x_batch])
-
-def image_write(x: np.ndarray, path: Path):
-    """writes an image to a bytes string"""
-    assert x.dtype == np.uint8, x.dtype
-    imsave(path, x, check_contrast=False)
-    logger.debug2(f"Saved image to '{path}'")
-
-def image_read(path: str) -> np.ndarray:
-    """PIL image reader"""
-    image = np.array(imread(path), dtype=np.uint8)[..., 0:3]
-    return image
-
 def gdown_mkdir(uri: str, local_path: Path):
     """calls gdown but also makes the directory of the parent path just to be sure it exists"""
     logger.debug(f"Downloading '{uri}' to '{local_path}'")
     local_path.parent.mkdir(exist_ok=True, parents=True)
     gdown.download(uri, f"{local_path}")
 
 def to_categorical(data: np.ndarray, num_classes: int = None) -> np.ndarray:
@@ -68,27 +40,14 @@
     MB = data.shape[0]
     y = np.squeeze(y)
     if MB == 1:
         y = np.expand_dims(y, axis=0)
     y = y.reshape(*data.shape, num_classes)
     return y
 
-def generate_diverse_colors(n: int, saturation: float, value: float) -> list[tuple[int, int, int]]:
-    """generates a list of n diverse colors using the hue from the HSV transform"""
-    assert 0 <= saturation <= 1, saturation
-    assert 0 <= value <= 1, value
-    colors = []
-    for i in range(n):
-        hue = i / n  # Vary the hue component
-        rgb = hsv2rgb([hue, saturation, value])
-        # Convert to 8-bit RGB values (0-255)
-        rgb = tuple(int(255 * x) for x in rgb)
-        colors.append(rgb)
-    return colors
-
 def took(prev: datetime.date, l: int, r: int) -> list[float]:
     """how much it took between [prev:now()] gien a [l:r] batch"""
     return [(datetime.now() - prev).total_seconds() / (r - l)] * (r - l)
 
 def make_batches(video: VREVideo, start_frame: int, end_frame: int, batch_size: int) -> np.ndarray:
     """return 1D array [start_frame, start_frame+bs, start_frame+2*bs... end_frame]"""
     if batch_size > end_frame - start_frame:
@@ -109,7 +68,26 @@
             return False
     logger.debug(f"Batch [{l}:{r}] skipped.")
     return True
 
 def is_dir_empty(dir_path: Path, pattern: str = "*") -> bool:
     """returns true if directory is not empty, false if it is empty"""
     return len(list(dir_path.glob(pattern))) == 0
+
+def get_closest_square(n: int) -> tuple[int, int]:
+    """
+    Given a stack of N images
+    Find the closest square X>=N*N and then remove rows 1 by 1 until it still fits X
+
+    Example: 9: 3*3; 12 -> 3*3 -> 3*4 (3 rows). 65 -> 8*8 -> 8*9. 73 -> 8*8 -> 8*9 -> 9*9
+    """
+
+    x = int(np.sqrt(n))
+    r, c = x, x
+    # There are only 2 rows possible between x^2 and (x+1)^2 because (x+1)^2 = x^2 + 2*x + 1, thus we can add 2 columns
+    #  at most. If a 3rd column is needed, then closest lower bound is (x+1)^2 and we must use that.
+    if c * r < n:
+        c += 1
+    if c * r < n:
+        r += 1
+    assert (c + 1) * r > n and c * (r + 1) > n
+    return r, c
```

### Comparing `video-representations-extractor-1.0.3/vre/video_representations_extractor.py` & `video-representations-extractor-1.0.4/vre/video_representations_extractor.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/vre_representation_mixin.py` & `video-representations-extractor-1.0.4/vre/vre_representation_mixin.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.3/vre/vre_runtime_args.py` & `video-representations-extractor-1.0.4/vre/vre_runtime_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         for name in self.vre.representations.keys():
             png_base_dir = self.output_dir / name / "png/"
             png_paths[name] = [png_base_dir / f"{t}.png" for t in range(len(self.vre.video))]
         return png_paths
 
     def _print_call(self):
         logger.info(f"""
-  - Video path: '{self.vre.video.file}'
+  - Video path: '{getattr(self.vre.video, "file", "")}'
   - Output dir: '{self.output_dir}' (exist mode: '{self.output_dir_exist_mode}')
   - Representations ({len(self.vre.representations)}): {", ".join(x for x in self.vre.representations.keys())}
   - Video shape: {self.vre.video.shape} (FPS: {self.vre.video.frame_rate:.2f})
   - Output frames ({self.end_frame - self.start_frame}): [{self.start_frame} : {self.end_frame - 1}]
   - Output shape: {self.output_size if self.output_size != "video_shape" else self.vre.video.frame_shape[0:2]}
   - Batch size: {self.batch_size}
   - Export npy: {self.export_npy}
```

