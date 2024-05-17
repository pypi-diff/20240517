# Comparing `tmp/biomedisa-2024.5.22.tar.gz` & `tmp/biomedisa-24.5.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biomedisa-2024.5.22.tar", last modified: Thu May 16 07:34:46 2024, max compression
+gzip compressed data, was "biomedisa-24.5.23.tar", last modified: Fri May 17 09:13:41 2024, max compression
```

## Comparing `biomedisa-2024.5.22.tar` & `biomedisa-24.5.23.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-16 07:34:46.951612 biomedisa-2024.5.22/
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    14152 2023-06-09 06:17:35.000000 biomedisa-2024.5.22/LICENSE
--rw-r--r--   0 philipp   (1000) philipp   (1000)    10786 2024-05-16 07:34:46.951612 biomedisa-2024.5.22/PKG-INFO
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    10178 2024-05-16 07:34:22.000000 biomedisa-2024.5.22/README.md
--rw-rw-r--   0 philipp   (1000) philipp   (1000)      664 2024-05-16 07:34:18.000000 biomedisa-2024.5.22/pyproject.toml
--rw-rw-r--   0 philipp   (1000) philipp   (1000)       38 2024-05-16 07:34:46.951612 biomedisa-2024.5.22/setup.cfg
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-16 07:34:46.951612 biomedisa-2024.5.22/src/
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-16 07:34:46.951612 biomedisa-2024.5.22/src/biomedisa/
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     1526 2024-05-16 02:12:35.000000 biomedisa-2024.5.22/src/biomedisa/__init__.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)      536 2024-05-08 09:06:16.000000 biomedisa-2024.5.22/src/biomedisa/__main__.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    27828 2024-05-16 07:30:05.000000 biomedisa-2024.5.22/src/biomedisa/deeplearning.py
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-16 07:34:46.951612 biomedisa-2024.5.22/src/biomedisa/features/
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    12770 2024-05-16 00:17:46.000000 biomedisa-2024.5.22/src/biomedisa/features/DataGenerator.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     5454 2024-05-16 00:17:55.000000 biomedisa-2024.5.22/src/biomedisa/features/DataGeneratorCrop.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     4074 2024-05-16 00:30:03.000000 biomedisa-2024.5.22/src/biomedisa/features/PredictDataGenerator.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     3431 2024-05-16 00:30:13.000000 biomedisa-2024.5.22/src/biomedisa/features/PredictDataGeneratorCrop.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2023-06-09 06:17:35.000000 biomedisa-2024.5.22/src/biomedisa/features/__init__.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    18096 2024-05-16 00:12:55.000000 biomedisa-2024.5.22/src/biomedisa/features/active_contour.py
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-16 07:34:46.951612 biomedisa-2024.5.22/src/biomedisa/features/amira_to_np/
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2023-06-09 06:17:35.000000 biomedisa-2024.5.22/src/biomedisa/features/amira_to_np/__init__.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    32618 2023-06-09 06:17:35.000000 biomedisa-2024.5.22/src/biomedisa/features/amira_to_np/amira_data_stream.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    14324 2023-06-09 06:17:35.000000 biomedisa-2024.5.22/src/biomedisa/features/amira_to_np/amira_grammar.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    11553 2023-06-09 06:17:35.000000 biomedisa-2024.5.22/src/biomedisa/features/amira_to_np/amira_header.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     2218 2023-06-09 06:17:35.000000 biomedisa-2024.5.22/src/biomedisa/features/amira_to_np/amira_helper.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     6537 2024-05-16 00:13:13.000000 biomedisa-2024.5.22/src/biomedisa/features/assd.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    32250 2024-05-16 00:14:20.000000 biomedisa-2024.5.22/src/biomedisa/features/biomedisa_helper.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    13001 2024-05-16 00:16:37.000000 biomedisa-2024.5.22/src/biomedisa/features/create_slices.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    24533 2024-05-16 00:17:17.000000 biomedisa-2024.5.22/src/biomedisa/features/crop_helper.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     7049 2024-05-16 00:17:36.000000 biomedisa-2024.5.22/src/biomedisa/features/curvop_numba.py
--rw-rw-r--   0 philipp   (1000) philipp   (1000)     8942 2024-05-16 00:19:36.000000 biomedisa-2024.5.22/src/biomedisa/features/django_env.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    50250 2024-05-16 00:20:22.000000 biomedisa-2024.5.22/src/biomedisa/features/keras_helper.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     7406 2024-05-16 00:20:46.000000 biomedisa-2024.5.22/src/biomedisa/features/nc_reader.py
--rw-rw-r--   0 philipp   (1000) philipp   (1000)     2545 2024-05-16 00:29:46.000000 biomedisa-2024.5.22/src/biomedisa/features/pid.py
--rw-rw-r--   0 philipp   (1000) philipp   (1000)    11091 2024-05-16 00:31:34.000000 biomedisa-2024.5.22/src/biomedisa/features/process_image.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     3275 2024-05-16 00:31:56.000000 biomedisa-2024.5.22/src/biomedisa/features/pycuda_test.py
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-16 07:34:46.951612 biomedisa-2024.5.22/src/biomedisa/features/random_walk/
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2023-06-09 06:17:35.000000 biomedisa-2024.5.22/src/biomedisa/features/random_walk/__init__.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     7191 2024-05-16 00:09:35.000000 biomedisa-2024.5.22/src/biomedisa/features/random_walk/gpu_kernels.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    32917 2024-05-16 00:10:02.000000 biomedisa-2024.5.22/src/biomedisa/features/random_walk/pycuda_large.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    30677 2024-05-16 00:10:19.000000 biomedisa-2024.5.22/src/biomedisa/features/random_walk/pycuda_large_allx.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    15786 2024-05-16 00:09:10.000000 biomedisa-2024.5.22/src/biomedisa/features/random_walk/pycuda_small.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    18225 2024-05-16 00:10:42.000000 biomedisa-2024.5.22/src/biomedisa/features/random_walk/pycuda_small_allx.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    31015 2024-05-16 00:10:54.000000 biomedisa-2024.5.22/src/biomedisa/features/random_walk/pyopencl_large.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    17068 2024-05-16 00:11:11.000000 biomedisa-2024.5.22/src/biomedisa/features/random_walk/pyopencl_small.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    19805 2024-05-16 00:08:50.000000 biomedisa-2024.5.22/src/biomedisa/features/random_walk/rw_large.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    14881 2024-05-16 00:08:13.000000 biomedisa-2024.5.22/src/biomedisa/features/random_walk/rw_small.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    16756 2024-05-16 00:33:15.000000 biomedisa-2024.5.22/src/biomedisa/features/remove_outlier.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     8917 2024-05-16 04:15:45.000000 biomedisa-2024.5.22/src/biomedisa/features/split_volume.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    17253 2024-05-16 00:15:01.000000 biomedisa-2024.5.22/src/biomedisa/interpolation.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    15819 2024-05-16 00:37:59.000000 biomedisa-2024.5.22/src/biomedisa/mesh.py
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-16 07:34:46.951612 biomedisa-2024.5.22/src/biomedisa.egg-info/
--rw-r--r--   0 philipp   (1000) philipp   (1000)    10786 2024-05-16 07:34:46.000000 biomedisa-2024.5.22/src/biomedisa.egg-info/PKG-INFO
--rw-rw-r--   0 philipp   (1000) philipp   (1000)     1832 2024-05-16 07:34:46.000000 biomedisa-2024.5.22/src/biomedisa.egg-info/SOURCES.txt
--rw-rw-r--   0 philipp   (1000) philipp   (1000)        1 2024-05-16 07:34:46.000000 biomedisa-2024.5.22/src/biomedisa.egg-info/dependency_links.txt
--rw-rw-r--   0 philipp   (1000) philipp   (1000)       10 2024-05-16 07:34:46.000000 biomedisa-2024.5.22/src/biomedisa.egg-info/top_level.txt
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-17 09:13:41.800840 biomedisa-24.5.23/
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    14152 2023-06-09 06:17:35.000000 biomedisa-24.5.23/LICENSE
+-rw-r--r--   0 philipp   (1000) philipp   (1000)    10475 2024-05-17 09:13:41.800840 biomedisa-24.5.23/PKG-INFO
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     9869 2024-05-17 09:05:24.000000 biomedisa-24.5.23/README.md
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)      662 2024-05-17 09:10:35.000000 biomedisa-24.5.23/pyproject.toml
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)       38 2024-05-17 09:13:41.800840 biomedisa-24.5.23/setup.cfg
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-17 09:13:41.800840 biomedisa-24.5.23/src/
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-17 09:13:41.800840 biomedisa-24.5.23/src/biomedisa/
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     1526 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/__init__.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)      536 2024-05-08 09:06:16.000000 biomedisa-24.5.23/src/biomedisa/__main__.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    27828 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/deeplearning.py
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-17 09:13:41.800840 biomedisa-24.5.23/src/biomedisa/features/
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    12770 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/DataGenerator.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     5454 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/DataGeneratorCrop.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     4074 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/PredictDataGenerator.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     3431 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/PredictDataGeneratorCrop.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/__init__.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    18096 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/active_contour.py
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-17 09:13:41.800840 biomedisa-24.5.23/src/biomedisa/features/amira_to_np/
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/amira_to_np/__init__.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    32618 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/amira_to_np/amira_data_stream.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    14324 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/amira_to_np/amira_grammar.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    11553 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/amira_to_np/amira_header.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     2218 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/amira_to_np/amira_helper.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     6537 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/assd.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    32250 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/biomedisa_helper.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    13001 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/create_slices.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    24533 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/crop_helper.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     7049 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/curvop_numba.py
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)     8942 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/django_env.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    50488 2024-05-17 08:57:50.000000 biomedisa-24.5.23/src/biomedisa/features/keras_helper.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     7406 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/nc_reader.py
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)     2545 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/pid.py
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)    11091 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/process_image.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     3275 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/pycuda_test.py
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-17 09:13:41.800840 biomedisa-24.5.23/src/biomedisa/features/random_walk/
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/random_walk/__init__.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     7191 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/random_walk/gpu_kernels.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    32917 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/random_walk/pycuda_large.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    30677 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/random_walk/pycuda_large_allx.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    15786 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/random_walk/pycuda_small.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    18225 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/random_walk/pycuda_small_allx.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    31015 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/random_walk/pyopencl_large.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    17068 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/random_walk/pyopencl_small.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    19805 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/random_walk/rw_large.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    14881 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/random_walk/rw_small.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    16756 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/remove_outlier.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     8917 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/features/split_volume.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    17253 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/interpolation.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    15819 2024-05-16 08:39:54.000000 biomedisa-24.5.23/src/biomedisa/mesh.py
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-17 09:13:41.800840 biomedisa-24.5.23/src/biomedisa.egg-info/
+-rw-r--r--   0 philipp   (1000) philipp   (1000)    10475 2024-05-17 09:13:41.000000 biomedisa-24.5.23/src/biomedisa.egg-info/PKG-INFO
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)     1832 2024-05-17 09:13:41.000000 biomedisa-24.5.23/src/biomedisa.egg-info/SOURCES.txt
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)        1 2024-05-17 09:13:41.000000 biomedisa-24.5.23/src/biomedisa.egg-info/dependency_links.txt
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)       10 2024-05-17 09:13:41.000000 biomedisa-24.5.23/src/biomedisa.egg-info/top_level.txt
```

### Comparing `biomedisa-2024.5.22/LICENSE` & `biomedisa-24.5.23/LICENSE`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/PKG-INFO` & `biomedisa-24.5.23/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,70 +1,56 @@
-Metadata-Version: 2.1
-Name: biomedisa
-Version: 2024.5.22
-Summary: Segmentation of 3D volumetric image data
-Author: Philipp Lösel
-Author-email: philipp.loesel@anu.edu.au
-Project-URL: Homepage, https://biomedisa.info
-Project-URL: Issues, https://github.com/biomedisa/biomedisa/issues
-Project-URL: GitHub, https://github.com/biomedisa/biomedisa
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![biomedisa](https://raw.githubusercontent.com/biomedisa/biomedisa/master/biomedisa_app/static/biomedisa_logo.svg)](https://biomedisa.info)
 -----------
 - [Overview](#overview)
 - [Hardware Requirements](#hardware-requirements)
 - [Installation (command-line based)](#installation-command-line-based)
 - [Installation (browser based)](#installation-browser-based)
 - [Download Data](#download-data)
 - [Revisions](#revisions)
+- [Quickstart](#quickstart)
 - [Smart Interpolation](#smart-interpolation)
 - [Deep Learning](#deep-learning)
+- [Mesh Generator](#mesh-generator)
 - [Biomedisa Features](#biomedisa-features)
 - [Authors](#authors)
 - [FAQ](#faq)
 - [Citation](#citation)
 - [License](#license)
 
 ## Overview
 Biomedisa (https://biomedisa.info) is a free and easy-to-use open-source application for segmenting large volumetric images, e.g. CT and MRI scans, developed at [The Australian National University CTLab](https://ctlab.anu.edu.au/). Biomedisa's semi-automated segmentation is based on a smart interpolation of sparsely pre-segmented slices, taking into account the complete underlying image data. In addition, Biomedisa enables deep learning for the fully automated segmentation of series of similar samples. It can be used in combination with segmentation tools such as Amira/Avizo, ImageJ/Fiji and 3D Slicer. If you are using Biomedisa or the data for your research please cite: Lösel, P.D. et al. [Introducing Biomedisa as an open-source online platform for biomedical image segmentation.](https://www.nature.com/articles/s41467-020-19303-w) *Nat. Commun.* **11**, 5577 (2020).
 
 ## Hardware Requirements
-+ One or more NVIDIA GPUs with compute capability 3.0 or higher or an Intel CPU.
++ One or more NVIDIA GPUs with compute capability 3.0 or higher or an Intel CPU
 
 ## Installation (command-line based)
 + [Ubuntu 22.04 + CUDA + GPU (recommended)](https://github.com/biomedisa/biomedisa/blob/master/README/ubuntu2204_cuda11.8_gpu_cli.md)
 + [Ubuntu 22.04 + OpenCL + CPU (smart interpolation only and very slow)](https://github.com/biomedisa/biomedisa/blob/master/README/ubuntu2204_opencl_cpu_cli.md)
 + [Windows 10 + CUDA + GPU (recommended)](https://github.com/biomedisa/biomedisa/blob/master/README/windows10_cuda_gpu_cli.md)
 + [Windows 10 + OpenCL + GPU (easy to install but lacks features like allaxis, smoothing, uncertainty, optimized GPU memory usage)](https://github.com/biomedisa/biomedisa/blob/master/README/windows10_opencl_gpu_cli.md)
 + [Windows 10 + OpenCL + CPU (very slow)](https://github.com/biomedisa/biomedisa/blob/master/README/windows10_opencl_cpu_cli.md)
 
 ## Installation (browser based)
 + [Ubuntu 22.04](https://github.com/biomedisa/biomedisa/blob/master/README/ubuntu2204_cuda11.8.md)
 
 ## Download Data
-+ Download the data from our [gallery](https://biomedisa.info/gallery/)
++ Download test data from our [gallery](https://biomedisa.info/gallery/)
 
 ## Revisions
-2024.05.22
+24.5.22
 + Pip is the preferred installation method
 + Commands, module names and imports have been changed to conform to the Pip standard
-+ For versions <=2023.09.1 please check [README](https://github.com/biomedisa/biomedisa/blob/master/README/deprecated/README_2023.09.1.md)
++ For versions <=23.9.1 please check [README](https://github.com/biomedisa/biomedisa/blob/master/README/deprecated/README_2023.09.1.md)
 
 ## Quickstart
 Install the Biomedisa package from the [Python Package Index](https://pypi.org/project/biomedisa/):
 ```
 python -m pip install -U biomedisa
 ```
-For smart interpolation and deep Learning modules, follow the [installation instructions](https://github.com/biomedisa/biomedisa#installation-command-line-based).
+For smart interpolation and deep Learning modules, follow the installation instructions above.
 
 ## Smart Interpolation
 + [Parameters and Examples](https://github.com/biomedisa/biomedisa/blob/master/README/smart_interpolation.md)
 
 #### Python example
 ```python
 from biomedisa.features.biomedisa_helper import load_data, save_data
