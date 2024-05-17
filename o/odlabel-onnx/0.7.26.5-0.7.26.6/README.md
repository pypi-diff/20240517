# Comparing `tmp/odlabel-onnx-0.7.26.5.tar.gz` & `tmp/odlabel-onnx-0.7.26.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odlabel-onnx-0.7.26.5.tar", last modified: Fri May 17 06:50:42 2024, max compression
+gzip compressed data, was "odlabel-onnx-0.7.26.6.tar", last modified: Fri May 17 08:11:09 2024, max compression
```

## Comparing `odlabel-onnx-0.7.26.5.tar` & `odlabel-onnx-0.7.26.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 06:50:42.670668 odlabel-onnx-0.7.26.5/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     8571 2024-05-17 06:50:42.670668 odlabel-onnx-0.7.26.5/PKG-INFO
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 06:50:42.666667 odlabel-onnx-0.7.26.5/app_onnx/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       29 2024-05-09 20:45:02.000000 odlabel-onnx-0.7.26.5/app_onnx/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      296 2024-05-05 15:20:09.000000 odlabel-onnx-0.7.26.5/app_onnx/main.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    29686 2024-05-16 09:50:35.000000 odlabel-onnx-0.7.26.5/app_onnx/main_window.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 06:50:42.666667 odlabel-onnx-0.7.26.5/app_onnx/workers/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-16 09:51:59.000000 odlabel-onnx-0.7.26.5/app_onnx/workers/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     3152 2024-05-13 17:03:11.000000 odlabel-onnx-0.7.26.5/app_onnx/workers/chart_worker.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    14369 2024-05-17 04:30:49.000000 odlabel-onnx-0.7.26.5/app_onnx/workers/detection_worker.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 06:50:42.666667 odlabel-onnx-0.7.26.5/app_onnx/workers/utils/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:33.000000 odlabel-onnx-0.7.26.5/app_onnx/workers/utils/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    10448 2024-05-13 17:39:51.000000 odlabel-onnx-0.7.26.5/app_onnx/workers/utils/chart_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     6004 2024-05-17 05:00:55.000000 odlabel-onnx-0.7.26.5/app_onnx/workers/utils/detection_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     1911 2024-05-10 17:32:16.000000 odlabel-onnx-0.7.26.5/app_onnx/workers/utils/draw_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     4818 2024-05-05 12:54:55.000000 odlabel-onnx-0.7.26.5/app_onnx/workers/utils/write_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     7076 2024-05-17 04:10:59.000000 odlabel-onnx-0.7.26.5/app_onnx/workers/yoloworld_onnx.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 06:50:42.670668 odlabel-onnx-0.7.26.5/odlabel_onnx.egg-info/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     8571 2024-05-17 06:50:42.000000 odlabel-onnx-0.7.26.5/odlabel_onnx.egg-info/PKG-INFO
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      622 2024-05-17 06:50:42.000000 odlabel-onnx-0.7.26.5/odlabel_onnx.egg-info/SOURCES.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        1 2024-05-17 06:50:42.000000 odlabel-onnx-0.7.26.5/odlabel_onnx.egg-info/dependency_links.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       59 2024-05-17 06:50:42.000000 odlabel-onnx-0.7.26.5/odlabel_onnx.egg-info/entry_points.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       98 2024-05-17 06:50:42.000000 odlabel-onnx-0.7.26.5/odlabel_onnx.egg-info/requires.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        9 2024-05-17 06:50:42.000000 odlabel-onnx-0.7.26.5/odlabel_onnx.egg-info/top_level.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      285 2024-05-17 06:50:42.670668 odlabel-onnx-0.7.26.5/setup.cfg
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     1317 2024-05-17 05:31:39.000000 odlabel-onnx-0.7.26.5/setup.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:11:09.814939 odlabel-onnx-0.7.26.6/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     8655 2024-05-17 08:11:09.814939 odlabel-onnx-0.7.26.6/PKG-INFO
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:11:09.814939 odlabel-onnx-0.7.26.6/app_onnx/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       29 2024-05-09 20:45:02.000000 odlabel-onnx-0.7.26.6/app_onnx/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      296 2024-05-05 15:20:09.000000 odlabel-onnx-0.7.26.6/app_onnx/main.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    29686 2024-05-16 09:50:35.000000 odlabel-onnx-0.7.26.6/app_onnx/main_window.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:11:09.814939 odlabel-onnx-0.7.26.6/app_onnx/workers/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-16 09:51:59.000000 odlabel-onnx-0.7.26.6/app_onnx/workers/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     3152 2024-05-13 17:03:11.000000 odlabel-onnx-0.7.26.6/app_onnx/workers/chart_worker.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    14369 2024-05-17 04:30:49.000000 odlabel-onnx-0.7.26.6/app_onnx/workers/detection_worker.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:11:09.814939 odlabel-onnx-0.7.26.6/app_onnx/workers/utils/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:33.000000 odlabel-onnx-0.7.26.6/app_onnx/workers/utils/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    10448 2024-05-13 17:39:51.000000 odlabel-onnx-0.7.26.6/app_onnx/workers/utils/chart_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     6004 2024-05-17 05:00:55.000000 odlabel-onnx-0.7.26.6/app_onnx/workers/utils/detection_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     1911 2024-05-10 17:32:16.000000 odlabel-onnx-0.7.26.6/app_onnx/workers/utils/draw_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     4818 2024-05-05 12:54:55.000000 odlabel-onnx-0.7.26.6/app_onnx/workers/utils/write_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     7076 2024-05-17 04:10:59.000000 odlabel-onnx-0.7.26.6/app_onnx/workers/yoloworld_onnx.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:11:09.814939 odlabel-onnx-0.7.26.6/odlabel_onnx.egg-info/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     8655 2024-05-17 08:11:09.000000 odlabel-onnx-0.7.26.6/odlabel_onnx.egg-info/PKG-INFO
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      622 2024-05-17 08:11:09.000000 odlabel-onnx-0.7.26.6/odlabel_onnx.egg-info/SOURCES.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        1 2024-05-17 08:11:09.000000 odlabel-onnx-0.7.26.6/odlabel_onnx.egg-info/dependency_links.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       59 2024-05-17 08:11:09.000000 odlabel-onnx-0.7.26.6/odlabel_onnx.egg-info/entry_points.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       98 2024-05-17 08:11:09.000000 odlabel-onnx-0.7.26.6/odlabel_onnx.egg-info/requires.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        9 2024-05-17 08:11:09.000000 odlabel-onnx-0.7.26.6/odlabel_onnx.egg-info/top_level.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      285 2024-05-17 08:11:09.814939 odlabel-onnx-0.7.26.6/setup.cfg
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     1317 2024-05-17 08:09:00.000000 odlabel-onnx-0.7.26.6/setup.py
```

### Comparing `odlabel-onnx-0.7.26.5/PKG-INFO` & `odlabel-onnx-0.7.26.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odlabel-onnx
-Version: 0.7.26.5
+Version: 0.7.26.6
 Summary: A tool for object detection, labeling and visualization using ONNX
 Home-page: https://github.com/Ziad-Algrafi/odlabel
 Author: Ziad-Algrafi
 Author-email: ZiadAlgrafi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -54,50 +54,53 @@
 ```bash
 pip install odlabel-onnx
 
 ```
 
 ## Usage
 
