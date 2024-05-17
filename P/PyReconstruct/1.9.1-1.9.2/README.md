# Comparing `tmp/pyreconstruct-1.9.1.tar.gz` & `tmp/pyreconstruct-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreconstruct-1.9.1.tar", last modified: Tue May 14 17:02:51 2024, max compression
+gzip compressed data, was "pyreconstruct-1.9.2.tar", last modified: Fri May 17 11:13:56 2024, max compression
```

## Comparing `pyreconstruct-1.9.1.tar` & `pyreconstruct-1.9.2.tar`

### file list

```diff
@@ -1,232 +1,232 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.311980 pyreconstruct-1.9.1/
--rw-r--r--   0 michael   (1000) michael   (1000)     1832 2024-05-14 17:02:51.311980 pyreconstruct-1.9.1/PKG-INFO
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.291980 pyreconstruct-1.9.1/PyReconstruct/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-01-25 17:07:28.000000 pyreconstruct-1.9.1/PyReconstruct/__init__.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.291980 pyreconstruct-1.9.1/PyReconstruct/assets/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.291980 pyreconstruct-1.9.1/PyReconstruct/assets/checker/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.295313 pyreconstruct-1.9.1/PyReconstruct/assets/checker/files/
--rw-r--r--   0 michael   (1000) michael   (1000)   559712 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/checker/files/class_series.jser
--rw-r--r--   0 michael   (1000) michael   (1000)    36001 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/checker/files/shapes1.jser
--rw-r--r--   0 michael   (1000) michael   (1000)    41248 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/checker/files/shapes2.jser
--rw-r--r--   0 michael   (1000) michael   (1000)   236652 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/checker/files/shapes_0.tif
--rw-r--r--   0 michael   (1000) michael   (1000)   236356 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/checker/files/shapes_1.tif
--rw-r--r--   0 michael   (1000) michael   (1000)   236908 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/checker/files/shapes_2.tif
--rw-r--r--   0 michael   (1000) michael   (1000)   236294 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/checker/files/shapes_3.tif
--rw-r--r--   0 michael   (1000) michael   (1000)   237372 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/checker/files/shapes_4.tif
--rw-r--r--   0 michael   (1000) michael   (1000)       69 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/checker/files/tforms.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.298646 pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/
--rw-r--r--   0 michael   (1000) michael   (1000)   559712 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/class_series.jser
--rw-r--r--   0 michael   (1000) michael   (1000)     7171 2024-01-25 14:10:42.000000 pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/shapes1.0
--rw-r--r--   0 michael   (1000) michael   (1000)     6900 2024-01-25 14:10:42.000000 pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/shapes1.1
--rw-r--r--   0 michael   (1000) michael   (1000)     6404 2024-01-25 14:10:42.000000 pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/shapes1.2
--rw-r--r--   0 michael   (1000) michael   (1000)     6225 2024-01-25 14:10:42.000000 pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/shapes1.3
--rw-r--r--   0 michael   (1000) michael   (1000)     7508 2024-01-25 14:10:42.000000 pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/shapes1.4
--rw-r--r--   0 michael   (1000) michael   (1000)    36001 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/shapes1.jser
--rw-r--r--   0 michael   (1000) michael   (1000)    13226 2024-01-25 14:10:42.000000 pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/shapes1.ser
--rw-r--r--   0 michael   (1000) michael   (1000)    41248 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/shapes2.jser
--rw-r--r--   0 michael   (1000) michael   (1000)   236652 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/shapes_0.tif
--rw-r--r--   0 michael   (1000) michael   (1000)   236356 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/shapes_1.tif
--rw-r--r--   0 michael   (1000) michael   (1000)   236908 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/shapes_2.tif
--rw-r--r--   0 michael   (1000) michael   (1000)   236294 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/shapes_3.tif
--rw-r--r--   0 michael   (1000) michael   (1000)   237372 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/shapes_4.tif
--rw-r--r--   0 michael   (1000) michael   (1000)       69 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/tforms.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.301980 pyreconstruct-1.9.1/PyReconstruct/assets/img/
--rw-r--r--   0 michael   (1000) michael   (1000)    72939 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/img/PyReconstruct.ico
--rw-r--r--   0 michael   (1000) michael   (1000)     1385 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/img/brightness_down.png
--rw-r--r--   0 michael   (1000) michael   (1000)     1685 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/img/brightness_up.png
--rw-r--r--   0 michael   (1000) michael   (1000)      294 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/img/closedpoly.png
--rw-r--r--   0 michael   (1000) michael   (1000)      362 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/img/closedtrace.png
--rw-r--r--   0 michael   (1000) michael   (1000)      826 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/img/contrast_down.png
--rw-r--r--   0 michael   (1000) michael   (1000)     1412 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/img/contrast_up.png
--rw-r--r--   0 michael   (1000) michael   (1000)      333 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/img/grid.png
--rw-r--r--   0 michael   (1000) michael   (1000)      326 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/img/knife.cur
--rw-r--r--   0 michael   (1000) michael   (1000)      303 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/img/knife.png
--rw-r--r--   0 michael   (1000) michael   (1000)    68732 2023-12-21 13:14:00.000000 pyreconstruct-1.9.1/PyReconstruct/assets/img/logo.png
--rw-r--r--   0 michael   (1000) michael   (1000)   863379 2023-12-21 13:14:00.000000 pyreconstruct-1.9.1/PyReconstruct/assets/img/main_window.png
--rw-r--r--   0 michael   (1000) michael   (1000)      258 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/img/openpoly.png
--rw-r--r--   0 michael   (1000) michael   (1000)      356 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/img/opentrace.png
--rw-r--r--   0 michael   (1000) michael   (1000)      413 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/img/panzoom.png
--rw-r--r--   0 michael   (1000) michael   (1000)      326 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/img/pencil.cur
--rw-r--r--   0 michael   (1000) michael   (1000)      237 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/img/pointer.png
--rw-r--r--   0 michael   (1000) michael   (1000)      469 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/img/scissors.png
--rw-r--r--   0 michael   (1000) michael   (1000)      300 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/img/stamp.png
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.301980 pyreconstruct-1.9.1/PyReconstruct/assets/misc/
--rw-r--r--   0 michael   (1000) michael   (1000)     2419 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/misc/crop_zarr.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15417 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/misc/jser_to_zarr.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2389 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/misc/jser_to_zarr_v2.py
--rw-r--r--   0 michael   (1000) michael   (1000)      174 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/misc/tif_to_zarr.bat
--rw-r--r--   0 michael   (1000) michael   (1000)      896 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/misc/tif_to_zarr.py
--rw-r--r--   0 michael   (1000) michael   (1000)       95 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/misc/tif_to_zarr.sh
--rw-r--r--   0 michael   (1000) michael   (1000)     2957 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/misc/zarr_to_jser.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.291980 pyreconstruct-1.9.1/PyReconstruct/assets/scripts/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.301980 pyreconstruct-1.9.1/PyReconstruct/assets/scripts/__pycache__/
--rw-r--r--   0 michael   (1000) michael   (1000)      278 2024-04-19 19:52:40.000000 pyreconstruct-1.9.1/PyReconstruct/assets/scripts/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.301980 pyreconstruct-1.9.1/PyReconstruct/assets/scripts/convert_zarr/
--rw-r--r--   0 michael   (1000) michael   (1000)     2701 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/assets/scripts/convert_zarr/start_process.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2607 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/assets/scripts/convert_zarr/zarree-2.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.301980 pyreconstruct-1.9.1/PyReconstruct/assets/scripts/create_ng_zarr/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.301980 pyreconstruct-1.9.1/PyReconstruct/assets/scripts/create_ng_zarr/__pycache__/
--rw-r--r--   0 michael   (1000) michael   (1000)    10453 2024-05-14 08:02:28.000000 pyreconstruct-1.9.1/PyReconstruct/assets/scripts/create_ng_zarr/__pycache__/create_ng_zarr.cpython-311.pyc
--rw-r--r--   0 michael   (1000) michael   (1000)     7018 2024-05-11 06:46:07.000000 pyreconstruct-1.9.1/PyReconstruct/assets/scripts/create_ng_zarr/create_ng_zarr.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.301980 pyreconstruct-1.9.1/PyReconstruct/assets/scripts/create_ng_zarr/examples/
--rw-r--r--   0 michael   (1000) michael   (1000)       69 2023-12-14 13:39:22.000000 pyreconstruct-1.9.1/PyReconstruct/assets/scripts/create_ng_zarr/examples/create_ng_example.toml
--rw-r--r--   0 michael   (1000) michael   (1000)     1272 2023-12-13 09:59:52.000000 pyreconstruct-1.9.1/PyReconstruct/assets/scripts/create_ng_zarr/ng_view.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.301980 pyreconstruct-1.9.1/PyReconstruct/assets/scripts/export_traces/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.301980 pyreconstruct-1.9.1/PyReconstruct/assets/scripts/export_traces/__pycache__/
--rw-r--r--   0 michael   (1000) michael   (1000)     3616 2024-04-19 21:22:00.000000 pyreconstruct-1.9.1/PyReconstruct/assets/scripts/export_traces/__pycache__/export_traces_svg.cpython-311.pyc
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-19 19:29:24.000000 pyreconstruct-1.9.1/PyReconstruct/assets/scripts/export_traces/export_traces_svg.py.~1~
--rw-r--r--   0 michael   (1000) michael   (1000)      216 2024-04-19 19:35:54.000000 pyreconstruct-1.9.1/PyReconstruct/assets/scripts/export_traces/export_traces_svg.py.~2~
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.305313 pyreconstruct-1.9.1/PyReconstruct/assets/welcome_series/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.308647 pyreconstruct-1.9.1/PyReconstruct/assets/welcome_series/.welcome/
--rw-r--r--   0 michael   (1000) michael   (1000)      239 2024-01-05 10:19:04.000000 pyreconstruct-1.9.1/PyReconstruct/assets/welcome_series/.welcome/welcome.0
--rw-r--r--   0 michael   (1000) michael   (1000)        2 2024-05-14 15:45:39.000000 pyreconstruct-1.9.1/PyReconstruct/assets/welcome_series/.welcome/welcome.0.s0
--rw-r--r--   0 michael   (1000) michael   (1000)    10818 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/welcome_series/.welcome/welcome.ser
--rw-r--r--   0 michael   (1000) michael   (1000)  1364886 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/welcome_series/hold-welcome.tif
--rw-r--r--   0 michael   (1000) michael   (1000)  5562503 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/assets/welcome_series/welcome.png
--rw-r--r--   0 michael   (1000) michael   (1000)    17485 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/checker.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2414 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/cli.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.308647 pyreconstruct-1.9.1/PyReconstruct/modules/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/__init__.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.308647 pyreconstruct-1.9.1/PyReconstruct/modules/backend/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/__init__.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.308647 pyreconstruct-1.9.1/PyReconstruct/modules/backend/autoseg/
--rw-r--r--   0 michael   (1000) michael   (1000)       87 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/autoseg/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15448 2024-05-10 15:48:07.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/autoseg/conversions.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.308647 pyreconstruct-1.9.1/PyReconstruct/modules/backend/func/
--rw-r--r--   0 michael   (1000) michael   (1000)      216 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/func/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6512 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/func/import_swift_transforms.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2203 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/func/import_transforms.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5150 2024-01-13 22:28:04.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/func/scan_zarr.py
--rw-r--r--   0 michael   (1000) michael   (1000)    25151 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/func/state_manager.py
--rw-r--r--   0 michael   (1000) michael   (1000)    10794 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/func/xml_json_conversions.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.308647 pyreconstruct-1.9.1/PyReconstruct/modules/backend/table/
--rw-r--r--   0 michael   (1000) michael   (1000)      190 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/table/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5778 2024-01-13 22:28:04.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/table/flag.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9977 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/table/object.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9602 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/table/section.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5278 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/table/trace.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5501 2024-02-07 17:24:29.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/table/ztrace.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.308647 pyreconstruct-1.9.1/PyReconstruct/modules/backend/threading/
--rw-r--r--   0 michael   (1000) michael   (1000)       60 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/threading/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4073 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/threading/threading.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.308647 pyreconstruct-1.9.1/PyReconstruct/modules/backend/view/
--rw-r--r--   0 michael   (1000) michael   (1000)      155 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/view/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    41051 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/view/field_view.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15318 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/view/image_layer.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4860 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/view/optimize_bc.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2785 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/view/section_layer.py
--rw-r--r--   0 michael   (1000) michael   (1000)    32396 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/view/trace_layer.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9670 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/view/zarr_layer.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.308647 pyreconstruct-1.9.1/PyReconstruct/modules/backend/volume/
--rw-r--r--   0 michael   (1000) michael   (1000)      131 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/volume/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2406 2024-05-09 11:03:05.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/volume/export_volumes.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2753 2024-05-09 09:58:02.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/volume/generate_volumes.py
--rw-r--r--   0 michael   (1000) michael   (1000)    10592 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/backend/volume/objects_3D.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.308647 pyreconstruct-1.9.1/PyReconstruct/modules/calc/
--rw-r--r--   0 michael   (1000) michael   (1000)      419 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/calc/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    12499 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/calc/grid.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1803 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/calc/pfconversions.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6443 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/calc/quantification.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.308647 pyreconstruct-1.9.1/PyReconstruct/modules/constants/
--rw-r--r--   0 michael   (1000) michael   (1000)      556 2024-05-14 14:59:30.000000 pyreconstruct-1.9.1/PyReconstruct/modules/constants/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    11630 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/constants/blank_legacy_files.py
--rw-r--r--   0 michael   (1000) michael   (1000)      357 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/constants/developers.py
--rw-r--r--   0 michael   (1000) michael   (1000)      344 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/constants/getdatetime.py
--rw-r--r--   0 michael   (1000) michael   (1000)      944 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/constants/locations.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2203 2024-05-14 15:49:50.000000 pyreconstruct-1.9.1/PyReconstruct/modules/constants/repo_info.py
--rw-r--r--   0 michael   (1000) michael   (1000)      310 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/constants/websites.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.308647 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes/
--rw-r--r--   0 michael   (1000) michael   (1000)      336 2023-12-13 16:31:06.000000 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6025 2024-05-07 08:45:45.000000 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes/contour.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4134 2024-05-08 13:53:29.000000 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes/default_settings.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5103 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes/flag.py
--rw-r--r--   0 michael   (1000) michael   (1000)    16076 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes/log.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4448 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes/obj_group_dict.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5167 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes/objects.py
--rw-r--r--   0 michael   (1000) michael   (1000)    35567 2024-05-07 10:18:59.000000 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes/section.py
--rw-r--r--   0 michael   (1000) michael   (1000)    82207 2024-05-08 13:53:29.000000 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes/series.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15170 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes/series_data.py
--rw-r--r--   0 michael   (1000) michael   (1000)    18450 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes/trace.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4257 2024-02-08 07:28:43.000000 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes/transform.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9110 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes/ztrace.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.308647 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes_legacy/
--rw-r--r--   0 michael   (1000) michael   (1000)      423 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes_legacy/__init__.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.311980 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes_legacy/classes/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes_legacy/classes/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2868 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes_legacy/classes/contour.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1952 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes_legacy/classes/image.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2916 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes_legacy/classes/section.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5647 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes_legacy/classes/series.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6958 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes_legacy/classes/transform.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1262 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes_legacy/classes/zcontour.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.311980 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes_legacy/utils/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes_legacy/utils/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15214 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes_legacy/utils/reconstruct_reader.py
--rw-r--r--   0 michael   (1000) michael   (1000)    12177 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/datatypes_legacy/utils/reconstruct_writer.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.311980 pyreconstruct-1.9.1/PyReconstruct/modules/gui/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/__init__.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.311980 pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/
--rw-r--r--   0 michael   (1000) michael   (1000)      773 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5254 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/addto_zarr.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6783 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/alignment.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15491 2024-05-09 13:00:44.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/all_options.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6258 2024-05-08 13:53:29.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/backup.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2203 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/backup_comment.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6443 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/bc_profiles.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1288 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/color_button.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4029 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/create_zarr.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2138 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/file_dialog.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5122 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/flag.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3851 2024-01-13 22:28:04.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/grid.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5278 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/helper.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8413 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/import_traces.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2464 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/object_group.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6385 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/predict.py
--rw-r--r--   0 michael   (1000) michael   (1000)    16146 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/quick_dialog.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4993 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/segment.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1123 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/shape_button.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2789 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/shapes.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8576 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/shortcuts.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2628 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/swift_importer.py
--rw-r--r--   0 michael   (1000) michael   (1000)    10648 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/trace.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6456 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/trace_palette.py
--rw-r--r--   0 michael   (1000) michael   (1000)     7927 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/train.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.311980 pyreconstruct-1.9.1/PyReconstruct/modules/gui/main/
--rw-r--r--   0 michael   (1000) michael   (1000)       73 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/main/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    71828 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/main/field_widget.py
--rw-r--r--   0 michael   (1000) michael   (1000)   107676 2024-05-14 15:03:42.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/main/main_window.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.311980 pyreconstruct-1.9.1/PyReconstruct/modules/gui/palette/
--rw-r--r--   0 michael   (1000) michael   (1000)      154 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/palette/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5498 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/palette/buttons.py
--rw-r--r--   0 michael   (1000) michael   (1000)    29199 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/palette/mouse_palette.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2826 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/palette/outlined_label.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2410 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/palette/zarr_palette.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.311980 pyreconstruct-1.9.1/PyReconstruct/modules/gui/popup/
--rw-r--r--   0 michael   (1000) michael   (1000)      108 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/popup/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1420 2024-05-08 14:29:08.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/popup/about.py
--rw-r--r--   0 michael   (1000) michael   (1000)    13250 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/popup/custom_plotter.py
--rw-r--r--   0 michael   (1000) michael   (1000)      859 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/popup/text_widget.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.311980 pyreconstruct-1.9.1/PyReconstruct/modules/gui/table/
--rw-r--r--   0 michael   (1000) michael   (1000)      305 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/table/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1853 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/table/copy_table_widget.py
--rw-r--r--   0 michael   (1000) michael   (1000)    18081 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/table/flag.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4367 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/table/help3D.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2459 2023-12-06 10:36:25.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/table/history.py
--rw-r--r--   0 michael   (1000) michael   (1000)    41966 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/table/object.py
--rw-r--r--   0 michael   (1000) michael   (1000)    18013 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/table/section.py
--rw-r--r--   0 michael   (1000) michael   (1000)      614 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/table/str_helper.py
--rw-r--r--   0 michael   (1000) michael   (1000)    23750 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/table/trace.py
--rw-r--r--   0 michael   (1000) michael   (1000)    18108 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/table/ztrace.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.311980 pyreconstruct-1.9.1/PyReconstruct/modules/gui/utils/
--rw-r--r--   0 michael   (1000) michael   (1000)      307 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/utils/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9697 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/modules/gui/utils/utils.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1638 2024-05-03 08:40:01.000000 pyreconstruct-1.9.1/PyReconstruct/run.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-14 17:02:51.311980 pyreconstruct-1.9.1/PyReconstruct.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     1832 2024-05-14 17:02:51.000000 pyreconstruct-1.9.1/PyReconstruct.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     8908 2024-05-14 17:02:51.000000 pyreconstruct-1.9.1/PyReconstruct.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-05-14 17:02:51.000000 pyreconstruct-1.9.1/PyReconstruct.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       57 2024-05-14 17:02:51.000000 pyreconstruct-1.9.1/PyReconstruct.egg-info/entry_points.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-05-14 17:02:51.000000 pyreconstruct-1.9.1/PyReconstruct.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       14 2024-05-14 17:02:51.000000 pyreconstruct-1.9.1/PyReconstruct.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2024-05-14 17:02:51.311980 pyreconstruct-1.9.1/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     1239 2024-05-14 16:57:44.000000 pyreconstruct-1.9.1/setup.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.856810 pyreconstruct-1.9.2/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1832 2024-05-17 11:13:56.856810 pyreconstruct-1.9.2/PKG-INFO
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.810142 pyreconstruct-1.9.2/PyReconstruct/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-01-25 17:07:28.000000 pyreconstruct-1.9.2/PyReconstruct/__init__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.806809 pyreconstruct-1.9.2/PyReconstruct/assets/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.806809 pyreconstruct-1.9.2/PyReconstruct/assets/checker/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.816809 pyreconstruct-1.9.2/PyReconstruct/assets/checker/files/
+-rw-r--r--   0 michael   (1000) michael   (1000)   559712 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/checker/files/class_series.jser
+-rw-r--r--   0 michael   (1000) michael   (1000)    36001 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/checker/files/shapes1.jser
+-rw-r--r--   0 michael   (1000) michael   (1000)    41248 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/checker/files/shapes2.jser
+-rw-r--r--   0 michael   (1000) michael   (1000)   236652 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/checker/files/shapes_0.tif
+-rw-r--r--   0 michael   (1000) michael   (1000)   236356 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/checker/files/shapes_1.tif
+-rw-r--r--   0 michael   (1000) michael   (1000)   236908 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/checker/files/shapes_2.tif
+-rw-r--r--   0 michael   (1000) michael   (1000)   236294 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/checker/files/shapes_3.tif
+-rw-r--r--   0 michael   (1000) michael   (1000)   237372 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/checker/files/shapes_4.tif
+-rw-r--r--   0 michael   (1000) michael   (1000)       69 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/checker/files/tforms.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.826809 pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/
+-rw-r--r--   0 michael   (1000) michael   (1000)   559712 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/class_series.jser
+-rw-r--r--   0 michael   (1000) michael   (1000)     7171 2024-01-25 14:10:42.000000 pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/shapes1.0
+-rw-r--r--   0 michael   (1000) michael   (1000)     6900 2024-01-25 14:10:42.000000 pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/shapes1.1
+-rw-r--r--   0 michael   (1000) michael   (1000)     6404 2024-01-25 14:10:42.000000 pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/shapes1.2
+-rw-r--r--   0 michael   (1000) michael   (1000)     6225 2024-01-25 14:10:42.000000 pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/shapes1.3
+-rw-r--r--   0 michael   (1000) michael   (1000)     7508 2024-01-25 14:10:42.000000 pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/shapes1.4
+-rw-r--r--   0 michael   (1000) michael   (1000)    36001 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/shapes1.jser
+-rw-r--r--   0 michael   (1000) michael   (1000)    13226 2024-01-25 14:10:42.000000 pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/shapes1.ser
+-rw-r--r--   0 michael   (1000) michael   (1000)    41248 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/shapes2.jser
+-rw-r--r--   0 michael   (1000) michael   (1000)   236652 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/shapes_0.tif
+-rw-r--r--   0 michael   (1000) michael   (1000)   236356 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/shapes_1.tif
+-rw-r--r--   0 michael   (1000) michael   (1000)   236908 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/shapes_2.tif
+-rw-r--r--   0 michael   (1000) michael   (1000)   236294 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/shapes_3.tif
+-rw-r--r--   0 michael   (1000) michael   (1000)   237372 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/shapes_4.tif
+-rw-r--r--   0 michael   (1000) michael   (1000)       69 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/tforms.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.830143 pyreconstruct-1.9.2/PyReconstruct/assets/img/
+-rw-r--r--   0 michael   (1000) michael   (1000)    72939 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/img/PyReconstruct.ico
+-rw-r--r--   0 michael   (1000) michael   (1000)     1385 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/img/brightness_down.png
+-rw-r--r--   0 michael   (1000) michael   (1000)     1685 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/img/brightness_up.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      294 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/img/closedpoly.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      362 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/img/closedtrace.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      826 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/img/contrast_down.png
+-rw-r--r--   0 michael   (1000) michael   (1000)     1412 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/img/contrast_up.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      333 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/img/grid.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      326 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/img/knife.cur
+-rw-r--r--   0 michael   (1000) michael   (1000)      303 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/img/knife.png
+-rw-r--r--   0 michael   (1000) michael   (1000)    68732 2023-12-21 13:14:00.000000 pyreconstruct-1.9.2/PyReconstruct/assets/img/logo.png
+-rw-r--r--   0 michael   (1000) michael   (1000)   863379 2023-12-21 13:14:00.000000 pyreconstruct-1.9.2/PyReconstruct/assets/img/main_window.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      258 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/img/openpoly.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      356 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/img/opentrace.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      413 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/img/panzoom.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      326 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/img/pencil.cur
+-rw-r--r--   0 michael   (1000) michael   (1000)      237 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/img/pointer.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      469 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/img/scissors.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      300 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/img/stamp.png
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.830143 pyreconstruct-1.9.2/PyReconstruct/assets/misc/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2419 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/misc/crop_zarr.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15417 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/misc/jser_to_zarr.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2389 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/misc/jser_to_zarr_v2.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      174 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/misc/tif_to_zarr.bat
+-rw-r--r--   0 michael   (1000) michael   (1000)      896 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/misc/tif_to_zarr.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       95 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/misc/tif_to_zarr.sh
+-rw-r--r--   0 michael   (1000) michael   (1000)     2957 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/misc/zarr_to_jser.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.806809 pyreconstruct-1.9.2/PyReconstruct/assets/scripts/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.830143 pyreconstruct-1.9.2/PyReconstruct/assets/scripts/__pycache__/
+-rw-r--r--   0 michael   (1000) michael   (1000)      278 2024-04-19 19:52:40.000000 pyreconstruct-1.9.2/PyReconstruct/assets/scripts/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.830143 pyreconstruct-1.9.2/PyReconstruct/assets/scripts/convert_zarr/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2701 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/assets/scripts/convert_zarr/start_process.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2607 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/assets/scripts/convert_zarr/zarree-2.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.830143 pyreconstruct-1.9.2/PyReconstruct/assets/scripts/create_ng_zarr/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.830143 pyreconstruct-1.9.2/PyReconstruct/assets/scripts/create_ng_zarr/__pycache__/
+-rw-r--r--   0 michael   (1000) michael   (1000)    10453 2024-05-14 08:02:28.000000 pyreconstruct-1.9.2/PyReconstruct/assets/scripts/create_ng_zarr/__pycache__/create_ng_zarr.cpython-311.pyc
+-rw-r--r--   0 michael   (1000) michael   (1000)     7018 2024-05-11 06:46:07.000000 pyreconstruct-1.9.2/PyReconstruct/assets/scripts/create_ng_zarr/create_ng_zarr.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.830143 pyreconstruct-1.9.2/PyReconstruct/assets/scripts/create_ng_zarr/examples/
+-rw-r--r--   0 michael   (1000) michael   (1000)       69 2023-12-14 13:39:22.000000 pyreconstruct-1.9.2/PyReconstruct/assets/scripts/create_ng_zarr/examples/create_ng_example.toml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1272 2023-12-13 09:59:52.000000 pyreconstruct-1.9.2/PyReconstruct/assets/scripts/create_ng_zarr/ng_view.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.830143 pyreconstruct-1.9.2/PyReconstruct/assets/scripts/export_traces/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.830143 pyreconstruct-1.9.2/PyReconstruct/assets/scripts/export_traces/__pycache__/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3616 2024-04-19 21:22:00.000000 pyreconstruct-1.9.2/PyReconstruct/assets/scripts/export_traces/__pycache__/export_traces_svg.cpython-311.pyc
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-19 19:29:24.000000 pyreconstruct-1.9.2/PyReconstruct/assets/scripts/export_traces/export_traces_svg.py.~1~
+-rw-r--r--   0 michael   (1000) michael   (1000)      216 2024-04-19 19:35:54.000000 pyreconstruct-1.9.2/PyReconstruct/assets/scripts/export_traces/export_traces_svg.py.~2~
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.833476 pyreconstruct-1.9.2/PyReconstruct/assets/welcome_series/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.836809 pyreconstruct-1.9.2/PyReconstruct/assets/welcome_series/.welcome/
+-rw-r--r--   0 michael   (1000) michael   (1000)      239 2024-01-05 10:19:04.000000 pyreconstruct-1.9.2/PyReconstruct/assets/welcome_series/.welcome/welcome.0
+-rw-r--r--   0 michael   (1000) michael   (1000)        2 2024-05-16 13:45:02.000000 pyreconstruct-1.9.2/PyReconstruct/assets/welcome_series/.welcome/welcome.0.s0
+-rw-r--r--   0 michael   (1000) michael   (1000)    10818 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/welcome_series/.welcome/welcome.ser
+-rw-r--r--   0 michael   (1000) michael   (1000)  1364886 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/welcome_series/hold-welcome.tif
+-rw-r--r--   0 michael   (1000) michael   (1000)  5562503 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/assets/welcome_series/welcome.png
+-rw-r--r--   0 michael   (1000) michael   (1000)    17485 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/checker.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2414 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/cli.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.836809 pyreconstruct-1.9.2/PyReconstruct/modules/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/__init__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.836809 pyreconstruct-1.9.2/PyReconstruct/modules/backend/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/__init__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.836809 pyreconstruct-1.9.2/PyReconstruct/modules/backend/autoseg/
+-rw-r--r--   0 michael   (1000) michael   (1000)       87 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/autoseg/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15448 2024-05-10 15:48:07.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/autoseg/conversions.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.840143 pyreconstruct-1.9.2/PyReconstruct/modules/backend/func/
+-rw-r--r--   0 michael   (1000) michael   (1000)      216 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/func/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6512 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/func/import_swift_transforms.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2203 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/func/import_transforms.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5150 2024-01-13 22:28:04.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/func/scan_zarr.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    25151 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/func/state_manager.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    10794 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/func/xml_json_conversions.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.840143 pyreconstruct-1.9.2/PyReconstruct/modules/backend/table/
+-rw-r--r--   0 michael   (1000) michael   (1000)      190 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/table/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5778 2024-01-13 22:28:04.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/table/flag.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9977 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/table/object.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9602 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/table/section.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5278 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/table/trace.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5501 2024-02-07 17:24:29.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/table/ztrace.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.840143 pyreconstruct-1.9.2/PyReconstruct/modules/backend/threading/
+-rw-r--r--   0 michael   (1000) michael   (1000)       60 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/threading/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4073 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/threading/threading.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.840143 pyreconstruct-1.9.2/PyReconstruct/modules/backend/view/
+-rw-r--r--   0 michael   (1000) michael   (1000)      155 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/view/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    41051 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/view/field_view.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15318 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/view/image_layer.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4860 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/view/optimize_bc.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2785 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/view/section_layer.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    32396 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/view/trace_layer.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9670 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/view/zarr_layer.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.840143 pyreconstruct-1.9.2/PyReconstruct/modules/backend/volume/
+-rw-r--r--   0 michael   (1000) michael   (1000)      131 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/volume/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2406 2024-05-09 11:03:05.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/volume/export_volumes.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2753 2024-05-09 09:58:02.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/volume/generate_volumes.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    10592 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/backend/volume/objects_3D.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.843476 pyreconstruct-1.9.2/PyReconstruct/modules/calc/
+-rw-r--r--   0 michael   (1000) michael   (1000)      419 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/calc/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    12499 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/calc/grid.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1803 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/calc/pfconversions.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6443 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/calc/quantification.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.843476 pyreconstruct-1.9.2/PyReconstruct/modules/constants/
+-rw-r--r--   0 michael   (1000) michael   (1000)      556 2024-05-14 14:59:30.000000 pyreconstruct-1.9.2/PyReconstruct/modules/constants/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11630 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/constants/blank_legacy_files.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      357 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/constants/developers.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      344 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/constants/getdatetime.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      944 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/constants/locations.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2203 2024-05-14 15:49:50.000000 pyreconstruct-1.9.2/PyReconstruct/modules/constants/repo_info.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      310 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/constants/websites.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.846809 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes/
+-rw-r--r--   0 michael   (1000) michael   (1000)      336 2023-12-13 16:31:06.000000 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6025 2024-05-07 08:45:45.000000 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes/contour.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4134 2024-05-08 13:53:29.000000 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes/default_settings.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5103 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes/flag.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    16076 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes/log.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4448 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes/obj_group_dict.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5167 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes/objects.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    35567 2024-05-07 10:18:59.000000 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes/section.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    82216 2024-05-17 11:08:13.000000 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes/series.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15170 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes/series_data.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    18450 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes/trace.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4257 2024-02-08 07:28:43.000000 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes/transform.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9110 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes/ztrace.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.846809 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes_legacy/
+-rw-r--r--   0 michael   (1000) michael   (1000)      423 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes_legacy/__init__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.846809 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes_legacy/classes/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes_legacy/classes/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2868 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes_legacy/classes/contour.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1952 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes_legacy/classes/image.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2916 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes_legacy/classes/section.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5647 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes_legacy/classes/series.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6958 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes_legacy/classes/transform.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1262 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes_legacy/classes/zcontour.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.850143 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes_legacy/utils/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes_legacy/utils/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15214 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes_legacy/utils/reconstruct_reader.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    12177 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/datatypes_legacy/utils/reconstruct_writer.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.850143 pyreconstruct-1.9.2/PyReconstruct/modules/gui/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/__init__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.853476 pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/
+-rw-r--r--   0 michael   (1000) michael   (1000)      773 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5254 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/addto_zarr.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6783 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/alignment.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15491 2024-05-09 13:00:44.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/all_options.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6258 2024-05-08 13:53:29.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/backup.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2203 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/backup_comment.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6443 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/bc_profiles.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1288 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/color_button.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4029 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/create_zarr.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2138 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/file_dialog.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5122 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/flag.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3851 2024-01-13 22:28:04.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/grid.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5278 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/helper.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8413 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/import_traces.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2464 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/object_group.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6385 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/predict.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    16146 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/quick_dialog.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4993 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/segment.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1123 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/shape_button.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2789 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/shapes.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8576 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/shortcuts.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2628 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/swift_importer.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    10648 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/trace.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6456 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/trace_palette.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     7927 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/train.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.853476 pyreconstruct-1.9.2/PyReconstruct/modules/gui/main/
+-rw-r--r--   0 michael   (1000) michael   (1000)       73 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/main/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    71828 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/main/field_widget.py
+-rw-r--r--   0 michael   (1000) michael   (1000)   107676 2024-05-14 15:03:42.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/main/main_window.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.853476 pyreconstruct-1.9.2/PyReconstruct/modules/gui/palette/
+-rw-r--r--   0 michael   (1000) michael   (1000)      154 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/palette/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5498 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/palette/buttons.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29199 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/palette/mouse_palette.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2826 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/palette/outlined_label.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2410 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/palette/zarr_palette.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.853476 pyreconstruct-1.9.2/PyReconstruct/modules/gui/popup/
+-rw-r--r--   0 michael   (1000) michael   (1000)      108 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/popup/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1420 2024-05-08 14:29:08.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/popup/about.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    13250 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/popup/custom_plotter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      859 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/popup/text_widget.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.856810 pyreconstruct-1.9.2/PyReconstruct/modules/gui/table/
+-rw-r--r--   0 michael   (1000) michael   (1000)      305 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/table/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1853 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/table/copy_table_widget.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    18081 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/table/flag.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4367 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/table/help3D.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2459 2023-12-06 10:36:25.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/table/history.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    41966 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/table/object.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    18013 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/table/section.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      614 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/table/str_helper.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    23750 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/table/trace.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    18108 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/table/ztrace.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.856810 pyreconstruct-1.9.2/PyReconstruct/modules/gui/utils/
+-rw-r--r--   0 michael   (1000) michael   (1000)      307 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/utils/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9697 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/modules/gui/utils/utils.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1638 2024-05-03 08:40:01.000000 pyreconstruct-1.9.2/PyReconstruct/run.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 11:13:56.856810 pyreconstruct-1.9.2/PyReconstruct.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1832 2024-05-17 11:13:56.000000 pyreconstruct-1.9.2/PyReconstruct.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     8908 2024-05-17 11:13:56.000000 pyreconstruct-1.9.2/PyReconstruct.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-05-17 11:13:56.000000 pyreconstruct-1.9.2/PyReconstruct.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       57 2024-05-17 11:13:56.000000 pyreconstruct-1.9.2/PyReconstruct.egg-info/entry_points.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-05-17 11:13:56.000000 pyreconstruct-1.9.2/PyReconstruct.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       14 2024-05-17 11:13:56.000000 pyreconstruct-1.9.2/PyReconstruct.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2024-05-17 11:13:56.856810 pyreconstruct-1.9.2/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     1239 2024-05-17 11:08:13.000000 pyreconstruct-1.9.2/setup.py
```

### Comparing `pyreconstruct-1.9.1/PKG-INFO` & `pyreconstruct-1.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyReconstruct
-Version: 1.9.1
+Version: 1.9.2
 Summary: RECONSTRUCT written in Python
 Home-page: https://github.com/SynapseWeb/PyReconstruct
 Author: Julian Falco & Michael Chirillo
 Author-email: julian.falco@utexas.edu
 License: GNU GLPv3
 Description-Content-Type: text/markdown
 Requires-Dist: PySide6==6.5.2
