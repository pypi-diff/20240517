# Comparing `tmp/TurboTouchPredictor-0.1.2-py3-none-any.whl.zip` & `tmp/TurboTouchPredictor-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 11570 bytes, number of entries: 10
+Zip file size: 11573 bytes, number of entries: 10
 -rw-r--r--  2.0 unx     2476 b- defN 24-May-17 18:14 TurboTouchPredictor/OneEuroVectorProcessor.py
 -rw-r--r--  2.0 unx     2356 b- defN 24-May-17 18:14 TurboTouchPredictor/TTPconfig.py
--rw-r--r--  2.0 unx     8104 b- defN 24-May-17 18:28 TurboTouchPredictor/TurboTouchPredictor.py
+-rw-r--r--  2.0 unx     8107 b- defN 24-May-17 18:47 TurboTouchPredictor/TurboTouchPredictor.py
 -rw-r--r--  2.0 unx       64 b- defN 24-May-17 18:14 TurboTouchPredictor/__init__.py
 -rw-r--r--  2.0 unx      404 b- defN 24-May-17 18:14 TurboTouchPredictor/pAttribut.py
--rw-r--r--  2.0 unx     7201 b- defN 24-May-17 18:35 TurboTouchPredictor-0.1.2.dist-info/LICENSE.md
--rw-r--r--  2.0 unx    14424 b- defN 24-May-17 18:35 TurboTouchPredictor-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-17 18:35 TurboTouchPredictor-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 24-May-17 18:35 TurboTouchPredictor-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      914 b- defN 24-May-17 18:35 TurboTouchPredictor-0.1.2.dist-info/RECORD
-10 files, 36055 bytes uncompressed, 9980 bytes compressed:  72.3%
+-rw-r--r--  2.0 unx     7201 b- defN 24-May-17 18:48 TurboTouchPredictor-0.1.3.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx    14424 b- defN 24-May-17 18:48 TurboTouchPredictor-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-17 18:48 TurboTouchPredictor-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 24-May-17 18:48 TurboTouchPredictor-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      914 b- defN 24-May-17 18:48 TurboTouchPredictor-0.1.3.dist-info/RECORD
+10 files, 36058 bytes uncompressed, 9983 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: TurboTouchPredictor/__init__.py
 Comment: 
 
 Filename: TurboTouchPredictor/pAttribut.py
 Comment: 
 
-Filename: TurboTouchPredictor-0.1.2.dist-info/LICENSE.md
+Filename: TurboTouchPredictor-0.1.3.dist-info/LICENSE.md
 Comment: 
 
-Filename: TurboTouchPredictor-0.1.2.dist-info/METADATA
+Filename: TurboTouchPredictor-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: TurboTouchPredictor-0.1.2.dist-info/WHEEL
+Filename: TurboTouchPredictor-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: TurboTouchPredictor-0.1.2.dist-info/top_level.txt
+Filename: TurboTouchPredictor-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: TurboTouchPredictor-0.1.2.dist-info/RECORD
+Filename: TurboTouchPredictor-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## TurboTouchPredictor/TurboTouchPredictor.py

```diff
@@ -1,16 +1,16 @@
 # Flavien Volant and Géry Casiez
 #
 # Licence defined in LICENCE.md file
 #
 
 import math
-from OneEuroVectorProcessor import OneEuroVectorProcessor
-from TTPconfig import cfg
-from pAttribut import pAttribut
+from .OneEuroVectorProcessor import OneEuroVectorProcessor
+from .TTPconfig import cfg
+from .pAttribut import pAttribut
 
 COMPENSATION_ALLOWED_VALUES = (0, 16, 32, 48, 64)
 
 class TurboTouchPredictor:
 
     """ TurboTouchPredictor
     :filter: OneEuroVectorProcessor
```

## Comparing `TurboTouchPredictor-0.1.2.dist-info/LICENSE.md` & `TurboTouchPredictor-0.1.3.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `TurboTouchPredictor-0.1.2.dist-info/METADATA` & `TurboTouchPredictor-0.1.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TurboTouchPredictor
-Version: 0.1.2
+Version: 0.1.3
 Summary: TurboTouch predictor
 Home-page: https://github.com/LokiResearch/TurboTouchPredictor/python
 Author: Flavien Volant and Géry Casiez
 Author-email: gery.casiez@univ-lille.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
```

## Comparing `TurboTouchPredictor-0.1.2.dist-info/RECORD` & `TurboTouchPredictor-0.1.3.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 TurboTouchPredictor/OneEuroVectorProcessor.py,sha256=CWg5kXLDhtNpOYPD3TwTvasD_bjWqLL_YY1NA_isWPw,2476
 TurboTouchPredictor/TTPconfig.py,sha256=AKrcVWEDUBDbFJyGxa_IJiCAG0nxx8U5bH2loQUizDs,2356
-TurboTouchPredictor/TurboTouchPredictor.py,sha256=xMzU5yzr0UVABbH39SJhFbVRmHd-rXS3fxn4Nw0y038,8104
+TurboTouchPredictor/TurboTouchPredictor.py,sha256=WOrOZzTJVgez51CZVzi4yS1chhVDI3z1v170OPtakxM,8107
 TurboTouchPredictor/__init__.py,sha256=3OSd_jA9cvreyayR7DTwZx-jRyDHC0YdM0Xd0JqCPKo,64
 TurboTouchPredictor/pAttribut.py,sha256=DfOorWRw7vtspQD_hNMDXOCoYhlIdIbH4nmhVx4zJ_4,404
-TurboTouchPredictor-0.1.2.dist-info/LICENSE.md,sha256=sC63Vpod7_CcZXyEwli5GqkAQUtblIvWaybTPMg2nj0,7201
-TurboTouchPredictor-0.1.2.dist-info/METADATA,sha256=zdHMqfzSLZwZcaEr_Zdl_L5wOw_3EoYKTp00tEoBIpA,14424
-TurboTouchPredictor-0.1.2.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-TurboTouchPredictor-0.1.2.dist-info/top_level.txt,sha256=1QOWVzYyQNRrsUN8nPjvWMsYhE9SurwYqwmDcWBLJMk,20
-TurboTouchPredictor-0.1.2.dist-info/RECORD,,
+TurboTouchPredictor-0.1.3.dist-info/LICENSE.md,sha256=sC63Vpod7_CcZXyEwli5GqkAQUtblIvWaybTPMg2nj0,7201
+TurboTouchPredictor-0.1.3.dist-info/METADATA,sha256=sPANKysERFc5hnHjUPci96ESFqo-T7BAIgsZR1x_Hyk,14424
+TurboTouchPredictor-0.1.3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+TurboTouchPredictor-0.1.3.dist-info/top_level.txt,sha256=1QOWVzYyQNRrsUN8nPjvWMsYhE9SurwYqwmDcWBLJMk,20
+TurboTouchPredictor-0.1.3.dist-info/RECORD,,
```

