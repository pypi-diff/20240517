# Comparing `tmp/Moore_SDK-1.0.11-py3-none-any.whl.zip` & `tmp/Moore_SDK-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 52705 bytes, number of entries: 56
+Zip file size: 52746 bytes, number of entries: 56
 -rw-rw-rw-  2.0 fat     6677 b- defN 24-May-13 09:04 moore/__init__.py
 -rw-rw-rw-  2.0 fat       76 b- defN 24-May-13 08:56 moore/_version.py
 -rw-rw-rw-  2.0 fat      837 b- defN 24-May-13 09:02 moore/api.py
 -rw-rw-rw-  2.0 fat       84 b- defN 24-May-13 09:04 moore/const.py
 -rw-rw-rw-  2.0 fat     1014 b- defN 24-May-13 09:02 moore/exception.py
 -rw-rw-rw-  2.0 fat     1851 b- defN 24-May-13 09:04 moore/moore_data.py
 -rw-rw-rw-  2.0 fat       23 b- defN 24-Jan-02 08:40 moore/check/__init__.py
@@ -46,13 +46,13 @@
 -rw-rw-rw-  2.0 fat     2343 b- defN 24-May-13 09:04 moore/visualize/labelme/visual_labelme.py
 -rw-rw-rw-  2.0 fat       48 b- defN 24-Jan-02 08:40 moore/visualize/source/__init__.py
 -rw-rw-rw-  2.0 fat     2691 b- defN 24-May-13 09:04 moore/visualize/source/visual_source.py
 -rw-rw-rw-  2.0 fat       48 b- defN 24-Jan-02 08:40 moore/visualize/voc/__init__.py
 -rw-rw-rw-  2.0 fat     3035 b- defN 24-Jan-02 08:40 moore/visualize/voc/visual_voc.py
 -rw-rw-rw-  2.0 fat       48 b- defN 24-Jan-02 08:40 moore/visualize/yolo/__init__.py
 -rw-rw-rw-  2.0 fat     2213 b- defN 24-Jan-02 08:40 moore/visualize/yolo/visual_yolo.py
--rw-rw-rw-  2.0 fat     1079 b- defN 24-May-17 14:09 Moore_SDK-1.0.11.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2044 b- defN 24-May-17 14:09 Moore_SDK-1.0.11.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-17 14:09 Moore_SDK-1.0.11.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-May-17 14:09 Moore_SDK-1.0.11.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     4830 b- defN 24-May-17 14:09 Moore_SDK-1.0.11.dist-info/RECORD
-56 files, 159088 bytes uncompressed, 44951 bytes compressed:  71.7%
+-rw-rw-rw-  2.0 fat     1079 b- defN 24-May-16 08:02 Moore_SDK-1.0.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2096 b- defN 24-May-16 08:02 Moore_SDK-1.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-16 08:02 Moore_SDK-1.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-May-16 08:02 Moore_SDK-1.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     4825 b- defN 24-May-16 08:02 Moore_SDK-1.0.9.dist-info/RECORD
+56 files, 159135 bytes uncompressed, 45002 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -147,23 +147,23 @@
 
 Filename: moore/visualize/yolo/__init__.py
 Comment: 
 
 Filename: moore/visualize/yolo/visual_yolo.py
 Comment: 
 
-Filename: Moore_SDK-1.0.11.dist-info/LICENSE
+Filename: Moore_SDK-1.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: Moore_SDK-1.0.11.dist-info/METADATA
+Filename: Moore_SDK-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: Moore_SDK-1.0.11.dist-info/WHEEL
+Filename: Moore_SDK-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: Moore_SDK-1.0.11.dist-info/top_level.txt
+Filename: Moore_SDK-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: Moore_SDK-1.0.11.dist-info/RECORD
+Filename: Moore_SDK-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `Moore_SDK-1.0.11.dist-info/LICENSE` & `Moore_SDK-1.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `Moore_SDK-1.0.11.dist-info/RECORD` & `Moore_SDK-1.0.9.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -45,12 +45,12 @@
 moore/visualize/labelme/visual_labelme.py,sha256=IRGZHT9VpOlUVvJvNGYFeK0curME5dIuQoVJUMYSw9U,2343
 moore/visualize/source/__init__.py,sha256=2un8k8GFsH9dCD4_ZThEPCMZq_JL335e0Wzkk034rmo,48
 moore/visualize/source/visual_source.py,sha256=pGyYpBslAhUlWuT-J4vWX5vNzqG8x6sVfJIrt-e_-m0,2691
 moore/visualize/voc/__init__.py,sha256=2un8k8GFsH9dCD4_ZThEPCMZq_JL335e0Wzkk034rmo,48
 moore/visualize/voc/visual_voc.py,sha256=Hsp92kk--tSrVIcTDIR7VV-mEDvn8tyG_FMjEWBVg9k,3035
 moore/visualize/yolo/__init__.py,sha256=2un8k8GFsH9dCD4_ZThEPCMZq_JL335e0Wzkk034rmo,48
 moore/visualize/yolo/visual_yolo.py,sha256=nkrSOnQc0elJCDZUo2gJy_dVg6_6UxzkntQCoL3y9Ts,2213
-Moore_SDK-1.0.11.dist-info/LICENSE,sha256=Jwv3fsn5Tp_DrJRAfUpZCprWtVOZWtWa7IQ2WMuJMZs,1079
-Moore_SDK-1.0.11.dist-info/METADATA,sha256=3k0WTOe7Lh5aMvdiBth3KZvH-a6CYESGoP8OBzbY6rU,2044
-Moore_SDK-1.0.11.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-Moore_SDK-1.0.11.dist-info/top_level.txt,sha256=rLvje0QJ2e4hrGqaQ5xvQb0xC0rH4shSHmk49v3GMDs,6
-Moore_SDK-1.0.11.dist-info/RECORD,,
+Moore_SDK-1.0.9.dist-info/LICENSE,sha256=Jwv3fsn5Tp_DrJRAfUpZCprWtVOZWtWa7IQ2WMuJMZs,1079
+Moore_SDK-1.0.9.dist-info/METADATA,sha256=dbnq4ehlIR34JWa95pjM-AzxU8yi6oGaucQPcKiBgFg,2096
+Moore_SDK-1.0.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+Moore_SDK-1.0.9.dist-info/top_level.txt,sha256=rLvje0QJ2e4hrGqaQ5xvQb0xC0rH4shSHmk49v3GMDs,6
+Moore_SDK-1.0.9.dist-info/RECORD,,
```

