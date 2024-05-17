# Comparing `tmp/TDSR-UWB-1.539.tar.gz` & `tmp/TDSR-UWB-1.540.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TDSR-UWB-1.539.tar", last modified: Thu May 16 03:42:37 2024, max compression
+gzip compressed data, was "TDSR-UWB-1.540.tar", last modified: Thu May 16 22:37:25 2024, max compression
```

## Comparing `TDSR-UWB-1.539.tar` & `TDSR-UWB-1.540.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-16 03:42:37.205335 TDSR-UWB-1.539/
--rw-rw-r--   0 senter    (1000) senter    (1000)       74 2024-05-09 23:00:07.000000 TDSR-UWB-1.539/LICENSE.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       37 2024-05-09 21:21:05.000000 TDSR-UWB-1.539/MANIFEST.in
--rw-rw-r--   0 senter    (1000) senter    (1000)      748 2024-05-16 03:42:37.205335 TDSR-UWB-1.539/PKG-INFO
--rw-rw-r--   0 senter    (1000) senter    (1000)       93 2024-05-09 23:01:32.000000 TDSR-UWB-1.539/README.md
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-16 03:42:37.201335 TDSR-UWB-1.539/TDSR-UWB/
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-16 03:42:37.201335 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-16 03:42:37.205335 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/
--rw-rw-r--   0 senter    (1000) senter    (1000)     6148 2023-03-30 19:11:25.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/.DS_Store
--rw-rw-r--   0 senter    (1000) senter    (1000)      161 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/.txt
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-16 03:42:37.205335 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/
--rw-rw-r--   0 senter    (1000) senter    (1000)      536 2023-03-02 20:09:11.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/launch.json
--rw-rw-r--   0 senter    (1000) senter    (1000)     9479 2023-02-26 18:51:27.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/API.md
--rw-rw-r--   0 senter    (1000) senter    (1000)     5515 2022-12-23 02:15:12.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/API.template.md
--rw-rw-r--   0 senter    (1000) senter    (1000)     5563 2022-12-23 02:08:30.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/APIwith_cat_template.md
--rw-rw-r--   0 senter    (1000) senter    (1000)       45 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/DATA_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      124 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/DATA_INFO.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      144 2023-08-10 03:26:43.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/DATA_REQUEST.txt
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-16 03:42:37.205335 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/Doc/
--rw-rw-r--   0 senter    (1000) senter    (1000)    12524 2022-10-06 21:41:33.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/Doc/TDSR_logo_250x134.png
--rw-rw-r--   0 senter    (1000) senter    (1000)      405 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_SLOT_MAP_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       50 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_SLOT_MAP_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      411 2023-03-30 02:12:35.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_STATS_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       47 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_STATS_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       64 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_SET_SLOT_MAP_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      405 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_SET_SLOT_MAP_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      111 2023-05-16 19:39:21.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/NET_DATA_QUEUE_STATUS_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       93 2023-05-16 19:38:24.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/NET_DATA_QUEUE_STATUS_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       61 2024-03-13 14:34:07.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_APPLY_PRESET_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       91 2024-03-13 02:20:50.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_APPLY_PRESET_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       62 2024-03-13 14:31:51.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_DELETE_PRESET_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       75 2024-03-13 02:21:52.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_DELETE_PRESET_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       75 2024-03-16 16:10:28.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_ACTIVE_PRESET_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       51 2024-03-16 16:10:10.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_ACTIVE_PRESET_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      228 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONFIG_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONFIG_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       44 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONNECT_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       41 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_INFO_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       41 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_INFO_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      143 2024-03-13 14:30:56.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_IP_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       40 2024-03-13 01:42:44.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_IP_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       77 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_NODE_CONFIG_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_NODE_CONFIG_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      379 2024-03-14 17:35:25.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_PRESET_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       72 2024-03-14 17:30:36.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_PRESET_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      120 2023-05-15 23:46:31.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATE_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       42 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATE_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      550 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       40 2022-12-20 14:51:26.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      136 2023-09-28 14:06:18.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_TUNING_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       43 2023-09-28 14:06:22.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_TUNING_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      173 2024-03-13 14:33:30.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_LIST_PRESETS_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       46 2024-03-13 02:21:17.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_LIST_PRESETS_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       61 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_MESSAGE_ERROR.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       53 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_REBOOT_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       39 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_REBOOT_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       60 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_RESET_FACTORY_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       46 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_RESET_FACTORY_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       60 2024-03-13 14:32:21.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SAVE_PRESET_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       87 2024-03-13 02:21:36.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SAVE_PRESET_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONFIG_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      228 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONFIG_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      138 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONNECT_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       55 2024-03-13 14:35:17.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_IP_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      116 2024-03-13 02:22:22.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_IP_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       62 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_NODE_CONFIG_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       77 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_NODE_CONFIG_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       56 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATE_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      184 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATE_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATS_CLEAR_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATS_CLEAR_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-09-28 14:06:26.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_TUNING_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      136 2023-09-28 14:06:29.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_TUNING_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      348 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_INFO.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_SEND_RANGE_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       81 2023-05-16 19:37:46.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_SEND_RANGE_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)    12521 2023-03-30 01:57:06.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/networking.md
--rw-rw-r--   0 senter    (1000) senter    (1000)   107545 2023-03-30 01:57:24.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/networking.pdf
--rw-rw-r--   0 senter    (1000) senter    (1000)     9971 2023-03-30 01:57:02.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/networking.template.md
--rw-rw-r--   0 senter    (1000) senter    (1000)     6747 2023-03-04 15:21:05.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/networking_.md
--rw-rw-r--   0 senter    (1000) senter    (1000)      157 2022-12-08 14:50:04.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/processJSONFiles.sh
--rw-rw-r--   0 senter    (1000) senter    (1000)     1097 2023-03-02 20:30:55.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/updateReadme.py
--rw-rw-r--   0 senter    (1000) senter    (1000)   253692 2024-05-16 02:50:22.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/TDSR_PW_GUI.py
--rw-rw-r--   0 senter    (1000) senter    (1000)     6303 2024-05-16 03:29:42.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/TDSR_logging.py
--rw-rw-r--   0 senter    (1000) senter    (1000)    14427 2024-05-16 01:41:06.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/TDSR_radioAPI.py
--rw-rw-r--   0 senter    (1000) senter    (1000)    19213 2024-05-16 03:23:03.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/TDSR_radioConnection.py
--rw-rw-r--   0 senter    (1000) senter    (1000)    83453 2024-05-16 01:43:15.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/TDSR_radioControl.py
--rw-rw-r--   0 senter    (1000) senter    (1000)     3982 2024-05-16 01:40:01.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/TDSR_settings.py
--rw-rw-r--   0 senter    (1000) senter    (1000)        0 2024-05-08 17:38:57.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/__init__.py
--rw-rw-r--   0 senter    (1000) senter    (1000)     2912 2022-12-27 01:25:43.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/crc16.py
--rw-rw-r--   0 senter    (1000) senter    (1000)     2280 2024-05-16 03:20:39.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/logReader.py
--rw-rw-r--   0 senter    (1000) senter    (1000)      376 2024-04-15 16:19:41.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/logReader_Minimal.py
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-16 03:42:37.205335 TDSR-UWB-1.539/TDSR-UWB/TDSR_UWB.egg-info/
--rw-rw-r--   0 senter    (1000) senter    (1000)      748 2024-05-16 03:42:37.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_UWB.egg-info/PKG-INFO
--rw-rw-r--   0 senter    (1000) senter    (1000)     4735 2024-05-16 03:42:37.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_UWB.egg-info/SOURCES.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)        1 2024-05-16 03:42:37.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_UWB.egg-info/dependency_links.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       62 2024-05-16 03:42:37.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_UWB.egg-info/requires.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       13 2024-05-16 03:42:37.000000 TDSR-UWB-1.539/TDSR-UWB/TDSR_UWB.egg-info/top_level.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       38 2024-05-16 03:42:37.205335 TDSR-UWB-1.539/setup.cfg
--rw-rw-r--   0 senter    (1000) senter    (1000)     7693 2024-05-16 03:35:34.000000 TDSR-UWB-1.539/setup.py
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-16 22:37:25.888751 TDSR-UWB-1.540/
+-rw-rw-r--   0 senter    (1000) senter    (1000)       74 2024-05-09 23:00:07.000000 TDSR-UWB-1.540/LICENSE.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       37 2024-05-09 21:21:05.000000 TDSR-UWB-1.540/MANIFEST.in
+-rw-rw-r--   0 senter    (1000) senter    (1000)      748 2024-05-16 22:37:25.888751 TDSR-UWB-1.540/PKG-INFO
+-rw-rw-r--   0 senter    (1000) senter    (1000)       93 2024-05-09 23:01:32.000000 TDSR-UWB-1.540/README.md
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-16 22:37:25.884751 TDSR-UWB-1.540/TDSR-UWB/
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-16 22:37:25.884751 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-16 22:37:25.888751 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/
+-rw-rw-r--   0 senter    (1000) senter    (1000)     6148 2023-03-30 19:11:25.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/.DS_Store
+-rw-rw-r--   0 senter    (1000) senter    (1000)      161 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/.txt
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-16 22:37:25.888751 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/
+-rw-rw-r--   0 senter    (1000) senter    (1000)      536 2023-03-02 20:09:11.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/launch.json
+-rw-rw-r--   0 senter    (1000) senter    (1000)     9479 2023-02-26 18:51:27.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/API.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)     5515 2022-12-23 02:15:12.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/API.template.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)     5563 2022-12-23 02:08:30.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/APIwith_cat_template.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)       45 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/DATA_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      124 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/DATA_INFO.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      144 2023-08-10 03:26:43.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/DATA_REQUEST.txt
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-16 22:37:25.888751 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/Doc/
+-rw-rw-r--   0 senter    (1000) senter    (1000)    12524 2022-10-06 21:41:33.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/Doc/TDSR_logo_250x134.png
+-rw-rw-r--   0 senter    (1000) senter    (1000)      405 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_SLOT_MAP_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       50 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_SLOT_MAP_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      411 2023-03-30 02:12:35.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_STATS_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       47 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_STATS_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       64 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_SET_SLOT_MAP_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      405 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_SET_SLOT_MAP_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      111 2023-05-16 19:39:21.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/NET_DATA_QUEUE_STATUS_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       93 2023-05-16 19:38:24.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/NET_DATA_QUEUE_STATUS_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       61 2024-03-13 14:34:07.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_APPLY_PRESET_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       91 2024-03-13 02:20:50.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_APPLY_PRESET_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       62 2024-03-13 14:31:51.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_DELETE_PRESET_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       75 2024-03-13 02:21:52.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_DELETE_PRESET_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       75 2024-03-16 16:10:28.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_ACTIVE_PRESET_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       51 2024-03-16 16:10:10.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_ACTIVE_PRESET_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      228 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONFIG_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONFIG_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       44 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONNECT_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       41 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_INFO_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       41 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_INFO_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      143 2024-03-13 14:30:56.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_IP_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       40 2024-03-13 01:42:44.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_IP_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       77 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_NODE_CONFIG_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_NODE_CONFIG_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      379 2024-03-14 17:35:25.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_PRESET_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       72 2024-03-14 17:30:36.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_PRESET_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      120 2023-05-15 23:46:31.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATE_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       42 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATE_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      550 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       40 2022-12-20 14:51:26.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      136 2023-09-28 14:06:18.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_TUNING_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       43 2023-09-28 14:06:22.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_TUNING_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      173 2024-03-13 14:33:30.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_LIST_PRESETS_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       46 2024-03-13 02:21:17.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_LIST_PRESETS_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       61 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_MESSAGE_ERROR.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       53 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_REBOOT_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       39 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_REBOOT_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       60 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_RESET_FACTORY_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       46 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_RESET_FACTORY_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       60 2024-03-13 14:32:21.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SAVE_PRESET_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       87 2024-03-13 02:21:36.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SAVE_PRESET_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONFIG_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      228 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONFIG_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      138 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONNECT_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       55 2024-03-13 14:35:17.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_IP_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      116 2024-03-13 02:22:22.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_IP_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       62 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_NODE_CONFIG_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       77 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_NODE_CONFIG_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       56 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATE_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      184 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATE_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATS_CLEAR_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATS_CLEAR_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-09-28 14:06:26.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_TUNING_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      136 2023-09-28 14:06:29.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_TUNING_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      348 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_INFO.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_SEND_RANGE_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       81 2023-05-16 19:37:46.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_SEND_RANGE_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)    12521 2023-03-30 01:57:06.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/networking.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)   107545 2023-03-30 01:57:24.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/networking.pdf
+-rw-rw-r--   0 senter    (1000) senter    (1000)     9971 2023-03-30 01:57:02.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/networking.template.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)     6747 2023-03-04 15:21:05.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/networking_.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)      157 2022-12-08 14:50:04.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/processJSONFiles.sh
+-rw-rw-r--   0 senter    (1000) senter    (1000)     1097 2023-03-02 20:30:55.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/updateReadme.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)   256697 2024-05-16 22:30:55.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/TDSR_PW_GUI.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)     6933 2024-05-16 22:14:25.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/TDSR_logging.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)    14427 2024-05-16 14:38:35.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/TDSR_radioAPI.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)    19260 2024-05-16 22:26:23.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/TDSR_radioConnection.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)    83453 2024-05-16 14:38:20.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/TDSR_radioControl.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)     4130 2024-05-16 22:29:03.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/TDSR_settings.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)        0 2024-05-08 17:38:57.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/__init__.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)     2912 2022-12-27 01:25:43.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/crc16.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)     2280 2024-05-16 03:20:39.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/logReader.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)      376 2024-04-15 16:19:41.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/logReader_Minimal.py
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-16 22:37:25.888751 TDSR-UWB-1.540/TDSR-UWB/TDSR_UWB.egg-info/
+-rw-rw-r--   0 senter    (1000) senter    (1000)      748 2024-05-16 22:37:25.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_UWB.egg-info/PKG-INFO
+-rw-rw-r--   0 senter    (1000) senter    (1000)     4735 2024-05-16 22:37:25.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_UWB.egg-info/SOURCES.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)        1 2024-05-16 22:37:25.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_UWB.egg-info/dependency_links.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       62 2024-05-16 22:37:25.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_UWB.egg-info/requires.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       13 2024-05-16 22:37:25.000000 TDSR-UWB-1.540/TDSR-UWB/TDSR_UWB.egg-info/top_level.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       38 2024-05-16 22:37:25.888751 TDSR-UWB-1.540/setup.cfg
+-rw-rw-r--   0 senter    (1000) senter    (1000)     7693 2024-05-16 14:34:30.000000 TDSR-UWB-1.540/setup.py
```

### Comparing `TDSR-UWB-1.539/PKG-INFO` & `TDSR-UWB-1.540/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDSR-UWB
-Version: 1.539
+Version: 1.540
 Summary: Support libraries for TDSR LLC UWB Radios
 Home-page: UNKNOWN
 Author: TDSR-LLC
 Author-email: contact@tdsr-uwb.com
 License: UNKNOWN
 Project-URL: Company:, https://www.tdsr-uwb.com
 Platform: UNKNOWN
