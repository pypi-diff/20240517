# Comparing `tmp/odlabel-0.7.26.4.tar.gz` & `tmp/odlabel-0.7.26.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odlabel-0.7.26.4.tar", last modified: Mon May 13 17:35:45 2024, max compression
+gzip compressed data, was "odlabel-0.7.26.6.tar", last modified: Fri May 17 08:35:42 2024, max compression
```

## Comparing `odlabel-0.7.26.4.tar` & `odlabel-0.7.26.6.tar`

### file list

```diff
@@ -1,27 +1,25 @@
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-13 17:35:45.355650 odlabel-0.7.26.4/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    34273 2024-05-06 11:36:33.000000 odlabel-0.7.26.4/LICENSE
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     7825 2024-05-13 17:35:45.355650 odlabel-0.7.26.4/PKG-INFO
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     7061 2024-05-13 17:34:36.000000 odlabel-0.7.26.4/README.md
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-13 17:35:45.355650 odlabel-0.7.26.4/app/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       29 2024-05-09 20:45:02.000000 odlabel-0.7.26.4/app/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      296 2024-05-05 15:20:09.000000 odlabel-0.7.26.4/app/main.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    29628 2024-05-13 17:05:33.000000 odlabel-0.7.26.4/app/main_window.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-13 17:35:45.355650 odlabel-0.7.26.4/app/workers/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:08.000000 odlabel-0.7.26.4/app/workers/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     3152 2024-05-13 17:03:11.000000 odlabel-0.7.26.4/app/workers/chart_worker.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    14405 2024-05-10 15:31:20.000000 odlabel-0.7.26.4/app/workers/detection_worker.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-13 17:35:45.355650 odlabel-0.7.26.4/app/workers/utils/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:33.000000 odlabel-0.7.26.4/app/workers/utils/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    10448 2024-05-13 17:05:28.000000 odlabel-0.7.26.4/app/workers/utils/chart_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     6216 2024-05-10 15:15:58.000000 odlabel-0.7.26.4/app/workers/utils/detection_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     1911 2024-05-10 17:32:16.000000 odlabel-0.7.26.4/app/workers/utils/draw_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     4818 2024-05-05 12:54:55.000000 odlabel-0.7.26.4/app/workers/utils/write_utils.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-13 17:35:45.355650 odlabel-0.7.26.4/odlabel.egg-info/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     7825 2024-05-13 17:35:45.000000 odlabel-0.7.26.4/odlabel.egg-info/PKG-INFO
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      520 2024-05-13 17:35:45.000000 odlabel-0.7.26.4/odlabel.egg-info/SOURCES.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        1 2024-05-13 17:35:45.000000 odlabel-0.7.26.4/odlabel.egg-info/dependency_links.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       49 2024-05-13 17:35:45.000000 odlabel-0.7.26.4/odlabel.egg-info/entry_points.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       89 2024-05-13 17:35:45.000000 odlabel-0.7.26.4/odlabel.egg-info/requires.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        4 2024-05-13 17:35:45.000000 odlabel-0.7.26.4/odlabel.egg-info/top_level.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      275 2024-05-13 17:35:45.359650 odlabel-0.7.26.4/setup.cfg
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     1268 2024-05-13 17:35:34.000000 odlabel-0.7.26.4/setup.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:35:42.570520 odlabel-0.7.26.6/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     8653 2024-05-17 08:35:42.570520 odlabel-0.7.26.6/PKG-INFO
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:35:42.566521 odlabel-0.7.26.6/app/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       29 2024-05-17 04:49:36.000000 odlabel-0.7.26.6/app/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      296 2024-05-05 15:20:09.000000 odlabel-0.7.26.6/app/main.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    29684 2024-05-16 04:14:53.000000 odlabel-0.7.26.6/app/main_window.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:35:42.566521 odlabel-0.7.26.6/app/workers/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:08.000000 odlabel-0.7.26.6/app/workers/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     3152 2024-05-13 17:03:11.000000 odlabel-0.7.26.6/app/workers/chart_worker.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    14405 2024-05-16 09:39:28.000000 odlabel-0.7.26.6/app/workers/detection_worker.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:35:42.566521 odlabel-0.7.26.6/app/workers/utils/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:33.000000 odlabel-0.7.26.6/app/workers/utils/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    10448 2024-05-13 17:39:51.000000 odlabel-0.7.26.6/app/workers/utils/chart_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     6216 2024-05-10 15:15:58.000000 odlabel-0.7.26.6/app/workers/utils/detection_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     1911 2024-05-10 17:32:16.000000 odlabel-0.7.26.6/app/workers/utils/draw_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     4818 2024-05-05 12:54:55.000000 odlabel-0.7.26.6/app/workers/utils/write_utils.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:35:42.570520 odlabel-0.7.26.6/odlabel.egg-info/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     8653 2024-05-17 08:35:42.000000 odlabel-0.7.26.6/odlabel.egg-info/PKG-INFO
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      502 2024-05-17 08:35:42.000000 odlabel-0.7.26.6/odlabel.egg-info/SOURCES.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        1 2024-05-17 08:35:42.000000 odlabel-0.7.26.6/odlabel.egg-info/dependency_links.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       49 2024-05-17 08:35:42.000000 odlabel-0.7.26.6/odlabel.egg-info/entry_points.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       89 2024-05-17 08:35:42.000000 odlabel-0.7.26.6/odlabel.egg-info/requires.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        4 2024-05-17 08:35:42.000000 odlabel-0.7.26.6/odlabel.egg-info/top_level.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      275 2024-05-17 08:35:42.570520 odlabel-0.7.26.6/setup.cfg
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     1285 2024-05-17 08:34:31.000000 odlabel-0.7.26.6/setup.py
```

### Comparing `odlabel-0.7.26.4/PKG-INFO` & `odlabel-0.7.26.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: odlabel
-Version: 0.7.26.4
-Summary: A tool for object detection, labeling and visualization
+Version: 0.7.26.6
+Summary: A tool for object detection, labeling and visualization using PyTorch
 Home-page: https://github.com/Ziad-Algrafi/odlabel
 Author: Ziad-Algrafi
 Author-email: ZiadAlgrafi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -13,15 +13,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 ![output](https://github.com/Ziad-Algrafi/ODLabel/assets/117011801/0bf8f35d-5337-4ee4-b694-5c957fe25992)
 
 # ODLabel
 
 ODLabel (Open Dictionary Labeler) is a powerful tool for zero-shot object detection, labeling and visualization. It provides an intuitive graphical user interface for labeling objects in images using the YOLO-World model and supports various output formats such as YOLO, COCO, CSV, and XML.
 
@@ -35,50 +34,74 @@
 - Select device type (CPU or GPU) for inference
 - Customize train/validation split ratio
 - Adjust confidence level and non-maximum suppression (IoU) threshold
 - Visualize input image statistics and output detection results
 
 ## Installation
 
-You can install ODLabel from [PyPI](https://pypi.org/project/odlabel/) using pip:
+### PyTorch Version
+
+To install the PyTorch version of ODLabel, run the following command:
 
 ```bash
 pip install odlabel
 
 ```
 
+### ONNX Version
+
+To install the ONNX version of ODLabel, run the following command:
+
+```bash
+pip install odlabel-onnx
+
+```
+
 ## Usage
 
-To launch the ODLabel application, run the following command:
+To launch the PyTorch version of ODLabel application, run the following command:
 
 ```bash
 odlabel
+
+```
+
+To launch the ONNX version of ODLabel application, run the following command:
+
+```bash
+odlabel-onnx
+
 ```
 
-1. Select a YOLO-World model file (.pt) for object detection.
+1. Select a YOLO-World model file based on your installation for object detection.
 2. Choose the folder containing the images you want to label.
 3. Specify the output directory where the labeled data will be saved.
 4. Enter the object categories you want to detect, separated by commas.
 5. Configure additional options such as SAHI, device type, output format, train/validation split, confidence level, and NMS threshold.
 6. Click the "Start" button to begin the labeling process.
 7. Monitor the progress and view the detection results in the application.
 
-## Model
+## Pytroch Model
 
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
 
+## ONNX Model
+
+| Model Type      | mAP  | mAP50 | mAP75 | Model                                                                                     |
+| --------------- | ---- | ----- | ----- | ----------------------------------------------------------------------------------------- |
+| yolov8s-worldv2 | 37.7 | 52.2  | 41.0  | [Download](https://github.com/Ziad-Algrafi/ODLabel/blob/main/assets/yolov8s-worldv2.onnx) |
+| yolov8m-worldv2 | 43.0 | 58.4  | 46.8  | [Download](https://github.com/Ziad-Algrafi/ODLabel/blob/main/assets/yolov8m-worldv2.onnx) |
+| yolov8l-worldv2 | 45.8 | 61.3  | 49.8  | [Download](https://github.com/Ziad-Algrafi/ODLabel/blob/main/assets/yolov8l-worldv2.onnx) |
+| yolov8x-worldv2 | 47.1 | 62.8  | 51.4  | [Download](https://github.com/Ziad-Algrafi/ODLabel/blob/main/assets/yolov8x-worldv2.onnx) |
+
 ## GUI Figures and Dashboard
 
 ODLabel provides a comprehensive dashboard with various figures and visualizations to assist in analyzing the input image data and object detection results. The dashboard is displayed within the graphical user interface (GUI) of the application, allowing for interactive exploration and understanding of the data.
 
 The following figures are available in the dashboard:
 
 1. **Format and Instances Chart:** This chart combines two visualizations in one figure:
@@ -103,41 +126,50 @@
 
 7. **Spatial Distribution of Objects:** A chart that visualizes the bounding boxes of detected objects. Each bounding box is represented by a rectangle, with the color intensity indicating the degree of overlap with other bounding boxes. Areas with darker colors signify a higher concentration of overlapping bounding boxes.
 
 8. **Heatmap of Detection:** A heatmap visualization that showcases the spatial distribution of detected objects within the image space. The heatmap uses different colors to indicate the density of detections at various locations, with brighter colors representing higher concentrations.
 
 These figures provide valuable insights into the input image data and the object detection results, enabling users to identify potential issues, patterns, and areas for further analysis or improvement. The dashboard serves as a powerful tool for exploring and understanding the data, facilitating informed decision-making and enhancing the overall object detection and labeling workflow.
 
-## Update
+## Upgrade
 
-You can upgrade ODLabel using pip:
+You can upgrade PyTorch version of ODLabel using pip:
 
 ```bash
 pip install --upgrade odlabel
 
 ```
 
+You can upgrade ONNX version of ODLabel using pip:
+
+```bash
+pip install --upgrade odlabel-onnx
+
+```
+
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
+  [onnx] (https://onnxruntime.ai)
 
-ODLabel runs locally on your machine and does not collect or send any data externally. Your data remains private and secure within your local environment.
+- ODLabel runs locally on your machine and does not collect or send any data externally. Your data remains private and secure within your local environment.
+- We extend our gratitude to [AILab-CVC](https://github.com/AILab-CVC) for generously open-sourcing their model.
 
 ## Contact
 
 For any questions or inquiries, please contact the maintainer at - ZiadAlgrafi@gmail.com.
```

### Comparing `odlabel-0.7.26.4/README.md` & `odlabel-0.7.26.6/odlabel.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: odlabel
+Version: 0.7.26.6
+Summary: A tool for object detection, labeling and visualization using PyTorch
+Home-page: https://github.com/Ziad-Algrafi/odlabel
+Author: Ziad-Algrafi
+Author-email: ZiadAlgrafi@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+
 ![output](https://github.com/Ziad-Algrafi/ODLabel/assets/117011801/0bf8f35d-5337-4ee4-b694-5c957fe25992)
 
 # ODLabel
 
 ODLabel (Open Dictionary Labeler) is a powerful tool for zero-shot object detection, labeling and visualization. It provides an intuitive graphical user interface for labeling objects in images using the YOLO-World model and supports various output formats such as YOLO, COCO, CSV, and XML.
 
 ## Features
@@ -14,50 +34,74 @@
 - Select device type (CPU or GPU) for inference
 - Customize train/validation split ratio
 - Adjust confidence level and non-maximum suppression (IoU) threshold
 - Visualize input image statistics and output detection results
 
 ## Installation
 
-You can install ODLabel from [PyPI](https://pypi.org/project/odlabel/) using pip:
+### PyTorch Version
+
+To install the PyTorch version of ODLabel, run the following command:
 
 ```bash
 pip install odlabel
 
 ```
 
+### ONNX Version
+
+To install the ONNX version of ODLabel, run the following command:
+
+```bash
+pip install odlabel-onnx
+
+```
+
 ## Usage
 
-To launch the ODLabel application, run the following command:
+To launch the PyTorch version of ODLabel application, run the following command:
 
 ```bash
 odlabel
+
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
 
-## Model
+## Pytroch Model
 
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
 
+## ONNX Model
+
+| Model Type      | mAP  | mAP50 | mAP75 | Model                                                                                     |
+| --------------- | ---- | ----- | ----- | ----------------------------------------------------------------------------------------- |
+| yolov8s-worldv2 | 37.7 | 52.2  | 41.0  | [Download](https://github.com/Ziad-Algrafi/ODLabel/blob/main/assets/yolov8s-worldv2.onnx) |
+| yolov8m-worldv2 | 43.0 | 58.4  | 46.8  | [Download](https://github.com/Ziad-Algrafi/ODLabel/blob/main/assets/yolov8m-worldv2.onnx) |
+| yolov8l-worldv2 | 45.8 | 61.3  | 49.8  | [Download](https://github.com/Ziad-Algrafi/ODLabel/blob/main/assets/yolov8l-worldv2.onnx) |
+| yolov8x-worldv2 | 47.1 | 62.8  | 51.4  | [Download](https://github.com/Ziad-Algrafi/ODLabel/blob/main/assets/yolov8x-worldv2.onnx) |
+
 ## GUI Figures and Dashboard
 
 ODLabel provides a comprehensive dashboard with various figures and visualizations to assist in analyzing the input image data and object detection results. The dashboard is displayed within the graphical user interface (GUI) of the application, allowing for interactive exploration and understanding of the data.
 
 The following figures are available in the dashboard:
 
 1. **Format and Instances Chart:** This chart combines two visualizations in one figure:
@@ -82,39 +126,50 @@
 
 7. **Spatial Distribution of Objects:** A chart that visualizes the bounding boxes of detected objects. Each bounding box is represented by a rectangle, with the color intensity indicating the degree of overlap with other bounding boxes. Areas with darker colors signify a higher concentration of overlapping bounding boxes.
 
 8. **Heatmap of Detection:** A heatmap visualization that showcases the spatial distribution of detected objects within the image space. The heatmap uses different colors to indicate the density of detections at various locations, with brighter colors representing higher concentrations.
 
 These figures provide valuable insights into the input image data and the object detection results, enabling users to identify potential issues, patterns, and areas for further analysis or improvement. The dashboard serves as a powerful tool for exploring and understanding the data, facilitating informed decision-making and enhancing the overall object detection and labeling workflow.
 
-## Update
+## Upgrade
 
-You can upgrade ODLabel using pip:
+You can upgrade PyTorch version of ODLabel using pip:
 
 ```bash
 pip install --upgrade odlabel
 
 ```
 
+You can upgrade ONNX version of ODLabel using pip:
+
+```bash
+pip install --upgrade odlabel-onnx
+
+```
+
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
+  [onnx] (https://onnxruntime.ai)
 
-ODLabel runs locally on your machine and does not collect or send any data externally. Your data remains private and secure within your local environment.
+- ODLabel runs locally on your machine and does not collect or send any data externally. Your data remains private and secure within your local environment.
+- We extend our gratitude to [AILab-CVC](https://github.com/AILab-CVC) for generously open-sourcing their model.
 
 ## Contact
 
 For any questions or inquiries, please contact the maintainer at - ZiadAlgrafi@gmail.com.
+
+
```

### Comparing `odlabel-0.7.26.4/app/main_window.py` & `odlabel-0.7.26.6/app/main_window.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import queue
 from queue import Queue
 import customtkinter
-import torch
+import torch.cuda as cuda
 from tkinter import messagebox, filedialog
 from .workers.chart_worker import ChartWorker
 from .workers.detection_worker import ObjectDetectionWorker
 
 
 class MainWindow:
     def __init__(self, root):
@@ -362,30 +362,31 @@
         device = "cpu"
 
         if not self.classes:
             self.show_error_message("Please enter class names.")
             return
         
         if self.device_var.get() == "GPU":
-            gpu_available = torch.cuda.is_available()
+            gpu_available = cuda.is_available()
             if gpu_available:
-                device = "0"
-                gpu_name = torch.cuda.get_device_name(0)
+                device = "cuda"
+                gpu_name = cuda.get_device_name(0)
                 self.log_text.configure(state="normal")
                 self.log_text.insert(customtkinter.END, f"Using GPU: {gpu_name}\n")
                 self.log_text.configure(state="disabled")
             else:
                 device = "cpu"
                 self.log_text.configure(state="normal")
                 self.log_text.insert(customtkinter.END, "No GPU found. Using CPU instead.\n")
-                self.log_text.configure(state="disabled")       
+                self.log_text.configure(state="disabled")
+                self.device_radiobutton_cpu.invoke()       
         else:
             self.log_text.configure(state="normal")
             self.log_text.insert(customtkinter.END, "Using CPU.\n")
-            self.log_text.configure(state="disabled")  
+            self.log_text.configure(state="disabled") 
 
         try:
             self.clear_output()
             self.worker_thread = ObjectDetectionWorker(
                 conf_threshold,
                 model_path,
                 images_folder,
```

### Comparing `odlabel-0.7.26.4/app/workers/chart_worker.py` & `odlabel-0.7.26.6/app/workers/chart_worker.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.4/app/workers/detection_worker.py` & `odlabel-0.7.26.6/app/workers/detection_worker.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.4/app/workers/utils/chart_utils.py` & `odlabel-0.7.26.6/app/workers/utils/chart_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.4/app/workers/utils/detection_utils.py` & `odlabel-0.7.26.6/app/workers/utils/detection_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.4/app/workers/utils/draw_utils.py` & `odlabel-0.7.26.6/app/workers/utils/draw_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.4/app/workers/utils/write_utils.py` & `odlabel-0.7.26.6/app/workers/utils/write_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.4/setup.py` & `odlabel-0.7.26.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="odlabel",
-    version="0.7.26.4",
+    version="0.7.26.6",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "customtkinter",
         "ultralytics",
         "matplotlib",
         "numpy",
@@ -17,16 +17,16 @@
     entry_points={
         "console_scripts": [
             "odlabel=app.main:launch_GUI",
         ],
     },
     author="Ziad-Algrafi",
     author_email="ZiadAlgrafi@gmail.com",
-    description="A tool for object detection, labeling and visualization",
-    long_description=open("README.md").read(),
+    description="A tool for object detection, labeling and visualization using PyTorch",
+    long_description=open("../README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Ziad-Algrafi/odlabel",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Programming Language :: Python :: 3",
```

