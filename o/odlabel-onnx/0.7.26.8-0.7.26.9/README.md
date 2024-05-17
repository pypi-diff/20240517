# Comparing `tmp/odlabel-onnx-0.7.26.8.tar.gz` & `tmp/odlabel_onnx-0.7.26.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odlabel-onnx-0.7.26.8.tar", last modified: Fri May 17 12:07:08 2024, max compression
+gzip compressed data, was "odlabel_onnx-0.7.26.9.tar", last modified: Fri May 17 15:26:43 2024, max compression
```

## Comparing `odlabel-onnx-0.7.26.8.tar` & `odlabel_onnx-0.7.26.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 12:07:08.128384 odlabel-onnx-0.7.26.8/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     8809 2024-05-17 12:07:08.128384 odlabel-onnx-0.7.26.8/PKG-INFO
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 12:07:08.128384 odlabel-onnx-0.7.26.8/app_onnx/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       29 2024-05-09 20:45:02.000000 odlabel-onnx-0.7.26.8/app_onnx/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      296 2024-05-05 15:20:09.000000 odlabel-onnx-0.7.26.8/app_onnx/main.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    29686 2024-05-16 09:50:35.000000 odlabel-onnx-0.7.26.8/app_onnx/main_window.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 12:07:08.128384 odlabel-onnx-0.7.26.8/app_onnx/workers/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-16 09:51:59.000000 odlabel-onnx-0.7.26.8/app_onnx/workers/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     3152 2024-05-13 17:03:11.000000 odlabel-onnx-0.7.26.8/app_onnx/workers/chart_worker.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    14369 2024-05-17 04:30:49.000000 odlabel-onnx-0.7.26.8/app_onnx/workers/detection_worker.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 12:07:08.128384 odlabel-onnx-0.7.26.8/app_onnx/workers/utils/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:33.000000 odlabel-onnx-0.7.26.8/app_onnx/workers/utils/__init__.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)    10448 2024-05-13 17:39:51.000000 odlabel-onnx-0.7.26.8/app_onnx/workers/utils/chart_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     6004 2024-05-17 05:00:55.000000 odlabel-onnx-0.7.26.8/app_onnx/workers/utils/detection_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     1911 2024-05-10 17:32:16.000000 odlabel-onnx-0.7.26.8/app_onnx/workers/utils/draw_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     4818 2024-05-05 12:54:55.000000 odlabel-onnx-0.7.26.8/app_onnx/workers/utils/write_utils.py
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     7076 2024-05-17 04:10:59.000000 odlabel-onnx-0.7.26.8/app_onnx/workers/yoloworld_onnx.py
-drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 12:07:08.128384 odlabel-onnx-0.7.26.8/odlabel_onnx.egg-info/
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     8809 2024-05-17 12:07:08.000000 odlabel-onnx-0.7.26.8/odlabel_onnx.egg-info/PKG-INFO
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      622 2024-05-17 12:07:08.000000 odlabel-onnx-0.7.26.8/odlabel_onnx.egg-info/SOURCES.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        1 2024-05-17 12:07:08.000000 odlabel-onnx-0.7.26.8/odlabel_onnx.egg-info/dependency_links.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)       59 2024-05-17 12:07:08.000000 odlabel-onnx-0.7.26.8/odlabel_onnx.egg-info/entry_points.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      110 2024-05-17 12:07:08.000000 odlabel-onnx-0.7.26.8/odlabel_onnx.egg-info/requires.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)        9 2024-05-17 12:07:08.000000 odlabel-onnx-0.7.26.8/odlabel_onnx.egg-info/top_level.txt
--rw-rw-r--   0 ziad      (1000) ziad      (1000)      297 2024-05-17 12:07:08.128384 odlabel-onnx-0.7.26.8/setup.cfg
--rw-rw-r--   0 ziad      (1000) ziad      (1000)     1329 2024-05-17 12:06:29.000000 odlabel-onnx-0.7.26.8/setup.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 15:26:43.115132 odlabel_onnx-0.7.26.9/
+-rw-r--r--   0 ziad      (1000) ziad      (1000)     9065 2024-05-17 15:26:43.115132 odlabel_onnx-0.7.26.9/PKG-INFO
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 15:26:43.111132 odlabel_onnx-0.7.26.9/app_onnx/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       29 2024-05-09 20:45:02.000000 odlabel_onnx-0.7.26.9/app_onnx/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      296 2024-05-05 15:20:09.000000 odlabel_onnx-0.7.26.9/app_onnx/main.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    29686 2024-05-16 09:50:35.000000 odlabel_onnx-0.7.26.9/app_onnx/main_window.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 15:26:43.111132 odlabel_onnx-0.7.26.9/app_onnx/workers/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-16 09:51:59.000000 odlabel_onnx-0.7.26.9/app_onnx/workers/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     3152 2024-05-13 17:03:11.000000 odlabel_onnx-0.7.26.9/app_onnx/workers/chart_worker.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    14369 2024-05-17 12:49:00.000000 odlabel_onnx-0.7.26.9/app_onnx/workers/detection_worker.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 15:26:43.115132 odlabel_onnx-0.7.26.9/app_onnx/workers/utils/
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        0 2024-05-02 18:27:33.000000 odlabel_onnx-0.7.26.9/app_onnx/workers/utils/__init__.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)    10448 2024-05-13 17:39:51.000000 odlabel_onnx-0.7.26.9/app_onnx/workers/utils/chart_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     6004 2024-05-17 05:00:55.000000 odlabel_onnx-0.7.26.9/app_onnx/workers/utils/detection_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     1911 2024-05-10 17:32:16.000000 odlabel_onnx-0.7.26.9/app_onnx/workers/utils/draw_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     4818 2024-05-05 12:54:55.000000 odlabel_onnx-0.7.26.9/app_onnx/workers/utils/write_utils.py
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     7076 2024-05-17 04:10:59.000000 odlabel_onnx-0.7.26.9/app_onnx/workers/yoloworld_onnx.py
+drwxrwxr-x   0 ziad      (1000) ziad      (1000)        0 2024-05-17 15:26:43.115132 odlabel_onnx-0.7.26.9/odlabel_onnx.egg-info/
+-rw-r--r--   0 ziad      (1000) ziad      (1000)     9065 2024-05-17 15:26:43.000000 odlabel_onnx-0.7.26.9/odlabel_onnx.egg-info/PKG-INFO
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      622 2024-05-17 15:26:43.000000 odlabel_onnx-0.7.26.9/odlabel_onnx.egg-info/SOURCES.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        1 2024-05-17 15:26:43.000000 odlabel_onnx-0.7.26.9/odlabel_onnx.egg-info/dependency_links.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)       58 2024-05-17 15:26:43.000000 odlabel_onnx-0.7.26.9/odlabel_onnx.egg-info/entry_points.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      143 2024-05-17 15:26:43.000000 odlabel_onnx-0.7.26.9/odlabel_onnx.egg-info/requires.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)        9 2024-05-17 15:26:43.000000 odlabel_onnx-0.7.26.9/odlabel_onnx.egg-info/top_level.txt
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)      332 2024-05-17 15:26:43.115132 odlabel_onnx-0.7.26.9/setup.cfg
+-rw-rw-r--   0 ziad      (1000) ziad      (1000)     1392 2024-05-17 15:22:44.000000 odlabel_onnx-0.7.26.9/setup.py
```

### Comparing `odlabel-onnx-0.7.26.8/PKG-INFO` & `odlabel_onnx-0.7.26.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 Metadata-Version: 2.1
 Name: odlabel-onnx
