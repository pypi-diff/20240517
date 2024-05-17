# Comparing `tmp/HelloPyOnly-0.1.25.tar.gz` & `tmp/HelloPyOnly-0.1.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HelloPyOnly-0.1.25.tar", last modified: Thu May  9 03:39:36 2024, max compression
+gzip compressed data, was "HelloPyOnly-0.1.26.tar", last modified: Fri May 17 14:14:17 2024, max compression
```

## Comparing `HelloPyOnly-0.1.25.tar` & `HelloPyOnly-0.1.26.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 03:39:36.363448 HelloPyOnly-0.1.25/
-drwxrwxrwx   0        0        0        0 2024-05-09 03:39:36.350428 HelloPyOnly-0.1.25/HelloPyOnly.egg-info/
--rw-rw-rw-   0        0        0      553 2024-05-09 03:39:36.000000 HelloPyOnly-0.1.25/HelloPyOnly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      831 2024-05-09 03:39:36.000000 HelloPyOnly-0.1.25/HelloPyOnly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 03:39:36.000000 HelloPyOnly-0.1.25/HelloPyOnly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-09 03:39:36.000000 HelloPyOnly-0.1.25/HelloPyOnly.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-09 03:39:36.000000 HelloPyOnly-0.1.25/HelloPyOnly.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      553 2024-05-09 03:39:36.363448 HelloPyOnly-0.1.25/PKG-INFO
--rw-rw-rw-   0        0        0       89 2024-05-04 08:02:44.000000 HelloPyOnly-0.1.25/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 03:39:36.355419 HelloPyOnly-0.1.25/hellopy/
--rw-rw-rw-   0        0        0     2069 2024-05-09 01:42:22.000000 HelloPyOnly-0.1.25/hellopy/__init__.py
--rw-rw-rw-   0        0        0     4597 2023-10-20 05:46:44.000000 HelloPyOnly-0.1.25/hellopy/collision.py
--rw-rw-rw-   0        0        0     2773 2023-10-17 14:39:56.000000 HelloPyOnly-0.1.25/hellopy/events.py
-drwxrwxrwx   0        0        0        0 2024-05-09 03:39:36.360994 HelloPyOnly-0.1.25/hellopy/gameobject/
--rw-rw-rw-   0        0        0      389 2023-10-18 06:44:19.000000 HelloPyOnly-0.1.25/hellopy/gameobject/__init__.py
--rw-rw-rw-   0        0        0     2051 2023-10-17 08:13:10.000000 HelloPyOnly-0.1.25/hellopy/gameobject/circle.py
--rw-rw-rw-   0        0        0      220 2023-10-17 06:43:33.000000 HelloPyOnly-0.1.25/hellopy/gameobject/ellipse.py
--rw-rw-rw-   0        0        0      384 2023-10-16 07:28:41.000000 HelloPyOnly-0.1.25/hellopy/gameobject/gameobject.py
--rw-rw-rw-   0        0        0     2467 2023-10-17 06:43:38.000000 HelloPyOnly-0.1.25/hellopy/gameobject/line.py
--rw-rw-rw-   0        0        0     3676 2023-12-28 02:51:59.000000 HelloPyOnly-0.1.25/hellopy/gameobject/polygon.py
--rw-rw-rw-   0        0        0      545 2023-10-19 01:46:38.000000 HelloPyOnly-0.1.25/hellopy/gameobject/rectangle.py
--rw-rw-rw-   0        0        0    10478 2024-04-06 00:45:00.000000 HelloPyOnly-0.1.25/hellopy/gameobject/sprite.py
--rw-rw-rw-   0        0        0        0 2024-04-06 00:29:09.000000 HelloPyOnly-0.1.25/hellopy/gameobject/test.py
--rw-rw-rw-   0        0        0     2777 2024-01-06 08:20:48.000000 HelloPyOnly-0.1.25/hellopy/gameobject/text.py
--rw-rw-rw-   0        0        0      649 2023-12-27 01:58:30.000000 HelloPyOnly-0.1.25/hellopy/gameobject/triangle.py
--rw-rw-rw-   0        0        0      258 2023-10-17 06:30:34.000000 HelloPyOnly-0.1.25/hellopy/key.py
--rw-rw-rw-   0        0        0      136 2023-10-16 05:53:09.000000 HelloPyOnly-0.1.25/hellopy/mouse.py
-drwxrwxrwx   0        0        0        0 2024-05-09 03:39:36.362002 HelloPyOnly-0.1.25/hellopy/onlydemos/
--rw-rw-rw-   0        0        0     5660 2024-05-09 03:28:43.000000 HelloPyOnly-0.1.25/hellopy/onlydemos/LoongPy.py
--rw-rw-rw-   0        0        0     1848 2024-05-09 01:41:06.000000 HelloPyOnly-0.1.25/hellopy/onlydemos/__init__.py
--rw-rw-rw-   0        0        0      253 2024-05-09 01:50:51.000000 HelloPyOnly-0.1.25/hellopy/onlydemos/christmas.py
--rw-rw-rw-   0        0        0     1882 2023-10-20 05:46:53.000000 HelloPyOnly-0.1.25/hellopy/resource.py
--rw-rw-rw-   0        0        0      388 2023-10-18 06:58:07.000000 HelloPyOnly-0.1.25/hellopy/sound.py
--rw-rw-rw-   0        0        0      341 2023-10-17 06:42:53.000000 HelloPyOnly-0.1.25/hellopy/util.py
--rw-rw-rw-   0        0        0     3263 2024-05-08 07:49:07.000000 HelloPyOnly-0.1.25/hellopy/window.py
-drwxrwxrwx   0        0        0        0 2024-05-09 03:39:36.363448 HelloPyOnly-0.1.25/onlyshow/
--rw-rw-rw-   0        0        0     5973 2024-05-09 03:29:46.000000 HelloPyOnly-0.1.25/onlyshow/LoongPy.py
--rw-rw-rw-   0        0        0     1828 2024-05-09 03:28:35.000000 HelloPyOnly-0.1.25/onlyshow/__init__.py
--rw-rw-rw-   0        0        0     4352 2023-10-20 07:23:57.000000 HelloPyOnly-0.1.25/onlyshow/pumpkin.py
--rw-rw-rw-   0        0        0       42 2024-05-09 03:39:36.364467 HelloPyOnly-0.1.25/setup.cfg
--rw-rw-rw-   0        0        0     1057 2024-05-09 03:39:28.000000 HelloPyOnly-0.1.25/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 14:14:17.601176 HelloPyOnly-0.1.26/
+drwxrwxrwx   0        0        0        0 2024-05-17 14:14:17.583990 HelloPyOnly-0.1.26/HelloPyOnly.egg-info/
+-rw-rw-rw-   0        0        0      553 2024-05-17 14:14:17.000000 HelloPyOnly-0.1.26/HelloPyOnly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      831 2024-05-17 14:14:17.000000 HelloPyOnly-0.1.26/HelloPyOnly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 14:14:17.000000 HelloPyOnly-0.1.26/HelloPyOnly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-17 14:14:17.000000 HelloPyOnly-0.1.26/HelloPyOnly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-17 14:14:17.000000 HelloPyOnly-0.1.26/HelloPyOnly.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      553 2024-05-17 14:14:17.601176 HelloPyOnly-0.1.26/PKG-INFO
+-rw-rw-rw-   0        0        0       89 2024-05-04 08:02:44.000000 HelloPyOnly-0.1.26/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 14:14:17.590693 HelloPyOnly-0.1.26/hellopy/
+-rw-rw-rw-   0        0        0     2069 2024-05-09 01:42:22.000000 HelloPyOnly-0.1.26/hellopy/__init__.py
+-rw-rw-rw-   0        0        0     4597 2023-10-20 05:46:44.000000 HelloPyOnly-0.1.26/hellopy/collision.py
+-rw-rw-rw-   0        0        0     2773 2023-10-17 14:39:56.000000 HelloPyOnly-0.1.26/hellopy/events.py
+drwxrwxrwx   0        0        0        0 2024-05-17 14:14:17.597892 HelloPyOnly-0.1.26/hellopy/gameobject/
+-rw-rw-rw-   0        0        0      389 2023-10-18 06:44:19.000000 HelloPyOnly-0.1.26/hellopy/gameobject/__init__.py
+-rw-rw-rw-   0        0        0     2051 2023-10-17 08:13:10.000000 HelloPyOnly-0.1.26/hellopy/gameobject/circle.py
+-rw-rw-rw-   0        0        0      220 2023-10-17 06:43:33.000000 HelloPyOnly-0.1.26/hellopy/gameobject/ellipse.py
+-rw-rw-rw-   0        0        0      384 2023-10-16 07:28:41.000000 HelloPyOnly-0.1.26/hellopy/gameobject/gameobject.py
+-rw-rw-rw-   0        0        0     2467 2023-10-17 06:43:38.000000 HelloPyOnly-0.1.26/hellopy/gameobject/line.py
+-rw-rw-rw-   0        0        0     3676 2023-12-28 02:51:59.000000 HelloPyOnly-0.1.26/hellopy/gameobject/polygon.py
+-rw-rw-rw-   0        0        0      545 2023-10-19 01:46:38.000000 HelloPyOnly-0.1.26/hellopy/gameobject/rectangle.py
+-rw-rw-rw-   0        0        0    10478 2024-04-06 00:45:00.000000 HelloPyOnly-0.1.26/hellopy/gameobject/sprite.py
+-rw-rw-rw-   0        0        0        0 2024-04-06 00:29:09.000000 HelloPyOnly-0.1.26/hellopy/gameobject/test.py
+-rw-rw-rw-   0        0        0     2777 2024-01-06 08:20:48.000000 HelloPyOnly-0.1.26/hellopy/gameobject/text.py
+-rw-rw-rw-   0        0        0      649 2023-12-27 01:58:30.000000 HelloPyOnly-0.1.26/hellopy/gameobject/triangle.py
+-rw-rw-rw-   0        0        0      258 2023-10-17 06:30:34.000000 HelloPyOnly-0.1.26/hellopy/key.py
+-rw-rw-rw-   0        0        0      136 2023-10-16 05:53:09.000000 HelloPyOnly-0.1.26/hellopy/mouse.py
+drwxrwxrwx   0        0        0        0 2024-05-17 14:14:17.598892 HelloPyOnly-0.1.26/hellopy/onlydemos/
+-rw-rw-rw-   0        0        0     5660 2024-05-09 03:28:43.000000 HelloPyOnly-0.1.26/hellopy/onlydemos/LoongPy.py
+-rw-rw-rw-   0        0        0     1848 2024-05-09 01:41:06.000000 HelloPyOnly-0.1.26/hellopy/onlydemos/__init__.py
+-rw-rw-rw-   0        0        0      253 2024-05-09 01:50:51.000000 HelloPyOnly-0.1.26/hellopy/onlydemos/christmas.py
+-rw-rw-rw-   0        0        0     1882 2023-10-20 05:46:53.000000 HelloPyOnly-0.1.26/hellopy/resource.py
+-rw-rw-rw-   0        0        0      388 2023-10-18 06:58:07.000000 HelloPyOnly-0.1.26/hellopy/sound.py
+-rw-rw-rw-   0        0        0      341 2023-10-17 06:42:53.000000 HelloPyOnly-0.1.26/hellopy/util.py
+-rw-rw-rw-   0        0        0     3263 2024-05-08 07:49:07.000000 HelloPyOnly-0.1.26/hellopy/window.py
+drwxrwxrwx   0        0        0        0 2024-05-17 14:14:17.600042 HelloPyOnly-0.1.26/onlyshow/
+-rw-rw-rw-   0        0        0     5973 2024-05-09 03:29:46.000000 HelloPyOnly-0.1.26/onlyshow/LoongPy.py
+-rw-rw-rw-   0        0        0     1828 2024-05-09 03:28:35.000000 HelloPyOnly-0.1.26/onlyshow/__init__.py
+-rw-rw-rw-   0        0        0     4356 2024-05-17 14:10:25.000000 HelloPyOnly-0.1.26/onlyshow/pumpkin.py
+-rw-rw-rw-   0        0        0       42 2024-05-17 14:14:17.601176 HelloPyOnly-0.1.26/setup.cfg
+-rw-rw-rw-   0        0        0     1057 2024-05-17 14:11:56.000000 HelloPyOnly-0.1.26/setup.py
```

### Comparing `HelloPyOnly-0.1.25/HelloPyOnly.egg-info/PKG-INFO` & `HelloPyOnly-0.1.26/HelloPyOnly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HelloPyOnly
-Version: 0.1.25
+Version: 0.1.26
 Summary: This is the game engine of Only Hello Science project.
 Home-page: https://github.com/zfan0311/hellopy.git
 Author: funk.zhang
 Author-email: zhangfangid@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `HelloPyOnly-0.1.25/HelloPyOnly.egg-info/SOURCES.txt` & `HelloPyOnly-0.1.26/HelloPyOnly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.25/PKG-INFO` & `HelloPyOnly-0.1.26/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HelloPyOnly
-Version: 0.1.25
+Version: 0.1.26
 Summary: This is the game engine of Only Hello Science project.
 Home-page: https://github.com/zfan0311/hellopy.git
 Author: funk.zhang
 Author-email: zhangfangid@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `HelloPyOnly-0.1.25/hellopy/__init__.py` & `HelloPyOnly-0.1.26/hellopy/__init__.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.25/hellopy/collision.py` & `HelloPyOnly-0.1.26/hellopy/collision.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.25/hellopy/events.py` & `HelloPyOnly-0.1.26/hellopy/events.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.25/hellopy/gameobject/circle.py` & `HelloPyOnly-0.1.26/hellopy/gameobject/circle.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.25/hellopy/gameobject/line.py` & `HelloPyOnly-0.1.26/hellopy/gameobject/line.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.25/hellopy/gameobject/polygon.py` & `HelloPyOnly-0.1.26/hellopy/gameobject/polygon.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.25/hellopy/gameobject/rectangle.py` & `HelloPyOnly-0.1.26/hellopy/gameobject/rectangle.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.25/hellopy/gameobject/sprite.py` & `HelloPyOnly-0.1.26/hellopy/gameobject/sprite.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.25/hellopy/gameobject/text.py` & `HelloPyOnly-0.1.26/hellopy/gameobject/text.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.25/hellopy/gameobject/triangle.py` & `HelloPyOnly-0.1.26/hellopy/gameobject/triangle.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.25/hellopy/onlydemos/LoongPy.py` & `HelloPyOnly-0.1.26/hellopy/onlydemos/LoongPy.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.25/hellopy/onlydemos/__init__.py` & `HelloPyOnly-0.1.26/hellopy/onlydemos/__init__.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.25/hellopy/resource.py` & `HelloPyOnly-0.1.26/hellopy/resource.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.25/hellopy/window.py` & `HelloPyOnly-0.1.26/hellopy/window.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.25/onlyshow/LoongPy.py` & `HelloPyOnly-0.1.26/onlyshow/LoongPy.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.25/onlyshow/__init__.py` & `HelloPyOnly-0.1.26/onlyshow/__init__.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.25/onlyshow/pumpkin.py` & `HelloPyOnly-0.1.26/onlyshow/pumpkin.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,21 +135,21 @@
         self.face.y = y
         self.left_eye.y = y + self._v2le[1]
         self.right_eye.y = y + self._v2re[1]
         self.mouth.y = y + self._v2m[1]
     
     def rotate_to(self, angle, r_center=None):
         rc = r_center or (self.x, self.y)
