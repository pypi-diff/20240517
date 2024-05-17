# Comparing `tmp/lacss-0.8.1.tar.gz` & `tmp/lacss-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacss-0.8.1.tar", max compression
+gzip compressed data, was "lacss-0.9.0.tar", max compression
```

## Comparing `lacss-0.8.1.tar` & `lacss-0.9.0.tar`

### file list

```diff
@@ -1,48 +1,53 @@
--rw-r--r--   0        0        0     1062 2024-04-12 13:57:54.798780 lacss-0.8.1/LICENSE
--rw-r--r--   0        0        0     2539 2024-04-12 13:57:54.798780 lacss-0.8.1/README.md
--rw-r--r--   0        0        0      157 2024-04-12 13:57:54.798780 lacss-0.8.1/lacss/__init__.py
--rw-r--r--   0        0        0       48 2024-04-12 13:57:54.798780 lacss-0.8.1/lacss/data/__init__.py
--rw-r--r--   0        0        0    14546 2024-04-12 13:57:54.798780 lacss-0.8.1/lacss/data/augment.py
--rw-r--r--   0        0        0    13109 2024-04-12 13:57:54.798780 lacss-0.8.1/lacss/data/generator.py
--rw-r--r--   0        0        0       43 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/deploy/__init__.py
--rw-r--r--   0        0        0     3151 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/deploy/lacss_pb2.py
--rw-r--r--   0        0        0    21615 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/deploy/predict.py
--rw-r--r--   0        0        0     4125 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/deploy/server.py
--rw-r--r--   0        0        0       74 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/losses/__init__.py
--rw-r--r--   0        0        0     6115 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/losses/auxiliary.py
--rw-r--r--   0        0        0      965 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/losses/common.py
--rw-r--r--   0        0        0     1748 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/losses/detection.py
--rw-r--r--   0        0        0     5406 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/losses/instance.py
--rw-r--r--   0        0        0       22 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/metrics/__init__.py
--rw-r--r--   0        0        0     5559 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/metrics/ranked.py
--rw-r--r--   0        0        0      330 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/modules/__init__.py
--rw-r--r--   0        0        0     2355 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/modules/common.py
--rw-r--r--   0        0        0     7968 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/modules/convnext.py
--rw-r--r--   0        0        0     7808 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/modules/detector.py
--rw-r--r--   0        0        0     3899 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/modules/lacss.py
--rw-r--r--   0        0        0     3292 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/modules/lpn.py
--rw-r--r--   0        0        0     3830 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/modules/resnet.py
--rw-r--r--   0        0        0     5557 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/modules/segmentor.py
--rw-r--r--   0        0        0     2297 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/modules/unet.py
--rw-r--r--   0        0        0      153 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/ops/__init__.py
--rw-r--r--   0        0        0     2474 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/ops/boxes.py
--rw-r--r--   0        0        0     3551 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/ops/image.py
--rw-r--r--   0        0        0     3136 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/ops/locations.py
--rw-r--r--   0        0        0     5961 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/ops/nms.py
--rw-r--r--   0        0        0    11822 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/ops/patches.py
--rw-r--r--   0        0        0      482 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/ops/uda.py
--rw-r--r--   0        0        0       63 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/tracking/__init__.py
--rw-r--r--   0        0        0     3340 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/tracking/predict.py
--rw-r--r--   0        0        0    12670 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/tracking/seqnms.py
--rw-r--r--   0        0        0     6741 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/tracking/smc.py
--rw-r--r--   0        0        0     5646 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/tracking/utils.py
--rw-r--r--   0        0        0      203 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/train/__init__.py
--rw-r--r--   0        0        0    10358 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/train/base_trainer.py
--rw-r--r--   0        0        0    10541 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/train/lacss_trainer.py
--rw-r--r--   0        0        0     1170 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/train/loss.py
--rw-r--r--   0        0        0     4564 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/train/strategy.py
--rw-r--r--   0        0        0     5541 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/train/utils.py
--rw-r--r--   0        0        0      931 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/typing.py
--rw-r--r--   0        0        0     5151 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/utils.py
--rw-r--r--   0        0        0      988 2024-04-12 13:58:13.111070 lacss-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     3337 1970-01-01 00:00:00.000000 lacss-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-16 18:47:45.020231 lacss-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2552 2024-05-16 18:47:45.020231 lacss-0.9.0/README.md
+-rw-r--r--   0        0        0      157 2024-05-16 18:47:45.020231 lacss-0.9.0/lacss/__init__.py
+-rw-r--r--   0        0        0       48 2024-05-16 18:47:45.020231 lacss-0.9.0/lacss/data/__init__.py
+-rw-r--r--   0        0        0    14546 2024-05-16 18:47:45.020231 lacss-0.9.0/lacss/data/augment.py
+-rw-r--r--   0        0        0    13109 2024-05-16 18:47:45.020231 lacss-0.9.0/lacss/data/generator.py
+-rw-r--r--   0        0        0       43 2024-05-16 18:47:45.020231 lacss-0.9.0/lacss/deploy/__init__.py
+-rw-r--r--   0        0        0    21615 2024-05-16 18:47:45.020231 lacss-0.9.0/lacss/deploy/predict.py
+-rw-r--r--   0        0        0        0 2024-05-16 18:47:45.020231 lacss-0.9.0/lacss/deploy/proto/__init__.py
+-rw-r--r--   0        0        0     1035 2024-05-16 18:47:45.020231 lacss-0.9.0/lacss/deploy/proto/lacss.proto
+-rw-r--r--   0        0        0     3382 2024-05-16 18:47:45.020231 lacss-0.9.0/lacss/deploy/proto/lacss_pb2.py
+-rw-r--r--   0        0        0     4000 2024-05-16 18:47:45.020231 lacss-0.9.0/lacss/deploy/proto/lacss_pb2.pyi
+-rw-r--r--   0        0        0     2382 2024-05-16 18:47:45.020231 lacss-0.9.0/lacss/deploy/proto/lacss_pb2_grpc.py
+-rw-r--r--   0        0        0     4484 2024-05-16 18:47:45.020231 lacss-0.9.0/lacss/deploy/remote_server.py
+-rw-r--r--   0        0        0     4139 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/deploy/server.py
+-rw-r--r--   0        0        0       74 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/losses/__init__.py
+-rw-r--r--   0        0        0     6115 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/losses/auxiliary.py
+-rw-r--r--   0        0        0      965 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/losses/common.py
+-rw-r--r--   0        0        0     1748 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/losses/detection.py
+-rw-r--r--   0        0        0     5406 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/losses/instance.py
+-rw-r--r--   0        0        0       22 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/metrics/__init__.py
+-rw-r--r--   0        0        0     5559 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/metrics/ranked.py
+-rw-r--r--   0        0        0      330 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/modules/__init__.py
+-rw-r--r--   0        0        0     2355 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/modules/common.py
+-rw-r--r--   0        0        0     7968 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/modules/convnext.py
+-rw-r--r--   0        0        0     7808 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/modules/detector.py
+-rw-r--r--   0        0        0     3899 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/modules/lacss.py
+-rw-r--r--   0        0        0     3292 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/modules/lpn.py
+-rw-r--r--   0        0        0     3830 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/modules/resnet.py
+-rw-r--r--   0        0        0     5557 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/modules/segmentor.py
+-rw-r--r--   0        0        0     2297 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/modules/unet.py
+-rw-r--r--   0        0        0      153 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/ops/__init__.py
+-rw-r--r--   0        0        0     2474 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/ops/boxes.py
+-rw-r--r--   0        0        0     3551 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/ops/image.py
+-rw-r--r--   0        0        0     3136 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/ops/locations.py
+-rw-r--r--   0        0        0     5961 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/ops/nms.py
+-rw-r--r--   0        0        0    11822 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/ops/patches.py
+-rw-r--r--   0        0        0      482 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/ops/uda.py
+-rw-r--r--   0        0        0       63 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/tracking/__init__.py
+-rw-r--r--   0        0        0     3340 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/tracking/predict.py
+-rw-r--r--   0        0        0    12670 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/tracking/seqnms.py
+-rw-r--r--   0        0        0     6741 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/tracking/smc.py
+-rw-r--r--   0        0        0     5646 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/tracking/utils.py
+-rw-r--r--   0        0        0      203 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/train/__init__.py
+-rw-r--r--   0        0        0    10358 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/train/base_trainer.py
+-rw-r--r--   0        0        0    10541 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/train/lacss_trainer.py
+-rw-r--r--   0        0        0     1170 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/train/loss.py
+-rw-r--r--   0        0        0     4564 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/train/strategy.py
+-rw-r--r--   0        0        0     5541 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/train/utils.py
+-rw-r--r--   0        0        0      931 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/typing.py
+-rw-r--r--   0        0        0     5151 2024-05-16 18:47:45.024231 lacss-0.9.0/lacss/utils.py
+-rw-r--r--   0        0        0     1057 2024-05-16 18:48:02.440390 lacss-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3300 1970-01-01 00:00:00.000000 lacss-0.9.0/PKG-INFO
```

### Comparing `lacss-0.8.1/LICENSE` & `lacss-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/README.md` & `lacss-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ## LACSS
 
 _LACSS is a deep-learning model for single-cell segmentation from microscopy images._ 
 
 References: 
 
