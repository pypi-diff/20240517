# Comparing `tmp/pypalex-1.3.3.tar.gz` & `tmp/pypalex-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypalex-1.3.3.tar", last modified: Sat Apr  8 02:05:04 2023, max compression
+gzip compressed data, was "pypalex-1.3.4.tar", last modified: Fri May 17 05:32:39 2024, max compression
```

## Comparing `pypalex-1.3.3.tar` & `pypalex-1.3.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:05:04.081787 pypalex-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-08 02:04:52.000000 pypalex-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-08 02:04:52.000000 pypalex-1.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-04-08 02:05:04.081787 pypalex-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-04-08 02:04:52.000000 pypalex-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:05:04.081787 pypalex-1.3.3/pypalex/
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-04-08 02:04:52.000000 pypalex-1.3.3/pypalex/Extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-08 02:04:52.000000 pypalex-1.3.3/pypalex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-04-08 02:04:52.000000 pypalex-1.3.3/pypalex/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-08 02:04:52.000000 pypalex-1.3.3/pypalex/arg_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-08 02:04:52.000000 pypalex-1.3.3/pypalex/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-04-08 02:04:52.000000 pypalex-1.3.3/pypalex/conversion_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    38484 2023-04-08 02:04:52.000000 pypalex-1.3.3/pypalex/extraction_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-04-08 02:04:52.000000 pypalex-1.3.3/pypalex/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-04-08 02:04:52.000000 pypalex-1.3.3/pypalex/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13513 2023-04-08 02:04:52.000000 pypalex-1.3.3/pypalex/print_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-08 02:04:52.000000 pypalex-1.3.3/pypalex/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:05:04.081787 pypalex-1.3.3/pypalex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-04-08 02:05:04.000000 pypalex-1.3.3/pypalex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-08 02:05:04.000000 pypalex-1.3.3/pypalex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 02:05:04.000000 pypalex-1.3.3/pypalex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-08 02:05:04.000000 pypalex-1.3.3/pypalex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 02:05:04.000000 pypalex-1.3.3/pypalex.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-08 02:05:04.000000 pypalex-1.3.3/pypalex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-08 02:05:04.000000 pypalex-1.3.3/pypalex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 02:05:04.081787 pypalex-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-08 02:04:52.000000 pypalex-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:32:39.049581 pypalex-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-17 05:32:28.000000 pypalex-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-17 05:32:28.000000 pypalex-1.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13919 2024-05-17 05:32:39.049581 pypalex-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12894 2024-05-17 05:32:28.000000 pypalex-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:32:39.045581 pypalex-1.3.4/pypalex/
+-rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-05-17 05:32:28.000000 pypalex-1.3.4/pypalex/Extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-17 05:32:28.000000 pypalex-1.3.4/pypalex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13934 2024-05-17 05:32:28.000000 pypalex-1.3.4/pypalex/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-17 05:32:28.000000 pypalex-1.3.4/pypalex/arg_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-17 05:32:28.000000 pypalex-1.3.4/pypalex/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-17 05:32:28.000000 pypalex-1.3.4/pypalex/conversion_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38484 2024-05-17 05:32:28.000000 pypalex-1.3.4/pypalex/extraction_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-17 05:32:28.000000 pypalex-1.3.4/pypalex/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-17 05:32:28.000000 pypalex-1.3.4/pypalex/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-05-17 05:32:28.000000 pypalex-1.3.4/pypalex/print_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-17 05:32:28.000000 pypalex-1.3.4/pypalex/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:32:39.045581 pypalex-1.3.4/pypalex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13919 2024-05-17 05:32:38.000000 pypalex-1.3.4/pypalex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-17 05:32:39.000000 pypalex-1.3.4/pypalex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 05:32:38.000000 pypalex-1.3.4/pypalex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-17 05:32:38.000000 pypalex-1.3.4/pypalex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 05:32:38.000000 pypalex-1.3.4/pypalex.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-17 05:32:38.000000 pypalex-1.3.4/pypalex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-17 05:32:38.000000 pypalex-1.3.4/pypalex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 05:32:39.049581 pypalex-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-17 05:32:28.000000 pypalex-1.3.4/setup.py
```

### Comparing `pypalex-1.3.3/LICENSE` & `pypalex-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypalex-1.3.3/PKG-INFO` & `pypalex-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pypalex
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python Palette Extractor: extracts color palettes from images into json files.
 Home-page: https://github.com/AlTimofeyev/pypalex
 Author: Al Timofeyev
 Author-email: al.timofeyev@outlook.com
 License: MIT
