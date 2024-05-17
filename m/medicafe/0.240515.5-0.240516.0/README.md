# Comparing `tmp/medicafe-0.240515.5.tar.gz` & `tmp/medicafe-0.240516.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240515.5.tar", last modified: Thu May 16 01:38:55 2024, max compression
+gzip compressed data, was "medicafe-0.240516.0.tar", last modified: Thu May 16 23:59:16 2024, max compression
```

## Comparing `medicafe-0.240515.5.tar` & `medicafe-0.240516.0.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 01:38:55.685000 medicafe-0.240515.5/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240515.5/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240515.5/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-16 01:38:54.728000 medicafe-0.240515.5/MediBot/
--rwxrwxrwx   0        0        0     5972 2024-05-12 18:02:44.000000 medicafe-0.240515.5/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    17490 2024-05-15 17:01:43.000000 medicafe-0.240515.5/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240515.5/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    14538 2024-05-15 19:07:33.000000 medicafe-0.240515.5/MediBot/MediBot_Crosswalk_Library.py
--rw-rw-rw-   0        0        0    14906 2024-05-15 16:48:28.000000 medicafe-0.240515.5/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0    17184 2024-05-15 17:38:32.000000 medicafe-0.240515.5/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0    10660 2024-05-16 01:23:48.000000 medicafe-0.240515.5/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     8912 2024-05-15 20:14:35.000000 medicafe-0.240515.5/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240515.5/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240515.5/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240515.5/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240515.5/MediBot/update_json.py
--rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240515.5/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-16 01:38:55.434000 medicafe-0.240515.5/MediLink/
--rw-rw-rw-   0        0        0    20316 2024-05-16 01:29:43.000000 medicafe-0.240515.5/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240515.5/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    25526 2024-05-16 00:37:08.000000 medicafe-0.240515.5/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    43551 2024-05-16 00:36:51.000000 medicafe-0.240515.5/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     6166 2024-05-15 17:49:28.000000 medicafe-0.240515.5/MediLink/MediLink_APIs.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240515.5/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    12235 2024-05-14 15:14:04.000000 medicafe-0.240515.5/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7248 2024-05-15 07:47:12.000000 medicafe-0.240515.5/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8710 2024-05-15 13:36:03.000000 medicafe-0.240515.5/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240515.5/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0      370 2024-05-14 22:24:45.000000 medicafe-0.240515.5/MediLink/MediLink_Mailer.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240515.5/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240515.5/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240515.5/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0    19286 2024-05-16 01:21:31.000000 medicafe-0.240515.5/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240515.5/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240515.5/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240515.5/MediLink/__init__.py
--rw-rw-rw-   0        0        0     3108 2024-05-13 04:52:22.000000 medicafe-0.240515.5/MediLink/test.py
--rw-rw-rw-   0        0        0     4396 2024-05-16 01:38:55.664000 medicafe-0.240515.5/PKG-INFO
--rw-rw-rw-   0        0        0     2960 2024-05-13 07:31:39.000000 medicafe-0.240515.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 01:38:55.641000 medicafe-0.240515.5/medicafe.egg-info/
--rw-rw-rw-   0        0        0     4396 2024-05-16 01:38:53.000000 medicafe-0.240515.5/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1114 2024-05-16 01:38:54.000000 medicafe-0.240515.5/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 01:38:53.000000 medicafe-0.240515.5/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240515.5/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-16 01:38:53.000000 medicafe-0.240515.5/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-16 01:38:53.000000 medicafe-0.240515.5/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 01:38:55.680000 medicafe-0.240515.5/setup.cfg
--rw-rw-rw-   0        0        0     4834 2024-05-16 01:38:52.000000 medicafe-0.240515.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 23:59:16.791000 medicafe-0.240516.0/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240516.0/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240516.0/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-16 23:59:15.977000 medicafe-0.240516.0/MediBot/
+-rwxrwxrwx   0        0        0     5972 2024-05-12 18:02:44.000000 medicafe-0.240516.0/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    17490 2024-05-15 17:01:43.000000 medicafe-0.240516.0/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240516.0/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    14544 2024-05-16 23:40:08.000000 medicafe-0.240516.0/MediBot/MediBot_Crosswalk_Library.py
+-rw-rw-rw-   0        0        0    14906 2024-05-15 16:48:28.000000 medicafe-0.240516.0/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0    17184 2024-05-15 17:38:32.000000 medicafe-0.240516.0/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10660 2024-05-16 01:23:48.000000 medicafe-0.240516.0/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     8912 2024-05-15 20:14:35.000000 medicafe-0.240516.0/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0     3049 2024-05-16 17:42:31.000000 medicafe-0.240516.0/MediBot/MediBot_docx_decoder.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240516.0/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240516.0/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240516.0/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240516.0/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240516.0/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-16 23:59:16.593000 medicafe-0.240516.0/MediLink/
+-rw-rw-rw-   0        0        0    20316 2024-05-16 01:29:43.000000 medicafe-0.240516.0/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240516.0/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    25526 2024-05-16 00:37:08.000000 medicafe-0.240516.0/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    43553 2024-05-16 23:40:06.000000 medicafe-0.240516.0/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     6127 2024-05-16 23:37:38.000000 medicafe-0.240516.0/MediLink/MediLink_API_v2.py
+-rw-rw-rw-   0        0        0     6166 2024-05-15 17:49:28.000000 medicafe-0.240516.0/MediLink/MediLink_APIs.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240516.0/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    12235 2024-05-14 15:14:04.000000 medicafe-0.240516.0/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7248 2024-05-15 07:47:12.000000 medicafe-0.240516.0/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8710 2024-05-15 13:36:03.000000 medicafe-0.240516.0/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     6370 2024-05-16 17:44:21.000000 medicafe-0.240516.0/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0      370 2024-05-14 22:24:45.000000 medicafe-0.240516.0/MediLink/MediLink_Mailer.py
+-rw-rw-rw-   0        0        0     7368 2024-05-16 18:14:48.000000 medicafe-0.240516.0/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240516.0/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240516.0/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0    19286 2024-05-16 01:21:31.000000 medicafe-0.240516.0/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240516.0/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240516.0/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240516.0/MediLink/__init__.py
+-rw-rw-rw-   0        0        0     3108 2024-05-13 04:52:22.000000 medicafe-0.240516.0/MediLink/test.py
+-rw-rw-rw-   0        0        0     4396 2024-05-16 23:59:16.776000 medicafe-0.240516.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2960 2024-05-13 07:31:39.000000 medicafe-0.240516.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 23:59:16.760000 medicafe-0.240516.0/medicafe.egg-info/
+-rw-rw-rw-   0        0        0     4396 2024-05-16 23:59:15.000000 medicafe-0.240516.0/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1174 2024-05-16 23:59:15.000000 medicafe-0.240516.0/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 23:59:15.000000 medicafe-0.240516.0/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240516.0/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-16 23:59:15.000000 medicafe-0.240516.0/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-16 23:59:15.000000 medicafe-0.240516.0/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 23:59:16.787000 medicafe-0.240516.0/setup.cfg
+-rw-rw-rw-   0        0        0     4834 2024-05-16 23:59:12.000000 medicafe-0.240516.0/setup.py
```

### Comparing `medicafe-0.240515.5/LICENSE` & `medicafe-0.240516.0/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.5/MediBot/MediBot.bat` & `medicafe-0.240516.0/MediBot/MediBot.bat`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.5/MediBot/MediBot.py` & `medicafe-0.240516.0/MediBot/MediBot.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.5/MediBot/MediBot_Charges.py` & `medicafe-0.240516.0/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.5/MediBot/MediBot_Crosswalk_Library.py` & `medicafe-0.240516.0/MediBot/MediBot_Crosswalk_Library.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 
 try:
     import MediLink_ConfigLoader
 except ImportError:
     from MediLink import MediLink_ConfigLoader
 
 try:
-    from MediLink_APIs import fetch_payer_name_from_api
+    from MediLink_API_v2 import fetch_payer_name_from_api
 except ImportError:
-    from MediLink import MediLink_APIs
-    fetch_payer_name_from_api = MediLink_APIs.fetch_payer_name_from_api
+    from MediLink import MediLink_API_v2
+    fetch_payer_name_from_api = MediLink_API_v2.fetch_payer_name_from_api
 
 try:
     from MediBot import MediBot_Preprocessor_lib
 except ImportError:
     import MediBot_Preprocessor_lib
 
 def check_and_initialize_crosswalk(config):
```

