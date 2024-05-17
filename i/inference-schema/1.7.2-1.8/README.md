# Comparing `tmp/inference_schema-1.7.2-py3-none-any.whl.zip` & `tmp/inference_schema-1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 21385 bytes, number of entries: 18
+Zip file size: 21360 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat      183 b- defN 22-Feb-04 18:09 inference_schema/__init__.py
 -rw-rw-rw-  2.0 fat      307 b- defN 22-Oct-28 16:24 inference_schema/_constants.py
 -rw-rw-rw-  2.0 fat    13098 b- defN 24-Apr-03 19:49 inference_schema/schema_decorators.py
 -rw-rw-rw-  2.0 fat     4189 b- defN 22-Oct-28 16:24 inference_schema/schema_util.py
 -rw-rw-rw-  2.0 fat      421 b- defN 22-Feb-04 18:09 inference_schema/parameter_types/__init__.py
 -rw-rw-rw-  2.0 fat      642 b- defN 22-Feb-04 18:09 inference_schema/parameter_types/_constants.py
 -rw-rw-rw-  2.0 fat     4001 b- defN 22-Feb-04 18:09 inference_schema/parameter_types/_swagger_from_dtype.py
 -rw-rw-rw-  2.0 fat     4446 b- defN 22-Oct-28 16:24 inference_schema/parameter_types/_util.py
 -rw-rw-rw-  2.0 fat     5229 b- defN 22-Apr-14 14:38 inference_schema/parameter_types/abstract_parameter_type.py
 -rw-rw-rw-  2.0 fat     6953 b- defN 22-Feb-04 18:09 inference_schema/parameter_types/numpy_parameter_type.py
 -rw-rw-rw-  2.0 fat     9372 b- defN 23-Jul-21 21:43 inference_schema/parameter_types/pandas_parameter_type.py
 -rw-rw-rw-  2.0 fat     9647 b- defN 22-Feb-04 18:09 inference_schema/parameter_types/spark_parameter_type.py
 -rw-rw-rw-  2.0 fat     3456 b- defN 22-Mar-28 20:14 inference_schema/parameter_types/standard_py_parameter_type.py
--rw-rw-rw-  2.0 fat     1183 b- defN 24-Apr-03 19:49 inference_schema-1.7.2.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     2451 b- defN 24-Apr-03 19:49 inference_schema-1.7.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-03 19:49 inference_schema-1.7.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 24-Apr-03 19:49 inference_schema-1.7.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1775 b- defN 24-Apr-03 19:49 inference_schema-1.7.2.dist-info/RECORD
-18 files, 67462 bytes uncompressed, 18375 bytes compressed:  72.8%
+-rw-rw-rw-  2.0 fat     1183 b- defN 24-May-17 17:50 inference_schema-1.8.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     2494 b- defN 24-May-17 17:50 inference_schema-1.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-17 17:50 inference_schema-1.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 24-May-17 17:50 inference_schema-1.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1765 b- defN 24-May-17 17:50 inference_schema-1.8.dist-info/RECORD
+18 files, 67495 bytes uncompressed, 18370 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: inference_schema/parameter_types/spark_parameter_type.py
 Comment: 
 
 Filename: inference_schema/parameter_types/standard_py_parameter_type.py
 Comment: 
 
-Filename: inference_schema-1.7.2.dist-info/LICENSE.txt
+Filename: inference_schema-1.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: inference_schema-1.7.2.dist-info/METADATA
+Filename: inference_schema-1.8.dist-info/METADATA
 Comment: 
 
-Filename: inference_schema-1.7.2.dist-info/WHEEL
+Filename: inference_schema-1.8.dist-info/WHEEL
 Comment: 
 
-Filename: inference_schema-1.7.2.dist-info/top_level.txt
+Filename: inference_schema-1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: inference_schema-1.7.2.dist-info/RECORD
+Filename: inference_schema-1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `inference_schema-1.7.2.dist-info/LICENSE.txt` & `inference_schema-1.8.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `inference_schema-1.7.2.dist-info/METADATA` & `inference_schema-1.8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inference-schema
-Version: 1.7.2
+Version: 1.8
 Summary: This package is intended to provide a uniform schema for common machine learning applications, as well as a set of decorators that can be used to aid in web based ML prediction applications.
 Author: Microsoft Corp
 License: MIT License        
             Copyright (c) Microsoft Corporation. All rights reserved.        
             Permission is hereby granted, free of charge, to any person obtaining a copy
             of this software and associated documentation files (the "Software"), to deal
             in the Software without restriction, including without limitation the rights
@@ -24,15 +24,16 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8,<3.12
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 License-File: LICENSE.txt
 Requires-Dist: python-dateutil (>=2.5.3)
 Requires-Dist: pytz (>=2017.2)
 Requires-Dist: wrapt (<=1.16.0,>=1.14.0)
 Provides-Extra: numpy-support
 Requires-Dist: numpy (>=1.13.0) ; extra == 'numpy-support'
 Provides-Extra: pandas-support
```

## Comparing `inference_schema-1.7.2.dist-info/RECORD` & `inference_schema-1.8.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -7,12 +7,12 @@
 inference_schema/parameter_types/_swagger_from_dtype.py,sha256=WWYVGo6-KiGoPg0CMmM3RBa_WTtbS33lTV9PS-dQ5T0,4001
 inference_schema/parameter_types/_util.py,sha256=vXKbnsTbVBpxrhBXpIHycKxYzBl1PE04dtWtQLY6G6M,4446
 inference_schema/parameter_types/abstract_parameter_type.py,sha256=qkdLkYgXlIHFA-NxGOTkYmG6FK-qdFgPenn9HMJrTzo,5229
 inference_schema/parameter_types/numpy_parameter_type.py,sha256=goBx3Vzti-9jlKvMPn55t4SS5FF416-tq-ZGEpAjb_Q,6953
 inference_schema/parameter_types/pandas_parameter_type.py,sha256=wPYgg7IlbJq6VAQB6wRQ_fj2Wvxfpu3RcJ9gpmMVjh4,9372
 inference_schema/parameter_types/spark_parameter_type.py,sha256=vVmYWZFRSNCReouZiS1cGoR30NGu5OJlPyvQ_flgY2g,9647
 inference_schema/parameter_types/standard_py_parameter_type.py,sha256=DO5Ty02A0D5zjt4ODodxw6WeOA7r2QyfK-NswN9yOzI,3456
-inference_schema-1.7.2.dist-info/LICENSE.txt,sha256=3qkmU0GCkALiwjpzcjk-su1uJghftiPzikugr4M_MKY,1183
-inference_schema-1.7.2.dist-info/METADATA,sha256=e4-vnUtGZqvagCTGUctyKEP_3ivA1UnVqljDX2V0Q8U,2451
-inference_schema-1.7.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-inference_schema-1.7.2.dist-info/top_level.txt,sha256=VppQqI390J43UCHv4CcDtEGPp8EktkSEi5Q80wWYq9M,17
-inference_schema-1.7.2.dist-info/RECORD,,
+inference_schema-1.8.dist-info/LICENSE.txt,sha256=3qkmU0GCkALiwjpzcjk-su1uJghftiPzikugr4M_MKY,1183
+inference_schema-1.8.dist-info/METADATA,sha256=LHpqoi0t8HnEpxkNFpIbmaswxM4WBcOCE87lBHh4FuA,2494
+inference_schema-1.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+inference_schema-1.8.dist-info/top_level.txt,sha256=VppQqI390J43UCHv4CcDtEGPp8EktkSEi5Q80wWYq9M,17
+inference_schema-1.8.dist-info/RECORD,,
```

