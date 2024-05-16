# Comparing `tmp/PythonToSW-1.1.3.tar.gz` & `tmp/PythonToSW-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonToSW-1.1.3.tar", last modified: Thu May 16 00:03:43 2024, max compression
+gzip compressed data, was "PythonToSW-1.2.0.tar", last modified: Thu May 16 22:39:11 2024, max compression
```

## Comparing `PythonToSW-1.1.3.tar` & `PythonToSW-1.2.0.tar`

### file list

```diff
@@ -1,101 +1,108 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 00:03:43.925675 PythonToSW-1.1.3/
--rw-rw-rw-   0        0        0    11558 2024-01-17 15:06:42.000000 PythonToSW-1.1.3/LICENSE
--rw-rw-rw-   0        0        0       92 2024-05-15 22:14:52.000000 PythonToSW-1.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1782 2024-05-16 00:03:43.925675 PythonToSW-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1246 2024-05-16 00:02:39.000000 PythonToSW-1.1.3/README.md
--rw-rw-rw-   0        0        0        5 2024-05-16 00:02:36.000000 PythonToSW-1.1.3/VERSION
--rw-rw-rw-   0        0        0       52 2024-05-15 22:15:14.000000 PythonToSW-1.1.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 00:03:43.925675 PythonToSW-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1878 2024-05-15 22:15:23.000000 PythonToSW-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 00:03:43.766994 PythonToSW-1.1.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-16 00:03:43.817008 PythonToSW-1.1.3/src/PythonToSW/
--rw-rw-rw-   0        0        0      973 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 00:03:43.859954 PythonToSW-1.1.3/src/PythonToSW/addon/
--rw-rw-rw-   0        0        0      143 2024-05-13 00:11:11.000000 PythonToSW-1.1.3/src/PythonToSW/addon/playlist.xml
--rw-rw-rw-   0        0        0   159991 2024-05-14 16:56:49.000000 PythonToSW-1.1.3/src/PythonToSW/addon/script.lua
--rw-rw-rw-   0        0        0    11087 2024-05-15 22:27:06.000000 PythonToSW-1.1.3/src/PythonToSW/addon.py
--rw-rw-rw-   0        0        0     1868 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/event.py
--rw-rw-rw-   0        0        0     1064 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-16 00:03:43.924158 PythonToSW-1.1.3/src/PythonToSW/executions/
--rw-rw-rw-   0        0        0     2809 2024-05-14 23:36:22.000000 PythonToSW-1.1.3/src/PythonToSW/executions/__createExecution.py
--rw-rw-rw-   0        0        0     1711 2024-05-14 23:24:00.000000 PythonToSW-1.1.3/src/PythonToSW/executions/__generateImportCode.py
--rw-rw-rw-   0        0        0     5426 2024-05-16 00:02:23.000000 PythonToSW-1.1.3/src/PythonToSW/executions/__init__.py
--rw-rw-rw-   0        0        0     1059 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/executions/addAdmin.py
--rw-rw-rw-   0        0        0     1056 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/executions/addAuth.py
--rw-rw-rw-   0        0        0     1216 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/executions/addMapLabel.py
--rw-rw-rw-   0        0        0     1220 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/executions/addMapLine.py
--rw-rw-rw-   0        0        0     1582 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/executions/addMapObject.py
--rw-rw-rw-   0        0        0     1107 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/executions/announce.py
--rw-rw-rw-   0        0        0     1027 2024-05-14 23:48:22.000000 PythonToSW-1.1.3/src/PythonToSW/executions/cancelGerstner.py
--rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/executions/clearOilSpills.py
--rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/executions/clearRadiation.py
--rw-rw-rw-   0        0        0     1025 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/executions/clearVehicles.py
--rw-rw-rw-   0        0        0     1106 2024-05-14 23:49:23.000000 PythonToSW-1.1.3/src/PythonToSW/executions/despawnObject.py
--rw-rw-rw-   0        0        0     1111 2024-05-14 23:49:25.000000 PythonToSW-1.1.3/src/PythonToSW/executions/despawnVehicle.py
--rw-rw-rw-   0        0        0     1123 2024-05-14 23:49:26.000000 PythonToSW-1.1.3/src/PythonToSW/executions/despawnVehicleGroup.py
--rw-rw-rw-   0        0        0     1105 2024-05-14 18:26:42.000000 PythonToSW-1.1.3/src/PythonToSW/executions/getCharacterItem.py
--rw-rw-rw-   0        0        0     1018 2024-05-15 22:28:57.000000 PythonToSW-1.1.3/src/PythonToSW/executions/getCurrency.py
--rw-rw-rw-   0        0        0     1079 2024-05-14 18:24:19.000000 PythonToSW-1.1.3/src/PythonToSW/executions/getObjectData.py
--rw-rw-rw-   0        0        0     1092 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/executions/getPlayerCharacter.py
--rw-rw-rw-   0        0        0     1103 2024-05-16 00:01:47.000000 PythonToSW-1.1.3/src/PythonToSW/executions/getPlayerLookDirection.py
--rw-rw-rw-   0        0        0     1075 2024-05-16 00:01:47.000000 PythonToSW-1.1.3/src/PythonToSW/executions/getPlayerName.py
--rw-rw-rw-   0        0        0     1072 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/executions/getPlayerPos.py
--rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/executions/getPlayers.py
--rw-rw-rw-   0        0        0     1035 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/executions/getSeasonalEvent.py
--rw-rw-rw-   0        0        0     1017 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/executions/getUniqueID.py
--rw-rw-rw-   0        0        0     1138 2024-05-14 23:44:48.000000 PythonToSW-1.1.3/src/PythonToSW/executions/getVehicleBatteryByName.py
--rw-rw-rw-   0        0        0     1172 2024-05-14 23:44:45.000000 PythonToSW-1.1.3/src/PythonToSW/executions/getVehicleBatteryByVoxel.py
--rw-rw-rw-   0        0        0     1102 2024-05-14 18:30:01.000000 PythonToSW-1.1.3/src/PythonToSW/executions/getVehicleComponents.py
--rw-rw-rw-   0        0        0     1084 2024-05-14 18:29:46.000000 PythonToSW-1.1.3/src/PythonToSW/executions/getVehicleData.py
--rw-rw-rw-   0        0        0     1083 2024-05-15 22:28:49.000000 PythonToSW-1.1.3/src/PythonToSW/executions/getVehicleGroup.py
--rw-rw-rw-   0        0        0     1162 2024-05-15 22:08:55.000000 PythonToSW-1.1.3/src/PythonToSW/executions/getVehiclePos.py
--rw-rw-rw-   0        0        0     1123 2024-05-14 23:44:59.000000 PythonToSW-1.1.3/src/PythonToSW/executions/getVehicleTankByName.py
--rw-rw-rw-   0        0        0     1163 2024-05-14 23:45:28.000000 PythonToSW-1.1.3/src/PythonToSW/executions/getVehicleTankByVoxel.py
--rw-rw-rw-   0        0        0     1012 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/executions/isAridDLC.py
--rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/executions/isSpaceDLC.py
--rw-rw-rw-   0        0        0     1021 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/executions/isWeaponsDLC.py
--rw-rw-rw-   0        0        0     1080 2024-05-16 00:01:47.000000 PythonToSW-1.1.3/src/PythonToSW/executions/moveGroup.py
--rw-rw-rw-   0        0        0     1093 2024-05-16 00:01:47.000000 PythonToSW-1.1.3/src/PythonToSW/executions/moveGroupSafe.py
--rw-rw-rw-   0        0        0     1090 2024-05-16 00:01:47.000000 PythonToSW-1.1.3/src/PythonToSW/executions/moveVehicle.py
--rw-rw-rw-   0        0        0     1103 2024-05-16 00:02:01.000000 PythonToSW-1.1.3/src/PythonToSW/executions/moveVehicleSafe.py
--rw-rw-rw-   0        0        0     1135 2024-05-14 23:47:34.000000 PythonToSW-1.1.3/src/PythonToSW/executions/notify.py
--rw-rw-rw-   0        0        0     1068 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/executions/removeAdmin.py
--rw-rw-rw-   0        0        0     1065 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/executions/removeAuth.py
--rw-rw-rw-   0        0        0     1097 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/executions/removeMapLabel.py
--rw-rw-rw-   0        0        0     1094 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/executions/removeMapLine.py
--rw-rw-rw-   0        0        0     1100 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/executions/removeMapObject.py
--rw-rw-rw-   0        0        0     1087 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/executions/removePopup.py
--rw-rw-rw-   0        0        0     1171 2024-05-14 18:25:00.000000 PythonToSW-1.1.3/src/PythonToSW/executions/setCharacterData.py
--rw-rw-rw-   0        0        0     1222 2024-05-14 18:26:10.000000 PythonToSW-1.1.3/src/PythonToSW/executions/setCharacterItem.py
--rw-rw-rw-   0        0        0     1120 2024-05-14 18:25:27.000000 PythonToSW-1.1.3/src/PythonToSW/executions/setCharacterTooltip.py
--rw-rw-rw-   0        0        0     1115 2024-05-14 23:49:29.000000 PythonToSW-1.1.3/src/PythonToSW/executions/setCreatureMoveTarget.py
--rw-rw-rw-   0        0        0     1115 2024-05-15 22:28:48.000000 PythonToSW-1.1.3/src/PythonToSW/executions/setCurrency.py
--rw-rw-rw-   0        0        0     1100 2024-05-16 00:01:49.000000 PythonToSW-1.1.3/src/PythonToSW/executions/setGroupPosSafe.py
--rw-rw-rw-   0        0        0     1089 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/executions/setOilSpill.py
--rw-rw-rw-   0        0        0     1088 2024-05-14 16:56:13.000000 PythonToSW-1.1.3/src/PythonToSW/executions/setPlayerPos.py
--rw-rw-rw-   0        0        0     1299 2024-05-14 18:18:44.000000 PythonToSW-1.1.3/src/PythonToSW/executions/setPopup.py
--rw-rw-rw-   0        0        0     1161 2024-05-14 23:43:28.000000 PythonToSW-1.1.3/src/PythonToSW/executions/setVehicleBatteryByName.py
--rw-rw-rw-   0        0        0     1194 2024-05-14 23:42:27.000000 PythonToSW-1.1.3/src/PythonToSW/executions/setVehicleBatteryByVoxel.py
--rw-rw-rw-   0        0        0     1126 2024-05-14 23:39:49.000000 PythonToSW-1.1.3/src/PythonToSW/executions/setVehicleEditable.py
--rw-rw-rw-   0        0        0     1146 2024-05-14 23:39:47.000000 PythonToSW-1.1.3/src/PythonToSW/executions/setVehicleInvulnerable.py
--rw-rw-rw-   0        0        0     1097 2024-05-15 22:08:43.000000 PythonToSW-1.1.3/src/PythonToSW/executions/setVehiclePos.py
--rw-rw-rw-   0        0        0     1110 2024-05-16 00:01:47.000000 PythonToSW-1.1.3/src/PythonToSW/executions/setVehiclePosSafe.py
--rw-rw-rw-   0        0        0     1123 2024-05-14 23:39:52.000000 PythonToSW-1.1.3/src/PythonToSW/executions/setVehicleShowOnMap.py
--rw-rw-rw-   0        0        0     1146 2024-05-14 23:43:54.000000 PythonToSW-1.1.3/src/PythonToSW/executions/setVehicleTankByName.py
--rw-rw-rw-   0        0        0     1186 2024-05-14 23:44:14.000000 PythonToSW-1.1.3/src/PythonToSW/executions/setVehicleTankByVoxel.py
--rw-rw-rw-   0        0        0     1095 2024-05-14 23:46:38.000000 PythonToSW-1.1.3/src/PythonToSW/executions/spawnCharacter.py
--rw-rw-rw-   0        0        0     1143 2024-05-14 23:47:06.000000 PythonToSW-1.1.3/src/PythonToSW/executions/spawnCreature.py
--rw-rw-rw-   0        0        0     1099 2024-05-14 23:47:30.000000 PythonToSW-1.1.3/src/PythonToSW/executions/spawnExplosion.py
--rw-rw-rw-   0        0        0     1128 2024-05-14 23:46:36.000000 PythonToSW-1.1.3/src/PythonToSW/executions/spawnMeteor.py
--rw-rw-rw-   0        0        0     1147 2024-05-14 23:45:56.000000 PythonToSW-1.1.3/src/PythonToSW/executions/spawnMeteorShower.py
--rw-rw-rw-   0        0        0     1093 2024-05-14 23:45:58.000000 PythonToSW-1.1.3/src/PythonToSW/executions/spawnTsunami.py
--rw-rw-rw-   0        0        0     1093 2024-05-14 23:45:54.000000 PythonToSW-1.1.3/src/PythonToSW/executions/spawnVolcano.py
--rw-rw-rw-   0        0        0     1099 2024-05-14 23:45:59.000000 PythonToSW-1.1.3/src/PythonToSW/executions/spawnWhirlpool.py
--rw-rw-rw-   0        0        0     1618 2024-05-14 17:19:17.000000 PythonToSW-1.1.3/src/PythonToSW/helpers.py
--rw-rw-rw-   0        0        0     1428 2024-05-15 22:17:00.000000 PythonToSW-1.1.3/src/PythonToSW/matrix.py
-drwxrwxrwx   0        0        0        0 2024-05-16 00:03:43.924928 PythonToSW-1.1.3/src/PythonToSW.egg-info/
--rw-rw-rw-   0        0        0     1782 2024-05-16 00:03:43.000000 PythonToSW-1.1.3/src/PythonToSW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3759 2024-05-16 00:03:43.000000 PythonToSW-1.1.3/src/PythonToSW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 00:03:43.000000 PythonToSW-1.1.3/src/PythonToSW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-16 00:03:43.000000 PythonToSW-1.1.3/src/PythonToSW.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-16 00:03:43.000000 PythonToSW-1.1.3/src/PythonToSW.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 22:39:11.565206 PythonToSW-1.2.0/
+-rw-rw-rw-   0        0        0    11558 2024-01-17 15:06:42.000000 PythonToSW-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0       92 2024-05-15 22:14:52.000000 PythonToSW-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1803 2024-05-16 22:39:11.563716 PythonToSW-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1242 2024-05-16 22:19:42.000000 PythonToSW-1.2.0/README.md
+-rw-rw-rw-   0        0        0        5 2024-05-16 22:39:04.000000 PythonToSW-1.2.0/VERSION
+-rw-rw-rw-   0        0        0       62 2024-05-16 22:06:47.000000 PythonToSW-1.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 22:39:11.565206 PythonToSW-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1878 2024-05-15 22:15:23.000000 PythonToSW-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 22:39:11.428155 PythonToSW-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-16 22:39:11.438942 PythonToSW-1.2.0/src/PythonToSW/
+-rw-rw-rw-   0        0        0      973 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 22:39:11.471940 PythonToSW-1.2.0/src/PythonToSW/addon/
+-rw-rw-rw-   0        0        0      315 2024-05-16 03:46:54.000000 PythonToSW-1.2.0/src/PythonToSW/addon/playlist.xml
+-rw-rw-rw-   0        0        0   161117 2024-05-16 21:57:12.000000 PythonToSW-1.2.0/src/PythonToSW/addon/script.lua
+-rw-rw-rw-   0        0        0    14905 2024-05-16 22:37:18.000000 PythonToSW-1.2.0/src/PythonToSW/addon.py
+-rw-rw-rw-   0        0        0     1868 2024-05-16 22:33:36.000000 PythonToSW-1.2.0/src/PythonToSW/event.py
+-rw-rw-rw-   0        0        0     1114 2024-05-16 03:34:55.000000 PythonToSW-1.2.0/src/PythonToSW/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-16 22:39:11.559641 PythonToSW-1.2.0/src/PythonToSW/executions/
+-rw-rw-rw-   0        0        0     2809 2024-05-14 23:36:22.000000 PythonToSW-1.2.0/src/PythonToSW/executions/__createExecution.py
+-rw-rw-rw-   0        0        0     1711 2024-05-14 23:24:00.000000 PythonToSW-1.2.0/src/PythonToSW/executions/__generateImportCode.py
+-rw-rw-rw-   0        0        0     5825 2024-05-16 22:21:16.000000 PythonToSW-1.2.0/src/PythonToSW/executions/__init__.py
+-rw-rw-rw-   0        0        0     1059 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/addAdmin.py
+-rw-rw-rw-   0        0        0     1056 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/addAuth.py
+-rw-rw-rw-   0        0        0     1216 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/addMapLabel.py
+-rw-rw-rw-   0        0        0     1220 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/addMapLine.py
+-rw-rw-rw-   0        0        0     1582 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/addMapObject.py
+-rw-rw-rw-   0        0        0     1107 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/announce.py
+-rw-rw-rw-   0        0        0     1027 2024-05-14 23:48:22.000000 PythonToSW-1.2.0/src/PythonToSW/executions/cancelGerstner.py
+-rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/clearOilSpills.py
+-rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/clearRadiation.py
+-rw-rw-rw-   0        0        0     1025 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/clearVehicles.py
+-rw-rw-rw-   0        0        0     1106 2024-05-14 23:49:23.000000 PythonToSW-1.2.0/src/PythonToSW/executions/despawnObject.py
+-rw-rw-rw-   0        0        0     1111 2024-05-14 23:49:25.000000 PythonToSW-1.2.0/src/PythonToSW/executions/despawnVehicle.py
+-rw-rw-rw-   0        0        0     1123 2024-05-14 23:49:26.000000 PythonToSW-1.2.0/src/PythonToSW/executions/despawnVehicleGroup.py
+-rw-rw-rw-   0        0        0     1025 2024-05-16 04:08:52.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getAddonIndex.py
+-rw-rw-rw-   0        0        0     1105 2024-05-14 18:26:42.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getCharacterItem.py
+-rw-rw-rw-   0        0        0     1018 2024-05-15 22:28:57.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getCurrency.py
+-rw-rw-rw-   0        0        0     1031 2024-05-16 22:21:02.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getGameSettings.py
+-rw-rw-rw-   0        0        0     1079 2024-05-14 18:24:19.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getObjectData.py
+-rw-rw-rw-   0        0        0     1092 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getPlayerCharacter.py
+-rw-rw-rw-   0        0        0     1103 2024-05-16 00:01:47.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getPlayerLookDirection.py
+-rw-rw-rw-   0        0        0     1075 2024-05-16 00:01:47.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getPlayerName.py
+-rw-rw-rw-   0        0        0     1072 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getPlayerPos.py
+-rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getPlayers.py
+-rw-rw-rw-   0        0        0     1035 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getSeasonalEvent.py
+-rw-rw-rw-   0        0        0     1017 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getUniqueID.py
+-rw-rw-rw-   0        0        0     1138 2024-05-14 23:44:48.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleBatteryByName.py
+-rw-rw-rw-   0        0        0     1172 2024-05-14 23:44:45.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleBatteryByVoxel.py
+-rw-rw-rw-   0        0        0     1102 2024-05-14 18:30:01.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleComponents.py
+-rw-rw-rw-   0        0        0     1084 2024-05-14 18:29:46.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleData.py
+-rw-rw-rw-   0        0        0     1083 2024-05-15 22:28:49.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleGroup.py
+-rw-rw-rw-   0        0        0     1162 2024-05-15 22:08:55.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getVehiclePos.py
+-rw-rw-rw-   0        0        0     1123 2024-05-14 23:44:59.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleTankByName.py
+-rw-rw-rw-   0        0        0     1163 2024-05-14 23:45:28.000000 PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleTankByVoxel.py
+-rw-rw-rw-   0        0        0     1012 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/isAridDLC.py
+-rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/isSpaceDLC.py
+-rw-rw-rw-   0        0        0     1021 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/isWeaponsDLC.py
+-rw-rw-rw-   0        0        0     1080 2024-05-16 00:01:47.000000 PythonToSW-1.2.0/src/PythonToSW/executions/moveGroup.py
+-rw-rw-rw-   0        0        0     1093 2024-05-16 00:01:47.000000 PythonToSW-1.2.0/src/PythonToSW/executions/moveGroupSafe.py
+-rw-rw-rw-   0        0        0     1090 2024-05-16 00:01:47.000000 PythonToSW-1.2.0/src/PythonToSW/executions/moveVehicle.py
+-rw-rw-rw-   0        0        0     1103 2024-05-16 00:02:01.000000 PythonToSW-1.2.0/src/PythonToSW/executions/moveVehicleSafe.py
+-rw-rw-rw-   0        0        0     1135 2024-05-14 23:47:34.000000 PythonToSW-1.2.0/src/PythonToSW/executions/notify.py
+-rw-rw-rw-   0        0        0     1068 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/removeAdmin.py
+-rw-rw-rw-   0        0        0     1065 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/removeAuth.py
+-rw-rw-rw-   0        0        0     1097 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/removeMapLabel.py
+-rw-rw-rw-   0        0        0     1094 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/removeMapLine.py
+-rw-rw-rw-   0        0        0     1100 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/removeMapObject.py
+-rw-rw-rw-   0        0        0     1087 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/removePopup.py
+-rw-rw-rw-   0        0        0     1171 2024-05-14 18:25:00.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setCharacterData.py
+-rw-rw-rw-   0        0        0     1222 2024-05-14 18:26:10.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setCharacterItem.py
+-rw-rw-rw-   0        0        0     1120 2024-05-14 18:25:27.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setCharacterTooltip.py
+-rw-rw-rw-   0        0        0     1115 2024-05-14 23:49:29.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setCreatureMoveTarget.py
+-rw-rw-rw-   0        0        0     1115 2024-05-15 22:28:48.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setCurrency.py
+-rw-rw-rw-   0        0        0     1120 2024-05-16 22:20:48.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setGameSetting.py
+-rw-rw-rw-   0        0        0     1100 2024-05-16 00:01:49.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setGroupPosSafe.py
+-rw-rw-rw-   0        0        0     1089 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setOilSpill.py
+-rw-rw-rw-   0        0        0     1088 2024-05-14 16:56:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setPlayerPos.py
+-rw-rw-rw-   0        0        0     1299 2024-05-14 18:18:44.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setPopup.py
+-rw-rw-rw-   0        0        0     1161 2024-05-14 23:43:28.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleBatteryByName.py
+-rw-rw-rw-   0        0        0     1194 2024-05-14 23:42:27.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleBatteryByVoxel.py
+-rw-rw-rw-   0        0        0     1126 2024-05-14 23:39:49.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleEditable.py
+-rw-rw-rw-   0        0        0     1146 2024-05-14 23:39:47.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleInvulnerable.py
+-rw-rw-rw-   0        0        0     1097 2024-05-15 22:08:43.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setVehiclePos.py
+-rw-rw-rw-   0        0        0     1110 2024-05-16 00:01:47.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setVehiclePosSafe.py
+-rw-rw-rw-   0        0        0     1123 2024-05-14 23:39:52.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleShowOnMap.py
+-rw-rw-rw-   0        0        0     1146 2024-05-14 23:43:54.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleTankByName.py
+-rw-rw-rw-   0        0        0     1186 2024-05-14 23:44:14.000000 PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleTankByVoxel.py
+-rw-rw-rw-   0        0        0     1122 2024-05-16 04:03:12.000000 PythonToSW-1.2.0/src/PythonToSW/executions/spawnAddonVehicle.py
+-rw-rw-rw-   0        0        0     1095 2024-05-14 23:46:38.000000 PythonToSW-1.2.0/src/PythonToSW/executions/spawnCharacter.py
+-rw-rw-rw-   0        0        0     1143 2024-05-14 23:47:06.000000 PythonToSW-1.2.0/src/PythonToSW/executions/spawnCreature.py
+-rw-rw-rw-   0        0        0     1157 2024-05-16 04:03:12.000000 PythonToSW-1.2.0/src/PythonToSW/executions/spawnEquipment.py
+-rw-rw-rw-   0        0        0     1099 2024-05-14 23:47:30.000000 PythonToSW-1.2.0/src/PythonToSW/executions/spawnExplosion.py
+-rw-rw-rw-   0        0        0     1128 2024-05-14 23:46:36.000000 PythonToSW-1.2.0/src/PythonToSW/executions/spawnMeteor.py
+-rw-rw-rw-   0        0        0     1147 2024-05-14 23:45:56.000000 PythonToSW-1.2.0/src/PythonToSW/executions/spawnMeteorShower.py
+-rw-rw-rw-   0        0        0     1090 2024-05-16 04:03:13.000000 PythonToSW-1.2.0/src/PythonToSW/executions/spawnObject.py
+-rw-rw-rw-   0        0        0     1093 2024-05-14 23:45:58.000000 PythonToSW-1.2.0/src/PythonToSW/executions/spawnTsunami.py
+-rw-rw-rw-   0        0        0     1089 2024-05-16 04:03:12.000000 PythonToSW-1.2.0/src/PythonToSW/executions/spawnVehicle.py
+-rw-rw-rw-   0        0        0     1093 2024-05-14 23:45:54.000000 PythonToSW-1.2.0/src/PythonToSW/executions/spawnVolcano.py
+-rw-rw-rw-   0        0        0     1099 2024-05-14 23:45:59.000000 PythonToSW-1.2.0/src/PythonToSW/executions/spawnWhirlpool.py
+-rw-rw-rw-   0        0        0     1618 2024-05-16 03:09:58.000000 PythonToSW-1.2.0/src/PythonToSW/helpers.py
+-rw-rw-rw-   0        0        0     1428 2024-05-15 22:17:00.000000 PythonToSW-1.2.0/src/PythonToSW/matrix.py
+drwxrwxrwx   0        0        0        0 2024-05-16 22:39:11.561941 PythonToSW-1.2.0/src/PythonToSW.egg-info/
+-rw-rw-rw-   0        0        0     1803 2024-05-16 22:39:11.000000 PythonToSW-1.2.0/src/PythonToSW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4065 2024-05-16 22:39:11.000000 PythonToSW-1.2.0/src/PythonToSW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 22:39:11.000000 PythonToSW-1.2.0/src/PythonToSW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-16 22:39:11.000000 PythonToSW-1.2.0/src/PythonToSW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-16 22:39:11.000000 PythonToSW-1.2.0/src/PythonToSW.egg-info/top_level.txt
```

### Comparing `PythonToSW-1.1.3/LICENSE` & `PythonToSW-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/PKG-INFO` & `PythonToSW-1.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: PythonToSW
-Version: 1.1.3
+Version: 1.2.0
 Summary: A package that allows you to create addons in Stormworks with Python, handled through HTTP.
 Author: Cuh4
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyperclip
 Requires-Dist: requests
 Requires-Dist: urllib3
 Requires-Dist: uuid
 Requires-Dist: xmltodict
 Requires-Dist: flask
