# Comparing `tmp/medicafe-0.240513.4.tar.gz` & `tmp/medicafe-0.240515.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240513.4.tar", last modified: Mon May 13 15:48:04 2024, max compression
+gzip compressed data, was "medicafe-0.240515.5.tar", last modified: Thu May 16 01:38:55 2024, max compression
```

## Comparing `medicafe-0.240513.4.tar` & `medicafe-0.240515.5.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 15:48:04.277000 medicafe-0.240513.4/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240513.4/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240513.4/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-13 15:48:03.506000 medicafe-0.240513.4/MediBot/
--rwxrwxrwx   0        0        0     5972 2024-05-12 18:02:44.000000 medicafe-0.240513.4/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    17343 2024-05-12 16:32:17.000000 medicafe-0.240513.4/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240513.4/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    33980 2024-05-12 16:14:26.000000 medicafe-0.240513.4/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4589 2024-05-12 17:14:28.000000 medicafe-0.240513.4/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240513.4/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     8636 2024-05-12 16:11:39.000000 medicafe-0.240513.4/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240513.4/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240513.4/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240513.4/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240513.4/MediBot/update_json.py
--rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240513.4/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-13 15:48:04.069000 medicafe-0.240513.4/MediLink/
--rw-rw-rw-   0        0        0    20170 2024-05-13 15:47:08.000000 medicafe-0.240513.4/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240513.4/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    26271 2024-05-13 14:06:59.000000 medicafe-0.240513.4/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    39431 2024-05-13 14:41:19.000000 medicafe-0.240513.4/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240513.4/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    11857 2024-05-12 18:32:20.000000 medicafe-0.240513.4/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240513.4/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240513.4/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240513.4/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240513.4/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240513.4/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240513.4/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0    19252 2024-05-13 14:56:52.000000 medicafe-0.240513.4/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240513.4/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240513.4/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240513.4/MediLink/__init__.py
--rw-rw-rw-   0        0        0     3108 2024-05-13 04:52:22.000000 medicafe-0.240513.4/MediLink/test.py
--rw-rw-rw-   0        0        0     4396 2024-05-13 15:48:04.259000 medicafe-0.240513.4/PKG-INFO
--rw-rw-rw-   0        0        0     2960 2024-05-13 07:31:39.000000 medicafe-0.240513.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 15:48:04.240000 medicafe-0.240513.4/medicafe.egg-info/
--rw-rw-rw-   0        0        0     4396 2024-05-13 15:48:02.000000 medicafe-0.240513.4/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1023 2024-05-13 15:48:02.000000 medicafe-0.240513.4/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 15:48:02.000000 medicafe-0.240513.4/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240513.4/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-13 15:48:02.000000 medicafe-0.240513.4/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-13 15:48:02.000000 medicafe-0.240513.4/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 15:48:04.272000 medicafe-0.240513.4/setup.cfg
--rw-rw-rw-   0        0        0     4834 2024-05-13 15:48:01.000000 medicafe-0.240513.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 01:38:55.685000 medicafe-0.240515.5/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240515.5/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240515.5/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-16 01:38:54.728000 medicafe-0.240515.5/MediBot/
+-rwxrwxrwx   0        0        0     5972 2024-05-12 18:02:44.000000 medicafe-0.240515.5/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    17490 2024-05-15 17:01:43.000000 medicafe-0.240515.5/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240515.5/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    14538 2024-05-15 19:07:33.000000 medicafe-0.240515.5/MediBot/MediBot_Crosswalk_Library.py
+-rw-rw-rw-   0        0        0    14906 2024-05-15 16:48:28.000000 medicafe-0.240515.5/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0    17184 2024-05-15 17:38:32.000000 medicafe-0.240515.5/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10660 2024-05-16 01:23:48.000000 medicafe-0.240515.5/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     8912 2024-05-15 20:14:35.000000 medicafe-0.240515.5/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240515.5/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240515.5/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240515.5/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240515.5/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240515.5/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-16 01:38:55.434000 medicafe-0.240515.5/MediLink/
+-rw-rw-rw-   0        0        0    20316 2024-05-16 01:29:43.000000 medicafe-0.240515.5/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240515.5/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    25526 2024-05-16 00:37:08.000000 medicafe-0.240515.5/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    43551 2024-05-16 00:36:51.000000 medicafe-0.240515.5/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     6166 2024-05-15 17:49:28.000000 medicafe-0.240515.5/MediLink/MediLink_APIs.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240515.5/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    12235 2024-05-14 15:14:04.000000 medicafe-0.240515.5/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7248 2024-05-15 07:47:12.000000 medicafe-0.240515.5/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8710 2024-05-15 13:36:03.000000 medicafe-0.240515.5/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240515.5/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0      370 2024-05-14 22:24:45.000000 medicafe-0.240515.5/MediLink/MediLink_Mailer.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240515.5/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240515.5/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240515.5/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0    19286 2024-05-16 01:21:31.000000 medicafe-0.240515.5/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240515.5/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240515.5/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240515.5/MediLink/__init__.py
+-rw-rw-rw-   0        0        0     3108 2024-05-13 04:52:22.000000 medicafe-0.240515.5/MediLink/test.py
+-rw-rw-rw-   0        0        0     4396 2024-05-16 01:38:55.664000 medicafe-0.240515.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2960 2024-05-13 07:31:39.000000 medicafe-0.240515.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 01:38:55.641000 medicafe-0.240515.5/medicafe.egg-info/
+-rw-rw-rw-   0        0        0     4396 2024-05-16 01:38:53.000000 medicafe-0.240515.5/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1114 2024-05-16 01:38:54.000000 medicafe-0.240515.5/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 01:38:53.000000 medicafe-0.240515.5/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240515.5/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-16 01:38:53.000000 medicafe-0.240515.5/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-16 01:38:53.000000 medicafe-0.240515.5/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 01:38:55.680000 medicafe-0.240515.5/setup.cfg
+-rw-rw-rw-   0        0        0     4834 2024-05-16 01:38:52.000000 medicafe-0.240515.5/setup.py
```

### Comparing `medicafe-0.240513.4/LICENSE` & `medicafe-0.240515.5/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.4/MediBot/MediBot.bat` & `medicafe-0.240515.5/MediBot/MediBot.bat`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.4/MediBot/MediBot.py` & `medicafe-0.240515.5/MediBot/MediBot.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,25 +2,30 @@
 import os
 import tempfile
 import traceback
 import re  #for addresses
 from collections import OrderedDict
 import MediBot_dataformat_library
 import MediBot_Preprocessor
-from MediBot_Preprocessor import initialize, AHK_EXECUTABLE, CSV_FILE_PATH, field_mapping
-import MediBot_Preprocessor_lib
+from MediBot_Preprocessor_lib import initialize, AHK_EXECUTABLE, CSV_FILE_PATH, field_mapping, load_csv_data
 from MediBot_UI import app_control, manage_script_pause, user_interaction
 
 # Add parent directory of the project to the Python path
 import sys
 project_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
 sys.path.append(project_dir)
 
 from MediLink import MediLink_ConfigLoader
 
+try:
+    from MediBot_Crosswalk_Library import crosswalk_update
+except ImportError:
+    from MediBot import MediBot_Crosswalk_Library
+    crosswalk_update = MediBot_Crosswalk_Library.crosswalk_update
+
 """
 # Development Task List for MediBot
 
 Error Handling Improvements
 - [ ] Its really difficult to get out of the main menu if you go open MediBot by accident
 - [ ] Develop a centralized error handling and logging mechanism for improved troubleshooting.
 - [ ] Implement validation checks during patient data entry to prevent submission of incomplete or incorrect records.
@@ -207,15 +212,15 @@
         try:
             config, crosswalk = MediLink_ConfigLoader.load_configuration(config_path, crosswalk_path)
             self.verify_config_type(config)
             self.crosswalk = crosswalk
             self.config = config
             MediLink_ConfigLoader.log("Config loaded successfully...")
             
-            MediBot_Preprocessor.crosswalk_update(config, crosswalk)
+            crosswalk_update(config, crosswalk)
             MediLink_ConfigLoader.log("Crosswalk update complete...")
             
             initialize(config)
             MediLink_ConfigLoader.log("Constants initialized...")
             
         except Exception as e:
             print("Failed to load or update configuration: {}".format(e))
@@ -243,15 +248,15 @@
             # If no arguments are provided, use default paths
             config_path = default_config_path
             crosswalk_path = default_crosswalk_path
         
         e_state = ExecutionState(config_path, crosswalk_path)
         
         MediLink_ConfigLoader.log("Loading CSV Data...")
-        csv_data = MediBot_Preprocessor_lib.load_csv_data(CSV_FILE_PATH)
+        csv_data = load_csv_data(CSV_FILE_PATH)
         
         # Pre-process CSV data to add combined fields & crosswalk values.
         MediLink_ConfigLoader.log("Pre-processing CSV Data...")
         MediBot_Preprocessor.preprocess_csv_data(csv_data, e_state.crosswalk)  
         headers = csv_data[0].keys() # Make sure all the headers are in place
         
         MediLink_ConfigLoader.log("Performing Intake Scan...")
```

### Comparing `medicafe-0.240513.4/MediBot/MediBot_Charges.py` & `medicafe-0.240515.5/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.4/MediBot/MediBot_UI.py` & `medicafe-0.240515.5/MediBot/MediBot_UI.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
             patient_id_header = reverse_mapping['Patient ID #2']
             patient_name_header = reverse_mapping['Patient Name']
             patient_id = row.get(patient_id_header, "N/A")
             patient_name = row.get(patient_name_header, "Unknown")
             surgery_date = row.get('Surgery Date', "Unknown Date")  # Access 'Surgery Date' as string directly from the row
             
-            print("{0:02d}: {3:.5s} (ID: {2}) {1} ".format(index+1, patient_name, patient_id, surgery_date))
+            print("{0:03d}: {3:.5s} (ID: {2}) {1} ".format(index+1, patient_name, patient_id, surgery_date))
 
             displayed_indices.append(index)
             displayed_patient_ids.append(patient_id)
 
         return displayed_indices, displayed_patient_ids
 
     if proceed_as_medicare:
```

### Comparing `medicafe-0.240513.4/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240515.5/MediBot/MediBot_dataformat_library.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 try: 
     from MediLink import MediLink_ConfigLoader
     config, crosswalk = MediLink_ConfigLoader.load_configuration()
 except ImportError:
     from MediLink_ConfigLoader import load_configuration
     config, crosswalk = load_configuration()
 
-from MediBot_Preprocessor import initialize
-from MediBot_Preprocessor_lib import open_csv_for_editing
+from MediBot_Preprocessor_lib import open_csv_for_editing, initialize
 from MediBot_UI import manage_script_pause, app_control
 
