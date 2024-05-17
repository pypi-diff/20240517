# Comparing `tmp/zorch-0.0.8.tar.gz` & `tmp/zorch-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zorch-0.0.8.tar", last modified: Fri May 17 06:20:01 2024, max compression
+gzip compressed data, was "zorch-0.0.9.tar", last modified: Fri May 17 06:11:40 2024, max compression
```

## Comparing `zorch-0.0.8.tar` & `zorch-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 zwhy      (1000) zwhy      (1000)        0 2024-05-17 06:20:01.409493 zorch-0.0.8/
--rw-r--r--   0 zwhy      (1000) zwhy      (1000)      162 2024-05-17 06:20:01.405493 zorch-0.0.8/PKG-INFO
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)       38 2024-05-17 06:20:01.409493 zorch-0.0.8/setup.cfg
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)      688 2024-05-17 06:14:06.000000 zorch-0.0.8/setup.py
-drwxrwxr-x   0 zwhy      (1000) zwhy      (1000)        0 2024-05-17 06:20:01.405493 zorch-0.0.8/zorch/
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)       22 2024-05-17 06:20:01.000000 zorch-0.0.8/zorch/__init__.py
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)        0 2024-05-16 07:24:14.000000 zorch-0.0.8/zorch/postprocess.py
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)      458 2024-05-16 09:58:45.000000 zorch-0.0.8/zorch/preprocess.py
-drwxrwxr-x   0 zwhy      (1000) zwhy      (1000)        0 2024-05-17 06:20:01.405493 zorch-0.0.8/zorch.egg-info/
--rw-r--r--   0 zwhy      (1000) zwhy      (1000)      162 2024-05-17 06:20:01.000000 zorch-0.0.8/zorch.egg-info/PKG-INFO
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)      183 2024-05-17 06:20:01.000000 zorch-0.0.8/zorch.egg-info/SOURCES.txt
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)        1 2024-05-17 06:20:01.000000 zorch-0.0.8/zorch.egg-info/dependency_links.txt
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)        6 2024-05-17 06:20:01.000000 zorch-0.0.8/zorch.egg-info/top_level.txt
+drwxrwxr-x   0 zwhy      (1000) zwhy      (1000)        0 2024-05-17 06:11:40.242652 zorch-0.0.9/
+-rw-r--r--   0 zwhy      (1000) zwhy      (1000)      162 2024-05-17 06:11:40.242652 zorch-0.0.9/PKG-INFO
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)       38 2024-05-17 06:11:40.242652 zorch-0.0.9/setup.cfg
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)     1247 2024-05-17 06:11:38.000000 zorch-0.0.9/setup.py
+drwxrwxr-x   0 zwhy      (1000) zwhy      (1000)        0 2024-05-17 06:11:40.242652 zorch-0.0.9/zorch/
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)       22 2024-05-17 06:11:40.000000 zorch-0.0.9/zorch/__init__.py
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)        0 2024-05-16 07:24:14.000000 zorch-0.0.9/zorch/postprocess.py
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)      458 2024-05-16 09:58:45.000000 zorch-0.0.9/zorch/preprocess.py
+drwxrwxr-x   0 zwhy      (1000) zwhy      (1000)        0 2024-05-17 06:11:40.242652 zorch-0.0.9/zorch.egg-info/
+-rw-r--r--   0 zwhy      (1000) zwhy      (1000)      162 2024-05-17 06:11:40.000000 zorch-0.0.9/zorch.egg-info/PKG-INFO
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)      183 2024-05-17 06:11:40.000000 zorch-0.0.9/zorch.egg-info/SOURCES.txt
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)        1 2024-05-17 06:11:40.000000 zorch-0.0.9/zorch.egg-info/dependency_links.txt
+-rw-rw-r--   0 zwhy      (1000) zwhy      (1000)        6 2024-05-17 06:11:40.000000 zorch-0.0.9/zorch.egg-info/top_level.txt
```

### Comparing `zorch-0.0.8/setup.py` & `zorch-0.0.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,35 @@
 import re
 from setuptools import setup, find_packages
 
-# 读取当前版本号
-with open('./zorch/__init__.py', 'r') as f:
-    version_line = f.read()
-    match = re.search(r'__version__ = \'(\d+\.\d+\.\d+)\'', version_line)
-    if not match:
-        raise ValueError("Unable to find version string")
-    version = match.group(1)
+def increment_version():
+    # 读取文件
+    with open('./zorch/__init__.py', 'r') as f:
+        # 找到对应的版本号
+        version_line = f.read()
+        match = re.search(r'__version__ = \'(\d+\.\d+\.\d+)\'', version_line)
+       
+        if not match:
+            raise ValueError("Unable to find version string")
+
+        # 解析版本号的部分
+        major, minor, patch = map(int, match.group(1).split('.'))
+        # 增加 PATCH 部分
+        patch += 1
+        # 重建版本号字符串
+        new_version = f"{major}.{minor}.{patch}"
+
+    # 重新打开文件以写入模式
+    with open('./zorch/__init__.py', 'w') as f:
+        # 写入到原始位置,不修改其他内容
+        f.write("__version__ = '{}'\n".format(new_version))
+        
+    return new_version
+    
+version = increment_version()
 
 print("zorch version:", version)
 
 setup(
     name='zorch',
     version=version,
     author='zwhy',
```