@@ -85,16 +71,17 @@
 save_data('Downloads/final.trigonopterus.am', regular_result, header=header)
 save_data('Downloads/final.trigonopterus.smooth.am', smooth_result, header=header)
 ```
 
 #### Command-line based
 ```
 python -m biomedisa.interpolation C:\Users\%USERNAME%\Downloads\tumor.tif C:\Users\%USERNAME%\Downloads\labels.tumor.tif
-
-# if pre-segmentation is not exclusively in the XY plane
+```
+If pre-segmentation is not exclusively in the XY plane:
+```
 python -m biomedisa.interpolation C:\Users\%USERNAME%\Downloads\tumor.tif C:\Users\%USERNAME%\Downloads\labels.tumor.tif --allaxis
 ```
 
 ## Deep Learning
 + [Parameters and Examples](https://github.com/biomedisa/biomedisa/blob/master/README/deep_learning.md)
 
 #### Python example (training)
@@ -124,22 +111,23 @@
 # deep learning 
 deep_learning(img_data, label_data, train=True, batch_size=12,
         val_img_data=val_img_data, val_label_data=val_label_data,
         header=header, extension=ext, path_to_model='honeybees.h5')
 ```
 
 #### Command-line based (training)
+Start training with a batch size of 12:
 ```
-# start training with a batch size of 12
 python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -bs=12
-
-# validation (optional)
+```
+Monitor training progress using validation data:
+```
 python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -vi=C:\Users\%USERNAME%\Downloads\val_img -vl=C:\Users\%USERNAME%\Downloads\val_labels
 ```
