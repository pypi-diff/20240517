# Comparing `tmp/vistudio-1.0.1.3-py3-none-any.whl.zip` & `tmp/vistudio-1.0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,18 @@
-Zip file size: 11327 bytes, number of entries: 19
--rw-r--r--  2.0 unx      173 b- defN 24-Feb-28 13:49 vistudio/__init__.py
--rw-r--r--  2.0 unx      329 b- defN 24-Feb-28 13:49 vistudio/annotation/__init__.py
--rw-r--r--  2.0 unx      341 b- defN 24-Feb-28 13:49 vistudio/annotation/api/__init__.py
--rw-r--r--  2.0 unx     3236 b- defN 24-Feb-28 13:49 vistudio/annotation/api/annotation.py
--rw-r--r--  2.0 unx       88 b- defN 24-Feb-28 13:49 vistudio/annotation/client/__init__.py
--rw-r--r--  2.0 unx     5088 b- defN 24-Feb-28 13:49 vistudio/annotation/client/annotation_client.py
--rw-r--r--  2.0 unx      250 b- defN 24-Feb-28 13:49 vistudio/annotation/datasource/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-28 13:49 vistudio/annotation/datasource/file_datasource.py
--rw-r--r--  2.0 unx     7888 b- defN 24-Feb-28 13:49 vistudio/annotation/datasource/sharded_mongo_datasource.py
--rw-r--r--  2.0 unx     1557 b- defN 24-Feb-28 13:49 vistudio/annotation/datasource/test_sharded_mongo_datasource.py
--rw-r--r--  2.0 unx      199 b- defN 24-Feb-28 13:49 vistudio/annotation/processor/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-28 13:49 vistudio/annotation/processor/coco_reader.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-28 13:49 vistudio/annotation/processor/image_uri_reader.py
--rw-r--r--  2.0 unx      517 b- defN 24-Feb-28 13:49 vistudio/annotation/processor/reader.py
--rw-r--r--  2.0 unx      571 b- defN 24-Feb-28 13:49 vistudio/annotation/processor/vistudio_v1_reader.py
--rw-r--r--  2.0 unx      777 b- defN 24-Feb-28 13:49 vistudio-1.0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-28 13:49 vistudio-1.0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-Feb-28 13:49 vistudio-1.0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1789 b- defN 24-Feb-28 13:49 vistudio-1.0.1.3.dist-info/RECORD
-19 files, 22904 bytes uncompressed, 8293 bytes compressed:  63.8%
+Zip file size: 13600 bytes, number of entries: 16
+-rw-r--r--  2.0 unx      173 b- defN 24-Mar-04 10:44 vistudio/__init__.py
+-rw-r--r--  2.0 unx      329 b- defN 24-Mar-04 10:44 vistudio/annotation/__init__.py
+-rw-r--r--  2.0 unx      341 b- defN 24-Mar-04 10:44 vistudio/annotation/api/__init__.py
+-rw-r--r--  2.0 unx     3365 b- defN 24-Mar-04 10:44 vistudio/annotation/api/annotation.py
+-rw-r--r--  2.0 unx      113 b- defN 24-Mar-04 10:44 vistudio/annotation/client/__init__.py
+-rw-r--r--  2.0 unx     5088 b- defN 24-Mar-04 10:44 vistudio/annotation/client/annotation_client.py
+-rw-r--r--  2.0 unx      250 b- defN 24-Mar-04 10:44 vistudio/annotation/datasource/__init__.py
+-rw-r--r--  2.0 unx     2755 b- defN 24-Mar-04 10:44 vistudio/annotation/datasource/annotation_datasink.py
+-rw-r--r--  2.0 unx     3243 b- defN 24-Mar-04 10:44 vistudio/annotation/datasource/file_datasource.py
+-rw-r--r--  2.0 unx    10253 b- defN 24-Mar-04 10:44 vistudio/annotation/datasource/sharded_mongo_datasource.py
+-rw-r--r--  2.0 unx      199 b- defN 24-Mar-04 10:44 vistudio/annotation/processor/__init__.py
+-rw-r--r--  2.0 unx     4203 b- defN 24-Mar-04 10:44 vistudio/annotation/processor/coco.py
+-rw-r--r--  2.0 unx      777 b- defN 24-Mar-04 10:44 vistudio-1.0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-04 10:44 vistudio-1.0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-Mar-04 10:44 vistudio-1.0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1475 b- defN 24-Mar-04 10:44 vistudio-1.0.1.4.dist-info/RECORD
+16 files, 32665 bytes uncompressed, 11106 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -15,44 +15,35 @@
 
 Filename: vistudio/annotation/client/annotation_client.py
 Comment: 
 
 Filename: vistudio/annotation/datasource/__init__.py
 Comment: 
 
-Filename: vistudio/annotation/datasource/file_datasource.py
+Filename: vistudio/annotation/datasource/annotation_datasink.py
 Comment: 
 
-Filename: vistudio/annotation/datasource/sharded_mongo_datasource.py
+Filename: vistudio/annotation/datasource/file_datasource.py
 Comment: 
 
-Filename: vistudio/annotation/datasource/test_sharded_mongo_datasource.py
+Filename: vistudio/annotation/datasource/sharded_mongo_datasource.py
 Comment: 
 
 Filename: vistudio/annotation/processor/__init__.py
 Comment: 
 
