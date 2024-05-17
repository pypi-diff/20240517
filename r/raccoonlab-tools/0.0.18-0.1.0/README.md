# Comparing `tmp/raccoonlab-tools-0.0.18.tar.gz` & `tmp/raccoonlab_tools-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raccoonlab-tools-0.0.18.tar", last modified: Sun Mar 31 10:27:25 2024, max compression
+gzip compressed data, was "raccoonlab_tools-0.1.0.tar", last modified: Fri May 17 20:31:43 2024, max compression
```

## Comparing `raccoonlab-tools-0.0.18.tar` & `raccoonlab_tools-0.1.0.tar`

### file list

```diff
@@ -1,60 +1,76 @@
-drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-03-31 10:27:25.505956 raccoonlab-tools-0.0.18/
--rw-rw-r--   0 nex       (1000) nex       (1000)     1073 2023-05-23 21:41:19.000000 raccoonlab-tools-0.0.18/LICENSE
--rw-r--r--   0 nex       (1000) nex       (1000)     8044 2024-03-31 10:27:25.505956 raccoonlab-tools-0.0.18/PKG-INFO
--rw-rw-r--   0 nex       (1000) nex       (1000)     7335 2024-03-31 10:25:22.000000 raccoonlab-tools-0.0.18/README.md
--rw-rw-r--   0 nex       (1000) nex       (1000)     1647 2024-03-31 10:25:22.000000 raccoonlab-tools-0.0.18/pyproject.toml
--rw-rw-r--   0 nex       (1000) nex       (1000)      115 2024-02-13 11:26:42.000000 raccoonlab-tools-0.0.18/requirements.txt
--rw-rw-r--   0 nex       (1000) nex       (1000)       38 2024-03-31 10:27:25.505956 raccoonlab-tools-0.0.18/setup.cfg
-drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-03-31 10:27:25.501955 raccoonlab-tools-0.0.18/src/
-drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-03-31 10:27:25.501955 raccoonlab-tools-0.0.18/src/raccoonlab_tools/
-drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-03-31 10:27:25.505956 raccoonlab-tools-0.0.18/src/raccoonlab_tools/common/
--rwxrwxr-x   0 nex       (1000) nex       (1000)     1697 2024-02-13 11:26:42.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/common/colorizer.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)     3921 2024-02-13 11:26:42.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/common/device_manager.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)     5327 2024-02-13 11:26:42.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/common/firmware_manager.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)     3349 2024-02-13 11:26:42.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/common/node.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)      952 2024-02-13 11:26:42.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/common/printer.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)     5479 2024-02-13 11:26:42.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/common/protocol_parser.py
-drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-03-31 10:27:25.505956 raccoonlab-tools-0.0.18/src/raccoonlab_tools/cyphal/
--rwxrwxr-x   0 nex       (1000) nex       (1000)     1252 2024-02-13 11:26:42.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/cyphal/fragments.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)     5092 2024-02-13 11:26:42.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/cyphal/gnss.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)     9465 2024-02-13 11:26:42.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/cyphal/utils.py
-drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-03-31 10:27:25.505956 raccoonlab-tools-0.0.18/src/raccoonlab_tools/dronecan/
--rwxrwxr-x   0 nex       (1000) nex       (1000)     3676 2024-03-30 18:43:38.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/dronecan/global_node.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)     9202 2024-03-30 18:43:38.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/dronecan/utils.py
-drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-03-31 10:27:25.501955 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/
-drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-03-31 10:27:25.505956 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/common/
--rwxrwxr-x   0 nex       (1000) nex       (1000)      485 2024-02-13 11:26:42.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/common/check_protocol.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)      830 2024-03-06 11:55:45.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/common/create_pkg.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)      182 2024-03-05 14:49:24.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/common/create_slcan.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)      618 2024-03-31 09:07:47.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/common/get_can_iface.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)     1626 2024-03-31 09:41:03.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/common/get_info.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)      684 2024-03-28 18:09:27.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/common/kek.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)      447 2024-02-10 11:47:41.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/common/parse_pytest_res_json.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)     1074 2024-02-13 11:26:42.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/common/upload_firmware.py
-drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-03-31 10:27:25.505956 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/cyphal/
--rwxrwxr-x   0 nex       (1000) nex       (1000)     2069 2024-03-28 17:30:53.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/cyphal/emulate_myxa_feedback.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)    15560 2024-03-30 19:38:35.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/cyphal/monitor.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)    17191 2024-02-13 11:26:42.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/cyphal/test_specification.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)     5736 2024-03-28 14:37:27.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/cyphal/ublox_center.py
-drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-03-31 10:27:25.505956 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/dronecan/
--rwxrwxr-x   0 nex       (1000) nex       (1000)     2547 2024-02-13 11:26:42.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/dronecan/config.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)      781 2024-02-13 11:26:42.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/dronecan/get_params.py
-drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-03-31 10:27:25.505956 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/dronecan/lights_tester/
--rwxrwxr-x   0 nex       (1000) nex       (1000)     4373 2024-03-17 14:43:48.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/dronecan/lights_tester/lights_tester.py
-drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-03-31 10:27:25.505956 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/dronecan/servo_tester/
--rw-rw-r--   0 nex       (1000) nex       (1000)     3078 2024-02-13 11:26:42.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/dronecan/servo_tester/node_parser.py
--rw-rw-r--   0 nex       (1000) nex       (1000)     2801 2024-02-13 11:26:42.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/dronecan/servo_tester/servo_tester.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)     1356 2024-02-13 11:26:42.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/dronecan/set_params.py
-drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-03-31 10:27:25.505956 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/dronecan/sim_battery/
--rwxrwxr-x   0 nex       (1000) nex       (1000)     1675 2024-02-13 11:26:42.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/dronecan/sim_battery/sim_battery.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)     2721 2024-02-13 11:26:42.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/dronecan/test_gps_mag_baro.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)     8729 2024-03-17 14:43:48.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/dronecan/test_lights.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)     2790 2024-03-05 08:36:56.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/dronecan/test_pwm_node.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)     2346 2024-02-13 11:26:42.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/dronecan/test_specification.py
-drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-03-31 10:27:25.505956 raccoonlab-tools-0.0.18/src/raccoonlab_tools.egg-info/
--rw-r--r--   0 nex       (1000) nex       (1000)     8044 2024-03-31 10:27:25.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools.egg-info/PKG-INFO
--rw-rw-r--   0 nex       (1000) nex       (1000)     2050 2024-03-31 10:27:25.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 nex       (1000) nex       (1000)        1 2024-03-31 10:27:25.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 nex       (1000) nex       (1000)      900 2024-03-31 10:27:25.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools.egg-info/entry_points.txt
--rw-rw-r--   0 nex       (1000) nex       (1000)       68 2024-03-31 10:27:25.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools.egg-info/requires.txt
--rw-rw-r--   0 nex       (1000) nex       (1000)       17 2024-03-31 10:27:25.000000 raccoonlab-tools-0.0.18/src/raccoonlab_tools.egg-info/top_level.txt
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-05-17 20:31:43.757022 raccoonlab_tools-0.1.0/
+-rw-rw-r--   0 nex       (1000) nex       (1000)     1073 2023-05-23 21:41:19.000000 raccoonlab_tools-0.1.0/LICENSE
+-rw-r--r--   0 nex       (1000) nex       (1000)     8198 2024-05-17 20:31:43.757022 raccoonlab_tools-0.1.0/PKG-INFO
+-rw-rw-r--   0 nex       (1000) nex       (1000)     7490 2024-04-09 14:50:33.000000 raccoonlab_tools-0.1.0/README.md
+-rw-rw-r--   0 nex       (1000) nex       (1000)     1877 2024-05-17 20:24:38.000000 raccoonlab_tools-0.1.0/pyproject.toml
+-rw-rw-r--   0 nex       (1000) nex       (1000)      115 2024-02-13 11:26:42.000000 raccoonlab_tools-0.1.0/requirements.txt
+-rw-rw-r--   0 nex       (1000) nex       (1000)       38 2024-05-17 20:31:43.757022 raccoonlab_tools-0.1.0/setup.cfg
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-05-17 20:31:43.753022 raccoonlab_tools-0.1.0/src/
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-05-17 20:31:43.753022 raccoonlab_tools-0.1.0/src/raccoonlab_tools/
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-05-17 20:31:43.757022 raccoonlab_tools-0.1.0/src/raccoonlab_tools/common/
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     1697 2024-02-13 11:26:42.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/common/colorizer.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     5292 2024-03-31 12:03:48.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/common/device_manager.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     5327 2024-02-13 11:26:42.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/common/firmware_manager.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     3349 2024-02-13 11:26:42.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/common/node.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     5483 2024-03-31 12:03:48.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/common/protocol_parser.py
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-05-17 20:31:43.757022 raccoonlab_tools-0.1.0/src/raccoonlab_tools/cyphal/
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     1252 2024-02-13 11:26:42.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/cyphal/fragments.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     5092 2024-02-13 11:26:42.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/cyphal/gnss.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     9509 2024-03-31 12:03:48.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/cyphal/utils.py
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-05-17 20:31:43.757022 raccoonlab_tools-0.1.0/src/raccoonlab_tools/dronecan/
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     3678 2024-03-31 12:03:48.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/dronecan/global_node.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     9202 2024-03-30 18:43:38.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/dronecan/utils.py
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-05-17 20:31:43.753022 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-05-17 20:31:43.757022 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/common/
+-rwxrwxr-x   0 nex       (1000) nex       (1000)      487 2024-03-31 12:03:48.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/common/check_protocol.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)      830 2024-03-06 11:55:45.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/common/create_pkg.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)      182 2024-03-05 14:49:24.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/common/create_slcan.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     1628 2024-03-31 12:03:48.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/common/get_info.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)      684 2024-04-04 12:46:47.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/common/kak.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)      684 2024-03-28 18:09:27.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/common/kek.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)      447 2024-02-10 11:47:41.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/common/parse_pytest_res_json.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     1074 2024-02-13 11:26:42.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/common/upload_firmware.py
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-05-17 20:31:43.757022 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/cyphal/
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     2069 2024-03-28 17:30:53.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/cyphal/emulate_myxa_feedback.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)    17191 2024-02-13 11:26:42.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/cyphal/test_specification.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     5742 2024-04-17 18:26:02.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/cyphal/ublox_center.py
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-05-17 20:31:43.757022 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/
+-rwxrwxr-x   0 nex       (1000) nex       (1000)      262 2024-04-03 13:08:40.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/beep.py
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-05-17 20:31:43.757022 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/buzzer_tester/
+-rw-rw-r--   0 nex       (1000) nex       (1000)     1902 2024-04-17 18:26:02.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/buzzer_tester/test_buzzer.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     2532 2024-03-31 12:07:50.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/config.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)      779 2024-03-31 12:03:48.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/get_params.py
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-05-17 20:31:43.757022 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/lights_tester/
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     4373 2024-03-17 14:43:48.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/lights_tester/lights_tester.py
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-05-17 20:31:43.757022 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/pwm_tester/
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     6523 2024-05-17 20:24:38.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/pwm_tester/pwm_tester.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     6031 2024-04-23 08:23:07.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/ramil.py
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-05-17 20:31:43.757022 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/servo_tester/
+-rw-rw-r--   0 nex       (1000) nex       (1000)     3078 2024-02-13 11:26:42.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/servo_tester/node_parser.py
+-rw-rw-r--   0 nex       (1000) nex       (1000)     2801 2024-02-13 11:26:42.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/servo_tester/servo_tester.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     1356 2024-02-13 11:26:42.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/set_params.py
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-05-17 20:31:43.757022 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/sim_battery/
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     1675 2024-04-17 09:47:39.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/sim_battery/sim_battery.py
+-rw-rw-r--   0 nex       (1000) nex       (1000)     3674 2024-04-09 17:56:07.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/test_circuit_status.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     2721 2024-02-13 11:26:42.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/test_gps_mag_baro.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     8729 2024-03-17 14:43:48.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/test_lights.py
+-rw-rw-r--   0 nex       (1000) nex       (1000)     9172 2024-04-17 18:26:02.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/test_pmu_buzzer.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     2790 2024-03-05 08:36:56.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/test_pwm_node.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     2346 2024-02-13 11:26:42.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/test_specification.py
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-05-17 20:31:43.757022 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/rl_git_info/
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     1426 2024-05-17 20:24:38.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/rl_git_info/script.py
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-05-17 20:31:43.757022 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/rl_monitor/
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     4210 2024-04-17 18:26:02.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/rl_monitor/base_subscriber.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)    18842 2024-04-17 18:26:02.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/rl_monitor/script.py
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-05-17 20:31:43.757022 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/rl_printer/
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     1193 2024-05-17 20:24:38.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/rl_printer/script.py
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-05-17 20:31:43.757022 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/stm32/
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     2987 2024-04-02 20:46:33.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/stm32/build_cubeide.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     2291 2024-04-02 21:22:53.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/stm32/test_ioc.py
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2024-05-17 20:31:43.757022 raccoonlab_tools-0.1.0/src/raccoonlab_tools.egg-info/
+-rw-r--r--   0 nex       (1000) nex       (1000)     8198 2024-05-17 20:31:43.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 nex       (1000) nex       (1000)     2604 2024-05-17 20:31:43.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 nex       (1000) nex       (1000)        1 2024-05-17 20:31:43.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 nex       (1000) nex       (1000)     1124 2024-05-17 20:31:43.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 nex       (1000) nex       (1000)       68 2024-05-17 20:31:43.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools.egg-info/requires.txt
+-rw-rw-r--   0 nex       (1000) nex       (1000)       17 2024-05-17 20:31:43.000000 raccoonlab_tools-0.1.0/src/raccoonlab_tools.egg-info/top_level.txt
```

### Comparing `raccoonlab-tools-0.0.18/LICENSE` & `raccoonlab_tools-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `raccoonlab-tools-0.0.18/PKG-INFO` & `raccoonlab_tools-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raccoonlab-tools
-Version: 0.0.18
+Version: 0.1.0
 Summary: RaccoonLab tools
 Author-email: Dmitry Ponomarev <PonomarevDA96@gmail.com>
 Project-URL: Homepage, https://github.com/PonomarevDA/tools
 Project-URL: Bug Tracker, https://github.com/PonomarevDA/tools/issues
 Keywords: cyphal,dronecan,can
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -73,26 +73,34 @@
 | UAVCAN__CAN__BITRATE | Arbitration/data segment bits per second |
 | UAVCAN__CAN__MTU     | Maximum transmission unit: 8 for classic CAN |
 
 > Check pycyphal/yakut/yukon docs for additional details
 
 </details>
 
-## 2. LINUX PREPARATION (SOCKETCAN)
+## 2. LINUX (SOCKETCAN)
 
 By default, DroneCAN and Cyphal/CAN uses cross-platform transport interface [Python-CAN](https://python-can.readthedocs.io/en/stable/) [CAN over Serial / SLCAN](https://python-can.readthedocs.io/en/stable/interfaces/slcan.html).
 
 On Linux, [the socketcan interface](https://python-can.readthedocs.io/en/stable/interfaces/socketcan.html) is recommended. Unlike SLCAN, socketcan interface allows to share the same CAN interface with multiple processes, so you can run a few pycyphal scripts, yukon, yakut simultaniously.
 
 You can run the following script:
 
 ```bash
 ./scripts/socketcan.sh
 ```
 
+If you don't have a real CAN device, you can create a virtual CAN interface:
+
+```bash
+./scripts/socketcan.sh --virtual-can
+```
+
+Try `--help` option for more details.
+
 For a Cyphal application after creating socketcan interface, you need to update `UAVCAN__CAN__IFACE` environment variable. Just call `source ~/.bashrc`.
 
 ## 3. USAGE
 
 ### 1. Test cyphal specification
 
 ```bash
