# Comparing `tmp/aliyun-python-sdk-tingwu-1.0.6.tar.gz` & `tmp/aliyun-python-sdk-tingwu-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-tingwu-1.0.6.tar", last modified: Wed May 15 03:17:55 2024, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-tingwu-1.0.7.tar", last modified: Fri May 17 07:19:04 2024, max compression
```

## Comparing `aliyun-python-sdk-tingwu-1.0.6.tar` & `aliyun-python-sdk-tingwu-1.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 03:17:55.000000 aliyun-python-sdk-tingwu-1.0.6/
--rw-r--r--   0 root         (0) root         (0)      575 2024-05-15 03:17:55.000000 aliyun-python-sdk-tingwu-1.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2024-05-15 03:17:55.000000 aliyun-python-sdk-tingwu-1.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1552 2024-05-15 03:17:55.000000 aliyun-python-sdk-tingwu-1.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      533 2024-05-15 03:17:55.000000 aliyun-python-sdk-tingwu-1.0.6/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 03:17:55.000000 aliyun-python-sdk-tingwu-1.0.6/aliyun_python_sdk_tingwu.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1552 2024-05-15 03:17:55.000000 aliyun-python-sdk-tingwu-1.0.6/aliyun_python_sdk_tingwu.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      859 2024-05-15 03:17:55.000000 aliyun-python-sdk-tingwu-1.0.6/aliyun_python_sdk_tingwu.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 03:17:55.000000 aliyun-python-sdk-tingwu-1.0.6/aliyun_python_sdk_tingwu.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-15 03:17:55.000000 aliyun-python-sdk-tingwu-1.0.6/aliyun_python_sdk_tingwu.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-15 03:17:55.000000 aliyun-python-sdk-tingwu-1.0.6/aliyun_python_sdk_tingwu.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 03:17:55.000000 aliyun-python-sdk-tingwu-1.0.6/aliyunsdktingwu/
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-15 03:17:55.000000 aliyun-python-sdk-tingwu-1.0.6/aliyunsdktingwu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 03:17:55.000000 aliyun-python-sdk-tingwu-1.0.6/aliyunsdktingwu/request/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 03:17:55.000000 aliyun-python-sdk-tingwu-1.0.6/aliyunsdktingwu/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 03:17:55.000000 aliyun-python-sdk-tingwu-1.0.6/aliyunsdktingwu/request/v20230930/
--rw-r--r--   0 root         (0) root         (0)     1573 2024-05-15 03:17:55.000000 aliyun-python-sdk-tingwu-1.0.6/aliyunsdktingwu/request/v20230930/CreateTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1278 2024-05-15 03:17:55.000000 aliyun-python-sdk-tingwu-1.0.6/aliyunsdktingwu/request/v20230930/CreateTranscriptionPhrasesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1314 2024-05-15 03:17:55.000000 aliyun-python-sdk-tingwu-1.0.6/aliyunsdktingwu/request/v20230930/DeleteTranscriptionPhrasesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1255 2024-05-15 03:17:55.000000 aliyun-python-sdk-tingwu-1.0.6/aliyunsdktingwu/request/v20230930/GetTaskInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1305 2024-05-15 03:17:55.000000 aliyun-python-sdk-tingwu-1.0.6/aliyunsdktingwu/request/v20230930/GetTranscriptionPhrasesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1119 2024-05-15 03:17:55.000000 aliyun-python-sdk-tingwu-1.0.6/aliyunsdktingwu/request/v20230930/ListTranscriptionPhrasesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1465 2024-05-15 03:17:55.000000 aliyun-python-sdk-tingwu-1.0.6/aliyunsdktingwu/request/v20230930/UpdateTranscriptionPhrasesRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 03:17:55.000000 aliyun-python-sdk-tingwu-1.0.6/aliyunsdktingwu/request/v20230930/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2024-05-15 03:17:55.000000 aliyun-python-sdk-tingwu-1.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2467 2024-05-15 03:17:55.000000 aliyun-python-sdk-tingwu-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 07:19:04.000000 aliyun-python-sdk-tingwu-1.0.7/
+-rw-r--r--   0 root         (0) root         (0)      575 2024-05-17 07:19:03.000000 aliyun-python-sdk-tingwu-1.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-17 07:19:03.000000 aliyun-python-sdk-tingwu-1.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1552 2024-05-17 07:19:04.000000 aliyun-python-sdk-tingwu-1.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      533 2024-05-17 07:19:03.000000 aliyun-python-sdk-tingwu-1.0.7/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 07:19:04.000000 aliyun-python-sdk-tingwu-1.0.7/aliyun_python_sdk_tingwu.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1552 2024-05-17 07:19:04.000000 aliyun-python-sdk-tingwu-1.0.7/aliyun_python_sdk_tingwu.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      859 2024-05-17 07:19:04.000000 aliyun-python-sdk-tingwu-1.0.7/aliyun_python_sdk_tingwu.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 07:19:04.000000 aliyun-python-sdk-tingwu-1.0.7/aliyun_python_sdk_tingwu.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-17 07:19:04.000000 aliyun-python-sdk-tingwu-1.0.7/aliyun_python_sdk_tingwu.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-17 07:19:04.000000 aliyun-python-sdk-tingwu-1.0.7/aliyun_python_sdk_tingwu.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 07:19:04.000000 aliyun-python-sdk-tingwu-1.0.7/aliyunsdktingwu/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-17 07:19:03.000000 aliyun-python-sdk-tingwu-1.0.7/aliyunsdktingwu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 07:19:04.000000 aliyun-python-sdk-tingwu-1.0.7/aliyunsdktingwu/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 07:19:03.000000 aliyun-python-sdk-tingwu-1.0.7/aliyunsdktingwu/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 07:19:04.000000 aliyun-python-sdk-tingwu-1.0.7/aliyunsdktingwu/request/v20230930/
+-rw-r--r--   0 root         (0) root         (0)     1573 2024-05-17 07:19:03.000000 aliyun-python-sdk-tingwu-1.0.7/aliyunsdktingwu/request/v20230930/CreateTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2024-05-17 07:19:03.000000 aliyun-python-sdk-tingwu-1.0.7/aliyunsdktingwu/request/v20230930/CreateTranscriptionPhrasesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2024-05-17 07:19:03.000000 aliyun-python-sdk-tingwu-1.0.7/aliyunsdktingwu/request/v20230930/DeleteTranscriptionPhrasesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2024-05-17 07:19:03.000000 aliyun-python-sdk-tingwu-1.0.7/aliyunsdktingwu/request/v20230930/GetTaskInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1305 2024-05-17 07:19:03.000000 aliyun-python-sdk-tingwu-1.0.7/aliyunsdktingwu/request/v20230930/GetTranscriptionPhrasesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1119 2024-05-17 07:19:03.000000 aliyun-python-sdk-tingwu-1.0.7/aliyunsdktingwu/request/v20230930/ListTranscriptionPhrasesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2024-05-17 07:19:03.000000 aliyun-python-sdk-tingwu-1.0.7/aliyunsdktingwu/request/v20230930/UpdateTranscriptionPhrasesRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 07:19:03.000000 aliyun-python-sdk-tingwu-1.0.7/aliyunsdktingwu/request/v20230930/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2024-05-17 07:19:04.000000 aliyun-python-sdk-tingwu-1.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2467 2024-05-17 07:19:03.000000 aliyun-python-sdk-tingwu-1.0.7/setup.py
```

### Comparing `aliyun-python-sdk-tingwu-1.0.6/LICENSE` & `aliyun-python-sdk-tingwu-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tingwu-1.0.6/PKG-INFO` & `aliyun-python-sdk-tingwu-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-tingwu
-Version: 1.0.6
+Version: 1.0.7
 Summary: The tingwu module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-tingwu
