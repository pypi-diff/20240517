# Comparing `tmp/g4f_xn-0.0.3.tar.gz` & `tmp/g4f_xn-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g4f_xn-0.0.3.tar", last modified: Thu May 16 21:40:01 2024, max compression
+gzip compressed data, was "g4f_xn-0.0.4.tar", last modified: Thu May 16 21:51:22 2024, max compression
```

## Comparing `g4f_xn-0.0.3.tar` & `g4f_xn-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 21:40:01.293288 g4f_xn-0.0.3/
--rw-rw-rw-   0        0        0     1083 2024-05-16 19:53:32.000000 g4f_xn-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      612 2024-05-16 21:40:01.277554 g4f_xn-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1608 2024-05-16 20:38:48.000000 g4f_xn-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 21:40:01.261890 g4f_xn-0.0.3/g4f_xn/
--rw-rw-rw-   0        0        0      115 2024-05-16 21:37:25.000000 g4f_xn-0.0.3/g4f_xn/__init__.py
--rw-rw-rw-   0        0        0     1280 2024-05-16 19:56:26.000000 g4f_xn-0.0.3/g4f_xn/gpt.py
--rw-rw-rw-   0        0        0      352 2024-05-16 19:34:22.000000 g4f_xn-0.0.3/g4f_xn/misc.py
--rw-rw-rw-   0        0        0      805 2024-05-16 12:55:08.000000 g4f_xn-0.0.3/g4f_xn/output.py
-drwxrwxrwx   0        0        0        0 2024-05-16 21:40:01.277554 g4f_xn-0.0.3/g4f_xn/sound/
--rw-rw-rw-   0        0        0       20 2024-05-16 21:38:06.000000 g4f_xn-0.0.3/g4f_xn/sound/__init__.py
--rw-rw-rw-   0        0        0     1673 2024-05-16 21:36:32.000000 g4f_xn-0.0.3/g4f_xn/sound/sound.py
--rw-rw-rw-   0        0        0     3272 2024-05-16 19:56:26.000000 g4f_xn-0.0.3/g4f_xn/test_providers.py
-drwxrwxrwx   0        0        0        0 2024-05-16 21:40:01.277554 g4f_xn-0.0.3/g4f_xn.egg-info/
--rw-rw-rw-   0        0        0      612 2024-05-16 21:40:01.000000 g4f_xn-0.0.3/g4f_xn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2024-05-16 21:40:01.000000 g4f_xn-0.0.3/g4f_xn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 21:40:01.000000 g4f_xn-0.0.3/g4f_xn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-05-16 21:40:01.000000 g4f_xn-0.0.3/g4f_xn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-16 21:40:01.000000 g4f_xn-0.0.3/g4f_xn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 21:40:01.293288 g4f_xn-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      861 2024-05-16 21:36:32.000000 g4f_xn-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 21:51:22.614815 g4f_xn-0.0.4/
+-rw-rw-rw-   0        0        0     1083 2024-05-16 19:53:32.000000 g4f_xn-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       44 2024-05-16 21:50:49.000000 g4f_xn-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      634 2024-05-16 21:51:22.614815 g4f_xn-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1608 2024-05-16 20:38:48.000000 g4f_xn-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 21:51:22.583565 g4f_xn-0.0.4/g4f_xn/
+-rw-rw-rw-   0        0        0      115 2024-05-16 21:37:25.000000 g4f_xn-0.0.4/g4f_xn/__init__.py
+-rw-rw-rw-   0        0        0     1280 2024-05-16 19:56:26.000000 g4f_xn-0.0.4/g4f_xn/gpt.py
+-rw-rw-rw-   0        0        0      352 2024-05-16 19:34:22.000000 g4f_xn-0.0.4/g4f_xn/misc.py
+-rw-rw-rw-   0        0        0      805 2024-05-16 12:55:08.000000 g4f_xn-0.0.4/g4f_xn/output.py
+drwxrwxrwx   0        0        0        0 2024-05-16 21:51:22.599191 g4f_xn-0.0.4/g4f_xn/sound/
+-rw-rw-rw-   0        0        0   177048 2024-05-15 18:32:58.000000 g4f_xn-0.0.4/g4f_xn/sound/Hint.wav
+-rw-rw-rw-   0        0        0       20 2024-05-16 21:38:06.000000 g4f_xn-0.0.4/g4f_xn/sound/__init__.py
+-rw-rw-rw-   0        0        0   140274 2024-05-13 18:33:47.000000 g4f_xn-0.0.4/g4f_xn/sound/coins.wav
+-rw-rw-rw-   0        0        0   728142 2024-05-15 10:32:05.000000 g4f_xn-0.0.4/g4f_xn/sound/metal-pipe.wav
+-rw-rw-rw-   0        0        0     1673 2024-05-16 21:36:32.000000 g4f_xn-0.0.4/g4f_xn/sound/sound.py
+-rw-rw-rw-   0        0        0     3272 2024-05-16 19:56:26.000000 g4f_xn-0.0.4/g4f_xn/test_providers.py
+drwxrwxrwx   0        0        0        0 2024-05-16 21:51:22.614815 g4f_xn-0.0.4/g4f_xn.egg-info/
+-rw-rw-rw-   0        0        0      634 2024-05-16 21:51:22.000000 g4f_xn-0.0.4/g4f_xn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2024-05-16 21:51:22.000000 g4f_xn-0.0.4/g4f_xn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 21:51:22.000000 g4f_xn-0.0.4/g4f_xn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-16 21:51:22.000000 g4f_xn-0.0.4/g4f_xn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-16 21:51:22.000000 g4f_xn-0.0.4/g4f_xn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 21:51:22.614815 g4f_xn-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      870 2024-05-16 21:50:59.000000 g4f_xn-0.0.4/setup.py
```

### Comparing `g4f_xn-0.0.3/LICENSE` & `g4f_xn-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `g4f_xn-0.0.3/PKG-INFO` & `g4f_xn-0.0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: g4f_xn
-Version: 0.0.3
+Version: 0.0.4
 Summary: library for easy access to GPT models based on g4f
 Author: Xandr0v
 Author-email: <olegalexandrov468@gmail.com>
 Keywords: python,g4f,gpt
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: g4f
 Requires-Dist: pyaudio
+Requires-Dist: pydub
 Requires-Dist: colorama
 Requires-Dist: ffmpeg-downloader
 
 long description. Will change in the future
```

