# Comparing `tmp/odlabel-0.7.26.7.tar.gz` & `tmp/odlabel-0.7.26.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odlabel-0.7.26.7.tar", last modified: Fri May 17 08:56:07 2024, max compression
+gzip compressed data, was "odlabel-0.7.26.8.tar", last modified: Fri May 17 12:09:41 2024, max compression
```

## Comparing `odlabel-0.7.26.7.tar` & `odlabel-0.7.26.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:56:07.043775 odlabel-0.7.26.7/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     8708 2024-05-17 08:56:07.043775 odlabel-0.7.26.7/PKG-INFO
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:56:07.043775 odlabel-0.7.26.7/app/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       29 2024-05-17 04:49:36.000000 odlabel-0.7.26.7/app/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      296 2024-05-05 15:20:09.000000 odlabel-0.7.26.7/app/main.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    29684 2024-05-16 04:14:53.000000 odlabel-0.7.26.7/app/main_window.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:56:07.043775 odlabel-0.7.26.7/app/workers/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:08.000000 odlabel-0.7.26.7/app/workers/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     3152 2024-05-13 17:03:11.000000 odlabel-0.7.26.7/app/workers/chart_worker.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    14405 2024-05-16 09:39:28.000000 odlabel-0.7.26.7/app/workers/detection_worker.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:56:07.043775 odlabel-0.7.26.7/app/workers/utils/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:33.000000 odlabel-0.7.26.7/app/workers/utils/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    10448 2024-05-13 17:39:51.000000 odlabel-0.7.26.7/app/workers/utils/chart_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     6216 2024-05-10 15:15:58.000000 odlabel-0.7.26.7/app/workers/utils/detection_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     1911 2024-05-10 17:32:16.000000 odlabel-0.7.26.7/app/workers/utils/draw_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     4818 2024-05-05 12:54:55.000000 odlabel-0.7.26.7/app/workers/utils/write_utils.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 08:56:07.043775 odlabel-0.7.26.7/odlabel.egg-info/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     8708 2024-05-17 08:56:07.000000 odlabel-0.7.26.7/odlabel.egg-info/PKG-INFO
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      502 2024-05-17 08:56:07.000000 odlabel-0.7.26.7/odlabel.egg-info/SOURCES.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        1 2024-05-17 08:56:07.000000 odlabel-0.7.26.7/odlabel.egg-info/dependency_links.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       49 2024-05-17 08:56:07.000000 odlabel-0.7.26.7/odlabel.egg-info/entry_points.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       89 2024-05-17 08:56:07.000000 odlabel-0.7.26.7/odlabel.egg-info/requires.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        4 2024-05-17 08:56:07.000000 odlabel-0.7.26.7/odlabel.egg-info/top_level.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      275 2024-05-17 08:56:07.043775 odlabel-0.7.26.7/setup.cfg
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     1285 2024-05-17 08:53:06.000000 odlabel-0.7.26.7/setup.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 12:09:41.576879 odlabel-0.7.26.8/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     8807 2024-05-17 12:09:41.576879 odlabel-0.7.26.8/PKG-INFO
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 12:09:41.576879 odlabel-0.7.26.8/app/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       29 2024-05-17 04:49:36.000000 odlabel-0.7.26.8/app/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      296 2024-05-05 15:20:09.000000 odlabel-0.7.26.8/app/main.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    29684 2024-05-16 04:14:53.000000 odlabel-0.7.26.8/app/main_window.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 12:09:41.576879 odlabel-0.7.26.8/app/workers/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:08.000000 odlabel-0.7.26.8/app/workers/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     3152 2024-05-13 17:03:11.000000 odlabel-0.7.26.8/app/workers/chart_worker.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    14405 2024-05-16 09:39:28.000000 odlabel-0.7.26.8/app/workers/detection_worker.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 12:09:41.576879 odlabel-0.7.26.8/app/workers/utils/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:33.000000 odlabel-0.7.26.8/app/workers/utils/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    10448 2024-05-13 17:39:51.000000 odlabel-0.7.26.8/app/workers/utils/chart_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     6216 2024-05-10 15:15:58.000000 odlabel-0.7.26.8/app/workers/utils/detection_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     1911 2024-05-10 17:32:16.000000 odlabel-0.7.26.8/app/workers/utils/draw_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     4818 2024-05-05 12:54:55.000000 odlabel-0.7.26.8/app/workers/utils/write_utils.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 12:09:41.576879 odlabel-0.7.26.8/odlabel.egg-info/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     8807 2024-05-17 12:09:41.000000 odlabel-0.7.26.8/odlabel.egg-info/PKG-INFO
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      502 2024-05-17 12:09:41.000000 odlabel-0.7.26.8/odlabel.egg-info/SOURCES.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        1 2024-05-17 12:09:41.000000 odlabel-0.7.26.8/odlabel.egg-info/dependency_links.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       49 2024-05-17 12:09:41.000000 odlabel-0.7.26.8/odlabel.egg-info/entry_points.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      106 2024-05-17 12:09:41.000000 odlabel-0.7.26.8/odlabel.egg-info/requires.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        4 2024-05-17 12:09:41.000000 odlabel-0.7.26.8/odlabel.egg-info/top_level.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      293 2024-05-17 12:09:41.580879 odlabel-0.7.26.8/setup.cfg
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     1313 2024-05-17 12:09:17.000000 odlabel-0.7.26.8/setup.py
```

### Comparing `odlabel-0.7.26.7/PKG-INFO` & `odlabel-0.7.26.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odlabel
-Version: 0.7.26.7
+Version: 0.7.26.8
 Summary: A tool for object detection, labeling and visualization using PyTorch
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

### Comparing `odlabel-0.7.26.7/app/main_window.py` & `odlabel-0.7.26.8/app/main_window.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.7/app/workers/chart_worker.py` & `odlabel-0.7.26.8/app/workers/chart_worker.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.7/app/workers/detection_worker.py` & `odlabel-0.7.26.8/app/workers/detection_worker.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.7/app/workers/utils/chart_utils.py` & `odlabel-0.7.26.8/app/workers/utils/chart_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.7/app/workers/utils/detection_utils.py` & `odlabel-0.7.26.8/app/workers/utils/detection_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.7/app/workers/utils/draw_utils.py` & `odlabel-0.7.26.8/app/workers/utils/draw_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.7/app/workers/utils/write_utils.py` & `odlabel-0.7.26.8/app/workers/utils/write_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-0.7.26.7/odlabel.egg-info/PKG-INFO` & `odlabel-0.7.26.8/odlabel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odlabel
-Version: 0.7.26.7
+Version: 0.7.26.8
 Summary: A tool for object detection, labeling and visualization using PyTorch
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

### Comparing `odlabel-0.7.26.7/setup.py` & `odlabel-0.7.26.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name="odlabel",
-    version="0.7.26.7",
+    version="0.7.26.8",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "customtkinter",
         "ultralytics",
         "matplotlib",
         "numpy",
         "opencv-python",
         "torch>=1.7.0",
         "torchvision>=0.8.0",
+        "clip-for-odlabel",
     ],
     entry_points={
         "console_scripts": [
             "odlabel=app.main:launch_GUI",
         ],
     },
     author="Ziad-Algrafi",
```