-Download-URL: https://github.com/AlTimofeyev/pypalex/archive/1.3.3.tar.gz
+Download-URL: https://github.com/AlTimofeyev/pypalex/archive/1.3.4.tar.gz
 Keywords: python,pypalex,palex,color-palette,colorscheme,extract-colorscheme,extract-palette,extractor
 Platform: UNKNOWN
 Classifier: Environment :: X11 Applications
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: pypalex Version: 1.3.3 Summary: Python Palette
+Metadata-Version: 2.1 Name: pypalex Version: 1.3.4 Summary: Python Palette
 Extractor: extracts color palettes from images into json files. Home-page:
 https://github.com/AlTimofeyev/pypalex Author: Al Timofeyev Author-email:
 al.timofeyev@outlook.com License: MIT Download-URL: https://github.com/
-AlTimofeyev/pypalex/archive/1.3.3.tar.gz Keywords: python,pypalex,palex,color-
+AlTimofeyev/pypalex/archive/1.3.4.tar.gz Keywords: python,pypalex,palex,color-
 palette,colorscheme,extract-colorscheme,extract-palette,extractor Platform:
 UNKNOWN Classifier: Environment :: X11 Applications Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: MacOS Classifier:
 Operating System :: POSIX :: Linux Classifier: Operating System :: Microsoft ::
 Windows Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `pypalex-1.3.3/README.md` & `pypalex-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pypalex-1.3.3/pypalex/Extractor.py` & `pypalex-1.3.4/pypalex/Extractor.py`

 * *Files identical despite different names*

### Comparing `pypalex-1.3.3/pypalex/__init__.py` & `pypalex-1.3.4/pypalex/__init__.py`

 * *Files identical despite different names*

### Comparing `pypalex-1.3.3/pypalex/__main__.py` & `pypalex-1.3.4/pypalex/__main__.py`

 * *Files identical despite different names*

### Comparing `pypalex-1.3.3/pypalex/arg_messages.py` & `pypalex-1.3.4/pypalex/arg_messages.py`

 * *Files identical despite different names*

### Comparing `pypalex-1.3.3/pypalex/constants.py` & `pypalex-1.3.4/pypalex/constants.py`

 * *Files identical despite different names*

### Comparing `pypalex-1.3.3/pypalex/conversion_utils.py` & `pypalex-1.3.4/pypalex/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `pypalex-1.3.3/pypalex/extraction_utils.py` & `pypalex-1.3.4/pypalex/extraction_utils.py`

 * *Files identical despite different names*

### Comparing `pypalex-1.3.3/pypalex/file_utils.py` & `pypalex-1.3.4/pypalex/file_utils.py`

 * *Files identical despite different names*

### Comparing `pypalex-1.3.3/pypalex/image_utils.py` & `pypalex-1.3.4/pypalex/image_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #   @brief  Utilities for processing image and file handling.
 #
 #   @section authors Author(s)
 #   - Created by Al Timofeyev on February 27, 2022.
 #   - Modified by Al Timofeyev on April 21, 2022.
 #   - Modified by Al Timofeyev on March 6, 2023.
 #   - Modified by Al Timofeyev on April 5, 2023.
+#   - Modified by Al Timofeyev on May 16, 2024.
 
 
 # ---- IMPORTS ----
 import numpy
 import multiprocessing
 from PIL import Image
 from . import conversion_utils as convert
@@ -54,39 +55,49 @@
 
     return hsv_matrix_2d
 
 
 # **************************************************************************
 # **************************************************************************
 
-##  Rescales image to a smaller sampling size.
+##  Rescales image to a smaller sampling size while maintaining aspect ration.
+#
+#   @note   The math behind rescaling the image came
+#           from: https://math.stackexchange.com/a/3078131
 #
 #   @param  image   PIL Image object.
 #
 #   @return Tuple of the new width and height of image.
 def rescale_image(image):
     width, height = image.size
     default_480p = [854, 480]   # 480p SD resolution with 16:9 ratio.
     default_360p = [640, 360]   # 360p SD resolution with 16:9 ratio.
 