```

### Comparing `raccoonlab-tools-0.0.18/README.md` & `raccoonlab_tools-0.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -51,26 +51,34 @@
 | UAVCAN__CAN__BITRATE | Arbitration/data segment bits per second |
 | UAVCAN__CAN__MTU     | Maximum transmission unit: 8 for classic CAN |
 
 > Check pycyphal/yakut/yukon docs for additional details
 
 </details>
 
-## 2. LINUX PREPARATION (SOCKETCAN)
+## 2. LINUX (SOCKETCAN)
 
 By default, DroneCAN and Cyphal/CAN uses cross-platform transport interface [Python-CAN](https://python-can.readthedocs.io/en/stable/) [CAN over Serial / SLCAN](https://python-can.readthedocs.io/en/stable/interfaces/slcan.html).
 
 On Linux, [the socketcan interface](https://python-can.readthedocs.io/en/stable/interfaces/socketcan.html) is recommended. Unlike SLCAN, socketcan interface allows to share the same CAN interface with multiple processes, so you can run a few pycyphal scripts, yukon, yakut simultaniously.
 
 You can run the following script:
 
 ```bash
 ./scripts/socketcan.sh
 ```
 
+If you don't have a real CAN device, you can create a virtual CAN interface:
+
+```bash
+./scripts/socketcan.sh --virtual-can
+```
+
+Try `--help` option for more details.
+
 For a Cyphal application after creating socketcan interface, you need to update `UAVCAN__CAN__IFACE` environment variable. Just call `source ~/.bashrc`.
 
 ## 3. USAGE
 
 ### 1. Test cyphal specification
 
 ```bash
```

### Comparing `raccoonlab-tools-0.0.18/pyproject.toml` & `raccoonlab_tools-0.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "raccoonlab-tools"
-version = "0.0.18"
+version = "0.1.0"
 authors = [
   { name="Dmitry Ponomarev", email="PonomarevDA96@gmail.com" },
 ]
 description = "RaccoonLab tools"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["cyphal", "dronecan", "can"]
@@ -20,24 +20,28 @@
 dynamic = ["dependencies"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
 [project.scripts]
 rl-get-info = "raccoonlab_tools.scripts.common.get_info:main"
-rl-get-can-iface = "raccoonlab_tools.scripts.common.get_can_iface:main"
+rl-get-cyphal-can-iface = "raccoonlab_tools.common.device_manager:print_cyphal_can_iface"
 rl-upload-firmware = "raccoonlab_tools.scripts.common.upload_firmware:main"
 rl-config = "raccoonlab_tools.scripts.dronecan.config:main"
-rl-monitor = "raccoonlab_tools.scripts.cyphal.monitor:main"
+rl-monitor = "raccoonlab_tools.scripts.rl_monitor.script:main"
 rl-ublox-center = "raccoonlab_tools.scripts.cyphal.ublox_center:main"
 
 rl-test-cyphal-specification = "raccoonlab_tools.scripts.cyphal.test_specification:main"
 
 rl-test-dronecan-gps-mag-baro = "raccoonlab_tools.scripts.dronecan.test_gps_mag_baro:main"
 rl-test-dronecan-lights = "raccoonlab_tools.scripts.dronecan.test_lights:main"
 rl-test-dronecan-specification = "raccoonlab_tools.scripts.dronecan.test_specification:main"
 rl-get-dronecan-params = "raccoonlab_tools.scripts.dronecan.get_params:main"
 rl-set-dronecan-params = "raccoonlab_tools.scripts.dronecan.set_params:main"
 
+rl-git-info = "raccoonlab_tools.scripts.rl_git_info.script:main"
+rl-build-stm32-cubeide = "raccoonlab_tools.scripts.stm32.build_cubeide:main"
+rl-stm32-test-ioc = "raccoonlab_tools.scripts.stm32.test_ioc:main"
+
 [project.urls]
 "Homepage" = "https://github.com/PonomarevDA/tools"
 "Bug Tracker" = "https://github.com/PonomarevDA/tools/issues"
```

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/common/colorizer.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/common/colorizer.py`

 * *Files identical despite different names*

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/common/device_manager.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/common/device_manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -53,20 +53,64 @@
 
         if verbose:
             DeviceManager._print_finding_transport_results(transports)
 
         return transports
 
     @staticmethod
-    def get_transport(verbose=False) -> str:
-        """ Return examples: ["/dev/ttyACM0", "COM16", "slcan0"] """
-        transports = DeviceManager.find_transports(verbose)
-        if len(transports) == 0:
+    def get_device_port(verbose=False) -> str:
+        """
+        Find device ports and return the best one.
+        Raise an exeption if it doesn't exist.
+        Return examples: ["/dev/ttyACM0", "COM16", "slcan0"]
+        """
+        devices = DeviceManager.find_transports(verbose)
+        if len(devices) == 0:
             raise TransportNotFoundException("[ERROR] CAN-transport has not been detected.")
-        return transports[0].port
+        return devices[0].port
+
+    @staticmethod
+    def get_cyphal_can_iface() -> str:
+        """
+        Examples of output.
+        - slcan:/dev/ttyACM0@1000000
+        - socketcan:slcan0
+        """
+        devices = DeviceManager.find_transports()
+
+        if len(devices) == 0:
+            return ""
+
+        best_device_port = devices[0].port
+        if best_device_port.startswith("slcan"):
+            can_iface_name = f"socketcan:{best_device_port}"
+        else:
+            can_iface_name = f"slcan:{best_device_port}@1000000"
+
+        return can_iface_name
+
+    @staticmethod
+    def get_dronecan_can_iface() -> str:
+        """
+        Examples of output.
+        - slcan:/dev/ttyACM0
+        - slcan0
+        """
+        devices = DeviceManager.find_transports()
+
+        if len(devices) == 0:
+            return ""
+
+        best_device_port = devices[0].port
+        if best_device_port.startswith("slcan"):
+            can_iface_name = best_device_port
+        else:
+            can_iface_name = f"slcan:{best_device_port}"
+
+        return can_iface_name
 
     @staticmethod
     def find_programmers(verbose=True) -> list:
         programmers = []
         ports = serial.tools.list_ports.comports()
         for port, desc, hwid in sorted(ports):
             for known_programmer in KNOWN_PROGRAMMERS:
@@ -98,11 +142,18 @@
         elif len(transports) == 1:
             print(f"Avaliable CAN-transports: {transports[0]}")
         else:
             print("Avaliable CAN-transports:")
             for transport in transports:
                 print(f"- {transport}")
 
+def print_cyphal_can_iface():
+    print(DeviceManager.get_cyphal_can_iface())
+
+def print_dronecan_can_iface():
+    print(DeviceManager.get_dronecan_can_iface())
 
 if __name__ == "__main__":
     DeviceManager.find_transports(verbose=True)
     DeviceManager.find_programmers(verbose=True)
+    print_cyphal_can_iface()
+    print_dronecan_can_iface()
```

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/common/firmware_manager.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/common/firmware_manager.py`

 * *Files identical despite different names*

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/common/node.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/common/node.py`

 * *Files identical despite different names*

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/common/protocol_parser.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/common/protocol_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         """
         Gently try to guess the protocol. Does Not raise an exception.
         """
         assert isinstance(transport, str) or transport is None
         assert isinstance(verbose, bool)
 
         if transport is None:
-            transport = DeviceManager.get_transport(verbose=verbose)
+            transport = DeviceManager.get_device_port(verbose=verbose)
 
         protocol = CanProtocolParser._parse_protocol(transport)
         if protocol == Protocol.NONE:
             print("[ERROR] CAN-node is offline.")
         elif protocol == Protocol.UNKNOWN:
             print("[ERROR] CAN-node is online, but the protocol couldn't be determined.")
         elif verbose:
@@ -142,9 +142,9 @@
                 protocol = CanMessage(can_frame).parse_protocol_from_message()
                 if protocol is not Protocol.UNKNOWN:
                     break
 
         return protocol
 
 if __name__ == "__main__":
-    transport = DeviceManager.get_transport(verbose=True)
+    transport = DeviceManager.get_device_port(verbose=True)
     CanProtocolParser.find_protocol(transport, verbose=True)
```

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/cyphal/fragments.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/cyphal/fragments.py`

 * *Files identical despite different names*

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/cyphal/gnss.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/cyphal/gnss.py`

 * *Files identical despite different names*

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/cyphal/utils.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/cyphal/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,21 +52,21 @@
             if transfer[1].source_node_id not in NodeFinder.black_list:
                 NodeFinder.target_node_id = transfer[1].source_node_id
                 break
         sub.close()
 
         return NodeFinder.target_node_id
 
-    async def get_info(self) -> dict:
+    async def get_info(self, number_of_attempts: int=3) -> dict:
         """Return a dictionary on success. Otherwise return None."""
         dest_node_id = await self.find_online_node()
 
         request = uavcan.node.GetInfo_1_0.Request()
         client = self.node.make_client(uavcan.node.GetInfo_1_0, dest_node_id)
-        for attempt in range(3):
+        for attempt in range(number_of_attempts):
             if attempt == 0:
                 print(f"[DEBUG] NodeInfo: send request to {dest_node_id}")
             else:
                 print(f"[DEBUG] NodeInfo: send request to {dest_node_id} ({attempt + 1})")
             response = await client.call(request)
             if response is not None:
                 break
```

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/dronecan/global_node.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/dronecan/global_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import List, Optional, Callable
 from raccoonlab_tools.common.device_manager import DeviceManager
 
 class DronecanNode:
     node = None
     def __init__(self) -> None:
         if DronecanNode.node is None:
-            transport = DeviceManager.get_transport()
+            transport = DeviceManager.get_device_port()
             if transport.startswith("slcan"):
                 dronecan_transport = f'{transport}'
             elif transport.startswith("/dev/") or transport.startswith("COM"):
                 dronecan_transport = f'slcan:{transport}'
             else:
                 print(f"Unsupported interface {transport}")
                 sys.exit(1)
```

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/dronecan/utils.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/dronecan/utils.py`

 * *Files identical despite different names*

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/common/create_pkg.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/common/create_pkg.py`

 * *Files identical despite different names*

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/common/get_info.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/common/get_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     import dronecan
     from raccoonlab_tools.dronecan.utils import NodeFinder
 
     node = dronecan.make_node(transport, node_id=100, bitrate=1000000, baudrate=1000000)
     return NodeFinder(node).get_info()
 
 def main():
-    transport = DeviceManager.get_transport(verbose=True)
+    transport = DeviceManager.get_device_port(verbose=True)
     can_protocol = CanProtocolParser.verify_protocol(transport, verbose=True)
     if can_protocol == Protocol.DRONECAN:
         node_info = get_info_dronecan(transport)
     elif can_protocol == Protocol.CYPHAL:
         node_info = asyncio.run(get_info_cyphal())
 
     if node_info is not None:
```

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/common/kek.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/common/kak.py`

 * *Files identical despite different names*

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/common/upload_firmware.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/common/upload_firmware.py`

 * *Files identical despite different names*

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/cyphal/emulate_myxa_feedback.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/cyphal/emulate_myxa_feedback.py`

 * *Files identical despite different names*

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/cyphal/monitor.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/rl_monitor/script.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # This software is distributed under the terms of the MIT License.
 # Copyright (c) 2023-2024 Dmitry Ponomarev.
 # Author: Dmitry Ponomarev <ponomarevda96@gmail.com>
 
 import os
 import sys
-import time
+import copy
 import datetime
 import math
 import asyncio
 import numpy as np
 import secrets
 
 import pycyphal.application
@@ -26,16 +26,21 @@
 import uavcan.primitive.scalar.Integer16_1_0
 import uavcan.time.SynchronizedTimestamp_1_0
 
 import reg.udral.physics.optics.HighColor_0_1
 import reg.udral.service.actuator.common.sp.Vector31_0_1
 import reg.udral.service.common.Readiness_0_1
 
+import reg.udral.physics.kinematics.geodetic.PointStateVarTs_0_1 as PointStateVarTs_0_1
+import ds015.service.gnss.Gnss_0_1
+import ds015.service.gnss.Covariance_0_1
+
+from raccoonlab_tools.scripts.rl_monitor.base_subscriber import BaseSubscriber
 from raccoonlab_tools.common.colorizer import Colorizer, Colors
-from raccoonlab_tools.cyphal.utils import NodeFinder, PortRegisterInterface
+from raccoonlab_tools.cyphal.utils import NodeFinder
 from raccoonlab_tools.common.protocol_parser import CanProtocolParser, Protocol
 
 
 class HighColorPub:
     def __init__(self, node : pycyphal.application._node_factory.SimpleNode, node_id : int) -> None:
         assert isinstance(node, pycyphal.application._node_factory.SimpleNode)
         assert isinstance(node_id, int)
@@ -58,62 +63,14 @@
         self.msg.blue  = self.blue  % 32 if self.blue  % 64  < 32 else 63 -  self.blue  % 64
         print("Lights:")
         print(f"- HighColor: red={self.msg.red}, green={self.msg.green}, blue={self.msg.blue}")
         self._pub_counter += 1
         await self._pub.publish(self.msg)
 
 
-class BaseSubscriber:
-    def __init__(self,
-                 node : pycyphal.application._node_factory.SimpleNode,
-                 node_id : int,
-                 def_id : int,
-                 reg_name : str,
-                 data_type) -> None:
-        assert isinstance(node, pycyphal.application._node_factory.SimpleNode)
-        assert isinstance(node_id, int)
-        assert isinstance(def_id, int)
-        assert isinstance(reg_name, str) or isinstance(reg_name, tuple)
-        self.node = node
-        self.data = None
-        self._id = None
-        self.id_updated = False
-        self.node_id = node_id
-        self.def_id = def_id
-        self.reg_names = reg_name if isinstance(reg_name, tuple) else (reg_name, )
-        self.data_type = data_type
-        self.port_interface = PortRegisterInterface(self.node)
-    async def init_sub(self):
-        for reg_name in self.reg_names:
-            self._id = await self.port_interface.get_id(self.node_id, reg_name)
-            print(f"y r {self.node_id} {reg_name} # {self._id}")
-            if self._id is not None:
-                break
-        if self._id is None:
-            print(f"[WARN] {self.reg_names} is not exist")
-            return
-
-        self.id_updated = (self._id == 0) or (self._id > 8191)
-
-        if self.id_updated:
-            self._id = await self.port_interface.set_id(self.node_id, reg_name, self.def_id)
-        assert isinstance(self._id, int), reg_name
-        self.sub = self.node.make_subscriber(self.data_type, self._id).receive_in_background(self.callback)
-
-    async def callback(self, data, transfer_from):
-        self.data = data
-        self._transfer_from = transfer_from
-    def get_id_string(self):
-        if not self.id_updated:
-            string =  str(self._id)
-        else:
-            toggle = bool(int(time.time() * 1000) % 1000 > 500)
-            string =  f"{Colors.OKCYAN}{self._id}{Colors.ENDC}" if toggle else str(self._id)
-        return string
-
 class CircuitStatusTemperatureSub(BaseSubscriber):
     def __init__(self,
                  node,
                  node_id,
                  def_id=2102,
                  reg_name=("uavcan.pub.crct.temp.id", "uavcan.pub.crct.temperature.id")) -> None:
         super().__init__(node, node_id, def_id, reg_name, uavcan.si.sample.temperature.Scalar_1_0)
@@ -139,75 +96,163 @@
         assert isinstance(node, pycyphal.application._node_factory.SimpleNode)
         assert isinstance(node_id, int)
         super().__init__(node, node_id, def_id, reg_name, uavcan.si.sample.voltage.Scalar_1_0)
     def print_data(self):
         volt = None if self.data is None else round(self.data.volt, 2)
         print(f"- crct.vin ({self.get_id_string()}): {volt} Volt")
 
-class GpsSatsSub(BaseSubscriber):
-    def __init__(self, node, node_id, def_id=2001, reg_name="uavcan.pub.zubax.gps.sats.id") -> None:
-        super().__init__(node, node_id, def_id, reg_name, uavcan.primitive.scalar.Integer16_1_0)
+GPS_DEF_PORTS = {
+    'cov': 2405,
+    'point': 2406,
+    'sats': 2407,
+    'status': 2408,
+    'pdop': 2409,
+}
+
+class ZubaxGpsPointSub(BaseSubscriber):
+    def __init__(self, node, node_id, def_id=GPS_DEF_PORTS['point'], reg_name="uavcan.pub.zubax.gps.point.id") -> None:
+        super().__init__(node, node_id, def_id, reg_name, PointStateVarTs_0_1)
+        self.str_data_type = "reg.udral.physics.kinematics.geodetic.PointStateVarTs.0.1"
     def print_data(self):
         print("GNSS:")
+        print(f"- zubax.gps.point ({self.get_id_string()}:{self.str_data_type}, {self.rate()} msg/sec)")
+
+class ZubaxGpsSatsSub(BaseSubscriber):
+    def __init__(self, node, node_id, def_id=GPS_DEF_PORTS['sats'], reg_name="uavcan.pub.zubax.gps.sats.id") -> None:
+        super().__init__(node, node_id, def_id, reg_name, uavcan.primitive.scalar.Integer16_1_0)
+        self.str_data_type = "uavcan.primitive.scalar.Integer16.1.0"
+    def print_data(self):
         value = self.data.value if self.data is not None else None
         if value == 0:
             value = Colorizer.header(value)
-        print(f"- sats ({self.get_id_string()}): {value}")
-        print("- lat:")
-        print("- lon:")
+        print(f"- zubax.gps.sats ({self.get_id_string()}:{self.str_data_type}, {self.rate()} msg/sec): {value}")
+
+class ZubaxGpsPdopSub(BaseSubscriber):
+    def __init__(self, node, node_id, def_id=GPS_DEF_PORTS['pdop'], reg_name="uavcan.pub.zubax.gps.pdop.id") -> None:
+        super().__init__(node, node_id, def_id, reg_name, uavcan.primitive.scalar.Real32_1_0)
+    def print_data(self):
+        value = self.data.value if self.data is not None else 0.0
+        print(f"- zubax.gps.pdop ({self.get_id_string()}:uavcan.primitive.scalar.Integer16.1.0): {value:.2f}")
+
+class ZubaxGpsStatusSub(BaseSubscriber):
+    def __init__(self, node, node_id, def_id=GPS_DEF_PORTS['status'], reg_name="uavcan.pub.zubax.gps.status.id") -> None:
+        super().__init__(node, node_id, def_id, reg_name, uavcan.primitive.scalar.Integer16_1_0)
+    def print_data(self):
+        value = self.data.value if self.data is not None else None
+        INT_TO_STR = {
+            0 : "NO FIX (0)",
+            1 : "TIME_ONLY (1)",
+            2 : "2D_FIX (2)",
+            3 : "3D_FIX (3)",
+        }
+        if value in INT_TO_STR:
+            value = INT_TO_STR[value]
+        print(f"- zubax.gps.status ({self.get_id_string()}:uavcan.primitive.scalar.Integer16.1.0, {self.rate()} msg/sec): {value}")
+
+class DS015GpsGnssSub(BaseSubscriber):
+    def __init__(self, node, node_id, def_id=2005, reg_name="uavcan.pub.ds015.gps.gnss.id") -> None:
+        super().__init__(node, node_id, def_id, reg_name, ds015.service.gnss.Gnss_0_1)
+    def print_data(self):
+        SPOOFING_INT_TO_STR = {
+            0 : "UNKNOWN (0)",
+            1 : "NO_SPOOFING_INDICATED (1)",
+            2 : "SPOOFING_INDICATED (2)",
+            3 : "MULTIPLE_SPOOFING_INDICATIONS (3)",
+        }
+        try:
+            jamming_state = self.data.status.jamming_state
+            spoofing_state = SPOOFING_INT_TO_STR.get(self.data.status.spoofing_state)
+        except Exception as err:
+            jamming_state = err
+            spoofing_state = "err2"
+
+        print(f"- ds015.gps.gnss ({self.get_id_string()}:ds015.service.gnss.Gnss.0.1, {self.rate()} msg/sec):\n"
+              f"    alt {self.data.point.altitude.meter:.2f} (from {self.min.point.altitude.meter:.2f} to {self.max.point.altitude.meter:.2f})\n"
+              f"    hdop {self.data.hdop:.2f} (from {self.min.hdop:.2f} to {self.max.hdop:.2f})\n"
+              f"    vdop {self.data.vdop:.2f} (from {self.min.vdop:.2f} to {self.max.vdop:.2f})\n"
+              f"    eph {self.data.horizontal_accuracy:.2f} (from {self.min.horizontal_accuracy:.2f} to {self.max.horizontal_accuracy:.2f})\n"
+              f"    epv {self.data.vertical_accuracy:.2f} (from {self.min.vertical_accuracy:.2f} to {self.max.vertical_accuracy:.2f})\n"
+              f"    jamming_state {jamming_state}\n"
+              f"    spoofing_state {spoofing_state}"
+        )
+
+class DS015GpsCovSub(BaseSubscriber):
+    def __init__(self, node, node_id, def_id=GPS_DEF_PORTS['cov'], reg_name="uavcan.pub.ds015.gps.cov.id") -> None:
+        super().__init__(node, node_id, def_id, reg_name, ds015.service.gnss.Covariance_0_1)
+    def print_data(self):
+        print(f"- ds015.gps.cov ({self.get_id_string()}:ds015.service.gnss.Covariance.0.1, {self.rate()} msg/sec):")
+        try:
+            pos = self.data.point_covariance_urt
+            vel = self.data.velocity_covariance_urt
+            print(
+                "  Position NED [m^2]                  Velocity NED [m^2/s^2]\n"
+                f"  {pos[0]:>10,.3E} {pos[1]:>10,.3E} {pos[2]:>10,.3E}  "
+                f"  {vel[0]:>10,.3E} {vel[1]:>10,.3E} {vel[2]:>10,.3E}\n"
+                f"  {pos[1]:>10,.3E} {pos[3]:>10,.3E} {pos[4]:>10,.3E}  "
+                f"  {vel[1]:>10,.3E} {vel[3]:>10,.3E} {vel[4]:>10,.3E}\n"
+                f"  {pos[2]:>10,.3E} {pos[4]:>10,.3E} {pos[5]:>10,.3E}  "
+                f"  {vel[2]:>10,.3E} {vel[4]:>10,.3E} {vel[5]:>10,.3E}"
+            )
+        except Exception:
+            pass
 
 class GpsTimeUtcSub(BaseSubscriber):
     def __init__(self, node, node_id, def_id=2002, reg_name="uavcan.pub.gps.time_utc.id") -> None:
         super().__init__(node, node_id, def_id, reg_name, uavcan.time.SynchronizedTimestamp_1_0)
     def print_data(self):
         seconds = int(self.data.microsecond / 1000000) if self.data is not None else 0
         print(f"- time_utc ({self.get_id_string()}): {seconds} ({datetime.datetime.fromtimestamp(seconds)})")
 
 class MagnetometerSub(BaseSubscriber):
     def __init__(self, node, node_id, def_id=2000, reg_name="uavcan.pub.zubax.mag.id") -> None:
         super().__init__(node, node_id, def_id, reg_name, uavcan.si.sample.magnetic_field_strength.Vector3_1_1)
         self.data = None
     def print_data(self):
+        print("MagneticFieldStrength:")
         if self.data is not None:
-            print(f"Magnetometer zubax.mag ({self.get_id_string()}):")
+            print(f"- zubax.mag ({self.get_id_string()}:uavcan.si.sample.magnetic_field_strength.Vector3.1.1, {self.rate()} msg/sec):")
             mag_field = self.data.ampere_per_meter.tolist()
-            print(f"- norm: {np.sqrt(np.sum(np.array(mag_field)**2)):.3f} Amper/meter")
-            print(f"- x: {mag_field[0]:.3f} Amper/meter")
-            print(f"- y: {mag_field[1]:.3f} Amper/meter")
-            print(f"- z: {mag_field[1]:.3f} Amper/meter")
+            print(f"   Norm: {np.sqrt(np.sum(np.array(mag_field)**2)):.3f} A/m")
+            print(f"   x: {mag_field[0]:.3f} A/m")
+            print(f"   y: {mag_field[1]:.3f} A/m")
+            print(f"   z: {mag_field[2]:.3f} A/m")
         else:
-            print(f"Magnetometer ({self.get_id_string()}) : {Colors.WARNING}NO DATA{Colors.ENDC}")
+            print(f"{Colors.WARNING}NO DATA{Colors.ENDC}")
 
 class BaroPressureSub(BaseSubscriber):
     def __init__(self, node, node_id, def_id=2100, reg_name="uavcan.pub.zubax.baro.press.id") -> None:
         super().__init__(node, node_id, def_id, reg_name, uavcan.si.sample.pressure.Scalar_1_0)
     def print_data(self):
         print("Barometer:")
         value = self.data.pascal if self.data is not None else 0.0
-        print(f"- zubax.baro.press ({self.get_id_string()}): {value:.2f} Pascal")
+        print(f"- zubax.baro.press ({self.get_id_string()}:uavcan.si.sample.pressure.Scalar_1.0, {self.rate()} msg/sec): {value:.2f} Pascal")
 
 class BaroTemperatureSub(BaseSubscriber):
     def __init__(self, node, node_id, def_id=2101, reg_name="uavcan.pub.zubax.baro.temp.id") -> None:
         super().__init__(node, node_id, def_id, reg_name, uavcan.si.sample.temperature.Scalar_1_0)
     def print_data(self):
         value = self.data.kelvin if self.data is not None else 0.0
-        print(f"- zubax.baro.temp ({self.get_id_string()}): {value:.2f} Kelvin")
+        print(f"- zubax.baro.temp ({self.get_id_string()}:uavcan.si.sample.temperature.Scalar_1.0, {self.rate()} msg/sec): {value:.2f} Kelvin")
 
 class SetpointSub(BaseSubscriber):
     def __init__(self, node, node_id, def_id=2342, reg_name="uavcan.pub.udral.esc.0.id") -> None:
         super().__init__(node, node_id, def_id, reg_name, reg.udral.service.actuator.common.sp.Vector31_0_1)
         self.max_recv_length = 0
     def print_data(self):
-        for idx in range(30, self.max_recv_length - 1, -1):
-            is_zero = math.isclose(self.data.value[idx], 0.0, rel_tol=1e-5)
-            if not is_zero:
-                self.max_recv_length = idx + 1
-                break
         print("Actuators:")
-        print(f"- udral.esc.0 ({self.get_id_string()}): {self.data.value[0:self.max_recv_length]}")
+        if self.data is None:
+            data = "NO DATA"
+        else:
+            for idx in range(30, self.max_recv_length - 1, -1):
+                is_zero = math.isclose(self.data.value[idx], 0.0, rel_tol=1e-5)
+                if not is_zero:
+                    self.max_recv_length = idx + 1
+                    break
+            data = self.data.value[0:self.max_recv_length]
+        print(f"- udral.esc.0 ({self.get_id_string()}): {data}")
 
 class ReadinessSub(BaseSubscriber):
     def __init__(self, node, node_id, def_id=2343, reg_name="uavcan.pub.udral.readiness.0.id") -> None:
         super().__init__(node, node_id, def_id, reg_name, reg.udral.service.common.Readiness_0_1)
         self.max_recv_length = 0
     def print_data(self):
         mapping = {
@@ -250,15 +295,20 @@
 
 
 class GpsMagBaroMonitor(BaseMonitor):
     def __init__(self, node : pycyphal.application._node_factory.SimpleNode, node_id : int) -> None:
         super().__init__(node, node_id)
 
         self.subs = [
-            GpsSatsSub(node, node_id),
+            ZubaxGpsPointSub(node, node_id),
+            ZubaxGpsSatsSub(node, node_id),
+            ZubaxGpsPdopSub(node, node_id),
+            ZubaxGpsStatusSub(node, node_id),
+            DS015GpsGnssSub(node, node_id),
+            DS015GpsCovSub(node, node_id),
             GpsTimeUtcSub(node, node_id),
             MagnetometerSub(node, node_id),
             BaroPressureSub(node, node_id),
             BaroTemperatureSub(node, node_id)
         ]
 
     @staticmethod
```

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/cyphal/test_specification.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/cyphal/test_specification.py`

 * *Files identical despite different names*

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/cyphal/ublox_center.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/cyphal/ublox_center.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             logging.error("GNSS node: %s is not configured.", CyphalGnss.UBX_TX_REG)
             config_required = True
 
         if config_required and attempts_left > 0:
             logging.info("Let's try to configure the registers, Attempts left = %s", attempts_left)
             await port_interface.set_id(gnss_id, CyphalGnss.UBX_RX_REG, 4000)
             await port_interface.set_id(gnss_id, CyphalGnss.UBX_TX_REG, 4001)
-            return CyphalGnss.create(node, gnss_id, attempts_left - 1)
+            return await CyphalGnss.create(node, gnss_id, attempts_left - 1)
 
         return CyphalGnss(node, fragment_pub_port_id, fragment_sub_port_id)
 
     def __init__(self, cyphal_node, fragment_pub_port_id : int, fragment_sub_port_id : int) -> None:
         assert isinstance(fragment_pub_port_id, int)
         assert isinstance(fragment_sub_port_id, int)
         self._fragment_pub = CyphalFragmentPub(cyphal_node, fragment_pub_port_id)
```

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/dronecan/config.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 def configure_parameters(config : dict, can_transport : str):
     if 'params' not in config or config['params'] is None:
         print("[WARN] Config file doesn't have parameters. Skip the configuration.")
         return
 
     if can_transport is None:
-        can_transport = f'slcan:{DeviceManager.get_transport()}'
+        can_transport = f'slcan:{DeviceManager.get_device_port()}'
 
     node = dronecan.make_node(can_transport, node_id=100, bitrate=1000000, baudrate=1000000)
     target_node_id = NodeFinder(node).find_online_node()
     params_interface = ParametersInterface(node=node, target_node_id=target_node_id)
     commander = NodeCommander(node=node, target_node_id=target_node_id)
     for name in config['params']:
         desired_param = Parameter(name=name, value=config['params'][name])
@@ -36,15 +36,15 @@
         print(param_after_change)
 
     print(f"[INFO] Save persistent parameters: {commander.store_persistent_states()}")
     print(f"[INFO] Reboot: {commander.restart()}")
 
 def main():
     parser = argparse.ArgumentParser()
-    parser.add_argument('--config', required=True, help="path to yaml file")
+    parser.add_argument('config', help="path to yaml file")
     parser.add_argument('--can-transport', default=None, help=("Auto detect by default. Options: "
                                                                "slcan:/dev/ttyACM0, "
                                                                "socketcan:slcan0.")
     )
     args = parser.parse_args()
 
     with open(args.config, "r", encoding='UTF-8') as stream:
```

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/dronecan/get_params.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/get_params.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (c) 2024 Dmitry Ponomarev.
 # Author: Dmitry Ponomarev <ponomarevda96@gmail.com>
 import dronecan
 from raccoonlab_tools.dronecan.utils import ParametersInterface, NodeFinder
 from raccoonlab_tools.common.device_manager import DeviceManager
 
 def main():
-    can_transport = f'slcan:{DeviceManager.get_transport()}'
+    can_transport = DeviceManager.get_dronecan_can_iface()
 
     node = dronecan.make_node(can_transport, node_id=100, bitrate=1000000, baudrate=1000000)
     target_node_id = NodeFinder(node).find_online_node()
     params_interface = ParametersInterface(node=node, target_node_id=target_node_id)
     all_params = params_interface.get_all()
     for param in all_params:
         print(param)
```

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/dronecan/lights_tester/lights_tester.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/lights_tester/lights_tester.py`

 * *Files identical despite different names*

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/dronecan/servo_tester/node_parser.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/servo_tester/node_parser.py`

 * *Files identical despite different names*

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/dronecan/servo_tester/servo_tester.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/servo_tester/servo_tester.py`

 * *Files identical despite different names*

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/dronecan/set_params.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/set_params.py`

 * *Files identical despite different names*

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/dronecan/sim_battery/sim_battery.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/sim_battery/sim_battery.py`

 * *Files identical despite different names*

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/dronecan/test_gps_mag_baro.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/test_gps_mag_baro.py`

 * *Files identical despite different names*

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/dronecan/test_lights.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/test_lights.py`

 * *Files identical despite different names*

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/dronecan/test_pwm_node.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/test_pwm_node.py`

 * *Files identical despite different names*

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools/scripts/dronecan/test_specification.py` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools/scripts/dronecan/test_specification.py`

 * *Files identical despite different names*

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools.egg-info/PKG-INFO` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raccoonlab-tools
-Version: 0.0.18
+Version: 0.1.0
 Summary: RaccoonLab tools
 Author-email: Dmitry Ponomarev <PonomarevDA96@gmail.com>
 Project-URL: Homepage, https://github.com/PonomarevDA/tools
 Project-URL: Bug Tracker, https://github.com/PonomarevDA/tools/issues
 Keywords: cyphal,dronecan,can
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -73,26 +73,34 @@
 | UAVCAN__CAN__BITRATE | Arbitration/data segment bits per second |
 | UAVCAN__CAN__MTU     | Maximum transmission unit: 8 for classic CAN |
 
 > Check pycyphal/yakut/yukon docs for additional details
 
 </details>
 
-## 2. LINUX PREPARATION (SOCKETCAN)
+## 2. LINUX (SOCKETCAN)
 
 By default, DroneCAN and Cyphal/CAN uses cross-platform transport interface [Python-CAN](https://python-can.readthedocs.io/en/stable/) [CAN over Serial / SLCAN](https://python-can.readthedocs.io/en/stable/interfaces/slcan.html).
 
 On Linux, [the socketcan interface](https://python-can.readthedocs.io/en/stable/interfaces/socketcan.html) is recommended. Unlike SLCAN, socketcan interface allows to share the same CAN interface with multiple processes, so you can run a few pycyphal scripts, yukon, yakut simultaniously.
 
 You can run the following script:
 
 ```bash
 ./scripts/socketcan.sh
 ```
 
+If you don't have a real CAN device, you can create a virtual CAN interface:
+
+```bash
+./scripts/socketcan.sh --virtual-can
+```
+
+Try `--help` option for more details.
+
 For a Cyphal application after creating socketcan interface, you need to update `UAVCAN__CAN__IFACE` environment variable. Just call `source ~/.bashrc`.
 
 ## 3. USAGE
 
 ### 1. Test cyphal specification
 
 ```bash
```

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools.egg-info/SOURCES.txt` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -8,37 +8,47 @@
 src/raccoonlab_tools.egg-info/entry_points.txt
 src/raccoonlab_tools.egg-info/requires.txt
 src/raccoonlab_tools.egg-info/top_level.txt
 src/raccoonlab_tools/common/colorizer.py
 src/raccoonlab_tools/common/device_manager.py
 src/raccoonlab_tools/common/firmware_manager.py
 src/raccoonlab_tools/common/node.py
-src/raccoonlab_tools/common/printer.py
 src/raccoonlab_tools/common/protocol_parser.py
 src/raccoonlab_tools/cyphal/fragments.py
 src/raccoonlab_tools/cyphal/gnss.py
 src/raccoonlab_tools/cyphal/utils.py
 src/raccoonlab_tools/dronecan/global_node.py
 src/raccoonlab_tools/dronecan/utils.py
 src/raccoonlab_tools/scripts/common/check_protocol.py
 src/raccoonlab_tools/scripts/common/create_pkg.py
 src/raccoonlab_tools/scripts/common/create_slcan.py
-src/raccoonlab_tools/scripts/common/get_can_iface.py
 src/raccoonlab_tools/scripts/common/get_info.py
+src/raccoonlab_tools/scripts/common/kak.py
 src/raccoonlab_tools/scripts/common/kek.py
 src/raccoonlab_tools/scripts/common/parse_pytest_res_json.py
 src/raccoonlab_tools/scripts/common/upload_firmware.py
 src/raccoonlab_tools/scripts/cyphal/emulate_myxa_feedback.py
-src/raccoonlab_tools/scripts/cyphal/monitor.py
 src/raccoonlab_tools/scripts/cyphal/test_specification.py
 src/raccoonlab_tools/scripts/cyphal/ublox_center.py
+src/raccoonlab_tools/scripts/dronecan/beep.py
 src/raccoonlab_tools/scripts/dronecan/config.py
 src/raccoonlab_tools/scripts/dronecan/get_params.py
+src/raccoonlab_tools/scripts/dronecan/ramil.py
 src/raccoonlab_tools/scripts/dronecan/set_params.py
+src/raccoonlab_tools/scripts/dronecan/test_circuit_status.py
 src/raccoonlab_tools/scripts/dronecan/test_gps_mag_baro.py
 src/raccoonlab_tools/scripts/dronecan/test_lights.py
+src/raccoonlab_tools/scripts/dronecan/test_pmu_buzzer.py
 src/raccoonlab_tools/scripts/dronecan/test_pwm_node.py
 src/raccoonlab_tools/scripts/dronecan/test_specification.py
+src/raccoonlab_tools/scripts/dronecan/buzzer_tester/test_buzzer.py
 src/raccoonlab_tools/scripts/dronecan/lights_tester/lights_tester.py
+src/raccoonlab_tools/scripts/dronecan/pwm_tester/pwm_tester.py
 src/raccoonlab_tools/scripts/dronecan/servo_tester/node_parser.py
 src/raccoonlab_tools/scripts/dronecan/servo_tester/servo_tester.py
-src/raccoonlab_tools/scripts/dronecan/sim_battery/sim_battery.py
+src/raccoonlab_tools/scripts/dronecan/sim_battery/sim_battery.py
+src/raccoonlab_tools/scripts/rl_git_info/script.py
+src/raccoonlab_tools/scripts/rl_monitor/base_subscriber.py
+src/raccoonlab_tools/scripts/rl_monitor/script.py
+src/raccoonlab_tools/scripts/rl_printer/script.py
+src/raccoonlab_tools/scripts/stm32/build_cubeide.py
+src/raccoonlab_tools/scripts/stm32/test_ioc.py
```

### Comparing `raccoonlab-tools-0.0.18/src/raccoonlab_tools.egg-info/entry_points.txt` & `raccoonlab_tools-0.1.0/src/raccoonlab_tools.egg-info/entry_points.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 [console_scripts]
+rl-build-stm32-cubeide = raccoonlab_tools.scripts.stm32.build_cubeide:main
 rl-config = raccoonlab_tools.scripts.dronecan.config:main
-rl-get-can-iface = raccoonlab_tools.scripts.common.get_can_iface:main
+rl-get-cyphal-can-iface = raccoonlab_tools.common.device_manager:print_cyphal_can_iface
 rl-get-dronecan-params = raccoonlab_tools.scripts.dronecan.get_params:main
 rl-get-info = raccoonlab_tools.scripts.common.get_info:main
-rl-monitor = raccoonlab_tools.scripts.cyphal.monitor:main
+rl-git-info = raccoonlab_tools.scripts.rl_git_info.script:main
+rl-monitor = raccoonlab_tools.scripts.rl_monitor.script:main
 rl-set-dronecan-params = raccoonlab_tools.scripts.dronecan.set_params:main
+rl-stm32-test-ioc = raccoonlab_tools.scripts.stm32.test_ioc:main
 rl-test-cyphal-specification = raccoonlab_tools.scripts.cyphal.test_specification:main
 rl-test-dronecan-gps-mag-baro = raccoonlab_tools.scripts.dronecan.test_gps_mag_baro:main
 rl-test-dronecan-lights = raccoonlab_tools.scripts.dronecan.test_lights:main
 rl-test-dronecan-specification = raccoonlab_tools.scripts.dronecan.test_specification:main
 rl-ublox-center = raccoonlab_tools.scripts.cyphal.ublox_center:main
 rl-upload-firmware = raccoonlab_tools.scripts.common.upload_firmware:main
```

