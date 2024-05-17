# Comparing `tmp/pychute-0.0.7.tar.gz` & `tmp/pychute-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychute-0.0.7.tar", last modified: Wed May  8 16:46:17 2024, max compression
+gzip compressed data, was "pychute-0.0.8.tar", last modified: Fri May 17 17:16:47 2024, max compression
```

## Comparing `pychute-0.0.7.tar` & `pychute-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 16:46:17.868662 pychute-0.0.7/
--rw-rw-rw-   0        0        0     1090 2024-05-07 10:43:46.000000 pychute-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     3971 2024-05-08 16:46:17.865395 pychute-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2046 2024-05-08 16:43:00.000000 pychute-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 16:46:17.840649 pychute-0.0.7/pychute/
--rw-rw-rw-   0        0        0      196 2024-05-07 16:42:55.000000 pychute-0.0.7/pychute/__init__.py
--rw-rw-rw-   0        0        0      110 2024-05-07 16:37:24.000000 pychute-0.0.7/pychute/config.py
--rw-rw-rw-   0        0        0      669 2024-05-07 10:59:12.000000 pychute-0.0.7/pychute/helpers.py
--rw-rw-rw-   0        0        0     3982 2024-05-08 16:40:03.000000 pychute-0.0.7/pychute/main.py
-drwxrwxrwx   0        0        0        0 2024-05-08 16:46:17.863539 pychute-0.0.7/pychute.egg-info/
--rw-rw-rw-   0        0        0     3971 2024-05-08 16:46:17.000000 pychute-0.0.7/pychute.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-05-08 16:46:17.000000 pychute-0.0.7/pychute.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 16:46:17.000000 pychute-0.0.7/pychute.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-08 16:46:17.000000 pychute-0.0.7/pychute.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-08 16:46:17.000000 pychute-0.0.7/pychute.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      760 2024-05-08 16:40:03.000000 pychute-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-08 16:46:17.868662 pychute-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      635 2024-05-08 16:40:03.000000 pychute-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 16:46:17.860091 pychute-0.0.7/tests/
--rw-rw-rw-   0        0        0     1252 2024-05-08 16:43:00.000000 pychute-0.0.7/tests/test_functionality.py
--rw-rw-rw-   0        0        0      915 2024-05-07 16:44:38.000000 pychute-0.0.7/tests/test_helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-17 17:16:47.587151 pychute-0.0.8/
+-rw-rw-rw-   0        0        0     1090 2024-05-07 10:43:46.000000 pychute-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     4076 2024-05-17 17:16:47.583829 pychute-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2151 2024-05-17 17:06:36.000000 pychute-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 17:16:47.561063 pychute-0.0.8/pychute/
+-rw-rw-rw-   0        0        0      196 2024-05-07 16:42:55.000000 pychute-0.0.8/pychute/__init__.py
+-rw-rw-rw-   0        0        0      110 2024-05-07 16:37:24.000000 pychute-0.0.8/pychute/config.py
+-rw-rw-rw-   0        0        0      669 2024-05-07 10:59:12.000000 pychute-0.0.8/pychute/helpers.py
+-rw-rw-rw-   0        0        0     4224 2024-05-17 17:05:05.000000 pychute-0.0.8/pychute/main.py
+drwxrwxrwx   0        0        0        0 2024-05-17 17:16:47.580530 pychute-0.0.8/pychute.egg-info/
+-rw-rw-rw-   0        0        0     4076 2024-05-17 17:16:47.000000 pychute-0.0.8/pychute.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-05-17 17:16:47.000000 pychute-0.0.8/pychute.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 17:16:47.000000 pychute-0.0.8/pychute.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-17 17:16:47.000000 pychute-0.0.8/pychute.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-17 17:16:47.000000 pychute-0.0.8/pychute.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      760 2024-05-17 17:05:05.000000 pychute-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 17:16:47.587151 pychute-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      635 2024-05-17 17:05:05.000000 pychute-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 17:16:47.580530 pychute-0.0.8/tests/
+-rw-rw-rw-   0        0        0     1281 2024-05-17 17:09:32.000000 pychute-0.0.8/tests/test_functionality.py
+-rw-rw-rw-   0        0        0      915 2024-05-07 16:44:38.000000 pychute-0.0.8/tests/test_helpers.py
```

### Comparing `pychute-0.0.7/LICENSE` & `pychute-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pychute-0.0.7/PKG-INFO` & `pychute-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychute
-Version: 0.0.7
+Version: 0.0.8
 Summary: A library that helps downloading videos from bitchute.com
 Home-page: http://github.com/paichiwo/pychute
 Author: Lukasz Zerucha
 Author-email: Lukasz Zerucha <lzerucha@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Lukasz Zerucha