+Requires-Dist: colorama
 
 # ⚙️ | PythonToSW
 
 ## 📚 | Overview
 A Python package that allows you to create basic addons in Stormworks: Build and Rescue with Python.
 
 ```python
@@ -41,12 +42,12 @@
 
 ## ⚙️ | Installing this package
 - Use `pip install PythonToSW --upgrade`
 - Import the package with `import PythonToSW as PTS` in your code
 
 ## 😔 | Quirks
 - Noticeable delays. This project works through HTTP instead of converting Python code to Lua code, and HTTP is unfortunately slow.
-- Lack of vehicle support. I likely won't add vehicle support, sorry! :-(
 - For your addon to function, the host of the server must run the Python script behind your addon. Closing the Python script will essentially stop the addon.
+- No support for `property.slider` and `property.checkbox` as of now.
 
 ## ✨ | Credit
 - **Cuh4** ([GitHub](https://github.com/Cuh4))
```

### Comparing `PythonToSW-1.1.3/README.md` & `PythonToSW-1.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -23,12 +23,12 @@
 
 ## ⚙️ | Installing this package
 - Use `pip install PythonToSW --upgrade`
 - Import the package with `import PythonToSW as PTS` in your code
 
 ## 😔 | Quirks
 - Noticeable delays. This project works through HTTP instead of converting Python code to Lua code, and HTTP is unfortunately slow.