+
 """
 - [X] (TEST) Address Formatting 30-character Limit:
     (LOW) Address the issue where the format_street function in Medibot may produce addresses exceeding
     the 30-character limit. Current stop-gap is removing period characters and the abbreviation "APT" 
     surrounded by spaces from all records as a temporary solution. 
     If the address still exceeds 30 characters, the function will attempt to remove spaces from right to left
     until it reaches 30 significant digits or runs out of spaces, then truncate to 30 characters if necessary.
@@ -67,42 +67,49 @@
     return alphanumeric
 
 def format_gender(value):
     return value[0].upper()
 
 def enforce_significant_length(output):
     # Replace spaces with a placeholder that counts as one significant digit
-    temp_output = output.replace(' ', '{Space}')
+    temp_output = output.replace('{Space}', ' ')
     
     # Check if the number of significant digits exceeds 30
     if len(temp_output) > 30:
+        
         # First line of defense: Replace ' APT ' with ' #' if the original length is longer than 30 characters.
         temp_output = temp_output.replace(' APT ', ' #')
-
-        # Remove spaces from right to left until we reach 30 significant digits or run out of spaces
-        while len(temp_output) > 30 and ' ' in temp_output:
-            temp_output = temp_output.rstrip(' ')
         
+        # Remove spaces in a controlled manner from right to left if still too long
+        while len(temp_output) > 30:
+            # Find the last space
+            last_space_index = temp_output.rfind(' ')
+            if last_space_index == -1:
+                break
+            # Remove the last space
+            temp_output = temp_output[:last_space_index] + temp_output[last_space_index+7:]
+
         # If still greater than 30, truncate to 30 characters
         if len(temp_output) > 30:
             temp_output = temp_output[:30]
-    
+
     # Replace placeholder back with actual space for final return
-    return temp_output.replace('{Space}', ' ')
+    return temp_output.replace(' ', '{Space}')
 
 def format_street(value, csv_data, reverse_mapping, parsed_address_components):
     # Temporarily disable script pause status
     app_control.set_pause_status(False)
     
-    # Remove period characters and the abbreviation "APT" surrounded by spaces from the input
+    # Remove period characters.
     value = value.replace('.', '')
     
     # Proceed only if there's a comma, indicating a likely full address
     if ',' in value:
         try:
+            MediLink_ConfigLoader.log("Attempting to resolve address via regex...")
             # Retrieve common city names from configuration and prepare a regex pattern
             common_cities = config.get('cities', [])
             city_pattern = '|'.join(re.escape(city) for city in common_cities)
             city_regex_pattern = r'(?P<City>{})'.format(city_pattern)
             city_regex = re.compile(city_regex_pattern, re.IGNORECASE)
 
             # Search for a common city in the address
@@ -143,15 +150,17 @@
             app_control.set_pause_status(True)
             open_csv_for_editing(CSV_FILE_PATH)
             manage_script_pause(csv_data, e, reverse_mapping)
             # Return original value with spaces formatted, enforcing significant length
             return enforce_significant_length(value.replace(' ', '{Space}'))
     else:
         # If no comma is present, treat the input as a simple street name
-        return enforce_significant_length(value.replace(' ', '{Space}'))
+        formatted_value = value.replace(' ', '{Space}')
+        enforced_format = enforce_significant_length(formatted_value)
+        return enforced_format
 
     # Fallback return in case no address components are matched even though a comma was present
     return enforce_significant_length(value.replace(' ', '{Space}')) 
 
 def format_zip(value):
     # Ensure the value is a string, in case it's provided as an integer
     value_str = str(value)
```

### Comparing `medicafe-0.240513.4/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240515.5/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.4/MediBot/update_json.py` & `medicafe-0.240515.5/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.4/MediBot/update_medicafe.py` & `medicafe-0.240515.5/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.4/MediLink/MediLink.py` & `medicafe-0.240515.5/MediLink/MediLink.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-
 import MediLink_Down
 import MediLink_Up
 import MediLink_ConfigLoader
 import MediLink_837p_encoder
 
 # For UI Functions
 import os
@@ -11,16 +10,17 @@
 from tqdm import tqdm
 
 # Add parent directory of the project to the Python path
 import sys
 project_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
 sys.path.append(project_dir)
 
-from MediBot.MediBot_Preprocessor import load_insurance_data_from_mains
-
+from MediBot import MediBot_Preprocessor_lib
+load_insurance_data_from_mains = MediBot_Preprocessor_lib.load_insurance_data_from_mains
+from MediBot import MediBot_Crosswalk_Library
 
 """
 Development Tasks for Backend Enhancement in MediSoft Claims Submittal (MediLink) Script:
 
 Implement dynamic configurations for multiple endpoints (Availity, Optum, PNT Data) with environmental settings support.
 Enhance file detection with detailed logging and introduce integrity checks for pre-processing validation.
 Verify file transmissions via WinSCP log analysis for successful endpoint acknowledgments and secure data transfer.
@@ -123,16 +123,16 @@
     """
     detailed_patient_data = []
     
     # Load insurance data from MAINS to create a mapping from insurance names to their respective IDs
     insurance_to_id = load_insurance_data_from_mains(config)
     MediLink_ConfigLoader.log("Insurance data loaded from MAINS. {} insurance providers found.".format(len(insurance_to_id)))
 
-    for personal_info, insurance_info, service_info in MediLink_837p_encoder.read_fixed_width_data(file_path, config.get('MediLink_Config', {})):
-        parsed_data = MediLink_837p_encoder.parse_fixed_width_data(personal_info, insurance_info, service_info, config.get('MediLink_Config', {}))
+    for personal_info, insurance_info, service_info in MediLink_837p_encoder.read_fixed_width_data(file_path):
+        parsed_data = MediLink_837p_encoder.parse_fixed_width_data(personal_info, insurance_info, service_info, config.get('MediLink_Config', config))
         
         primary_insurance = parsed_data.get('INAME')
         
         # Retrieve the insurance ID associated with the primary insurance
         insurance_id = insurance_to_id.get(primary_insurance)
         MediLink_ConfigLoader.log("Primary insurance ID retrieved for '{}': {}".format(primary_insurance, insurance_id))
 
@@ -305,19 +305,21 @@
 def main_menu():
     """
     Initializes the main menu loop and handles the overall program flow,
     including loading configurations and managing user input for menu selections.
     """
     # Load configuration settings and display the initial welcome message.
     config, crosswalk = MediLink_ConfigLoader.load_configuration() 
-    # BUG (Low, Config) does this need an argument? Not sure.
     
-    # TODO (Test Mode) Add here a check in config.json for key "MediLink_Config": { "TestMode": true, ...}. If it is true,
-    # prompt the user to say that MediLink is in Test Mode and ask if the user wants to stay in test mode? 
-    # Then put placeholder text for now because I don't know what the logic should be.
+    # Check to make sure payer_id key is available in crosswalk, otherwise, go through that crosswalk initialization flow
+    MediBot_Crosswalk_Library.check_and_initialize_crosswalk(config)
+    
+    # Check if the application is in test mode
+    if config.get("MediLink_Config", {}).get("TestMode", False):
+        print("\n--- MEDILINK TEST MODE --- \nTo enable full functionality, please update the config file \nand set 'TestMode' to 'false'.")
     
     # Display Welcome Message
     MediLink_UI.display_welcome()
 
     # Normalize the directory path for file operations.
     directory_path = os.path.normpath(config['MediLink_Config']['inputFilePath'])
```

### Comparing `medicafe-0.240513.4/MediLink/MediLink_277_decoder.py` & `medicafe-0.240515.5/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.4/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240515.5/MediLink/MediLink_837p_encoder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import re
 from datetime import datetime
 import argparse
 import os
-import sys
 import MediLink_ConfigLoader
 from MediLink_DataMgmt import parse_fixed_width_data, read_fixed_width_data
 import MediLink_837p_encoder_library
 #from tqdm import tqdm
 
 """
 Single File Processing Flow:
@@ -28,64 +27,39 @@
 - [ ] 3. Validation and Logging: Strengthen validation processes for input data, incorporating thorough checks against business rules and enhanced detailed logging for improved traceability and troubleshooting.
 - [ ] 4. Batch Processing and Output Handling: Enhance output file management to support efficient batch operations, including systematic naming and organization for output files.
 - [ ] 5. Comprehensive Documentation: Maintain up-to-date and detailed documentation within the codebase, ensuring all functions and complex logic are clearly explained.
 - [ ] 6. De-persisting Intermediate Files.
 - [ ] 7. Determination of Relationship to Patient for insurance holder. Can Compare Insured Name & closeness of DOB (usually spouse [2], child [3]). 
 - [ ] 8. Consolidation of certain functions needs to happen here.
 """
-def create_interchange_elements(config, endpoint, transaction_set_control_number):
-    """
-    Create interchange headers and trailers for an 837P document.
-
-    Parameters:
-    - config: Configuration settings loaded from a JSON file.
-    - endpoint: The endpoint for which the data is being processed.
-    - transaction_set_control_number: The starting transaction set control number.
-
-    Returns:
-    - Tuple containing (ISA header, GS header, GE trailer, IEA trailer).
-    """
-    endpoint_config = config['endpoints'].get(endpoint.upper(), {})
-    
-    # Get the current system time and format it as 'HHMMSS' in 24-hour clock.
-    current_time = datetime.now().strftime('%H%M%S')
-    isa13 = '000' + current_time  # Format ISA13 with '000HHMMSS'.
-
-    # Check if isa13 could not be generated from the current time
-    if len(isa13) != 9:
-        # If isa13 cannot be generated from the current time, use the configured value.
-        isa13 = endpoint_config.get('isa_13_value', '000000001')
-    
-    # Create interchange header and trailer using provided library functions.
-    isa_header, gs_header = MediLink_837p_encoder_library.create_interchange_header(config, endpoint, isa13)
-    ge_trailer, iea_trailer = MediLink_837p_encoder_library.create_interchange_trailer(config, transaction_set_control_number, isa13)
-    
-    return isa_header, gs_header, ge_trailer, iea_trailer
 
 def format_single_claim(patient_data, config, endpoint, transaction_set_control_number):
     """
     Formats a single claim into 837P segments based on the provided patient data and endpoint.
     
     Parameters:
     - patient_data: Dictionary containing detailed patient data.
     - config: Configuration settings loaded from a JSON file.
     - endpoint: The endpoint key representing the specific endpoint.
     - transaction_set_control_number: Starting transaction set control number for 837P segments.
     
     Returns:
     - String representation of the formatted 837P claim.
     """
+    # Pre-resolve and enrich with Payer Name and ID for special case handling like Florida Blue.
+    patient_data = MediLink_837p_encoder_library.payer_id_to_payer_name(patient_data, config, endpoint)
+    
     segments = []
         
     # Initialize with standard segments for all claims
     segments.append(MediLink_837p_encoder_library.create_st_segment(transaction_set_control_number))
     segments.append(MediLink_837p_encoder_library.create_bht_segment(patient_data))
 
     # Submitter Name Segment and PER Contact Information (1000A Loop)
-    segments.extend(MediLink_837p_encoder_library.create_1000A_submitter_name_segment(config, endpoint))
+    segments.extend(MediLink_837p_encoder_library.create_1000A_submitter_name_segment(patient_data, config, endpoint))
     
     # Receiver Name Segment (1000B Loop)
     segments.extend([MediLink_837p_encoder_library.create_1000B_receiver_name_segment(config, endpoint)])
     
     # Billing Provider Segments (2010AA Loop)
     segments.extend([MediLink_837p_encoder_library.create_hl_billing_provider_segment()])
     segments.extend(MediLink_837p_encoder_library.create_nm1_billing_provider_segment(config, endpoint))
@@ -103,15 +77,15 @@
     segments.extend(MediLink_837p_encoder_library.create_subscriber_address_segments(patient_data))
     segments.append(MediLink_837p_encoder_library.create_dmg_segment(patient_data))
     
     # Payer information (2010BB loop)
     # TODO This function now includes detailed outputs and potential user interactions with the new implementation.
     # The new implementation introduces user inputs directly in the flow, which could disrupt automated batch processes. 
     # Ensure that there are mechanisms or workflows in place to handle such interruptions appropriately.
-    segments.extend([MediLink_837p_encoder_library.create_2010BB_payer_information_segment(patient_data, config, endpoint)])
+    segments.extend([MediLink_837p_encoder_library.create_2010BB_payer_information_segment(patient_data)])
     #segments.extend(MediLink_837p_encoder_library.create_payer_address_segments(config)) OMITTED
     
     # Rendering Provider (2310B Loop)
     segments.extend(MediLink_837p_encoder_library.create_nm1_rendering_provider_segment(config))
     
     # Claim information 2300, 2310C Service Facility and 2400 loop segments
     segments.extend(MediLink_837p_encoder_library.create_clm_and_related_segments(patient_data, config))
@@ -124,17 +98,14 @@
 
     # Optionally, print or log the formatted 837P for debugging or verification
     # TODO (Low UI/usability) Add chart number to this.
     MediLink_ConfigLoader.log("Formatted 837P for endpoint {}.".format(endpoint), config, level="INFO")
 
     return formatted_837p
 
-import os
-from datetime import datetime
-
 def write_output_file(document_segments, output_directory, endpoint_key, input_file_path, config):
     """
     Writes formatted 837P document segments to an output file with a dynamically generated name.
     
     Development Roadmap:
     - Ensure input `document_segments` is a non-empty list to avoid creating empty files.
     - Verify `output_directory` exists and is writable before proceeding. Create the directory if it does not exist.
