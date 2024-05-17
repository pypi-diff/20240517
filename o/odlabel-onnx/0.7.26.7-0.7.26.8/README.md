# Comparing `tmp/odlabel-onnx-0.7.26.7.tar.gz` & `tmp/odlabel-onnx-0.7.26.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odlabel-onnx-0.7.26.7.tar", last modified: Fri May 17 08:56:25 2024, max compression
+gzip compressed data, was "odlabel-onnx-0.7.26.8.tar", last modified: Fri May 17 12:07:08 2024, max compression
```

## Comparing `odlabel-onnx-0.7.26.7.tar` & `odlabel-onnx-0.7.26.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:56:25.063944 odlabel-onnx-0.7.26.7/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     8710 2024-05-17 08:56:25.063944 odlabel-onnx-0.7.26.7/PKG-INFO
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:56:25.063944 odlabel-onnx-0.7.26.7/app_onnx/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       29 2024-05-09 20:45:02.000000 odlabel-onnx-0.7.26.7/app_onnx/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      296 2024-05-05 15:20:09.000000 odlabel-onnx-0.7.26.7/app_onnx/main.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    29686 2024-05-16 09:50:35.000000 odlabel-onnx-0.7.26.7/app_onnx/main_window.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:56:25.063944 odlabel-onnx-0.7.26.7/app_onnx/workers/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-16 09:51:59.000000 odlabel-onnx-0.7.26.7/app_onnx/workers/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     3152 2024-05-13 17:03:11.000000 odlabel-onnx-0.7.26.7/app_onnx/workers/chart_worker.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    14369 2024-05-17 04:30:49.000000 odlabel-onnx-0.7.26.7/app_onnx/workers/detection_worker.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:56:25.063944 odlabel-onnx-0.7.26.7/app_onnx/workers/utils/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:33.000000 odlabel-onnx-0.7.26.7/app_onnx/workers/utils/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    10448 2024-05-13 17:39:51.000000 odlabel-onnx-0.7.26.7/app_onnx/workers/utils/chart_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     6004 2024-05-17 05:00:55.000000 odlabel-onnx-0.7.26.7/app_onnx/workers/utils/detection_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     1911 2024-05-10 17:32:16.000000 odlabel-onnx-0.7.26.7/app_onnx/workers/utils/draw_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     4818 2024-05-05 12:54:55.000000 odlabel-onnx-0.7.26.7/app_onnx/workers/utils/write_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     7076 2024-05-17 04:10:59.000000 odlabel-onnx-0.7.26.7/app_onnx/workers/yoloworld_onnx.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:56:25.063944 odlabel-onnx-0.7.26.7/odlabel_onnx.egg-info/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     8710 2024-05-17 08:56:25.000000 odlabel-onnx-0.7.26.7/odlabel_onnx.egg-info/PKG-INFO
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      622 2024-05-17 08:56:25.000000 odlabel-onnx-0.7.26.7/odlabel_onnx.egg-info/SOURCES.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        1 2024-05-17 08:56:25.000000 odlabel-onnx-0.7.26.7/odlabel_onnx.egg-info/dependency_links.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       59 2024-05-17 08:56:25.000000 odlabel-onnx-0.7.26.7/odlabel_onnx.egg-info/entry_points.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       98 2024-05-17 08:56:25.000000 odlabel-onnx-0.7.26.7/odlabel_onnx.egg-info/requires.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        9 2024-05-17 08:56:25.000000 odlabel-onnx-0.7.26.7/odlabel_onnx.egg-info/top_level.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      285 2024-05-17 08:56:25.063944 odlabel-onnx-0.7.26.7/setup.cfg
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     1317 2024-05-17 08:55:33.000000 odlabel-onnx-0.7.26.7/setup.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 12:07:08.128384 odlabel-onnx-0.7.26.8/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     8809 2024-05-17 12:07:08.128384 odlabel-onnx-0.7.26.8/PKG-INFO
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 12:07:08.128384 odlabel-onnx-0.7.26.8/app_onnx/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       29 2024-05-09 20:45:02.000000 odlabel-onnx-0.7.26.8/app_onnx/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      296 2024-05-05 15:20:09.000000 odlabel-onnx-0.7.26.8/app_onnx/main.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    29686 2024-05-16 09:50:35.000000 odlabel-onnx-0.7.26.8/app_onnx/main_window.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 12:07:08.128384 odlabel-onnx-0.7.26.8/app_onnx/workers/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-16 09:51:59.000000 odlabel-onnx-0.7.26.8/app_onnx/workers/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     3152 2024-05-13 17:03:11.000000 odlabel-onnx-0.7.26.8/app_onnx/workers/chart_worker.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    14369 2024-05-17 04:30:49.000000 odlabel-onnx-0.7.26.8/app_onnx/workers/detection_worker.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 12:07:08.128384 odlabel-onnx-0.7.26.8/app_onnx/workers/utils/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:33.000000 odlabel-onnx-0.7.26.8/app_onnx/workers/utils/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    10448 2024-05-13 17:39:51.000000 odlabel-onnx-0.7.26.8/app_onnx/workers/utils/chart_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     6004 2024-05-17 05:00:55.000000 odlabel-onnx-0.7.26.8/app_onnx/workers/utils/detection_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     1911 2024-05-10 17:32:16.000000 odlabel-onnx-0.7.26.8/app_onnx/workers/utils/draw_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     4818 2024-05-05 12:54:55.000000 odlabel-onnx-0.7.26.8/app_onnx/workers/utils/write_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     7076 2024-05-17 04:10:59.000000 odlabel-onnx-0.7.26.8/app_onnx/workers/yoloworld_onnx.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 12:07:08.128384 odlabel-onnx-0.7.26.8/odlabel_onnx.egg-info/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     8809 2024-05-17 12:07:08.000000 odlabel-onnx-0.7.26.8/odlabel_onnx.egg-info/PKG-INFO
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      622 2024-05-17 12:07:08.000000 odlabel-onnx-0.7.26.8/odlabel_onnx.egg-info/SOURCES.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        1 2024-05-17 12:07:08.000000 odlabel-onnx-0.7.26.8/odlabel_onnx.egg-info/dependency_links.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       59 2024-05-17 12:07:08.000000 odlabel-onnx-0.7.26.8/odlabel_onnx.egg-info/entry_points.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      110 2024-05-17 12:07:08.000000 odlabel-onnx-0.7.26.8/odlabel_onnx.egg-info/requires.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        9 2024-05-17 12:07:08.000000 odlabel-onnx-0.7.26.8/odlabel_onnx.egg-info/top_level.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      297 2024-05-17 12:07:08.128384 odlabel-onnx-0.7.26.8/setup.cfg
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     1329 2024-05-17 12:06:29.000000 odlabel-onnx-0.7.26.8/setup.py
```

### Comparing `odlabel-onnx-0.7.26.7/PKG-INFO` & `odlabel-onnx-0.7.26.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odlabel-onnx
-Version: 0.7.26.7
+Version: 0.7.26.8
 Summary: A tool for object detection, labeling and visualization using ONNX
 Home-page: https://github.com/Ziad-Algrafi/odlabel
 Author: Ziad-Algrafi
 Author-email: ZiadAlgrafi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -148,26 +148,26 @@
 
 ## License
 
 This project is licensed under the GNU Affero General Public License v3.0 (AGPL-3.0). See the [LICENSE](LICENSE) file for details.
 
 ## Contributing
 
