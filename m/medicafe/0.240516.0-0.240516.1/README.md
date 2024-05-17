# Comparing `tmp/medicafe-0.240516.0.tar.gz` & `tmp/medicafe-0.240516.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240516.0.tar", last modified: Thu May 16 23:59:16 2024, max compression
+gzip compressed data, was "medicafe-0.240516.1.tar", last modified: Fri May 17 02:28:08 2024, max compression
```

## Comparing `medicafe-0.240516.0.tar` & `medicafe-0.240516.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 23:59:16.791000 medicafe-0.240516.0/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240516.0/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240516.0/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-16 23:59:15.977000 medicafe-0.240516.0/MediBot/
--rwxrwxrwx   0        0        0     5972 2024-05-12 18:02:44.000000 medicafe-0.240516.0/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    17490 2024-05-15 17:01:43.000000 medicafe-0.240516.0/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240516.0/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    14544 2024-05-16 23:40:08.000000 medicafe-0.240516.0/MediBot/MediBot_Crosswalk_Library.py
--rw-rw-rw-   0        0        0    14906 2024-05-15 16:48:28.000000 medicafe-0.240516.0/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0    17184 2024-05-15 17:38:32.000000 medicafe-0.240516.0/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0    10660 2024-05-16 01:23:48.000000 medicafe-0.240516.0/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     8912 2024-05-15 20:14:35.000000 medicafe-0.240516.0/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0     3049 2024-05-16 17:42:31.000000 medicafe-0.240516.0/MediBot/MediBot_docx_decoder.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240516.0/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240516.0/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240516.0/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240516.0/MediBot/update_json.py
--rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240516.0/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-16 23:59:16.593000 medicafe-0.240516.0/MediLink/
--rw-rw-rw-   0        0        0    20316 2024-05-16 01:29:43.000000 medicafe-0.240516.0/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240516.0/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    25526 2024-05-16 00:37:08.000000 medicafe-0.240516.0/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    43553 2024-05-16 23:40:06.000000 medicafe-0.240516.0/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     6127 2024-05-16 23:37:38.000000 medicafe-0.240516.0/MediLink/MediLink_API_v2.py
--rw-rw-rw-   0        0        0     6166 2024-05-15 17:49:28.000000 medicafe-0.240516.0/MediLink/MediLink_APIs.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240516.0/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    12235 2024-05-14 15:14:04.000000 medicafe-0.240516.0/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7248 2024-05-15 07:47:12.000000 medicafe-0.240516.0/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8710 2024-05-15 13:36:03.000000 medicafe-0.240516.0/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6370 2024-05-16 17:44:21.000000 medicafe-0.240516.0/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0      370 2024-05-14 22:24:45.000000 medicafe-0.240516.0/MediLink/MediLink_Mailer.py
--rw-rw-rw-   0        0        0     7368 2024-05-16 18:14:48.000000 medicafe-0.240516.0/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240516.0/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240516.0/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0    19286 2024-05-16 01:21:31.000000 medicafe-0.240516.0/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240516.0/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240516.0/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240516.0/MediLink/__init__.py
--rw-rw-rw-   0        0        0     3108 2024-05-13 04:52:22.000000 medicafe-0.240516.0/MediLink/test.py
--rw-rw-rw-   0        0        0     4396 2024-05-16 23:59:16.776000 medicafe-0.240516.0/PKG-INFO
--rw-rw-rw-   0        0        0     2960 2024-05-13 07:31:39.000000 medicafe-0.240516.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 23:59:16.760000 medicafe-0.240516.0/medicafe.egg-info/
--rw-rw-rw-   0        0        0     4396 2024-05-16 23:59:15.000000 medicafe-0.240516.0/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1174 2024-05-16 23:59:15.000000 medicafe-0.240516.0/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 23:59:15.000000 medicafe-0.240516.0/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240516.0/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-16 23:59:15.000000 medicafe-0.240516.0/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-16 23:59:15.000000 medicafe-0.240516.0/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 23:59:16.787000 medicafe-0.240516.0/setup.cfg
--rw-rw-rw-   0        0        0     4834 2024-05-16 23:59:12.000000 medicafe-0.240516.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 02:28:08.129000 medicafe-0.240516.1/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240516.1/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240516.1/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-17 02:28:07.073000 medicafe-0.240516.1/MediBot/
+-rwxrwxrwx   0        0        0     5972 2024-05-12 18:02:44.000000 medicafe-0.240516.1/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    17490 2024-05-15 17:01:43.000000 medicafe-0.240516.1/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240516.1/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    14544 2024-05-16 23:40:08.000000 medicafe-0.240516.1/MediBot/MediBot_Crosswalk_Library.py
+-rw-rw-rw-   0        0        0    14906 2024-05-15 16:48:28.000000 medicafe-0.240516.1/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0    17184 2024-05-15 17:38:32.000000 medicafe-0.240516.1/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10660 2024-05-16 01:23:48.000000 medicafe-0.240516.1/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     8912 2024-05-15 20:14:35.000000 medicafe-0.240516.1/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0     3049 2024-05-16 17:42:31.000000 medicafe-0.240516.1/MediBot/MediBot_docx_decoder.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240516.1/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240516.1/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240516.1/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240516.1/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240516.1/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-17 02:28:07.793000 medicafe-0.240516.1/MediLink/
+-rw-rw-rw-   0        0        0    20316 2024-05-16 01:29:43.000000 medicafe-0.240516.1/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240516.1/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    25526 2024-05-16 00:37:08.000000 medicafe-0.240516.1/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    43588 2024-05-17 02:10:40.000000 medicafe-0.240516.1/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     7584 2024-05-17 02:27:46.000000 medicafe-0.240516.1/MediLink/MediLink_API_v2.py
+-rw-rw-rw-   0        0        0     6166 2024-05-15 17:49:28.000000 medicafe-0.240516.1/MediLink/MediLink_APIs.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240516.1/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    12235 2024-05-14 15:14:04.000000 medicafe-0.240516.1/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7248 2024-05-15 07:47:12.000000 medicafe-0.240516.1/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8710 2024-05-15 13:36:03.000000 medicafe-0.240516.1/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     6370 2024-05-16 17:44:21.000000 medicafe-0.240516.1/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0      370 2024-05-14 22:24:45.000000 medicafe-0.240516.1/MediLink/MediLink_Mailer.py
+-rw-rw-rw-   0        0        0     7368 2024-05-16 18:14:48.000000 medicafe-0.240516.1/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240516.1/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240516.1/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0    19286 2024-05-16 01:21:31.000000 medicafe-0.240516.1/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240516.1/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240516.1/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240516.1/MediLink/__init__.py
+-rw-rw-rw-   0        0        0     3108 2024-05-13 04:52:22.000000 medicafe-0.240516.1/MediLink/test.py
+-rw-rw-rw-   0        0        0     4396 2024-05-17 02:28:08.090000 medicafe-0.240516.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2960 2024-05-13 07:31:39.000000 medicafe-0.240516.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 02:28:08.009000 medicafe-0.240516.1/medicafe.egg-info/
+-rw-rw-rw-   0        0        0     4396 2024-05-17 02:28:06.000000 medicafe-0.240516.1/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1174 2024-05-17 02:28:06.000000 medicafe-0.240516.1/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 02:28:06.000000 medicafe-0.240516.1/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240516.1/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-17 02:28:06.000000 medicafe-0.240516.1/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-17 02:28:06.000000 medicafe-0.240516.1/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 02:28:08.124000 medicafe-0.240516.1/setup.cfg
+-rw-rw-rw-   0        0        0     4834 2024-05-17 02:28:03.000000 medicafe-0.240516.1/setup.py
```

### Comparing `medicafe-0.240516.0/LICENSE` & `medicafe-0.240516.1/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/MediBot/MediBot.bat` & `medicafe-0.240516.1/MediBot/MediBot.bat`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/MediBot/MediBot.py` & `medicafe-0.240516.1/MediBot/MediBot.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/MediBot/MediBot_Charges.py` & `medicafe-0.240516.1/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/MediBot/MediBot_Crosswalk_Library.py` & `medicafe-0.240516.1/MediBot/MediBot_Crosswalk_Library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240516.1/MediBot/MediBot_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240516.1/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/MediBot/MediBot_UI.py` & `medicafe-0.240516.1/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240516.1/MediBot/MediBot_dataformat_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/MediBot/MediBot_docx_decoder.py` & `medicafe-0.240516.1/MediBot/MediBot_docx_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240516.1/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/MediBot/update_json.py` & `medicafe-0.240516.1/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/MediBot/update_medicafe.py` & `medicafe-0.240516.1/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/MediLink/MediLink.py` & `medicafe-0.240516.1/MediLink/MediLink.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/MediLink/MediLink_277_decoder.py` & `medicafe-0.240516.1/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240516.1/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240516.1/MediLink/MediLink_837p_encoder_library.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,24 +270,25 @@
     try:
         return fetch_payer_name_from_api(payer_id, config, primary_endpoint)
     except Exception as api_error:
         # Step 2: Log API resolution failure and initiate user intervention
         MediLink_ConfigLoader.log("API resolution failed for {}: {}. Initiating user intervention.".format(payer_id, str(api_error)), config, level="WARNING")
         
         # Step 3: Print warning message for user intervention
-        print("\nWARNING: Unable to verify Payer ID '{}' for patient '{}'!".format(payer_id, parsed_data.get('CHART', 'unknown')))
-        print("         Claims for '{}' may be incorrectly routed or fail without intervention.".format(insurance_name))
-        print("\nACTION REQUIRED: Please verify the internet connection and the Payer ID by searching it at the expected endpoint's website or using Google.")
-        print("Note: If the Payer ID '{}' is incorrect for '{}', it may need to be manually corrected.".format(payer_id, insurance_name))
+        print("\n\nWARNING: Unable to verify Payer ID '{}' for patient '{}'!".format(payer_id, parsed_data.get('CHART', 'unknown')))
+        print("         Claims for '{}' may be incorrectly\nrouted or fail without intervention.".format(insurance_name))
+        print("\nACTION REQUIRED: Please verify the internet connection and the Payer ID by searching for it")
+        print("at the expected endpoint's website or using Google.")
+        print("\nNote: If the Payer ID '{}' is incorrect for '{}', \nit may need to be manually corrected.".format(payer_id, insurance_name))
         print("If the Payer ID appears correct, you may skip the correction and force-continue with this one.")
-        print("\nPlease check the Payer ID in the Crosswalk and the initial data source (e.g., Carol's CSV) as needed.")
+        print("\nPlease check the Payer ID in the Crosswalk and the initial \ndata source (e.g., Carol's CSV) as needed.")
         print("If unsure, llamar a Dani for guidance on manual corrections.")
 
         # Step 4: Integrate user input logic
-        user_decision = input("Type 'FORCE' to force-continue with the Medisoft name, or press Enter to pause processing and make corrections: ")
+        user_decision = input("\nType 'FORCE' to force-continue with the Medisoft name, \nor press Enter to pause processing and make corrections: ")
         user_decision = user_decision.strip().lower()  # Convert to lowercase and remove leading/trailing whitespace
         if user_decision == 'force':
             # Step 5: Fallback to truncated insurance name
             truncated_name = insurance_name[:10]  # Temporary fallback
             MediLink_ConfigLoader.log("Using truncated insurance name '{}' as a fallback for {}".format(truncated_name, payer_id), config, level="WARNING")
             return truncated_name
         elif not user_decision:  # Check if user pressed Enter
```

