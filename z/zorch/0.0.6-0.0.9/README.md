# Comparing `tmp/zorch-0.0.6.tar.gz` & `tmp/zorch-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zorch-0.0.6.tar", last modified: Fri May 17 06:10:00 2024, max compression
+gzip compressed data, was "zorch-0.0.9.tar", last modified: Fri May 17 06:11:40 2024, max compression
```

## Comparing `zorch-0.0.6.tar` & `zorch-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 zwhy      (1000) zwhy      (1000)        0 2024-05-17 06:10:00.380265 zorch-0.0.6/
--rw-r--r--   0 zwhy      (1000) zwhy      (1000)      162 2024-05-17 06:10:00.380265 zorch-0.0.6/PKG-INFO
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)       38 2024-05-17 06:10:00.380265 zorch-0.0.6/setup.cfg
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)     1416 2024-05-17 05:58:06.000000 zorch-0.0.6/setup.py
-drwxrwxr-x   0 zwhy      (1000) zwhy      (1000)        0 2024-05-17 06:10:00.380265 zorch-0.0.6/zorch/
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)       22 2024-05-17 06:10:00.000000 zorch-0.0.6/zorch/__init__.py
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)        0 2024-05-16 07:24:14.000000 zorch-0.0.6/zorch/postprocess.py
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)      458 2024-05-16 09:58:45.000000 zorch-0.0.6/zorch/preprocess.py
-drwxrwxr-x   0 zwhy      (1000) zwhy      (1000)        0 2024-05-17 06:10:00.380265 zorch-0.0.6/zorch.egg-info/
--rw-r--r--   0 zwhy      (1000) zwhy      (1000)      162 2024-05-17 06:10:00.000000 zorch-0.0.6/zorch.egg-info/PKG-INFO
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)      183 2024-05-17 06:10:00.000000 zorch-0.0.6/zorch.egg-info/SOURCES.txt
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)        1 2024-05-17 06:10:00.000000 zorch-0.0.6/zorch.egg-info/dependency_links.txt
--rw-rw-r--   0 zwhy      (1000) zwhy      (1000)        6 2024-05-17 06:10:00.000000 zorch-0.0.6/zorch.egg-info/top_level.txt
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

### Comparing `zorch-0.0.6/setup.py` & `zorch-0.0.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,46 @@
-
 import re
 from setuptools import setup, find_packages
 
-
 def increment_version():
     # 读取文件
     with open('./zorch/__init__.py', 'r') as f:
-        # 找到 对应的版本号
-        version_line = f.read()  #
-        match = re.search(r'(\d+\.\d+\.\d+)', version_line)
+        # 找到对应的版本号
+        version_line = f.read()
+        match = re.search(r'__version__ = \'(\d+\.\d+\.\d+)\'', version_line)
        
         if not match:
             raise ValueError("Unable to find version string")
 
         # 解析版本号的部分
-        major, minor, patch = map(int,match.group(1).split('.'))
+        major, minor, patch = map(int, match.group(1).split('.'))
         # 增加 PATCH 部分
         patch += 1
         # 重建版本号字符串
         new_version = f"{major}.{minor}.{patch}"
 
     # 重新打开文件以写入模式
     with open('./zorch/__init__.py', 'w') as f:
         # 写入到原始位置,不修改其他内容
         f.write("__version__ = '{}'\n".format(new_version))
         
     return new_version
     
 version = increment_version()
 
-
-print("zorch version:", type(version), version)
+print("zorch version:", version)
 
 setup(
     name='zorch',
     version=version,
     author='zwhy',
     author_email='zwhy2025@gmail.com',
     description='A brief description of the package',
-    # long_description=open('README.md').read(),
-    # long_description_content_type='text/markdown',
-    # url='https://github.com/yourusername/your_package_name',
     packages=find_packages(),
     install_requires=[
         # 依赖列表
     ],
     classifiers=[
         # 分类器列表
     ],
     python_requires='>=3.9',
 )
-
```