```

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/checker/files/class_series.jser` & `pyreconstruct-1.9.2/PyReconstruct/assets/checker/files/class_series.jser`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/checker/files/shapes1.jser` & `pyreconstruct-1.9.2/PyReconstruct/assets/checker/files/shapes1.jser`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/checker/files/shapes2.jser` & `pyreconstruct-1.9.2/PyReconstruct/assets/checker/files/shapes2.jser`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/checker/files/shapes_0.tif` & `pyreconstruct-1.9.2/PyReconstruct/assets/checker/files/shapes_0.tif`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/checker/files/shapes_1.tif` & `pyreconstruct-1.9.2/PyReconstruct/assets/checker/files/shapes_1.tif`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/checker/files/shapes_2.tif` & `pyreconstruct-1.9.2/PyReconstruct/assets/checker/files/shapes_2.tif`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/checker/files/shapes_3.tif` & `pyreconstruct-1.9.2/PyReconstruct/assets/checker/files/shapes_3.tif`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/checker/files/shapes_4.tif` & `pyreconstruct-1.9.2/PyReconstruct/assets/checker/files/shapes_4.tif`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/class_series.jser` & `pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/class_series.jser`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/shapes1.0` & `pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/shapes1.0`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/shapes1.1` & `pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/shapes1.1`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/shapes1.2` & `pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/shapes1.2`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/shapes1.3` & `pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/shapes1.3`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/shapes1.4` & `pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/shapes1.4`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/shapes1.jser` & `pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/shapes1.jser`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/shapes1.ser` & `pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/shapes1.ser`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/shapes2.jser` & `pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/shapes2.jser`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/shapes_0.tif` & `pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/shapes_0.tif`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/shapes_1.tif` & `pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/shapes_1.tif`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/shapes_2.tif` & `pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/shapes_2.tif`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/shapes_3.tif` & `pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/shapes_3.tif`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/checker/testing/shapes_4.tif` & `pyreconstruct-1.9.2/PyReconstruct/assets/checker/testing/shapes_4.tif`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/img/PyReconstruct.ico` & `pyreconstruct-1.9.2/PyReconstruct/assets/img/PyReconstruct.ico`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/img/brightness_down.png` & `pyreconstruct-1.9.2/PyReconstruct/assets/img/brightness_down.png`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/img/brightness_up.png` & `pyreconstruct-1.9.2/PyReconstruct/assets/img/brightness_up.png`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/img/contrast_down.png` & `pyreconstruct-1.9.2/PyReconstruct/assets/img/contrast_down.png`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/img/contrast_up.png` & `pyreconstruct-1.9.2/PyReconstruct/assets/img/contrast_up.png`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/img/logo.png` & `pyreconstruct-1.9.2/PyReconstruct/assets/img/logo.png`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/img/main_window.png` & `pyreconstruct-1.9.2/PyReconstruct/assets/img/main_window.png`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/misc/crop_zarr.py` & `pyreconstruct-1.9.2/PyReconstruct/assets/misc/crop_zarr.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/misc/jser_to_zarr.py` & `pyreconstruct-1.9.2/PyReconstruct/assets/misc/jser_to_zarr.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/misc/jser_to_zarr_v2.py` & `pyreconstruct-1.9.2/PyReconstruct/assets/misc/jser_to_zarr_v2.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/misc/tif_to_zarr.py` & `pyreconstruct-1.9.2/PyReconstruct/assets/misc/tif_to_zarr.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/misc/zarr_to_jser.py` & `pyreconstruct-1.9.2/PyReconstruct/assets/misc/zarr_to_jser.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/scripts/convert_zarr/start_process.py` & `pyreconstruct-1.9.2/PyReconstruct/assets/scripts/convert_zarr/start_process.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/scripts/convert_zarr/zarree-2.py` & `pyreconstruct-1.9.2/PyReconstruct/assets/scripts/convert_zarr/zarree-2.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/scripts/create_ng_zarr/__pycache__/create_ng_zarr.cpython-311.pyc` & `pyreconstruct-1.9.2/PyReconstruct/assets/scripts/create_ng_zarr/__pycache__/create_ng_zarr.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/scripts/create_ng_zarr/create_ng_zarr.py` & `pyreconstruct-1.9.2/PyReconstruct/assets/scripts/create_ng_zarr/create_ng_zarr.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/scripts/create_ng_zarr/ng_view.py` & `pyreconstruct-1.9.2/PyReconstruct/assets/scripts/create_ng_zarr/ng_view.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/scripts/export_traces/__pycache__/export_traces_svg.cpython-311.pyc` & `pyreconstruct-1.9.2/PyReconstruct/assets/scripts/export_traces/__pycache__/export_traces_svg.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/welcome_series/.welcome/welcome.ser` & `pyreconstruct-1.9.2/PyReconstruct/assets/welcome_series/.welcome/welcome.ser`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/welcome_series/hold-welcome.tif` & `pyreconstruct-1.9.2/PyReconstruct/assets/welcome_series/hold-welcome.tif`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/assets/welcome_series/welcome.png` & `pyreconstruct-1.9.2/PyReconstruct/assets/welcome_series/welcome.png`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/checker.py` & `pyreconstruct-1.9.2/PyReconstruct/checker.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/cli.py` & `pyreconstruct-1.9.2/PyReconstruct/cli.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/backend/autoseg/conversions.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/backend/autoseg/conversions.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/backend/func/import_swift_transforms.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/backend/func/import_swift_transforms.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/backend/func/import_transforms.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/backend/func/import_transforms.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/backend/func/scan_zarr.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/backend/func/scan_zarr.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/backend/func/state_manager.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/backend/func/state_manager.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/backend/func/xml_json_conversions.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/backend/func/xml_json_conversions.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/backend/table/flag.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/backend/table/flag.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/backend/table/object.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/backend/table/object.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/backend/table/section.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/backend/table/section.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/backend/table/trace.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/backend/table/trace.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/backend/table/ztrace.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/backend/table/ztrace.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/backend/threading/threading.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/backend/threading/threading.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/backend/view/field_view.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/backend/view/field_view.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/backend/view/image_layer.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/backend/view/image_layer.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/backend/view/optimize_bc.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/backend/view/optimize_bc.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/backend/view/section_layer.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/backend/view/section_layer.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/backend/view/trace_layer.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/backend/view/trace_layer.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/backend/view/zarr_layer.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/backend/view/zarr_layer.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/backend/volume/export_volumes.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/backend/volume/export_volumes.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/backend/volume/generate_volumes.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/backend/volume/generate_volumes.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/backend/volume/objects_3D.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/backend/volume/objects_3D.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/calc/grid.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/calc/grid.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/calc/pfconversions.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/calc/pfconversions.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/calc/quantification.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/calc/quantification.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/constants/__init__.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/constants/blank_legacy_files.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/constants/blank_legacy_files.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/constants/locations.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/constants/locations.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/constants/repo_info.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/constants/repo_info.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/datatypes/contour.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/datatypes/contour.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/datatypes/default_settings.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/datatypes/default_settings.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/datatypes/flag.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/datatypes/flag.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/datatypes/log.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/datatypes/log.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/datatypes/obj_group_dict.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/datatypes/obj_group_dict.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/datatypes/objects.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/datatypes/objects.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/datatypes/section.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/datatypes/section.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/datatypes/series.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/datatypes/series.py`

 * *Files 0% similar despite different names*

