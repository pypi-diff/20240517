# Comparing `tmp/why-tools-0.0.2b3.tar.gz` & `tmp/why-tools-0.0.2b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "why-tools-0.0.2b3.tar", last modified: Tue Apr 16 13:35:09 2024, max compression
+gzip compressed data, was "why-tools-0.0.2b5.tar", last modified: Fri May 17 08:51:12 2024, max compression
```

## Comparing `why-tools-0.0.2b3.tar` & `why-tools-0.0.2b5.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxrwxr-x   0 yintian   (1000) yintian   (1000)        0 2024-04-16 13:35:09.874463 why-tools-0.0.2b3/
--rw-rw-r--   0 yintian   (1000) yintian   (1000)      701 2024-04-16 13:35:09.874463 why-tools-0.0.2b3/PKG-INFO
--rw-rw-r--   0 yintian   (1000) yintian   (1000)      111 2024-04-15 15:11:28.000000 why-tools-0.0.2b3/README.md
--rw-rw-r--   0 yintian   (1000) yintian   (1000)       38 2024-04-16 13:35:09.874463 why-tools-0.0.2b3/setup.cfg
--rw-rw-r--   0 yintian   (1000) yintian   (1000)     4188 2024-04-16 13:35:09.000000 why-tools-0.0.2b3/setup.py
-drwxrwxr-x   0 yintian   (1000) yintian   (1000)        0 2024-04-16 13:35:09.874463 why-tools-0.0.2b3/why_tools.egg-info/
--rw-rw-r--   0 yintian   (1000) yintian   (1000)      701 2024-04-16 13:35:09.000000 why-tools-0.0.2b3/why_tools.egg-info/PKG-INFO
--rw-rw-r--   0 yintian   (1000) yintian   (1000)      261 2024-04-16 13:35:09.000000 why-tools-0.0.2b3/why_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 yintian   (1000) yintian   (1000)        1 2024-04-16 13:35:09.000000 why-tools-0.0.2b3/why_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 yintian   (1000) yintian   (1000)       14 2024-04-16 13:35:09.000000 why-tools-0.0.2b3/why_tools.egg-info/requires.txt
--rw-rw-r--   0 yintian   (1000) yintian   (1000)        7 2024-04-16 13:35:09.000000 why-tools-0.0.2b3/why_tools.egg-info/top_level.txt
-drwxrwxr-x   0 yintian   (1000) yintian   (1000)        0 2024-04-16 13:35:09.874463 why-tools-0.0.2b3/ytools/
--rw-rw-r--   0 yintian   (1000) yintian   (1000)      187 2024-04-16 13:35:09.000000 why-tools-0.0.2b3/ytools/__init__.py
--rw-rw-r--   0 yintian   (1000) yintian   (1000)     1578 2024-04-16 13:31:34.000000 why-tools-0.0.2b3/ytools/date.py
--rw-rw-r--   0 yintian   (1000) yintian   (1000)      566 2024-04-15 11:36:15.000000 why-tools-0.0.2b3/ytools/file.py
--rw-rw-r--   0 yintian   (1000) yintian   (1000)      194 2024-04-15 12:01:24.000000 why-tools-0.0.2b3/ytools/log.py
--rw-rw-r--   0 yintian   (1000) yintian   (1000)     1752 2024-04-16 12:19:04.000000 why-tools-0.0.2b3/ytools/utils.py
+drwxrwxr-x   0 yintian   (1000) yintian   (1000)        0 2024-05-17 08:51:12.372786 why-tools-0.0.2b5/
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)       21 2024-05-17 08:51:07.000000 why-tools-0.0.2b5/MANIFEST.in
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)      701 2024-05-17 08:51:12.372786 why-tools-0.0.2b5/PKG-INFO
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)      111 2024-04-15 15:11:28.000000 why-tools-0.0.2b5/README.md
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)       38 2024-05-17 08:51:12.372786 why-tools-0.0.2b5/setup.cfg
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)     4220 2024-05-17 08:51:07.000000 why-tools-0.0.2b5/setup.py
+drwxrwxr-x   0 yintian   (1000) yintian   (1000)        0 2024-05-17 08:51:12.372786 why-tools-0.0.2b5/why_tools.egg-info/
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)      701 2024-05-17 08:51:12.000000 why-tools-0.0.2b5/why_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)      350 2024-05-17 08:51:12.000000 why-tools-0.0.2b5/why_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)        1 2024-05-17 08:51:12.000000 why-tools-0.0.2b5/why_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)       14 2024-05-17 08:51:12.000000 why-tools-0.0.2b5/why_tools.egg-info/requires.txt
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)        7 2024-05-17 08:51:12.000000 why-tools-0.0.2b5/why_tools.egg-info/top_level.txt
+drwxrwxr-x   0 yintian   (1000) yintian   (1000)        0 2024-05-17 08:51:12.372786 why-tools-0.0.2b5/ytools/
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)      187 2024-05-17 08:51:07.000000 why-tools-0.0.2b5/ytools/__init__.py
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)     1578 2024-04-16 13:31:34.000000 why-tools-0.0.2b5/ytools/date.py
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)      566 2024-04-15 11:36:15.000000 why-tools-0.0.2b5/ytools/file.py
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)      194 2024-04-15 12:01:24.000000 why-tools-0.0.2b5/ytools/log.py
+drwxrwxr-x   0 yintian   (1000) yintian   (1000)        0 2024-05-17 08:51:12.372786 why-tools-0.0.2b5/ytools/network/
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)      154 2024-05-17 08:51:07.000000 why-tools-0.0.2b5/ytools/network/__init__.py
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)    15874 2024-05-17 08:51:07.000000 why-tools-0.0.2b5/ytools/network/request.py
+drwxrwxr-x   0 yintian   (1000) yintian   (1000)        0 2024-05-17 08:51:12.372786 why-tools-0.0.2b5/ytools/tpls/
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)       84 2024-05-17 08:51:07.000000 why-tools-0.0.2b5/ytools/tpls/__init__.py
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)     1752 2024-04-16 12:19:04.000000 why-tools-0.0.2b5/ytools/utils.py
```

### Comparing `why-tools-0.0.2b3/PKG-INFO` & `why-tools-0.0.2b5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: why-tools
-Version: 0.0.2b3
+Version: 0.0.2b5
 Summary: 为什么还要使用别的工具呢？
 Home-page: https://github.com/yintian710/whytools
 Author: yintian
 Author-email: yintian710@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `why-tools-0.0.2b3/setup.py` & `why-tools-0.0.2b5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# -*- coding: utf-8 -*-
+# -*- coding: gbk -*-
 """
 @File    : setup.py
-@Date    : 2024/4/15 下午7:23
+@Date    : 2024/4/15 ÏÂÎç7:23
 @Author  : yintian
 @Desc    : 
 """
 # Note: To use the 'upload' functionality of this file, you must:
 #   $ pipenv install twine --dev
 
 import io
@@ -17,15 +17,15 @@
 
 from ytools.file import get_file_read
 from ytools.log import logger
 from ytools import __version__
 
 # Package meta-data.
 NAME = 'why-tools'
-DESCRIPTION = '为什么还要使用别的工具呢？'
+DESCRIPTION = 'ÎªÊ²Ã´»¹ÒªÊ¹ÓÃ±ðµÄ¹¤¾ßÄØ£¿'
 URL = 'https://github.com/yintian710/whytools'
 EMAIL = 'yintian710@gmail.com'
 AUTHOR = 'yintian'
 REQUIRES_PYTHON = '>=3.8.0'
 VERSION = __version__
 
 # What packages are required for this module to be executed?
@@ -78,34 +78,34 @@
         pass
 
     def run(self):
 
         if len(sys.argv) > 1:
             return
         try:
-            self.status('Removing previous builds…')
+            self.status('Removing previous builds¡­')
             rmtree(os.path.join(here, 'dist'))
         except OSError:
             pass
 
-        self.status('Building Source and Wheel (universal) distribution…')
+        self.status('Building Source and Wheel (universal) distribution¡­')
         os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
-        self.status('Building Source and Wheel (universal) distribution…')
+        self.status('Building Source and Wheel (universal) distribution¡­')
         os.system(f'{sys.executable} setup.py sdist build')
 
-        self.status('Uploading the package to PyPI via Twine…')
+        self.status('Uploading the package to PyPI via Twine¡­')
         os.system('twine upload dist/*')
 
-        self.status('Pushing git tags…')
-        os.system('git tag v{0}'.format(about['__version__']))
-        os.system('git commit -m v{0}'.format(about['__version__']))
-        # os.system()
-        os.system('git push --tags')
+        self.status('Pushing git tags¡­')
+        os.system('git commit -a -m v{0}'.format(about['__version__']))
         os.system('git push')
-
+        # os.system()
+        if 'b' not in about['__version__']:
+            os.system('git tag v{0}'.format(about['__version__']))
+            os.system('git push --tags')
         sys.exit()
 
 
 # Where the magic happens:
 setup(
     name=NAME,
     version=about['__version__'],
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+iso-8859-1
```

### Comparing `why-tools-0.0.2b3/why_tools.egg-info/PKG-INFO` & `why-tools-0.0.2b5/why_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: why-tools
-Version: 0.0.2b3
+Version: 0.0.2b5
 Summary: 为什么还要使用别的工具呢？
 Home-page: https://github.com/yintian710/whytools
 Author: yintian
 Author-email: yintian710@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `why-tools-0.0.2b3/ytools/date.py` & `why-tools-0.0.2b5/ytools/date.py`

 * *Files identical despite different names*

### Comparing `why-tools-0.0.2b3/ytools/file.py` & `why-tools-0.0.2b5/ytools/file.py`

 * *Files identical despite different names*

### Comparing `why-tools-0.0.2b3/ytools/utils.py` & `why-tools-0.0.2b5/ytools/utils.py`

 * *Files identical despite different names*

