# Comparing `tmp/phenopype_plugins-0.1.1.tar.gz` & `tmp/phenopype_plugins-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phenopype_plugins-0.1.1.tar", last modified: Mon Apr 15 18:18:27 2024, max compression
+gzip compressed data, was "phenopype_plugins-0.1.2.tar", last modified: Thu May 16 15:52:10 2024, max compression
```

## Comparing `phenopype_plugins-0.1.1.tar` & `phenopype_plugins-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 18:18:27.572697 phenopype_plugins-0.1.1/
--rw-rw-rw-   0        0        0     7815 2022-04-25 22:33:40.000000 phenopype_plugins-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      558 2024-04-15 18:18:27.572697 phenopype_plugins-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      120 2024-04-15 04:19:07.000000 phenopype_plugins-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 18:18:27.541051 phenopype_plugins-0.1.1/phenopype_plugins/
--rw-rw-rw-   0        0        0      191 2024-04-15 04:10:50.000000 phenopype_plugins-0.1.1/phenopype_plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:18:27.557065 phenopype_plugins-0.1.1/phenopype_plugins/plugins/
--rw-rw-rw-   0        0        0     3579 2024-04-14 22:05:58.000000 phenopype_plugins-0.1.1/phenopype_plugins/plugins/measurement.py
--rw-rw-rw-   0        0        0    14595 2024-04-15 04:07:33.000000 phenopype_plugins-0.1.1/phenopype_plugins/plugins/segmentation.py
--rw-rw-rw-   0        0        0     1156 2024-04-15 00:38:38.000000 phenopype_plugins-0.1.1/phenopype_plugins/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:18:27.572697 phenopype_plugins-0.1.1/phenopype_plugins.egg-info/
--rw-rw-rw-   0        0        0      558 2024-04-15 18:18:27.000000 phenopype_plugins-0.1.1/phenopype_plugins.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2024-04-15 18:18:27.000000 phenopype_plugins-0.1.1/phenopype_plugins.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 18:18:27.000000 phenopype_plugins-0.1.1/phenopype_plugins.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-15 18:18:27.000000 phenopype_plugins-0.1.1/phenopype_plugins.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-04-15 18:18:27.000000 phenopype_plugins-0.1.1/phenopype_plugins.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      581 2024-04-15 18:17:21.000000 phenopype_plugins-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 18:18:27.572697 phenopype_plugins-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-16 15:52:10.428912 phenopype_plugins-0.1.2/
+-rw-rw-rw-   0        0        0     7815 2022-04-25 22:33:40.000000 phenopype_plugins-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1942 2024-05-16 15:52:10.427932 phenopype_plugins-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1504 2024-05-09 19:59:50.000000 phenopype_plugins-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 15:52:10.406863 phenopype_plugins-0.1.2/phenopype_plugins/
+-rw-rw-rw-   0        0        0      256 2024-05-09 22:07:56.000000 phenopype_plugins-0.1.2/phenopype_plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:52:10.425910 phenopype_plugins-0.1.2/phenopype_plugins/plugins/
+-rw-rw-rw-   0        0        0     3491 2024-05-16 15:47:13.000000 phenopype_plugins-0.1.2/phenopype_plugins/plugins/measurement.py
+-rw-rw-rw-   0        0        0    16665 2024-05-16 15:45:49.000000 phenopype_plugins-0.1.2/phenopype_plugins/plugins/segmentation.py
+-rw-rw-rw-   0        0        0     5503 2024-05-16 15:45:19.000000 phenopype_plugins-0.1.2/phenopype_plugins/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:52:10.427932 phenopype_plugins-0.1.2/phenopype_plugins.egg-info/
+-rw-rw-rw-   0        0        0     1942 2024-05-16 15:52:10.000000 phenopype_plugins-0.1.2/phenopype_plugins.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2024-05-16 15:52:10.000000 phenopype_plugins-0.1.2/phenopype_plugins.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 15:52:10.000000 phenopype_plugins-0.1.2/phenopype_plugins.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-16 15:52:10.000000 phenopype_plugins-0.1.2/phenopype_plugins.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-16 15:52:10.000000 phenopype_plugins-0.1.2/phenopype_plugins.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      581 2024-05-16 15:39:37.000000 phenopype_plugins-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 15:52:10.428912 phenopype_plugins-0.1.2/setup.cfg
```

### Comparing `phenopype_plugins-0.1.1/LICENSE` & `phenopype_plugins-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `phenopype_plugins-0.1.1/phenopype_plugins/plugins/measurement.py` & `phenopype_plugins-0.1.2/phenopype_plugins/plugins/measurement.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,19 +6,18 @@
 import cv2
 import math
 import numpy as np
 import os
 import sys
 
 from phenopype import __version__
-from phenopype import _config
-# from phenopype import plugins
-from phenopype import settings
+from phenopype import _vars
+from phenopype import config
 from phenopype import utils
-from phenopype import utils_lowlevel
+from phenopype import utils_lowlevel as ul
 
 #%% namespace cleanup
 
 funs = ['detect_landmark']
 
 def __dir__():
     return clean_namespace + funs
@@ -61,18 +60,18 @@
 
     # =============================================================================
     # annotation management
 
     fun_name = sys._getframe().f_code.co_name
     
     annotations = kwargs.get("annotations", {})
-    annotation_type = utils_lowlevel._get_annotation_type(fun_name)
+    annotation_type = ul._get_annotation_type(fun_name)
     annotation_id = kwargs.get("annotation_id", None)
 
-    annotation = utils_lowlevel._get_annotation(
+    annotation = ul._get_annotation(
         annotations=annotations,
         annotation_type=annotation_type,
         annotation_id=annotation_id,
         kwargs=kwargs,
     )
     
         
@@ -82,23 +81,23 @@
     landmark_tuple_list = []
         
     if mask:        
         if not annotations:
             print("- no mask coordinates provided - cannot detect within mask")
             pass
         else:
-            annotation_id_mask = kwargs.get(settings._mask_type + "_id", None)
-            annotation_mask = utils_lowlevel._get_annotation(
+            annotation_id_mask = kwargs.get(_vars._mask_type + "_id", None)
+            annotation_mask = ul._get_annotation(
                 annotations,
-                settings._mask_type,
+                _vars._mask_type,
                 annotation_id_mask,
                 prep_msg="- masking regions in thresholded image:",
             )
             
-            bbox_coords = cv2.boundingRect(np.asarray(annotation_mask["data"][settings._mask_type], dtype="int32"))
+            bbox_coords = cv2.boundingRect(np.asarray(annotation_mask["data"][_vars._mask_type], dtype="int32"))
     else:
         bbox_coords = None
         
     landmark_tuple_list = plugins.libraries.phenomorph.main.predict_image(
         img=image, model_path=model_path, bbox_coords=bbox_coords, plot=False)
 
     print("- found {} points".format(len(landmark_tuple_list)))
@@ -113,15 +112,15 @@
         },
         "data": {
             annotation_type: landmark_tuple_list
             },
     }
 
 
-    return utils_lowlevel._update_annotations(
+    return ul._update_annotations(
         annotations=annotations,
         annotation=annotation,
         annotation_type=annotation_type,
         annotation_id=annotation_id,
         kwargs=kwargs,
     )
```