-We welcome contributions! Please read our [Code of Conduct](CONTRIBUTING.md#code-of-conduct) and follow the [contribution guidelines](CONTRIBUTING.md#how-to-contribute) when submitting issues or pull requests.
+We welcome contributions! Please read our [Code of Conduct](https://github.com/Ziad-Algrafi/ODLabel/blob/main/CONTRIBUTING.md#code-of-conduct) and follow the [contribution guidelines](https://github.com/Ziad-Algrafi/ODLabel/blob/main/CONTRIBUTING.md#how-to-contribute) when submitting issues or pull requests.
 
 ## Acknowledgements
 
 ODLabel is built using the following open-source libraries:
 
 - [CustomTkinter](https://github.com/TomSchimansky/CustomTkinter)
 - [Ultralytics YOLO](https://github.com/ultralytics/ultralytics)
 - [Matplotlib](https://matplotlib.org)
 - [OpenCV](https://opencv.org)
 - [PyTorch](https://pytorch.org)
-  [onnx] (https://onnxruntime.ai)
+- [ONNX](https://onnxruntime.ai)
 
 - ODLabel runs locally on your machine and does not collect or send any data externally. Your data remains private and secure within your local environment.
 - We extend our gratitude to [AILab-CVC](https://github.com/AILab-CVC) for generously open-sourcing their model.
 
 ## Contact
 
 For any questions or inquiries, please contact the maintainer at - ZiadAlgrafi@gmail.com.
```

### Comparing `odlabel-onnx-0.7.26.7/app_onnx/main_window.py` & `odlabel-onnx-0.7.26.8/app_onnx/main_window.py`

 * *Files identical despite different names*

### Comparing `odlabel-onnx-0.7.26.7/app_onnx/workers/chart_worker.py` & `odlabel-onnx-0.7.26.8/app_onnx/workers/chart_worker.py`

 * *Files identical despite different names*

### Comparing `odlabel-onnx-0.7.26.7/app_onnx/workers/detection_worker.py` & `odlabel-onnx-0.7.26.8/app_onnx/workers/detection_worker.py`

 * *Files identical despite different names*

### Comparing `odlabel-onnx-0.7.26.7/app_onnx/workers/utils/chart_utils.py` & `odlabel-onnx-0.7.26.8/app_onnx/workers/utils/chart_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-onnx-0.7.26.7/app_onnx/workers/utils/detection_utils.py` & `odlabel-onnx-0.7.26.8/app_onnx/workers/utils/detection_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-onnx-0.7.26.7/app_onnx/workers/utils/draw_utils.py` & `odlabel-onnx-0.7.26.8/app_onnx/workers/utils/draw_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-onnx-0.7.26.7/app_onnx/workers/utils/write_utils.py` & `odlabel-onnx-0.7.26.8/app_onnx/workers/utils/write_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-onnx-0.7.26.7/app_onnx/workers/yoloworld_onnx.py` & `odlabel-onnx-0.7.26.8/app_onnx/workers/yoloworld_onnx.py`

 * *Files identical despite different names*

### Comparing `odlabel-onnx-0.7.26.7/odlabel_onnx.egg-info/PKG-INFO` & `odlabel-onnx-0.7.26.8/odlabel_onnx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odlabel-onnx
-Version: 0.7.26.7
+Version: 0.7.26.8
 Summary: A tool for object detection, labeling and visualization using ONNX
 Home-page: https://github.com/Ziad-Algrafi/odlabel
 Author: Ziad-Algrafi
 Author-email: ZiadAlgrafi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -148,26 +148,26 @@
 
 ## License
 
 This project is licensed under the GNU Affero General Public License v3.0 (AGPL-3.0). See the [LICENSE](LICENSE) file for details.
 
 ## Contributing
 
-We welcome contributions! Please read our [Code of Conduct](CONTRIBUTING.md#code-of-conduct) and follow the [contribution guidelines](CONTRIBUTING.md#how-to-contribute) when submitting issues or pull requests.
+We welcome contributions! Please read our [Code of Conduct](https://github.com/Ziad-Algrafi/ODLabel/blob/main/CONTRIBUTING.md#code-of-conduct) and follow the [contribution guidelines](https://github.com/Ziad-Algrafi/ODLabel/blob/main/CONTRIBUTING.md#how-to-contribute) when submitting issues or pull requests.
 
 ## Acknowledgements
 
 ODLabel is built using the following open-source libraries:
 
 - [CustomTkinter](https://github.com/TomSchimansky/CustomTkinter)
 - [Ultralytics YOLO](https://github.com/ultralytics/ultralytics)
 - [Matplotlib](https://matplotlib.org)
 - [OpenCV](https://opencv.org)
 - [PyTorch](https://pytorch.org)
-  [onnx] (https://onnxruntime.ai)
+- [ONNX](https://onnxruntime.ai)
 
 - ODLabel runs locally on your machine and does not collect or send any data externally. Your data remains private and secure within your local environment.
 - We extend our gratitude to [AILab-CVC](https://github.com/AILab-CVC) for generously open-sourcing their model.
 
 ## Contact
 
 For any questions or inquiries, please contact the maintainer at - ZiadAlgrafi@gmail.com.
```

### Comparing `odlabel-onnx-0.7.26.7/odlabel_onnx.egg-info/SOURCES.txt` & `odlabel-onnx-0.7.26.8/odlabel_onnx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odlabel-onnx-0.7.26.7/setup.py` & `odlabel-onnx-0.7.26.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name="odlabel-onnx",
-    version="0.7.26.7",
+    version="0.7.26.8",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "customtkinter",
         "matplotlib",
         "numpy",
         "opencv-python",
         "onnxruntime-gpu",
-        "clip",
         "torch>=1.7.0",
         "torchvision>=0.8.0",
+        "clip-for-odlabel",
     ],
     entry_points={
         "console_scripts": [
             "odlabel-onnx=app_onnx.main:launch_GUI",
         ],
     },
     author="Ziad-Algrafi",
```