@@ -182,177 +153,95 @@
         return new_output_file_path
     except Exception as e:
         MediLink_ConfigLoader.log("Error: Failed to write output file. {}".format(e), config, level="ERROR")
         return None
 
 def process_file(file_path, config, endpoint_key, transaction_set_control_number):
     """
-    Reads, validates, and formats claim data from a given file into the 837P format.
+    Process the claim data from a file into the 837P format.
 
-    :param file_path: The path to the file containing claim data.
-    :param config: Configuration settings loaded from a JSON file.
-    :param endpoint_key: The key representing the endpoint for which the claim is being processed.
-    :param transaction_set_control_number: The starting transaction set control number for 837P segments.
-    :return: A tuple containing the formatted claim segments and the next transaction set control number.
+    Args:
+        file_path (str): The path to the file containing the claim data.
+        config (dict): Configuration settings loaded from a JSON file.
+        endpoint_key (str): The key representing the endpoint for which the claim is being processed.
+        transaction_set_control_number (int): The starting transaction set control number for 837P segments.
+
+    Returns:
+        tuple: A tuple containing the formatted claim segments and the next transaction set control number.
     """
-    formatted_claims = []
+    valid_claims, validation_errors = read_and_validate_claims(file_path, config)
     
-    for personal_info, insurance_info, service_info in read_fixed_width_data(file_path, config):
-        parsed_data = parse_fixed_width_data(personal_info, insurance_info, service_info, config)
-        
-        # Re-enable validation using validate_claim_data
-        is_valid, validation_errors = validate_claim_data(parsed_data, config)
-        if not is_valid:
-            MediLink_ConfigLoader.log("Validation failed for claim data in file: {}. Errors: {}".format(file_path, validation_errors), config, level="ERROR")
-            continue  # Skip invalid claims
-        
-        formatted_claim = format_single_claim(parsed_data, config, endpoint_key, transaction_set_control_number)
-        formatted_claims.append(formatted_claim)
-        transaction_set_control_number += 1  # Increment for each successfully processed claim
+    # Handle validation errors
+    if validation_errors:
+        if not MediLink_837p_encoder_library.handle_validation_errors(transaction_set_control_number, validation_errors, config):
+            return None, transaction_set_control_number  # Halt processing if the user chooses
+
+    # Process each valid claim
+    formatted_claims, transaction_set_control_number = format_claims(valid_claims, config, endpoint_key, transaction_set_control_number)
 
-    formatted_claims_str = '\n'.join(formatted_claims)
+    formatted_claims_str = '\n'.join(formatted_claims)  # Join formatted claims into a single string
     return formatted_claims_str, transaction_set_control_number
 
-def winscp_validate_output_directory(output_directory):
+def read_and_validate_claims(file_path, config):
     """
-    Validates the output directory path to ensure it has no spaces.
-    If spaces are found, prompts the user to input a new path.
-    If the directory doesn't exist, creates it.
-    """
-    while ' ' in output_directory:
-        print("\nWARNING: The output directory path contains spaces, which can cause issues with upload operations.")
-        print("    Current proposed path: {}".format(output_directory))
-        new_path = input("Please enter a new path for the output directory: ")
-        output_directory = new_path.strip()  # Remove leading/trailing spaces
-    
-    # Check if the directory exists, if not, create it
-    if not os.path.exists(output_directory):
-        os.makedirs(output_directory)
-        print("INFO: Created output directory: {}".format(output_directory))
-    
-    return output_directory
+    Read and validate claim data from a file.
 
-def convert_files_for_submission(detailed_patient_data, config):
-    """    
-    Processes detailed patient data for submission based on their confirmed endpoints,
-    generating a separate 837P file for each endpoint.
-
-    Parameters:
-    - detailed_patient_data: A list containing detailed patient data with endpoint information.
-    - config: Configuration settings loaded from a JSON file.
+    Args:
+        file_path (str): The path to the file containing the claim data.
+        config (dict): Configuration settings loaded from a JSON file.
 
     Returns:
-    - A list of paths to the converted files ready for submission.
+        tuple: A tuple containing a list of valid parsed data and a list of validation errors.
     """
+    valid_claims = []  # List to store valid parsed data
+    validation_errors = []  # List to store validation errors
 
-    # Initialize a dictionary to hold patient data segregated by confirmed endpoints
-    data_by_endpoint = {}
-        
-    # Populate the dictionary with patient data
-    for data in detailed_patient_data:
-        endpoint = data['confirmed_endpoint']
-        if endpoint not in data_by_endpoint:
-            data_by_endpoint[endpoint] = []
-        data_by_endpoint[endpoint].append(data)
-
-    # List to store paths of converted files for each endpoint
-    converted_files_paths = []
+    # Iterate over data in the file
+    for personal_info, insurance_info, service_info in read_fixed_width_data(file_path):
+        # Parse data into a usable format
+        parsed_data = parse_fixed_width_data(personal_info, insurance_info, service_info, config.get('MediLink_Config', config))
+        # Validate the parsed data
+        is_valid, errors = validate_claim_data(parsed_data, config)
+        if is_valid:
+            valid_claims.append(parsed_data)  # Add valid data to the list
+        else:
+            validation_errors.append(errors)  # Add validation errors to the list
+            # Log validation failure
+            MediLink_ConfigLoader.log("Validation failed for claim data in file: {}. Errors: {}".format(file_path, errors), config, level="ERROR")
 
-    # Determine the total number of unique endpoints for progress bar
-    # total_endpoints = len(data_by_endpoint)
+    return valid_claims, validation_errors
 
-    # Iterate over each endpoint and process its corresponding patient data
-    for endpoint, patient_data_list in data_by_endpoint.items():
-        # tqdm(data_by_endpoint.items(), desc="Creating 837p(s)", total=total_endpoints, ascii=True)
-        # Each endpoint might have multiple patients' data to be processed into a single 837P file
-        if patient_data_list:
-            converted_path = process_claim(config['MediLink_Config'], endpoint, patient_data_list)
-            if converted_path:
-                converted_files_paths.append(converted_path)
-        
-    return converted_files_paths
-
-def process_claim(config, endpoint, patient_data_list):
+def format_claims(parsed_data_list, config, endpoint, starting_transaction_set_control_number):
     """
-    Processes patient data for a specified endpoint, converting it into the 837P format.
-    Generates a separate 837P file for each endpoint based on detailed patient data.
+    Formats a list of parsed claim data into 837P segments.
 
     Parameters:
+    - parsed_data_list: List of dictionaries containing parsed claim data.
     - config: Configuration settings loaded from a JSON file.
-    - endpoint_key: The key representing the endpoint for which the data is being processed.
-    - patient_data_list: A list of dictionaries, each containing detailed patient data.
+    - endpoint: The endpoint key representing the specific endpoint.
+    - starting_transaction_set_control_number: Starting transaction set control number for 837P segments.
 
     Returns:
-    - Path to the converted file, or None if an error occurs.
-    
-    TODO (LOW) Why are there duplicated interchange flows? Because the arg if we're doing a .dat directory or not. 
-    Although, that shouldn't be making duplicates of these interchange headers. That's still confusing and could end up making 
-    duplicate interchange headers because processing .dat in batch might be fast enough to be a problem.
+    - A list of formatted 837P claims and the next transaction set control number.
     """
-    # Retrieve endpoint-specific configuration
-    endpoint_config = config['endpoints'].get(endpoint)
-    if not endpoint_config:
-        print("Endpoint configuration for {} not found.".format(endpoint))
-        return None
-
-    # Retrieve desired default output file path from config
-    output_directory = config.get('outputFilePath', '')
-    
-    # BUG (Low SFTP) This is a WinSCP validation because of the mishandling of spaces in paths. 
-    # This shouldn't need to exist.
-    output_directory = winscp_validate_output_directory(output_directory)
-    
-    if not os.path.isdir(output_directory):
-        print("Output directory does not exist. Please check the configuration.")
-        return None
-
-    # Initialize the transaction set control number and document segments
-    transaction_set_control_number = 1
-    document_segments = []
-
-    # Process each patient's data in the list
-    for patient_data in patient_data_list:
-        # Validate each patient's data
-        is_valid, validation_errors = validate_claim_data(patient_data, config)
-        if is_valid:
-            # Format the claim if data is valid
-            formatted_claim = format_single_claim(patient_data, config, endpoint, transaction_set_control_number)
-            document_segments.append(formatted_claim)
-            transaction_set_control_number += 1
-        else:
-            # Log validation errors
-            for error in validation_errors:
-                MediLink_ConfigLoader.log("Validation error for transaction set {}: {}".format(transaction_set_control_number, error), config, level="WARNING")
-            
-            # Prompt user for input on how to proceed
-            print("Validation errors encountered for transaction set {}. Errors: {}".format(transaction_set_control_number, validation_errors))
-            user_input = input("Skip this patient and continue without incrementing transaction set number? (yes/no): ")
-            if user_input.lower() == 'yes':
-                print("Skipping patient...")
-                MediLink_ConfigLoader.log("Skipped processing of transaction set {} due to user decision.".format(transaction_set_control_number), config, level="INFO")
-                continue  # Skip the current patient and do not increment the transaction set number
-            else:
-                print("Processing halted due to validation errors.")
-                MediLink_ConfigLoader.log("Processing halted at transaction set {} due to unresolved validation errors.".format(transaction_set_control_number), config, level="ERROR")
-                sys.exit()  # Optionally halt further processing
-
-    # Create interchange elements with the final transaction set control number
-    isa_header, gs_header, ge_trailer, iea_trailer = create_interchange_elements(config, endpoint, transaction_set_control_number - 1)
+    formatted_claims = []
+    transaction_set_control_number = starting_transaction_set_control_number
 
