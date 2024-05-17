# Comparing `tmp/medicafe-0.240516.2.tar.gz` & `tmp/medicafe-0.240517.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240516.2.tar", last modified: Fri May 17 02:54:05 2024, max compression
+gzip compressed data, was "medicafe-0.240517.0.tar", last modified: Fri May 17 12:51:12 2024, max compression
```

## Comparing `medicafe-0.240516.2.tar` & `medicafe-0.240517.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 02:54:05.343000 medicafe-0.240516.2/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240516.2/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240516.2/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-17 02:54:04.425000 medicafe-0.240516.2/MediBot/
--rwxrwxrwx   0        0        0     6003 2024-05-17 02:35:22.000000 medicafe-0.240516.2/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    17762 2024-05-17 02:46:35.000000 medicafe-0.240516.2/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240516.2/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    14544 2024-05-16 23:40:08.000000 medicafe-0.240516.2/MediBot/MediBot_Crosswalk_Library.py
--rw-rw-rw-   0        0        0    14906 2024-05-15 16:48:28.000000 medicafe-0.240516.2/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0    17376 2024-05-17 02:52:14.000000 medicafe-0.240516.2/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0    10660 2024-05-16 01:23:48.000000 medicafe-0.240516.2/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     8912 2024-05-15 20:14:35.000000 medicafe-0.240516.2/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0     3049 2024-05-16 17:42:31.000000 medicafe-0.240516.2/MediBot/MediBot_docx_decoder.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240516.2/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240516.2/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240516.2/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240516.2/MediBot/update_json.py
--rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240516.2/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-17 02:54:05.103000 medicafe-0.240516.2/MediLink/
--rw-rw-rw-   0        0        0    20316 2024-05-16 01:29:43.000000 medicafe-0.240516.2/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240516.2/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    25526 2024-05-16 00:37:08.000000 medicafe-0.240516.2/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    43588 2024-05-17 02:10:40.000000 medicafe-0.240516.2/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     7584 2024-05-17 02:27:46.000000 medicafe-0.240516.2/MediLink/MediLink_API_v2.py
--rw-rw-rw-   0        0        0     6166 2024-05-15 17:49:28.000000 medicafe-0.240516.2/MediLink/MediLink_APIs.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240516.2/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    12235 2024-05-14 15:14:04.000000 medicafe-0.240516.2/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7248 2024-05-15 07:47:12.000000 medicafe-0.240516.2/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8710 2024-05-15 13:36:03.000000 medicafe-0.240516.2/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6370 2024-05-16 17:44:21.000000 medicafe-0.240516.2/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0      370 2024-05-14 22:24:45.000000 medicafe-0.240516.2/MediLink/MediLink_Mailer.py
--rw-rw-rw-   0        0        0     7368 2024-05-16 18:14:48.000000 medicafe-0.240516.2/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240516.2/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240516.2/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0    19283 2024-05-17 02:40:11.000000 medicafe-0.240516.2/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240516.2/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240516.2/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240516.2/MediLink/__init__.py
--rw-rw-rw-   0        0        0     3108 2024-05-13 04:52:22.000000 medicafe-0.240516.2/MediLink/test.py
--rw-rw-rw-   0        0        0     4396 2024-05-17 02:54:05.321000 medicafe-0.240516.2/PKG-INFO
--rw-rw-rw-   0        0        0     2960 2024-05-13 07:31:39.000000 medicafe-0.240516.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 02:54:05.297000 medicafe-0.240516.2/medicafe.egg-info/
--rw-rw-rw-   0        0        0     4396 2024-05-17 02:54:03.000000 medicafe-0.240516.2/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1174 2024-05-17 02:54:03.000000 medicafe-0.240516.2/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 02:54:03.000000 medicafe-0.240516.2/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240516.2/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-17 02:54:03.000000 medicafe-0.240516.2/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-17 02:54:03.000000 medicafe-0.240516.2/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 02:54:05.337000 medicafe-0.240516.2/setup.cfg
--rw-rw-rw-   0        0        0     4834 2024-05-17 02:54:02.000000 medicafe-0.240516.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 12:51:12.131000 medicafe-0.240517.0/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240517.0/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240517.0/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-17 12:51:11.299000 medicafe-0.240517.0/MediBot/
+-rwxrwxrwx   0        0        0     6003 2024-05-17 02:35:22.000000 medicafe-0.240517.0/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    17762 2024-05-17 02:46:35.000000 medicafe-0.240517.0/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240517.0/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    14544 2024-05-16 23:40:08.000000 medicafe-0.240517.0/MediBot/MediBot_Crosswalk_Library.py
+-rw-rw-rw-   0        0        0    14909 2024-05-17 03:01:04.000000 medicafe-0.240517.0/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0    17380 2024-05-17 03:01:06.000000 medicafe-0.240517.0/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10660 2024-05-16 01:23:48.000000 medicafe-0.240517.0/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     8912 2024-05-15 20:14:35.000000 medicafe-0.240517.0/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0     3049 2024-05-16 17:42:31.000000 medicafe-0.240517.0/MediBot/MediBot_docx_decoder.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240517.0/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240517.0/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240517.0/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240517.0/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240517.0/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-17 12:51:11.928000 medicafe-0.240517.0/MediLink/
+-rw-rw-rw-   0        0        0    20316 2024-05-16 01:29:43.000000 medicafe-0.240517.0/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240517.0/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    25526 2024-05-16 00:37:08.000000 medicafe-0.240517.0/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    43572 2024-05-17 12:46:58.000000 medicafe-0.240517.0/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     7670 2024-05-17 04:13:26.000000 medicafe-0.240517.0/MediLink/MediLink_API_v2.py
+-rw-rw-rw-   0        0        0     6166 2024-05-15 17:49:28.000000 medicafe-0.240517.0/MediLink/MediLink_APIs.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240517.0/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    12235 2024-05-14 15:14:04.000000 medicafe-0.240517.0/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7248 2024-05-15 07:47:12.000000 medicafe-0.240517.0/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8710 2024-05-15 13:36:03.000000 medicafe-0.240517.0/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     6370 2024-05-16 17:44:21.000000 medicafe-0.240517.0/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0      370 2024-05-14 22:24:45.000000 medicafe-0.240517.0/MediLink/MediLink_Mailer.py
+-rw-rw-rw-   0        0        0     7368 2024-05-16 18:14:48.000000 medicafe-0.240517.0/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240517.0/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240517.0/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0    19283 2024-05-17 02:40:11.000000 medicafe-0.240517.0/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240517.0/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240517.0/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240517.0/MediLink/__init__.py
+-rw-rw-rw-   0        0        0     3108 2024-05-13 04:52:22.000000 medicafe-0.240517.0/MediLink/test.py
+-rw-rw-rw-   0        0        0     4396 2024-05-17 12:51:12.113000 medicafe-0.240517.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2960 2024-05-13 07:31:39.000000 medicafe-0.240517.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 12:51:12.093000 medicafe-0.240517.0/medicafe.egg-info/
+-rw-rw-rw-   0        0        0     4396 2024-05-17 12:51:10.000000 medicafe-0.240517.0/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1174 2024-05-17 12:51:10.000000 medicafe-0.240517.0/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 12:51:10.000000 medicafe-0.240517.0/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240517.0/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-17 12:51:10.000000 medicafe-0.240517.0/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-17 12:51:10.000000 medicafe-0.240517.0/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 12:51:12.125000 medicafe-0.240517.0/setup.cfg
+-rw-rw-rw-   0        0        0     4834 2024-05-17 12:51:07.000000 medicafe-0.240517.0/setup.py
```

### Comparing `medicafe-0.240516.2/LICENSE` & `medicafe-0.240517.0/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.2/MediBot/MediBot.bat` & `medicafe-0.240517.0/MediBot/MediBot.bat`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.2/MediBot/MediBot.py` & `medicafe-0.240517.0/MediBot/MediBot.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.2/MediBot/MediBot_Charges.py` & `medicafe-0.240517.0/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.2/MediBot/MediBot_Crosswalk_Library.py` & `medicafe-0.240517.0/MediBot/MediBot_Crosswalk_Library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.2/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240517.0/MediBot/MediBot_Preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,17 +173,17 @@
    
     # CSV Integrity Checks
     # Check for blank or partially blank CSV
     if len(csv_headers) == 0 or all(header == "" for header in csv_headers):
         missing_fields_warnings.append("WARNING: The CSV appears to be blank or contains only headers without data.")
 
     # Display the identified fields and missing fields warnings
-    MediLink_ConfigLoader.log("The following Medisoft fields have been identified in the CSV:")
-    for header, medisoft_field in identified_fields.items():
-        MediLink_ConfigLoader.log("{} (CSV header: {})".format(medisoft_field, header))
+    #MediLink_ConfigLoader.log("The following Medisoft fields have been identified in the CSV:")
+    #for header, medisoft_field in identified_fields.items():
+    #    MediLink_ConfigLoader.log("{} (CSV header: {})".format(medisoft_field, header))
 
     # This section interprets the information from identified_fields and decides if there are significant issues.
     # e.g. If the 'Street' value:key is 'Address', then any warnings about City, State, Zip can be ignored.
     for header, field in identified_fields.items():
         # Insurance Policy Numbers should be all alphanumeric with no other characters. 
         if 'Insurance Policy Number' in field:
             policy_number = identified_fields.get(header)
```