-- Lack of vehicle support. I likely won't add vehicle support, sorry! :-(
 - For your addon to function, the host of the server must run the Python script behind your addon. Closing the Python script will essentially stop the addon.
+- No support for `property.slider` and `property.checkbox` as of now.
 
 ## ✨ | Credit
 - **Cuh4** ([GitHub](https://github.com/Cuh4))
```

### Comparing `PythonToSW-1.1.3/setup.py` & `PythonToSW-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/__init__.py` & `PythonToSW-1.2.0/src/PythonToSW/__init__.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/addon/script.lua` & `PythonToSW-1.2.0/src/PythonToSW/addon/script.lua`

 * *Files 1% similar despite different names*

```diff
@@ -4945,14 +4945,15 @@
 ---@type CodeExecution
 CodeExecution = Class("CodeExecution", function(self, backendPort, executionTickRate)
     self.backendPort = backendPort
     self.executionTickRate = executionTickRate
     self.tickTimer = 0
     self.started = false
     self.handled = {}
+    self.requestCooldown = false
 end, BaseLibrary)
 
 -- Start the code execution
 function CodeExecution:start()
     -- error check
     if self.started then
         self:error("Addon", "Attempted to start code execution when it has already started.")
@@ -4977,41 +4978,41 @@
             goto continue
         end
 
         -- connect to event and trigger backend callback
         self:sendLog(("Connecting to event: %s."):format(name))
 
         callback.main:connect(function(...)
-            self:triggerCallback(name, ...)
+            self:triggerCallback(name, true, ...)
         end)
 
         ::continue::
     end
 
     -- manually handle http reply
     AuroraFramework.callbacks.httpReply.main:connect(function(port, ...)
         if port == 0 or port == self.backendPort then -- port 0 returns response the very next tick. not good for http!
             return
         end
 
-        self:triggerCallback("httpReply", ...)
+        self:triggerCallback("httpReply", true, ...)
     end)
 
     -- count up ticks
     AuroraFramework.callbacks.onTick.main:connect(function()
         -- increment ticks
         self.tickTimer = self.tickTimer + 1
 
         -- check if we should handle pending executions
         if self.tickTimer < self.executionTickRate then
             return
         end
 
         -- call ontick callback
-        self:triggerCallback("onTick")
+        self:triggerCallback("onTick", false)
 
         -- handle them
         self:handlePendingExecutions()
 
         -- reset timer
         self.tickTimer = 0
     end)
@@ -5022,28 +5023,30 @@
 -------------------------------
 ---@class CodeExecution: BaseLibrary
 ---@field backendPort number
 ---@field executionTickRate number
 ---@field tickTimer number
 ---@field started boolean
 ---@field handled table<string, boolean>
+---@field requestCooldown boolean
+---@field requestCooldownDelay af_services_timer_delay|nil
 ---
 ---
 ---@field start fun(self: CodeExecution) Start fetching pending executions and executing them
 ---
 ---@field copyTable fun(self: CodeExecution, tbl: table): table Copy a table
----@field sendRequest fun(self: CodeExecution, URL: string, callback: fun(response: string, successful: boolean)|nil): af_services_http_request Send a GET request
+---@field sendRequest fun(self: CodeExecution, URL: string, callback: fun(response: string, successful: boolean)|nil, priority: boolean|nil): af_services_http_request Send a GET request
 ---
 ---@field sendLog fun(self: CodeExecution, log: string) Send a log
 ---@field error fun(self: CodeExecution, errorType: string, errorMessage: string) Trigger an error in the backend
 ---
 ---@field handlePendingExecutions fun(self: CodeExecution) Handle pending executions
 ---@field getFunctionFromExecution fun(self: CodeExecution, execution: CodeExecution_PendingExecution): function|nil Get a server function from an execution
 ---@field returnExecutionResults fun(self: CodeExecution, execution: CodeExecution_PendingExecution, returnValues: table<integer, any>) Send return values to backend
----@field triggerCallback fun(self: CodeExecution, name: string, ...: any) Trigger a callback in the backend
+---@field triggerCallback fun(self: CodeExecution, name: string, priority: boolean, ...: any) Trigger a callback in the backend
 
 ---@class CodeExecution_PendingExecution
 ---@field ID string The ID of this execution
 ---@field functionName string The name of the function
 ---@field arguments table<integer, any> The arguments
 ---@field handled boolean Whether the execution has been handled or not
 
@@ -5095,16 +5098,46 @@
 
     return new
 end
 
 -- Send a request
 ---@param URL string
 ---@param callback fun(response: string, successful: boolean)|nil
+---@param priority boolean|nil
 ---@return af_services_http_request
-function CodeExecution:sendRequest(URL, callback)
+function CodeExecution:sendRequest(URL, callback, priority)
+    -- Send log
+    self:sendLog(("Sending request to %s. | Priority: %s | Is Cooldown: %s"):format(URL, tostring(priority), tostring(self.requestCooldown)))
+
+    -- stop here if this is not a priority request and a cooldown is active
+    if self.requestCooldown and not priority then
+        self:sendLog("Failed to send request due to cooldown. URL: "..URL)
+        return
+    end
+
+    -- if this is a priority request, then send the request straight away and add a tick cooldown to prevent rate limit
+    if priority then
+        -- set cooldown
+        self.requestCooldown = true
+
+        -- remove old cooldown if any
+        if self.requestCooldownDelay then
+            self.requestCooldownDelay:remove()
+        end
+
+        -- remove cooldown the next tick
+        self.requestCooldownDelay = AuroraFramework.services.timerService.delay.create(0, function()
+            self.requestCooldown = false
+            self.requestCooldownDelay = nil
+        end)
+    end
+
+    -- send request
+    self:sendLog("Successfully sent request.")
+
     return AuroraFramework.services.HTTPService.request(
         self.backendPort,
         URL,
         callback
     )
 end
 
@@ -5155,15 +5188,15 @@
 function CodeExecution:error(errorType, errorMessage)
     self:sendLog(("ERROR (%s): %s"):format(errorType, errorMessage))
 
     self:sendRequest(AuroraFramework.services.HTTPService.URLArgs(
         "/error",
         {name = "errorType", value = errorType},
         {name = "errorMessage", value = errorMessage}
-    ))
+    ), nil, true)
 end
 
 ----------------------------------------------
 -- // [File] src/addon\p2_libraries\1_CodeExecution\4_execution.lua
 ----------------------------------------------
 --------------------------------------------------------
 -- [Libraries] Code Execution - Execution