### Comparing `medicafe-0.240516.0/MediLink/MediLink_API_v2.py` & `medicafe-0.240516.1/MediLink/MediLink_API_v2.py`

 * *Files 23% similar despite different names*

```diff
@@ -95,26 +95,49 @@
     # Method for getting payer list
     def get_payer_list(self, endpoint_name, params=None):
         return self.make_api_call(endpoint_name, 'GET', url_extension="/availity-payer-list", params=params)
 
 # Function to fetch payer name from API
 def fetch_payer_name_from_api(payer_id, config, primary_endpoint='AVAILITY'):
     client = APIClient()
-    # Make API call to get payer list
-    response = client.get_payer_list(primary_endpoint, params={'payerId': payer_id})
-    # Check if payer found
-    if 'payers' in response and response['payers']:
-        payer = response['payers'][0]
-        payer_name = payer.get('displayName') or payer.get('name')
-        
-        # Log successful retrieval of payer name
-        MediLink_ConfigLoader.log("Successfully found payer at {} for ID {}: {}".format(primary_endpoint, payer_id, payer_name), config, level="INFO")
-        return payer_name
-    # Raise error if no payer found
-    raise ValueError("No payer found for the given ID")
+
+    # Step 1: Reload configuration for safety (This should be able to be replaced by APIClient())
+    config, _ = MediLink_ConfigLoader.load_configuration()
+
+    # Step 2: Check if the primary endpoint is specified and is valid 
+    # (these validity checks will need to be incorporated into the main functionality)
+    endpoints = config['MediLink_Config']['endpoints']
+    if primary_endpoint and primary_endpoint in endpoints:
+        endpoint_order = [primary_endpoint] + [endpoint for endpoint in endpoints if endpoint != primary_endpoint]
+    else:
+        endpoint_order = list(endpoints.keys())
+
+    # Step 3: Iterate through available endpoints in specified order
+    for endpoint_name in endpoint_order:
+        endpoint_config = endpoints[endpoint_name]
+        if not all(key in endpoint_config for key in ['token_url', 'client_id', 'client_secret']):
+            MediLink_ConfigLoader.log("Skipping {} due to missing API keys.".format(endpoint_name), config, level="WARNING")
+            continue
+
+        try:
+            response = client.get_payer_list(endpoint_name, params={'payerId': payer_id})
+            if 'payers' in response and response['payers']:
+                payer = response['payers'][0]
+                payer_name = payer.get('displayName') or payer.get('name')
+                
+                MediLink_ConfigLoader.log("Successfully found payer at {} for ID {}: {}".format(endpoint_name, payer_id, payer_name), config, level="INFO")
+                return payer_name
+            else:
+                MediLink_ConfigLoader.log("No payer found at {} for ID: {}. Trying next available endpoint.".format(endpoint_name, payer_id), config, level="INFO")
+        except requests.RequestException as e:
+            MediLink_ConfigLoader.log("API call failed at {} for Payer ID '{}': {}".format(endpoint_name, payer_id, str(e)), config, level="ERROR")
+
+    error_message = "All endpoints exhausted for Payer ID {}.".format(payer_id)
+    MediLink_ConfigLoader.log(error_message, config, level="CRITICAL")
+    raise ValueError(error_message)
 
 # Example usage
 if __name__ == "__main__":
     client = APIClient()
     try:
         # Fetch and print payer name
         payer_name = fetch_payer_name_from_api("11347", 'config.yaml')
```