-If running into ResourceExhaustedError due to out of memory (OOM), try to use smaller batch size.
+If running into ResourceExhaustedError due to out of memory (OOM), try to use a smaller batch size.
 
 #### Python example (prediction)
 ```python
 from biomedisa.features.biomedisa_helper import load_data, save_data
 from biomedisa.deeplearning import deep_learning
 
 # load data
@@ -154,61 +142,52 @@
 ```
 
 #### Command-line based (prediction)
 ```
 python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\testing_axial_crop_pat13.nii.gz C:\Users\%USERNAME%\Downloads\heart.h5 -p
 ```
 
-## Biomedisa Features
-
-#### Load and save data (such as Amira Mesh, TIFF, NRRD, NIfTI or DICOM)
-```python
-from biomedisa.features.biomedisa_helper import load_data, save_data
-
-# load data as numpy array
-# for DICOM, PNG files, or similar formats, 'path_to_data' must reference
-# either a directory or a ZIP file containing the image slices
-data, header = load_data(path_to_data)
+## Mesh Generator
++ [Parameters and Examples](https://github.com/biomedisa/biomedisa/blob/master/README/save_mesh.md)
 
-# save data (for TIFF, header=None)
-save_data(path_to_data, data, header)
-```
-
-#### Create STL mesh from segmentation (label values are saved as attributes)
+#### Python example
+Create STL mesh from segmentation (label values are saved as attributes)
 ```python
 from biomedisa.features.biomedisa_helper import load_data, save_data
 from biomedisa.mesh import get_voxel_spacing, save_mesh
 
 # load segmentation
-data, header, extension = load_data(path_to_data, return_extension=True)
+data, header, extension = load_data('final.Head5.am', return_extension=True)
 
 # get voxel spacing
 x_res, y_res, z_res = get_voxel_spacing(header, data, extension)
 print(f'Voxel spacing: x_spacing, y_spacing, z_spacing = {x_res}, {y_res}, {z_res}')
 
 # save stl file
-path_to_data = path_to_data.replace(os.path.splitext(path_to_data)[1],'.stl')
-save_mesh(path_to_data, data, x_res, y_res, z_res, poly_reduction=0.9, smoothing_iterations=15)
+save_mesh('final.Head5.stl', data, x_res, y_res, z_res, poly_reduction=0.9, smoothing_iterations=15)
 ```
 