@@ -5195,77 +5228,73 @@
 ]]
 
 -------------------------------
 -- // Main
 -------------------------------
 -- Fetch pending executions
 function CodeExecution:handlePendingExecutions()
-    AuroraFramework.services.HTTPService.request(
-        self.backendPort,
-        "/get-pending-executions",
-        function(response, successful)
-            -- success check
-            if not successful then
-                return
-            end
-
-            -- get pending executions
-            local pendingExecutions = AuroraFramework.services.HTTPService.JSON.decode(response) ---@type table<integer, CodeExecution_PendingExecution>
-
-            if not pendingExecutions then
-                return
-            end
+    self:sendRequest("/get-pending-executions", function(response, successful)
+        -- success check
+        if not successful then
+            return
+        end
 
-            -- log
-            self:sendLog("Fetched pending executions, processing...")
+        -- get pending executions
+        local pendingExecutions = AuroraFramework.services.HTTPService.JSON.decode(response) ---@type table<integer, CodeExecution_PendingExecution>
 
-            -- iterate through executions
-            for _, execution in pairs(pendingExecutions) do
-                -- check if we've already handled this execution
-                if self.handled[execution.ID] then -- this is in place because the "/return" http request takes time, and this may take enough time that we get the same execution again before it is recognized as handled by "/return" request
-                    if execution.handled then
-                        self.handled[execution.ID] = nil -- garbage cleanup
-                    end
+        if not pendingExecutions then
+            return
+        end
 
-                    goto continue
-                end
+        -- log
+        self:sendLog("Fetched pending executions, processing...")
 
+        -- iterate through executions
+        for _, execution in pairs(pendingExecutions) do
+            -- check if we've already handled this execution
+            if self.handled[execution.ID] then -- this is in place because the "/return" http request takes time, and this may take enough time that we get the same execution again before it is recognized as handled by "/return" request
                 if execution.handled then
-                    goto continue
+                    self.handled[execution.ID] = nil -- garbage cleanup
                 end
 
-                -- log
-                self:sendLog(("Processing execution: %s (%s)"):format(execution.ID, execution.functionName))
+                goto continue
+            end
 
-                -- get function
-                local executionFunction = self:getFunctionFromExecution(execution)
+            if execution.handled then
+                goto continue
+            end
 
-                if not executionFunction then
-                    self:error("Execution", ("Function name in execution is invalid, got: %s"):format(execution.functionName))
-                    goto continue
-                end
+            -- log
+            self:sendLog(("Processing execution: %s (%s)"):format(execution.ID, execution.functionName))
+
+            -- get function
+            local executionFunction = self:getFunctionFromExecution(execution)
 
-                -- call function
-                local returnValues = table.pack(
-                    executionFunction(table.unpack(execution.arguments))
-                )
+            if not executionFunction then
+                self:error("Execution", ("Function name in execution is invalid, got: %s"):format(execution.functionName))
+                goto continue
+            end
 
-                -- send result to backend
-                self:returnExecutionResults(execution, returnValues)
+            -- call function
+            local returnValues = table.pack(
+                executionFunction(table.unpack(execution.arguments))
+            )
 
-                -- mark as handled
-                self.handled[execution.ID] = true
+            -- send result to backend
+            self:returnExecutionResults(execution, returnValues)
 
-                -- log
-                self:sendLog(("Handled execution %s. Sent return values back."):format(execution.ID))
+            -- mark as handled
+            self.handled[execution.ID] = true
 
-                ::continue::
-            end
+            -- log
+            self:sendLog(("Handled execution %s. Sent return values back."):format(execution.ID))
+
+            ::continue::
         end
-    )
+    end, false)
 end
 
 -- Get function from execution
 ---@param execution CodeExecution_PendingExecution
 ---@return function
 function CodeExecution:getFunctionFromExecution(execution)
     return server[execution.functionName]