```diff
@@ -998,15 +998,15 @@
                 section (list): the section numbers to modify the object on (default: all)
                 series_states: the series states as store in the GUI
                 log_event (bool): True if event should be logged
         """
         # preemptively create log
         if log_event:
             for obj_name in obj_names:
-                if obj_name != name:
+                if name and obj_name != name:
                     self.addLog(obj_name, None, f"Rename object to {name}")
                     self.addLog(name, None, f"Create trace(s) from {obj_name}")
                     # move object attrs
                     self.renameObjAttrs(obj_name, name)
                 else:
                     self.addLog(obj_name, None, "Modify object")
```

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/datatypes/series_data.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/datatypes/series_data.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/datatypes/trace.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/datatypes/trace.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/datatypes/transform.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/datatypes/transform.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/datatypes/ztrace.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/datatypes/ztrace.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/datatypes_legacy/classes/contour.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/datatypes_legacy/classes/contour.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/datatypes_legacy/classes/image.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/datatypes_legacy/classes/image.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/datatypes_legacy/classes/section.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/datatypes_legacy/classes/section.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/datatypes_legacy/classes/series.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/datatypes_legacy/classes/series.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/datatypes_legacy/classes/transform.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/datatypes_legacy/classes/transform.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/datatypes_legacy/classes/zcontour.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/datatypes_legacy/classes/zcontour.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/datatypes_legacy/utils/reconstruct_reader.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/datatypes_legacy/utils/reconstruct_reader.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/datatypes_legacy/utils/reconstruct_writer.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/datatypes_legacy/utils/reconstruct_writer.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/__init__.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/addto_zarr.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/addto_zarr.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/alignment.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/alignment.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/all_options.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/all_options.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/backup.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/backup.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/backup_comment.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/backup_comment.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/bc_profiles.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/bc_profiles.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/color_button.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/color_button.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/create_zarr.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/create_zarr.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/file_dialog.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/file_dialog.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/flag.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/flag.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/grid.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/grid.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/helper.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/helper.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/import_traces.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/import_traces.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/object_group.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/object_group.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/predict.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/predict.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/quick_dialog.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/quick_dialog.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/segment.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/segment.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/shape_button.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/shape_button.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/shapes.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/shapes.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/shortcuts.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/shortcuts.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/swift_importer.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/swift_importer.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/trace.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/trace.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/trace_palette.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/trace_palette.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/dialog/train.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/dialog/train.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/main/field_widget.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/main/field_widget.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/main/main_window.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/main/main_window.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/palette/buttons.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/palette/buttons.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/palette/mouse_palette.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/palette/mouse_palette.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/palette/outlined_label.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/palette/outlined_label.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/palette/zarr_palette.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/palette/zarr_palette.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/popup/about.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/popup/about.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/popup/custom_plotter.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/popup/custom_plotter.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/popup/text_widget.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/popup/text_widget.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/table/copy_table_widget.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/table/copy_table_widget.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/table/flag.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/table/flag.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/table/help3D.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/table/help3D.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/table/history.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/table/history.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/table/object.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/table/object.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/table/section.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/table/section.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/table/str_helper.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/table/str_helper.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/table/trace.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/table/trace.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/table/ztrace.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/table/ztrace.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/modules/gui/utils/utils.py` & `pyreconstruct-1.9.2/PyReconstruct/modules/gui/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct/run.py` & `pyreconstruct-1.9.2/PyReconstruct/run.py`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/PyReconstruct.egg-info/PKG-INFO` & `pyreconstruct-1.9.2/PyReconstruct.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyReconstruct
-Version: 1.9.1
+Version: 1.9.2
 Summary: RECONSTRUCT written in Python
 Home-page: https://github.com/SynapseWeb/PyReconstruct
 Author: Julian Falco & Michael Chirillo
 Author-email: julian.falco@utexas.edu
 License: GNU GLPv3
 Description-Content-Type: text/markdown
 Requires-Dist: PySide6==6.5.2
```

### Comparing `pyreconstruct-1.9.1/PyReconstruct.egg-info/SOURCES.txt` & `pyreconstruct-1.9.2/PyReconstruct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyreconstruct-1.9.1/setup.py` & `pyreconstruct-1.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import setup, find_packages
 
 ROOT = pathlib.Path(__file__).parent
 
-VERSION = '1.9.1'
+VERSION = '1.9.2'
 PACKAGE_NAME = 'PyReconstruct'
 AUTHOR = 'Julian Falco & Michael Chirillo'
 AUTHOR_EMAIL = 'julian.falco@utexas.edu'
 URL = 'https://github.com/SynapseWeb/PyReconstruct'
 LICENSE = 'GNU GLPv3'
 DESCRIPTION = 'RECONSTRUCT written in Python'
```

