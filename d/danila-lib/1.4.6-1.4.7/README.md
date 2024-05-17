# Comparing `tmp/danila-lib-1.4.6.tar.gz` & `tmp/danila-lib-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danila-lib-1.4.6.tar", last modified: Fri May 17 05:46:23 2024, max compression
+gzip compressed data, was "danila-lib-1.4.7.tar", last modified: Fri May 17 05:59:28 2024, max compression
```

## Comparing `danila-lib-1.4.6.tar` & `danila-lib-1.4.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 05:46:23.846000 danila-lib-1.4.6/
--rw-rw-rw-   0        0        0     9615 2024-05-17 05:46:23.846000 danila-lib-1.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.4.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 05:46:23.735494 danila-lib-1.4.6/danila/
--rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.4.6/danila/__init__.py
--rw-rw-rw-   0        0        0     2004 2024-05-14 12:46:28.000000 danila-lib-1.4.6/danila/danila.py
--rw-rw-rw-   0        0        0     9777 2024-05-14 12:46:28.000000 danila-lib-1.4.6/danila/danila_v1.py
--rw-rw-rw-   0        0        0    10195 2024-05-14 12:46:28.000000 danila-lib-1.4.6/danila/danila_v2.py
--rw-rw-rw-   0        0        0    10693 2024-05-14 12:37:43.000000 danila-lib-1.4.6/danila/danila_v3.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:46:23.751423 danila-lib-1.4.6/danila_lib.egg-info/
--rw-rw-rw-   0        0        0     9615 2024-05-17 05:46:23.000000 danila-lib-1.4.6/danila_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      920 2024-05-17 05:46:23.000000 danila-lib-1.4.6/danila_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 05:46:23.000000 danila-lib-1.4.6/danila_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1879 2024-05-17 05:46:23.000000 danila-lib-1.4.6/danila_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-17 05:46:23.000000 danila-lib-1.4.6/danila_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-17 05:46:23.752418 danila-lib-1.4.6/data/
--rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.4.6/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:46:23.800205 danila-lib-1.4.6/data/neuro/
--rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.4.6/data/neuro/Letters_recognize.py
--rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.4.6/data/neuro/Rama_classify_class.py
--rw-rw-rw-   0        0        0     2121 2024-04-22 11:59:10.000000 danila-lib-1.4.6/data/neuro/Rama_detect_class.py
--rw-rw-rw-   0        0        0     2614 2024-05-14 12:37:43.000000 danila-lib-1.4.6/data/neuro/Rama_prod_classify_class.py
--rw-rw-rw-   0        0        0     3159 2024-04-22 19:35:07.000000 danila-lib-1.4.6/data/neuro/Text_detect_class.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.4.6/data/neuro/__init__.py
--rw-rw-rw-   0        0        0     6373 2024-05-06 15:05:03.000000 danila-lib-1.4.6/data/neuro/letters_in_image.py
--rw-rw-rw-   0        0        0      910 2024-05-17 05:45:50.000000 danila-lib-1.4.6/data/neuro/models.py
--rw-rw-rw-   0        0        0     2975 2024-05-14 11:04:15.000000 danila-lib-1.4.6/data/neuro/objs_in_image.py
--rw-rw-rw-   0        0        0     4337 2024-05-07 07:39:22.000000 danila-lib-1.4.6/data/neuro/text_recognize_yolo.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:46:23.845004 danila-lib-1.4.6/data/result/
--rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.4.6/data/result/Class_im.py
--rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.4.6/data/result/Class_text.py
--rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.4.6/data/result/Image_text_areas.py
--rw-rw-rw-   0        0        0      311 2024-04-22 18:52:56.000000 danila-lib-1.4.6/data/result/Label_area.py
--rw-rw-rw-   0        0        0      105 2024-05-14 11:34:55.000000 danila-lib-1.4.6/data/result/Rama_prod.py
--rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.4.6/data/result/Rect.py
--rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.4.6/data/result/Text_area.py
--rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.4.6/data/result/Yolo_label_rect.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.4.6/data/result/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.4.6/data/result/prod_classify_result.py
--rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.4.6/data/result/word_compare_result.py
--rw-rw-rw-   0        0        0       42 2024-05-17 05:46:23.849981 danila-lib-1.4.6/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-05-17 05:46:21.000000 danila-lib-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 05:59:28.666083 danila-lib-1.4.7/
+-rw-rw-rw-   0        0        0     9615 2024-05-17 05:59:28.666083 danila-lib-1.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.4.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 05:59:28.587977 danila-lib-1.4.7/danila/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.4.7/danila/__init__.py
+-rw-rw-rw-   0        0        0     2004 2024-05-14 12:46:28.000000 danila-lib-1.4.7/danila/danila.py
+-rw-rw-rw-   0        0        0     9777 2024-05-14 12:46:28.000000 danila-lib-1.4.7/danila/danila_v1.py
+-rw-rw-rw-   0        0        0    10195 2024-05-14 12:46:28.000000 danila-lib-1.4.7/danila/danila_v2.py
+-rw-rw-rw-   0        0        0    10693 2024-05-14 12:37:43.000000 danila-lib-1.4.7/danila/danila_v3.py
+drwxrwxrwx   0        0        0        0 2024-05-17 05:59:28.603598 danila-lib-1.4.7/danila_lib.egg-info/
+-rw-rw-rw-   0        0        0     9615 2024-05-17 05:59:28.000000 danila-lib-1.4.7/danila_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      920 2024-05-17 05:59:28.000000 danila-lib-1.4.7/danila_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 05:59:28.000000 danila-lib-1.4.7/danila_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1879 2024-05-17 05:59:28.000000 danila-lib-1.4.7/danila_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-17 05:59:28.000000 danila-lib-1.4.7/danila_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 05:59:28.603598 danila-lib-1.4.7/data/
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.4.7/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 05:59:28.666083 danila-lib-1.4.7/data/neuro/
+-rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.4.7/data/neuro/Letters_recognize.py
+-rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.4.7/data/neuro/Rama_classify_class.py
+-rw-rw-rw-   0        0        0     2121 2024-04-22 11:59:10.000000 danila-lib-1.4.7/data/neuro/Rama_detect_class.py
+-rw-rw-rw-   0        0        0     2614 2024-05-14 12:37:43.000000 danila-lib-1.4.7/data/neuro/Rama_prod_classify_class.py
+-rw-rw-rw-   0        0        0     3159 2024-04-22 19:35:07.000000 danila-lib-1.4.7/data/neuro/Text_detect_class.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.4.7/data/neuro/__init__.py
+-rw-rw-rw-   0        0        0     6373 2024-05-06 15:05:03.000000 danila-lib-1.4.7/data/neuro/letters_in_image.py
+-rw-rw-rw-   0        0        0      830 2024-05-17 05:59:17.000000 danila-lib-1.4.7/data/neuro/models.py
+-rw-rw-rw-   0        0        0     2975 2024-05-14 11:04:15.000000 danila-lib-1.4.7/data/neuro/objs_in_image.py
+-rw-rw-rw-   0        0        0     4337 2024-05-07 07:39:22.000000 danila-lib-1.4.7/data/neuro/text_recognize_yolo.py
+drwxrwxrwx   0        0        0        0 2024-05-17 05:59:28.666083 danila-lib-1.4.7/data/result/
+-rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.4.7/data/result/Class_im.py
+-rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.4.7/data/result/Class_text.py
+-rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.4.7/data/result/Image_text_areas.py
+-rw-rw-rw-   0        0        0      311 2024-04-22 18:52:56.000000 danila-lib-1.4.7/data/result/Label_area.py
+-rw-rw-rw-   0        0        0      105 2024-05-14 11:34:55.000000 danila-lib-1.4.7/data/result/Rama_prod.py
+-rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.4.7/data/result/Rect.py
+-rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.4.7/data/result/Text_area.py
+-rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.4.7/data/result/Yolo_label_rect.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.4.7/data/result/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.4.7/data/result/prod_classify_result.py
+-rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.4.7/data/result/word_compare_result.py
+-rw-rw-rw-   0        0        0       42 2024-05-17 05:59:28.681704 danila-lib-1.4.7/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-05-17 05:59:17.000000 danila-lib-1.4.7/setup.py
```

### Comparing `danila-lib-1.4.6/PKG-INFO` & `danila-lib-1.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.4.6
+Version: 1.4.7
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.4.6/README.md` & `danila-lib-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.6/danila/danila.py` & `danila-lib-1.4.7/danila/danila.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.6/danila/danila_v1.py` & `danila-lib-1.4.7/danila/danila_v1.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.6/danila/danila_v2.py` & `danila-lib-1.4.7/danila/danila_v2.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.6/danila/danila_v3.py` & `danila-lib-1.4.7/danila/danila_v3.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.6/danila_lib.egg-info/PKG-INFO` & `danila-lib-1.4.7/danila_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.4.6
+Version: 1.4.7
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.4.6/danila_lib.egg-info/SOURCES.txt` & `danila-lib-1.4.7/danila_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.6/danila_lib.egg-info/requires.txt` & `danila-lib-1.4.7/danila_lib.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.6/data/neuro/Letters_recognize.py` & `danila-lib-1.4.7/data/neuro/Letters_recognize.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.6/data/neuro/Rama_classify_class.py` & `danila-lib-1.4.7/data/neuro/Rama_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.6/data/neuro/Rama_detect_class.py` & `danila-lib-1.4.7/data/neuro/Rama_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.6/data/neuro/Rama_prod_classify_class.py` & `danila-lib-1.4.7/data/neuro/Rama_prod_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.6/data/neuro/Text_detect_class.py` & `danila-lib-1.4.7/data/neuro/Text_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.6/data/neuro/letters_in_image.py` & `danila-lib-1.4.7/data/neuro/letters_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.6/data/neuro/models.py` & `danila-lib-1.4.7/data/neuro/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,9 +3,8 @@
 RAMA_SPRING_DETECT_MODEL_ADDRESS = 'https://disk.yandex.ru/d/zAEw0_ALgtBg9Q'
 RAMA_SPRING_RUZHIMMASH_TEXT_DETECT_MODEL_ADDRESS = 'https://disk.yandex.ru/d/b4vCbEzg3t3mTg'
 RAMA_NO_SPRING_BEJICKAYA_TEXT_DETECT_MODEL_ADDRESS = 'https://disk.yandex.ru/d/ZbbcscTS2Han1A'
 LETTERS_RECOGNIZE = 'https://disk.yandex.ru/d/ooaMrpqxl_egoA'
 RAMA_NO_SPRING_RUZHIMMASH_TEXT_DETECT_MODEL_ADDRESS = 'https://disk.yandex.ru/d/b4vCbEzg3t3mTg'
 RAMA_SPRING_BEJICKAYA_TEXT_DETECT_MODEL_ADDRESS = 'https://disk.yandex.ru/d/ZbbcscTS2Han1A'
 TEXT_RECOGNIZE_YOLO_MODEL_ADDRESS = 'https://disk.yandex.ru/d/HN5Cs2zffXipIg'