-- [IEEE TMI doi:10.1109/TMI.2023.3312988](https://arxiv.org/abs/2304.10671)
+- [IEEE TMI doi:10.1109/TMI.2023.3312988](https://ieeexplore.ieee.org/document/10243149)
 - [Communications Biology 6,232 (2023)](https://www.nature.com/articles/s42003-023-04608-5)
 
 ### Installation
 ```
 pip install lacss
 ```
 For more details, see [documentation](https://jiyuuchc.github.io/lacss/install/)
```

### Comparing `lacss-0.8.1/lacss/data/augment.py` & `lacss-0.9.0/lacss/data/augment.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/data/generator.py` & `lacss-0.9.0/lacss/data/generator.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/deploy/lacss_pb2.py` & `lacss-0.9.0/lacss/deploy/proto/lacss_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: lacss.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0blacss.proto\x12\x0ftrackmate.lacss\"l\n\x05Image\x12\x0e\n\x06height\x18\x01 \x01(\x04\x12\r\n\x05width\x18\x02 \x01(\x04\x12\x0f\n\x07\x63hannel\x18\x03 \x01(\x04\x12%\n\x05\x64type\x18\x04 \x01(\x0e\x32\x16.trackmate.lacss.DType\x12\x0c\n\x04\x64\x61ta\x18\x05 \x01(\x0c\"\xb5\x01\n\x08Settings\x12\x15\n\rmin_cell_area\x18\x01 \x01(\x02\x12\x1b\n\x13remove_out_of_bound\x18\x02 \x01(\x08\x12\x0f\n\x07scaling\x18\x03 \x01(\x02\x12\x0f\n\x07nms_iou\x18\x04 \x01(\x02\x12\x1b\n\x13\x64\x65tection_threshold\x18\x05 \x01(\x02\x12\x1e\n\x16segmentation_threshold\x18\x06 \x01(\x02\x12\x16\n\x0ereturn_polygon\x18\x07 \x01(\x08\"[\n\x05Input\x12+\n\x08settings\x18\x01 \x01(\x0b\x32\x19.trackmate.lacss.Settings\x12%\n\x05image\x18\x02 \x01(\x0b\x32\x16.trackmate.lacss.Image\"4\n\x05Label\x12\x0e\n\x06height\x18\x01 \x01(\x04\x12\r\n\x05width\x18\x02 \x01(\x04\x12\x0c\n\x04\x64\x61ta\x18\x06 \x01(\x0c\"V\n\x06Result\x12%\n\x05score\x18\x01 \x01(\x0b\x32\x16.trackmate.lacss.Label\x12%\n\x05label\x18\x02 \x01(\x0b\x32\x16.trackmate.lacss.Label\"\x1d\n\x05Point\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\"@\n\x07Polygon\x12\r\n\x05score\x18\x01 \x01(\x02\x12&\n\x06points\x18\x02 \x03(\x0b\x32\x16.trackmate.lacss.Point\";\n\rPolygonResult\x12*\n\x08polygons\x18\x01 \x03(\x0b\x32\x18.trackmate.lacss.Polygon*\x14\n\x05\x44Type\x12\x0b\n\x07\x46LOAT32\x10\x00\x42\x30\n$fiji.plugin.trackmate.detector.lacssB\x08LacssMsgb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0blacss.proto\x12\x0ftrackmate.lacss\"l\n\x05Image\x12\x0e\n\x06height\x18\x01 \x01(\x04\x12\r\n\x05width\x18\x02 \x01(\x04\x12\x0f\n\x07\x63hannel\x18\x03 \x01(\x04\x12%\n\x05\x64type\x18\x04 \x01(\x0e\x32\x16.trackmate.lacss.DType\x12\x0c\n\x04\x64\x61ta\x18\x05 \x01(\x0c\"\xb5\x01\n\x08Settings\x12\x15\n\rmin_cell_area\x18\x01 \x01(\x02\x12\x1b\n\x13remove_out_of_bound\x18\x02 \x01(\x08\x12\x0f\n\x07scaling\x18\x03 \x01(\x02\x12\x0f\n\x07nms_iou\x18\x04 \x01(\x02\x12\x1b\n\x13\x64\x65tection_threshold\x18\x05 \x01(\x02\x12\x1e\n\x16segmentation_threshold\x18\x06 \x01(\x02\x12\x16\n\x0ereturn_polygon\x18\x07 \x01(\x08\"[\n\x05Input\x12+\n\x08settings\x18\x01 \x01(\x0b\x32\x19.trackmate.lacss.Settings\x12%\n\x05image\x18\x02 \x01(\x0b\x32\x16.trackmate.lacss.Image\"4\n\x05Label\x12\x0e\n\x06height\x18\x01 \x01(\x04\x12\r\n\x05width\x18\x02 \x01(\x04\x12\x0c\n\x04\x64\x61ta\x18\x06 \x01(\x0c\"V\n\x06Result\x12%\n\x05score\x18\x01 \x01(\x0b\x32\x16.trackmate.lacss.Label\x12%\n\x05label\x18\x02 \x01(\x0b\x32\x16.trackmate.lacss.Label\"\x1d\n\x05Point\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\"@\n\x07Polygon\x12\r\n\x05score\x18\x01 \x01(\x02\x12&\n\x06points\x18\x02 \x03(\x0b\x32\x16.trackmate.lacss.Point\";\n\rPolygonResult\x12*\n\x08polygons\x18\x01 \x03(\x0b\x32\x18.trackmate.lacss.Polygon*\x14\n\x05\x44Type\x12\x0b\n\x07\x46LOAT32\x10\x00\x32Q\n\x05Lacss\x12H\n\x0cRunDetection\x12\x16.trackmate.lacss.Input\x1a\x1e.trackmate.lacss.PolygonResult\"\x00\x42\x30\n$fiji.plugin.trackmate.detector.lacssB\x08LacssMsgb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'lacss_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n$fiji.plugin.trackmate.detector.lacssB\010LacssMsg'
@@ -35,8 +36,10 @@
   _globals['_RESULT']._serialized_end=559
   _globals['_POINT']._serialized_start=561
   _globals['_POINT']._serialized_end=590
   _globals['_POLYGON']._serialized_start=592
   _globals['_POLYGON']._serialized_end=656
   _globals['_POLYGONRESULT']._serialized_start=658
   _globals['_POLYGONRESULT']._serialized_end=717
+  _globals['_LACSS']._serialized_start=741
+  _globals['_LACSS']._serialized_end=822
 # @@protoc_insertion_point(module_scope)
```

### Comparing `lacss-0.8.1/lacss/deploy/predict.py` & `lacss-0.9.0/lacss/deploy/predict.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/deploy/server.py` & `lacss-0.9.0/lacss/deploy/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,60 +4,60 @@
 from zipfile import ZipFile
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 import typer
 
-import lacss.deploy.lacss_pb2 as LacssMsg
+import lacss.deploy.proto.lacss_pb2 as lacss_pb2
 from lacss.ops import patches_to_label, sorted_non_max_suppression
 
 from .predict import Predictor
 
 app = typer.Typer(pretty_exceptions_enable=False)
 
 def read_input(st = sys.stdin.buffer):
     msg_size = st.read(4)
     msg_size = struct.unpack(">i", msg_size)[0]
 
-    msg = LacssMsg.Input()
+    msg = lacss_pb2.Input()
     msg.ParseFromString(st.read(msg_size))
 
     image = msg.image
     np_img = np.frombuffer(image.data, dtype=">f4").astype("float32")
     np_img = np_img.reshape(image.height, image.width, image.channel)
     # np_img = np_img.transpose(2, 1, 0)
 
-    import imageio.v2 as imageio
-    imageio.imwrite("tmpin.tif", np_img)
+    # import imageio.v2 as imageio
+    # imageio.imwrite("tmpin.tif", np_img)
 
     return np_img, msg.settings
 
 def img_to_msg(msg, img):
     img = np.ascontiguousarray(img, dtype=">i2") # match java format
 
     msg.height = img.shape[0]
     msg.width = img.shape[1]
     msg.data = img.tobytes()
 
     assert len(msg.data) == msg.height * msg.width * 2
 
 def write_result(label, score, st = sys.stdout.buffer):
 
-    msg = LacssMsg.Result()
+    msg = lacss_pb2.Result()
     img_to_msg(msg.score, (score * 1000).astype(np.int16))
     img_to_msg(msg.label, label)
 
     msg_size_bits = struct.pack(">i", msg.ByteSize())
 
     st.write(msg_size_bits)
     st.write(msg.SerializeToString())
 
 def write_polygon_result(polygons, scores, st = sys.stdout.buffer):
-    msg = LacssMsg.PolygonResult()
+    msg = lacss_pb2.PolygonResult()
     for polygon, score in zip(polygons, scores):
         if len(polygon) > 1:
             polygon_msg = LacssMsg.Polygon()
             polygon_msg.score = score
             for p in polygon:
                 point = LacssMsg.Point()
                 point.x = p[0]
```

### Comparing `lacss-0.8.1/lacss/losses/auxiliary.py` & `lacss-0.9.0/lacss/losses/auxiliary.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/losses/common.py` & `lacss-0.9.0/lacss/losses/common.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/losses/detection.py` & `lacss-0.9.0/lacss/losses/detection.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/losses/instance.py` & `lacss-0.9.0/lacss/losses/instance.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/metrics/ranked.py` & `lacss-0.9.0/lacss/metrics/ranked.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/modules/common.py` & `lacss-0.9.0/lacss/modules/common.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/modules/convnext.py` & `lacss-0.9.0/lacss/modules/convnext.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/modules/detector.py` & `lacss-0.9.0/lacss/modules/detector.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/modules/lacss.py` & `lacss-0.9.0/lacss/modules/lacss.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/modules/lpn.py` & `lacss-0.9.0/lacss/modules/lpn.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/modules/resnet.py` & `lacss-0.9.0/lacss/modules/resnet.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/modules/segmentor.py` & `lacss-0.9.0/lacss/modules/segmentor.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/modules/unet.py` & `lacss-0.9.0/lacss/modules/unet.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/ops/boxes.py` & `lacss-0.9.0/lacss/ops/boxes.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/ops/image.py` & `lacss-0.9.0/lacss/ops/image.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/ops/locations.py` & `lacss-0.9.0/lacss/ops/locations.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/ops/nms.py` & `lacss-0.9.0/lacss/ops/nms.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/ops/patches.py` & `lacss-0.9.0/lacss/ops/patches.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/tracking/predict.py` & `lacss-0.9.0/lacss/tracking/predict.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/tracking/seqnms.py` & `lacss-0.9.0/lacss/tracking/seqnms.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/tracking/smc.py` & `lacss-0.9.0/lacss/tracking/smc.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/tracking/utils.py` & `lacss-0.9.0/lacss/tracking/utils.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/train/base_trainer.py` & `lacss-0.9.0/lacss/train/base_trainer.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/train/lacss_trainer.py` & `lacss-0.9.0/lacss/train/lacss_trainer.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/train/loss.py` & `lacss-0.9.0/lacss/train/loss.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/train/strategy.py` & `lacss-0.9.0/lacss/train/strategy.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/train/utils.py` & `lacss-0.9.0/lacss/train/utils.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/typing.py` & `lacss-0.9.0/lacss/typing.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/lacss/utils.py` & `lacss-0.9.0/lacss/utils.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.1/pyproject.toml` & `lacss-0.9.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 [tool.poetry]
 name = "lacss"
-version = "0.8.1"
+version = "0.9.0"
 description = "Cell segmentation and tracking"
 authors = ["Ji Yu <jyu@uchc.edu>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.10, <3.12"
 flax = "^0.7.2"
 tqdm = "^4.65.0"
 imageio = "^2.9.0"
 scikit-image = ">=0.19.0"
 typer = ">=0.4.0"
 imagecodecs = "^2023.3.16"
 opencv-python = "^4.8.1.78"
 orbax-checkpoint = "^0.5"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 jupyterlab = "^3.6.1"
 jax = {extras = ["cuda11-pip"], version = "^0.4.14"}
-tensorflow-cpu = "^2.13.0"
+tensorflow = "^2.13.0"
 protoc-wheel-0 = "^24.4"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.2.3"
 mkdocstrings = {extras = ["python"], version = "^0.22.0"}
 mkdocs-gen-files = "^0.5.0"
 
+
+[tool.poetry.group.grpc.dependencies]
+grpcio-tools = "^1.62.0"
+
 [[tool.poetry.source]]
 name = "jax"
 url = "https://storage.googleapis.com/jax-releases/jax_cuda_releases.html"
 priority = "supplemental"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `lacss-0.8.1/PKG-INFO` & `lacss-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: lacss
-Version: 0.8.1
+Version: 0.9.0
 Summary: Cell segmentation and tracking
 License: MIT
 Author: Ji Yu
 Author-email: jyu@uchc.edu
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: flax (>=0.7.2,<0.8.0)
 Requires-Dist: imagecodecs (>=2023.3.16,<2024.0.0)
 Requires-Dist: imageio (>=2.9.0,<3.0.0)
 Requires-Dist: opencv-python (>=4.8.1.78,<5.0.0.0)
 Requires-Dist: orbax-checkpoint (>=0.5,<0.6)
 Requires-Dist: scikit-image (>=0.19.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
@@ -23,15 +22,15 @@
 
 ## LACSS
 
 _LACSS is a deep-learning model for single-cell segmentation from microscopy images._ 
 
 References: 
 
-- [IEEE TMI doi:10.1109/TMI.2023.3312988](https://arxiv.org/abs/2304.10671)
+- [IEEE TMI doi:10.1109/TMI.2023.3312988](https://ieeexplore.ieee.org/document/10243149)
 - [Communications Biology 6,232 (2023)](https://www.nature.com/articles/s42003-023-04608-5)
 
 ### Installation
 ```
 pip install lacss
 ```
 For more details, see [documentation](https://jiyuuchc.github.io/lacss/install/)
```