### Comparing `medicafe-0.240515.5/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240516.0/MediBot/MediBot_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.5/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240516.0/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.5/MediBot/MediBot_UI.py` & `medicafe-0.240516.0/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.5/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240516.0/MediBot/MediBot_dataformat_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.5/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240516.0/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.5/MediBot/update_json.py` & `medicafe-0.240516.0/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.5/MediBot/update_medicafe.py` & `medicafe-0.240516.0/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.5/MediLink/MediLink.py` & `medicafe-0.240516.0/MediLink/MediLink.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.5/MediLink/MediLink_277_decoder.py` & `medicafe-0.240516.0/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.5/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240516.0/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.5/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240516.0/MediLink/MediLink_837p_encoder_library.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 project_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
 sys.path.append(project_dir)
 
 from MediBot import MediBot_Preprocessor_lib
 load_insurance_data_from_mains = MediBot_Preprocessor_lib.load_insurance_data_from_mains
 from MediBot import MediBot_Crosswalk_Library
-from MediLink_APIs import fetch_payer_name_from_api
+from MediLink_API_v2 import fetch_payer_name_from_api
 
 """
 - [ ] 1. Code Refactoring: Increase modularity and clarity, particularly in segment creation functions (e.g., `create_st_segment`, `create_nm1_billing_provider_segment`), for better maintenance and readability.
 - [ ] 2. Endpoint Support: Extend support within segment creation for additional endpoints with attention to their unique claim submission requirements.
 - [ ] 3. Payer Identification Mechanism: Refine the mechanism for dynamically identifying payers, leveraging payer mappings and integrating with external APIs like Availity for precise payer information retrieval.
 - [ ] 4. Adherence to Endpoint-Specific Standards: Implement and verify the compliance of claim data formatting and inclusion based on the specific demands of each target endpoint within the segment creation logic.
 - [ ] 5. De-persisting Intermediate Files.
```

### Comparing `medicafe-0.240515.5/MediLink/MediLink_APIs.py` & `medicafe-0.240516.0/MediLink/MediLink_APIs.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.5/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240516.0/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.5/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240516.0/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.5/MediLink/MediLink_Down.py` & `medicafe-0.240516.0/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.5/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240516.0/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.5/MediLink/MediLink_Gmail.py` & `medicafe-0.240516.0/MediLink/MediLink_Gmail.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 3. **Python Script (Client-side)**:
     - Interfaces with the server-side web app to initiate processes like link retrieval.
     - Manages opening URLs in the user's browser, allowing for interaction with the web app directly from the client-side 
         environment.
 
 **Future Work:**
+- [ ] Consider disabling OTP triggers for now since we don't really use it for the present implementation. The phone solution works.
 - [ ] Implement and troubleshoot the OTP extraction and validation system to fully automate the secured content retrieval process.
 - [X] Gmail Server-side Authentication flow & Webapp build
 - [X] Upgrade to handle multiple possible emails selection
 - [ ] Augment to detect Surgery Schedule emails with doc attachments that don't require OTP.
 - [X] Upgrade Gmail query to only get emails with the protected links.
 - [ ] Something that goes here that I forgot.
```

### Comparing `medicafe-0.240515.5/MediLink/MediLink_Scheduler.py` & `medicafe-0.240516.0/MediLink/MediLink_Scheduler.py`

 * *Files 14% similar despite different names*

```diff
@@ -58,14 +58,55 @@
 Database Management:
 - Maintains a JSON-based database for patient billing data, labeled as patient_billing_db, storing information from various sources (Z.dat file, APIs, SFTP).
 - Database content includes claim statuses, deductible details, error logs, and identifiers for billing readiness.
 - Facilitates efficient tracking and processing of claims, with considerations for integrating individual patient data in batched submissions.
 - Stays on the local machine in a defined secure location per config, ensuring HIPAA compliance without the need for data encryption at rest.
 
 Note: Potential for data corruption or synchronization issues due to system limitations; backup and manual verification measures are advised.
+
+Crosswalk Example:
+    "payer_id": {
+        "87726": {
+            "medisoft_medicare_id": [],
+            "medisoft_id": [
+                "320"
+            ],
+            "endpoint": "OPTUMEDI"
+        },
+        "60054": {
+            "medisoft_medicare_id": [],
+            "medisoft_id": [
+                "369"
+            ],
+            "endpoint": "OPTUMEDI"
+        },
+        "00590": {
+            "medisoft_medicare_id": [],
+            "medisoft_id": [
+                "317"
+            ],
+            "endpoint": "OPTUMEDI"
+        },
+        
+
+Crosswalk add:
+- submit_buffer_maria per payer_id
+- submit_limit_days per payer_id
+- deductible_max = $2500.
+- submit limit buffer = 15 days before final.
+
+MediLink_Scheduler logic to produce dates of submission:
+deductible slows it until a max limit ($2500), then send anyway.
+after maria buffer, before submit (-15?) limit day.
+Maria collects pre-payment, this is a factor, needs to be somehow accounted for in the process where a quantity gets pre-assigned to a patient so we know when to submit the claim.
+
+Date last reviewed, Insurance Type, In network, Annual Deductable Remaining, Recieved pre-payment amount, Check# or 'Cash'.
+
+In the future those pre-payments should be either eCheck, Zelle or by CC + 5% surcharge.
+
 """
 
 
 # JSON DB structure draft.
 {
   "patients": {
     "patient_id": {
```

### Comparing `medicafe-0.240515.5/MediLink/MediLink_UI.py` & `medicafe-0.240516.0/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.5/MediLink/MediLink_Up.py` & `medicafe-0.240516.0/MediLink/MediLink_Up.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.5/MediLink/test.py` & `medicafe-0.240516.0/MediLink/test.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.5/PKG-INFO` & `medicafe-0.240516.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240515.5
+Version: 0.240516.0
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240515.5/README.md` & `medicafe-0.240516.0/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240515.5/medicafe.egg-info/PKG-INFO` & `medicafe-0.240516.0/medicafe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240515.5
+Version: 0.240516.0
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240515.5/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240516.0/medicafe.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 MediBot/MediBot.py
 MediBot/MediBot_Charges.py
 MediBot/MediBot_Crosswalk_Library.py
 MediBot/MediBot_Preprocessor.py
 MediBot/MediBot_Preprocessor_lib.py
 MediBot/MediBot_UI.py
 MediBot/MediBot_dataformat_library.py
+MediBot/MediBot_docx_decoder.py
 MediBot/MediPost.py
 MediBot/PDF_to_CSV_Cleaner.py
 MediBot/__init__.py
 MediBot/update_json.py
 MediBot/update_medicafe.py
 MediLink/MediLink.py
 MediLink/MediLink_277_decoder.py
 MediLink/MediLink_837p_encoder.py
 MediLink/MediLink_837p_encoder_library.py
+MediLink/MediLink_API_v2.py
 MediLink/MediLink_APIs.py
 MediLink/MediLink_ConfigLoader.py
 MediLink/MediLink_DataMgmt.py
 MediLink/MediLink_Down.py
 MediLink/MediLink_ERA_decoder.py
 MediLink/MediLink_Gmail.py
 MediLink/MediLink_Mailer.py
```

### Comparing `medicafe-0.240515.5/setup.py` & `medicafe-0.240516.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240515.5",
+    version="0.240516.0",
     description='MediCafe',
     long_description="""
     # Project Overview: MediCafe
 
     ## Project Description
     MediCafe is a comprehensive suite designed to automate and streamline several aspects of medical administrative tasks within Medisoft, a popular medical practice management software. The system consists of two main components: MediBot and MediLink, each serving distinct functions but integrated to enhance the workflow of medical practices.
```