-Filename: vistudio/annotation/processor/coco_reader.py
-Comment: 
-
-Filename: vistudio/annotation/processor/image_uri_reader.py
-Comment: 
-
-Filename: vistudio/annotation/processor/reader.py
-Comment: 
-
-Filename: vistudio/annotation/processor/vistudio_v1_reader.py
+Filename: vistudio/annotation/processor/coco.py
 Comment: 
 
-Filename: vistudio-1.0.1.3.dist-info/METADATA
+Filename: vistudio-1.0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: vistudio-1.0.1.3.dist-info/WHEEL
+Filename: vistudio-1.0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: vistudio-1.0.1.3.dist-info/top_level.txt
+Filename: vistudio-1.0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: vistudio-1.0.1.3.dist-info/RECORD
+Filename: vistudio-1.0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vistudio/annotation/api/annotation.py

```diff
@@ -1,56 +1,56 @@
 # !/usr/bin/env python3
 # -*- coding: UTF-8 -*-
 #
 # Copyright (c) 2024 Baidu.com, Inc. All Rights Reserved
 """
 Vistudio Spec
 """
-from typing import List, Tuple, Any
+from typing import List, Tuple
 import pyarrow as pa
 from pydantic import BaseModel
 
 
 class Label(BaseModel):
     """Label"""
     id: int
     name: str
     confidence: float
 
     @classmethod
-    def get_data_type(cls) -> pa.DataType:
+    def to_pyarrow_schema(cls) -> pa.DataType:
         """Label to pyarrow data type"""
         return pa.struct([
             ("id", pa.int32()), 
             ("name", pa.string()), 
             ("confidence", pa.float32())
         ])
 
 
 class OCR(BaseModel):
     """OCR"""
     word: str
     direction: str
 
     @classmethod
-    def get_data_type(cls) -> pa.DataType:
+    def to_pyarrow_schema(cls) -> pa.DataType:
         """OCR to pyarrow data type"""
         return pa.struct([
             ("word", pa.string()), 
             ("direction", pa.string())
         ])
 
 
 class RLE(BaseModel):
     """RLE"""
     counts: List[float]
     size: Tuple[float, float]
 
     @classmethod
-    def get_data_type(cls) -> pa.DataType:
+    def to_pyarrow_schema(cls) -> pa.DataType:
         """RLE to pyarrow data type"""
         return pa.struct([
             ("count", pa.list_(pa.float32())), 
             ("size", pa.list_(pa.float32()))
         ])
 
 
@@ -62,76 +62,78 @@
     rle: RLE
     keypoints: List[float]
     ocr: OCR
     area: float
     labels: List[Label]
 
     @classmethod
-    def get_data_type(cls) -> pa.DataType:
+    def to_pyarrow_schema(cls) -> pa.DataType:
         """Annotation to pyarrow data type"""
         return pa.struct([
             ("id", pa.int32()),
             ("bbox", pa.list_(pa.float32())),
             ("segmentation", pa.list_(pa.float32())),
-            ("rle", RLE.get_data_type()),
+            ("rle", RLE.to_pyarrow_schema()),
             ("keypoints", pa.list_(pa.float32())),
-            ("ocr", OCR.get_data_type()),
+            ("ocr", OCR.to_pyarrow_schema()),
             ("area", pa.float32()),
-            ("labels", pa.list_(Label.get_data_type()))
+            ("labels", pa.list_(Label.to_pyarrow_schema()))
         ])
 
 
 class Annotations(BaseModel):
     """Annotations"""
-    imageID: int
-    modelName: str
-    modelVersion: str
+    image_id: str
+    model_name: str
+    model_version: str
     annotations: List[Annotation]
 
     @classmethod
-    def get_data_type(cls) -> pa.DataType:
+    def to_pyarrow_schema(cls) -> pa.DataType:
         """Annotations to pyarrow data type"""
         return pa.struct([
-            ("modelName", pa.string()), 
-            ("modelVersion", pa.string()),
-            ("annotations", pa.list_(Annotation.get_data_type()))
+            ("image_id", pa.string()),
+            ("model_name", pa.string()), 
+            ("model_version", pa.string()),
+            ("annotations", pa.list_(Annotation.to_pyarrow_schema()))
         ])
 
 
 class Image(BaseModel):
     """Image"""
-    id: int
+    id: str
     name: str
-    fileUri: str
+    file_uri: str
     width: int
     height: int
+    annotations: List[Annotations]
 
     @classmethod
-    def get_data_type(cls) -> pa.DataType:
+    def to_pyarrow_schema(cls) -> pa.DataType:
         """Image to pyarrow data type"""
         return pa.struct([
-            ("id", pa.int32()),
+            ("id", pa.string()),
+            ("name", pa.string()),
+            ("file_uri", pa.string()),
             ("width", pa.int32()),
             ("height", pa.int32()),
-            ("fileName", pa.string()),
+            ("annotations", pa.list_(Annotations.to_pyarrow_schema()))
         ])
 
 
 class Vistudio(BaseModel):
     """Vistudio"""
     images: List[Image]
-    annotations: List[Annotations]
     labels: List[Label]
 
     @classmethod
     def to_pyarrow_schema(cls) -> pa.Schema:
         """Vistudio to pyarrow schema"""
         return pa.schema([
-            pa.field("images", Image.get_data_type()),
-            pa.field("annotations", Annotations.get_data_type()),
-            pa.field("labels", Label.get_data_type()),
+            pa.field("images", Image.to_pyarrow_schema()),
+            pa.field("labels", Label.to_pyarrow_schema()),
         ])
 
 
 if __name__ == "__main__":
     print(Vistudio.to_pyarrow_schema())
```