-    # Try scaling images down to 480p with 16:9 ratio.
-    if height < width:      # ---- Landscape, 16:9 ratio.
-        percent_change_width = default_480p[0] / width
-        percent_change_height = default_480p[1] / height
-    elif width < height:    # ---- Portrait, 9:16 ratio.
-        percent_change_width = default_480p[1] / width
-        percent_change_height = default_480p[0] / height
-    else:                   # ---- Square, 1:1 ratio.
-        percent_change_width = default_360p[0] / width
-        percent_change_height = default_360p[0] / height
-
-    width *= percent_change_width
-    height *= percent_change_height
+    # Try scaling images down to 480p.
+    # new_width = (width/height) * new_height
+    # new_height = (height/width) * new_width
+    if height < width:  # ---- Landscape.
+        new_width = default_480p[0]
+        new_height = round((height / width) * new_width)
+
+        if new_height > default_480p[1]:
+            new_height = default_480p[1]
+            new_width = round((width / height) * new_height)
+    elif width < height:  # ---- Portrait.
+        new_height = default_480p[0]
+        new_width = round((width / height) * new_height)
+
+        if new_width > default_480p[1]:
+            new_width = default_480p[1]
+            new_height = round((height / width) * new_width)
+    else:  # ---- Square, 1:1 ratio.
+        new_width = default_360p[0]
+        new_height = round((width / height) * new_width)
 
-    return round(width), round(height)
+    return round(new_width), round(new_height)
 
 
 # --------------------------------------------------------------------------
 # --------------------------------------------------------------------------
 
 ##  Helper function for multiprocessing conversion operations.
 #   @details    Helps convert from [r,g,b] to [h,s,v].
```

### Comparing `pypalex-1.3.3/pypalex/print_utils.py` & `pypalex-1.3.4/pypalex/print_utils.py`

 * *Files identical despite different names*

### Comparing `pypalex-1.3.3/pypalex/settings.py` & `pypalex-1.3.4/pypalex/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 #   @section authors Author(s)
 #   - Created by Al Timofeyev on March 2, 2022
 #   - Modified by Al Timofeyev on April 21, 2022.
 #   - Modified by Al Timofeyev on March 11, 2023.
 #   - Modified by Al Timofeyev on March 22, 2023.
 #   - Modified by Al Timofeyev on March 26, 2023.
 #   - Modified by Al Timofeyev on April 7, 2023.
+#   - Modified by Al Timofeyev on May 16, 2024.
 
 
 import os
 import platform
 
-__version__ = "1.3.3"
+__version__ = "1.3.4"
 __cache_version__ = "1.0.0"
 
 HOME = os.getenv("HOME", os.getenv("USERPROFILE"))
 XDG_CACHE_DIR = os.getenv("XDG_CACHE_HOME", os.path.join(HOME, ".cache"))
 XDG_CONF_DIR = os.getenv("XDG_CONFIG_HOME", os.path.join(HOME, ".config"))
 
 # NOTE: CONF_DIR will just be the place where PyPalEx saves color palettes
```

### Comparing `pypalex-1.3.3/pypalex.egg-info/PKG-INFO` & `pypalex-1.3.4/pypalex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pypalex
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python Palette Extractor: extracts color palettes from images into json files.
 Home-page: https://github.com/AlTimofeyev/pypalex
 Author: Al Timofeyev
 Author-email: al.timofeyev@outlook.com
 License: MIT
-Download-URL: https://github.com/AlTimofeyev/pypalex/archive/1.3.3.tar.gz
+Download-URL: https://github.com/AlTimofeyev/pypalex/archive/1.3.4.tar.gz
 Keywords: python,pypalex,palex,color-palette,colorscheme,extract-colorscheme,extract-palette,extractor
 Platform: UNKNOWN
 Classifier: Environment :: X11 Applications
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: pypalex Version: 1.3.3 Summary: Python Palette
+Metadata-Version: 2.1 Name: pypalex Version: 1.3.4 Summary: Python Palette
 Extractor: extracts color palettes from images into json files. Home-page:
 https://github.com/AlTimofeyev/pypalex Author: Al Timofeyev Author-email:
 al.timofeyev@outlook.com License: MIT Download-URL: https://github.com/
-AlTimofeyev/pypalex/archive/1.3.3.tar.gz Keywords: python,pypalex,palex,color-
+AlTimofeyev/pypalex/archive/1.3.4.tar.gz Keywords: python,pypalex,palex,color-
 palette,colorscheme,extract-colorscheme,extract-palette,extractor Platform:
 UNKNOWN Classifier: Environment :: X11 Applications Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: MacOS Classifier:
 Operating System :: POSIX :: Linux Classifier: Operating System :: Microsoft ::
 Windows Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `pypalex-1.3.3/setup.py` & `pypalex-1.3.4/setup.py`

 * *Files identical despite different names*

