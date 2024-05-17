# Comparing `tmp/odlabel-0.7.26.6.tar.gz` & `tmp/odlabel-0.7.26.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odlabel-0.7.26.6.tar", last modified: Fri May 17 08:35:42 2024, max compression
+gzip compressed data, was "odlabel-0.7.26.7.tar", last modified: Fri May 17 08:56:07 2024, max compression
```

## Comparing `odlabel-0.7.26.6.tar` & `odlabel-0.7.26.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:35:42.570520 odlabel-0.7.26.6/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     8653 2024-05-17 08:35:42.570520 odlabel-0.7.26.6/PKG-INFO
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:35:42.566521 odlabel-0.7.26.6/app/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       29 2024-05-17 04:49:36.000000 odlabel-0.7.26.6/app/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      296 2024-05-05 15:20:09.000000 odlabel-0.7.26.6/app/main.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    29684 2024-05-16 04:14:53.000000 odlabel-0.7.26.6/app/main_window.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:35:42.566521 odlabel-0.7.26.6/app/workers/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:08.000000 odlabel-0.7.26.6/app/workers/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     3152 2024-05-13 17:03:11.000000 odlabel-0.7.26.6/app/workers/chart_worker.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    14405 2024-05-16 09:39:28.000000 odlabel-0.7.26.6/app/workers/detection_worker.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:35:42.566521 odlabel-0.7.26.6/app/workers/utils/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:33.000000 odlabel-0.7.26.6/app/workers/utils/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    10448 2024-05-13 17:39:51.000000 odlabel-0.7.26.6/app/workers/utils/chart_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     6216 2024-05-10 15:15:58.000000 odlabel-0.7.26.6/app/workers/utils/detection_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     1911 2024-05-10 17:32:16.000000 odlabel-0.7.26.6/app/workers/utils/draw_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     4818 2024-05-05 12:54:55.000000 odlabel-0.7.26.6/app/workers/utils/write_utils.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:35:42.570520 odlabel-0.7.26.6/odlabel.egg-info/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     8653 2024-05-17 08:35:42.000000 odlabel-0.7.26.6/odlabel.egg-info/PKG-INFO
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      502 2024-05-17 08:35:42.000000 odlabel-0.7.26.6/odlabel.egg-info/SOURCES.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        1 2024-05-17 08:35:42.000000 odlabel-0.7.26.6/odlabel.egg-info/dependency_links.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       49 2024-05-17 08:35:42.000000 odlabel-0.7.26.6/odlabel.egg-info/entry_points.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       89 2024-05-17 08:35:42.000000 odlabel-0.7.26.6/odlabel.egg-info/requires.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        4 2024-05-17 08:35:42.000000 odlabel-0.7.26.6/odlabel.egg-info/top_level.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      275 2024-05-17 08:35:42.570520 odlabel-0.7.26.6/setup.cfg
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     1285 2024-05-17 08:34:31.000000 odlabel-0.7.26.6/setup.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:56:07.043775 odlabel-0.7.26.7/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     8708 2024-05-17 08:56:07.043775 odlabel-0.7.26.7/PKG-INFO
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:56:07.043775 odlabel-0.7.26.7/app/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       29 2024-05-17 04:49:36.000000 odlabel-0.7.26.7/app/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      296 2024-05-05 15:20:09.000000 odlabel-0.7.26.7/app/main.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    29684 2024-05-16 04:14:53.000000 odlabel-0.7.26.7/app/main_window.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:56:07.043775 odlabel-0.7.26.7/app/workers/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:08.000000 odlabel-0.7.26.7/app/workers/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     3152 2024-05-13 17:03:11.000000 odlabel-0.7.26.7/app/workers/chart_worker.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    14405 2024-05-16 09:39:28.000000 odlabel-0.7.26.7/app/workers/detection_worker.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:56:07.043775 odlabel-0.7.26.7/app/workers/utils/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:33.000000 odlabel-0.7.26.7/app/workers/utils/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    10448 2024-05-13 17:39:51.000000 odlabel-0.7.26.7/app/workers/utils/chart_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     6216 2024-05-10 15:15:58.000000 odlabel-0.7.26.7/app/workers/utils/detection_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     1911 2024-05-10 17:32:16.000000 odlabel-0.7.26.7/app/workers/utils/draw_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     4818 2024-05-05 12:54:55.000000 odlabel-0.7.26.7/app/workers/utils/write_utils.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:56:07.043775 odlabel-0.7.26.7/odlabel.egg-info/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     8708 2024-05-17 08:56:07.000000 odlabel-0.7.26.7/odlabel.egg-info/PKG-INFO
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      502 2024-05-17 08:56:07.000000 odlabel-0.7.26.7/odlabel.egg-info/SOURCES.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        1 2024-05-17 08:56:07.000000 odlabel-0.7.26.7/odlabel.egg-info/dependency_links.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       49 2024-05-17 08:56:07.000000 odlabel-0.7.26.7/odlabel.egg-info/entry_points.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       89 2024-05-17 08:56:07.000000 odlabel-0.7.26.7/odlabel.egg-info/requires.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        4 2024-05-17 08:56:07.000000 odlabel-0.7.26.7/odlabel.egg-info/top_level.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      275 2024-05-17 08:56:07.043775 odlabel-0.7.26.7/setup.cfg
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     1285 2024-05-17 08:53:06.000000 odlabel-0.7.26.7/setup.py
```

### Comparing `odlabel-0.7.26.6/PKG-INFO` & `odlabel-0.7.26.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odlabel
-Version: 0.7.26.6
+Version: 0.7.26.7
 Summary: A tool for object detection, labeling and visualization using PyTorch
 Home-page: https://github.com/Ziad-Algrafi/odlabel
 Author: Ziad-Algrafi
 Author-email: ZiadAlgrafi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -85,22 +85,22 @@
 | Model Type      | mAP  | mAP50 | mAP75 | Model                                                                                         |
 | --------------- | ---- | ----- | ----- | --------------------------------------------------------------------------------------------- |
 | yolov8s-worldv2 | 37.7 | 52.2  | 41.0  | [Download](https://github.com/ultralytics/assets/releases/download/v8.2.0/yolov8s-worldv2.pt) |
 | yolov8m-worldv2 | 43.0 | 58.4  | 46.8  | [Download](https://github.com/ultralytics/assets/releases/download/v8.2.0/yolov8m-worldv2.pt) |
 | yolov8l-worldv2 | 45.8 | 61.3  | 49.8  | [Download](https://github.com/ultralytics/assets/releases/download/v8.2.0/yolov8l-worldv2.pt) |
 | yolov8x-worldv2 | 47.1 | 62.8  | 51.4  | [Download](https://github.com/ultralytics/assets/releases/download/v8.2.0/yolov8x-worldv2.pt) |
 
-## ONNX Model
+## ONNX Models
 
-| Model Type      | mAP  | mAP50 | mAP75 | Model                                                                                     |
-| --------------- | ---- | ----- | ----- | ----------------------------------------------------------------------------------------- |
-| yolov8s-worldv2 | 37.7 | 52.2  | 41.0  | [Download](https://github.com/Ziad-Algrafi/ODLabel/blob/main/assets/yolov8s-worldv2.onnx) |
-| yolov8m-worldv2 | 43.0 | 58.4  | 46.8  | [Download](https://github.com/Ziad-Algrafi/ODLabel/blob/main/assets/yolov8m-worldv2.onnx) |
-| yolov8l-worldv2 | 45.8 | 61.3  | 49.8  | [Download](https://github.com/Ziad-Algrafi/ODLabel/blob/main/assets/yolov8l-worldv2.onnx) |
-| yolov8x-worldv2 | 47.1 | 62.8  | 51.4  | [Download](https://github.com/Ziad-Algrafi/ODLabel/blob/main/assets/yolov8x-worldv2.onnx) |
+| Model Type      | mAP  | mAP50 | mAP75 | Model                                                                                              |
+| --------------- | ---- | ----- | ----- | -------------------------------------------------------------------------------------------------- |
+| yolov8s-worldv2 | 37.7 | 52.2  | 41.0  | [Download](https://github.com/Ziad-Algrafi/ODLabel/raw/main/assets/yolov8s-worldv2.onnx?download=) |
+| yolov8m-worldv2 | 43.0 | 58.4  | 46.8  | [Download](https://github.com/Ziad-Algrafi/ODLabel/raw/main/assets/yolov8m-worldv2.onnx?download=) |
+| yolov8l-worldv2 | 45.8 | 61.3  | 49.8  | [Download](https://github.com/Ziad-Algrafi/ODLabel/raw/main/assets/yolov8l-worldv2.onnx?download=) |
+| yolov8x-worldv2 | 47.1 | 62.8  | 51.4  | [Download](https://github.com/Ziad-Algrafi/ODLabel/raw/main/assets/yolov8x-worldv2.onnx?download=) |
 
 ## GUI Figures and Dashboard
 
 ODLabel provides a comprehensive dashboard with various figures and visualizations to assist in analyzing the input image data and object detection results. The dashboard is displayed within the graphical user interface (GUI) of the application, allowing for interactive exploration and understanding of the data.
 
 The following figures are available in the dashboard:
```

### Comparing `odlabel-0.7.26.6/app/main_window.py` & `odlabel-0.7.26.7/app/main_window.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.6/app/workers/chart_worker.py` & `odlabel-0.7.26.7/app/workers/chart_worker.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.6/app/workers/detection_worker.py` & `odlabel-0.7.26.7/app/workers/detection_worker.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.6/app/workers/utils/chart_utils.py` & `odlabel-0.7.26.7/app/workers/utils/chart_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.6/app/workers/utils/detection_utils.py` & `odlabel-0.7.26.7/app/workers/utils/detection_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.6/app/workers/utils/draw_utils.py` & `odlabel-0.7.26.7/app/workers/utils/draw_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.6/app/workers/utils/write_utils.py` & `odlabel-0.7.26.7/app/workers/utils/write_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.6/odlabel.egg-info/PKG-INFO` & `odlabel-0.7.26.7/odlabel.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odlabel
-Version: 0.7.26.6
+Version: 0.7.26.7
 Summary: A tool for object detection, labeling and visualization using PyTorch
 Home-page: https://github.com/Ziad-Algrafi/odlabel
 Author: Ziad-Algrafi
 Author-email: ZiadAlgrafi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -85,22 +85,22 @@
 | Model Type      | mAP  | mAP50 | mAP75 | Model                                                                                         |
 | --------------- | ---- | ----- | ----- | --------------------------------------------------------------------------------------------- |
 | yolov8s-worldv2 | 37.7 | 52.2  | 41.0  | [Download](https://github.com/ultralytics/assets/releases/download/v8.2.0/yolov8s-worldv2.pt) |
 | yolov8m-worldv2 | 43.0 | 58.4  | 46.8  | [Download](https://github.com/ultralytics/assets/releases/download/v8.2.0/yolov8m-worldv2.pt) |
 | yolov8l-worldv2 | 45.8 | 61.3  | 49.8  | [Download](https://github.com/ultralytics/assets/releases/download/v8.2.0/yolov8l-worldv2.pt) |
 | yolov8x-worldv2 | 47.1 | 62.8  | 51.4  | [Download](https://github.com/ultralytics/assets/releases/download/v8.2.0/yolov8x-worldv2.pt) |
 
-## ONNX Model
+## ONNX Models
 
-| Model Type      | mAP  | mAP50 | mAP75 | Model                                                                                     |
-| --------------- | ---- | ----- | ----- | ----------------------------------------------------------------------------------------- |
-| yolov8s-worldv2 | 37.7 | 52.2  | 41.0  | [Download](https://github.com/Ziad-Algrafi/ODLabel/blob/main/assets/yolov8s-worldv2.onnx) |
-| yolov8m-worldv2 | 43.0 | 58.4  | 46.8  | [Download](https://github.com/Ziad-Algrafi/ODLabel/blob/main/assets/yolov8m-worldv2.onnx) |
-| yolov8l-worldv2 | 45.8 | 61.3  | 49.8  | [Download](https://github.com/Ziad-Algrafi/ODLabel/blob/main/assets/yolov8l-worldv2.onnx) |
-| yolov8x-worldv2 | 47.1 | 62.8  | 51.4  | [Download](https://github.com/Ziad-Algrafi/ODLabel/blob/main/assets/yolov8x-worldv2.onnx) |
+| Model Type      | mAP  | mAP50 | mAP75 | Model                                                                                              |
+| --------------- | ---- | ----- | ----- | -------------------------------------------------------------------------------------------------- |
+| yolov8s-worldv2 | 37.7 | 52.2  | 41.0  | [Download](https://github.com/Ziad-Algrafi/ODLabel/raw/main/assets/yolov8s-worldv2.onnx?download=) |
+| yolov8m-worldv2 | 43.0 | 58.4  | 46.8  | [Download](https://github.com/Ziad-Algrafi/ODLabel/raw/main/assets/yolov8m-worldv2.onnx?download=) |
+| yolov8l-worldv2 | 45.8 | 61.3  | 49.8  | [Download](https://github.com/Ziad-Algrafi/ODLabel/raw/main/assets/yolov8l-worldv2.onnx?download=) |
+| yolov8x-worldv2 | 47.1 | 62.8  | 51.4  | [Download](https://github.com/Ziad-Algrafi/ODLabel/raw/main/assets/yolov8x-worldv2.onnx?download=) |
 
 ## GUI Figures and Dashboard
 
 ODLabel provides a comprehensive dashboard with various figures and visualizations to assist in analyzing the input image data and object detection results. The dashboard is displayed within the graphical user interface (GUI) of the application, allowing for interactive exploration and understanding of the data.
 
 The following figures are available in the dashboard:
```

### Comparing `odlabel-0.7.26.6/setup.py` & `odlabel-0.7.26.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="odlabel",
-    version="0.7.26.6",
+    version="0.7.26.7",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "customtkinter",
         "ultralytics",
         "matplotlib",
         "numpy",
```