@@ -5275,33 +5304,34 @@
 ---@param execution CodeExecution_PendingExecution
 ---@param returnValues table<integer, any>
 function CodeExecution:returnExecutionResults(execution, returnValues)
     self:sendRequest(AuroraFramework.services.HTTPService.URLArgs(
         "/return",
         {name = "id", value = execution.ID},
         {name = "returnValues", value = AuroraFramework.services.HTTPService.JSON.encode(returnValues)} -- sorry, sw only allows GET requests
-    ))
+    ), nil, true)
 end
 
 -- Trigger a callback
 ---@param name string
+---@param priority boolean
 ---@param ... any
-function CodeExecution:triggerCallback(name, ...)
+function CodeExecution:triggerCallback(name, priority, ...)
     self:sendRequest(AuroraFramework.services.HTTPService.URLArgs(
         "/trigger-callback",
         {name = "name", value = name},
         {name = "args", value = AuroraFramework.services.HTTPService.JSON.encode({...})}
-    ))
+    ), nil, priority)
 end
 
 ----------------------------------------------
 -- // [File] src/addon\p3_main\main.lua
 ----------------------------------------------
 --------------------------------------------------------
--- [Main] SW Python Addons
+-- [Main] Python To SW
 --------------------------------------------------------
 
 --[[
     ----------------------------
 
     CREDIT:
         Author: @Cuh4 (GitHub)
@@ -5327,9 +5357,9 @@
 ]]
 
 -------------------------------
 -- // Main
 -------------------------------
 -- Setup CodeExecution
 ---@type CodeExecution