### Comparing `phenopype_plugins-0.1.1/phenopype_plugins/plugins/segmentation.py` & `phenopype_plugins-0.1.2/phenopype_plugins/plugins/segmentation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,126 +1,156 @@
 #%% modules
 
 import copy
 import cv2
 import numpy as np
 import sys
-
+from rich.pretty import pretty_repr
 from dataclasses import make_dataclass
+import time
 
-from phenopype import _config
-from phenopype import settings
-from phenopype import utils_lowlevel
+from phenopype import _vars
+from phenopype import utils as pp_utils
+from phenopype import utils_lowlevel as pp_ul
 from phenopype.core import segmentation, visualization
-from phenopype import utils_lowlevel as ul
 
-from phenopype_plugins.utils import parse_model_config
+from phenopype_plugins import utils
+
+import warnings
 
 try:
     import torch
 except ImportError:
-    pass
+    warnings.warn("Failed to import PyTorch. Some functionalities may not work.", ImportWarning)
 
 try:
     import keras
 except ImportError:
-    pass
+    warnings.warn("Failed to import Keras. Some functionalities may not work.", ImportWarning)
 
 try:
-    import fastsam
+    from ultralytics import FastSAM, engine
+    from ultralytics.models.fastsam import FastSAMPrompt
 except ImportError:
-    pass
+    warnings.warn("Failed to import Ultralytics. Some functionalities may not work.", ImportWarning)
+
+
 
 #%% functions
  
- 
-def predict_contour_fastSAM(
+@utils.model_path_resolver
+def predict_fastSAM(
         image,
+        model_path,
         model_id="a",
         prompt="everything",
-        center=0.9,
+        trim=0.05,
         resize_roi=1024,
         confidence=0.8,
         iou=0.65,
-        force_reload=False,
         **kwargs,
         ):
     
+    """
+    Process an input image using the FastSAM model to detect and segment objects based on specified prompts.
+
+    This function handles model loading (with caching capabilities), image preprocessing according to the prompt type,
+    object detection, and segmentation, and returns an image with detections applied.
+
+    Parameters
+    ----------
+    image : ndarray
+        The input image to process.
+    model_id : str, optional
+        Identifier for the model configuration to use, defaults to 'a'.
+    prompt : str, optional
+        Type of detection and segmentation to perform. Options include 'everything', 'text', 'everything-box', or 'box', defaults to 'everything'.
+    center : float, optional
+        Fraction of the image center to consider for processing, relevant only for certain prompts, defaults to 0.9.
+    resize_roi : int, optional
+        The size to which regions of interest (ROIs) are resized before processing, defaults to 1024.
+    confidence : float, optional
+        Confidence threshold for the detection to consider a detection valid, defaults to 0.8.
+    iou : float, optional
+        Intersection over Union (IoU) threshold for determining object uniqueness, defaults to 0.65.
+    **kwargs
+        Additional keyword arguments for extended functionality, like 'max_dim' or specific annotations.
+
+    Returns
+    -------
+    ndarray
+        The processed image with detections and segmentations applied as specified by the prompt.
+
+    Examples
+    --------
+    >>> processed_image = predict_fastSAM(input_image, model_id='b', prompt='box', resize_roi=512)
+        Process 'input_image' using model configuration 'b', focusing on bounding box detections, resizing the ROI to 512x512 pixels.
+    """
+    
     # =============================================================================
     # setup
         
     ## set flags
     flags = make_dataclass(
         cls_name="flags",
-        fields=[("prompt", str, prompt), 
-                ("max_dim", str, kwargs.get("max_dim")), 
-                ],
-    )
+        fields=[
+            ("prompt", str, prompt), 
+             ])
     
     # =============================================================================
     # model management
     
-    # Check if model_id is not None and exists in the configuration
-    if model_id in _config.models:
-        model_path = _config.models[model_id]["model_path"]
-        
-    # Check if the model hasn't been loaded yet
-    if "model" not in _config.models[model_id]:
-        print(f"- loading model  \"{model_id}\" into memory")
-        _config.models[model_id]["model"] = fastsam.FastSAM(model_path)
-    else:
-        print(f"- using cached model \"{model_id}\"")
-    _config.active_model = _config.models[model_id]["model"]
-
-    # init model and device
+    # Load or retrieve the cached model
+    model = utils.model_loader_cacher(model_id, FastSAM, model_path)
+    
+    ## set device
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-    model = _config.active_model
-                            
+
     # =============================================================================
     # prepare image
     
