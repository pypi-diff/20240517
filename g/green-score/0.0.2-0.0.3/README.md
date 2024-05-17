# Comparing `tmp/green_score-0.0.2.tar.gz` & `tmp/green_score-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "green_score-0.0.2.tar", last modified: Fri May 17 04:41:59 2024, max compression
+gzip compressed data, was "green_score-0.0.3.tar", last modified: Fri May 17 05:04:48 2024, max compression
```

## Comparing `green_score-0.0.2.tar` & `green_score-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2024-05-17 04:41:59.276035 green_score-0.0.2/
--rw-rw-r--   0 jb        (1000) jb        (1000)     3529 2024-05-17 04:41:59.272035 green_score-0.0.2/PKG-INFO
--rw-rw-r--   0 jb        (1000) jb        (1000)     3208 2024-05-16 17:03:12.000000 green_score-0.0.2/README.md
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2024-05-17 04:41:59.272035 green_score-0.0.2/green_score/
--rw-rw-r--   0 jb        (1000) jb        (1000)       25 2024-05-16 16:46:03.000000 green_score-0.0.2/green_score/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    12754 2024-05-17 04:38:24.000000 green_score-0.0.2/green_score/green.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3460 2024-05-17 04:33:11.000000 green_score-0.0.2/green_score/utils.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2024-05-17 04:41:59.272035 green_score-0.0.2/green_score.egg-info/
--rw-rw-r--   0 jb        (1000) jb        (1000)     3529 2024-05-17 04:41:58.000000 green_score-0.0.2/green_score.egg-info/PKG-INFO
--rw-rw-r--   0 jb        (1000) jb        (1000)      292 2024-05-17 04:41:59.000000 green_score-0.0.2/green_score.egg-info/SOURCES.txt
--rw-rw-r--   0 jb        (1000) jb        (1000)        1 2024-05-17 04:41:58.000000 green_score-0.0.2/green_score.egg-info/dependency_links.txt
--rw-rw-r--   0 jb        (1000) jb        (1000)        1 2024-05-16 16:55:48.000000 green_score-0.0.2/green_score.egg-info/not-zip-safe
--rw-rw-r--   0 jb        (1000) jb        (1000)       71 2024-05-17 04:41:58.000000 green_score-0.0.2/green_score.egg-info/requires.txt
--rw-rw-r--   0 jb        (1000) jb        (1000)       12 2024-05-17 04:41:58.000000 green_score-0.0.2/green_score.egg-info/top_level.txt
--rw-rw-r--   0 jb        (1000) jb        (1000)       38 2024-05-17 04:41:59.276035 green_score-0.0.2/setup.cfg
--rw-rw-r--   0 jb        (1000) jb        (1000)      687 2024-05-17 04:41:42.000000 green_score-0.0.2/setup.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2024-05-17 05:04:48.544066 green_score-0.0.3/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3529 2024-05-17 05:04:48.544066 green_score-0.0.3/PKG-INFO
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3208 2024-05-16 17:03:12.000000 green_score-0.0.3/README.md
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2024-05-17 05:04:48.544066 green_score-0.0.3/green_score/
+-rw-rw-r--   0 jb        (1000) jb        (1000)       25 2024-05-16 16:46:03.000000 green_score-0.0.3/green_score/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    12798 2024-05-17 05:03:50.000000 green_score-0.0.3/green_score/green.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3460 2024-05-17 04:33:11.000000 green_score-0.0.3/green_score/utils.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2024-05-17 05:04:48.544066 green_score-0.0.3/green_score.egg-info/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3529 2024-05-17 05:04:48.000000 green_score-0.0.3/green_score.egg-info/PKG-INFO
+-rw-rw-r--   0 jb        (1000) jb        (1000)      292 2024-05-17 05:04:48.000000 green_score-0.0.3/green_score.egg-info/SOURCES.txt
+-rw-rw-r--   0 jb        (1000) jb        (1000)        1 2024-05-17 05:04:48.000000 green_score-0.0.3/green_score.egg-info/dependency_links.txt
+-rw-rw-r--   0 jb        (1000) jb        (1000)        1 2024-05-16 16:55:48.000000 green_score-0.0.3/green_score.egg-info/not-zip-safe
+-rw-rw-r--   0 jb        (1000) jb        (1000)       71 2024-05-17 05:04:48.000000 green_score-0.0.3/green_score.egg-info/requires.txt
+-rw-rw-r--   0 jb        (1000) jb        (1000)       12 2024-05-17 05:04:48.000000 green_score-0.0.3/green_score.egg-info/top_level.txt
+-rw-rw-r--   0 jb        (1000) jb        (1000)       38 2024-05-17 05:04:48.544066 green_score-0.0.3/setup.cfg
+-rw-rw-r--   0 jb        (1000) jb        (1000)      687 2024-05-17 05:04:30.000000 green_score-0.0.3/setup.py
```

### Comparing `green_score-0.0.2/PKG-INFO` & `green_score-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: green_score
-Version: 0.0.2
+Version: 0.0.3
 Author: Jean-Benoit Delbrouck
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `green_score-0.0.2/README.md` & `green_score-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `green_score-0.0.2/green_score/green.py` & `green_score-0.0.3/green_score/green.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             pretrained_model_name_or_path=model_id_or_path,
             add_eos_token=True,
             use_fast=True,
             trust_remote_code=True,
             padding_side="left",
         )
         self.tokenizer.pad_token = self.tokenizer.eos_token
-        self.tokenizer.chat_template = "{% for message in messages %}\n{% if message['from'] == 'human' %}\n{{ '\n' + message['value'] + eos_token }}\n{% elif message['from'] == 'system' %}\n{{ '\n' + message['value'] + eos_token }}\n{% elif message['from'] == 'gpt' %}\n{{ '\n'  + message['value'] + eos_token }}\n{% endif %}\n{% if loop.last and add_generation_prompt %}\n{{ '' }}\n{% endif %}\n{% endfor %}"
+        self.tokenizer.chat_template = "{% for message in messages %}\n{% if message['from'] == 'human' %}\n{{ '<|user|>\n' + message['value'] + eos_token }}\n{% elif message['from'] == 'system' %}\n{{ '<|system|>\n' + message['value'] + eos_token }}\n{% elif message['from'] == 'gpt' %}\n{{ '<|assistant|>\n'  + message['value'] + eos_token }}\n{% endif %}\n{% if loop.last and add_generation_prompt %}\n{{ '<|assistant|>' }}\n{% endif %}\n{% endfor %}"
 
         self.categories = [
             "Clinically Significant Errors",
             "Clinically Insignificant Errors",
             "Matched Findings",
         ]
```

### Comparing `green_score-0.0.2/green_score/utils.py` & `green_score-0.0.3/green_score/utils.py`

 * *Files identical despite different names*

### Comparing `green_score-0.0.2/green_score.egg-info/PKG-INFO` & `green_score-0.0.3/green_score.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: green-score
-Version: 0.0.2
+Version: 0.0.3
 Author: Jean-Benoit Delbrouck
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `green_score-0.0.2/setup.py` & `green_score-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='green_score',
-    version='0.0.2',
+    version='0.0.3',
     author='Jean-Benoit Delbrouck',
     license='MIT',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
```

