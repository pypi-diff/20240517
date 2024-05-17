# Comparing `tmp/PythonToSW-1.2.0.tar.gz` & `tmp/PythonToSW-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonToSW-1.2.0.tar", last modified: Thu May 16 22:39:11 2024, max compression
+gzip compressed data, was "PythonToSW-1.2.1.tar", last modified: Thu May 16 22:45:56 2024, max compression
```

## Comparing `PythonToSW-1.2.0.tar` & `PythonToSW-1.2.1.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 22:39:11.565206 PythonToSW-1.2.0/
--rw-rw-rw-   0        0        0    11558 2024-01-17 15:06:42.000000 PythonToSW-1.2.0/LICENSE
--rw-rw-rw-   0        0        0       92 2024-05-15 22:14:52.000000 PythonToSW-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1803 2024-05-16 22:39:11.563716 PythonToSW-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1242 2024-05-16 22:19:42.000000 PythonToSW-1.2.0/README.md
--rw-rw-rw-   0        0        0        5 2024-05-16 22:39:04.000000 PythonToSW-1.2.0/VERSION
--rw-rw-rw-   0        0        0       62 2024-05-16 22:06:47.000000 PythonToSW-1.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 22:39:11.565206 PythonToSW-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1878 2024-05-15 22:15:23.000000 PythonToSW-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 22:39:11.428155 PythonToSW-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-16 22:39:11.438942 PythonToSW-1.2.0/src/PythonToSW/
--rw-rw-rw-   0        0        0      973 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 22:39:11.471940 PythonToSW-1.2.0/src/PythonToSW/addon/
--rw-rw-rw-   0        0        0      315 2024-05-16 03:46:54.000000 PythonToSW-1.2.0/src/PythonToSW/addon/playlist.xml
--rw-rw-rw-   0        0        0   161117 2024-05-16 21:57:12.000000 PythonToSW-1.2.0/src/PythonToSW/addon/script.lua
--rw-rw-rw-   0        0        0    14905 2024-05-16 22:37:18.000000 PythonToSW-1.2.0/src/PythonToSW/addon.py
--rw-rw-rw-   0        0        0     1868 2024-05-16 22:33:36.000000 PythonToSW-1.2.0/src/PythonToSW/event.py
--rw-rw-rw-   0        0        0     1114 2024-05-16 03:34:55.000000 PythonToSW-1.2.0/src/PythonToSW/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-16 22:39:11.559641 PythonToSW-1.2.0/src/PythonToSW/executions/
--rw-rw-rw-   0        0        0     2809 2024-05-14 23:36:22.000000 PythonToSW-1.2.0/src/PythonToSW/executions/__createExecution.py
--rw-rw-rw-   0        0        0     1711 2024-05-14 23:24:00.000000 PythonToSW-1.2.0/src/PythonToSW/executions/__generateImportCode.py
--rw-rw-rw-   0        0        0     5825 2024-05-16 22:21:16.000000 PythonToSW-1.2.0/src/PythonToSW/executions/__init__.py
--rw-rw-rw-   0        0        0     1059 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/addAdmin.py
--rw-rw-rw-   0        0        0     1056 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/addAuth.py
--rw-rw-rw-   0        0        0     1216 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/addMapLabel.py
--rw-rw-rw-   0        0        0     1220 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/addMapLine.py
--rw-rw-rw-   0        0        0     1582 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/addMapObject.py
--rw-rw-rw-   0        0        0     1107 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/announce.py
--rw-rw-rw-   0        0        0     1027 2024-05-14 23:48:22.000000 PythonToSW-1.2.0/src/PythonToSW/executions/cancelGerstner.py
--rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/clearOilSpills.py
--rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/clearRadiation.py
--rw-rw-rw-   0        0        0     1025 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/clearVehicles.py
--rw-rw-rw-   0        0        0     1106 2024-05-14 23:49:23.000000 PythonToSW-1.2.0/src/PythonToSW/executions/despawnObject.py
--rw-rw-rw-   0        0        0     1111 2024-05-14 23:49:25.000000 PythonToSW-1.2.0/src/PythonToSW/executions/despawnVehicle.py
--rw-rw-rw-   0        0        0     1123 2024-05-14 23:49:26.000000 PythonToSW-1.2.0/src/PythonToSW/executions/despawnVehicleGroup.py
--rw-rw-rw-   0        0        0     1025 2024-05-16 04:08:52.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getAddonIndex.py
--rw-rw-rw-   0        0        0     1105 2024-05-14 18:26:42.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getCharacterItem.py
--rw-rw-rw-   0        0        0     1018 2024-05-15 22:28:57.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getCurrency.py
--rw-rw-rw-   0        0        0     1031 2024-05-16 22:21:02.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getGameSettings.py
--rw-rw-rw-   0        0        0     1079 2024-05-14 18:24:19.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getObjectData.py
--rw-rw-rw-   0        0        0     1092 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getPlayerCharacter.py
--rw-rw-rw-   0        0        0     1103 2024-05-16 00:01:47.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getPlayerLookDirection.py
--rw-rw-rw-   0        0        0     1075 2024-05-16 00:01:47.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getPlayerName.py
--rw-rw-rw-   0        0        0     1072 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getPlayerPos.py
--rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getPlayers.py
--rw-rw-rw-   0        0        0     1035 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getSeasonalEvent.py
--rw-rw-rw-   0        0        0     1017 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getUniqueID.py
--rw-rw-rw-   0        0        0     1138 2024-05-14 23:44:48.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleBatteryByName.py
--rw-rw-rw-   0        0        0     1172 2024-05-14 23:44:45.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleBatteryByVoxel.py
--rw-rw-rw-   0        0        0     1102 2024-05-14 18:30:01.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleComponents.py
--rw-rw-rw-   0        0        0     1084 2024-05-14 18:29:46.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleData.py
--rw-rw-rw-   0        0        0     1083 2024-05-15 22:28:49.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleGroup.py
--rw-rw-rw-   0        0        0     1162 2024-05-15 22:08:55.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getVehiclePos.py
--rw-rw-rw-   0        0        0     1123 2024-05-14 23:44:59.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleTankByName.py
--rw-rw-rw-   0        0        0     1163 2024-05-14 23:45:28.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleTankByVoxel.py
--rw-rw-rw-   0        0        0     1012 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/isAridDLC.py
--rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/isSpaceDLC.py
--rw-rw-rw-   0        0        0     1021 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/isWeaponsDLC.py
--rw-rw-rw-   0        0        0     1080 2024-05-16 00:01:47.000000 PythonToSW-1.2.0/src/PythonToSW/executions/moveGroup.py
--rw-rw-rw-   0        0        0     1093 2024-05-16 00:01:47.000000 PythonToSW-1.2.0/src/PythonToSW/executions/moveGroupSafe.py
--rw-rw-rw-   0        0        0     1090 2024-05-16 00:01:47.000000 PythonToSW-1.2.0/src/PythonToSW/executions/moveVehicle.py
--rw-rw-rw-   0        0        0     1103 2024-05-16 00:02:01.000000 PythonToSW-1.2.0/src/PythonToSW/executions/moveVehicleSafe.py
--rw-rw-rw-   0        0        0     1135 2024-05-14 23:47:34.000000 PythonToSW-1.2.0/src/PythonToSW/executions/notify.py
--rw-rw-rw-   0        0        0     1068 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/removeAdmin.py
--rw-rw-rw-   0        0        0     1065 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/removeAuth.py
--rw-rw-rw-   0        0        0     1097 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/removeMapLabel.py
--rw-rw-rw-   0        0        0     1094 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/removeMapLine.py
--rw-rw-rw-   0        0        0     1100 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/removeMapObject.py
--rw-rw-rw-   0        0        0     1087 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/removePopup.py
--rw-rw-rw-   0        0        0     1171 2024-05-14 18:25:00.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setCharacterData.py
--rw-rw-rw-   0        0        0     1222 2024-05-14 18:26:10.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setCharacterItem.py
--rw-rw-rw-   0        0        0     1120 2024-05-14 18:25:27.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setCharacterTooltip.py
--rw-rw-rw-   0        0        0     1115 2024-05-14 23:49:29.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setCreatureMoveTarget.py
--rw-rw-rw-   0        0        0     1115 2024-05-15 22:28:48.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setCurrency.py
--rw-rw-rw-   0        0        0     1120 2024-05-16 22:20:48.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setGameSetting.py
--rw-rw-rw-   0        0        0     1100 2024-05-16 00:01:49.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setGroupPosSafe.py
--rw-rw-rw-   0        0        0     1089 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setOilSpill.py
--rw-rw-rw-   0        0        0     1088 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setPlayerPos.py
--rw-rw-rw-   0        0        0     1299 2024-05-14 18:18:44.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setPopup.py
--rw-rw-rw-   0        0        0     1161 2024-05-14 23:43:28.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleBatteryByName.py
--rw-rw-rw-   0        0        0     1194 2024-05-14 23:42:27.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleBatteryByVoxel.py
--rw-rw-rw-   0        0        0     1126 2024-05-14 23:39:49.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleEditable.py
--rw-rw-rw-   0        0        0     1146 2024-05-14 23:39:47.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleInvulnerable.py
--rw-rw-rw-   0        0        0     1097 2024-05-15 22:08:43.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setVehiclePos.py
--rw-rw-rw-   0        0        0     1110 2024-05-16 00:01:47.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setVehiclePosSafe.py
--rw-rw-rw-   0        0        0     1123 2024-05-14 23:39:52.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleShowOnMap.py
--rw-rw-rw-   0        0        0     1146 2024-05-14 23:43:54.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleTankByName.py
--rw-rw-rw-   0        0        0     1186 2024-05-14 23:44:14.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleTankByVoxel.py
--rw-rw-rw-   0        0        0     1122 2024-05-16 04:03:12.000000 PythonToSW-1.2.0/src/PythonToSW/executions/spawnAddonVehicle.py
--rw-rw-rw-   0        0        0     1095 2024-05-14 23:46:38.000000 PythonToSW-1.2.0/src/PythonToSW/executions/spawnCharacter.py
--rw-rw-rw-   0        0        0     1143 2024-05-14 23:47:06.000000 PythonToSW-1.2.0/src/PythonToSW/executions/spawnCreature.py
--rw-rw-rw-   0        0        0     1157 2024-05-16 04:03:12.000000 PythonToSW-1.2.0/src/PythonToSW/executions/spawnEquipment.py
--rw-rw-rw-   0        0        0     1099 2024-05-14 23:47:30.000000 PythonToSW-1.2.0/src/PythonToSW/executions/spawnExplosion.py
--rw-rw-rw-   0        0        0     1128 2024-05-14 23:46:36.000000 PythonToSW-1.2.0/src/PythonToSW/executions/spawnMeteor.py
--rw-rw-rw-   0        0        0     1147 2024-05-14 23:45:56.000000 PythonToSW-1.2.0/src/PythonToSW/executions/spawnMeteorShower.py
--rw-rw-rw-   0        0        0     1090 2024-05-16 04:03:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/spawnObject.py
--rw-rw-rw-   0        0        0     1093 2024-05-14 23:45:58.000000 PythonToSW-1.2.0/src/PythonToSW/executions/spawnTsunami.py
--rw-rw-rw-   0        0        0     1089 2024-05-16 04:03:12.000000 PythonToSW-1.2.0/src/PythonToSW/executions/spawnVehicle.py
--rw-rw-rw-   0        0        0     1093 2024-05-14 23:45:54.000000 PythonToSW-1.2.0/src/PythonToSW/executions/spawnVolcano.py
--rw-rw-rw-   0        0        0     1099 2024-05-14 23:45:59.000000 PythonToSW-1.2.0/src/PythonToSW/executions/spawnWhirlpool.py
--rw-rw-rw-   0        0        0     1618 2024-05-16 03:09:58.000000 PythonToSW-1.2.0/src/PythonToSW/helpers.py
--rw-rw-rw-   0        0        0     1428 2024-05-15 22:17:00.000000 PythonToSW-1.2.0/src/PythonToSW/matrix.py
-drwxrwxrwx   0        0        0        0 2024-05-16 22:39:11.561941 PythonToSW-1.2.0/src/PythonToSW.egg-info/
--rw-rw-rw-   0        0        0     1803 2024-05-16 22:39:11.000000 PythonToSW-1.2.0/src/PythonToSW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4065 2024-05-16 22:39:11.000000 PythonToSW-1.2.0/src/PythonToSW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 22:39:11.000000 PythonToSW-1.2.0/src/PythonToSW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-05-16 22:39:11.000000 PythonToSW-1.2.0/src/PythonToSW.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-16 22:39:11.000000 PythonToSW-1.2.0/src/PythonToSW.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 22:45:56.379657 PythonToSW-1.2.1/
+-rw-rw-rw-   0        0        0    11558 2024-01-17 15:06:42.000000 PythonToSW-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0       92 2024-05-15 22:14:52.000000 PythonToSW-1.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1803 2024-05-16 22:45:56.378134 PythonToSW-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1242 2024-05-16 22:19:42.000000 PythonToSW-1.2.1/README.md
+-rw-rw-rw-   0        0        0        5 2024-05-16 22:45:50.000000 PythonToSW-1.2.1/VERSION
+-rw-rw-rw-   0        0        0       62 2024-05-16 22:06:47.000000 PythonToSW-1.2.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 22:45:56.380661 PythonToSW-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1878 2024-05-15 22:15:23.000000 PythonToSW-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 22:45:56.286203 PythonToSW-1.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-16 22:45:56.296108 PythonToSW-1.2.1/src/PythonToSW/
+-rw-rw-rw-   0        0        0      973 2024-05-14 16:56:13.000000 PythonToSW-1.2.1/src/PythonToSW/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 22:45:56.311404 PythonToSW-1.2.1/src/PythonToSW/addon/
+-rw-rw-rw-   0        0        0      315 2024-05-16 03:46:54.000000 PythonToSW-1.2.1/src/PythonToSW/addon/playlist.xml
+-rw-rw-rw-   0        0        0   161117 2024-05-16 21:57:12.000000 PythonToSW-1.2.1/src/PythonToSW/addon/script.lua
+-rw-rw-rw-   0        0        0    14680 2024-05-16 22:43:59.000000 PythonToSW-1.2.1/src/PythonToSW/addon.py
+-rw-rw-rw-   0        0        0     1868 2024-05-16 22:33:36.000000 PythonToSW-1.2.1/src/PythonToSW/event.py
+-rw-rw-rw-   0        0        0     1114 2024-05-16 03:34:55.000000 PythonToSW-1.2.1/src/PythonToSW/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-16 22:45:56.375354 PythonToSW-1.2.1/src/PythonToSW/executions/
+-rw-rw-rw-   0        0        0     2809 2024-05-14 23:36:22.000000 PythonToSW-1.2.1/src/PythonToSW/executions/__createExecution.py
+-rw-rw-rw-   0        0        0     1711 2024-05-14 23:24:00.000000 PythonToSW-1.2.1/src/PythonToSW/executions/__generateImportCode.py
+-rw-rw-rw-   0        0        0     5825 2024-05-16 22:21:16.000000 PythonToSW-1.2.1/src/PythonToSW/executions/__init__.py
+-rw-rw-rw-   0        0        0     1059 2024-05-14 16:56:13.000000 PythonToSW-1.2.1/src/PythonToSW/executions/addAdmin.py
+-rw-rw-rw-   0        0        0     1056 2024-05-14 16:56:13.000000 PythonToSW-1.2.1/src/PythonToSW/executions/addAuth.py
+-rw-rw-rw-   0        0        0     1216 2024-05-14 16:56:13.000000 PythonToSW-1.2.1/src/PythonToSW/executions/addMapLabel.py
+-rw-rw-rw-   0        0        0     1220 2024-05-14 16:56:13.000000 PythonToSW-1.2.1/src/PythonToSW/executions/addMapLine.py
+-rw-rw-rw-   0        0        0     1582 2024-05-14 16:56:13.000000 PythonToSW-1.2.1/src/PythonToSW/executions/addMapObject.py
+-rw-rw-rw-   0        0        0     1107 2024-05-14 16:56:13.000000 PythonToSW-1.2.1/src/PythonToSW/executions/announce.py
+-rw-rw-rw-   0        0        0     1027 2024-05-14 23:48:22.000000 PythonToSW-1.2.1/src/PythonToSW/executions/cancelGerstner.py
+-rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.2.1/src/PythonToSW/executions/clearOilSpills.py
+-rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.2.1/src/PythonToSW/executions/clearRadiation.py
+-rw-rw-rw-   0        0        0     1025 2024-05-14 16:56:13.000000 PythonToSW-1.2.1/src/PythonToSW/executions/clearVehicles.py
+-rw-rw-rw-   0        0        0     1106 2024-05-14 23:49:23.000000 PythonToSW-1.2.1/src/PythonToSW/executions/despawnObject.py
+-rw-rw-rw-   0        0        0     1111 2024-05-14 23:49:25.000000 PythonToSW-1.2.1/src/PythonToSW/executions/despawnVehicle.py
+-rw-rw-rw-   0        0        0     1123 2024-05-14 23:49:26.000000 PythonToSW-1.2.1/src/PythonToSW/executions/despawnVehicleGroup.py
+-rw-rw-rw-   0        0        0     1025 2024-05-16 04:08:52.000000 PythonToSW-1.2.1/src/PythonToSW/executions/getAddonIndex.py
+-rw-rw-rw-   0        0        0     1105 2024-05-14 18:26:42.000000 PythonToSW-1.2.1/src/PythonToSW/executions/getCharacterItem.py
+-rw-rw-rw-   0        0        0     1018 2024-05-15 22:28:57.000000 PythonToSW-1.2.1/src/PythonToSW/executions/getCurrency.py
+-rw-rw-rw-   0        0        0     1031 2024-05-16 22:21:02.000000 PythonToSW-1.2.1/src/PythonToSW/executions/getGameSettings.py
+-rw-rw-rw-   0        0        0     1079 2024-05-14 18:24:19.000000 PythonToSW-1.2.1/src/PythonToSW/executions/getObjectData.py
+-rw-rw-rw-   0        0        0     1092 2024-05-14 16:56:13.000000 PythonToSW-1.2.1/src/PythonToSW/executions/getPlayerCharacter.py
+-rw-rw-rw-   0        0        0     1103 2024-05-16 00:01:47.000000 PythonToSW-1.2.1/src/PythonToSW/executions/getPlayerLookDirection.py
+-rw-rw-rw-   0        0        0     1075 2024-05-16 00:01:47.000000 PythonToSW-1.2.1/src/PythonToSW/executions/getPlayerName.py
+-rw-rw-rw-   0        0        0     1072 2024-05-14 16:56:13.000000 PythonToSW-1.2.1/src/PythonToSW/executions/getPlayerPos.py
+-rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.2.1/src/PythonToSW/executions/getPlayers.py
+-rw-rw-rw-   0        0        0     1035 2024-05-14 16:56:13.000000 PythonToSW-1.2.1/src/PythonToSW/executions/getSeasonalEvent.py
+-rw-rw-rw-   0        0        0     1017 2024-05-14 16:56:13.000000 PythonToSW-1.2.1/src/PythonToSW/executions/getUniqueID.py
+-rw-rw-rw-   0        0        0     1138 2024-05-14 23:44:48.000000 PythonToSW-1.2.1/src/PythonToSW/executions/getVehicleBatteryByName.py
+-rw-rw-rw-   0        0        0     1172 2024-05-14 23:44:45.000000 PythonToSW-1.2.1/src/PythonToSW/executions/getVehicleBatteryByVoxel.py
+-rw-rw-rw-   0        0        0     1102 2024-05-14 18:30:01.000000 PythonToSW-1.2.1/src/PythonToSW/executions/getVehicleComponents.py
+-rw-rw-rw-   0        0        0     1084 2024-05-14 18:29:46.000000 PythonToSW-1.2.1/src/PythonToSW/executions/getVehicleData.py
+-rw-rw-rw-   0        0        0     1083 2024-05-15 22:28:49.000000 PythonToSW-1.2.1/src/PythonToSW/executions/getVehicleGroup.py
+-rw-rw-rw-   0        0        0     1162 2024-05-15 22:08:55.000000 PythonToSW-1.2.1/src/PythonToSW/executions/getVehiclePos.py
+-rw-rw-rw-   0        0        0     1123 2024-05-14 23:44:59.000000 PythonToSW-1.2.1/src/PythonToSW/executions/getVehicleTankByName.py
+-rw-rw-rw-   0        0        0     1163 2024-05-14 23:45:28.000000 PythonToSW-1.2.1/src/PythonToSW/executions/getVehicleTankByVoxel.py
+-rw-rw-rw-   0        0        0     1012 2024-05-14 16:56:13.000000 PythonToSW-1.2.1/src/PythonToSW/executions/isAridDLC.py
+-rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.2.1/src/PythonToSW/executions/isSpaceDLC.py
+-rw-rw-rw-   0        0        0     1021 2024-05-14 16:56:13.000000 PythonToSW-1.2.1/src/PythonToSW/executions/isWeaponsDLC.py
+-rw-rw-rw-   0        0        0     1080 2024-05-16 00:01:47.000000 PythonToSW-1.2.1/src/PythonToSW/executions/moveGroup.py
+-rw-rw-rw-   0        0        0     1093 2024-05-16 00:01:47.000000 PythonToSW-1.2.1/src/PythonToSW/executions/moveGroupSafe.py
+-rw-rw-rw-   0        0        0     1090 2024-05-16 00:01:47.000000 PythonToSW-1.2.1/src/PythonToSW/executions/moveVehicle.py
+-rw-rw-rw-   0        0        0     1103 2024-05-16 00:02:01.000000 PythonToSW-1.2.1/src/PythonToSW/executions/moveVehicleSafe.py
+-rw-rw-rw-   0        0        0     1135 2024-05-14 23:47:34.000000 PythonToSW-1.2.1/src/PythonToSW/executions/notify.py
+-rw-rw-rw-   0        0        0     1068 2024-05-14 16:56:13.000000 PythonToSW-1.2.1/src/PythonToSW/executions/removeAdmin.py
+-rw-rw-rw-   0        0        0     1065 2024-05-14 16:56:13.000000 PythonToSW-1.2.1/src/PythonToSW/executions/removeAuth.py
+-rw-rw-rw-   0        0        0     1097 2024-05-14 16:56:13.000000 PythonToSW-1.2.1/src/PythonToSW/executions/removeMapLabel.py
+-rw-rw-rw-   0        0        0     1094 2024-05-14 16:56:13.000000 PythonToSW-1.2.1/src/PythonToSW/executions/removeMapLine.py
+-rw-rw-rw-   0        0        0     1100 2024-05-14 16:56:13.000000 PythonToSW-1.2.1/src/PythonToSW/executions/removeMapObject.py
+-rw-rw-rw-   0        0        0     1087 2024-05-14 16:56:13.000000 PythonToSW-1.2.1/src/PythonToSW/executions/removePopup.py
+-rw-rw-rw-   0        0        0     1171 2024-05-14 18:25:00.000000 PythonToSW-1.2.1/src/PythonToSW/executions/setCharacterData.py
+-rw-rw-rw-   0        0        0     1222 2024-05-14 18:26:10.000000 PythonToSW-1.2.1/src/PythonToSW/executions/setCharacterItem.py
+-rw-rw-rw-   0        0        0     1120 2024-05-14 18:25:27.000000 PythonToSW-1.2.1/src/PythonToSW/executions/setCharacterTooltip.py
+-rw-rw-rw-   0        0        0     1115 2024-05-14 23:49:29.000000 PythonToSW-1.2.1/src/PythonToSW/executions/setCreatureMoveTarget.py
+-rw-rw-rw-   0        0        0     1115 2024-05-15 22:28:48.000000 PythonToSW-1.2.1/src/PythonToSW/executions/setCurrency.py
+-rw-rw-rw-   0        0        0     1120 2024-05-16 22:20:48.000000 PythonToSW-1.2.1/src/PythonToSW/executions/setGameSetting.py
+-rw-rw-rw-   0        0        0     1100 2024-05-16 00:01:49.000000 PythonToSW-1.2.1/src/PythonToSW/executions/setGroupPosSafe.py
+-rw-rw-rw-   0        0        0     1089 2024-05-14 16:56:13.000000 PythonToSW-1.2.1/src/PythonToSW/executions/setOilSpill.py
+-rw-rw-rw-   0        0        0     1088 2024-05-14 16:56:13.000000 PythonToSW-1.2.1/src/PythonToSW/executions/setPlayerPos.py
+-rw-rw-rw-   0        0        0     1299 2024-05-14 18:18:44.000000 PythonToSW-1.2.1/src/PythonToSW/executions/setPopup.py
+-rw-rw-rw-   0        0        0     1161 2024-05-14 23:43:28.000000 PythonToSW-1.2.1/src/PythonToSW/executions/setVehicleBatteryByName.py
+-rw-rw-rw-   0        0        0     1194 2024-05-14 23:42:27.000000 PythonToSW-1.2.1/src/PythonToSW/executions/setVehicleBatteryByVoxel.py
+-rw-rw-rw-   0        0        0     1126 2024-05-14 23:39:49.000000 PythonToSW-1.2.1/src/PythonToSW/executions/setVehicleEditable.py
+-rw-rw-rw-   0        0        0     1146 2024-05-14 23:39:47.000000 PythonToSW-1.2.1/src/PythonToSW/executions/setVehicleInvulnerable.py
+-rw-rw-rw-   0        0        0     1097 2024-05-15 22:08:43.000000 PythonToSW-1.2.1/src/PythonToSW/executions/setVehiclePos.py
+-rw-rw-rw-   0        0        0     1110 2024-05-16 00:01:47.000000 PythonToSW-1.2.1/src/PythonToSW/executions/setVehiclePosSafe.py
+-rw-rw-rw-   0        0        0     1123 2024-05-14 23:39:52.000000 PythonToSW-1.2.1/src/PythonToSW/executions/setVehicleShowOnMap.py
+-rw-rw-rw-   0        0        0     1146 2024-05-14 23:43:54.000000 PythonToSW-1.2.1/src/PythonToSW/executions/setVehicleTankByName.py
+-rw-rw-rw-   0        0        0     1186 2024-05-14 23:44:14.000000 PythonToSW-1.2.1/src/PythonToSW/executions/setVehicleTankByVoxel.py
+-rw-rw-rw-   0        0        0     1122 2024-05-16 04:03:12.000000 PythonToSW-1.2.1/src/PythonToSW/executions/spawnAddonVehicle.py
+-rw-rw-rw-   0        0        0     1095 2024-05-14 23:46:38.000000 PythonToSW-1.2.1/src/PythonToSW/executions/spawnCharacter.py
+-rw-rw-rw-   0        0        0     1143 2024-05-14 23:47:06.000000 PythonToSW-1.2.1/src/PythonToSW/executions/spawnCreature.py
+-rw-rw-rw-   0        0        0     1157 2024-05-16 04:03:12.000000 PythonToSW-1.2.1/src/PythonToSW/executions/spawnEquipment.py
+-rw-rw-rw-   0        0        0     1099 2024-05-14 23:47:30.000000 PythonToSW-1.2.1/src/PythonToSW/executions/spawnExplosion.py
+-rw-rw-rw-   0        0        0     1128 2024-05-14 23:46:36.000000 PythonToSW-1.2.1/src/PythonToSW/executions/spawnMeteor.py
+-rw-rw-rw-   0        0        0     1147 2024-05-14 23:45:56.000000 PythonToSW-1.2.1/src/PythonToSW/executions/spawnMeteorShower.py
+-rw-rw-rw-   0        0        0     1090 2024-05-16 04:03:13.000000 PythonToSW-1.2.1/src/PythonToSW/executions/spawnObject.py
+-rw-rw-rw-   0        0        0     1093 2024-05-14 23:45:58.000000 PythonToSW-1.2.1/src/PythonToSW/executions/spawnTsunami.py
+-rw-rw-rw-   0        0        0     1089 2024-05-16 04:03:12.000000 PythonToSW-1.2.1/src/PythonToSW/executions/spawnVehicle.py
+-rw-rw-rw-   0        0        0     1093 2024-05-14 23:45:54.000000 PythonToSW-1.2.1/src/PythonToSW/executions/spawnVolcano.py
+-rw-rw-rw-   0        0        0     1099 2024-05-14 23:45:59.000000 PythonToSW-1.2.1/src/PythonToSW/executions/spawnWhirlpool.py
+-rw-rw-rw-   0        0        0     1618 2024-05-16 03:09:58.000000 PythonToSW-1.2.1/src/PythonToSW/helpers.py
+-rw-rw-rw-   0        0        0     1428 2024-05-15 22:17:00.000000 PythonToSW-1.2.1/src/PythonToSW/matrix.py
+drwxrwxrwx   0        0        0        0 2024-05-16 22:45:56.377131 PythonToSW-1.2.1/src/PythonToSW.egg-info/
+-rw-rw-rw-   0        0        0     1803 2024-05-16 22:45:56.000000 PythonToSW-1.2.1/src/PythonToSW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4065 2024-05-16 22:45:56.000000 PythonToSW-1.2.1/src/PythonToSW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 22:45:56.000000 PythonToSW-1.2.1/src/PythonToSW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-16 22:45:56.000000 PythonToSW-1.2.1/src/PythonToSW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-16 22:45:56.000000 PythonToSW-1.2.1/src/PythonToSW.egg-info/top_level.txt
```

### Comparing `PythonToSW-1.2.0/LICENSE` & `PythonToSW-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/PKG-INFO` & `PythonToSW-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonToSW
-Version: 1.2.0
+Version: 1.2.1
 Summary: A package that allows you to create addons in Stormworks with Python, handled through HTTP.
 Author: Cuh4
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `PythonToSW-1.2.0/README.md` & `PythonToSW-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/setup.py` & `PythonToSW-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/__init__.py` & `PythonToSW-1.2.1/src/PythonToSW/__init__.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/addon/script.lua` & `PythonToSW-1.2.1/src/PythonToSW/addon/script.lua`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/addon.py` & `PythonToSW-1.2.1/src/PythonToSW/addon.py`

 * *Files 3% similar despite different names*

```diff
@@ -153,35 +153,27 @@
         # halt execution
         execution._halt()
         
         # remove it
         self.pendingExecutions.pop(executionID)
     
     # Register a vehicle. The path must be the path to the vehicle .xml file