## vistudio/annotation/client/__init__.py

```diff
@@ -1,4 +1,6 @@
-# -*- coding: utf-8 -*-
+# !/usr/bin/env python3
+# -*- coding: UTF-8 -*-
+
 """
 # Copyright (c) 2024 Baidu.com, Inc. All Rights Reserved
 """
```

## vistudio/annotation/datasource/file_datasource.py

```diff
@@ -0,0 +1,203 @@
+00000000: 2320 212f 7573 722f 6269 6e2f 656e 7620  # !/usr/bin/env 
+00000010: 7079 7468 6f6e 330a 2320 2d2a 2d20 636f  python3.# -*- co
+00000020: 6469 6e67 3a20 5554 462d 3820 2d2a 2d0a  ding: UTF-8 -*-.
+00000030: 230a 2320 436f 7079 7269 6768 7420 2863  #.# Copyright (c
+00000040: 2920 3230 3234 2042 6169 6475 2e63 6f6d  ) 2024 Baidu.com
+00000050: 2c20 496e 632e 2041 6c6c 2052 6967 6874  , Inc. All Right
+00000060: 7320 5265 7365 7276 6564 0a22 2222 0a46  s Reserved.""".F
+00000070: 696c 6544 6174 6173 6f75 7263 650a 2222  ileDatasource.""
+00000080: 220a 0a69 6d70 6f72 7420 6c6f 6767 696e  "..import loggin
+00000090: 670a 6672 6f6d 2074 7970 696e 6720 696d  g.from typing im
+000000a0: 706f 7274 2044 6963 742c 2041 6e79 2c20  port Dict, Any, 
+000000b0: 556e 696f 6e2c 204c 6973 740a 0a69 6d70  Union, List..imp
+000000c0: 6f72 7420 7261 792e 6461 7461 0a66 726f  ort ray.data.fro
+000000d0: 6d20 7769 6e64 6d69 6c6c 636f 6d70 7574  m windmillcomput
+000000e0: 6576 312e 6669 6c65 7379 7374 656d 2e62  ev1.filesystem.b
+000000f0: 6c6f 6273 746f 7265 2069 6d70 6f72 7420  lobstore import 
+00000100: 5333 426c 6f62 5374 6f72 650a 696d 706f  S3BlobStore.impo
+00000110: 7274 206f 730a 6672 6f6d 2070 7964 616e  rt os.from pydan
+00000120: 7469 6320 696d 706f 7274 2042 6173 654d  tic import BaseM
+00000130: 6f64 656c 0a0a 0a6c 6f67 6765 7220 3d20  odel...logger = 
+00000140: 6c6f 6767 696e 672e 6765 744c 6f67 6765  logging.getLogge
+00000150: 7228 5f5f 6e61 6d65 5f5f 290a 0a44 4154  r(__name__)..DAT
+00000160: 415f 5459 5045 5f49 4d41 4745 203d 2022  A_TYPE_IMAGE = "
+00000170: 696d 6167 6522 0a44 4154 415f 5459 5045  image".DATA_TYPE
+00000180: 5f41 4e4e 4f54 4154 494f 4e20 3d20 2261  _ANNOTATION = "a
+00000190: 6e6e 6f74 6174 696f 6e22 0a41 4e4e 4f54  nnotation".ANNOT
+000001a0: 4154 494f 4e5f 5459 5045 5f43 4f43 4f20  ATION_TYPE_COCO 
+000001b0: 3d20 2263 6f63 6f22 0a41 4e4e 4f54 4154  = "coco".ANNOTAT
+000001c0: 494f 4e5f 5459 5045 5f56 4953 5455 4449  ION_TYPE_VISTUDI
+000001d0: 4f5f 5631 203d 2022 7669 7374 7564 696f  O_V1 = "vistudio
+000001e0: 7631 220a 0a69 6d61 6765 5f65 7874 656e  v1"..image_exten
+000001f0: 7369 6f6e 7320 3d20 2827 2e6a 7065 6727  sions = ('.jpeg'
+00000200: 2c20 272e 6a70 6727 2c20 272e 706e 6727  , '.jpg', '.png'
+00000210: 2c20 272e 626d 7027 290a 0a0a 636c 6173  , '.bmp')...clas
+00000220: 7320 4669 6c65 4461 7461 736f 7572 6365  s FileDatasource
+00000230: 286f 626a 6563 7429 3a0a 2020 2020 2222  (object):.    ""
+00000240: 220a 2020 2020 4669 6c65 4461 7461 736f  ".    FileDataso
+00000250: 7572 6365 0a20 2020 2022 2222 0a20 2020  urce.    """.   
+00000260: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00000270: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
+00000280: 2020 2020 2073 335f 6275 636b 6574 3a20       s3_bucket: 
+00000290: 7374 7220 3d20 2222 2c0a 2020 2020 2020  str = "",.      
+000002a0: 2020 2020 2020 2020 2020 2062 733a 2053             bs: S
+000002b0: 3342 6c6f 6253 746f 7265 203d 204e 6f6e  3BlobStore = Non
+000002c0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+000002d0: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
+000002e0: 656c 662e 7333 5f62 7563 6b65 7420 3d20  elf.s3_bucket = 
+000002f0: 7333 5f62 7563 6b65 740a 2020 2020 2020  s3_bucket.      
+00000300: 2020 7365 6c66 2e62 7320 3d20 6273 0a0a    self.bs = bs..
+00000310: 2020 2020 6465 6620 7265 6164 5f6a 736f      def read_jso
+00000320: 6e5f 6669 6c65 2873 656c 662c 2066 696c  n_file(self, fil
+00000330: 655f 7572 693a 2020 556e 696f 6e5b 7374  e_uri:  Union[st
+00000340: 725d 203d 2022 2229 202d 3e20 7261 792e  r] = "") -> ray.
+00000350: 6461 7461 2e44 6174 6173 6574 3a0a 2020  data.Dataset:.  
+00000360: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00000370: 2020 7265 6164 5f6a 736f 6e5f 6669 6c65    read_json_file
+00000380: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00000390: 6669 6c65 5f75 7269 3a0a 2020 2020 2020  file_uri:.      
+000003a0: 2020 3a72 6574 7572 6e3a 2072 6179 2e64    :return: ray.d
+000003b0: 6174 612e 4461 7461 7365 740a 2020 2020  ata.Dataset.    
+000003c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000003d0: 6c6f 6767 6572 2e69 6e66 6f28 2252 6561  logger.info("Rea
+000003e0: 6420 4a73 6f6e 2e20 5374 6172 7420 7072  d Json. Start pr
+000003f0: 6f63 6573 7320 6669 6c65 3a20 7b7d 2e22  ocess file: {}."
+00000400: 2e66 6f72 6d61 7428 6669 6c65 5f75 7269  .format(file_uri
+00000410: 2929 0a20 2020 2020 2020 2065 7874 203d  )).        ext =
+00000420: 206f 732e 7061 7468 2e73 706c 6974 6578   os.path.splitex
+00000430: 7428 6669 6c65 5f75 7269 295b 315d 2e6c  t(file_uri)[1].l
+00000440: 6f77 6572 2829 0a20 2020 2020 2020 2069  ower().        i
+00000450: 6620 6578 7420 3d3d 2022 223a 0a20 2020  f ext == "":.   
+00000460: 2020 2020 2020 2020 2066 696c 656e 616d           filenam
+00000470: 6573 203d 2073 656c 662e 5f67 6574 5f66  es = self._get_f
+00000480: 696c 656e 616d 6573 2866 696c 655f 7572  ilenames(file_ur
+00000490: 692c 2030 2c20 7365 6c66 2e73 335f 6275  i, 0, self.s3_bu
+000004a0: 636b 6574 2c20 7365 6c66 2e62 7329 0a20  cket, self.bs). 
+000004b0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000004c0: 2020 2020 2020 2020 2066 696c 656e 616d           filenam
+000004d0: 6573 203d 205b 6669 6c65 5f75 7269 5d0a  es = [file_uri].
+000004e0: 2020 2020 2020 2020 6669 6c65 5f70 6174          file_pat
+000004f0: 6873 203d 206c 6973 7428 290a 2020 2020  hs = list().    
+00000500: 2020 2020 666f 7220 6669 6c65 6e61 6d65      for filename
+00000510: 2069 6e20 6669 6c65 6e61 6d65 733a 0a20   in filenames:. 
+00000520: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00000530: 7420 6669 6c65 6e61 6d65 2e6c 6f77 6572  t filename.lower
+00000540: 2829 2e65 6e64 7377 6974 6828 272e 6a73  ().endswith('.js
+00000550: 6f6e 2729 3a0a 2020 2020 2020 2020 2020  on'):.          
+00000560: 2020 2020 2020 636f 6e74 696e 7565 0a0a        continue..
+00000570: 2020 2020 2020 2020 2020 2020 6465 7374              dest
+00000580: 5f70 6174 6820 3d20 6669 6c65 6e61 6d65  _path = filename
+00000590: 5b35 3a5d 0a20 2020 2020 2020 2020 2020  [5:].           
+000005a0: 2073 656c 662e 6273 2e64 6f77 6e6c 6f61   self.bs.downloa
+000005b0: 645f 6669 6c65 2866 696c 656e 616d 652c  d_file(filename,
+000005c0: 2064 6573 745f 7061 7468 290a 2020 2020   dest_path).    
+000005d0: 2020 2020 2020 2020 6669 6c65 5f70 6174          file_pat
+000005e0: 6873 2e61 7070 656e 6428 6465 7374 5f70  hs.append(dest_p
+000005f0: 6174 6829 0a0a 2020 2020 2020 2020 6473  ath)..        ds
+00000600: 203d 2072 6179 2e64 6174 612e 7265 6164   = ray.data.read
+00000610: 5f6a 736f 6e28 6669 6c65 5f70 6174 6873  _json(file_paths
+00000620: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00000630: 2064 730a 0a20 2020 2064 6566 2072 6561   ds..    def rea
+00000640: 645f 696d 6167 655f 6669 6c65 2873 656c  d_image_file(sel
+00000650: 662c 2066 696c 655f 7572 693a 2020 556e  f, file_uri:  Un
+00000660: 696f 6e5b 7374 725d 203d 2022 2229 202d  ion[str] = "") -
+00000670: 3e20 7261 792e 6461 7461 2e44 6174 6173  > ray.data.Datas
+00000680: 6574 3a0a 2020 2020 2020 2020 2222 220a  et:.        """.
+00000690: 2020 2020 2020 2020 7265 6164 5f69 6d61          read_ima
+000006a0: 6765 5f66 696c 650a 2020 2020 2020 2020  ge_file.        
+000006b0: 3a72 6574 7572 6e3a 2072 6179 2e64 6174  :return: ray.dat
+000006c0: 612e 4461 7461 7365 740a 2020 2020 2020  a.Dataset.      
+000006d0: 2020 2222 220a 2020 2020 2020 2020 6c6f    """.        lo
+000006e0: 6767 6572 2e69 6e66 6f28 2246 726f 6d20  gger.info("From 
+000006f0: 496d 6167 652e 2053 7461 7274 2070 726f  Image. Start pro
+00000700: 6365 7373 2066 696c 653a 207b 7d2e 222e  cess file: {}.".
+00000710: 666f 726d 6174 2866 696c 655f 7572 6929  format(file_uri)
+00000720: 290a 0a20 2020 2020 2020 2065 7874 203d  )..        ext =
+00000730: 206f 732e 7061 7468 2e73 706c 6974 6578   os.path.splitex
+00000740: 7428 6669 6c65 5f75 7269 295b 315d 2e6c  t(file_uri)[1].l
+00000750: 6f77 6572 2829 0a20 2020 2020 2020 2069  ower().        i
+00000760: 6620 6578 7420 3d3d 2022 223a 0a20 2020  f ext == "":.   
+00000770: 2020 2020 2020 2020 2066 696c 656e 616d           filenam
+00000780: 6573 203d 2073 656c 662e 5f67 6574 5f66  es = self._get_f
+00000790: 696c 656e 616d 6573 2866 696c 655f 7572  ilenames(file_ur
+000007a0: 692c 2032 2c20 7365 6c66 2e73 335f 6275  i, 2, self.s3_bu
+000007b0: 636b 6574 2c20 7365 6c66 2e62 7329 0a20  cket, self.bs). 
+000007c0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000007d0: 2020 2020 2020 2020 2066 696c 656e 616d           filenam
+000007e0: 6573 203d 205b 6669 6c65 5f75 7269 5d0a  es = [file_uri].
+000007f0: 2020 2020 2020 2020 696d 6167 655f 6c69          image_li
+00000800: 7374 203d 206c 6973 7428 290a 2020 2020  st = list().    
+00000810: 2020 2020 666f 7220 6669 6c65 6e61 6d65      for filename
+00000820: 2069 6e20 6669 6c65 6e61 6d65 733a 0a20   in filenames:. 
+00000830: 2020 2020 2020 2020 2020 2064 6174 6120             data 
+00000840: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+00000850: 2020 2020 2266 696c 655f 7572 6922 3a20      "file_uri": 
+00000860: 6669 6c65 6e61 6d65 2c0a 2020 2020 2020  filename,.      
+00000870: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00000880: 2020 2020 696d 6167 655f 6c69 7374 2e61      image_list.a
+00000890: 7070 656e 6428 6461 7461 290a 2020 2020  ppend(data).    
+000008a0: 2020 2020 2320 696d 6167 655f 6c69 7374      # image_list
+000008b0: 203d 205b 496d 6167 6528 6669 6c65 5572   = [Image(fileUr
+000008c0: 693d 6669 6c65 6e61 6d65 2c20 7769 6474  i=filename, widt
+000008d0: 683d 302c 2068 6569 6768 743d 3029 2066  h=0, height=0) f
+000008e0: 6f72 2066 696c 656e 616d 6520 696e 2066  or filename in f
+000008f0: 696c 656e 616d 6573 5d0a 2020 2020 2020  ilenames].      
+00000900: 2020 6473 203d 2072 6179 2e64 6174 612e    ds = ray.data.
+00000910: 6672 6f6d 5f69 7465 6d73 2869 6d61 6765  from_items(image
+00000920: 5f6c 6973 7429 0a0a 2020 2020 2020 2020  _list)..        
+00000930: 7265 7475 726e 2064 730a 0a0a 2020 2020  return ds...    
+00000940: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
+00000950: 2020 6465 6620 5f67 6574 5f66 696c 656e    def _get_filen
+00000960: 616d 6573 2866 696c 655f 7572 692c 206c  ames(file_uri, l
+00000970: 6179 6572 2c20 7333 5f62 7563 6b65 742c  ayer, s3_bucket,
+00000980: 2062 7329 3a0a 2020 2020 2020 2020 2222   bs):.        ""
+00000990: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
+000009a0: 2066 696c 655f 7572 693a 2073 33e5 9cb0   file_uri: s3...
+000009b0: e59d 800a 2020 2020 2020 2020 3a70 6172  ....        :par
+000009c0: 616d 206c 6179 6572 3a20 e981 8de5 8e86  am layer: ......
+000009d0: e79a 84e5 b182 e695 b00a 2020 2020 2020  ..........      
+000009e0: 2020 3a72 6574 7572 6e3a 20e6 9687 e4bb    :return: .....
+000009f0: b666 696c 656e 616d 65e5 8897 e8a1 a80a  .filename.......
+00000a00: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00000a10: 2020 2020 6669 6c65 6e61 6d65 7320 3d20      filenames = 
+00000a20: 5b5d 0a20 2020 2020 2020 2064 6573 745f  [].        dest_
+00000a30: 7061 7468 203d 2066 696c 655f 7572 692e  path = file_uri.
+00000a40: 7370 6c69 7428 7333 5f62 7563 6b65 7420  split(s3_bucket 
+00000a50: 2b20 272f 2729 5b31 5d0a 2020 2020 2020  + '/')[1].      
+00000a60: 2020 6966 206e 6f74 2064 6573 745f 7061    if not dest_pa
+00000a70: 7468 2e65 6e64 7377 6974 6828 222f 2229  th.endswith("/")
+00000a80: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
+00000a90: 7374 5f70 6174 6820 2b3d 2022 2f22 0a20  st_path += "/". 
+00000aa0: 2020 2020 2020 2064 6573 745f 7061 7274         dest_part
+00000ab0: 7320 3d20 6465 7374 5f70 6174 682e 7370  s = dest_path.sp
+00000ac0: 6c69 7428 272f 2729 5b3a 2d31 5d0a 0a20  lit('/')[:-1].. 
+00000ad0: 2020 2020 2020 2066 696c 655f 6c69 7374         file_list
+00000ae0: 203d 2062 732e 6c69 7374 5f66 696c 6528   = bs.list_file(
+00000af0: 6465 7374 5f70 6174 6829 0a20 2020 2020  dest_path).     
+00000b00: 2020 2066 6f72 2066 696c 6520 696e 2066     for file in f
+00000b10: 696c 655f 6c69 7374 3a0a 2020 2020 2020  ile_list:.      
+00000b20: 2020 2020 2020 665f 7061 7468 203d 2066        f_path = f
+00000b30: 696c 655b 274b 6579 275d 0a20 2020 2020  ile['Key'].     
+00000b40: 2020 2020 2020 2066 5f70 6172 7473 203d         f_parts =
+00000b50: 2066 5f70 6174 682e 7370 6c69 7428 272f   f_path.split('/
+00000b60: 2729 5b3a 2d31 5d0a 2020 2020 2020 2020  ')[:-1].        
+00000b70: 2020 2020 2320 e6ad a4e5 a484 e8a1 a8e7      # ..........
+00000b80: a4ba e58f 96e6 9687 e4bb b6e5 a4b9 33e5  ..............3.
+00000b90: b182 e586 85e7 9a84 e695 b0e6 8dae 0a20  ............... 
+00000ba0: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+00000bb0: 6e28 665f 7061 7274 7329 202d 206c 656e  n(f_parts) - len
+00000bc0: 2864 6573 745f 7061 7274 7329 203e 206c  (dest_parts) > l
+00000bd0: 6179 6572 3a0a 2020 2020 2020 2020 2020  ayer:.          
+00000be0: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+00000bf0: 2020 2020 2020 2020 2020 2066 696c 656e             filen
+00000c00: 616d 6520 3d20 2273 333a 2f2f 2220 2b20  ame = "s3://" + 
+00000c10: 6f73 2e70 6174 682e 6a6f 696e 2873 335f  os.path.join(s3_
+00000c20: 6275 636b 6574 2c20 665f 7061 7468 290a  bucket, f_path).
+00000c30: 2020 2020 2020 2020 2020 2020 6669 6c65              file
+00000c40: 6e61 6d65 732e 6170 7065 6e64 2866 696c  names.append(fil
+00000c50: 656e 616d 6529 0a0a 2020 2020 2020 2020  ename)..        
+00000c60: 7265 7475 726e 2066 696c 656e 616d 6573  return filenames
+00000c70: 0a0a 0a0a 0a0a 6672 6f6d 2070 7961 7272  ......from pyarr
+00000c80: 6f77 2e66 7320 696d 706f 7274 2053 3346  ow.fs import S3F
+00000c90: 696c 6553 7973 7465 6d0a 0a53 3346 696c  ileSystem..S3Fil
+00000ca0: 6553 7973 7465 6d28 290a 0a              eSystem()..
```