-local CodeExecution = CodeExecution.new(__PORT__, 4) ---@diagnostic disable-line -- port is overridden by package
+local CodeExecution = CodeExecution.new(__PORT__, 3) ---@diagnostic disable-line -- port is overridden by package
 CodeExecution:start()
```

### Comparing `PythonToSW-1.1.3/src/PythonToSW/event.py` & `PythonToSW-1.2.0/src/PythonToSW/event.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/exceptions.py` & `PythonToSW-1.2.0/src/PythonToSW/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,8 +31,11 @@
 class FailedStartAttempt(Exception):
     pass
 
 class FailedExecutionAttempt(Exception):
     pass
 
 class InvalidExecutionID(Exception):
+    pass
+
+class InvalidVehiclePath(Exception):
     pass
```

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/__createExecution.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/__createExecution.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/__generateImportCode.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/__generateImportCode.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/__init__.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,17 @@
         self.functionName = functionName
         self.arguments = arguments
         
         self.handled = False
         self.returnValues = []
         self.isWaiting = False
         
+    def __str__(self):
+        return f"Execution-{self.ID} ({self.functionName})"
+        
     # Convert this execution to a JSON format
     def _toDict(self):
         return {
             "ID" : self.ID,
             "functionName": self.functionName,
             "arguments": self.arguments,
             "handled": self.handled
@@ -82,16 +85,18 @@
 from .cancelGerstner import CancelGerstner
 from .clearOilSpills import ClearOilSpills
 from .clearRadiation import ClearRadiation
 from .clearVehicles import ClearVehicles
 from .despawnObject import DespawnObject
 from .despawnVehicle import DespawnVehicle
 from .despawnVehicleGroup import DespawnVehicleGroup
+from .getAddonIndex import GetAddonIndex
 from .getCharacterItem import GetCharacterItem
 from .getCurrency import GetCurrency
+from .getGameSettings import GetGameSettings
 from .getObjectData import GetObjectData
 from .getPlayerCharacter import GetPlayerCharacter
 from .getPlayerLookDirection import GetPlayerLookDirection
 from .getPlayerName import GetPlayerName
 from .getPlayerPos import GetPlayerPos
 from .getPlayers import GetPlayers
 from .getSeasonalEvent import GetSeasonalEvent
@@ -119,28 +124,33 @@
 from .removeMapObject import RemoveMapObject
 from .removePopup import RemovePopup
 from .setCharacterData import SetCharacterData
 from .setCharacterItem import SetCharacterItem
 from .setCharacterTooltip import SetCharacterTooltip
 from .setCreatureMoveTarget import SetCreatureMoveTarget
 from .setCurrency import SetCurrency
+from .setGameSetting import SetGameSetting
 from .setGroupPosSafe import SetGroupPosSafe
 from .setOilSpill import SetOilSpill
 from .setPlayerPos import SetPlayerPos
 from .setPopup import SetPopup
 from .setVehicleBatteryByName import SetVehicleBatteryByName
 from .setVehicleBatteryByVoxel import SetVehicleBatteryByName
 from .setVehicleEditable import SetVehicleEditable
 from .setVehicleInvulnerable import SetVehicleInvulnerable
 from .setVehiclePos import SetVehiclePos
 from .setVehiclePosSafe import SetVehiclePosSafe
 from .setVehicleShowOnMap import SetVehicleShowOnMap
 from .setVehicleTankByName import SetVehicleTankByName
 from .setVehicleTankByVoxel import SetVehicleTankByVoxel
+from .spawnAddonVehicle import SpawnAddonVehicle
 from .spawnCharacter import SpawnCharacter
 from .spawnCreature import SpawnCreature
+from .spawnEquipment import SpawnEquipment
 from .spawnExplosion import SpawnExplosion
 from .spawnMeteor import SpawnMeteor
 from .spawnMeteorShower import SpawnMeteorShower
+from .spawnObject import SpawnObject
 from .spawnTsunami import SpawnTsunami
+from .spawnVehicle import SpawnVehicle
 from .spawnVolcano import SpawnVolcano
 from .spawnWhirlpool import SpawnWhirlpool
```

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/addAdmin.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/addAdmin.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/addAuth.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/addAuth.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/addMapLabel.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/addMapLabel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/addMapLine.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/addMapLine.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/addMapObject.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/addMapObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/announce.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/announce.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/cancelGerstner.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/cancelGerstner.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/clearOilSpills.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/clearOilSpills.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/clearRadiation.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/clearRadiation.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/clearVehicles.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/clearVehicles.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/despawnObject.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/despawnObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/despawnVehicle.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/despawnVehicle.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/despawnVehicleGroup.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/despawnVehicleGroup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/getCharacterItem.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/getCharacterItem.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/getCurrency.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/getCurrency.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/getObjectData.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/getObjectData.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/getPlayerCharacter.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/getPlayerCharacter.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/getPlayerLookDirection.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/getPlayerLookDirection.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/getPlayerName.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/getPlayerName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/getPlayerPos.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/getPlayerPos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/getPlayers.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/getPlayers.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/getSeasonalEvent.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/getSeasonalEvent.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/getUniqueID.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/getUniqueID.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/getVehicleBatteryByName.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleBatteryByName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/getVehicleBatteryByVoxel.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleBatteryByVoxel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/getVehicleComponents.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleComponents.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/getVehicleData.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleData.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/getVehicleGroup.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleGroup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/getVehiclePos.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/getVehiclePos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/getVehicleTankByName.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleTankByName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/getVehicleTankByVoxel.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/getVehicleTankByVoxel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/isAridDLC.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/isAridDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/isSpaceDLC.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/isSpaceDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/isWeaponsDLC.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/isWeaponsDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/moveGroup.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/moveGroup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/moveGroupSafe.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/moveGroupSafe.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/moveVehicle.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/moveVehicle.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/moveVehicleSafe.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/moveVehicleSafe.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/notify.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/notify.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/removeAdmin.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/removeAdmin.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/removeAuth.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/removeAuth.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/removeMapLabel.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/removeMapLabel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/removeMapLine.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/removeMapLine.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/removeMapObject.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/removeMapObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/removePopup.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/removePopup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/setCharacterData.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/setCharacterData.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/setCharacterItem.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/setCharacterItem.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/setCharacterTooltip.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/setCharacterTooltip.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/setCreatureMoveTarget.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/setCreatureMoveTarget.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/setCurrency.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/setCurrency.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/setGroupPosSafe.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/setGroupPosSafe.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/setOilSpill.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/setOilSpill.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/setPlayerPos.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/setPlayerPos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/setPopup.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/setPopup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/setVehicleBatteryByName.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleBatteryByName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/setVehicleBatteryByVoxel.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleBatteryByVoxel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/setVehicleEditable.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleEditable.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/setVehicleInvulnerable.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleInvulnerable.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/setVehiclePos.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/setVehiclePos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/setVehiclePosSafe.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/setVehiclePosSafe.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/setVehicleShowOnMap.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleShowOnMap.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/setVehicleTankByName.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleTankByName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/setVehicleTankByVoxel.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/setVehicleTankByVoxel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/spawnCharacter.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/spawnCharacter.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/spawnCreature.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/spawnCreature.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/spawnExplosion.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/spawnExplosion.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/spawnMeteor.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/spawnMeteor.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/spawnMeteorShower.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/spawnMeteorShower.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/spawnTsunami.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/spawnTsunami.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/spawnVolcano.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/spawnVolcano.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/executions/spawnWhirlpool.py` & `PythonToSW-1.2.0/src/PythonToSW/executions/spawnWhirlpool.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/helpers.py` & `PythonToSW-1.2.0/src/PythonToSW/helpers.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW/matrix.py` & `PythonToSW-1.2.0/src/PythonToSW/matrix.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.3/src/PythonToSW.egg-info/PKG-INFO` & `PythonToSW-1.2.0/src/PythonToSW.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: PythonToSW
-Version: 1.1.3
+Version: 1.2.0
 Summary: A package that allows you to create addons in Stormworks with Python, handled through HTTP.
 Author: Cuh4
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyperclip
 Requires-Dist: requests
 Requires-Dist: urllib3
 Requires-Dist: uuid
 Requires-Dist: xmltodict
 Requires-Dist: flask
