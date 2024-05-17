# Comparing `tmp/g3tables-0.2.3.tar.gz` & `tmp/g3tables-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g3tables-0.2.3.tar", last modified: Mon May 13 09:41:58 2024, max compression
+gzip compressed data, was "g3tables-0.2.4.tar", last modified: Fri May 17 06:51:40 2024, max compression
```

## Comparing `g3tables-0.2.3.tar` & `g3tables-0.2.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 09:41:58.776576 g3tables-0.2.3/
--rw-rw-rw-   0        0        0     1091 2024-04-29 08:48:33.000000 g3tables-0.2.3/LICENCE
--rw-rw-rw-   0        0        0     1325 2024-05-13 09:41:58.776576 g3tables-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0       81 2024-04-29 08:48:33.000000 g3tables-0.2.3/README.md
--rw-rw-rw-   0        0        0     1679 2024-05-13 09:39:47.000000 g3tables-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-13 09:41:58.776576 g3tables-0.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-13 09:41:58.698450 g3tables-0.2.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-13 09:41:58.714093 g3tables-0.2.3/src/g3tables/
--rw-rw-rw-   0        0        0      550 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:41:58.729703 g3tables-0.2.3/src/g3tables/plc_composition_io_table/
--rw-rw-rw-   0        0        0      361 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/plc_composition_io_table/__init__.py
--rw-rw-rw-   0        0        0    14539 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/plc_composition_io_table/_extend_table.py
--rw-rw-rw-   0        0        0    21360 2024-04-30 11:02:43.000000 g3tables-0.2.3/src/g3tables/plc_composition_io_table/_table.py
--rw-rw-rw-   0        0        0     5780 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/plc_composition_io_table/io_signals.json
--rw-rw-rw-   0        0        0        0 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/py.typed
-drwxrwxrwx   0        0        0        0 2024-05-13 09:41:58.729703 g3tables-0.2.3/src/g3tables/sw_definition_table/
--rw-rw-rw-   0        0        0      182 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/sw_definition_table/__init__.py
--rw-rw-rw-   0        0        0    54470 2024-05-13 09:37:12.000000 g3tables-0.2.3/src/g3tables/sw_definition_table/_table.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:41:58.745326 g3tables-0.2.3/src/g3tables/system_config/
--rw-rw-rw-   0        0        0      225 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/system_config/__init__.py
--rw-rw-rw-   0        0        0    15259 2024-05-13 09:37:18.000000 g3tables-0.2.3/src/g3tables/system_config/_cli.py
--rw-rw-rw-   0        0        0    22338 2024-04-30 11:02:43.000000 g3tables-0.2.3/src/g3tables/system_config/_g3core_updater.py
--rw-rw-rw-   0        0        0      972 2024-04-30 11:02:43.000000 g3tables-0.2.3/src/g3tables/system_config/_hw_connections.py
--rw-rw-rw-   0        0        0     8599 2024-04-30 11:02:43.000000 g3tables-0.2.3/src/g3tables/system_config/_iomap_updater.py
--rw-rw-rw-   0        0        0       74 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/system_config/_logger.py
--rw-rw-rw-   0        0        0     7326 2024-04-30 11:02:43.000000 g3tables-0.2.3/src/g3tables/system_config/_sw_system_dict_wrapper.py
--rw-rw-rw-   0        0        0     4132 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/system_config/_system_config_processor.py
--rw-rw-rw-   0        0        0     1192 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/system_config/type_hinting.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:41:58.745326 g3tables-0.2.3/src/g3tables/utils/
--rw-rw-rw-   0        0        0      146 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/utils/__init__.py
--rw-rw-rw-   0        0        0     1552 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/utils/_d2nd.py
--rw-rw-rw-   0        0        0     3706 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/utils/_interval.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:41:58.760955 g3tables-0.2.3/src/g3tables/utils/gdrive/
--rw-rw-rw-   0        0        0      365 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/utils/gdrive/__init__.py
--rw-rw-rw-   0        0        0     5172 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/utils/gdrive/_gdrive.py
--rw-rw-rw-   0        0        0     1263 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/utils/gdrive/_update_creds.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:41:58.760955 g3tables-0.2.3/src/g3tables/visualization_table/
--rw-rw-rw-   0        0        0      207 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/visualization_table/__init__.py
--rw-rw-rw-   0        0        0    14812 2024-05-12 17:57:40.000000 g3tables-0.2.3/src/g3tables/visualization_table/_table.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:41:58.760955 g3tables-0.2.3/src/g3tables.egg-info/
--rw-rw-rw-   0        0        0     1325 2024-05-13 09:41:58.000000 g3tables-0.2.3/src/g3tables.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1290 2024-05-13 09:41:58.000000 g3tables-0.2.3/src/g3tables.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 09:41:58.000000 g3tables-0.2.3/src/g3tables.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      207 2024-05-13 09:41:58.000000 g3tables-0.2.3/src/g3tables.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       79 2024-05-13 09:41:58.000000 g3tables-0.2.3/src/g3tables.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-13 09:41:58.000000 g3tables-0.2.3/src/g3tables.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 06:51:40.027411 g3tables-0.2.4/
+-rw-rw-rw-   0        0        0     1091 2024-04-29 08:48:33.000000 g3tables-0.2.4/LICENCE
+-rw-rw-rw-   0        0        0     1325 2024-05-17 06:51:40.026394 g3tables-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0       81 2024-04-29 08:48:33.000000 g3tables-0.2.4/README.md
+-rw-rw-rw-   0        0        0     1679 2024-05-17 06:30:23.000000 g3tables-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 06:51:40.027411 g3tables-0.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 06:51:39.944073 g3tables-0.2.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 06:51:39.958897 g3tables-0.2.4/src/g3tables/
+-rw-rw-rw-   0        0        0      550 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 06:51:39.974540 g3tables-0.2.4/src/g3tables/plc_composition_io_table/
+-rw-rw-rw-   0        0        0      361 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/plc_composition_io_table/__init__.py
+-rw-rw-rw-   0        0        0    14539 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/plc_composition_io_table/_extend_table.py
+-rw-rw-rw-   0        0        0    21360 2024-04-30 11:02:43.000000 g3tables-0.2.4/src/g3tables/plc_composition_io_table/_table.py
+-rw-rw-rw-   0        0        0     5780 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/plc_composition_io_table/io_signals.json
+-rw-rw-rw-   0        0        0        0 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-17 06:51:39.974540 g3tables-0.2.4/src/g3tables/sw_definition_table/
+-rw-rw-rw-   0        0        0      182 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/sw_definition_table/__init__.py
+-rw-rw-rw-   0        0        0    54470 2024-05-16 21:09:28.000000 g3tables-0.2.4/src/g3tables/sw_definition_table/_table.py
+drwxrwxrwx   0        0        0        0 2024-05-17 06:51:40.005803 g3tables-0.2.4/src/g3tables/system_config/
+-rw-rw-rw-   0        0        0      225 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/system_config/__init__.py
+-rw-rw-rw-   0        0        0    15259 2024-05-13 09:37:18.000000 g3tables-0.2.4/src/g3tables/system_config/_cli.py
+-rw-rw-rw-   0        0        0    22338 2024-04-30 11:02:43.000000 g3tables-0.2.4/src/g3tables/system_config/_g3core_updater.py
+-rw-rw-rw-   0        0        0      972 2024-04-30 11:02:43.000000 g3tables-0.2.4/src/g3tables/system_config/_hw_connections.py
+-rw-rw-rw-   0        0        0    12584 2024-05-17 06:27:59.000000 g3tables-0.2.4/src/g3tables/system_config/_iomap_updater.py
+-rw-rw-rw-   0        0        0       74 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/system_config/_logger.py
+-rw-rw-rw-   0        0        0     7323 2024-05-16 16:24:24.000000 g3tables-0.2.4/src/g3tables/system_config/_sw_system_dict_wrapper.py
+-rw-rw-rw-   0        0        0     4132 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/system_config/_system_config_processor.py
+-rw-rw-rw-   0        0        0     1192 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/system_config/type_hinting.py
+drwxrwxrwx   0        0        0        0 2024-05-17 06:51:40.005803 g3tables-0.2.4/src/g3tables/utils/
+-rw-rw-rw-   0        0        0      146 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/utils/__init__.py
+-rw-rw-rw-   0        0        0     1552 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/utils/_d2nd.py
+-rw-rw-rw-   0        0        0     3706 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/utils/_interval.py
+drwxrwxrwx   0        0        0        0 2024-05-17 06:51:40.005803 g3tables-0.2.4/src/g3tables/utils/gdrive/
+-rw-rw-rw-   0        0        0      365 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/utils/gdrive/__init__.py
+-rw-rw-rw-   0        0        0     5172 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/utils/gdrive/_gdrive.py
+-rw-rw-rw-   0        0        0     1263 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/utils/gdrive/_update_creds.py
+drwxrwxrwx   0        0        0        0 2024-05-17 06:51:40.021412 g3tables-0.2.4/src/g3tables/visualization_table/
+-rw-rw-rw-   0        0        0      207 2024-04-29 08:48:33.000000 g3tables-0.2.4/src/g3tables/visualization_table/__init__.py
+-rw-rw-rw-   0        0        0    14812 2024-05-16 16:24:45.000000 g3tables-0.2.4/src/g3tables/visualization_table/_table.py
+drwxrwxrwx   0        0        0        0 2024-05-17 06:51:40.021412 g3tables-0.2.4/src/g3tables.egg-info/
+-rw-rw-rw-   0        0        0     1325 2024-05-17 06:51:39.000000 g3tables-0.2.4/src/g3tables.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1290 2024-05-17 06:51:39.000000 g3tables-0.2.4/src/g3tables.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 06:51:39.000000 g3tables-0.2.4/src/g3tables.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      207 2024-05-17 06:51:39.000000 g3tables-0.2.4/src/g3tables.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       79 2024-05-17 06:51:39.000000 g3tables-0.2.4/src/g3tables.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-17 06:51:39.000000 g3tables-0.2.4/src/g3tables.egg-info/top_level.txt
```

### Comparing `g3tables-0.2.3/LICENCE` & `g3tables-0.2.4/LICENCE`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.3/PKG-INFO` & `g3tables-0.2.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g3tables
-Version: 0.2.3
+Version: 0.2.4
 Summary: G3 SW Definition, HW and PLC components, and Visualisation tables parser
 Author: Elektroline a.s.
 Project-URL: Homepage, https://gitlab.elektroline.cz/plc/systemg3-py/SystemG3Tables
 Keywords: Elektroline,Google Drive,Project table
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
```

