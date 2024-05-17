# Comparing `tmp/openi-1.2.2.tar.gz` & `tmp/openi-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-1.2.2.tar", last modified: Fri Sep 15 06:12:00 2023, max compression
+gzip compressed data, was "openi-1.3.0.tar", last modified: Tue Feb 27 09:05:36 2024, max compression
```

## Comparing `openi-1.2.2.tar` & `openi-1.3.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-09-15 06:12:00.297921 openi-1.2.2/
--rw-rw-rw-   0        0        0     3004 2023-09-15 06:12:00.296909 openi-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2368 2023-09-06 09:50:51.000000 openi-1.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-09-15 06:12:00.297921 openi-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1015 2023-09-15 01:48:36.000000 openi-1.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-09-15 06:12:00.251583 openi-1.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-09-15 06:12:00.258571 openi-1.2.2/src/openi/
--rw-rw-rw-   0        0        0      140 2023-09-15 03:57:43.000000 openi-1.2.2/src/openi/__init__.py
--rw-rw-rw-   0        0        0    13681 2023-09-15 03:18:05.000000 openi-1.2.2/src/openi/apis.py
--rw-rw-rw-   0        0        0     7584 2023-09-06 09:50:51.000000 openi-1.2.2/src/openi/cli.py
-drwxrwxrwx   0        0        0        0 2023-09-15 06:12:00.268570 openi-1.2.2/src/openi/dataset/
--rw-rw-rw-   0        0        0       48 2023-09-06 09:50:51.000000 openi-1.2.2/src/openi/dataset/__init__.py
--rw-rw-rw-   0        0        0     2852 2023-09-15 04:07:33.000000 openi-1.2.2/src/openi/dataset/download.py
--rw-rw-rw-   0        0        0     2271 2023-09-15 04:05:18.000000 openi-1.2.2/src/openi/dataset/upload.py
--rw-rw-rw-   0        0        0     3109 2023-09-06 09:50:51.000000 openi-1.2.2/src/openi/login.py
-drwxrwxrwx   0        0        0        0 2023-09-15 06:12:00.269568 openi-1.2.2/src/openi/model/
--rw-rw-rw-   0        0        0       48 2023-09-06 09:50:51.000000 openi-1.2.2/src/openi/model/__init__.py
--rw-rw-rw-   0        0        0     4951 2023-09-15 04:02:53.000000 openi-1.2.2/src/openi/model/download.py
--rw-rw-rw-   0        0        0     5461 2023-09-15 04:07:58.000000 openi-1.2.2/src/openi/model/upload.py
-drwxrwxrwx   0        0        0        0 2023-09-15 06:12:00.294224 openi-1.2.2/src/openi/services/
--rw-rw-rw-   0        0        0      182 2023-09-06 09:50:51.000000 openi-1.2.2/src/openi/services/__init__.py
--rw-rw-rw-   0        0        0     2262 2023-09-06 09:50:51.000000 openi-1.2.2/src/openi/services/dataset_struct.py
--rw-rw-rw-   0        0        0     3552 2023-09-15 04:02:50.000000 openi-1.2.2/src/openi/services/file_download.py
--rw-rw-rw-   0        0        0     1479 2023-09-15 01:48:54.000000 openi-1.2.2/src/openi/services/file_progress_bar.py
--rw-rw-rw-   0        0        0    10217 2023-09-15 06:11:05.000000 openi-1.2.2/src/openi/services/file_upload.py
--rw-rw-rw-   0        0        0     2857 2023-09-06 09:50:51.000000 openi-1.2.2/src/openi/services/model_struct.py
--rw-rw-rw-   0        0        0     2725 2023-09-12 01:14:06.000000 openi-1.2.2/src/openi/services/repo_struct.py
-drwxrwxrwx   0        0        0        0 2023-09-15 06:12:00.296909 openi-1.2.2/src/openi/utils/
--rw-rw-rw-   0        0        0       49 2023-09-06 09:50:51.000000 openi-1.2.2/src/openi/utils/__init__.py
--rw-rw-rw-   0        0        0     5819 2023-09-06 09:50:51.000000 openi-1.2.2/src/openi/utils/constants.py
--rw-rw-rw-   0        0        0     1956 2023-09-06 09:50:51.000000 openi-1.2.2/src/openi/utils/logger.py
-drwxrwxrwx   0        0        0        0 2023-09-15 06:12:00.263568 openi-1.2.2/src/openi.egg-info/
--rw-rw-rw-   0        0        0     3004 2023-09-15 06:12:00.000000 openi-1.2.2/src/openi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      794 2023-09-15 06:12:00.000000 openi-1.2.2/src/openi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-15 06:12:00.000000 openi-1.2.2/src/openi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-09-15 06:12:00.000000 openi-1.2.2/src/openi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-09-15 06:12:00.000000 openi-1.2.2/src/openi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-09-15 06:12:00.000000 openi-1.2.2/src/openi.egg-info/top_level.txt
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2024-02-27 09:05:36.226088 openi-1.3.0/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2919 2024-02-27 09:05:36.225925 openi-1.3.0/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2301 2023-10-30 08:41:14.000000 openi-1.3.0/README.md
+-rw-r--r--   0 jochen10518   (501) staff       (20)       38 2024-02-27 09:05:36.226143 openi-1.3.0/setup.cfg
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1027 2024-02-27 09:05:19.000000 openi-1.3.0/setup.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2024-02-27 09:05:36.221337 openi-1.3.0/src/
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2024-02-27 09:05:36.222427 openi-1.3.0/src/openi/
+-rw-r--r--   0 jochen10518   (501) staff       (20)      116 2024-02-02 09:40:48.000000 openi-1.3.0/src/openi/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     3029 2024-02-02 09:40:48.000000 openi-1.3.0/src/openi/_login.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)    13205 2024-02-01 09:36:13.000000 openi-1.3.0/src/openi/apis.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     7414 2024-02-02 09:40:48.000000 openi-1.3.0/src/openi/cli.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2024-02-27 09:05:36.223752 openi-1.3.0/src/openi/dataset/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       46 2023-08-25 03:48:07.000000 openi-1.3.0/src/openi/dataset/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2679 2024-02-02 09:40:48.000000 openi-1.3.0/src/openi/dataset/download.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1815 2024-02-02 09:40:48.000000 openi-1.3.0/src/openi/dataset/upload.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2024-02-27 09:05:36.224245 openi-1.3.0/src/openi/model/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       46 2023-08-25 03:48:00.000000 openi-1.3.0/src/openi/model/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     4864 2023-10-30 01:51:32.000000 openi-1.3.0/src/openi/model/download.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     5237 2024-02-06 09:04:29.000000 openi-1.3.0/src/openi/model/upload.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2024-02-27 09:05:36.225233 openi-1.3.0/src/openi/services/
+-rw-r--r--   0 jochen10518   (501) staff       (20)      175 2023-08-25 03:22:07.000000 openi-1.3.0/src/openi/services/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2196 2023-08-31 11:41:27.000000 openi-1.3.0/src/openi/services/dataset_struct.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     3443 2023-10-30 01:51:32.000000 openi-1.3.0/src/openi/services/file_download.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1370 2024-02-02 09:40:48.000000 openi-1.3.0/src/openi/services/file_progress_bar.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)    10687 2024-02-06 09:04:29.000000 openi-1.3.0/src/openi/services/file_upload.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2741 2024-02-02 09:40:48.000000 openi-1.3.0/src/openi/services/model_struct.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2528 2024-02-02 09:40:48.000000 openi-1.3.0/src/openi/services/repo_struct.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2024-02-27 09:05:36.225689 openi-1.3.0/src/openi/utils/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       47 2023-08-25 03:22:16.000000 openi-1.3.0/src/openi/utils/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     4588 2024-02-02 09:40:48.000000 openi-1.3.0/src/openi/utils/constants.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1883 2023-08-31 11:41:27.000000 openi-1.3.0/src/openi/utils/logger.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2024-02-27 09:05:36.223358 openi-1.3.0/src/openi.egg-info/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2919 2024-02-27 09:05:36.000000 openi-1.3.0/src/openi.egg-info/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)      795 2024-02-27 09:05:36.000000 openi-1.3.0/src/openi.egg-info/SOURCES.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        1 2024-02-27 09:05:36.000000 openi-1.3.0/src/openi.egg-info/dependency_links.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)       41 2024-02-27 09:05:36.000000 openi-1.3.0/src/openi.egg-info/entry_points.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)       14 2024-02-27 09:05:36.000000 openi-1.3.0/src/openi.egg-info/requires.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        6 2024-02-27 09:05:36.000000 openi-1.3.0/src/openi.egg-info/top_level.txt
```

### Comparing `openi-1.2.2/PKG-INFO` & `openi-1.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-Metadata-Version: 2.1
-Name: openi
-Version: 1.2.2
-Summary: A package for openi pypi
-Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
-Author: chenzh05
-Author-email: chenzh.ds@outlook.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-# OpenI
-
-> PYPI package for 启智 AI 协作平台。
-
-## 安装
-
-_适配 python3.6 及以上版本_
-
-```bash
-pip install openi
-```
-
-## 功能介绍
-
-- 提供命令行与代码使用
-- 具体请参考 [帮助文档-API参考](https://openi.pcl.ac.cn/docs/index.html#/api/intro)
-
-```python
-from openi.dataset import download_file
-
-download_file(
-    file="my_data.zip",
-    repo_id="user1/repo1",
-    cluster="gpu",
-    save_path="local_path/",
-)
-
-""" output
-Complete( my_data.zip)(gpu): 100%|██████████████████████████████████████████| 22.0MB/22.0MB [00:01<00:00, 15.9MB/s]
-"""
-```
-
-```bash
->>> openi
-usage: openi {login, whoami, dataset, ...} [<args>] [-h]
-
-OpenI command line tool 启智AI协作平台命令行工具
-
-commands:
-  {login,logout,whoami,dataset,d,model,m}
-    login               使用令牌登录启智并保存到本机
-    logout              登出当前用户并删除本地令牌文件
-    whoami              查询当前登录用户
-    dataset (d)         {upload,download} 上传/下载启智AI协作平台的数据集
-    model (m)           {upload,download} 上传/下载启智AI协作平台的模型
-```
-
-```bash
->>> openi login
-
-
-             ██████╗   ██████╗  ███████╗  ███╗   ██╗  ██████╗
-            ██╔═══██╗  ██╔══██╗ ██╔════╝  ████╗  ██║    ██╔═╝
-            ██║   ██║  ██████╔╝ █████╗    ██╔██╗ ██║    ██║
-            ██║   ██║  ██╔═══╝  ██╔══╝    ██║╚██╗██║    ██║
-            ╚██████╔╝  ██║      ███████╗  ██║ ╚████║  ██████╗
-             ╚═════╝   ╚═╝      ╚══════╝  ╚═╝  ╚═══╝  ╚═════╝
-
-
-点击链接获取令牌并复制粘贴到下列输入栏 https://openi.pcl.ac.cn/user/settings/applications
-
-[WARNING] 若本机已存在登录令牌，本次输入的令牌会将其覆盖
-          粘贴前请先按 退格键⇦ 删除多余空格
-
-  🔒 token:
-
-```
+Metadata-Version: 2.1
+Name: openi
+Version: 1.3.0
+Summary: A package for openi pypi
+Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
+Author: chenzh05
+Author-email: chenzh.ds@outlook.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+# OpenI
+
+> PYPI package for 启智 AI 协作平台。
+
+## 安装
+
+_适配 python3.6 及以上版本_
+
+```bash
+pip install openi
+```
+
+## 功能介绍
+
+- 提供命令行与代码使用
+- 具体请参考 [帮助文档-API参考](https://openi.pcl.ac.cn/docs/index.html#/api/intro)
+
+```python
+from openi.dataset import download_file
+
+download_file(
+    file="my_data.zip",
+    repo_id="user1/repo1",
+    cluster="gpu",
+    save_path="local_path/",
+)
+
+""" output
+Complete( my_data.zip)(gpu): 100%|██████████████████████████████████████████| 22.0MB/22.0MB [00:01<00:00, 15.9MB/s]
+"""
+```
+
+```bash
+>>> openi
+usage: openi {login, whoami, dataset, ...} [<args>] [-h]
+
+OpenI command line tool 启智AI协作平台命令行工具
+
+commands:
+  {login,logout,whoami,dataset,d,model,m}
+    login               使用令牌登录启智并保存到本机
+    logout              登出当前用户并删除本地令牌文件
+    whoami              查询当前登录用户
+    dataset (d)         {upload,download} 上传/下载启智AI协作平台的数据集
+    model (m)           {upload,download} 上传/下载启智AI协作平台的模型
+```
+
+```bash
+>>> openi login
+
+
+             ██████╗   ██████╗  ███████╗  ███╗   ██╗  ██████╗
+            ██╔═══██╗  ██╔══██╗ ██╔════╝  ████╗  ██║    ██╔═╝
+            ██║   ██║  ██████╔╝ █████╗    ██╔██╗ ██║    ██║
+            ██║   ██║  ██╔═══╝  ██╔══╝    ██║╚██╗██║    ██║
+            ╚██████╔╝  ██║      ███████╗  ██║ ╚████║  ██████╗
+             ╚═════╝   ╚═╝      ╚══════╝  ╚═╝  ╚═══╝  ╚═════╝
+
+
+点击链接获取令牌并复制粘贴到下列输入栏 https://openi.pcl.ac.cn/user/settings/applications
+
+[WARNING] 若本机已存在登录令牌，本次输入的令牌会将其覆盖
+          粘贴前请先按 退格键⇦ 删除多余空格
+
+  🔒 token:
+
+```
```

### Comparing `openi-1.2.2/README.md` & `openi-1.3.0/src/openi.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,85 @@
-# OpenI
-
-> PYPI package for 启智 AI 协作平台。
-
-## 安装
-
-_适配 python3.6 及以上版本_
-
-```bash
-pip install openi
-```
-
-## 功能介绍
-
-- 提供命令行与代码使用
-- 具体请参考 [帮助文档-API参考](https://openi.pcl.ac.cn/docs/index.html#/api/intro)
-
-```python
-from openi.dataset import download_file
-
-download_file(
-    file="my_data.zip",
-    repo_id="user1/repo1",
-    cluster="gpu",
-    save_path="local_path/",
-)
-
-""" output
-Complete( my_data.zip)(gpu): 100%|██████████████████████████████████████████| 22.0MB/22.0MB [00:01<00:00, 15.9MB/s]
-"""
-```
-
-```bash
->>> openi
-usage: openi {login, whoami, dataset, ...} [<args>] [-h]
-
-OpenI command line tool 启智AI协作平台命令行工具
-
-commands:
-  {login,logout,whoami,dataset,d,model,m}
-    login               使用令牌登录启智并保存到本机
-    logout              登出当前用户并删除本地令牌文件
-    whoami              查询当前登录用户
-    dataset (d)         {upload,download} 上传/下载启智AI协作平台的数据集
-    model (m)           {upload,download} 上传/下载启智AI协作平台的模型
-```
-
-```bash
->>> openi login
-
-
-             ██████╗   ██████╗  ███████╗  ███╗   ██╗  ██████╗
-            ██╔═══██╗  ██╔══██╗ ██╔════╝  ████╗  ██║    ██╔═╝
-            ██║   ██║  ██████╔╝ █████╗    ██╔██╗ ██║    ██║
-            ██║   ██║  ██╔═══╝  ██╔══╝    ██║╚██╗██║    ██║
-            ╚██████╔╝  ██║      ███████╗  ██║ ╚████║  ██████╗
-             ╚═════╝   ╚═╝      ╚══════╝  ╚═╝  ╚═══╝  ╚═════╝
-
-
-点击链接获取令牌并复制粘贴到下列输入栏 https://openi.pcl.ac.cn/user/settings/applications
-
-[WARNING] 若本机已存在登录令牌，本次输入的令牌会将其覆盖
-          粘贴前请先按 退格键⇦ 删除多余空格
-
-  🔒 token:
-
-```
+Metadata-Version: 2.1
+Name: openi
+Version: 1.3.0
+Summary: A package for openi pypi
+Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
+Author: chenzh05
+Author-email: chenzh.ds@outlook.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+# OpenI
+
+> PYPI package for 启智 AI 协作平台。
+
+## 安装
+
+_适配 python3.6 及以上版本_
+
+```bash
+pip install openi
+```
+
+## 功能介绍
+
+- 提供命令行与代码使用
+- 具体请参考 [帮助文档-API参考](https://openi.pcl.ac.cn/docs/index.html#/api/intro)
+
+```python
+from openi.dataset import download_file
+
+download_file(
+    file="my_data.zip",
+    repo_id="user1/repo1",
+    cluster="gpu",
+    save_path="local_path/",
+)
+
+""" output
+Complete( my_data.zip)(gpu): 100%|██████████████████████████████████████████| 22.0MB/22.0MB [00:01<00:00, 15.9MB/s]
+"""
+```
+
+```bash
+>>> openi
+usage: openi {login, whoami, dataset, ...} [<args>] [-h]
+
+OpenI command line tool 启智AI协作平台命令行工具
+
+commands:
+  {login,logout,whoami,dataset,d,model,m}
+    login               使用令牌登录启智并保存到本机
+    logout              登出当前用户并删除本地令牌文件
+    whoami              查询当前登录用户
+    dataset (d)         {upload,download} 上传/下载启智AI协作平台的数据集
+    model (m)           {upload,download} 上传/下载启智AI协作平台的模型
+```
+
+```bash
+>>> openi login
+
+
+             ██████╗   ██████╗  ███████╗  ███╗   ██╗  ██████╗
+            ██╔═══██╗  ██╔══██╗ ██╔════╝  ████╗  ██║    ██╔═╝
+            ██║   ██║  ██████╔╝ █████╗    ██╔██╗ ██║    ██║
+            ██║   ██║  ██╔═══╝  ██╔══╝    ██║╚██╗██║    ██║
+            ╚██████╔╝  ██║      ███████╗  ██║ ╚████║  ██████╗
+             ╚═════╝   ╚═╝      ╚══════╝  ╚═╝  ╚═══╝  ╚═════╝
+
+
+点击链接获取令牌并复制粘贴到下列输入栏 https://openi.pcl.ac.cn/user/settings/applications
+
+[WARNING] 若本机已存在登录令牌，本次输入的令牌会将其覆盖
+          粘贴前请先按 退格键⇦ 删除多余空格
+
+  🔒 token:
+
+```
```

### Comparing `openi-1.2.2/src/openi/apis.py` & `openi-1.3.0/src/openi/apis.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,476 +1,476 @@
-import requests
-import json
-import os
-import time
-from pathlib import Path
-from dataclasses import dataclass
-
-from .utils import logger, constants
-
-log = logger.setup_logger()
-
-
-"""
-APIS
-"""
-
-
-@dataclass  # (frozen=True)
-class OpeniAPI:
-    endpoint: str = None
-    token: str = None
-
-    def __post_init__(self):
-        if self.endpoint is None and self.token is None:
-            try:
-                saved_token = json.loads(Path(constants.PATH.TOKEN_PATH).read_text())
-                self.token = saved_token["token"]
-                self.endpoint = saved_token["endpoint"]
-            except:
-                msg = "❌ 本机尚未登录OpenI，请参考 https://openi.pcl.ac.cn/docs/index.html#/api/cli/login."
-                log.error(msg)
-                raise FileNotFoundError(msg)
-
-        self.base_url = self.endpoint + constants.API.VERSION
-
-    """
-    basics
-    """
-
-    def send_api(
-        self,
-        method,
-        route,
-        params=dict(),
-        stream=False,
-        allow_redirects=False,
-        *args,
-        **kwargs,
-    ):
-        """
-        General API call template to OpenI
-        """
-
-        url = self.base_url + route
-
-        # 若不需要带token，则调用此函数时明确传入params=None
-        if params is not None:
-            params["access_token"] = self.token
-
-        log.info(f"api.send_api() starts...")
-        ts = time.time()
-        response = requests.request(
-            method=method,
-            url=url,
-            params=params,
-            stream=stream,
-            allow_redirects=allow_redirects,
-        )
-        log.info(f"{time.time() -ts }s used for requests returns...")
-        try:
-            if not kwargs.get("is_collaborator"):
-                response.raise_for_status()
-
-            log.http(
-                f"{method} {route} {response.status_code} {response.reason} {response.url}"
-            )
-
-            return response
-
-        except requests.exceptions.HTTPError as e:
-            msg = f"{method} {route} {e}"
-            log.warn(msg)
-            raise ConnectionError(msg)
-
-    def file_put_upload(self, url, data, upload_type):
-        """
-        API call to upload a chunk of the file(bytes data) to OpenI
-        """
-        headers = {"Content-Type": "text/plain"} if upload_type == 0 else {}
-        response = requests.request(
-            method="PUT",
-            url=url,
-            data=data,
-            headers=headers,
-        )
-        try:
-            response.raise_for_status()
-            log.http(
-                f"file_put_upload PUT {response.status_code} {response.reason} {response.url}"
-            )
-        except requests.exceptions.HTTPError as e:
-            log.warn(f"{e}")
-
-        return response
-
-    """
-    repo and user apis
-    """
-
-    def user_my_info(self):
-        method = "GET"
-        route = f"/user"
-        response = self.send_api(method, route)
-        log.response(f" {route} {response.json()}")
-        return response
-
-    def user_info(self, username):
-        method = "GET"
-        route = f"/users/{username}"
-        response = self.send_api(method, route)
-        log.response(f" {route} {response.json()}")
-        return response
-
-    def repo_my_list(self):
-        method = "GET"
-        route = f"/user/repos"
-        response = self.send_api(method, route)
-        log.response(f" {route} {response.json()}")
-        return response
-
-    def repo_list(self, username):
-        method = "GET"
-        route = f"/users/{username}/repos"
-        response = self.send_api(method, route)
-        log.response(f" {route} {response.json()}")
-        return response
-
-    def repo_info(self, repo_id):
-        method = "GET"
-        route = f"/repos/{repo_id}"
-        response = self.send_api(method, route)
-        log.response(f" {route} {response.json()}")
-        return response
-
-    def repo_access(self, repo_id):
-        method = "GET"
-        route = f"/repos/{repo_id}/right"
-        response = self.send_api(method, route)
-        log.response(f" {route} {response.json()}")
-        return response
-
-    def repo_get_collaborators(self, repo_id):
-        method = "GET"
-        route = f"/repos/{repo_id}/collaborators"
-        response = self.send_api(method, route)
-        log.response(f" {route} {response.json()}")
-        return response
-
-    def repo_is_colloborator(self, repo_id, username):
-        method = "GET"
-        route = f"/repos/{repo_id}/collaborators/{username}"
-        response = self.send_api(method, route, is_collaborator=True)
-        log.response(f" {route} {response.status_code}")
-        return response.status_code
-
-    """
-    dataset api
-    """
-
-    def dataset_query(self, repo_id):
-        method = "GET"
-        route = f"/datasets/{repo_id}"
-        response = self.send_api(method, route)
-        log.response(f" {route} {response.json()}")
-        return response
-
-    def dataset_query_with_attachment(
-        self,
-        repo_id: str,
-        upload_type: int = 0,
-    ):
-        method = "GET"
-        route = f"/datasets/{repo_id}/current_repo"
-        params = {"type": upload_type}
-        response = self.send_api(method, route, params=params)
-        log.response(f" {route} {response.json()}")
-        return response
-
-    def dataset_file_get_chunks(
-        self,
-        dataset_id,
-        md5,
-        filename,
-        upload_type,
-    ):
-        """
-        Get information of a file chunk
-        """
-        method = "GET"
-        route = "/attachments/get_chunks"
-        params = {
-            "dataset_id": dataset_id,
-            "md5": md5,
-            "file_name": filename,
-            "type": upload_type,
-        }
-        response = self.send_api(method, route, params=params)
-        log.response(f" {route} {response.json()}")
-        return response
-
-    def dataset_file_get_multipart_url(
-        self,
-        chunk_number,
-        chunk_size,
-        dataset_id,
-        filename,
-        upload_type,
-        upload_id,
-        uuid,
-    ):
-        method = "GET"
-        route = "/attachments/get_multipart_url"
-        params = {
-            "dataset_id": dataset_id,
-            "file_name": filename,
-            "type": upload_type,
-            "chunkNumber": chunk_number,
-            "size": chunk_size,
-            "uploadID": upload_id,
-            "uuid": uuid,
-        }
-        response = self.send_api(method, route, params=params)
-        log.response(f" {route} {response.json()}")
-        return response
-
-    def dataset_file_new_multipart(
-        self,
-        dataset_id,
-        md5,
-        filename,
-        upload_type,
-        size,
-        total_chunks_count,
-    ):
-        method = "GET"
-        route = "/attachments/new_multipart"
-        params = {
-            "dataset_id": dataset_id,
-            "md5": md5,
-            "file_name": filename,
-            "type": upload_type,
-            "totalChunkCounts": total_chunks_count,
-            "size": size,
-        }
-        response = self.send_api(method, route, params=params)
-        if response.json()["result_code"] == "0":
-            return response
-        else:
-            msg = f"{method} {route} {response.json()['msg']}"
-            log.warn(msg)
-            raise ConnectionError(msg)
-
-    def dataset_file_complete_multipart(
-        self,
-        dataset_id,
-        filename,
-        upload_type,
-        size,
-        upload_id,
-        uuid,
-    ):
-        method = "POST"
-        route = "/attachments/complete_multipart"
-        params = {
-            "dataset_id": dataset_id,
-            "file_name": filename,
-            "type": upload_type,
-            "size": size,
-            "uploadID": upload_id,
-            "uuid": uuid,
-        }
-        response = self.send_api(method, route, params=params)
-        log.response(f" {route} {response.json()}")
-        return response
-
-    def dataset_download_file(
-        self,
-        uuid: str,
-        upload_type: int,
-    ):
-        method = "GET"
-        route = f"/attachments/{uuid}"
-        params = {"type": upload_type}
-        response = self.send_api(
-            method,
-            route,
-            params=params,
-            allow_redirects=True,
-            stream=True,
-        )
-        return response
-
-    """
-    model management api
-    """
-
-    def model_create(
-        self,
-        repo_id,
-        model_name,
-        upload_type=1,
-        engine=0,
-        is_private=True,
-    ):
-        method = "POST"
-        route = f"/repos/{repo_id}/modelmanage/create_local_model"
-        params = dict(
-            name=model_name,
-            type=upload_type,
-            engine=engine,
-            isPrivate=is_private,
-        )
-        response = self.send_api(method, route, params=params)
-        log.response(f" {route} {response.json()}")
-        return response
-
-    def model_query_by_id(self, repo_id, model_id):
-        method = "GET"
-        route = f"/repos/{repo_id}/modelmanage/query_model_byId"
-        params = dict(id=model_id)  # {"id": model_id}
-        response = self.send_api(method, route, params=params)
-        log.response(f" {route} {response.json()}")
-        return response
-
-    def model_query_by_name(self, repo_id, model_name):
-        method = "GET"
-        route = f"/repos/{repo_id}/modelmanage/query_model_byName"
-        params = dict(name=model_name)  # {"name": model_name}
-        response = self.send_api(method, route, params=params)
-        log.response(f" {route} {response.json()}")
-        return response
-
-    def model_file_query_by_id(self, repo_id, model_id):
-        method = "GET"
-        route = f"/repos/{repo_id}/modelmanage/query_modelfile_for_predict"
-        params = dict(id=model_id)  # {"id": model_id}
-        response = self.send_api(method, route, params=params)
-        log.response(f" {route} {response.json()}")
-        return response
-
-    def model_download_all(self, repo_id, model_id):
-        method = "GET"
-        route = f"/repos/{repo_id}/modelmanage/downloadall"
-        params = dict(id=model_id)  # {"id": model_id}
-        response = self.send_api(method, route, params=params, stream=True)
-        return response
-
-    def model_download_single(
-        self,
-        repo_id,
-        model_id,
-        filename,
-    ):
-        method = "GET"
-        route = f"/repos/{repo_id}/modelmanage/downloadsingle/{model_id}"
-        params = dict(fileName=filename)
-        response = self.send_api(
-            method, route, params=params, allow_redirects=True, stream=True
-        )
-        return response
-
-    def model_file_get_chunks(
-        self,
-        modeluuid,
-        md5,
-        filename,
-        upload_type,
-    ):
-        method = "GET"
-        route = f"/attachments/model/get_chunks"
-        params = dict(
-            modeluuid=modeluuid,
-            md5=md5,
-            file_name=filename,
-            type=upload_type,
-        )
-        response = self.send_api(method, route, params=params)
-        log.response(f" {route} {response.json()}")
-        return response
-
-    def model_file_new_multipart(
-        self,
-        modeluuid,
-        md5,
-        filename,
-        upload_type,
-        total_chunks_count,
-        size,
-    ):
-        method = "GET"
-        route = f"/attachments/model/new_multipart"
-        params = dict(
-            modeluuid=modeluuid,
-            md5=md5,
-            file_name=filename,
-            type=upload_type,
-            totalChunkCounts=total_chunks_count,
-            size=size,
-        )
-        response = self.send_api(method, route, params=params)
-        log.response(f" {route} {response.json()}")
-        return response
-
-    def model_file_get_multipart_url(
-        self,
-        upload_type,
-        chunk_number,
-        chunk_size,
-        upload_id,
-        uuid,
-    ):
-        method = "GET"
-        route = f"/attachments/model/get_multipart_url"
-        params = dict(
-            type=upload_type,
-            chunkNumber=chunk_number,
-            size=chunk_size,
-            uploadID=upload_id,
-            uuid=uuid,
-        )
-        response = self.send_api(method, route, params=params)
-        # log.response(f" {route} {response.json()}")
-        return response
-
-    def model_file_complete_multipart(
-        self,
-        modeluuid,
-        upload_type,
-        upload_id,
-        uuid,
-    ):
-        method = "POST"
-        route = f"/attachments/model/complete_multipart"
-        params = dict(
-            modeluuid=modeluuid,
-            type=upload_type,
-            uploadID=upload_id,
-            uuid=uuid,
-        )
-        response = self.send_api(method, route, params=params)
-        log.response(f" {route} {response.json()}")
-        return response
-
-    """
-    AI tasks apis
-    """
-
-    def aitask_repo_list(
-        self,
-        repo_id,
-        job_type: str = "DEBUG",
-        compute_resource: str = "GPU",
-        page: int = 1,
-    ):
-        """
-        test
-        """
-        method = "GET"
-        route = f"/{repo_id}/ai_task/list"
-        params = dict(
-            job_type=job_type,
-            compute_resource=compute_resource,
-            page=page,
-        )
-        response = self.send_api(method, route, params=params)
-        return response
+import requests
+import json
+import os
+import time
+from pathlib import Path
+from dataclasses import dataclass
+
+from .utils import logger, constants
+
+log = logger.setup_logger()
+
+
+"""
+APIS
+"""
+
+
+@dataclass  # (frozen=True)
+class OpeniAPI:
+    endpoint: str = None
+    token: str = None
+
+    def __post_init__(self):
+        if self.endpoint is None and self.token is None:
+            try:
+                saved_token = json.loads(Path(constants.PATH.TOKEN_PATH).read_text())
+                self.token = saved_token["token"]
+                self.endpoint = saved_token["endpoint"]
+            except:
+                msg = "❌ 本机尚未登录OpenI，请参考 https://openi.pcl.ac.cn/docs/index.html#/api/cli/login."
+                log.error(msg)
+                raise FileNotFoundError(msg)
+
+        self.base_url = self.endpoint + constants.API.VERSION
+
+    """
+    basics
+    """
+
+    def send_api(
+        self,
+        method,
+        route,
+        params=dict(),
+        stream=False,
+        allow_redirects=False,
+        *args,
+        **kwargs,
+    ):
+        """
+        General API call template to OpenI
+        """
+
+        url = self.base_url + route
+
+        # 若不需要带token，则调用此函数时明确传入params=None
+        if params is not None:
+            params["access_token"] = self.token
+
+        log.info(f"api.send_api() starts...")
+        ts = time.time()
+        response = requests.request(
+            method=method,
+            url=url,
+            params=params,
+            stream=stream,
+            allow_redirects=allow_redirects,
+        )
+        log.info(f"{time.time() -ts }s used for requests returns...")
+        try:
+            if not kwargs.get("is_collaborator"):
+                response.raise_for_status()
+
+            log.http(
+                f"{method} {route} {response.status_code} {response.reason} {response.url}"
+            )
+
+            return response
+
+        except requests.exceptions.HTTPError as e:
+            msg = f"{method} {route} {e}"
+            log.warn(msg)
+            raise ConnectionError(msg)
+
+    def file_put_upload(self, url, data, upload_type):
+        """
+        API call to upload a chunk of the file(bytes data) to OpenI
+        """
+        headers = {"Content-Type": "text/plain"} if upload_type == 0 else {}
+        response = requests.request(
+            method="PUT",
+            url=url,
+            data=data,
+            headers=headers,
+        )
+        try:
+            response.raise_for_status()
+            log.http(
+                f"file_put_upload PUT {response.status_code} {response.reason} {response.url}"
+            )
+        except requests.exceptions.HTTPError as e:
+            log.warn(f"{e}")
+
+        return response
+
+    """
+    repo and user apis
+    """
+
+    def user_my_info(self):
+        method = "GET"
+        route = f"/user"
+        response = self.send_api(method, route)
+        log.response(f" {route} {response.json()}")
+        return response
+
+    def user_info(self, username):
+        method = "GET"
+        route = f"/users/{username}"
+        response = self.send_api(method, route)
+        log.response(f" {route} {response.json()}")
+        return response
+
+    def repo_my_list(self):
+        method = "GET"
+        route = f"/user/repos"
+        response = self.send_api(method, route)
+        log.response(f" {route} {response.json()}")
+        return response
+
+    def repo_list(self, username):
+        method = "GET"
+        route = f"/users/{username}/repos"
+        response = self.send_api(method, route)
+        log.response(f" {route} {response.json()}")
+        return response
+
+    def repo_info(self, repo_id):
+        method = "GET"
+        route = f"/repos/{repo_id}"
+        response = self.send_api(method, route)
+        log.response(f" {route} {response.json()}")
+        return response
+
+    def repo_access(self, repo_id):
+        method = "GET"
+        route = f"/repos/{repo_id}/right"
+        response = self.send_api(method, route)
+        log.response(f" {route} {response.json()}")
+        return response
+
+    def repo_get_collaborators(self, repo_id):
+        method = "GET"
+        route = f"/repos/{repo_id}/collaborators"
+        response = self.send_api(method, route)
+        log.response(f" {route} {response.json()}")
+        return response
+
+    def repo_is_colloborator(self, repo_id, username):
+        method = "GET"
+        route = f"/repos/{repo_id}/collaborators/{username}"
+        response = self.send_api(method, route, is_collaborator=True)
+        log.response(f" {route} {response.status_code}")
+        return response.status_code
+
+    """
+    dataset api
+    """
+
+    def dataset_query(self, repo_id):
+        method = "GET"
+        route = f"/datasets/{repo_id}"
+        response = self.send_api(method, route)
+        log.response(f" {route} {response.json()}")
+        return response
+
+    def dataset_query_with_attachment(
+        self,
+        repo_id: str,
+        upload_type: int = 0,
+    ):
+        method = "GET"
+        route = f"/datasets/{repo_id}/current_repo"
+        params = {"type": upload_type}
+        response = self.send_api(method, route, params=params)
+        log.response(f" {route} {response.json()}")
+        return response
+
+    def dataset_file_get_chunks(
+        self,
+        dataset_id,
+        md5,
+        filename,
+        upload_type,
+    ):
+        """
+        Get information of a file chunk
+        """
+        method = "GET"
+        route = "/attachments/get_chunks"
+        params = {
+            "dataset_id": dataset_id,
+            "md5": md5,
+            "file_name": filename,
+            "type": upload_type,
+        }
+        response = self.send_api(method, route, params=params)
+        log.response(f" {route} {response.json()}")
+        return response
+
+    def dataset_file_get_multipart_url(
+        self,
+        chunk_number,
+        chunk_size,
+        dataset_id,
+        filename,
+        upload_type,
+        upload_id,
+        uuid,
+    ):
+        method = "GET"
+        route = "/attachments/get_multipart_url"
+        params = {
+            "dataset_id": dataset_id,
+            "file_name": filename,
+            "type": upload_type,
+            "chunkNumber": chunk_number,
+            "size": chunk_size,
+            "uploadID": upload_id,
+            "uuid": uuid,
+        }
+        response = self.send_api(method, route, params=params)
+        log.response(f" {route} {response.json()}")
+        return response
+
+    def dataset_file_new_multipart(
+        self,
+        dataset_id,
+        md5,
+        filename,
+        upload_type,
+        size,
+        total_chunks_count,
+    ):
+        method = "GET"
+        route = "/attachments/new_multipart"
+        params = {
+            "dataset_id": dataset_id,
+            "md5": md5,
+            "file_name": filename,
+            "type": upload_type,
+            "totalChunkCounts": total_chunks_count,
+            "size": size,
+        }
+        response = self.send_api(method, route, params=params)
+        if response.json()["result_code"] == "0":
+            return response
+        else:
+            msg = f"{method} {route} {response.json()['msg']}"
+            log.warn(msg)
+            raise ConnectionError(msg)
+
+    def dataset_file_complete_multipart(
+        self,
+        dataset_id,
+        filename,
+        upload_type,
+        size,
+        upload_id,
+        uuid,
+    ):
+        method = "POST"
+        route = "/attachments/complete_multipart"
+        params = {
+            "dataset_id": dataset_id,
+            "file_name": filename,
+            "type": upload_type,
+            "size": size,
+            "uploadID": upload_id,
+            "uuid": uuid,
+        }
+        response = self.send_api(method, route, params=params)
+        log.response(f" {route} {response.json()}")
+        return response
+
+    def dataset_download_file(
+        self,
+        uuid: str,
+        upload_type: int,
+    ):
+        method = "GET"
+        route = f"/attachments/{uuid}"
+        params = {"type": upload_type}
+        response = self.send_api(
+            method,
+            route,
+            params=params,
+            allow_redirects=True,
+            stream=True,
+        )
+        return response
+
+    """
+    model management api
+    """
+
+    def model_create(
+        self,
+        repo_id,
+        model_name,
+        upload_type=1,
+        engine=0,
+        is_private=True,
+    ):
+        method = "POST"
+        route = f"/repos/{repo_id}/modelmanage/create_local_model"
+        params = dict(
+            name=model_name,
+            type=upload_type,
+            engine=engine,
+            isPrivate=is_private,
+        )
+        response = self.send_api(method, route, params=params)
+        log.response(f" {route} {response.json()}")
+        return response
+
+    def model_query_by_id(self, repo_id, model_id):
+        method = "GET"
+        route = f"/repos/{repo_id}/modelmanage/query_model_byId"
+        params = dict(id=model_id)  # {"id": model_id}
+        response = self.send_api(method, route, params=params)
+        log.response(f" {route} {response.json()}")
+        return response
+
+    def model_query_by_name(self, repo_id, model_name):
+        method = "GET"
+        route = f"/repos/{repo_id}/modelmanage/query_model_byName"
+        params = dict(name=model_name)  # {"name": model_name}
+        response = self.send_api(method, route, params=params)
+        log.response(f" {route} {response.json()}")
+        return response
+
+    def model_file_query_by_id(self, repo_id, model_id):
+        method = "GET"
+        route = f"/repos/{repo_id}/modelmanage/query_modelfile_for_predict"
+        params = dict(id=model_id)  # {"id": model_id}
+        response = self.send_api(method, route, params=params)
+        log.response(f" {route} {response.json()}")
+        return response
+
+    def model_download_all(self, repo_id, model_id):
+        method = "GET"
+        route = f"/repos/{repo_id}/modelmanage/downloadall"
+        params = dict(id=model_id)  # {"id": model_id}
+        response = self.send_api(method, route, params=params, stream=True)
+        return response
+
+    def model_download_single(
+        self,
+        repo_id,
+        model_id,
+        filename,
+    ):
+        method = "GET"
+        route = f"/repos/{repo_id}/modelmanage/downloadsingle/{model_id}"
+        params = dict(fileName=filename)
+        response = self.send_api(
+            method, route, params=params, allow_redirects=True, stream=True
+        )
+        return response
+
+    def model_file_get_chunks(
+        self,
+        modeluuid,
+        md5,
+        filename,
+        upload_type,
+    ):
+        method = "GET"
+        route = f"/attachments/model/get_chunks"
+        params = dict(
+            modeluuid=modeluuid,
+            md5=md5,
+            file_name=filename,
+            type=upload_type,
+        )
+        response = self.send_api(method, route, params=params)
+        log.response(f" {route} {response.json()}")
+        return response
+
+    def model_file_new_multipart(
+        self,
+        modeluuid,
+        md5,
+        filename,
+        upload_type,
+        total_chunks_count,
+        size,
+    ):
+        method = "GET"
+        route = f"/attachments/model/new_multipart"
+        params = dict(
+            modeluuid=modeluuid,
+            md5=md5,
+            file_name=filename,
+            type=upload_type,
+            totalChunkCounts=total_chunks_count,
+            size=size,
+        )
+        response = self.send_api(method, route, params=params)
+        log.response(f" {route} {response.json()}")
+        return response
+
+    def model_file_get_multipart_url(
+        self,
+        upload_type,
+        chunk_number,
+        chunk_size,
+        upload_id,
+        uuid,
+    ):
+        method = "GET"
+        route = f"/attachments/model/get_multipart_url"
+        params = dict(
+            type=upload_type,
+            chunkNumber=chunk_number,
+            size=chunk_size,
+            uploadID=upload_id,
+            uuid=uuid,
+        )
+        response = self.send_api(method, route, params=params)
+        # log.response(f" {route} {response.json()}")
+        return response
+
+    def model_file_complete_multipart(
+        self,
+        modeluuid,
+        upload_type,
+        upload_id,
+        uuid,
+    ):
+        method = "POST"
+        route = f"/attachments/model/complete_multipart"
+        params = dict(
+            modeluuid=modeluuid,
+            type=upload_type,
+            uploadID=upload_id,
+            uuid=uuid,
+        )
+        response = self.send_api(method, route, params=params)
+        log.response(f" {route} {response.json()}")
+        return response
+
+    """
+    AI tasks apis
+    """
+
+    def aitask_repo_list(
+        self,
+        repo_id,
+        job_type: str = "DEBUG",
+        compute_resource: str = "GPU",
+        page: int = 1,
+    ):
+        """
+        test
+        """
+        method = "GET"
+        route = f"/{repo_id}/ai_task/list"
+        params = dict(
+            job_type=job_type,
+            compute_resource=compute_resource,
+            page=page,
+        )
+        response = self.send_api(method, route, params=params)
+        return response
```

### Comparing `openi-1.2.2/src/openi/cli.py` & `openi-1.3.0/src/openi/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,234 +1,237 @@
-import argparse
-
-from .login import login, logout, whoami
-from .utils.constants import *
-from .utils.logger import *
-from .dataset import *
-from .model import *
-
-# import textwrap
-
-
-def main():
-    parser = argparse.ArgumentParser(
-        formatter_class=argparse.RawDescriptionHelpFormatter,
-        usage=CLI.usage,
-        description=CLI.banner,
-    )
-    parser._action_groups.pop()
-    subparsers = parser.add_subparsers(title="commands", dest="commands")
-    subparsers.required = False
-    # subparsers.choices = Help.openi_choices
-    parse_login(subparsers)
-    parse_logout(subparsers)
-    parse_whoami(subparsers)
-    parse_dataset(subparsers)
-    parse_model(subparsers)
-    args = parser.parse_args()
-    if not hasattr(args, "func"):
-        parser.print_help()
-        exit(1)
-
-    command_args = {}
-    command_args.update(vars(args))
-    del command_args["func"]
-    del command_args["commands"]
-    error = False
-    try:
-        out = args.func(**command_args)
-    except Exception as e:
-        print(e)
-        out = None
-        error = True
-    except ValueError as e:
-        print(e)
-        out = None
-        error = True
-    except KeyboardInterrupt:
-        print("User cancelled operation")
-        out = None
-    if out is not None:
-        print(out, end="")
-
-    # This is so that scripts that pick up on error codes can tell when there was a failure
-    if error:
-        exit(1)
-
-
-def parse_login(subparsers):
-    parse_login = subparsers.add_parser(
-        "login",
-        description=CLI.command_login,
-        usage=CLI.login_usage,
-        help=CLI.command_login,
-    )
-    parse_login.add_argument(
-        "-e",  # '--endpoint',
-        dest="endpoint",
-        default=API.DEFAULT_ENDPOINT,
-        required=False,
-        help=CLI.param_endpoint,
-    )
-    parse_login.add_argument(
-        "-t",  # '--token',
-        dest="token",
-        default=None,
-        required=False,
-        help=CLI.param_token,
-    )
-    parse_login.set_defaults(func=login)
-
-
-def parse_logout(subparsers):
-    parse_logout = subparsers.add_parser(
-        "logout",
-        description=CLI.command_logout,
-        usage="openi logout [-h]",
-        help=CLI.command_logout,
-    )
-    parse_logout.set_defaults(func=logout)
-
-
-def parse_whoami(subparsers):
-    parse_whoami = subparsers.add_parser(
-        "whoami",
-        description=CLI.command_whoami,
-        usage="openi whoami [-h]",
-        help=CLI.command_whoami,
-    )
-    parse_whoami.set_defaults(func=whoami)
-
-
-def parse_dataset(subparsers):
-    parser_dataset = subparsers.add_parser(
-        "dataset", usage=CLI.dataset_usage, help=CLI.command_dataset, aliases=["d"]
-    )
-    parser_dataset._action_groups.pop()
-    subparsers_dataset = parser_dataset.add_subparsers(
-        title="commands", dest="commands"
-    )
-    subparsers_dataset.required = True
-
-    # dataset upload
-    parser_dataset_upload = subparsers_dataset.add_parser(
-        "upload",
-        description=CLI.command_dataset_upload,
-        usage=CLI.dataset_upload_usage,
-        help=CLI.dataset_upload_help,
-        # epilog=CLI.dataset_upload_epilog,
-        formatter_class=argparse.RawDescriptionHelpFormatter,
-    )
-    parser_dataset_upload._action_groups.pop()
-    parser_dataset_upload_args = parser_dataset_upload.add_argument_group("arguments")
-    parser_dataset_upload_args.add_argument(
-        "-f", dest="file", required=True, help=CLI.dataset_upload_param_file
-    )
-    parser_dataset_upload_args.add_argument(
-        "-r", dest="repo_id", required=True, help=CLI.dataset_upload_param_repo_id
-    )
-    parser_dataset_upload_args.add_argument(
-        "-c",
-        dest="cluster",
-        required=False,
-        default="NPU",
-        choices=["gpu", "npu"],
-        help=CLI.dataset_upload_param_cluster,
-    )
-    parser_dataset_upload.set_defaults(func=upload_file)
-
-    # dataset download
-    parser_dataset_download = subparsers_dataset.add_parser(
-        "download",
-        description=CLI.command_dataset_download,
-        usage=CLI.dataset_download_usage,
-        help=CLI.dataset_download_help,
-        # epilog = CLI.dataset_download_epilog,
-        formatter_class=argparse.RawDescriptionHelpFormatter,
-    )
-    parser_dataset_download._action_groups.pop()
-    parser_dataset_download_args = parser_dataset_download.add_argument_group(
-        "arguments"
-    )
-    parser_dataset_download_args.add_argument(
-        "-f", dest="file", required=True, help=CLI.dataset_download_param_file
-    )
-    parser_dataset_download_args.add_argument(
-        "-r", dest="repo_id", required=True, help=CLI.dataset_upload_param_repo_id
-    )
-    parser_dataset_download_args.add_argument(
-        "-c",  #'--cluster',
-        dest="cluster",
-        required=False,
-        default="npu",
-        choices=["gpu", "npu"],
-        help=CLI.dataset_upload_param_cluster,
-    )
-    parser_dataset_download_args.add_argument(
-        "-p",  #'--save_path',
-        dest="save_path",
-        required=False,
-        default=PATH.DATASET_SAVE_PATH,
-        help=CLI.dataset_download_param_save_path,
-    )
-    parser_dataset_download.set_defaults(func=download_file)
-
-
-def parse_model(subparsers):
-    parser_model = subparsers.add_parser(
-        "model", usage=CLI.model_usage, help=CLI.command_model, aliases=["m"]
-    )
-    parser_model._action_groups.pop()
-    subparsers_model = parser_model.add_subparsers(title="commands", dest="commands")
-    subparsers_model.required = True
-
-    # model upload
-    parser_model_upload = subparsers_model.add_parser(
-        "upload",
-        description=CLI.command_model_upload,
-        usage=CLI.model_upload_usage,
-        help=CLI.model_upload_help,
-        formatter_class=argparse.RawDescriptionHelpFormatter,
-    )
-    parser_model_upload._action_groups.pop()
-    parser_model_upload_args = parser_model_upload.add_argument_group("arguments")
-    parser_model_upload_args.add_argument(
-        "-f", dest="folder", required=True, help=CLI.model_upload_param_folder
-    )
-    parser_model_upload_args.add_argument(
-        "-r", dest="repo_id", required=True, help=CLI.model_upload_param_repo_id
-    )
-    parser_model_upload_args.add_argument(
-        "-m",
-        dest="model_name",
-        required=True,
-        help=CLI.model_upload_param_model_name,
-    )
-    parser_model_upload.set_defaults(func=upload_model)
-
-    # model upload
-    parser_model_download = subparsers_model.add_parser(
-        "download",
-        description=CLI.command_model_download,
-        usage=CLI.model_download_usage,
-        help=CLI.model_download_help,
-        formatter_class=argparse.RawDescriptionHelpFormatter,
-    )
-    parser_model_download._action_groups.pop()
-    parser_model_download_args = parser_model_download.add_argument_group("arguments")
-    parser_model_download_args.add_argument(
-        "-r", dest="repo_id", required=True, help=CLI.model_upload_param_repo_id
-    )
-    parser_model_download_args.add_argument(
-        "-m",
-        dest="model_name",
-        required=True,
-        help=CLI.model_upload_param_model_name,
-    )
-    parser_model_download_args.add_argument(
-        "-p",  #'--save_path',
-        dest="save_path",
-        required=False,
-        default=PATH.MODEL_SAVE_PATH,
-        help=CLI.model_download_param_save_path,
-    )
-    parser_model_download.set_defaults(func=download_model)
+import argparse
+
+from ._login import login, logout, whoami
+from .dataset import *
+from .model import *
+
+
+# import textwrap
+
+
+def main():
+    parser = argparse.ArgumentParser(
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+        usage=CLI.usage,
+        description=CLI.banner,
+    )
+    parser._action_groups.pop()
+    subparsers = parser.add_subparsers(title="commands", dest="commands")
+    subparsers.required = False
+    # subparsers.choices = Help.openi_choices
+    parse_login(subparsers)
+    parse_logout(subparsers)
+    parse_whoami(subparsers)
+    parse_dataset(subparsers)
+    parse_model(subparsers)
+    args = parser.parse_args()
+    if not hasattr(args, "func"):
+        parser.print_help()
+        exit(1)
+
+    command_args = {}
+    command_args.update(vars(args))
+    del command_args["func"]
+    del command_args["commands"]
+    error = False
+
+    out = args.func(**command_args)
+    if out is not None:
+        print(out, end="")
+    # try:
+    #     out = args.func(**command_args)
+    # except Exception as e:
+    #     print(e)
+    #     out = None
+    #     error = True
+    # except ValueError as e:
+    #     print(e)
+    #     out = None
+    #     error = True
+    # except KeyboardInterrupt:
+    #     print("User cancelled operation")
+    #     out = None
+    # if out is not None:
+    #     print(out, end="")
+
+    # This is so that scripts that pick up on error codes can tell when there was a failure
+    if error:
+        exit(1)
+
+
+def parse_login(subparsers):
+    parse_login = subparsers.add_parser(
+        "login",
+        description=CLI.command_login,
+        usage=CLI.login_usage,
+        help=CLI.command_login,
+    )
+    parse_login.add_argument(
+        "-e",  # '--endpoint',
+        dest="endpoint",
+        default=API.DEFAULT_ENDPOINT,
+        required=False,
+        help=CLI.param_endpoint,
+    )
+    parse_login.add_argument(
+        "-t",  # '--token',
+        dest="token",
+        default=None,
+        required=False,
+        help=CLI.param_token,
+    )
+    parse_login.set_defaults(func=login)
+
+
+def parse_logout(subparsers):
+    parse_logout = subparsers.add_parser(
+        "logout",
+        description=CLI.command_logout,
+        usage="openi logout [-h]",
+        help=CLI.command_logout,
+    )
+    parse_logout.set_defaults(func=logout)
+
+
+def parse_whoami(subparsers):
+    parse_whoami = subparsers.add_parser(
+        "whoami",
+        description=CLI.command_whoami,
+        usage="openi whoami [-h]",
+        help=CLI.command_whoami,
+    )
+    parse_whoami.set_defaults(func=whoami)
+
+
+def parse_dataset(subparsers):
+    parser_dataset = subparsers.add_parser(
+        "dataset", usage=CLI.dataset_usage, help=CLI.command_dataset, aliases=["d"]
+    )
+    parser_dataset._action_groups.pop()
+    subparsers_dataset = parser_dataset.add_subparsers(
+        title="commands", dest="commands"
+    )
+    subparsers_dataset.required = True
+
+    # dataset upload
+    parser_dataset_upload = subparsers_dataset.add_parser(
+        "upload",
+        description=CLI.command_dataset_upload,
+        usage=CLI.dataset_upload_usage,
+        help=CLI.dataset_upload_help,
+        # epilog=CLI.dataset_upload_epilog,
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
+    parser_dataset_upload._action_groups.pop()
+    parser_dataset_upload_args = parser_dataset_upload.add_argument_group("arguments")
+    parser_dataset_upload_args.add_argument(
+        "-f", dest="file", required=True, help=CLI.dataset_upload_param_file
+    )
+    parser_dataset_upload_args.add_argument(
+        "-r", dest="repo_id", required=True, help=CLI.dataset_upload_param_repo_id
+    )
+    parser_dataset_upload_args.add_argument(
+        "-c",
+        dest="cluster",
+        required=False,
+        default="NPU",
+        choices=["gpu", "npu"],
+        help=CLI.dataset_upload_param_cluster,
+    )
+    parser_dataset_upload.set_defaults(func=upload_file)
+
+    # dataset download
+    parser_dataset_download = subparsers_dataset.add_parser(
+        "download",
+        description=CLI.command_dataset_download,
+        usage=CLI.dataset_download_usage,
+        help=CLI.dataset_download_help,
+        # epilog = CLI.dataset_download_epilog,
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
+    parser_dataset_download._action_groups.pop()
+    parser_dataset_download_args = parser_dataset_download.add_argument_group(
+        "arguments"
+    )
+    parser_dataset_download_args.add_argument(
+        "-f", dest="file", required=True, help=CLI.dataset_download_param_file
+    )
+    parser_dataset_download_args.add_argument(
+        "-r", dest="repo_id", required=True, help=CLI.dataset_upload_param_repo_id
+    )
+    parser_dataset_download_args.add_argument(
+        "-c",  # '--cluster',
+        dest="cluster",
+        required=False,
+        default="npu",
+        choices=["gpu", "npu"],
+        help=CLI.dataset_upload_param_cluster,
+    )
+    parser_dataset_download_args.add_argument(
+        "-p",  # '--save_path',
+        dest="save_path",
+        required=False,
+        default=PATH.DATASET_SAVE_PATH,
+        help=CLI.dataset_download_param_save_path,
+    )
+    parser_dataset_download.set_defaults(func=download_file)
+
+
+def parse_model(subparsers):
+    parser_model = subparsers.add_parser(
+        "model", usage=CLI.model_usage, help=CLI.command_model, aliases=["m"]
+    )
+    parser_model._action_groups.pop()
+    subparsers_model = parser_model.add_subparsers(title="commands", dest="commands")
+    subparsers_model.required = True
+
+    # model upload
+    parser_model_upload = subparsers_model.add_parser(
+        "upload",
+        description=CLI.command_model_upload,
+        usage=CLI.model_upload_usage,
+        help=CLI.model_upload_help,
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
+    parser_model_upload._action_groups.pop()
+    parser_model_upload_args = parser_model_upload.add_argument_group("arguments")
+    parser_model_upload_args.add_argument(
+        "-f", dest="folder", required=True, help=CLI.model_upload_param_folder
+    )
+    parser_model_upload_args.add_argument(
+        "-r", dest="repo_id", required=True, help=CLI.model_upload_param_repo_id
+    )
+    parser_model_upload_args.add_argument(
+        "-m",
+        dest="model_name",
+        required=True,
+        help=CLI.model_upload_param_model_name,
+    )
+    parser_model_upload.set_defaults(func=upload_model)
+
+    # model upload
+    parser_model_download = subparsers_model.add_parser(
+        "download",
+        description=CLI.command_model_download,
+        usage=CLI.model_download_usage,
+        help=CLI.model_download_help,
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
+    parser_model_download._action_groups.pop()
+    parser_model_download_args = parser_model_download.add_argument_group("arguments")
+    parser_model_download_args.add_argument(
+        "-r", dest="repo_id", required=True, help=CLI.model_upload_param_repo_id
+    )
+    parser_model_download_args.add_argument(
+        "-m",
+        dest="model_name",
+        required=True,
+        help=CLI.model_upload_param_model_name,
+    )
+    parser_model_download_args.add_argument(
+        "-p",  # '--save_path',
+        dest="save_path",
+        required=False,
+        default=PATH.MODEL_SAVE_PATH,
+        help=CLI.model_download_param_save_path,
+    )
+    parser_model_download.set_defaults(func=download_model)
```

### Comparing `openi-1.2.2/src/openi/dataset/download.py` & `openi-1.3.0/src/openi/dataset/download.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,87 +1,84 @@
-import os
-import re
-
-from ..utils import logger, constants
-from ..services import *
-
-log = logger.setup_logger()
-
-
-def download_file(
-    file: str,
-    repo_id: str,
-    cluster: str = "npu",
-    save_path: str = constants.PATH.DATASET_SAVE_PATH,
-):
-    """
-    download a zip or tar.gz dataset file from OpenI
-
-    :param file: dataset file name
-    :param repo_id: repo id in form of `owner/repo_name`
-    :param cluster: cluster type in [gpu,npu], default is `npu`
-    :param save_path: local save path, default is `./dataset`
-    :return:
-
-    e.g.
-    >>> from openi.dataset import download_file
-    >>> download_file("cifar10.zip", "openi/official", cluster="gpu", save_path="mydata")
-
-    Complete( cifar10.zip)(gpu): 100%|████████████████████████| 163MB/163MB [00:00<00:00, 54.0MB/s]
-
-    """
-
-    log.info(f"{'-'*200}")
-    log.info(f"params - {locals()}")
-
-    upload_type = get_upload_type(cluster)
-
-    # Define a regex pattern to match the desired formats
-    pattern = r"^.+\.(zip|tar\.gz)$"
-    if not re.match(pattern, file):
-        msg = f"❌ `{file}` 非压缩文件（`zip`或`tar.gz`）无法通过sdk下载"
-        log.error(msg)
-        raise ValueError(msg)
-
-    openi_repo = OpeniRepo(repo_id=repo_id)
-    if openi_repo.access not in ["read", "write"]:
-        msg = f"`{repo_id}` 无权限操作此仓库"
-        log.error(msg)
-        raise ValueError(msg)
-
-    openi_dataset = OpeniDataset(repo_id=openi_repo.repo_id)
-    openi_dataset.get_dataset_file(upload_type=upload_type)
-    targe_file = None
-    log.info(f"openi_dataset.dataset_files,{openi_dataset.dataset_files}")
-    if openi_dataset.dataset_files is not None:
-        for f in openi_dataset.dataset_files:
-            if f["name"] == file:
-                targe_file = f
-    log.info(f"targe_file,{targe_file}")
-    if openi_dataset.dataset_files is None or targe_file is None:
-        msg = (
-            f"❌ `{openi_repo.repo_id}`-`{openi_dataset.dataset_name}` "
-            f"数据集内未找到名为{file}({cluster})的文件"
-        )
-        log.error(msg)
-        raise ValueError(msg)
-
-    local_dir = os.path.expanduser(save_path)
-    if not os.path.exists(local_dir):
-        os.makedirs(local_dir, exist_ok=True)
-
-    openi_file = OpeniFileDownload(
-        filename=targe_file["name"],
-        size=targe_file["size"],
-        local_dir=local_dir,
-        repo_id=openi_repo.repo_id,
-        dataset_or_model_id=openi_dataset.dataset_id,
-        dataset_or_model_name=openi_dataset.dataset_name,
-        target_type="dataset",
-        upload_type=upload_type,
-        uuid=targe_file["uuid"],
-    )
-
-    display_progress_bar([openi_file])
-    openi_file.download_with_tqdm()
-
-    log.info(f"{'-'*200}")
+import re
+
+from ..services import *
+
+log = logger.setup_logger()
+
+
+def download_file(
+        file: str,
+        repo_id: str,
+        cluster: str = "npu",
+        save_path: str = constants.PATH.DATASET_SAVE_PATH,
+):
+    """
+    download a zip or tar.gz dataset file from OpenI
+
+    :param file: dataset file name
+    :param repo_id: repo id in form of `owner/repo_name`
+    :param cluster: cluster type in [gpu,npu], default is `npu`
+    :param save_path: local save path, default is `./dataset`
+    :return:
+
+    e.g.
+    >>> from openi.dataset import download_file
+    >>> download_file("cifar10.zip", "openi/official", cluster="gpu", save_path="mydata")
+
+    Complete( cifar10.zip)(gpu): 100%|████████████████████████| 163MB/163MB [00:00<00:00, 54.0MB/s]
+
+    """
+
+    log.info(f"{'-' * 200}")
+    log.info(f"params - {locals()}")
+
+    upload_type = get_upload_type(cluster)
+
+    pattern = r"^.+\.(zip|tar\.gz)$"
+    if not re.match(pattern, file):
+        msg = f"❌ `{file}` 非压缩文件（`zip`或`tar.gz`）无法通过sdk下载"
+        log.error(msg)
+        raise ValueError(msg)
+
+    openi_repo = OpeniRepo(repo_id=repo_id)
+    if openi_repo.access not in ["read", "write"]:
+        msg = f"`{repo_id}` 无权限操作此仓库"
+        log.error(msg)
+        raise ValueError(msg)
+
+    openi_dataset = OpeniDataset(repo_id=openi_repo.repo_id)
+    openi_dataset.get_dataset_file(upload_type=upload_type)
+    targe_file = None
+    log.info(f"openi_dataset.dataset_files,{openi_dataset.dataset_files}")
+    if openi_dataset.dataset_files is not None:
+        for f in openi_dataset.dataset_files:
+            if f["name"] == file:
+                targe_file = f
+    log.info(f"targe_file,{targe_file}")
+    if openi_dataset.dataset_files is None or targe_file is None:
+        msg = (
+            f"❌ `{openi_repo.repo_id}`-`{openi_dataset.dataset_name}` "
+            f"数据集内未找到名为{file}({cluster})的文件"
+        )
+        log.error(msg)
+        raise ValueError(msg)
+
+    local_dir = os.path.expanduser(save_path)
+    if not os.path.exists(local_dir):
+        os.makedirs(local_dir, exist_ok=True)
+
+    openi_file = OpeniFileDownload(
+        filename=targe_file["name"],
+        size=targe_file["size"],
+        local_dir=local_dir,
+        repo_id=openi_repo.repo_id,
+        dataset_or_model_id=openi_dataset.dataset_id,
+        dataset_or_model_name=openi_dataset.dataset_name,
+        target_type="dataset",
+        upload_type=upload_type,
+        uuid=targe_file["uuid"],
+    )
+
+    display_progress_bar([openi_file])
+    openi_file.download_with_tqdm()
+
+    log.info(f"{'-' * 200}")
```

### Comparing `openi-1.2.2/src/openi/dataset/upload.py` & `openi-1.3.0/src/openi/dataset/upload.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,60 @@
-import os
-from tqdm.auto import tqdm
-
-from ..utils import logger
-from ..services import *
-
-log = logger.setup_logger()
-
-
-def upload_file(
-    file: str,
-    repo_id: str,
-    cluster: str = "npu",
-):
-    """
-    upload a dataset file to OpenI
-
-    :param file: lcoal file name
-    :param repo_id: repo id in form of `owner/repo_name`
-    :param cluster: cluster type in [gpu,npu], default is `npu`
-    :return:
-
-    e.g.
-    >>> from openi.dataset import upload_file
-    >>> upload_file("cifar10.zip", "openi/official", cluster="gpu")
-
-    Calculating file md5, this might take a while for large file…
-    Complete( cifar10.zip)(gpu): 100%|████████████████████████| 163MB/163MB [00:00<00:00, 54.0MB/s]
-
-    """
-
-    log.info(f"{'-'*200}")
-    log.info(f"params - {locals()}")
-
-    upload_type = get_upload_type(cluster)
-
-    # OpeniFileUpload
-    local_file = os.path.expanduser(file)
-    if not os.path.exists(local_file):
-        msg = f"❌ {local_file} 未找到本地文件"
-        log.error(msg)
-        raise ValueError(msg)
-
-    openi_repo = OpeniRepo(repo_id=repo_id)
-    can_operate = (
-        (openi_repo.access == "write" and openi_repo.is_collaborator)
-        or openi_repo.is_admin
-        or openi_repo.is_onwer
-    )
-    if can_operate is False:
-        msg = f"❌ `{openi_repo.current_user}` 无权限操作此仓库数据集 `{openi_repo.full_display_name}`"
-        log.error(msg)
-        raise ValueError(msg)
-
-    openi_dataset = OpeniDataset(repo_id=openi_repo.repo_id)
-
-    # openifiles
-    tiltle_pbar = tqdm(
-        leave=True,
-        bar_format="{desc}",
-        desc=f"Calculating file md5, this might take a while for large file… ",
-        position=0,
-    )
-
-    openi_file = OpeniFileUpload(
-        local_file=local_file,
-        repo_id=openi_repo.repo_id,
-        upload_type=upload_type,
-        dataset_or_model_id=openi_dataset.dataset_id,
-        dataset_or_model_name=openi_dataset.dataset_name,
-        target_type="dataset",
-    )
-    # tiltle_pbar.close()
-
-    # Display pbar
-    display_progress_bar([openi_file])
-
-    # Upload
-    openi_file.upload_with_tqdm()
-
-    log.info(f"{'-'*200}")
+from ..services import *
+
+log = logger.setup_logger()
+
+
+def upload_file(
+        file: str,
+        repo_id: str,
+        cluster: str = "npu",
+):
+    """
+    upload a dataset file to OpenI
+
+    :param file: lcoal file name
+    :param repo_id: repo id in form of `owner/repo_name`
+    :param cluster: cluster type in [gpu,npu], default is `npu`
+    :return:
+
+    e.g.
+    >>> from openi.dataset import upload_file
+    >>> upload_file("cifar10.zip", "openi/official", cluster="gpu")
+
+    Calculating file md5, this might take a while for large file…
+    Complete( cifar10.zip)(gpu): 100%|████████████████████████| 163MB/163MB [00:00<00:00, 54.0MB/s]
+
+    """
+
+    log.info(f"{'-' * 200}")
+    log.info(f"params - {locals()}")
+
+    upload_type = get_upload_type(cluster)
+
+    # OpeniFileUpload
+    local_file = os.path.expanduser(file)
+    if not os.path.exists(local_file):
+        msg = f"❌ {local_file} 未找到本地文件"
+        log.error(msg)
+        raise ValueError(msg)
+
+    openi_repo = OpeniRepo(repo_id=repo_id)
+    if openi_repo.access != "write":
+        msg = f"❌ `{openi_repo.current_user}` 无权限操作此仓库数据集 `{openi_repo.full_display_name}`"
+        log.error(msg)
+        raise ValueError(msg)
+
+    openi_dataset = OpeniDataset(repo_id=openi_repo.repo_id)
+
+    tqdm.write("Calculating file md5, this might take a while for large file… ")
+    openi_file = OpeniFileUpload(
+        local_file=local_file,
+        repo_id=openi_repo.repo_id,
+        upload_type=upload_type,
+        dataset_or_model_id=openi_dataset.dataset_id,
+        dataset_or_model_name=openi_dataset.dataset_name,
+        target_type="dataset",
+    )
+
+    display_progress_bar([openi_file])
+    openi_file.upload_with_tqdm()
+    log.info(f"{'-' * 200}")
```

### Comparing `openi-1.2.2/src/openi/model/download.py` & `openi-1.3.0/src/openi/model/download.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-import os
-
-from ..utils import logger, constants
-from ..utils.logger import *
-from ..services import *
-
-log = logger.setup_logger()
-
-
-def download_model(
-    repo_id: str,
-    model_name: str,
-    save_path: str = constants.PATH.MODEL_SAVE_PATH,
-):
-    """
-    download a list of model files from OpenI
-
-    :param repo_id: repo id in form of `owner/repo_name`
-    :param model_name: name of model shown on web page
-    :param save_path: local save path, default is `./model`
-    :return:
-
-    e.g.
-    >>> from openi.model import download_model
-    >>> download_model("openi/official", "chatglm2b", save_path="mydata")
-
-    Complete(…kenizer_config.json): 100%|█████████████████████████████████████████████████| 244B/244B [00:00<00:00, 795B/s]
-    Complete(         config.json): 100%|███████████████████████████████████████████| 1.19kB/1.19kB [00:00<00:00, 1.71kB/s]
-    Complete(      .gitattributes): 100%|███████████████████████████████████████████| 1.48kB/1.48kB [00:00<00:00, 1.15kB/s]
-    Complete(…guration_chatglm.py): 100%|█████████████████████████████████████████████| 2.19kB/2.19kB [00:01<00:00, 859B/s]
-    Complete(       MODEL_LICENSE): 100%|█████████████████████████████████████████████| 4.04kB/4.04kB [00:01<00:00, 686B/s]
-    Complete(           README.md): 100%|█████████████████████████████████████████████| 7.89kB/7.89kB [00:01<00:00, 575B/s]
-    Complete(…nization_chatglm.py): 100%|█████████████████████████████████████████████| 9.83kB/9.83kB [00:02<00:00, 491B/s]
-    Complete(     quantization.py): 100%|█████████████████████████████████████████████| 14.3kB/14.3kB [00:02<00:00, 432B/s]
-    Complete(…odel.bin.index.json): 100%|█████████████████████████████████████████████| 20.0kB/20.0kB [00:02<00:00, 384B/s]
-    Complete( modeling_chatglm.py): 100%|█████████████████████████████████████████████| 49.5kB/49.5kB [00:02<00:00, 344B/s]
-    Complete(     tokenizer.model): 100%|███████████████████████████████████████████████| 995kB/995kB [00:03<00:00, 311B/s]
-    Downloading(…-00001-of-00007.bin):   35%|██████████████████████                         | 0.34GB/0.98GB [00:03<?, ?B/s]
-    Waiting(…-00002-of-00007.bin):   0%|                                                     | 0.00B/1.69GB [00:00<?, ?B/s]
-
-    """
-
-    log.info(f"{'-'*200}")
-    log.info(f"params - {locals()}")
-    openi_repo = OpeniRepo(repo_id=repo_id)
-    if openi_repo.access not in ["read", "write"]:
-        msg = f"`{repo_id}` 无权限操作此仓库"
-        log.error(msg)
-        raise ValueError(msg)
-
-    openi_model = OpeniModel(
-        model_name=model_name,
-        repo_id=openi_repo.repo_id,
-    )
-    if openi_model.model_files == []:
-        msg = f"❌ `{model_name}` 未找到文件"
-        log.error(msg)
-        raise ValueError(msg)
-    if openi_model.can_download is False:
-        msg = f"❌ 本机登录用户无此模型下载权限，模型名称 `{openi_model.model_name}`, 仓库名称 `{openi_model.repo_id}`"
-        log.error(msg)
-        raise ValueError(msg)
-
-    save_path = os.path.expanduser(save_path)
-    local_dir = os.path.join(save_path, f"{model_name}")
-    if not os.path.exists(local_dir):
-        os.makedirs(local_dir, exist_ok=True)
-
-    openifiles = list()
-    for targe_file in openi_model.model_files:
-        openi_file = OpeniFileDownload(
-            filename=targe_file["fileName"],
-            size=targe_file["size"],
-            local_dir=local_dir,
-            repo_id=openi_repo.repo_id,
-            dataset_or_model_id=openi_model.model_id,
-            dataset_or_model_name=openi_model.model_name,
-            target_type="model",
-        )
-        openifiles.append(openi_file)
-
-    display_progress_bar(openifiles)
-    for openi_file in openifiles:
-        log.info(f"{'-'*100}")
-        openi_file.download_with_tqdm()
-
-    log.info(f"{'-'*200}")
+import os
+
+from ..utils import logger, constants
+from ..utils.logger import *
+from ..services import *
+
+log = logger.setup_logger()
+
+
+def download_model(
+    repo_id: str,
+    model_name: str,
+    save_path: str = constants.PATH.MODEL_SAVE_PATH,
+):
+    """
+    download a list of model files from OpenI
+
+    :param repo_id: repo id in form of `owner/repo_name`
+    :param model_name: name of model shown on web page
+    :param save_path: local save path, default is `./model`
+    :return:
+
+    e.g.
+    >>> from openi.model import download_model
+    >>> download_model("openi/official", "chatglm2b", save_path="mydata")
+
+    Complete(…kenizer_config.json): 100%|█████████████████████████████████████████████████| 244B/244B [00:00<00:00, 795B/s]
+    Complete(         config.json): 100%|███████████████████████████████████████████| 1.19kB/1.19kB [00:00<00:00, 1.71kB/s]
+    Complete(      .gitattributes): 100%|███████████████████████████████████████████| 1.48kB/1.48kB [00:00<00:00, 1.15kB/s]
+    Complete(…guration_chatglm.py): 100%|█████████████████████████████████████████████| 2.19kB/2.19kB [00:01<00:00, 859B/s]
+    Complete(       MODEL_LICENSE): 100%|█████████████████████████████████████████████| 4.04kB/4.04kB [00:01<00:00, 686B/s]
+    Complete(           README.md): 100%|█████████████████████████████████████████████| 7.89kB/7.89kB [00:01<00:00, 575B/s]
+    Complete(…nization_chatglm.py): 100%|█████████████████████████████████████████████| 9.83kB/9.83kB [00:02<00:00, 491B/s]
+    Complete(     quantization.py): 100%|█████████████████████████████████████████████| 14.3kB/14.3kB [00:02<00:00, 432B/s]
+    Complete(…odel.bin.index.json): 100%|█████████████████████████████████████████████| 20.0kB/20.0kB [00:02<00:00, 384B/s]
+    Complete( modeling_chatglm.py): 100%|█████████████████████████████████████████████| 49.5kB/49.5kB [00:02<00:00, 344B/s]
+    Complete(     tokenizer.model): 100%|███████████████████████████████████████████████| 995kB/995kB [00:03<00:00, 311B/s]
+    Downloading(…-00001-of-00007.bin):   35%|██████████████████████                         | 0.34GB/0.98GB [00:03<?, ?B/s]
+    Waiting(…-00002-of-00007.bin):   0%|                                                     | 0.00B/1.69GB [00:00<?, ?B/s]
+
+    """
+
+    log.info(f"{'-'*200}")
+    log.info(f"params - {locals()}")
+    openi_repo = OpeniRepo(repo_id=repo_id)
+    if openi_repo.access not in ["read", "write"]:
+        msg = f"`{repo_id}` 无权限操作此仓库"
+        log.error(msg)
+        raise ValueError(msg)
+
+    openi_model = OpeniModel(
+        model_name=model_name,
+        repo_id=openi_repo.repo_id,
+    )
+    if openi_model.model_files == []:
+        msg = f"❌ `{model_name}` 未找到文件"
+        log.error(msg)
+        raise ValueError(msg)
+    if openi_model.can_download is False:
+        msg = f"❌ 本机登录用户无此模型下载权限，模型名称 `{openi_model.model_name}`, 仓库名称 `{openi_model.repo_id}`"
+        log.error(msg)
+        raise ValueError(msg)
+
+    save_path = os.path.expanduser(save_path)
+    local_dir = os.path.join(save_path, f"{model_name}")
+    if not os.path.exists(local_dir):
+        os.makedirs(local_dir, exist_ok=True)
+
+    openifiles = list()
+    for targe_file in openi_model.model_files:
+        openi_file = OpeniFileDownload(
+            filename=targe_file["fileName"],
+            size=targe_file["size"],
+            local_dir=local_dir,
+            repo_id=openi_repo.repo_id,
+            dataset_or_model_id=openi_model.model_id,
+            dataset_or_model_name=openi_model.model_name,
+            target_type="model",
+        )
+        openifiles.append(openi_file)
+
+    display_progress_bar(openifiles)
+    for openi_file in openifiles:
+        log.info(f"{'-'*100}")
+        openi_file.download_with_tqdm()
+
+    log.info(f"{'-'*200}")
```

### Comparing `openi-1.2.2/src/openi/model/upload.py` & `openi-1.3.0/src/openi/model/upload.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,100 +1,92 @@
-from tqdm.auto import tqdm
-
-from ..utils import logger, constants
-from ..services import *
-
-log = logger.setup_logger()
-
-
-def upload_model(
-    folder: str,
-    repo_id: str,
-    model_name: str,
-):
-    """
-    upload a local dir (list of model files) to OpenI, not subfolder allowed
-
-    :param folder: local folder name
-    :param repo_id: repo id in form of `owner/repo_name`
-    :param model_name: name of model shown on web page
-    :return:
-
-    e.g.
-    >>> from openi.model import upload_model
-    >>> upload_model("local_dir/chatglm2", "openi/official", "chatglm2b")
-
-    Calculating file md5… (13/13) |███████████████████████████████████████████████████████████████████████████████| [00:00]
-    Complete(…kenizer_config.json): 100%|█████████████████████████████████████████████████| 244B/244B [00:00<00:00, 795B/s]
-    Complete(         config.json): 100%|███████████████████████████████████████████| 1.19kB/1.19kB [00:00<00:00, 1.71kB/s]
-    Complete(      .gitattributes): 100%|███████████████████████████████████████████| 1.48kB/1.48kB [00:00<00:00, 1.15kB/s]
-    Complete(…guration_chatglm.py): 100%|█████████████████████████████████████████████| 2.19kB/2.19kB [00:01<00:00, 859B/s]
-    Complete(       MODEL_LICENSE): 100%|█████████████████████████████████████████████| 4.04kB/4.04kB [00:01<00:00, 686B/s]
-    Complete(           README.md): 100%|█████████████████████████████████████████████| 7.89kB/7.89kB [00:01<00:00, 575B/s]
-    Complete(…nization_chatglm.py): 100%|█████████████████████████████████████████████| 9.83kB/9.83kB [00:02<00:00, 491B/s]
-    Complete(     quantization.py): 100%|█████████████████████████████████████████████| 14.3kB/14.3kB [00:02<00:00, 432B/s]
-    Complete(…odel.bin.index.json): 100%|█████████████████████████████████████████████| 20.0kB/20.0kB [00:02<00:00, 384B/s]
-    Complete( modeling_chatglm.py): 100%|█████████████████████████████████████████████| 49.5kB/49.5kB [00:02<00:00, 344B/s]
-    Complete(     tokenizer.model): 100%|███████████████████████████████████████████████| 995kB/995kB [00:03<00:00, 311B/s]
-    Uploading(…-00001-of-00007.bin):   35%|██████████████████████                           | 0.34GB/0.98GB [00:03<?, ?B/s]
-    Waiting(…-00002-of-00007.bin):   0%|                                                     | 0.00B/1.69GB [00:00<?, ?B/s]
-
-    """
-
-    log.info(f"{'-'*200}")
-    log.info(f"params - {locals()}")
-
-    # OpeniFileUpload
-    local_dir, targe_files = get_upload_folder_files(folder)
-    if targe_files == []:
-        msg = f"❌ {local_dir} 未找到任何本地文件"
-        log.error(msg)
-        raise ValueError(msg)
-
-    # OpeniRepo, check repo_id, access
-    openi_repo = OpeniRepo(repo_id=repo_id)
-
-    # OpeniModel
-    openi_model = OpeniModel(
-        model_name=model_name,
-        repo_id=openi_repo.repo_id,
-    )
-    if openi_model.can_operate is False:
-        msg = f"❌ `{openi_repo.current_user}` 无此模型上传权限，模型名称 `{openi_model.model_name}`, 仓库名称 `{openi_model.repo_id}`"
-        log.error(msg)
-        raise ValueError(msg)
-    if openi_model.model_type == 0:
-        msg = f"❌ `{openi_model.model_name}` 为线上模型，无法上传本地文件"
-        log.error(msg)
-        raise ValueError(msg)
-
-    # openifiles
-    tiltle_pbar = tqdm(
-        total=len(targe_files),
-        leave=True,
-        bar_format="{desc}({n_fmt}/{total_fmt}) |{bar}| [{elapsed}]",
-        desc=f"Calculating file md5… ",
-        position=0,
-    )
-    openifiles = list()
-    for file in targe_files:
-        openi_file = OpeniFileUpload(
-            local_file=file,
-            repo_id=openi_repo.repo_id,
-            upload_type=constants.FILE.DEFAULT_UPLOAD_TYPE,
-            dataset_or_model_id=openi_model.model_id,
-            dataset_or_model_name=openi_model.model_name,
-            target_type="model",
-        )
-        tiltle_pbar.update(1)
-        openifiles.append(openi_file)
-    # tiltle_pbar.close()
-
-    # # Display pbar
-    display_progress_bar(openifiles)
-
-    # # Upload
-    for openi_file in openifiles:
-        log.info(f"{'-'*200}")
-        openi_file.upload_with_tqdm()
-
-    log.info(f"{'-'*200}")
+from ..services import *
+
+log = logger.setup_logger()
+
+
+def upload_model(
+        folder: str,
+        repo_id: str,
+        model_name: str,
+):
+    """
+    upload a local dir (list of model files) to OpenI, not subfolder allowed
+
+    :param folder: local folder name
+    :param repo_id: repo id in form of `owner/repo_name`
+    :param model_name: name of model shown on web page
+    :return:
+
+    e.g.
+    >>> from openi.model import upload_model
+    >>> upload_model("local_dir/chatglm2", "openi/official", "chatglm2b")
+
+    Calculating file md5… (13/13) |███████████████████████████████████████████████████████████████████████████████| [00:00]
+    Complete(…kenizer_config.json): 100%|█████████████████████████████████████████████████| 244B/244B [00:00<00:00, 795B/s]
+    Complete(         config.json): 100%|███████████████████████████████████████████| 1.19kB/1.19kB [00:00<00:00, 1.71kB/s]
+    Complete(      .gitattributes): 100%|███████████████████████████████████████████| 1.48kB/1.48kB [00:00<00:00, 1.15kB/s]
+    Complete(…guration_chatglm.py): 100%|█████████████████████████████████████████████| 2.19kB/2.19kB [00:01<00:00, 859B/s]
+    Complete(       MODEL_LICENSE): 100%|█████████████████████████████████████████████| 4.04kB/4.04kB [00:01<00:00, 686B/s]
+    Complete(           README.md): 100%|█████████████████████████████████████████████| 7.89kB/7.89kB [00:01<00:00, 575B/s]
+    Complete(…nization_chatglm.py): 100%|█████████████████████████████████████████████| 9.83kB/9.83kB [00:02<00:00, 491B/s]
+    Complete(     quantization.py): 100%|█████████████████████████████████████████████| 14.3kB/14.3kB [00:02<00:00, 432B/s]
+    Complete(…odel.bin.index.json): 100%|█████████████████████████████████████████████| 20.0kB/20.0kB [00:02<00:00, 384B/s]
+    Complete( modeling_chatglm.py): 100%|█████████████████████████████████████████████| 49.5kB/49.5kB [00:02<00:00, 344B/s]
+    Complete(     tokenizer.model): 100%|███████████████████████████████████████████████| 995kB/995kB [00:03<00:00, 311B/s]
+    Uploading(…-00001-of-00007.bin):   35%|██████████████████████                           | 0.34GB/0.98GB [00:03<?, ?B/s]
+    Waiting(…-00002-of-00007.bin):   0%|                                                     | 0.00B/1.69GB [00:00<?, ?B/s]
+
+    """
+
+    log.info(f"{'-' * 200}")
+    log.info(f"params - {locals()}")
+
+    local_root, targe_files = get_upload_all_files(folder)
+    if not targe_files:
+        msg = f"❌ {local_root} 未找到任何本地文件"
+        log.error(msg)
+        raise ValueError(msg)
+
+    openi_repo = OpeniRepo(repo_id=repo_id)
+
+    openi_model = OpeniModel(
+        model_name=model_name,
+        repo_id=openi_repo.repo_id,
+    )
+    if openi_model.can_operate is False:
+        msg = f"❌ `{openi_repo.current_user}` 无此模型上传权限，模型名称 `{openi_model.model_name}`, 仓库名称 `{openi_model.repo_id}`"
+        log.error(msg)
+        raise ValueError(msg)
+    if openi_model.model_type == 0:
+        msg = f"❌ `{openi_model.model_name}` 为线上模型，无法上传本地文件"
+        log.error(msg)
+        raise ValueError(msg)
+
+    tiltle_pbar = tqdm(
+        total=len(targe_files),
+        leave=True,
+        bar_format="{desc}({n_fmt}/{total_fmt}) |{bar}| [{elapsed}]",
+        desc=f"Calculating file md5… ",
+        position=0,
+    )
+    openifiles = list()
+    for file in targe_files:
+        openi_file = OpeniFileUpload(
+            local_root=local_root,
+            local_file=file,
+            repo_id=openi_repo.repo_id,
+            upload_type=constants.FILE.DEFAULT_UPLOAD_TYPE,
+            dataset_or_model_id=openi_model.model_id,
+            dataset_or_model_name=openi_model.model_name,
+            target_type="model",
+        )
+        tiltle_pbar.update(1)
+        openifiles.append(openi_file)
+    tiltle_pbar.refresh()
+    tiltle_pbar.close()
+
+    display_progress_bar(openifiles)
+
+    for openi_file in openifiles:
+        log.info(f"{'-' * 200}")
+        openi_file.upload_with_tqdm()
+    log.info(f"{'-' * 200}")
```

### Comparing `openi-1.2.2/src/openi/services/model_struct.py` & `openi-1.3.0/src/openi/services/model_struct.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,91 +1,88 @@
-from dataclasses import dataclass
-
-from ..apis import OpeniAPI
-from ..utils import logger, constants
-
-
-log = logger.setup_logger()
-
-
-def get_engine(engine: str):
-    try:
-        engine_type = constants.API.ENGINE_TYPE.index(engine.lower())
-        return engine_type
-    except:
-        msg = f"❌ `engine` 参数为[pytorch, tensorflow, mindspore, paddlepaddle, oneflow, mxnet, other]其中之一，不区分大小写"
-        log.error(msg)
-        raise ValueError(msg)
-
-
-@dataclass
-class OpeniModel:
-    model_name: str
-    repo_id: str
-    model_id: str = None
-    storage_path: str = None
-    model_files: list = None
-    model_type: int = None
-    model_creator: str = None
-
-    # api = OpeniAPI()
-
-    def __post_init__(self):
-        self.api = OpeniAPI()
-        self.get_model_id_by_name()
-        self.get_model_file()
-        log.info(f"OpeniModel Object init: {self.__dict__}")
-
-    def get_model_id_by_name(self):  # repo_id, model_name):
-        try:
-            response = self.api.model_query_by_name(
-                repo_id=self.repo_id,
-                model_name=self.model_name,
-            ).json()
-            self.model_id = response[0]["id"]
-            self.storage_path = response[0]["path"]
-            self.model_type = response[0]["modelType"]
-            self.model_creator = response[0]["userName"]
-            self.can_operate = response[0]["isCanOper"]
-            self.can_download = response[0]["isCanDownload"]
-        except:
-            msg = f"❌ `{self.repo_id}` 未找到名为 `{self.model_name}` 的模型"
-            log.error(msg)
-            raise ValueError(msg)
-
-    def get_model_file(self):
-        try:
-            response = self.api.model_file_query_by_id(
-                repo_id=self.repo_id,
-                model_id=self.model_id,
-            ).json()
-            sorted_model_files = sorted(response, key=lambda x: x["size"])
-            self.model_files = sorted_model_files
-        except:
-            msg = f"❌ `{self.repo_id}`-`{self.model_name}` 获取模型文件列表失败"
-            log.error(msg)
-            raise ValueError(msg)
-
-
-def get_model_files_by_id(repo_id, model_id):
-    try:
-        api = OpeniAPI()
-        model_files = api.model_file_query_by_id(
-            repo_id=repo_id, model_id=model_id
-        ).json()
-        return model_files
-    except:
-        msg = f"❌ "
-        log.error(msg)
-        raise ValueError(msg)
-
-
-def create_model(repo_id, model_name):
-    api = OpeniAPI()
-    response = api.model_create(repo_id, model_name)
-    if response.json()["code"] == "0":
-        model_id = response.json()["id"]
-        return model_id
-    else:
-        msg = f"model create failed, {response.json()['msg']}"
-        log.error(msg)
-        raise ValueError(msg)
+from dataclasses import dataclass
+
+from ..apis import OpeniAPI
+from ..utils import logger, constants
+
+log = logger.setup_logger()
+
+
+def get_engine(engine: str):
+    try:
+        engine_type = constants.API.ENGINE_TYPE.index(engine.lower())
+        return engine_type
+    except:
+        msg = f"❌ `engine` 参数为[pytorch, tensorflow, mindspore, paddlepaddle, oneflow, mxnet, other]其中之一，不区分大小写"
+        log.error(msg)
+        raise ValueError(msg)
+
+
+@dataclass
+class OpeniModel:
+    model_name: str
+    repo_id: str
+    model_id: str = None
+    storage_path: str = None
+    model_files: list = None
+    model_type: int = None
+    model_creator: str = None
+
+    def __post_init__(self):
+        self.api = OpeniAPI()
+        self.get_model_id_by_name()
+        self.get_model_file()
+        log.info(f"OpeniModel Object init: {self.__dict__}")
+
+    def get_model_id_by_name(self):  # repo_id, model_name):
+        try:
+            response = self.api.model_query_by_name(
+                repo_id=self.repo_id,
+                model_name=self.model_name,
+            ).json()
+            self.model_id = response[0]["id"]
+            self.storage_path = response[0]["path"]
+            self.model_type = response[0]["modelType"]
+            self.model_creator = response[0]["userName"]
+            self.can_operate = response[0]["isCanOper"]
+            self.can_download = response[0]["isCanDownload"]
+        except:
+            msg = f"❌ `{self.repo_id}` 未找到名为 `{self.model_name}` 的模型"
+            log.error(msg)
+            raise ValueError(msg)
+
+    def get_model_file(self):
+        try:
+            response = self.api.model_file_query_by_id(
+                repo_id=self.repo_id,
+                model_id=self.model_id,
+            ).json()
+            sorted_model_files = sorted(response, key=lambda x: x["size"])
+            self.model_files = sorted_model_files
+        except:
+            msg = f"❌ `{self.repo_id}`-`{self.model_name}` 获取模型文件列表失败"
+            log.error(msg)
+            raise ValueError(msg)
+
+
+def get_model_files_by_id(repo_id, model_id):
+    try:
+        api = OpeniAPI()
+        model_files = api.model_file_query_by_id(
+            repo_id=repo_id, model_id=model_id
+        ).json()
+        return model_files
+    except:
+        msg = f"❌ "
+        log.error(msg)
+        raise ValueError(msg)
+
+
+def create_model(repo_id, model_name):
+    api = OpeniAPI()
+    response = api.model_create(repo_id, model_name)
+    if response.json()["code"] == "0":
+        model_id = response.json()["id"]
+        return model_id
+    else:
+        msg = f"model create failed, {response.json()['msg']}"
+        log.error(msg)
+        raise ValueError(msg)
```

### Comparing `openi-1.2.2/src/openi/utils/logger.py` & `openi-1.3.0/src/openi/utils/logger.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-import logging
-import os
-import json
-import time
-from datetime import datetime
-
-from .constants import *
-
-
-def setup_logger():
-    LOG_FORMAT = "%(asctime)s [%(levelname)s] %(funcName)s(): %(message)s"  # %(filename)s %(funcName)s():
-    DATE_FORMAT = "%Y/%m/%d %H:%M:%S"
-    LOG_SUFFIX = time.strftime("%Y%m%d")
-    LOG_FILE = os.path.join(PATH.LOG_PATH, f"{LOG_SUFFIX}.log")
-    logging.addLevelName(25, "HTTP")
-    logging.addLevelName(26, "RESPONSE")
-
-    logging.basicConfig(
-        filename=LOG_FILE,
-        level=logging.INFO,
-        format=LOG_FORMAT,
-        datefmt=DATE_FORMAT,
-    )
-    logger = logging.getLogger(__name__)
-
-    def http(self, message, *args, **kws):
-        if self.isEnabledFor(25):
-            self._log(25, message, args, **kws)
-
-    def response(self, message, *args, **kws):
-        if self.isEnabledFor(26):
-            self._log(26, message, args, **kws)
-
-    logging.Logger.http = http
-    logging.Logger.response = response
-
-    return logger
-
-
-def get_time():
-    return datetime.now().strftime("%H:%M:%S")
-
-
-def algnprint(input_dict):
-    max_key_length = max(len(key) for key in input_dict.keys()) + 1
-    for key, value in input_dict.items():
-        key += ":"
-        formatted_key = f"{key:{max_key_length}}"
-        print(f"{formatted_key} {value}")
-
-
-def jprint(dict):
-    print(json.dumps(dict, indent=4, ensure_ascii=False))
-
-
-def jlog(dict):
-    return json.dumps(dict, indent=4, ensure_ascii=False)
-
-
-def jsave(dict, dir=None):
-    with open(dir, "w+") as f:
-        json.dump(dict, f, indent=4, ensure_ascii=False)
-    print(f"jsave to {dir}")
-
-
-def lprint(list, with_index=True):
-    max_index_width = len(str(len(list) - 1))
-    for index, item in enumerate(list):
-        if with_index:
-            index_str = str(index).rjust(max_index_width)
-            print(f"{index_str} {item}")
-        else:
-            print(item)
+import logging
+import os
+import json
+import time
+from datetime import datetime
+
+from .constants import *
+
+
+def setup_logger():
+    LOG_FORMAT = "%(asctime)s [%(levelname)s] %(funcName)s(): %(message)s"  # %(filename)s %(funcName)s():
+    DATE_FORMAT = "%Y/%m/%d %H:%M:%S"
+    LOG_SUFFIX = time.strftime("%Y%m%d")
+    LOG_FILE = os.path.join(PATH.LOG_PATH, f"{LOG_SUFFIX}.log")
+    logging.addLevelName(25, "HTTP")
+    logging.addLevelName(26, "RESPONSE")
+
+    logging.basicConfig(
+        filename=LOG_FILE,
+        level=logging.INFO,
+        format=LOG_FORMAT,
+        datefmt=DATE_FORMAT,
+    )
+    logger = logging.getLogger(__name__)
+
+    def http(self, message, *args, **kws):
+        if self.isEnabledFor(25):
+            self._log(25, message, args, **kws)
+
+    def response(self, message, *args, **kws):
+        if self.isEnabledFor(26):
+            self._log(26, message, args, **kws)
+
+    logging.Logger.http = http
+    logging.Logger.response = response
+
+    return logger
+
+
+def get_time():
+    return datetime.now().strftime("%H:%M:%S")
+
+
+def algnprint(input_dict):
+    max_key_length = max(len(key) for key in input_dict.keys()) + 1
+    for key, value in input_dict.items():
+        key += ":"
+        formatted_key = f"{key:{max_key_length}}"
+        print(f"{formatted_key} {value}")
+
+
+def jprint(dict):
+    print(json.dumps(dict, indent=4, ensure_ascii=False))
+
+
+def jlog(dict):
+    return json.dumps(dict, indent=4, ensure_ascii=False)
+
+
+def jsave(dict, dir=None):
+    with open(dir, "w+") as f:
+        json.dump(dict, f, indent=4, ensure_ascii=False)
+    print(f"jsave to {dir}")
+
+
+def lprint(list, with_index=True):
+    max_index_width = len(str(len(list) - 1))
+    for index, item in enumerate(list):
+        if with_index:
+            index_str = str(index).rjust(max_index_width)
+            print(f"{index_str} {item}")
+        else:
+            print(item)
```

### Comparing `openi-1.2.2/src/openi.egg-info/SOURCES.txt` & `openi-1.3.0/src/openi.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 README.md
 setup.py
 src/openi/__init__.py
+src/openi/_login.py
 src/openi/apis.py
 src/openi/cli.py
-src/openi/login.py
 src/openi.egg-info/PKG-INFO
 src/openi.egg-info/SOURCES.txt
 src/openi.egg-info/dependency_links.txt
 src/openi.egg-info/entry_points.txt
 src/openi.egg-info/requires.txt
 src/openi.egg-info/top_level.txt
 src/openi/dataset/__init__.py
```