+Requires-Dist: colorama
 
 # ⚙️ | PythonToSW
 
 ## 📚 | Overview
 A Python package that allows you to create basic addons in Stormworks: Build and Rescue with Python.
 
 ```python
@@ -41,12 +42,12 @@
 
 ## ⚙️ | Installing this package
 - Use `pip install PythonToSW --upgrade`
 - Import the package with `import PythonToSW as PTS` in your code
 
 ## 😔 | Quirks
 - Noticeable delays. This project works through HTTP instead of converting Python code to Lua code, and HTTP is unfortunately slow.
-- Lack of vehicle support. I likely won't add vehicle support, sorry! :-(
 - For your addon to function, the host of the server must run the Python script behind your addon. Closing the Python script will essentially stop the addon.
+- No support for `property.slider` and `property.checkbox` as of now.
 
 ## ✨ | Credit
 - **Cuh4** ([GitHub](https://github.com/Cuh4))
```

### Comparing `PythonToSW-1.1.3/src/PythonToSW.egg-info/SOURCES.txt` & `PythonToSW-1.2.0/src/PythonToSW.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -29,16 +29,18 @@
 src/PythonToSW/executions/cancelGerstner.py
 src/PythonToSW/executions/clearOilSpills.py
 src/PythonToSW/executions/clearRadiation.py
 src/PythonToSW/executions/clearVehicles.py
 src/PythonToSW/executions/despawnObject.py
 src/PythonToSW/executions/despawnVehicle.py
 src/PythonToSW/executions/despawnVehicleGroup.py
