# Comparing `tmp/satsure-core-test-0.2.6.tar.gz` & `tmp/satsure-core-test-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satsure-core-test-0.2.6.tar", last modified: Thu May 16 10:31:14 2024, max compression
+gzip compressed data, was "satsure-core-test-0.2.7.tar", last modified: Fri May 17 11:30:37 2024, max compression
```

## Comparing `satsure-core-test-0.2.6.tar` & `satsure-core-test-0.2.7.tar`

### file list

```diff
@@ -1,63 +1,61 @@
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 10:31:14.410365 satsure-core-test-0.2.6/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:02.000000 satsure-core-test-0.2.6/LICENCE.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       24 2024-05-16 06:11:06.000000 satsure-core-test-0.2.6/MANIFEST.in
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      515 2024-05-16 10:31:14.410186 satsure-core-test-0.2.6/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:18.000000 satsure-core-test-0.2.6/README.md
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 10:31:14.401372 satsure-core-test-0.2.6/satelite/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-06 07:15:52.000000 satsure-core-test-0.2.6/satelite/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      976 2024-05-16 05:55:40.000000 satsure-core-test-0.2.6/satelite/config.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 10:31:14.402069 satsure-core-test-0.2.6/satelite/core/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.6/satelite/core/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     4877 2024-05-16 02:50:40.000000 satsure-core-test-0.2.6/satelite/core/downloader.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      825 2024-05-16 05:29:12.000000 satsure-core-test-0.2.6/satelite/core/uploader.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2361 2024-04-25 12:00:27.000000 satsure-core-test-0.2.6/satelite/gcp.json
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 10:31:14.402546 satsure-core-test-0.2.6/satelite/gdal/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.6/satelite/gdal/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2511 2024-05-14 15:24:54.000000 satsure-core-test-0.2.6/satelite/gdal/gdal_commands.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 10:31:14.402879 satsure-core-test-0.2.6/satelite/models/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.6/satelite/models/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-13 07:33:26.000000 satsure-core-test-0.2.6/satelite/models/s2_enum.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 10:31:14.403173 satsure-core-test-0.2.6/satelite/raster/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.6/satelite/raster/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8913 2024-05-13 07:51:34.000000 satsure-core-test-0.2.6/satelite/raster/raster.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 10:31:14.405527 satsure-core-test-0.2.6/satelite/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      499 2024-05-15 14:34:51.000000 satsure-core-test-0.2.6/satelite/sentinel2/__init__.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 10:31:14.405855 satsure-core-test-0.2.6/satelite/sentinel2/band_stack/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.6/satelite/sentinel2/band_stack/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2834 2024-05-15 12:28:03.000000 satsure-core-test-0.2.6/satelite/sentinel2/band_stack/generate_band_stack.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-13 07:33:26.000000 satsure-core-test-0.2.6/satelite/sentinel2/fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-06 07:15:52.000000 satsure-core-test-0.2.6/satelite/sentinel2/fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3204 2024-05-14 12:04:20.000000 satsure-core-test-0.2.6/satelite/sentinel2/get_tiles.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 10:31:14.406218 satsure-core-test-0.2.6/satelite/sentinel2/indices/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.6/satelite/sentinel2/indices/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3975 2024-05-15 12:01:41.000000 satsure-core-test-0.2.6/satelite/sentinel2/indices/general_indices.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      835 2024-05-15 14:22:44.000000 satsure-core-test-0.2.6/satelite/sentinel2/mosaic_custom_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2804 2024-05-16 10:31:04.000000 satsure-core-test-0.2.6/satelite/sentinel2/mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-13 07:51:34.000000 satsure-core-test-0.2.6/satelite/sentinel2/path_row_from_shp.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3251 2024-05-16 05:49:19.000000 satsure-core-test-0.2.6/satelite/sentinel2/s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2912 2024-05-13 07:33:26.000000 satsure-core-test-0.2.6/satelite/sentinel2/s2_l2a_urls.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 10:31:14.406578 satsure-core-test-0.2.6/satelite/tests/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure-core-test-0.2.6/satelite/tests/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1004 2024-05-14 12:00:39.000000 satsure-core-test-0.2.6/satelite/tests/conftest.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 10:31:14.409154 satsure-core-test-0.2.6/satelite/tests/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure-core-test-0.2.6/satelite/tests/sentinel2/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      384 2024-05-13 07:58:31.000000 satsure-core-test-0.2.6/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      430 2024-05-06 07:34:13.000000 satsure-core-test-0.2.6/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1176 2024-05-15 12:53:42.000000 satsure-core-test-0.2.6/satelite/tests/sentinel2/test_genarate_band_stack.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1318 2024-05-16 03:04:58.000000 satsure-core-test-0.2.6/satelite/tests/sentinel2/test_general_indices.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1326 2024-05-14 12:00:39.000000 satsure-core-test-0.2.6/satelite/tests/sentinel2/test_get_tile.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      322 2024-05-13 07:33:26.000000 satsure-core-test-0.2.6/satelite/tests/sentinel2/test_mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      871 2024-05-13 07:33:26.000000 satsure-core-test-0.2.6/satelite/tests/sentinel2/test_s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      898 2024-05-13 07:33:26.000000 satsure-core-test-0.2.6/satelite/tests/sentinel2/test_s2_l2a_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1543 2024-05-13 07:33:26.000000 satsure-core-test-0.2.6/satelite/tests/sentinel2/test_validate.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 10:31:14.409366 satsure-core-test-0.2.6/satelite/validators/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:51:34.000000 satsure-core-test-0.2.6/satelite/validators/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2381 2024-05-13 07:51:34.000000 satsure-core-test-0.2.6/satelite/validators/check_shape_of_rid.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 10:31:14.409978 satsure-core-test-0.2.6/satsure_core_test.egg-info/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      515 2024-05-16 10:31:14.000000 satsure-core-test-0.2.6/satsure_core_test.egg-info/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1691 2024-05-16 10:31:14.000000 satsure-core-test-0.2.6/satsure_core_test.egg-info/SOURCES.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-16 10:31:14.000000 satsure-core-test-0.2.6/satsure_core_test.egg-info/dependency_links.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      141 2024-05-16 10:31:14.000000 satsure-core-test-0.2.6/satsure_core_test.egg-info/requires.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        9 2024-05-16 10:31:14.000000 satsure-core-test-0.2.6/satsure_core_test.egg-info/top_level.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-16 10:31:14.410408 satsure-core-test-0.2.6/setup.cfg
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      601 2024-05-16 10:31:11.000000 satsure-core-test-0.2.6/setup.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 11:30:37.602675 satsure-core-test-0.2.7/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:02.000000 satsure-core-test-0.2.7/LICENCE.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      515 2024-05-17 11:30:37.602450 satsure-core-test-0.2.7/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:18.000000 satsure-core-test-0.2.7/README.md
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 11:30:37.592689 satsure-core-test-0.2.7/satelite/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      976 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/config.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 11:30:37.593378 satsure-core-test-0.2.7/satelite/core/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       65 2024-05-17 10:57:24.000000 satsure-core-test-0.2.7/satelite/core/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     5297 2024-05-17 10:57:24.000000 satsure-core-test-0.2.7/satelite/core/downloader.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      826 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/core/uploader.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 11:30:37.593705 satsure-core-test-0.2.7/satelite/gdal/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/gdal/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     5973 2024-05-17 10:57:24.000000 satsure-core-test-0.2.7/satelite/gdal/gdal_commands.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 11:30:37.594020 satsure-core-test-0.2.7/satelite/models/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/models/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/models/s2_enum.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 11:30:37.594279 satsure-core-test-0.2.7/satelite/raster/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/raster/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8913 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/raster/raster.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 11:30:37.596502 satsure-core-test-0.2.7/satelite/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      499 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/sentinel2/__init__.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 11:30:37.596934 satsure-core-test-0.2.7/satelite/sentinel2/band_stack/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       50 2024-05-17 11:04:57.000000 satsure-core-test-0.2.7/satelite/sentinel2/band_stack/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2834 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/sentinel2/band_stack/generate_band_stack.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/sentinel2/fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/sentinel2/fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3204 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/sentinel2/get_tiles.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 11:30:37.597301 satsure-core-test-0.2.7/satelite/sentinel2/indices/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       43 2024-05-17 11:04:57.000000 satsure-core-test-0.2.7/satelite/sentinel2/indices/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3975 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/sentinel2/indices/general_indices.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      835 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/sentinel2/mosaic_custom_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2553 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/sentinel2/mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/sentinel2/path_row_from_shp.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3251 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/sentinel2/s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2912 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/sentinel2/s2_l2a_urls.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 11:30:37.597560 satsure-core-test-0.2.7/satelite/tests/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/tests/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1004 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/tests/conftest.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 11:30:37.600005 satsure-core-test-0.2.7/satelite/tests/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/tests/sentinel2/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      384 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      430 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1176 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/tests/sentinel2/test_genarate_band_stack.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1318 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/tests/sentinel2/test_general_indices.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1326 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/tests/sentinel2/test_get_tile.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      322 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/tests/sentinel2/test_mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      871 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/tests/sentinel2/test_s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      898 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/tests/sentinel2/test_s2_l2a_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1543 2024-05-17 10:21:25.000000 satsure-core-test-0.2.7/satelite/tests/sentinel2/test_validate.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 11:30:37.600557 satsure-core-test-0.2.7/satelite/validators/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       47 2024-05-17 11:04:57.000000 satsure-core-test-0.2.7/satelite/validators/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2360 2024-05-17 11:02:14.000000 satsure-core-test-0.2.7/satelite/validators/check_shape_of_rid.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-17 11:30:37.602056 satsure-core-test-0.2.7/satsure_core_test.egg-info/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      515 2024-05-17 11:30:37.000000 satsure-core-test-0.2.7/satsure_core_test.egg-info/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1661 2024-05-17 11:30:37.000000 satsure-core-test-0.2.7/satsure_core_test.egg-info/SOURCES.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-17 11:30:37.000000 satsure-core-test-0.2.7/satsure_core_test.egg-info/dependency_links.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      141 2024-05-17 11:30:37.000000 satsure-core-test-0.2.7/satsure_core_test.egg-info/requires.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        9 2024-05-17 11:30:37.000000 satsure-core-test-0.2.7/satsure_core_test.egg-info/top_level.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-17 11:30:37.602774 satsure-core-test-0.2.7/setup.cfg
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      601 2024-05-17 11:04:57.000000 satsure-core-test-0.2.7/setup.py
```

### Comparing `satsure-core-test-0.2.6/PKG-INFO` & `satsure-core-test-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satsure-core-test
-Version: 0.2.6
+Version: 0.2.7
 Summary: satsure core package
 Author: Satsure
 Author-email: kmstpm@email.com
 License-File: LICENCE.txt
 Requires-Dist: awscli
 Requires-Dist: fiona
 Requires-Dist: gdal==3.6.2
