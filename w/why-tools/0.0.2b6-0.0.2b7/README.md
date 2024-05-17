# Comparing `tmp/why-tools-0.0.2b6.tar.gz` & `tmp/why-tools-0.0.2b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "why-tools-0.0.2b6.tar", last modified: Fri May 17 08:53:54 2024, max compression
+gzip compressed data, was "why-tools-0.0.2b7.tar", last modified: Fri May 17 08:55:27 2024, max compression
```

## Comparing `why-tools-0.0.2b6.tar` & `why-tools-0.0.2b7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 yintian   (1000) yintian   (1000)        0 2024-05-17 08:53:54.949856 why-tools-0.0.2b6/
--rw-rw-r--   0 yintian   (1000) yintian   (1000)       21 2024-05-17 08:51:07.000000 why-tools-0.0.2b6/MANIFEST.in
--rw-rw-r--   0 yintian   (1000) yintian   (1000)      701 2024-05-17 08:53:54.949856 why-tools-0.0.2b6/PKG-INFO
--rw-rw-r--   0 yintian   (1000) yintian   (1000)      111 2024-04-15 15:11:28.000000 why-tools-0.0.2b6/README.md
--rw-rw-r--   0 yintian   (1000) yintian   (1000)       38 2024-05-17 08:53:54.949856 why-tools-0.0.2b6/setup.cfg
--rw-rw-r--   0 yintian   (1000) yintian   (1000)     4220 2024-05-17 08:51:07.000000 why-tools-0.0.2b6/setup.py
-drwxrwxr-x   0 yintian   (1000) yintian   (1000)        0 2024-05-17 08:53:54.949856 why-tools-0.0.2b6/why_tools.egg-info/
--rw-rw-r--   0 yintian   (1000) yintian   (1000)      701 2024-05-17 08:53:54.000000 why-tools-0.0.2b6/why_tools.egg-info/PKG-INFO
--rw-rw-r--   0 yintian   (1000) yintian   (1000)      381 2024-05-17 08:53:54.000000 why-tools-0.0.2b6/why_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 yintian   (1000) yintian   (1000)        1 2024-05-17 08:53:54.000000 why-tools-0.0.2b6/why_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 yintian   (1000) yintian   (1000)       14 2024-05-17 08:53:54.000000 why-tools-0.0.2b6/why_tools.egg-info/requires.txt
--rw-rw-r--   0 yintian   (1000) yintian   (1000)        7 2024-05-17 08:53:54.000000 why-tools-0.0.2b6/why_tools.egg-info/top_level.txt
-drwxrwxr-x   0 yintian   (1000) yintian   (1000)        0 2024-05-17 08:53:54.949856 why-tools-0.0.2b6/ytools/
--rw-rw-r--   0 yintian   (1000) yintian   (1000)      187 2024-05-17 08:53:54.000000 why-tools-0.0.2b6/ytools/__init__.py
--rw-rw-r--   0 yintian   (1000) yintian   (1000)     1578 2024-04-16 13:31:34.000000 why-tools-0.0.2b6/ytools/date.py
--rw-rw-r--   0 yintian   (1000) yintian   (1000)      566 2024-04-15 11:36:15.000000 why-tools-0.0.2b6/ytools/file.py
--rw-rw-r--   0 yintian   (1000) yintian   (1000)      194 2024-04-15 12:01:24.000000 why-tools-0.0.2b6/ytools/log.py
-drwxrwxr-x   0 yintian   (1000) yintian   (1000)        0 2024-05-17 08:53:54.949856 why-tools-0.0.2b6/ytools/network/
--rw-rw-r--   0 yintian   (1000) yintian   (1000)      154 2024-05-17 08:51:07.000000 why-tools-0.0.2b6/ytools/network/__init__.py
--rw-rw-r--   0 yintian   (1000) yintian   (1000)    15874 2024-05-17 08:51:07.000000 why-tools-0.0.2b6/ytools/network/request.py
-drwxrwxr-x   0 yintian   (1000) yintian   (1000)        0 2024-05-17 08:53:54.949856 why-tools-0.0.2b6/ytools/tpls/
--rw-rw-r--   0 yintian   (1000) yintian   (1000)       84 2024-05-17 08:51:07.000000 why-tools-0.0.2b6/ytools/tpls/__init__.py
-drwxrwxr-x   0 yintian   (1000) yintian   (1000)        0 2024-05-17 08:53:54.949856 why-tools-0.0.2b6/ytools/tpls/spider/
--rw-rw-r--   0 yintian   (1000) yintian   (1000)      155 2024-05-17 08:53:18.000000 why-tools-0.0.2b6/ytools/tpls/spider/__init__.py
--rw-rw-r--   0 yintian   (1000) yintian   (1000)     1752 2024-04-16 12:19:04.000000 why-tools-0.0.2b6/ytools/utils.py
+drwxrwxr-x   0 yintian   (1000) yintian   (1000)        0 2024-05-17 08:55:27.786459 why-tools-0.0.2b7/
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)       21 2024-05-17 08:51:07.000000 why-tools-0.0.2b7/MANIFEST.in
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)      701 2024-05-17 08:55:27.782459 why-tools-0.0.2b7/PKG-INFO
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)      111 2024-04-15 15:11:28.000000 why-tools-0.0.2b7/README.md
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)       38 2024-05-17 08:55:27.786459 why-tools-0.0.2b7/setup.cfg
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)     4220 2024-05-17 08:51:07.000000 why-tools-0.0.2b7/setup.py
+drwxrwxr-x   0 yintian   (1000) yintian   (1000)        0 2024-05-17 08:55:27.782459 why-tools-0.0.2b7/why_tools.egg-info/
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)      701 2024-05-17 08:55:27.000000 why-tools-0.0.2b7/why_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)      381 2024-05-17 08:55:27.000000 why-tools-0.0.2b7/why_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)        1 2024-05-17 08:55:27.000000 why-tools-0.0.2b7/why_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)       14 2024-05-17 08:55:27.000000 why-tools-0.0.2b7/why_tools.egg-info/requires.txt
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)        7 2024-05-17 08:55:27.000000 why-tools-0.0.2b7/why_tools.egg-info/top_level.txt
+drwxrwxr-x   0 yintian   (1000) yintian   (1000)        0 2024-05-17 08:55:27.782459 why-tools-0.0.2b7/ytools/
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)      187 2024-05-17 08:55:27.000000 why-tools-0.0.2b7/ytools/__init__.py
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)     1578 2024-04-16 13:31:34.000000 why-tools-0.0.2b7/ytools/date.py
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)      566 2024-04-15 11:36:15.000000 why-tools-0.0.2b7/ytools/file.py
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)      194 2024-04-15 12:01:24.000000 why-tools-0.0.2b7/ytools/log.py
+drwxrwxr-x   0 yintian   (1000) yintian   (1000)        0 2024-05-17 08:55:27.782459 why-tools-0.0.2b7/ytools/network/
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)      154 2024-05-17 08:51:07.000000 why-tools-0.0.2b7/ytools/network/__init__.py
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)    15874 2024-05-17 08:51:07.000000 why-tools-0.0.2b7/ytools/network/request.py
+drwxrwxr-x   0 yintian   (1000) yintian   (1000)        0 2024-05-17 08:55:27.782459 why-tools-0.0.2b7/ytools/tpls/
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)       84 2024-05-17 08:51:07.000000 why-tools-0.0.2b7/ytools/tpls/__init__.py
+drwxrwxr-x   0 yintian   (1000) yintian   (1000)        0 2024-05-17 08:55:27.782459 why-tools-0.0.2b7/ytools/tpls/spider/
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)      155 2024-05-17 08:53:18.000000 why-tools-0.0.2b7/ytools/tpls/spider/__init__.py
+-rw-rw-r--   0 yintian   (1000) yintian   (1000)     1752 2024-04-16 12:19:04.000000 why-tools-0.0.2b7/ytools/utils.py
```

### Comparing `why-tools-0.0.2b6/PKG-INFO` & `why-tools-0.0.2b7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: why-tools
-Version: 0.0.2b6
+Version: 0.0.2b7
 Summary: 为什么还要使用别的工具呢？
 Home-page: https://github.com/yintian710/whytools
 Author: yintian
 Author-email: yintian710@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `why-tools-0.0.2b6/setup.py` & `why-tools-0.0.2b7/setup.py`

 * *Files identical despite different names*

### Comparing `why-tools-0.0.2b6/why_tools.egg-info/PKG-INFO` & `why-tools-0.0.2b7/why_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: why-tools
-Version: 0.0.2b6
+Version: 0.0.2b7
 Summary: 为什么还要使用别的工具呢？
 Home-page: https://github.com/yintian710/whytools
 Author: yintian
 Author-email: yintian710@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `why-tools-0.0.2b6/ytools/date.py` & `why-tools-0.0.2b7/ytools/date.py`

 * *Files identical despite different names*

### Comparing `why-tools-0.0.2b6/ytools/file.py` & `why-tools-0.0.2b7/ytools/file.py`

 * *Files identical despite different names*

### Comparing `why-tools-0.0.2b6/ytools/network/request.py` & `why-tools-0.0.2b7/ytools/network/request.py`

 * *Files identical despite different names*

### Comparing `why-tools-0.0.2b6/ytools/utils.py` & `why-tools-0.0.2b7/ytools/utils.py`

 * *Files identical despite different names*

