# Comparing `tmp/gempy_viewer-2024.1.2.tar.gz` & `tmp/gempy_viewer-2024.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gempy_viewer-2024.1.2.tar", last modified: Mon Apr 29 09:07:50 2024, max compression
+gzip compressed data, was "gempy_viewer-2024.1.4.tar", last modified: Fri May 17 07:16:46 2024, max compression
```

## Comparing `gempy_viewer-2024.1.2.tar` & `gempy_viewer-2024.1.4.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:07:49.985435 gempy_viewer-2024.1.2/
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3101 2023-06-19 10:17:18.000000 gempy_viewer-2024.1.2/.gitignore
--rw-r--r--   0 leguark   (1000) leguark   (1000)      623 2023-06-19 10:23:48.000000 gempy_viewer-2024.1.2/AUTHORS.rst
--rw-r--r--   0 leguark   (1000) leguark   (1000)    13874 2023-06-19 10:23:48.000000 gempy_viewer-2024.1.2/LICENSE
--rw-r--r--   0 leguark   (1000) leguark   (1000)      852 2024-04-29 09:07:49.985435 gempy_viewer-2024.1.2/PKG-INFO
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1484 2023-07-26 10:50:13.000000 gempy_viewer-2024.1.2/README.md
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:07:49.975435 gempy_viewer-2024.1.2/gempy_viewer/
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:07:49.975435 gempy_viewer-2024.1.2/gempy_viewer/API/
--rw-r--r--   0 leguark   (1000) leguark   (1000)      348 2024-04-24 08:21:05.000000 gempy_viewer-2024.1.2/gempy_viewer/API/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    10875 2023-10-10 11:45:51.000000 gempy_viewer-2024.1.2/gempy_viewer/API/_plot_2d_API.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     7959 2024-04-12 09:01:44.000000 gempy_viewer-2024.1.2/gempy_viewer/API/_plot_2d_sections_api.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6119 2023-11-21 15:10:45.000000 gempy_viewer-2024.1.2/gempy_viewer/API/_plot_3d_API.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1295 2024-04-25 08:23:03.000000 gempy_viewer-2024.1.2/gempy_viewer/API/_plot_LiquidEarth.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3638 2023-11-21 16:20:52.000000 gempy_viewer-2024.1.2/gempy_viewer/API/_plot_others.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:07:49.975435 gempy_viewer-2024.1.2/gempy_viewer/DEP/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:59:27.000000 gempy_viewer-2024.1.2/gempy_viewer/DEP/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    14538 2023-06-22 11:01:14.000000 gempy_viewer-2024.1.2/gempy_viewer/DEP/_plot.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    54327 2023-06-22 10:59:32.000000 gempy_viewer-2024.1.2/gempy_viewer/DEP/_visualization_2d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4308 2023-06-22 10:59:32.000000 gempy_viewer-2024.1.2/gempy_viewer/DEP/decorators.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    60928 2024-04-16 12:28:49.000000 gempy_viewer-2024.1.2/gempy_viewer/DEP/visualization_3d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      397 2024-04-12 12:54:09.000000 gempy_viewer-2024.1.2/gempy_viewer/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      417 2024-04-29 09:07:49.000000 gempy_viewer-2024.1.2/gempy_viewer/_version.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:07:49.975435 gempy_viewer-2024.1.2/gempy_viewer/core/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:53:54.000000 gempy_viewer-2024.1.2/gempy_viewer/core/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1976 2023-09-27 08:52:01.000000 gempy_viewer-2024.1.2/gempy_viewer/core/data_to_show.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      479 2023-07-10 13:33:23.000000 gempy_viewer-2024.1.2/gempy_viewer/core/plotting_2d_options.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      301 2023-07-26 12:29:31.000000 gempy_viewer-2024.1.2/gempy_viewer/core/scalar_data_type.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      496 2023-07-25 14:27:44.000000 gempy_viewer-2024.1.2/gempy_viewer/core/section_data_2d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      380 2023-07-25 14:27:44.000000 gempy_viewer-2024.1.2/gempy_viewer/core/slicer_data.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:07:49.975435 gempy_viewer-2024.1.2/gempy_viewer/modules/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:54:05.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/__init__.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:07:49.985435 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:54:45.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3921 2023-08-02 09:19:49.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/drawer_contours_2d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     8783 2024-04-12 09:01:44.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/drawer_input_2d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2807 2023-12-05 14:47:00.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/drawer_regular_grid_2d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2983 2023-08-22 13:43:39.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/drawer_scalar_field_2d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4905 2024-04-12 09:01:44.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/drawer_topography_2d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      764 2024-04-12 09:01:44.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/drawer_traces_2d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      847 2023-11-08 11:53:57.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/helpers.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     7313 2024-04-12 09:01:44.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/multi_axis_manager.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     5067 2024-04-12 09:01:44.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/plot_2d_utils.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    12753 2023-06-18 07:52:19.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/plot_utils_DEP.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4242 2023-10-09 13:35:04.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/visualization_2d.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:07:49.985435 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:54:58.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    42075 2024-04-16 12:28:49.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/_vista.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4352 2024-04-12 09:01:44.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/drawer_input_3d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     5800 2024-04-12 12:58:30.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/drawer_structured_grid_3d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1321 2023-11-21 15:13:49.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/drawer_surfaces_3d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3000 2024-04-16 12:28:49.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/drawer_topography_3d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1715 2023-09-08 13:45:29.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/plot_3d_utils.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4520 2024-04-16 12:28:49.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/vista.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2523 2023-06-22 11:38:56.000000 gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/vista_qt.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1150 2024-04-24 08:21:06.000000 gempy_viewer-2024.1.2/gempy_viewer/optional_dependencies.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:07:49.985435 gempy_viewer-2024.1.2/gempy_viewer.egg-info/
--rw-r--r--   0 leguark   (1000) leguark   (1000)      852 2024-04-29 09:07:49.000000 gempy_viewer-2024.1.2/gempy_viewer.egg-info/PKG-INFO
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2209 2024-04-29 09:07:49.000000 gempy_viewer-2024.1.2/gempy_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)        1 2024-04-29 09:07:49.000000 gempy_viewer-2024.1.2/gempy_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)        1 2024-04-29 09:07:49.000000 gempy_viewer-2024.1.2/gempy_viewer.egg-info/not-zip-safe
--rw-r--r--   0 leguark   (1000) leguark   (1000)       81 2024-04-29 09:07:49.000000 gempy_viewer-2024.1.2/gempy_viewer.egg-info/requires.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)       19 2024-04-29 09:07:49.000000 gempy_viewer-2024.1.2/gempy_viewer.egg-info/top_level.txt
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:07:49.985435 gempy_viewer-2024.1.2/requirements/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        6 2023-09-14 06:30:21.000000 gempy_viewer-2024.1.2/requirements/dev-requirements.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)       50 2024-04-29 09:05:44.000000 gempy_viewer-2024.1.2/requirements/optional_requirements.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)       34 2024-04-29 09:06:54.000000 gempy_viewer-2024.1.2/requirements/requirements.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)       38 2024-04-29 09:07:49.985435 gempy_viewer-2024.1.2/setup.cfg
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2115 2024-04-29 09:05:44.000000 gempy_viewer-2024.1.2/setup.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:07:49.985435 gempy_viewer-2024.1.2/tests/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-19 11:53:13.000000 gempy_viewer-2024.1.2/tests/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2313 2023-10-11 08:49:21.000000 gempy_viewer-2024.1.2/tests/conftest.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-04-29 09:07:49.985435 gempy_viewer-2024.1.2/tests/test_plotting/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:52:19.000000 gempy_viewer-2024.1.2/tests/test_plotting/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     7826 2024-04-12 12:56:44.000000 gempy_viewer-2024.1.2/tests/test_plotting/test_plot_2d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2715 2023-08-04 09:08:59.000000 gempy_viewer-2024.1.2/tests/test_plotting/test_plot_3d.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:16:46.560167 gempy_viewer-2024.1.4/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3101 2023-06-19 10:17:18.000000 gempy_viewer-2024.1.4/.gitignore
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      623 2023-06-19 10:23:48.000000 gempy_viewer-2024.1.4/AUTHORS.rst
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    13874 2023-06-19 10:23:48.000000 gempy_viewer-2024.1.4/LICENSE
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      852 2024-05-17 07:16:46.560167 gempy_viewer-2024.1.4/PKG-INFO
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1484 2023-07-26 10:50:13.000000 gempy_viewer-2024.1.4/README.md
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:16:46.550167 gempy_viewer-2024.1.4/gempy_viewer/
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:16:46.550167 gempy_viewer-2024.1.4/gempy_viewer/API/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      357 2024-05-16 14:04:48.000000 gempy_viewer-2024.1.4/gempy_viewer/API/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    10893 2024-05-16 14:06:55.000000 gempy_viewer-2024.1.4/gempy_viewer/API/_plot_2d_API.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     7977 2024-05-16 14:06:55.000000 gempy_viewer-2024.1.4/gempy_viewer/API/_plot_2d_sections_api.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6231 2024-05-16 14:06:55.000000 gempy_viewer-2024.1.4/gempy_viewer/API/_plot_3d_API.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1332 2024-05-16 14:04:48.000000 gempy_viewer-2024.1.4/gempy_viewer/API/_plot_LiquidEarth.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3638 2023-11-21 16:20:52.000000 gempy_viewer-2024.1.4/gempy_viewer/API/_plot_others.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:16:46.550167 gempy_viewer-2024.1.4/gempy_viewer/DEP/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:59:27.000000 gempy_viewer-2024.1.4/gempy_viewer/DEP/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    14538 2023-06-22 11:01:14.000000 gempy_viewer-2024.1.4/gempy_viewer/DEP/_plot.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    54327 2023-06-22 10:59:32.000000 gempy_viewer-2024.1.4/gempy_viewer/DEP/_visualization_2d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4308 2023-06-22 10:59:32.000000 gempy_viewer-2024.1.4/gempy_viewer/DEP/decorators.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    60928 2024-05-16 14:04:48.000000 gempy_viewer-2024.1.4/gempy_viewer/DEP/visualization_3d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      411 2024-05-16 14:02:47.000000 gempy_viewer-2024.1.4/gempy_viewer/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      417 2024-05-17 07:16:46.000000 gempy_viewer-2024.1.4/gempy_viewer/_version.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:16:46.550167 gempy_viewer-2024.1.4/gempy_viewer/core/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:53:54.000000 gempy_viewer-2024.1.4/gempy_viewer/core/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1976 2023-09-27 08:52:01.000000 gempy_viewer-2024.1.4/gempy_viewer/core/data_to_show.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      479 2023-07-10 13:33:23.000000 gempy_viewer-2024.1.4/gempy_viewer/core/plotting_2d_options.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      301 2023-07-26 12:29:31.000000 gempy_viewer-2024.1.4/gempy_viewer/core/scalar_data_type.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      496 2023-07-25 14:27:44.000000 gempy_viewer-2024.1.4/gempy_viewer/core/section_data_2d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      380 2023-07-25 14:27:44.000000 gempy_viewer-2024.1.4/gempy_viewer/core/slicer_data.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:16:46.550167 gempy_viewer-2024.1.4/gempy_viewer/modules/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:54:05.000000 gempy_viewer-2024.1.4/gempy_viewer/modules/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:16:46.550167 gempy_viewer-2024.1.4/gempy_viewer/modules/plot_2d/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:54:45.000000 gempy_viewer-2024.1.4/gempy_viewer/modules/plot_2d/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3921 2023-08-02 09:19:49.000000 gempy_viewer-2024.1.4/gempy_viewer/modules/plot_2d/drawer_contours_2d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     8665 2024-05-16 14:33:46.000000 gempy_viewer-2024.1.4/gempy_viewer/modules/plot_2d/drawer_input_2d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2807 2024-05-13 09:16:16.000000 gempy_viewer-2024.1.4/gempy_viewer/modules/plot_2d/drawer_regular_grid_2d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2983 2023-08-22 13:43:39.000000 gempy_viewer-2024.1.4/gempy_viewer/modules/plot_2d/drawer_scalar_field_2d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4905 2024-04-12 09:01:44.000000 gempy_viewer-2024.1.4/gempy_viewer/modules/plot_2d/drawer_topography_2d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      764 2024-04-12 09:01:44.000000 gempy_viewer-2024.1.4/gempy_viewer/modules/plot_2d/drawer_traces_2d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      847 2023-11-08 11:53:57.000000 gempy_viewer-2024.1.4/gempy_viewer/modules/plot_2d/helpers.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     7313 2024-05-16 14:02:47.000000 gempy_viewer-2024.1.4/gempy_viewer/modules/plot_2d/multi_axis_manager.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     5067 2024-04-12 09:01:44.000000 gempy_viewer-2024.1.4/gempy_viewer/modules/plot_2d/plot_2d_utils.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    12753 2023-06-18 07:52:19.000000 gempy_viewer-2024.1.4/gempy_viewer/modules/plot_2d/plot_utils_DEP.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4242 2023-10-09 13:35:04.000000 gempy_viewer-2024.1.4/gempy_viewer/modules/plot_2d/visualization_2d.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:16:46.550167 gempy_viewer-2024.1.4/gempy_viewer/modules/plot_3d/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:54:58.000000 gempy_viewer-2024.1.4/gempy_viewer/modules/plot_3d/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    42075 2024-05-16 14:04:48.000000 gempy_viewer-2024.1.4/gempy_viewer/modules/plot_3d/_vista.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4352 2024-05-16 14:02:47.000000 gempy_viewer-2024.1.4/gempy_viewer/modules/plot_3d/drawer_input_3d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6012 2024-05-16 14:06:55.000000 gempy_viewer-2024.1.4/gempy_viewer/modules/plot_3d/drawer_structured_grid_3d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1321 2023-11-21 15:13:49.000000 gempy_viewer-2024.1.4/gempy_viewer/modules/plot_3d/drawer_surfaces_3d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3085 2024-05-16 14:04:48.000000 gempy_viewer-2024.1.4/gempy_viewer/modules/plot_3d/drawer_topography_3d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1715 2023-09-08 13:45:29.000000 gempy_viewer-2024.1.4/gempy_viewer/modules/plot_3d/plot_3d_utils.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4520 2024-05-16 14:04:48.000000 gempy_viewer-2024.1.4/gempy_viewer/modules/plot_3d/vista.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2523 2023-06-22 11:38:56.000000 gempy_viewer-2024.1.4/gempy_viewer/modules/plot_3d/vista_qt.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1192 2024-05-16 14:04:48.000000 gempy_viewer-2024.1.4/gempy_viewer/optional_dependencies.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:16:46.560167 gempy_viewer-2024.1.4/gempy_viewer.egg-info/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      852 2024-05-17 07:16:46.000000 gempy_viewer-2024.1.4/gempy_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2209 2024-05-17 07:16:46.000000 gempy_viewer-2024.1.4/gempy_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        1 2024-05-17 07:16:46.000000 gempy_viewer-2024.1.4/gempy_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        1 2024-04-29 09:07:49.000000 gempy_viewer-2024.1.4/gempy_viewer.egg-info/not-zip-safe
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       81 2024-05-17 07:16:46.000000 gempy_viewer-2024.1.4/gempy_viewer.egg-info/requires.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       19 2024-05-17 07:16:46.000000 gempy_viewer-2024.1.4/gempy_viewer.egg-info/top_level.txt
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:16:46.550167 gempy_viewer-2024.1.4/requirements/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        6 2024-05-16 14:04:48.000000 gempy_viewer-2024.1.4/requirements/dev-requirements.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       50 2024-05-16 14:04:48.000000 gempy_viewer-2024.1.4/requirements/optional_requirements.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       34 2024-05-17 07:10:38.000000 gempy_viewer-2024.1.4/requirements/requirements.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       38 2024-05-17 07:16:46.560167 gempy_viewer-2024.1.4/setup.cfg
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2115 2024-05-16 14:04:48.000000 gempy_viewer-2024.1.4/setup.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:16:46.550167 gempy_viewer-2024.1.4/tests/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-19 11:53:13.000000 gempy_viewer-2024.1.4/tests/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2313 2023-10-11 08:49:21.000000 gempy_viewer-2024.1.4/tests/conftest.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2024-05-17 07:16:46.560167 gempy_viewer-2024.1.4/tests/test_plotting/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:52:19.000000 gempy_viewer-2024.1.4/tests/test_plotting/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     8100 2024-05-16 15:22:00.000000 gempy_viewer-2024.1.4/tests/test_plotting/test_plot_2d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2847 2024-05-16 15:22:00.000000 gempy_viewer-2024.1.4/tests/test_plotting/test_plot_3d.py
```

### Comparing `gempy_viewer-2024.1.2/.gitignore` & `gempy_viewer-2024.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/AUTHORS.rst` & `gempy_viewer-2024.1.4/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/LICENSE` & `gempy_viewer-2024.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/PKG-INFO` & `gempy_viewer-2024.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gempy_viewer
-Version: 2024.1.2
+Version: 2024.1.4
 Summary: Viewer for the geological modeling package GemPy
 Home-page: 
 Author: Miguel de la Varga
 Author-email: miguel@terranigma-solutions.com
 License: EUPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 License-File: LICENSE
 License-File: AUTHORS.rst