```

### Comparing `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/.DS_Store` & `TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/.DS_Store`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/launch.json` & `TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/API.md` & `TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/API.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/API.template.md` & `TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/API.template.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/APIwith_cat_template.md` & `TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/APIwith_cat_template.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/Doc/TDSR_logo_250x134.png` & `TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/Doc/TDSR_logo_250x134.png`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_CONFIRM.txt` & `TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_CONFIRM.txt`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/networking.md` & `TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/networking.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/networking.pdf` & `TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/networking.pdf`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/networking.template.md` & `TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/networking.template.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/networking_.md` & `TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/networking_.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/JsonDoc/updateReadme.py` & `TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/JsonDoc/updateReadme.py`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/TDSR_PW_GUI.py` & `TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/TDSR_PW_GUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,44 +5,48 @@
 from pyqtgraph import PlotWidget, mkPen
 from pathlib import Path
 from time import time, sleep
 
 from json import loads, dumps
 from os import path
 from glob import glob
+from sys import platform
 
 from TDSR_Support import TDSR_logging
 from TDSR_Support import TDSR_settings
 from TDSR_Support import TDSR_radioControl
 from TDSR_Support import TDSR_radioConnection
 
 # Primary window GUI class. All sub windows are launched from here as well.
-__version__ = "1.539"
+__version__ = "1.540"
 # Primary application window and GUI
 class MainWindow(QMainWindow):
     def __init__(self, app, *args, **kwargs):
         super(MainWindow, self).__init__(*args, **kwargs)
         title = "PennyWhistle Ranging GUI V" + __version__
         self.setWindowTitle(title)
         self.myScreen = app.primaryScreen()                      # self is mainwindow Widget and myScreen is the display it lives on
         self.monitor = self.myScreen.availableVirtualGeometry()  # space across entire virtual display
         app.aboutToQuit.connect(self.closeItDown)
         self.connectedResponder = 0
         self.connectedRequester = 0
         self.connectedMultiCast = 0
         self.radioConfigReq = None
         self.radioConfigResp = None
+        self.defineSheets()
+        self.platform = platform
         self.radioRanging = TDSR_radioControl.rangeCmds(self)
             # link in saved settings data
         self.settings = TDSR_settings.appSettings()
         self.settings.settingsSetup()
         self.appSettings = self.settings.settings
         self.initWindows()
         self.screenSetup()
         self.chipTempTimer = QTimer()
+        self.setStyleSheet(self.mainWindowSheet)
         self.initGUI()
         self.show()
         self.appSetup()
 
     def screenSetup(self):
         allScreens = self.myScreen.virtualSiblings() # list of each available monitor as a QScreen
         # print(allScreens)
@@ -102,14 +106,15 @@
         self.configID = 0
         self.radioConfigReq = None
         self.radioConfigResp = None
         self.radioStateReq = None
         self.radioStateResp = None
         self.radioReqNodeID = None
         self.radioRespNodeID = None
+        self.rangeDispType = "precision"
         self.interface   = 'ip'
         self.messageTypes = self.radioMessageTypes("JsonDoc")
         self.mode = 4
         self.rangeMax = 0
         self.rangeMin = 1000000
         self.powerMax = -200
         self.powerMin = 0
@@ -309,41 +314,14 @@
             radioObj['type'] = "ip"
             radioObj['name'] = addr
             radioObj['addr'] = addr
             radioObj['port'] = self.radioIP_Port
             ipRadios.append(radioObj)
         return ipRadios
 
-    # def getMultiCastRadioIPs(self):
-    #     self.radioConnectMultiCast()
-    #     ipRadios = []
-    #     if self.connectedMultiCast == 1:
-    #         stats,packet,addr = self.radioMultiCast.API.radio_GetIP_Request(self.multiCastIP)
-    #         sleep(.1)
-    #         if 'RADIO_GET_IP_CONFIRM' in packet.keys():
-    #             radioObj = {}
-    #             addr = packet['RADIO_GET_IP_CONFIRM']['ipv4']
-    #             radioObj['type'] = "ip"
-    #             radioObj['name'] = addr
-    #             radioObj['addr'] = addr
-    #             radioObj['port'] = self.radioIP_Port
-    #             ipRadios.append(radioObj)
-    #         for i in self.radioMultiCast.messageQueues:
-    #             while not self.radioMultiCast.messageQueues[i].empty():
-    #                 packet = self.radioMultiCast.messageQueues[i].get()
-    #                 if 'RADIO_GET_IP_CONFIRM' in packet.keys():
-    #                     radioObj = {}
-    #                     addr = packet['RADIO_GET_IP_CONFIRM']['ipv4']
-    #                     radioObj['type'] = "ip"
-    #                     radioObj['name'] = addr
-    #                     radioObj['addr'] = addr
-    #                     radioObj['port'] = self.radioIP_Port
-    #                     ipRadios.append(radioObj)
-    #     return ipRadios
-
     def getUSBPorts(self):
         usbRadiosCheck = TDSR_radioConnection.Radio(self, self.messageTypes, 'usb', '', 'find')
         radios = usbRadiosCheck.findUsbRadios()
         usbRadios = []
         for radio in radios:
             radioObj = {}
             radioName = str(radio)
@@ -507,20 +485,24 @@
                 else:
                     self.dispRespID.setStyleSheet("QLineEdit {background-color: lightgreen;}")
             else:
                 # print("guiPacketUpdates Range Error Error2")
                 self.dispRange.setStyleSheet("QLineEdit {background-color: rgb(255,0,0);}")
                 if self.radioMode != 'networking':
                     self.dispRespID.setStyleSheet("QLineEdit {background-color: coral;}")
+            displayRange = ""
+            if self.rangeDispType == "precision":
+                displayRange = f"{packet['RANGE_INFO']['precisionRangeM']:.3f}"
+            else:
+                displayRange = f"{packet['RANGE_INFO']['filteredRangeM']:.3f}"
             if self.windowRangeLarge.isVisible():   # If large range window open, then update it.
-                self.windowRangeLarge.processData(str(packet['RANGE_INFO']['precisionRangeM']),shade)
+                self.windowRangeLarge.processData(displayRange,shade)
             if self.windowRangeData.isVisible():
                 self.windowRangeData.processData(packet)
-            precRange = f"{packet['RANGE_INFO']['precisionRangeM']:.3f}"
-            self.dispRange.setText(precRange)
+            self.dispRange.setText(displayRange)
             if self.radioMode == 'ranging':
                 for k in range(len(self.dispStatWindow)):
                     self.dispStatWindow[k].setText(str(packet['RANGE_INFO'][self.statKeys[k]]))
         else:
             self.dispRange.setStyleSheet("QLineEdit {background-color: rgb(255,0,0);}")
             self.dispRespID.setStyleSheet("QLineEdit {background-color: coral;}")
             if self.windowRangeLarge.isVisible():   # If large range window open, then update it.
@@ -839,15 +821,15 @@
         yWidth = 40
         x = 5
         y = 0
         self.but_run = QPushButton('Start\nRanging', self)
         self.but_run.setToolTip('Start/Stop Ranging')
         self.but_run.resize(100, 100)
         self.but_run.setFont(self.guiFont.guiFont18)
-        self.but_run.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_run.setStyleSheet(self.buttonSheetBlue)
         self.but_run.move(x*xBump+xBias, y*yBump+yBias)
         self.but_run.clicked.connect(self.radioRanging.toggleRun)
 
         xStart = 715
         yStart = 145
         xBias = 0
         yBias = 0
@@ -926,14 +908,15 @@
         xBump = 140
         yBump = 80
         xWidth = 700
         yWidth = 180
         self.consoleOutput = QTextBrowser(self)
         self.consoleOutput.setGeometry(xStart,yStart,xWidth, yWidth)
         self.consoleOutput.setText("")
+        self.consoleOutput.setStyleSheet("QTextBrowser {background-color: rgb(240,240,240);}")
         self.consoleOutputScrollBar = self.consoleOutput.verticalScrollBar()
 
         xStart = 150
         yStart = 0
         xBias = 0
         yBias = 0
         xBump = 210
@@ -951,15 +934,15 @@
         self.dropMenuReqRadio = QComboBox(self)
         self.dropMenuReqRadio.resize(xWidth,yWidth)
         self.dropMenuReqRadio.setToolTip("Select range requesting radio")
         self.dropMenuReqRadio.setFont(self.guiFont.guiFont20)
         self.dropMenuReqRadio.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias + 35)
         self.dropMenuReqRadio.addItems([])
         self.dropMenuReqRadio.setEditable(False)
-        self.dropMenuReqRadio.setStyleSheet("QComboBox {color: GhostWhite; background-color: SteelBlue;} QAbstractItemView {color: GhostWhite; background-color: DarkBlue;}")
+        self.dropMenuReqRadio.setStyleSheet(self.dropSheetBlue)
         self.dropMenuReqRadio.currentTextChanged.connect(self.updateReqRadio)
 
         x = 0
         y = 1
         self.labelrespRadio = QLabel(self)
         self.labelrespRadio.resize(xWidth,yWidth)
         self.labelrespRadio.move(x*xBump + xStart + xBias + 10, yStart + y*yBump + yBias)
@@ -970,15 +953,15 @@
         self.dropMenuRespRadio = QComboBox(self)
         self.dropMenuRespRadio.resize(xWidth,yWidth)
         self.dropMenuRespRadio.setToolTip("Select range responding radio")
         self.dropMenuRespRadio.setFont(self.guiFont.guiFont20)
         self.dropMenuRespRadio.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias + 35)
         self.dropMenuRespRadio.addItems([])
         self.dropMenuRespRadio.setEditable(False)
-        self.dropMenuRespRadio.setStyleSheet("QComboBox {color: GhostWhite; background-color: SteelBlue;} QAbstractItemView {color: GhostWhite; background-color: DarkBlue;}")
+        self.dropMenuRespRadio.setStyleSheet(self.dropSheetBlue)
         self.dropMenuRespRadio.currentTextChanged.connect(self.updateRespRadio)
 
         self.check_connectResp = QCheckBox('', self)
         self.check_connectResp.setToolTip('Connect GUI to Responding Radio')
         self.check_connectResp.setFont(self.guiFont.guiFont14)
         self.check_connectResp.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias)
         self.check_connectResp.resize(200,40)
@@ -1027,25 +1010,25 @@
         xWidth = 120
         yBias = 35
         x = 2
         y = 0
         self.but_RadioConfigReq = QPushButton('Req Settings', self)
         self.but_RadioConfigReq.setToolTip('Show Requester Radio Configuration Screen')
         self.but_RadioConfigReq.resize(xWidth, yWidth)
-        self.but_RadioConfigReq.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_RadioConfigReq.setStyleSheet(self.buttonSheetBlue)
         self.but_RadioConfigReq.setFont(self.guiFont.guiFont14)
         self.but_RadioConfigReq.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         self.but_RadioConfigReq.clicked.connect(self.windowConfigReq.displayWindow)
 
         x = 2
         y = 1
         self.but_RadioConfigResp = QPushButton('Resp Settings', self)
         self.but_RadioConfigResp.setToolTip('Show Responder Radio (if connected) Configuration Screen')
         self.but_RadioConfigResp.resize(xWidth, yWidth)
-        self.but_RadioConfigResp.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_RadioConfigResp.setStyleSheet(self.buttonSheetBlue)
         self.but_RadioConfigResp.setFont(self.guiFont.guiFont14)
         self.but_RadioConfigResp.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         self.but_RadioConfigResp.clicked.connect(self.windowConfigResp.displayWindow)
 
         xStart = 10
         yStart = 350
         xBias = 0
@@ -1081,15 +1064,15 @@
         # xWidth = 160
         self.dropMenuChart = QComboBox(self)
         self.dropMenuChart.resize(xWidth,yWidth)
         self.dropMenuChart.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias + 45)
         self.dropMenuChart.setFont(self.guiFont.guiFont20)
         self.dropMenuChart.addItems(dropMenuOptions)
         self.dropMenuChart.setEditable(False)
-        self.dropMenuChart.setStyleSheet("QComboBox {color: GhostWhite; background-color: SteelBlue;} QAbstractItemView {color: GhostWhite; background-color: DarkBlue;}")
+        self.dropMenuChart.setStyleSheet(self.dropSheetBlue)
         self.dropMenuChart.setToolTip("Pick what should be charted")
         self.dropMenuChart.currentTextChanged.connect(self.updateDropMenuChart)
         x = 2
         y = 0
         self.labelChartStore = QLabel(self)
         self.labelChartStore.resize(xWidth,yWidth)
         self.labelChartStore.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias)
@@ -1126,20 +1109,20 @@
         xStart = 755
         yStart = 305
         xBias = 0
         yBias = 0
         xBump = 0
         yBump = 0
         xWidth = 200
-        yWidth = 45
+        yWidth = 50
         x = 0
         y = 0
         self.labelRange = QLabel(self)
         self.labelRange.resize(xWidth,yWidth)
-        self.labelRange.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias)
+        self.labelRange.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias + 5)
         self.labelRange.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self.labelRange.setFont(self.guiFont.guiFont30)
         self.labelRange.setText("Range(m)")
         xStart = 735
         yStart = 365
         xWidth = 240
         yWidth = 80
@@ -1155,16 +1138,16 @@
         yStart = 210
         xBump = 240
         yBump = 80
         # Range Chart
 
         self.dataWindow = PlotWidget(self)
         # self.dataWindow.setYRange(self.yScaleNeg,self.yScalePos,padding = 0)
-        # self.dataWindow.setBackground('w')
-        self.dataWindow.setBackground([255,255,255])
+        # self.dataWindow.setBackground(255,0,0,255)
+        self.dataWindow.setBackground([230,230,230])
         self.dataWindow.setGeometry(5,450,990,500 - self.reduceSize)
         self.dataWindow.showGrid(x=True, y=True)
         self.dataWindow.setHidden(False)
         self.plotX = []
         self.plotY = []
         self.chartData1 = self.dataWindow.plot(self.plotX, self.plotY, pen=self.pen[0])
         self.chartData2 = self.dataWindow.plot(self.plotX, self.plotY, pen=self.pen[2])
@@ -1215,47 +1198,47 @@
         xWidth = 130
         yWidth = 40
         x = 0
         y = 0
         self.but_networkWindow = QPushButton('Networking', self)
         self.but_networkWindow.setToolTip('Show Networking Window')
         self.but_networkWindow.resize(xWidth, yWidth)
-        self.but_networkWindow.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_networkWindow.setStyleSheet(self.buttonSheetBlue)
         self.but_networkWindow.setFont(self.guiFont.guiFont14)
         self.but_networkWindow.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         self.but_networkWindow.clicked.connect(self.networkWindow)
 
         x = 1
         y = 0
         self.but_rangeWindow = QPushButton('Range Window', self)
         self.but_rangeWindow.setToolTip('Show Large Range Window')
         self.but_rangeWindow.resize(xWidth, yWidth)
-        self.but_rangeWindow.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_rangeWindow.setStyleSheet(self.buttonSheetBlue)
         self.but_rangeWindow.setFont(self.guiFont.guiFont14)
         self.but_rangeWindow.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         self.but_rangeWindow.clicked.connect(self.rangeWindowLarge)
 
         xWidth = 80
         x = 2
         y = 0
         self.but_LoggingWindow = QPushButton('Logging', self)
         self.but_LoggingWindow.setToolTip('Show Data Logging Parameters')
         self.but_LoggingWindow.resize(xWidth, yWidth)
-        self.but_LoggingWindow.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_LoggingWindow.setStyleSheet(self.buttonSheetBlue)
         self.but_LoggingWindow.setFont(self.guiFont.guiFont14)
         self.but_LoggingWindow.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         self.but_LoggingWindow.clicked.connect(self.openLoggingWindow)
         xBump = 123
         xWidth = 60
         x = 3
         y = 0
         self.but_dataWindow = QPushButton('Data', self)
         self.but_dataWindow.setToolTip('Open Data Transfer Window')
         self.but_dataWindow.resize(xWidth, yWidth)
-        self.but_dataWindow.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_dataWindow.setStyleSheet(self.buttonSheetBlue)
         self.but_dataWindow.setFont(self.guiFont.guiFont14)
         self.but_dataWindow.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         self.but_dataWindow.clicked.connect(self.openDataTransferWindow)
 
         xStart = 450
         yStart = 955 - self.reduceSize
         xBias = 0
@@ -1265,57 +1248,57 @@
         xWidth = 100
         yWidth = 40
         x = 0
         y = 0
         self.but_rangeData = QPushButton('Range Data', self)
         self.but_rangeData.setToolTip('Show Ranging Data')
         self.but_rangeData.resize(xWidth, yWidth)
-        self.but_rangeData.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_rangeData.setStyleSheet(self.buttonSheetBlue)
         self.but_rangeData.setFont(self.guiFont.guiFont14)
         self.but_rangeData.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         self.but_rangeData.clicked.connect(self.openRangeData)
 
         x = 1
         y = 0
         self.but_reqStats = QPushButton('Req Stats', self)
         self.but_reqStats.setToolTip('Show Requester Stats')
         self.but_reqStats.resize(xWidth, yWidth)
-        self.but_reqStats.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_reqStats.setStyleSheet(self.buttonSheetBlue)
         self.but_reqStats.setFont(self.guiFont.guiFont14)
         self.but_reqStats.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         # self.but_reqStats.clicked.connect(self.ranging.getReqStats)
         self.but_reqStats.clicked.connect(self.openReqStats)
 
         x = 2
         y = 0
         self.but_respStats = QPushButton('Resp Stats', self)
         self.but_respStats.setToolTip('Show Responder Stats')
         self.but_respStats.resize(xWidth, yWidth)
-        self.but_respStats.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_respStats.setStyleSheet(self.buttonSheetBlue)
         self.but_respStats.setFont(self.guiFont.guiFont14)
         self.but_respStats.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         # self.but_reqStats.clicked.connect(self.ranging.getRespStats)
         self.but_respStats.clicked.connect(self.openRespStats)
 
         x = 3
         y = 0
         self.but_reqRadioInfo = QPushButton('Req Info', self)
         self.but_reqRadioInfo.setToolTip('Show Radio Information')
         self.but_reqRadioInfo.resize(xWidth, yWidth)
-        self.but_reqRadioInfo.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_reqRadioInfo.setStyleSheet(self.buttonSheetBlue)
         self.but_reqRadioInfo.setFont(self.guiFont.guiFont14)
         self.but_reqRadioInfo.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         self.but_reqRadioInfo.clicked.connect(self.getReqRadioInfo)
 
         x = 4
         y = 0
         self.but_respRadioInfo = QPushButton('Resp Info', self)
         self.but_respRadioInfo.setToolTip('Show Radio Information')
         self.but_respRadioInfo.resize(xWidth, yWidth)
-        self.but_respRadioInfo.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_respRadioInfo.setStyleSheet(self.buttonSheetBlue)
         self.but_respRadioInfo.setFont(self.guiFont.guiFont14)
         self.but_respRadioInfo.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         self.but_respRadioInfo.clicked.connect(self.getRespRadioInfo)
 # tests to see if reqeusted range number is valid and updates variables and GUI
     def updateRunTotal(self):
         try:
             self.appSettings['rangeRequests'] = int(self.dispRangeRunTotal.text())
@@ -1446,14 +1429,19 @@
             self.dataWindowT.setHidden(False)
             self.dataWindowB.setHidden(False)
             self.checkChartRange(None)
             # self.chartScale([self.rangeMax, self.rangeMin],[self.powerMax, self.powerMin])
         self.dataWindow.enableAutoRange(axis = 'x', enable = True)
         self.dataWindowT.enableAutoRange(axis = 'x', enable = True)
         self.dataWindowB.enableAutoRange(axis = 'x', enable = True)
+        filterList = {"Filtered", "Both", "MultiFilt"}
+        if self.dropMenuChart.currentText() in filterList:
+            self.rangeDispType = "filtered"
+        else:
+            self.rangeDispType = "precision"
         self.plotData()
 
 # tests to see if new chart depth number is valid and updates variables and GUI. Otherwise uses default.
     def updateChartStore(self):
         try:
             self.appSettings['chartDepth'] = int(self.dispChartStore.text())
         except:
@@ -1589,15 +1577,15 @@
         if status == False:
             self.dropMenuReqRadio.setStyleSheet("QComboBox {background-color: red;}")
             self.but_RadioConfigReq.setStyleSheet("QPushButton {background-color: red;}")
             text = "== Could not connect to primary radio address " + self.appSettings['reqRadio'] + " ==\n"
             self.updateConsole(text)
         else:
             self.dropMenuReqRadio.setStyleSheet("QComboBox {background-color: lightgreen;}")
-            self.but_RadioConfigReq.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+            self.but_RadioConfigReq.setStyleSheet(self.buttonSheetBlue)
             self.dispReqID.setText(str(self.radioReqNodeID))
             text = "Connected to Primary Radio Address " + self.appSettings['reqRadio'] + "\n"
             self.updateConsole(text)
 # Updates GUI connection status of responder
     def updateConnectResp(self, status):
         if status == False:
             # self.connectedResponder = 0
@@ -1611,17 +1599,17 @@
             else:
                 # self.connectedResponder = 0
                 text = "Connected responder not selected\n"
                 self.updateConsole(text)
         else:
             # self.connectedResponder = 1
             self.dropMenuRespRadio.setStyleSheet("QComboBox {background-color: lightgreen;}")
-            self.but_RadioConfigResp.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
-            self.but_respRadioInfo.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
-            self.but_respStats.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+            self.but_RadioConfigResp.setStyleSheet(self.buttonSheetBlue)
+            self.but_respRadioInfo.setStyleSheet(self.buttonSheetBlue)
+            self.but_respStats.setStyleSheet(self.buttonSheetBlue)
             text = "Connected to Secondary Radio Address " + self.appSettings['respRadio'] + "\n"
             self.updateConsole(text)
         self.windowDataTransfer.updateRespAvailable()
 # Updates text in GUI console output.
     def updateConsole(self, text):
         self.consoleBuf = self.consoleBuf + text
         self.consoleOutput.setText(self.consoleBuf)
@@ -1738,22 +1726,34 @@
         self.pen.append(mkPen(width = 4, color=(0,63,0)))
         self.pen.append(mkPen(width = 4, color=(0,0,63)))
         self.pen.append(mkPen(width = 4, color=(31,31,0)))
         self.pen.append(mkPen(width = 4, color=(0,63,63)))
         self.pen.append(mkPen(width = 4, color=(63,0,63)))
         self.pen.append(mkPen(width = 4, color=(0,0,0)))
 
+    def defineSheets(self):
+        self.buttonSheetBlue = "QPushButton {background-color: rgb(0,60,100); color: GhostWhite;}"
+        self.buttonSheetGray = "QPushButton {background-color: lightgrey; color: black;}"
+        self.dropSheetBlue = "QComboBox {color: GhostWhite; background-color: rgb(0,60,100);} QAbstractItemView {color: GhostWhite; background-color: DarkBlue;}"
+        self.dropSheetGray = "QComboBox {color: black; background-color: lightgrey;} QAbstractItemView {color: black; background-color: GhostWhite;}"
+        self.lineSheet = "QLineEdit {background-color: rgb(240,240,240);}"
+        self.windowSheet = "QWidget {background-color: rgb(100,160,220);}"
+        self.mainWindowSheet = "QMainWindow {background-color: rgb(100,160,220);}"
+        self.checkBoxSheet = "QCheckBox {color: GhostWhite;} QCheckBox::indicator {width:20px; height:20px;}"
+
 # Class window to display long running radio statistics
 class windowChipStats(QWidget):
     def __init__(self, gui, name):
         super().__init__()
         # self.setGeometry(10, 10, 800, 480)
         self.setFixedSize(800,480)
         self.setWindowTitle(name)
         self.gui = gui
+        # self.setStyleSheet("QWidget {background-color: rgb(200,200,200);}")
+        self.setStyleSheet(self.gui.windowSheet)
         self.name = name
         self.guiFont = guiFonts()
         self.initChipStatsGUI()
 
     def displayWindow(self):
         self.show()
         xOffset = self.gui.x() + self.gui.mainWindowWidth + 5
@@ -1835,17 +1835,19 @@
             self.dispChipStatWindow.append(tmpD)
             x = x + 1
 
 class windowChipTuning(QWidget):
     def __init__(self, gui):
         super().__init__()
         self.setFixedSize(640,330)
+        self.gui = gui
+        # self.setStyleSheet("QWidget {background-color: rgb(200,200,200);}")
+        self.setStyleSheet(self.gui.windowSheet)
         self.name = "Chip Tuning"
         self.setWindowTitle(self.name)
-        self.gui = gui
         self.guiFont = guiFonts()
         self.initGUI()
 
     def displayWindow(self):
         self.show()
         xOffset = self.gui.x() + self.gui.mainWindowWidth + 5
         yOffset = self.gui.y()
@@ -2006,15 +2008,15 @@
         xWidth = 160
         xStart = 60
         x = 0
         y = 2
         self.but_getTuning = QPushButton('Get Config', self)
         self.but_getTuning.setToolTip('Get Radio Tuning Values')
         self.but_getTuning.resize(xWidth, yWidth)
-        self.but_getTuning.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_getTuning.setStyleSheet(self.gui.buttonSheetBlue)
         self.but_getTuning.setFont(self.guiFont.guiFont14)
         self.but_getTuning.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         self.but_getTuning.clicked.connect(self.radioGetTuning)
 
         x = 1
         self.but_storeTuning = QPushButton('Store in Flash', self)
         self.but_storeTuning.setToolTip('Store Radio Tuning In Flash')
@@ -2102,17 +2104,19 @@
 
 # Class for window to display data from current range message.
 class windowRangeData(QWidget):
     def __init__(self, gui):
         super().__init__()
         # self.setGeometry(10, 10, 640, 330)
         self.setFixedSize(640,330)
+        self.gui = gui
+        # self.setStyleSheet("QWidget {background-color: rgb(200,200,200);}")
+        self.setStyleSheet(self.gui.windowSheet)
         self.name = "Range Data"
         self.setWindowTitle(self.name)
-        self.gui = gui
         self.guiFont = guiFonts()
         self.initGUI()
 
     def displayWindow(self):
         self.show()
         xOffset = self.gui.x() + self.gui.mainWindowWidth + 5
         yOffset = self.gui.y()
@@ -2205,14 +2209,16 @@
 class windowRadioInfo(QWidget):
     def __init__(self, gui, name, req):
         super().__init__()
         # self.setGeometry(10, 10, 780, 500)
         self.setFixedSize(780,500)
         self.setWindowTitle(name)
         self.gui = gui
+        # self.setStyleSheet("QWidget {background-color: rgb(200,200,200);}")
+        self.setStyleSheet(self.gui.windowSheet)
         self.name = name
         self.req = req
         self.guiFont = guiFonts()
         self.initGUI()
 
     def displayWindow(self):
         self.show()
@@ -2291,14 +2297,16 @@
 class windowConfiguration(QWidget):
     def __init__(self, gui, req):
         super().__init__()
         # self.setGeometry(10, 10, 620, 400)
         self.setFixedSize(620,840)
         self.setWindowTitle("Radio Configuration")
         self.gui = gui
+        # self.setStyleSheet("QWidget {background-color: rgb(200,200,200);}")
+        self.setStyleSheet(self.gui.windowSheet)
         self.guiFont = guiFonts()
         self.configFormUpdate = 0
         self.req = req  # 0 = responder, 1 = requester
         if self.req == 1:
             self.radioConfig = self.gui.radioConfigReq
         else:
             self.radioConfig = self.gui.radioConfigResp
@@ -2498,15 +2506,15 @@
         self.updateNodeID()
         self.configFormUpdate = 1
         self.updateTxPower()
         self.configFormUpdate = 1
         self.updateAntDelay()
         text = "Configuration Downloaded From Radio\n"
         self.gui.updateConsole(text)
-        self.but_setRadioConfig.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_setRadioConfig.setStyleSheet(self.gui.buttonSheetBlue)
 
 # Sets radio confiuration and makes it persist after reboot.
     def radioStoreConfig(self):
         self.configFormUpdate = 0
         self.updateMenuPRF()
         self.updateMenuPreamLen()
         self.updateMenuBitRate()
@@ -2556,15 +2564,15 @@
             self.gui.radioReq.API.radio_SetNodeID_Request(self.gui.appSettings['reqRadio'], self.gui.radioReqNodeID, 0)
         else:
             self.gui.radioResp.API.radio_SetConfig_Request(self.gui.appSettings['respRadio'], self.radioConfig, 0)
             self.gui.radioResp.API.radio_SetNodeID_Request(self.gui.appSettings['respRadio'], self.gui.radioRespNodeID, 0)
         text =  "Configuration Set\n"
         self.gui.updateConsole(text)
         self.radioGetConfig()
-        self.but_setRadioConfig.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_setRadioConfig.setStyleSheet(self.gui.buttonSheetBlue)
 
 ## IP Config
     def radioGetIP(self):
         ip = ""
         if self.req:
             ip = self.gui.appSettings['reqRadio']
             status, msg, addr = self.gui.radioReq.API.radio_GetIP_Request(ip)
@@ -3072,15 +3080,15 @@
         xWidth = 160
         yWidth = 40
         x = 0
         y = 0
         self.but_getRadioConfig = QPushButton('Get Config', self)
         self.but_getRadioConfig.setToolTip('Get Radio Configuration')
         self.but_getRadioConfig.resize(xWidth, yWidth)
-        self.but_getRadioConfig.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_getRadioConfig.setStyleSheet(self.gui.buttonSheetBlue)
         self.but_getRadioConfig.setFont(self.guiFont.guiFont14)
         self.but_getRadioConfig.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         self.but_getRadioConfig.clicked.connect(self.radioGetConfig)
 
         x = 1
         y = 0
         self.but_storeRadioConfig = QPushButton('Store in Flash', self)
@@ -3092,15 +3100,15 @@
         self.but_storeRadioConfig.clicked.connect(self.radioStoreConfig)
 
         x = 2
         y = 0
         self.but_setRadioConfig = QPushButton('Set Config', self)
         self.but_setRadioConfig.setToolTip('Set Radio Configuration')
         self.but_setRadioConfig.resize(xWidth, yWidth)
-        self.but_setRadioConfig.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_setRadioConfig.setStyleSheet(self.gui.buttonSheetBlue)
         self.but_setRadioConfig.setFont(self.guiFont.guiFont14)
         self.but_setRadioConfig.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         self.but_setRadioConfig.clicked.connect(self.radioSetConfig)
 
         self.dispSep1 = QLineEdit(self)
         self.dispSep1.move(60, yStart + y*yBump + yBias + 60)
         self.dispSep1.resize(500,1)
@@ -3123,24 +3131,24 @@
         xStart = 30
         xBump = 200
         x = 0
         y = 0
         self.but_getIP = QPushButton('Get IP Config', self)
         self.but_getIP.setToolTip('Get Current IP config')
         self.but_getIP.resize(xWidth, yWidth)
-        self.but_getIP.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_getIP.setStyleSheet(self.gui.buttonSheetBlue)
         self.but_getIP.setFont(self.guiFont.guiFont14)
         self.but_getIP.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         self.but_getIP.clicked.connect(self.radioGetIP)
         x = 1
         y = 0
         self.but_setIP = QPushButton('Set IP Config', self)
         self.but_setIP.setToolTip('Set new IP config')
         self.but_setIP.resize(xWidth, yWidth)
-        self.but_setIP.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_setIP.setStyleSheet(self.gui.buttonSheetBlue)
         self.but_setIP.setFont(self.guiFont.guiFont14)
         self.but_setIP.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         self.but_setIP.clicked.connect(self.radioSetIP)
         x = 2
         y = 0
         self.but_reboot = QPushButton('Reboot', self)
         self.but_reboot.setToolTip('Reboot radio using new IP settings')
@@ -3221,15 +3229,15 @@
         xStart = 20
         yBump = 50
         x = 0
         y = 1
         self.but_savePreset = QPushButton('Store/Update', self)
         self.but_savePreset.setToolTip('Store/Update listed radio preset')
         self.but_savePreset.resize(xWidth, yWidth)
-        self.but_savePreset.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_savePreset.setStyleSheet(self.gui.buttonSheetBlue)
         self.but_savePreset.setFont(self.guiFont.guiFont14)
         self.but_savePreset.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         self.but_savePreset.clicked.connect(self.radioSavePreset)
 
         x = 0
         y = 1
         xBias = 180
@@ -3251,15 +3259,15 @@
         xStart = 30
         yBias = 40
         x = 0
         y = 2
         self.but_applyPreset = QPushButton('Apply Preset', self)
         self.but_applyPreset.setToolTip('Apply Listed Radio Preset')
         self.but_applyPreset.resize(xWidth, yWidth)
-        self.but_applyPreset.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_applyPreset.setStyleSheet(self.gui.buttonSheetBlue)
         self.but_applyPreset.setFont(self.guiFont.guiFont14)
         self.but_applyPreset.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         self.but_applyPreset.clicked.connect(self.radioApplyPreset)
 
         x = 1
         y = 2
         self.but_persistPreset = QPushButton('Persist Preset', self)
@@ -3271,15 +3279,15 @@
         self.but_persistPreset.clicked.connect(self.radioPersistPreset)
 
         x = 2
         y = 2
         self.but_deletePreset = QPushButton('Delete Preset', self)
         self.but_deletePreset.setToolTip('Delete Preset Listed in Drop Menu')
         self.but_deletePreset.resize(xWidth, yWidth)
-        self.but_deletePreset.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_deletePreset.setStyleSheet(self.gui.buttonSheetBlue)
         self.but_deletePreset.setFont(self.guiFont.guiFont14)
         self.but_deletePreset.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         self.but_deletePreset.clicked.connect(self.radioDeletePreset)
 
         x = 0
         y = 3
         xStart = 50
@@ -3288,25 +3296,27 @@
         # dropMenuOptions = ["HDR - Omni", "HDR - Directional", "MDR - Omni", "MDR - Directional"]
         self.dropMenuPresets = QComboBox(self)
         self.dropMenuPresets.resize(520,yWidth)
         self.dropMenuPresets.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias)
         self.dropMenuPresets.setFont(self.guiFont.guiFont20)
         self.dropMenuPresets.addItems(dropMenuOptions)
         self.dropMenuPresets.setEditable(False)
-        self.dropMenuPresets.setStyleSheet("QComboBox {color: GhostWhite; background-color: SteelBlue;} QAbstractItemView {color: GhostWhite; background-color: DarkBlue;}")
+        self.dropMenuPresets.setStyleSheet(self.dropSheetBlue)
         self.dropMenuPresets.setToolTip("Selects which preset to load")
         self.dropMenuPresets.currentTextChanged.connect(self.radioUpdatePresets)
 
 # Class for window for data transfer
 class windowDataTransfer(QWidget):
     def __init__(self, gui):
         super().__init__()
         self.setWindowTitle("Data Transfer")
         self.setGeometry(0, 0, 800, 540)
         self.gui = gui
+        # self.setStyleSheet("QWidget {background-color: rgb(200,200,200);}")
+        self.setStyleSheet(self.gui.windowSheet)
         self.guiFont = guiFonts()
         self.radioData = TDSR_radioControl.dataCmds(self.gui)
         self.dataDestination = 0
         self.dataDestinationSlot = 0
         self.initGUI()
 
     def displayWindow(self):
@@ -3315,24 +3325,30 @@
             self.dropMenuDestination.addItems([str(self.gui.appSettings['respID'])])
         self.show()
         xOffset = self.gui.x() + self.gui.mainWindowWidth + 5
         yOffset = self.gui.y()
         self.gui.windowDataTransfer.move(self.gui.monitor.left()+xOffset, self.gui.monitor.top()+yOffset)
 
     def getTransferFilename(self):
-        xfrFileName = QFileDialog.getOpenFileName(self, 'Pick File to Transfer', "./Uploads")
+        if self.gui.platform == "linux":
+            xfrFileName = QFileDialog.getOpenFileName(self, 'Pick File to Transfer', "./Uploads", options=QFileDialog.Option.DontUseNativeDialog)
+        else:
+            xfrFileName = QFileDialog.getOpenFileName(self, 'Pick File to Transfer', "./Uploads")
         if xfrFileName != "":
             xfrFileName = xfrFileName[0]
             self.dispfileSelect.setText(str(xfrFileName))
 # Update settings for Download Path.
     def updateDownloadName(self):
         self.gui.appSettings['downloadDirectory'] = self.dispDownloads.text()
 
     def getDownloadPath(self):
-        downloadPath = QFileDialog.getExistingDirectory(self, 'Choose Download Directory', str(self.gui.appSettings['downloadDirectory']))
+        if self.gui.platform == "linux":
+            downloadPath = QFileDialog.getExistingDirectory(self, 'Choose Download Directory', str(self.gui.appSettings['downloadDirectory']), options=QFileDialog.Option.DontUseNativeDialog)
+        else:
+            downloadPath = QFileDialog.getExistingDirectory(self, 'Choose Download Directory', str(self.gui.appSettings['downloadDirectory']))
         if downloadPath != "":
             downloadPath = downloadPath + "/"
             self.dispDownloads.setText(str(downloadPath))
             self.gui.appSettings['downloadDirectory'] = downloadPath
 # Update settings for Download Path.
     def updateDownloadName(self):
         self.gui.appSettings['downloadDirectory'] = self.dispDownloads.text()
@@ -3429,15 +3445,15 @@
         x = 2
         xBias = 120
         self.dropMenuDestination = QComboBox(self)
         self.dropMenuDestination.resize(xWidth,yWidth)
         self.dropMenuDestination.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias - 10)
         self.dropMenuDestination.setFont(self.guiFont.guiFont20)
         self.dropMenuDestination.setEditable(False)
-        self.dropMenuDestination.setStyleSheet("QComboBox {color: GhostWhite; background-color: SteelBlue;} QAbstractItemView {color: GhostWhite; background-color: DarkBlue;}")
+        self.dropMenuDestination.setStyleSheet(self.gui.dropSheetBlue)
         self.dropMenuDestination.setToolTip("Which radio are we sending to?")
         self.dropMenuDestination.currentTextChanged.connect(self.updateDropMenuDest)
         xBias = 0
         x = 0
         y = 0
         self.labelTextInput = QLabel(self)
         self.labelTextInput.resize(xWidth,yWidth)
@@ -3448,26 +3464,27 @@
         xStart = 200
         yStart = 60
         xWidth = 60
         yWidth = 40
         self.but_textSend = QPushButton('Send', self)
         self.but_textSend.setToolTip('Sends text from requester to responder')
         self.but_textSend.resize(xWidth, yWidth)
-        self.but_textSend.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_textSend.setStyleSheet(self.gui.buttonSheetBlue)
         self.but_textSend.setFont(self.guiFont.guiFont14)
         self.but_textSend.move(x*xBump + xBias + xStart, y*yBump + yBias - 5 + yStart)
         self.but_textSend.clicked.connect(self.radioData.reqSendTextData)
         xStart = 10
         yStart = 100
         xWidth = 780
         yWidth = 100
         self.dataTextInput = QTextEdit(self)
         self.dataTextInput.setGeometry(xStart,yStart,xWidth, yWidth)
         self.dataTextInput.setText("")
         self.dataTextInputScrollBar = self.dataTextInput.verticalScrollBar()
+        self.dataTextInput.setStyleSheet("QTextEdit {background-color: rgb(240,240,240);}")
         xStart = 10
         yStart = 220
         xWidth = 200
         yWidth = 40
         self.labelTextReceived = QLabel(self)
         self.labelTextReceived.resize(xWidth,yWidth)
         self.labelTextReceived.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias)
@@ -3478,14 +3495,15 @@
         yStart = 255
         xWidth = 780
         yWidth = 100
         self.dataReqTextReceived = QTextBrowser(self)
         self.dataReqTextReceived.setGeometry(xStart,yStart,xWidth, yWidth)
         self.dataReqTextReceived.setText("")
         self.dataReqTextReceivedScrollBar = self.dataReqTextReceived.verticalScrollBar()
+        self.dataReqTextReceived.setStyleSheet("QTextBrowser {background-color: rgb(240,240,240);}")
 
         yStart = 380
         xStart = 10
         xBias = 0
         yBias = 0
         xBump = 210
         yBump = 30
@@ -3500,15 +3518,15 @@
         self.labelTransfers.setFont(self.guiFont.guiFont20)
         self.labelTransfers.setText("File Transfer")
         x = 0
         y = 1
         self.but_fileSelect = QPushButton('Choose File', self)
         self.but_fileSelect.setToolTip('Pick File to Transfer')
         self.but_fileSelect.resize(xWidth, yWidth)
-        self.but_fileSelect.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_fileSelect.setStyleSheet(self.gui.buttonSheetBlue)
         self.but_fileSelect.setFont(self.guiFont.guiFont14)
         self.but_fileSelect.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         self.but_fileSelect.clicked.connect(self.getTransferFilename)
         xWidth = 500
         x = 1
         y = 1
         self.dispfileSelect = QLineEdit(self)
@@ -3519,15 +3537,15 @@
         self.dispfileSelect.setAlignment(Qt.AlignmentFlag.AlignLeft)
         xStart = 730
         xWidth = 60
         x = 0
         self.but_fileSend = QPushButton('Send', self)
         self.but_fileSend.setToolTip('Pick File to Transfer')
         self.but_fileSend.resize(xWidth, yWidth)
-        self.but_fileSend.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_fileSend.setStyleSheet(self.gui.buttonSheetBlue)
         self.but_fileSend.setFont(self.guiFont.guiFont14)
         self.but_fileSend.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         self.but_fileSend.clicked.connect(self.radioData.reqSendBase64File)
         # self.dispfileSelect.setText("-")
         xStart = 10
         xWidth = 200
         yWidth = 40
@@ -3542,15 +3560,15 @@
         self.labelIncoming.setText("Incoming Files")
         xWidth = 200
         x = 0
         y = 3
         self.but_Downloads = QPushButton('Download Directory', self)
         self.but_Downloads.setToolTip('Pick Download Directory Name')
         self.but_Downloads.resize(xWidth, yWidth)
-        self.but_Downloads.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_Downloads.setStyleSheet(self.gui.buttonSheetBlue)
         self.but_Downloads.setFont(self.guiFont.guiFont14)
         self.but_Downloads.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         self.but_Downloads.clicked.connect(self.getDownloadPath)
         xWidth = 570
         x = 1
         y = 3
         self.dispDownloads = QLineEdit(self)
@@ -3585,23 +3603,26 @@
         yWidth = 100
         self.dataRespTextReceived = QTextBrowser(self)
         self.dataRespTextReceived.setGeometry(xStart,yStart + yBias,xWidth, yWidth)
         self.dataRespTextReceived.setText("")
         self.dataRespTextReceived.setHidden(False)
         self.dataRespTextReceivedScrollBar = self.dataRespTextReceived.verticalScrollBar()
         self.dataRespTextReceivedScrollBar.setHidden(False)
+        self.dataRespTextReceived.setStyleSheet("QTextBrowser {background-color: rgb(240,240,240);}")
 
 # Class for window to display and set data logging options.
 class windowLogFile(QWidget):
     def __init__(self, gui):
         super().__init__()
         # self.setGeometry(10, 10, 800, 400)
-        self.setFixedSize(800,400)
-        self.setWindowTitle("Data Logging")
+        self.setFixedSize(730,350)
         self.gui = gui
+        # self.setStyleSheet("QWidget {background-color: rgb(200,200,200);}")
+        self.setStyleSheet(self.gui.windowSheet)
+        self.setWindowTitle("Data Logging")
         self.guiFont = guiFonts()
         self.initGUI()
 
     def displayWindow(self):
         self.show()
         xOffset = self.gui.x() + self.gui.mainWindowWidth + 5
         yOffset = self.gui.y()
@@ -3615,15 +3636,15 @@
         self.gui.logFile.closeLogFile()
         self.gui.appSettings['logDirectory'] = self.dispLogDir.text()
 # Turn logging on and off
     def toggleLogging(self):
         if self.gui.appSettings['enableLogging'] == 1:
             self.gui.appSettings['enableLogging'] = 0
             self.but_enableLogging.setText("Logging Disabled")
-            self.but_enableLogging.setStyleSheet("QPushButton {background-color: lightyellow;}")
+            self.but_enableLogging.setStyleSheet(self.gui.buttonSheetBlue)
             self.gui.logFile.closeLogFile()
         else:
             self.gui.appSettings['enableLogging'] = 1
             self.but_enableLogging.setText("Logging Enabled")
             self.but_enableLogging.setStyleSheet("QPushButton {background-color: coral;}")
             # self.gui.logFile.logToFile(None, self.gui.appSettings['reqRadio'])
 # Sets whether logs are one large file or broken up by a determined length of time.
@@ -3647,40 +3668,57 @@
             self.gui.appSettings['logJson'] = 0
 # Sets whether all json messages are logged or just range_info messges.
     def updateLogRangeInfo(self):
         if self.check_logRangeInfo.isChecked():
             self.gui.appSettings['logRangeInfoOnly'] = 1
         else:
             self.gui.appSettings['logRangeInfoOnly'] = 0
+# Sets whether all logging happens when radio is idle or just while ranging.
+    def updateWhileIdle(self):
+        if self.check_logIdle.isChecked():
+            self.gui.appSettings['logWhileIdle'] = 1
+        else:
+            self.gui.appSettings['logWhileIdle'] = 0
+
 # Get root directory for log storage.
     def getLogPath(self):
-        logPath = QFileDialog.getExistingDirectory(self, 'Choose Log Directory', str(self.gui.appSettings['logDirectory']))
+        if self.gui.platform == "linux":
+            logPath = QFileDialog.getExistingDirectory(self, 'Choose Log Directory', str(self.gui.appSettings['logDirectory']), options=QFileDialog.Option.DontUseNativeDialog)
+        else:
+            logPath = QFileDialog.getExistingDirectory(self, 'Choose Log Directory', str(self.gui.appSettings['logDirectory']))
         if logPath != "":
             logPath = logPath + "/"
             self.dispLogDir.setText(str(logPath))
             self.gui.appSettings['logDirectory'] = logPath
 # Get name for name based logging.
     def getLogFilename(self):
         logDir = Path(str(self.gui.appSettings['logDirectory']))
         if logDir.is_dir() == True:
-            logDir = QFileDialog.getSaveFileName(self, 'Choose Logfile Name', str(self.gui.appSettings['logDirectory']) + "/" + str(self.gui.appSettings['logFile']), "log (*.log)")
+            if self.gui.platform == "linux":
+                logDir = QFileDialog.getSaveFileName(self, 'Choose Logfile Name', str(self.gui.appSettings['logDirectory']) + "/" + str(self.gui.appSettings['logFile']), "log (*.log)", options=QFileDialog.Option.DontUseNativeDialog)
+
+            else:
+                logDir = QFileDialog.getSaveFileName(self, 'Choose Logfile Name', str(self.gui.appSettings['logDirectory']) + "/" + str(self.gui.appSettings['logFile']), "log (*.log)")
         else:
-            logDir = QFileDialog.getSaveFileName(self, 'Choose Logfile Name', "./" + str(self.gui.appSettings['logFile']), "log (*.log)")
+            if self.gui.platform == "linux":
+                logDir = QFileDialog.getSaveFileName(self, 'Choose Logfile Name', "./" + str(self.gui.appSettings['logFile']), "log (*.log)", options=QFileDialog.Option.DontUseNativeDialog)
+            else:
+                logDir = QFileDialog.getSaveFileName(self, 'Choose Logfile Name', "./" + str(self.gui.appSettings['logFile']), "log (*.log)")
         logName = logDir[0].split("/")
         if logDir[0] != '':
             logName = logName[len(logName) - 1]
             logDir = logDir[0].split(logName)
             logDir = logDir[0]
             self.dispLogName.setText(str(logName))
             self.gui.appSettings['logFile'] = logName
             self.dispLogDir.setText(str(logDir))
             self.gui.appSettings['logDirectory'] = logDir
 
     def initGUI(self):
-        xStart = 225
+        xStart = 190
         yStart = 10
         xBias = 0
         yBias = 0
         xBump = 160
         yBump = 80
         xWidth = 350
         yWidth = 50
@@ -3688,14 +3726,15 @@
         y = 0
         self.labelWindow = QLabel(self)
         self.labelWindow.resize(xWidth,yWidth)
         self.labelWindow.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias)
         self.labelWindow.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self.labelWindow.setFont(self.guiFont.guiFont34)
         self.labelWindow.setText("Data Logging")
+        self.labelWindow.setStyleSheet("QLabel {color: black;}")
 
         yStart = 70
         xStart = 0
         xBias = 0
         yBias = 0
         xBump = 220
         yBump = 60
@@ -3729,25 +3768,24 @@
         xStart = 10
         xWidth = 200
         x = 0
         y = 0
         self.but_LogFile = QPushButton('Base LogFile Name', self)
         self.but_LogFile.setToolTip('Pick LogFile Name')
         self.but_LogFile.resize(xWidth, yWidth)
-        self.but_LogFile.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_LogFile.setStyleSheet(self.gui.buttonSheetBlue)
         self.but_LogFile.setFont(self.guiFont.guiFont14)
         self.but_LogFile.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         self.but_LogFile.clicked.connect(self.getLogFilename)
-
         x = 0
         y = 1
         self.but_LogDir = QPushButton('Log Directory', self)
         self.but_LogDir.setToolTip('Pick LogFile Directory')
         self.but_LogDir.resize(xWidth, yWidth)
-        self.but_LogDir.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_LogDir.setStyleSheet(self.gui.buttonSheetBlue)
         self.but_LogDir.setFont(self.guiFont.guiFont14)
         self.but_LogDir.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         self.but_LogDir.clicked.connect(self.getLogPath)
         yStart = 70
         yStart = 100
         xBias = 0
         yBias = 0
@@ -3758,53 +3796,71 @@
         x = 0
         y = 2
         self.check_logJson = QCheckBox('Log json', self)
         self.check_logJson.setToolTip('Log Full Messages')
         self.check_logJson.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         self.check_logJson.resize(200,40)
         self.check_logJson.setFont(self.guiFont.guiFont18)
+        self.check_logJson.setStyleSheet(self.gui.checkBoxSheet)
         if self.gui.appSettings['logJson'] == 0:
             self.check_logJson.setChecked(False)
         else:
             self.check_logJson.setChecked(True)
         self.check_logJson.stateChanged.connect(self.updateLogJson)
 
         x = 0
         y = 3
         self.check_logRangeInfo = QCheckBox('Log RangeInfo Only', self)
         self.check_logRangeInfo.setToolTip('Log Only Range Info Messages')
         self.check_logRangeInfo.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         self.check_logRangeInfo.resize(300,40)
         self.check_logRangeInfo.setFont(self.guiFont.guiFont18)
+        self.check_logRangeInfo.setStyleSheet(self.gui.checkBoxSheet)
         if self.gui.appSettings['logRangeInfoOnly'] == 0:
             self.check_logRangeInfo.setChecked(False)
         else:
             self.check_logRangeInfo.setChecked(True)
         self.check_logRangeInfo.stateChanged.connect(self.updateLogRangeInfo)
 
+        x = 0
+        y = 4
+        self.check_logIdle = QCheckBox('Log While Idle', self)
+        self.check_logIdle.setToolTip('Log data when radio idle as well as ranging')
+        self.check_logIdle.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
+        self.check_logIdle.resize(300,40)
+        self.check_logIdle.setFont(self.guiFont.guiFont18)
+        self.check_logIdle.setStyleSheet(self.gui.checkBoxSheet)
+        if self.gui.appSettings['logWhileIdle'] == 0:
+            self.check_logIdle.setChecked(False)
+        else:
+            self.check_logIdle.setChecked(True)
+        self.check_logIdle.stateChanged.connect(self.updateWhileIdle)
+
         x = 1
         y = 2
         self.check_logDateBased = QCheckBox('Time Based Naming', self)
         self.check_logDateBased.setToolTip('Generate Log Names based on radio ID and logging times')
         self.check_logDateBased.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         self.check_logDateBased.resize(300,40)
         self.check_logDateBased.setFont(self.guiFont.guiFont18)
+        self.check_logDateBased.setStyleSheet(self.gui.checkBoxSheet)
         if self.gui.appSettings['logDateBased'] == 0:
             self.check_logDateBased.setChecked(False)
         else:
             self.check_logDateBased.setChecked(True)
         self.check_logDateBased.stateChanged.connect(self.updateLogDateBased)
 
         x = 1
         y = 3
         self.check_logSegmented = QCheckBox('Time Segmented', self)
         self.check_logSegmented.setToolTip('Break into multiple logs based on run time')
         self.check_logSegmented.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         self.check_logSegmented.resize(300,40)
         self.check_logSegmented.setFont(self.guiFont.guiFont18)
+        self.check_logSegmented.setStyleSheet(self.gui.checkBoxSheet)
         if self.gui.appSettings['logSegmented'] == 0:
             self.check_logSegmented.setChecked(False)
         else:
             self.check_logSegmented.setChecked(True)
         self.check_logSegmented.stateChanged.connect(self.updateLogSegmented)
 
         x = 2
@@ -3812,62 +3868,66 @@
         xWidth = 160
         self.labelSegmentTime = QLabel(self)
         self.labelSegmentTime.resize(xWidth,yWidth)
         self.labelSegmentTime.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias)
         self.labelSegmentTime.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self.labelSegmentTime.setFont(self.guiFont.guiFont18)
         self.labelSegmentTime.setText("Seg Time(Sec)")
+        self.labelSegmentTime.setStyleSheet("QLabel {color: GhostWhite;}")
         self.dispSegmentTime = QLineEdit(self)
         self.dispSegmentTime.setStyleSheet("QLineEdit {background-color: lightgreen;}")
         self.dispSegmentTime.setFont(self.guiFont.guiFont18)
         self.dispSegmentTime.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias + 40)
         self.dispSegmentTime.resize(xWidth,yWidth)
         self.dispSegmentTime.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self.dispSegmentTime.setText(str(self.gui.appSettings['segmentTime']))
         self.dispSegmentTime.editingFinished.connect(self.updateLogSegmented)
         self.guiSegmentTime = 1
 
-        xStart = 300
-        yStart = 300
+        xStart = 265
+        yStart = 255
         xBias = 0
         yBias = 0
         xBump = 220
         yBump = 60
         xWidth = 200
         yWidth = 40
         x = 0
         y = 0
         self.labelLoggingStatus = QLabel(self)
         self.labelLoggingStatus.resize(xWidth,yWidth)
         self.labelLoggingStatus.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias)
         self.labelLoggingStatus.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self.labelLoggingStatus.setFont(self.guiFont.guiFont20)
         self.labelLoggingStatus.setText("Logging Status")
-        yStart = 340
+        self.labelLoggingStatus.setStyleSheet("QLabel {color: black;}")
+        yStart = 295
         self.but_enableLogging = QPushButton('Enable Logging', self)
         self.but_enableLogging.setToolTip('Toggle Data Logging')
         self.but_enableLogging.resize(xWidth, yWidth)
         self.but_enableLogging.setFont(self.guiFont.guiFont20)
         self.but_enableLogging.move(x*xBump + xBias + xStart, y*yBump + yBias + yStart)
         self.but_enableLogging.clicked.connect(self.toggleLogging)
         if self.gui.appSettings['enableLogging'] == 1:
             self.but_enableLogging.setText("Logging Enabled")
             self.but_enableLogging.setStyleSheet("QPushButton {background-color: coral;}")
         else:
             self.but_enableLogging.setText("Logging Disabled")
-            self.but_enableLogging.setStyleSheet("QPushButton {background-color: lightyellow;}")
+            self.but_enableLogging.setStyleSheet(self.gui.buttonSheetBlue)
 
 # Class for large range window that can more easily be seen from a distance.
 class windowNetwork(QWidget):
     def __init__(self, gui):
         super().__init__()
         self.setGeometry(10, 10, 975, 60)
         self.setMinimumWidth(975)
         self.setWindowTitle("Radio Network Settings")
         self.gui = gui
+        # self.setStyleSheet("QWidget {background-color: rgb(200,200,200);}")
+        self.setStyleSheet(self.gui.windowSheet)
         self.guiFont = guiFonts()
         self.layoutSlots = None
         self.layoutStats = None
         self.layoutTop = None
         self.layoutNetRanges = None
         self.layoutNetStats = None
         self.layoutNetRangePlots = None
@@ -4001,15 +4061,15 @@
         tabs = QTabWidget()
         tabs.addTab(self.netSlotsTab(), "SlotMap")
         tabs.addTab(self.netRangesTab(), "Ranges")
         # tabs.addTab(self.netPlottingTab(), "Graphs")
         tabs.addTab(self.netStatsTab(), "Stats")
         self.layoutTop.addWidget(tabs)
         but_networkRunToggle = QPushButton("Start Network")
-        but_networkRunToggle.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        but_networkRunToggle.setStyleSheet(self.gui.buttonSheetBlue)
         but_networkRunToggle.clicked.connect(self.buttonHandlerNetworkToggle)
         self.layoutTop.addWidget(but_networkRunToggle,1)
         self.setLayout(self.layoutTop)
 
     def netSlotsTab(self):
         self.slotTab = QWidget()
         self.layoutSlots = QVBoxLayout()
@@ -4047,40 +4107,40 @@
     def makeControlLine(self):
         controlLine = QHBoxLayout()
         height = 30
         width = 120
         # Button to send slotmap to radio
         self.but_slotMapSetMap = QPushButton("Set Map")
         self.but_slotMapSetMap.setFixedSize(width,height)
-        self.but_slotMapSetMap.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_slotMapSetMap.setStyleSheet(self.gui.buttonSheetBlue)
         self.but_slotMapSetMap.clicked.connect(self.buttonHandlerSetMap)
         # Button to get slotmap from radio
         but_slotMapGetMap = QPushButton("Get Map")
         but_slotMapGetMap.setFixedSize(width,height)
-        but_slotMapGetMap.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        but_slotMapGetMap.setStyleSheet(self.gui.buttonSheetBlue)
         but_slotMapGetMap.clicked.connect(self.buttonHandlerGetMap)
         # Button to load slotmap from disk
         but_slotMapLoad = QPushButton("Load Map")
         but_slotMapLoad.setFixedSize(width,height)
-        but_slotMapLoad.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        but_slotMapLoad.setStyleSheet(self.gui.buttonSheetBlue)
         but_slotMapLoad.clicked.connect(self.buttonHandlerLoadMap)
         # Button to clear slotmap
         but_slotMapClear = QPushButton("New Map")
         but_slotMapClear.setFixedSize(width,height)
-        but_slotMapClear.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        but_slotMapClear.setStyleSheet(self.gui.buttonSheetBlue)
         but_slotMapClear.clicked.connect(self.buttonHandlerClearMap)
         # Button to save slotmap to disk
         but_slotMapSave = QPushButton("Save Map")
         but_slotMapSave.setFixedSize(width,height)
-        but_slotMapSave.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        but_slotMapSave.setStyleSheet(self.gui.buttonSheetBlue)
         but_slotMapSave.clicked.connect(self.buttonHandlerSaveMap)
         # Button to get network stats from the radio
         but_networkStats = QPushButton("Show Stats")
         but_networkStats.setFixedSize(width,height)
-        but_networkStats.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        but_networkStats.setStyleSheet(self.gui.buttonSheetBlue)
         but_networkStats.clicked.connect(self.buttonHandlerShowStats)
         controlLine.addWidget(self.but_slotMapSetMap,1)
         controlLine.addWidget(but_slotMapGetMap,1)
         controlLine.addWidget(but_slotMapLoad,1)
         controlLine.addWidget(but_slotMapClear,1)
         controlLine.addWidget(but_slotMapSave,1)
         controlLine.addWidget(but_networkStats,1)
@@ -4148,53 +4208,64 @@
         layoutSlotData = QHBoxLayout()
         # Slot Number Field
         # slot = len(self.layoutSlots)-self.startField
         # idColor = self.gui.pen[slot].color().getRgb()
         # idColor = idColor[0:3]
         # idColor = "QLineEdit {background-color: rgb" + str(idColor) + ";}"
         slotNum = QLineEdit(str(len(self.layoutSlots)-self.startField))
+        slotNum.setStyleSheet(self.gui.lineSheet)
         slotNum.setReadOnly(True)
         slotNum.setFixedSize(width,height)
-        slotNum.setStyleSheet("QLineEdit {background-color: lightgrey;}")
+        # slotNum.setStyleSheet("QLineEdit {background-color: lightgrey;}")
         # slotNum.setStyleSheet(idColor)
         # What type of slot is it?
         slotType = QComboBox(self)
         slotType.addItems(["Range", "Data"])
         slotType.setFixedSize(width,height)
+        slotType.setStyleSheet(self.gui.dropSheetGray)
         # Which configuration does this slot use?
         slotConfig = QLineEdit("0")
         slotConfig.setFixedSize(width,height)
+        slotConfig.setStyleSheet(self.gui.lineSheet)
         # Who is the requester for this slot?
         slotReq = QLineEdit(str(self.gui.radioReqNodeID))
         slotReq.setFixedSize(width,height)
+        slotReq.setStyleSheet(self.gui.lineSheet)
         # Who are we ranging to?
         slotResp = QLineEdit(str(base + len(self.layoutSlots) - self.startField))
         slotResp.setFixedSize(width,height)
+        slotResp.setStyleSheet(self.gui.lineSheet)
         # How long does this slow have in table?
         slotPeriod = QLineEdit("20")
         slotPeriod.setFixedSize(width,height)
+        slotPeriod.setStyleSheet(self.gui.lineSheet)
         # Maximum size of data allowed in this slot
         slotDataMax = QLineEdit("100")
         slotDataMax.setFixedSize(width,height)
+        slotDataMax.setStyleSheet(self.gui.lineSheet)
         # Button to move slot down
         but_slotUp = QPushButton("Up")
         but_slotUp.setFixedSize(width,height)
+        but_slotUp.setStyleSheet(self.gui.buttonSheetGray)
         but_slotUp.clicked.connect(self.buttonHandlerUp)
         # Button to move slot down
         but_slotDown = QPushButton("Down")
         but_slotDown.setFixedSize(width,height)
+        but_slotDown.setStyleSheet(self.gui.buttonSheetGray)
         but_slotDown.setObjectName(str(len(self.layoutSlots)))
         but_slotDown.clicked.connect(self.buttonHandlerDown)
         # Button to move slot down
         but_slotAdd = QPushButton("Add")
         but_slotAdd.setFixedSize(width,height)
+        but_slotAdd.setStyleSheet(self.gui.buttonSheetGray)
         but_slotAdd.clicked.connect(self.buttonHandlerAdd)
         # Button to move slot down
         but_slotDel = QPushButton("Del")
         but_slotDel.setFixedSize(width,height)
+        but_slotDel.setStyleSheet(self.gui.buttonSheetGray)
         but_slotDel.setObjectName(str(len(self.layoutSlots)))
         but_slotDel.clicked.connect(self.buttonHandlerDel)
         #Add them all to the horizontal line
         layoutSlotData.addWidget(slotNum,0)
         layoutSlotData.addWidget(slotType,0)
         layoutSlotData.addWidget(slotConfig,0)
         layoutSlotData.addWidget(slotReq,0)
@@ -4340,15 +4411,15 @@
                 self.gui.updateConsole(text)
                 self.buttonHandlerGetMap()
             else:
                 text = "Need to connect to a primary radio@!\n"
                 self.gui.updateConsole(text)
                 self.slotMap = [{"slotIdx":0,"slotType":"SLOT_RANGE","configId":0,"ownerId":100,"targetId":101,"period":20,"maxUserData":10}]
                 self.populateMap()
-            self.but_slotMapSetMap.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+            self.but_slotMapSetMap.setStyleSheet(self.gui.buttonSheetBlue)
 
 
     def buttonHandlerGetMap(self):
         if self.gui.connectedRequester == 1:
             status, self.slotMap, addr = self.gui.radioReq.API.network_GetSlotMap_Request(self.gui.appSettings['reqRadio'])
             self.slotMap = self.slotMap['NETWORKING_GET_SLOT_MAP_CONFIRM']['slotMap']
         else:
@@ -4366,15 +4437,15 @@
             print("No slotmap found, generating default")
             self.buttonHandlerClearMap()
             # self.buttonHandlerSetMap()
         # print("Get\n",self.slotMap)
         self.resetDataArrays()
         self.updateDestMenu()
         self.updateTabs()
-        self.but_slotMapSetMap.setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+        self.but_slotMapSetMap.setStyleSheet(self.gui.buttonSheetBlue)
 
     def resetDataArrays(self):
         self.gui.plotYT = []
         self.gui.plotYB = []
         self.gui.plotX = []
         self.gui.rangeMax = 0
         self.gui.rangeMin = 1000000
@@ -4435,15 +4506,18 @@
 
     def buttonHandlerShowStats(self):
         status, stats, addr = self.gui.radioReq.API.network_Stats_Request(self.gui.appSettings['reqRadio'])
         print(stats)
 
     def buttonHandlerLoadMap(self):
         self.clearMap()
-        filename = QFileDialog.getOpenFileName(self, 'Open SlotMap File', "./slotMaps/slotMap.map", "map (*.map)")
+        if self.gui.platform == "linux":
+            filename = QFileDialog.getOpenFileName(self, 'Open SlotMap File', "./slotMaps/slotMap.map", "map (*.map)", options=QFileDialog.Option.DontUseNativeDialog)
+        else:
+            filename = QFileDialog.getOpenFileName(self, 'Open SlotMap File', "./slotMaps/slotMap.map", "map (*.map)")
         filename = filename[0]
         f = open(filename, "r")
         self.slotMap = loads(f.read())
         self.populateMap()
         self.updateTabs()
         text = "Slotmap loaded\n"
         self.gui.updateConsole(text)
@@ -4457,15 +4531,18 @@
         text = "Slotmap Cleared\n"
         self.gui.updateConsole(text)
         self.updateTabs()
         self.but_slotMapSetMap.setStyleSheet("QPushButton {background-color: coral; color: GhostWhite;}")
 
     def buttonHandlerSaveMap(self):
         self.makeMap()
-        saveName = QFileDialog.getSaveFileName(self, 'Choose SlotMap Name', "./slotMaps/slotMap.map","map (*.map)")
+        if self.gui.platform == "linux":
+            saveName = QFileDialog.getSaveFileName(self, 'Choose SlotMap Name', "./slotMaps/slotMap.map","map (*.map)", options=QFileDialog.Option.DontUseNativeDialog)
+        else:
+            saveName = QFileDialog.getSaveFileName(self, 'Choose SlotMap Name', "./slotMaps/slotMap.map","map (*.map)")
         saveName = saveName[0]
         try:
             f = open(saveName, "w")
             f.write(dumps(self.slotMap))
             f.close()
             text = "Slotmap save successful\n"
             self.gui.updateConsole(text)
@@ -4512,15 +4589,15 @@
             else:
                 if self.gui.radioMode == 'networking':
                     # self.gui.radioStateReq[list([self.gui.radioStateReq.keys()][0])[0]]['state'] = "RADIO_STATE_IDLE"
                     self.gui.dispRespID.setText(str(self.savedNodeId))
                     self.gui.dispRespID.setStyleSheet("QLineEdit {background-color: lightgreen;}")
                     self.gui.radioStateReq[list([self.gui.radioStateReq.keys()][0])[0]]['state'] = "RADIO_STATE_RANGING"
                     self.layoutTop.itemAt(len(self.layoutTop)-1).widget().setText("Start Network")
-                    self.layoutTop.itemAt(len(self.layoutTop)-1).widget().setStyleSheet("QPushButton {background-color: SteelBlue; color: GhostWhite;}")
+                    self.layoutTop.itemAt(len(self.layoutTop)-1).widget().setStyleSheet(self.gui.buttonSheetBlue)
                     self.gui.radioMode = 'idle'
                     self.gui.radioCheckTimer.start()
                     self.gui.radioRanging.networkTimer.stop()
                     # self.gui.guiUpdateTimer.stop()
                     self.netGuiTimer.stop()
                     self.gui.radioStateReq[list([self.gui.radioStateReq.keys()][0])[0]]['flags']  = ""
                     self.gui.radioStateReq[list([self.gui.radioStateReq.keys()][0])[0]]['persistFlag'] = 1
@@ -4740,30 +4817,31 @@
 class windowRangeLarge(QWidget):
     def __init__(self, gui):
         super().__init__()
         # self.setGeometry(10, 10, 1100, 540)
         self.setFixedSize(1100,540)
         self.setWindowTitle("Range Output")
         self.gui = gui
+        self.setStyleSheet(self.gui.windowSheet)
         self.guiFont = guiFonts()
         self.initGUI()
 
     def displayWindow(self):
         self.show()
         xOffset = self.gui.x() + self.gui.mainWindowWidth + 5
         yOffset = self.gui.y()
         self.gui.windowRangeLarge.move(self.gui.monitor.left()+xOffset, self.gui.monitor.top()+yOffset)
 
     def processData(self, range, shade):
-        range = float(range)
-        precRange = f"{range:.3f}"
-        self.dispRange.setText(precRange)
+        # range = float(range)
+        # precRange = f"{range:.3f}"
+        self.dispRange.setText(range)
         tmp = "QLineEdit {background-color: rgb(255," + str(shade) + "," + str(shade) + ");}"
         if range != "-":
-            if int(range) != 0:
+            if range != "0.0":
                 self.dispRange.setStyleSheet(tmp)
             else:
                 self.dispRange.setStyleSheet("QLineEdit {background-color: rgb(255,0,0);}")
         else:
             self.dispRange.setStyleSheet("QLineEdit {background-color: rgb(255,255,255);}")
 
     def initGUI(self):
```