-    # Insert headers at the beginning and append trailers at the end of document segments
-    document_segments.insert(0, gs_header)
-    document_segments.insert(0, isa_header)
-    document_segments.extend([ge_trailer, iea_trailer])
+    for parsed_data in parsed_data_list:
+        formatted_claim = format_single_claim(parsed_data, config, endpoint, transaction_set_control_number)
+        formatted_claims.append(formatted_claim)
+        transaction_set_control_number += 1  # Increment for each successfully processed claim
 
-    # Write the complete 837P document to an output file and return its path
-    return write_output_file(document_segments, output_directory, endpoint, patient_data_list[0]['file_path'], config)
+    return formatted_claims, transaction_set_control_number
 
 # Validation Function checks the completeness and correctness of each claim's data
 def validate_claim_data(parsed_data, config, required_fields=[]):
     """
+    Used by both paths. 
+    
     Validates the completeness and correctness of each claim's data based on configurable requirements.
 
     Parameters:
     - parsed_data: Dictionary containing claim data to validate.
     - config: Configuration settings loaded from a JSON file.
     - required_fields: Optional list of tuples indicating required fields and their respective regex patterns for validation.
 
@@ -370,14 +259,15 @@
             ('DATE', r'^\d{8}$'),
             ('AMOUNT', None),
             ('TOS', None),
             ('DIAG', None)
         ]
     """    
     errors = []
+    MediLink_ConfigLoader.log("Starting claim vata validation...")
     if not required_fields:
         # If no required fields are specified, assume validation is true
         return True, []
     
     expected_keys = {field[0] for field in required_fields}  # Set of expected field keys
     received_keys = set(parsed_data.keys())  # Set of keys present in the parsed data
 
@@ -411,15 +301,43 @@
     if errors:
         for error in errors:
             MediLink_ConfigLoader.log(error, config, level="ERROR")
         return False, errors
 
     return True, []
 
-if __name__ == "__main__":
+def process_and_write_file(file_path, config, endpoint, starting_tscn=1):
+    """        
+    Process a single file, create complete 837P document with headers and trailers, and write to output file.
+
+    Parameters:
+    - file_path: Path to the .DAT file to be processed.
+    - config: Configuration settings.
+    - endpoint: Endpoint key.
+    - starting_tscn: Starting Transaction Set Control Number.
+    """
+    print("Processing: {}".format(file_path))
+    MediLink_ConfigLoader.log("Processing: {}".format(file_path))
+    formatted_data, transaction_set_control_number = process_file(file_path, config, endpoint, starting_tscn)
+    isa_header, gs_header, ge_trailer, iea_trailer = MediLink_837p_encoder_library.create_interchange_elements(config, endpoint, transaction_set_control_number - 1)
+    
+    # Combine everything into a single document
+    complete_document = "{}\n{}\n{}\n{}\n{}".format(
+        isa_header,
+        gs_header,
+        formatted_data,
+        ge_trailer,            
+        iea_trailer
+    )
+    
+    # Write to output file
+    output_file_path = write_output_file([complete_document], config.get('outputFilePath', ''), endpoint, file_path, config)
+    print("File processed. Output saved to: {}".format(output_file_path))
+
+def main():
     """
     Converts fixed-width files to 837P format for health claim submissions.
 
     Usage:
     ------
     1. Convert a single file:
         python MediLink_837p_encoder.py -e [endpoint] -p [file_path]
@@ -455,48 +373,130 @@
         action='store_true',
         help="Flag indicating the path provided is a directory. If set, all .DAT files within the directory will be processed."
     )
     args = parser.parse_args()
 
     print("Starting the conversion process for {}. Processing {} at '{}'.".format(args.endpoint, 'directory' if args.is_directory else 'file', args.path))
 
-    # Load configuration
     config, _ = MediLink_ConfigLoader.load_configuration()
+    config = config.get('MediLink_Config', config)
     
-    def process_and_write_file(file_path, config, endpoint, starting_tscn=1):
-        """        
-        Process a single file, create complete 837P document with headers and trailers, and write to output file.
-
-        Parameters:
-        - file_path: Path to the .DAT file to be processed.
-        - config: Configuration settings.
-        - endpoint: Endpoint key.
-        - starting_tscn: Starting Transaction Set Control Number.
-        """
-        print("Processing: {}".format(file_path))
-        formatted_data, transaction_set_control_number = process_file(file_path, config, endpoint, starting_tscn)
-        isa_header, gs_header, ge_trailer, iea_trailer = create_interchange_elements(config, endpoint, transaction_set_control_number - 1)
-        
-        # Combine everything into a single document
-        complete_document = "{}\n{}\n{}\n{}\n{}".format(
-            isa_header,
-            gs_header,
-            formatted_data,
-            ge_trailer,            
-            iea_trailer
-        )
-        
-        # Write to output file
-        output_file_path = write_output_file([complete_document], config.get('outputFilePath', ''), endpoint, file_path, config)
-        print("File processed. Output saved to: {}".format(output_file_path))
-    
-    if args.is_directory:
-        # Process each .DAT file within the directory
-        for file_name in os.listdir(args.path):
+    process_files(args.path, config, args.endpoint, args.is_directory)
+    print("Conversion complete.")
+
+def process_files(path, config, endpoint, is_directory):
+    """
+    Processes either a single file or all files within a directory.
+
+    Parameters:
+    - path: Path to the input fixed-width file or directory to process.
+    - config: Configuration settings loaded from a JSON file.
+    - endpoint: The endpoint for which the conversion is intended.
+    - is_directory: Boolean flag indicating if the path is a directory.
+
+    Returns:
+    - None
+    """
+    if is_directory:
+        MediLink_ConfigLoader.log("Processing all .DAT files in: {}".format(path))
+        for file_name in os.listdir(path):
             if file_name.endswith(".DAT"):
-                file_path = os.path.join(args.path, file_name)
-                process_and_write_file(file_path, config, args.endpoint)
+                file_path = os.path.join(path, file_name)
+                process_and_write_file(file_path, config, endpoint)
     else:
-        # Process a single file
-        process_and_write_file(args.path, config, args.endpoint)
+        MediLink_ConfigLoader.log("Processing the single file: {}".format(path))
+        process_and_write_file(path, config, endpoint)
+
+if __name__ == "__main__":
+    main()
+    
+# The functions below are the ones that are used as non-main library by outside scripts.
+#######################################################################################
+
+def convert_files_for_submission(detailed_patient_data, config):
+    """    
+    Processes detailed patient data for submission based on their confirmed endpoints,
+    generating a separate 837P file for each endpoint.
+
+    Parameters:
+    - detailed_patient_data: A list containing detailed patient data with endpoint information.
+    - config: Configuration settings loaded from a JSON file.
+
+    Returns:
+    - A list of paths to the converted files ready for submission.
+    """
+
+    # Initialize a dictionary to hold patient data segregated by confirmed endpoints
+    data_by_endpoint = {}
+        
+    # Populate the dictionary with patient data
+    for data in detailed_patient_data:
+        endpoint = data['confirmed_endpoint']
+        if endpoint not in data_by_endpoint:
+            data_by_endpoint[endpoint] = []
+        data_by_endpoint[endpoint].append(data)
+
+    # List to store paths of converted files for each endpoint
+    converted_files_paths = []
+
+    # Determine the total number of unique endpoints for progress bar
+    # total_endpoints = len(data_by_endpoint)
+
+    # Iterate over each endpoint and process its corresponding patient data
+    for endpoint, patient_data_list in data_by_endpoint.items():
+        # tqdm(data_by_endpoint.items(), desc="Creating 837p(s)", total=total_endpoints, ascii=True)
+        # Each endpoint might have multiple patients' data to be processed into a single 837P file
+        if patient_data_list:
+            converted_path = process_claim(config['MediLink_Config'], endpoint, patient_data_list)
+            if converted_path:
+                converted_files_paths.append(converted_path)
+        
+    return converted_files_paths
+
+def process_claim(config, endpoint, patient_data_list):
+    """
+    Processes patient data for a specified endpoint, converting it into the 837P format.
+    Generates a separate 837P file for each endpoint based on detailed patient data.
 
-    print("Conversion complete.")
+    Parameters:
+    - config: Configuration settings loaded from a JSON file.
+    - endpoint_key: The key representing the endpoint for which the data is being processed.
+    - patient_data_list: A list of dictionaries, each containing detailed patient data.
+
+    Returns:
+    - Path to the converted file, or None if an error occurs.
+    
+    TODO (LOW) Why are there duplicated interchange flows? Because the arg if we're doing a .dat directory or not. 
+    Although, that shouldn't be making duplicates of these interchange headers. That's still confusing and could end up making 
+    duplicate interchange headers because processing .dat in batch might be fast enough to be a problem.
+    """
+    output_directory = MediLink_837p_encoder_library.get_output_directory(config)
+    if not output_directory:
+        return None
+
+    # Initialize the transaction set control number and document segments
+    transaction_set_control_number = 1
+    document_segments = []
+
+    # Process each patient's data in the list
+    for patient_data in patient_data_list:
+        # Validate each patient's data
+        is_valid, validation_errors = validate_claim_data(patient_data, config)
+        if is_valid:
+            # Format the claim if data is valid
+            formatted_claim = format_single_claim(patient_data, config, endpoint, transaction_set_control_number)
+            document_segments.append(formatted_claim)
+            transaction_set_control_number += 1
+        else:
+            if MediLink_837p_encoder_library.handle_validation_errors(transaction_set_control_number, validation_errors, config):
+                continue # Skip the current patient
+
+    # Create interchange elements with the final transaction set control number
+    isa_header, gs_header, ge_trailer, iea_trailer = MediLink_837p_encoder_library.create_interchange_elements(config, endpoint, transaction_set_control_number - 1)
+
+    # Insert headers at the beginning and append trailers at the end of document segments
+    document_segments.insert(0, gs_header)
+    document_segments.insert(0, isa_header)
+    document_segments.extend([ge_trailer, iea_trailer])
+
+    # Write the complete 837P document to an output file and return its path
+    return write_output_file(document_segments, output_directory, endpoint, patient_data_list[0]['file_path'], config)
```

### Comparing `medicafe-0.240513.4/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240515.5/MediLink/MediLink_837p_encoder_library.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from datetime import datetime
-import requests
-import time
 import sys
 from MediLink import MediLink_ConfigLoader
 
 # Add parent directory of the project to the Python path
 import sys
 import os
 project_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
 sys.path.append(project_dir)
 
-from MediBot import MediBot_Preprocessor
+from MediBot import MediBot_Preprocessor_lib
+load_insurance_data_from_mains = MediBot_Preprocessor_lib.load_insurance_data_from_mains
+from MediBot import MediBot_Crosswalk_Library
+from MediLink_APIs import fetch_payer_name_from_api
 
 """
 - [ ] 1. Code Refactoring: Increase modularity and clarity, particularly in segment creation functions (e.g., `create_st_segment`, `create_nm1_billing_provider_segment`), for better maintenance and readability.
 - [ ] 2. Endpoint Support: Extend support within segment creation for additional endpoints with attention to their unique claim submission requirements.
 - [ ] 3. Payer Identification Mechanism: Refine the mechanism for dynamically identifying payers, leveraging payer mappings and integrating with external APIs like Availity for precise payer information retrieval.
 - [ ] 4. Adherence to Endpoint-Specific Standards: Implement and verify the compliance of claim data formatting and inclusion based on the specific demands of each target endpoint within the segment creation logic.
 - [ ] 5. De-persisting Intermediate Files.
