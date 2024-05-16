# Comparing `tmp/marker_pdf-0.2.5.tar.gz` & `tmp/marker_pdf-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marker_pdf-0.2.5.tar", max compression
+gzip compressed data, was "marker_pdf-0.2.6.tar", max compression
```

## Comparing `marker_pdf-0.2.5.tar` & `marker_pdf-0.2.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    35101 2024-05-10 16:02:45.056295 marker_pdf-0.2.5/LICENSE
--rw-r--r--   0        0        0    12609 2024-05-10 16:02:45.056295 marker_pdf-0.2.5/README.md
--rwxr-xr-x   0        0        0      638 2024-05-10 16:02:45.056295 marker_pdf-0.2.5/chunk_convert.py
--rwxr-xr-x   0        0        0     1151 2024-05-10 16:02:45.056295 marker_pdf-0.2.5/chunk_convert.sh
--rwxr-xr-x   0        0        0     4853 2024-05-10 16:02:45.056295 marker_pdf-0.2.5/convert.py
--rwxr-xr-x   0        0        0     1246 2024-05-10 16:02:45.056295 marker_pdf-0.2.5/convert_single.py
--rw-r--r--   0        0        0     1376 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/benchmark/scoring.py
--rw-r--r--   0        0        0      231 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/cleaners/bullets.py
--rw-r--r--   0        0        0     4457 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/cleaners/code.py
--rw-r--r--   0        0        0      950 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/cleaners/fontstyle.py
--rw-r--r--   0        0        0     2766 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/cleaners/headers.py
--rw-r--r--   0        0        0     2456 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/cleaners/headings.py
--rw-r--r--   0        0        0      248 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/cleaners/text.py
--rw-r--r--   0        0        0     5164 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/convert.py
--rw-r--r--   0        0        0     2450 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/debug/data.py
--rw-r--r--   0        0        0     7884 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/equations/equations.py
--rw-r--r--   0        0        0     1549 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/equations/inference.py
--rw-r--r--   0        0        0     2594 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/images/extract.py
--rw-r--r--   0        0        0      473 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/images/save.py
--rw-r--r--   0        0        0     1928 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/layout/layout.py
--rw-r--r--   0        0        0     2516 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/layout/order.py
--rw-r--r--   0        0        0      396 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/logger.py
--rw-r--r--   0        0        0     2178 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/models.py
--rw-r--r--   0        0        0      888 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/ocr/detection.py
--rw-r--r--   0        0        0     2468 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/ocr/heuristics.py
--rw-r--r--   0        0        0     1223 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/ocr/lang.py
--rw-r--r--   0        0        0     5742 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/ocr/recognition.py
--rw-r--r--   0        0        0     2180 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/ocr/tesseract.py
--rw-r--r--   0        0        0      258 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/ocr/utils.py
--rw-r--r--   0        0        0     1266 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/output.py
--rw-r--r--   0        0        0     3932 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/pdf/extract_text.py
--rw-r--r--   0        0        0      817 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/pdf/images.py
--rw-r--r--   0        0        0     2442 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/pdf/utils.py
--rw-r--r--   0        0        0     3904 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/postprocessors/editor.py
--rw-r--r--   0        0        0     7226 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/postprocessors/markdown.py
--rw-r--r--   0        0        0     4977 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/postprocessors/t5.py
--rw-r--r--   0        0        0     2849 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/schema/bbox.py
--rw-r--r--   0        0        0     3259 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/schema/block.py
--rw-r--r--   0        0        0      502 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/schema/merged.py
--rw-r--r--   0        0        0     1618 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/schema/page.py
--rw-r--r--   0        0        0     4238 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/settings.py
--rw-r--r--   0        0        0     3384 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/tables/cells.py
--rw-r--r--   0        0        0     7178 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/tables/table.py
--rw-r--r--   0        0        0     1128 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/tables/utils.py
--rw-r--r--   0        0        0      156 2024-05-10 16:02:45.064295 marker_pdf-0.2.5/marker/utils.py
--rw-r--r--   0        0        0     1338 2024-05-10 16:02:45.068295 marker_pdf-0.2.5/pyproject.toml
--rw-r--r--   0        0        0    14231 1970-01-01 00:00:00.000000 marker_pdf-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    35101 2024-05-16 22:46:38.271131 marker_pdf-0.2.6/LICENSE
+-rw-r--r--   0        0        0    12609 2024-05-16 22:46:38.271131 marker_pdf-0.2.6/README.md
+-rwxr-xr-x   0        0        0      638 2024-05-16 22:46:38.271131 marker_pdf-0.2.6/chunk_convert.py
+-rwxr-xr-x   0        0        0     1151 2024-05-16 22:46:38.271131 marker_pdf-0.2.6/chunk_convert.sh
+-rwxr-xr-x   0        0        0     4853 2024-05-16 22:46:38.271131 marker_pdf-0.2.6/convert.py
+-rwxr-xr-x   0        0        0     1246 2024-05-16 22:46:38.271131 marker_pdf-0.2.6/convert_single.py
+-rw-r--r--   0        0        0     1376 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/benchmark/scoring.py
+-rw-r--r--   0        0        0      231 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/cleaners/bullets.py
+-rw-r--r--   0        0        0     4457 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/cleaners/code.py
+-rw-r--r--   0        0        0      950 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/cleaners/fontstyle.py
+-rw-r--r--   0        0        0     2766 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/cleaners/headers.py
+-rw-r--r--   0        0        0     2456 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/cleaners/headings.py
+-rw-r--r--   0        0        0      248 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/cleaners/text.py
+-rw-r--r--   0        0        0     5172 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/convert.py
+-rw-r--r--   0        0        0     2450 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/debug/data.py
+-rw-r--r--   0        0        0     7884 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/equations/equations.py
+-rw-r--r--   0        0        0     1549 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/equations/inference.py
+-rw-r--r--   0        0        0     2594 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/images/extract.py
+-rw-r--r--   0        0        0      473 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/images/save.py
+-rw-r--r--   0        0        0     1928 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/layout/layout.py
+-rw-r--r--   0        0        0     2516 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/layout/order.py
+-rw-r--r--   0        0        0      396 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/logger.py
+-rw-r--r--   0        0        0     3121 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/models.py
+-rw-r--r--   0        0        0      888 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/ocr/detection.py
+-rw-r--r--   0        0        0     2468 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/ocr/heuristics.py
+-rw-r--r--   0        0        0     1223 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/ocr/lang.py
+-rw-r--r--   0        0        0     5742 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/ocr/recognition.py
+-rw-r--r--   0        0        0     2180 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/ocr/tesseract.py
+-rw-r--r--   0        0        0      258 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/ocr/utils.py
+-rw-r--r--   0        0        0     1266 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/output.py
+-rw-r--r--   0        0        0     3932 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/pdf/extract_text.py
+-rw-r--r--   0        0        0      817 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/pdf/images.py
+-rw-r--r--   0        0        0     2442 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/pdf/utils.py
+-rw-r--r--   0        0        0     4134 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/postprocessors/editor.py
+-rw-r--r--   0        0        0     7226 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/postprocessors/markdown.py
+-rw-r--r--   0        0        0     4977 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/postprocessors/t5.py
+-rw-r--r--   0        0        0     2849 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/schema/bbox.py
+-rw-r--r--   0        0        0     3259 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/schema/block.py
+-rw-r--r--   0        0        0      502 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/schema/merged.py
+-rw-r--r--   0        0        0     1618 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/schema/page.py
+-rw-r--r--   0        0        0     4238 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/settings.py
+-rw-r--r--   0        0        0     3384 2024-05-16 22:46:38.279132 marker_pdf-0.2.6/marker/tables/cells.py
+-rw-r--r--   0        0        0     7178 2024-05-16 22:46:38.283131 marker_pdf-0.2.6/marker/tables/table.py
+-rw-r--r--   0        0        0     1128 2024-05-16 22:46:38.283131 marker_pdf-0.2.6/marker/tables/utils.py
+-rw-r--r--   0        0        0      156 2024-05-16 22:46:38.283131 marker_pdf-0.2.6/marker/utils.py
+-rw-r--r--   0        0        0     1338 2024-05-16 22:46:38.283131 marker_pdf-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0    14231 1970-01-01 00:00:00.000000 marker_pdf-0.2.6/PKG-INFO
```

### Comparing `marker_pdf-0.2.5/LICENSE` & `marker_pdf-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/README.md` & `marker_pdf-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/chunk_convert.py` & `marker_pdf-0.2.6/chunk_convert.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/chunk_convert.sh` & `marker_pdf-0.2.6/chunk_convert.sh`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/convert.py` & `marker_pdf-0.2.6/convert.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/convert_single.py` & `marker_pdf-0.2.6/convert_single.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/benchmark/scoring.py` & `marker_pdf-0.2.6/marker/benchmark/scoring.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/cleaners/code.py` & `marker_pdf-0.2.6/marker/cleaners/code.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/cleaners/fontstyle.py` & `marker_pdf-0.2.6/marker/cleaners/fontstyle.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/cleaners/headers.py` & `marker_pdf-0.2.6/marker/cleaners/headers.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/cleaners/headings.py` & `marker_pdf-0.2.6/marker/cleaners/headings.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/convert.py` & `marker_pdf-0.2.6/marker/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     # Setup output metadata
     out_meta = {
         "languages": langs,
         "filetype": filetype,
     }
 
     if filetype == "other": # We can't process this file
-        return "", out_meta
+        return "", {}, out_meta
 
     # Get initial text blocks from the pdf
     doc = pdfium.PdfDocument(fname)
     pages, toc = get_text_blocks(
         doc,
         max_pages=max_pages,
     )
@@ -81,15 +81,15 @@
     # OCR pages as needed
     pages, ocr_stats = run_ocr(doc, pages, langs, ocr_model, batch_multiplier=batch_multiplier)
     flush_cuda_memory()
 
     out_meta["ocr_stats"] = ocr_stats
     if len([b for p in pages for b in p.blocks]) == 0:
         print(f"Could not extract any text blocks for {fname}")
-        return "", out_meta
+        return "", {}, out_meta
 
     surya_layout(doc, pages, layout_model, batch_multiplier=batch_multiplier)
     flush_cuda_memory()
 
     # Find headers and footers
     bad_span_ids = filter_header_footer(pages)
     out_meta["block_stats"] = {"header_footer": len(bad_span_ids)}
```