-    if flags.prompt == "everything":
-        if center < 1:
+    if flags.prompt in ["everything", "text"]:
+        if trim > 0:
             height, width = image.shape[:2]
-            rx, ry = int(round((1 - center) * 0.5 * width)), int(round((1 - center) * 0.5 * height))
-            rh, rw = int(round(center * height)), int(round(center * width))
+            rx, ry = int(round(trim * 0.5 * width)), int(round(trim * 0.5 * width))
+            rh, rw = int(round((1 - trim) * height)), int(round((1 - trim) * width))
             roi_orig = image[ry : ry + rh, rx : rx + rw]
         else:
             roi_orig = copy.deepcopy(image)
 
     elif flags.prompt in ["everything-box", "box"]:
         ## get mask from annotations
         annotations = kwargs.get("annotations", {})
-        annotation_id_mask = kwargs.get(settings._mask_type + "_id", None)
-        annotation_mask = utils_lowlevel._get_annotation(
+        annotation_id_mask = kwargs.get(_vars._mask_type + "_id", None)
+        annotation_mask = pp_ul._get_annotation(
             annotations,
-            settings._mask_type,
+            _vars._mask_type,
             annotation_id_mask,
         )
         ## convert mask coords to ROI
         coords = annotation_mask["data"]["mask"]
-        coords = utils_lowlevel._convert_tup_list_arr(coords)
+        coords = pp_ul._convert_tup_list_arr(coords)
         rx, ry, rw, rh = cv2.boundingRect(coords[0])  
         
         if flags.prompt == "everything-box":
             roi_orig = image[ry : ry + rh, rx : rx + rw]
         elif flags.prompt == "box":
             roi_orig = image
             resize_x = resize_roi / roi_orig.shape[1]
-            resize_y = resize_roi / roi_orig.shape[0]
+            resize_y = resize_roi / roi_orig.shape[0]       
         
     ## resize roi
     roi_orig_height, roi_orig_width = roi_orig.shape[:2]
-    roi = utils_lowlevel._resize_image(
+    roi = pp_utils.resize_image(
         roi_orig, width=resize_roi, height=resize_roi)
-    
+        
     # =============================================================================
     # apply model
     
-    print(f"- starting prompt on device {device}")
+    print(f"- starting {flags.prompt} prompt on device {device}")
         
     ## encode roi 
     everything_results = model(
         roi,
         device=device,
         retina_masks=True,
         imgsz=[int(roi.shape[1]), int(roi.shape[0])],
@@ -133,80 +163,82 @@
         speed = everything_results[0].speed
         speed = {
             "preprocess": round(speed["preprocess"], 2),
             "inference": round(speed["inference"], 2),
             "postprocess": round(speed["postprocess"], 2),
             }
         print(f"- sucessfully processed image of shape {everything_results[0].orig_shape}")
-        print(f"- speed: {speed}")
+        print(f"- speed: {pretty_repr(speed)}")
 
     else:
         return image
 
     # =============================================================================
     ## set up prompt
-    
-    prompt_process = fastsam.FastSAMPrompt(
+        
+    prompt_process = FastSAMPrompt(
         roi, everything_results, device=device)
     
     # =============================================================================
     ## get detected objects
     
     ## box-post
     if flags.prompt == "box":      
-        mask_coords = ul._resize_mask([rx, ry, rw, rh], resize_x, resize_y)
-        mask_coords_sam = utils_lowlevel._convert_box_xywh_to_xyxy(mask_coords)
-        detections = prompt_process.box_prompt(bboxes=[mask_coords_sam])
+        mask_coords = pp_ul._resize_mask([rx, ry, rw, rh], resize_x, resize_y)
+        mask_coords_sam = pp_ul._convert_box_xywh_to_xyxy(mask_coords)
+        detections = prompt_process.box_prompt(bbox=mask_coords_sam)
     
     ## everything prompt 
     elif flags.prompt in ["everything","everything-box"]:
         detections = prompt_process.everything_prompt()
+
+    elif flags.prompt == "text":
+        detections = prompt_process.text_prompt(text=kwargs.get("text",""))
         
-    ## tensor to array
-    if detections.__class__.__name__ == "Tensor":    
-        detections_array = np.asarray(detections.cpu(), "uint8")
-    else: 
-        detections_array = np.asarray(detections, "uint8")
-        
-    ## create binary mask
-    roi_bin = np.bitwise_or.reduce(detections_array, axis=0)
-    roi_bin[roi_bin==1] = 255
-        
+    ## ultralytics.results to array
+    if type(detections[0]) == engine.results.Results:
+        results = detections[0].cpu()
+        roi_bin = np.array(results.masks[0].data[0], dtype=np.uint8)
+        for mask in results.masks[1:]:
+            roi_bin |= np.array(mask.data[0], dtype=np.uint8)
+        roi_bin[roi_bin==1] = 255
+
     ## resize to original dimensions
-    roi_det = utils_lowlevel._resize_image(
+    roi_det = pp_utils.resize_image(
         roi_bin, width=roi_orig_width, height=roi_orig_height)
     
-    if flags.prompt in ["everything", "everything-box"]:
-        if center == 1 and flags.prompt == "everything":
+    if flags.prompt in ["everything", "everything-box", "text"]:
+        if trim == 0 and flags.prompt in ["everything", "text"]:
             image_bin = roi_det
         else:
             image_bin = np.zeros(image.shape[:2], "uint8")
             image_bin[ry : ry + rh, rx : rx + rw] = roi_det
         
-    elif flags.prompt == "box":
+    elif flags.prompt in ["box"]:
         image_bin = roi_det
             
         
     return image_bin
 
-
-def predict_contour_keras(
+@utils.model_path_resolver
+def predict_keras(
     image,
+    model_path,
     model_id="a",
     binary_mask=False,
     threshold=True,
     threshold_method="otsu",
     threshold_value=127,
     threshold_blocksize=99,
     threshold_constant=5,
     force_reload=False,
     **kwargs,
 ):
     """
-    Applies a trained deep learning model to an image and returns a grayscale mask 
+    Applies a pre-trained deep learning model to an image and returns a grayscale mask 
     of foreground predictions, which can then be thresholded to return a binary mask.
     
     Three types of thresholding algorithms are supported: 
         - otsu: use Otsu algorithm to choose the optimal threshold value
         - adaptive: dynamic threshold values across image (uses arguments
           "blocksize" and "constant")
         - binary: fixed threshold value (uses argument "value")    
@@ -247,155 +279,171 @@
     
     fun_name = sys._getframe().f_code.co_name
     
     ## flags
     flags = make_dataclass(cls_name="flags", 
                            fields=[("binary_mask", bool, binary_mask)])
     
+
+        
     # =============================================================================
-    # annotation management
-    if flags.binary_mask:
+    # model management
+    
+    # Load or retrieve the cached model
+    model = utils.model_loader_cacher(model_id, keras.models.load_model, model_path)
         
-        annotations = kwargs.get("annotations", {})
-        annotation_type = kwargs.get("annotation_type", settings._mask_type)
-        annotation_id = kwargs.get(annotation_type + "_id", None)
+    ## set device
+    device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
             
     # =============================================================================
-    # execute
     
     image_source = copy.deepcopy(image)
-    
+
+    ## apply binary mask from annotations to image
     if flags.binary_mask:
+        
+        annotations = kwargs.get("annotations", {})
+        annotation_type = kwargs.get("annotation_type", _vars._mask_type)
+        annotation_id = kwargs.get(annotation_type + "_id", None)
+
         binary_mask = np.zeros(image_source.shape, dtype="uint8")
-        if annotation_type == settings._mask_type:
+        if annotation_type == _vars._mask_type:
             print("mask")
             binary_mask = visualization.draw_mask(
                 image=binary_mask, 
                 annotations=annotations, 
                 contour_id=annotation_id, 
                 line_colour=255,
                 line_width=0,
                 fill=1)
-        elif annotation_type == settings._contour_type:
+        elif annotation_type == _vars._contour_type:
             print("contour")
             binary_mask = visualization.draw_contour(
                 image=binary_mask, 
                 annotations=annotations, 
                 contour_id=annotation_id, 
                 line_colour=255,
                 line_width=0,
                 fill=1)
 
         image_source = cv2.bitwise_and(image_source, binary_mask)    
-    if not model_id.__class__.__name__ == "NoneType":
-        model_path = _config.models[model_id]["model_phenopype_path"]
-        if not "model_loaded" in _config.models[model_id]:
-            print("loading model " + model_id)
-            _config.models[model_id]["model_loaded"] = keras.models.load_model(model_path)
-        _config.active_model = _config.models[model_id]["model_loaded"]
-        _config.active_model_path = model_path
-    
-    elif not _config.active_model_path == model_path or _config.active_model.__class__.__name__ == "NoneType" or force_reload==True:
-        _config.active_model = keras.models.load_model(model_path)
-        _config.active_model_path = model_path
 
-    print("Using current model at " + _config.active_model_path)
-    
-    model = _config.active_model
+    # =============================================================================
+    ## inference
 
-    image_source = utils_lowlevel._resize_image(image_source, width=model.input.shape[1], height=model.input.shape[2])/255
+    image_source = pp_utils.resize_image(image_source, width=model.input.shape[1], height=model.input.shape[2])/255
     image_source = np.expand_dims(image_source, axis=0)
+    
     pred = model.predict(image_source)
      
     mask_predicted = pred[0,:,:,1]*255
     mask_predicted = mask_predicted.astype(np.uint8)
-    mask_predicted = utils_lowlevel._resize_image(mask_predicted, width=image.shape[1], height=image.shape[0], interpolation="linear")
+    mask_predicted = pp_utils.resize_image(mask_predicted, width=image.shape[1], height=image.shape[0], interpolation="linear")
     
     if threshold:
         mask_predicted = segmentation.threshold(
             mask_predicted, 
             invert=True,
             method=threshold_method,
             value=threshold_value, 
             blocksize=threshold_blocksize,
             constant=threshold_constant
             )
-           
 
     # tf.keras.backend.clear_session()
     
     return mask_predicted
 
-
-def predict_contour_torch(
+@utils.model_path_resolver
+@utils.model_config_path_resolver
+def predict_torch(
         image,
+        model_path,
+        model_config_path,
         model_id="a",
-        model_config_path=None,
         primer="contour",
         confidence=0.8,
         **kwargs,
         ):
-    
-    # =============================================================================
-    # setup
+    """
+    Perform image segmentation prediction using a pre-trained PyTorch model. This function handles
+    model loading, preprocessing, and prediction, returning a binary mask of the segmented area
+    based on the specified 'primer' type.
 
+    Parameters:
+    ----------
+    image : ndarray
+        The input image array on which segmentation prediction is performed.
+    model_path : str
+        The path to the trained model file.
+    model_config_path : str
+        The path to the model's configuration file.
+    model_id : str, optional
+        Identifier for the model, used to cache or differentiate between models. Default is 'a'.
+    primer : str, optional
+        Type of annotation to use for determining region of interest (ROI) in the image. Supported
+        types are 'contour' and 'mask'. Default is 'contour'.
+    confidence : float, optional
+        Confidence threshold for converting model output to a binary mask. Default is 0.8.
+    **kwargs : dict
+        Additional keyword arguments which may include 'annotations' to specify existing 
+        annotations for refining predictions or other custom parameters.
+
+    Returns:
+    -------
+    ndarray
+        A binary mask image of the segmented region, where the segmentation is based on the 
+        primer type and specified region of interest within the image.
+
+    Examples:
+    --------
+    >>> image = pp.load_image('path/to/image.jpg')
+    >>> mask = pp.plugins.predict_torch(image, 'path/to/model.pth', 'path/to/model_config.py', primer="mask", confidence=0.9)
+    >>> pp.show_image(mask)
+    """
+    
     # =============================================================================
     # model management
-    
-    ## supply script with model specification 
-    if model_config_path:
-        fun_load_model, fun_preprocess = parse_model_config(model_config_path)
-        _config.models[model_id]["fun_preprocess"] = fun_preprocess
-        _config.models[model_id]["fun_load_model"] = fun_load_model
-    
-    # Check if model_id is not None and exists in the configuration
-    if model_id in _config.models:
-        preprocess = _config.models[model_id]["fun_preprocess"]
-        load_model = _config.models[model_id]["fun_load_model"]
-        model_path = _config.models[model_id]["model_path"]
-        
-    # Check if the model hasn't been loaded yet
-    if "model" not in _config.models[model_id]:
-        print(f"- loading model  \"{model_id}\" into memory")
-        _config.models[model_id]["model"] = load_model(model_path)
-    else:
-        print(f"- using cached model \"{model_id}\"")
-    _config.active_model = _config.models[model_id]["model"]
+        
+    ## load model config
+    model_config = utils.modularize_model_config('model_config', model_config_path)
+
+    # Load or retrieve the cached model
+    model = utils.model_loader_cacher(model_id, model_config.load_model, model_path)
 
-    # init model and device
+    ## set device
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-    model = _config.active_model
-    
+
     # =============================================================================
     ## annotation management
     
     annotations = kwargs.get("annotations", {})
     
     if primer=="contour":
-        annotation_id_input = kwargs.get(settings._contour_type + "_id", None)
-        annotation = utils_lowlevel._get_annotation(
+        annotation_id_input = kwargs.get(_vars._contour_type + "_id", None)
+        annotation = pp_ul._get_annotation(
             annotations,
-            settings._contour_type,
+            _vars._contour_type,
             annotation_id_input,
         )
-        coords = annotation["data"][settings._contour_type][0]
+        coords = annotation["data"][_vars._contour_type][0]
     elif primer=="mask":
-        annotation_id_input = kwargs.get(settings._mask_type + "_id", None)
-        annotation = utils_lowlevel._get_annotation(
+        annotation_id_input = kwargs.get(_vars._mask_type + "_id", None)
+        annotation = pp_ul._get_annotation(
             annotations,
-            settings._mask_type,
+            _vars._mask_type,
             annotation_id_input,
         )      
-        coords = annotation["data"][settings._mask_type][0]
+        coords = annotation["data"][_vars._mask_type][0]
         
     # =============================================================================
     ## inference
 
-    roi, roi_box = ul._extract_roi_center(image, coords, 512)
-    image_tensor = preprocess(roi)
+    roi, roi_box = pp_ul._extract_roi_center(image, coords, 512)
+    image_tensor = model_config.preprocess(roi)
     image_tensor = image_tensor.unsqueeze(0)
     image_tensor.to(device)
     
     predict_masks = model(image_tensor)
     
     mask = predict_masks[0].clone().cpu()
     mask = mask > confidence
```

### Comparing `phenopype_plugins-0.1.1/pyproject.toml` & `phenopype_plugins-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors = [
 	{name = "Moritz Lürig", email = "moritz.luerig@gmail.com"},
 	]
 description = "Plugins for phenopype"
 readme = "README.md"
 requires-python = "==3.9.*"
 keywords = ["computer vision", "biology"]
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
     "phenopype>=5.0",
 ]
 
 [project.urls]
 "Homepage" = "https://phenopype.org"
 "Bug Tracker" = "https://github.com/phenopype/phenopype-plugins/issues"
```