@@ -133,23 +134,42 @@
     n3_segment = "N3*{}~".format(address_line_1)
     # N4 segment for facility city, state, and ZIP
     n4_segment = "N4*{}*{}*{}~".format(city, state, zip_code)
 
     return [nm1_segment, n3_segment, n4_segment]
 
 # Constructs the NM1 segment for submitter name and includes PER segment for contact information.
-def create_1000A_submitter_name_segment(config, endpoint):
+def create_1000A_submitter_name_segment(patient_data, config, endpoint):
+    """
+    Creates the 1000A submitter name segment, including the PER segment for contact information.
+
+    Args:
+        patient_data (dict): Enriched patient data containing payer information.
+        config (dict): Configuration settings.
+        endpoint (str): Intended Endpoint for resolving submitter information.
+
+    Returns:
+        list: A list containing the NM1 segment for the submitter name and the PER segment for contact information.
+    """
     endpoint_config = config['endpoints'].get(endpoint.upper(), {})
     submitter_id_qualifier = endpoint_config.get('submitter_id_qualifier', '46')  # '46' for ETIN or 'XX' for NPI
     submitter_name = endpoint_config.get('nm_103_value', 'DEFAULT NAME')  # Default name if not in config
-    submitter_id = endpoint_config.get('nm_109_value', 'DEFAULT ID')  # Default ID if not specified in endpoint
+    
+    # Extract payer_id from patient_data
+    payer_id = patient_data.get('payer_id', '')
+    
+    # Check if payer_id is Florida Blue (00590 or BCBSF) and assign submitter_id accordingly
+    if payer_id in ['00590', 'BCBSF']:
+        submitter_id = endpoint_config.get('nm_109_bcbsf', 'DEFAULT BCBSF ID')
+    else:
+        submitter_id = endpoint_config.get('nm_109_value', 'DEFAULT ID')  # Default ID if not specified in endpoint
     
     # Submitter contact details
-    contact_name = config.get('submitter_contact_name', 'RAFAEL OLIVERVIDAUD')
-    contact_telephone_number = config.get('submitter_contact_tel', '9543821782')
+    contact_name = config.get('submitter_contact_name', 'NONE')
+    contact_telephone_number = config.get('submitter_contact_tel', 'NONE')
     
     # Construct NM1 segment for the submitter
     nm1_segment = "NM1*41*2*{}*****{}*{}~".format(submitter_name, submitter_id_qualifier, submitter_id)
     
     # Construct PER segment for the submitter's contact information
     per_segment = "PER*IC*{}*TE*{}~".format(contact_name, contact_telephone_number)
 
@@ -170,36 +190,68 @@
     return "NM1*{entity_code}*2*{receiver_name}*****{id_qualifier}*{receiver_edi}~".format(
         entity_code=receiver_entity_code,
         receiver_name=receiver_name,
         id_qualifier=receiver_id_qualifier,
         receiver_edi=receiver_edi
     )
 
-def create_2010BB_payer_information_segment(parsed_data, config, endpoint):
+def payer_id_to_payer_name(parsed_data, config, endpoint):
     """
-    Creates the 2010BB payer information segment.
+    Preprocesses payer information from parsed data and enriches parsed_data with the payer name and ID.
 
     Args:
         parsed_data (dict): Parsed data containing Z-dat information.
         config (dict): Configuration settings.
         endpoint (str): Intended Endpoint for resolving payer information.
 
     Returns:
-        str: The 2010BB payer information segment.
+        dict: Enriched parsed data with payer name and payer ID.
     """
     # Step 1: Extract insurance name from parsed data
     insurance_name = parsed_data.get('INAME', '')
 
     # Step 2: Map insurance name to payer ID
     payer_id = map_insurance_name_to_payer_id(insurance_name, config)
 
-    # Step 3: Resolve payer name using payer ID
+    # Step 3: Validate payer_id
+    if payer_id is None:
+        error_message = "Payer ID for '{}' cannot be None.".format(insurance_name)
+        MediLink_ConfigLoader.log(error_message, level="WARNING")
+        raise ValueError(error_message)
+
+    # Step 4: Resolve payer name using payer ID
     payer_name = resolve_payer_name(payer_id, config, endpoint, insurance_name, parsed_data)
 
-    # Step 4: Build NM1 segment using resolved payer name and payer ID
+    # Enrich parsed_data with payer name and payer ID
+    parsed_data['payer_name'] = payer_name
+    parsed_data['payer_id'] = payer_id
+
+    return parsed_data
+
+# Then you can use the enriched parsed_data in your main function
+def create_2010BB_payer_information_segment(parsed_data):
+    """
+    Creates the 2010BB payer information segment.
+
+    Args:
+        parsed_data (dict): Parsed data containing enriched payer information.
+
+    Returns:
+        str: The 2010BB payer information segment.
+    """
+    # Extract enriched payer name and payer ID
+    payer_name = parsed_data.get('payer_name')
+    payer_id = parsed_data.get('payer_id')
+
+    # Validate payer_name and payer_id
+    if not payer_name or not payer_id:
+        error_message = "Payer name and payer ID must be provided."
+        raise ValueError(error_message)
+
+    # Build NM1 segment using provided payer name and payer ID
     return build_nm1_segment(payer_name, payer_id)
 
 def resolve_payer_name(payer_id, config, primary_endpoint, insurance_name, parsed_data):
     """
     Resolves the payer name using the provided payer ID.
 
     Args:
@@ -210,110 +262,176 @@
         parsed_data (dict): Parsed data containing patient information.
 
     Returns:
         str: The resolved payer name.
     """
 
     # Step 1: Attempt to fetch payer name from API using primary endpoint
+    MediLink_ConfigLoader.log("Attempting to resolve Payer ID {} via API.".format(payer_id), level="INFO")
     try:
         return fetch_payer_name_from_api(payer_id, config, primary_endpoint)
     except Exception as api_error:
         # Step 2: Log API resolution failure and initiate user intervention
         MediLink_ConfigLoader.log("API resolution failed for {}: {}. Initiating user intervention.".format(payer_id, str(api_error)), config, level="WARNING")
         
         # Step 3: Print warning message for user intervention
-        print("WARNING: Unable to verify Payer ID '{}' for patient '{}'. Claims for '{}' may be incorrectly routed or fail without intervention.".format(payer_id, parsed_data.get('CHART', 'unknown'), insurance_name))
-        print("ACTION REQUIRED: Please verify internet connection and the Payer ID by searching it at the expected endpoint's website.")
-        print("Note: If the Payer ID '{}' appears incorrect for '{}', it may need to be manually corrected.".format(payer_id, insurance_name))
-        print("Please update the Payer ID in the Crosswalk and initial data source (e.g., Carol's CSV) as needed.")
-        print("If unsure, llamar a dani for guidance on manual corrections.")
-        
-        # Future implementation for direct in-situ user corrections and automated retry
-        # Once the correct payer ID is input:
-        # - Retry resolving the payer name using the new payer ID as if starting afresh.
-        # - Log the outcome, and if resolution is successful, prompt the user to confirm if they wish to permanently update the crosswalk.
-        # - If confirmed:
-        #   a) Update the crosswalk by replacing the old payer ID with the new one.
-        #   b) Record a converter to adjust the far-upstream data source (e.g., Carol's CSV) to reflect the newly corrected payer ID.
-        # Future implementation to be handled by a class or system capable of pausing and resuming processes
-        # To be developed: pass_to_user_intervention_module(payer_id, insurance_name)
-        # After user correction:
-        # corrected_payer_id = get_corrected_payer_id(payer_id)
-        # return resolve_payer_name(corrected_payer_id, config, primary_endpoint, insurance_name)
-        # Considerations for implementation:
-        # - Ensure robust logging and tracking of user interventions for auditing and error resolution purposes.
-        # - Develop a mechanism to seamlessly pause and resume processing, maintaining state and context for batch operations.
+        print("\nWARNING: Unable to verify Payer ID '{}' for patient '{}'!".format(payer_id, parsed_data.get('CHART', 'unknown')))
+        print("         Claims for '{}' may be incorrectly routed or fail without intervention.".format(insurance_name))
+        print("\nACTION REQUIRED: Please verify the internet connection and the Payer ID by searching it at the expected endpoint's website or using Google.")
+        print("Note: If the Payer ID '{}' is incorrect for '{}', it may need to be manually corrected.".format(payer_id, insurance_name))
+        print("If the Payer ID appears correct, you may skip the correction and force-continue with this one.")
+        print("\nPlease check the Payer ID in the Crosswalk and the initial data source (e.g., Carol's CSV) as needed.")
+        print("If unsure, llamar a Dani for guidance on manual corrections.")
 
         # Step 4: Integrate user input logic
-        user_decision = input("Type 'continue' to force-continue with the Medisoft name, or 'exit' to stop processing and make corrections: ")
-        if user_decision.lower() == 'continue':
+        user_decision = input("Type 'FORCE' to force-continue with the Medisoft name, or press Enter to pause processing and make corrections: ")
+        user_decision = user_decision.strip().lower()  # Convert to lowercase and remove leading/trailing whitespace
+        if user_decision == 'force':
             # Step 5: Fallback to truncated insurance name
             truncated_name = insurance_name[:10]  # Temporary fallback
             MediLink_ConfigLoader.log("Using truncated insurance name '{}' as a fallback for {}".format(truncated_name, payer_id), config, level="WARNING")
             return truncated_name
