# Comparing `tmp/PythonToSW-1.2.2.tar.gz` & `tmp/PythonToSW-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonToSW-1.2.2.tar", last modified: Fri May 17 03:25:46 2024, max compression
+gzip compressed data, was "PythonToSW-1.2.3.tar", last modified: Fri May 17 07:28:54 2024, max compression
```

## Comparing `PythonToSW-1.2.2.tar` & `PythonToSW-1.2.3.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 03:25:46.811280 PythonToSW-1.2.2/
--rw-rw-rw-   0        0        0    11558 2024-01-17 15:06:42.000000 PythonToSW-1.2.2/LICENSE
--rw-rw-rw-   0        0        0       92 2024-05-15 22:14:52.000000 PythonToSW-1.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1803 2024-05-17 03:25:46.810534 PythonToSW-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1242 2024-05-16 22:19:42.000000 PythonToSW-1.2.2/README.md
--rw-rw-rw-   0        0        0        5 2024-05-17 03:24:25.000000 PythonToSW-1.2.2/VERSION
--rw-rw-rw-   0        0        0       62 2024-05-16 22:06:47.000000 PythonToSW-1.2.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 03:25:46.812027 PythonToSW-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1878 2024-05-15 22:15:23.000000 PythonToSW-1.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 03:25:46.723212 PythonToSW-1.2.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-17 03:25:46.732998 PythonToSW-1.2.2/src/PythonToSW/
--rw-rw-rw-   0        0        0     1136 2024-05-17 02:54:27.000000 PythonToSW-1.2.2/src/PythonToSW/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 03:25:46.754015 PythonToSW-1.2.2/src/PythonToSW/addon/
--rw-rw-rw-   0        0        0      315 2024-05-16 03:46:54.000000 PythonToSW-1.2.2/src/PythonToSW/addon/playlist.xml
--rw-rw-rw-   0        0        0   161117 2024-05-16 21:57:12.000000 PythonToSW-1.2.2/src/PythonToSW/addon/script.lua
--rw-rw-rw-   0        0        0    20382 2024-05-17 03:15:24.000000 PythonToSW-1.2.2/src/PythonToSW/addon.py
--rw-rw-rw-   0        0        0     3006 2024-05-17 03:19:13.000000 PythonToSW-1.2.2/src/PythonToSW/event.py
--rw-rw-rw-   0        0        0     1247 2024-05-17 03:19:53.000000 PythonToSW-1.2.2/src/PythonToSW/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-17 03:25:46.809246 PythonToSW-1.2.2/src/PythonToSW/executions/
--rw-rw-rw-   0        0        0     2809 2024-05-14 23:36:22.000000 PythonToSW-1.2.2/src/PythonToSW/executions/__createExecution.py
--rw-rw-rw-   0        0        0     1711 2024-05-14 23:24:00.000000 PythonToSW-1.2.2/src/PythonToSW/executions/__generateImportCode.py
--rw-rw-rw-   0        0        0     7282 2024-05-17 02:53:52.000000 PythonToSW-1.2.2/src/PythonToSW/executions/__init__.py
--rw-rw-rw-   0        0        0     1059 2024-05-14 16:56:13.000000 PythonToSW-1.2.2/src/PythonToSW/executions/addAdmin.py
--rw-rw-rw-   0        0        0     1056 2024-05-14 16:56:13.000000 PythonToSW-1.2.2/src/PythonToSW/executions/addAuth.py
--rw-rw-rw-   0        0        0     1216 2024-05-14 16:56:13.000000 PythonToSW-1.2.2/src/PythonToSW/executions/addMapLabel.py
--rw-rw-rw-   0        0        0     1220 2024-05-14 16:56:13.000000 PythonToSW-1.2.2/src/PythonToSW/executions/addMapLine.py
--rw-rw-rw-   0        0        0     1582 2024-05-14 16:56:13.000000 PythonToSW-1.2.2/src/PythonToSW/executions/addMapObject.py
--rw-rw-rw-   0        0        0     1107 2024-05-14 16:56:13.000000 PythonToSW-1.2.2/src/PythonToSW/executions/announce.py
--rw-rw-rw-   0        0        0     1027 2024-05-14 23:48:22.000000 PythonToSW-1.2.2/src/PythonToSW/executions/cancelGerstner.py
--rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.2.2/src/PythonToSW/executions/clearOilSpills.py
--rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.2.2/src/PythonToSW/executions/clearRadiation.py
--rw-rw-rw-   0        0        0     1025 2024-05-14 16:56:13.000000 PythonToSW-1.2.2/src/PythonToSW/executions/clearVehicles.py
--rw-rw-rw-   0        0        0     1106 2024-05-14 23:49:23.000000 PythonToSW-1.2.2/src/PythonToSW/executions/despawnObject.py
--rw-rw-rw-   0        0        0     1111 2024-05-14 23:49:25.000000 PythonToSW-1.2.2/src/PythonToSW/executions/despawnVehicle.py
--rw-rw-rw-   0        0        0     1123 2024-05-14 23:49:26.000000 PythonToSW-1.2.2/src/PythonToSW/executions/despawnVehicleGroup.py
--rw-rw-rw-   0        0        0     1025 2024-05-16 04:08:52.000000 PythonToSW-1.2.2/src/PythonToSW/executions/getAddonIndex.py
--rw-rw-rw-   0        0        0     1105 2024-05-14 18:26:42.000000 PythonToSW-1.2.2/src/PythonToSW/executions/getCharacterItem.py
--rw-rw-rw-   0        0        0     1018 2024-05-15 22:28:57.000000 PythonToSW-1.2.2/src/PythonToSW/executions/getCurrency.py
--rw-rw-rw-   0        0        0     1031 2024-05-16 22:21:02.000000 PythonToSW-1.2.2/src/PythonToSW/executions/getGameSettings.py
--rw-rw-rw-   0        0        0     1079 2024-05-14 18:24:19.000000 PythonToSW-1.2.2/src/PythonToSW/executions/getObjectData.py
--rw-rw-rw-   0        0        0     1092 2024-05-14 16:56:13.000000 PythonToSW-1.2.2/src/PythonToSW/executions/getPlayerCharacter.py
--rw-rw-rw-   0        0        0     1103 2024-05-16 00:01:47.000000 PythonToSW-1.2.2/src/PythonToSW/executions/getPlayerLookDirection.py
--rw-rw-rw-   0        0        0     1075 2024-05-16 00:01:47.000000 PythonToSW-1.2.2/src/PythonToSW/executions/getPlayerName.py
--rw-rw-rw-   0        0        0     1072 2024-05-14 16:56:13.000000 PythonToSW-1.2.2/src/PythonToSW/executions/getPlayerPos.py
--rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.2.2/src/PythonToSW/executions/getPlayers.py
--rw-rw-rw-   0        0        0     1035 2024-05-14 16:56:13.000000 PythonToSW-1.2.2/src/PythonToSW/executions/getSeasonalEvent.py
--rw-rw-rw-   0        0        0     1017 2024-05-14 16:56:13.000000 PythonToSW-1.2.2/src/PythonToSW/executions/getUniqueID.py
--rw-rw-rw-   0        0        0     1138 2024-05-14 23:44:48.000000 PythonToSW-1.2.2/src/PythonToSW/executions/getVehicleBatteryByName.py
--rw-rw-rw-   0        0        0     1172 2024-05-14 23:44:45.000000 PythonToSW-1.2.2/src/PythonToSW/executions/getVehicleBatteryByVoxel.py
--rw-rw-rw-   0        0        0     1102 2024-05-14 18:30:01.000000 PythonToSW-1.2.2/src/PythonToSW/executions/getVehicleComponents.py
--rw-rw-rw-   0        0        0     1084 2024-05-14 18:29:46.000000 PythonToSW-1.2.2/src/PythonToSW/executions/getVehicleData.py
--rw-rw-rw-   0        0        0     1083 2024-05-15 22:28:49.000000 PythonToSW-1.2.2/src/PythonToSW/executions/getVehicleGroup.py
--rw-rw-rw-   0        0        0     1162 2024-05-15 22:08:55.000000 PythonToSW-1.2.2/src/PythonToSW/executions/getVehiclePos.py
--rw-rw-rw-   0        0        0     1123 2024-05-14 23:44:59.000000 PythonToSW-1.2.2/src/PythonToSW/executions/getVehicleTankByName.py
--rw-rw-rw-   0        0        0     1163 2024-05-14 23:45:28.000000 PythonToSW-1.2.2/src/PythonToSW/executions/getVehicleTankByVoxel.py
--rw-rw-rw-   0        0        0     1012 2024-05-14 16:56:13.000000 PythonToSW-1.2.2/src/PythonToSW/executions/isAridDLC.py
--rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.2.2/src/PythonToSW/executions/isSpaceDLC.py
--rw-rw-rw-   0        0        0     1021 2024-05-14 16:56:13.000000 PythonToSW-1.2.2/src/PythonToSW/executions/isWeaponsDLC.py
--rw-rw-rw-   0        0        0     1080 2024-05-16 00:01:47.000000 PythonToSW-1.2.2/src/PythonToSW/executions/moveGroup.py
--rw-rw-rw-   0        0        0     1093 2024-05-16 00:01:47.000000 PythonToSW-1.2.2/src/PythonToSW/executions/moveGroupSafe.py
--rw-rw-rw-   0        0        0     1090 2024-05-16 00:01:47.000000 PythonToSW-1.2.2/src/PythonToSW/executions/moveVehicle.py
--rw-rw-rw-   0        0        0     1103 2024-05-16 00:02:01.000000 PythonToSW-1.2.2/src/PythonToSW/executions/moveVehicleSafe.py
--rw-rw-rw-   0        0        0     1135 2024-05-14 23:47:34.000000 PythonToSW-1.2.2/src/PythonToSW/executions/notify.py
--rw-rw-rw-   0        0        0     1068 2024-05-14 16:56:13.000000 PythonToSW-1.2.2/src/PythonToSW/executions/removeAdmin.py
--rw-rw-rw-   0        0        0     1065 2024-05-14 16:56:13.000000 PythonToSW-1.2.2/src/PythonToSW/executions/removeAuth.py
--rw-rw-rw-   0        0        0     1097 2024-05-14 16:56:13.000000 PythonToSW-1.2.2/src/PythonToSW/executions/removeMapLabel.py
--rw-rw-rw-   0        0        0     1094 2024-05-14 16:56:13.000000 PythonToSW-1.2.2/src/PythonToSW/executions/removeMapLine.py
--rw-rw-rw-   0        0        0     1100 2024-05-14 16:56:13.000000 PythonToSW-1.2.2/src/PythonToSW/executions/removeMapObject.py
--rw-rw-rw-   0        0        0     1087 2024-05-14 16:56:13.000000 PythonToSW-1.2.2/src/PythonToSW/executions/removePopup.py
--rw-rw-rw-   0        0        0     1171 2024-05-14 18:25:00.000000 PythonToSW-1.2.2/src/PythonToSW/executions/setCharacterData.py
--rw-rw-rw-   0        0        0     1222 2024-05-14 18:26:10.000000 PythonToSW-1.2.2/src/PythonToSW/executions/setCharacterItem.py
--rw-rw-rw-   0        0        0     1120 2024-05-14 18:25:27.000000 PythonToSW-1.2.2/src/PythonToSW/executions/setCharacterTooltip.py
--rw-rw-rw-   0        0        0     1115 2024-05-14 23:49:29.000000 PythonToSW-1.2.2/src/PythonToSW/executions/setCreatureMoveTarget.py
--rw-rw-rw-   0        0        0     1115 2024-05-15 22:28:48.000000 PythonToSW-1.2.2/src/PythonToSW/executions/setCurrency.py
--rw-rw-rw-   0        0        0     1120 2024-05-16 22:20:48.000000 PythonToSW-1.2.2/src/PythonToSW/executions/setGameSetting.py
--rw-rw-rw-   0        0        0     1100 2024-05-16 00:01:49.000000 PythonToSW-1.2.2/src/PythonToSW/executions/setGroupPosSafe.py
--rw-rw-rw-   0        0        0     1089 2024-05-14 16:56:13.000000 PythonToSW-1.2.2/src/PythonToSW/executions/setOilSpill.py
--rw-rw-rw-   0        0        0     1088 2024-05-14 16:56:13.000000 PythonToSW-1.2.2/src/PythonToSW/executions/setPlayerPos.py
--rw-rw-rw-   0        0        0     1299 2024-05-14 18:18:44.000000 PythonToSW-1.2.2/src/PythonToSW/executions/setPopup.py
--rw-rw-rw-   0        0        0     1161 2024-05-14 23:43:28.000000 PythonToSW-1.2.2/src/PythonToSW/executions/setVehicleBatteryByName.py
--rw-rw-rw-   0        0        0     1194 2024-05-14 23:42:27.000000 PythonToSW-1.2.2/src/PythonToSW/executions/setVehicleBatteryByVoxel.py
--rw-rw-rw-   0        0        0     1126 2024-05-14 23:39:49.000000 PythonToSW-1.2.2/src/PythonToSW/executions/setVehicleEditable.py
--rw-rw-rw-   0        0        0     1146 2024-05-14 23:39:47.000000 PythonToSW-1.2.2/src/PythonToSW/executions/setVehicleInvulnerable.py
--rw-rw-rw-   0        0        0     1097 2024-05-15 22:08:43.000000 PythonToSW-1.2.2/src/PythonToSW/executions/setVehiclePos.py
--rw-rw-rw-   0        0        0     1110 2024-05-16 00:01:47.000000 PythonToSW-1.2.2/src/PythonToSW/executions/setVehiclePosSafe.py
--rw-rw-rw-   0        0        0     1123 2024-05-14 23:39:52.000000 PythonToSW-1.2.2/src/PythonToSW/executions/setVehicleShowOnMap.py
--rw-rw-rw-   0        0        0     1146 2024-05-14 23:43:54.000000 PythonToSW-1.2.2/src/PythonToSW/executions/setVehicleTankByName.py
--rw-rw-rw-   0        0        0     1186 2024-05-14 23:44:14.000000 PythonToSW-1.2.2/src/PythonToSW/executions/setVehicleTankByVoxel.py
--rw-rw-rw-   0        0        0     1122 2024-05-16 04:03:12.000000 PythonToSW-1.2.2/src/PythonToSW/executions/spawnAddonVehicle.py
--rw-rw-rw-   0        0        0     1095 2024-05-14 23:46:38.000000 PythonToSW-1.2.2/src/PythonToSW/executions/spawnCharacter.py
--rw-rw-rw-   0        0        0     1143 2024-05-14 23:47:06.000000 PythonToSW-1.2.2/src/PythonToSW/executions/spawnCreature.py
--rw-rw-rw-   0        0        0     1157 2024-05-16 04:03:12.000000 PythonToSW-1.2.2/src/PythonToSW/executions/spawnEquipment.py
--rw-rw-rw-   0        0        0     1099 2024-05-14 23:47:30.000000 PythonToSW-1.2.2/src/PythonToSW/executions/spawnExplosion.py
--rw-rw-rw-   0        0        0     1128 2024-05-14 23:46:36.000000 PythonToSW-1.2.2/src/PythonToSW/executions/spawnMeteor.py
--rw-rw-rw-   0        0        0     1147 2024-05-14 23:45:56.000000 PythonToSW-1.2.2/src/PythonToSW/executions/spawnMeteorShower.py
--rw-rw-rw-   0        0        0     1090 2024-05-16 04:03:13.000000 PythonToSW-1.2.2/src/PythonToSW/executions/spawnObject.py
--rw-rw-rw-   0        0        0     1093 2024-05-14 23:45:58.000000 PythonToSW-1.2.2/src/PythonToSW/executions/spawnTsunami.py
--rw-rw-rw-   0        0        0     1089 2024-05-16 04:03:12.000000 PythonToSW-1.2.2/src/PythonToSW/executions/spawnVehicle.py
--rw-rw-rw-   0        0        0     1093 2024-05-14 23:45:54.000000 PythonToSW-1.2.2/src/PythonToSW/executions/spawnVolcano.py
--rw-rw-rw-   0        0        0     1099 2024-05-14 23:45:59.000000 PythonToSW-1.2.2/src/PythonToSW/executions/spawnWhirlpool.py
--rw-rw-rw-   0        0        0     2510 2024-05-17 03:22:43.000000 PythonToSW-1.2.2/src/PythonToSW/helpers.py
--rw-rw-rw-   0        0        0     2039 2024-05-17 03:24:07.000000 PythonToSW-1.2.2/src/PythonToSW/matrix.py
-drwxrwxrwx   0        0        0        0 2024-05-17 03:25:46.809775 PythonToSW-1.2.2/src/PythonToSW.egg-info/
--rw-rw-rw-   0        0        0     1803 2024-05-17 03:25:46.000000 PythonToSW-1.2.2/src/PythonToSW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4065 2024-05-17 03:25:46.000000 PythonToSW-1.2.2/src/PythonToSW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 03:25:46.000000 PythonToSW-1.2.2/src/PythonToSW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-05-17 03:25:46.000000 PythonToSW-1.2.2/src/PythonToSW.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-17 03:25:46.000000 PythonToSW-1.2.2/src/PythonToSW.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 07:28:54.471118 PythonToSW-1.2.3/
+-rw-rw-rw-   0        0        0    11558 2024-01-17 15:06:42.000000 PythonToSW-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0       92 2024-05-15 22:14:52.000000 PythonToSW-1.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1803 2024-05-17 07:28:54.470116 PythonToSW-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1242 2024-05-16 22:19:42.000000 PythonToSW-1.2.3/README.md
+-rw-rw-rw-   0        0        0        5 2024-05-17 07:25:58.000000 PythonToSW-1.2.3/VERSION
+-rw-rw-rw-   0        0        0       62 2024-05-16 22:06:47.000000 PythonToSW-1.2.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 07:28:54.471890 PythonToSW-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1878 2024-05-15 22:15:23.000000 PythonToSW-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 07:28:54.341318 PythonToSW-1.2.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 07:28:54.350144 PythonToSW-1.2.3/src/PythonToSW/
+-rw-rw-rw-   0        0        0     1136 2024-05-17 02:54:27.000000 PythonToSW-1.2.3/src/PythonToSW/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 07:28:54.385782 PythonToSW-1.2.3/src/PythonToSW/addon/
+-rw-rw-rw-   0        0        0      315 2024-05-16 03:46:54.000000 PythonToSW-1.2.3/src/PythonToSW/addon/playlist.xml
+-rw-rw-rw-   0        0        0   161117 2024-05-16 21:57:12.000000 PythonToSW-1.2.3/src/PythonToSW/addon/script.lua
+-rw-rw-rw-   0        0        0    21012 2024-05-17 07:24:53.000000 PythonToSW-1.2.3/src/PythonToSW/addon.py
+-rw-rw-rw-   0        0        0     3176 2024-05-17 07:21:16.000000 PythonToSW-1.2.3/src/PythonToSW/event.py
+-rw-rw-rw-   0        0        0     1247 2024-05-17 03:19:53.000000 PythonToSW-1.2.3/src/PythonToSW/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-17 07:28:54.468348 PythonToSW-1.2.3/src/PythonToSW/executions/
+-rw-rw-rw-   0        0        0     2809 2024-05-14 23:36:22.000000 PythonToSW-1.2.3/src/PythonToSW/executions/__createExecution.py
+-rw-rw-rw-   0        0        0     1711 2024-05-14 23:24:00.000000 PythonToSW-1.2.3/src/PythonToSW/executions/__generateImportCode.py
+-rw-rw-rw-   0        0        0     7408 2024-05-17 07:25:30.000000 PythonToSW-1.2.3/src/PythonToSW/executions/__init__.py
+-rw-rw-rw-   0        0        0     1059 2024-05-14 16:56:13.000000 PythonToSW-1.2.3/src/PythonToSW/executions/addAdmin.py
+-rw-rw-rw-   0        0        0     1056 2024-05-14 16:56:13.000000 PythonToSW-1.2.3/src/PythonToSW/executions/addAuth.py
+-rw-rw-rw-   0        0        0     1216 2024-05-14 16:56:13.000000 PythonToSW-1.2.3/src/PythonToSW/executions/addMapLabel.py
+-rw-rw-rw-   0        0        0     1220 2024-05-14 16:56:13.000000 PythonToSW-1.2.3/src/PythonToSW/executions/addMapLine.py
+-rw-rw-rw-   0        0        0     1582 2024-05-14 16:56:13.000000 PythonToSW-1.2.3/src/PythonToSW/executions/addMapObject.py
+-rw-rw-rw-   0        0        0     1107 2024-05-14 16:56:13.000000 PythonToSW-1.2.3/src/PythonToSW/executions/announce.py
+-rw-rw-rw-   0        0        0     1027 2024-05-14 23:48:22.000000 PythonToSW-1.2.3/src/PythonToSW/executions/cancelGerstner.py
+-rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.2.3/src/PythonToSW/executions/clearOilSpills.py
+-rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.2.3/src/PythonToSW/executions/clearRadiation.py
+-rw-rw-rw-   0        0        0     1025 2024-05-14 16:56:13.000000 PythonToSW-1.2.3/src/PythonToSW/executions/clearVehicles.py
+-rw-rw-rw-   0        0        0     1106 2024-05-14 23:49:23.000000 PythonToSW-1.2.3/src/PythonToSW/executions/despawnObject.py
+-rw-rw-rw-   0        0        0     1111 2024-05-14 23:49:25.000000 PythonToSW-1.2.3/src/PythonToSW/executions/despawnVehicle.py
+-rw-rw-rw-   0        0        0     1123 2024-05-14 23:49:26.000000 PythonToSW-1.2.3/src/PythonToSW/executions/despawnVehicleGroup.py
+-rw-rw-rw-   0        0        0     1025 2024-05-16 04:08:52.000000 PythonToSW-1.2.3/src/PythonToSW/executions/getAddonIndex.py
+-rw-rw-rw-   0        0        0     1105 2024-05-14 18:26:42.000000 PythonToSW-1.2.3/src/PythonToSW/executions/getCharacterItem.py
+-rw-rw-rw-   0        0        0     1018 2024-05-15 22:28:57.000000 PythonToSW-1.2.3/src/PythonToSW/executions/getCurrency.py
+-rw-rw-rw-   0        0        0     1031 2024-05-16 22:21:02.000000 PythonToSW-1.2.3/src/PythonToSW/executions/getGameSettings.py
+-rw-rw-rw-   0        0        0     1079 2024-05-14 18:24:19.000000 PythonToSW-1.2.3/src/PythonToSW/executions/getObjectData.py
+-rw-rw-rw-   0        0        0     1092 2024-05-14 16:56:13.000000 PythonToSW-1.2.3/src/PythonToSW/executions/getPlayerCharacter.py
+-rw-rw-rw-   0        0        0     1103 2024-05-16 00:01:47.000000 PythonToSW-1.2.3/src/PythonToSW/executions/getPlayerLookDirection.py
+-rw-rw-rw-   0        0        0     1075 2024-05-16 00:01:47.000000 PythonToSW-1.2.3/src/PythonToSW/executions/getPlayerName.py
+-rw-rw-rw-   0        0        0     1072 2024-05-14 16:56:13.000000 PythonToSW-1.2.3/src/PythonToSW/executions/getPlayerPos.py
+-rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.2.3/src/PythonToSW/executions/getPlayers.py
+-rw-rw-rw-   0        0        0     1035 2024-05-14 16:56:13.000000 PythonToSW-1.2.3/src/PythonToSW/executions/getSeasonalEvent.py
+-rw-rw-rw-   0        0        0     1017 2024-05-14 16:56:13.000000 PythonToSW-1.2.3/src/PythonToSW/executions/getUniqueID.py
+-rw-rw-rw-   0        0        0     1138 2024-05-14 23:44:48.000000 PythonToSW-1.2.3/src/PythonToSW/executions/getVehicleBatteryByName.py
+-rw-rw-rw-   0        0        0     1172 2024-05-14 23:44:45.000000 PythonToSW-1.2.3/src/PythonToSW/executions/getVehicleBatteryByVoxel.py
+-rw-rw-rw-   0        0        0     1102 2024-05-14 18:30:01.000000 PythonToSW-1.2.3/src/PythonToSW/executions/getVehicleComponents.py
+-rw-rw-rw-   0        0        0     1084 2024-05-14 18:29:46.000000 PythonToSW-1.2.3/src/PythonToSW/executions/getVehicleData.py
+-rw-rw-rw-   0        0        0     1083 2024-05-15 22:28:49.000000 PythonToSW-1.2.3/src/PythonToSW/executions/getVehicleGroup.py
+-rw-rw-rw-   0        0        0     1162 2024-05-15 22:08:55.000000 PythonToSW-1.2.3/src/PythonToSW/executions/getVehiclePos.py
+-rw-rw-rw-   0        0        0     1123 2024-05-14 23:44:59.000000 PythonToSW-1.2.3/src/PythonToSW/executions/getVehicleTankByName.py
+-rw-rw-rw-   0        0        0     1163 2024-05-14 23:45:28.000000 PythonToSW-1.2.3/src/PythonToSW/executions/getVehicleTankByVoxel.py
+-rw-rw-rw-   0        0        0     1012 2024-05-14 16:56:13.000000 PythonToSW-1.2.3/src/PythonToSW/executions/isAridDLC.py
+-rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.2.3/src/PythonToSW/executions/isSpaceDLC.py
+-rw-rw-rw-   0        0        0     1021 2024-05-14 16:56:13.000000 PythonToSW-1.2.3/src/PythonToSW/executions/isWeaponsDLC.py
+-rw-rw-rw-   0        0        0     1080 2024-05-16 00:01:47.000000 PythonToSW-1.2.3/src/PythonToSW/executions/moveGroup.py
+-rw-rw-rw-   0        0        0     1093 2024-05-16 00:01:47.000000 PythonToSW-1.2.3/src/PythonToSW/executions/moveGroupSafe.py
+-rw-rw-rw-   0        0        0     1090 2024-05-16 00:01:47.000000 PythonToSW-1.2.3/src/PythonToSW/executions/moveVehicle.py
+-rw-rw-rw-   0        0        0     1103 2024-05-16 00:02:01.000000 PythonToSW-1.2.3/src/PythonToSW/executions/moveVehicleSafe.py
+-rw-rw-rw-   0        0        0     1135 2024-05-14 23:47:34.000000 PythonToSW-1.2.3/src/PythonToSW/executions/notify.py
+-rw-rw-rw-   0        0        0     1068 2024-05-14 16:56:13.000000 PythonToSW-1.2.3/src/PythonToSW/executions/removeAdmin.py
+-rw-rw-rw-   0        0        0     1065 2024-05-14 16:56:13.000000 PythonToSW-1.2.3/src/PythonToSW/executions/removeAuth.py
+-rw-rw-rw-   0        0        0     1097 2024-05-14 16:56:13.000000 PythonToSW-1.2.3/src/PythonToSW/executions/removeMapLabel.py
+-rw-rw-rw-   0        0        0     1094 2024-05-14 16:56:13.000000 PythonToSW-1.2.3/src/PythonToSW/executions/removeMapLine.py
+-rw-rw-rw-   0        0        0     1100 2024-05-14 16:56:13.000000 PythonToSW-1.2.3/src/PythonToSW/executions/removeMapObject.py
+-rw-rw-rw-   0        0        0     1087 2024-05-14 16:56:13.000000 PythonToSW-1.2.3/src/PythonToSW/executions/removePopup.py
+-rw-rw-rw-   0        0        0     1171 2024-05-14 18:25:00.000000 PythonToSW-1.2.3/src/PythonToSW/executions/setCharacterData.py
+-rw-rw-rw-   0        0        0     1222 2024-05-14 18:26:10.000000 PythonToSW-1.2.3/src/PythonToSW/executions/setCharacterItem.py
+-rw-rw-rw-   0        0        0     1120 2024-05-14 18:25:27.000000 PythonToSW-1.2.3/src/PythonToSW/executions/setCharacterTooltip.py
+-rw-rw-rw-   0        0        0     1115 2024-05-14 23:49:29.000000 PythonToSW-1.2.3/src/PythonToSW/executions/setCreatureMoveTarget.py
+-rw-rw-rw-   0        0        0     1115 2024-05-15 22:28:48.000000 PythonToSW-1.2.3/src/PythonToSW/executions/setCurrency.py
+-rw-rw-rw-   0        0        0     1120 2024-05-16 22:20:48.000000 PythonToSW-1.2.3/src/PythonToSW/executions/setGameSetting.py
+-rw-rw-rw-   0        0        0     1100 2024-05-16 00:01:49.000000 PythonToSW-1.2.3/src/PythonToSW/executions/setGroupPosSafe.py
+-rw-rw-rw-   0        0        0     1089 2024-05-14 16:56:13.000000 PythonToSW-1.2.3/src/PythonToSW/executions/setOilSpill.py
+-rw-rw-rw-   0        0        0     1088 2024-05-14 16:56:13.000000 PythonToSW-1.2.3/src/PythonToSW/executions/setPlayerPos.py
+-rw-rw-rw-   0        0        0     1299 2024-05-14 18:18:44.000000 PythonToSW-1.2.3/src/PythonToSW/executions/setPopup.py
+-rw-rw-rw-   0        0        0     1161 2024-05-14 23:43:28.000000 PythonToSW-1.2.3/src/PythonToSW/executions/setVehicleBatteryByName.py
+-rw-rw-rw-   0        0        0     1194 2024-05-14 23:42:27.000000 PythonToSW-1.2.3/src/PythonToSW/executions/setVehicleBatteryByVoxel.py
+-rw-rw-rw-   0        0        0     1126 2024-05-14 23:39:49.000000 PythonToSW-1.2.3/src/PythonToSW/executions/setVehicleEditable.py
+-rw-rw-rw-   0        0        0     1146 2024-05-14 23:39:47.000000 PythonToSW-1.2.3/src/PythonToSW/executions/setVehicleInvulnerable.py
+-rw-rw-rw-   0        0        0     1097 2024-05-15 22:08:43.000000 PythonToSW-1.2.3/src/PythonToSW/executions/setVehiclePos.py
+-rw-rw-rw-   0        0        0     1110 2024-05-16 00:01:47.000000 PythonToSW-1.2.3/src/PythonToSW/executions/setVehiclePosSafe.py
+-rw-rw-rw-   0        0        0     1123 2024-05-14 23:39:52.000000 PythonToSW-1.2.3/src/PythonToSW/executions/setVehicleShowOnMap.py
+-rw-rw-rw-   0        0        0     1146 2024-05-14 23:43:54.000000 PythonToSW-1.2.3/src/PythonToSW/executions/setVehicleTankByName.py
+-rw-rw-rw-   0        0        0     1186 2024-05-14 23:44:14.000000 PythonToSW-1.2.3/src/PythonToSW/executions/setVehicleTankByVoxel.py
+-rw-rw-rw-   0        0        0     1122 2024-05-16 04:03:12.000000 PythonToSW-1.2.3/src/PythonToSW/executions/spawnAddonVehicle.py
+-rw-rw-rw-   0        0        0     1095 2024-05-14 23:46:38.000000 PythonToSW-1.2.3/src/PythonToSW/executions/spawnCharacter.py
+-rw-rw-rw-   0        0        0     1143 2024-05-14 23:47:06.000000 PythonToSW-1.2.3/src/PythonToSW/executions/spawnCreature.py
+-rw-rw-rw-   0        0        0     1157 2024-05-16 04:03:12.000000 PythonToSW-1.2.3/src/PythonToSW/executions/spawnEquipment.py
+-rw-rw-rw-   0        0        0     1099 2024-05-14 23:47:30.000000 PythonToSW-1.2.3/src/PythonToSW/executions/spawnExplosion.py
+-rw-rw-rw-   0        0        0     1128 2024-05-14 23:46:36.000000 PythonToSW-1.2.3/src/PythonToSW/executions/spawnMeteor.py
+-rw-rw-rw-   0        0        0     1147 2024-05-14 23:45:56.000000 PythonToSW-1.2.3/src/PythonToSW/executions/spawnMeteorShower.py
+-rw-rw-rw-   0        0        0     1090 2024-05-16 04:03:13.000000 PythonToSW-1.2.3/src/PythonToSW/executions/spawnObject.py
+-rw-rw-rw-   0        0        0     1093 2024-05-14 23:45:58.000000 PythonToSW-1.2.3/src/PythonToSW/executions/spawnTsunami.py
+-rw-rw-rw-   0        0        0     1089 2024-05-16 04:03:12.000000 PythonToSW-1.2.3/src/PythonToSW/executions/spawnVehicle.py
+-rw-rw-rw-   0        0        0     1093 2024-05-14 23:45:54.000000 PythonToSW-1.2.3/src/PythonToSW/executions/spawnVolcano.py
+-rw-rw-rw-   0        0        0     1099 2024-05-14 23:45:59.000000 PythonToSW-1.2.3/src/PythonToSW/executions/spawnWhirlpool.py
+-rw-rw-rw-   0        0        0     2688 2024-05-17 07:20:38.000000 PythonToSW-1.2.3/src/PythonToSW/helpers.py
+-rw-rw-rw-   0        0        0     2157 2024-05-17 07:25:51.000000 PythonToSW-1.2.3/src/PythonToSW/matrix.py
+drwxrwxrwx   0        0        0        0 2024-05-17 07:28:54.469350 PythonToSW-1.2.3/src/PythonToSW.egg-info/
+-rw-rw-rw-   0        0        0     1803 2024-05-17 07:28:54.000000 PythonToSW-1.2.3/src/PythonToSW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4065 2024-05-17 07:28:54.000000 PythonToSW-1.2.3/src/PythonToSW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 07:28:54.000000 PythonToSW-1.2.3/src/PythonToSW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-17 07:28:54.000000 PythonToSW-1.2.3/src/PythonToSW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-17 07:28:54.000000 PythonToSW-1.2.3/src/PythonToSW.egg-info/top_level.txt
```

### Comparing `PythonToSW-1.2.2/LICENSE` & `PythonToSW-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/PKG-INFO` & `PythonToSW-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonToSW
-Version: 1.2.2
+Version: 1.2.3
 Summary: A package that allows you to create addons in Stormworks with Python, handled through HTTP.
 Author: Cuh4
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `PythonToSW-1.2.2/README.md` & `PythonToSW-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/setup.py` & `PythonToSW-1.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/__init__.py` & `PythonToSW-1.2.3/src/PythonToSW/__init__.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/addon/script.lua` & `PythonToSW-1.2.3/src/PythonToSW/addon/script.lua`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/addon.py` & `PythonToSW-1.2.3/src/PythonToSW/addon.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,28 +61,29 @@
         allowLogging: (bool = True: Whether to allow logging.
         destinationAddonPath: (str = None) The destination path for the addon. You will need to provide this if you are on a non-Windows OS. Defaults to %APPDATA%\Stormworks\data\missions.
         
     Raises:
         exceptions.InternalError: Raised if the PythonToSW base addon doesn't exist.
         exceptions.PathNotFound: Raised if the destination addon path does not exist. If this is raised, you likely haven't installed and ran Stormworks. If you have, you will need to manually set the destinationAddonPath argument.
     """
+
     def __init__(self, addonName: str, port: int, *, allowLogging: bool = True, destinationAddonPath: str = os.path.join(os.getenv("APPDATA"), "Stormworks", "data", "missions")):
         # main attributes
         self.addonName = addonName
         self.port = port
         self.app = flask.Flask(__name__)
         self.running = False
         self.allowLogging = allowLogging
         self.addonPath = os.path.join(os.path.dirname(__file__), "addon")
         self.destinationAddonPath = destinationAddonPath
         self.pendingExecutions: dict[str, executions.BaseExecution] = {}
         self.callbacks: dict[str, Event] = {}
         
-        self.playlistEncoded = self.__parsePlaylist()
-        self.script = self.__parseScript()
+        self.playlistEncoded = self._parsePlaylist()
+        self.script = self._parseScript()
         self.vehicles: list[str] = []
         
         # check if paths exist
         if not os.path.exists(self.addonPath):
             raise exceptions.InternalError(f"Addon path does not exist: {os.path.abspath(self.addonPath)}")
         
         if not os.path.exists(self.destinationAddonPath):
@@ -91,84 +92,87 @@
         # edit playlist
         self.playlistEncoded["playlist"]["@name"] = f"[P2SW] {self.addonName}"
         self.playlistEncoded["playlist"]["@folder_path"] = f"data/missions/{self.addonName}"
         
         # edit script
         self.script = self.script.replace("__PORT__", str(self.port))
         
-    """
-    Sends a message to the terminal. It's just a fancy print()
-    
-    Args:
-        message: (str) The message to send.
-    """
     def log(self, message: str):
+        """
+        Sends a message to the terminal. It's just a fancy print()
+        
+        Args:
+            message: (str) The message to send.
+        """
+
         if not self.allowLogging:
             return
         
         print(f"{colorama.Fore.BLUE}{colorama.Style.BRIGHT}[PythonToSW - {datetime.now()}]{colorama.Style.RESET_ALL}{colorama.Fore.RESET} {message}")
         
-    """
-    Starts the addon, automatically creating needed files, as well as hosting a HTTP server locally.
-    
-    >>> import PythonToSW as PTS
-    >>> addon = PTS.Addon("MyAddon", port = 3000)
-    >>>
-    >>> def main():
-    >>>     addon.execute(PTS.Announce("Server", "Hello World", -1))
-    >>>
-    >>> addon.start(target = main) # Start the addon. This automatically creates an addon and places it in your Stormworks' addon directory, so you can easily use the addon in a save.
-    
-    Args:
-        target: (function) The function to start the addon with.
-        
-    Raises:
-        exceptions.FailedStartAttempt: Raised if the addon is already running.
-    """
     def start(self, target: "function"):
+        """
+        Starts the addon, automatically creating needed files, as well as hosting a HTTP server locally.
+        
+        >>> import PythonToSW as PTS
+        >>> addon = PTS.Addon("MyAddon", port = 3000)
+        >>>
+        >>> def main():
+        >>>     addon.execute(PTS.Announce("Server", "Hello World", -1))
+        >>>
+        >>> addon.start(target = main) # Start the addon. This automatically creates an addon and places it in your Stormworks' addon directory, so you can easily use the addon in a save.
+        
+        Args:
+            target: (function) The function to start the addon with.
+            
+        Raises:
+            exceptions.FailedStartAttempt: Raised if the addon is already running.
+        """
+
         if self.running:
             raise exceptions.FailedStartAttempt("Addon is already running")
         
         # set running
         self.running = True
         
         # setup addon
-        self.__setupAddon()
+        self._setupAddon()
         
         # setup routes
-        self.__setupRoutes()
+        self._setupRoutes()
         
         # hide flask output
-        self.__hideFlaskOutput()
+        self._hideFlaskOutput()
         
         # send startup message
         self.log(f"{self.addonName} (addon) has started, listening on port {self.port}. Create a save with your addon enabled in Stormworks and keep this running.")
         
         # start server
         threading.Thread(target = target).start()
         self.app.run(host = "127.0.0.1", port = self.port, threaded = True)
         
-    """
-    Sends an execution to the in-game addon.
-    
-    >>> import PythonToSW as PTS
-    >>> addon = PTS.Addon("MyAddon", port = 3000)
-    >>>
-    >>> def main():
-    >>>     addon.execute(PTS.Announce("Server", "Hello World", -1)) # Sends a message to everyone
-    >>>
-    >>> addon.start(target = main)
-    
-    Args:
-        execution: (executions.BaseExecution) The execution to send.
-        
-    Raises:
-        exceptions.FailedExecutionAttempt: Raised if the addon is not running, or if an execution with the same ID already exists.
-    """
     def execute(self, execution: executions.BaseExecution):
+        """
+        Sends an execution to the in-game addon.
+        
+        >>> import PythonToSW as PTS
+        >>> addon = PTS.Addon("MyAddon", port = 3000)
+        >>>
+        >>> def main():
+        >>>     addon.execute(PTS.Announce("Server", "Hello World", -1)) # Sends a message to everyone
+        >>>
+        >>> addon.start(target = main)
+        
+        Args:
+            execution: (executions.BaseExecution) The execution to send.
+            
+        Raises:
+            exceptions.FailedExecutionAttempt: Raised if the addon is not running, or if an execution with the same ID already exists.
+        """
+
         # check if addon is running
         if not self.running:
             raise exceptions.FailedExecutionAttempt("Attempted to execute server function when addon is not running")
         
         # check if execution already exists
         if self.getPendingExecution(execution.ID):
             raise exceptions.FailedExecutionAttempt(f"Attempted to execute server function with duplicate ID: {execution.ID}")
@@ -186,46 +190,49 @@
         
         # remove execution now that its complete
         self.removePendingExecution(execution.ID)
         
         # return
         return returnValues
     
-    """
-    Returns the pending execution with the given ID.
-    
-    Args:
-        executionID: (str) The ID of the execution to return.
-        
-    Returns:
-        (executions.BaseExecution|None) The pending execution with the given ID, or None if it doesn't exist.
-    """
     def getPendingExecution(self, executionID: str) -> executions.BaseExecution|None:
+        """
+        Returns the pending execution with the given ID.
+        
+        Args:
+            executionID: (str) The ID of the execution to return.
+            
+        Returns:
+            (executions.BaseExecution|None) The pending execution with the given ID, or None if it doesn't exist.
+        """
+
         return self.getPendingExecutions().get(executionID)
         
-    """
-    Returns the pending executions.
-    
-    Returns:
-        (dict[str, executions.BaseExecution]) The pending executions, with the keys being the execution IDs.
-    """
     def getPendingExecutions(self) -> dict[str, executions.BaseExecution]:
+        """
+        Returns the pending executions.
+        
+        Returns:
+            (dict[str, executions.BaseExecution]) The pending executions, with the keys being the execution IDs.
+        """
+
         return self.pendingExecutions.copy()
     
-    """
-    Removes the pending execution with the given ID.
-    
-    Args:
-        executionID: (str) The ID of the execution to remove.
-        
-    Raises:
-        exceptions.FailedExecutionAttempt: Raised if the execution with the given ID doesn't exist.
-        exceptions.ExecutionNotFound: Raised if no execution with the given ID exists.
-    """
     def removePendingExecution(self, executionID: str):
+        """
+        Removes the pending execution with the given ID.
+        
+        Args:
+            executionID: (str) The ID of the execution to remove.
+            
+        Raises:
+            exceptions.FailedExecutionAttempt: Raised if the execution with the given ID doesn't exist.
+            exceptions.ExecutionNotFound: Raised if no execution with the given ID exists.
+        """
+
         # check if addon is running
         if not self.running:
             raise exceptions.FailedExecutionAttempt("Attempted to remove pending execution when addon is not running")
         
         # get the execution
         execution = self.getPendingExecution(executionID)
         
@@ -234,30 +241,31 @@
         
         # halt execution
         execution._halt()
         
         # remove it
         self.pendingExecutions.pop(executionID)
     
-    """
-    Registers a vehicle with the addon.
-    
-    Args:
-        path: (str) The path to the vehicle file.
-        vehicleID: (int) The ID of the vehicle.
-        isStatic: (bool = False) Whether the vehicle is static.
-        isEditable: (bool = False) Whether the vehicle is editable.
-        isInvulnerable: (bool = False) Whether the vehicle is invulnerable.
-        isShowOnMap: (bool = False) Whether the vehicle is shown on the map.
-        isTransponderActive: (bool = False) Whether the vehicle's transponder is active.
-        
-    Raises:
-        exceptions.InvalidVehiclePath: Raised if the path to the vehicle file is invalid (doesn't exist, isn't a file, or isn't an XML file).
-    """
     def registerVehicle(self, path: str, vehicleID: int, isStatic: bool = False, isEditable: bool = False, isInvulnerable: bool = False, isShowOnMap: bool = False, isTransponderActive: bool = False):
+        """
+        Registers a vehicle with the addon.
+        
+        Args:
+            path: (str) The path to the vehicle file.
+            vehicleID: (int) The ID of the vehicle.
+            isStatic: (bool = False) Whether the vehicle is static.
+            isEditable: (bool = False) Whether the vehicle is editable.
+            isInvulnerable: (bool = False) Whether the vehicle is invulnerable.
+            isShowOnMap: (bool = False) Whether the vehicle is shown on the map.
+            isTransponderActive: (bool = False) Whether the vehicle's transponder is active.
+            
+        Raises:
+            exceptions.InvalidVehiclePath: Raised if the path to the vehicle file is invalid (doesn't exist, isn't a file, or isn't an XML file).
+        """
+
         # check if path exists and is valid
         if not os.path.exists(path):
             raise exceptions.InvalidVehiclePath(f"Invalid vehicle path: {path}")
         
         if not os.path.isfile(path):
             raise exceptions.InvalidVehiclePath(f"Invalid vehicle path: {path} is not a file")
         
@@ -324,85 +332,90 @@
             vehicle["@vehicle_is_transponder_active"] = "true"
 
         root["components"]["c"].append(vehicle)
         
         # send log
         self.log(f"Registered vehicle #{vehicleID}.")
         
-    """
-    Listens for a game callback.
-    
-    >>> import PythonToSW as PTS
-    >>> addon = PTS.Addon("MyAddon", port = 3000)
-    >>>
-    >>> def main():
-    >>>     def onTick(game_ticks):
-    >>>         PTS.Announce("Server", "Tick", -1)
-    >>>
-    >>>     addon.listen("onTick", onTick)
-    >>>
-    >>> addon.start(target = main)
-    
-    Args:
-        name: (str) The name of the callback.
-        callback: (function) The callback to listen for.
-        
-    Returns:
-        (Event) The event that was created.
-    """
     def listen(self, name: str, callback: "function") -> Event:
+        """
+        Listens for a game callback.
+        
+        >>> import PythonToSW as PTS
+        >>> addon = PTS.Addon("MyAddon", port = 3000)
+        >>>
+        >>> def main():
+        >>>     def onTick(game_ticks):
+        >>>         PTS.Announce("Server", "Tick", -1)
+        >>>
+        >>>     addon.listen("onTick", onTick)
+        >>>
+        >>> addon.start(target = main)
+        
+        Args:
+            name: (str) The name of the callback.
+            callback: (function) The callback to listen for.
+            
+        Returns:
+            (Event) The event that was created.
+        """
+
         # send log
         self.log(f"{callback.__name__} is listening for callback: {name}")
         
         # create if not exists
-        self.__createCallbackIfNotExists(name)
+        self._createCallbackIfNotExists(name)
         event = self.getCallback(name)
 
         # connect
         event.connect(callback)
         return event
         
-    """
-    Get a callback by its name.
-    
-    Args:
-        name: (str) The name of the callback.
-        
-    Returns:
-        (Event|None) The event representing the callback, or None if it doesn't exist.
-    """
     def getCallback(self, name: str) -> Event|None:
+        """
+        Get a callback by its name.
+        
+        Args:
+            name: (str) The name of the callback.
+            
+        Returns:
+            (Event|None) The event representing the callback, or None if it doesn't exist.
+        """
+
         return self.getCallbacks().get(name)
     
-    """
-    Get all callbacks.
-    
-    Returns:
-        (dict[str, Event]) A dictionary of events representing callbacks.
-    """
     def getCallbacks(self) -> dict[str, Event]:
+        """
+        Get all callbacks.
+        
+        Returns:
+            (dict[str, Event]) A dictionary of events representing callbacks.
+        """
+
         return self.callbacks.copy()
     
-    """
-    Create a callback if it doesn't exist.
-    
-    Args:
-        name: (str) The name of the callback.
-    """
-    def __createCallbackIfNotExists(self, name: str):
+    def _createCallbackIfNotExists(self, name: str):
+        """
+        Create a callback if it doesn't exist.
+        
+        Args:
+            name: (str) The name of the callback.
+        """
+
         if not self.getCallback(name):
             self.callbacks[name] = Event()
         
-    """
-    Sets up API routes for this addon's HTTP server.
-    
-    Raises:
-        (exceptions.InternalError) Raised if the addon is not running.
-    """
-    def __setupRoutes(self):
+    def _setupRoutes(self):
+        """
+        Sets up API routes for this addon's HTTP server.
+        
+        Raises:
+            (exceptions.InternalError) Raised if the addon is not running.
+        """
+
         # check if addon is running
         if not self.running:
             raise exceptions.InternalError("Attempted to setup routes when addon is not running")
         
         # route - raise error from addon
         @self.app.get("/error")
         def error():
@@ -483,60 +496,64 @@
             
             # trigger
             callback.fire(*args)
             
             # return
             return "Ok", 200
         
-    """
-    Hides Werkzeug and Flask logging. This is used to hide the Flask server banner and request logs.
-    """
-    def __hideFlaskOutput(self):
+    def _hideFlaskOutput(self):
+        """
+        Hides Werkzeug and Flask logging. This is used to hide the Flask server banner and request logs.
+        """
+
         logging.getLogger("werkzeug").disabled = True
         self.app.logger.disabled = True
         flask.cli.show_server_banner = lambda *_, **__: None
         
-    """
-    Parses (XML decoded) the addon's playlist.xml file.
-    
-    Returns:
-        (dict) The XML decoded playlist.
-        
-    Raises:
-        (exceptions.PathNotFound) Raised if the playlist file does not exist.
-    """
-    def __parsePlaylist(self):
+    def _parsePlaylist(self):
+        """
+        Parses (XML decodes) the addon's playlist.xml file.
+        
+        Returns:
+            (dict) The XML decoded playlist.
+            
+        Raises:
+            (exceptions.PathNotFound) Raised if the playlist file does not exist.
+        """
+
         playlistFile = os.path.join(self.addonPath, "playlist.xml")
         
         if not os.path.exists(playlistFile):
             raise exceptions.PathNotFound(f"Playlist file does not exist: {playlistFile}")
         
         return helpers.XMLDecode(helpers.quickRead(playlistFile))
     
-    """
-    Parses the addon's script.lua file.
-    
-    Returns:
-        (str) The script contents.
-        
-    Raises:
-        (exceptions.PathNotFound) Raised if the script file does not exist.
-    """
-    def __parseScript(self):
+    def _parseScript(self):
+        """
+        Parses the addon's script.lua file.
+        
+        Returns:
+            (str) The script contents.
+            
+        Raises:
+            (exceptions.PathNotFound) Raised if the script file does not exist.
+        """
+
         scriptFile = os.path.join(self.addonPath, "script.lua")
         
         if not os.path.exists(scriptFile):
             raise exceptions.PathNotFound(f"Script file does not exist: {scriptFile}")
         
         return helpers.quickRead(scriptFile)
         
-    """
-    Sets up the addon by writing the playlist and script files to the destination path, as well as setting up vehicles, etc.
-    """
-    def __setupAddon(self):
+    def _setupAddon(self):
+        """
+        Sets up the addon by writing the playlist and script files to the destination path, as well as setting up vehicles, etc.
+        """
+
         # set destination path
         secureAddonName = werkzeug.utils.secure_filename(self.addonName)
         destinationPath = os.path.join(self.destinationAddonPath, secureAddonName)
         
         # write files to destination
         helpers.quickWrite(os.path.join(destinationPath, "playlist.xml"), helpers.XMLEncode(self.playlistEncoded))
         helpers.quickWrite(os.path.join(destinationPath, "script.lua"), self.script)
```

### Comparing `PythonToSW-1.2.2/src/PythonToSW/event.py` & `PythonToSW-1.2.3/src/PythonToSW/event.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,71 +32,78 @@
     A class that allows you to pack functions together and call them all at once in different threads.
     
     >>> event = Event()
     >>> event.connect(lambda: print("Hello, world!"))
     >>>
     >>> event.fire()
     """
+
     def __init__(self):
         self.callbacks: list["function"] = []
     
-    """
-    Register a callback to this event.
-    
-    Args:
-        callback: (function) The callback to register.
-    """
     def connect(self, callback: "function"):
-        self.callbacks.append(callback)
+        """
+        Register a callback to this event.
         
-    """
-    Unregister a callback from this event.
-    
-    Args:
-        callback: (function) The callback to unregister.
+        Args:
+            callback: (function) The callback to register.
+        """
+
+        self.callbacks.append(callback)
         
-    Raises:
-        ValueError: Raised if the callback is not connected to this event.
-    """
     def disconnect(self, callback: "function"):
+        """
+        Unregister a callback from this event.
+        
+        Args:
+            callback: (function) The callback to unregister.
+            
+        Raises:
+            ValueError: Raised if the callback is not connected to this event.
+        """
+
         self.callbacks.remove(callback)
         
-    """
-    Unregister all callbacks from this event.
-    """
     def disconnectAll(self):
+        """
+        Unregister all callbacks from this event.
+        """
+
         self.callbacks = []
         
-    """
-    Return all callbacks connected to this event.
-    
-    Returns:
-        list[function]: The callbacks connected to this event.
-    """
     def getCallbacks(self):
+        """
+        Return all callbacks connected to this event.
+        
+        Returns:
+            list[function]: The callbacks connected to this event.
+        """
+
         return self.callbacks.copy()
 
-    """
-    Fire all callbacks connected to this event.
-    
-    Args:
-        *args: (list) The arguments to pass to the callbacks.
-        **kwargs: (dict) The keyword arguments to pass to the callbacks.
-    """
     def fire(self, *args, **kwargs):
+        """
+        Fire all callbacks connected to this event.
+        
+        Args:
+            *args: (list) The arguments to pass to the callbacks.
+            **kwargs: (dict) The keyword arguments to pass to the callbacks.
+        """
+
         for callback in self.getCallbacks():
             self._call(callback, *args, **kwargs)
             
-    """
-    Call a function in a new thread.
-    
-    Args:
-        func: (function) The function to call.
-        *args: (list) The arguments to pass to the function.
-        **kwargs: (dict) The keyword arguments to pass to the function.
-    """
     def _call(self, func: "function", *args, **kwargs):
+        """
+        Call a function in a new thread.
+        
+        Args:
+            func: (function) The function to call.
+            *args: (list) The arguments to pass to the function.
+            **kwargs: (dict) The keyword arguments to pass to the function.
+        """
+
         threading.Thread(
             target = func,
             args = args,
             kwargs = kwargs
         ).start()
```

### Comparing `PythonToSW-1.2.2/src/PythonToSW/exceptions.py` & `PythonToSW-1.2.3/src/PythonToSW/exceptions.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/__createExecution.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/__createExecution.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/__generateImportCode.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/__generateImportCode.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/__init__.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,83 +41,88 @@
     >>> class MoveGroup(BaseExecution):
     >>>     def __init__(self, group_id: int, pos: list):
     >>>         super().__init__(
     >>>             functionName = "moveGroup",
     >>>             arguments = [group_id, pos]
     >>>         )
     
-    
     Args:
         functionName: (str) The name of the in-game function to call
         arguments: (list) The arguments to pass to the in-game function
     """
+
     def __init__(self, functionName: str, arguments: list = []):
         self.ID = str(uuid4())
         self.functionName = functionName
         self.arguments = arguments
         
         self.handled = False
         self.returnValues = []
         self.isWaiting = False
         
     def __str__(self):
         return f"Execution-{self.ID} ({self.functionName})"
         
-    """
-    Converts this execution into a dictionary that can be sent to the addon
-    
-    Returns:
-        (dict) The dictionary representation of this execution
-    """
     def _toDict(self):
+        """
+        Converts this execution into a dictionary that can be sent to the addon
+        
+        Returns:
+            (dict) The dictionary representation of this execution
+        """
+
         return {
             "ID" : self.ID,
             "functionName": self.functionName,
             "arguments": self.arguments,
             "handled": self.handled
         }
         
-    """
-    Marks this execution as handled and saves return values.
-    
-    Args:
-        returnValues: (list) The return values from the in-game function.
-        
-    Raises:
-        exceptions.InternalError: Raised if this method is called when the execution is already handled.
-    """
     def _return(self, returnValues: list):
+        """
+        Marks this execution as handled and saves return values.
+        
+        Args:
+            returnValues: (list) The return values from the in-game function.
+            
+        Raises:
+            exceptions.InternalError: Raised if this method is called when the execution is already handled.
+        """
+
         if self.handled:
             raise exceptions.InternalError("Tried to return after already returning")
         
         self.handled = True
         self.returnValues = returnValues
     
-    """
-    Stops waiting on this execution via _wait() method.
-    """
     def _halt(self):
+        """
+        Stops waiting on this execution via _wait() method.
+        """
+
         self.isWaiting = False
         
-    """
-    Returns whether this execution has been handled.
-    
-    Returns:
-        (bool) Whether this execution has been handled.
-    """
     def _obsolete(self):
+        """
+        Returns whether this execution has been handled.
+        
+        Returns:
+            (bool) Whether this execution has been handled.
+        """
+
         return not self.isWaiting
         
-    """
-    Waits until this execution has been handled and returns the return values.
-    
-    Returns:
-        (list) The return values from the in-game function call.
-    """
     def _wait(self) -> list:
+        """
+        Waits until this execution has been handled and returns the return values.
+        
+        Returns:
+            (list) The return values from the in-game function call.
+        """
+
         self.isWaiting = True
         
         while not self.handled and self.isWaiting:
             time.sleep(0.01)
             
         return self.returnValues
```

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/addAdmin.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/addAdmin.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/addAuth.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/addAuth.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/addMapLabel.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/addMapLabel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/addMapLine.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/addMapLine.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/addMapObject.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/addMapObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/announce.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/announce.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/cancelGerstner.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/cancelGerstner.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/clearOilSpills.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/clearOilSpills.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/clearRadiation.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/clearRadiation.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/clearVehicles.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/clearVehicles.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/despawnObject.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/despawnObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/despawnVehicle.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/despawnVehicle.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/despawnVehicleGroup.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/despawnVehicleGroup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/getAddonIndex.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/getAddonIndex.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/getCharacterItem.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/getCharacterItem.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/getCurrency.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/getCurrency.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/getGameSettings.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/getGameSettings.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/getObjectData.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/getObjectData.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/getPlayerCharacter.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/getPlayerCharacter.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/getPlayerLookDirection.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/getPlayerLookDirection.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/getPlayerName.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/getPlayerName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/getPlayerPos.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/getPlayerPos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/getPlayers.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/getPlayers.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/getSeasonalEvent.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/getSeasonalEvent.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/getUniqueID.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/getUniqueID.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/getVehicleBatteryByName.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/getVehicleBatteryByName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/getVehicleBatteryByVoxel.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/getVehicleBatteryByVoxel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/getVehicleComponents.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/getVehicleComponents.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/getVehicleData.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/getVehicleData.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/getVehicleGroup.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/getVehicleGroup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/getVehiclePos.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/getVehiclePos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/getVehicleTankByName.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/getVehicleTankByName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/getVehicleTankByVoxel.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/getVehicleTankByVoxel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/isAridDLC.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/isAridDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/isSpaceDLC.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/isSpaceDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/isWeaponsDLC.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/isWeaponsDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/moveGroup.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/moveGroup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/moveGroupSafe.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/moveGroupSafe.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/moveVehicle.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/moveVehicle.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/moveVehicleSafe.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/moveVehicleSafe.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/notify.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/notify.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/removeAdmin.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/removeAdmin.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/removeAuth.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/removeAuth.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/removeMapLabel.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/removeMapLabel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/removeMapLine.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/removeMapLine.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/removeMapObject.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/removeMapObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/removePopup.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/removePopup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/setCharacterData.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/setCharacterData.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/setCharacterItem.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/setCharacterItem.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/setCharacterTooltip.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/setCharacterTooltip.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/setCreatureMoveTarget.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/setCreatureMoveTarget.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/setCurrency.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/setCurrency.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/setGameSetting.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/setGameSetting.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/setGroupPosSafe.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/setGroupPosSafe.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/setOilSpill.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/setOilSpill.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/setPlayerPos.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/setPlayerPos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/setPopup.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/setPopup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/setVehicleBatteryByName.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/setVehicleBatteryByName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/setVehicleBatteryByVoxel.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/setVehicleBatteryByVoxel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/setVehicleEditable.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/setVehicleEditable.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/setVehicleInvulnerable.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/setVehicleInvulnerable.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/setVehiclePos.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/setVehiclePos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/setVehiclePosSafe.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/setVehiclePosSafe.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/setVehicleShowOnMap.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/setVehicleShowOnMap.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/setVehicleTankByName.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/setVehicleTankByName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/setVehicleTankByVoxel.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/setVehicleTankByVoxel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/spawnAddonVehicle.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/spawnAddonVehicle.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/spawnCharacter.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/spawnCharacter.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/spawnCreature.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/spawnCreature.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/spawnEquipment.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/spawnEquipment.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/spawnExplosion.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/spawnExplosion.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/spawnMeteor.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/spawnMeteor.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/spawnMeteorShower.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/spawnMeteorShower.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/spawnObject.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/spawnObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/spawnTsunami.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/spawnTsunami.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/spawnVehicle.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/spawnVehicle.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/spawnVolcano.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/spawnVolcano.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/executions/spawnWhirlpool.py` & `PythonToSW-1.2.3/src/PythonToSW/executions/spawnWhirlpool.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.2/src/PythonToSW/helpers.py` & `PythonToSW-1.2.3/src/PythonToSW/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,76 +25,81 @@
 
 # ---- // Imports
 import urllib.parse
 import xmltodict
 import os
 
 # ---- // Main
-"""
-URL decode a URL encoded string.
-
-Args:
-    string: (str) The URL encoded string to decode.
-    
-Returns:
-    (str) The decoded string.
-"""
 def URLDecode(string: str) -> str:
-    return urllib.parse.unquote(string)
+    """
+    URL decode a URL encoded string.
 
-"""
-URL encode a string.
+    Args:
+        string: (str) The URL encoded string to decode.
+        
+    Returns:
+        (str) The decoded string.
+    """
+
+    return urllib.parse.unquote(string)
 
-Args:
-    string: (str) The string to URL encode.
-    
-Returns:
-    (str) The URL encoded string.
-"""
 def XMLEncode(dictionary: dict) -> str:
-    return xmltodict.unparse(dictionary)
+    """
+    URL encode a string.
 
-"""
-Decode an XML string into a dictionary.
+    Args:
+        string: (str) The string to URL encode.
+        
+    Returns:
+        (str) The URL encoded string.
+    """
+
+    return xmltodict.unparse(dictionary)
 
-Args:
-    string: (str) The XML string to decode.
-    
-Returns:
-    (dict) The result of the XML decoding.
-"""
 def XMLDecode(string: str) -> dict:
-    return xmltodict.parse(string)
+    """
+    Decode an XML string into a dictionary.
+
+    Args:
+        string: (str) The XML string to decode.
+        
+    Returns:
+        (dict) The result of the XML decoding.
+    """
 
-"""
-Read a file.
+    return xmltodict.parse(string)
 
-Args:
-    path: (str) The path to the file to read.
-    mode: (str = "r") The mode to open the file in.
-
-Returns:
-    (str) The content of the file.
-"""
 def quickRead(path: str, mode: str = "r"):
+    """
+    Read a file.
+
+    Args:
+        path: (str) The path to the file to read.
+        mode: (str = "r") The mode to open the file in.
+
+    Returns:
+        (str) The content of the file.
+    """
+
     with open(path, mode) as f:
         return f.read()
     
-"""
-Write to a file, creating the directories if they don't exist.
-
-Args:
-    path: (str) The path to the file to write to.
-    content: (str) The content to write to the file.
-    mode: (str = "w") The mode to open the file in.
-    
-Returns:
-    (int) The result of the write operation.
-"""
 def quickWrite(path: str, content: str, mode: str = "w"):
+    """
+    Write to a file, creating the directories if they don't exist.
+
+    Args:
+        path: (str) The path to the file to write to.
+        content: (str) The content to write to the file.
+        mode: (str = "w") The mode to open the file in.
+        
+    Returns:
+        (int) The result of the write operation.
+    """
+
     directory = os.path.dirname(path)
 
     if not os.path.exists(directory):
         os.makedirs(directory, exist_ok = True)
     
     with open(path, mode) as f:
         return f.write(content)
```

### Comparing `PythonToSW-1.2.2/src/PythonToSW/matrix.py` & `PythonToSW-1.2.3/src/PythonToSW/matrix.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,52 +23,55 @@
 limitations under the License.
 """
 
 # ---- // Variables
 import math
 
 # ---- // Main
-"""
-Creates a new matrix with the given XYZ.
-
-Args:
-    x: (float|int) The X coordinate.
-    y: (float|int) The Y coordinate.
-    z: (float|int) The Z coordinate. 
-    
-Returns:
-    (list) The constructed matrix.
-"""
 def new(x: float|int, y: float|int, z: float|int) -> list:
+    """
+    Creates a new matrix with the given XYZ.
+
+    Args:
+        x: (float|int) The X coordinate.
+        y: (float|int) The Y coordinate.
+        z: (float|int) The Z coordinate. 
+        
+    Returns:
+        (list) The constructed matrix.
+    """
+
     return [
         1, 0, 0, 0,
         0, 0, 0, 0,
         0, 0, 1, 0,
         x, y, z, 1
     ]
-    
-"""
-Returns the X, Y, and Z coordinates of a matrix.
 
-Args:
-    matrix: (list) The matrix to get the XYZ from.
-    
-Returns:
-    (float) The X coordinate.
-    (float) The Y coordinate.
-    (float) The Z coordinate.
-"""
 def getXYZ(matrix: list) -> tuple[float, float, float]:
-    return matrix[12], matrix[13], matrix[14]
+    """
+    Returns the X, Y, and Z coordinates of a matrix.
 
-"""
-Returns the distance between two matrices.
+    Args:
+        matrix: (list) The matrix to get the XYZ from.
+        
+    Returns:
+        (float) The X coordinate.
+        (float) The Y coordinate.
+        (float) The Z coordinate.
+    """
+
+    return matrix[12], matrix[13], matrix[14]
 
-Args:
-    matrix1: (list) The first matrix.
-    matrix2: (list) The second matrix.
-    
-Returns:
-    (float) The distance between the two matrices.
-"""
 def distance(matrix1: list, matrix2: list) -> float:
+    """
+    Returns the distance between two matrices.
+
+    Args:
+        matrix1: (list) The first matrix.
+        matrix2: (list) The second matrix.
+        
+    Returns:
+        (float) The distance between the two matrices.
+    """
+
     return math.sqrt((matrix1[12] - matrix2[12])**2 + (matrix1[13] - matrix2[13])**2 + (matrix1[14] - matrix2[14])**2)
```

### Comparing `PythonToSW-1.2.2/src/PythonToSW.egg-info/PKG-INFO` & `PythonToSW-1.2.3/src/PythonToSW.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonToSW
-Version: 1.2.2
+Version: 1.2.3
 Summary: A package that allows you to create addons in Stormworks with Python, handled through HTTP.
 Author: Cuh4
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `PythonToSW-1.2.2/src/PythonToSW.egg-info/SOURCES.txt` & `PythonToSW-1.2.3/src/PythonToSW.egg-info/SOURCES.txt`

 * *Files identical despite different names*