-Requires-Dist: gempy==2024.1.2
+Requires-Dist: gempy~=2024.1.4
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Provides-Extra: opt
 Requires-Dist: pyvista; extra == "opt"
 Requires-Dist: scipy; extra == "opt"
 Requires-Dist: pooch; extra == "opt"
 Requires-Dist: pandas; extra == "opt"
```

### Comparing `gempy_viewer-2024.1.2/README.md` & `gempy_viewer-2024.1.4/README.md`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/API/_plot_2d_API.py` & `gempy_viewer-2024.1.4/gempy_viewer/API/_plot_2d_API.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from gempy_viewer.API._plot_2d_sections_api import plot_sections
 from gempy_viewer.core.data_to_show import DataToShow
 from gempy_viewer.core.section_data_2d import SectionData2D
 from gempy_viewer.modules.plot_2d.multi_axis_manager import sections_iterator, orthogonal_sections_iterator
 from gempy_viewer.modules.plot_2d.visualization_2d import Plot2D
 
 
+# noinspection t
 def plot_2d(model: GeoModel,
             n_axis=None,
             section_names: list = None,
             cell_number: Optional[Union[int | list[int] | str | list[str]]] = None,
             direction: Optional[Union[str | list[str]]] = 'y',
             series_n: Union[int, List[int]] = 0,
             legend: bool = True,
```

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/API/_plot_2d_sections_api.py` & `gempy_viewer-2024.1.4/gempy_viewer/API/_plot_2d_sections_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from ..modules.plot_2d.drawer_regular_grid_2d import plot_section_area, plot_regular_grid_area
 from ..modules.plot_2d.drawer_scalar_field_2d import plot_section_scalar_field, plot_regular_grid_scalar_field
 from ..modules.plot_2d.drawer_topography_2d import plot_topography
 from ..modules.plot_2d.drawer_traces_2d import plot_section_traces
 from ..modules.plot_2d.plot_2d_utils import get_geo_model_cmap, get_geo_model_norm
 
 