-        elif user_decision.lower() == 'exit':
-            print("Exiting script. Please make the necessary corrections and retry.")
-            exit(1)  # Exiting the script; adjust based on actual flow control requirements.
+        elif not user_decision:  # Check if user pressed Enter
+            corrected_payer_id = prompt_user_for_payer_id(insurance_name)
+            if corrected_payer_id:
+                try:
+                    resolved_name = fetch_payer_name_from_api(corrected_payer_id, config, primary_endpoint)
+                    print("API resolved to insurance name: {}".format(resolved_name))
+                    MediLink_ConfigLoader.log("API Resolved to standard insurance name: {} for corrected payer ID: {}".format(resolved_name, corrected_payer_id), config, level="INFO")
+                    
+                    confirmation = input("Is the standard insurance name '{}' correct? (yes/no): ".format(resolved_name)).strip().lower()
+                    
+                    if confirmation in ['yes', 'y']:
+                        if MediBot_Crosswalk_Library.update_crosswalk_with_corrected_payer_id(payer_id, corrected_payer_id):
+                            return resolved_name
+                        else:
+                            print("Failed to update crosswalk with the corrected Payer ID.")
+                            exit(1) # probably needs a different failure direction here.
+                    else:
+                        print("User did not confirm the standard insurance name. Manual intervention is required.")
+                        MediLink_ConfigLoader.log("User did not confirm the standard insurance name. Manual intervention is required.", config, level="CRITICAL")
+                        exit(1) # probably needs a different failure direction here.
+                except Exception as e:
+                    print("Failed to resolve corrected payer ID to standard insurance name: {}".format(e))
+                    MediLink_ConfigLoader.log("Failed to resolve corrected payer ID to standard insurance name: {}".format(e), config, level="ERROR")
+                    exit(1) # probably needs a different failure direction here.
+            else:
+                print("Exiting script. Please make the necessary corrections and retry.")
+                exit(1) # probably needs a different failure direction here.
+
+def prompt_user_for_payer_id(insurance_name):
+    """
+    Prompts the user to input the payer ID manually.
+    """
+    print("Manual intervention required: No payer ID found for insurance name '{}'.".format(insurance_name))
+    payer_id = input("Please enter the payer ID manually: ").strip()
+    return payer_id
 
 def build_nm1_segment(payer_name, payer_id):
     # Step 1: Build NM1 segment using payer name and ID
     return "NM1*PR*2*{}*****PI*{}~".format(payer_name, payer_id)
 
 def map_insurance_name_to_payer_id(insurance_name, config):
     """
-    Maps the insurance name provided by Medisoft to the corresponding payer ID by referencing
-    a crosswalk mapping stored in the "crosswalk" JSON file. This file must be located at a path
-    specified in the config under the key 'crosswalk_path'.
-
-    Inputs:
-    - insurance_name: The name of the insurance as provided by Medisoft.
-    - config: A dictionary containing configuration parameters, including the path to the crosswalk JSON file.
-
-    Outputs:
-    - payer_id: The unique identifier (ID) corresponding to the insurance name, if the mapping
-      is successful. It will be a 5-character alphanumeric code.
-
-    Functionality:
-    - This function retrieves the mapping from a "crosswalk" JSON file using the provided configuration.
-    - It first uses the MAINS data to map the insurance name to its corresponding Medisoft ID.
-    - Then, it looks up the payer ID associated with the Medisoft ID in the crosswalk.
-    - If the mapping is successful, it returns the payer ID.
-    - If the mapping fails or the payer ID cannot be retrieved, it raises an error indicating
-      the inability to extract the payer ID.
+    Maps insurance name to payer ID using the crosswalk configuration.
+
+    Args:
+        insurance_name (str): Name of the insurance.
+        config (dict): Configuration settings.
+
+    Returns:
+        str: The payer ID corresponding to the insurance name.
     """
-    _, crosswalk = MediLink_ConfigLoader.load_configuration(None, config.get('crosswalkPath', 'crosswalk.json'))
-    
     try:
+        # Ensure crosswalk is initialized and 'payer_id' key is available
+        MediBot_Crosswalk_Library.check_and_initialize_crosswalk(config)
+        
+        # Load crosswalk configuration
+        _, crosswalk = MediLink_ConfigLoader.load_configuration(None, config.get('crosswalkPath', 'crosswalk.json'))
+        
         # Load insurance data from MAINS to get insurance ID
-        insurance_to_id = MediBot_Preprocessor.load_insurance_data_from_mains(config)
+        insurance_to_id = load_insurance_data_from_mains(config)
         
         # Get medisoft ID corresponding to the insurance name
         medisoft_id = insurance_to_id.get(insurance_name)
         if medisoft_id is None:
-            raise ValueError("No Medisoft ID found for insurance name: {}".format(insurance_name))
+            error_message = "No Medisoft ID found for insurance name: {}. Consider checking MAINS directly.".format(insurance_name)
+            MediLink_ConfigLoader.log(error_message, config, level="ERROR")
+            raise ValueError(error_message)
         
         # Convert medisoft_id to string to match the JSON data type
         medisoft_id_str = str(medisoft_id)
         
         # Get payer ID corresponding to the medisoft ID
+        payer_id = None
         for payer, payer_info in crosswalk['payer_id'].items():
             if medisoft_id_str in payer_info['medisoft_id']:
-                return payer
-        
-        raise ValueError("No payer ID found for Medisoft ID: {}".format(medisoft_id))
-        # TODO (Med Crosswalk) OK so then what? This is when the crosswalk has insufficient information.
-        # This means there is a new insurance from the Z data that we haven't seen before?
-        # update_crosswalk would have had to catch this earlier in the flow.
-        
+                payer_id = payer
+                break
+
+        # Handle the case where no payer ID is found
+        if payer_id is None:
+            error_message = "No payer ID found for Medisoft ID: {}".format(medisoft_id)
+            MediLink_ConfigLoader.log(error_message, config, level="ERROR")
+            print(error_message)
+            payer_id = handle_missing_payer_id(insurance_name, config)
+
+        return payer_id
+
     except ValueError as e:
         if "JSON" in str(e) and "decode" in str(e):
-            raise ValueError("Error decoding the crosswalk JSON file")
+            error_message = "Error decoding the crosswalk JSON file in map_insurance_name_to_payer_id"
+            MediLink_ConfigLoader.log(error_message, config, level="CRITICAL")
+            raise ValueError(error_message)
         else:
+            error_message = "Unexpected error in map_insurance_name_to_payer_id: {}".format(e)
+            MediLink_ConfigLoader.log(error_message, config, level="ERROR")
             raise e
 
+def handle_missing_payer_id(insurance_name, config):
+    """
+    Handles cases where the payer ID is not found for a given Medisoft ID.
+
+    """
+    print("Missing Payer ID for insurance name: {}".format(insurance_name))
+    MediLink_ConfigLoader.log("Missing Payer ID for insurance name: {}".format(insurance_name), config, level="WARNING")
+
+    # Prompt the user for manual intervention to input the payer ID
+    payer_id = prompt_user_for_payer_id(insurance_name)
+    
+    if not payer_id:
+        message = "Unable to resolve missing Payer ID. Manual intervention is required."
+        MediLink_ConfigLoader.log(message, config, level="CRITICAL")
+        return None
+    
+    # Resolve the payer ID to a standard insurance name via API
+    try:
+        # primary_endpoint=None should kick to the default in the api function.
+        standard_insurance_name = resolve_payer_name(payer_id, config, primary_endpoint=None, insurance_name=insurance_name, parsed_data={})
+        message = "Resolved to standard insurance name: {} for payer ID: {}".format(standard_insurance_name, payer_id)
+        print(message)
+        MediLink_ConfigLoader.log(message, config, level="INFO")
+    except Exception as e:
+        message = "Failed to resolve payer ID to standard insurance name: {}".format(e)
+        print(message)
+        MediLink_ConfigLoader.log(message, config, level="ERROR")
+        return None
+    
+    # Ask for user confirmation
+    confirmation = input("Is the standard insurance name '{}' correct? (yes/no): ".format(standard_insurance_name)).strip().lower() or 'yes'
+    
+    if confirmation in ['yes', 'y']:
+        # Update the crosswalk with the new payer ID and insurance name mapping
+        MediBot_Crosswalk_Library.update_crosswalk_with_new_payer_id(insurance_name, payer_id, config)
+        return payer_id
+    else:
+        print("User did not confirm the standard insurance name. Manual intervention is required.")
+        MediLink_ConfigLoader.log("User did not confirm the standard insurance name. Manual intervention is required.", config, level="CRITICAL")
+        return None
+
 def create_nm1_payto_address_segments(config):
     """
     Constructs the NM1 segment for the Pay-To Address, N3 for street address, and N4 for city, state, and ZIP.
     This is used if the Pay-To Address is different from the Billing Provider Address.
     """
     payto_provider_name = config.get('payto_provider_name', 'DEFAULT PAY-TO NAME')
     payto_address = config.get('payto_address', 'DEFAULT PAY-TO ADDRESS')
@@ -338,139 +456,14 @@
     payer_zip = config.get('payer_zip', '')
 
     n3_segment = "N3*{}~".format(payer_address_line_1)
     n4_segment = "N4*{}*{}*{}~".format(payer_city, payer_state, payer_zip)
 
     return [n3_segment, n4_segment]
 
