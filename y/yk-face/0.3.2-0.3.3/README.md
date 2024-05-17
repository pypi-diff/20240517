# Comparing `tmp/yk_face-0.3.2.tar.gz` & `tmp/yk_face-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/YK-Face-Python/YK-Face-Python/dist/.tmp-flw92oog/yk_face-0.3.2.tar", last modified: Thu Mar  2 11:21:59 2023, max compression
+gzip compressed data, was "/home/runner/work/YK-Face-Python/YK-Face-Python/dist/.tmp-0pbl93l6/yk_face-0.3.3.tar", last modified: Mon Nov 27 16:34:33 2023, max compression
```

## Comparing `yk_face-0.3.2.tar` & `yk_face-0.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 11:21:59.000000 yk_face-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-03-02 11:21:29.000000 yk_face-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-03-02 11:21:59.000000 yk_face-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-03-02 11:21:29.000000 yk_face-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 11:21:59.000000 yk_face-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-02 11:21:29.000000 yk_face-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 11:21:59.000000 yk_face-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    14909 2023-03-02 11:21:29.000000 yk_face-0.3.2/tests/test_face.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 11:21:59.000000 yk_face-0.3.2/yk_face/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-02 11:21:29.000000 yk_face-0.3.2/yk_face/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10780 2023-03-02 11:21:29.000000 yk_face-0.3.2/yk_face/face.py
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-03-02 11:21:29.000000 yk_face-0.3.2/yk_face/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-03-02 11:21:29.000000 yk_face-0.3.2/yk_face/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 11:21:59.000000 yk_face-0.3.2/yk_face.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-03-02 11:21:59.000000 yk_face-0.3.2/yk_face.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-02 11:21:59.000000 yk_face-0.3.2/yk_face.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 11:21:59.000000 yk_face-0.3.2/yk_face.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-02 11:21:59.000000 yk_face-0.3.2/yk_face.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-02 11:21:59.000000 yk_face-0.3.2/yk_face.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 16:34:33.000000 yk_face-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2023-11-27 16:34:25.000000 yk_face-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2023-11-27 16:34:33.000000 yk_face-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2023-11-27 16:34:25.000000 yk_face-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-27 16:34:33.000000 yk_face-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2023-11-27 16:34:25.000000 yk_face-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 16:34:33.000000 yk_face-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14909 2023-11-27 16:34:25.000000 yk_face-0.3.3/tests/test_face.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 16:34:33.000000 yk_face-0.3.3/yk_face/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2023-11-27 16:34:25.000000 yk_face-0.3.3/yk_face/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10779 2023-11-27 16:34:25.000000 yk_face-0.3.3/yk_face/face.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2023-11-27 16:34:25.000000 yk_face-0.3.3/yk_face/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2023-11-27 16:34:25.000000 yk_face-0.3.3/yk_face/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 16:34:33.000000 yk_face-0.3.3/yk_face.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2023-11-27 16:34:33.000000 yk_face-0.3.3/yk_face.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2023-11-27 16:34:33.000000 yk_face-0.3.3/yk_face.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 16:34:33.000000 yk_face-0.3.3/yk_face.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2023-11-27 16:34:33.000000 yk_face-0.3.3/yk_face.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-27 16:34:33.000000 yk_face-0.3.3/yk_face.egg-info/top_level.txt
```

### Comparing `yk_face-0.3.2/LICENSE` & `yk_face-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yk_face-0.3.2/PKG-INFO` & `yk_face-0.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yk_face
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python SDK for the YouFace API.
 Home-page: https://github.com/dev-yoonik/YK-Face-Python
 Author: Youverse
 Author-email: tech@youverse.id
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yk_face-0.3.2/README.md` & `yk_face-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `yk_face-0.3.2/setup.py` & `yk_face-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="yk_face",
-    version="0.3.2",
+    version="0.3.3",
     description="Python SDK for the YouFace API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Youverse",
     author_email="tech@youverse.id",
     url="https://github.com/dev-yoonik/YK-Face-Python",
     license='MIT',
```

### Comparing `yk_face-0.3.2/tests/test_face.py` & `yk_face-0.3.3/tests/test_face.py`

 * *Files identical despite different names*

### Comparing `yk_face-0.3.2/yk_face/face.py` & `yk_face-0.3.3/yk_face/face.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     image_b64 = parse_image(image)
     if processings is None:
         processings = ['detect', 'analyze', 'templify']
     process_request = ProcessRequest(
         image=image_b64,
         processings=processings,
-        configurations=configurations
+        configuration=configurations
     ).dict()
     return process_request
 
 
 def process(
         image,
         processings: List[str] = None,
```

### Comparing `yk_face-0.3.2/yk_face/group.py` & `yk_face-0.3.3/yk_face/group.py`

 * *Files identical despite different names*

### Comparing `yk_face-0.3.2/yk_face/util.py` & `yk_face-0.3.3/yk_face/util.py`

 * *Files identical despite different names*

### Comparing `yk_face-0.3.2/yk_face.egg-info/PKG-INFO` & `yk_face-0.3.3/yk_face.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yk-face
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python SDK for the YouFace API.
 Home-page: https://github.com/dev-yoonik/YK-Face-Python
 Author: Youverse
 Author-email: tech@youverse.id
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