### Comparing `g3tables-0.2.3/pyproject.toml` & `g3tables-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "g3tables"
-version = "0.2.3"
+version = "0.2.4"
 description = "G3 SW Definition, HW and PLC components, and Visualisation tables parser"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
   { name="Elektroline a.s." },
 ]
 classifiers = [
```

### Comparing `g3tables-0.2.3/src/g3tables/__init__.py` & `g3tables-0.2.4/src/g3tables/__init__.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.3/src/g3tables/plc_composition_io_table/_extend_table.py` & `g3tables-0.2.4/src/g3tables/plc_composition_io_table/_extend_table.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.3/src/g3tables/plc_composition_io_table/_table.py` & `g3tables-0.2.4/src/g3tables/plc_composition_io_table/_table.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.3/src/g3tables/plc_composition_io_table/io_signals.json` & `g3tables-0.2.4/src/g3tables/plc_composition_io_table/io_signals.json`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.3/src/g3tables/sw_definition_table/_table.py` & `g3tables-0.2.4/src/g3tables/sw_definition_table/_table.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.3/src/g3tables/system_config/_cli.py` & `g3tables-0.2.4/src/g3tables/system_config/_cli.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.3/src/g3tables/system_config/_g3core_updater.py` & `g3tables-0.2.4/src/g3tables/system_config/_g3core_updater.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.3/src/g3tables/system_config/_hw_connections.py` & `g3tables-0.2.4/src/g3tables/system_config/_hw_connections.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.3/src/g3tables/system_config/_iomap_updater.py` & `g3tables-0.2.4/src/g3tables/system_config/_iomap_updater.py`

 * *Files 22% similar despite different names*

```diff
@@ -33,14 +33,29 @@
             "inFromSafety": {
                 "UDINT": itertools.count(1),
                 "UINT": itertools.count(1)
             },
             "outToSafety": {
                 "UDINT": itertools.count(1001),
                 "UINT": itertools.count(1001)
+            },
+            "inAuthKey": {
+                "INT": itertools.count(1)
+            },
+            "inAuthBusy": {
+                "BOOL": itertools.count(1)
+            },
+            "inAuthResult": {
+                "BOOL": itertools.count(2)
+            },
+            "outAuthKey": {
+                "INT": itertools.count(1001)
+            },
+            "outAuthCmd": {
+                "INT": itertools.count(1002)
             }
         }
 
     def _update_iomap_device(
         self, device_data: SWDeviceDict, iomap_key: str
     ) -> None:
         if not self.iomap:
@@ -55,29 +70,45 @@
     def _generate_safety_hardware_mapping(self, var: STVariable) -> str:
         assert self.sl8101_name is not None
         match var.name, var.dtype:
             case 'inFromSafety', 'UINT':
                 prefix = '%IW'
             case 'inFromSafety', 'UDINT':
                 prefix = '%ID'
+            case 'inAuthKey', 'INT':
+                prefix = '%IW'
+            case 'inAuthBusy', 'BOOL':
+                prefix = '%IX'
+            case 'inAuthResult', 'BOOL':
+                prefix = '%IX'
+            case 'outAuthKey', 'INT':
+                prefix = '%QW'
+            case 'outAuthCmd', 'INT':
+                prefix = '%QW'
             case 'outToSafety', 'UINT':
                 prefix = '%QW'
             case 'outToSafety', 'UDINT':
                 prefix = '%QD'
             case _:
                 logger.warning(
                     'Unable to generate safety IO mapping for variable "%s" '
                     'of type "%s"', var.name, var.dtype
                     )
                 return ''
         counter = self._counters[var.name][var.dtype]
-        return (
-            f'{prefix}."{self.sl8101_name}".{var.dtype}'
-            f'{next(counter):04}'
-            )
+        if (var.name == "inAuthBusy") or (var.name == "inAuthResult") :
+            return (
+                f'{prefix}."{self.sl8101_name}".{var.dtype}'
+                f'{next(counter):05}'
+                )
+        else:
+            return (
+                f'{prefix}."{self.sl8101_name}".{var.dtype}'
+                f'{next(counter):04}'
+                )
 
     def _update_iomap_device_safety(
         self, device_type: str, device_data: SWDeviceDict
     ) -> None:
         device_name = self.wrapper.get_device_name(device_data)
         # get the control fb name
         fb_name = self.wrapper.get_device_control_fb(device_data)
@@ -144,14 +175,66 @@
                 if hardware_signal:
                     logger.info(
                         'Mapping %s "%s" "outToSafety" connector to "%s".',
                         device_type, device_name, hardware_signal
                         )
                     iomap_dict['outToSafety'] = hardware_signal
                     break
+        for var in control_fb.var_input:
+            if var.name == "inAuthKey":
+                hardware_signal = self._generate_safety_hardware_mapping(var)
+                if hardware_signal:
+                    logger.info(
+                        'Mapping %s "%s" "inAuthKey" connector to "%s".',
+                        device_type, device_name, hardware_signal
+                        )
+                    iomap_dict['inAuthKey'] = hardware_signal
+                    break 
+        for var in control_fb.var_input:
+            if var.name == "inAuthBusy":
+                hardware_signal = self._generate_safety_hardware_mapping(var)
+                print(hardware_signal)
+                if hardware_signal:
+                    logger.info(
+                        'Mapping %s "%s" "inAuthBusy" connector to "%s".',
+                        device_type, device_name, hardware_signal
+                        )
+                    iomap_dict['inAuthBusy'] = hardware_signal
+                    break        
+        for var in control_fb.var_input:
+            if var.name == "inAuthResult":
+                hardware_signal = self._generate_safety_hardware_mapping(var)
+                print(hardware_signal)
+                if hardware_signal:
+                    logger.info(
+                        'Mapping %s "%s" "inAuthResult" connector to "%s".',
+                        device_type, device_name, hardware_signal
+                        )
+                    iomap_dict['inAuthResult'] = hardware_signal
+                    break    
+        for var in control_fb.var_out:
+            if var.name == "outAuthKey":
+                hardware_signal = self._generate_safety_hardware_mapping(var)
+                if hardware_signal:
+                    logger.info(
+                        'Mapping %s "%s" "outAuthKey" connector to "%s".',
+                        device_type, device_name, hardware_signal
+                        )
+                    iomap_dict['outAuthKey'] = hardware_signal
+                    break    
+        for var in control_fb.var_out:
+            if var.name == "outAuthCmd":
+                hardware_signal = self._generate_safety_hardware_mapping(var)
+                if hardware_signal:
+                    logger.info(
+                        'Mapping %s "%s" "outAuthCmd" connector to "%s".',
+                        device_type, device_name, hardware_signal
+                        )
+                    iomap_dict['outAuthCmd'] = hardware_signal
+                    break    
 
     def _update_iomap_module(
         self,
         module_name: str,
         module_data: SWModuleDict,
         ignore: list[str] | None = None
     ) -> None:
@@ -191,14 +274,21 @@
                     self._update_iomap_device_safety(
                         ch_module_name, ch_device_data
                         )
 
     def update(self) -> None:
         for zone_name, zone_data in self.wrapper.system_dict.items():
             if zone_name == 'Common':  # nothing to update in the 'Common' data
+                for module_name, module_data in zone_data.items():
+                    if module_name == 'SystemSafety':
+                        self._update_iomap_module(
+                            module_name,
+                            module_data,
+                            ignore=self.EXCLUDED_FOR_SAFETY_IOMAP
+                            )
                 continue
             for module_name, module_data in zone_data.items():
                 if module_name == 'Cabinet':
                     self._update_iomap_module_cabinet(module_data)
                 else:
                     self._update_iomap_module(
                         module_name,
```

### Comparing `g3tables-0.2.3/src/g3tables/system_config/_sw_system_dict_wrapper.py` & `g3tables-0.2.4/src/g3tables/system_config/_sw_system_dict_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             ]
 
     def get_zone_taskname(self, zone_name: str) -> str:
         if len(self.system_dict.keys()) < 3:  # not a multizone
             taskname = "Zone"
         else:
             zone_data = self.system_dict[zone_name]['Zone'][zone_name]
-            varname = zone_data['general']['varname']
+            varname = zone_data['general']['name']
             taskname = varname[:self.ZONE_TASKNAME_MAXLEN].strip('_')
         return taskname
 
     def has_system_safety(self) -> bool:
         return bool(self.system_dict['Common'].get('SystemSafety'))
 
     def has_shv(self) -> bool:
```

### Comparing `g3tables-0.2.3/src/g3tables/system_config/_system_config_processor.py` & `g3tables-0.2.4/src/g3tables/system_config/_system_config_processor.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.3/src/g3tables/system_config/type_hinting.py` & `g3tables-0.2.4/src/g3tables/system_config/type_hinting.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.3/src/g3tables/utils/_d2nd.py` & `g3tables-0.2.4/src/g3tables/utils/_d2nd.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.3/src/g3tables/utils/_interval.py` & `g3tables-0.2.4/src/g3tables/utils/_interval.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.3/src/g3tables/utils/gdrive/_gdrive.py` & `g3tables-0.2.4/src/g3tables/utils/gdrive/_gdrive.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.3/src/g3tables/utils/gdrive/_update_creds.py` & `g3tables-0.2.4/src/g3tables/utils/gdrive/_update_creds.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.3/src/g3tables/visualization_table/_table.py` & `g3tables-0.2.4/src/g3tables/visualization_table/_table.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.3/src/g3tables.egg-info/PKG-INFO` & `g3tables-0.2.4/src/g3tables.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g3tables
-Version: 0.2.3
+Version: 0.2.4
 Summary: G3 SW Definition, HW and PLC components, and Visualisation tables parser
 Author: Elektroline a.s.
 Project-URL: Homepage, https://gitlab.elektroline.cz/plc/systemg3-py/SystemG3Tables
 Keywords: Elektroline,Google Drive,Project table
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
```

### Comparing `g3tables-0.2.3/src/g3tables.egg-info/SOURCES.txt` & `g3tables-0.2.4/src/g3tables.egg-info/SOURCES.txt`

 * *Files identical despite different names*