### Comparing `marker_pdf-0.2.5/marker/debug/data.py` & `marker_pdf-0.2.6/marker/debug/data.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/equations/equations.py` & `marker_pdf-0.2.6/marker/equations/equations.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/equations/inference.py` & `marker_pdf-0.2.6/marker/equations/inference.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/images/extract.py` & `marker_pdf-0.2.6/marker/images/extract.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/layout/layout.py` & `marker_pdf-0.2.6/marker/layout/layout.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/layout/order.py` & `marker_pdf-0.2.6/marker/layout/order.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/models.py` & `marker_pdf-0.2.6/marker/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,54 +5,73 @@
 from marker.settings import settings
 from surya.model.recognition.model import load_model as load_recognition_model
 from surya.model.recognition.processor import load_processor as load_recognition_processor
 from surya.model.ordering.model import load_model as load_order_model
 from surya.model.ordering.processor import load_processor as load_order_processor
 
 
-def setup_recognition_model(langs):
-    rec_model = load_recognition_model(langs=langs)
+def setup_recognition_model(langs, device=None, dtype=None):
+    if device:
+        rec_model = load_recognition_model(langs=langs, device=device, dtype=dtype)
+    else:
+        rec_model = load_recognition_model(langs=langs)
     rec_processor = load_recognition_processor()
     rec_model.processor = rec_processor
     return rec_model
 
 