### Comparing `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/TDSR_logging.py` & `TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/TDSR_logging.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from datetime import datetime, date
 from time import time
 from pathlib import Path
 from os import path, mkdir, makedirs
 from json import dumps
 
-__version__ = "1.539"
+__version__ = "1.540"
 
 # All application data logging functions
 class logData():
     def __init__(self, gui):
         self.gui = gui
         self.settings = gui.appSettings
         self.logFile = ""
+        self.msgList = []
+
 # Creates a new filename and directory under the chosen log directory.
 #  Naming is cased on radio nodes and times logs were taken. Autogenerated filenames.
     def createTimeBasedLog(self, nodeIPs):
         if self.gui.connectedRequester == 1:
+            self.msgList = []
             print("Time Based Log")
             today = date.today()
             nodeStr = nodeIPs[0]
             self.startDataTime = time()
             dateDirectory = "RN_NODES" + nodeStr + "_" + today.strftime("%m-%d-%y")
             dataDirectoryName = path.join(self.settings['logDirectory'],dateDirectory)
             if not path.isdir(dataDirectoryName):
@@ -36,14 +39,15 @@
             self.logFile.write(dumps(self.gui.radioReqNodeIDMsg))
             self.logFile.write("\n\n")
             print(logFileName)
 # Creates a new filename and directory under the chosen log directory. Subdirectory is created for Month/Year
 #  log was taken. Name is based on user entered base name with 4 digit increasing file counter at the end.
     def createNameBasedLog(self):
         if self.gui.connectedRequester == 1:
+            self.msgList = []
             logFileName = self.settings['logFile']
             logFilePath = self.settings['logDirectory']
             print("Name Based Log")
             self.startDataTime = time()
             self.logFile = logFilePath + logFileName
             tmp = Path(logFilePath)
             if tmp.is_dir() == False:
@@ -100,36 +104,49 @@
                     if self.settings['logDateBased'] == 1:
                         self.createTimeBasedLog(nodeIPs)
                     else:
                         self.createNameBasedLog()
         # do the logging
         if packet != None:
             # if Json
-            # if self.settings['logJson'] == 1:
+            if self.settings['logJson'] == 1:
             # if range info only
-            if self.settings['logRangeInfoOnly'] == 1:
-                if "RANGE_INFO" in packet.keys():
+                if self.settings['logRangeInfoOnly'] == 1:
+                    if "RANGE_INFO" in packet.keys():
+                        self.logFile.write(dumps(packet))
+                        self.logFile.write("\n")
+                else:
                     self.logFile.write(dumps(packet))
                     self.logFile.write("\n")
-            else:
-                self.logFile.write(dumps(packet))
-                self.logFile.write("\n")
             # if csv
-            # else:
-                # if "RANGE_INFO" in packet.keys():
-                #         msg = packet['RANGE_INFO']
-                #         text = ""
-                #         for field in msg.keys():
-                #             text = text + str(msg[field]) + ","
-                #         text = text[:len(text)-1] + "\n"
-                #         self.logFile.write(text)
-                #     tmp = dict()
-                #     tmp['RANGE_ONLY'] = dict()
-                #     tmp['RANGE_ONLY']['msgId'] = packet['RANGE_INFO']['msgId']
-                #     tmp['RANGE_ONLY']['precisionRangeM'] = packet['RANGE_INFO']['precisionRangeM']
-                #     self.logFile.write(dumps(tmp))
+            else:
+                msgKey = list(packet.keys())
+                if self.settings['logRangeInfoOnly'] == 1:
+                    if msgKey[0] == "RANGE_INFO":
+                        if msgKey[0] not in self.msgList:
+                            self.msgList.append(msgKey[0])
+                            self.logFile.write(dumps(packet))
+                            self.logFile.write("\n")
+                        msg = packet['RANGE_INFO']
+                        text = ""
+                        for field in msg.keys():
+                            text = text + str(msg[field]) + ","
+                        text = text[:len(text)-1] + "\n"
+                        self.logFile.write(text)
+                else:
+                    if msgKey[0] not in self.msgList:
+                        self.msgList.append(msgKey[0])
+                        self.logFile.write(dumps(packet))
+                        self.logFile.write("\n")
+                    msg = packet[msgKey[0]]
+                    text = ""
+                    for field in msg.keys():
+                        text = text + str(msg[field]) + ","
+                    text = text[:len(text)-1] + "\n"
+                    self.logFile.write(text)
+
 # Closes logfile if open
     def closeLogFile(self):
         if self.logFile != "":
             self.logFile.close()
             self.logFile = ""
             print("Closed Log")