### Comparing `medicafe-0.240516.2/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240517.0/MediBot/MediBot_Preprocessor_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,23 +153,23 @@
                 row['Primary Insurance'] = new_value
             elif row.get('Ins1 Payer ID') == old_value:
                 row['Ins1 Payer ID'] = new_value
 
 def update_insurance_ids(csv_data, crosswalk):
     for row in csv_data:
         ins1_payer_id = row.get('Ins1 Payer ID', '').strip()
-        MediLink_ConfigLoader.log("Ins1 Payer ID '{}' associated with Patient ID {}.".format(ins1_payer_id, row.get('Patient ID', "None")))
+        # MediLink_ConfigLoader.log("Ins1 Payer ID '{}' associated with Patient ID {}.".format(ins1_payer_id, row.get('Patient ID', "None")))
         if ins1_payer_id:
             if ins1_payer_id in crosswalk.get('payer_id', {}):
                 medisoft_ids = crosswalk['payer_id'][ins1_payer_id].get('medisoft_id', [])
                 if medisoft_ids:
                     medisoft_ids = [int(id) for id in medisoft_ids]
                     # TODO Try to match OpenPM's Insurance Name to get a better match
                     row['Ins1 Insurance ID'] = medisoft_ids[0] 
-                    MediLink_ConfigLoader.log("Ins1 Insurance ID '{}' used for Payer ID {} in crosswalk.".format(row.get('Ins1 Insurance ID', ''), ins1_payer_id))
+                    # MediLink_ConfigLoader.log("Ins1 Insurance ID '{}' used for Payer ID {} in crosswalk.".format(row.get('Ins1 Insurance ID', ''), ins1_payer_id))
             else:
                 MediLink_ConfigLoader.log("Ins1 Payer ID '{}' not found in the crosswalk.".format(ins1_payer_id))
                 # Create a placeholder entry in the crosswalk, need to consider the medisoft_medicare_id handling later.
                 if 'payer_id' not in crosswalk:
                     crosswalk['payer_id'] = {}
                 crosswalk['payer_id'][ins1_payer_id] = {
                     'medisoft_id': [],
```

### Comparing `medicafe-0.240516.2/MediBot/MediBot_UI.py` & `medicafe-0.240517.0/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.2/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240517.0/MediBot/MediBot_dataformat_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.2/MediBot/MediBot_docx_decoder.py` & `medicafe-0.240517.0/MediBot/MediBot_docx_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.2/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240517.0/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.2/MediBot/update_json.py` & `medicafe-0.240517.0/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.2/MediBot/update_medicafe.py` & `medicafe-0.240517.0/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.2/MediLink/MediLink.py` & `medicafe-0.240517.0/MediLink/MediLink.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.2/MediLink/MediLink_277_decoder.py` & `medicafe-0.240517.0/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.2/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240517.0/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.2/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240517.0/MediLink/MediLink_837p_encoder_library.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,16 +160,16 @@
     # Check if payer_id is Florida Blue (00590 or BCBSF) and assign submitter_id accordingly
     if payer_id in ['00590', 'BCBSF']:
         submitter_id = endpoint_config.get('nm_109_bcbsf', 'DEFAULT BCBSF ID')
     else:
         submitter_id = endpoint_config.get('nm_109_value', 'DEFAULT ID')  # Default ID if not specified in endpoint
     
     # Submitter contact details
-    contact_name = config.get('submitter_contact_name', 'NONE')
-    contact_telephone_number = config.get('submitter_contact_tel', 'NONE')
+    contact_name = config.get('submitter_name', 'NONE')
+    contact_telephone_number = config.get('submitter_tel', 'NONE')
     
     # Construct NM1 segment for the submitter
     nm1_segment = "NM1*41*2*{}*****{}*{}~".format(submitter_name, submitter_id_qualifier, submitter_id)
     
     # Construct PER segment for the submitter's contact information
     per_segment = "PER*IC*{}*TE*{}~".format(contact_name, contact_telephone_number)
```

### Comparing `medicafe-0.240516.2/MediLink/MediLink_API_v2.py` & `medicafe-0.240517.0/MediLink/MediLink_API_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,16 +68,18 @@
             headers['Content-Type'] = 'application/json'
             response = requests.post(url, headers=headers, json=data)
         elif call_type == 'DELETE':
             response = requests.delete(url, headers=headers)
         else:
             raise ValueError("Unsupported call type")
 
-        # Check for errors in response
-        response.raise_for_status()
+        if response.status_code >= 400:
+            print("Error {}: {}".format(response.status_code, response.text))
+            response.raise_for_status()
+
         return response.json()
 
     # Method for creating coverage
     def create_coverage(self, endpoint_name, patient_info):
         return self.make_api_call(endpoint_name, 'POST', url_extension="/coverages", data=patient_info)
 
     # Method for getting all coverages
```

### Comparing `medicafe-0.240516.2/MediLink/MediLink_APIs.py` & `medicafe-0.240517.0/MediLink/MediLink_APIs.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.2/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240517.0/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.2/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240517.0/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.2/MediLink/MediLink_Down.py` & `medicafe-0.240517.0/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.2/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240517.0/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.2/MediLink/MediLink_Gmail.py` & `medicafe-0.240517.0/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.2/MediLink/MediLink_Scheduler.py` & `medicafe-0.240517.0/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.2/MediLink/MediLink_UI.py` & `medicafe-0.240517.0/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.2/MediLink/MediLink_Up.py` & `medicafe-0.240517.0/MediLink/MediLink_Up.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.2/MediLink/test.py` & `medicafe-0.240517.0/MediLink/test.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.2/PKG-INFO` & `medicafe-0.240517.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240516.2
+Version: 0.240517.0
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240516.2/README.md` & `medicafe-0.240517.0/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.2/medicafe.egg-info/PKG-INFO` & `medicafe-0.240517.0/medicafe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240516.2
+Version: 0.240517.0
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240516.2/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240517.0/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240516.2/setup.py` & `medicafe-0.240517.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240516.2",
+    version="0.240517.0",
     description='MediCafe',
     long_description="""
     # Project Overview: MediCafe
 
     ## Project Description
     MediCafe is a comprehensive suite designed to automate and streamline several aspects of medical administrative tasks within Medisoft, a popular medical practice management software. The system consists of two main components: MediBot and MediLink, each serving distinct functions but integrated to enhance the workflow of medical practices.
```