-def setup_detection_model():
-    model = segformer.load_model()
+def setup_detection_model(device=None, dtype=None):
+    if device:
+        model = segformer.load_model(device=device, dtype=dtype)
+    else:
+        model = segformer.load_model()
+
     processor = segformer.load_processor()
     model.processor = processor
     return model
 
 
-def setup_texify_model():
-    texify_model = load_texify_model(checkpoint=settings.TEXIFY_MODEL_NAME, device=settings.TORCH_DEVICE_MODEL, dtype=settings.TEXIFY_DTYPE)
+def setup_texify_model(device=None, dtype=None):
+    if device:
+        texify_model = load_texify_model(checkpoint=settings.TEXIFY_MODEL_NAME, device=device, dtype=dtype)
+    else:
+        texify_model = load_texify_model(checkpoint=settings.TEXIFY_MODEL_NAME, device=settings.TORCH_DEVICE_MODEL, dtype=settings.TEXIFY_DTYPE)
     texify_processor = load_texify_processor()
     texify_model.processor = texify_processor
     return texify_model
 
 
-def setup_layout_model():
-    model = segformer.load_model(checkpoint=settings.LAYOUT_MODEL_CHECKPOINT)
+def setup_layout_model(device=None, dtype=None):
+    if device:
+        model = segformer.load_model(checkpoint=settings.LAYOUT_MODEL_CHECKPOINT, device=device, dtype=dtype)
+    else:
+        model = segformer.load_model(checkpoint=settings.LAYOUT_MODEL_CHECKPOINT)
     processor = segformer.load_processor(checkpoint=settings.LAYOUT_MODEL_CHECKPOINT)
     model.processor = processor
     return model
 
 
-def setup_order_model():
-    model = load_order_model()
+def setup_order_model(device=None, dtype=None):
+    if device:
+        model = load_order_model(device=device, dtype=dtype)
+    else:
+        model = load_order_model()
     processor = load_order_processor()
     model.processor = processor
     return model
 
 
-def load_all_models(langs=None):
+def load_all_models(langs=None, device=None, dtype=None, force_load_ocr=False):
+    if device is not None:
+        assert dtype is not None, "Must provide dtype if device is provided"
+
     # langs is optional list of languages to prune from recognition MoE model
