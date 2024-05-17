# Comparing `tmp/qtmodel-0.3.3.tar.gz` & `tmp/qtmodel-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtmodel-0.3.3.tar", last modified: Thu May 16 02:38:25 2024, max compression
+gzip compressed data, was "qtmodel-0.3.4.tar", last modified: Fri May 17 07:11:14 2024, max compression
```

## Comparing `qtmodel-0.3.3.tar` & `qtmodel-0.3.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 02:38:25.225954 qtmodel-0.3.3/
--rw-rw-rw-   0        0        0    37701 2024-05-16 02:38:25.224593 qtmodel-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0    37273 2024-05-13 05:54:03.000000 qtmodel-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 02:38:25.217157 qtmodel-0.3.3/qtmodel/
--rw-rw-rw-   0        0        0       93 2024-05-15 02:13:58.000000 qtmodel-0.3.3/qtmodel/__init__.py
--rw-rw-rw-   0        0        0    83827 2024-05-16 02:19:25.000000 qtmodel-0.3.3/qtmodel/qt_mdb.py
--rw-rw-rw-   0        0        0     5547 2024-05-16 02:10:32.000000 qtmodel-0.3.3/qtmodel/qt_odb.py
--rw-rw-rw-   0        0        0     1029 2024-05-16 02:05:34.000000 qtmodel-0.3.3/qtmodel/qt_operate.py
--rw-rw-rw-   0        0        0     3891 2024-05-16 02:31:35.000000 qtmodel-0.3.3/qtmodel/res_db.py
-drwxrwxrwx   0        0        0        0 2024-05-16 02:38:25.223243 qtmodel-0.3.3/qtmodel.egg-info/
--rw-rw-rw-   0        0        0    37701 2024-05-16 02:38:24.000000 qtmodel-0.3.3/qtmodel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-16 02:38:25.000000 qtmodel-0.3.3/qtmodel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 02:38:24.000000 qtmodel-0.3.3/qtmodel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-16 02:38:24.000000 qtmodel-0.3.3/qtmodel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 02:38:25.225954 qtmodel-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      758 2024-05-16 02:38:18.000000 qtmodel-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 07:11:14.711145 qtmodel-0.3.4/
+-rw-rw-rw-   0        0        0    37701 2024-05-17 07:11:14.711145 qtmodel-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0    37273 2024-05-13 05:54:03.000000 qtmodel-0.3.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 07:11:14.702908 qtmodel-0.3.4/qtmodel/
+-rw-rw-rw-   0        0        0       91 2024-05-17 07:08:34.000000 qtmodel-0.3.4/qtmodel/__init__.py
+-rw-rw-rw-   0        0        0    83827 2024-05-16 02:19:25.000000 qtmodel-0.3.4/qtmodel/qt_mdb.py
+-rw-rw-rw-   0        0        0     8492 2024-05-17 07:07:31.000000 qtmodel-0.3.4/qtmodel/qt_odb.py
+-rw-rw-rw-   0        0        0     1029 2024-05-17 05:05:06.000000 qtmodel-0.3.4/qtmodel/qt_operate.py
+-rw-rw-rw-   0        0        0     9890 2024-05-17 07:07:30.000000 qtmodel-0.3.4/qtmodel/res_db.py
+drwxrwxrwx   0        0        0        0 2024-05-17 07:11:14.708909 qtmodel-0.3.4/qtmodel.egg-info/
+-rw-rw-rw-   0        0        0    37701 2024-05-17 07:11:14.000000 qtmodel-0.3.4/qtmodel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-17 07:11:14.000000 qtmodel-0.3.4/qtmodel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 07:11:14.000000 qtmodel-0.3.4/qtmodel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-17 07:11:14.000000 qtmodel-0.3.4/qtmodel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 07:11:14.711145 qtmodel-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      758 2024-05-17 07:11:08.000000 qtmodel-0.3.4/setup.py
```

### Comparing `qtmodel-0.3.3/PKG-INFO` & `qtmodel-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtmodel
-Version: 0.3.3
+Version: 0.3.4
 Summary: python modeling for qt  24/05/06 
 Home-page: https://github.com/Inface0443/pyqt
 Author: dqy-zhj
 Author-email: 1105417715@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qtmodel-0.3.3/README.md` & `qtmodel-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `qtmodel-0.3.3/qtmodel/qt_mdb.py` & `qtmodel-0.3.4/qtmodel/qt_mdb.py`

 * *Files identical despite different names*

### Comparing `qtmodel-0.3.3/qtmodel/qt_operate.py` & `qtmodel-0.3.4/qtmodel/qt_operate.py`

 * *Files identical despite different names*

### Comparing `qtmodel-0.3.3/qtmodel.egg-info/PKG-INFO` & `qtmodel-0.3.4/qtmodel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtmodel
-Version: 0.3.3
+Version: 0.3.4
 Summary: python modeling for qt  24/05/06 
 Home-page: https://github.com/Inface0443/pyqt
 Author: dqy-zhj
 Author-email: 1105417715@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qtmodel-0.3.3/setup.py` & `qtmodel-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # 读取文件内容
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="qtmodel",
-    version="0.3.3",
+    version="0.3.4",
     author="dqy-zhj",
     author_email="1105417715@qq.com",
     description="python modeling for qt  24/05/06 ",
     long_description=long_description,  # 使用读取的 README.md 文件内容
     long_description_content_type="text/markdown",  # 指明内容格式为markdown
     url="https://github.com/Inface0443/pyqt",
     packages=find_packages(),
```