+# noinspection t
 def plot_sections(gempy_model: GeoModel, sections_data: list[SectionData2D], data_to_show: DataToShow,
                   ve: float = 1, series_n: Optional[list[int]] = None, override_regular_grid: Optional[np.ndarray] = None,
                   legend: bool = True,
                   kwargs_topography: dict = None,
                   kwargs_scalar_field: dict = None,
                   kwargs_lithology: dict = None
                   ):
```

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/API/_plot_3d_API.py` & `gempy_viewer-2024.1.4/gempy_viewer/API/_plot_3d_API.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     import mplstereonet
 
     mplstereonet_import = True
 except ImportError:
     mplstereonet_import = False
 
 
+# noinspection t
 def plot_3d(
         model: GeoModel,
         plotter_type='basic',
         active_scalar_field: str = None,
         ve=None,
         topography_scalar_type: TopographyDataType = TopographyDataType.GEOMAP,
         kwargs_pyvista_bounds=None,
@@ -152,19 +153,24 @@
         gempy_vista.p.set_scale(zscale=ve)
 
     fig_path: str = kwargs.get('fig_path', None)
     if fig_path is not None:
         gempy_vista.p.show(screenshot=fig_path)
 
     if image is True:
-        gempy_vista.p.show(screenshot=True)
-        img = gempy_vista.p.last_image
-        plt.imshow(img)
-        plt.axis('off')
-        plt.show(block=False)
-        gempy_vista.p.close()
-        show= False
+        show = _plot_in_matplotlib(gempy_vista, show)
 
     if show is True:
         gempy_vista.p.show()
 
     return gempy_vista
+
+
+def _plot_in_matplotlib(gempy_vista, show):
+    gempy_vista.p.show(screenshot=True)
+    img = gempy_vista.p.last_image
+    plt.imshow(img)
+    plt.axis('off')
+    plt.show(block=False)
+    gempy_vista.p.close()
+    show = False
+    return show
```

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/API/_plot_others.py` & `gempy_viewer-2024.1.4/gempy_viewer/API/_plot_others.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/DEP/_plot.py` & `gempy_viewer-2024.1.4/gempy_viewer/DEP/_plot.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/DEP/_visualization_2d.py` & `gempy_viewer-2024.1.4/gempy_viewer/DEP/_visualization_2d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/DEP/decorators.py` & `gempy_viewer-2024.1.4/gempy_viewer/DEP/decorators.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/DEP/visualization_3d.py` & `gempy_viewer-2024.1.4/gempy_viewer/DEP/visualization_3d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/core/data_to_show.py` & `gempy_viewer-2024.1.4/gempy_viewer/core/data_to_show.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/drawer_contours_2d.py` & `gempy_viewer-2024.1.4/gempy_viewer/modules/plot_2d/drawer_contours_2d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/drawer_input_2d.py` & `gempy_viewer-2024.1.4/gempy_viewer/modules/plot_2d/drawer_input_2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,17 +113,14 @@
         edgecolors='white',
         zorder=102
     )
 
 
 def _projection_params_regular_grid(regular_grid: RegularGrid, cell_number, direction, orientations, points,
                                     projection_distance) -> SlicerData:
-    # if cell_number is None or cell_number == "mid":
-    #     cell_number = int(regular_grid.resolution[0] / 2)
-
     if direction == 'x' or direction == 'X':
         arg_ = 0
         dx = regular_grid.dx
         dir = 'X'
     elif direction == 'y' or direction == 'Y':
         arg_ = 2
         dx = regular_grid.dy
```

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/drawer_regular_grid_2d.py` & `gempy_viewer-2024.1.4/gempy_viewer/modules/plot_2d/drawer_regular_grid_2d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/drawer_scalar_field_2d.py` & `gempy_viewer-2024.1.4/gempy_viewer/modules/plot_2d/drawer_scalar_field_2d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/drawer_topography_2d.py` & `gempy_viewer-2024.1.4/gempy_viewer/modules/plot_2d/drawer_topography_2d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/drawer_traces_2d.py` & `gempy_viewer-2024.1.4/gempy_viewer/modules/plot_2d/drawer_traces_2d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/helpers.py` & `gempy_viewer-2024.1.4/gempy_viewer/modules/plot_2d/helpers.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/multi_axis_manager.py` & `gempy_viewer-2024.1.4/gempy_viewer/modules/plot_2d/multi_axis_manager.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/plot_2d_utils.py` & `gempy_viewer-2024.1.4/gempy_viewer/modules/plot_2d/plot_2d_utils.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/plot_utils_DEP.py` & `gempy_viewer-2024.1.4/gempy_viewer/modules/plot_2d/plot_utils_DEP.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_2d/visualization_2d.py` & `gempy_viewer-2024.1.4/gempy_viewer/modules/plot_2d/visualization_2d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/_vista.py` & `gempy_viewer-2024.1.4/gempy_viewer/modules/plot_3d/_vista.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/drawer_input_3d.py` & `gempy_viewer-2024.1.4/gempy_viewer/modules/plot_3d/drawer_input_3d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/drawer_structured_grid_3d.py` & `gempy_viewer-2024.1.4/gempy_viewer/modules/plot_3d/drawer_structured_grid_3d.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,154 +1,154 @@
-﻿from typing import Union, Optional
-
-import numpy as np
-from matplotlib import colors as mcolors
-
-from gempy_engine.core.data.raw_arrays_solution import RawArraysSolution
-from gempy_viewer.core.scalar_data_type import ScalarDataType
-from gempy.core.data.grid_modules import RegularGrid, Topography
-from gempy_viewer.modules.plot_3d.vista import GemPyToVista
-from gempy_viewer.optional_dependencies import require_pyvista
-
-
-def plot_structured_grid(
-        gempy_vista: GemPyToVista,
-        regular_grid: RegularGrid,
-        scalar_data_type: ScalarDataType,
-        solution: RawArraysSolution,
-        cmap: Union[mcolors.Colormap or str],
-        active_scalar_field: Optional[str] = None,
-        opacity=.5,
-        **kwargs
-):
-    pv = require_pyvista()
-    structured_grid: pv.StructuredGrid | pv.PolyData = create_regular_mesh(gempy_vista, regular_grid)
-
-    # Set the scalar field-Activate it-getting cmap?
-    structured_grid = set_scalar_data(
-        structured_grid=structured_grid,
-        data=solution,
-        resolution = regular_grid.resolution,
-        scalar_data_type=scalar_data_type
-    )
-
-    structured_grid = set_active_scalar_fields(
-        structured_grid=structured_grid,
-        active_scalar_field=active_scalar_field
-    )
-    topography_polydata: pv.PolyData = gempy_vista.surface_poly.get('topography', None)
-    if topography_polydata is not None:
-        structured_grid = structured_grid.clip_surface(
-            surface=topography_polydata,
-            value=-10,
-            crinkle=False,
-            invert=True
-        )
-
-    add_regular_grid_mesh(
-        gempy_vista=gempy_vista,
-        structured_grid=structured_grid,
-        cmap=cmap,
-        opacity=opacity,  # BUG pass this as an argument
-        **kwargs
-    )
-
-
-def add_regular_grid_mesh(
-        gempy_vista: GemPyToVista,
-        structured_grid: 'pv.StructuredGrid',
-        cmap: Union[mcolors.Colormap or str],
-        opacity: float,
-        **kwargs
-):
-    if isinstance(cmap, mcolors.Colormap):
-        _clim = (0, cmap.N - 1)
-    else:
-        _clim = None
-    gempy_vista.regular_grid_actor = gempy_vista.p.add_mesh(
-        mesh=structured_grid,
-        cmap=cmap,
-        # ? scalars=main_scalar, if we prepare the structured grid do we need this arg?
-        show_scalar_bar=True,
-        scalar_bar_args=gempy_vista.scalar_bar_arguments,
-        interpolate_before_map=True,
-        opacity=opacity,
-        clim=_clim,
-        **kwargs
-    )
-
-
-def create_regular_mesh(gempy_vista: GemPyToVista, regular_grid: RegularGrid) -> "pv.StructuredGrid":
-    gempy_vista._grid_values = regular_grid.values
-
-    if False:
-        grid_3d = regular_grid.values.reshape(*regular_grid.resolution, 3).T
-        regular_grid_mesh = pv.StructuredGrid(*grid_3d)
-    else:
-        x = np.linspace(regular_grid.extent[0], regular_grid.extent[1], regular_grid.resolution[0] + 1)
-        y = np.linspace(regular_grid.extent[2], regular_grid.extent[3], regular_grid.resolution[1] + 1)
-        z = np.linspace(regular_grid.extent[4], regular_grid.extent[5], regular_grid.resolution[2] + 1)
-
-        x, y, z = np.meshgrid(x, y, z, indexing='ij')
-        pv = require_pyvista()
-        regular_grid_mesh = pv.StructuredGrid( x , y, z ) 
-    return regular_grid_mesh
-
-
-def _mask_topography(structured_grid: "pv.StructuredGrid", topography: Topography) -> "pv.StructuredGrid":
-    # ? Obsolete? I am using pyvista clipping and seems to do the job very good.
-    threshold = -100
-    structured_grid.active_scalars[topography.topography_mask.ravel(order='C')] = threshold - 1
-
-    # ? Is this messing up the data type?
-    pv = require_pyvista()
-    structured_grid: pv.StructuredGrid = structured_grid.threshold(
-        value=threshold,
-        method="upper"
-    )
-
-    return structured_grid
-
-
-def set_scalar_data(
-        data: RawArraysSolution,
-        structured_grid: "pv.StructuredGrid",
-        resolution: np.ndarray,
-        scalar_data_type: ScalarDataType,
-) -> "pv.StructuredGrid":
-    
-    def _convert_sol_array_to_fortran_order(array: np.ndarray) -> np.ndarray:
-        return array.reshape(*resolution, order='C').ravel(order='F')
-    # Substitute the madness of the previous if with match
-    match scalar_data_type:
-        case ScalarDataType.LITHOLOGY | ScalarDataType.ALL:
-            structured_grid.cell_data['id'] = _convert_sol_array_to_fortran_order(data.lith_block - 1)
-        case ScalarDataType.SCALAR_FIELD | ScalarDataType.ALL:
-            scalar_field_ = 'sf_'
-            for e in range(data.scalar_field_matrix.shape[0]):
-                # TODO: Ideally we will have the group name instead the enumeration
-                structured_grid[scalar_field_ + str(e)] = _convert_sol_array_to_fortran_order(data.scalar_field_matrix[e])
-        case ScalarDataType.VALUES | ScalarDataType.ALL:
-            scalar_field_ = 'values_'
-            for e in range(data.values_matrix.shape[0]):
-                structured_grid[scalar_field_ + str(e)] = _convert_sol_array_to_fortran_order(data.values_matrix[e])
-        case _:
-            raise ValueError(f'Unknown scalar data type: {scalar_data_type}')
-
-    return structured_grid  # , cmap
-
-
-def set_active_scalar_fields(structured_grid: "pv.StructuredGrid", active_scalar_field: Optional[str]) -> "pv.StructuredGrid":
-    if active_scalar_field is None:
-        active_scalar_field = structured_grid.array_names[0]
-
-    if active_scalar_field == 'lith':
-        active_scalar_field = 'id'
-
-    # Set the scalar field active
-    try:
-        structured_grid.set_active_scalars(active_scalar_field)
-    except ValueError:
-        raise AttributeError('The scalar field provided does not exist. Please pass '
-                             'a valid field: {}'.format(structured_grid.array_names))
-    return structured_grid
+﻿from typing import Union, Optional
+
+import numpy as np
+from matplotlib import colors as mcolors
+
+from gempy_engine.core.data.raw_arrays_solution import RawArraysSolution
+from gempy_viewer.core.scalar_data_type import ScalarDataType
+from gempy.core.data.grid_modules import RegularGrid, Topography
+from gempy_viewer.modules.plot_3d.vista import GemPyToVista
+from gempy_viewer.optional_dependencies import require_pyvista
+
+
+def plot_structured_grid(
+        gempy_vista: GemPyToVista,
+        regular_grid: RegularGrid,
+        scalar_data_type: ScalarDataType,
+        solution: RawArraysSolution,
+        cmap: Union[mcolors.Colormap or str],
+        active_scalar_field: Optional[str] = None,
+        opacity=.5,
+        **kwargs
+):
+    pv = require_pyvista()
+    structured_grid: "subsurface.core.structs.structured_elements.structured_grid.StructuredGrid" | pv.PolyData = create_regular_mesh(gempy_vista, regular_grid)
+
+    # Set the scalar field-Activate it-getting cmap?
+    structured_grid = set_scalar_data(
+        structured_grid=structured_grid,
+        data=solution,
+        resolution = regular_grid.resolution,
+        scalar_data_type=scalar_data_type
+    )
+
+    structured_grid = set_active_scalar_fields(
+        structured_grid=structured_grid,
+        active_scalar_field=active_scalar_field
+    )
+    topography_polydata: pv.PolyData = gempy_vista.surface_poly.get('topography', None)
+    if topography_polydata is not None:
+        structured_grid = structured_grid.clip_surface(
+            surface=topography_polydata,
+            value=-10,
+            crinkle=False,
+            invert=True
+        )
+
+    add_regular_grid_mesh(
+        gempy_vista=gempy_vista,
+        structured_grid=structured_grid,
+        cmap=cmap,
+        opacity=opacity,  # BUG pass this as an argument
+        **kwargs
+    )
+
+
+def add_regular_grid_mesh(
+        gempy_vista: GemPyToVista,
+        structured_grid: "pv.StructuredGrid",
+        cmap: Union[mcolors.Colormap or str],
+        opacity: float,
+        **kwargs
+):
+    if isinstance(cmap, mcolors.Colormap):
+        _clim = (0, cmap.N - 1)
+    else:
+        _clim = None
+    gempy_vista.regular_grid_actor = gempy_vista.p.add_mesh(
+        mesh=structured_grid,
+        cmap=cmap,
+        # ? scalars=main_scalar, if we prepare the structured grid do we need this arg?
+        show_scalar_bar=True,
+        scalar_bar_args=gempy_vista.scalar_bar_arguments,
+        interpolate_before_map=True,
+        opacity=opacity,
+        clim=_clim,
+        **kwargs
+    )
+
+
+def create_regular_mesh(gempy_vista: GemPyToVista, regular_grid: RegularGrid) -> "pv.StructuredGrid":
+    gempy_vista._grid_values = regular_grid.values
+
+    if False:
+        grid_3d = regular_grid.values.reshape(*regular_grid.resolution, 3).T
+        regular_grid_mesh = pv.StructuredGrid(*grid_3d)
+    else:
+        x = np.linspace(regular_grid.extent[0], regular_grid.extent[1], regular_grid.resolution[0] + 1)
+        y = np.linspace(regular_grid.extent[2], regular_grid.extent[3], regular_grid.resolution[1] + 1)
+        z = np.linspace(regular_grid.extent[4], regular_grid.extent[5], regular_grid.resolution[2] + 1)
+
+        x, y, z = np.meshgrid(x, y, z, indexing='ij')
+        pv = require_pyvista()
+        regular_grid_mesh = pv.StructuredGrid( x , y, z ) 
+    return regular_grid_mesh
+
+
+def _mask_topography(structured_grid: "pv.StructuredGrid", topography: Topography) -> "pv.StructuredGrid":
+    # ? Obsolete? I am using pyvista clipping and seems to do the job very good.
+    threshold = -100
+    structured_grid.active_scalars[topography.topography_mask.ravel(order='C')] = threshold - 1
+
+    # ? Is this messing up the data type?
+    pv = require_pyvista()
+    structured_grid: pv.StructuredGrid = structured_grid.threshold(
+        value=threshold,
+        method="upper"
+    )
+
+    return structured_grid
+
+
+def set_scalar_data(
+        data: RawArraysSolution,
+        structured_grid: "pv.StructuredGrid",
+        resolution: np.ndarray,
+        scalar_data_type: ScalarDataType,
+) -> "pv.StructuredGrid":
+    
+    def _convert_sol_array_to_fortran_order(array: np.ndarray) -> np.ndarray:
+        return array.reshape(*resolution, order='C').ravel(order='F')
+    # Substitute the madness of the previous if with match
+    match scalar_data_type:
+        case ScalarDataType.LITHOLOGY | ScalarDataType.ALL:
+            structured_grid.cell_data['id'] = _convert_sol_array_to_fortran_order(data.lith_block - 1)
+        case ScalarDataType.SCALAR_FIELD | ScalarDataType.ALL:
+            scalar_field_ = 'sf_'
+            for e in range(data.scalar_field_matrix.shape[0]):
+                # TODO: Ideally we will have the group name instead the enumeration
+                structured_grid[scalar_field_ + str(e)] = _convert_sol_array_to_fortran_order(data.scalar_field_matrix[e])
+        case ScalarDataType.VALUES | ScalarDataType.ALL:
+            scalar_field_ = 'values_'
+            for e in range(data.values_matrix.shape[0]):
+                structured_grid[scalar_field_ + str(e)] = _convert_sol_array_to_fortran_order(data.values_matrix[e])
+        case _:
+            raise ValueError(f'Unknown scalar data type: {scalar_data_type}')
+
+    return structured_grid  # , cmap
+
+
+def set_active_scalar_fields(structured_grid: "pv.StructuredGrid", active_scalar_field: Optional[str]) -> "pv.StructuredGrid":
+    if active_scalar_field is None:
+        active_scalar_field = structured_grid.array_names[0]
+
+    if active_scalar_field == 'lith':
+        active_scalar_field = 'id'
+
+    # Set the scalar field active
+    try:
+        structured_grid.set_active_scalars(active_scalar_field)
+    except ValueError:
+        raise AttributeError('The scalar field provided does not exist. Please pass '
+                             'a valid field: {}'.format(structured_grid.array_names))
+    return structured_grid
```

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/drawer_surfaces_3d.py` & `gempy_viewer-2024.1.4/gempy_viewer/modules/plot_3d/drawer_surfaces_3d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/drawer_topography_3d.py` & `gempy_viewer-2024.1.4/gempy_viewer/modules/plot_3d/drawer_topography_3d.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-﻿from typing import Optional
-
-import numpy as np
-import matplotlib.colors as mcolors
-
-from gempy.core.data.grid_modules import Topography
-from gempy_viewer.core.scalar_data_type import TopographyDataType
-from gempy_engine.core.data.raw_arrays_solution import RawArraysSolution
-from gempy_viewer.modules.plot_3d.vista import GemPyToVista
-from ...optional_dependencies import require_pyvista
-
-
-def plot_topography_3d(
-        gempy_vista: GemPyToVista,
-        topography: Topography,
-        solution: Optional[RawArraysSolution],
-        topography_scalar_type: TopographyDataType,
-        elements_colors: list[str],
-        contours=True,
-        **kwargs
-):
-    pv = require_pyvista()
-    
-    rgb = False
-
-    xx, yy = np.meshgrid(topography.y, topography.x)
-
-    grid = pv.StructuredGrid(yy, xx, topography.values_2d[:, :, 2])
-    polydata = grid.extract_surface()
-
-    if solution is None:
-        is_geological_map = False
-    else:
-        geological_map: np.array = solution.geological_map
-        is_geological_map = not(geological_map is None or geological_map.size == 0)
-    
-    match topography_scalar_type, is_geological_map:
-        case TopographyDataType.GEOMAP, True:
-            colors_hex = elements_colors
-            colors_rgb_ = [list(mcolors.hex2color(val)) for val in colors_hex]  # Convert hex to RGB using list comprehension
-
-            colors_rgb = np.array(colors_rgb_) * 255  # Multiply by 255 to get RGB values in [0, 255]
-            sel = np.round(geological_map).astype(int) - 1
-            selected_colors = colors_rgb[sel]  # Use numpy advanced indexing to get the corresponding RGB values
-            scalars_val = pv.convert_array(selected_colors, array_type=3)  # Convert to vtk array
-
-            cm = mcolors.ListedColormap(elements_colors)
-            rgb = True
-
-            show_scalar_bar = False
-            scalars = 'id'
-            clim = (0, len(elements_colors) - 1),
-
-        case TopographyDataType.SCALARS, True:
-            raise NotImplementedError('Not implemented yet')
-            clim = None
-        case _:  # * Plot topography 
-            scalars_val = topography.values[:, 2]
-            cm = 'terrain'
-            clim = None
-            show_scalar_bar = True
-            scalars = 'height'
-
-    polydata['id'] = scalars_val
-    polydata['height'] = topography.values[:, 2]
-
-    topography_actor = gempy_vista.p.add_mesh(
-        polydata,
-        scalars=scalars,
-        cmap=cm,
-        rgb=rgb,
-        show_scalar_bar=False,
-        clim= clim,
-        **kwargs
-    )
-
-    if contours is True:
-        contours = polydata.contour(scalars='height')
-        contours_actor = gempy_vista.p.add_mesh(contours, color="white", line_width=3)
-
-        gempy_vista.surface_poly['topography'] = polydata
-        gempy_vista.surface_poly['topography_cont'] = contours
-        gempy_vista.surface_actors["topography"] = topography_actor
-        gempy_vista.surface_actors["topography_cont"] = contours_actor
-    return topography_actor
+﻿from typing import Optional
+
+import numpy as np
+import matplotlib.colors as mcolors
+
+from gempy.core.data.grid_modules import Topography
+from gempy_viewer.core.scalar_data_type import TopographyDataType
+from gempy_engine.core.data.raw_arrays_solution import RawArraysSolution
+from gempy_viewer.modules.plot_3d.vista import GemPyToVista
+from ...optional_dependencies import require_pyvista
+
+
+def plot_topography_3d(
+        gempy_vista: GemPyToVista,
+        topography: Topography,
+        solution: Optional[RawArraysSolution],
+        topography_scalar_type: TopographyDataType,
+        elements_colors: list[str],
+        contours=True,
+        **kwargs
+):
+    pv = require_pyvista()
+    
+    rgb = False
+
+    xx, yy = np.meshgrid(topography.y, topography.x)
+
+    grid = pv.StructuredGrid(yy, xx, topography.values_2d[:, :, 2])
+    polydata = grid.extract_surface()
+
+    if solution is None:
+        is_geological_map = False
+    else:
+        geological_map: np.array = solution.geological_map
+        is_geological_map = not(geological_map is None or geological_map.size == 0)
+    
+    match topography_scalar_type, is_geological_map:
+        case TopographyDataType.GEOMAP, True:
+            colors_hex = elements_colors
+            colors_rgb_ = [list(mcolors.hex2color(val)) for val in colors_hex]  # Convert hex to RGB using list comprehension
+
+            colors_rgb = np.array(colors_rgb_) * 255  # Multiply by 255 to get RGB values in [0, 255]
+            sel = np.round(geological_map).astype(int) - 1
+            selected_colors = colors_rgb[sel]  # Use numpy advanced indexing to get the corresponding RGB values
+            scalars_val = pv.convert_array(selected_colors, array_type=3)  # Convert to vtk array
+
+            cm = mcolors.ListedColormap(elements_colors)
+            rgb = True
+
+            show_scalar_bar = False
+            scalars = 'id'
+            clim = (0, len(elements_colors) - 1),
+
+        case TopographyDataType.SCALARS, True:
+            raise NotImplementedError('Not implemented yet')
+            clim = None
+        case _:  # * Plot topography 
+            scalars_val = topography.values[:, 2]
+            cm = 'terrain'
+            clim = None
+            show_scalar_bar = True
+            scalars = 'height'
+
+    polydata['id'] = scalars_val
+    polydata['height'] = topography.values[:, 2]
+
+    topography_actor = gempy_vista.p.add_mesh(
+        polydata,
+        scalars=scalars,
+        cmap=cm,
+        rgb=rgb,
+        show_scalar_bar=False,
+        clim= clim,
+        **kwargs
+    )
+
+    if contours is True:
+        contours = polydata.contour(scalars='height')
+        contours_actor = gempy_vista.p.add_mesh(contours, color="white", line_width=3)
+
+        gempy_vista.surface_poly['topography'] = polydata
+        gempy_vista.surface_poly['topography_cont'] = contours
+        gempy_vista.surface_actors["topography"] = topography_actor
+        gempy_vista.surface_actors["topography_cont"] = contours_actor
+    return topography_actor
```

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/plot_3d_utils.py` & `gempy_viewer-2024.1.4/gempy_viewer/modules/plot_3d/plot_3d_utils.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/vista.py` & `gempy_viewer-2024.1.4/gempy_viewer/modules/plot_3d/vista.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/gempy_viewer/modules/plot_3d/vista_qt.py` & `gempy_viewer-2024.1.4/gempy_viewer/modules/plot_3d/vista_qt.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/gempy_viewer.egg-info/PKG-INFO` & `gempy_viewer-2024.1.4/gempy_viewer.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gempy_viewer
-Version: 2024.1.2
+Version: 2024.1.4
 Summary: Viewer for the geological modeling package GemPy
 Home-page: 
 Author: Miguel de la Varga
 Author-email: miguel@terranigma-solutions.com
 License: EUPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 License-File: LICENSE
 License-File: AUTHORS.rst
-Requires-Dist: gempy==2024.1.2
+Requires-Dist: gempy~=2024.1.4
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Provides-Extra: opt
 Requires-Dist: pyvista; extra == "opt"
 Requires-Dist: scipy; extra == "opt"
 Requires-Dist: pooch; extra == "opt"
 Requires-Dist: pandas; extra == "opt"
```