-#### Create mesh directly
+#### Command-line based
 ```
-python -m biomedisa.mesh <path_to_data>
+python -m biomedisa.mesh 'final.Head5.am'
 ```
 
-#### Options
-`--poly_reduction` or `-pr`: Reduce number of polygons by this factor (default: 0.9)
-
-`--smoothing_iterations` or `-s`: Iteration steps for smoothing (default: 15)
+## Biomedisa Features
 
-`--x_res` or `-xres`: Voxel spacing/resolution x-axis (default: None)
+#### Load and save data (such as Amira Mesh, TIFF, NRRD, NIfTI or DICOM)
+For DICOM, PNG files, or similar formats, file path must reference either a directory or a ZIP file containing the image slices.
+```python
+from biomedisa.features.biomedisa_helper import load_data, save_data
 
-`--y_res` or `-yres`: Voxel spacing/resolution y-axis (default: None)
+# load data as numpy array
+data, header = load_data('temp.tif')
 
-`--z_res` or `-zres`: Voxel spacing/resolution z-axis (default: None)
+# save data (for TIFF, header=None)
+save_data('temp.tif', data, header)
+```
 
 #### Resize data
 ```python
 from biomedisa.features.biomedisa_helper import img_resize
 
 # resize image data
 zsh, ysh, xsh = data.shape
```