### Comparing `medicafe-0.240516.0/MediLink/MediLink_APIs.py` & `medicafe-0.240516.1/MediLink/MediLink_APIs.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240516.1/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240516.1/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/MediLink/MediLink_Down.py` & `medicafe-0.240516.1/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240516.1/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/MediLink/MediLink_Gmail.py` & `medicafe-0.240516.1/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/MediLink/MediLink_Scheduler.py` & `medicafe-0.240516.1/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/MediLink/MediLink_UI.py` & `medicafe-0.240516.1/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/MediLink/MediLink_Up.py` & `medicafe-0.240516.1/MediLink/MediLink_Up.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/MediLink/test.py` & `medicafe-0.240516.1/MediLink/test.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/PKG-INFO` & `medicafe-0.240516.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240516.0
+Version: 0.240516.1
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240516.0/README.md` & `medicafe-0.240516.1/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/medicafe.egg-info/PKG-INFO` & `medicafe-0.240516.1/medicafe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240516.0
+Version: 0.240516.1
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240516.0/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240516.1/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.0/setup.py` & `medicafe-0.240516.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240516.0",
+    version="0.240516.1",
     description='MediCafe',
     long_description="""
     # Project Overview: MediCafe
 
     ## Project Description
     MediCafe is a comprehensive suite designed to automate and streamline several aspects of medical administrative tasks within Medisoft, a popular medical practice management software. The system consists of two main components: MediBot and MediLink, each serving distinct functions but integrated to enhance the workflow of medical practices.
```