+src/PythonToSW/executions/getAddonIndex.py
 src/PythonToSW/executions/getCharacterItem.py
 src/PythonToSW/executions/getCurrency.py
+src/PythonToSW/executions/getGameSettings.py
 src/PythonToSW/executions/getObjectData.py
 src/PythonToSW/executions/getPlayerCharacter.py
 src/PythonToSW/executions/getPlayerLookDirection.py
 src/PythonToSW/executions/getPlayerName.py
 src/PythonToSW/executions/getPlayerPos.py
 src/PythonToSW/executions/getPlayers.py
 src/PythonToSW/executions/getSeasonalEvent.py
@@ -66,28 +68,33 @@
 src/PythonToSW/executions/removeMapObject.py
 src/PythonToSW/executions/removePopup.py
 src/PythonToSW/executions/setCharacterData.py
 src/PythonToSW/executions/setCharacterItem.py
 src/PythonToSW/executions/setCharacterTooltip.py
 src/PythonToSW/executions/setCreatureMoveTarget.py
 src/PythonToSW/executions/setCurrency.py
+src/PythonToSW/executions/setGameSetting.py
 src/PythonToSW/executions/setGroupPosSafe.py
 src/PythonToSW/executions/setOilSpill.py
 src/PythonToSW/executions/setPlayerPos.py
 src/PythonToSW/executions/setPopup.py
 src/PythonToSW/executions/setVehicleBatteryByName.py
 src/PythonToSW/executions/setVehicleBatteryByVoxel.py
 src/PythonToSW/executions/setVehicleEditable.py
 src/PythonToSW/executions/setVehicleInvulnerable.py
 src/PythonToSW/executions/setVehiclePos.py
 src/PythonToSW/executions/setVehiclePosSafe.py
 src/PythonToSW/executions/setVehicleShowOnMap.py
 src/PythonToSW/executions/setVehicleTankByName.py
 src/PythonToSW/executions/setVehicleTankByVoxel.py
+src/PythonToSW/executions/spawnAddonVehicle.py
 src/PythonToSW/executions/spawnCharacter.py
 src/PythonToSW/executions/spawnCreature.py
+src/PythonToSW/executions/spawnEquipment.py
 src/PythonToSW/executions/spawnExplosion.py
 src/PythonToSW/executions/spawnMeteor.py
 src/PythonToSW/executions/spawnMeteorShower.py
+src/PythonToSW/executions/spawnObject.py
 src/PythonToSW/executions/spawnTsunami.py
+src/PythonToSW/executions/spawnVehicle.py
 src/PythonToSW/executions/spawnVolcano.py
 src/PythonToSW/executions/spawnWhirlpool.py
```