-    detection = setup_detection_model()
-    layout = setup_layout_model()
-    order = setup_order_model()
-    edit = load_editing_model()
+    detection = setup_detection_model(device, dtype)
+    layout = setup_layout_model(device, dtype)
+    order = setup_order_model(device, dtype)
+    edit = load_editing_model(device, dtype)
 
     # Only load recognition model if we'll need it for all pdfs
-    ocr = setup_recognition_model(langs) if (settings.OCR_ENGINE == "surya" and settings.OCR_ALL_PAGES) else None
-    texify = setup_texify_model()
+    ocr = setup_recognition_model(langs, device, dtype) if ((settings.OCR_ENGINE == "surya" and settings.OCR_ALL_PAGES) or force_load_ocr) else None
+    texify = setup_texify_model(device, dtype)
     model_lst = [texify, layout, order, edit, detection, ocr]
     return model_lst
```

### Comparing `marker_pdf-0.2.5/marker/ocr/detection.py` & `marker_pdf-0.2.6/marker/ocr/detection.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/ocr/heuristics.py` & `marker_pdf-0.2.6/marker/ocr/heuristics.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/ocr/lang.py` & `marker_pdf-0.2.6/marker/ocr/lang.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/ocr/recognition.py` & `marker_pdf-0.2.6/marker/ocr/recognition.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/ocr/tesseract.py` & `marker_pdf-0.2.6/marker/ocr/tesseract.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/output.py` & `marker_pdf-0.2.6/marker/output.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/pdf/extract_text.py` & `marker_pdf-0.2.6/marker/pdf/extract_text.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/pdf/images.py` & `marker_pdf-0.2.6/marker/pdf/images.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/pdf/utils.py` & `marker_pdf-0.2.6/marker/pdf/utils.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/postprocessors/editor.py` & `marker_pdf-0.2.6/marker/postprocessors/editor.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,22 +12,29 @@
     if settings.EDITOR_BATCH_SIZE is not None:
         return settings.EDITOR_BATCH_SIZE
     elif settings.TORCH_DEVICE_MODEL == "cuda":
         return 12
     return 6
 
 
-def load_editing_model():
+def load_editing_model(device=None, dtype=None):
     if not settings.ENABLE_EDITOR_MODEL:
         return None
 
-    model = T5ForTokenClassification.from_pretrained(
+    if device:
+        model = T5ForTokenClassification.from_pretrained(
             settings.EDITOR_MODEL_NAME,
-            torch_dtype=settings.MODEL_DTYPE,
-        ).to(settings.TORCH_DEVICE_MODEL)
+            torch_dtype=dtype,
+            device=device,
+        )
+    else:
+        model = T5ForTokenClassification.from_pretrained(
+                settings.EDITOR_MODEL_NAME,
+                torch_dtype=settings.MODEL_DTYPE,
+            ).to(settings.TORCH_DEVICE_MODEL)
     model.eval()
 
     model.config.label2id = {
         "equal": 0,
         "delete": 1,
         "newline-1": 2,
         "space-1": 3,
```

### Comparing `marker_pdf-0.2.5/marker/postprocessors/markdown.py` & `marker_pdf-0.2.6/marker/postprocessors/markdown.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/postprocessors/t5.py` & `marker_pdf-0.2.6/marker/postprocessors/t5.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/schema/bbox.py` & `marker_pdf-0.2.6/marker/schema/bbox.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/schema/block.py` & `marker_pdf-0.2.6/marker/schema/block.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/schema/page.py` & `marker_pdf-0.2.6/marker/schema/page.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/settings.py` & `marker_pdf-0.2.6/marker/settings.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/tables/cells.py` & `marker_pdf-0.2.6/marker/tables/cells.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/tables/table.py` & `marker_pdf-0.2.6/marker/tables/table.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/marker/tables/utils.py` & `marker_pdf-0.2.6/marker/tables/utils.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.5/pyproject.toml` & `marker_pdf-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "marker-pdf"
-version = "0.2.5"
+version = "0.2.6"
 description = "Convert PDF to markdown with high speed and accuracy."
 authors = ["Vik Paruchuri <github@vikas.sh>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 repository = "https://github.com/VikParuchuri/marker"
 keywords = ["pdf", "markdown", "ocr", "nlp"]
 packages = [
```

### Comparing `marker_pdf-0.2.5/PKG-INFO` & `marker_pdf-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marker-pdf
-Version: 0.2.5
+Version: 0.2.6
 Summary: Convert PDF to markdown with high speed and accuracy.
 Home-page: https://github.com/VikParuchuri/marker
 License: GPL-3.0-or-later
 Keywords: pdf,markdown,ocr,nlp
 Author: Vik Paruchuri
 Author-email: github@vikas.sh
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
```

