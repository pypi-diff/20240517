# Comparing `tmp/ffprint-0.0.1.tar.gz` & `tmp/ffprint-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\001_coding\feifei\my_pypi\ffprint\dist\.tmp-9j56wmkj\ffprint-0.0.1.tar", last modified: Fri May 17 05:54:25 2024, max compression
+gzip compressed data, was "dist\ffprint-0.0.2.tar", last modified: Fri May 17 07:50:10 2024, max compression
```

## Comparing `ffprint-0.0.1.tar` & `ffprint-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 05:54:25.000000 ffprint-0.0.1/
--rw-rw-rw-   0        0        0     1093 2024-05-17 05:38:27.000000 ffprint-0.0.1/LICENSE.license
--rw-rw-rw-   0        0        0      308 2024-05-17 05:54:25.000000 ffprint-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       80 2024-05-17 05:40:49.000000 ffprint-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-17 05:54:25.000000 ffprint-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1225 2024-05-17 05:50:51.000000 ffprint-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 05:54:25.000000 ffprint-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-17 05:54:25.000000 ffprint-0.0.1/src/ffprint.egg-info/
--rw-rw-rw-   0        0        0      308 2024-05-17 05:54:25.000000 ffprint-0.0.1/src/ffprint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2024-05-17 05:54:25.000000 ffprint-0.0.1/src/ffprint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 05:54:25.000000 ffprint-0.0.1/src/ffprint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-17 05:54:25.000000 ffprint-0.0.1/src/ffprint.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-17 05:54:25.000000 ffprint-0.0.1/src/module/
--rw-rw-rw-   0        0        0        0 2024-05-17 05:36:37.000000 ffprint-0.0.1/src/module/__init__.py
--rw-rw-rw-   0        0        0      883 2024-05-17 05:52:31.000000 ffprint-0.0.1/src/module/core.py
+drwxrwxrwx   0        0        0        0 2024-05-17 07:50:10.000000 ffprint-0.0.2/
+-rw-rw-rw-   0        0        0     1093 2024-05-17 05:38:27.000000 ffprint-0.0.2/LICENSE.license
+-rw-rw-rw-   0        0        0      308 2024-05-17 07:50:10.000000 ffprint-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       80 2024-05-17 05:40:49.000000 ffprint-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-17 07:50:10.000000 ffprint-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1225 2024-05-17 07:46:49.000000 ffprint-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 07:50:10.000000 ffprint-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 07:50:10.000000 ffprint-0.0.2/src/ffprint/
+-rw-rw-rw-   0        0        0        0 2024-05-17 05:36:37.000000 ffprint-0.0.2/src/ffprint/__init__.py
+-rw-rw-rw-   0        0        0      883 2024-05-17 05:52:31.000000 ffprint-0.0.2/src/ffprint/core.py
+drwxrwxrwx   0        0        0        0 2024-05-17 07:50:10.000000 ffprint-0.0.2/src/ffprint.egg-info/
+-rw-rw-rw-   0        0        0      308 2024-05-17 07:50:10.000000 ffprint-0.0.2/src/ffprint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-05-17 07:50:10.000000 ffprint-0.0.2/src/ffprint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 07:50:10.000000 ffprint-0.0.2/src/ffprint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-17 07:50:10.000000 ffprint-0.0.2/src/ffprint.egg-info/top_level.txt
```

### Comparing `ffprint-0.0.1/LICENSE.license` & `ffprint-0.0.2/LICENSE.license`

 * *Files identical despite different names*

### Comparing `ffprint-0.0.1/setup.py` & `ffprint-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 # with open('requirements.txt', "r", encoding="utf-8") as f:
 #     required = f.read().splitlines()
 
 setup(
     name="ffprint",                               # 包名
-    version="0.0.1",                                 # 版本号
+    version="0.0.2",                                 # 版本号
     author="eric.gao",                               # 作者
     author_email="18655035787@163.com",              # 邮箱
     description="self print",                        # 简短描述
     long_description=long_description,               # 详细说明
     long_description_content_type="text/markdown",   # 详细说明使用标记类型
     # url="https://github.com/",                     # 项目主页
     packages=find_packages(where="src"),             # 需要打包的部分
```

### Comparing `ffprint-0.0.1/src/module/core.py` & `ffprint-0.0.2/src/ffprint/core.py`

 * *Files identical despite different names*