-# Fetches the payer name from API based on the payer ID.
-# Initialize a global dictionary to store the access token and its expiry time
-# TODO (Low API) This will need to get setup for each endpoint separately. 
-token_cache = {
-    'access_token': None,
-    'expires_at': 0  # Timestamp of when the token expires
-}
-
-def get_access_token(endpoint_config):
-    current_time = time.time()
-    
-    # Check if the cached token is still valid
-    if token_cache['access_token'] and token_cache['expires_at'] > current_time:
-        return token_cache['access_token']
-
-    # Validate endpoint configuration
-    if not endpoint_config or not all(k in endpoint_config for k in ['client_id', 'client_secret', 'token_url']):
-        raise ValueError("Endpoint configuration is incomplete or missing necessary fields.")
-
-    # Extract credentials and URL from the config
-    CLIENT_ID = endpoint_config.get("client_id")
-    CLIENT_SECRET = endpoint_config.get("client_secret")
-    url = endpoint_config.get("token_url")
-
-    # Setup the data payload and headers for the HTTP request
-    data = {
-        'grant_type': 'client_credentials',
-        'client_id': CLIENT_ID,
-        'client_secret': CLIENT_SECRET,
-        'scope': 'hipaa'
-    }
-    headers = {
-        'Content-Type': 'application/x-www-form-urlencoded'
-    }
-
-    try:
-        # Perform the HTTP request to get the access token
-        response = requests.post(url, headers=headers, data=data)
-        response.raise_for_status()  # This will raise an exception for HTTP error statuses
-        json_response = response.json()
-        access_token = json_response.get('access_token')
-        expires_in = json_response.get('expires_in', 3600)  # Default to 3600 seconds if not provided
-
-        if not access_token:
-            raise ValueError("No access token returned by the server.")
-        
-        # Store the access token and calculate the expiry time
-        token_cache['access_token'] = access_token
-        token_cache['expires_at'] = current_time + expires_in - 120  # Subtracting 120 seconds to provide buffer
-
-        return access_token
-    except requests.RequestException as e:
-        # Handle HTTP errors (e.g., network problems, invalid response)
-        error_msg = "Failed to retrieve access token: {0}. Response status: {1}".format(str(e), response.status_code if response else 'No response')
-        raise Exception(error_msg)
-    except ValueError as e:
-        # Handle specific errors like missing access token
-        raise Exception("Configuration or server response error: {0}".format(str(e)))
-
-def fetch_payer_name_from_api(payer_id, config, primary_endpoint):
-    """
-    Fetches the payer name from the API using the provided payer ID.
-
-    Args:
-        payer_id (str): The ID of the payer.
-        config (dict): Configuration settings.
-        primary_endpoint (str): The primary endpoint for resolving payer information.
-
-    Raises:
-        ValueError: If all endpoints are exhausted without finding the payer.
-
-    Returns:
-        str: The fetched payer name.
-    """
-    # Step 1: Retrieve endpoint configurations
-    endpoints = config['endpoints']
-    tried_endpoints = []
-
-    # Step 2: Check if the primary endpoint is specified and is valid
-    if primary_endpoint and primary_endpoint in endpoints:
-        endpoint_order = [primary_endpoint] + [endpoint for endpoint in endpoints if endpoint != primary_endpoint]
-    else:
-        endpoint_order = list(endpoints.keys())
-
-    # Step 3: Iterate through available endpoints in specified order
-    for endpoint_name in endpoint_order:
-        endpoint_config = endpoints[endpoint_name]
-        if not all(key in endpoint_config for key in ['token_url', 'client_id', 'client_secret']):
-            MediLink_ConfigLoader.log("Skipping {} due to missing API keys.".format(endpoint_name), config, level="WARNING")
-            continue
-
-        # Consider abstracting out the API call.
-
-        # Step 4: Get access token for the endpoint
-        token = get_access_token(endpoint_config)
-        api_url = endpoint_config.get("api_url", "")
-        headers = {'Authorization': 'Bearer {}'.format(token), 'Accept': 'application/json'}
-        params = {'payerId': payer_id}
-
-        try:
-            # Step 5: Make API call to fetch payer name
-            response = requests.get(api_url, headers=headers, params=params)
-            response.raise_for_status()
-            data = response.json()
-            if 'payers' in data and data['payers']:
-                payer = data['payers'][0]
-                return payer.get('displayName') or payer.get('name')
-            else:
-                MediLink_ConfigLoader.log("No payer found at {} for ID: {}. Trying next available endpoint.".format(endpoint_name, payer_id), config, level="INFO")
-        except requests.RequestException as e:
-            # Step 6: Log API call failure
-            MediLink_ConfigLoader.log("API call failed at {} for Payer ID '{}': {}".format(endpoint_name, payer_id, str(e)), config, level="ERROR")
-            tried_endpoints.append(endpoint_name)
-    
-    # Step 7: Log all endpoints exhaustion and raise error
-    error_message = "All endpoints exhausted for Payer ID {}. Endpoints tried: {}".format(payer_id, ', '.join(tried_endpoints))
-    MediLink_ConfigLoader.log(error_message, config, level="CRITICAL")
-    raise ValueError(error_message)
-
-# Test Case for API fetch
-#payer_id = "11347"
-#config = load_configuration() 
-#payer_name = fetch_payer_name_from_api(payer_id, config, endpoint='AVAILITY')
-#print(payer_id, payer_name)
-
 # Constructs the PRV segment for billing provider.
 def create_billing_prv_segment(config, endpoint):
     if endpoint.lower() == 'optumedi':
         return "PRV*BI*PXC*{}~".format(config['billing_provider_taxonomy'])
     return ""
 
 # Constructs the HL segment for subscriber [hierarchical level (HL*2)]
@@ -560,32 +553,36 @@
         print("Insurance Type Options:")
         # Sorting the dictionary keys to ensure consistent order
         sorted_keys = sorted(options.keys())
         for code in sorted_keys:
             description = options[code]
             print("{} - {}".format(code, description))
 
-    # Prompt to display full list
-    display_full_list = input("Do you want to see the full list of insurance options? (yes/no): ").strip().lower()
-
-    # Display full list if user confirms
-    if display_full_list in ['yes', 'y']:
-        display_insurance_options(insurance_options)
+    def prompt_display_insurance_options():
+        # Prompt to display full list
+        display_full_list = input("Do you want to see the full list of insurance options? (yes/no): ").strip().lower()
+
+        # Display full list if user confirms
+        if display_full_list in ['yes', 'y']:
+            display_insurance_options(insurance_options)
 
+    # Horrible menu
+    prompt_display_insurance_options()
+    
     # Default selection
     insurance_type_code = '12'
 
     # User input for insurance type
     user_input = input("Enter the 2-character code for the insurance type (or press Enter to default to '12' for PPO): ").strip().upper()
 
     # Validate input and set the insurance type code
     if user_input in insurance_options:
         insurance_type_code = user_input
     else:
-        print("Invalid input. Defaulting to Preferred Provider Organization (PPO)")
+        print("Skipped or Input not recognized. Defaulting to Preferred Provider Organization (PPO)\n")
 
     return insurance_type_code
 
 # Constructs the NM1 segment for subscriber based on parsed data and configuration.
 def create_nm1_subscriber_segment(config, parsed_data, endpoint):
     if endpoint.lower() == 'optumedi':
         entity_identifier_code = config['endpoints']['OPTUMEDI'].get('subscriber_entity_code', 'IL')
@@ -711,14 +708,50 @@
     # DTP - Date
     segments.append("DTP*472*D8*{}~".format(convert_date_format(parsed_data['DATE'])))
     
     # Is there REF - Line Item Control Number missing here?
     
     return segments
 
+def get_endpoint_config(config, endpoint):
+    endpoint_config = config['endpoints'].get(endpoint.upper(), {})
+    if not endpoint_config:
+        print("Endpoint configuration for {} not found.".format(endpoint))
+        return None
+    return endpoint_config
+
+def create_interchange_elements(config, endpoint, transaction_set_control_number):
+    """
+    Create interchange headers and trailers for an 837P document.
+
+    Parameters:
+    - config: Configuration settings loaded from a JSON file.
+    - endpoint: The endpoint for which the data is being processed.
+    - transaction_set_control_number: The starting transaction set control number.
+
+    Returns:
+    - Tuple containing (ISA header, GS header, GE trailer, IEA trailer).
+    """
+    endpoint_config = get_endpoint_config(config, endpoint)
+    
+    # Get the current system time and format it as 'HHMMSS' in 24-hour clock.
+    current_time = datetime.now().strftime('%H%M%S')
+    isa13 = '000' + current_time  # Format ISA13 with '000HHMMSS'.
+
+    # Check if isa13 could not be generated from the current time
+    if len(isa13) != 9:
+        # If isa13 cannot be generated from the current time, use the configured value.
+        isa13 = endpoint_config.get('isa_13_value', '000000001')
+    
+    # Create interchange header and trailer using provided library functions.
+    isa_header, gs_header = create_interchange_header(config, endpoint, isa13)
+    ge_trailer, iea_trailer = create_interchange_trailer(config, transaction_set_control_number, isa13)
+    
+    return isa_header, gs_header, ge_trailer, iea_trailer
+
 # Generates the ISA and GS segments for the interchange header based on configuration and endpoint.
 def create_interchange_header(config, endpoint, isa13):
     """
     Generate ISA and GS segments for the interchange header, ensuring endpoint-specific requirements are met.
     Includes support for Availity, Optum, and PNT_DATA endpoints, with streamlined configuration and default handling.
 
     Parameters:
@@ -805,8 +838,52 @@
     # Construct the SE segment with the actual segment count and the formatted transaction set control_number
     se_segment = "SE*{0}*{1}~".format(segment_count, formatted_control_number)
 
     # Assuming the placeholder SE segment was the last segment added before compiling
     # This time, we directly replace the placeholder with the correct SE segment
     formatted_837p = compiled_segments.rsplit('SE**', 1)[0] + se_segment
     
-    return formatted_837p
+    return formatted_837p
+
+def handle_validation_errors(transaction_set_control_number, validation_errors, config):
+    for error in validation_errors:
+        MediLink_ConfigLoader.log("Validation error for transaction set {}: {}".format(transaction_set_control_number, error), config, level="WARNING")
+    
+    print("Validation errors encountered for transaction set {}. Errors: {}".format(transaction_set_control_number, validation_errors))
+    user_input = input("Skip this patient and continue without incrementing transaction set number? (yes/no): ")
+    if user_input.lower() == 'yes':
+        print("Skipping patient...")
+        MediLink_ConfigLoader.log("Skipped processing of transaction set {} due to user decision.".format(transaction_set_control_number), config, level="INFO")
+        return True  # Skip the current patient
+    else:
+        print("Processing halted due to validation errors.")
+        MediLink_ConfigLoader.log("HALT: Processing halted at transaction set {} due to unresolved validation errors.".format(transaction_set_control_number), config, level="ERROR")
+        sys.exit()  # Optionally halt further processing
+        
+def winscp_validate_output_directory(output_directory):
+    """
+    Validates the output directory path to ensure it has no spaces.
+    If spaces are found, prompts the user to input a new path.
+    If the directory doesn't exist, creates it.
+    """
+    while ' ' in output_directory:
+        print("\nWARNING: The output directory path contains spaces, which can cause issues with upload operations.")
+        print("    Current proposed path: {}".format(output_directory))
+        new_path = input("Please enter a new path for the output directory: ")
+        output_directory = new_path.strip()  # Remove leading/trailing spaces
+    
+    # Check if the directory exists, if not, create it
+    if not os.path.exists(output_directory):
+        os.makedirs(output_directory)
+        print("INFO: Created output directory: {}".format(output_directory))
+    
+    return output_directory
+
+def get_output_directory(config):
+    # Retrieve desired default output file path from config 
+    output_directory = config.get('outputFilePath', '')
+    # BUG (Low SFTP) Add WinSCP validation because of the mishandling of spaces in paths. (This shouldn't need to exist.)
+    output_directory = winscp_validate_output_directory(output_directory)
+    if not os.path.isdir(output_directory):
+        print("Output directory does not exist. Please check the configuration.")
+        return None
+    return output_directory
```

### Comparing `medicafe-0.240513.4/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240515.5/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.4/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240515.5/MediLink/MediLink_DataMgmt.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,23 @@
 
 # Helper function to slice and strip values
 def slice_data(data, slices):
     # Convert slices list to a tuple for slicing operation
     return {key: data[slice(*slices[key])].strip() for key in slices}
 
 # Function to parse fixed-width Medisoft output and extract claim data
-def parse_fixed_width_data(personal_info, insurance_info, service_info, config):
+def parse_fixed_width_data(personal_info, insurance_info, service_info, config=None):
+    
+    # Make sure we have the right config
+    if not config:  # Checks if config is None or an empty dictionary
+        MediLink_ConfigLoader.log("No config passed to parse_fixed_width_data. Re-loading config...", level="WARNING")
+        config, _ = MediLink_ConfigLoader.load_configuration()
+    
+    config = config.get('MediLink_Config', config) # Safest config call.
+    
     # Load slice definitions from config within the MediLink_Config section
     personal_slices = config['fixedWidthSlices']['personal_slices']
     insurance_slices = config['fixedWidthSlices']['insurance_slices']
     service_slices = config['fixedWidthSlices']['service_slices']
 
     # Parse each segment
     parsed_data = {}
@@ -28,28 +36,28 @@
     parsed_data.update(slice_data(service_info, service_slices))
     
     MediLink_ConfigLoader.log("Successfully parsed data from segments", config, level="INFO")
     
     return parsed_data
 
 # Function to read fixed-width Medisoft output and extract claim data
-def read_fixed_width_data(file_path, config):
+def read_fixed_width_data(file_path):
     # Reads the fixed width data from the file and yields each patient's
     # personal, insurance, and service information.
     MediLink_ConfigLoader.log("Starting to read fixed width data...")
     with open(file_path, 'r') as file:
         lines_buffer = []  # Buffer to hold lines for current patient data
         for line in file:
             stripped_line = line.strip()
             if stripped_line:  # Only process non-empty lines
                 lines_buffer.append(stripped_line)
                 # Once we have 3 lines of data, yield them as a patient record
                 if len(lines_buffer) == 3:
                     personal_info, insurance_info, service_info = lines_buffer
-                    MediLink_ConfigLoader.log("Successfully read data from file: {}".format(file_path), config, level="INFO")
+                    MediLink_ConfigLoader.log("Successfully read data from file: {}".format(file_path), level="INFO")
                     yield personal_info, insurance_info, service_info
                     lines_buffer.clear()  # Reset buffer for the next patient record
             # If the line is blank but we have already started collecting a patient record,
             # we continue without resetting the buffer, effectively skipping blank lines.
 
 # TODO (Refactor) Consider consolidating with the other read_fixed_with_data 
 def read_general_fixed_width_data(file_path, slices):
```

### Comparing `medicafe-0.240513.4/MediLink/MediLink_Down.py` & `medicafe-0.240515.5/MediLink/MediLink_Down.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import logging
 import argparse
 import shutil
 from datetime import datetime
 import glob
 import MediLink_ERA_decoder
 from MediLink_DataMgmt import operate_winscp
 import MediLink_ConfigLoader
```

### Comparing `medicafe-0.240513.4/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240515.5/MediLink/MediLink_ERA_decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
-import logging
 import sys
+import csv
 from MediLink_ConfigLoader import load_configuration, log
 from MediLink_DataMgmt import consolidate_csvs
-import csv
+
 
 """
 1. ERA File Processing: Implement robust mechanisms for reading and parsing ERA files, addressing potential file integrity issues and accommodating scenarios with multiple payer addresses within a single ERA.
 2. Wildcard File Processing: Enable effective batch processing of ERA files using wildcard patterns in the `--era_file_path` argument, resulting in a unified CSV output.
 3. Date of Service Parsing: Enhance the parsing logic for 'Date of Service' to accommodate different segment identifiers, improving data extraction reliability.
 4. Payer Address Extraction: Fine-tune the logic for extracting payer and provider addresses from ERA files, ensuring only relevant information is captured.
 5. De-persisting Intermediate Files.