```

### Comparing `aliyun-python-sdk-tingwu-1.0.6/README.rst` & `aliyun-python-sdk-tingwu-1.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tingwu-1.0.6/aliyun_python_sdk_tingwu.egg-info/PKG-INFO` & `aliyun-python-sdk-tingwu-1.0.7/aliyun_python_sdk_tingwu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-tingwu
-Version: 1.0.6
+Version: 1.0.7
 Summary: The tingwu module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-tingwu
```

### Comparing `aliyun-python-sdk-tingwu-1.0.6/aliyun_python_sdk_tingwu.egg-info/SOURCES.txt` & `aliyun-python-sdk-tingwu-1.0.7/aliyun_python_sdk_tingwu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tingwu-1.0.6/aliyunsdktingwu/request/v20230930/CreateTaskRequest.py` & `aliyun-python-sdk-tingwu-1.0.7/aliyunsdktingwu/request/v20230930/CreateTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tingwu-1.0.6/aliyunsdktingwu/request/v20230930/CreateTranscriptionPhrasesRequest.py` & `aliyun-python-sdk-tingwu-1.0.7/aliyunsdktingwu/request/v20230930/CreateTranscriptionPhrasesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tingwu-1.0.6/aliyunsdktingwu/request/v20230930/DeleteTranscriptionPhrasesRequest.py` & `aliyun-python-sdk-tingwu-1.0.7/aliyunsdktingwu/request/v20230930/DeleteTranscriptionPhrasesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tingwu-1.0.6/aliyunsdktingwu/request/v20230930/GetTaskInfoRequest.py` & `aliyun-python-sdk-tingwu-1.0.7/aliyunsdktingwu/request/v20230930/GetTaskInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tingwu-1.0.6/aliyunsdktingwu/request/v20230930/GetTranscriptionPhrasesRequest.py` & `aliyun-python-sdk-tingwu-1.0.7/aliyunsdktingwu/request/v20230930/GetTranscriptionPhrasesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tingwu-1.0.6/aliyunsdktingwu/request/v20230930/ListTranscriptionPhrasesRequest.py` & `aliyun-python-sdk-tingwu-1.0.7/aliyunsdktingwu/request/v20230930/ListTranscriptionPhrasesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tingwu-1.0.6/aliyunsdktingwu/request/v20230930/UpdateTranscriptionPhrasesRequest.py` & `aliyun-python-sdk-tingwu-1.0.7/aliyunsdktingwu/request/v20230930/UpdateTranscriptionPhrasesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tingwu-1.0.6/setup.py` & `aliyun-python-sdk-tingwu-1.0.7/setup.py`

 * *Files identical despite different names*

