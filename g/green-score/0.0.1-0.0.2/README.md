# Comparing `tmp/green_score-0.0.1.tar.gz` & `tmp/green_score-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "green_score-0.0.1.tar", last modified: Thu May 16 16:55:49 2024, max compression
+gzip compressed data, was "green_score-0.0.2.tar", last modified: Fri May 17 04:41:59 2024, max compression
```

## Comparing `green_score-0.0.1.tar` & `green_score-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2024-05-16 16:55:49.240056 green_score-0.0.1/
--rw-rw-r--   0 jb        (1000) jb        (1000)     3402 2024-05-16 16:55:49.240056 green_score-0.0.1/PKG-INFO
--rw-rw-r--   0 jb        (1000) jb        (1000)     3045 2024-05-16 16:52:31.000000 green_score-0.0.1/README.md
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2024-05-16 16:55:49.236056 green_score-0.0.1/green_score/
--rw-rw-r--   0 jb        (1000) jb        (1000)       25 2024-05-16 16:46:03.000000 green_score-0.0.1/green_score/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    12754 2024-05-16 16:44:38.000000 green_score-0.0.1/green_score/green.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3430 2024-05-16 16:42:57.000000 green_score-0.0.1/green_score/utils.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2024-05-16 16:55:49.236056 green_score-0.0.1/green_score.egg-info/
--rw-rw-r--   0 jb        (1000) jb        (1000)     3402 2024-05-16 16:55:48.000000 green_score-0.0.1/green_score.egg-info/PKG-INFO
--rw-rw-r--   0 jb        (1000) jb        (1000)      292 2024-05-16 16:55:49.000000 green_score-0.0.1/green_score.egg-info/SOURCES.txt
--rw-rw-r--   0 jb        (1000) jb        (1000)        1 2024-05-16 16:55:48.000000 green_score-0.0.1/green_score.egg-info/dependency_links.txt
--rw-rw-r--   0 jb        (1000) jb        (1000)        1 2024-05-16 16:55:48.000000 green_score-0.0.1/green_score.egg-info/not-zip-safe
--rw-rw-r--   0 jb        (1000) jb        (1000)       71 2024-05-16 16:55:48.000000 green_score-0.0.1/green_score.egg-info/requires.txt
--rw-rw-r--   0 jb        (1000) jb        (1000)       12 2024-05-16 16:55:48.000000 green_score-0.0.1/green_score.egg-info/top_level.txt
--rw-rw-r--   0 jb        (1000) jb        (1000)       38 2024-05-16 16:55:49.240056 green_score-0.0.1/setup.cfg
--rw-rw-r--   0 jb        (1000) jb        (1000)      687 2024-05-16 16:40:55.000000 green_score-0.0.1/setup.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2024-05-17 04:41:59.276035 green_score-0.0.2/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3529 2024-05-17 04:41:59.272035 green_score-0.0.2/PKG-INFO
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3208 2024-05-16 17:03:12.000000 green_score-0.0.2/README.md
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2024-05-17 04:41:59.272035 green_score-0.0.2/green_score/
+-rw-rw-r--   0 jb        (1000) jb        (1000)       25 2024-05-16 16:46:03.000000 green_score-0.0.2/green_score/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    12754 2024-05-17 04:38:24.000000 green_score-0.0.2/green_score/green.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3460 2024-05-17 04:33:11.000000 green_score-0.0.2/green_score/utils.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2024-05-17 04:41:59.272035 green_score-0.0.2/green_score.egg-info/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3529 2024-05-17 04:41:58.000000 green_score-0.0.2/green_score.egg-info/PKG-INFO
+-rw-rw-r--   0 jb        (1000) jb        (1000)      292 2024-05-17 04:41:59.000000 green_score-0.0.2/green_score.egg-info/SOURCES.txt
+-rw-rw-r--   0 jb        (1000) jb        (1000)        1 2024-05-17 04:41:58.000000 green_score-0.0.2/green_score.egg-info/dependency_links.txt
+-rw-rw-r--   0 jb        (1000) jb        (1000)        1 2024-05-16 16:55:48.000000 green_score-0.0.2/green_score.egg-info/not-zip-safe
+-rw-rw-r--   0 jb        (1000) jb        (1000)       71 2024-05-17 04:41:58.000000 green_score-0.0.2/green_score.egg-info/requires.txt
+-rw-rw-r--   0 jb        (1000) jb        (1000)       12 2024-05-17 04:41:58.000000 green_score-0.0.2/green_score.egg-info/top_level.txt
+-rw-rw-r--   0 jb        (1000) jb        (1000)       38 2024-05-17 04:41:59.276035 green_score-0.0.2/setup.cfg
+-rw-rw-r--   0 jb        (1000) jb        (1000)      687 2024-05-17 04:41:42.000000 green_score-0.0.2/setup.py
```

### Comparing `green_score-0.0.1/PKG-INFO` & `green_score-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: green_score
-Version: 0.0.1
-Summary: UNKNOWN
+Version: 0.0.2
 Author: Jean-Benoit Delbrouck
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-# GREEN
+# GREEN: Generative Radiology Report Evaluation and Error Notation
+[[Project Page](https://stanford-aimi.github.io/green.html)][[Paper](https://arxiv.org/pdf/2405.03595)]
 
 ## Installation
 
 ```bash
 pip install green-score
 ```
 
@@ -58,8 +57,7 @@
 @article{ostmeier2024green,
     title={GREEN: Generative Radiology Report Evaluation and Error Notation},
     author={Ostmeier, Sophie and Xu, Justin and Chen, Zhihong and Varma, Maya and Blankemeier, Louis and Bluethgen, Christian and Michalson, Arne Edward and Moseley, Michael and Langlotz, Curtis and Chaudhari, Akshay S and others},
     journal={arXiv preprint arXiv:2405.03595},
     year={2024}
 }
 ```
-
```

### Comparing `green_score-0.0.1/README.md` & `green_score-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# GREEN
+# GREEN: Generative Radiology Report Evaluation and Error Notation
+[[Project Page](https://stanford-aimi.github.io/green.html)][[Paper](https://arxiv.org/pdf/2405.03595)]
 
 ## Installation
 
 ```bash
 pip install green-score
 ```
```

### Comparing `green_score-0.0.1/green_score/green.py` & `green_score-0.0.2/green_score/green.py`

 * *Files identical despite different names*

### Comparing `green_score-0.0.1/green_score/utils.py` & `green_score-0.0.2/green_score/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
         responses (list): List of response strings.
 
     Returns:
         list: List of cleaned response strings.
     """
     response_list = []
     for i in responses:
-        if "" in i:
-            i = i.split("")[-1]
-        i = i.replace("</s>", "").replace("<unk>", "")
+        if "<|assistant|>" in i:
+            i = i.split("<|assistant|>")[-1]
+            i = i.replace("</s>", "").replace("<unk>", "")
         response_list.append(i)
     return response_list
 
 
 def make_prompt(text1, text2):
     """
     Creates a prompt for evaluating the accuracy of a candidate radiology report in comparison to a reference radiology report.
```

### Comparing `green_score-0.0.1/green_score.egg-info/PKG-INFO` & `green_score-0.0.2/green_score.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: green-score
-Version: 0.0.1
-Summary: UNKNOWN
+Version: 0.0.2
 Author: Jean-Benoit Delbrouck
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-# GREEN
+# GREEN: Generative Radiology Report Evaluation and Error Notation
+[[Project Page](https://stanford-aimi.github.io/green.html)][[Paper](https://arxiv.org/pdf/2405.03595)]
 
 ## Installation
 
 ```bash
 pip install green-score
 ```
 
@@ -58,8 +57,7 @@
 @article{ostmeier2024green,
     title={GREEN: Generative Radiology Report Evaluation and Error Notation},
     author={Ostmeier, Sophie and Xu, Justin and Chen, Zhihong and Varma, Maya and Blankemeier, Louis and Bluethgen, Christian and Michalson, Arne Edward and Moseley, Michael and Langlotz, Curtis and Chaudhari, Akshay S and others},
     journal={arXiv preprint arXiv:2405.03595},
     year={2024}
 }
 ```
-
```

### Comparing `green_score-0.0.1/setup.py` & `green_score-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='green_score',
-    version='0.0.1',
+    version='0.0.2',
     author='Jean-Benoit Delbrouck',
     license='MIT',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
```