## vistudio/annotation/datasource/sharded_mongo_datasource.py

```diff
@@ -3,15 +3,15 @@
 #
 # Copyright (c) 2024 Baidu.com, Inc. All Rights Reserved
 """
 ShardedMongoDatasource
 """
 
 import logging
-from typing import Dict, List
+from typing import Dict, List, Optional, Callable
 import bson
 import pymongo
 import pymongoarrow.api
 
 from ray.util.annotations import PublicAPI
 from ray.data.block import Block, BlockMetadata
 from ray.data.datasource.datasource import ReadTask
@@ -20,21 +20,46 @@
 
 logger = logging.getLogger(__name__)
 
 
 @PublicAPI(stability="alpha")
 class ShardedMongoDatasource(MongoDatasource):
     """Datasource for reading from and writing to MongoDB."""
+    def __init__(
+        self,
+        uri: str,
+        database: str,
+        collection: str,
+        pipeline: Optional[List[Dict]] = None,
+        pipeline_func: Optional[Callable[[], Block]] = None,
+        schema: Optional["pymongoarrow.api.Schema"] = None,
+        **mongo_args,
+    ):
+        """
+        Args:
+        uri: The URI of the MongoDB cluster.
+        database: The database to read from.
+        collection: The collection to read from.
+        pipeline: The aggregation pipeline to apply.
+        pipeline_func: A function that takes a pymongo.MongoClient and returns a Block.
+        schema: The schema to use for reading.
+        mongo_args: Additional arguments to pass to the pymongo.MongoClient constructor.
+        """
+        self._pipeline_func = pipeline_func
+        super().__init__(uri, database, collection, pipeline=pipeline, schema=schema, **mongo_args)
+
+
 
     def get_read_tasks(self, parallelism: int) -> List[ReadTask]:
         def make_block(
             uri: str,
             database: str,
             collection: str,
             pipeline: List[Dict],
+            pipeline_func: Optional[Callable[[], Block]],
             shard_match: Dict,
             shard_hosts: List[str],
             schema: "pymongoarrow.api.Schema",
             kwargs: dict,
         ) -> Block:
             import pymongo
             from pymongo.uri_parser import parse_uri
@@ -48,14 +73,17 @@
             ]
 
             uri_info = parse_uri(uri)
             uri_info["nodelist"] = shard_hosts
             shard_uri = _to_mongo_uri(uri_info)
             client = pymongo.MongoClient(shard_uri)
 
+            if pipeline_func is not None:
+                return pipeline_func(client[database][collection], shard_match=match, schema=schema, **kwargs)
+
             return aggregate_arrow_all(
                 client[database][collection], match + pipeline, schema=schema, **kwargs
             )
         
         def _to_mongo_uri(uri_info: Dict) -> str:
             nodelist = uri_info.get('nodelist', [])
             username = uri_info.get('username', None)
@@ -160,62 +188,95 @@
                 exec_stats=None,
             )
             make_shard_block_args = (
                 self._uri,
                 self._database,
                 self._collection,
                 self._pipeline,
+                self._pipeline_func,
                 input_partition[0],
                 input_partition[1],
                 self._schema,
                 self._mongo_args,
             )
 
             read_task = ReadTask(
                 lambda args=make_shard_block_args: [make_block(*args)],
                 metadata,
             )
             read_tasks.append(read_task)
         return read_tasks
 
 
+def _example_read(item):
+    """Example for reading data from ShardedMongoDatasource."""
+    name = item["name"]
+    float_field = item["float_field"]
+    int_field = item["int_field"]
+    print(f"name: {name}, float_field: {float_field}, int_field: {int_field}")
+
+    return {
+        "name": name,
+        "float_field": float_field,
+        "int_field": int_field
+    }
+
 import ray
 
 @ray.remote
-def start():
-    """Example for using ShardedMongoDatasource."""
+def _example_pipeline():
+    """Example for using ShardedMongoDatasource by mongo pipeline."""
     from ray.data.read_api import read_datasource
     from pymongoarrow.api import Schema
     import pyarrow as pa
 
-    def read(item):
-        name = item["name"]
-        float_field = item["float_field"]
-        int_field = item["int_field"]
-        print(f"name: {name}, float_field: {float_field}, int_field: {int_field}")
-
-        return {
-            "name": name,
-            "float_field": float_field,
-            "int_field": int_field
-        }
+    uri = "mongodb://root:mongo123#@10.27.240.45:8719"
+    db_name = "lyw"
+    collection_name = "test"
+    schema = Schema({"name": pa.string(), "float_field": pa.float64(), "int_field": pa.int32()})
+
+    source = ShardedMongoDatasource(
+        uri=uri,
+        database=db_name,
+        collection=collection_name,
+        pipeline=[{ "$match": { "name": { "$exists": True } } }],
+        schema=schema)
+    ds = read_datasource(source, parallelism=10)
+
+    ds = ds.map(_example_read)
+    ds.show(1)
+
+@ray.remote
+def _example_pipeline_func():
+    """Example for using ShardedMongoDatasource by custom pipeline function."""
+    from ray.data.read_api import read_datasource
+    from pymongoarrow.api import Schema
+    import pyarrow as pa
 
     uri = "mongodb://root:mongo123#@10.27.240.45:8719"
     db_name = "lyw"
     collection_name = "test"
     schema = Schema({"name": pa.string(), "float_field": pa.float64(), "int_field": pa.int32()})
 
+    def pipeline_func(collection, shard_match, schema=None, **kwargs):
+        from pymongoarrow.api import aggregate_arrow_all
+
+        pipeline = [{ "$match": { "name": { "$exists": True } } }]
+        return aggregate_arrow_all(collection, shard_match + pipeline, schema=schema, **kwargs)
+
     source = ShardedMongoDatasource(
         uri=uri,
         database=db_name,
         collection=collection_name,
+        pipeline_func=pipeline_func,
         schema=schema)
     ds = read_datasource(source, parallelism=10)
 
-    ds = ds.map(read)
+    ds = ds.map(_example_read)
     ds.show(1)
 
 
 if __name__ == "__main__":
     ray.init(address="ray://10.27.240.45:8887")
-    ray.get(start.remote())
+    ray.get(_example_pipeline.remote())
+    ray.get(_example_pipeline_func.remote())
     ray.shutdown()
```

