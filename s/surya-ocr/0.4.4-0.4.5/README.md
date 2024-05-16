# Comparing `tmp/surya_ocr-0.4.4.tar.gz` & `tmp/surya_ocr-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surya_ocr-0.4.4.tar", max compression
+gzip compressed data, was "surya_ocr-0.4.5.tar", max compression
```

## Comparing `surya_ocr-0.4.4.tar` & `surya_ocr-0.4.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    35085 2024-05-09 17:24:33.788128 surya_ocr-0.4.4/LICENSE
--rw-r--r--   0        0        0    24927 2024-05-09 17:24:33.788128 surya_ocr-0.4.4/README.md
--rw-r--r--   0        0        0     3084 2024-05-09 17:24:33.788128 surya_ocr-0.4.4/detect_layout.py
--rw-r--r--   0        0        0     3314 2024-05-09 17:24:33.788128 surya_ocr-0.4.4/detect_text.py
--rw-r--r--   0        0        0     6909 2024-05-09 17:24:33.788128 surya_ocr-0.4.4/ocr_app.py
--rw-r--r--   0        0        0     4112 2024-05-09 17:24:33.788128 surya_ocr-0.4.4/ocr_text.py
--rw-r--r--   0        0        0     1343 2024-05-09 17:24:33.792128 surya_ocr-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     3720 2024-05-09 17:24:33.792128 surya_ocr-0.4.4/reading_order.py
--rw-r--r--   0        0        0      530 2024-05-09 17:24:33.792128 surya_ocr-0.4.4/run_ocr_app.py
--rw-r--r--   0        0        0      827 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/benchmark/bbox.py
--rw-r--r--   0        0        0     4239 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/benchmark/metrics.py
--rw-r--r--   0        0        0     4971 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/benchmark/tesseract.py
--rw-r--r--   0        0        0      887 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/benchmark/util.py
--rw-r--r--   0        0        0     4802 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/detection.py
--rw-r--r--   0        0        0      603 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/input/langs.py
--rw-r--r--   0        0        0     2268 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/input/load.py
--rw-r--r--   0        0        0     3167 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/input/processing.py
--rw-r--r--   0        0        0     2138 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/languages.py
--rw-r--r--   0        0        0     8598 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/layout.py
--rw-r--r--   0        0        0     6139 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/model/detection/segformer.py
--rw-r--r--   0        0        0      159 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/model/ordering/config.py
--rw-r--r--   0        0        0    25734 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/model/ordering/decoder.py
--rw-r--r--   0        0        0     3670 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/model/ordering/encoder.py
--rw-r--r--   0        0        0     3902 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/model/ordering/encoderdecoder.py
--rw-r--r--   0        0        0     1568 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/model/ordering/model.py
--rw-r--r--   0        0        0     6199 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/model/ordering/processor.py
--rw-r--r--   0        0        0     1676 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/model/recognition/config.py
--rw-r--r--   0        0        0    32140 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/model/recognition/decoder.py
--rw-r--r--   0        0        0     2762 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/model/recognition/encoder.py
--rw-r--r--   0        0        0     2842 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/model/recognition/model.py
--rw-r--r--   0        0        0     9296 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/model/recognition/processor.py
--rw-r--r--   0        0        0     3588 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/model/recognition/tokenizer.py
--rw-r--r--   0        0        0     4154 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/ocr.py
--rw-r--r--   0        0        0     5667 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/ordering.py
--rw-r--r--   0        0        0     6085 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/postprocessing/affinity.py
--rw-r--r--   0        0        0      853 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/postprocessing/fonts.py
--rw-r--r--   0        0        0     7862 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/postprocessing/heatmap.py
--rw-r--r--   0        0        0     3313 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/postprocessing/math/latex.py
--rw-r--r--   0        0        0     3114 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/postprocessing/math/render.py
--rw-r--r--   0        0        0     4382 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/postprocessing/text.py
--rw-r--r--   0        0        0     1253 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/postprocessing/util.py
--rw-r--r--   0        0        0     3882 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/recognition.py
--rw-r--r--   0        0        0     4529 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/schema.py
--rw-r--r--   0        0        0     3615 2024-05-09 17:24:33.936128 surya_ocr-0.4.4/surya/settings.py
--rw-r--r--   0        0        0    26263 1970-01-01 00:00:00.000000 surya_ocr-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0    35085 2024-05-16 22:00:38.015767 surya_ocr-0.4.5/LICENSE
+-rw-r--r--   0        0        0    25121 2024-05-16 22:00:38.015767 surya_ocr-0.4.5/README.md
+-rw-r--r--   0        0        0     3084 2024-05-16 22:00:38.015767 surya_ocr-0.4.5/detect_layout.py
+-rw-r--r--   0        0        0     3314 2024-05-16 22:00:38.015767 surya_ocr-0.4.5/detect_text.py
+-rw-r--r--   0        0        0     6909 2024-05-16 22:00:38.015767 surya_ocr-0.4.5/ocr_app.py
+-rw-r--r--   0        0        0     4112 2024-05-16 22:00:38.015767 surya_ocr-0.4.5/ocr_text.py
+-rw-r--r--   0        0        0     1343 2024-05-16 22:00:38.019767 surya_ocr-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     3720 2024-05-16 22:00:38.019767 surya_ocr-0.4.5/reading_order.py
+-rw-r--r--   0        0        0      530 2024-05-16 22:00:38.019767 surya_ocr-0.4.5/run_ocr_app.py
+-rw-r--r--   0        0        0      827 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/benchmark/bbox.py
+-rw-r--r--   0        0        0     4239 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/benchmark/metrics.py
+-rw-r--r--   0        0        0     4971 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/benchmark/tesseract.py
+-rw-r--r--   0        0        0      887 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/benchmark/util.py
+-rw-r--r--   0        0        0     5460 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/detection.py
+-rw-r--r--   0        0        0      603 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/input/langs.py
+-rw-r--r--   0        0        0     2268 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/input/load.py
+-rw-r--r--   0        0        0     3486 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/input/processing.py
+-rw-r--r--   0        0        0     2138 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/languages.py
+-rw-r--r--   0        0        0     8598 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/layout.py
+-rw-r--r--   0        0        0     5902 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/model/detection/segformer.py
+-rw-r--r--   0        0        0      159 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/model/ordering/config.py
+-rw-r--r--   0        0        0    25734 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/model/ordering/decoder.py
+-rw-r--r--   0        0        0     3670 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/model/ordering/encoder.py
+-rw-r--r--   0        0        0     3902 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/model/ordering/encoderdecoder.py
+-rw-r--r--   0        0        0     1568 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/model/ordering/model.py
+-rw-r--r--   0        0        0     6199 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/model/ordering/processor.py
+-rw-r--r--   0        0        0     1676 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/model/recognition/config.py
+-rw-r--r--   0        0        0    32140 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/model/recognition/decoder.py
+-rw-r--r--   0        0        0     2762 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/model/recognition/encoder.py
+-rw-r--r--   0        0        0     2842 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/model/recognition/model.py
+-rw-r--r--   0        0        0     9296 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/model/recognition/processor.py
+-rw-r--r--   0        0        0     3588 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/model/recognition/tokenizer.py
+-rw-r--r--   0        0        0     4154 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/ocr.py
+-rw-r--r--   0        0        0     5848 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/ordering.py
+-rw-r--r--   0        0        0     6085 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/postprocessing/affinity.py
+-rw-r--r--   0        0        0      853 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/postprocessing/fonts.py
+-rw-r--r--   0        0        0     7833 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/postprocessing/heatmap.py
+-rw-r--r--   0        0        0     3313 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/postprocessing/math/latex.py
+-rw-r--r--   0        0        0     3114 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/postprocessing/math/render.py
+-rw-r--r--   0        0        0     4382 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/postprocessing/text.py
+-rw-r--r--   0        0        0     1253 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/postprocessing/util.py
+-rw-r--r--   0        0        0     3882 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/recognition.py
+-rw-r--r--   0        0        0     4529 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/schema.py
+-rw-r--r--   0        0        0     3615 2024-05-16 22:00:38.163767 surya_ocr-0.4.5/surya/settings.py
+-rw-r--r--   0        0        0    26457 1970-01-01 00:00:00.000000 surya_ocr-0.4.5/PKG-INFO
```

### Comparing `surya_ocr-0.4.4/LICENSE` & `surya_ocr-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/README.md` & `surya_ocr-0.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,20 @@
 | Presentation     |   [Image](static/images/pres.png)   |     [Image](static/images/pres_text.jpg) |     [Image](static/images/pres_layout.jpg) |     [Image](static/images/pres_reading.jpg) |
 | Scientific Paper |  [Image](static/images/paper.jpg)   |    [Image](static/images/paper_text.jpg) |    [Image](static/images/paper_layout.jpg) |    [Image](static/images/paper_reading.jpg) |
 | Scanned Document | [Image](static/images/scanned.png)  |  [Image](static/images/scanned_text.jpg) |  [Image](static/images/scanned_layout.jpg) |  [Image](static/images/scanned_reading.jpg) |
 | New York Times   |   [Image](static/images/nyt.jpg)    |      [Image](static/images/nyt_text.jpg) |      [Image](static/images/nyt_layout.jpg) |        [Image](static/images/nyt_order.jpg) |
 | Scanned Form     |  [Image](static/images/funsd.png)   |    [Image](static/images/funsd_text.jpg) |    [Image](static/images/funsd_layout.jpg) |    [Image](static/images/funsd_reading.jpg) |
 | Textbook         | [Image](static/images/textbook.jpg) | [Image](static/images/textbook_text.jpg) | [Image](static/images/textbook_layout.jpg) |   [Image](static/images/textbook_order.jpg) |
 
