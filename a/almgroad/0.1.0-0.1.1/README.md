# Comparing `tmp/almgroad-0.1.0-py3-none-any.whl.zip` & `tmp/almgroad-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 25003 bytes, number of entries: 11
--rw-rw----  2.0 unx      168 b- defN 24-May-16 19:20 almgroad/__init__.py
+Zip file size: 25924 bytes, number of entries: 12
+-rw-rw----  2.0 unx      212 b- defN 24-May-17 09:16 almgroad/__init__.py
 -rw-rw----  2.0 unx      182 b- defN 24-May-15 18:03 almgroad/chat.py
 -rw-rw----  2.0 unx     1331 b- defN 24-May-16 06:55 almgroad/info_tik.py
 -rw-rw----  2.0 unx     1071 b- defN 24-May-15 04:51 almgroad/infoinsta.py
+-rw-rw----  2.0 unx     1517 b- defN 24-May-17 08:57 almgroad/insta.py
 -rw-rw----  2.0 unx    84898 b- defN 24-May-15 18:03 almgroad/ktkt.py
 -rw-rw----  2.0 unx      460 b- defN 24-May-16 19:19 almgroad/pryer.py
 -rw-rw----  2.0 unx      880 b- defN 24-May-15 18:02 almgroad/tik_tok.py
--rw-rw----  2.0 unx     1434 b- defN 24-May-16 19:21 almgroad-0.1.0.dist-info/METADATA
--rw-rw----  2.0 unx       92 b- defN 24-May-16 19:21 almgroad-0.1.0.dist-info/WHEEL
--rw-rw----  2.0 unx        9 b- defN 24-May-16 19:21 almgroad-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      826 b- defN 24-May-16 19:21 almgroad-0.1.0.dist-info/RECORD
-11 files, 91351 bytes uncompressed, 23623 bytes compressed:  74.1%
+-rw-rw----  2.0 unx     1434 b- defN 24-May-17 09:18 almgroad-0.1.1.dist-info/METADATA
+-rw-rw----  2.0 unx       92 b- defN 24-May-17 09:18 almgroad-0.1.1.dist-info/WHEEL
+-rw-rw----  2.0 unx        9 b- defN 24-May-17 09:18 almgroad-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      900 b- defN 24-May-17 09:18 almgroad-0.1.1.dist-info/RECORD
+12 files, 92986 bytes uncompressed, 24434 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -6,29 +6,32 @@
 
 Filename: almgroad/info_tik.py
 Comment: 
 
 Filename: almgroad/infoinsta.py
 Comment: 
 
+Filename: almgroad/insta.py
+Comment: 
+
 Filename: almgroad/ktkt.py
 Comment: 
 
 Filename: almgroad/pryer.py
 Comment: 
 
 Filename: almgroad/tik_tok.py
 Comment: 
 
-Filename: almgroad-0.1.0.dist-info/METADATA
+Filename: almgroad-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: almgroad-0.1.0.dist-info/WHEEL
+Filename: almgroad-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: almgroad-0.1.0.dist-info/top_level.txt
+Filename: almgroad-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: almgroad-0.1.0.dist-info/RECORD
+Filename: almgroad-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## almgroad/__init__.py

```diff
@@ -1,6 +1,8 @@
 from .infoinsta import Info_Insta
 from .chat import GPT
 from .ktkt import kt
 from .tik_tok import Tik_Tok
 from .info_tik import Info_Tik
-from .pryer import prayer_times
+from .pryer import prayer_times
+from .insta import instagram
+import asyncio
```

## Comparing `almgroad-0.1.0.dist-info/METADATA` & `almgroad-0.1.1.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almgroad
-Version: 0.1.0
+Version: 0.1.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Ibrahim Mohammed
 Author-email: ibrahom0780@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `almgroad-0.1.0.dist-info/RECORD` & `almgroad-0.1.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-almgroad/__init__.py,sha256=qHkZRljXCGqGVzJAXDrSbmWFGNcD3S31fdUa9NwvUwk,168
+almgroad/__init__.py,sha256=vJ0uzJnFBs78z-7QQC62hCvD5_9RDtnB61RykfwowqU,212
 almgroad/chat.py,sha256=QOkrkf2gUrcjSstul9hqhPWkTREsasSilv5nMvp_sq4,182
 almgroad/info_tik.py,sha256=dURJKszAIWQPeuHpgVHADcNTz4sTpFWbkxqvwH0RAo4,1331
 almgroad/infoinsta.py,sha256=DzqhmwPWbeBrSXoSZp9DsZQiVC6Nlx8PnZn9wM8sNrM,1071
+almgroad/insta.py,sha256=MKOPtEn7YRFm79pluSNKP1-d_-HYiKkVlpAx_9qz4GM,1517
 almgroad/ktkt.py,sha256=CoUbwbOAd18fMb2fTVPr3BHt81DR43hnSvNuKywcSlU,84898
 almgroad/pryer.py,sha256=jM3M_7DThca_-FvYOMuOnSelTUR49MnDxHYlS9k-6S4,460
 almgroad/tik_tok.py,sha256=22laOxfsGV1NhHq7YCQqxl3ZDxIBoGQtP9FSNffgEpI,880
-almgroad-0.1.0.dist-info/METADATA,sha256=j_nQguTKx7G1GJ3GeEUg_lU_r2Qw_a_nIooFwN0OhTI,1434
-almgroad-0.1.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-almgroad-0.1.0.dist-info/top_level.txt,sha256=Sp5hguX1HExRTUrSZFyTESQ8fyBMsW2XsjXu84UhJ-w,9
-almgroad-0.1.0.dist-info/RECORD,,
+almgroad-0.1.1.dist-info/METADATA,sha256=nb5dLYinIxKBl1v7cOgGH0BRuz8Im5lRnDvLZjWiKvc,1434
+almgroad-0.1.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+almgroad-0.1.1.dist-info/top_level.txt,sha256=Sp5hguX1HExRTUrSZFyTESQ8fyBMsW2XsjXu84UhJ-w,9
+almgroad-0.1.1.dist-info/RECORD,,
```