## Comparing `vistudio-1.0.1.3.dist-info/METADATA` & `vistudio-1.0.1.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vistudio
-Version: 1.0.1.3
+Version: 1.0.1.4
 Summary: sdk in python for annotation
 Home-page: https://console.cloud.baidu-int.com/devops/icode/repos/baidu/bce-vistudio/vistudio-annotation/tree/master/sdk
 Author: yangtingyu01
 Author-email: yangtingyu01@baidu.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

## Comparing `vistudio-1.0.1.3.dist-info/RECORD` & `vistudio-1.0.1.4.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 vistudio/__init__.py,sha256=Djy5xyEmFQHilSmahGmMflEDrNWhB22DyBBKZgBav1k,173
 vistudio/annotation/__init__.py,sha256=GUpiiJdJhXDGl0dBEcjbJwMKzd5JolcTo-eG7-AiRXI,329
 vistudio/annotation/api/__init__.py,sha256=8Ar6AQMcstAqWEdbe1zneFVGnk5Ibtuh8DRyAdZGtCA,341
-vistudio/annotation/api/annotation.py,sha256=VjGQ0yVWKepcbwbZxyN3EkReLGtAvczvFcDoSJDf3w0,3236
-vistudio/annotation/client/__init__.py,sha256=dfB3J9IohKbrEkcbGZ7JpPfKZCQOOmp1wVJnaJcsq8M,88
+vistudio/annotation/api/annotation.py,sha256=MdKb_nD7iqYx83JEx01ZyEJQte6-BQ0KR6nUrX4FX58,3365
+vistudio/annotation/client/__init__.py,sha256=02MmYPTyqBxB4O8wQMigBzYpKeodE7G_RbALErakyAc,113
 vistudio/annotation/client/annotation_client.py,sha256=OlNISdK2wDAuVv5OUDzWkyXFfWi43rgdQTmFBWcNY2g,5088
 vistudio/annotation/datasource/__init__.py,sha256=ClqXuy88n0lZ5nB90BHRQtrk0X9f_pnZ1PBqDW5KV5Q,250