```

### Comparing `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/TDSR_radioAPI.py` & `TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/TDSR_radioAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from json import dumps
 from time import sleep
 
-__version__ = "1.539"
+__version__ = "1.540"
 
 class RadioAPI:
     _msgId = 0
 
     def __init__(self, messageQueues, messageList, TxQueue):
         self.TxQueue = TxQueue
         self.messageList = messageList
```

### Comparing `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/TDSR_radioConnection.py` & `TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/TDSR_radioConnection.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import serial
 import serial.tools.list_ports
 import ipaddress
 import netifaces
 
 from TDSR_Support import TDSR_radioAPI
 
-__version__ = "1.539"
+__version__ = "1.540"
 
 # Use netifaces to find local IP addresses.
 netifaces_available = False
 try:
     import netifaces
     netifaces_available = True
 
@@ -115,15 +115,15 @@
                                     ...
                                     # print("Dumping Request")
                     else:
                         print("RX Thread: MessageType not in API keys")
                         print(f"   Type: {msgType}")
                         print(f"   Keys: {self.API.messageList.keys()}")
                         print(f"   Type: {packet}")
-                    if self.gui.appSettings['enableLogging'] == 1 and self.gui.radioMode != "idle":
+                    if self.gui.appSettings['enableLogging'] == 1 and (self.gui.radioMode != "idle" or self.gui.appSettings['logWhileIdle'] == 1):
                         self.gui.logFile.logToFile(packet, self.gui.appSettings['reqRadio'])
             except:
                 pass
 
     def findUsbRadios(self):
         radios = []
         ports = [port for port in serial.tools.list_ports.comports() if port != "n/a" and port.vid == 0x1027 and port.pid == 0x1234]