-Version: 0.7.26.8
+Version: 0.7.26.9
 Summary: A tool for object detection, labeling and visualization using ONNX
 Home-page: https://github.com/Ziad-Algrafi/odlabel
 Author: Ziad-Algrafi
 Author-email: ZiadAlgrafi@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Requires-Dist: setuptools==69.5.1
+Requires-Dist: wheel==0.43.0
+Requires-Dist: customtkinter
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: opencv-python
+Requires-Dist: onnxruntime-gpu
+Requires-Dist: torch>=1.7.0
+Requires-Dist: torchvision>=0.8.0
+Requires-Dist: clip-for-odlabel
 
 ![output](https://github.com/Ziad-Algrafi/ODLabel/assets/117011801/0bf8f35d-5337-4ee4-b694-5c957fe25992)
 
 # ODLabel
 
 ODLabel (Open Dictionary Labeler) is a powerful tool for zero-shot object detection, labeling and visualization. It provides an intuitive graphical user interface for labeling objects in images using the YOLO-World model and supports various output formats such as YOLO, COCO, CSV, and XML.
 
@@ -167,9 +175,7 @@
 
 - ODLabel runs locally on your machine and does not collect or send any data externally. Your data remains private and secure within your local environment.
 - We extend our gratitude to [AILab-CVC](https://github.com/AILab-CVC) for generously open-sourcing their model.
 
 ## Contact
 
 For any questions or inquiries, please contact the maintainer at - ZiadAlgrafi@gmail.com.
-
-
```

### Comparing `odlabel-onnx-0.7.26.8/app_onnx/main_window.py` & `odlabel_onnx-0.7.26.9/app_onnx/main_window.py`

 * *Files identical despite different names*

### Comparing `odlabel-onnx-0.7.26.8/app_onnx/workers/chart_worker.py` & `odlabel_onnx-0.7.26.9/app_onnx/workers/chart_worker.py`

 * *Files identical despite different names*

### Comparing `odlabel-onnx-0.7.26.8/app_onnx/workers/detection_worker.py` & `odlabel_onnx-0.7.26.9/app_onnx/workers/detection_worker.py`

 * *Files identical despite different names*

### Comparing `odlabel-onnx-0.7.26.8/app_onnx/workers/utils/chart_utils.py` & `odlabel_onnx-0.7.26.9/app_onnx/workers/utils/chart_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-onnx-0.7.26.8/app_onnx/workers/utils/detection_utils.py` & `odlabel_onnx-0.7.26.9/app_onnx/workers/utils/detection_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-onnx-0.7.26.8/app_onnx/workers/utils/draw_utils.py` & `odlabel_onnx-0.7.26.9/app_onnx/workers/utils/draw_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-onnx-0.7.26.8/app_onnx/workers/utils/write_utils.py` & `odlabel_onnx-0.7.26.9/app_onnx/workers/utils/write_utils.py`

 * *Files identical despite different names*

### Comparing `odlabel-onnx-0.7.26.8/app_onnx/workers/yoloworld_onnx.py` & `odlabel_onnx-0.7.26.9/app_onnx/workers/yoloworld_onnx.py`

 * *Files identical despite different names*

### Comparing `odlabel-onnx-0.7.26.8/odlabel_onnx.egg-info/PKG-INFO` & `odlabel_onnx-0.7.26.9/odlabel_onnx.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 Metadata-Version: 2.1
 Name: odlabel-onnx
-Version: 0.7.26.8
+Version: 0.7.26.9
 Summary: A tool for object detection, labeling and visualization using ONNX
 Home-page: https://github.com/Ziad-Algrafi/odlabel
 Author: Ziad-Algrafi
 Author-email: ZiadAlgrafi@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Requires-Dist: setuptools==69.5.1
+Requires-Dist: wheel==0.43.0
+Requires-Dist: customtkinter
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: opencv-python
+Requires-Dist: onnxruntime-gpu
+Requires-Dist: torch>=1.7.0
+Requires-Dist: torchvision>=0.8.0
+Requires-Dist: clip-for-odlabel
 
 ![output](https://github.com/Ziad-Algrafi/ODLabel/assets/117011801/0bf8f35d-5337-4ee4-b694-5c957fe25992)
 
 # ODLabel
 
 ODLabel (Open Dictionary Labeler) is a powerful tool for zero-shot object detection, labeling and visualization. It provides an intuitive graphical user interface for labeling objects in images using the YOLO-World model and supports various output formats such as YOLO, COCO, CSV, and XML.
 
@@ -167,9 +175,7 @@
 
 - ODLabel runs locally on your machine and does not collect or send any data externally. Your data remains private and secure within your local environment.
 - We extend our gratitude to [AILab-CVC](https://github.com/AILab-CVC) for generously open-sourcing their model.
 
 ## Contact
 
 For any questions or inquiries, please contact the maintainer at - ZiadAlgrafi@gmail.com.
-
-
```

### Comparing `odlabel-onnx-0.7.26.8/odlabel_onnx.egg-info/SOURCES.txt` & `odlabel_onnx-0.7.26.9/odlabel_onnx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odlabel-onnx-0.7.26.8/setup.py` & `odlabel_onnx-0.7.26.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name="odlabel-onnx",
-    version="0.7.26.8",
+    version="0.7.26.9",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
+        "setuptools==69.5.1",
+        "wheel==0.43.0",
         "customtkinter",
         "matplotlib",
         "numpy",
         "opencv-python",
         "onnxruntime-gpu",
         "torch>=1.7.0",
         "torchvision>=0.8.0",
@@ -33,9 +35,9 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
     python_requires=">=3.9",
-    setup_requires=["setuptools>=38.6.0", "wheel"],
+    setup_requires=["setuptools>=69.5.1", "wheel>=0.43.0"],
 )
```