```

### Comparing `medicafe-0.240513.4/MediLink/MediLink_Gmail.py` & `medicafe-0.240515.5/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.4/MediLink/MediLink_Scheduler.py` & `medicafe-0.240515.5/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.4/MediLink/MediLink_UI.py` & `medicafe-0.240515.5/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.4/MediLink/MediLink_Up.py` & `medicafe-0.240515.5/MediLink/MediLink_Up.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime
 import os
 import re
 import subprocess
+from tqdm import tqdm
 import MediLink_837p_encoder
 from MediLink_ConfigLoader import log
-from tqdm import tqdm
 from MediLink_DataMgmt import operate_winscp
 
 """
 Handles the transmission of files to endpoints and related tasks for the MediLink script.
 
 Functions:
 - check_internet_connection(): Checks for an active internet connection.
@@ -185,24 +185,18 @@
     # Save the receipt to a text file
     save_receipt_to_file(receipt_content, config)
     
     # Probably return receipt_data since its the easier to use dictionary
     return receipt_data
 
 def prepare_receipt_data(submission_results):
-    # Perform any necessary data processing to prepare the submission results for the receipt
-    # This includes extracting from a multi-patient 837p the patient names, dates of service, amounts billed.
-    # Also the date & time of batch claim submission from the header segment. 
-    # Get the receiver name from the 1000B receiver name segment (will be common for that file).
-    # Organize the data in dictionary by endpoint (receiver name) and then patient information.
-    # This function should completely fill out the dictionary with the necessary information for the receipt. 
     """
     Prepare submission results for a receipt, including data from both successful and failed submissions.
     
-    This function extracts patient names, dates of service, and amounts billed from an 837p file.
+    This function extracts patient names, dates of service, amounts billed, and insurance names from an 837p file.
     It also includes the date and time of batch claim submission, and the receiver name from the 1000B segment.
     Data is organized by receiver name and includes both successful and failed submissions.
     
     Parameters:
     - submission_results (dict): Contains submission results grouped by endpoint, with success status.
     
     Returns:
@@ -230,15 +224,15 @@
     return receipt_data
 
 def validate_data(receipt_data):
     # Simple validation to check if data fields are correctly populated
     for endpoint, data in receipt_data.items():
         patients = data.get("patients", [])
         for index, patient in enumerate(patients, start=1):
-            missing_fields = [field for field in ('name', 'service_date', 'amount_billed', 'success') if not patient.get(field)]
+            missing_fields = [field for field in ('name', 'service_date', 'amount_billed', 'insurance_name', 'success') if not patient.get(field)]
             
             if missing_fields:
                 # Log the missing fields without revealing PHI
                 log("Receipt Data validation error for endpoint '{}', patient {}: Missing information in fields: {}".format(endpoint, index, ", ".join(missing_fields)))
     return True
 
 def parse_837p_file(file_path):
@@ -283,50 +277,68 @@
             for record in patient_records:
                 # Extract patient name
                 name_match = re.search(r'NM1\*IL\*1\*([^*]+)\*([^*]+)\*([^*]*)', record)
                 # Extract service date
                 service_date_match = re.search(r'DTP\*472\D*8\*([0-9]{8})', record)
                 # Extract claim amount
                 amount_match = re.search(r'CLM\*[^\*]*\*([0-9]+\.?[0-9]*)', record)
+                # Extract insurance name (payer_name)
+                insurance_name_match = re.search(r'NM1\*PR\*2\*([^*]+)\*', record)
                 
                 if name_match and service_date_match and amount_match:
                     # Handle optional middle name
                     middle_name = name_match.group(3).strip() if name_match.group(3) else ""
                     patient_name = "{} {} {}".format(name_match.group(2), middle_name, name_match.group(1)).strip()
                     service_date = "{}-{}-{}".format(service_date_match.group(1)[:4], service_date_match.group(1)[4:6], service_date_match.group(1)[6:])
                     amount_billed = float(amount_match.group(1))
+                    insurance_name = insurance_name_match.group(1)
                     
                     patient_details.append({
                         "name": patient_name,
                         "service_date": service_date,
-                        "amount_billed": amount_billed
+                        "amount_billed": amount_billed,
+                        "insurance_name": insurance_name
                     })
     except Exception as e:
         print("Error reading or parsing the 837p file: {0}".format(str(e)))
     
-    # Optionally, return also date_of_submission as a separate variable  
     return patient_details, date_of_submission
 
 def build_receipt_content(receipt_data):
+    """
+    Build the receipt content in a human-readable ASCII format with a tabular data presentation for patient information.
+
+    Args:
+        receipt_data (dict): Dictionary containing receipt data with patient details.
+
+    Returns:
+        str: Formatted receipt content as a string.
+    """
     # Build the receipt content in a human-readable ASCII format
-    # Improved layout with tabular data presentation for patient information
-    receipt_lines = ["Submission Receipt", "="*60, ""]  # Header
+    receipt_lines = ["Submission Receipt", "=" * 60, ""]  # Header
+
     for endpoint, data in receipt_data.items():
         header = "Endpoint: {0} (Submitted: {1})".format(endpoint, data['date_of_submission'])
-        receipt_lines.extend([header, "-"*len(header)])
+        receipt_lines.extend([header, "-" * len(header)])
         
         # Table headers
-        table_header = "{:<20} | {:<15} | {:<15} | {:<10}".format("Patient", "Service Date", "Amount Billed", "Status")
+        table_header = "{:<20} | {:<15} | {:<15} | {:<20} | {:<10}".format("Patient", "Service Date", "Amount Billed", "Insurance", "Status")
         receipt_lines.append(table_header)
-        receipt_lines.append("-"*len(table_header))
+        receipt_lines.append("-" * len(table_header))
         
         # Adding patient information in a tabular format
         for patient in data["patients"]:
             success_status = "SUCCESS" if patient['success'] else "FAILED"
-            patient_info = "{:<20} | {:<15} | ${:<14} | {:<10}".format(patient['name'], patient['service_date'], patient['amount_billed'], success_status)
+            patient_info = "{:<20} | {:<15} | ${:<14} | {:<20} | {:<10}".format(
+                patient['name'], 
+                patient['service_date'], 
+                patient['amount_billed'], 
+                patient['insurance_name'], 
+                success_status
+            )
             receipt_lines.append(patient_info)
         
         receipt_lines.append("")  # Blank line for separation
     
     receipt_content = "\n".join(receipt_lines)
     return receipt_content
```

### Comparing `medicafe-0.240513.4/MediLink/test.py` & `medicafe-0.240515.5/MediLink/test.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.4/PKG-INFO` & `medicafe-0.240515.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240513.4
+Version: 0.240515.5
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240513.4/README.md` & `medicafe-0.240515.5/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.4/medicafe.egg-info/PKG-INFO` & `medicafe-0.240515.5/medicafe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240513.4
+Version: 0.240515.5
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240513.4/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240515.5/medicafe.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 MediBot/MediBot.bat
 MediBot/MediBot.py
 MediBot/MediBot_Charges.py
+MediBot/MediBot_Crosswalk_Library.py
 MediBot/MediBot_Preprocessor.py
 MediBot/MediBot_Preprocessor_lib.py
 MediBot/MediBot_UI.py
 MediBot/MediBot_dataformat_library.py
 MediBot/MediPost.py
 MediBot/PDF_to_CSV_Cleaner.py
 MediBot/__init__.py
 MediBot/update_json.py
 MediBot/update_medicafe.py
 MediLink/MediLink.py
 MediLink/MediLink_277_decoder.py
 MediLink/MediLink_837p_encoder.py
 MediLink/MediLink_837p_encoder_library.py
+MediLink/MediLink_APIs.py
 MediLink/MediLink_ConfigLoader.py
 MediLink/MediLink_DataMgmt.py
 MediLink/MediLink_Down.py
 MediLink/MediLink_ERA_decoder.py
 MediLink/MediLink_Gmail.py
+MediLink/MediLink_Mailer.py
 MediLink/MediLink_Scheduler.py
 MediLink/MediLink_StatusCheck.py
 MediLink/MediLink_UI.py
 MediLink/MediLink_Up.py
 MediLink/MediLink_batch.bat
 MediLink/Soumit_api.py
 MediLink/__init__.py
```

### Comparing `medicafe-0.240513.4/setup.py` & `medicafe-0.240515.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240513.4",
+    version="0.240515.5",
     description='MediCafe',
     long_description="""
     # Project Overview: MediCafe
 
     ## Project Description
     MediCafe is a comprehensive suite designed to automate and streamline several aspects of medical administrative tasks within Medisoft, a popular medical practice management software. The system consists of two main components: MediBot and MediLink, each serving distinct functions but integrated to enhance the workflow of medical practices.
```