```

### Comparing `satsure-core-test-0.2.6/satelite/config.py` & `satsure-core-test-0.2.7/satelite/config.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.6/satelite/core/downloader.py` & `satsure-core-test-0.2.7/satelite/core/downloader.py`

 * *Files 7% similar despite different names*

```diff
@@ -85,16 +85,15 @@
         """
         start_date = datetime.strptime(start_date, '%Y-%m-%d')
         end_date = datetime.strptime(end_date, '%Y-%m-%d')
         num_days = (end_date - start_date).days + 1
         return [(start_date + timedelta(days=i)).strftime('%Y-%m-%d') for i in
                 range(num_days)]
 
-    @staticmethod
-    def _list_objects_from_s3(bucket_name: str, prefix: str = "",
+    def list_objects_from_s3(self,bucket_name: str, prefix: str = "",
                               include: List[str] = ["*"],
                               exclude: List[str] = ["*"]) -> List[str]:
         """
             fetching data from AWS
         :param bucket_name:
         :param prefix:
         :param include:
@@ -129,9 +128,23 @@
         """
 
         includes = [f"*{date.replace('-', '')}*" for date in
                     self._get_dates_between(start_date, end_date)]
         if include:
             includes = include + includes
 
-        return self._list_objects_from_s3(bucket_name, prefix, includes,
+        return self.list_objects_from_s3(bucket_name, prefix, includes,
                                           exclude)
+
+    def download_object_from_s3(self, s3_path: str, local_path: PosixPath):
+        """
+            Download from s3_path to local_path
+        :param s3_path:
+        :param local_path:
+        :return:
+        """
+        command = f"""aws s3 cp "{s3_path}" "{local_path}" --request-payer"""
+
+        process = Popen(command, shell=True, stdout=PIPE)
+        stdout, _ = process.communicate()
+
+        return stdout.decode("utf-8")
```

### Comparing `satsure-core-test-0.2.6/satelite/core/uploader.py` & `satsure-core-test-0.2.7/satelite/core/uploader.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,7 +19,8 @@
         """
         command = f"""aws s3 cp "{local_folder}" "s3://{bucket_name}/{prefix}" --recursive --exclude "{exclude}" --include "{include}" --request-payer"""
         process = Popen(command, shell=True, stdout=PIPE)
         process.communicate()
 
         if delete_local:
             shutil.rmtree(Path(local_folder))