```

### Comparing `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/TDSR_radioControl.py` & `TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/TDSR_radioControl.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from time import time, sleep
 from math import sqrt, log10
 from numpy import power
 from pathlib import Path
 from base64 import b64encode, b64decode
 from threading import Thread
 
-__version__ = "1.539"
+__version__ = "1.540"
 
 # Primary ranging functions
 class rangeCmds():
     def __init__(self, gui):
         self.gui = gui
         self.appSetup()
```

### Comparing `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/TDSR_settings.py` & `TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/TDSR_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 from json import dumps, loads
 
-__version__ = "1.539"
+__version__ = "1.540"
 
 # loads and saves GUI settings. Also sets default values if settings file does not include all keys.
 class appSettings():
     def __init__(self):
         self.settings = {}
 
     def settingsSetup(self):
@@ -35,14 +35,16 @@
                 self.settings['respID'] = "101"
             if 'logDirectory' not in self.settings:
                 self.settings['logDirectory'] = "./data_directory/"
             if 'logFile' not in self.settings:
                 self.settings['logFile'] = "logfile.log"
             if 'logJson' not in self.settings:
                 self.settings['logJson'] = 1
+            if 'logWhileIdle' not in self.settings:
+                self.settings['logWhileIdle'] = 0
             if 'enableLogging' not in self.settings:
                 self.settings['enableLogging'] = 0
             if 'logRangeInfoOnly' not in self.settings:
                 self.settings['logRangeInfoOnly'] = 1
             if 'logDateBased' not in self.settings:
                 self.settings['logDateBased'] = 0
             if 'logSegmented' not in self.settings:
@@ -65,14 +67,15 @@
             self.settings['rangeRate'] = 5
             self.settings['reqRadio'] = "192.168.1.51"
             self.settings['respRadio'] = "192.168.1.52"
             self.settings['respID'] = "52"
             self.settings['logDirectory'] = "./data_directory/"
             self.settings['logFile'] = "logfile.log"
             self.settings['logJson'] = 1
+            self.settings['logWhileIdle'] = 0
             self.settings['enableLogging'] = 0
             self.settings['logRangeInfoOnly'] = 1
             self.settings['logDateBased'] = 0
             self.settings['logSegmented'] = 0
             self.settings['segmentTime'] = 60
             self.settings['guiUpdateRate'] = 10
             self.settings['downloadDirectory'] = "./Downloads/"
```

### Comparing `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/crc16.py` & `TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/crc16.py`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.539/TDSR-UWB/TDSR_Support/logReader.py` & `TDSR-UWB-1.540/TDSR-UWB/TDSR_Support/logReader.py`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.539/TDSR-UWB/TDSR_UWB.egg-info/PKG-INFO` & `TDSR-UWB-1.540/TDSR-UWB/TDSR_UWB.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDSR-UWB
-Version: 1.539
+Version: 1.540
 Summary: Support libraries for TDSR LLC UWB Radios
 Home-page: UNKNOWN
 Author: TDSR-LLC
 Author-email: contact@tdsr-uwb.com
 License: UNKNOWN
 Project-URL: Company:, https://www.tdsr-uwb.com
 Platform: UNKNOWN
```

### Comparing `TDSR-UWB-1.539/TDSR-UWB/TDSR_UWB.egg-info/SOURCES.txt` & `TDSR-UWB-1.540/TDSR-UWB/TDSR_UWB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.539/setup.py` & `TDSR-UWB-1.540/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     name="TDSR-UWB",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="1.539",  # Required
+    version="1.540",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Support libraries for TDSR LLC UWB Radios",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