### Comparing `biomedisa-2024.5.22/README.md` & `biomedisa-24.5.23/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,72 @@
+Metadata-Version: 2.1
+Name: biomedisa
+Version: 24.5.23
+Summary: Segmentation of 3D volumetric image data
+Author: Philipp Lösel
+Author-email: philipp.loesel@anu.edu.au
+Project-URL: Homepage, https://biomedisa.info
+Project-URL: Issues, https://github.com/biomedisa/biomedisa/issues
+Project-URL: GitHub, https://github.com/biomedisa/biomedisa
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![biomedisa](https://raw.githubusercontent.com/biomedisa/biomedisa/master/biomedisa_app/static/biomedisa_logo.svg)](https://biomedisa.info)
 -----------
 - [Overview](#overview)
 - [Hardware Requirements](#hardware-requirements)
 - [Installation (command-line based)](#installation-command-line-based)
 - [Installation (browser based)](#installation-browser-based)
 - [Download Data](#download-data)
 - [Revisions](#revisions)
+- [Quickstart](#quickstart)
 - [Smart Interpolation](#smart-interpolation)
 - [Deep Learning](#deep-learning)
+- [Mesh Generator](#mesh-generator)
 - [Biomedisa Features](#biomedisa-features)
 - [Authors](#authors)
 - [FAQ](#faq)
 - [Citation](#citation)
 - [License](#license)
 
 ## Overview
 Biomedisa (https://biomedisa.info) is a free and easy-to-use open-source application for segmenting large volumetric images, e.g. CT and MRI scans, developed at [The Australian National University CTLab](https://ctlab.anu.edu.au/). Biomedisa's semi-automated segmentation is based on a smart interpolation of sparsely pre-segmented slices, taking into account the complete underlying image data. In addition, Biomedisa enables deep learning for the fully automated segmentation of series of similar samples. It can be used in combination with segmentation tools such as Amira/Avizo, ImageJ/Fiji and 3D Slicer. If you are using Biomedisa or the data for your research please cite: Lösel, P.D. et al. [Introducing Biomedisa as an open-source online platform for biomedical image segmentation.](https://www.nature.com/articles/s41467-020-19303-w) *Nat. Commun.* **11**, 5577 (2020).
 
 ## Hardware Requirements
-+ One or more NVIDIA GPUs with compute capability 3.0 or higher or an Intel CPU.
++ One or more NVIDIA GPUs with compute capability 3.0 or higher or an Intel CPU
 
 ## Installation (command-line based)
 + [Ubuntu 22.04 + CUDA + GPU (recommended)](https://github.com/biomedisa/biomedisa/blob/master/README/ubuntu2204_cuda11.8_gpu_cli.md)
 + [Ubuntu 22.04 + OpenCL + CPU (smart interpolation only and very slow)](https://github.com/biomedisa/biomedisa/blob/master/README/ubuntu2204_opencl_cpu_cli.md)
 + [Windows 10 + CUDA + GPU (recommended)](https://github.com/biomedisa/biomedisa/blob/master/README/windows10_cuda_gpu_cli.md)
 + [Windows 10 + OpenCL + GPU (easy to install but lacks features like allaxis, smoothing, uncertainty, optimized GPU memory usage)](https://github.com/biomedisa/biomedisa/blob/master/README/windows10_opencl_gpu_cli.md)
 + [Windows 10 + OpenCL + CPU (very slow)](https://github.com/biomedisa/biomedisa/blob/master/README/windows10_opencl_cpu_cli.md)
 
 ## Installation (browser based)
 + [Ubuntu 22.04](https://github.com/biomedisa/biomedisa/blob/master/README/ubuntu2204_cuda11.8.md)
 
 ## Download Data
-+ Download the data from our [gallery](https://biomedisa.info/gallery/)
++ Download test data from our [gallery](https://biomedisa.info/gallery/)
 
 ## Revisions
-2024.05.22
+24.5.22
 + Pip is the preferred installation method
 + Commands, module names and imports have been changed to conform to the Pip standard
-+ For versions <=2023.09.1 please check [README](https://github.com/biomedisa/biomedisa/blob/master/README/deprecated/README_2023.09.1.md)
++ For versions <=23.9.1 please check [README](https://github.com/biomedisa/biomedisa/blob/master/README/deprecated/README_2023.09.1.md)
 
 ## Quickstart
 Install the Biomedisa package from the [Python Package Index](https://pypi.org/project/biomedisa/):
 ```
 python -m pip install -U biomedisa
 ```
-For smart interpolation and deep Learning modules, follow the [installation instructions](https://github.com/biomedisa/biomedisa#installation-command-line-based).
+For smart interpolation and deep Learning modules, follow the installation instructions above.
 
 ## Smart Interpolation
 + [Parameters and Examples](https://github.com/biomedisa/biomedisa/blob/master/README/smart_interpolation.md)
 
 #### Python example
 ```python
 from biomedisa.features.biomedisa_helper import load_data, save_data
@@ -69,16 +87,17 @@
 save_data('Downloads/final.trigonopterus.am', regular_result, header=header)
 save_data('Downloads/final.trigonopterus.smooth.am', smooth_result, header=header)
 ```
 
 #### Command-line based
 ```
 python -m biomedisa.interpolation C:\Users\%USERNAME%\Downloads\tumor.tif C:\Users\%USERNAME%\Downloads\labels.tumor.tif
-
-# if pre-segmentation is not exclusively in the XY plane
+```
+If pre-segmentation is not exclusively in the XY plane:
+```
 python -m biomedisa.interpolation C:\Users\%USERNAME%\Downloads\tumor.tif C:\Users\%USERNAME%\Downloads\labels.tumor.tif --allaxis
 ```
 
 ## Deep Learning
 + [Parameters and Examples](https://github.com/biomedisa/biomedisa/blob/master/README/deep_learning.md)
 
 #### Python example (training)
@@ -108,22 +127,23 @@
 # deep learning 
 deep_learning(img_data, label_data, train=True, batch_size=12,
         val_img_data=val_img_data, val_label_data=val_label_data,
         header=header, extension=ext, path_to_model='honeybees.h5')
 ```
 
 #### Command-line based (training)
+Start training with a batch size of 12:
 ```
-# start training with a batch size of 12
 python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -bs=12
-
-# validation (optional)
+```
+Monitor training progress using validation data:
+```
 python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -vi=C:\Users\%USERNAME%\Downloads\val_img -vl=C:\Users\%USERNAME%\Downloads\val_labels
 ```
-If running into ResourceExhaustedError due to out of memory (OOM), try to use smaller batch size.
+If running into ResourceExhaustedError due to out of memory (OOM), try to use a smaller batch size.
 
 #### Python example (prediction)
 ```python
 from biomedisa.features.biomedisa_helper import load_data, save_data
 from biomedisa.deeplearning import deep_learning
 
 # load data
@@ -138,61 +158,52 @@
 ```
 
 #### Command-line based (prediction)
 ```
 python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\testing_axial_crop_pat13.nii.gz C:\Users\%USERNAME%\Downloads\heart.h5 -p
 ```
 
-## Biomedisa Features
-
-#### Load and save data (such as Amira Mesh, TIFF, NRRD, NIfTI or DICOM)
-```python
-from biomedisa.features.biomedisa_helper import load_data, save_data
-
-# load data as numpy array
-# for DICOM, PNG files, or similar formats, 'path_to_data' must reference
-# either a directory or a ZIP file containing the image slices
-data, header = load_data(path_to_data)
+## Mesh Generator
++ [Parameters and Examples](https://github.com/biomedisa/biomedisa/blob/master/README/save_mesh.md)
 
-# save data (for TIFF, header=None)
-save_data(path_to_data, data, header)
-```
-
-#### Create STL mesh from segmentation (label values are saved as attributes)
+#### Python example
+Create STL mesh from segmentation (label values are saved as attributes)
 ```python
 from biomedisa.features.biomedisa_helper import load_data, save_data
 from biomedisa.mesh import get_voxel_spacing, save_mesh
 
 # load segmentation
-data, header, extension = load_data(path_to_data, return_extension=True)
+data, header, extension = load_data('final.Head5.am', return_extension=True)
 
 # get voxel spacing
 x_res, y_res, z_res = get_voxel_spacing(header, data, extension)
 print(f'Voxel spacing: x_spacing, y_spacing, z_spacing = {x_res}, {y_res}, {z_res}')
 
 # save stl file
-path_to_data = path_to_data.replace(os.path.splitext(path_to_data)[1],'.stl')
-save_mesh(path_to_data, data, x_res, y_res, z_res, poly_reduction=0.9, smoothing_iterations=15)
+save_mesh('final.Head5.stl', data, x_res, y_res, z_res, poly_reduction=0.9, smoothing_iterations=15)
 ```
 
-#### Create mesh directly
+#### Command-line based
 ```
-python -m biomedisa.mesh <path_to_data>
+python -m biomedisa.mesh 'final.Head5.am'
 ```
 
-#### Options
-`--poly_reduction` or `-pr`: Reduce number of polygons by this factor (default: 0.9)
-
-`--smoothing_iterations` or `-s`: Iteration steps for smoothing (default: 15)
+## Biomedisa Features
 
-`--x_res` or `-xres`: Voxel spacing/resolution x-axis (default: None)
+#### Load and save data (such as Amira Mesh, TIFF, NRRD, NIfTI or DICOM)
+For DICOM, PNG files, or similar formats, file path must reference either a directory or a ZIP file containing the image slices.
+```python
+from biomedisa.features.biomedisa_helper import load_data, save_data
 
-`--y_res` or `-yres`: Voxel spacing/resolution y-axis (default: None)
+# load data as numpy array
+data, header = load_data('temp.tif')
 
-`--z_res` or `-zres`: Voxel spacing/resolution z-axis (default: None)
+# save data (for TIFF, header=None)
+save_data('temp.tif', data, header)
+```
 
 #### Resize data
 ```python
 from biomedisa.features.biomedisa_helper import img_resize
 
 # resize image data
 zsh, ysh, xsh = data.shape
```

### Comparing `biomedisa-2024.5.22/pyproject.toml` & `biomedisa-24.5.23/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "biomedisa"
-version = "2024.5.22"
+version = "24.5.23"
 authors = [
   { name="Philipp Lösel"}, {email="philipp.loesel@anu.edu.au" },
 ]
 description = "Segmentation of 3D volumetric image data"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `biomedisa-2024.5.22/src/biomedisa/__init__.py` & `biomedisa-24.5.23/src/biomedisa/__init__.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/__main__.py` & `biomedisa-24.5.23/src/biomedisa/__main__.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/deeplearning.py` & `biomedisa-24.5.23/src/biomedisa/deeplearning.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/DataGenerator.py` & `biomedisa-24.5.23/src/biomedisa/features/DataGenerator.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/DataGeneratorCrop.py` & `biomedisa-24.5.23/src/biomedisa/features/DataGeneratorCrop.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/PredictDataGenerator.py` & `biomedisa-24.5.23/src/biomedisa/features/PredictDataGenerator.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/PredictDataGeneratorCrop.py` & `biomedisa-24.5.23/src/biomedisa/features/PredictDataGeneratorCrop.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/active_contour.py` & `biomedisa-24.5.23/src/biomedisa/features/active_contour.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/amira_to_np/amira_data_stream.py` & `biomedisa-24.5.23/src/biomedisa/features/amira_to_np/amira_data_stream.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/amira_to_np/amira_grammar.py` & `biomedisa-24.5.23/src/biomedisa/features/amira_to_np/amira_grammar.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/amira_to_np/amira_header.py` & `biomedisa-24.5.23/src/biomedisa/features/amira_to_np/amira_header.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/amira_to_np/amira_helper.py` & `biomedisa-24.5.23/src/biomedisa/features/amira_to_np/amira_helper.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/assd.py` & `biomedisa-24.5.23/src/biomedisa/features/assd.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/biomedisa_helper.py` & `biomedisa-24.5.23/src/biomedisa/features/biomedisa_helper.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/create_slices.py` & `biomedisa-24.5.23/src/biomedisa/features/create_slices.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/crop_helper.py` & `biomedisa-24.5.23/src/biomedisa/features/crop_helper.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/curvop_numba.py` & `biomedisa-24.5.23/src/biomedisa/features/curvop_numba.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/django_env.py` & `biomedisa-24.5.23/src/biomedisa/features/django_env.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/keras_helper.py` & `biomedisa-24.5.23/src/biomedisa/features/keras_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,16 +371,18 @@
             if any(img_list):
                 label, header, extension = load_data(label_names[0], 'first_queue', True)
                 if label is None:
                     InputError.message = f'Invalid label data "{os.path.basename(label_names[0])}"'
                     raise InputError()
             elif type(label_in) is list:
                 label = label_in[0]
+                label_names = [f'label_{i}' for i in range(1, len(label_in) + 1)]
             else:
                 label = label_in
+                label_names = ['label_1']
             label_dim = label.shape
             label = set_labels_to_zero(label, labels_to_compute, labels_to_remove)
             label_values, counts = np.unique(label, return_counts=True)
             print(f'{os.path.basename(label_names[0])}:', 'Labels:', label_values[1:], 'Sizes:', counts[1:])
             if crop_data:
                 argmin_z,argmax_z,argmin_y,argmax_y,argmin_x,argmax_x = predict_blocksize(label, x_puffer, y_puffer, z_puffer)
                 label = np.copy(label[argmin_z:argmax_z,argmin_y:argmax_y,argmin_x:argmax_x], order='C')
@@ -402,16 +404,18 @@
             if any(img_list):
                 img, _ = load_data(img_names[0], 'first_queue')
                 if img is None:
                     InputError.message = f'Invalid image data "{os.path.basename(img_names[0])}"'
                     raise InputError()
             elif type(img_in) is list:
                 img = img_in[0]
+                img_names = [f'img_{i}' for i in range(1, len(img_in) + 1)]
             else:
                 img = img_in
+                img_names = ['img_1']
             if label_dim != img.shape:
                 InputError.message = f'Dimensions of "{os.path.basename(img_names[0])}" and "{os.path.basename(label_names[0])}" do not match'
                 raise InputError()
 
             # ensure images have channels >=1
             if len(img.shape)==3:
                 z_shape, y_shape, x_shape = img.shape
```

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/nc_reader.py` & `biomedisa-24.5.23/src/biomedisa/features/nc_reader.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/pid.py` & `biomedisa-24.5.23/src/biomedisa/features/pid.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/process_image.py` & `biomedisa-24.5.23/src/biomedisa/features/process_image.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/pycuda_test.py` & `biomedisa-24.5.23/src/biomedisa/features/pycuda_test.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/random_walk/gpu_kernels.py` & `biomedisa-24.5.23/src/biomedisa/features/random_walk/gpu_kernels.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/random_walk/pycuda_large.py` & `biomedisa-24.5.23/src/biomedisa/features/random_walk/pycuda_large.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/random_walk/pycuda_large_allx.py` & `biomedisa-24.5.23/src/biomedisa/features/random_walk/pycuda_large_allx.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/random_walk/pycuda_small.py` & `biomedisa-24.5.23/src/biomedisa/features/random_walk/pycuda_small.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/random_walk/pycuda_small_allx.py` & `biomedisa-24.5.23/src/biomedisa/features/random_walk/pycuda_small_allx.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/random_walk/pyopencl_large.py` & `biomedisa-24.5.23/src/biomedisa/features/random_walk/pyopencl_large.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/random_walk/pyopencl_small.py` & `biomedisa-24.5.23/src/biomedisa/features/random_walk/pyopencl_small.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/random_walk/rw_large.py` & `biomedisa-24.5.23/src/biomedisa/features/random_walk/rw_large.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/random_walk/rw_small.py` & `biomedisa-24.5.23/src/biomedisa/features/random_walk/rw_small.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/remove_outlier.py` & `biomedisa-24.5.23/src/biomedisa/features/remove_outlier.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/features/split_volume.py` & `biomedisa-24.5.23/src/biomedisa/features/split_volume.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/interpolation.py` & `biomedisa-24.5.23/src/biomedisa/interpolation.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa/mesh.py` & `biomedisa-24.5.23/src/biomedisa/mesh.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.22/src/biomedisa.egg-info/PKG-INFO` & `biomedisa-24.5.23/src/biomedisa.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biomedisa
-Version: 2024.5.22
+Version: 24.5.23
 Summary: Segmentation of 3D volumetric image data
 Author: Philipp Lösel
 Author-email: philipp.loesel@anu.edu.au
 Project-URL: Homepage, https://biomedisa.info
 Project-URL: Issues, https://github.com/biomedisa/biomedisa/issues
 Project-URL: GitHub, https://github.com/biomedisa/biomedisa
 Classifier: Programming Language :: Python :: 3
@@ -18,53 +18,55 @@
 -----------
 - [Overview](#overview)
 - [Hardware Requirements](#hardware-requirements)
 - [Installation (command-line based)](#installation-command-line-based)
 - [Installation (browser based)](#installation-browser-based)
 - [Download Data](#download-data)
 - [Revisions](#revisions)
+- [Quickstart](#quickstart)
 - [Smart Interpolation](#smart-interpolation)
 - [Deep Learning](#deep-learning)
+- [Mesh Generator](#mesh-generator)
 - [Biomedisa Features](#biomedisa-features)
 - [Authors](#authors)
 - [FAQ](#faq)
 - [Citation](#citation)
 - [License](#license)
 
 ## Overview
 Biomedisa (https://biomedisa.info) is a free and easy-to-use open-source application for segmenting large volumetric images, e.g. CT and MRI scans, developed at [The Australian National University CTLab](https://ctlab.anu.edu.au/). Biomedisa's semi-automated segmentation is based on a smart interpolation of sparsely pre-segmented slices, taking into account the complete underlying image data. In addition, Biomedisa enables deep learning for the fully automated segmentation of series of similar samples. It can be used in combination with segmentation tools such as Amira/Avizo, ImageJ/Fiji and 3D Slicer. If you are using Biomedisa or the data for your research please cite: Lösel, P.D. et al. [Introducing Biomedisa as an open-source online platform for biomedical image segmentation.](https://www.nature.com/articles/s41467-020-19303-w) *Nat. Commun.* **11**, 5577 (2020).
 
 ## Hardware Requirements
-+ One or more NVIDIA GPUs with compute capability 3.0 or higher or an Intel CPU.
++ One or more NVIDIA GPUs with compute capability 3.0 or higher or an Intel CPU
 
 ## Installation (command-line based)
 + [Ubuntu 22.04 + CUDA + GPU (recommended)](https://github.com/biomedisa/biomedisa/blob/master/README/ubuntu2204_cuda11.8_gpu_cli.md)
 + [Ubuntu 22.04 + OpenCL + CPU (smart interpolation only and very slow)](https://github.com/biomedisa/biomedisa/blob/master/README/ubuntu2204_opencl_cpu_cli.md)
 + [Windows 10 + CUDA + GPU (recommended)](https://github.com/biomedisa/biomedisa/blob/master/README/windows10_cuda_gpu_cli.md)
 + [Windows 10 + OpenCL + GPU (easy to install but lacks features like allaxis, smoothing, uncertainty, optimized GPU memory usage)](https://github.com/biomedisa/biomedisa/blob/master/README/windows10_opencl_gpu_cli.md)
 + [Windows 10 + OpenCL + CPU (very slow)](https://github.com/biomedisa/biomedisa/blob/master/README/windows10_opencl_cpu_cli.md)
 
 ## Installation (browser based)
 + [Ubuntu 22.04](https://github.com/biomedisa/biomedisa/blob/master/README/ubuntu2204_cuda11.8.md)
 
 ## Download Data
-+ Download the data from our [gallery](https://biomedisa.info/gallery/)
++ Download test data from our [gallery](https://biomedisa.info/gallery/)
 
 ## Revisions
-2024.05.22
+24.5.22
 + Pip is the preferred installation method
 + Commands, module names and imports have been changed to conform to the Pip standard
-+ For versions <=2023.09.1 please check [README](https://github.com/biomedisa/biomedisa/blob/master/README/deprecated/README_2023.09.1.md)
++ For versions <=23.9.1 please check [README](https://github.com/biomedisa/biomedisa/blob/master/README/deprecated/README_2023.09.1.md)
 
 ## Quickstart
 Install the Biomedisa package from the [Python Package Index](https://pypi.org/project/biomedisa/):
 ```
 python -m pip install -U biomedisa
 ```
-For smart interpolation and deep Learning modules, follow the [installation instructions](https://github.com/biomedisa/biomedisa#installation-command-line-based).
+For smart interpolation and deep Learning modules, follow the installation instructions above.
 
 ## Smart Interpolation
 + [Parameters and Examples](https://github.com/biomedisa/biomedisa/blob/master/README/smart_interpolation.md)
 
 #### Python example
 ```python
 from biomedisa.features.biomedisa_helper import load_data, save_data
@@ -85,16 +87,17 @@
 save_data('Downloads/final.trigonopterus.am', regular_result, header=header)
 save_data('Downloads/final.trigonopterus.smooth.am', smooth_result, header=header)
 ```
 
 #### Command-line based
 ```
 python -m biomedisa.interpolation C:\Users\%USERNAME%\Downloads\tumor.tif C:\Users\%USERNAME%\Downloads\labels.tumor.tif
-
-# if pre-segmentation is not exclusively in the XY plane
+```
+If pre-segmentation is not exclusively in the XY plane:
+```
 python -m biomedisa.interpolation C:\Users\%USERNAME%\Downloads\tumor.tif C:\Users\%USERNAME%\Downloads\labels.tumor.tif --allaxis
 ```
 
 ## Deep Learning
 + [Parameters and Examples](https://github.com/biomedisa/biomedisa/blob/master/README/deep_learning.md)
 
 #### Python example (training)
@@ -124,22 +127,23 @@
 # deep learning 
 deep_learning(img_data, label_data, train=True, batch_size=12,
         val_img_data=val_img_data, val_label_data=val_label_data,
         header=header, extension=ext, path_to_model='honeybees.h5')
 ```
 
 #### Command-line based (training)
+Start training with a batch size of 12:
 ```
-# start training with a batch size of 12
 python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -bs=12
-
-# validation (optional)
+```
+Monitor training progress using validation data:
+```
 python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -vi=C:\Users\%USERNAME%\Downloads\val_img -vl=C:\Users\%USERNAME%\Downloads\val_labels
 ```
-If running into ResourceExhaustedError due to out of memory (OOM), try to use smaller batch size.
+If running into ResourceExhaustedError due to out of memory (OOM), try to use a smaller batch size.
 
 #### Python example (prediction)
 ```python
 from biomedisa.features.biomedisa_helper import load_data, save_data
 from biomedisa.deeplearning import deep_learning
 
 # load data
@@ -154,61 +158,52 @@
 ```
 
 #### Command-line based (prediction)
 ```
 python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\testing_axial_crop_pat13.nii.gz C:\Users\%USERNAME%\Downloads\heart.h5 -p
 ```
 
-## Biomedisa Features
-
-#### Load and save data (such as Amira Mesh, TIFF, NRRD, NIfTI or DICOM)
-```python
-from biomedisa.features.biomedisa_helper import load_data, save_data
-
-# load data as numpy array
-# for DICOM, PNG files, or similar formats, 'path_to_data' must reference
-# either a directory or a ZIP file containing the image slices
-data, header = load_data(path_to_data)
-
-# save data (for TIFF, header=None)
-save_data(path_to_data, data, header)
-```
+## Mesh Generator
++ [Parameters and Examples](https://github.com/biomedisa/biomedisa/blob/master/README/save_mesh.md)
 
-#### Create STL mesh from segmentation (label values are saved as attributes)
+#### Python example
+Create STL mesh from segmentation (label values are saved as attributes)
 ```python
 from biomedisa.features.biomedisa_helper import load_data, save_data
 from biomedisa.mesh import get_voxel_spacing, save_mesh
 
 # load segmentation
-data, header, extension = load_data(path_to_data, return_extension=True)
+data, header, extension = load_data('final.Head5.am', return_extension=True)
 
 # get voxel spacing
 x_res, y_res, z_res = get_voxel_spacing(header, data, extension)
 print(f'Voxel spacing: x_spacing, y_spacing, z_spacing = {x_res}, {y_res}, {z_res}')
 
 # save stl file
-path_to_data = path_to_data.replace(os.path.splitext(path_to_data)[1],'.stl')
-save_mesh(path_to_data, data, x_res, y_res, z_res, poly_reduction=0.9, smoothing_iterations=15)
+save_mesh('final.Head5.stl', data, x_res, y_res, z_res, poly_reduction=0.9, smoothing_iterations=15)
 ```
 
-#### Create mesh directly
+#### Command-line based
 ```
-python -m biomedisa.mesh <path_to_data>
+python -m biomedisa.mesh 'final.Head5.am'
 ```
 
-#### Options
-`--poly_reduction` or `-pr`: Reduce number of polygons by this factor (default: 0.9)
-
-`--smoothing_iterations` or `-s`: Iteration steps for smoothing (default: 15)
+## Biomedisa Features
 
-`--x_res` or `-xres`: Voxel spacing/resolution x-axis (default: None)
+#### Load and save data (such as Amira Mesh, TIFF, NRRD, NIfTI or DICOM)
+For DICOM, PNG files, or similar formats, file path must reference either a directory or a ZIP file containing the image slices.
+```python
+from biomedisa.features.biomedisa_helper import load_data, save_data
 
-`--y_res` or `-yres`: Voxel spacing/resolution y-axis (default: None)
+# load data as numpy array
+data, header = load_data('temp.tif')
 
-`--z_res` or `-zres`: Voxel spacing/resolution z-axis (default: None)
+# save data (for TIFF, header=None)
+save_data('temp.tif', data, header)
+```
 
 #### Resize data
 ```python
 from biomedisa.features.biomedisa_helper import img_resize
 
 # resize image data
 zsh, ysh, xsh = data.shape
```

### Comparing `biomedisa-2024.5.22/src/biomedisa.egg-info/SOURCES.txt` & `biomedisa-24.5.23/src/biomedisa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