+
```

### Comparing `satsure-core-test-0.2.6/satelite/raster/raster.py` & `satsure-core-test-0.2.7/satelite/raster/raster.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.6/satelite/sentinel2/band_stack/generate_band_stack.py` & `satsure-core-test-0.2.7/satelite/sentinel2/band_stack/generate_band_stack.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.6/satelite/sentinel2/fetch_unique_tile_date.py` & `satsure-core-test-0.2.7/satelite/sentinel2/fetch_unique_tile_date.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.6/satelite/sentinel2/fetch_unique_tile_date_pystac.py` & `satsure-core-test-0.2.7/satelite/sentinel2/fetch_unique_tile_date_pystac.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.6/satelite/sentinel2/get_tiles.py` & `satsure-core-test-0.2.7/satelite/sentinel2/get_tiles.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.6/satelite/sentinel2/indices/general_indices.py` & `satsure-core-test-0.2.7/satelite/sentinel2/indices/general_indices.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.6/satelite/sentinel2/mosaic_custom_bands.py` & `satsure-core-test-0.2.7/satelite/sentinel2/mosaic_custom_bands.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.6/satelite/sentinel2/mosaic_same_bands.py` & `satsure-core-test-0.2.7/satelite/sentinel2/mosaic_same_bands.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,13 +60,10 @@
                     output_datatype=None,
                     output_crs=None,
                     output_pixel_size=(10, 10),
                     creation_option=creation_option
                 )
 
                 for file in files:
-                    print(file.name, f"{date}_{unique_tile}_{band}.{input_file_format}","pacakes")
-                    print(file.name == f"{date}_{unique_tile}_{band}.{input_file_format}", "this assert")
                     if file.name == f"{date}_{unique_tile}_{band}.{input_file_format}":
                         continue
-                    print("file unlink",file)
                     file.unlink()
```

### Comparing `satsure-core-test-0.2.6/satelite/sentinel2/path_row_from_shp.py` & `satsure-core-test-0.2.7/satelite/sentinel2/path_row_from_shp.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.6/satelite/sentinel2/s2_l1c_urls.py` & `satsure-core-test-0.2.7/satelite/sentinel2/s2_l1c_urls.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.6/satelite/sentinel2/s2_l2a_urls.py` & `satsure-core-test-0.2.7/satelite/sentinel2/s2_l2a_urls.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.6/satelite/tests/conftest.py` & `satsure-core-test-0.2.7/satelite/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.6/satelite/tests/sentinel2/test_genarate_band_stack.py` & `satsure-core-test-0.2.7/satelite/tests/sentinel2/test_genarate_band_stack.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.6/satelite/tests/sentinel2/test_general_indices.py` & `satsure-core-test-0.2.7/satelite/tests/sentinel2/test_general_indices.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.6/satelite/tests/sentinel2/test_get_tile.py` & `satsure-core-test-0.2.7/satelite/tests/sentinel2/test_get_tile.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.6/satelite/tests/sentinel2/test_s2_l1c_urls.py` & `satsure-core-test-0.2.7/satelite/tests/sentinel2/test_s2_l1c_urls.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.6/satelite/tests/sentinel2/test_s2_l2a_urls.py` & `satsure-core-test-0.2.7/satelite/tests/sentinel2/test_s2_l2a_urls.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.6/satelite/tests/sentinel2/test_validate.py` & `satsure-core-test-0.2.7/satelite/tests/sentinel2/test_validate.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.6/satelite/validators/check_shape_of_rid.py` & `satsure-core-test-0.2.7/satelite/validators/check_shape_of_rid.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,9 +57,9 @@
             total_count = stats[0]['count']
             area = abs(
                 (resolution_x * resolution_y * total_count) / 1000000)
             vector_area = utm_geom.area / 1000000
             raster_area = area
             if abs(vector_area - raster_area) < 20:
                 return rid
-            else:
-                return None
+
+            return None
```

### Comparing `satsure-core-test-0.2.6/satsure_core_test.egg-info/PKG-INFO` & `satsure-core-test-0.2.7/satsure_core_test.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satsure-core-test
-Version: 0.2.6
+Version: 0.2.7
 Summary: satsure core package
 Author: Satsure
 Author-email: kmstpm@email.com
 License-File: LICENCE.txt
 Requires-Dist: awscli
 Requires-Dist: fiona
 Requires-Dist: gdal==3.6.2
```

### Comparing `satsure-core-test-0.2.6/satsure_core_test.egg-info/SOURCES.txt` & `satsure-core-test-0.2.7/satsure_core_test.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 LICENCE.txt
-MANIFEST.in
 README.md
 setup.py
 satelite/__init__.py
 satelite/config.py
-satelite/gcp.json
 satelite/core/__init__.py
 satelite/core/downloader.py
 satelite/core/uploader.py
 satelite/gdal/__init__.py
 satelite/gdal/gdal_commands.py
 satelite/models/__init__.py
 satelite/models/s2_enum.py
```

### Comparing `satsure-core-test-0.2.6/setup.py` & `satsure-core-test-0.2.7/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='satsure-core-test',
-    version='0.2.6',
+    version='0.2.7',
     description='satsure core package',
     author='Satsure',
     author_email='kmstpm@email.com',
     packages=find_packages(),
     install_requires=['awscli', 'fiona','gdal==3.6.2', 'google-cloud-storage', 'pandas',
                       'pyproj', 'pystac','pystac-client', 'python-dotenv', 'rasterstats',
                       'rasterio', 'requests', 'requests', 'sqlalchemy', 'wget'],
```

