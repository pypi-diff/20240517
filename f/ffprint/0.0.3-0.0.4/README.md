# Comparing `tmp/ffprint-0.0.3.tar.gz` & `tmp/ffprint-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\001_coding\feifei\my_pypi\ffprint\dist\.tmp-6ioosdq3\ffprint-0.0.3.tar", last modified: Fri May 17 08:52:36 2024, max compression
+gzip compressed data, was "D:\001_coding\feifei\my_pypi\ffprint\dist\.tmp-k3xftmwv\ffprint-0.0.4.tar", last modified: Fri May 17 12:16:23 2024, max compression
```

## Comparing `ffprint-0.0.3.tar` & `ffprint-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 08:52:36.000000 ffprint-0.0.3/
--rw-rw-rw-   0        0        0     1093 2024-05-17 05:38:27.000000 ffprint-0.0.3/LICENSE.license
--rw-rw-rw-   0        0        0      308 2024-05-17 08:52:36.000000 ffprint-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       80 2024-05-17 05:40:49.000000 ffprint-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-17 08:52:36.000000 ffprint-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1259 2024-05-17 08:52:29.000000 ffprint-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 08:52:36.000000 ffprint-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-17 08:52:36.000000 ffprint-0.0.3/src/ffprint/
--rw-rw-rw-   0        0        0       23 2024-05-17 08:29:24.000000 ffprint-0.0.3/src/ffprint/__init__.py
--rw-rw-rw-   0        0        0      884 2024-05-17 08:39:45.000000 ffprint-0.0.3/src/ffprint/core.py
-drwxrwxrwx   0        0        0        0 2024-05-17 08:52:36.000000 ffprint-0.0.3/src/ffprint.egg-info/
--rw-rw-rw-   0        0        0      308 2024-05-17 08:52:36.000000 ffprint-0.0.3/src/ffprint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2024-05-17 08:52:36.000000 ffprint-0.0.3/src/ffprint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 08:52:36.000000 ffprint-0.0.3/src/ffprint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-17 08:52:36.000000 ffprint-0.0.3/src/ffprint.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-17 08:52:36.000000 ffprint-0.0.3/src/ffprint.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 12:16:23.000000 ffprint-0.0.4/
+-rw-rw-rw-   0        0        0     1093 2024-05-17 05:38:27.000000 ffprint-0.0.4/LICENSE.license
+-rw-rw-rw-   0        0        0      316 2024-05-17 12:16:23.000000 ffprint-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       80 2024-05-17 05:40:49.000000 ffprint-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-17 12:16:23.000000 ffprint-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1259 2024-05-17 12:15:22.000000 ffprint-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 12:16:23.000000 ffprint-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 12:16:23.000000 ffprint-0.0.4/src/ffprint/
+-rw-rw-rw-   0        0        0       36 2024-05-17 12:06:26.000000 ffprint-0.0.4/src/ffprint/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 12:16:23.000000 ffprint-0.0.4/src/ffprint.egg-info/
+-rw-rw-rw-   0        0        0      316 2024-05-17 12:16:23.000000 ffprint-0.0.4/src/ffprint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2024-05-17 12:16:23.000000 ffprint-0.0.4/src/ffprint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 12:16:23.000000 ffprint-0.0.4/src/ffprint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-17 12:16:23.000000 ffprint-0.0.4/src/ffprint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-17 12:16:23.000000 ffprint-0.0.4/src/ffprint.egg-info/top_level.txt
```

### Comparing `ffprint-0.0.3/LICENSE.license` & `ffprint-0.0.4/LICENSE.license`

 * *Files identical despite different names*

### Comparing `ffprint-0.0.3/setup.py` & `ffprint-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,18 +4,18 @@
     long_description = f.read()
 
 with open(r'D:\001_coding\feifei\my_pypi\ffprint\requirements.txt', "r", encoding="utf-8") as f:
     required = f.read().splitlines()
 
 setup(
     name="ffprint",                               # 包名
-    version="0.0.3",                                 # 版本号
+    version="0.0.4",                                 # 版本号
     author="eric.gao",                               # 作者
     author_email="18655035787@163.com",              # 邮箱
-    description="self print",                        # 简短描述
+    description="self-defined print",                # 简短描述
     long_description=long_description,               # 详细说明
     long_description_content_type="text/markdown",   # 详细说明使用标记类型
     # url="https://github.com/",                     # 项目主页
     packages=find_packages(where="src"),             # 需要打包的部分
     package_dir={"": "src"},                         # 设置src目录为根目录
     python_requires=">=3.6",                         # 项目支持的Python版本
     install_requires=required,                       # 项目必须的依赖
```