@@ -35,14 +35,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: selenium
 Requires-Dist: beautifulsoup4
 
 # PyChute
 
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pychute)
+
 
 ### A library that helps download videos from BitChute website
 
 
 
 ### Installation:
 `pip install pychute`
@@ -138,10 +140,13 @@
 
 # video views
 print(pc.views())
 
 # file size in bytes
 print(pc.filesize())
 
+# description
+print(pc.description())
+
 # thumbnail image
 print(pc.thumbnail())
 ```
```

### Comparing `pychute-0.0.7/README.md` & `pychute-0.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # PyChute
 
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pychute)
+
 
 ### A library that helps download videos from BitChute website
 
 
 
 ### Installation:
 `pip install pychute`
@@ -99,10 +101,13 @@
 
 # video views
 print(pc.views())
 
 # file size in bytes
 print(pc.filesize())
 
+# description
+print(pc.description())
+
 # thumbnail image
 print(pc.thumbnail())
 ```
```

### Comparing `pychute-0.0.7/pychute/helpers.py` & `pychute-0.0.8/pychute/helpers.py`

 * *Files identical despite different names*

### Comparing `pychute-0.0.7/pychute/main.py` & `pychute-0.0.8/pychute/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,14 +90,21 @@
     def thumbnail(self) -> str:
         result = self.__soup.find('div', {'id': 'player'})
         if len(result) != 0:
             return result.find('img').get('src')
         else:
             raise Exception('Thumbnail could not be fetched')
 
+    def description(self) -> str:
+        result = self.__soup.find('div', {'class': 'teaser'}).text
+        if len(result) != 0:
+            return result
+        else:
+            raise Exception('Description could not be fetched')
+
     def download(self, on_progress_callback=None, filename=None):
         result = self.__soup.find('div', {'id': 'player'})
 
         if len(result) != 0:
             target = result.find('source').get('src')
             output_filename = f'{filename if filename else self.title()}.mp4'  # add extension
```

### Comparing `pychute-0.0.7/pychute.egg-info/PKG-INFO` & `pychute-0.0.8/pychute.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychute
-Version: 0.0.7
+Version: 0.0.8
 Summary: A library that helps downloading videos from bitchute.com
 Home-page: http://github.com/paichiwo/pychute
 Author: Lukasz Zerucha
 Author-email: Lukasz Zerucha <lzerucha@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Lukasz Zerucha
@@ -35,14 +35,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: selenium
 Requires-Dist: beautifulsoup4
 
 # PyChute
 
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pychute)
+
 
 ### A library that helps download videos from BitChute website
 
 
 
 ### Installation:
 `pip install pychute`
@@ -138,10 +140,13 @@
 
 # video views
 print(pc.views())
 
 # file size in bytes
 print(pc.filesize())
 
+# description
+print(pc.description())
+
 # thumbnail image
 print(pc.thumbnail())
 ```
```

### Comparing `pychute-0.0.7/pyproject.toml` & `pychute-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pychute"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Lukasz Zerucha", email="lzerucha@gmail.com" },
 ]
 description = "A library that helps downloading videos from bitchute.com"
 readme = "README.md"
 requires-python = ">=3.8"
 license={file="LICENSE"}
```

### Comparing `pychute-0.0.7/setup.py` & `pychute-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_desc = f.read()
 
 setup(
     name='pychute',
-    version='0.0.7',
+    version='0.0.8',
     packages=setuptools.find_packages(),
     url='http://github.com/paichiwo/pychute',
     author='Lukasz Zerucha',
     author_email='lzerucha@gmail.com',
     description='A library that helps downloading videos from bitchute.com',
     long_description=long_desc,
     long_description_content_type='text/markdown',
```

### Comparing `pychute-0.0.7/tests/test_functionality.py` & `pychute-0.0.8/tests/test_functionality.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,20 +20,21 @@
         # download speed
         elapsed_time = time.time() - start_time
         if elapsed_time > 0:
             speed = (count * block_size) / (1024 * elapsed_time)  # speed in KB/s
             print(f'Download speed: {speed:.2f} KB/s')
 
     link1 = 'https://www.bitchute.com/video/n75YV5it6lHm/'
-    link2 = 'https://www.bitchute.com/video/C8dHQCDlRlvY/'
+    link2 = 'https://www.bitchute.com/video/3Hfh7Kz7cb3A/'
 
     pc = PyChute(url=link2)
     pc.download(on_progress_callback=report_hook, filename='d:\\test')
     print(pc.title())
     print(pc.channel())
     print(pc.publish_date())
     print(pc.duration())
     print(pc.subscriptions())
     print(pc.likes())
     print(pc.views())
     print(pc.filesize())
     print(pc.thumbnail())
+    print(pc.description())
```

### Comparing `pychute-0.0.7/tests/test_helpers.py` & `pychute-0.0.8/tests/test_helpers.py`

 * *Files identical despite different names*