-    def registerVehicle(self, path: str, isStatic: bool = False, isEditable: bool = False, isInvulnerable: bool = False, isShowOnMap: bool = False, isTransponderActive: bool = False):
+    def registerVehicle(self, path: str, vehicleID: int, isStatic: bool = False, isEditable: bool = False, isInvulnerable: bool = False, isShowOnMap: bool = False, isTransponderActive: bool = False):
         # check if path exists
         if not os.path.exists(path):
             raise exceptions.InvalidVehiclePath(f"Invalid vehicle path: {path}")
         
         # validate playlist structure (this is awful)
         root = self.playlistEncoded["playlist"]["locations"]["locations"]["l"]
         
         if root["components"].get("components", None) is None and root["components"].get("c", None) is None:
             root["components"] = {"c" : []}
-            
-        # get vehicle id
-        vehicleID = os.path.basename(path).replace("vehicle_", "").replace(".xml", "")
-        
-        if not vehicleID.isnumeric():
-            raise exceptions.InvalidVehiclePath(f"Invalid vehicle path (can't get ID?): {path}")
-        
-        vehicleID = int(vehicleID)
         
         # register vehicle
-        self.vehicles.append(path)
+        self.vehicles.append({"path" : path, "vehicleID" : vehicleID})
         
         # add vehicle to playlist
         vehicle = {
             "@component_type": "3",
             "@id": f"{vehicleID}",
             "@name": "Vehicle",
             "@dynamic_object_type": "2",
@@ -380,13 +372,13 @@
         secureAddonName = werkzeug.utils.secure_filename(self.addonName)
         destinationPath = os.path.join(self.destinationAddonPath, secureAddonName)
         
         # write files to destination
         helpers.quickWrite(os.path.join(destinationPath, "playlist.xml"), helpers.XMLEncode(self.playlistEncoded))
         helpers.quickWrite(os.path.join(destinationPath, "script.lua"), self.script)
         
-        # save vehicles
+        # add vehicles to addon directory
         for vehicle in self.vehicles:
-            name = os.path.basename(vehicle)
-            content = helpers.quickRead(vehicle)
+            vehicleID = vehicle["vehicleID"]
+            content = helpers.quickRead(vehicle["path"])
             
-            helpers.quickWrite(os.path.join(destinationPath, name), content)
+            helpers.quickWrite(os.path.join(destinationPath, f"vehicle_{vehicleID}"), content)
```

### Comparing `PythonToSW-1.2.0/src/PythonToSW/event.py` & `PythonToSW-1.2.1/src/PythonToSW/event.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/exceptions.py` & `PythonToSW-1.2.1/src/PythonToSW/exceptions.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/__createExecution.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/__createExecution.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/__generateImportCode.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/__generateImportCode.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/__init__.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/__init__.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/addAdmin.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/addAdmin.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/addAuth.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/addAuth.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/addMapLabel.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/addMapLabel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/addMapLine.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/addMapLine.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/addMapObject.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/addMapObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/announce.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/announce.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/cancelGerstner.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/cancelGerstner.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/clearOilSpills.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/clearOilSpills.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/clearRadiation.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/clearRadiation.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/clearVehicles.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/clearVehicles.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/despawnObject.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/despawnObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/despawnVehicle.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/despawnVehicle.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/despawnVehicleGroup.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/despawnVehicleGroup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/getAddonIndex.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/getAddonIndex.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/getCharacterItem.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/getCharacterItem.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/getCurrency.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/getCurrency.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/getGameSettings.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/getGameSettings.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/getObjectData.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/getObjectData.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/getPlayerCharacter.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/getPlayerCharacter.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/getPlayerLookDirection.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/getPlayerLookDirection.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/getPlayerName.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/getPlayerName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/getPlayerPos.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/getPlayerPos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/getPlayers.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/getPlayers.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/getSeasonalEvent.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/getSeasonalEvent.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/getUniqueID.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/getUniqueID.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleBatteryByName.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/getVehicleBatteryByName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleBatteryByVoxel.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/getVehicleBatteryByVoxel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleComponents.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/getVehicleComponents.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleData.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/getVehicleData.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleGroup.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/getVehicleGroup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/getVehiclePos.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/getVehiclePos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleTankByName.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/getVehicleTankByName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleTankByVoxel.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/getVehicleTankByVoxel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/isAridDLC.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/isAridDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/isSpaceDLC.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/isSpaceDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/isWeaponsDLC.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/isWeaponsDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/moveGroup.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/moveGroup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/moveGroupSafe.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/moveGroupSafe.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/moveVehicle.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/moveVehicle.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/moveVehicleSafe.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/moveVehicleSafe.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/notify.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/notify.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/removeAdmin.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/removeAdmin.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/removeAuth.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/removeAuth.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/removeMapLabel.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/removeMapLabel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/removeMapLine.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/removeMapLine.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/removeMapObject.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/removeMapObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/removePopup.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/removePopup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/setCharacterData.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/setCharacterData.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/setCharacterItem.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/setCharacterItem.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/setCharacterTooltip.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/setCharacterTooltip.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/setCreatureMoveTarget.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/setCreatureMoveTarget.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/setCurrency.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/setCurrency.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/setGameSetting.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/setGameSetting.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/setGroupPosSafe.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/setGroupPosSafe.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/setOilSpill.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/setOilSpill.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/setPlayerPos.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/setPlayerPos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/setPopup.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/setPopup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleBatteryByName.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/setVehicleBatteryByName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleBatteryByVoxel.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/setVehicleBatteryByVoxel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleEditable.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/setVehicleEditable.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleInvulnerable.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/setVehicleInvulnerable.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/setVehiclePos.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/setVehiclePos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/setVehiclePosSafe.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/setVehiclePosSafe.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleShowOnMap.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/setVehicleShowOnMap.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleTankByName.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/setVehicleTankByName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleTankByVoxel.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/setVehicleTankByVoxel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/spawnAddonVehicle.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/spawnAddonVehicle.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/spawnCharacter.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/spawnCharacter.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/spawnCreature.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/spawnCreature.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/spawnEquipment.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/spawnEquipment.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/spawnExplosion.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/spawnExplosion.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/spawnMeteor.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/spawnMeteor.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/spawnMeteorShower.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/spawnMeteorShower.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/spawnObject.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/spawnObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/spawnTsunami.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/spawnTsunami.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/spawnVehicle.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/spawnVehicle.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/spawnVolcano.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/spawnVolcano.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/executions/spawnWhirlpool.py` & `PythonToSW-1.2.1/src/PythonToSW/executions/spawnWhirlpool.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/helpers.py` & `PythonToSW-1.2.1/src/PythonToSW/helpers.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW/matrix.py` & `PythonToSW-1.2.1/src/PythonToSW/matrix.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.0/src/PythonToSW.egg-info/PKG-INFO` & `PythonToSW-1.2.1/src/PythonToSW.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonToSW
-Version: 1.2.0
+Version: 1.2.1
 Summary: A package that allows you to create addons in Stormworks with Python, handled through HTTP.
 Author: Cuh4
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `PythonToSW-1.2.0/src/PythonToSW.egg-info/SOURCES.txt` & `PythonToSW-1.2.1/src/PythonToSW.egg-info/SOURCES.txt`

 * *Files identical despite different names*