### Comparing `g4f_xn-0.0.3/README.md` & `g4f_xn-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `g4f_xn-0.0.3/g4f_xn/gpt.py` & `g4f_xn-0.0.4/g4f_xn/gpt.py`

 * *Files identical despite different names*

### Comparing `g4f_xn-0.0.3/g4f_xn/output.py` & `g4f_xn-0.0.4/g4f_xn/output.py`

 * *Files identical despite different names*

### Comparing `g4f_xn-0.0.3/g4f_xn/sound/sound.py` & `g4f_xn-0.0.4/g4f_xn/sound/sound.py`

 * *Files identical despite different names*

### Comparing `g4f_xn-0.0.3/g4f_xn/test_providers.py` & `g4f_xn-0.0.4/g4f_xn/test_providers.py`

 * *Files identical despite different names*

### Comparing `g4f_xn-0.0.3/g4f_xn.egg-info/PKG-INFO` & `g4f_xn-0.0.4/g4f_xn.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: g4f_xn
-Version: 0.0.3
+Version: 0.0.4
 Summary: library for easy access to GPT models based on g4f
 Author: Xandr0v
 Author-email: <olegalexandrov468@gmail.com>
 Keywords: python,g4f,gpt
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: g4f
 Requires-Dist: pyaudio
+Requires-Dist: pydub
 Requires-Dist: colorama
 Requires-Dist: ffmpeg-downloader
 
 long description. Will change in the future
```

### Comparing `g4f_xn-0.0.3/setup.py` & `g4f_xn-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'library for easy access to GPT models based on g4f'
 LONG_DESCRIPTION = 'long description. Will change in the future'
 
 # Setting up
 setup(
     name="g4f_xn",
     version=VERSION,
     author="Xandr0v",
     author_email="<olegalexandrov468@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=['g4f', 'pyaudio', 'colorama', 'ffmpeg-downloader'],
+    install_requires=['g4f', 'pyaudio', 'pydub', 'colorama', 'ffmpeg-downloader'],
     keywords=['python', 'g4f', 'gpt'],
     include_package_data=True,
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Microsoft :: Windows",
```