-vistudio/annotation/datasource/file_datasource.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-vistudio/annotation/datasource/sharded_mongo_datasource.py,sha256=eVNtfI7xsWX4oRAw2K2KBhY6QJAMww6zkPAFT8BvC-M,7888
-vistudio/annotation/datasource/test_sharded_mongo_datasource.py,sha256=Xb9bpQsAbF2B_698vrqfHmLv_NyvuBSvZ-qfkvLp2zw,1557
+vistudio/annotation/datasource/annotation_datasink.py,sha256=2OutcQP513s5klBC-8I8MgLFPtUc2oB1Rxe0Vte7Yuc,2755
+vistudio/annotation/datasource/file_datasource.py,sha256=XtlnQmRVPsPXb8tlOlXsV_vsyuL0CBOKRhb0YSf2l2w,3243
+vistudio/annotation/datasource/sharded_mongo_datasource.py,sha256=CoSXeyiz11ggiZabw9lo1YHg4SnFCsA9hkXKXtAxJ1I,10253
 vistudio/annotation/processor/__init__.py,sha256=HGuINroMtnLTmzQ0dqtFm8Xn4PTwCTD6PJf4sHWXiJ4,199
-vistudio/annotation/processor/coco_reader.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-vistudio/annotation/processor/image_uri_reader.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-vistudio/annotation/processor/reader.py,sha256=5kdhgxBzYaLkCk_6qcHdacVF16lCl1k0rccft_LBJDs,517
-vistudio/annotation/processor/vistudio_v1_reader.py,sha256=l-swl57efPvganJe3bk8ImLnlgNPAuQ2A6nxl8Ma2FI,571
-vistudio-1.0.1.3.dist-info/METADATA,sha256=OmpAsgk2PRsPFpzjBjsR2-d9_42lSqdt6Ix1jsD-rAw,777
-vistudio-1.0.1.3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-vistudio-1.0.1.3.dist-info/top_level.txt,sha256=VHB8Z0A6SBR206Y_7CHETjwf1_WHcHFF5fPeBoLrxZ0,9
-vistudio-1.0.1.3.dist-info/RECORD,,
+vistudio/annotation/processor/coco.py,sha256=5qgZ_rNf6RejQzR7-5fVj61m_ExRaGgNL5hCl4xaJeI,4203
+vistudio-1.0.1.4.dist-info/METADATA,sha256=N1hCZn9NAvs1hzkJmnYjSbnDJMdbCKxSwlIcrO26oZo,777
+vistudio-1.0.1.4.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+vistudio-1.0.1.4.dist-info/top_level.txt,sha256=VHB8Z0A6SBR206Y_7CHETjwf1_WHcHFF5fPeBoLrxZ0,9
+vistudio-1.0.1.4.dist-info/RECORD,,
```

