# Comparing `tmp/gendc_python-0.2.4-py3-none-any.whl.zip` & `tmp/gendc_python-0.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 8017 bytes, number of entries: 11
--rw-r--r--  2.0 unx       52 b- defN 24-May-16 18:29 gendc_python/__init__.py
--rw-r--r--  2.0 unx       34 b- defN 24-May-16 18:29 gendc_python/gendc_separator/__init__.py
--rw-r--r--  2.0 unx     2534 b- defN 24-May-16 18:29 gendc_python/gendc_separator/component.py
--rw-r--r--  2.0 unx     3798 b- defN 24-May-16 18:29 gendc_python/gendc_separator/descriptor.py
--rw-r--r--  2.0 unx     3540 b- defN 24-May-16 18:29 gendc_python/gendc_separator/part.py
--rw-r--r--  2.0 unx     1313 b- defN 24-May-16 18:29 gendc_python/gendc_separator/utils.py
--rw-r--r--  2.0 unx     1070 b- defN 24-May-16 18:29 gendc_python-0.2.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     8712 b- defN 24-May-16 18:29 gendc_python-0.2.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-16 18:29 gendc_python-0.2.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-May-16 18:29 gendc_python-0.2.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      973 b- defN 24-May-16 18:29 gendc_python-0.2.4.dist-info/RECORD
+-rw-r--r--  2.0 unx       52 b- defN 24-May-16 22:43 gendc_python/__init__.py
+-rw-r--r--  2.0 unx       34 b- defN 24-May-16 22:43 gendc_python/gendc_separator/__init__.py
+-rw-r--r--  2.0 unx     2534 b- defN 24-May-16 22:43 gendc_python/gendc_separator/component.py
+-rw-r--r--  2.0 unx     3798 b- defN 24-May-16 22:43 gendc_python/gendc_separator/descriptor.py
+-rw-r--r--  2.0 unx     3540 b- defN 24-May-16 22:43 gendc_python/gendc_separator/part.py
+-rw-r--r--  2.0 unx     1313 b- defN 24-May-16 22:43 gendc_python/gendc_separator/utils.py
+-rw-r--r--  2.0 unx     1070 b- defN 24-May-16 22:43 gendc_python-0.2.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     8712 b- defN 24-May-16 22:43 gendc_python-0.2.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-16 22:43 gendc_python-0.2.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-May-16 22:43 gendc_python-0.2.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      973 b- defN 24-May-16 22:43 gendc_python-0.2.5.dist-info/RECORD
 11 files, 22131 bytes uncompressed, 6343 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: gendc_python/gendc_separator/part.py
 Comment: 
 
 Filename: gendc_python/gendc_separator/utils.py
 Comment: 
 
-Filename: gendc_python-0.2.4.dist-info/LICENSE.txt
+Filename: gendc_python-0.2.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: gendc_python-0.2.4.dist-info/METADATA
+Filename: gendc_python-0.2.5.dist-info/METADATA
 Comment: 
 
-Filename: gendc_python-0.2.4.dist-info/WHEEL
+Filename: gendc_python-0.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: gendc_python-0.2.4.dist-info/top_level.txt
+Filename: gendc_python-0.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: gendc_python-0.2.4.dist-info/RECORD
+Filename: gendc_python-0.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gendc_python/__init__.py

```diff
@@ -1,2 +1,2 @@
-__version__ = '0.2.4'
+__version__ = '0.2.5'
 from . import gendc_separator
```

## Comparing `gendc_python-0.2.4.dist-info/LICENSE.txt` & `gendc_python-0.2.5.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `gendc_python-0.2.4.dist-info/METADATA` & `gendc_python-0.2.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gendc-python
-Version: 0.2.4
+Version: 0.2.5
 Summary: GenDC Python package
 Author-email: Momoko Kono <momoko.kono@fixstars.com>
 License: MIT License
         
         Copyright (c) Olli-Pekka Heinisuo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

## Comparing `gendc_python-0.2.4.dist-info/RECORD` & `gendc_python-0.2.5.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-gendc_python/__init__.py,sha256=znVyvV6yIT02mjenHAJyBN7zO2aE-v_EScvQpPsqHCY,52
+gendc_python/__init__.py,sha256=ZLsI4O4Pe6WxlxM1JjAN7lwqyIyXILOFLyASht3h5bY,52
 gendc_python/gendc_separator/__init__.py,sha256=ENTmzRdCKWv0RfDY8WnzaiwvZ0tEitTsYDQJiXArU9w,34
 gendc_python/gendc_separator/component.py,sha256=OXVtRtW33xWbRyb_eQZC_q0KNdmAn-fzMpgOK0KnOe8,2534
 gendc_python/gendc_separator/descriptor.py,sha256=ZHdePtY6pWZPbOHeoGq3TEIm2lrTOS5eusZDx7w4V0Y,3798
 gendc_python/gendc_separator/part.py,sha256=JPz9WuZGRqvmAk1WhqQGohG7Cr6zqMpUBkhyX9Bwr1I,3540
 gendc_python/gendc_separator/utils.py,sha256=3F6DcNJjYrcWBWMAx9KEEanDOVOnoVK9oZtavIhv57w,1313
-gendc_python-0.2.4.dist-info/LICENSE.txt,sha256=CdcZBY54Kse8cbohyUThE2zeK7lXwOiIEh8CGNa18Cw,1070
-gendc_python-0.2.4.dist-info/METADATA,sha256=xY9-OnTX3elDR-7AbMsxcVcHRmf0LP0Z0OXp_E_5INA,8712
-gendc_python-0.2.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-gendc_python-0.2.4.dist-info/top_level.txt,sha256=HKTB6hISpv3f-3THLIPKPYvaZzcHVGNM1hznVOVy0bY,13
-gendc_python-0.2.4.dist-info/RECORD,,
+gendc_python-0.2.5.dist-info/LICENSE.txt,sha256=CdcZBY54Kse8cbohyUThE2zeK7lXwOiIEh8CGNa18Cw,1070
+gendc_python-0.2.5.dist-info/METADATA,sha256=56nYWvK8SiJb6vfaKIE2F4R1OVmRErDjVD7RTCYI-vg,8712
+gendc_python-0.2.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+gendc_python-0.2.5.dist-info/top_level.txt,sha256=HKTB6hISpv3f-3THLIPKPYvaZzcHVGNM1hznVOVy0bY,13
+gendc_python-0.2.5.dist-info/RECORD,,
```