-        self.face.rotate_to(angle, rc)
+        self.face.rotate_to(-angle, rc)
         if self.left_eye:
-            self.left_eye.rotate_to(angle, rc)
+            self.left_eye.rotate_to(-angle, rc)
         if self.right_eye:
-            self.right_eye.rotate_to(angle, rc)
+            self.right_eye.rotate_to(-angle, rc)
         if self.mouth:
-            self.mouth.rotate_to(angle, rc)
+            self.mouth.rotate_to(-angle, rc)
     
     def draw(self):
         self.face.draw()
         self.left_eye.draw()
         self.right_eye.draw()
         self.mouth.draw()
```

### Comparing `HelloPyOnly-0.1.25/setup.py` & `HelloPyOnly-0.1.26/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='HelloPyOnly',  # 您的库的名称
-    version='0.1.25',  # 版本号
+    version='0.1.26',  # 版本号
     author='funk.zhang',  # 您的名字
     author_email='zhangfangid@126.com',  # 您的电子邮件地址
     description='This is the game engine of Only Hello Science project.',  # 您库的简短描述
     long_description='This is the game engine of Only Hello Science project. Based on pygame.',  # 更详细的描述
     # long_description_content_type='text/markdown',  # 描述类型（通常为Markdown）
     url='https://github.com/zfan0311/hellopy.git',  # 您库的代码托管URL
     packages=find_packages(),  # 包含的Python包
```