+# Commercial usage
+
+I want surya to be as widely accessible as possible, while still funding my development/training costs. Research and personal usage is always okay, but there are some restrictions on commercial usage.
+
+The weights for the models are licensed `cc-by-nc-sa-4.0`, but I will waive that for any organization under $5M USD in gross revenue in the most recent 12-month period AND under $5M in lifetime VC/angel funding raised. If you want to remove the GPL license requirements (dual-license) and/or use the weights commercially over the revenue limit, check out the options [here](https://www.datalab.to).
+
 # Installation
 
 You'll need python 3.9+ and PyTorch. You may need to install the CPU version of torch first if you're not using a Mac or a GPU machine.  See [here](https://pytorch.org/get-started/locally/) for more details.
 
 Install with:
 
 ```shell
@@ -424,20 +430,14 @@
 
 # Training
 
 Text detection was trained on 4x A6000s for 3 days.  It used a diverse set of images as training data.  It was trained from scratch using a modified segformer architecture that reduces inference RAM requirements.
 
 Text recognition was trained on 4x A6000s for 2 weeks.  It was trained using a modified donut model (GQA, MoE layer, UTF-16 decoding, layer config changes).
 
-# Commercial usage
-
-All models were trained from scratch, so they're okay for commercial usage.  The weights are licensed cc-by-nc-sa-4.0, but I will waive that for any organization under $5M USD in gross revenue in the most recent 12-month period.
-
-If you want to remove the GPL license requirements for inference or use the weights commercially over the revenue limit, please contact me at surya@vikas.sh for dual licensing.
-
 # Thanks
 
 This work would not have been possible without amazing open source AI work:
 
 - [Segformer](https://arxiv.org/pdf/2105.15203.pdf) from NVIDIA
 - [Donut](https://github.com/clovaai/donut) from Naver
 - [transformers](https://github.com/huggingface/transformers) from huggingface
```

### Comparing `surya_ocr-0.4.4/detect_layout.py` & `surya_ocr-0.4.5/detect_layout.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/detect_text.py` & `surya_ocr-0.4.5/detect_text.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/ocr_app.py` & `surya_ocr-0.4.5/ocr_app.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/ocr_text.py` & `surya_ocr-0.4.5/ocr_text.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/pyproject.toml` & `surya_ocr-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "surya-ocr"
-version = "0.4.4"
+version = "0.4.5"
 description = "OCR, layout, reading order, and line detection in 90+ languages"
 authors = ["Vik Paruchuri <vik.paruchuri@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 repository = "https://github.com/VikParuchuri/surya"
 keywords = ["ocr", "pdf", "text detection", "text recognition"]
 packages = [
```

### Comparing `surya_ocr-0.4.4/reading_order.py` & `surya_ocr-0.4.5/reading_order.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/run_ocr_app.py` & `surya_ocr-0.4.5/run_ocr_app.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/benchmark/bbox.py` & `surya_ocr-0.4.5/surya/benchmark/bbox.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/benchmark/metrics.py` & `surya_ocr-0.4.5/surya/benchmark/metrics.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/benchmark/tesseract.py` & `surya_ocr-0.4.5/surya/benchmark/tesseract.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/benchmark/util.py` & `surya_ocr-0.4.5/surya/benchmark/util.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/detection.py` & `surya_ocr-0.4.5/surya/detection.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,96 +1,108 @@
-import os
 from typing import List, Tuple
 
-import cv2
 import torch
 import numpy as np
 from PIL import Image
+
+from surya.model.detection.segformer import SegformerForRegressionMask
 from surya.postprocessing.heatmap import get_and_clean_boxes
 from surya.postprocessing.affinity import get_vertical_lines, get_horizontal_lines
-from surya.input.processing import prepare_image, split_image
+from surya.input.processing import prepare_image, split_image, get_total_splits
 from surya.schema import TextDetectionResult
 from surya.settings import settings
 from tqdm import tqdm
 from concurrent.futures import ProcessPoolExecutor
+import torch.nn.functional as F
 
 
 def get_batch_size():
     batch_size = settings.DETECTOR_BATCH_SIZE
     if batch_size is None:
         batch_size = 6
         if settings.TORCH_DEVICE_MODEL == "cuda":
             batch_size = 24
     return batch_size
 
 
-def batch_detection(images: List, model, processor, batch_size=None) -> Tuple[List[List[np.ndarray]], List[Tuple[int, int]]]:
+def batch_detection(images: List, model: SegformerForRegressionMask, processor, batch_size=None) -> Tuple[List[List[np.ndarray]], List[Tuple[int, int]]]:
     assert all([isinstance(image, Image.Image) for image in images])
     if batch_size is None:
         batch_size = get_batch_size()
     heatmap_count = model.config.num_labels
 
-    images = [image.convert("RGB") for image in images]
     orig_sizes = [image.size for image in images]
-    split_index = []
-    split_heights = []
-    image_splits = []
-    for i, image in enumerate(images):
-        image_parts, split_height = split_image(image, processor)
-        image_splits.extend(image_parts)
-        split_index.extend([i] * len(image_parts))
-        split_heights.extend(split_height)
-
-    image_splits = [prepare_image(image, processor) for image in image_splits]
-
-    pred_parts = []
-    for i in tqdm(range(0, len(image_splits), batch_size), desc="Detecting bboxes"):
-        batch = image_splits[i:i+batch_size]
+    splits_per_image = [get_total_splits(size, processor) for size in orig_sizes]
+
+    batches = []
+    current_batch_size = 0
+    current_batch = []
+    for i in range(len(images)):
+        if current_batch_size + splits_per_image[i] > batch_size:
+            if len(current_batch) > 0:
+                batches.append(current_batch)
+            current_batch = []
+            current_batch_size = 0
+        current_batch.append(i)
+        current_batch_size += splits_per_image[i]
+
+    if len(current_batch) > 0:
+        batches.append(current_batch)
+
+    all_preds = []
+    for batch_idx in tqdm(range(len(batches)), desc="Detecting bboxes"):
+        batch_image_idxs = batches[batch_idx]
+        batch_images = [images[j].convert("RGB") for j in batch_image_idxs]
+
+        split_index = []
+        split_heights = []
+        image_splits = []
+        for image_idx, image in enumerate(batch_images):
+            image_parts, split_height = split_image(image, processor)
+            image_splits.extend(image_parts)
+            split_index.extend([image_idx] * len(image_parts))
+            split_heights.extend(split_height)
+
+        image_splits = [prepare_image(image, processor) for image in image_splits]
         # Batch images in dim 0
-        batch = torch.stack(batch, dim=0)
-        batch = batch.to(model.dtype)
-        batch = batch.to(model.device)
+        batch = torch.stack(image_splits, dim=0).to(model.dtype).to(model.device)
 
         with torch.inference_mode():
             pred = model(pixel_values=batch)
 
         logits = pred.logits
-        for j in range(logits.shape[0]):
-            heatmaps = []
-            for k in range(heatmap_count):
-                heatmap = logits[j, k, :, :].detach().cpu().numpy().astype(np.float32)
-                heatmap_shape = list(heatmap.shape)
-
-                correct_shape = [processor.size["height"], processor.size["width"]]
-                cv2_size = list(reversed(correct_shape)) # opencv uses (width, height) instead of (height, width)
-                if heatmap_shape != correct_shape:
-                    heatmap = cv2.resize(heatmap, cv2_size, interpolation=cv2.INTER_LINEAR)
-
-                heatmaps.append(heatmap)
-            pred_parts.append(heatmaps)
-
-    preds = []
-    for i, (idx, height) in enumerate(zip(split_index, split_heights)):
-        if len(preds) <= idx:
-            preds.append(pred_parts[i])
-        else:
-            heatmaps = preds[idx]
-            pred_heatmaps = [pred_parts[i][k] for k in range(heatmap_count)]
-
-            if height < processor.size["height"]:
-                # Cut off padding to get original height
-                pred_heatmaps = [pred_heatmap[:height, :] for pred_heatmap in pred_heatmaps]
-
-            for k in range(heatmap_count):
-                heatmaps[k] = np.vstack([heatmaps[k], pred_heatmaps[k]])
-            preds[idx] = heatmaps
-
-    assert len(preds) == len(images)
-    assert all([len(pred) == heatmap_count for pred in preds])
-    return preds, orig_sizes
+        correct_shape = [processor.size["height"], processor.size["width"]]
+        current_shape = list(logits.shape[2:])
+        if current_shape != correct_shape:
+            logits = F.interpolate(logits, size=correct_shape, mode='bilinear', align_corners=False)
+
+        logits = logits.cpu().detach().numpy().astype(np.float32)
+        preds = []
+        for i, (idx, height) in enumerate(zip(split_index, split_heights)):
+            # If our current prediction length is below the image idx, that means we have a new image
+            # Otherwise, we need to add to the current image
+            if len(preds) <= idx:
+                preds.append([logits[i][k] for k in range(heatmap_count)])
+            else:
+                heatmaps = preds[idx]
+                pred_heatmaps = [logits[i][k] for k in range(heatmap_count)]
+
+                if height < processor.size["height"]:
+                    # Cut off padding to get original height
+                    pred_heatmaps = [pred_heatmap[:height, :] for pred_heatmap in pred_heatmaps]
+
+                for k in range(heatmap_count):
+                    heatmaps[k] = np.vstack([heatmaps[k], pred_heatmaps[k]])
+                preds[idx] = heatmaps
+
+        all_preds.extend(preds)
+
+    assert len(all_preds) == len(images)
+    assert all([len(pred) == heatmap_count for pred in all_preds])
+    return all_preds, orig_sizes
 
 
 def parallel_get_lines(preds, orig_sizes):
     heatmap, affinity_map = preds
     heat_img = Image.fromarray((heatmap * 255).astype(np.uint8))
     aff_img = Image.fromarray((affinity_map * 255).astype(np.uint8))
     affinity_size = list(reversed(affinity_map.shape))
```

### Comparing `surya_ocr-0.4.4/surya/input/langs.py` & `surya_ocr-0.4.5/surya/input/langs.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/input/load.py` & `surya_ocr-0.4.5/surya/input/load.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/input/processing.py` & `surya_ocr-0.4.5/surya/input/processing.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,24 @@
 import math
 import pypdfium2
 from PIL import Image, ImageOps, ImageDraw
 import torch
 from surya.settings import settings
 
 
+def get_total_splits(image_size, processor):
+    img_height = list(image_size)[1]
+    max_height = settings.DETECTOR_IMAGE_CHUNK_HEIGHT
+    processor_height = processor.size["height"]
+    if img_height > max_height:
+        num_splits = math.ceil(img_height / processor_height)
+        return num_splits
+    return 1
+
+
 def split_image(img, processor):
     # This will not modify/return the original image - it will either crop, or copy the image
     img_height = list(img.size)[1]
     max_height = settings.DETECTOR_IMAGE_CHUNK_HEIGHT
     processor_height = processor.size["height"]
     if img_height > max_height:
         num_splits = math.ceil(img_height / processor_height)
```

### Comparing `surya_ocr-0.4.4/surya/languages.py` & `surya_ocr-0.4.5/surya/languages.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/layout.py` & `surya_ocr-0.4.5/surya/layout.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/model/detection/segformer.py` & `surya_ocr-0.4.5/surya/model/detection/segformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import gc
 import warnings
 warnings.filterwarnings("ignore", message="torch.utils._pytree._register_pytree_node is deprecated")
 
 import math
 from typing import Optional, Tuple, Union
 
 from transformers import SegformerConfig, SegformerForSemanticSegmentation, SegformerImageProcessor, \
@@ -115,30 +116,27 @@
         pixel_values: torch.FloatTensor,
         labels: Optional[torch.LongTensor] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
     ) -> Union[Tuple, SemanticSegmenterOutput]:
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
-        output_hidden_states = (
-            output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
-        )
 
         outputs = self.segformer(
             pixel_values,
             output_attentions=output_attentions,
             output_hidden_states=True,  # we need the intermediate hidden states
-            return_dict=return_dict,
+            return_dict=False,
         )
 
-        encoder_hidden_states = outputs.hidden_states if return_dict else outputs[1]
+        encoder_hidden_states = outputs[1]
 
         logits = self.decode_head(encoder_hidden_states)
         # Apply sigmoid to get 0-1 output
-        logits = torch.special.expit(logits)
+        sigmoid_logits = torch.special.expit(logits)
 
         return SemanticSegmenterOutput(
             loss=None,
-            logits=logits,
-            hidden_states=outputs.hidden_states if output_hidden_states else None,
-            attentions=outputs.attentions,
+            logits=sigmoid_logits,
+            hidden_states=None,
+            attentions=None,
         )
```

### Comparing `surya_ocr-0.4.4/surya/model/ordering/decoder.py` & `surya_ocr-0.4.5/surya/model/ordering/decoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/model/ordering/encoder.py` & `surya_ocr-0.4.5/surya/model/ordering/encoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/model/ordering/encoderdecoder.py` & `surya_ocr-0.4.5/surya/model/ordering/encoderdecoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/model/ordering/model.py` & `surya_ocr-0.4.5/surya/model/ordering/model.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/model/ordering/processor.py` & `surya_ocr-0.4.5/surya/model/ordering/processor.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/model/recognition/config.py` & `surya_ocr-0.4.5/surya/model/recognition/config.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/model/recognition/decoder.py` & `surya_ocr-0.4.5/surya/model/recognition/decoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/model/recognition/encoder.py` & `surya_ocr-0.4.5/surya/model/recognition/encoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/model/recognition/model.py` & `surya_ocr-0.4.5/surya/model/recognition/model.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/model/recognition/processor.py` & `surya_ocr-0.4.5/surya/model/recognition/processor.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/model/recognition/tokenizer.py` & `surya_ocr-0.4.5/surya/model/recognition/tokenizer.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/ocr.py` & `surya_ocr-0.4.5/surya/ocr.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/ordering.py` & `surya_ocr-0.4.5/surya/ordering.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from copy import deepcopy
 from typing import List, Optional
 import torch
 from PIL import Image
 
+from surya.model.ordering.encoderdecoder import OrderVisionEncoderDecoderModel
 from surya.schema import OrderBox, OrderResult
 from surya.settings import settings
 from tqdm import tqdm
 import numpy as np
 
 
 def get_batch_size():
@@ -26,15 +27,15 @@
 
     for rank_value, (original_index, value) in enumerate(enumerated_and_sorted):
         rank[original_index] = rank_value
 
     return rank
 
 
-def batch_ordering(images: List, bboxes: List[List[List[float]]], model, processor, batch_size=None) -> List[OrderResult]:
+def batch_ordering(images: List, bboxes: List[List[List[float]]], model: OrderVisionEncoderDecoderModel, processor, batch_size=None) -> List[OrderResult]:
     assert all([isinstance(image, Image.Image) for image in images])
     assert len(images) == len(bboxes)
     if batch_size is None:
         batch_size = get_batch_size()
 
     images = [image.convert("RGB") for image in images]
 
@@ -55,60 +56,60 @@
         batch_pixel_values = torch.tensor(np.array(batch_pixel_values), dtype=model.dtype).to(model.device)
         batch_bbox_counts = torch.tensor(np.array(batch_bbox_counts), dtype=torch.long).to(model.device)
 
         token_count = 0
         past_key_values = None
         encoder_outputs = None
         batch_predictions = [[] for _ in range(len(batch_images))]
-        done = [False for _ in range(len(batch_images))]
-        while token_count < settings.ORDER_MAX_BOXES:
-            with torch.inference_mode():
+        done = torch.zeros(len(batch_images), dtype=torch.bool, device=model.device)
+
+        with torch.inference_mode():
+            while token_count < settings.ORDER_MAX_BOXES:
                 return_dict = model(
                     pixel_values=batch_pixel_values,
                     decoder_input_boxes=batch_bboxes,
                     decoder_input_boxes_mask=batch_bbox_mask,
                     decoder_input_boxes_counts=batch_bbox_counts,
                     encoder_outputs=encoder_outputs,
                     past_key_values=past_key_values,
                 )
-                logits = return_dict["logits"].detach().cpu()
+                logits = return_dict["logits"].detach()
 
-            last_tokens = []
-            last_token_mask = []
-            min_val = torch.finfo(model.dtype).min
-            for j in range(logits.shape[0]):
-                label_count = batch_bbox_counts[j, 1] - batch_bbox_counts[j, 0] - 1 # Subtract 1 for the sep token
-                new_logits = logits[j, -1].clone()
-                new_logits[batch_predictions[j]] = min_val # Mask out already predicted tokens, we can only predict each token once
-                new_logits[label_count:] = min_val # Mask out all logit positions above the number of bboxes
-                pred = int(torch.argmax(new_logits, dim=-1).item())
-
-                # Add one to avoid colliding with the 1000 height/width token for bboxes
-                last_tokens.append([[pred + processor.box_size["height"] + 1] * 4])
-                if len(batch_predictions[j]) == label_count - 1: # Minus one since we're appending the final label
-                    last_token_mask.append([0])
-                    batch_predictions[j].append(pred)
-                    done[j] = True
-                elif len(batch_predictions[j]) < label_count - 1:
-                    last_token_mask.append([1])
-                    batch_predictions[j].append(pred)  # Get rank prediction for given position
-                else:
-                    last_token_mask.append([0])
-
-            # Break when we finished generating all sequences
-            if all(done):
-                break
-
-            past_key_values = return_dict["past_key_values"]
-            encoder_outputs = (return_dict["encoder_last_hidden_state"],)
-
-            batch_bboxes = torch.tensor(last_tokens, dtype=torch.long).to(model.device)
-            token_bbox_mask = torch.tensor(last_token_mask, dtype=torch.long).to(model.device)
-            batch_bbox_mask = torch.cat([batch_bbox_mask, token_bbox_mask], dim=1)
-            token_count += 1
+                last_tokens = []
+                last_token_mask = []
+                min_val = torch.finfo(model.dtype).min
+                for j in range(logits.shape[0]):
+                    label_count = batch_bbox_counts[j, 1] - batch_bbox_counts[j, 0] - 1  # Subtract 1 for the sep token
+                    new_logits = logits[j, -1]
+                    new_logits[batch_predictions[j]] = min_val  # Mask out already predicted tokens, we can only predict each token once
+                    new_logits[label_count:] = min_val  # Mask out all logit positions above the number of bboxes
+                    pred = int(torch.argmax(new_logits, dim=-1).item())
+
+                    # Add one to avoid colliding with the 1000 height/width token for bboxes
+                    last_tokens.append([[pred + processor.box_size["height"] + 1] * 4])
+                    if len(batch_predictions[j]) == label_count - 1:  # Minus one since we're appending the final label
+                        last_token_mask.append([0])
+                        batch_predictions[j].append(pred)
+                        done[j] = True
+                    elif len(batch_predictions[j]) < label_count - 1:
+                        last_token_mask.append([1])
+                        batch_predictions[j].append(pred)  # Get rank prediction for given position
+                    else:
+                        last_token_mask.append([0])
+
+                if done.all():
+                    break
+
+                past_key_values = return_dict["past_key_values"]
+                encoder_outputs = (return_dict["encoder_last_hidden_state"],)
+
+                batch_bboxes = torch.tensor(last_tokens, dtype=torch.long).to(model.device)
+                token_bbox_mask = torch.tensor(last_token_mask, dtype=torch.long).to(model.device)
+                batch_bbox_mask = torch.cat([batch_bbox_mask, token_bbox_mask], dim=1)
+                token_count += 1
 
         for j, row_pred in enumerate(batch_predictions):
             row_bboxes = bboxes[i+j]
             assert len(row_pred) == len(row_bboxes), f"Mismatch between logits and bboxes. Logits: {len(row_pred)}, Bboxes: {len(row_bboxes)}"
 
             orig_size = orig_sizes[j]
             ranks = [0] * len(row_bboxes)
```

### Comparing `surya_ocr-0.4.4/surya/postprocessing/affinity.py` & `surya_ocr-0.4.5/surya/postprocessing/affinity.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/postprocessing/fonts.py` & `surya_ocr-0.4.5/surya/postprocessing/fonts.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/postprocessing/heatmap.py` & `surya_ocr-0.4.5/surya/postprocessing/heatmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,14 @@
     text_threshold = min(text_threshold, 0.8)
     return text_threshold, low_text
 
 
 def detect_boxes(linemap, text_threshold, low_text):
     # From CRAFT - https://github.com/clovaai/CRAFT-pytorch
     # prepare data
-    linemap = linemap.copy()
     img_h, img_w = linemap.shape
 
     text_threshold, low_text = get_dynamic_thresholds(linemap, text_threshold, low_text)
 
     ret, text_score = cv2.threshold(linemap, low_text, 1, cv2.THRESH_BINARY)
 
     text_score_comb = np.clip(text_score, 0, 1)
```

### Comparing `surya_ocr-0.4.4/surya/postprocessing/math/latex.py` & `surya_ocr-0.4.5/surya/postprocessing/math/latex.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/postprocessing/math/render.py` & `surya_ocr-0.4.5/surya/postprocessing/math/render.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/postprocessing/text.py` & `surya_ocr-0.4.5/surya/postprocessing/text.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/postprocessing/util.py` & `surya_ocr-0.4.5/surya/postprocessing/util.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/recognition.py` & `surya_ocr-0.4.5/surya/recognition.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/schema.py` & `surya_ocr-0.4.5/surya/schema.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/surya/settings.py` & `surya_ocr-0.4.5/surya/settings.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.4/PKG-INFO` & `surya_ocr-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surya-ocr
-Version: 0.4.4
+Version: 0.4.5
 Summary: OCR, layout, reading order, and line detection in 90+ languages
 Home-page: https://github.com/VikParuchuri/surya
 License: GPL-3.0-or-later
 Keywords: ocr,pdf,text detection,text recognition
 Author: Vik Paruchuri
 Author-email: vik.paruchuri@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
@@ -65,14 +65,20 @@
 | Presentation     |   [Image](static/images/pres.png)   |     [Image](static/images/pres_text.jpg) |     [Image](static/images/pres_layout.jpg) |     [Image](static/images/pres_reading.jpg) |
 | Scientific Paper |  [Image](static/images/paper.jpg)   |    [Image](static/images/paper_text.jpg) |    [Image](static/images/paper_layout.jpg) |    [Image](static/images/paper_reading.jpg) |
 | Scanned Document | [Image](static/images/scanned.png)  |  [Image](static/images/scanned_text.jpg) |  [Image](static/images/scanned_layout.jpg) |  [Image](static/images/scanned_reading.jpg) |
 | New York Times   |   [Image](static/images/nyt.jpg)    |      [Image](static/images/nyt_text.jpg) |      [Image](static/images/nyt_layout.jpg) |        [Image](static/images/nyt_order.jpg) |
 | Scanned Form     |  [Image](static/images/funsd.png)   |    [Image](static/images/funsd_text.jpg) |    [Image](static/images/funsd_layout.jpg) |    [Image](static/images/funsd_reading.jpg) |
 | Textbook         | [Image](static/images/textbook.jpg) | [Image](static/images/textbook_text.jpg) | [Image](static/images/textbook_layout.jpg) |   [Image](static/images/textbook_order.jpg) |
 
+# Commercial usage
+
+I want surya to be as widely accessible as possible, while still funding my development/training costs. Research and personal usage is always okay, but there are some restrictions on commercial usage.
+
+The weights for the models are licensed `cc-by-nc-sa-4.0`, but I will waive that for any organization under $5M USD in gross revenue in the most recent 12-month period AND under $5M in lifetime VC/angel funding raised. If you want to remove the GPL license requirements (dual-license) and/or use the weights commercially over the revenue limit, check out the options [here](https://www.datalab.to).
+
 # Installation
 
 You'll need python 3.9+ and PyTorch. You may need to install the CPU version of torch first if you're not using a Mac or a GPU machine.  See [here](https://pytorch.org/get-started/locally/) for more details.
 
 Install with:
 
 ```shell
@@ -454,20 +460,14 @@
 
 # Training
 
 Text detection was trained on 4x A6000s for 3 days.  It used a diverse set of images as training data.  It was trained from scratch using a modified segformer architecture that reduces inference RAM requirements.
 
 Text recognition was trained on 4x A6000s for 2 weeks.  It was trained using a modified donut model (GQA, MoE layer, UTF-16 decoding, layer config changes).
 
-# Commercial usage
-
-All models were trained from scratch, so they're okay for commercial usage.  The weights are licensed cc-by-nc-sa-4.0, but I will waive that for any organization under $5M USD in gross revenue in the most recent 12-month period.
-
-If you want to remove the GPL license requirements for inference or use the weights commercially over the revenue limit, please contact me at surya@vikas.sh for dual licensing.
-
 # Thanks
 
 This work would not have been possible without amazing open source AI work:
 
 - [Segformer](https://arxiv.org/pdf/2105.15203.pdf) from NVIDIA
 - [Donut](https://github.com/clovaai/donut) from Naver
 - [transformers](https://github.com/huggingface/transformers) from huggingface
```