### Comparing `gempy_viewer-2024.1.2/gempy_viewer.egg-info/SOURCES.txt` & `gempy_viewer-2024.1.4/gempy_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/setup.py` & `gempy_viewer-2024.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/tests/conftest.py` & `gempy_viewer-2024.1.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2024.1.2/tests/test_plotting/test_plot_2d.py` & `gempy_viewer-2024.1.4/tests/test_plotting/test_plot_2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,16 +104,17 @@
 class TestPlot2DSolutions:
     @pytest.fixture(scope='class')
     def one_fault_model_topo_solution(self) -> gp.data.GeoModel:
         one_fault_model = _one_fault_model_generator()
 
         gp.set_section_grid(
             grid=one_fault_model.grid,
-            section_dict={'section_SW-NE': ([250, 250], [1750, 1750], [100, 100]),
-                          'section_NW-SE': ([250, 1750], [1750, 250], [100, 100])}
+            section_dict={'section_SW-NE': ([250, 250], [250, 1750], [50, 50]),
+                          'section_NW-SE': ([250, 1750], [1750, 250], [100, 100])
+                          }
         )
 
         gp.set_topography_from_random(
             grid=one_fault_model.grid,
             fractal_dimension=1.8,
             d_z=np.array([600, 2000]),
             topography_resolution=np.array([60, 60])
@@ -122,14 +123,22 @@
         gp.compute_model(one_fault_model)
         return one_fault_model
 
     def test_plot_2d_solutions_default(self, one_fault_model_topo_solution):
         print(one_fault_model_topo_solution.structural_frame)
         _: Plot2D = gpv.plot_2d(one_fault_model_topo_solution)
 
+    def test_plot_2d_section(self, one_fault_model_topo_solution):
+        _: Plot2D = gpv.plot_2d(
+            model=one_fault_model_topo_solution,
+            section_names=['section_SW-NE'],
+            show_boundaries=True,
+            show_topography=True
+        )
+
     def test_plot_2d_all_together(self, one_fault_model_topo_solution):
         gpv.plot_2d(
             model=one_fault_model_topo_solution,
             section_names=['section_SW-NE', 'section_NW-SE', 'topography'],
             direction=['x', 'y', 'y'], cell_number=['mid', 'mid', 'mid'],
             show_lith=[False, False, True, True, True, True],
             show_boundaries=[False, False, False, True, True, True],
@@ -137,28 +146,28 @@
             series_n=[0, 0, 0, 0, 0, 1],
             show_topography=True,
             show_section_traces=True  # TODO: Test this one
         )
 
     def test_ve(self, one_fault_model_topo_solution):
         # Test ve
-        p2d = gpv.plot_2d(one_fault_model_topo_solution, direction='x', cell_number='mid', 
+        p2d = gpv.plot_2d(one_fault_model_topo_solution, direction='x', cell_number='mid',
                           show_topography=True, ve=1)
 
         plt.show()
 
 
 class TestPlot2DSolutionsOctrees:
     @pytest.fixture(scope='class')
     def one_fault_model_topo_solution_octrees(self) -> gp.data.GeoModel:
         one_fault_model = _one_fault_model_generator()
         one_fault_model.grid.regular_grid.resolution = [2, 4, 2]
 
         one_fault_model.interpolation_options.number_octree_levels = 5
-        
+
         # TODO: Test octree regular grid with everything else combined
         gp.set_section_grid(
             grid=one_fault_model.grid,
             section_dict={'section_SW-NE': ([250, 250], [1750, 1750], [100, 100]),
                           'section_NW-SE': ([250, 1750], [1750, 250], [100, 100])}
         )
 
@@ -174,25 +183,24 @@
 
     def test_plot_2d_solutions_default(self, one_fault_model_topo_solution_octrees):
         print(one_fault_model_topo_solution_octrees.structural_frame)
         _: Plot2D = gpv.plot_2d(
             model=one_fault_model_topo_solution_octrees,
             show_boundaries=True
         )
-    
+
     def test_plot_2d_solutions_scalar(self, one_fault_model_topo_solution_octrees):
         print(one_fault_model_topo_solution_octrees.structural_frame)
         _: Plot2D = gpv.plot_2d(
             model=one_fault_model_topo_solution_octrees,
             show_boundaries=False,
             show_scalar=True,
             series_n=1
         )
-        
-        
+
     def test_plot_2d_all_together(self, one_fault_model_topo_solution_octrees):
         gpv.plot_2d(
             model=one_fault_model_topo_solution_octrees,
             section_names=['section_SW-NE', 'section_NW-SE', 'topography'],
             direction=['x', 'y', 'y'], cell_number=['mid', 'mid', 'mid'],
             show_lith=[False, False, False, True, True, True],
             show_boundaries=[False, False, False, True, True, True],
```

### Comparing `gempy_viewer-2024.1.2/tests/test_plotting/test_plot_3d.py` & `gempy_viewer-2024.1.4/tests/test_plotting/test_plot_3d.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,51 +6,55 @@
 from gempy.core.data import GeoModel
 from gempy_viewer.core.scalar_data_type import TopographyDataType
 from tests.conftest import _one_fault_model_generator
 
 
 class TestPlot3dInputData:
     def test_plot_3d_input_data(self, one_fault_model_no_interp):
-        gpv.plot_3d(one_fault_model_no_interp)
+        gpv.plot_3d(one_fault_model_no_interp, image=True)
 
 
 class TestPlot3DSolutions:
     def test_plot_3d_solutions_default(self, one_fault_model_topo_solution):
-        gpv.plot_3d(one_fault_model_topo_solution)
+        gpv.plot_3d(one_fault_model_topo_solution, image=True)
     
     def test_plot_3d_solutions(self, one_fault_model_topo_solution):
         gpv.plot_3d(
             model=one_fault_model_topo_solution,
             show_scalar=False,
             show_lith=True,
             show_data=True,
-            show_boundaries=True
+            show_boundaries=True,
+            image=True
         )
     
     def test_plot_3d_scalar_field(self, one_fault_model_topo_solution):
         gpv.plot_3d(
             model=one_fault_model_topo_solution,
             active_scalar_field="sf_1",
             show_scalar=True,
-            show_lith=False
+            show_lith=False,
+            image=True
         )
     
     def test_plot_3d_solutions_topography(self, one_fault_model_topo_solution):
         gpv.plot_3d(
             model=one_fault_model_topo_solution,
             show_topography=True,
-            topography_scalar_type=TopographyDataType.TOPOGRAPHY
+            topography_scalar_type=TopographyDataType.TOPOGRAPHY,
+            image=True
         )
     
     def test_plot_3d_solutions_topography_geological_map(self, one_fault_model_topo_solution):
         gpv.plot_3d(
             model=one_fault_model_topo_solution,
             show_lith=True,
             show_topography=True,
-            topography_scalar_type=TopographyDataType.GEOMAP
+            topography_scalar_type=TopographyDataType.GEOMAP,
+            image=True
         )
 
 
 class TestPlot2DSolutionsOctrees:
     @pytest.fixture(scope='class')
     def one_fault_model_topo_solution_octrees(self) -> GeoModel:
         one_fault_model = _one_fault_model_generator()
@@ -73,8 +77,8 @@
         )
 
         gp.compute_model(one_fault_model)
         return one_fault_model
 
 
     def test_plot_3d_solutions_default(self, one_fault_model_topo_solution_octrees):
-        gpv.plot_3d(one_fault_model_topo_solution_octrees)
+        gpv.plot_3d(one_fault_model_topo_solution_octrees, image=True)
```

