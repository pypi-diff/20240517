# Comparing `tmp/almgroad-0.0.9-py3-none-any.whl.zip` & `tmp/almgroad-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 24504 bytes, number of entries: 10
--rw-rw----  2.0 unx      136 b- defN 24-May-16 06:56 almgroad/__init__.py
+Zip file size: 25003 bytes, number of entries: 11
+-rw-rw----  2.0 unx      168 b- defN 24-May-16 19:20 almgroad/__init__.py
 -rw-rw----  2.0 unx      182 b- defN 24-May-15 18:03 almgroad/chat.py
 -rw-rw----  2.0 unx     1331 b- defN 24-May-16 06:55 almgroad/info_tik.py
 -rw-rw----  2.0 unx     1071 b- defN 24-May-15 04:51 almgroad/infoinsta.py
 -rw-rw----  2.0 unx    84898 b- defN 24-May-15 18:03 almgroad/ktkt.py
+-rw-rw----  2.0 unx      460 b- defN 24-May-16 19:19 almgroad/pryer.py
 -rw-rw----  2.0 unx      880 b- defN 24-May-15 18:02 almgroad/tik_tok.py
--rw-rw----  2.0 unx     1434 b- defN 24-May-16 06:57 almgroad-0.0.9.dist-info/METADATA
--rw-rw----  2.0 unx       92 b- defN 24-May-16 06:57 almgroad-0.0.9.dist-info/WHEEL
--rw-rw----  2.0 unx        9 b- defN 24-May-16 06:57 almgroad-0.0.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      753 b- defN 24-May-16 06:57 almgroad-0.0.9.dist-info/RECORD
-10 files, 90786 bytes uncompressed, 23234 bytes compressed:  74.4%
+-rw-rw----  2.0 unx     1434 b- defN 24-May-16 19:21 almgroad-0.1.0.dist-info/METADATA
+-rw-rw----  2.0 unx       92 b- defN 24-May-16 19:21 almgroad-0.1.0.dist-info/WHEEL
+-rw-rw----  2.0 unx        9 b- defN 24-May-16 19:21 almgroad-0.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      826 b- defN 24-May-16 19:21 almgroad-0.1.0.dist-info/RECORD
+11 files, 91351 bytes uncompressed, 23623 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -9,23 +9,26 @@
 
 Filename: almgroad/infoinsta.py
 Comment: 
 
 Filename: almgroad/ktkt.py
 Comment: 
 
+Filename: almgroad/pryer.py
+Comment: 
+
 Filename: almgroad/tik_tok.py
 Comment: 
 
-Filename: almgroad-0.0.9.dist-info/METADATA
+Filename: almgroad-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: almgroad-0.0.9.dist-info/WHEEL
+Filename: almgroad-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: almgroad-0.0.9.dist-info/top_level.txt
+Filename: almgroad-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: almgroad-0.0.9.dist-info/RECORD
+Filename: almgroad-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## almgroad/__init__.py

```diff
@@ -1,5 +1,6 @@
 from .infoinsta import Info_Insta
 from .chat import GPT
 from .ktkt import kt
 from .tik_tok import Tik_Tok
-from .info_tik import Info_Tik
+from .info_tik import Info_Tik
+from .pryer import prayer_times
```

## Comparing `almgroad-0.0.9.dist-info/METADATA` & `almgroad-0.1.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almgroad
-Version: 0.0.9
+Version: 0.1.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Ibrahim Mohammed
 Author-email: ibrahom0780@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

