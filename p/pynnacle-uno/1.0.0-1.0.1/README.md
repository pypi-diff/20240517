# Comparing `tmp/pynnacle_uno-1.0.0.tar.gz` & `tmp/pynnacle_uno-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynnacle_uno-1.0.0.tar", last modified: Sat May 11 13:52:52 2024, max compression
+gzip compressed data, was "pynnacle_uno-1.0.1.tar", last modified: Fri May 17 08:21:34 2024, max compression
```

## Comparing `pynnacle_uno-1.0.0.tar` & `pynnacle_uno-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 13:52:52.022098 pynnacle_uno-1.0.0/
--rw-rw-rw-   0        0        0    35549 2024-05-11 13:51:43.000000 pynnacle_uno-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3086 2024-05-11 13:52:52.020098 pynnacle_uno-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2017 2024-05-11 13:51:43.000000 pynnacle_uno-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 13:52:51.948842 pynnacle_uno-1.0.0/pynnacle_uno/
--rw-rw-rw-   0        0        0      862 2024-05-11 13:51:43.000000 pynnacle_uno-1.0.0/pynnacle_uno/__init__.py
--rw-rw-rw-   0        0        0    14009 2024-05-11 13:51:43.000000 pynnacle_uno-1.0.0/pynnacle_uno/main.py
-drwxrwxrwx   0        0        0        0 2024-05-11 13:52:52.017097 pynnacle_uno-1.0.0/pynnacle_uno.egg-info/
--rw-rw-rw-   0        0        0     3086 2024-05-11 13:52:51.000000 pynnacle_uno-1.0.0/pynnacle_uno.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2024-05-11 13:52:51.000000 pynnacle_uno-1.0.0/pynnacle_uno.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 13:52:51.000000 pynnacle_uno-1.0.0/pynnacle_uno.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-11 13:52:51.000000 pynnacle_uno-1.0.0/pynnacle_uno.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-11 13:52:51.000000 pynnacle_uno-1.0.0/pynnacle_uno.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 13:52:52.022098 pynnacle_uno-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1294 2024-05-11 13:51:43.000000 pynnacle_uno-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:21:34.014593 pynnacle_uno-1.0.1/
+-rw-rw-rw-   0        0        0    35549 2024-05-11 13:51:43.000000 pynnacle_uno-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3086 2024-05-17 08:21:34.013594 pynnacle_uno-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2017 2024-05-11 13:51:43.000000 pynnacle_uno-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 08:21:33.995589 pynnacle_uno-1.0.1/pynnacle_uno/
+-rw-rw-rw-   0        0        0      862 2024-05-11 13:51:43.000000 pynnacle_uno-1.0.1/pynnacle_uno/__init__.py
+-rw-rw-rw-   0        0        0    14014 2024-05-17 08:19:23.000000 pynnacle_uno-1.0.1/pynnacle_uno/main.py
+drwxrwxrwx   0        0        0        0 2024-05-17 08:21:34.010595 pynnacle_uno-1.0.1/pynnacle_uno.egg-info/
+-rw-rw-rw-   0        0        0     3086 2024-05-17 08:21:33.000000 pynnacle_uno-1.0.1/pynnacle_uno.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-05-17 08:21:33.000000 pynnacle_uno-1.0.1/pynnacle_uno.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 08:21:33.000000 pynnacle_uno-1.0.1/pynnacle_uno.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-17 08:21:33.000000 pynnacle_uno-1.0.1/pynnacle_uno.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-17 08:21:33.000000 pynnacle_uno-1.0.1/pynnacle_uno.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 08:21:34.014593 pynnacle_uno-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1294 2024-05-17 08:20:51.000000 pynnacle_uno-1.0.1/setup.py
```

### Comparing `pynnacle_uno-1.0.0/LICENSE` & `pynnacle_uno-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynnacle_uno-1.0.0/PKG-INFO` & `pynnacle_uno-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynnacle_uno
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python module that provides hands-on robotics coding experience in Python that closely mirrors the structure and functionality of Arduino's programming language.
 Home-page: https://github.com/Red-Pula/Pynnacle-Uno
 Author: Rafael Red Angelo M. Hizon, Jenel M. Justo, Serena Mae C.S. Lee
 Author-email: redhizon@gmail.com, jenel.just88@gmail.com, nmae.lee@gmail.com
 License: GNU Affero General Public License
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pynnacle_uno-1.0.0/README.md` & `pynnacle_uno-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pynnacle_uno-1.0.0/pynnacle_uno/__init__.py` & `pynnacle_uno-1.0.1/pynnacle_uno/__init__.py`

 * *Files identical despite different names*

### Comparing `pynnacle_uno-1.0.0/pynnacle_uno/main.py` & `pynnacle_uno-1.0.1/pynnacle_uno/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,14 +380,14 @@
 # See more at:
 #   1. <https://www.arduino.cc/reference/en/language/functions/advanced-io/tone/>
 #   2. <https://mryslab.github.io/pymata4/device_writes/#play_tone>
 def tone(pin, frequency, duration=None):
     if duration is None:
         _board.play_tone_continuously(pin, frequency)
     else:
-        _board.play_tone(pin, frequency, duration)
+        _board.play_tone(pin, frequency, int(duration))
 
 
 # This function accepts a pin as a parameter.
 # This function turns off the tone being played on the pin that was passed as a parameter.
 def noTone(pin):
     _board.play_tone_off(pin)
```

### Comparing `pynnacle_uno-1.0.0/pynnacle_uno.egg-info/PKG-INFO` & `pynnacle_uno-1.0.1/pynnacle_uno.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynnacle_uno
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python module that provides hands-on robotics coding experience in Python that closely mirrors the structure and functionality of Arduino's programming language.
 Home-page: https://github.com/Red-Pula/Pynnacle-Uno
 Author: Rafael Red Angelo M. Hizon, Jenel M. Justo, Serena Mae C.S. Lee
 Author-email: redhizon@gmail.com, jenel.just88@gmail.com, nmae.lee@gmail.com
 License: GNU Affero General Public License
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pynnacle_uno-1.0.0/setup.py` & `pynnacle_uno-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name='pynnacle_uno',
-    version='1.0.0', 
+    version='1.0.1', 
     packages=find_packages(),
     description='A Python module that provides hands-on robotics coding experience in Python that closely mirrors the structure and functionality of Arduino\'s programming language.',
     url='https://github.com/Red-Pula/Pynnacle-Uno',
     author='Rafael Red Angelo M. Hizon, Jenel M. Justo, Serena Mae C.S. Lee',
     author_email='redhizon@gmail.com, jenel.just88@gmail.com, nmae.lee@gmail.com',
     license='GNU Affero General Public License',
     install_requires=['pymata4>=1.15'],
```