-# RAMA_PROD_CLASSIFY_MODEL_ADDRESS = 'https://disk.yandex.ru/d/iV7PHQcN-c2G-Q'
 RAMA_PROD_CLASSIFY_MODEL_ADDRESS = 'https://disk.yandex.ru/d/i66NFBasb6AbbA'
```

### Comparing `danila-lib-1.4.6/data/neuro/objs_in_image.py` & `danila-lib-1.4.7/data/neuro/objs_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.6/data/neuro/text_recognize_yolo.py` & `danila-lib-1.4.7/data/neuro/text_recognize_yolo.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.6/data/result/Image_text_areas.py` & `danila-lib-1.4.7/data/result/Image_text_areas.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.6/data/result/Rect.py` & `danila-lib-1.4.7/data/result/Rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.6/data/result/Text_area.py` & `danila-lib-1.4.7/data/result/Text_area.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.6/data/result/Yolo_label_rect.py` & `danila-lib-1.4.7/data/result/Yolo_label_rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.6/setup.py` & `danila-lib-1.4.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   with open('requirements.txt', 'r') as f:
     a = f.read()
   b = a.split()
   return b
 
 setup(
   name='danila-lib',
-  version='1.4.6',
+  version='1.4.7',
   author='arseniy_zhuck',
   author_email='arseniyzhuck@mail.ru',
   description='This is the module for detecting and classifying text on rama pictures',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Arseniy-Zhuck/danila_lib',
   packages=find_packages(),
```

