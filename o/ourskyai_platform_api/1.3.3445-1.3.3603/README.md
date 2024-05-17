# Comparing `tmp/ourskyai_platform_api-1.3.3445.tar.gz` & `tmp/ourskyai_platform_api-1.3.3603.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourskyai_platform_api-1.3.3445.tar", max compression
+gzip compressed data, was "ourskyai_platform_api-1.3.3603.tar", max compression
```

## Comparing `ourskyai_platform_api-1.3.3445.tar` & `ourskyai_platform_api-1.3.3603.tar`

### file list

```diff
@@ -1,72 +1,75 @@
--rw-r--r--   0        0        0     9332 2024-04-25 01:25:01.703317 ourskyai_platform_api-1.3.3445/README.md
--rw-r--r--   0        0        0     6036 2024-04-25 01:25:05.399339 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/__init__.py
--rw-r--r--   0        0        0      109 2024-04-25 01:25:05.439339 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/api/__init__.py
--rw-r--r--   0        0        0   192993 2024-04-25 01:25:05.523340 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/api/default_api.py
--rw-r--r--   0        0        0    30373 2024-04-25 01:25:05.575340 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/api_client.py
--rw-r--r--   0        0        0      852 2024-04-25 01:25:05.627341 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/api_response.py
--rw-r--r--   0        0        0    14693 2024-04-25 01:25:05.739341 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/configuration.py
--rw-r--r--   0        0        0     5436 2024-04-25 01:25:05.791342 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/exceptions.py
--rw-r--r--   0        0        0     5365 2024-04-25 01:25:05.867342 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/__init__.py
--rw-r--r--   0        0        0      745 2024-04-25 01:25:05.919342 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/camera_mode.py
--rw-r--r--   0        0        0     1907 2024-04-25 01:25:05.975343 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/empty_success.py
--rw-r--r--   0        0        0     1189 2024-04-25 01:25:06.019343 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/filter_type.py
--rw-r--r--   0        0        0     2158 2024-04-25 01:25:06.075343 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/location.py
--rw-r--r--   0        0        0      777 2024-04-25 01:25:06.119344 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/metric_type.py
--rw-r--r--   0        0        0      750 2024-04-25 01:25:06.171344 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/mount_type.py
--rw-r--r--   0        0        0      890 2024-04-25 01:25:06.243344 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/node_state.py
--rw-r--r--   0        0        0      830 2024-04-25 01:25:06.303345 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/optical_tube_type.py
--rw-r--r--   0        0        0     2407 2024-04-25 01:25:06.355345 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/plate_solve_parameters.py
--rw-r--r--   0        0        0      754 2024-04-25 01:25:06.391345 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/shutter_type.py
--rw-r--r--   0        0        0     1895 2024-04-25 01:25:06.435346 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/successful_create.py
--rw-r--r--   0        0        0      771 2024-04-25 01:25:06.479346 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/tracking_type.py
--rw-r--r--   0        0        0     4920 2024-04-25 01:25:06.555346 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_camera.py
--rw-r--r--   0        0        0     2115 2024-04-25 01:25:06.591347 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_client_token.py
--rw-r--r--   0        0        0     2047 2024-04-25 01:25:06.635347 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_complete_observation_request.py
--rw-r--r--   0        0        0     2047 2024-04-25 01:25:06.667347 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_create_image_set_image_request.py
--rw-r--r--   0        0        0     2118 2024-04-25 01:25:06.719347 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_create_image_set_image_response.py
--rw-r--r--   0        0        0     2692 2024-04-25 01:25:06.775348 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_create_image_set_request.py
--rw-r--r--   0        0        0     2302 2024-04-25 01:25:06.851348 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_create_mount_request.py
--rw-r--r--   0        0        0     2710 2024-04-25 01:25:06.903349 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_create_node_diagnostic.py
--rw-r--r--   0        0        0     2715 2024-04-25 01:25:06.947349 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py
--rw-r--r--   0        0        0     3152 2024-04-25 01:25:06.995349 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_create_node_request.py
--rw-r--r--   0        0        0     2453 2024-04-25 01:25:07.055349 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_create_optical_tube_request.py
--rw-r--r--   0        0        0     2124 2024-04-25 01:25:07.135350 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_diagnostic_instruction.py
--rw-r--r--   0        0        0     2444 2024-04-25 01:25:07.171350 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_elevation_mask_point.py
--rw-r--r--   0        0        0     3298 2024-04-25 01:25:07.247351 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_gain_curve.py
--rw-r--r--   0        0        0     2054 2024-04-25 01:25:07.295351 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_gain_curve_point.py
--rw-r--r--   0        0        0     2570 2024-04-25 01:25:07.351351 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_get_instruction_request.py
--rw-r--r--   0        0        0     2370 2024-04-25 01:25:07.391351 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_get_nodes.py
--rw-r--r--   0        0        0     7081 2024-04-25 01:25:07.435352 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_get_or_create_camera_request.py
--rw-r--r--   0        0        0     2330 2024-04-25 01:25:07.483352 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_get_or_create_mount_request.py
--rw-r--r--   0        0        0     2519 2024-04-25 01:25:07.531352 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py
--rw-r--r--   0        0        0     2902 2024-04-25 01:25:07.579352 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py
--rw-r--r--   0        0        0     3985 2024-04-25 01:25:07.627353 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_ground_station_participant.py
--rw-r--r--   0        0        0     3445 2024-04-25 01:25:07.667353 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_image_set.py
--rw-r--r--   0        0        0     5170 2024-04-25 01:25:07.711353 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_image_set_image.py
--rw-r--r--   0        0        0     3305 2024-04-25 01:25:07.755354 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_instruction.py
--rw-r--r--   0        0        0     2400 2024-04-25 01:25:07.803354 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_metric.py
--rw-r--r--   0        0        0     1917 2024-04-25 01:25:07.871354 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_mount.py
--rw-r--r--   0        0        0     4470 2024-04-25 01:25:07.931355 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_node.py
--rw-r--r--   0        0        0      850 2024-04-25 01:25:07.975355 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_node_component_type.py
--rw-r--r--   0        0        0     1595 2024-04-25 01:25:08.023355 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_node_diagnostic_type.py
--rw-r--r--   0        0        0     2573 2024-04-25 01:25:08.079356 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_node_with_location.py
--rw-r--r--   0        0        0     5537 2024-04-25 01:25:08.127356 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_observation_instruction.py
--rw-r--r--   0        0        0     2242 2024-04-25 01:25:08.175356 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_optical_tube.py
--rw-r--r--   0        0        0     2135 2024-04-25 01:25:08.227357 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py
--rw-r--r--   0        0        0     2273 2024-04-25 01:25:08.279357 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py
--rw-r--r--   0        0        0      870 2024-04-25 01:25:08.323357 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_plate_solve_catalog_identifier.py
--rw-r--r--   0        0        0     2054 2024-04-25 01:25:08.367357 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_read_noise_point.py
--rw-r--r--   0        0        0     2053 2024-04-25 01:25:08.403358 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_setup_action.py
--rw-r--r--   0        0        0     2946 2024-04-25 01:25:08.443358 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_slew_timing.py
--rw-r--r--   0        0        0     2243 2024-04-25 01:25:08.495358 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_slew_timing_interval.py
--rw-r--r--   0        0        0     3601 2024-04-25 01:25:08.547359 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_update_node_components_request.py
--rw-r--r--   0        0        0     6269 2024-04-25 01:25:08.595359 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_update_node_components_request_camera.py
--rw-r--r--   0        0        0     2402 2024-04-25 01:25:08.635359 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_update_node_components_request_mount.py
--rw-r--r--   0        0        0     2591 2024-04-25 01:25:08.687359 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py
--rw-r--r--   0        0        0     4620 2024-04-25 01:25:08.739360 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_update_node_request.py
--rw-r--r--   0        0        0     2525 2024-04-25 01:25:08.791360 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_video_mode_framerate_property.py
--rw-r--r--   0        0        0     2224 2024-04-25 01:25:08.827360 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v2_complete_observation_request.py
--rw-r--r--   0        0        0        0 2024-04-25 01:25:08.859360 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/py.typed
--rw-r--r--   0        0        0    12941 2024-04-25 01:25:08.907361 ourskyai_platform_api-1.3.3445/ourskyai_platform_api/rest.py
--rw-r--r--   0        0        0      751 2024-04-25 01:25:08.947361 ourskyai_platform_api-1.3.3445/pyproject.toml
--rw-r--r--   0        0        0    10309 1970-01-01 00:00:00.000000 ourskyai_platform_api-1.3.3445/PKG-INFO
+-rw-r--r--   0        0        0     9625 2024-05-17 19:15:26.351834 ourskyai_platform_api-1.3.3603/README.md
+-rw-r--r--   0        0        0     6272 2024-05-17 19:15:30.007971 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/__init__.py
+-rw-r--r--   0        0        0      109 2024-05-17 19:15:30.039972 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/api/__init__.py
+-rw-r--r--   0        0        0   199259 2024-05-17 19:15:30.135976 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/api/default_api.py
+-rw-r--r--   0        0        0    30373 2024-05-17 19:15:30.207979 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/api_client.py
+-rw-r--r--   0        0        0      852 2024-05-17 19:15:30.263980 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/api_response.py
+-rw-r--r--   0        0        0    14693 2024-05-17 19:15:30.319983 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/configuration.py
+-rw-r--r--   0        0        0     5436 2024-05-17 19:15:30.355984 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/exceptions.py
+-rw-r--r--   0        0        0     5601 2024-05-17 19:15:30.411986 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/__init__.py
+-rw-r--r--   0        0        0      745 2024-05-17 19:15:30.487989 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/camera_mode.py
+-rw-r--r--   0        0        0     1907 2024-05-17 19:15:30.531991 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/empty_success.py
+-rw-r--r--   0        0        0     1189 2024-05-17 19:15:30.571992 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/filter_type.py
+-rw-r--r--   0        0        0     2158 2024-05-17 19:15:30.611994 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/location.py
+-rw-r--r--   0        0        0      777 2024-05-17 19:15:30.659995 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/metric_type.py
+-rw-r--r--   0        0        0      750 2024-05-17 19:15:30.715998 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/mount_type.py
+-rw-r--r--   0        0        0      890 2024-05-17 19:15:30.751999 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/node_state.py
+-rw-r--r--   0        0        0      830 2024-05-17 19:15:30.800001 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/optical_tube_type.py
+-rw-r--r--   0        0        0     2407 2024-05-17 19:15:30.852003 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/plate_solve_parameters.py
+-rw-r--r--   0        0        0      754 2024-05-17 19:15:30.904005 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/shutter_type.py
+-rw-r--r--   0        0        0     1895 2024-05-17 19:15:30.968007 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/successful_create.py
+-rw-r--r--   0        0        0      771 2024-05-17 19:15:31.000008 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/tracking_type.py
+-rw-r--r--   0        0        0     2622 2024-05-17 19:15:31.048010 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_auto_focus_instruction.py
+-rw-r--r--   0        0        0     2366 2024-05-17 19:15:31.116013 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py
+-rw-r--r--   0        0        0     4920 2024-05-17 19:15:31.180015 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_camera.py
+-rw-r--r--   0        0        0     2115 2024-05-17 19:15:31.228017 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_client_token.py
+-rw-r--r--   0        0        0     2047 2024-05-17 19:15:31.288019 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_complete_observation_request.py
+-rw-r--r--   0        0        0     2047 2024-05-17 19:15:31.348021 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_image_set_image_request.py
+-rw-r--r--   0        0        0     2118 2024-05-17 19:15:31.404024 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_image_set_image_response.py
+-rw-r--r--   0        0        0     2692 2024-05-17 19:15:31.448025 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_image_set_request.py
+-rw-r--r--   0        0        0     2302 2024-05-17 19:15:31.512028 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_mount_request.py
+-rw-r--r--   0        0        0     2710 2024-05-17 19:15:31.548029 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_node_diagnostic.py
+-rw-r--r--   0        0        0     2715 2024-05-17 19:15:31.604031 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py
+-rw-r--r--   0        0        0     3152 2024-05-17 19:15:31.644033 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_node_request.py
+-rw-r--r--   0        0        0     2453 2024-05-17 19:15:31.692034 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2124 2024-05-17 19:15:31.732036 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_diagnostic_instruction.py
+-rw-r--r--   0        0        0     2444 2024-05-17 19:15:31.804039 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_elevation_mask_point.py
+-rw-r--r--   0        0        0      719 2024-05-17 19:15:31.896042 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_file_type.py
+-rw-r--r--   0        0        0     3298 2024-05-17 19:15:31.944044 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_gain_curve.py
+-rw-r--r--   0        0        0     2054 2024-05-17 19:15:31.988046 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_gain_curve_point.py
+-rw-r--r--   0        0        0     2570 2024-05-17 19:15:32.064048 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_get_instruction_request.py
+-rw-r--r--   0        0        0     2370 2024-05-17 19:15:32.120051 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_get_nodes.py
+-rw-r--r--   0        0        0     7081 2024-05-17 19:15:32.164052 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_get_or_create_camera_request.py
+-rw-r--r--   0        0        0     2330 2024-05-17 19:15:32.248055 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_get_or_create_mount_request.py
+-rw-r--r--   0        0        0     2519 2024-05-17 19:15:32.308057 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2675 2024-05-17 19:15:32.380060 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py
+-rw-r--r--   0        0        0     3985 2024-05-17 19:15:32.476064 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_ground_station_participant.py
+-rw-r--r--   0        0        0     3445 2024-05-17 19:15:32.516065 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_image_set.py
+-rw-r--r--   0        0        0     5170 2024-05-17 19:15:32.552067 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_image_set_image.py
+-rw-r--r--   0        0        0     3763 2024-05-17 19:15:32.612069 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_instruction.py
+-rw-r--r--   0        0        0     2400 2024-05-17 19:15:32.656071 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_metric.py
+-rw-r--r--   0        0        0     1917 2024-05-17 19:15:32.716073 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_mount.py
+-rw-r--r--   0        0        0     4470 2024-05-17 19:15:32.780075 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_node.py
+-rw-r--r--   0        0        0      850 2024-05-17 19:15:32.812076 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_node_component_type.py
+-rw-r--r--   0        0        0     1655 2024-05-17 19:15:32.876079 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_node_diagnostic_type.py
+-rw-r--r--   0        0        0     2573 2024-05-17 19:15:32.932081 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_node_with_location.py
+-rw-r--r--   0        0        0     5537 2024-05-17 19:15:32.980083 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_observation_instruction.py
+-rw-r--r--   0        0        0     2242 2024-05-17 19:15:33.024084 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_optical_tube.py
+-rw-r--r--   0        0        0     2135 2024-05-17 19:15:33.072086 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py
+-rw-r--r--   0        0        0     2648 2024-05-17 19:15:33.112088 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py
+-rw-r--r--   0        0        0     2054 2024-05-17 19:15:33.168090 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_read_noise_point.py
+-rw-r--r--   0        0        0     2401 2024-05-17 19:15:33.216092 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_release.py
+-rw-r--r--   0        0        0     2053 2024-05-17 19:15:33.268094 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_setup_action.py
+-rw-r--r--   0        0        0     2946 2024-05-17 19:15:33.316095 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_slew_timing.py
+-rw-r--r--   0        0        0     2243 2024-05-17 19:15:33.364097 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_slew_timing_interval.py
+-rw-r--r--   0        0        0     3601 2024-05-17 19:15:33.420099 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_update_node_components_request.py
+-rw-r--r--   0        0        0     6269 2024-05-17 19:15:33.484102 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_update_node_components_request_camera.py
+-rw-r--r--   0        0        0     2402 2024-05-17 19:15:33.532104 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_update_node_components_request_mount.py
+-rw-r--r--   0        0        0     2591 2024-05-17 19:15:33.580105 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py
+-rw-r--r--   0        0        0     4620 2024-05-17 19:15:33.648108 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_update_node_request.py
+-rw-r--r--   0        0        0     2525 2024-05-17 19:15:33.696110 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_video_mode_framerate_property.py
+-rw-r--r--   0        0        0     2224 2024-05-17 19:15:33.768113 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v2_complete_observation_request.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:15:33.804114 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/py.typed
+-rw-r--r--   0        0        0    12941 2024-05-17 19:15:33.860116 ourskyai_platform_api-1.3.3603/ourskyai_platform_api/rest.py
+-rw-r--r--   0        0        0      751 2024-05-17 19:15:33.912118 ourskyai_platform_api-1.3.3603/pyproject.toml
+-rw-r--r--   0        0        0    10602 1970-01-01 00:00:00.000000 ourskyai_platform_api-1.3.3603/PKG-INFO
```

### Comparing `ourskyai_platform_api-1.3.3445/README.md` & `ourskyai_platform_api-1.3.3603/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,39 @@
+Metadata-Version: 2.1
+Name: ourskyai_platform_api
+Version: 1.3.3603
+Summary: OurSky Platform
+Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
+License: NoLicense
+Keywords: OpenAPI,OpenAPI-Generator,OurSky Platform
+Author: OpenAPI Generator Community
+Author-email: team@openapitools.org
+Requires-Python: >=3.7,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aenum (>=3.1.11)
+Requires-Dist: pydantic (>=1.10.5,<2.0.0)
+Requires-Dist: python-dateutil (>=2.8.2)
+Requires-Dist: urllib3 (>=1.25.3)
+Project-URL: Repository, https://github.com/GIT_USER_ID/GIT_REPO_ID
+Description-Content-Type: text/markdown
+
 # ourskyai-platform-api
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3445
-- Package version: 1.3.3445
+- API version: 1.3.3603
+- Package version: 1.3.3603
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
@@ -94,14 +119,15 @@
 *DefaultApi* | [**v1_delete_image_set**](docs/DefaultApi.md#v1_delete_image_set) | **DELETE** /v1/image-set | 
 *DefaultApi* | [**v1_delete_image_set_image**](docs/DefaultApi.md#v1_delete_image_set_image) | **DELETE** /v1/image-set-image | 
 *DefaultApi* | [**v1_get_cameras**](docs/DefaultApi.md#v1_get_cameras) | **GET** /v1/cameras | 
 *DefaultApi* | [**v1_get_image_set**](docs/DefaultApi.md#v1_get_image_set) | **GET** /v1/image-set | 
 *DefaultApi* | [**v1_get_image_set_image**](docs/DefaultApi.md#v1_get_image_set_image) | **GET** /v1/image-set-image | 
 *DefaultApi* | [**v1_get_instruction**](docs/DefaultApi.md#v1_get_instruction) | **PUT** /v1/instruction | 
 *DefaultApi* | [**v1_get_mount**](docs/DefaultApi.md#v1_get_mount) | **GET** /v1/mount | 
+*DefaultApi* | [**v1_get_node_controller_release**](docs/DefaultApi.md#v1_get_node_controller_release) | **GET** /v1/node-controller-releases | 
 *DefaultApi* | [**v1_get_node_diagnostic_tasks**](docs/DefaultApi.md#v1_get_node_diagnostic_tasks) | **GET** /v1/node-diagnostic-tasks | 
 *DefaultApi* | [**v1_get_node_properties**](docs/DefaultApi.md#v1_get_node_properties) | **GET** /v1/node-properties | 
 *DefaultApi* | [**v1_get_nodes**](docs/DefaultApi.md#v1_get_nodes) | **GET** /v1/nodes | 
 *DefaultApi* | [**v1_get_optical_tube**](docs/DefaultApi.md#v1_get_optical_tube) | **GET** /v1/optical-tube | 
 *DefaultApi* | [**v1_get_or_create_camera**](docs/DefaultApi.md#v1_get_or_create_camera) | **PUT** /v1/camera-match | 
 *DefaultApi* | [**v1_get_or_create_mount**](docs/DefaultApi.md#v1_get_or_create_mount) | **PUT** /v1/mount-match | 
 *DefaultApi* | [**v1_get_or_create_optical_tube**](docs/DefaultApi.md#v1_get_or_create_optical_tube) | **PUT** /v1/optical-tube-match | 
@@ -123,27 +149,30 @@
  - [MountType](docs/MountType.md)
  - [NodeState](docs/NodeState.md)
  - [OpticalTubeType](docs/OpticalTubeType.md)
  - [PlateSolveParameters](docs/PlateSolveParameters.md)
  - [ShutterType](docs/ShutterType.md)
  - [SuccessfulCreate](docs/SuccessfulCreate.md)
  - [TrackingType](docs/TrackingType.md)
+ - [V1AutoFocusInstruction](docs/V1AutoFocusInstruction.md)
+ - [V1AutoFocusInstructionCoordinatesInner](docs/V1AutoFocusInstructionCoordinatesInner.md)
  - [V1Camera](docs/V1Camera.md)
  - [V1ClientToken](docs/V1ClientToken.md)
  - [V1CompleteObservationRequest](docs/V1CompleteObservationRequest.md)
  - [V1CreateImageSetImageRequest](docs/V1CreateImageSetImageRequest.md)
  - [V1CreateImageSetImageResponse](docs/V1CreateImageSetImageResponse.md)
  - [V1CreateImageSetRequest](docs/V1CreateImageSetRequest.md)
  - [V1CreateMountRequest](docs/V1CreateMountRequest.md)
  - [V1CreateNodeDiagnostic](docs/V1CreateNodeDiagnostic.md)
  - [V1CreateNodeDiagnosticsRequest](docs/V1CreateNodeDiagnosticsRequest.md)
  - [V1CreateNodeRequest](docs/V1CreateNodeRequest.md)
  - [V1CreateOpticalTubeRequest](docs/V1CreateOpticalTubeRequest.md)
  - [V1DiagnosticInstruction](docs/V1DiagnosticInstruction.md)
  - [V1ElevationMaskPoint](docs/V1ElevationMaskPoint.md)
+ - [V1FileType](docs/V1FileType.md)
  - [V1GainCurve](docs/V1GainCurve.md)
  - [V1GainCurvePoint](docs/V1GainCurvePoint.md)
  - [V1GetInstructionRequest](docs/V1GetInstructionRequest.md)
  - [V1GetNodes](docs/V1GetNodes.md)
  - [V1GetOrCreateCameraRequest](docs/V1GetOrCreateCameraRequest.md)
  - [V1GetOrCreateMountRequest](docs/V1GetOrCreateMountRequest.md)
  - [V1GetOrCreateOpticalTubeRequest](docs/V1GetOrCreateOpticalTubeRequest.md)
@@ -158,16 +187,16 @@
  - [V1NodeComponentType](docs/V1NodeComponentType.md)
  - [V1NodeDiagnosticType](docs/V1NodeDiagnosticType.md)
  - [V1NodeWithLocation](docs/V1NodeWithLocation.md)
  - [V1ObservationInstruction](docs/V1ObservationInstruction.md)
  - [V1OpticalTube](docs/V1OpticalTube.md)
  - [V1PlateSolveCatalogFile](docs/V1PlateSolveCatalogFile.md)
  - [V1PlateSolveCatalogFileDownload](docs/V1PlateSolveCatalogFileDownload.md)
- - [V1PlateSolveCatalogIdentifier](docs/V1PlateSolveCatalogIdentifier.md)
  - [V1ReadNoisePoint](docs/V1ReadNoisePoint.md)
+ - [V1Release](docs/V1Release.md)
  - [V1SetupAction](docs/V1SetupAction.md)
  - [V1SlewTiming](docs/V1SlewTiming.md)
  - [V1SlewTimingInterval](docs/V1SlewTimingInterval.md)
  - [V1UpdateNodeComponentsRequest](docs/V1UpdateNodeComponentsRequest.md)
  - [V1UpdateNodeComponentsRequestCamera](docs/V1UpdateNodeComponentsRequestCamera.md)
  - [V1UpdateNodeComponentsRequestMount](docs/V1UpdateNodeComponentsRequestMount.md)
  - [V1UpdateNodeComponentsRequestOpticalTube](docs/V1UpdateNodeComponentsRequestOpticalTube.md)
@@ -190,7 +219,8 @@
 ### Roles
 
 
 
 ## Author
 
 
+
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/__init__.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.3.3445"
+__version__ = "1.3.3603"
 
 # import apis into sdk package
 from ourskyai_platform_api.api.default_api import DefaultApi
 
 # import ApiClient
 from ourskyai_platform_api.api_response import ApiResponse
 from ourskyai_platform_api.api_client import ApiClient
@@ -39,27 +39,30 @@
 from ourskyai_platform_api.models.mount_type import MountType
 from ourskyai_platform_api.models.node_state import NodeState
 from ourskyai_platform_api.models.optical_tube_type import OpticalTubeType
 from ourskyai_platform_api.models.plate_solve_parameters import PlateSolveParameters
 from ourskyai_platform_api.models.shutter_type import ShutterType
 from ourskyai_platform_api.models.successful_create import SuccessfulCreate
 from ourskyai_platform_api.models.tracking_type import TrackingType
+from ourskyai_platform_api.models.v1_auto_focus_instruction import V1AutoFocusInstruction
+from ourskyai_platform_api.models.v1_auto_focus_instruction_coordinates_inner import V1AutoFocusInstructionCoordinatesInner
 from ourskyai_platform_api.models.v1_camera import V1Camera
 from ourskyai_platform_api.models.v1_client_token import V1ClientToken
 from ourskyai_platform_api.models.v1_complete_observation_request import V1CompleteObservationRequest
 from ourskyai_platform_api.models.v1_create_image_set_image_request import V1CreateImageSetImageRequest
 from ourskyai_platform_api.models.v1_create_image_set_image_response import V1CreateImageSetImageResponse
 from ourskyai_platform_api.models.v1_create_image_set_request import V1CreateImageSetRequest
 from ourskyai_platform_api.models.v1_create_mount_request import V1CreateMountRequest
 from ourskyai_platform_api.models.v1_create_node_diagnostic import V1CreateNodeDiagnostic
 from ourskyai_platform_api.models.v1_create_node_diagnostics_request import V1CreateNodeDiagnosticsRequest
 from ourskyai_platform_api.models.v1_create_node_request import V1CreateNodeRequest
 from ourskyai_platform_api.models.v1_create_optical_tube_request import V1CreateOpticalTubeRequest
 from ourskyai_platform_api.models.v1_diagnostic_instruction import V1DiagnosticInstruction
 from ourskyai_platform_api.models.v1_elevation_mask_point import V1ElevationMaskPoint
+from ourskyai_platform_api.models.v1_file_type import V1FileType
 from ourskyai_platform_api.models.v1_gain_curve import V1GainCurve
 from ourskyai_platform_api.models.v1_gain_curve_point import V1GainCurvePoint
 from ourskyai_platform_api.models.v1_get_instruction_request import V1GetInstructionRequest
 from ourskyai_platform_api.models.v1_get_nodes import V1GetNodes
 from ourskyai_platform_api.models.v1_get_or_create_camera_request import V1GetOrCreateCameraRequest
 from ourskyai_platform_api.models.v1_get_or_create_mount_request import V1GetOrCreateMountRequest
 from ourskyai_platform_api.models.v1_get_or_create_optical_tube_request import V1GetOrCreateOpticalTubeRequest
@@ -74,16 +77,16 @@
 from ourskyai_platform_api.models.v1_node_component_type import V1NodeComponentType
 from ourskyai_platform_api.models.v1_node_diagnostic_type import V1NodeDiagnosticType
 from ourskyai_platform_api.models.v1_node_with_location import V1NodeWithLocation
 from ourskyai_platform_api.models.v1_observation_instruction import V1ObservationInstruction
 from ourskyai_platform_api.models.v1_optical_tube import V1OpticalTube
 from ourskyai_platform_api.models.v1_plate_solve_catalog_file import V1PlateSolveCatalogFile
 from ourskyai_platform_api.models.v1_plate_solve_catalog_file_download import V1PlateSolveCatalogFileDownload
-from ourskyai_platform_api.models.v1_plate_solve_catalog_identifier import V1PlateSolveCatalogIdentifier
 from ourskyai_platform_api.models.v1_read_noise_point import V1ReadNoisePoint
+from ourskyai_platform_api.models.v1_release import V1Release
 from ourskyai_platform_api.models.v1_setup_action import V1SetupAction
 from ourskyai_platform_api.models.v1_slew_timing import V1SlewTiming
 from ourskyai_platform_api.models.v1_slew_timing_interval import V1SlewTimingInterval
 from ourskyai_platform_api.models.v1_update_node_components_request import V1UpdateNodeComponentsRequest
 from ourskyai_platform_api.models.v1_update_node_components_request_camera import V1UpdateNodeComponentsRequestCamera
 from ourskyai_platform_api.models.v1_update_node_components_request_mount import V1UpdateNodeComponentsRequestMount
 from ourskyai_platform_api.models.v1_update_node_components_request_optical_tube import V1UpdateNodeComponentsRequestOpticalTube
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/api/default_api.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/api/default_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import re  # noqa: F401
 import io
 import warnings
 
 from pydantic import validate_arguments, ValidationError
 
-from pydantic import StrictBool, StrictFloat, StrictInt, StrictStr, conlist
+from typing_extensions import Annotated
+from pydantic import Field, StrictBool, StrictFloat, StrictInt, StrictStr, conlist
 
 from typing import List, Optional, Union
 
 from ourskyai_platform_api.models.empty_success import EmptySuccess
 from ourskyai_platform_api.models.successful_create import SuccessfulCreate
 from ourskyai_platform_api.models.v1_camera import V1Camera
 from ourskyai_platform_api.models.v1_client_token import V1ClientToken
@@ -46,14 +47,15 @@
 from ourskyai_platform_api.models.v1_instruction import V1Instruction
 from ourskyai_platform_api.models.v1_metric import V1Metric
 from ourskyai_platform_api.models.v1_mount import V1Mount
 from ourskyai_platform_api.models.v1_node import V1Node
 from ourskyai_platform_api.models.v1_node_diagnostic_type import V1NodeDiagnosticType
 from ourskyai_platform_api.models.v1_optical_tube import V1OpticalTube
 from ourskyai_platform_api.models.v1_plate_solve_catalog_file_download import V1PlateSolveCatalogFileDownload
+from ourskyai_platform_api.models.v1_release import V1Release
 from ourskyai_platform_api.models.v1_update_node_components_request import V1UpdateNodeComponentsRequest
 from ourskyai_platform_api.models.v1_update_node_request import V1UpdateNodeRequest
 from ourskyai_platform_api.models.v2_complete_observation_request import V2CompleteObservationRequest
 
 from ourskyai_platform_api.api_client import ApiClient
 from ourskyai_platform_api.api_response import ApiResponse
 from ourskyai_platform_api.exceptions import (  # noqa: F401
@@ -2545,14 +2547,154 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def v1_get_node_controller_release(self, lineage_id : Annotated[StrictStr, Field(..., description="lineage id")], **kwargs) -> V1Release:  # noqa: E501
+        """v1_get_node_controller_release  # noqa: E501
+
+        returns the current release for the node  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_get_node_controller_release(lineage_id, async_req=True)
+        >>> result = thread.get()
+
+        :param lineage_id: lineage id (required)
+        :type lineage_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request.
+               If one number provided, it will be total request
+               timeout. It can also be a pair (tuple) of
+               (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: V1Release
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            message = "Error! Please call the v1_get_node_controller_release_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            raise ValueError(message)
+        return self.v1_get_node_controller_release_with_http_info(lineage_id, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def v1_get_node_controller_release_with_http_info(self, lineage_id : Annotated[StrictStr, Field(..., description="lineage id")], **kwargs) -> ApiResponse:  # noqa: E501
+        """v1_get_node_controller_release  # noqa: E501
+
+        returns the current release for the node  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_get_node_controller_release_with_http_info(lineage_id, async_req=True)
+        >>> result = thread.get()
+
+        :param lineage_id: lineage id (required)
+        :type lineage_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(V1Release, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'lineage_id'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method v1_get_node_controller_release" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+        if _params.get('lineage_id') is not None:  # noqa: E501
+            _query_params.append(('lineageId', _params['lineage_id']))
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['Roles', 'BearerToken']  # noqa: E501
+
+        _response_types_map = {
+            '200': "V1Release",
+        }
+
+        return self.api_client.call_api(
+            '/v1/node-controller-releases', 'GET',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/api_client.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import atexit
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.3.3445/python'
+        self.user_agent = 'OpenAPI-Generator/1.3.3603/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/api_response.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/api_response.py`

 * *Files identical despite different names*

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/configuration.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import copy
@@ -371,16 +371,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.3.3445\n"\
-               "SDK Package Version: 1.3.3445".\
+               "Version of the API: 1.3.3603\n"\
+               "SDK Package Version: 1.3.3603".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/exceptions.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 class OpenApiException(Exception):
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/__init__.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
@@ -22,27 +22,30 @@
 from ourskyai_platform_api.models.mount_type import MountType
 from ourskyai_platform_api.models.node_state import NodeState
 from ourskyai_platform_api.models.optical_tube_type import OpticalTubeType
 from ourskyai_platform_api.models.plate_solve_parameters import PlateSolveParameters
 from ourskyai_platform_api.models.shutter_type import ShutterType
 from ourskyai_platform_api.models.successful_create import SuccessfulCreate
 from ourskyai_platform_api.models.tracking_type import TrackingType
+from ourskyai_platform_api.models.v1_auto_focus_instruction import V1AutoFocusInstruction
+from ourskyai_platform_api.models.v1_auto_focus_instruction_coordinates_inner import V1AutoFocusInstructionCoordinatesInner
 from ourskyai_platform_api.models.v1_camera import V1Camera
 from ourskyai_platform_api.models.v1_client_token import V1ClientToken
 from ourskyai_platform_api.models.v1_complete_observation_request import V1CompleteObservationRequest
 from ourskyai_platform_api.models.v1_create_image_set_image_request import V1CreateImageSetImageRequest
 from ourskyai_platform_api.models.v1_create_image_set_image_response import V1CreateImageSetImageResponse
 from ourskyai_platform_api.models.v1_create_image_set_request import V1CreateImageSetRequest
 from ourskyai_platform_api.models.v1_create_mount_request import V1CreateMountRequest
 from ourskyai_platform_api.models.v1_create_node_diagnostic import V1CreateNodeDiagnostic
 from ourskyai_platform_api.models.v1_create_node_diagnostics_request import V1CreateNodeDiagnosticsRequest
 from ourskyai_platform_api.models.v1_create_node_request import V1CreateNodeRequest
 from ourskyai_platform_api.models.v1_create_optical_tube_request import V1CreateOpticalTubeRequest
 from ourskyai_platform_api.models.v1_diagnostic_instruction import V1DiagnosticInstruction
 from ourskyai_platform_api.models.v1_elevation_mask_point import V1ElevationMaskPoint
+from ourskyai_platform_api.models.v1_file_type import V1FileType
 from ourskyai_platform_api.models.v1_gain_curve import V1GainCurve
 from ourskyai_platform_api.models.v1_gain_curve_point import V1GainCurvePoint
 from ourskyai_platform_api.models.v1_get_instruction_request import V1GetInstructionRequest
 from ourskyai_platform_api.models.v1_get_nodes import V1GetNodes
 from ourskyai_platform_api.models.v1_get_or_create_camera_request import V1GetOrCreateCameraRequest
 from ourskyai_platform_api.models.v1_get_or_create_mount_request import V1GetOrCreateMountRequest
 from ourskyai_platform_api.models.v1_get_or_create_optical_tube_request import V1GetOrCreateOpticalTubeRequest
@@ -57,16 +60,16 @@
 from ourskyai_platform_api.models.v1_node_component_type import V1NodeComponentType
 from ourskyai_platform_api.models.v1_node_diagnostic_type import V1NodeDiagnosticType
 from ourskyai_platform_api.models.v1_node_with_location import V1NodeWithLocation
 from ourskyai_platform_api.models.v1_observation_instruction import V1ObservationInstruction
 from ourskyai_platform_api.models.v1_optical_tube import V1OpticalTube
 from ourskyai_platform_api.models.v1_plate_solve_catalog_file import V1PlateSolveCatalogFile
 from ourskyai_platform_api.models.v1_plate_solve_catalog_file_download import V1PlateSolveCatalogFileDownload
-from ourskyai_platform_api.models.v1_plate_solve_catalog_identifier import V1PlateSolveCatalogIdentifier
 from ourskyai_platform_api.models.v1_read_noise_point import V1ReadNoisePoint
+from ourskyai_platform_api.models.v1_release import V1Release
 from ourskyai_platform_api.models.v1_setup_action import V1SetupAction
 from ourskyai_platform_api.models.v1_slew_timing import V1SlewTiming
 from ourskyai_platform_api.models.v1_slew_timing_interval import V1SlewTimingInterval
 from ourskyai_platform_api.models.v1_update_node_components_request import V1UpdateNodeComponentsRequest
 from ourskyai_platform_api.models.v1_update_node_components_request_camera import V1UpdateNodeComponentsRequestCamera
 from ourskyai_platform_api.models.v1_update_node_components_request_mount import V1UpdateNodeComponentsRequestMount
 from ourskyai_platform_api.models.v1_update_node_components_request_optical_tube import V1UpdateNodeComponentsRequestOpticalTube
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/camera_mode.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/camera_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/empty_success.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/empty_success.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/filter_type.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/filter_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/location.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/location.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/metric_type.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/metric_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/mount_type.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/mount_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/node_state.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/node_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/optical_tube_type.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/optical_tube_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/plate_solve_parameters.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/plate_solve_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/shutter_type.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/shutter_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/successful_create.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/successful_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/tracking_type.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/tracking_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_camera.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_camera.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_client_token.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_client_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_complete_observation_request.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_complete_observation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_create_image_set_image_request.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_image_set_image_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_create_image_set_image_response.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_image_set_image_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_create_image_set_request.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_image_set_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_create_mount_request.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_mount_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_create_node_diagnostic.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_node_diagnostic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_create_node_request.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_node_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_create_optical_tube_request.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_create_optical_tube_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_diagnostic_instruction.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_diagnostic_instruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_elevation_mask_point.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_elevation_mask_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_gain_curve.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_gain_curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_gain_curve_point.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_gain_curve_point.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_get_instruction_request.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_get_instruction_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_get_nodes.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_get_nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_get_or_create_camera_request.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_get_or_create_camera_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_get_or_create_mount_request.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_get_or_create_mount_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -17,23 +17,21 @@
 import re  # noqa: F401
 import json
 
 
 from typing import List
 from pydantic import BaseModel, Field, conlist
 from ourskyai_platform_api.models.v1_plate_solve_catalog_file import V1PlateSolveCatalogFile
-from ourskyai_platform_api.models.v1_plate_solve_catalog_identifier import V1PlateSolveCatalogIdentifier
 
 class V1GetPlateSolveCatalogDiffRequest(BaseModel):
     """
     V1GetPlateSolveCatalogDiffRequest
     """
-    identifier: V1PlateSolveCatalogIdentifier = Field(...)
     existing_files: conlist(V1PlateSolveCatalogFile) = Field(..., alias="existingFiles")
-    __properties = ["identifier", "existingFiles"]
+    __properties = ["existingFiles"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -70,13 +68,12 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return V1GetPlateSolveCatalogDiffRequest.parse_obj(obj)
 
         _obj = V1GetPlateSolveCatalogDiffRequest.parse_obj({
-            "identifier": obj.get("identifier"),
             "existing_files": [V1PlateSolveCatalogFile.from_dict(_item) for _item in obj.get("existingFiles")] if obj.get("existingFiles") is not None else None
         })
         return _obj
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_ground_station_participant.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_ground_station_participant.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_image_set.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_image_set.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_image_set_image.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_image_set_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_instruction.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_instruction.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, conlist
+from ourskyai_platform_api.models.v1_auto_focus_instruction import V1AutoFocusInstruction
 from ourskyai_platform_api.models.v1_diagnostic_instruction import V1DiagnosticInstruction
 from ourskyai_platform_api.models.v1_observation_instruction import V1ObservationInstruction
 
 class V1Instruction(BaseModel):
     """
     Instruction  # noqa: E501
     """
     observation: Optional[V1ObservationInstruction] = None
     diagnostic: Optional[V1DiagnosticInstruction] = None
     search: Optional[conlist(V1ObservationInstruction)] = None
-    __properties = ["observation", "diagnostic", "search"]
+    autofocus: Optional[V1AutoFocusInstruction] = None
+    __properties = ["observation", "diagnostic", "search", "autofocus"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -65,26 +67,30 @@
         # override the default output from pydantic by calling `to_dict()` of each item in search (list)
         _items = []
         if self.search:
             for _item in self.search:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['search'] = _items
+        # override the default output from pydantic by calling `to_dict()` of autofocus
+        if self.autofocus:
+            _dict['autofocus'] = self.autofocus.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> V1Instruction:
         """Create an instance of V1Instruction from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return V1Instruction.parse_obj(obj)
 
         _obj = V1Instruction.parse_obj({
             "observation": V1ObservationInstruction.from_dict(obj.get("observation")) if obj.get("observation") is not None else None,
             "diagnostic": V1DiagnosticInstruction.from_dict(obj.get("diagnostic")) if obj.get("diagnostic") is not None else None,
-            "search": [V1ObservationInstruction.from_dict(_item) for _item in obj.get("search")] if obj.get("search") is not None else None
+            "search": [V1ObservationInstruction.from_dict(_item) for _item in obj.get("search")] if obj.get("search") is not None else None,
+            "autofocus": V1AutoFocusInstruction.from_dict(obj.get("autofocus")) if obj.get("autofocus") is not None else None
         })
         return _obj
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_metric.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_mount.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_mount.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_node.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_node_component_type.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_node_component_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_node_diagnostic_type.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_node_diagnostic_type.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -42,14 +42,16 @@
     AVAILABLE_MEMORY_BYTES = 'AVAILABLE_MEMORY_BYTES'
     NTP_TIME_DRIFT_MS = 'NTP_TIME_DRIFT_MS'
     SYSTEM_UPTIME_S = 'SYSTEM_UPTIME_S'
     APPLICATION_UPTIME_S = 'APPLICATION_UPTIME_S'
     APPLICATION_CPU_TIME_S = 'APPLICATION_CPU_TIME_S'
     CPU_USAGE_LAST_SECOND_PCT = 'CPU_USAGE_LAST_SECOND_PCT'
     CPU_USAGE_LAST_MINUTE_PCT = 'CPU_USAGE_LAST_MINUTE_PCT'
+    FOCUS_HFR = 'FOCUS_HFR'
+    HAS_FOCUSER = 'HAS_FOCUSER'
 
     @classmethod
     def from_json(cls, json_str: str) -> V1NodeDiagnosticType:
         """Create an instance of V1NodeDiagnosticType from a JSON string"""
         return V1NodeDiagnosticType(json.loads(json_str))
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_node_with_location.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_node_with_location.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_observation_instruction.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_observation_instruction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_optical_tube.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_optical_tube.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 
-from pydantic import BaseModel, Field, StrictStr
+from pydantic import BaseModel, Field, StrictStr, validator
 
 class V1PlateSolveCatalogFileDownload(BaseModel):
     """
     V1PlateSolveCatalogFileDownload
     """
     name: StrictStr = Field(...)
     url: StrictStr = Field(...)
     base64_sha256_checksum: StrictStr = Field(..., alias="base64Sha256Checksum")
-    __properties = ["name", "url", "base64Sha256Checksum"]
+    action: StrictStr = Field(...)
+    __properties = ["name", "url", "base64Sha256Checksum", "action"]
+
+    @validator('action')
+    def action_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in ('DOWNLOAD', 'DELETE', 'NO_ACTION'):
+            raise ValueError("must be one of enum values ('DOWNLOAD', 'DELETE', 'NO_ACTION')")
+        return value
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -64,12 +72,13 @@
 
         if not isinstance(obj, dict):
             return V1PlateSolveCatalogFileDownload.parse_obj(obj)
 
         _obj = V1PlateSolveCatalogFileDownload.parse_obj({
             "name": obj.get("name"),
             "url": obj.get("url"),
-            "base64_sha256_checksum": obj.get("base64Sha256Checksum")
+            "base64_sha256_checksum": obj.get("base64Sha256Checksum"),
+            "action": obj.get("action")
         })
         return _obj
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_read_noise_point.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_read_noise_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_setup_action.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_setup_action.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_slew_timing.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_slew_timing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_slew_timing_interval.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_slew_timing_interval.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_update_node_components_request.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_update_node_components_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_update_node_components_request_camera.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_update_node_components_request_camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_update_node_components_request_mount.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_update_node_components_request_mount.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_update_node_request.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_update_node_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v1_video_mode_framerate_property.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v1_video_mode_framerate_property.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/models/v2_complete_observation_request.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/models/v2_complete_observation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3445/ourskyai_platform_api/rest.py` & `ourskyai_platform_api-1.3.3603/ourskyai_platform_api/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3445
+    The version of the OpenAPI document: 1.3.3603
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `ourskyai_platform_api-1.3.3445/pyproject.toml` & `ourskyai_platform_api-1.3.3603/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ourskyai_platform_api"
-version = "1.3.3445"
+version = "1.3.3603"
 description = "OurSky Platform"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "OurSky Platform"]
 include = ["ourskyai_platform_api/py.typed"]
```

### Comparing `ourskyai_platform_api-1.3.3445/PKG-INFO` & `ourskyai_platform_api-1.3.3603/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,14 @@
-Metadata-Version: 2.1
-Name: ourskyai_platform_api
-Version: 1.3.3445
-Summary: OurSky Platform
-Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
-License: NoLicense
-Keywords: OpenAPI,OpenAPI-Generator,OurSky Platform
-Author: OpenAPI Generator Community
-Author-email: team@openapitools.org
-Requires-Python: >=3.7,<4.0
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: aenum (>=3.1.11)
-Requires-Dist: pydantic (>=1.10.5,<2.0.0)
-Requires-Dist: python-dateutil (>=2.8.2)
-Requires-Dist: urllib3 (>=1.25.3)
-Project-URL: Repository, https://github.com/GIT_USER_ID/GIT_REPO_ID
-Description-Content-Type: text/markdown
-
 # ourskyai-platform-api
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3445
-- Package version: 1.3.3445
+- API version: 1.3.3603
+- Package version: 1.3.3603
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
@@ -119,14 +94,15 @@
 *DefaultApi* | [**v1_delete_image_set**](docs/DefaultApi.md#v1_delete_image_set) | **DELETE** /v1/image-set | 
 *DefaultApi* | [**v1_delete_image_set_image**](docs/DefaultApi.md#v1_delete_image_set_image) | **DELETE** /v1/image-set-image | 
 *DefaultApi* | [**v1_get_cameras**](docs/DefaultApi.md#v1_get_cameras) | **GET** /v1/cameras | 
 *DefaultApi* | [**v1_get_image_set**](docs/DefaultApi.md#v1_get_image_set) | **GET** /v1/image-set | 
 *DefaultApi* | [**v1_get_image_set_image**](docs/DefaultApi.md#v1_get_image_set_image) | **GET** /v1/image-set-image | 
 *DefaultApi* | [**v1_get_instruction**](docs/DefaultApi.md#v1_get_instruction) | **PUT** /v1/instruction | 
 *DefaultApi* | [**v1_get_mount**](docs/DefaultApi.md#v1_get_mount) | **GET** /v1/mount | 
+*DefaultApi* | [**v1_get_node_controller_release**](docs/DefaultApi.md#v1_get_node_controller_release) | **GET** /v1/node-controller-releases | 
 *DefaultApi* | [**v1_get_node_diagnostic_tasks**](docs/DefaultApi.md#v1_get_node_diagnostic_tasks) | **GET** /v1/node-diagnostic-tasks | 
 *DefaultApi* | [**v1_get_node_properties**](docs/DefaultApi.md#v1_get_node_properties) | **GET** /v1/node-properties | 
 *DefaultApi* | [**v1_get_nodes**](docs/DefaultApi.md#v1_get_nodes) | **GET** /v1/nodes | 
 *DefaultApi* | [**v1_get_optical_tube**](docs/DefaultApi.md#v1_get_optical_tube) | **GET** /v1/optical-tube | 
 *DefaultApi* | [**v1_get_or_create_camera**](docs/DefaultApi.md#v1_get_or_create_camera) | **PUT** /v1/camera-match | 
 *DefaultApi* | [**v1_get_or_create_mount**](docs/DefaultApi.md#v1_get_or_create_mount) | **PUT** /v1/mount-match | 
 *DefaultApi* | [**v1_get_or_create_optical_tube**](docs/DefaultApi.md#v1_get_or_create_optical_tube) | **PUT** /v1/optical-tube-match | 
@@ -148,27 +124,30 @@
  - [MountType](docs/MountType.md)
  - [NodeState](docs/NodeState.md)
  - [OpticalTubeType](docs/OpticalTubeType.md)
  - [PlateSolveParameters](docs/PlateSolveParameters.md)
  - [ShutterType](docs/ShutterType.md)
  - [SuccessfulCreate](docs/SuccessfulCreate.md)
  - [TrackingType](docs/TrackingType.md)
+ - [V1AutoFocusInstruction](docs/V1AutoFocusInstruction.md)
+ - [V1AutoFocusInstructionCoordinatesInner](docs/V1AutoFocusInstructionCoordinatesInner.md)
  - [V1Camera](docs/V1Camera.md)
  - [V1ClientToken](docs/V1ClientToken.md)
  - [V1CompleteObservationRequest](docs/V1CompleteObservationRequest.md)
  - [V1CreateImageSetImageRequest](docs/V1CreateImageSetImageRequest.md)
  - [V1CreateImageSetImageResponse](docs/V1CreateImageSetImageResponse.md)
  - [V1CreateImageSetRequest](docs/V1CreateImageSetRequest.md)
  - [V1CreateMountRequest](docs/V1CreateMountRequest.md)
  - [V1CreateNodeDiagnostic](docs/V1CreateNodeDiagnostic.md)
  - [V1CreateNodeDiagnosticsRequest](docs/V1CreateNodeDiagnosticsRequest.md)
  - [V1CreateNodeRequest](docs/V1CreateNodeRequest.md)
  - [V1CreateOpticalTubeRequest](docs/V1CreateOpticalTubeRequest.md)
  - [V1DiagnosticInstruction](docs/V1DiagnosticInstruction.md)
  - [V1ElevationMaskPoint](docs/V1ElevationMaskPoint.md)
+ - [V1FileType](docs/V1FileType.md)
  - [V1GainCurve](docs/V1GainCurve.md)
  - [V1GainCurvePoint](docs/V1GainCurvePoint.md)
  - [V1GetInstructionRequest](docs/V1GetInstructionRequest.md)
  - [V1GetNodes](docs/V1GetNodes.md)
  - [V1GetOrCreateCameraRequest](docs/V1GetOrCreateCameraRequest.md)
  - [V1GetOrCreateMountRequest](docs/V1GetOrCreateMountRequest.md)
  - [V1GetOrCreateOpticalTubeRequest](docs/V1GetOrCreateOpticalTubeRequest.md)
@@ -183,16 +162,16 @@
  - [V1NodeComponentType](docs/V1NodeComponentType.md)
  - [V1NodeDiagnosticType](docs/V1NodeDiagnosticType.md)
  - [V1NodeWithLocation](docs/V1NodeWithLocation.md)
  - [V1ObservationInstruction](docs/V1ObservationInstruction.md)
  - [V1OpticalTube](docs/V1OpticalTube.md)
  - [V1PlateSolveCatalogFile](docs/V1PlateSolveCatalogFile.md)
  - [V1PlateSolveCatalogFileDownload](docs/V1PlateSolveCatalogFileDownload.md)
- - [V1PlateSolveCatalogIdentifier](docs/V1PlateSolveCatalogIdentifier.md)
  - [V1ReadNoisePoint](docs/V1ReadNoisePoint.md)
+ - [V1Release](docs/V1Release.md)
  - [V1SetupAction](docs/V1SetupAction.md)
  - [V1SlewTiming](docs/V1SlewTiming.md)
  - [V1SlewTimingInterval](docs/V1SlewTimingInterval.md)
  - [V1UpdateNodeComponentsRequest](docs/V1UpdateNodeComponentsRequest.md)
  - [V1UpdateNodeComponentsRequestCamera](docs/V1UpdateNodeComponentsRequestCamera.md)
  - [V1UpdateNodeComponentsRequestMount](docs/V1UpdateNodeComponentsRequestMount.md)
  - [V1UpdateNodeComponentsRequestOpticalTube](docs/V1UpdateNodeComponentsRequestOpticalTube.md)
@@ -215,8 +194,7 @@
 ### Roles
 
 
 
 ## Author
 
 
-
```

