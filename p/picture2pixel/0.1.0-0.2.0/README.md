# Comparing `tmp/picture2pixel-0.1.0.tar.gz` & `tmp/picture2pixel-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picture2pixel-0.1.0.tar", last modified: Thu May 16 18:04:11 2024, max compression
+gzip compressed data, was "picture2pixel-0.2.0.tar", last modified: Fri May 17 19:54:52 2024, max compression
```

## Comparing `picture2pixel-0.1.0.tar` & `picture2pixel-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 18:04:11.398419 picture2pixel-0.1.0/
--rw-rw-rw-   0        0        0     1297 2024-05-16 18:04:11.397419 picture2pixel-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      510 2024-05-16 16:54:22.000000 picture2pixel-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 18:04:11.383419 picture2pixel-0.1.0/picture2pixel/
--rw-rw-rw-   0        0        0      132 2024-05-16 16:35:45.000000 picture2pixel-0.1.0/picture2pixel/__init__.py
--rw-rw-rw-   0        0        0     2095 2024-05-16 16:36:00.000000 picture2pixel-0.1.0/picture2pixel/image_processing.py
--rw-rw-rw-   0        0        0     1085 2024-05-16 16:49:37.000000 picture2pixel-0.1.0/picture2pixel/main.py
--rw-rw-rw-   0        0        0     2851 2024-05-16 16:39:07.000000 picture2pixel-0.1.0/picture2pixel/verilog_generator.py
-drwxrwxrwx   0        0        0        0 2024-05-16 18:04:11.396418 picture2pixel-0.1.0/picture2pixel.egg-info/
--rw-rw-rw-   0        0        0     1297 2024-05-16 18:04:11.000000 picture2pixel-0.1.0/picture2pixel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2024-05-16 18:04:11.000000 picture2pixel-0.1.0/picture2pixel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 18:04:11.000000 picture2pixel-0.1.0/picture2pixel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-16 18:04:11.000000 picture2pixel-0.1.0/picture2pixel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-16 18:04:11.000000 picture2pixel-0.1.0/picture2pixel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 18:04:11.399420 picture2pixel-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      991 2024-05-16 18:00:42.000000 picture2pixel-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 18:04:11.393417 picture2pixel-0.1.0/tests/
--rw-rw-rw-   0        0        0      916 2024-05-16 17:02:26.000000 picture2pixel-0.1.0/tests/test_picture2pixel.py
+drwxrwxrwx   0        0        0        0 2024-05-17 19:54:52.937959 picture2pixel-0.2.0/
+-rw-rw-rw-   0        0        0     4293 2024-05-17 19:54:52.935958 picture2pixel-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3506 2024-05-17 19:50:56.000000 picture2pixel-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 19:54:52.916959 picture2pixel-0.2.0/picture2pixel/
+-rw-rw-rw-   0        0        0      132 2024-05-16 16:35:45.000000 picture2pixel-0.2.0/picture2pixel/__init__.py
+-rw-rw-rw-   0        0        0     4731 2024-05-17 19:23:44.000000 picture2pixel-0.2.0/picture2pixel/convert2picture.py
+-rw-rw-rw-   0        0        0     1825 2024-05-17 18:18:07.000000 picture2pixel-0.2.0/picture2pixel/convert2pixel.py
+-rw-rw-rw-   0        0        0     2095 2024-05-16 16:36:00.000000 picture2pixel-0.2.0/picture2pixel/image_processing.py
+drwxrwxrwx   0        0        0        0 2024-05-17 19:54:52.932959 picture2pixel-0.2.0/picture2pixel/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-17 18:26:32.000000 picture2pixel-0.2.0/picture2pixel/tests/__init__.py
+-rw-rw-rw-   0        0        0     1409 2024-05-17 19:15:22.000000 picture2pixel-0.2.0/picture2pixel/tests/test_picture2pixel.py
+-rw-rw-rw-   0        0        0     2247 2024-05-17 19:15:39.000000 picture2pixel-0.2.0/picture2pixel/tests/test_pixel2picture.py
+-rw-rw-rw-   0        0        0     2851 2024-05-16 16:39:07.000000 picture2pixel-0.2.0/picture2pixel/verilog_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-17 19:54:52.934958 picture2pixel-0.2.0/picture2pixel.egg-info/
+-rw-rw-rw-   0        0        0     4293 2024-05-17 19:54:52.000000 picture2pixel-0.2.0/picture2pixel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      477 2024-05-17 19:54:52.000000 picture2pixel-0.2.0/picture2pixel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 19:54:52.000000 picture2pixel-0.2.0/picture2pixel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-17 19:54:52.000000 picture2pixel-0.2.0/picture2pixel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-17 19:54:52.000000 picture2pixel-0.2.0/picture2pixel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 19:54:52.937959 picture2pixel-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1066 2024-05-17 19:54:47.000000 picture2pixel-0.2.0/setup.py
```

### Comparing `picture2pixel-0.1.0/picture2pixel/image_processing.py` & `picture2pixel-0.2.0/picture2pixel/image_processing.py`

 * *Files identical despite different names*

### Comparing `picture2pixel-0.1.0/picture2pixel/verilog_generator.py` & `picture2pixel-0.2.0/picture2pixel/verilog_generator.py`

 * *Files identical despite different names*

### Comparing `picture2pixel-0.1.0/setup.py` & `picture2pixel-0.2.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from setuptools import setup, find_packages
 
+with open('README.md', encoding='utf-8') as f:
+    long_description = f.read()
+
 setup(
     name='picture2pixel',
-    version='0.1.0',
+    version='0.2.0',
     description='A package for processing images and generating Verilog code for FPGA',
-    long_description=open('README.md').read(),
+    long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://www.comp.nus.edu.sg/~guoyi/project/picture2pixel/',
     author='Chen Guoyi',
     author_email='guoyi@comp.nus.edu.sg',
     license='MIT',
     packages=find_packages(),
     install_requires=[
```

### Comparing `picture2pixel-0.1.0/tests/test_picture2pixel.py` & `picture2pixel-0.2.0/picture2pixel/tests/test_picture2pixel.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,30 @@
 import unittest
+import sys
+import os
 import numpy as np
-from picture2pixel import process_image, apply_floyd_steinberg_dithering, generate_verilog_code
+from urllib.request import urlopen
+from urllib.error import URLError
+
+# Add parent directory to PYTHONPATH
+sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
+
+from picture2pixel.convert2pixel import process_image, apply_floyd_steinberg_dithering, generate_verilog_code
 
 class TestPicture2Pixel(unittest.TestCase):
 
     def test_process_image(self):
-        reconstructed_image = process_image('https://www.comp.nus.edu.sg/~guoyi/project/picture2pixel/default.png', 96, 64, 20)
+        url = 'https://www.comp.nus.edu.sg/~guoyi/project/picture2pixel/tests/default.png'
+        try:
+            urlopen(url)
+            print(f"[ OK! ] Picture data retrieved from {url} successfully.")
+        except URLError:
+            self.fail(f"[ ERR ] Failed to retrieve picture data from {url}.")
+        
+        reconstructed_image = process_image(url, 96, 64, 20)
         self.assertEqual(reconstructed_image.shape, (64, 96, 3))
 
     def test_apply_floyd_steinberg_dithering(self):
         image = np.zeros((64, 96, 3), dtype=np.uint8)
         dithered_image = apply_floyd_steinberg_dithering(image)
         self.assertEqual(dithered_image.shape, (64, 96, 3))
```