-To launch the ODLabel application, run the following command:
+To launch the PyTorch version of ODLabel application, run the following command:
 
 ```bash
 odlabel
 
 ```
 
-1. Select a YOLO-World model file (.pt) for object detection.
+To launch the ONNX version of ODLabel application, run the following command:
+
+```bash
+odlabel-onnx
+
+```
+
+1. Select a YOLO-World model file based on your installation for object detection.
 2. Choose the folder containing the images you want to label.
 3. Specify the output directory where the labeled data will be saved.
 4. Enter the object categories you want to detect, separated by commas.
 5. Configure additional options such as SAHI, device type, output format, train/validation split, confidence level, and NMS threshold.
 6. Click the "Start" button to begin the labeling process.
 7. Monitor the progress and view the detection results in the application.
 
 ## Pytroch Model
 
 | Model Type      | mAP  | mAP50 | mAP75 | Model                                                                                         |
 | --------------- | ---- | ----- | ----- | --------------------------------------------------------------------------------------------- |
-| yolov8s-world   | 37.4 | 52.0  | 40.6  | [Download](https://github.com/ultralytics/assets/releases/download/v8.2.0/yolov8s-world.pt)   |
 | yolov8s-worldv2 | 37.7 | 52.2  | 41.0  | [Download](https://github.com/ultralytics/assets/releases/download/v8.2.0/yolov8s-worldv2.pt) |
-| yolov8m-world   | 42.0 | 57.0  | 45.6  | [Download](https://github.com/ultralytics/assets/releases/download/v8.2.0/yolov8m-world.pt)   |
 | yolov8m-worldv2 | 43.0 | 58.4  | 46.8  | [Download](https://github.com/ultralytics/assets/releases/download/v8.2.0/yolov8m-worldv2.pt) |
-| yolov8l-world   | 45.7 | 61.3  | 49.8  | [Download](https://github.com/ultralytics/assets/releases/download/v8.2.0/yolov8l-world.pt)   |
 | yolov8l-worldv2 | 45.8 | 61.3  | 49.8  | [Download](https://github.com/ultralytics/assets/releases/download/v8.2.0/yolov8l-worldv2.pt) |
-| yolov8x-world   | 47.0 | 63.0  | 51.2  | [Download](https://github.com/ultralytics/assets/releases/download/v8.2.0/yolov8x-world.pt)   |
 | yolov8x-worldv2 | 47.1 | 62.8  | 51.4  | [Download](https://github.com/ultralytics/assets/releases/download/v8.2.0/yolov8x-worldv2.pt) |
 
 ## ONNX Model
 
-| Model Type      | mAP  | mAP50 | mAP75 | Model        |
-| --------------- | ---- | ----- | ----- | ------------ |
-| yolov8s-worldv2 | 37.7 | 52.2  | 41.0  | [Download]() |
-| yolov8m-worldv2 | 43.0 | 58.4  | 46.8  | [Download]() |
-| yolov8l-worldv2 | 45.8 | 61.3  | 49.8  | [Download]() |
-| yolov8x-worldv2 | 47.1 | 62.8  | 51.4  | [Download]() |
+| Model Type      | mAP  | mAP50 | mAP75 | Model                                                                                     |
+| --------------- | ---- | ----- | ----- | ----------------------------------------------------------------------------------------- |
+| yolov8s-worldv2 | 37.7 | 52.2  | 41.0  | [Download](https://github.com/Ziad-Algrafi/ODLabel/blob/main/assets/yolov8s-worldv2.onnx) |
+| yolov8m-worldv2 | 43.0 | 58.4  | 46.8  | [Download](https://github.com/Ziad-Algrafi/ODLabel/blob/main/assets/yolov8m-worldv2.onnx) |
+| yolov8l-worldv2 | 45.8 | 61.3  | 49.8  | [Download](https://github.com/Ziad-Algrafi/ODLabel/blob/main/assets/yolov8l-worldv2.onnx) |
+| yolov8x-worldv2 | 47.1 | 62.8  | 51.4  | [Download](https://github.com/Ziad-Algrafi/ODLabel/blob/main/assets/yolov8x-worldv2.onnx) |
 
 ## GUI Figures and Dashboard
 
 ODLabel provides a comprehensive dashboard with various figures and visualizations to assist in analyzing the input image data and object detection results. The dashboard is displayed within the graphical user interface (GUI) of the application, allowing for interactive exploration and understanding of the data.
 
 The following figures are available in the dashboard:
 
@@ -145,26 +148,26 @@
 
 ## License
 
 This project is licensed under the GNU Affero General Public License v3.0 (AGPL-3.0). See the [LICENSE](LICENSE) file for details.
 
 ## Contributing
 
-Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the [GitHub repository](https://github.com/Ziad-Algrafi/odlabel).
+We welcome contributions! Please read our [Code of Conduct](CONTRIBUTING.md#code-of-conduct) and follow the [contribution guidelines](CONTRIBUTING.md#how-to-contribute) when submitting issues or pull requests.
 
 ## Acknowledgements
 
 ODLabel is built using the following open-source libraries:
 
 - [CustomTkinter](https://github.com/TomSchimansky/CustomTkinter)
 - [Ultralytics YOLO](https://github.com/ultralytics/ultralytics)
 - [Matplotlib](https://matplotlib.org)
 - [OpenCV](https://opencv.org)
 - [PyTorch](https://pytorch.org)
-  [onnx]
+  [onnx] (https://onnxruntime.ai)
 
 - ODLabel runs locally on your machine and does not collect or send any data externally. Your data remains private and secure within your local environment.
 - We extend our gratitude to [AILab-CVC](https://github.com/AILab-CVC) for generously open-sourcing their model.
 
 ## Contact
 
 For any questions or inquiries, please contact the maintainer at - ZiadAlgrafi@gmail.com.
```

### Comparing `odlabel-onnx-0.7.26.5/app_onnx/main_window.py` & `odlabel-onnx-0.7.26.6/app_onnx/main_window.py`

 * *Files identical despite different names*

### Comparing `odlabel-onnx-0.7.26.5/app_onnx/workers/chart_worker.py` & `odlabel-onnx-0.7.26.6/app_onnx/workers/chart_worker.py`

 * *Files identical despite different names*

### Comparing `odlabel-onnx-0.7.26.5/app_onnx/workers/detection_worker.py` & `odlabel-onnx-0.7.26.6/app_onnx/workers/detection_worker.py`

 * *Files identical despite different names*

### Comparing `odlabel-onnx-0.7.26.5/app_onnx/workers/utils/chart_utils.py` & `odlabel-onnx-0.7.26.6/app_onnx/workers/utils/chart_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-onnx-0.7.26.5/app_onnx/workers/utils/detection_utils.py` & `odlabel-onnx-0.7.26.6/app_onnx/workers/utils/detection_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-onnx-0.7.26.5/app_onnx/workers/utils/draw_utils.py` & `odlabel-onnx-0.7.26.6/app_onnx/workers/utils/draw_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-onnx-0.7.26.5/app_onnx/workers/utils/write_utils.py` & `odlabel-onnx-0.7.26.6/app_onnx/workers/utils/write_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-onnx-0.7.26.5/app_onnx/workers/yoloworld_onnx.py` & `odlabel-onnx-0.7.26.6/app_onnx/workers/yoloworld_onnx.py`

 * *Files identical despite different names*

### Comparing `odlabel-onnx-0.7.26.5/odlabel_onnx.egg-info/PKG-INFO` & `odlabel-onnx-0.7.26.6/odlabel_onnx.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odlabel-onnx
-Version: 0.7.26.5
+Version: 0.7.26.6
 Summary: A tool for object detection, labeling and visualization using ONNX
 Home-page: https://github.com/Ziad-Algrafi/odlabel
 Author: Ziad-Algrafi
 Author-email: ZiadAlgrafi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -54,50 +54,53 @@
 ```bash
 pip install odlabel-onnx
 
 ```
 
 ## Usage
 
-To launch the ODLabel application, run the following command:
+To launch the PyTorch version of ODLabel application, run the following command:
 
 ```bash
 odlabel
 
 ```
 
-1. Select a YOLO-World model file (.pt) for object detection.
+To launch the ONNX version of ODLabel application, run the following command:
+
+```bash
+odlabel-onnx
+
+```
+
+1. Select a YOLO-World model file based on your installation for object detection.
 2. Choose the folder containing the images you want to label.
 3. Specify the output directory where the labeled data will be saved.
 4. Enter the object categories you want to detect, separated by commas.
 5. Configure additional options such as SAHI, device type, output format, train/validation split, confidence level, and NMS threshold.
 6. Click the "Start" button to begin the labeling process.
 7. Monitor the progress and view the detection results in the application.
 
 ## Pytroch Model
 
 | Model Type      | mAP  | mAP50 | mAP75 | Model                                                                                         |
 | --------------- | ---- | ----- | ----- | --------------------------------------------------------------------------------------------- |
-| yolov8s-world   | 37.4 | 52.0  | 40.6  | [Download](https://github.com/ultralytics/assets/releases/download/v8.2.0/yolov8s-world.pt)   |
 | yolov8s-worldv2 | 37.7 | 52.2  | 41.0  | [Download](https://github.com/ultralytics/assets/releases/download/v8.2.0/yolov8s-worldv2.pt) |
-| yolov8m-world   | 42.0 | 57.0  | 45.6  | [Download](https://github.com/ultralytics/assets/releases/download/v8.2.0/yolov8m-world.pt)   |
 | yolov8m-worldv2 | 43.0 | 58.4  | 46.8  | [Download](https://github.com/ultralytics/assets/releases/download/v8.2.0/yolov8m-worldv2.pt) |
-| yolov8l-world   | 45.7 | 61.3  | 49.8  | [Download](https://github.com/ultralytics/assets/releases/download/v8.2.0/yolov8l-world.pt)   |
 | yolov8l-worldv2 | 45.8 | 61.3  | 49.8  | [Download](https://github.com/ultralytics/assets/releases/download/v8.2.0/yolov8l-worldv2.pt) |
-| yolov8x-world   | 47.0 | 63.0  | 51.2  | [Download](https://github.com/ultralytics/assets/releases/download/v8.2.0/yolov8x-world.pt)   |
 | yolov8x-worldv2 | 47.1 | 62.8  | 51.4  | [Download](https://github.com/ultralytics/assets/releases/download/v8.2.0/yolov8x-worldv2.pt) |
 
 ## ONNX Model
 
-| Model Type      | mAP  | mAP50 | mAP75 | Model        |
-| --------------- | ---- | ----- | ----- | ------------ |
-| yolov8s-worldv2 | 37.7 | 52.2  | 41.0  | [Download]() |
-| yolov8m-worldv2 | 43.0 | 58.4  | 46.8  | [Download]() |
-| yolov8l-worldv2 | 45.8 | 61.3  | 49.8  | [Download]() |
-| yolov8x-worldv2 | 47.1 | 62.8  | 51.4  | [Download]() |
+| Model Type      | mAP  | mAP50 | mAP75 | Model                                                                                     |
+| --------------- | ---- | ----- | ----- | ----------------------------------------------------------------------------------------- |
+| yolov8s-worldv2 | 37.7 | 52.2  | 41.0  | [Download](https://github.com/Ziad-Algrafi/ODLabel/blob/main/assets/yolov8s-worldv2.onnx) |
+| yolov8m-worldv2 | 43.0 | 58.4  | 46.8  | [Download](https://github.com/Ziad-Algrafi/ODLabel/blob/main/assets/yolov8m-worldv2.onnx) |
+| yolov8l-worldv2 | 45.8 | 61.3  | 49.8  | [Download](https://github.com/Ziad-Algrafi/ODLabel/blob/main/assets/yolov8l-worldv2.onnx) |
+| yolov8x-worldv2 | 47.1 | 62.8  | 51.4  | [Download](https://github.com/Ziad-Algrafi/ODLabel/blob/main/assets/yolov8x-worldv2.onnx) |
 
 ## GUI Figures and Dashboard
 
 ODLabel provides a comprehensive dashboard with various figures and visualizations to assist in analyzing the input image data and object detection results. The dashboard is displayed within the graphical user interface (GUI) of the application, allowing for interactive exploration and understanding of the data.
 
 The following figures are available in the dashboard:
 
@@ -145,26 +148,26 @@
 
 ## License
 
 This project is licensed under the GNU Affero General Public License v3.0 (AGPL-3.0). See the [LICENSE](LICENSE) file for details.
 
 ## Contributing
 
-Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the [GitHub repository](https://github.com/Ziad-Algrafi/odlabel).
+We welcome contributions! Please read our [Code of Conduct](CONTRIBUTING.md#code-of-conduct) and follow the [contribution guidelines](CONTRIBUTING.md#how-to-contribute) when submitting issues or pull requests.
 
 ## Acknowledgements
 
 ODLabel is built using the following open-source libraries:
 
 - [CustomTkinter](https://github.com/TomSchimansky/CustomTkinter)
 - [Ultralytics YOLO](https://github.com/ultralytics/ultralytics)
 - [Matplotlib](https://matplotlib.org)
 - [OpenCV](https://opencv.org)
 - [PyTorch](https://pytorch.org)
-  [onnx]
+  [onnx] (https://onnxruntime.ai)
 
 - ODLabel runs locally on your machine and does not collect or send any data externally. Your data remains private and secure within your local environment.
 - We extend our gratitude to [AILab-CVC](https://github.com/AILab-CVC) for generously open-sourcing their model.
 
 ## Contact
 
 For any questions or inquiries, please contact the maintainer at - ZiadAlgrafi@gmail.com.
```

### Comparing `odlabel-onnx-0.7.26.5/odlabel_onnx.egg-info/SOURCES.txt` & `odlabel-onnx-0.7.26.6/odlabel_onnx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odlabel-onnx-0.7.26.5/setup.py` & `odlabel-onnx-0.7.26.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="odlabel-onnx",
-    version="0.7.26.5",
+    version="0.7.26.6",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "customtkinter",
         "matplotlib",
         "numpy",
         "opencv-python",
```

