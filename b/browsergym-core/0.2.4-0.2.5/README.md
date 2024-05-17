# Comparing `tmp/browsergym_core-0.2.4-py3-none-any.whl.zip` & `tmp/browsergym_core-0.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 181680 bytes, number of entries: 25
+Zip file size: 181682 bytes, number of entries: 25
 -rw-r--r--  2.0 unx      579 b- defN 20-Feb-02 00:00 browsergym/core/__init__.py
 -rw-r--r--  2.0 unx     3438 b- defN 20-Feb-02 00:00 browsergym/core/chat.py
 -rw-r--r--  2.0 unx      253 b- defN 20-Feb-02 00:00 browsergym/core/constants.py
 -rw-r--r--  2.0 unx    21281 b- defN 20-Feb-02 00:00 browsergym/core/env.py
 -rw-r--r--  2.0 unx    20773 b- defN 20-Feb-02 00:00 browsergym/core/observation.py
 -rw-r--r--  2.0 unx      926 b- defN 20-Feb-02 00:00 browsergym/core/registration.py
 -rw-r--r--  2.0 unx     3969 b- defN 20-Feb-02 00:00 browsergym/core/spaces.py
@@ -17,11 +17,11 @@
 -rw-r--r--  2.0 unx   133496 b- defN 20-Feb-02 00:00 browsergym/core/chat_files/assistant.png
 -rw-r--r--  2.0 unx     6687 b- defN 20-Feb-02 00:00 browsergym/core/chat_files/chatbox.html
 -rw-r--r--  2.0 unx    10919 b- defN 20-Feb-02 00:00 browsergym/core/chat_files/chatbox_modern.html
 -rw-r--r--  2.0 unx      643 b- defN 20-Feb-02 00:00 browsergym/core/chat_files/img/send.svg
 -rw-r--r--  2.0 unx    11891 b- defN 20-Feb-02 00:00 browsergym/core/javascript/frame_mark_elements.js
 -rw-r--r--  2.0 unx     1705 b- defN 20-Feb-02 00:00 browsergym/core/javascript/frame_unmark_elements.js
 -rw-r--r--  2.0 unx    18836 b- defN 20-Feb-02 00:00 browsergym/utils/obs.py
-?rw-r--r--  2.0 unx     1167 b- defN 20-Feb-02 00:00 browsergym_core-0.2.4.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 browsergym_core-0.2.4.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2211 b- defN 20-Feb-02 00:00 browsergym_core-0.2.4.dist-info/RECORD
-25 files, 288054 bytes uncompressed, 178076 bytes compressed:  38.2%
+?rw-r--r--  2.0 unx     1167 b- defN 20-Feb-02 00:00 browsergym_core-0.2.5.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 browsergym_core-0.2.5.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2211 b- defN 20-Feb-02 00:00 browsergym_core-0.2.5.dist-info/RECORD
+25 files, 288054 bytes uncompressed, 178078 bytes compressed:  38.2%
```

## zipnote {}

```diff
@@ -60,17 +60,17 @@
 
 Filename: browsergym/core/javascript/frame_unmark_elements.js
 Comment: 
 
 Filename: browsergym/utils/obs.py
 Comment: 
 
-Filename: browsergym_core-0.2.4.dist-info/METADATA
+Filename: browsergym_core-0.2.5.dist-info/METADATA
 Comment: 
 
-Filename: browsergym_core-0.2.4.dist-info/WHEEL
+Filename: browsergym_core-0.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: browsergym_core-0.2.4.dist-info/RECORD
+Filename: browsergym_core-0.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## browsergym/core/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 
 import playwright.sync_api
 
 # we use a global playwright instance
 _PLAYWRIGHT = None
```

## Comparing `browsergym_core-0.2.4.dist-info/METADATA` & `browsergym_core-0.2.5.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: browsergym-core
-Version: 0.2.4
+Version: 0.2.5
 Summary: BrowserGym: a gym environment for web task automation in the Chromium browser
 Project-URL: homepage, https://github.com/ServiceNow/BrowserGym
 Author: Rim Assouel, Léo Boisvert, Massimo Caccia, Alex Drouin, Maxime Gasse, Alex Lacoste, Tom Marty
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `browsergym_core-0.2.4.dist-info/RECORD` & `browsergym_core-0.2.5.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-browsergym/core/__init__.py,sha256=RdhNEd6wih96_1al_zzivkASOLCsuU5aJ58FOE-mz34,579
+browsergym/core/__init__.py,sha256=_QNH094xjsFBdKjpociwAZKBZEUs9oKyahvIGVApiX8,579
 browsergym/core/chat.py,sha256=HuWAWNtqVPb59v82fskPxN_gOyGqD5GDVqvq-eWNT34,3438
 browsergym/core/constants.py,sha256=wWO_e4QpuiHjYYTqA5V7U_uXYJEgGx9AHsdFRP35iYE,253
 browsergym/core/env.py,sha256=-dsbQJ7qOPjYOWJjxTR91hBhn7e9Hgi65hsXRLM2yGw,21281
 browsergym/core/observation.py,sha256=Wi7J_WOjOOelHVlhO0cN3Ad9usF2yipNYm2ZsSPzZ0g,20773
 browsergym/core/registration.py,sha256=vgEFNRJXaiWpNsslb_zOtpirwIyqzYHlybhrKAU_ygE,926
 browsergym/core/spaces.py,sha256=y8ZjVDlAvVrMRQfeeGk0W1eJRuBpMyUWZ5qhLfEHXqc,3969
 browsergym/core/task.py,sha256=D5kjDW5olvPYl2dYf6GlMezQWnF1x6O9BaLggK8aWQQ,3094
@@ -16,10 +16,10 @@
 browsergym/core/chat_files/assistant.png,sha256=7I6eXO_f7i_5yPlZ65IldvtBBDojTNswExL2CYjeY_g,133496
 browsergym/core/chat_files/chatbox.html,sha256=Fqa2Cv3bpUJhiRvqc8kUe_DQ6xnxbAjQk0vgIRjAuMU,6687
 browsergym/core/chat_files/chatbox_modern.html,sha256=q4KVhwYJUFKbXdUKR3I9MqXr5q4iX7Bi0hdtIODgGsc,10919
 browsergym/core/chat_files/img/send.svg,sha256=kNTpxvqiiUK_LbmZrcEEvHaLhdMG2AOT9gNpy6zPLIM,643
 browsergym/core/javascript/frame_mark_elements.js,sha256=wSfW_540t-yjEZG1fuyLSGci12XhQ45voM7Va10j77M,11891
 browsergym/core/javascript/frame_unmark_elements.js,sha256=fgT4in_F3vdCzbMqRsFTsPuKYl9bh5q--bXiovlUbgk,1705
 browsergym/utils/obs.py,sha256=cqH69-D2S53CqX5qW4bPbl3ORjgSc4ih3fkM4QeU0GE,18836
-browsergym_core-0.2.4.dist-info/METADATA,sha256=VLphmh19VhNl7PYbvBTJakIatTHo0Q-rB6FrmCxqcyI,1167
-browsergym_core-0.2.4.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
-browsergym_core-0.2.4.dist-info/RECORD,,
+browsergym_core-0.2.5.dist-info/METADATA,sha256=RuWaR2JNcTgl24UZ6p1reDtY4NuAGVTbAqeLcDTMNz8,1167
+browsergym_core-0.2.5.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+browsergym_core-0.2.5.dist-info/RECORD,,
```

