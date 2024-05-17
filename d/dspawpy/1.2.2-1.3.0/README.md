# Comparing `tmp/dspawpy-1.2.2.tar.gz` & `tmp/dspawpy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dspawpy-1.2.2.tar", last modified: Thu Apr 11 08:22:12 2024, max compression
+gzip compressed data, was "dspawpy-1.3.0.tar", last modified: Fri May 17 09:31:09 2024, max compression
```

## Comparing `dspawpy-1.2.2.tar` & `dspawpy-1.3.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-11 08:22:12.338863 dspawpy-1.2.2/
--rw-r--r--   0 zzl       (1000) zzl       (1000)     1055 2024-01-26 06:56:39.000000 dspawpy-1.2.2/LICENSE.txt
--rw-r--r--   0 zzl       (1000) zzl       (1000)    11717 2024-04-11 08:22:12.336866 dspawpy-1.2.2/PKG-INFO
--rw-r--r--   0 zzl       (1000) zzl       (1000)    11526 2024-04-11 08:13:27.000000 dspawpy-1.2.2/README.md
-drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-11 08:22:12.294652 dspawpy-1.2.2/dspawpy/
--rw-r--r--   0 zzl       (1000) zzl       (1000)       46 2024-04-11 08:22:10.000000 dspawpy-1.2.2/dspawpy/__init__.py
-drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-11 08:22:12.308867 dspawpy-1.2.2/dspawpy/analysis/
--rw-r--r--   0 zzl       (1000) zzl       (1000)        0 2023-11-28 02:22:30.000000 dspawpy-1.2.2/dspawpy/analysis/__init__.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    29688 2024-03-27 08:59:24.000000 dspawpy-1.2.2/dspawpy/analysis/aimdtools.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    19672 2024-03-27 09:01:23.000000 dspawpy-1.2.2/dspawpy/analysis/vacf.py
-drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-11 08:22:12.312867 dspawpy-1.2.2/dspawpy/cli/
--rw-r--r--   0 zzl       (1000) zzl       (1000)        0 2024-01-26 06:56:39.000000 dspawpy-1.2.2/dspawpy/cli/__init__.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    65500 2024-04-11 08:13:27.000000 dspawpy-1.2.2/dspawpy/cli/cli.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    65297 2024-04-11 08:13:27.000000 dspawpy-1.2.2/dspawpy/cli/cli_en.py
-drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-11 08:22:12.321865 dspawpy-1.2.2/dspawpy/diffusion/
--rw-r--r--   0 zzl       (1000) zzl       (1000)        0 2023-11-28 02:22:30.000000 dspawpy-1.2.2/dspawpy/diffusion/__init__.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)     3718 2024-03-27 02:02:22.000000 dspawpy-1.2.2/dspawpy/diffusion/neb.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    60374 2024-03-28 02:11:43.000000 dspawpy-1.2.2/dspawpy/diffusion/nebtools.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    10749 2024-03-27 09:26:05.000000 dspawpy-1.2.2/dspawpy/diffusion/pathfinder.py
-drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-11 08:22:12.331862 dspawpy-1.2.2/dspawpy/io/
--rw-r--r--   0 zzl       (1000) zzl       (1000)        0 2023-11-28 02:22:30.000000 dspawpy-1.2.2/dspawpy/io/__init__.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    62058 2024-04-10 09:19:19.000000 dspawpy-1.2.2/dspawpy/io/read.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    26244 2024-03-27 09:31:14.000000 dspawpy-1.2.2/dspawpy/io/structure.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    33242 2024-03-27 09:28:27.000000 dspawpy-1.2.2/dspawpy/io/utils.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    27196 2024-03-27 09:29:46.000000 dspawpy-1.2.2/dspawpy/io/write.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    48744 2024-04-11 08:13:21.000000 dspawpy-1.2.2/dspawpy/plot.py
-drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-11 08:22:12.332863 dspawpy-1.2.2/dspawpy.egg-info/
--rw-r--r--   0 zzl       (1000) zzl       (1000)    11717 2024-04-11 08:22:12.000000 dspawpy-1.2.2/dspawpy.egg-info/PKG-INFO
--rw-r--r--   0 zzl       (1000) zzl       (1000)      626 2024-04-11 08:22:12.000000 dspawpy-1.2.2/dspawpy.egg-info/SOURCES.txt
--rw-r--r--   0 zzl       (1000) zzl       (1000)        1 2024-04-11 08:22:12.000000 dspawpy-1.2.2/dspawpy.egg-info/dependency_links.txt
--rw-r--r--   0 zzl       (1000) zzl       (1000)       76 2024-04-11 08:22:12.000000 dspawpy-1.2.2/dspawpy.egg-info/entry_points.txt
--rw-r--r--   0 zzl       (1000) zzl       (1000)       64 2024-04-11 08:22:12.000000 dspawpy-1.2.2/dspawpy.egg-info/requires.txt
--rw-r--r--   0 zzl       (1000) zzl       (1000)        8 2024-04-11 08:22:12.000000 dspawpy-1.2.2/dspawpy.egg-info/top_level.txt
--rw-r--r--   0 zzl       (1000) zzl       (1000)       38 2024-04-11 08:22:12.338863 dspawpy-1.2.2/setup.cfg
--rw-r--r--   0 zzl       (1000) zzl       (1000)     1308 2024-04-11 08:22:10.000000 dspawpy-1.2.2/setup.py
+drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-17 09:31:09.927343 dspawpy-1.3.0/
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)     1055 2024-05-16 07:21:06.000000 dspawpy-1.3.0/LICENSE.txt
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    13057 2024-05-17 09:31:09.926342 dspawpy-1.3.0/PKG-INFO
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    12869 2024-05-17 02:08:20.000000 dspawpy-1.3.0/README.md
+drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-17 09:31:09.894337 dspawpy-1.3.0/dspawpy/
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)      727 2024-05-17 09:31:08.000000 dspawpy-1.3.0/dspawpy/__init__.py
+drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-17 09:31:09.905368 dspawpy-1.3.0/dspawpy/analysis/
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-16 07:21:06.000000 dspawpy-1.3.0/dspawpy/analysis/__init__.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    30293 2024-05-17 02:08:20.000000 dspawpy-1.3.0/dspawpy/analysis/aimdtools.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    17645 2024-05-17 02:08:20.000000 dspawpy-1.3.0/dspawpy/analysis/vacf.py
+drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-17 09:31:09.910338 dspawpy-1.3.0/dspawpy/cli/
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-16 07:21:06.000000 dspawpy-1.3.0/dspawpy/cli/__init__.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    47124 2024-05-17 02:08:20.000000 dspawpy-1.3.0/dspawpy/cli/aux.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)     8493 2024-05-17 02:08:20.000000 dspawpy-1.3.0/dspawpy/cli/cli.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    17882 2024-05-17 02:08:20.000000 dspawpy-1.3.0/dspawpy/cli/menu_prompts.py
+drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-17 09:31:09.915337 dspawpy-1.3.0/dspawpy/diffusion/
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-16 07:21:06.000000 dspawpy-1.3.0/dspawpy/diffusion/__init__.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)     3551 2024-05-17 02:08:20.000000 dspawpy-1.3.0/dspawpy/diffusion/neb.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    63167 2024-05-17 02:08:20.000000 dspawpy-1.3.0/dspawpy/diffusion/nebtools.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    10751 2024-05-17 02:08:20.000000 dspawpy-1.3.0/dspawpy/diffusion/pathfinder.py
+drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-17 09:31:09.923341 dspawpy-1.3.0/dspawpy/io/
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-16 07:21:06.000000 dspawpy-1.3.0/dspawpy/io/__init__.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    63584 2024-05-17 02:08:20.000000 dspawpy-1.3.0/dspawpy/io/read.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    26571 2024-05-17 02:08:20.000000 dspawpy-1.3.0/dspawpy/io/structure.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    30750 2024-05-17 02:08:20.000000 dspawpy-1.3.0/dspawpy/io/utils.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    27382 2024-05-17 02:08:20.000000 dspawpy-1.3.0/dspawpy/io/write.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    53586 2024-05-17 02:08:20.000000 dspawpy-1.3.0/dspawpy/plot.py
+drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-17 09:31:09.924343 dspawpy-1.3.0/dspawpy.egg-info/
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    13057 2024-05-17 09:31:09.000000 dspawpy-1.3.0/dspawpy.egg-info/PKG-INFO
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)      651 2024-05-17 09:31:09.000000 dspawpy-1.3.0/dspawpy.egg-info/SOURCES.txt
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        1 2024-05-17 09:31:09.000000 dspawpy-1.3.0/dspawpy.egg-info/dependency_links.txt
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)       76 2024-05-17 09:31:09.000000 dspawpy-1.3.0/dspawpy.egg-info/entry_points.txt
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)       67 2024-05-17 09:31:09.000000 dspawpy-1.3.0/dspawpy.egg-info/requires.txt
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        8 2024-05-17 09:31:09.000000 dspawpy-1.3.0/dspawpy.egg-info/top_level.txt
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)       38 2024-05-17 09:31:09.928338 dspawpy-1.3.0/setup.cfg
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)     1016 2024-05-17 09:31:08.000000 dspawpy-1.3.0/setup.py
```

### Comparing `dspawpy-1.2.2/LICENSE.txt` & `dspawpy-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dspawpy-1.2.2/PKG-INFO` & `dspawpy-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: dspawpy
-Version: 1.2.2
+Version: 1.3.0
 Summary: Tools for dspaw
 Home-page: http://www.hzwtech.com/
 Author: Hzwtech
 Author-email: ZhengZhilin@hzwtech.com
 License: MIT
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: pymatgen>=2022.2.7
+Requires-Dist: pymatgen
 Requires-Dist: statsmodels
 Requires-Dist: h5py
-Requires-Dist: monty
 Requires-Dist: prompt_toolkit
 Requires-Dist: loguru
+Requires-Dist: polars
+Requires-Dist: ruamel.yaml
 
 ![Pyversion](https://img.shields.io/badge/dynamic/json?query=info.requires_python&label=python&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fgeojson-rewind%2Fjson)
 ![PyPI](https://img.shields.io/pypi/v/dspawpy?label=pypi%20package)
 ![PyPI - Downloads](https://static.pepy.tech/badge/dspawpy/month)
 
 # Introduction （简介）
 
@@ -36,23 +37,44 @@
 
 ```bash
 conda install -c conda-forge dspawpy
 ```
 
 ## CHANGELOG （版本更新简述）
 
+### 1.3.0
+
+- 重要变更： 不再支持python3.8（不含）以下版本
+- 重要变更： 合并cli.py和cli_en.py，通过命令行选项 -l 或 --language 切换交互提示语言
+- 重构： 命令行交互程序增加静默运行模式，便于编程调用
+- 重构： 命令行交互程序大幅提高可读性，在等待用户输入同时多线程动态载入最终调用的函数
+- 重构： 懒导入——将导包语句从文件开头尽量移入函数中，避免导入不必要模块，减少导包耗时
+- 重构： 绝大多数参数补充类型提示，解决所有已知的静态检查问题
+- 体验优化： cli在输入部分参数时增加Tab键获取提示的功能
+- 体验优化： cli增加命令行参数帮助菜单
+- 体验优化： 全局使用 loguru 库的 catch 修饰器，控制报错信息的详细程度
+- 体验优化:  average_along_axis potential类型支持自动判断内部subtype类型为 TotalLocalPotential 的情况
+- 体验优化： 用 polars 库替换了 pandas 库，加速处理多维数据
+- BUG修复： write_vesta 插值体积数据部分变量未及时更新
+- BUG修复： rdf 修复 density 变量缺失的问题
+- BUG修复： cli 8.4 neb 
+
+
+### 1.2.2
+
+- BUG修复： dos和band读取非线性自旋算例的 h5/json 输出文件时，对自旋判断不准
+
 ### 1.2.0
 
-- 体验优化： 将导包语句从文件开头移入函数中，大幅减少python脚本的import时间
+- 体验优化： cli将导包语句从文件开头移入函数中，大幅减少python脚本的import时间
 - 体验优化： cli增加模糊匹配功能
 - 体验优化： optical绘图默认绘制全部数据以便查看
 - 体验优化： neb备份时如果目标文件夹已存在，将原先的改名成附加时间戳的文件夹
 - BUG修复： dos非线性自旋时无法读取h5/json数据
 
-
 ### 1.1.9
 
 - BUG修复： 修复cli的一些已知bug
 
 ### 1.1.8
 
 - 功能强化： 体数据（volumetric data）支持自定义网格插值（调用scipy的RegularGridInterpolator插值器）；增加 txt 格式支持，每行包含格点的 xyz 坐标和具体数值
```

### Comparing `dspawpy-1.2.2/README.md` & `dspawpy-1.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -18,23 +18,44 @@
 
 ```bash
 conda install -c conda-forge dspawpy
 ```
 
 ## CHANGELOG （版本更新简述）
 
+### 1.3.0
+
+- 重要变更： 不再支持python3.8（不含）以下版本
+- 重要变更： 合并cli.py和cli_en.py，通过命令行选项 -l 或 --language 切换交互提示语言
+- 重构： 命令行交互程序增加静默运行模式，便于编程调用
+- 重构： 命令行交互程序大幅提高可读性，在等待用户输入同时多线程动态载入最终调用的函数
+- 重构： 懒导入——将导包语句从文件开头尽量移入函数中，避免导入不必要模块，减少导包耗时
+- 重构： 绝大多数参数补充类型提示，解决所有已知的静态检查问题
+- 体验优化： cli在输入部分参数时增加Tab键获取提示的功能
+- 体验优化： cli增加命令行参数帮助菜单
+- 体验优化： 全局使用 loguru 库的 catch 修饰器，控制报错信息的详细程度
+- 体验优化:  average_along_axis potential类型支持自动判断内部subtype类型为 TotalLocalPotential 的情况
+- 体验优化： 用 polars 库替换了 pandas 库，加速处理多维数据
+- BUG修复： write_vesta 插值体积数据部分变量未及时更新
+- BUG修复： rdf 修复 density 变量缺失的问题
+- BUG修复： cli 8.4 neb 
+
+
+### 1.2.2
+
+- BUG修复： dos和band读取非线性自旋算例的 h5/json 输出文件时，对自旋判断不准
+
 ### 1.2.0
 
-- 体验优化： 将导包语句从文件开头移入函数中，大幅减少python脚本的import时间
+- 体验优化： cli将导包语句从文件开头移入函数中，大幅减少python脚本的import时间
 - 体验优化： cli增加模糊匹配功能
 - 体验优化： optical绘图默认绘制全部数据以便查看
 - 体验优化： neb备份时如果目标文件夹已存在，将原先的改名成附加时间戳的文件夹
 - BUG修复： dos非线性自旋时无法读取h5/json数据
 
-
 ### 1.1.9
 
 - BUG修复： 修复cli的一些已知bug
 
 ### 1.1.8
 
 - 功能强化： 体数据（volumetric data）支持自定义网格插值（调用scipy的RegularGridInterpolator插值器）；增加 txt 格式支持，每行包含格点的 xyz 坐标和具体数值
```

### Comparing `dspawpy-1.2.2/dspawpy/analysis/aimdtools.py` & `dspawpy-1.3.0/dspawpy/io/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,885 +1,1144 @@
 # -*- coding: utf-8 -*-
-import os
-import warnings
-from typing import List, Union
+# ! some functions are extracted from ase
+# see https://wiki.fysik.dtu.dk/ase/index.html
 
+from typing import List
+from loguru import logger
+import numpy as np
+
+Na = 6.02214179e23  # 阿伏伽德罗常数 单位 /mol
+h = 6.6260696e-34  # 普朗克常数 单位J*s
+kB = 1.3806503e-23  # 玻尔兹曼常数 J/K
+R = Na * kB  # 理想气体常数 J/(K*mol)
+amu = 1.66053906660e-27  # 原子质量单位 kg
+k = 1.380649e-23 / 1.602176634e-19  # eV/K
+atomic_masses_iupac2016 = np.array(
+    [
+        1.0,  # X
+        1.008,  # H [1.00784, 1.00811]
+        4.002602,  # He
+        6.94,  # Li [6.938, 6.997]
+        9.0121831,  # Be
+        10.81,  # B [10.806, 10.821]
+        12.011,  # C [12.0096, 12.0116]
+        14.007,  # N [14.00643, 14.00728]
+        15.999,  # O [15.99903, 15.99977]
+        18.998403163,  # F
+        20.1797,  # Ne
+        22.98976928,  # Na
+        24.305,  # Mg [24.304, 24.307]
+        26.9815385,  # Al
+        28.085,  # Si [28.084, 28.086]
+        30.973761998,  # P
+        32.06,  # S [32.059, 32.076]
+        35.45,  # Cl [35.446, 35.457]
+        39.948,  # Ar
+        39.0983,  # K
+        40.078,  # Ca
+        44.955908,  # Sc
+        47.867,  # Ti
+        50.9415,  # V
+        51.9961,  # Cr
+        54.938044,  # Mn
+        55.845,  # Fe
+        58.933194,  # Co
+        58.6934,  # Ni
+        63.546,  # Cu
+        65.38,  # Zn
+        69.723,  # Ga
+        72.630,  # Ge
+        74.921595,  # As
+        78.971,  # Se
+        79.904,  # Br [79.901, 79.907]
+        83.798,  # Kr
+        85.4678,  # Rb
+        87.62,  # Sr
+        88.90584,  # Y
+        91.224,  # Zr
+        92.90637,  # Nb
+        95.95,  # Mo
+        97.90721,  # 98Tc
+        101.07,  # Ru
+        102.90550,  # Rh
+        106.42,  # Pd
+        107.8682,  # Ag
+        112.414,  # Cd
+        114.818,  # In
+        118.710,  # Sn
+        121.760,  # Sb
+        127.60,  # Te
+        126.90447,  # I
+        131.293,  # Xe
+        132.90545196,  # Cs
+        137.327,  # Ba
+        138.90547,  # La
+        140.116,  # Ce
+        140.90766,  # Pr
+        144.242,  # Nd
+        144.91276,  # 145Pm
+        150.36,  # Sm
+        151.964,  # Eu
+        157.25,  # Gd
+        158.92535,  # Tb
+        162.500,  # Dy
+        164.93033,  # Ho
+        167.259,  # Er
+        168.93422,  # Tm
+        173.054,  # Yb
+        174.9668,  # Lu
+        178.49,  # Hf
+        180.94788,  # Ta
+        183.84,  # W
+        186.207,  # Re
+        190.23,  # Os
+        192.217,  # Ir
+        195.084,  # Pt
+        196.966569,  # Au
+        200.592,  # Hg
+        204.38,  # Tl [204.382, 204.385]
+        207.2,  # Pb
+        208.98040,  # Bi
+        208.98243,  # 209Po
+        209.98715,  # 210At
+        222.01758,  # 222Rn
+        223.01974,  # 223Fr
+        226.02541,  # 226Ra
+        227.02775,  # 227Ac
+        232.0377,  # Th
+        231.03588,  # Pa
+        238.02891,  # U
+        237.04817,  # 237Np
+        244.06421,  # 244Pu
+        243.06138,  # 243Am
+        247.07035,  # 247Cm
+        247.07031,  # 247Bk
+        251.07959,  # 251Cf
+        252.0830,  # 252Es
+        257.09511,  # 257Fm
+        258.09843,  # 258Md
+        259.1010,  # 259No
+        262.110,  # 262Lr
+        267.122,  # 267Rf
+        268.126,  # 268Db
+        271.134,  # 271Sg
+        270.133,  # 270Bh
+        269.1338,  # 269Hs
+        278.156,  # 278Mt
+        281.165,  # 281Ds
+        281.166,  # 281Rg
+        285.177,  # 285Cn
+        286.182,  # 286Nh
+        289.190,  # 289Fl
+        289.194,  # 289Mc
+        293.204,  # 293Lv
+        293.208,  # 293Ts
+        294.214,  # 294Og
+    ]
+)
+
+chemical_symbols = [
+    # 0
+    "X",
+    # 1
+    "H",
+    "He",
+    # 2
+    "Li",
+    "Be",
+    "B",
+    "C",
+    "N",
+    "O",
+    "F",
+    "Ne",
+    # 3
+    "Na",
+    "Mg",
+    "Al",
+    "Si",
+    "P",
+    "S",
+    "Cl",
+    "Ar",
+    # 4
+    "K",
+    "Ca",
+    "Sc",
+    "Ti",
+    "V",
+    "Cr",
+    "Mn",
+    "Fe",
+    "Co",
+    "Ni",
+    "Cu",
+    "Zn",
+    "Ga",
+    "Ge",
+    "As",
+    "Se",
+    "Br",
+    "Kr",
+    # 5
+    "Rb",
+    "Sr",
+    "Y",
+    "Zr",
+    "Nb",
+    "Mo",
+    "Tc",
+    "Ru",
+    "Rh",
+    "Pd",
+    "Ag",
+    "Cd",
+    "In",
+    "Sn",
+    "Sb",
+    "Te",
+    "I",
+    "Xe",
+    # 6
+    "Cs",
+    "Ba",
+    "La",
+    "Ce",
+    "Pr",
+    "Nd",
+    "Pm",
+    "Sm",
+    "Eu",
+    "Gd",
+    "Tb",
+    "Dy",
+    "Ho",
+    "Er",
+    "Tm",
+    "Yb",
+    "Lu",
+    "Hf",
+    "Ta",
+    "W",
+    "Re",
+    "Os",
+    "Ir",
+    "Pt",
+    "Au",
+    "Hg",
+    "Tl",
+    "Pb",
+    "Bi",
+    "Po",
+    "At",
+    "Rn",
+    # 7
+    "Fr",
+    "Ra",
+    "Ac",
+    "Th",
+    "Pa",
+    "U",
+    "Np",
+    "Pu",
+    "Am",
+    "Cm",
+    "Bk",
+    "Cf",
+    "Es",
+    "Fm",
+    "Md",
+    "No",
+    "Lr",
+    "Rf",
+    "Db",
+    "Sg",
+    "Bh",
+    "Hs",
+    "Mt",
+    "Ds",
+    "Rg",
+    "Cn",
+    "Nh",
+    "Fl",
+    "Mc",
+    "Lv",
+    "Ts",
+    "Og",
+]
+
+atomic_numbers = {}
+for Z, symbol in enumerate(chemical_symbols):
+    atomic_numbers[symbol] = Z
+
+
+@logger.catch
+def eles2masses(eles: List[str]) -> np.ndarray:
+    """将元素列表转换为质量列表
 
-class MSD:
-    # 用于实际计算均方位移的类，摘自pymatgen开源项目
-    def __init__(
-        self,
-        structures,
-        select: Union[str, List[int]] = "all",
-        msd_type="xyz",
-    ):
-        self.structures = structures
-        self.msd_type = msd_type
-
-        self.n_frames = len(structures)
-        self.lattice = structures[0].lattice
-
-        self._parse_msd_type()
-
-        import numpy as np
-
-        if select == "all":
-            self.n_particles = len(structures[0])
-            self._position_array = np.zeros(
-                (self.n_frames, self.n_particles, self.dim_fac)
-            )
-            for i, s in enumerate(self.structures):
-                self._position_array[i, :, :] = s.frac_coords[:, self._dim]
-        else:
-            if isinstance(select, str):  # ':', '-3:', 'H' or even 'H1'
-                if ":" in select:
-                    exec(
-                        f"self.n_particles = self.structures[0].frac_coords[{select}, :][:, self._dim].shape[0]"
-                    )
-                    self._position_array = np.zeros(
-                        (self.n_frames, self.n_particles, self.dim_fac)
-                    )
-                    for i, s in enumerate(self.structures):
-                        exec(
-                            f"self._position_array[i, :, :] = s.frac_coords[{select}, :][:, self._dim]"
-                        )
-                else:
-                    indices = [
-                        j
-                        for j, s in enumerate(self.structures[0])
-                        if select == s.species_string
-                    ]
-                    assert (
-                        indices != []
-                    ), f"{select} did not match any element symbol, {self.structures[0].species}"
-                    self.n_particles = (
-                        self.structures[0]
-                        .frac_coords[indices, :][:, self._dim]
-                        .shape[0]
-                    )
-                    self._position_array = np.zeros(
-                        (self.n_frames, self.n_particles, self.dim_fac)
-                    )
-                    for i, s in enumerate(self.structures):
-                        self._position_array[i, :, :] = s.frac_coords[indices, :][
-                            :, self._dim
-                        ]
-            else:
-                if isinstance(select, int):  # 1
-                    indices = [select]
-                elif isinstance(select, list) or isinstance(
-                    select, np.ndarray
-                ):  # [1,2,3] or ['H','O']
-                    # if all elements are int, then select by index
-                    if all(isinstance(i, int) for i in select):
-                        indices = select
-                    # if all elements are str, then select by element
-                    elif all(isinstance(i, str) for i in select):
-                        indices = []
-                        for sel in select:
-                            indices += [
-                                j
-                                for j, s in enumerate(self.structures[0])
-                                if sel == s.species_string
-                            ]
-                else:
-                    raise ValueError(
-                        f"select = {select} should be string, int, list or np.ndarray"
-                    )
-                # get shape of returned array
-                self.n_particles = (
-                    self.structures[0].frac_coords[indices, :][:, self._dim].shape[0]
-                )
-                self._position_array = np.zeros(
-                    (self.n_frames, self.n_particles, self.dim_fac)
-                )
-                for i, s in enumerate(self.structures):
-                    self._position_array[i, :, :] = s.frac_coords[indices, :][
-                        :, self._dim
-                    ]
-
-    def _parse_msd_type(self):
-        r"""Sets up the desired dimensionality of the MSD."""
-        keys = {
-            "x": [0],
-            "y": [1],
-            "z": [2],
-            "xy": [0, 1],
-            "xz": [0, 2],
-            "yz": [1, 2],
-            "xyz": [0, 1, 2],
-        }
-
-        self.msd_type = self.msd_type.lower()
-
-        try:
-            self._dim = keys[self.msd_type]
-        except KeyError:
-            raise ValueError(
-                "invalid msd_type: {} specified, please specify one of xyz, "
-                "xy, xz, yz, x, y, z".format(self.msd_type)
-            )
-
-        self.dim_fac = len(self._dim)
-
-    def run(self):
-        print("Calculating MSD...")
-        import numpy as np
-
-        result = np.zeros((self.n_frames, self.n_particles))
-
-        rd = np.zeros((self.n_frames, self.n_particles, self.dim_fac))
-        for i in range(1, self.n_frames):
-            disp = self._position_array[i, :, :] - self._position_array[i - 1, :, :]
-            # mic by periodic boundary condition
-            disp[np.abs(disp) > 0.5] = disp[np.abs(disp) > 0.5] - np.sign(
-                disp[np.abs(disp) > 0.5]
-            )
-            disp = np.dot(disp, self.lattice.matrix)
-            rd[i, :, :] = disp
-        rd = np.cumsum(rd, axis=0)
-        for n in range(1, self.n_frames):
-            disp = rd[n:, :, :] - rd[:-n, :, :]  # [n:-n] window
-            sqdist = np.square(disp).sum(axis=-1)
-            result[n, :] = sqdist.mean(axis=0)
-
-        return result.mean(axis=1)
-
+    Parameters
+    ----------
+    eles : List[str]
+        元素列表
 
-class RDF:
-    # 用于快速计算径向分布函数的类
-    # Copyright (c) Materials Virtual Lab.
-    # Distributed under the terms of the BSD License.
-    def __init__(
-        self,
-        structures,
-        rmin: float = 0.0,
-        rmax: float = 10.0,
-        ngrid: float = 101,
-        sigma: float = 0.0,
-    ):
-        """This method calculates rdf on `np.linspace(rmin, rmax, ngrid)` points
+    Returns
+    -------
+    List[float]
+        质量列表
 
-        Parameters
-        ----------
-        structures (list of pymatgen Structures): structures to compute RDF
-        rmin (float): minimal radius
-        rmax (float): maximal radius
-        ngrid (int): number of grid points, defaults to 101
-        sigma (float): smooth parameter
-        """
-        from pymatgen.core import Structure
+    Examples
+    --------
+    >>> from dspawpy.io.utils import eles2masses
+    >>> eles = ["H", "O"]
+    >>> masses = eles2masses(eles)
+    >>> masses
+    [1.008, 15.999]
+    """
+    masses = []
+    for e in eles:
+        masses.append(atomic_masses_iupac2016[atomic_numbers[e]])
+    return np.array(masses).tolist()
 
-        if isinstance(structures, Structure):
-            structures = [structures]
-        self.structures = structures
-        # Number of atoms in all structures should be the same
-        assert (
-            len({len(i) for i in self.structures}) == 1
-        ), "Different configurations have different numbers of atoms!"
-        elements = [[i.specie for i in j.sites] for j in self.structures]
-        unique_elements_on_sites = [len(set(i)) == 1 for i in list(zip(*elements))]
-
-        # For the same site index, all structures should have the same element there
-        if not all(unique_elements_on_sites):
-            raise RuntimeError("Elements are not the same at least for one site")
-
-        self.rmin = rmin
-        self.rmax = rmax
-        self.ngrid = ngrid
-
-        self.dr = (self.rmax - self.rmin) / (self.ngrid - 1)  # end points are on grid
-        import numpy as np
-
-        self.r = np.linspace(self.rmin, self.rmax, self.ngrid)  # type: ignore
-        self.shell_volumes = 4.0 * np.pi * self.r**2 * self.dr
-        self.shell_volumes[self.shell_volumes < 1e-8] = 1e8  # avoid divide by zero
 
-        self.n_structures = len(self.structures)
-        self.sigma = np.ceil(sigma / self.dr)
+@logger.catch
+def get_ma(elements, positions, Natom):
+    """Get the moments of inertia along the principal axes.
+
+    The three principal moments of inertia are computed from the
+    eigenvalues of the symmetric inertial tensor. Periodic boundary
+    conditions are ignored. Units of the moments of inertia are
+    amu*angstrom**2.
+    """
+    masses = eles2masses(elements)
+    com = np.dot(masses, positions) / np.sum(masses)
+    positions -= com  # translate center of mass to origin
+    masses = eles2masses(elements)
+
+    # Initialize elements of the inertial tensor
+    I11 = I22 = I33 = I12 = I13 = I23 = 0.0
+    for i in range(Natom):
+        x, y, z = positions[i]
+        m = masses[i]
+
+        I11 += m * (y**2 + z**2)
+        I22 += m * (x**2 + z**2)
+        I33 += m * (x**2 + y**2)
+        I12 += -m * x * y
+        I13 += -m * x * z
+        I23 += -m * y * z
 
-    def _dist_to_counts(self, d):
-        """Convert a distance array for counts in the bin
+    inertia = np.array([[I11, I12, I13], [I12, I22, I23], [I13, I23, I33]])
 
-        Parameters
-        ----------
-            d: (1D np.array)
+    evals, evecs = np.linalg.eigh(inertia)
+    return evals
 
-        Returns:
-            1D array of counts in the bins centered on self.r
-        """
-        import numpy as np
 
-        counts = np.zeros((self.ngrid,))
-        indices = np.array(
-            np.floor((d - self.rmin + 0.5 * self.dr) / self.dr), dtype=int
-        )  # 将找到配对的距离转换为格点序号 (向下取整)
-        unique, val_counts = np.unique(indices, return_counts=True)
-        counts[unique] = val_counts
-        return counts
+class IdealGasThermo:
+    """import from ase.thermochemistry.IdealGasThermo
 
-    def get_rdf(
-        self,
-        ref_species: Union[str, List[str]],
-        species: Union[str, List[str]],
-        is_average=True,
-    ):
-        """Wrapper to get the rdf for a given species pair
-
-        Parameters
-        ----------
-        ref_species (list of species or just single specie str):
-            The reference species. The rdfs are calculated with these species at the center
-        species (list of species or just single specie str):
-            the species that we are interested in. The rdfs are calculated on these species.
-        is_average (bool):
-            whether to take the average over all structures
-
-        Returns
-        -------
-        (x, rdf)
-            x is the radial points, and rdf is the rdf value.
-        """
-        print("Calculating RDF...")
-        if isinstance(ref_species, str):
-            ref_species = [ref_species]
-
-        if isinstance(species, str):
-            species = [species]
-        ref_species_index = []
-        species_index = []
-        for i in range(len(self.structures[0].species)):
-            ele = str(self.structures[0].species[i])
-            if ele in ref_species:
-                ref_species_index.append(i)
-            if (
-                ele in species
-            ):  # @syyl use if instead of elif in case of `species = ref_species`
-                species_index.append(i)
-        all_rdfs = [
-            self.get_one_rdf(ref_species_index, species_index, i)[1]
-            for i in range(self.n_structures)
-        ]
-        if is_average:
-            import numpy as np
+    Parameters
+    ----------
+    vib_energies : list
+        List of vibrational energies in eV.
+    geometry : str
+        One of 'linear', 'nonlinear', 'monatomic'
+    potentialenergy : float
+        Potential energy in eV.
+    elements : list
+        such as ['H', 'O'].
+    symmetrynumber : int
+        Symmetry number.
+    spin : int
+        Spin multiplicity.
+    natoms : int
+        Number of atoms.
 
-            all_rdfs = np.mean(all_rdfs, axis=0)
-        return self.r, all_rdfs
+    Examples
+    --------
+    >>> from dspawpy.io.utils import IdealGasThermo
+    >>> thermo = IdealGasThermo(vib_energies=[0.1, 0.2, 0.3, 0.4, 0.5, 0.6],
+    ...                         geometry='linear', potentialenergy=0.,  # eV
+    ...                         elements=['H', 'O'], positions=[[0, 0, 0], [0, 0, 1]],  # angstrom
+    ...                         symmetrynumber=None, spin=None, natoms=None)
+    >>> thermo.get_enthalpy(298.15)  # K
+    Enthalpy components at T = 298.15 K:
+    ===============================
+    E_pot                  0.000 eV
+    E_ZPE                  0.300 eV
+    Cv_trans (0->T)        0.039 eV
+    Cv_rot (0->T)          0.026 eV
+    Cv_vib (0->T)          0.000 eV
+    (C_v -> C_p)           0.026 eV
+    -------------------------------
+    H                      0.390 eV
+    ===============================
+    0.389924026967057
+    """
 
-    def get_one_rdf(
+    @logger.catch
+    def __init__(
         self,
-        ref_species_index: Union[str, List[str]],
-        species_index: Union[str, List[str]],
-        index=0,
+        vib_energies,
+        geometry,
+        potentialenergy=0.0,
+        elements=None,
+        positions=None,
+        symmetrynumber=None,
+        spin=None,
+        natoms=None,
     ):
-        """Get the RDF for one structure, indicated by the index of the structure
-        in all structures"""
-        lattice = self.structures[index].lattice
-        distances = []
-        refsp_frac_coord = self.structures[index].frac_coords[ref_species_index]
-        sp_frac_coord = self.structures[index].frac_coords[species_index]
-        d = lattice.get_all_distances(refsp_frac_coord, sp_frac_coord)
-        indices = (
-            (d >= self.rmin - self.dr / 2.0)
-            & (d <= self.rmax + self.dr / 2.0)
-            & (d > 1e-8)
-        )
-        import numpy as np
-
-        distances = d[indices]
-        counts = self._dist_to_counts(
-            np.array(distances)
-        )  # 统计该距离内目标元素的原子数，列表
-
-        npairs = len(distances)
-        rdf_temp = counts / npairs / self.shell_volumes / self.structures[index].volume
-
-        if self.sigma > 1e-8:
-            from scipy.ndimage import gaussian_filter1d
-
-            rdf_temp = gaussian_filter1d(rdf_temp, self.sigma)
-        return self.r, rdf_temp, npairs
-
-    def get_coordination_number(self, ref_species, species, is_average=True):
-        """returns running coordination number
-
-        Parameters
-        ----------
-        ref_species (list of species or just single specie str):
-            the reference species. The rdfs are calculated with these species at the center
-        species (list of species or just single specie str):
-            the species that we are interested in. The rdfs are calculated on these species.
-        is_average (bool): whether to take structural average
-
-        Returns
-        --------
-        numpy array
-        """
-        print("Calculating coordination number...")
-        # Note: The average density from all input structures is used here.
-        all_rdf = self.get_rdf(ref_species, species, is_average=False)[1]
-        if isinstance(species, str):
-            species = [species]
-        density = [sum(i[j] for j in species) for i in self.density]
-        import numpy as np
-
-        cn = [
-            np.cumsum(rdf * density[i] * 4.0 * np.pi * self.r**2 * self.dr)
-            for i, rdf in enumerate(all_rdf)
-        ]
-        if is_average:
-            cn = np.mean(cn, axis=0)
-        return self.r, cn
-
-
-class RMSD:
-    # 用于计算均方根偏差（Root Mean Square Deviation）的类，摘自pymatgen开源项目
-    def __init__(self, structures):
-        self.structures = structures
-
-        self.n_frames = len(self.structures)
-        self.n_particles = len(self.structures[0])
-        self.lattice = self.structures[0].lattice
-
-        import numpy as np
-
-        self._position_array = np.zeros((self.n_frames, self.n_particles, 3))
-
-        for i, s in enumerate(self.structures):
-            self._position_array[i, :, :] = s.frac_coords
-
-    def run(self, base_index=0):
-        print("Calculating RMSD...")
-        import numpy as np
-
-        result = np.zeros(self.n_frames)
-        rd = np.zeros((self.n_frames, self.n_particles, 3))
-        for i in range(1, self.n_frames):
-            disp = self._position_array[i, :, :] - self._position_array[i - 1, :, :]
-            # mic by periodic boundary condition
-            disp[np.abs(disp) > 0.5] = disp[np.abs(disp) > 0.5] - np.sign(
-                disp[np.abs(disp) > 0.5]
+        self.potentialenergy = potentialenergy
+        self.geometry = geometry
+        self.elements = elements
+        if isinstance(positions, list):
+            self.positions = np.array(positions, dtype=float)
+        elif isinstance(positions, np.ndarray):
+            self.positions = positions
+        else:
+            raise TypeError("positions must be list or np.ndarray")
+        if isinstance(vib_energies, list):
+            vib_energies = np.array(vib_energies)
+        elif isinstance(vib_energies, np.ndarray):
+            pass
+        else:
+            raise TypeError("vib_energies must be list or np.ndarray")
+        self.sigma = symmetrynumber
+        self.spin = spin
+        if natoms is None:
+            if elements:
+                natoms = len(elements)
+        # Cut the vibrations to those needed from the geometry.
+        if natoms:
+            if geometry == "nonlinear":
+                self.vib_energies = vib_energies[-(3 * natoms - 6) :]
+            elif geometry == "linear":
+                self.vib_energies = vib_energies[-(3 * natoms - 5) :]
+            elif geometry == "monatomic":
+                self.vib_energies = []
+        else:
+            self.vib_energies = vib_energies
+        # Make sure no imaginary frequencies remain.
+        if sum(np.iscomplex(self.vib_energies)):
+            raise ValueError("Imaginary frequencies are present.")
+        else:
+            self.vib_energies = np.real(self.vib_energies)  # clear +0.j
+        self.referencepressure = 1.0e5  # Pa
+        self.natoms = natoms
+
+    @logger.catch
+    def get_ZPE_correction(self):
+        """Returns the zero-point vibrational energy correction in eV."""
+        zpe = 0.0
+        for energy in self.vib_energies:
+            zpe += 0.5 * energy
+        return zpe
+
+    @logger.catch
+    def _vibrational_energy_contribution(self, temperature):
+        """Calculates the change in internal energy due to vibrations from
+        0K to the specified temperature for a set of vibrations given in
+        eV and a temperature given in Kelvin. Returns the energy change
+        in eV."""
+        kT = k * temperature
+        dU = 0.0
+        for energy in self.vib_energies:
+            dU += energy / (np.exp(energy / kT) - 1.0)
+        return dU
+
+    @logger.catch
+    def _vibrational_entropy_contribution(self, temperature):
+        """Calculates the entropy due to vibrations for a set of vibrations
+        given in eV and a temperature given in Kelvin.  Returns the entropy
+        in eV/K."""
+        kT = k * temperature
+        S_v = 0.0
+        for energy in self.vib_energies:
+            x = energy / kT
+            S_v += x / (np.exp(x) - 1.0) - np.log(1.0 - np.exp(-x))
+        S_v *= k
+        return S_v
+
+    @logger.catch
+    def get_enthalpy(self, temperature):
+        """Returns the enthalpy, in eV, in the ideal gas approximation
+        at a specified temperature (K)."""
+
+        fmt = "%-15s%13.3f eV"
+        print("Enthalpy components at T = %.2f K:" % temperature)
+        print("=" * 31)
+
+        H = 0.0
+
+        print(fmt % ("E_pot", self.potentialenergy))
+        H += self.potentialenergy
+
+        zpe = self.get_ZPE_correction()
+        print(fmt % ("E_ZPE", zpe))
+        H += zpe
+
+        Cv_t = 3.0 / 2.0 * k  # translational heat capacity (3-d gas)
+        print(fmt % ("Cv_trans (0->T)", Cv_t * temperature))
+        H += Cv_t * temperature
+
+        if self.geometry == "nonlinear":  # rotational heat capacity
+            Cv_r = 3.0 / 2.0 * k
+        elif self.geometry == "linear":
+            Cv_r = k
+        elif self.geometry == "monatomic":
+            Cv_r = 0.0
+        print(fmt % ("Cv_rot (0->T)", Cv_r * temperature))
+        H += Cv_r * temperature
+
+        dH_v = self._vibrational_energy_contribution(temperature)
+        print(fmt % ("Cv_vib (0->T)", dH_v))
+        H += dH_v
+
+        Cp_corr = k * temperature
+        print(fmt % ("(C_v -> C_p)", Cp_corr))
+        H += Cp_corr
+
+        print("-" * 31)
+        print(fmt % ("H", H))
+        print("=" * 31)
+        return H
+
+    @logger.catch
+    def get_entropy(self, temperature, pressure):
+        """Returns the entropy, in eV/K, in the ideal gas approximation
+        at a specified temperature (K) and pressure (Pa)."""
+
+        if self.elements is None or self.sigma is None or self.spin is None:
+            raise RuntimeError(
+                "elements, symmetrynumber, and spin must be "
+                "specified for entropy and free energy "
+                "calculations."
             )
-            disp = np.dot(disp, self.lattice.matrix)
-            rd[i, :, :] = disp
-        rd = np.cumsum(rd, axis=0)
-
-        for i in range(self.n_frames):
-            sqdist = np.square(rd[i] - rd[base_index]).sum(axis=-1)
-            result[i] = sqdist.mean()
-
-        return np.sqrt(result)
-
-
-def get_lagtime_msd(
-    datafile: Union[str, List[str]],
-    select: Union[str, List[int]] = "all",
-    msd_type: str = "xyz",
-    timestep: float = None,
+        S = 0.0
+        # Translational entropy (term inside the log is in SI units).
+        mass = sum(eles2masses(self.elements)) * amu  # kg/molecule
+        S_t = (2 * np.pi * mass * kB * temperature / h**2) ** (3.0 / 2)
+        S_t *= kB * temperature / self.referencepressure
+        S_t = k * (np.log(S_t) + 5.0 / 2.0)
+        S += S_t
+
+        # Rotational entropy (term inside the log is in SI units).
+        if self.geometry == "monatomic":
+            S_r = 0.0
+        elif self.geometry == "nonlinear":
+            inertias = (
+                get_ma(self.elements, self.positions, self.natoms)
+                * amu
+                / (10.0**10) ** 2
+            )  # kg m^2
+            S_r = np.sqrt(np.pi * np.product(inertias)) / self.sigma
+            S_r *= (8.0 * np.pi**2 * kB * temperature / h**2) ** (3.0 / 2.0)
+            S_r = k * (np.log(S_r) + 3.0 / 2.0)
+        elif self.geometry == "linear":
+            inertias = (
+                get_ma(self.elements, self.positions, self.natoms)
+                * amu
+                / (10.0**10) ** 2
+            )  # kg m^2
+            inertia = max(inertias)  # should be two identical and one zero
+            S_r = 8 * np.pi**2 * inertia * kB * temperature / self.sigma / h**2
+            S_r = k * (np.log(S_r) + 1.0)
+        S += S_r
+        # Electronic entropy.
+        S_e = k * np.log(2 * self.spin + 1)
+        S += S_e
+        # Vibrational entropy.
+        S_v = self._vibrational_entropy_contribution(temperature)
+        S += S_v
+        # Pressure correction to translational entropy.
+        S_p = -k * np.log(pressure / self.referencepressure)
+        S += S_p
+        return S
+
+    @logger.catch
+    def get_gibbs_energy(self, temperature, pressure):
+        """Returns the Gibbs free energy, in eV, in the ideal gas
+        approximation at a specified temperature (K) and pressure (Pa)."""
+
+        H = self.get_enthalpy(temperature)
+        print("")
+        S = self.get_entropy(temperature, pressure)
+        G = H - temperature * S
+
+        print("")
+        print(
+            "Free energy components at T = %.2f K and P = %.1f Pa:"
+            % (temperature, pressure)
+        )
+        print("=" * 23)
+        fmt = "%5s%15.3f eV"
+        print(fmt % ("H", H))
+        print(fmt % ("-T*S", -temperature * S))
+        print("-" * 23)
+        print(fmt % ("G", G))
+        print("=" * 23)
+        return G
+
+
+@logger.catch
+def getTSgas(
+    fretxt="frequency.txt",
+    datafile=".",
+    potentialenergy=0,  # eV
+    elements=None,
+    geometry="linear",
+    positions=None,  # Angstrom
+    symmetrynumber=1,
+    spin=1,
+    temperature=298.15,
+    pressure: float = 101325,
 ):
-    r"""计算不同时间步长下的均方位移
+    """理想气体近似下，计算熵的能量贡献
+
 
     Parameters
     ----------
-    datafile : str or list of str
-        - aimd.h5/aimd.json文件路径或包含这些文件的文件夹路径（优先寻找aimd.h5）
-        - 写成列表将依次读取数据并合并到一起
-        - 例如['aimd1.h5', 'aimd2.h5', '/data/home/my_aimd_task']
-    select : str or list of int
-        选择原子序号或元素，原子序号从0开始；默认为'all'，计算所有原子
-    msd_type : str
-        计算MSD的类型，可选xyz,xy,xz,yz,x,y,z，默认为'xyz'，即计算所有分量
-    timestep : float
-        相邻结构的时间间隔，单位为fs，默认None，将从datafile中读取，失败则设为1.0fs；
-        若不为None，则将使用该值计算时间序列
+    fretxt : str
+        记录频率信息的文件所在路径, 默认当前路径下的'frequency.txt'
+    datafile : str
+        计算结果json或h5文件或包含它们的文件夹路径, 默认当前路径；
+        如果设置为None，则需要传入elements和positions参数
+    potentialenergy : float
+        势能，单位eV
+    elements : list
+        元素列表，如果
+    geometry : str
+        分子几何，monatomic, linear, nonlinear
+    positions : list
+        原子坐标，单位Angstrom
+    symmetrynumber : int
+        对称数
+    spin : int
+        自旋数
+    temperature : float
+        温度，单位K
+    pressure : float
+        压强，单位Pa
 
     Returns
     -------
-    lagtime : np.ndarray
-        时间序列
-    result : np.ndarray
-        均方位移序列
+    TSgas : float
+        理想气体近似下，计算熵的能量贡献，单位eV
 
     Examples
     --------
-    >>> from dspawpy.analysis.aimdtools import get_lagtime_msd
-    >>> lagtime, msd = get_lagtime_msd(datafile='dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5') # doctest: +ELLIPSIS
-    Reading ...dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5...
-    Calculating MSD...
-    >>> lagtime
-    array([0.000e+00, 1.000e+00, 2.000e+00, ..., 1.997e+03, 1.998e+03,
-           1.999e+03])
-    >>> msd
-    array([0.00000000e+00, 8.80447550e-02, 1.83768134e-01, ...,
-           9.66185452e+02, 9.66812755e+02, 9.67357702e+02])
-    >>> lagtime, msd = get_lagtime_msd(datafile='dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5', select='H') # doctest: +ELLIPSIS
-    Reading ...dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5...
-    Calculating MSD...
-    >>> lagtime, msd = get_lagtime_msd(datafile='dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5', select=[0,1]) # doctest: +ELLIPSIS
-    Reading ...dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5...
-    Calculating MSD...
-    >>> lagtime, msd = get_lagtime_msd(datafile='dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5', select=['H','O']) # doctest: +ELLIPSIS
-    Reading ...dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5...
-    Calculating MSD...
-    >>> lagtime, msd = get_lagtime_msd(datafile='dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5', select=0) # doctest: +ELLIPSIS
-    Reading ...dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5...
-    Calculating MSD...
+    >>> from dspawpy.io.utils import getTSgas
+    >>> TSgas=getTSgas(fretxt='dspawpy_proj/dspawpy_tests/inputs/2.13/frequency.txt', datafile='dspawpy_proj/dspawpy_tests/inputs/2.13/frequency.h5', potentialenergy=-0.0,  geometry='linear', symmetrynumber=1, spin=1, temperature=298.15, pressure=101325.0)
+    --> T*S (eV): 0.8515317035550232
     """
-    from dspawpy.io.structure import read
-
-    strs = read(datafile, task="aimd")
-    if timestep is None:
-        if isinstance(datafile, str) or len(datafile) == 1:
-            ts = _get_time_step(datafile)
-        else:
-            warnings.warn(
-                "For multiple datafiles, you must manually specify the timestep. It will default to 1.0fs."
-            )
-            ts = 1.0
-    else:
-        ts = timestep
+    import os
 
-    msd = MSD(strs, select, msd_type)
-    result = msd.run()
+    abstxt = os.path.abspath(fretxt)
+    ve = []
+    with open(abstxt) as ft:
+        lines = ft.readlines()
+        for i in range(2, len(lines)):
+            if lines[i].strip()[1] == "f/i":
+                ve.append(complex(lines[i].split()[-1]) / 1000)
+            else:
+                ve.append(float(lines[i].split()[-1]) / 1000)
+    if datafile is not None:
+        absfile = get_absfile(datafile, task="frequency")
+        if absfile.endswith(".h5"):
+            from dspawpy.io.read import get_ele_from_h5
 
-    nframes = msd.n_frames
-    import numpy as np
+            eles = get_ele_from_h5(absfile)
+            import h5py
 
-    lagtime = np.arange(nframes) * ts  # make the lag-time axis
+            data = h5py.File(absfile)
+            poses = np.array(data.get("/AtomInfo/Position")).reshape(-1, 3)
 
-    return lagtime, result
+        elif absfile.endswith(".json"):
+            import json
 
+            with open(absfile) as f:
+                data = json.load(f)
+            atoms = data["AtomInfo"]["Atoms"]
+            eles = []
+            poses = []
+            for i in range(len(atoms)):
+                eles.append(atoms[i]["Element"])
+                poses.append(atoms[i]["Position"])
+        else:
+            raise TypeError("Only support h5/json file")
+    else:
+        eles = elements
+        poses = positions
 
-def get_lagtime_rmsd(datafile: Union[str, List[str]], timestep: float = None):
-    r"""
+    # 计算熵的能量贡献
+    thermo = IdealGasThermo(
+        vib_energies=ve,  # eV
+        potentialenergy=potentialenergy,  # eV
+        elements=eles,
+        geometry=geometry,
+        positions=poses,  # Angstrom
+        symmetrynumber=symmetrynumber,
+        spin=spin,
+    )
+    S = thermo.get_entropy(temperature, pressure)
+    dE = S * temperature
+    print(f"--> T*S (eV): {dE}")
+
+    return S * temperature
+
+
+@logger.catch
+def d_band(spin, dos_data):  # 定义函数，括号里给出函数的两个变量
+    """计算d带中心
 
     Parameters
     ----------
-    datafile : str or list of str
-        - aimd.h5/aimd.json文件路径或包含这些文件的文件夹路径（优先寻找aimd.h5）
-        - 写成列表将依次读取数据并合并到一起
-        - 例如['aimd1.h5', 'aimd2.h5', '/data/home/my_aimd_task']
-    timestep : float
-        相邻结构的时间间隔，单位为fs，默认None，将从datafile中读取，失败则设为1.0fs；
-        若不为None，则将使用该值计算时间序列
+    spin : Spin.up或Spin.down
+        自旋类型，
+    dos_data : pymatgen.electronic_structure.dos.CompleteDos
+        dos数据
 
     Returns
     -------
-    lagtime : numpy.ndarray
-        时间序列
-    rmsd : numpy.ndarray
-        均方根偏差序列
+    db1 : float
+        d带中心数值
 
     Examples
     --------
-    >>> from dspawpy.analysis.aimdtools import get_lagtime_rmsd
-    >>> lagtime, rmsd = get_lagtime_rmsd(datafile='dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5', timestep=0.1) # doctest: +ELLIPSIS
-    Reading ...dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5...
-    Calculating RMSD...
-    >>> lagtime
-    array([0.000e+00, 1.000e-01, 2.000e-01, ..., 1.997e+02, 1.998e+02,
-           1.999e+02])
-    >>> rmsd
-    array([ 0.        ,  0.04849931,  0.09181907, ..., 31.09991413,
-           31.10077061, 31.10237454])
+    >>> from dspawpy.io.utils import d_band
+    >>> from dspawpy.io.read import get_dos_data
+    >>> dos_data = get_dos_data("dspawpy_proj/dspawpy_tests/inputs/supplement/dos.h5")  # 从dos.h5中读取数据
+    >>> for spin in dos_data.densities:
+    ...     print('spin=', spin)
+    ...     c = d_band(spin, dos_data)
+    ...     print(c) # doctest: +ELLIPSIS
+    spin= 1
+    -3.666508...
     """
-    from dspawpy.io.structure import read
+    from pymatgen.electronic_structure.core import OrbitalType
 
-    strs = read(datafile, task="aimd")
-    if timestep is None:
-        if isinstance(datafile, str) or len(datafile) == 1:
-            ts = _get_time_step(datafile)
-        else:
-            warnings.warn(
-                "For multiple datafiles, you must manually specify the timestep. It will default to 1.0fs."
-            )
-            ts = 1.0
-    else:
-        ts = timestep
+    dos_d = dos_data.get_spd_dos()[OrbitalType.d]
+    # dos_d = dos_data.get_spd_dos()[d]
+    Efermi = dos_data.efermi
+    epsilon = dos_d.energies - Efermi  # shift d-band center
 
-    rmsd = RMSD(structures=strs)
-    result = rmsd.run()
+    N1 = dos_d.densities[spin]
+    M1 = epsilon * N1
+    from scipy import integrate
 
-    # Plot
-    nframes = rmsd.n_frames
-    import numpy as np
+    SummaM1 = integrate.simps(M1, epsilon)
+    SummaN1 = integrate.simps(N1, epsilon)
 
-    lagtime = np.arange(nframes) * ts  # make the lag-time axis
+    return SummaM1 / SummaN1
 
-    return lagtime, result
 
+@logger.catch
+def getZPE(fretxt: str = "frequency.txt"):
+    """从fretext中读取数据，计算ZPE
 
-def get_rs_rdfs(
-    datafile: Union[str, List[str]],
-    ele1: str,
-    ele2: str,
-    rmin: float = 0,
-    rmax: float = 10,
-    ngrid: float = 101,
-    sigma: float = 0,
-):
-    r"""计算rdf分布函数
+    将另外保存结果到 ZPE_TS.dat 中
 
     Parameters
     ----------
-    datafile : str or list of str
-        - aimd.h5/aimd.json文件路径或包含这些文件的文件夹路径（优先寻找aimd.h5）
-        - 写成列表将依次读取数据并合并到一起
-        - 例如['aimd1.h5', 'aimd2.h5', '/data/home/my_aimd_task']
-    ele1 : list
-        中心元素
-    ele2 : list
-        相邻元素
-    rmin : float
-        径向分布最小值，默认为0
-    rmax : float
-        径向分布最大值，默认为10
-    ngrid : int
-        径向分布网格数，默认为101
-    sigma : float
-        平滑参数
+    fretxt : str
+        记录频率信息的文件所在路径, 默认当前路径下的'frequency.txt'
 
     Returns
     -------
-    r : numpy.ndarray
-        径向分布网格点
-    rdf : numpy.ndarray
-        径向分布函数
+    ZPE: float
+        零点能
 
     Examples
     --------
-    >>> from dspawpy.analysis.aimdtools import get_rs_rdfs
-    >>> rs, rdfs = get_rs_rdfs(datafile='dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5',ele1='H',ele2='O') # doctest: +ELLIPSIS
-    Reading ...dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5...
-    Calculating RDF...
-    >>> rdfs
-    array([0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           6.90409153e-05, 7.47498606e-04, 2.40555636e-03, 2.57666881e-03,
-           2.53257125e-03, 2.37964722e-03, 1.80028135e-03, 1.20224160e-03,
-           7.57927477e-04, 3.41004760e-04, 2.85680407e-04, 1.72795412e-04,
-           1.49718401e-04, 1.44477999e-04, 2.23702566e-04, 2.11836218e-04,
-           1.34146448e-04, 1.78839343e-04, 9.16910363e-05, 1.45492991e-05,
-           3.70494493e-05, 3.72784113e-05, 2.82725837e-05, 3.19750004e-05,
-           8.46456322e-07, 4.72401470e-06, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00])
+    >>> from dspawpy.io.utils import getZPE
+    >>> ZPE=getZPE(fretxt='dspawpy_proj/dspawpy_tests/inputs/2.13/frequency.txt')
+    --> Zero-point energy,  ZPE (eV): 0.1424200165
     """
-    from dspawpy.io.structure import read
+    import os
 
-    strs = read(datafile, task="aimd")
-
-    # 计算rdf并绘制主要曲线
-    obj = RDF(structures=strs, rmin=rmin, rmax=rmax, ngrid=ngrid, sigma=sigma)
-
-    rs, rdfs = obj.get_rdf(ele1, ele2)
-    return rs, rdfs
-
-
-def plot_msd(
-    lagtime,
-    result,
-    xlim: List[float] = None,
-    ylim: List[float] = None,
-    figname: str = None,
-    show: bool = True,
-    ax=None,
-    **kwargs,
+    abstxt = os.path.abspath(fretxt)
+    data_get_ZPE = []
+    with open(abstxt, "r") as f:
+        for line in f.readlines():
+            data_line = line.strip().split()
+            if len(data_line) != 6:
+                continue
+            if data_line[1] == "f":
+                data_get_ZPE.append(float(data_line[5]))
+
+    data_get_ZPE = np.array(data_get_ZPE)
+
+    assert (
+        len(data_get_ZPE) > 0
+    ), "Only imaginary frequencies, please consider re-optimizing the structure"
+
+    ZPE = 0
+    for data in data_get_ZPE:
+        ZPE += data / 2000.0
+    print("--> Zero-point energy,  ZPE (eV):", ZPE)
+
+    return ZPE
+
+
+@logger.catch
+def getTSads(
+    fretxt: str = "frequency.txt",
+    T: float = 298.15,
 ):
-    r"""AIMD任务完成后，计算均方位移（MSD）
+    """从fretext中读取数据，计算ZPE和TS
+
+    将另外保存结果到 TSads.dat 中
 
     Parameters
     ----------
-    lagtime : np.ndarray
-        时间序列
-    result : np.ndarray
-        均方位移序列
-    xlim : list of float
-        x轴的范围，默认为None，自动设置
-    ylim : list of float
-        y轴的范围，默认为None，自动设置
-    figname : str
-        图片名称，默认为None，不保存图片
-    show : bool
-        是否显示图片，默认为True
-    ax: matplotlib axes object
-        用于将图片绘制到matplotlib的子图上
-    **kwargs : dict
-        其他参数，如线条宽度、颜色等，传递给plt.plot函数
+    fretxt : str
+        记录频率信息的文件所在路径, 默认当前路径下的'frequency.txt'
+    T : float
+        温度，单位K, 默认298.15
 
     Returns
     -------
-    MSD分析后的图片
+    TS: float
+        熵校正
 
     Examples
     --------
-    >>> from dspawpy.analysis.aimdtools import get_lagtime_msd, plot_msd
-
-    指定h5文件位置，用 get_lagtime_msd 函数获取数据，select 参数选择第n个原子（不是元素）
-
-    >>> lagtime, msd = get_lagtime_msd('dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5', select=[0]) # doctest: +ELLIPSIS
-    Reading ...dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5...
-    Calculating MSD...
-
-    用获取的数据画图并保存
-
-    >>> plot_msd(lagtime, msd, figname='dspawpy_proj/dspawpy_tests/inputs/out/MSD.png', show=False) # doctest: +ELLIPSIS
-    ==> ...dspawpy_proj/dspawpy_tests/inputs/out/MSD.png
-    ...
+    >>> from dspawpy.io.utils import getTSads
+    >>> TSads=getTSads(fretxt='dspawpy_proj/dspawpy_tests/inputs/2.13/frequency.txt', T=298.15)
+    --> T*S (eV): 4.7566997225177686e-06
     """
-    import matplotlib.pyplot as plt
+    import os
 
-    if ax:
-        ishow = False
-        ax.plot(lagtime, result, c="black", ls="-", **kwargs)
-    else:
-        ishow = True
-        fig, ax = plt.subplots()
-        ax.plot(lagtime, result, c="black", ls="-", **kwargs)
-        ax.set_xlabel("Time (fs)")
-        ax.set_ylabel(r"MSD ($Å^2$)")
-
-    if xlim:
-        ax.set_xlim(xlim)
-    if ylim:
-        ax.set_ylim(ylim)
-
-    plt.tight_layout()
-    if figname:
-        absfig = os.path.abspath(figname)
-        os.makedirs(os.path.dirname(absfig), exist_ok=True)
-        plt.savefig(absfig, dpi=300)
-        print(f"==> {absfig}")
-    if show and ishow:  # 画子图的话，不应每个子图都show
-        plt.show()  # show会自动清空图片
-
-    return ax
-
-
-def plot_rdf(
-    rs,
-    rdfs,
-    ele1: str,
-    ele2: str,
-    xlim: list = None,
-    ylim: list = None,
-    figname: str = None,
-    show: bool = True,
-    ax=None,
-    **kwargs,
-):
-    r"""AIMD计算后分析rdf并画图
+    abstxt = os.path.abspath(fretxt)
+
+    data_get_TS = []
+    with open(abstxt, "r") as f:
+        for line in f.readlines():
+            data_line = line.strip().split()
+            if len(data_line) != 6:
+                continue
+            if data_line[1] == "f":
+                data_get_TS.append(float(data_line[2]))
+
+    data_get_TS = np.array(data_get_TS)
+
+    assert (
+        len(data_get_TS) > 0
+    ), "Only imaginary frequencies, please consider re-optimizing the structure"
+
+    sum_S = 0
+    import math  # 因为要使用 e的多少次方，ln（）对数
+
+    for vi_THz in data_get_TS:
+        vi_Hz = vi_THz * 1e12
+        m1 = h * Na * vi_Hz
+        m2 = h * vi_Hz / (kB * T)
+        m3 = math.exp(m2) - 1
+        m4 = T * m3
+        m5 = 1 - math.exp(-m2)  # math.exp(3) 就是e的3次方
+        m6 = math.log(m5, math.e)  # m6= ln(m5)   math.e在python中=e ，以右边为底的对数
+        m7 = R * m6
+        m8 = m1 / m4 - m7  # S 单位J/(mol*K)
+        m9 = (T * m8 / 1000) / 96.49  # T*S,将单位化为KJ/mol, 96.49 kJ/mol = 1 eV 单位eV
+        sum_S += m9
+
+    print("--> T*S (eV):", sum_S)
+
+    return sum_S
+
+
+@logger.catch
+def get_absfile(datafile: str, task: str, only_h5: bool = False):  # -> absfile
+    """根据给定的datafile，返回所需数据文件的绝对路径
 
     Parameters
     ----------
-    rs : numpy.ndarray
-        径向分布网格点
-    rdfs : numpy.ndarray
-        径向分布函数
-    ele1 : list
-        中心元素
-    ele2 : list
-        相邻元素
-    xlim : list
-        x轴范围，默认为None，即自动设置
-    ylim : list
-        y轴范围，默认为None，即自动设置
-    figname : str
-        图片名称，默认为None，即不保存图片
-    show : bool
-        是否显示图片，默认为True
-    ax: matplotlib.axes.Axes
-        画图的坐标轴，默认为None，即新建坐标轴
-    **kwargs : dict
-        其他参数，如线条宽度、颜色等，传递给plt.plot函数
+    datafile: str
+        h5/json数据文件路径或其文件夹路径，可以是相对路径
+    task: str
+        计算任务类型，如 scf, optical 等
+    only_h5: bool
+        是否只寻找h5文件，默认False
+
+    Raises
+    ------
+    FileNotFoundError
+        - 指定的文件夹路径不包含相应h5/json数据文件
+        - 指定的文件路径不存在
 
     Returns
     -------
-    rdf分析后的图片
-
-    Examples
-    --------
-    >>> from dspawpy.analysis.aimdtools import get_rs_rdfs, plot_rdf
-
-    先获取rs和rdfs数据作为xy轴数据
+    absfile: str
+        所需数据文件的绝对路径
+    """
+    assert datafile is not None, "datafile is None"
+    import os
 
-    >>> rs, rdfs = get_rs_rdfs('dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5', 'H', 'O', rmax=6) # doctest: +ELLIPSIS
-    Reading ...dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5...
-    Calculating RDF...
+    absfile = os.path.abspath(datafile)
+    if only_h5:
+        if os.path.isdir(absfile):  # specified datafile is actually a directory
+            directory = absfile  # search datafile in the given directory
+            absh5 = os.path.join(directory, f"{task}.h5")
+            if os.path.exists(absh5):
+                absfile = absh5
+            else:
+                raise FileNotFoundError(f"No {absh5}/{absfile}")
+        else:
+            if not os.path.isfile(absfile):
+                raise FileNotFoundError(f"No {absfile}")
+            else:
+                assert absfile.endswith(
+                    ".h5"
+                ), f"Only support h5 file, but got {absfile}"
+    else:
+        if os.path.isdir(absfile):  # specified datafile is actually a directory
+            directory = absfile  # search datafile in the given directory
+            absh5 = os.path.join(directory, f"{task}.h5")
+            absjs = os.path.join(directory, f"{task}.json")
+            if os.path.exists(absh5):
+                absfile = absh5
+            elif os.path.exists(absjs):
+                absfile = absjs
+            else:
+                raise FileNotFoundError(f"No {absh5}/{absjs}")
+        else:
+            if not os.path.isfile(absfile):
+                raise FileNotFoundError(f"No {absfile}")
+            else:
+                assert absfile.endswith(".h5") or absfile.endswith(
+                    ".json"
+                ), f"Only support h5/json file, but got {absfile}"
+
+    return absfile
+
+
+# extract from ASE
+@logger.catch
+def string2symbols(s: str) -> List[str]:
+    """Convert string to list of chemical symbols."""
+    return list(Formula(s))
+
+
+@logger.catch
+def _symbols2numbers(symbols) -> List[int]:
+    if isinstance(symbols, str):
+        symbols = string2symbols(symbols)
+    numbers = []
+    for s in symbols:
+        if isinstance(s, str):
+            numbers.append(atomic_numbers[s])
+        else:
+            numbers.append(int(s))
+    return numbers
 
-    将xy轴数据传入plot_rdf函数绘图
 
-    >>> plot_rdf(rs, rdfs, 'H','O', figname='dspawpy_proj/dspawpy_tests/inputs/out/RDF.png', show=False) # doctest: +ELLIPSIS
-    ==> ...dspawpy_proj/dspawpy_tests/inputs/out/RDF.png
-    """
-
-    import matplotlib.pyplot as plt
+class Formula:
+    @logger.catch
+    def __init__(
+        self,
+        formula: str = "",
+        *,
+        strict: bool = False,
+        format: str = "",
+        _tree=None,
+        _count=None,
+    ):
+        """Chemical formula object.
 
-    if ax:
-        ishow = False
-        ax.plot(
-            rs,
-            rdfs,
-            label=r"$g_{\alpha\beta}(r)$" + f"[{ele1},{ele2}]",
-            **kwargs,
-        )
+        Parameters
+        ----------
+        formula: str
+            Text string representation of formula.  Examples: ``'6CO2'``,
+            ``'30Cu+2CO'``, ``'Pt(CO)6'``.
+        strict: bool
+            Only allow real chemical symbols.
+        format: str
+            Reorder according to *format*.  Must be one of hill, metal,
+            abc or reduce.
 
-    else:
-        ishow = True
-        fig, ax = plt.subplots()
-        ax.plot(
-            rs,
-            rdfs,
-            label=r"$g_{\alpha\beta}(r)$" + f"[{ele1},{ele2}]",
-            **kwargs,
-        )
+        Examples
+        --------
+        >>> from dspawpy.io.utils import Formula
+        >>> w = Formula('H2O')
 
-        ax.set_xlabel(r"$r$" + "(Å)")
-        ax.set_ylabel(r"$g(r)$")
+        Raises
+        ------
+        ValueError
+            on malformed formula
+        """
+        if format:
+            assert _tree is None and _count is None
+            if format not in {"hill", "metal", "abc", "reduce"}:
+                raise ValueError(f"Illegal format: {format}")
+            formula = Formula(formula).format(format)
+        self._formula = formula
+        self._tree = _tree or parse(formula)
+        self._count = _count or count_tree(self._tree)
+        if strict:
+            for symbol in self._count:
+                if symbol not in atomic_numbers:
+                    raise ValueError("Unknown chemical symbol: " + symbol)
+
+    @logger.catch
+    def __iter__(self, tree=None):
+        if tree is None:
+            tree = self._tree
+        if isinstance(tree, str):
+            yield tree
+        elif isinstance(tree, tuple):
+            tree, N = tree
+            for _ in range(N):
+                yield from self.__iter__(tree)
+        else:
+            for tree in tree:
+                yield from self.__iter__(tree)
 
-    ax.legend()
 
-    # 绘图细节
-    if xlim:
-        ax.set_xlim(xlim)
-    if ylim:
-        ax.set_ylim(ylim)
-
-    plt.tight_layout()
-    if figname:
-        absfig = os.path.abspath(figname)
-        os.makedirs(os.path.dirname(absfig), exist_ok=True)
-        plt.savefig(absfig, dpi=300)
-        print(f"==> {absfig}")
-    if show and ishow:  # 画子图的话，不应每个子图都show
-        plt.show()  # show会自动清空图片
-
-
-def plot_rmsd(
-    lagtime,
-    result,
-    xlim: list = None,
-    ylim: list = None,
-    figname: str = None,
-    show: bool = True,
-    ax=None,
-    **kwargs,
-):
-    r"""AIMD计算后分析rmsd并画图
+@logger.catch
+def parse(f: str):  # -> Tree
+    if not f:
+        return []
+    parts = f.split("+")
+    result = []
+    for part in parts:
+        n, f = strip_number(part)
+        result.append((parse2(f), n))
+    return result
+
+
+@logger.catch
+def strip_number(s: str):
+    import re
+
+    m = re.match("[0-9]*", s)
+    assert m is not None
+    return int(m.group() or 1), s[m.end() :]
+
+
+@logger.catch
+def parse2(f: str):
+    units = []
+    import re
+
+    while f:
+        if f[0] == "(":
+            level = 0
+            for i, c in enumerate(f[1:], 1):
+                if c == "(":
+                    level += 1
+                elif c == ")":
+                    if level == 0:
+                        break
+                    level -= 1
+            else:
+                raise ValueError
+            f2 = f[1:i]
+            n, f = strip_number(f[i + 1 :])
+            unit = (parse2(f2), n)
+        else:
+            m = re.match("([A-Z][a-z]?)([0-9]*)", f)
+            if m is None:
+                raise ValueError
+            symb = m.group(1)
+            number = m.group(2)
+            if number:
+                unit = (symb, int(number))
+            else:
+                unit = symb
+            f = f[m.end() :]
+        units.append(unit)
+    if len(units) == 1:
+        return unit
+    return units
+
+
+@logger.catch
+def count_tree(tree):
+    if isinstance(tree, str):
+        return {tree: 1}
+    if isinstance(tree, tuple):
+        tree, N = tree
+        return {symb: n * N for symb, n in count_tree(tree).items()}
+    dct = {}
+    for tree in tree:
+        for symb, n in count_tree(tree).items():
+            m = dct.get(symb, 0)
+            dct[symb] = m + n
+    return dct
+
+
+import functools  # noqa: E402
+from pathlib import PurePath  # noqa: E402
+
+
+class iofunction:
+    """Decorate func so it accepts either str or file.
+
+    (Won't work on functions that return a generator.)"""
+
+    @logger.catch
+    def __init__(self, mode):
+        self.mode = mode
+
+    @logger.catch
+    def __call__(self, func):
+        @functools.wraps(func)
+        def iofunc(file, *args, **kwargs):
+            openandclose = isinstance(file, (str, PurePath))
+            fd = None
+            try:
+                if openandclose:
+                    fd = open(str(file), self.mode)
+                else:
+                    fd = file
+                obj = func(fd, *args, **kwargs)
+                return obj
+            finally:
+                if openandclose and fd is not None:
+                    # fd may be None if open() failed
+                    fd.close()
+
+        return iofunc
+
+
+@logger.catch
+def reader(func):
+    return iofunction("r")(func)
+
+
+@logger.catch
+def label_to_symbol(label):
+    """Convert a valid espresso ATOMIC_SPECIES label to a
+    chemical symbol.
 
     Parameters
     ----------
-    lagtime:
-        时间序列
-    result:
-        均方根偏差序列
-    xlim : list
-        x轴范围
-    ylim : list
-        y轴范围
-    figname : str
-        图片保存路径
-    show : bool
-        是否显示图片
-    ax : matplotlib.axes._subplots.AxesSubplot
-        画子图的话，传入子图对象
-    **kwargs : dict
-        传入plt.plot的参数
+    label : str
+        chemical symbol X (1 or 2 characters, case-insensitive)
+        or chemical symbol plus a number or a letter, as in
+        "Xn" (e.g. Fe1) or "X_*" or "X-*" (e.g. C1, C_h;
+        max total length cannot exceed 3 characters).
 
     Returns
     -------
-    rmsd分析结构的图片
+    symbol : str
+        The best matching species from ase.utils.chemical_symbols
 
-    Examples
-    --------
-    >>> from dspawpy.analysis.aimdtools import get_lagtime_rmsd, plot_rmsd
-
-    timestep 表示时间步长
-
-    >>> lagtime, rmsd = get_lagtime_rmsd(datafile='dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5', timestep=0.1) # doctest: +ELLIPSIS
-    Reading ...dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5...
-    Calculating RMSD...
-
-    直接保存为RMSD.png图片
-
-    >>> plot_rmsd(lagtime, rmsd, figname='dspawpy_proj/dspawpy_tests/inputs/out/RMSD.png', show=False) # doctest: +ELLIPSIS
-    ==> ...dspawpy_proj/dspawpy_tests/inputs/out/RMSD.png
-    ...
+    Raises
+    ------
+    KeyError
+        Couldn't find an appropriate species.
+
+    Notes
+    -----
+        It's impossible to tell whether e.g. He is helium
+        or hydrogen labelled 'e'.
     """
-    # 参数初始化
-    if not ax:
-        ishow = True
-    else:
-        ishow = False
-
-    import matplotlib.pyplot as plt
 
-    if ax:
-        ax.plot(lagtime, result, **kwargs)
+    if len(label) >= 2:
+        test_symbol = label[0].upper() + label[1].lower()
+        if test_symbol in chemical_symbols:
+            return test_symbol
+    test_symbol = label[0].upper()
+    if test_symbol in chemical_symbols:
+        return test_symbol
     else:
-        fig, ax = plt.subplots()
-        ax.plot(lagtime, result, **kwargs)
-        ax.set_xlabel("Time (fs)")
-        ax.set_ylabel("RMSD (Å)")
-
-    if xlim:
-        ax.set_xlim(xlim)
-    if ylim:
-        ax.set_ylim(ylim)
-
-    plt.tight_layout()
-    if figname:
-        absfig = os.path.abspath(figname)
-        os.makedirs(os.path.dirname(absfig), exist_ok=True)
-        plt.savefig(absfig, dpi=300)
-        print(f"==> {absfig}")
-    if show and ishow:  # 画子图的话，不应每个子图都show
-        plt.show()  # show会自动清空图片
-
-    return ax
-
-
-def _get_time_step(datafile):
-    absfile = os.path.abspath(datafile)
-    if absfile.endswith(".h5"):
-        hpath = os.path.abspath(absfile)
-        import h5py
-        import numpy as np
-
-        hf = h5py.File(hpath)
-        try:
-            t = np.array(hf["/Structures/TimeStep"])[0]
-            timestep = float(t)
-        except Exception:
-            print(str(Exception))
-            timestep = 1.0
-    elif absfile.endswith(".json"):
-        jpath = os.path.abspath(absfile)
-        with open(jpath, "r") as f:
-            import json
-
-            jdata = json.load(f)
-        try:
-            t = jdata["Structures"][0]["TimeStep"]
-            timestep = float(t)
-        except Exception:
-            print(str(Exception))
-            timestep = 1.0
-    else:
-        raise ValueError(f"{absfile} must be .h5 or .json")
-
-    return timestep
+        raise KeyError("Could not parse species from label {0}." "".format(label))
```

### Comparing `dspawpy-1.2.2/dspawpy/analysis/vacf.py` & `dspawpy-1.3.0/dspawpy/analysis/vacf.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 
 def pad_zeros(
     arr, axis=0, where="end", nadd=None, upto=None, tonext=None, tonext_min=None
 ):
     """Pad an nd-array with zeros. Default is to append an array of zeros of
     the same shape as `arr` to arr's end along `axis`.
+
     Parameters
     ----------
     arr :  nd array
     axis : the axis along which to pad
     where : string {'end', 'start'}, pad at the end ("append to array") or
         start ("prepend to array") of `axis`
     nadd : number of items to padd (i.e. nadd=3 means padd w/ 3 zeros in case
@@ -45,46 +46,18 @@
     upto : pad until arr.shape[axis] == upto
     tonext : bool, pad up to the next power of two (pad so that the padded
         array has a length of power of two)
     tonext_min : int, when using `tonext`, pad the array to the next possible
         power of two for which the resulting array length along `axis` is at
         least `tonext_min`; the default is tonext_min = arr.shape[axis]
     Use only one of nadd, upto, tonext.
+
     Returns
     -------
     padded array
-    Examples
-    --------
-    >>> # 1d
-    >>> pad_zeros(a)
-    array([1, 2, 3, 0, 0, 0])
-    >>> pad_zeros(a, nadd=3)
-    array([1, 2, 3, 0, 0, 0])
-    >>> pad_zeros(a, upto=6)
-    array([1, 2, 3, 0, 0, 0])
-    >>> pad_zeros(a, nadd=1)
-    array([1, 2, 3, 0])
-    >>> pad_zeros(a, nadd=1, where='start')
-    array([0, 1, 2, 3])
-    >>> # 2d
-    >>> a=arange(9).reshape(3,3)
-    >>> pad_zeros(a, nadd=1, axis=0)
-    array([[0, 1, 2],
-           [3, 4, 5],
-           [6, 7, 8],
-           [0, 0, 0]])
-    >>> pad_zeros(a, nadd=1, axis=1)
-    array([[0, 1, 2, 0],
-           [3, 4, 5, 0],
-           [6, 7, 8, 0]])
-    >>> # up to next power of two
-    >>> 2**arange(10)
-    array([  1,   2,   4,   8,  16,  32,  64, 128, 256, 512])
-    >>> pydos.pad_zeros(arange(9), tonext=True).shape
-    (16,)
     """
     if tonext is False:
         tonext = None
     lst = [nadd, upto, tonext]
     assert lst.count(None) in [2, 3], (
         "`nadd`, `upto` and `tonext` must be " + "all None or only one of them not None"
     )
@@ -118,44 +91,30 @@
         raise Exception("illegal `where` arg: %s" % where)
 
 
 def slicetake(a, sl, axis=None, copy=False):
     """The equivalent of numpy.take(a, ..., axis=<axis>), but accepts slice
     objects instead of an index array. Also by default, it returns a *view* and
     no copy.
+
     Parameters
     ----------
     a : numpy ndarray
     sl : slice object, list or tuple of slice objects
         axis=<int>
             one slice object for *that* axis
         axis=None
             `sl` is a list or tuple of slice objects, one for each axis.
             It must index the whole array, i.e. len(sl) == len(a.shape).
     axis : {None, int}
     copy : bool, return a copy instead of a view
+
     Returns
     -------
     A view into `a` or copy of a slice of `a`.
-    Examples
-    --------
-    >>> from numpy import s_
-    >>> a = np.random.rand(20,20,20)
-    >>> b1 = a[:,:,10:]
-    >>> # single slice for axis 2
-    >>> b2 = slicetake(a, s_[10:], axis=2)
-    >>> # tuple of slice objects
-    >>> b3 = slicetake(a, s_[:,:,10:])
-    >>> (b2 == b1).all()
-    True
-    >>> (b3 == b1).all()
-    True
-    >>> # simple extraction too, sl = integer
-    >>> (a[...,5] == slicetake(a, 5, axis=-1))
-    True
     """
     # The long story
     # --------------
     #
     # 1) Why do we need that:
     #
     # # no problem
@@ -234,14 +193,15 @@
 def sum(arr, axis=None, keepdims=False, **kwds):
     """This numpy.sum() with some features implemented which can be found in
     numpy v1.7 and later: `axis` can be a tuple to select arbitrary axes to sum
     over.
     We also have a `keepdims` keyword, which however works completely different
     from numpy. Docstrings shamelessly stolen from numpy and adapted here
     and there.
+
     Parameters
     ----------
     arr : nd array
     axis : None or int or tuple of ints, optional
         Axis or axes along which a sum is performed. The default (`axis` =
         `None`) is to perform a sum over all the dimensions of the input array.
         `axis` may be negative, in which case it counts from the last to the
@@ -249,39 +209,14 @@
         If this is a tuple of ints, a sum is performed on multiple
         axes, instead of a single axis or all the axes as before.
     keepdims : bool, optional
         If this is set to True, the axes from `axis` are left in the result
         and the reduction (sum) is performed for all remaining axes. Therefore,
         it reverses the `axis` to be summed over.
     **kwds : passed to np.sum().
-    Examples
-    --------
-    >>> a=rand(2,3,4)
-    >>> num.sum(a)
-    12.073636268676152
-    >>> a.sum()
-    12.073636268676152
-    >>> num.sum(a, axis=1).shape
-    (2, 4)
-    >>> num.sum(a, axis=(1,)).shape
-    (2, 4)
-    >>> # same as axis=1, i.e. it inverts the axis over which we sum
-    >>> num.sum(a, axis=(0,2), keepdims=True).shape
-    (2, 4)
-    >>> # numpy's keepdims has another meaning: it leave the summed axis (0,2)
-    >>> # as dimension of size 1 to allow broadcasting
-    >>> numpy.sum(a, axis=(0,2), keepdims=True).shape
-    (1, 3, 1)
-    >>> num.sum(a, axis=(1,)) - num.sum(a, axis=1)
-    array([[ 0.,  0.,  0.,  0.],
-           [ 0.,  0.,  0.,  0.]])
-    >>> num.sum(a, axis=(0,2)).shape
-    (3,)
-    >>> num.sum(a, axis=(0,2)) - a.sum(axis=0).sum(axis=1)
-    array([ 0.,  0.,  0.])
     """
 
     # Recursion rocks!
     def _sum(arr, tosum):
         if len(tosum) > 0:
             # Choose axis to sum over, remove from list w/ remaining axes.
             axis = tosum.pop(0)
@@ -311,28 +246,31 @@
             alldims = range(arr.ndim)
             tosum = [xx for xx in alldims if xx not in tosum]
         return _sum(arr, tosum)
 
 
 def norm_int(y, x, area=1.0, scale=True, func=None):
     """Normalize integral area of y(x) to `area`.
+
     Parameters
     ----------
     x,y : numpy 1d arrays
     area : float
     scale : bool, optional
         Scale x and y to the same order of magnitude before integration.
         This may be necessary to avoid numerical trouble if x and y have very
         different scales.
     func : callable
         Function to do integration (like scipy.integrate.{simps,trapz,...}
         Called as ``func(y,x)``. Default: simps
+
     Returns
     -------
     scaled y
+
     Notes
     -----
     The argument order y,x might be confusing. x,y would be more natural but we
     stick to the order used in the scipy.integrate routines.
     """
     from scipy.integrate import simps
```

### Comparing `dspawpy-1.2.2/dspawpy/diffusion/neb.py` & `dspawpy-1.3.0/dspawpy/diffusion/neb.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,44 @@
 # -*- coding: utf-8 -*-
-import os
+from loguru import logger
 
 
 class NEB:
-    """NEB插值算法
-
-    Parameters
-    ----------
-    initial_structure: Structure
-        初态
-    final_structure: Structure
-        终态
-    nimages: int
-        中间构型数
-    """
-
-    def __init__(self, initial_structure, final_structure, nimages):
-        """
-
-        Args:
-            initial_structure:
-            final_structure:
-            nimages: number of images,contain initial and final structure
-        """
-
+    @logger.catch
+    def __init__(self, initial_structure, final_structure, nimages: int):
         self.nimages = nimages
         from dspawpy.diffusion.pathfinder import IDPPSolver
 
         self.iddp = IDPPSolver.from_endpoints(
             endpoints=[initial_structure, final_structure],
             nimages=self.nimages - 2,
             sort_tol=0,  # 锁定原子编号
         )
 
+    @logger.catch
     def linear_interpolate(self):
         return self.iddp.structures
 
+    @logger.catch
     def idpp_interpolate(
         self,
-        maxiter=1000,
-        tol=1e-5,
-        gtol=1e-3,
-        step_size=0.05,
-        max_disp=0.05,
-        spring_const=5.0,
+        maxiter: int = 1000,
+        tol: float = 1e-5,
+        gtol: float = 1e-3,
+        step_size: float = 0.05,
+        max_disp: float = 0.05,
+        spring_const: float = 5.0,
     ):
         return self.iddp.run(maxiter, tol, gtol, step_size, max_disp, spring_const)
 
 
+@logger.catch
 def write_neb_structures(
-    structures,
-    coords_are_cartesian=True,
+    structures: list,
+    coords_are_cartesian: bool = True,
     fmt: str = "as",
     path: str = ".",
     prefix="structure",
 ):
     r"""插值并生成中间构型文件
 
     Parameters
@@ -88,30 +72,32 @@
 
     >>> from dspawpy.diffusion.neb import NEB,write_neb_structures
     >>> neb = NEB(init_struct,final_struct,8)
     >>> structures = neb.linear_interpolate()   #线性插值
 
     插值完成的构型可指定保存到neb文件夹下
 
-    >>> write_neb_structures(structures, fmt="as", path="dspawpy_proj/dspawpy_tests/inputs/out/11neb_interpolate_structures") # doctest: +ELLIPSIS
-    ==> ...dspawpy_proj/dspawpy_tests/inputs/out/11neb_interpolate_structures/00/structure00.as
-    ==> ...dspawpy_proj/dspawpy_tests/inputs/out/11neb_interpolate_structures/01/structure01.as
-    ==> ...dspawpy_proj/dspawpy_tests/inputs/out/11neb_interpolate_structures/02/structure02.as
-    ==> ...dspawpy_proj/dspawpy_tests/inputs/out/11neb_interpolate_structures/03/structure03.as
-    ==> ...dspawpy_proj/dspawpy_tests/inputs/out/11neb_interpolate_structures/04/structure04.as
-    ==> ...dspawpy_proj/dspawpy_tests/inputs/out/11neb_interpolate_structures/05/structure05.as
-    ==> ...dspawpy_proj/dspawpy_tests/inputs/out/11neb_interpolate_structures/06/structure06.as
-    ==> ...dspawpy_proj/dspawpy_tests/inputs/out/11neb_interpolate_structures/07/structure07.as
+    >>> write_neb_structures(structures, path="dspawpy_proj/dspawpy_tests/outputs/doctest/11neb_interpolate_structures") # doctest: +ELLIPSIS
+    ==> ...dspawpy_proj/dspawpy_tests/outputs/doctest/11neb_interpolate_structures/00/structure00.as
+    ==> ...dspawpy_proj/dspawpy_tests/outputs/doctest/11neb_interpolate_structures/01/structure01.as
+    ==> ...dspawpy_proj/dspawpy_tests/outputs/doctest/11neb_interpolate_structures/02/structure02.as
+    ==> ...dspawpy_proj/dspawpy_tests/outputs/doctest/11neb_interpolate_structures/03/structure03.as
+    ==> ...dspawpy_proj/dspawpy_tests/outputs/doctest/11neb_interpolate_structures/04/structure04.as
+    ==> ...dspawpy_proj/dspawpy_tests/outputs/doctest/11neb_interpolate_structures/05/structure05.as
+    ==> ...dspawpy_proj/dspawpy_tests/outputs/doctest/11neb_interpolate_structures/06/structure06.as
+    ==> ...dspawpy_proj/dspawpy_tests/outputs/doctest/11neb_interpolate_structures/07/structure07.as
     """
     if fmt is None:
         fmt = "as"
+    import os
+
     absdir = os.path.abspath(path)
     N = len(str(len(structures)))
     if N <= 2:
         N = 2
-    from dspawpy.io.write import to_file
+    from dspawpy.io.structure import write
 
     for i, structure in enumerate(structures):
         path_name = str(i).zfill(N)
         os.makedirs(os.path.join(absdir, path_name), exist_ok=True)
         filename = os.path.join(absdir, path_name, "%s%s.%s" % (prefix, path_name, fmt))
-        to_file(structure, filename, fmt, coords_are_cartesian)
+        write(structure, filename, fmt, coords_are_cartesian)
```

### Comparing `dspawpy-1.2.2/dspawpy/diffusion/nebtools.py` & `dspawpy-1.3.0/dspawpy/diffusion/nebtools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 # -*- coding: utf-8 -*-
-import json
-import os
-import shutil
-import warnings
+from typing import Optional
+from loguru import logger
 
-import numpy as np
 
-np.set_printoptions(suppress=True)  # 不使用科学计数法
+@logger.catch
+def _zip_folder(folder_path: str, output_path: str):
+    import os
 
-
-def _zip_folder(folder_path, output_path):
     absdir1 = os.path.abspath(folder_path)
     absdir2 = os.path.abspath(output_path)
     import zipfile
 
     with zipfile.ZipFile(absdir2, "w", zipfile.ZIP_DEFLATED) as zipf:
         for root, _, files in os.walk(absdir1):
             for file in files:
                 file_path = os.path.join(root, file)
                 zipf.write(file_path, os.path.relpath(file_path, absdir1))
 
 
-def get_distance(
-    spo1: np.ndarray, spo2: np.ndarray, lat1: np.ndarray, lat2: np.ndarray
-):
+@logger.catch
+def get_distance(spo1, spo2, lat1, lat2):
     r"""根据两个结构的分数坐标和晶胞计算距离
 
     Parameters
     ----------
     spo1 : np.ndarray
         分数坐标列表1
     spo2 : np.ndarray
@@ -54,25 +50,28 @@
     计算两个构型的距离
 
     >>> from dspawpy.diffusion.nebtools import get_distance
     >>> dist = get_distance(s1.frac_coords, s2.frac_coords, s1.lattice.matrix, s2.lattice.matrix)
     >>> print('两个构型的距离为：', dist, 'Angstrom')
     两个构型的距离为： 0.476972808803491 Angstrom
     """
+    import numpy as np
+
     diff_spo = spo1 - spo2  # 分数坐标差
     avglatv = 0.5 * (lat1 + lat2)  # 平均晶格矢量
     pbc_diff_spo = set_pbc(diff_spo)  # 笛卡尔坐标差
     # 分数坐标点乘平均晶胞，转回笛卡尔坐标
     pbc_diff_pos = np.dot(pbc_diff_spo, avglatv)  # 笛卡尔坐标差
     distance = np.sqrt(np.sum(pbc_diff_pos**2))
 
     return distance
 
 
-def get_neb_subfolders(directory: str = ".", return_abs=False):
+@logger.catch
+def get_neb_subfolders(directory: str = ".", return_abs: bool = False):
     r"""将directory路径下的子文件夹名称列表按照数字大小排序
 
     仅保留形如00，01数字类型的NEB子文件夹路径
 
     Parameters
     ----------
     subfolders : list
@@ -88,14 +87,16 @@
     Examples
     --------
     >>> from dspawpy.diffusion.nebtools import get_neb_subfolders
     >>> directory = 'dspawpy_proj/dspawpy_tests/inputs/2.15'
     >>> get_neb_subfolders(directory)
     ['00', '01', '02', '03', '04']
     """
+    import os
+
     absdir = os.path.abspath(directory)
     raw_subfolders = next(os.walk(absdir))[1]
     subfolders = []
     for subfolder in raw_subfolders:
         try:
             assert 0 <= int(subfolder) < 100
             subfolders.append(subfolder)
@@ -105,25 +106,26 @@
     if return_abs:
         subfolders = [
             os.path.abspath(os.path.join(absdir, subfolder)) for subfolder in subfolders
         ]
     return subfolders
 
 
+@logger.catch
 def plot_barrier(
     datafile: str = "neb.h5",
-    directory: str = None,
-    ri: float = None,
-    rf: float = None,
-    ei: float = None,
-    ef: float = None,
+    directory: Optional[str] = None,
+    ri: Optional[float] = None,
+    rf: Optional[float] = None,
+    ei: Optional[float] = None,
+    ef: Optional[float] = None,
     method: str = "PchipInterpolator",
     figname: str = "neb_barrier.png",
     show: bool = True,
-    raw=False,
+    raw: bool = False,
     **kwargs,
 ):
     r"""调用 scipy.interpolate 插值算法，拟合NEB能垒并绘图
 
     Parameters
     ----------
     datafile: str
@@ -160,24 +162,27 @@
     >>> import matplotlib.pyplot as plt
 
     对比不同插值算法
 
     >>> plot_barrier(directory='dspawpy_proj/dspawpy_tests/inputs/2.15', method='interp1d', kind=2, figname=None, show=False)
     >>> plot_barrier(directory='dspawpy_proj/dspawpy_tests/inputs/2.15', method='interp1d', kind=3, figname=None, show=False)
     >>> plot_barrier(directory='dspawpy_proj/dspawpy_tests/inputs/2.15', method='CubicSpline', figname=None, show=False)
-    >>> plot_barrier(directory='dspawpy_proj/dspawpy_tests/inputs/2.15', method='pchip', figname='dspawpy_proj/dspawpy_tests/outputs/doctest_out/barrier_comparison.png', show=False) # doctest: +ELLIPSIS
-    ==> .../doctest_out/barrier_comparison.png
+    >>> plot_barrier(directory='dspawpy_proj/dspawpy_tests/inputs/2.15', method='pchip', figname='dspawpy_proj/dspawpy_tests/outputs/doctest/barrier_comparison.png', show=False) # doctest: +ELLIPSIS
+    ==> .../doctest/barrier_comparison.png
 
     尝试读取neb.h5文件或neb.json文件
 
-    >>> plot_barrier(datafile='dspawpy_proj/dspawpy_tests/inputs/2.15/neb.h5', method='pchip', figname='dspawpy_proj/dspawpy_tests/outputs/doctest_out/barrier_h5.png', show=False) # doctest: +ELLIPSIS
-    ==> .../doctest_out/barrier_h5.png
-    >>> plot_barrier(datafile='dspawpy_proj/dspawpy_tests/inputs/2.15/neb.json', method='pchip', figname='dspawpy_proj/dspawpy_tests/outputs/doctest_out/barrier_json.png', show=False) # doctest: +ELLIPSIS
-    ==> .../doctest_out/barrier_json.png
+    >>> plot_barrier(datafile='dspawpy_proj/dspawpy_tests/inputs/2.15/neb.h5', method='pchip', figname='dspawpy_proj/dspawpy_tests/outputs/doctest/barrier_h5.png', show=False) # doctest: +ELLIPSIS
+    ==> .../doctest/barrier_h5.png
+    >>> plot_barrier(datafile='dspawpy_proj/dspawpy_tests/inputs/2.15/neb.json', method='pchip', figname='dspawpy_proj/dspawpy_tests/outputs/doctest/barrier_json.png', show=False) # doctest: +ELLIPSIS
+    ==> .../doctest/barrier_json.png
     """
+    import os
+    import numpy as np
+
     if directory is not None:
         # read data
         subfolders, resort_mfs, rcs, ens, dEs = _getef(os.path.abspath(directory))
 
     elif datafile:
         from dspawpy.io.utils import get_absfile
 
@@ -190,21 +195,25 @@
                 reaction_coordinate = neb["/BarrierInfo/ReactionCoordinate"]
                 energy = neb["/BarrierInfo/TotalEnergy"]
             else:  # old version
                 reaction_coordinate = neb["/Distance/ReactionCoordinate"]
                 energy = neb["/Energy/TotalEnergy"]
         elif absfile.endswith(".json"):
             with open(absfile, "r") as fin:
-                neb = json.load(fin)
+                from json import load
+
+                neb = load(fin)
             if "BarrierInfo" in neb.keys():
                 reaction_coordinate = neb["BarrierInfo"]["ReactionCoordinate"]
                 energy = neb["BarrierInfo"]["TotalEnergy"]
             else:  # old version
                 reaction_coordinate = neb["Distance"]["ReactionCoordinate"]
                 energy = neb["Energy"]["TotalEnergy"]
+        else:
+            raise ValueError("only h5 and json file are supported")
 
         x = reaction_coordinate  # 从neb.h5/json 读取的不需要累加
 
         y = [x - energy[0] for x in energy]
         # initial and final info
         if ri is not None:  # add initial reaction coordinate
             x.insert(0, ri)
@@ -235,20 +244,30 @@
     except Exception:
         raise ValueError(f"Please check whether {kwargs} is valid for {method}！")
 
     xnew = np.linspace(rcs[0], rcs[-1], 100)
     ynew = inter_f(xnew)
 
     if raw:
-        import pandas as pd
+        try:
+            import polars as pl
 
-        pd.DataFrame({"x_raw": rcs, "y_raw": dEs}).to_csv("raw_xy.csv", index=False)
-        pd.DataFrame({"x_interpolated": xnew, "y_interpolated": ynew}).to_csv(
-            "raw_interpolated_xy.csv", index=False
-        )
+            pl.DataFrame({"x_raw": rcs, "y_raw": dEs}).write_csv(
+                "raw_xy.csv",
+            )
+            pl.DataFrame({"x_interpolated": xnew, "y_interpolated": ynew}).write_csv(
+                "raw_interpolated_xy.csv",
+            )
+        except ModuleNotFoundError:
+            import pandas as pd
+
+            pd.DataFrame({"x_raw": rcs, "y_raw": dEs}).to_csv("raw_xy.csv")
+            pd.DataFrame({"x_interpolated": xnew, "y_interpolated": ynew}).to_csv(
+                "raw_interpolated_xy.csv",
+            )
 
     # plot
     import matplotlib.pyplot as plt  # noqa: E402
 
     if kwargs:
         plt.plot(xnew, ynew, label=method + str(kwargs))
     else:
@@ -265,14 +284,15 @@
         os.makedirs(os.path.dirname(absfig), exist_ok=True)
         plt.savefig(absfig, dpi=300)
         print(f"==> {absfig}")
     if show:
         plt.show()
 
 
+@logger.catch
 def plot_neb_converge(
     neb_dir: str,
     image_key: str = "01",
     show: bool = True,
     figname: str = "neb_conv.png",
     raw=False,
 ):
@@ -295,21 +315,23 @@
     -------
     ax1, ax2 : matplotlib.axes.Axes
         两个子图的Axes对象
 
     Examples
     --------
     >>> from dspawpy.diffusion.nebtools import plot_neb_converge
-    >>> result = plot_neb_converge(neb_dir='dspawpy_proj/dspawpy_tests/inputs/2.15', image_key='01', figname='dspawpy_proj/dspawpy_tests/inputs/out/neb_converge1.png',show=False) # doctest: +ELLIPSIS
-    ==> ...dspawpy_proj/dspawpy_tests/inputs/out/neb_converge1.png
+    >>> result = plot_neb_converge(neb_dir='dspawpy_proj/dspawpy_tests/inputs/2.15', image_key='01', figname='dspawpy_proj/dspawpy_tests/outputs/doctest/neb_converge1.png',show=False) # doctest: +ELLIPSIS
+    ==> ...dspawpy_proj/dspawpy_tests/outputs/doctest/neb_converge1.png
     """
     from dspawpy.io.utils import get_absfile
+    import os
+    import numpy as np
 
     absfile = get_absfile(neb_dir, "neb")
-    if os.path.isfile(absfile):
+    if absfile.endswith("h5"):
         import h5py
 
         neb_total = h5py.File(absfile)
         # new output (>=2022B)
         if "/LoopInfo/01/MaxForce" in neb_total.keys():
             maxforce = np.array(neb_total.get("/LoopInfo/" + image_key + "/MaxForce"))
         else:  # old output
@@ -320,51 +342,63 @@
                 neb_total.get("/LoopInfo/" + image_key + "/TotalEnergy")
             )
         else:  # old output
             total_energy = np.array(
                 neb_total.get("/Iteration/" + image_key + "/TotalEnergy")
             )
 
-    elif os.path.isfile(absfile):
+    elif absfile.endswith("json"):
         with open(absfile, "r") as fin:
-            neb_total = json.load(fin)
+            from json import load
+
+            neb_total = load(fin)
         if "LoopInfo" in neb_total.keys():
             neb = neb_total["LoopInfo"][image_key]
         else:
             neb = neb_total["Iteration"][image_key]
         maxforce = []
         total_energy = []
         for n in neb:
             maxforce.append(n["MaxForce"])
             total_energy.append(n["TotalEnergy"])
 
         maxforce = np.array(maxforce)
         total_energy = np.array(total_energy)
 
+    else:
+        raise ValueError("Only h5 and json file are supported")
+
     x = np.arange(len(maxforce))
 
     force = maxforce
     energy = total_energy
 
     if raw:
-        import pandas as pd
+        try:
+            import polars as pl
 
-        pd.DataFrame({"x": x, "force": force, "energy": energy}).to_csv(
-            "neb_conv.csv", index=False
-        )
+            pl.DataFrame({"x": x, "force": force, "energy": energy}).write_csv(
+                "neb_conv.csv",
+            )
+        except ModuleNotFoundError:
+            import pandas as pd
+
+            pd.DataFrame({"x": x, "force": force, "energy": energy}).to_csv(
+                "neb_conv.csv",
+            )
 
     import matplotlib.pyplot as plt  # noqa: E402
 
     fig = plt.figure()
     ax1 = fig.add_subplot(111)
     ax1.plot(x, force, label="Max Force", c="black")
     ax1.set_xlabel("Number of ionic step")
     ax1.set_ylabel("Force (eV/Å)")
     ax2 = ax1.twinx()
-    ax2.plot(x, energy, label="Energy", c="r")
+    ax2.plot(x, energy, label="Energy", c="r")  # type: ignore
     ax2.set_xlabel("Number of ionic step")
     ax2.set_ylabel("Energy (eV)")
     ax2.ticklabel_format(useOffset=False)  # y轴坐标显示绝对值而不是相对值
     fig.legend(loc=1, bbox_to_anchor=(1, 1), bbox_transform=ax1.transAxes)
 
     plt.tight_layout()
     # save and show
@@ -375,15 +409,16 @@
         print(f"==> {absfig}")
     if show:
         plt.show()
 
     return ax1, ax2
 
 
-def printef(directory):
+@logger.catch
+def printef(directory: str):
     """打印NEB计算时各构型的能量和受力
 
     Parameters
     ----------
     directory : str
         NEB计算的目录，默认为当前目录
 
@@ -391,33 +426,59 @@
     -------
     打印各构型的能量和受力
 
     Examples
     --------
     >>> from dspawpy.diffusion.nebtools import printef
     >>> printef(directory='dspawpy_proj/dspawpy_tests/inputs/2.15')
-        Force(eV/Å)     RC(Å)    Energy(eV)  E-E0(eV)
-    00     0.180272  0.000000 -39637.098409  0.000000
-    01     0.026337  0.542789 -39637.018595  0.079814
-    02     0.024798  1.086800 -39636.880144  0.218265
-    03     0.234429  1.588367 -39636.998366  0.100043
-    04     0.014094  2.089212 -39637.089994  0.008414
+    FolderName  Force(eV/Å)    RC(Å)    Energy(eV)  E-E0(eV)
+            00     0.180272 0.000000 -39637.098409  0.000000
+            01     0.026337 0.542789 -39637.018595  0.079814
+            02     0.024798 1.086800 -39636.880144  0.218265
+            03     0.234429 1.588367 -39636.998366  0.100043
+            04     0.014094 2.089212 -39637.089994  0.008414
     """
-    subfolders, resort_mfs, rcs, ens, dEs = _getef(directory)
-    data = np.array([resort_mfs, rcs, ens, dEs], dtype=float)
+    from dspawpy.diffusion.nebtools import _getef
+    import numpy as np
+
+    data = np.array(_getef(directory)).T
+
     import pandas as pd
 
+    pd.set_option("display.float_format", "{:.6f}".format)
+
     df = pd.DataFrame(
-        data.T,
-        columns=["Force(eV/Å)", "RC(Å)", "Energy(eV)", "E-E0(eV)"],
-        index=subfolders,
+        data,
+        columns=["FolderName", "Force(eV/Å)", "RC(Å)", "Energy(eV)", "E-E0(eV)"],
     )
-    print(df)
+    df["Force(eV/Å)"] = df["Force(eV/Å)"].astype(float)
+    df["RC(Å)"] = df["RC(Å)"].astype(float)
+    df["Energy(eV)"] = df["Energy(eV)"].astype(float)
+    df["E-E0(eV)"] = df["E-E0(eV)"].astype(float)
+    print(df.to_string(index=False))
+    # try:
+    #     import polars as pl
+    #
+    #     df = pl.DataFrame(
+    #         data,
+    #         schema=["FolderName", "Force(eV/Å)", "RC(Å)", "Energy(eV)", "E-E0(eV)"],
+    #     )
+    #     col_names = [col_name for col_name in df.columns if col_name != "FolderName"]
+    #     df.with_columns(pl.col(col_names).cast(pl.Float32, strict=False))
+    #     print(df)
+    # except ModuleNotFoundError:
+    #     import pandas as pd
+    #
+    #     df = pd.DataFrame(
+    #         data,
+    #         columns=["FolderName", "Force(eV/Å)", "RC(Å)", "Energy(eV)", "E-E0(eV)"],
+    #     )
 
 
+@logger.catch
 def restart(directory: str = ".", output: str = "bakfile"):
     """将旧NEB任务归档压缩，并在原路径下准备续算
 
     Parameters
     ----------
     directory : str
         旧NEB任务所在路径，默认当前路径
@@ -425,28 +486,32 @@
         备份文件夹路径，默认将在当前路径新建一个bakfile文件夹用于备份；
         也可以任意指定一个路径，但不能与当前路径相同
 
     Examples
     ----------
     >>> from dspawpy.diffusion.nebtools import restart
     >>> from shutil import copytree
-    >>> if not os.path.exists('dspawpy_proj/dspawpy_tests/inputs/supplement/neb4bk2'):
-    ...     copytree('dspawpy_proj/dspawpy_tests/inputs/2.15', 'dspawpy_proj/dspawpy_tests/inputs/supplement/neb4bk2')
-    >>> restart(directory='dspawpy_proj/dspawpy_tests/inputs/supplement/neb4bk2', output='dspawpy_proj/dspawpy_tests/inputs/out/neb_backup') # doctest: +ELLIPSIS
-    ==> ...dspawpy_proj/dspawpy_tests/inputs/out/neb_backup
+    >>> copytree('dspawpy_proj/dspawpy_tests/inputs/2.15', 'dspawpy_proj/dspawpy_tests/outputs/doctest/neb4bk2', dirs_exist_ok=True)
+    'dspawpy_proj/dspawpy_tests/outputs/doctest/neb4bk2'
+    >>> restart(directory='dspawpy_proj/dspawpy_tests/outputs/doctest/neb4bk2', output='dspawpy_proj/dspawpy_tests/outputs/doctest/neb_backup') # doctest: +ELLIPSIS
+    ==> ...dspawpy_proj/dspawpy_tests/outputs/doctest/neb_backup
 
     续算准备工作可能需要较长时间才能完成，请耐心等待
     """
+    import os
+    import shutil
+
     absout = os.path.abspath(output)
     absdir = os.path.abspath(directory)
 
     if os.path.isdir(absout):
         from datetime import datetime
 
         shutil.move(absout, absout + "_" + datetime.now().strftime("%Y%m%d%H%M%S"))
+        logger.warning(f"{absout} already exists, renamed to {absout}_datetime")
 
     subfolders = get_neb_subfolders(absdir, return_abs=True)  # 获取子文件夹路径
     os.makedirs(absout, exist_ok=True)  # 创建bakfile文件夹
     # 先处理子文件夹00，01...
     for subfolder_old in subfolders:
         folder_index = subfolder_old.split("/")[-1]  # 00，01...
         subfolder_back = os.path.join(absout, folder_index)  # 子文件夹备份到此
@@ -510,14 +575,15 @@
 
     if os.path.isfile(f"{absdir}/DS-PAW.log"):
         shutil.move(f"{absdir}/DS-PAW.log", f"{absout}/DS-PAW.log")
 
     print(f"==> {absout}")
 
 
+@logger.catch
 def set_pbc(spo):
     """根据周期性边界条件将分数坐标分量移入 [-0.5, 0.5) 区间
 
     Parameters
     ----------
     spo : np.ndarray or list
         分数坐标列表
@@ -530,21 +596,28 @@
     Examples
     --------
     >>> from dspawpy.diffusion.nebtools import set_pbc
     >>> set_pbc([-0.6, 1.2, 2.3])
     array([0.4, 0.2, 0.3])
     """
     # wrap into [-0.5, 0.5)
+    import numpy as np
+
     pbc_spo = np.mod(np.array(spo) + 0.5, 1.0) - 0.5
 
     return pbc_spo
 
 
+@logger.catch
 def summary(
-    directory: str = ".", raw=False, show_converge=False, outdir: str = None, **kwargs
+    directory: str = ".",
+    raw=False,
+    show_converge=False,
+    outdir: Optional[str] = None,
+    **kwargs,
 ):
     r"""NEB任务完成总结，依次执行以下步骤：
 
     - 1. 打印各构型受力、反应坐标、能量、与初始构型的能量差
     - 2. 绘制能垒图
     - 3. 绘制并保存结构优化过程的能量和受力收敛过程图
 
@@ -561,31 +634,30 @@
     **kwargs : dict
         传递给plot_barrier的参数
 
     Examples
     --------
     >>> from dspawpy.diffusion.nebtools import summary
     >>> directory = 'dspawpy_proj/dspawpy_tests/inputs/2.15' # NEB计算路径，默认当前路径
-    >>> summary(directory, show=False, figname='dspawpy_proj/dspawpy_tests/outputs/doctest_out/neb_barrier.png') # doctest: +ELLIPSIS
-        Force(eV/Å)     RC(Å)    Energy(eV)  E-E0(eV)
-    00     0.180272  0.000000 -39637.098409  0.000000
-    01     0.026337  0.542789 -39637.018595  0.079814
-    02     0.024798  1.086800 -39636.880144  0.218265
-    03     0.234429  1.588367 -39636.998366  0.100043
-    04     0.014094  2.089212 -39637.089994  0.008414
-    ==> .../doctest_out/neb_barrier.png
-    ==> ...dspawpy_proj/dspawpy_tests/inputs/2.15/01/converge.png...
-    ==> ...dspawpy_proj/dspawpy_tests/inputs/2.15/01/converge.png
-    ==> ...dspawpy_proj/dspawpy_tests/inputs/2.15/02/converge.png...
-    ==> ...dspawpy_proj/dspawpy_tests/inputs/2.15/02/converge.png
-    ==> ...dspawpy_proj/dspawpy_tests/inputs/2.15/03/converge.png...
-    ==> ...dspawpy_proj/dspawpy_tests/inputs/2.15/03/converge.png
+    >>> summary(directory, show=False, figname='dspawpy_proj/dspawpy_tests/outputs/doctest/neb_barrier.png') # doctest: +ELLIPSIS
+    FolderName  Force(eV/Å)    RC(Å)    Energy(eV)  E-E0(eV)
+            00     0.180272 0.000000 -39637.098409  0.000000
+            01     0.026337 0.542789 -39637.018595  0.079814
+            02     0.024798 1.086800 -39636.880144  0.218265
+            03     0.234429 1.588367 -39636.998366  0.100043
+            04     0.014094 2.089212 -39637.089994  0.008414
+    ==> .../doctest/neb_barrier.png
+    ==> .../doctest/01/converge.png
+    ==> .../doctest/02/converge.png
+    ==> .../doctest/03/converge.png
 
     若inifin=false，用户必须将自洽的scf.h5或system.json放到初末态子文件夹中
     """
+    import os
+
     # 1. 绘制能垒图
     absdir = os.path.abspath(directory)
     printef(absdir)
 
     # 2. 打印各构型受力、反应坐标、能量、与初始构型的能量差
     import matplotlib.pyplot as plt  # noqa: E402
 
@@ -596,39 +668,45 @@
     subfolders = get_neb_subfolders(absdir)
     for subfolder in subfolders[1 : len(subfolders) - 1]:
         if outdir:
             absout = os.path.abspath(outdir)
             os.makedirs(os.path.join(absout, subfolder), exist_ok=True)
             pngfile = f"{absout}/{subfolder}/converge.png"
         else:
-            pngfile = f"{absdir}/{subfolder}/converge.png"
+            pngfile = (
+                f"dspawpy_proj/dspawpy_tests/outputs/doctest/{subfolder}/converge.png"
+            )
 
-        print(f"==> {pngfile}...")
         plot_neb_converge(
             neb_dir=absdir,
             image_key=subfolder,
             figname=pngfile,
             raw=raw,
             show=show_converge,
         )
     plt.clf()
 
 
+@logger.catch
 def write_movie_json(
-    preview: bool = False, directory: str = ".", step: int = -1, dst: str = None
+    preview: bool = False,
+    directory: str = ".",
+    step: int = -1,
+    dst: Optional[str] = None,
 ):
     DeprecationWarning("Please use write_json_chain() instead")
     write_json_chain(preview=preview, directory=directory, step=step, dst=dst)
 
 
+@logger.catch
 def write_json_chain(
     preview: bool = False,
     directory: str = ".",
     step: int = -1,
-    dst: str = None,
+    dst: Optional[str] = None,
     ignorels=False,
 ):
     r"""NEB计算或者初始插值后，读取信息，保存为 neb_chain*.json 文件
 
     用 Device Studio 打开该文件可以观察结构等信息
 
     Parameters
@@ -648,33 +726,35 @@
 
     Examples
     ----------
     >>> from dspawpy.diffusion.nebtools import write_json_chain
 
     NEB计算完成后要观察轨迹变化全过程，只需指定NEB计算路径即可
 
-    >>> write_json_chain(directory='dspawpy_proj/dspawpy_tests/inputs/2.15', dst='dspawpy_proj/dspawpy_tests/outputs/doctest_out') # doctest: +ELLIPSIS
+    >>> write_json_chain(directory='dspawpy_proj/dspawpy_tests/inputs/2.15', dst='dspawpy_proj/dspawpy_tests/outputs/doctest') # doctest: +ELLIPSIS
     structure info collected from latestStructure.as
-    ==> .../doctest_out/neb_chain_last.json
+    ==> .../doctest/neb_chain_last.json
 
     NEB计算完成后要观察第n离子步结构，请设置step为n，注意step从1开始计数
 
-    >>> write_json_chain(directory='dspawpy_proj/dspawpy_tests/inputs/2.15', step=1, dst='dspawpy_proj/dspawpy_tests/outputs/doctest_out') # doctest: +ELLIPSIS
-    ==> .../doctest_out/neb_chain_1.json
+    >>> write_json_chain(directory='dspawpy_proj/dspawpy_tests/inputs/2.15', step=1, dst='dspawpy_proj/dspawpy_tests/outputs/doctest') # doctest: +ELLIPSIS
+    ==> .../doctest/neb_chain_1.json
 
     如果指定的step数超过NEB实际完成的离子步，将会自动修改为最后一步
 
-    >>> write_json_chain(directory='dspawpy_proj/dspawpy_tests/inputs/2.15', step=10, dst='dspawpy_proj/dspawpy_tests/outputs/doctest_out') # doctest: +ELLIPSIS
-    ==> .../doctest_out/neb_chain_10.json
+    >>> write_json_chain(directory='dspawpy_proj/dspawpy_tests/inputs/2.15', step=10, dst='dspawpy_proj/dspawpy_tests/outputs/doctest') # doctest: +ELLIPSIS
+    ==> .../doctest/neb_chain_10.json
 
     另外，如需预览初插结构，请将preview设置为True，并将directory指定为NEB计算主路径
 
-    >>> write_json_chain(preview=True, directory='dspawpy_proj/dspawpy_tests/inputs/2.15', dst='dspawpy_proj/dspawpy_tests/outputs/doctest_out') # doctest: +ELLIPSIS
-    ==> .../doctest_out/neb_chain_init.json
+    >>> write_json_chain(preview=True, directory='dspawpy_proj/dspawpy_tests/inputs/2.15', dst='dspawpy_proj/dspawpy_tests/outputs/doctest') # doctest: +ELLIPSIS
+    ==> .../doctest/neb_chain_init.json
     """
+    import os
+
     absdir = os.path.abspath(directory)
     if preview:  # preview mode
         raw = get_raw_from_structure(absdir)
     else:
         if step == 0:  # try preview mode to save time
             raw = get_raw_from_structure(absdir)
         elif step == -1:  # 优先级 latestStructure.as > h5 > json
@@ -682,68 +762,72 @@
                 raw = get_raw_from_h5_json(absdir, step)
             else:
                 try:  # read ls.as
                     raw = _from_structures(absdir, ls=True)
                     print("structure info collected from latestStructure.as")
                 except FileNotFoundError:
                     raw = get_raw_from_h5_json(absdir, step)
-                except Exception as e:
-                    print(e)
         else:
             raw = get_raw_from_h5_json(absdir, step)
 
     new = []
+    assert raw is not None
     if dst is not None:
         abs_dst = os.path.abspath(dst)
         os.makedirs(abs_dst, exist_ok=True)
         new.append(f"{abs_dst}/{raw[0]}")
         for i in range(1, len(raw)):
             new.append(raw[i])
         _dump_neb_chain_json(new)
     else:
         _dump_neb_chain_json(raw)
 
 
+@logger.catch
 def write_xyz(
-    preview: bool = False, directory: str = ".", step: int = -1, dst: str = None
+    preview: bool = False,
+    directory: str = ".",
+    step: int = -1,
+    dst: Optional[str] = None,
 ):
     DeprecationWarning("Please use write_xyz_chain() instead")
     write_xyz_chain(preview=preview, directory=directory, step=step, dst=dst)
 
 
-def get_raw_from_structure(dire):
+@logger.catch
+def get_raw_from_structure(dire: str):
     try:
         raw = _from_structures(dire)
         return raw
     except FileNotFoundError:
         print("No structure file")
     except Exception as e:
         print(e)
 
 
-def get_raw_from_h5_json(dire, step):
+@logger.catch
+def get_raw_from_h5_json(dire: str, step: int):
     try:
         raw = _from_h5(dire, step)
         return raw
     except FileNotFoundError:
         try:
             raw = _from_json(dire, step)
-        except json.decoder.JSONDecodeError:
-            print("json decode error!")
         except Exception as e:
             print(e)
     except Exception as e:
         print(e)
 
 
+@logger.catch
 def write_xyz_chain(
     preview: bool = False,
     directory: str = ".",
     step: int = -1,
-    dst: str = None,
+    dst: Optional[str] = None,
     ignorels=False,
 ):
     r"""
     将NEB结构链条写成xyz轨迹文件用于可视化
 
     Parameters
     ----------
@@ -762,33 +846,35 @@
 
     Examples
     ----------
     >>> from dspawpy.diffusion.nebtools import write_xyz_chain
 
     NEB计算完成后要观察轨迹变化全过程，只需指定NEB计算路径即可
 
-    >>> write_xyz_chain(directory='dspawpy_proj/dspawpy_tests/inputs/2.15', dst='dspawpy_proj/dspawpy_tests/outputs/doctest_out') # doctest: +ELLIPSIS
+    >>> write_xyz_chain(directory='dspawpy_proj/dspawpy_tests/inputs/2.15', dst='dspawpy_proj/dspawpy_tests/outputs/doctest') # doctest: +ELLIPSIS
     structure info collected from latestStructure.as
-    ==> .../doctest_out/neb_chain_last.xyz
+    ==> .../doctest/neb_chain_last.xyz
 
     NEB计算完成后要观察第n离子步结构，请设置step为n，注意step从1开始计数
 
-    >>> write_xyz_chain(directory='dspawpy_proj/dspawpy_tests/inputs/2.15', step=1, dst='dspawpy_proj/dspawpy_tests/outputs/doctest_out') # doctest: +ELLIPSIS
-    ==> .../doctest_out/neb_chain_1.xyz
+    >>> write_xyz_chain(directory='dspawpy_proj/dspawpy_tests/inputs/2.15', step=1, dst='dspawpy_proj/dspawpy_tests/outputs/doctest') # doctest: +ELLIPSIS
+    ==> .../doctest/neb_chain_1.xyz
 
     如果指定的step数超过NEB实际完成的离子步，会被自动修改为最后一步
 
-    >>> write_xyz_chain(directory='dspawpy_proj/dspawpy_tests/inputs/2.15', step=10, dst='dspawpy_proj/dspawpy_tests/outputs/doctest_out') # doctest: +ELLIPSIS
-    ==> .../doctest_out/neb_chain_10.xyz
+    >>> write_xyz_chain(directory='dspawpy_proj/dspawpy_tests/inputs/2.15', step=10, dst='dspawpy_proj/dspawpy_tests/outputs/doctest') # doctest: +ELLIPSIS
+    ==> .../doctest/neb_chain_10.xyz
 
     另外，如需预览初插结构，请将preview设置为True，并将directory指定为NEB计算主路径
 
-    >>> write_xyz_chain(preview=True, directory='dspawpy_proj/dspawpy_tests/inputs/2.15', dst='dspawpy_proj/dspawpy_tests/outputs/doctest_out') # doctest: +ELLIPSIS
-    ==> .../doctest_out/neb_chain_init.xyz
+    >>> write_xyz_chain(preview=True, directory='dspawpy_proj/dspawpy_tests/inputs/2.15', dst='dspawpy_proj/dspawpy_tests/outputs/doctest') # doctest: +ELLIPSIS
+    ==> .../doctest/neb_chain_init.xyz
     """
+    import os
+
     absdir = os.path.abspath(directory)
     if preview:  # preview mode, write neb_chain_init.xyz from structure.as
         raw = get_raw_from_structure(absdir)
     else:
         if step == 0:  # try preview mode to save time
             raw = get_raw_from_structure(absdir)
         elif step == -1:  # 优先级 latestStructure.as > h5 > json
@@ -796,33 +882,35 @@
                 raw = get_raw_from_h5_json(absdir, step)
             else:
                 try:  # read ls.as
                     raw = _from_structures(absdir, ls=True)
                     print("structure info collected from latestStructure.as")
                 except FileNotFoundError:
                     raw = get_raw_from_h5_json(absdir, step)
-                except Exception as e:
-                    print(e)
         else:
             raw = get_raw_from_h5_json(absdir, step)
 
     new = []
+    assert raw is not None
     if dst is not None:
         abs_dst = os.path.abspath(dst)
         os.makedirs(abs_dst, exist_ok=True)
         new.append(f"{abs_dst}/{raw[0]}")
         for i in range(1, len(raw)):
             new.append(raw[i])
         _dump_neb_xyz(new)
     else:
         _dump_neb_xyz(raw)
 
 
+@logger.catch
 def _dump_neb_xyz(raw):
     """根据之前收集到的各数据列表，dump json文件到output"""
+    import os
+
     (
         output,
         subfolders,
         step,
         MaxForces,
         TotalEnergies,
         Poses,  # Nimage x Natom x 3 , read
@@ -866,36 +954,43 @@
                 f.write(
                     "%s %f %f %f\n"
                     % (eles[i], Poses[n, i, 0], Poses[n, i, 1], Poses[n, i, 2])
                 )
     print(f"==> {absout}")
 
 
-def _from_structures(directory: str, ls=False):
+@logger.catch
+def _from_structures(directory: str, ls: bool = False):
     """从structure00.as，structure01.as，...，中读取结构信息，
     写入neb_chain_init，以便用DeviceStudio打开观察
 
     Parameters
     ----------
     directory : str
         NEB计算路径，默认当前路径
+    ls: bool
+        是否是最新构型
 
     Returns
     -------
     用于json文件的各个数组
     """
+    import os
+
     absdir = os.path.abspath(directory)
     if ls:
         output = "neb_chain_last.json"
     else:
         output = "neb_chain_init.json"
     step = 0
 
     subfolders = get_neb_subfolders(absdir)
     nimage = len(subfolders)
+    import numpy as np
+
     reactionCoordinates = np.zeros(shape=nimage)  # optional
     totalEnergies = np.zeros(shape=nimage)  # optional
     maxForces = np.zeros(shape=nimage - 2)  # optional
     tangents = np.zeros(shape=nimage - 2)  # optional
     MaxForces = np.zeros(shape=(nimage - 2, step + 1))  # optional
     TotalEnergies = np.zeros(shape=(nimage - 2, step + 1))  # optional
 
@@ -954,14 +1049,15 @@
         totalEnergies,
         maxForces,
         tangents,
         iDirects,
     )
 
 
+@logger.catch
 def _from_h5(directory: str, step: int):
     """从NEB路径下的h5文件读取 从第一步开始到指定step数 的结构和能量信息，
     写入json文件，以便用DeviceStudio打开观察。
 
     支持热读取结构信息（其他信息忽略）
 
     Parameters
@@ -971,24 +1067,28 @@
     step : int
         step数，默认-1，读取最后一个构型
 
     Returns
     -------
     用于json文件的各个数组
     """
+    import os
+
     absdir = os.path.abspath(directory)
     # ^ 前期设置
     neb_h5 = os.path.abspath(os.path.join(absdir, "01", "neb01.h5"))
     from dspawpy.io.read import get_ele_from_h5
 
     ele = get_ele_from_h5(hpath=neb_h5)
     Natom = len(ele)
     import h5py
 
     data = h5py.File(neb_h5)
+    import numpy as np
+
     try:
         total_steps = np.array(data.get("/NebSize"))[0]
     except Exception:
         print("Reading latest info for unfinished NEB task...")
         try:
             total_steps = np.array(data.get("/Structures/FinalStep"))[0]
         except Exception:
@@ -998,15 +1098,15 @@
 
     if step == -1:
         output = "neb_chain_last.json"
         step = total_steps
     elif step > total_steps:
         output = "neb_chain_last.json"
         step = total_steps
-        warnings.warn(
+        logger.warning(
             "specified %s > %s, reading last step info..." % (step, total_steps)
         )
     else:
         output = "neb_chain_{}.json".format(step)
 
     # ^ 读取前，准备好json文件所需数组框架
     subfolders = get_neb_subfolders(absdir)
@@ -1043,14 +1143,15 @@
 
     # ^ 开始分功能读取数据
     from dspawpy.io.structure import read
 
     for i, folder in enumerate(subfolders):
         if folder == subfolders[0] or folder == subfolders[-1]:
             h5_path = os.path.join(absdir, folder, "scf.h5")
+            spath = os.path.join(absdir, folder, f"structure{folder}.as")
             if os.path.isfile(h5_path):
                 data = h5py.File(h5_path)
                 # 不影响可视化，直接定为0
                 if folder == subfolders[0]:
                     reactionCoordinates[i] = 0
                 pos = np.array(data.get("/Structures/Step-1/Position")).reshape(
                     -1, 3
@@ -1137,14 +1238,15 @@
         totalEnergies,
         maxForces,
         tangents,
         iDirects,
     )
 
 
+@logger.catch
 def _from_json(directory: str, step: int):
     """从NEB路径下的json文件读取 从第一步开始到指定step数 的结构和能量信息，
     写入json文件，以便用DeviceStudio打开观察
 
     Parameters
     ----------
     directory : str
@@ -1153,28 +1255,32 @@
         step数，默认-1，读取最后一个构型
 
     Returns
     -------
     用于json文件的各个数组
     """
 
+    import os
+    import numpy as np
+    from json import load
+
     absdir = os.path.abspath(directory)
     # ^ 前期设置
     neb_js = os.path.join(absdir, "01/neb01.json")
     with open(neb_js, "r") as f:
-        data = json.load(f)
+        data = load(f)
     total_steps = len(data)
 
     if step == -1:
         output = "neb_chain_last.json"
         step = total_steps
     elif step > total_steps:
         output = "neb_chain_last.json"
         step = total_steps
-        warnings.warn(
+        logger.warning(
             "specified %s > %s, reading last step info..." % (step, total_steps)
         )
     else:
         output = f"neb_chain_{step}.json"
 
     # ^ 读取前，准备好json文件所需数组框架
     subfolders = get_neb_subfolders(absdir)
@@ -1209,19 +1315,19 @@
         if i == 0:  # 初末态在NEB计算过程中不会优化结构
             # 1. 外部自洽后移动system.json
             js_path = os.path.join(absdir, folder, "system.json")
             # 2. 直接NEB计算，得到system00.json
             neb_js_path = os.path.join(absdir, folder, f"system{folder}.json")
             if os.path.isfile(neb_js_path):  # 优先读取neb计算得到的system00.json
                 with open(neb_js_path, "r") as f:
-                    data = json.load(f)
+                    data = load(f)
 
             elif os.path.isfile(js_path):
                 with open(js_path, "r") as f:
-                    data = json.load(f)
+                    data = load(f)
 
             else:
                 raise FileNotFoundError(f"No {js_path}/{neb_js_path}")
 
             lat = data["AtomInfo"]["Lattice"]
             Latvs.append(lat)
 
@@ -1235,30 +1341,30 @@
 
         elif i > 0 and i < nimage - 1:  # 中间构型会优化结构
             # 读取晶胞矢量、原子坐标
             relax_json = os.path.join(absdir, folder, "relax.json")
             assert os.path.isfile(relax_json), f"No {relax_json}!"
 
             with open(relax_json, "r") as f:
-                rdata = json.load(f)
+                rdata = load(f)
 
             lat = rdata[step - 1]["Lattice"]  # 第step步优化后的晶胞
             Latvs.append(lat)
 
             Natom = len(rdata[0]["Atoms"])
             for j in range(Natom):  # for each atom
                 pos = rdata[step - 1]["Atoms"][j][
                     "Position"
                 ]  # 第step步优化后的原子坐标
                 Sposes.append(pos)  # ! 输出的都是分数坐标
 
             # 读取能量和反应坐标
             nj = os.path.join(absdir, folder, f"neb{folder}.json")
             with open(nj, "r") as f:
-                ndata = json.load(f)
+                ndata = load(f)
 
             totalEnergies[i] = ndata[step - 1][
                 "TotalEnergy"
             ]  # 读取第step步优化后的能量
 
             # 读取与前一个构型相比的反应坐标
             reactionCoordinates[i - 1] = ndata[step - 1]["ReactionCoordinate"][-2]
@@ -1271,19 +1377,19 @@
                 TotalEnergies[i - 1, j] = ndata[j]["TotalEnergy"]
 
         else:  # 末态构型
             js_path = os.path.join(absdir, folder, "system.json")
             neb_js_path = os.path.join(absdir, folder, f"system{folder}.json")
             if os.path.isfile(neb_js_path):  # 优先读取neb计算得到的json文件
                 with open(neb_js_path, "r") as f:
-                    data = json.load(f)
+                    data = load(f)
 
             elif os.path.isfile(js_path):
                 with open(js_path, "r") as f:
-                    data = json.load(f)
+                    data = load(f)
 
             else:
                 raise FileNotFoundError(f"No {js_path}/{neb_js_path}")
 
             lat = data["AtomInfo"]["Lattice"]
             Latvs.append(lat)
 
@@ -1294,15 +1400,15 @@
 
             energy = data["Energy"]["TotalEnergy0"]
             totalEnergies[i] = energy
 
     # 读取原子元素
     tneb_js = os.path.join(absdir, "neb.json")
     with open(tneb_js, "r") as f:
-        tdata = json.load(f)
+        tdata = load(f)
 
     Natom = len(tdata["UnrelaxStructure"][0]["Atoms"])
     elems = []
     for k in range(Natom):
         ele = tdata["UnrelaxStructure"][0]["Atoms"][k]["Element"]
         elems.append(ele)
 
@@ -1347,14 +1453,15 @@
         totalEnergies,
         maxForces,
         tangents,
         iDirects,
     )
 
 
+@logger.catch
 def _dump_neb_chain_json(raw):
     """根据之前收集到的各数据列表，dump json文件到output"""
     (
         output,
         subfolders,
         step,
         MaxForces,
@@ -1423,22 +1530,27 @@
         "Force": {"MaxForce": maxForces.tolist(), "Tangent": tangents.tolist()},
         "Iteration": IterDict,
         "RelaxedStructure": RSList,
         "UnrelaxedStructure": URSList,
     }
 
     # ^ 将字典写入json文件
+    import os
+
     absout = os.path.abspath(output)
     with open(absout, "w") as f:
-        json.dump(data, f, indent=4)
+        from json import dump
+
+        dump(data, f, indent=4)
 
     print(f"==> {absout}")
 
 
-def _getef(directory: str = ".") -> list:
+@logger.catch
+def _getef(directory: str = "."):
     """读取NEB计算时各构型的能量和受力，NEB计算可以未收敛
     但如果初末态自洽在别处完成，请手动将其移入00等文件夹中！
 
     Parameters
     ----------
     directory: str
         NEB计算的路径，默认当前路径
@@ -1452,14 +1564,17 @@
     rcs: list
         反应坐标列表
     ens: list
         电子总能列表
     dEs: list
         与初始构型的能量差列表
     """
+    import os
+    import numpy as np
+
     absdir = os.path.abspath(directory)
     subfolders = get_neb_subfolders(absdir)
     Nimage = len(subfolders)
 
     ens = []
     dEs = np.zeros(Nimage)
     rcs = [0]
@@ -1480,23 +1595,27 @@
                 en = np.array(data.get("/Energy/TotalEnergy0"))[0]
                 if i == 0 or i == Nimage - 1:
                     mf = np.max(np.abs(np.array(data.get("/Force/ForceOnAtoms"))))
                     mfs.append(mf)
 
             elif os.path.isfile(jsf):  # 其次读取json文件内容
                 with open(jsf, "r") as f:
-                    data = json.load(f)
+                    from json import load
+
+                    data = load(f)
                 en = data["Energy"]["TotalEnergy0"]
                 if i == 0 or i == Nimage - 1:
                     mf = np.max(np.abs(data["Force"]["ForceOnAtoms"]))
                     mfs.append(mf)
 
             elif os.path.isfile(old_jsf):  # 兼容老json
                 with open(old_jsf, "r") as f:
-                    data = json.load(f)
+                    from json import load
+
+                    data = load(f)
                 en = data["Energy"]["TotalEnergy0"]
                 if i == 0 or i == Nimage - 1:
                     mf = np.max(np.abs(data["Force"]["ForceOnAtoms"]))
                     mfs.append(mf)
 
             else:
                 raise FileNotFoundError(f"No {jsf}/{old_jsf}/{hf} for {subfolder}")
@@ -1530,27 +1649,29 @@
                     else:
                         raise KeyError(
                             f"Neither /Distance/Next nor /ReactionCoordinate in {hf}"
                         )
                     rcs.append(rc)
 
             elif os.path.isfile(jsf):
+                from json import load
+
                 if os.path.isfile(sysjsf):
                     with open(sysjsf, "r") as f:
-                        data = json.load(f)
+                        data = load(f)
                     en = data["Energy"]["TotalEnergy0"]
                 elif os.path.isfile(old_sysjsf):  # 兼容旧版DS-PAW
                     with open(old_sysjsf, "r") as f:
-                        data = json.load(f)
+                        data = load(f)
                     en = data["Energy"]["TotalEnergy0"]
                 else:
                     raise FileNotFoundError(f"No {sysjsf}/{old_sysjsf}")
 
                 with open(jsf, "r") as f:
-                    data = json.load(f)
+                    data = load(f)
                 Nion_step = len(data)
                 # en = data[Nion_step - 1]["TotalEnergy"] # invalid
                 mf = data[Nion_step - 1]["MaxForce"]  # 最后一步的最大受力
                 rc = data[Nion_step - 1]["ReactionCoordinate"][0]  # 最后一步的反应坐标
                 rcs.append(rc)
                 if count == Nimage - 2:  # before final image
                     rc = data[Nion_step - 1]["ReactionCoordinate"][
@@ -1581,28 +1702,34 @@
     for j in range(2, len(mfs)):
         resort_mfs.append(mfs[j])
     resort_mfs.append(final_mf)
 
     return subfolders, resort_mfs, rcs, ens, dEs
 
 
+@logger.catch
 def plot_barrier_old(
     datafile: str = "neb.h5",
-    directory: str = None,
-    ri: float = None,
-    rf: float = None,
-    ei: float = None,
-    ef: float = None,
+    directory: Optional[str] = None,
+    ri: Optional[float] = None,
+    rf: Optional[float] = None,
+    ei: Optional[float] = None,
+    ef: Optional[float] = None,
     method: str = "PchipInterpolator",
     figname: str = "neb_barrier.png",
     show: bool = True,
-    raw=False,
+    raw: bool = False,
     **kwargs,
 ):
     r"""与plot_barrier()唯一的区别在于反应坐标视为累加值，而不是单个值"""
+    import os
+    from json import load
+
+    import numpy as np
+
     if directory is not None:
         # read data
         subfolders, resort_mfs, rcs, ens, dEs = _getef(os.path.abspath(directory))
 
     elif datafile:
         from dspawpy.io.utils import get_absfile
 
@@ -1615,22 +1742,25 @@
                 reaction_coordinate = neb["/BarrierInfo/ReactionCoordinate"]
                 energy = neb["/BarrierInfo/TotalEnergy"]
             else:  # old version
                 reaction_coordinate = neb["/Distance/ReactionCoordinate"]
                 energy = neb["/Energy/TotalEnergy"]
         elif absfile.endswith(".json"):
             with open(absfile, "r") as fin:
-                neb = json.load(fin)
+                neb = load(fin)
             if "BarrierInfo" in neb.keys():
                 reaction_coordinate = neb["BarrierInfo"]["ReactionCoordinate"]
                 energy = neb["BarrierInfo"]["TotalEnergy"]
             else:  # old version
                 reaction_coordinate = neb["Distance"]["ReactionCoordinate"]
                 energy = neb["Energy"]["TotalEnergy"]
 
+        else:
+            raise ValueError("Only h5 and json file are supported")
+
         x = []
         for c in reaction_coordinate:
             if len(x) > 0:  # add previous reaction coordinate
                 x.append(x[-1] + c)
             else:
                 x.append(c)
 
@@ -1665,20 +1795,28 @@
     except Exception:
         raise ValueError(f"Please check whether {kwargs} is valid for {method}！")
 
     xnew = np.linspace(rcs[0], rcs[-1], 100)
     ynew = inter_f(xnew)
 
     if raw:
-        import pandas as pd
+        try:
+            import polars as pl
 
-        pd.DataFrame({"x_raw": rcs, "y_raw": dEs}).to_csv("raw_xy.csv", index=False)
-        pd.DataFrame({"x_interpolated": xnew, "y_interpolated": ynew}).to_csv(
-            "raw_interpolated_xy.csv", index=False
-        )
+            pl.DataFrame({"x_raw": rcs, "y_raw": dEs}).write_csv("raw_xy.csv")
+            pl.DataFrame({"x_interpolated": xnew, "y_interpolated": ynew}).write_csv(
+                "raw_interpolated_xy.csv"
+            )
+        except ModuleNotFoundError:
+            import pandas as pd
+
+            pd.DataFrame({"x_raw": rcs, "y_raw": dEs}).to_csv("raw_xy.csv")
+            pd.DataFrame({"x_interpolated": xnew, "y_interpolated": ynew}).to_csv(
+                "raw_interpolated_xy.csv"
+            )
 
     # plot
     import matplotlib.pyplot as plt  # noqa: E402
 
     if kwargs:
         plt.plot(xnew, ynew, label=method + str(kwargs))
     else:
```

### Comparing `dspawpy-1.2.2/dspawpy/diffusion/pathfinder.py` & `dspawpy-1.3.0/dspawpy/diffusion/pathfinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 import itertools
 import warnings
 
 import numpy as np
 
 
-# copy from pymatgen-analysis-diffusion https://github.com/materialsvirtuallab/pymatgen-analysis-diffusion
+# copied from pymatgen-analysis-diffusion https://github.com/materialsvirtuallab/pymatgen-analysis-diffusion
 class IDPPSolver:
     """
     A solver using image dependent pair potential (IDPP) algo to get an improved
     initial NEB path. For more details about this algo, please refer to
     Smidstrup et al., J. Chem. Phys. 140, 214106 (2014).
 
     """
```

### Comparing `dspawpy-1.2.2/dspawpy/io/read.py` & `dspawpy-1.3.0/dspawpy/io/read.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
-import json
-import os
-import re
-import warnings
+from loguru import logger
+from typing import Optional, TYPE_CHECKING, Sequence
 
-import numpy as np
+if TYPE_CHECKING:
+    from pymatgen.electronic_structure.bandstructure import BandStructureSymmLine
 
 
+@logger.catch
 def get_band_data(
     band_dir: str,
-    syst_dir: str = None,
-    efermi: float = None,
+    syst_dir: str = "",
+    efermi: Optional[float] = None,
     zero_to_efermi: bool = False,
-):
+) -> "BandStructureSymmLine":
     """读取h5或json文件中的能带数据，构建BandStructureSymmLine对象
 
     Parameters
     ----------
     band_dir : str
         - 能带文件路径，band.h5 / band.json 或包含band.h5 / band.json的文件夹
         - 注意，wannier.h5 也可以使用此函数读取，但band_dir不支持文件夹类型
@@ -68,25 +68,28 @@
                 kpoints,
                 eigenvals,
                 rEf,
                 labels_dict,
                 projections,
             ) = _get_band_data_h5(band, iwan=False, zero_to_efermi=zero_to_efermi)
         else:
-            print("BandInfo or WannBandInfo key not found in h5file!")
-            return
+            raise KeyError("BandInfo or WannBandInfo key not found in h5file!")
     elif absfile.endswith(".json"):
         with open(absfile, "r") as fin:
-            band = json.load(fin)
+            from json import load
+
+            band = load(fin)
         if "WannBandInfo" in band.keys():
             assert (
                 syst_dir is not None
             ), "system.json is required for processing wannier band info!"
             with open(syst_dir) as system_json:
-                syst = json.load(system_json)
+                from json import load
+
+                syst = load(system_json)
             (
                 structure,
                 kpoints,
                 eigenvals,
                 rEf,
                 labels_dict,
                 projections,
@@ -125,15 +128,16 @@
         efermi=rEf,
         labels_dict=labels_dict,
         structure=structure,
         projections=projections,
     )
 
 
-def get_dos_data(dos_dir: str, return_dos=False):
+@logger.catch
+def get_dos_data(dos_dir: str, return_dos: bool = False):
     """读取h5或json文件中的态密度数据，构建CompleteDos或DOS对象
 
     Parameters
     ----------
     dos_dir : str
         态密度文件路径，dos.h5 / dos.json 或包含dos.h5 / dos.json的文件夹
     return_dos : bool, optional
@@ -149,37 +153,35 @@
     >>> dos = get_dos_data(dos_dir='dspawpy_proj/dspawpy_tests/inputs/2.5/dos.h5')
     """
     from dspawpy.io.utils import get_absfile
 
     absfile = get_absfile(dos_dir, task="dos")
     if absfile.endswith(".h5"):
         dos = load_h5(absfile)
-        if return_dos:
-            if dos["/DosInfo/Project"][0]:
-                return _get_complete_dos(dos)
-            else:
-                return _get_total_dos(dos)
+        if return_dos and not dos["/DosInfo/Project"][0]:
+            return _get_total_dos(dos)
         else:
             return _get_complete_dos(dos)
 
     elif absfile.endswith(".json"):
         with open(absfile, "r") as fin:
-            dos = json.load(fin)
-        if return_dos:
-            if dos["DosInfo"]["Project"]:
-                return _get_complete_dos_json(dos)
-            else:
-                return _get_total_dos_json(dos)
-        return _get_complete_dos_json(dos)
+            from json import load
+
+            dos = load(fin)
+        if return_dos and not dos["DosInfo"]["Project"]:
+            return _get_total_dos_json(dos)
+        else:
+            return _get_complete_dos_json(dos)
 
     else:
         raise TypeError(f"{absfile} must be h5 or json file!")
 
 
-def get_ele_from_h5(hpath: str = "aimd.h5"):
+@logger.catch
+def get_ele_from_h5(hpath: str = "aimd.h5") -> list:
     """从h5文件中读取元素列表；
     多离子步并不会在每个离子步的Structure中保存元素信息，只能读取初始结构的元素信息
 
     Parameters
     ----------
     hpath : str
         h5文件路径
@@ -192,51 +194,61 @@
     Examples
     --------
     >>> from dspawpy.io.read import get_ele_from_h5
     >>> ele = get_ele_from_h5(hpath='dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5')
     >>> ele
     ['H', 'H_1', 'O']
     """
+    import os
+
     absh5 = os.path.abspath(hpath)
     from h5py import File
 
     data = File(absh5)
+    import numpy as np
+
     Elements_bytes = np.array(data.get("/AtomInfo/Elements"))
     tempdata = np.array([i.decode() for i in Elements_bytes])
     ele = "".join(tempdata).split(";")
 
     return ele
 
 
-def get_lines_without_comment(filename: str, comment: str = "#"):
+@logger.catch
+def get_lines_without_comment(filename: str, comment: str = "#") -> list:
     """读取as文件内容，移除批注后返回行列表
 
     Examples
     --------
     >>> from dspawpy.io.read import get_lines_without_comment
     >>> lines = get_lines_without_comment(filename='dspawpy_proj/dspawpy_tests/inputs/2.15/01/structure01.as', comment='#')
     >>> lines
     ['Total number of atoms', '13', 'Lattice', '5.60580000 0.00000000 0.00000000', '0.00000000 5.60580000 0.00000000', '0.00000000 0.00000000 16.81740000', 'Cartesian', 'H 2.48700709 3.85367720 6.93461994', 'Pt 1.40145000 1.40145000 1.98192999', 'Pt 4.20434996 1.40145000 1.98192999', 'Pt 1.40145000 4.20434996 1.98192999', 'Pt 4.20434996 4.20434996 1.98192999', 'Pt 0.00843706 0.00042409 3.91500875', 'Pt 0.00881029 2.80247953 3.91551673', 'Pt 2.81216310 -0.00105882 3.91807627', 'Pt 2.81156629 2.80392163 3.91572506', 'Pt 1.41398585 1.39603492 5.85554462', 'Pt 4.22886663 1.39820574 5.84677553', 'Pt 1.40485707 4.20963461 5.89521929', 'Pt 4.23788559 4.20753128 5.88625580']
     """
     lines = []
+    import os
+
     absfile = os.path.abspath(filename)
+    import re
+
     with open(absfile) as file:
         while True:
             line = file.readline()
             if line:
                 line = re.sub(comment + r".*$", "", line)  # remove comment
                 line = line.strip()
                 if line:
                     lines.append(line)
             else:
                 break
 
     return lines
 
 
+@logger.catch
 def get_phonon_band_data(phonon_band_dir: str):
     """读取h5或json文件中的声子能带数据，构建PhononBandStructureSymmLine对象
 
     Parameters
     ----------
     phonon_band_dir : str
         能带文件路径，phonon.h5 / phonon.json 或包含这两个文件的文件夹
@@ -255,50 +267,53 @@
     absfile = get_absfile(phonon_band_dir, task="phonon")
 
     if absfile.endswith(".h5"):
         band = load_h5(absfile)
         (
             symmmetry_kpoints,
             symmetry_kPoints_index,
-            kpoints,
+            qpoints,
             structure,
             frequencies,
         ) = _get_phonon_band_data_h5(band)
     elif absfile.endswith(".json"):
         with open(absfile, "r") as fin:
-            band = json.load(fin)
+            from json import load
+
+            band = load(fin)
         (
             symmmetry_kpoints,
             symmetry_kPoints_index,
-            kpoints,
+            qpoints,
             structure,
             frequencies,
         ) = _get_phonon_band_data_json(band)
     else:
         raise TypeError(f"{absfile} must be h5 or json file")
 
     labels_dict = {}
     for i, s in enumerate(symmmetry_kpoints):
-        labels_dict[s] = kpoints[symmetry_kPoints_index[i] - 1]
+        labels_dict[s] = qpoints[symmetry_kPoints_index[i] - 1]
     from pymatgen.core.lattice import Lattice
 
     lattice_new = Lattice(structure.lattice.reciprocal_lattice.matrix)
 
     from pymatgen.phonon.bandstructure import PhononBandStructureSymmLine
 
     return PhononBandStructureSymmLine(
-        qpoints=kpoints,
+        qpoints=qpoints,  # type: ignore
         frequencies=frequencies,
         lattice=lattice_new,
         has_nac=False,
         labels_dict=labels_dict,
         structure=structure,
     )
 
 
+@logger.catch
 def get_phonon_dos_data(phonon_dos_dir: str):
     """读取h5或json文件中的声子态密度数据，构建PhononDos对象
 
     Parameters
     ----------
     phonon_dos_dir : str
         声子态密度文件路径，phonon_dos.h5 / phonon_dos.json 或包含这两个文件的文件夹
@@ -333,30 +348,33 @@
            19.8, 19.9, 20. ])
     """
     from dspawpy.io.utils import get_absfile
 
     absfile = get_absfile(phonon_dos_dir, task="phonon_dos")
     if absfile.endswith(".h5"):
         dos = load_h5(absfile)
-        frequencies = np.asarray(dos["/DosInfo/DosEnergy"])
+        frequencies = dos["/DosInfo/DosEnergy"]
         densities = dos["/DosInfo/Spin1/Dos"]
     elif absfile.endswith(".json"):
         with open(absfile, "r") as fin:
-            dos = json.load(fin)
-        frequencies = np.asarray(dos["DosInfo"]["DosEnergy"])
+            from json import load
+
+            dos = load(fin)
+        frequencies = dos["DosInfo"]["DosEnergy"]
         densities = dos["DosInfo"]["Spin1"]["Dos"]
     else:
         raise TypeError(f"{absfile} must be h5 or json file")
 
     from pymatgen.phonon.dos import PhononDos
 
     return PhononDos(frequencies, densities)
 
 
-def get_sinfo(datafile: str, scaled=False, si=None, ele=None, ai=None):
+@logger.catch
+def get_sinfo(datafile: str, scaled: bool = False, si=None, ele=None, ai=None):
     r"""从datafile中读取结构信息
 
     Parameters
     ----------
     datafile : str
         h5 / json 文件路径
     scaled : bool, optional
@@ -404,14 +422,17 @@
         ele is None or ai is None
     ), "Cannot select element and atomic number at the same time"
 
     from dspawpy.io.utils import get_absfile
 
     absfile = get_absfile(datafile, task="free")
     print(f"Reading {absfile}...")
+    import numpy as np
+
+    D_mag_fix = {}
     if absfile.endswith(".h5"):
         from h5py import File
 
         hf = File(absfile)  # 加载h5文件
 
         # decide task type by check the internal key
         if "/Structures" in hf.keys():  # multi-steps
@@ -487,31 +508,14 @@
                 pos = np.array(hf.get("/Structures/Step-" + str(ind) + "/Position"))
                 wrapped_pos = pos - np.floor(pos)  # wrap into [0,1)
                 wrapped_pos = (
                     wrapped_pos.flatten().reshape(-1, 3).T
                 )  # reshape to 3 x Natom
                 wrapped_poses[i] = wrapped_pos
 
-            iNoncollinear = False
-            try:  # 自旋计算
-                if "/MagInfo/TotalMagOnAtom" in hf.keys():  # collinear
-                    mag = np.array(hf.get("/MagInfo/TotalMagOnAtom"))  # Natom x 1
-                elif "/MagInfo/TotalMagOnAtomX" in hf.keys():  # noncollinear
-                    magx = np.array(hf.get("/MagInfo/TotalMagOnAtomX"))  # Natom x 1
-                    magy = np.array(hf.get("/MagInfo/TotalMagOnAtomY"))  # Natom x 1
-                    magz = np.array(hf.get("/MagInfo/TotalMagOnAtomZ"))  # Natom x 1
-                    iNoncollinear = True
-                else:
-                    mag = np.zeros(shape=(Natom, 1))
-
-            except Exception as e:
-                if str(e):  # ignore empty AssertionError()
-                    print(e)
-                mag = np.zeros(shape=(Natom, 1))
-
             if "/AtomInfo/Fix" in hf.keys():  # fix atom
                 atomFixs_raw = np.array(hf.get("/AtomInfo/Fix"))
                 atomFixs = np.array(
                     ["True" if _v else "False" for _v in atomFixs_raw]
                 ).reshape(-1, 3)
             else:
                 atomFixs = np.full(shape=(Natom, 3), fill_value="False")
@@ -525,233 +529,258 @@
                     9,
                 )  # (9,)
             except Exception as e:
                 if str(e):  # ignore empty AssertionError()
                     print(e)
                 latticeFixs = np.full(shape=(9,), fill_value="False")
 
-            # repeat atomFixs of shape Natom x 3 to Nstep x Natom x 3
-            atomFixs = np.repeat(atomFixs[np.newaxis, :], Nstep, axis=0).reshape(
-                Nstep, Natom, 3
-            )
-
-            # repeat latticeFixs of shape 9 x 1 to Nstep x Natom x 9
-            latticeFixs = (
-                np.repeat(latticeFixs[np.newaxis, :], Nstep * Natom, axis=0)
-                .reshape(Nstep, Natom, 9)
-                .tolist()
-            )
-
-            if iNoncollinear is False:
-                mags = np.repeat(mag[np.newaxis, :], Nstep, axis=0).tolist()
-                D_mag_fix = {
-                    "Mag": mags,
-                    "Fix_x": atomFixs[:, :, 0],
-                    "Fix_y": atomFixs[:, :, 1],
-                    "Fix_z": atomFixs[:, :, 2],
-                    "LatticeFixs": latticeFixs,
-                }
-            else:
-                D_mag_fix = {
-                    "Mag_x": np.repeat(magx[np.newaxis, :], Nstep, axis=0).tolist(),
-                    "Mag_y": np.repeat(magy[np.newaxis, :], Nstep, axis=0).tolist(),
-                    "Mag_z": np.repeat(magz[np.newaxis, :], Nstep, axis=0).tolist(),
-                    "Fix_x": atomFixs[:, :, 0],
-                    "Fix_y": atomFixs[:, :, 1],
-                    "Fix_z": atomFixs[:, :, 2],
-                    "LatticeFixs": latticeFixs,
-                }
-
-            if scaled:  # Fractional coordinates
-                for k, ind in enumerate(indices):  # 步数
-                    for j, sli in enumerate(location):  # atom si
-                        poses[k, j, :] = np.dot(wrapped_poses[k, :, sli], np.eye(3, 3))
-            else:  # Cartesian coordinates
-                for k, ind in enumerate(indices):  # 步数
-                    for j, sli in enumerate(location):
-                        poses[k, j, :] = np.dot(wrapped_poses[k, :, sli], lats)
-
-        elif "/RelaxedStructure" in hf.keys():  # 最新NEB链
-            N_images = hf.get("/RelaxedStructure").shape[0]  # Image00, Image01, ...
-            elements = np.empty(shape=(N_images,), dtype=np.float32)
-            lattices = np.empty(shape=(N_images, 3, 3), dtype=np.float32)
-            poses = np.empty(shape=(N_images, Natom, 3), dtype=np.float32)
-            atomFixs = np.empty(shape=(N_images, Natom, 3))
-            latticeFixs = np.empty(shape=(N_images, 9))
-            for i in range(N_images):
-                subfolder_name = "Image%02d" % i
-                _ele = np.array(hf.get(f"/RelaxedStructure/{subfolder_name}/Elements"))[
-                    0
-                ]
-                _lat = np.array(hf.get(f"/RelaxedStructure/{subfolder_name}/Lattice"))[
-                    0
-                ]
-                _pos = np.array(hf.get(f"/RelaxedStructure/{subfolder_name}/Position"))[
-                    0
-                ]
-                elements[i] = _ele
-                lattices[i] = _lat
-                poses[i] = _pos
-
-                try:  # fix atom
-                    atomFix_raw = np.array(
-                        hf.get(f"/RelaxedStructure/{subfolder_name}/Fix")
-                    )
-                    atomFix = np.array(
-                        ["True" if _v else "False" for _v in atomFix_raw]
-                    ).reshape(-1, 3)
-                except Exception:
-                    atomFix = np.full(shape=(Natom, 3), fill_value="False")
-                atomFixs[i] = atomFix
-
-                try:  # fix lattice
-                    latticeFix = (
-                        np.array(
-                            hf.get(f"/RelaxedStructure/{subfolder_name}/FixLattice")
-                        )
-                        .astype(bool)
-                        .flatten()
-                    )
-                    assert latticeFix.shape == (9,)
-                    latticeFix = latticeFix.reshape(
-                        9,
-                    )  # (9,)
-                except Exception as e:
-                    if str(e):  # ignore empty AssertionError()
-                        print(e)
-                    latticeFix = np.full(shape=(9,), fill_value="False")
-                latticeFixs[i] = latticeFix
-
-            iNoncollinear = False
+            # iNoncollinear = False
             try:  # 自旋计算
                 if "/MagInfo/TotalMagOnAtom" in hf.keys():  # collinear
                     mag = np.array(hf.get("/MagInfo/TotalMagOnAtom"))  # Natom x 1
+                    mags = np.repeat(mag[np.newaxis, :], Nstep, axis=0).tolist()
+                    D_mag_fix = {
+                        "Mag": mags,
+                        "Fix_x": atomFixs[:, :, 0],
+                        "Fix_y": atomFixs[:, :, 1],
+                        "Fix_z": atomFixs[:, :, 2],
+                        "LatticeFixs": latticeFixs,
+                    }
                 elif "/MagInfo/TotalMagOnAtomX" in hf.keys():  # noncollinear
                     magx = np.array(hf.get("/MagInfo/TotalMagOnAtomX"))  # Natom x 1
                     magy = np.array(hf.get("/MagInfo/TotalMagOnAtomY"))  # Natom x 1
                     magz = np.array(hf.get("/MagInfo/TotalMagOnAtomZ"))  # Natom x 1
-                    iNoncollinear = True
+                    # iNoncollinear = True
+                    D_mag_fix = {
+                        "Mag_x": np.repeat(magx[np.newaxis, :], Nstep, axis=0).tolist(),
+                        "Mag_y": np.repeat(magy[np.newaxis, :], Nstep, axis=0).tolist(),
+                        "Mag_z": np.repeat(magz[np.newaxis, :], Nstep, axis=0).tolist(),
+                        "Fix_x": atomFixs[:, :, 0],
+                        "Fix_y": atomFixs[:, :, 1],
+                        "Fix_z": atomFixs[:, :, 2],
+                        "LatticeFixs": latticeFixs,
+                    }
                 else:
                     mag = np.zeros(shape=(Natom, 1))
+                    mags = np.repeat(mag[np.newaxis, :], Nstep, axis=0).tolist()
+                    D_mag_fix = {
+                        "Mag": mags,
+                        "Fix_x": atomFixs[:, :, 0],
+                        "Fix_y": atomFixs[:, :, 1],
+                        "Fix_z": atomFixs[:, :, 2],
+                        "LatticeFixs": latticeFixs,
+                    }
 
             except Exception as e:
                 if str(e):  # ignore empty AssertionError()
                     print(e)
                 mag = np.zeros(shape=(Natom, 1))
 
-            if iNoncollinear is False:
-                mags = np.repeat(mag[np.newaxis, :], Nstep, axis=0).tolist()
-                D_mag_fix = {
-                    "Mag": mags,
-                    "Fix_x": atomFixs[:, :, 0],
-                    "Fix_y": atomFixs[:, :, 1],
-                    "Fix_z": atomFixs[:, :, 2],
-                    "LatticeFixs": latticeFixs,
-                }
-            else:
-                D_mag_fix = {
-                    "Mag_x": np.repeat(magx[np.newaxis, :], Nstep, axis=0).tolist(),
-                    "Mag_y": np.repeat(magy[np.newaxis, :], Nstep, axis=0).tolist(),
-                    "Mag_z": np.repeat(magz[np.newaxis, :], Nstep, axis=0).tolist(),
-                    "Fix_x": atomFixs[:, :, 0],
-                    "Fix_y": atomFixs[:, :, 1],
-                    "Fix_z": atomFixs[:, :, 2],
-                    "LatticeFixs": latticeFixs,
-                }
-
-            if scaled:  # Fractional coordinates
-                for k, ind in enumerate(indices):  # 步数
-                    for j, sli in enumerate(location):  # atom si
-                        poses[k, j, :] = np.dot(poses[k, :, sli], np.eye(3, 3))
-            else:  # Cartesian coordinates
-                for k, ind in enumerate(indices):  # 步数
-                    for j, sli in enumerate(location):
-                        poses[k, j, :] = np.dot(poses[k, :, sli], lats)
-
-        elif "/UnitAtomInfo" in hf.keys():  # phonon 仅读取单胞信息
-            hfDict = load_h5(absfile)
-            s = _get_structure(hfDict, "/UnitAtomInfo")
-            elements = np.array(get_ele_from_h5(absfile), dtype=object)
-            Natom = len(elements)
-            poses = [s.cart_coords]
-            lattices = [s.lattice.matrix]
-            Nstep = 1
-
-            atomFixs = np.empty(shape=(N_images, Natom, 3))
-            atomFix = np.full(shape=(Natom, 3), fill_value="False")
-            atomFixs[0] = atomFix
-            latticeFixs = np.empty(shape=(N_images, 9))
-            latticeFix = np.full(shape=(9,), fill_value="False")
-            latticeFixs[0] = latticeFix
-
-            iNoncollinear = False
-            try:  # 自旋计算
-                if "/MagInfo/TotalMagOnAtom" in hf.keys():  # collinear
-                    mag = np.array(hf.get("/MagInfo/TotalMagOnAtom"))  # Natom x 1
-                elif "/MagInfo/TotalMagOnAtomX" in hf.keys():  # noncollinear
-                    magx = np.array(hf.get("/MagInfo/TotalMagOnAtomX"))  # Natom x 1
-                    magy = np.array(hf.get("/MagInfo/TotalMagOnAtomY"))  # Natom x 1
-                    magz = np.array(hf.get("/MagInfo/TotalMagOnAtomZ"))  # Natom x 1
-                    iNoncollinear = True
-                else:
-                    mag = np.zeros(shape=(Natom, 1))
-
-            except Exception as e:
-                if str(e):  # ignore empty AssertionError()
-                    print(e)
-                mag = np.zeros(shape=(Natom, 1))
+            # repeat atomFixs of shape Natom x 3 to Nstep x Natom x 3
+            atomFixs = np.repeat(atomFixs[np.newaxis, :], Nstep, axis=0).reshape(
+                Nstep, Natom, 3
+            )
 
-            if iNoncollinear is False:
-                mags = np.repeat(mag[np.newaxis, :], Nstep, axis=0).tolist()
-                D_mag_fix = {
-                    "Mag": mags,
-                    "Fix_x": atomFixs[:, :, 0],
-                    "Fix_y": atomFixs[:, :, 1],
-                    "Fix_z": atomFixs[:, :, 2],
-                    "LatticeFixs": latticeFixs,
-                }
-            else:
-                D_mag_fix = {
-                    "Mag_x": np.repeat(magx[np.newaxis, :], Nstep, axis=0).tolist(),
-                    "Mag_y": np.repeat(magy[np.newaxis, :], Nstep, axis=0).tolist(),
-                    "Mag_z": np.repeat(magz[np.newaxis, :], Nstep, axis=0).tolist(),
-                    "Fix_x": atomFixs[:, :, 0],
-                    "Fix_y": atomFixs[:, :, 1],
-                    "Fix_z": atomFixs[:, :, 2],
-                    "LatticeFixs": latticeFixs,
-                }
+            # repeat latticeFixs of shape 9 x 1 to Nstep x Natom x 9
+            latticeFixs = (
+                np.repeat(latticeFixs[np.newaxis, :], Nstep * Natom, axis=0)
+                .reshape(Nstep, Natom, 9)
+                .tolist()
+            )
 
             if scaled:  # Fractional coordinates
                 for k, ind in enumerate(indices):  # 步数
                     for j, sli in enumerate(location):  # atom si
                         poses[k, j, :] = np.dot(wrapped_poses[k, :, sli], np.eye(3, 3))
             else:  # Cartesian coordinates
                 for k, ind in enumerate(indices):  # 步数
                     for j, sli in enumerate(location):
-                        poses[k, j, :] = np.dot(wrapped_poses[k, :, sli], lats)
+                        poses[k, j, :] = np.dot(wrapped_poses[k, :, sli], lattices[k])
+
+        elif "/RelaxedStructure" in hf.keys():  # 最新NEB链
+            raise NotImplementedError("neb.h5 is not supported yet")
+        #     N_images = np.array(hf.get("/RelaxedStructure")).shape[
+        #         0
+        #     ]  # Image00, Image01, ...
+        #     elements = np.empty(shape=(N_images,), dtype=np.float32)
+        #     Natom = len(elements)
+        #     lattices = np.empty(shape=(N_images, 3, 3), dtype=np.float32)
+        #     poses = np.empty(shape=(N_images, Natom, 3), dtype=np.float32)
+        #     atomFixs = np.empty(shape=(N_images, Natom, 3))
+        #     latticeFixs = np.empty(shape=(N_images, 9))
+        #     for i in range(N_images):
+        #         subfolder_name = "Image%02d" % i
+        #         _ele = np.array(hf.get(f"/RelaxedStructure/{subfolder_name}/Elements"))[
+        #             0
+        #         ]
+        #         _lat = np.array(hf.get(f"/RelaxedStructure/{subfolder_name}/Lattice"))[
+        #             0
+        #         ]
+        #         _pos = np.array(hf.get(f"/RelaxedStructure/{subfolder_name}/Position"))[
+        #             0
+        #         ]
+        #         elements[i] = _ele
+        #         lattices[i] = _lat
+        #         poses[i] = _pos
+        #
+        #         try:  # fix atom
+        #             atomFix_raw = np.array(
+        #                 hf.get(f"/RelaxedStructure/{subfolder_name}/Fix")
+        #             )
+        #             atomFix = np.array(
+        #                 ["True" if _v else "False" for _v in atomFix_raw]
+        #             ).reshape(-1, 3)
+        #         except Exception:
+        #             atomFix = np.full(shape=(Natom, 3), fill_value="False")
+        #         atomFixs[i] = atomFix
+        #
+        #         try:  # fix lattice
+        #             latticeFix = (
+        #                 np.array(
+        #                     hf.get(f"/RelaxedStructure/{subfolder_name}/FixLattice")
+        #                 )
+        #                 .astype(bool)
+        #                 .flatten()
+        #             )
+        #             assert latticeFix.shape == (9,)
+        #             latticeFix = latticeFix.reshape(
+        #                 9,
+        #             )  # (9,)
+        #         except Exception as e:
+        #             if str(e):  # ignore empty AssertionError()
+        #                 print(e)
+        #             latticeFix = np.full(shape=(9,), fill_value="False")
+        #         latticeFixs[i] = latticeFix
+        #
+        #     iNoncollinear = False
+        #     try:  # 自旋计算
+        #         if "/MagInfo/TotalMagOnAtom" in hf.keys():  # collinear
+        #             mag = np.array(hf.get("/MagInfo/TotalMagOnAtom"))  # Natom x 1
+        #             mags = np.repeat(mag[np.newaxis, :], Nstep, axis=0).tolist()
+        #             D_mag_fix = {
+        #                 "Mag": mags,
+        #                 "Fix_x": atomFixs[:, :, 0],
+        #                 "Fix_y": atomFixs[:, :, 1],
+        #                 "Fix_z": atomFixs[:, :, 2],
+        #                 "LatticeFixs": latticeFixs,
+        #             }
+        #         elif "/MagInfo/TotalMagOnAtomX" in hf.keys():  # noncollinear
+        #             magx = np.array(hf.get("/MagInfo/TotalMagOnAtomX"))  # Natom x 1
+        #             magy = np.array(hf.get("/MagInfo/TotalMagOnAtomY"))  # Natom x 1
+        #             magz = np.array(hf.get("/MagInfo/TotalMagOnAtomZ"))  # Natom x 1
+        #             iNoncollinear = True
+        #             D_mag_fix = {
+        #                 "Mag_x": np.repeat(magx[np.newaxis, :], Nstep, axis=0).tolist(),
+        #                 "Mag_y": np.repeat(magy[np.newaxis, :], Nstep, axis=0).tolist(),
+        #                 "Mag_z": np.repeat(magz[np.newaxis, :], Nstep, axis=0).tolist(),
+        #                 "Fix_x": atomFixs[:, :, 0],
+        #                 "Fix_y": atomFixs[:, :, 1],
+        #                 "Fix_z": atomFixs[:, :, 2],
+        #                 "LatticeFixs": latticeFixs,
+        #             }
+        #         else:
+        #             mag = np.zeros(shape=(Natom, 1))
+        #
+        #     except Exception as e:
+        #         if str(e):  # ignore empty AssertionError()
+        #             print(e)
+        #         mag = np.zeros(shape=(Natom, 1))
+        #
+        #     if scaled:  # Fractional coordinates
+        #         for k, ind in enumerate(indices):  # 步数
+        #             for j, sli in enumerate(location):  # atom si
+        #                 poses[k, j, :] = np.dot(poses[k, :, sli], np.eye(3, 3))
+        #     else:  # Cartesian coordinates
+        #         for k, ind in enumerate(indices):  # 步数
+        #             for j, sli in enumerate(location):
+        #                 poses[k, j, :] = np.dot(poses[k, :, sli], lats)
+        #
+        elif "/UnitAtomInfo" in hf.keys():  # phonon 仅读取单胞信息
+            raise NotImplementedError("phonon.h5 is not supported yet")
+            # hfDict = load_h5(absfile)
+            # s = _get_structure(hfDict, "/UnitAtomInfo")
+            # elements = np.array(get_ele_from_h5(absfile), dtype=object)
+            # Natom = len(elements)
+            # poses = [s.cart_coords]
+            # lattices = [s.lattice.matrix]
+            # Nstep = 1
+            #
+            # atomFixs = np.empty(shape=(Natom, 3))
+            # atomFix = np.full(shape=(Natom, 3), fill_value="False")
+            # atomFixs[0] = atomFix
+            # latticeFixs = np.empty(shape=(9,))
+            # latticeFix = np.full(shape=(9,), fill_value="False")
+            # latticeFixs[0] = latticeFix
+
+            # iNoncollinear = False
+            # try:  # 自旋计算
+            #     if "/MagInfo/TotalMagOnAtom" in hf.keys():  # collinear
+            #         mag = np.array(hf.get("/MagInfo/TotalMagOnAtom"))  # Natom x 1
+            #     elif "/MagInfo/TotalMagOnAtomX" in hf.keys():  # noncollinear
+            #         magx = np.array(hf.get("/MagInfo/TotalMagOnAtomX"))  # Natom x 1
+            #         magy = np.array(hf.get("/MagInfo/TotalMagOnAtomY"))  # Natom x 1
+            #         magz = np.array(hf.get("/MagInfo/TotalMagOnAtomZ"))  # Natom x 1
+            #         iNoncollinear = True
+            #     else:
+            #         mag = np.zeros(shape=(Natom, 1))
+            #
+            # except Exception as e:
+            #     if str(e):  # ignore empty AssertionError()
+            #         print(e)
+            #     mag = np.zeros(shape=(Natom, 1))
+            #
+            # if iNoncollinear is False:
+            #     mags = np.repeat(mag[np.newaxis, :], Nstep, axis=0).tolist()
+            #     D_mag_fix = {
+            #         "Mag": mags,
+            #         "Fix_x": atomFixs[:, :, 0],
+            #         "Fix_y": atomFixs[:, :, 1],
+            #         "Fix_z": atomFixs[:, :, 2],
+            #         "LatticeFixs": latticeFixs,
+            #     }
+            # else:
+            #     D_mag_fix = {
+            #         "Mag_x": np.repeat(magx[np.newaxis, :], Nstep, axis=0).tolist(),
+            #         "Mag_y": np.repeat(magy[np.newaxis, :], Nstep, axis=0).tolist(),
+            #         "Mag_z": np.repeat(magz[np.newaxis, :], Nstep, axis=0).tolist(),
+            #         "Fix_x": atomFixs[:, :, 0],
+            #         "Fix_y": atomFixs[:, :, 1],
+            #         "Fix_z": atomFixs[:, :, 2],
+            #         "LatticeFixs": latticeFixs,
+            #     }
+
+            # if scaled:  # Fractional coordinates
+            #     for j, sli in enumerate(location):  # atom si
+            #         poses[k, j, :] = np.dot(wrapped_poses[:, sli], np.eye(3, 3))
+            # else:  # Cartesian coordinates
+            #     for j, sli in enumerate(location):
+            #         poses[k, j, :] = np.dot(wrapped_poses[:, sli], lats)
 
         else:  # rho, potential, elf, pcharge
             hfDict = load_h5(absfile)
             s = _get_structure(hfDict, "/AtomInfo")
             elements = np.array(get_ele_from_h5(absfile), dtype=object)
             poses = [s.cart_coords]
             lattices = [s.lattice.matrix]
             Nstep = 1
             D_mag_fix = None
-            warnings.warn(
+
+            logger.warning(
                 "--> rho/potential/elf/pcharge.h5 has no mag or fix info,\nyou should manually set it before starting new calculations.."
             )
 
     elif absfile.endswith(".json"):
-        warnings.warn(
+        logger.warning(
             "float number in json has precision of 4 digits by default, which may cause inconsistency with h5/log file, you may use io.jsonPrec to adjust the precision",
             category=UserWarning,
         )
         with open(absfile, "r") as f:
-            data = json.load(f)  # 加载json文件
+            from json import load
+
+            data = load(f)  # 加载json文件
 
         # decide the task type by checking the internal keys
         if "AtomInfo" in data:  # single-step task
             s = _get_structure_json(data["AtomInfo"])
             elements = [str(i) for i in s.species]
             poses = [s.cart_coords]
             lattices = [s.lattice.matrix]
@@ -894,15 +923,15 @@
 
                     mags.append(mag_for_each_step)
                     Atomfixs.append(fix_for_each_step)
                     if not scaled:
                         poses[i] = np.dot(poses[i], lattices[i])
 
             else:  # relax, neb01
-                warnings.warn(
+                logger.warning(
                     "mag and fix info are not available for relax.json and nebXX.json yet, trying read info...",
                     category=UserWarning,
                 )
 
                 for i, ind in enumerate(indices):  # for every ionic step
                     lat = data[ind - 1]["Lattice"]
                     lattices[i] = np.array(lat).reshape(3, 3)
@@ -950,14 +979,15 @@
         raise ValueError(
             "get_sinfo function only accept datafile of .h5 / .json format!"
         )
 
     return Nstep, elements, poses, lattices, D_mag_fix
 
 
+@logger.catch
 def load_h5(dir_h5: str) -> dict:
     """遍历读取h5文件中的数据，保存为字典格式
 
     慎用此函数，因为会读取很多不需要的数据，耗时很长。
 
     Parameters
     ----------
@@ -973,46 +1003,54 @@
     --------
     >>> from dspawpy.io.read import load_h5
     >>> datas = load_h5(dir_h5='dspawpy_proj/dspawpy_tests/inputs/2.2/scf.h5')
     >>> datas.keys()
     dict_keys(['/AtomInfo/CoordinateType', '/AtomInfo/Elements', '/AtomInfo/Grid', '/AtomInfo/Lattice', '/AtomInfo/Position', '/Eigenvalue/CBM/BandIndex', '/Eigenvalue/CBM/Energy', '/Eigenvalue/CBM/Kpoint', '/Eigenvalue/NumberOfBand', '/Eigenvalue/Spin1/BandEnergies', '/Eigenvalue/Spin1/Kpoints/Coordinates', '/Eigenvalue/Spin1/Kpoints/Grid', '/Eigenvalue/Spin1/Kpoints/NumberOfKpoints', '/Eigenvalue/Spin1/Occupation', '/Eigenvalue/VBM/BandIndex', '/Eigenvalue/VBM/Energy', '/Eigenvalue/VBM/Kpoint', '/Electron', '/Energy/EFermi', '/Energy/TotalEnergy', '/Energy/TotalEnergy0', '/Force/ForceOnAtoms', '/Stress/Direction', '/Stress/Pressure', '/Stress/Stress', '/Stress/Total', '/Structures/FinalStep', '/Structures/Step-1/Lattice', '/Structures/Step-1/Position'])
     """
 
+    @logger.catch
     def get_names(key, h5_object):
         names.append(h5_object.name)
 
+    @logger.catch
     def is_dataset(name):
         for name_inTheList in names:
             if name_inTheList.find(name + "/") != -1:
                 return False
         return True
 
+    import numpy as np
+
+    @logger.catch
     def get_datas(key, h5_object):
         if is_dataset(h5_object.name):
             data = np.asarray(h5_object)
             if data.dtype == "|S1":  # 转成字符串 并根据";"分割
                 byte2str = [str(bi, "utf-8") for bi in data]
                 string = ""
                 for char in byte2str:
                     string += char
                 data = np.array([elem for elem in string.strip().split(";")])
             # "/group1/group2/.../groupN/dataset" : value
             datas[h5_object.name] = data.tolist()
 
     from h5py import File
 
+    import os
+
     with File(os.path.abspath(dir_h5), "r") as fin:
         names = []
         datas = {}
         fin.visititems(get_names)
         fin.visititems(get_datas)
 
         return datas
 
 
+@logger.catch
 def load_h5_todict(dir_h5: str) -> dict:
     """与上一个函数区别在于合并了部分同类数据，例如
 
     /Structures/Step-1/* 和 /Structures/Step-2/* 并入 /Structures/ 组内
     """
 
     def create_dict(L: list, D: dict):
@@ -1036,15 +1074,16 @@
     groups_value_dict = {}
     for data in groups_value_list:
         create_dict(data, groups_value_dict)
 
     return groups_value_dict
 
 
-def __parse_indices(index: str, maxIndex) -> list:
+@logger.catch
+def __parse_indices(index: str, maxIndex: int) -> list:
     """解析用户输入的原子、结构序号字符串
 
     输入：
         - index: 用户输入的原子序号/元素字符串，例如 '1:3,5,7:10'
         - maxIndex: 最大序号，例如 10
     输出：
         - indices: 解析后的原子序号列表，例如 [1,2,3,4,5,6,7,8,9,10]
@@ -1072,15 +1111,16 @@
             for i in range(low, high + 1):
                 indices.append(i)
         else:  # 单个数字
             indices.append(int(blc))
     return indices
 
 
-def _get_lammps_non_orthogonal_box(lat: np.ndarray):
+@logger.catch
+def _get_lammps_non_orthogonal_box(lat: Sequence):
     """计算用于输入lammps的盒子边界参数，用于生成dump结构文件
 
     Parameters
     ----------
     lat : np.ndarray
         常见的非三角3x3矩阵
 
@@ -1089,14 +1129,16 @@
     box_bounds:
         用于输入lammps的盒子边界
     """
     # https://docs.lammps.org/Howto_triclinic.html
     A = lat[0]
     B = lat[1]
     C = lat[2]
+    import numpy as np
+
     assert np.cross(A, B).dot(C) > 0, "Lat is not right handed"
 
     # 将常规3x3矩阵转成标准的上三角矩阵
     alpha = np.arccos(np.dot(B, C) / (np.linalg.norm(B) * np.linalg.norm(C)))
     beta = np.arccos(np.dot(A, C) / (np.linalg.norm(A) * np.linalg.norm(C)))
     gamma = np.arccos(np.dot(A, B) / (np.linalg.norm(A) * np.linalg.norm(B)))
 
@@ -1146,16 +1188,19 @@
             [zlo_bound, zhi_bound, yz],
         ]
     )
 
     return box_bounds
 
 
+@logger.catch
 def _get_total_dos(dos: dict):
     # h5 -> Dos Obj
+    import numpy as np
+
     energies = np.asarray(dos["/DosInfo/DosEnergy"])
     from pymatgen.electronic_structure.core import Spin
 
     if dos["/DosInfo/SpinType"][0] != "collinear":
         densities = {Spin.up: np.asarray(dos["/DosInfo/Spin1/Dos"])}
     else:
         densities = {
@@ -1166,16 +1211,19 @@
     efermi = dos["/DosInfo/EFermi"][0]
 
     from pymatgen.electronic_structure.dos import Dos
 
     return Dos(efermi, energies, densities)
 
 
+@logger.catch
 def _get_total_dos_json(dos: dict):
     # json -> Dos Obj
+    import numpy as np
+
     energies = np.asarray(dos["DosInfo"]["DosEnergy"])
     from pymatgen.electronic_structure.core import Spin
 
     if dos["DosInfo"]["SpinType"] != "collinear":
         densities = {Spin.up: np.asarray(dos["DosInfo"]["Spin1"]["Dos"])}
     else:
         densities = {
@@ -1184,31 +1232,30 @@
         }
     efermi = dos["DosInfo"]["EFermi"]
     from pymatgen.electronic_structure.dos import Dos
 
     return Dos(efermi, energies, densities)
 
 
+@logger.catch
 def _get_complete_dos(dos: dict):
     # h5 -> CompleteDos Obj
     total_dos = _get_total_dos(dos)
     structure = _get_structure(dos, "/AtomInfo")
     N = len(structure)
     pdos = [{} for i in range(N)]
     number_of_spin = 2 if dos["/DosInfo/SpinType"][0] == "collinear" else 1
 
-    if dos["/DosInfo/Project"][0] == 0:  # not project dos
-        pdoss = None
-    else:
-        from pymatgen.electronic_structure.core import Orbital
-        from pymatgen.electronic_structure.core import Spin
+    from pymatgen.electronic_structure.core import Orbital
+    from pymatgen.electronic_structure.core import Spin
 
-        for i in range(number_of_spin):
-            spin_key = "Spin" + str(i + 1)
-            spin = Spin.up if i == 0 else Spin.down
+    for i in range(number_of_spin):
+        spin_key = "Spin" + str(i + 1)
+        spin = Spin.up if i == 0 else Spin.down
+        if dos["/DosInfo/Project"][0]:
             atomindexs = dos["/DosInfo/" + spin_key + "/ProjectDos/AtomIndexs"][0]
             orbitindexs = dos["/DosInfo/" + spin_key + "/ProjectDos/OrbitIndexs"][0]
             for atom_index in range(atomindexs):
                 for orbit_index in range(orbitindexs):
                     orbit_name = Orbital(orbit_index)
                     Contribution = dos[
                         "/DosInfo/"
@@ -1219,86 +1266,102 @@
                         + str(orbit_index + 1)
                     ]
                     if orbit_name in pdos[atom_index].keys():
                         pdos[atom_index][orbit_name].update({spin: Contribution})
                     else:
                         pdos[atom_index][orbit_name] = {spin: Contribution}
 
-        pdoss = {structure[i]: pd for i, pd in enumerate(pdos)}
+            pdoss = {structure[i]: pd for i, pd in enumerate(pdos)}
+        else:
+            pdoss = {}
+
     from pymatgen.electronic_structure.dos import CompleteDos
 
-    return CompleteDos(structure, total_dos, pdoss)
+    return CompleteDos(structure, total_dos, pdoss)  # type: ignore
 
 
+@logger.catch
 def _get_complete_dos_json(dos: dict):
     # json -> CompleteDos Obj
     total_dos = _get_total_dos_json(dos)
     structure = _get_structure_json(dos["AtomInfo"])
     N = len(structure)
     pdos = [{} for i in range(N)]
     number_of_spin = 2 if dos["DosInfo"]["SpinType"] == "collinear" else 1
 
-    if dos["DosInfo"]["Project"] is False:  # not project dos
-        pdoss = None
-    else:
-        from pymatgen.electronic_structure.core import Orbital
-        from pymatgen.electronic_structure.core import Spin
+    from pymatgen.electronic_structure.core import Orbital
+    from pymatgen.electronic_structure.core import Spin
 
-        for i in range(number_of_spin):
-            spin_key = "Spin" + str(i + 1)
-            spin = Spin.up if i == 0 else Spin.down
+    for i in range(number_of_spin):
+        spin_key = "Spin" + str(i + 1)
+        spin = Spin.up if i == 0 else Spin.down
+        if dos["DosInfo"]["Project"]:
             project = dos["DosInfo"][spin_key]["ProjectDos"]
             for p in project:
                 atom_index = p["AtomIndex"] - 1
                 o = p["OrbitIndex"] - 1
                 orbit_name = Orbital(o)
                 if orbit_name in pdos[atom_index].keys():
                     pdos[atom_index][orbit_name].update({spin: p["Contribution"]})
                 else:
                     pdos[atom_index][orbit_name] = {spin: p["Contribution"]}
-        pdoss = {structure[i]: pd for i, pd in enumerate(pdos)}
+            pdoss = {structure[i]: pd for i, pd in enumerate(pdos)}
+        else:
+            pdoss = {}
+
     from pymatgen.electronic_structure.dos import CompleteDos
 
-    return CompleteDos(structure, total_dos, pdoss)
+    return CompleteDos(structure, total_dos, pdoss)  # type: ignore
 
 
+@logger.catch
 def _get_structure(hdf5: dict, key: str):
     """For single-step task"""
     # load_h5 -> Structure Obj
+    import numpy as np
+
     lattice = np.asarray(hdf5[key + "/Lattice"]).reshape(3, 3)
     elements = hdf5[key + "/Elements"]
     positions = hdf5[key + "/Position"]
     coords = np.asarray(positions).reshape(-1, 3)
     is_direct = hdf5[key + "/CoordinateType"][0] == "Direct"
+    import re
+
     elements = [re.sub(r"_", "", e) for e in elements]
 
     from pymatgen.core.structure import Structure
 
     return Structure(lattice, elements, coords, coords_are_cartesian=(not is_direct))
 
 
-def _get_structure_json(atominfo):
+@logger.catch
+def _get_structure_json(atominfo: dict):
     """For single-step task"""
+    import numpy as np
+
     lattice = np.asarray(atominfo["Lattice"]).reshape(3, 3)
     elements = []
     positions = []
     for atom in atominfo["Atoms"]:
         elements.append(atom["Element"])
         positions.extend(atom["Position"])
 
     coords = np.asarray(positions).reshape(-1, 3)
     is_direct = atominfo["CoordinateType"] == "Direct"
+    import re
+
     elements = [re.sub(r"_", "", e) for e in elements]
 
     from pymatgen.core.structure import Structure
 
     return Structure(lattice, elements, coords, coords_are_cartesian=(not is_direct))
 
 
-def _get_band_data_h5(band: dict, iwan=False, zero_to_efermi=False):
+@logger.catch
+def _get_band_data_h5(band: dict, iwan: bool = False, zero_to_efermi: bool = False):
     if iwan:
         bd = "WannBandInfo"
     else:
         bd = "BandInfo"
     number_of_band = band[f"/{bd}/NumberOfBand"][0]
     number_of_kpoints = band[f"/{bd}/NumberOfKpoints"][0]
     if band[f"/{bd}/SpinType"][0] != "collinear":
@@ -1307,26 +1370,26 @@
         number_of_spin = 2
 
     symmetry_kPoints_index = band[f"/{bd}/SymmetryKPointsIndex"]
 
     efermi = band[f"/{bd}/EFermi"][0]
     eigenvals = {}
     from pymatgen.electronic_structure.core import Spin
+    import numpy as np
 
     for i in range(number_of_spin):
         spin_key = "Spin" + str(i + 1)
         spin = Spin.up if i == 0 else Spin.down
 
         if f"/{bd}/" + spin_key + "/BandEnergies" in band:
             data = band[f"/{bd}/" + spin_key + "/BandEnergies"]
         elif f"/{bd}/" + spin_key + "/Band" in band:
             data = band[f"/{bd}/" + spin_key + "/Band"]
         else:
-            print("Band key error")
-            return
+            raise KeyError("Band key error")
         band_data = np.array(data).reshape((number_of_kpoints, number_of_band)).T
 
         if zero_to_efermi:
             eigenvals[spin] = band_data - efermi
         else:
             eigenvals[spin] = band_data
 
@@ -1375,64 +1438,70 @@
 
     if zero_to_efermi:
         efermi = 0  # set to 0
 
     return structure, kpoints, eigenvals, efermi, labels_dict, projections
 
 
+@logger.catch
 def _get_band_data_json(
-    band: dict, syst: dict = None, iwan=False, zero_to_efermi=False
+    band: dict,
+    syst: Optional[dict] = None,
+    iwan: bool = False,
+    zero_to_efermi: bool = False,
 ):
     # syst is only required for wannier band structure
     if iwan:
         bd = "WannBandInfo"
+        assert syst is not None, "syst is required for wannier band structure"
         structure = _get_structure_json(syst["AtomInfo"])
         efermi = syst["Energy"]["EFermi"]
     else:
         bd = "BandInfo"
         structure = _get_structure_json(band["AtomInfo"])
 
     number_of_band = band[bd]["NumberOfBand"]
     number_of_kpoints = band[bd]["NumberOfKpoints"]
-    if band[bd]['SpinType'][0] != 'collinear':
+    if band[bd]["SpinType"][0] != "collinear":
         number_of_spin = 1
     else:
         number_of_spin = 2
 
     symmetry_kPoints_index = band[bd]["SymmetryKPointsIndex"]
 
     if "EFermi" in band[bd]:
         efermi = band[bd]["EFermi"]
+    else:
+        logger.warning("EFermi not found in band data, set to 0")
+        efermi = 0
 
     eigenvals = {}
     from pymatgen.electronic_structure.core import Spin
+    import numpy as np
 
     for i in range(number_of_spin):
         spin_key = "Spin" + str(i + 1)
         spin = Spin.up if i == 0 else Spin.down
 
         if "BandEnergies" in band[bd][spin_key]:
             data = band[bd][spin_key]["BandEnergies"]
         elif "Band" in band[bd][spin_key]:
             data = band[bd][spin_key]["Band"]
         else:
-            print("Band key error")
-            return
+            raise KeyError("Band key error")
 
         band_data = np.array(data).reshape((number_of_kpoints, number_of_band)).T
 
         if zero_to_efermi:
             eigenvals[spin] = band_data - efermi
 
         else:
             eigenvals[spin] = band_data
 
-    kpoints = np.asarray(band[bd]["CoordinatesOfKPoints"]).reshape(
-        number_of_kpoints, 3
-    )
+    kpoints = np.asarray(band[bd]["CoordinatesOfKPoints"]).reshape(number_of_kpoints, 3)
 
     labels_dict = {}
 
     for i, s in enumerate(band[bd]["SymmetryKPoints"]):
         labels_dict[s] = kpoints[symmetry_kPoints_index[i] - 1]
 
     # read projection data
@@ -1463,82 +1532,78 @@
 
     if zero_to_efermi:
         efermi = 0  # set to 0
 
     return structure, kpoints, eigenvals, efermi, labels_dict, projections
 
 
+@logger.catch
 def _get_phonon_band_data_h5(band: dict):
-    number_of_band = band["/BandInfo/NumberOfBand"][0]
-    number_of_kpoints = band["/BandInfo/NumberOfQPoints"][0]
-    number_of_spin = 1
-    symmmetry_kpoints = band["/BandInfo/SymmetryQPoints"]
-    symmetry_kPoints_index = band["/BandInfo/SymmetryQPointsIndex"]
-    eigenvals = {}
-    from pymatgen.electronic_structure.core import Spin
+    import numpy as np
 
-    for i in range(number_of_spin):
-        spin_key = "Spin" + str(i + 1)
-        spin = Spin.up if i == 0 else Spin.down
-        if "/BandInfo/" + spin_key + "/BandEnergies" in band:
-            data = band["/BandInfo/" + spin_key + "/BandEnergies"]
-        elif "/BandInfo/" + spin_key + "/Band" in band:
-            data = band["/BandInfo/" + spin_key + "/Band"]
-        else:
-            print("Band key error")
-            return
-        frequencies = np.array(data).reshape((number_of_kpoints, number_of_band)).T
-        eigenvals[spin] = frequencies
-    kpoints = np.asarray(band["/BandInfo/CoordinatesOfQPoints"]).reshape(
-        number_of_kpoints, 3
+    number_of_band = band["/BandInfo/NumberOfBand"][0]
+    number_of_qpoints = band["/BandInfo/NumberOfQPoints"][0]
+    symmmetry_qpoints = band["/BandInfo/SymmetryQPoints"]
+    symmetry_qPoints_index = band["/BandInfo/SymmetryQPointsIndex"]
+    qpoints = np.asarray(band["/BandInfo/CoordinatesOfQPoints"]).reshape(
+        number_of_qpoints, 3
     )
     if "/SupercellAtomInfo/CoordinateType" in band.keys():
         structure = _get_structure(band, "/SupercellAtomInfo")
     else:
         structure = _get_structure(band, "/AtomInfo")
-    return symmmetry_kpoints, symmetry_kPoints_index, kpoints, structure, frequencies
 
+    spin_key = "Spin1"
+    if "/BandInfo/" + spin_key + "/BandEnergies" in band:
+        data = band["/BandInfo/" + spin_key + "/BandEnergies"]
+    elif "/BandInfo/" + spin_key + "/Band" in band:
+        data = band["/BandInfo/" + spin_key + "/Band"]
+    else:
+        raise KeyError("Band key error")
+    frequencies = np.array(data).reshape((number_of_qpoints, number_of_band)).T
 
-def _get_phonon_band_data_json(band: dict):
-    number_of_band = band["BandInfo"]["NumberOfBand"]
-    number_of_kpoints = band["BandInfo"]["NumberOfQPoints"]
-    number_of_spin = 1
-    symmmetry_kpoints = band["BandInfo"]["SymmetryQPoints"]
-    symmetry_kPoints_index = band["BandInfo"]["SymmetryQPointsIndex"]
+    return symmmetry_qpoints, symmetry_qPoints_index, qpoints, structure, frequencies
 
-    eigenvals = {}
-    from pymatgen.electronic_structure.core import Spin
 
-    for i in range(number_of_spin):
-        spin_key = "Spin" + str(i + 1)
-        spin = Spin.up if i == 0 else Spin.down
-        if "BandEnergies" in band["BandInfo"][spin_key]:
-            data = band["BandInfo"][spin_key]["BandEnergies"]
-        elif "Band" in band["BandInfo"][spin_key]:
-            data = band["BandInfo"][spin_key]["Band"]
-        else:
-            print("Band key error")
-            return
-        frequencies = np.array(data).reshape((number_of_kpoints, number_of_band)).T
-        eigenvals[spin] = frequencies
+@logger.catch
+def _get_phonon_band_data_json(band: dict):
+    import numpy as np
 
-    kpoints = np.asarray(band["BandInfo"]["CoordinatesOfQPoints"]).reshape(
-        number_of_kpoints, 3
-    )
+    number_of_band = band["BandInfo"]["NumberOfBand"]
+    number_of_qpoints = band["BandInfo"]["NumberOfQPoints"]
 
+    symmmetry_qpoints = band["BandInfo"]["SymmetryQPoints"]
+    symmetry_qPoints_index = band["BandInfo"]["SymmetryQPointsIndex"]
+    qpoints = np.asarray(band["BandInfo"]["CoordinatesOfQPoints"]).reshape(
+        number_of_qpoints, 3
+    )
     if "SupercellAtomInfo" in band.keys():
         structure = _get_structure_json(band["SupercellAtomInfo"])
     else:
         structure = _get_structure_json(band["AtomInfo"])
 
-    return symmmetry_kpoints, symmetry_kPoints_index, kpoints, structure, frequencies
+    spin_key = "Spin1"
+    if "BandEnergies" in band["BandInfo"][spin_key]:
+        data = band["BandInfo"][spin_key]["BandEnergies"]
+    elif "Band" in band["BandInfo"][spin_key]:
+        data = band["BandInfo"][spin_key]["Band"]
+    else:
+        raise KeyError("Band key error")
+    frequencies = np.array(data).reshape((number_of_qpoints, number_of_band)).T
+
+    return symmmetry_qpoints, symmetry_qPoints_index, qpoints, structure, frequencies
 
 
-def pel_from_as(spath: str, scaled=False):
+@logger.catch
+def pel_from_as(spath: str, scaled: bool = False):
     """backup here for compatibility"""
+    import numpy as np
+
+    import os
+
     absfile = os.path.abspath(spath)
     with open(absfile, "r") as f:
         lines = f.readlines()
         Natom = int(lines[1])  # 原子总数
         ele = [line.split()[0] for line in lines[7 : 7 + Natom]]  # 元素列表
 
         # 晶格矢量
@@ -1559,15 +1624,18 @@
             pos = spos
         else:
             pos = np.dot(spos, latv)
 
     return pos, ele, latv
 
 
-def _remove_extra_kpoint(band_data, symmetry_kPoints_index, number_of_band):
+@logger.catch
+def _remove_extra_kpoint(
+    band_data: dict, symmetry_kPoints_index: Sequence, number_of_band: int
+):
     keep_data = []
     for i in range(len(symmetry_kPoints_index) - 1):
         if i == 0:
             start_index = symmetry_kPoints_index[i] - 1
             end_index = symmetry_kPoints_index[i + 1]
         else:
             start_index = symmetry_kPoints_index[i] + 1
```

### Comparing `dspawpy-1.2.2/dspawpy/io/structure.py` & `dspawpy-1.3.0/dspawpy/io/structure.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # -*- coding: utf-8 -*-
-import os
-import re
-import warnings
-from typing import List, Union
-
+from loguru import logger
+from typing import List, Union, Optional
 from dspawpy.io.utils import reader
 
 
+@logger.catch
 def build_Structures_from_datafile(
     datafile: Union[str, List[str]], si=None, ele=None, ai=None, fmt=None, task="scf"
 ):
     """Deprecated alias to read"""
-    warnings.warn(
+    logger.warning(
         "build_Structures_from_datafile is deprecated; use read instead",
         DeprecationWarning,
     )
     return read(datafile, si=si, ele=ele, ai=ai, fmt=fmt, task=task)
 
 
+@logger.catch
 def _get_structure_list(df: str, si=None, ele=None, ai=None, fmt=None, task="scf"):
     """get pymatgen structures from single datafile
 
     Parameters
     ----------
     df : str
         数据文件路径或包含数据文件的文件夹路径
@@ -29,14 +28,16 @@
     Returns
     -------
     List[Structure] : list of pymatgen structures
     """
     if task is None:
         task = "scf"
 
+    import os
+
     if os.path.isdir(df) or df.endswith(".h5") or df.endswith(".json"):
         from dspawpy.io.utils import get_absfile
 
         absfile = get_absfile(df, task=task)
     else:  # for other type of datafile, such as .as, .hzw, POSCAR
         absfile = os.path.abspath(df)
 
@@ -44,25 +45,27 @@
         fmt = absfile.split(".")[-1]
     else:
         assert isinstance(fmt, str), "fmt must be str"
 
     if fmt == "as":
         strs = [_from_dspaw_as(absfile)]
     elif fmt == "hzw":
-        warnings.warn("build from .hzw may lack mag & fix info!", category=UserWarning)
+        logger.warning("build from .hzw may lack mag & fix info!", category=UserWarning)
         strs = [_from_hzw(absfile)]
     elif fmt == "pdb":
         strs = _from_pdb(absfile)
-    elif fmt == "h5" or fmt == "json":
+    elif fmt == "h5":
         from dspawpy.io.read import get_sinfo
 
         Nstep, elements, positions, lattices, D_mag_fix = get_sinfo(
             datafile=absfile, si=si, ele=ele, ai=ai
         )  # returned positions, not scaled-positions
         # remove _ from elements
+        import re
+
         elements = [re.sub(r"_", "", e) for e in elements]
 
         strs = []
         from pymatgen.core import Structure
 
         for i in range(Nstep):
             if D_mag_fix:
@@ -80,35 +83,77 @@
                     Structure(
                         lattices[i],
                         elements,
                         positions[i],
                         coords_are_cartesian=True,
                     )
                 )
+
+    elif fmt == "json":
+        try:
+            from dspawpy.io.read import get_sinfo
+
+            Nstep, elements, positions, lattices, D_mag_fix = get_sinfo(
+                datafile=absfile, si=si, ele=ele, ai=ai
+            )  # returned positions, not scaled-positions
+            # remove _ from elements
+            elements = [re.sub(r"_", "", e) for e in elements]
+
+            strs = []
+            from pymatgen.core import Structure
+
+            for i in range(Nstep):
+                if D_mag_fix:
+                    strs.append(
+                        Structure(
+                            lattices[i],
+                            elements,
+                            positions[i],
+                            coords_are_cartesian=True,
+                            site_properties={k: v[i] for k, v in D_mag_fix.items()},
+                        )
+                    )
+                else:
+                    strs.append(
+                        Structure(
+                            lattices[i],
+                            elements,
+                            positions[i],
+                            coords_are_cartesian=True,
+                        )
+                    )
+        except Exception:  # try parse json with pymatgen
+            from pymatgen.core import Structure
+
+            strs = [Structure.from_file(absfile)]
+
     else:
         from pymatgen.core import Structure
 
         strs = [Structure.from_file(absfile)]
 
     return strs
 
 
+@logger.catch
 def _from_dspaw_as(as_file: str = "structure.as"):
     """从DSPAW的as结构文件中读取结构信息
 
     Parameters
     ----------
     as_file : str
         DSPAW的as结构文件, 默认'structure.as'
 
     Returns
     -------
     Structure
         pymatgen的Structure对象
     """
+    import os
+
     absfile = os.path.abspath(as_file)
     from dspawpy.io.read import get_lines_without_comment
 
     lines = get_lines_without_comment(absfile, "#")
     N = int(lines[1])  # number of atoms
 
     # parse lattice info
@@ -199,18 +244,20 @@
                                 value[value.index(v)] = "True"
                             elif v.startswith("F"):
                                 value[value.index(v)] = "False"
             mag_fix_dict[item] = values
 
     if lat_fixs != []:
         # replicate lat_fixs to N atoms
-        mag_fix_dict["LatticeFixs"] = [lat_fixs for i in range(N)]
+        mag_fix_dict["LatticeFixs"] = [lat_fixs for _ in range(N)]
 
     coords = np.asarray(positions).reshape(-1, 3)
     # remove _ from elements
+    import re
+
     elements = [re.sub(r"_", "", e) for e in elements]
 
     from pymatgen.core import Structure
 
     if mag_fix_dict == {}:
         return Structure(
             lattice, elements, coords, coords_are_cartesian=(not is_direct)
@@ -221,27 +268,30 @@
             elements,
             coords,
             coords_are_cartesian=(not is_direct),
             site_properties=mag_fix_dict,
         )
 
 
+@logger.catch
 def _from_hzw(hzw_file):
     """从hzw结构文件中读取结构信息
 
     Parameters
     ----------
     hzw_file : str
         hzw结构文件，以 .hzw 结尾
 
     Returns
     -------
     Structure
         pymatgen的Structure对象
     """
+    import os
+
     absfile = os.path.abspath(hzw_file)
     from dspawpy.io.read import get_lines_without_comment
 
     lines = get_lines_without_comment(absfile, "%")
     number_of_probes = int(lines[0])
     if number_of_probes != 0:
         raise ValueError("dspaw only support 0 probes hzw file")
@@ -263,14 +313,15 @@
 
     coords = np.asarray(positions).reshape(-1, 3)
     from pymatgen.core import Structure
 
     return Structure(lattice, elements, coords, coords_are_cartesian=True)
 
 
+@logger.catch
 def _read_atom_line(line_full):
     """从PDB文件读取 原子名称、xyz坐标、元素符号
     PDB文件中ATOM部分的格式如下（不含磁矩、自由度信息）：
     HETATM    1  H14 ORTE    0       6.301   0.693   1.919  1.00  0.00        H
     固定标记 原子序号 原子名称 残基名称 残基序号 x y z 占有率 温度因子 元素符号
 
     剔除多余信息，仅保留
@@ -296,14 +347,15 @@
 
     else:
         raise ValueError("Only ATOM and HETATM supported")
 
     return name, coord, symbol
 
 
+@logger.catch
 @reader
 def _from_pdb(fileobj):
     """Read PDB files. Modified from ASE"""
     images = []  # 构型列表
     import numpy as np
 
     orig = np.identity(3)  # 原点
@@ -363,17 +415,18 @@
     if len(images) == 0:
         atoms = _build_atoms(cell, symbols, positions)
         images.append(atoms)
 
     return images
 
 
+@logger.catch
 def _build_atoms(cell, symbols, positions):
     if cell is None:
-        warnings.warn(
+        logger.warning(
             "No lattice info in PDB file! The lattice defaults to [[2xmax, 0, 0]; [0, 2ymax, 0]; [0, 0, 2zmax]])",
             category=UserWarning,
         )
         # cell = np.zeros(shape=(3, 3))
         import numpy as np
 
         max_xyz = np.max(positions, axis=0)
@@ -381,28 +434,19 @@
 
     from pymatgen.core import Structure
 
     atoms = Structure(
         lattice=cell, species=symbols, coords=positions, coords_are_cartesian=True
     )
 
-    # if cell is None:
-    #     warnings.warn('No lattice info in PDB file!', category=UserWarning)
-    #     atoms = Molecule(species=symbols,
-    #                     coords=positions)
-    # else:
-    #     atoms = Structure(lattice=cell,
-    #                     species=symbols,
-    #                     coords=positions,
-    #                     coords_are_cartesian=True)
-
     return atoms
 
 
-def read(datafile: str or list, si=None, ele=None, ai=None, fmt=None, task="scf"):
+@logger.catch
+def read(datafile: Union[str, list], si=None, ele=None, ai=None, fmt=None, task="scf"):
     r"""读取一/多个h5/json文件，返回pymatgen的Structures列表
 
     Parameters
     ----------
     datafile : str or list
         - h5/json/as/hzw/cif/poscar/cssr/xsf/mcsqs/prismatic/yaml/fleur-inpgen文件路径;
         - 若给定文件夹路径，可配合task参数读取内部的 {task}.h5/json 文件
@@ -481,18 +525,19 @@
     for df in dfs:
         structure_list = _get_structure_list(df, si, ele, ai, fmt, task)
         pymatgen_Structures.extend(structure_list)
 
     return pymatgen_Structures
 
 
+@logger.catch
 def write(
     structure,
     filename: str,
-    fmt: str = None,
+    fmt: Optional[str] = None,
     coords_are_cartesian: bool = True,
 ):
     r"""往结构文件中写入信息
 
     Parameters
     ----------
     structure : Structure
@@ -515,64 +560,39 @@
     Reading ...dspawpy_proj/dspawpy_tests/inputs/2.15/01/neb01.h5...
     >>> len(s)
     17
 
     将结构信息写入文件：
 
     >>> from dspawpy.io.structure import write
-    >>> write(s, filename='dspawpy_proj/dspawpy_tests/inputs/out/PtH.json', coords_are_cartesian=True) # doctest: +ELLIPSIS
-    ==> ...dspawpy_proj/dspawpy_tests/inputs/out/PtH.json
-    >>> write(s, filename='dspawpy_proj/dspawpy_tests/inputs/out/PtH.as', coords_are_cartesian=True) # doctest: +ELLIPSIS
-    ==> ...dspawpy_proj/dspawpy_tests/inputs/out/PtH.as
-    >>> write(s, filename='dspawpy_proj/dspawpy_tests/inputs/out/PtH.hzw', coords_are_cartesian=True) # doctest: +ELLIPSIS
-    ==> ...dspawpy_proj/dspawpy_tests/inputs/out/PtH.hzw
+    >>> write(s, filename='dspawpy_proj/dspawpy_tests/outputs/doctest/PtH.json', coords_are_cartesian=True) # doctest: +ELLIPSIS
+    ==> ...dspawpy_proj/dspawpy_tests/outputs/doctest/PtH.json
+    >>> write(s, filename='dspawpy_proj/dspawpy_tests/outputs/doctest/PtH.as', coords_are_cartesian=True) # doctest: +ELLIPSIS
+    ==> ...dspawpy_proj/dspawpy_tests/outputs/doctest/PtH.as
+    >>> write(s, filename='dspawpy_proj/dspawpy_tests/outputs/doctest/PtH.hzw', coords_are_cartesian=True) # doctest: +ELLIPSIS
+    ==> ...dspawpy_proj/dspawpy_tests/outputs/doctest/PtH.hzw
 
     pdb, xyz, dump 三种类型的文件，可以写入多个构型，形成“轨迹”。生成的 xyz 等轨迹文件可使用 OVITO 等可视化软件打开观察。
 
-    >>> write(s, filename='dspawpy_proj/dspawpy_tests/inputs/out/PtH.pdb', coords_are_cartesian=True) # doctest: +ELLIPSIS
-    ==> ...dspawpy_proj/dspawpy_tests/inputs/out/PtH.pdb
-    >>> write(s, filename='dspawpy_proj/dspawpy_tests/inputs/out/PtH.xyz', coords_are_cartesian=True) # doctest: +ELLIPSIS
-    ==> ...dspawpy_proj/dspawpy_tests/inputs/out/PtH.xyz
-    >>> write(s, filename='dspawpy_proj/dspawpy_tests/inputs/out/PtH.dump', coords_are_cartesian=True) # doctest: +ELLIPSIS
-    ==> ...dspawpy_proj/dspawpy_tests/inputs/out/PtH.dump
-
-    单结构信息推荐使用 as 格式存储，如果 Structure 中有磁矩或自由度信息，将会按最完整的格式统一写入，形如 Fix_x, Fix_y, Fix_z, Mag_x, Mag_y, Mag_z，自由度信息默认为 F，磁矩默认为 0.0。可视情况自行手动删除生成的 as 文件中的这些默认信息
-
-    >>> with open('dspawpy_proj/dspawpy_tests/inputs/out/PtH.as') as f:
-    ...     print(f.read())
-    ...
-    Total number of atoms
-    13
-    Lattice Fix_x Fix_y Fix_z
-     5.60580000 0.00000000 0.00000000 F F F
-     0.00000000 5.60580000 0.00000000 F F F
-     0.00000000 0.00000000 16.81740000 F F F
-    Cartesian Fix_x Fix_y Fix_z Mag
-    H 2.58985263 3.72755271 6.94246998 F F F 0.0
-    Pt 1.37942121 1.39655502 1.96304099 F F F 0.0
-    Pt 4.20055071 1.40326436 1.94681875 F F F 0.0
-    Pt 1.37462277 4.20932677 2.00221003 F F F 0.0
-    Pt 4.21197615 4.21324064 1.99578112 F F F 0.0
-    Pt 5.58740047 5.59517338 3.93274445 F F F 0.0
-    Pt 5.58633749 2.78068345 3.91301343 F F F 0.0
-    Pt 2.79076605 5.59305895 3.91208092 F F F 0.0
-    Pt 2.78904685 2.78501463 3.89610696 F F F 0.0
-    Pt 1.38102265 1.36691874 5.84326681 F F F 0.0
-    Pt 4.19057728 1.36788897 5.84877666 F F F 0.0
-    Pt 1.34667410 4.16198043 5.89298591 F F F 0.0
-    Pt 4.17046728 4.15729941 5.89874209 F F F 0.0
-    <BLANKLINE>
+    >>> write(s, filename='dspawpy_proj/dspawpy_tests/outputs/doctest/PtH.pdb', coords_are_cartesian=True) # doctest: +ELLIPSIS
+    ==> ...dspawpy_proj/dspawpy_tests/outputs/doctest/PtH.pdb
+    >>> write(s, filename='dspawpy_proj/dspawpy_tests/outputs/doctest/PtH.xyz', coords_are_cartesian=True) # doctest: +ELLIPSIS
+    ==> ...dspawpy_proj/dspawpy_tests/outputs/doctest/PtH.xyz
+    >>> write(s, filename='dspawpy_proj/dspawpy_tests/outputs/doctest/PtH.dump', coords_are_cartesian=True) # doctest: +ELLIPSIS
+    ==> ...dspawpy_proj/dspawpy_tests/outputs/doctest/PtH.dump
 
-    写成其他类型的结构文件，将忽略磁矩和自由度信息
+    单结构信息推荐使用 as 格式存储，如果 Structure 中有磁矩或自由度信息，将会按最完整的格式统一写入，形如 Fix_x, Fix_y, Fix_z, Mag_x, Mag_y, Mag_z，自由度信息默认为 F，磁矩默认为 0.0。可视情况自行手动删除生成的 as 文件中的这些默认信息。写成其他类型的结构文件，将忽略磁矩和自由度信息
     """
     from pymatgen.core import Structure
 
     if isinstance(structure, Structure):
         structure = [structure]
 
+    import os
+
     absfilename = os.path.abspath(filename)
     if fmt is None:
         fmt = absfilename.split(".")[-1]
 
     if fmt == "pdb":  # 可以是多个构型
         from .write import _to_pdb
 
@@ -607,35 +627,36 @@
         "xsf",
         "mcsqs",
         "yaml",
         "fleur-inpgen",
         "prismatic",
         "res",
     ]:
-        structure[-1].to(filename=absfilename, fmt=fmt)
+        structure[-1].to(filename=absfilename, fmt=fmt)  # type: ignore
 
     else:
         try:
             structure[-1].to(filename=absfilename)
         except Exception as e:
             raise NotImplementedError(
-                f"formats other that [pdb, xyz, dump, json, as, hzw] are handled by pymatgen, while it returns: {e}"
+                f"formats other than [pdb, xyz, dump, json, as, hzw] are handled by pymatgen, while it returns: {e}"
             )
 
 
+@logger.catch
 def convert(
     infile,
     si=None,
     ele=None,
     ai=None,
-    infmt=None,
-    task="scf",
-    outfile="temp.xyz",
-    outfmt=None,
-    coords_are_cartesian=True,
+    infmt: Optional[str] = None,
+    task: str = "scf",
+    outfile: str = "temp.xyz",
+    outfmt: Optional[str] = None,
+    coords_are_cartesian: bool = True,
 ):
     """从infile中读取结构信息，完成格式转化后写入outfile
 
     - 多构型 -> 单构型，仅写入最后一个离子步信息
     - 晶体结构 -> 分子结构，将丢失晶胞信息
     - 分子结构 -> 晶体结构，将添加一个2倍最大原子xyz坐标的晶胞
     - pdb 和 dump 格式可能存在浮点数精度损失
@@ -676,22 +697,22 @@
     coords_are_cartesian : bool
         - 是否写作笛卡尔坐标，默认为True；否则写成分数坐标形式
         - 此选项暂时仅对 as 和 json 格式有效
 
     Examples
     --------
     >>> from dspawpy.io.structure import convert
-    >>> convert('dspawpy_proj/dspawpy_tests/inputs/supplement/PtH.as', outfile='dspawpy_proj/dspawpy_tests/outputs/doctest_out/PtH.hzw') # doctest: +ELLIPSIS
+    >>> convert('dspawpy_proj/dspawpy_tests/inputs/supplement/PtH.as', outfile='dspawpy_proj/dspawpy_tests/outputs/doctest/PtH.hzw') # doctest: +ELLIPSIS
     ==> .../PtH.hzw
 
     格式转换批量测试
 
     >>> for readable in ['relax.h5', 'system.json', 'aimd.pdb', 'latestStructure.as', 'CuO.hzw', 'POSCAR']:
     ...     for writable in ['pdb', 'xyz', 'dump', 'as', 'hzw', 'POSCAR']:
-    ...         convert('dspawpy_proj/dspawpy_tests/inputs/supplement/stru/'+readable, outfile=f"dspawpy_proj/dspawpy_tests/outputs/doctest_out/{readable.split('.')[0]}.{writable}") # doctest: +ELLIPSIS
+    ...         convert('dspawpy_proj/dspawpy_tests/inputs/supplement/stru/'+readable, outfile=f"dspawpy_proj/dspawpy_tests/outputs/doctest/{readable.split('.')[0]}.{writable}") # doctest: +ELLIPSIS
     Reading ...dspawpy_proj/dspawpy_tests/inputs/supplement/stru/relax.h5...
     ==> .../relax.pdb
     Reading ...dspawpy_proj/dspawpy_tests/inputs/supplement/stru/relax.h5...
     ==> .../relax.xyz
     Reading ...dspawpy_proj/dspawpy_tests/inputs/supplement/stru/relax.h5...
     ==> .../relax.dump
     Reading ...dspawpy_proj/dspawpy_tests/inputs/supplement/stru/relax.h5...
```

### Comparing `dspawpy-1.2.2/dspawpy/io/write.py` & `dspawpy-1.3.0/dspawpy/io/write.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 # -*- coding: utf-8 -*-
-import json
-import os
-import time
-import warnings
-from typing import Optional, Tuple
+from loguru import logger
+from typing import Optional, List, Sequence
 
 Bohr = 0.52917721067  # Angstrom
 
 
+@logger.catch
 def _write_xyz_traj(
-    structures,
-    xyzfile="aimdTraj.xyz",
+    structures: list,
+    xyzfile: str = "aimdTraj.xyz",
 ):
     r"""保存xyz格式的轨迹文件
 
     Parameters
     ----------
     structures: list
         pymatgen的Structures列表
     xyzfile : str
         写入xyz格式的轨迹文件，默认为aimdTraj.xyz
     """
+    import os
+
     if not isinstance(structures, list):  # single Structure
         structures = [structures]
-    if xyzfile is not None:
-        absxyz = os.path.abspath(xyzfile)
+    absxyz = os.path.abspath(xyzfile)
     if os.path.isfile(absxyz):
-        warnings.warn(
-            f"{absxyz} already exists and will be overwritten!", category=UserWarning
+        logger.warning(
+            f"{absxyz} already exists and will be overwritten!",
+            category=UserWarning,
         )
     os.makedirs(os.path.dirname(absxyz), exist_ok=True)
     with open(absxyz, "w") as f:
         # Nstep
         for _, structure in enumerate(structures):
-            # 原子数不会变，就是不合并的元素总数
             eles = [s.species_string for s in structure.sites]
             f.write("%d\n" % len(eles))
             # lattice
             lm = structure.lattice.matrix
             f.write(
                 'Lattice="%f %f %f %f %f %f %f %f %f" Properties=species:S:1:pos:R:3 pbc="T T T"\n'
                 % (
@@ -58,33 +57,34 @@
                 f.write(
                     "%s %f %f %f\n" % (eles[j], poses[j, 0], poses[j, 1], poses[j, 2])
                 )
 
     print(f"==> {absxyz}")
 
 
+@logger.catch
 def _write_dump_traj(
-    structures,
-    dumpfile="aimdTraj.dump",
+    structures: list,
+    dumpfile: str = "aimdTraj.dump",
 ):
     r"""保存为lammps的dump格式的轨迹文件，暂时只支持正交晶胞
 
     Parameters
     ----------
     structures: list
         pymatgen的Structures列表
     dumpfile : str
         dump格式的轨迹文件名，默认为aimdTraj.dump
     """
+    import os
+
     if not isinstance(structures, list):  # single Structure
         structures = [structures]
-    if dumpfile is not None:
-        absdump = os.path.abspath(dumpfile)
-    if os.path.isfile(absdump):
-        warnings.warn(f"{absdump} already exists and will be overwritten!")
+    absdump = os.path.abspath(dumpfile)
+    logger.warning(f"{absdump} already exists and will be overwritten!")
     os.makedirs(os.path.dirname(absdump), exist_ok=True)
     from dspawpy.io.read import _get_lammps_non_orthogonal_box
 
     with open(absdump, "w") as f:
         for n, structure in enumerate(structures):
             lat = structure.lattice.matrix
             eles = [s.species_string for s in structure.sites]
@@ -119,85 +119,86 @@
                         poses[i, 2],
                         i + 1,
                     )
                 )
     print(f"==> {absdump}")
 
 
+@logger.catch
 def write_VESTA(
     in_filename: str,
     data_type: str,
     out_filename: str = "DS-PAW.cube",
     subtype: Optional[str] = None,
     format: str = "cube",
     compact: bool = False,
     inorm: bool = False,
-    gridsize: Optional[Tuple[int]] = None,
+    gridsize: Optional[Sequence[int]] = None,
 ):
     """从包含电子体系信息的json或h5文件中读取数据并写入VESTA格式的文件中
 
     Parameters
     ----------
     in_filename : str
         包含电子体系信息的json或h5文件路径
     data_type: str
         数据类型，支持 "rho", "potential", "elf", "pcharge", "rhoBound"
     out_filename : str
         输出文件路径, 默认 "DS-PAW.cube"
-    subtype : str
+    subtype : Optional[str]
         用于指定data_type的数据子类型，默认为None，将读取 potential 的 TotalElectrostaticPotential 数据
     format : str
         输出的数据格式，支持 "cube" 和 "vesta" （"vasp"），默认为 "cube"，大小写不敏感
     compact : bool
         每个格点的数据都换行，通过减少空格数量减小文件体积（不会影响VESTA软件的解析），默认为False
     inorm : bool
         是否归一化体积数据，使其总和为1，默认为False
-    gridsize: tuple
+    gridsize: Optional[Sequence[int]]
         重新定义的格点数，格式为 (ngx, ngy, ngz)，默认为None，即使用原始格点数
 
     Returns
     --------
     out_filename : file
         VESTA格式的文件
 
     Examples
     --------
     >>> from dspawpy.io.write import write_VESTA
-    >>> write_VESTA("dspawpy_proj/dspawpy_tests/inputs/2.2/rho.json", "rho", out_filename='dspawpy_proj/dspawpy_tests/inputs/doctest_out/rho.cube') # doctest: +ELLIPSIS
+    >>> write_VESTA("dspawpy_proj/dspawpy_tests/inputs/2.2/rho.json", "rho", out_filename='dspawpy_proj/dspawpy_tests/outputs/doctest/rho.cube') # doctest: +ELLIPSIS
     Reading ...dspawpy_proj/dspawpy_tests/inputs/2.2/rho.json...
-    ==> ...dspawpy_proj/dspawpy_tests/inputs/doctest_out/rho.cube
+    ==> ...dspawpy_proj/dspawpy_tests/outputs/doctest/rho.cube
 
     >>> from dspawpy.io.write import write_VESTA
     >>> write_VESTA(
     ...     in_filename="dspawpy_proj/dspawpy_tests/inputs/2.7/potential.h5",
     ...     data_type="potential",
-    ...     out_filename="dspawpy_proj/dspawpy_tests/inputs/doctest_out/my_potential.txt",
+    ...     out_filename="dspawpy_proj/dspawpy_tests/outputs/doctest/my_potential.txt",
     ...     subtype='TotalElectrostaticPotential', # or 'TotalLocalPotential'
     ...     format='txt',
     ...     gridsize=(50,50,50), # all integer, can be larger or less than the original gridsize
     ... ) # doctest: +ELLIPSIS
     Reading .../potential.h5...
     Interpolating volumetric data...
     volumetric data interpolated
     ==> .../my_potential.txt
 
-    >>> with open("dspawpy_proj/dspawpy_tests/inputs/doctest_out/my_potential.txt") as t:
+    >>> with open("dspawpy_proj/dspawpy_tests/outputs/doctest/my_potential.txt") as t:
     ...     contents = t.readlines()
     ...     for line in contents[:10]:
     ...         print(line.strip())
     # 2 atoms
     # 50 50 50 grid size
     # x y z value
     0.000 0.000 0.000      0.3279418
     0.055 0.055 0.000     -0.0740864
-    0.110 0.110 0.000     -0.8811763
-    0.165 0.165 0.000     -2.1283865
-    0.220 0.220 0.000     -4.0559145
-    0.275 0.275 0.000     -6.8291030
-    0.330 0.330 0.000    -10.1550909
+    0.110 0.110 0.000     -0.8811762
+    0.165 0.165 0.000     -2.1283864
+    0.220 0.220 0.000     -4.0559144
+    0.275 0.275 0.000     -6.8291031
+    0.330 0.330 0.000    -10.1550910
     """
     from dspawpy.io.structure import read
     from dspawpy.io.read import load_h5
 
     if in_filename.endswith(".h5"):
         data = load_h5(in_filename)
         structure = read(in_filename)[0]
@@ -209,33 +210,39 @@
                 subtype = "TotalElectrostaticPotential"
             vd = data[f"/Potential/{subtype}"]
         elif data_type == "elf":
             vd = data["/ELF/TotalELF"]
         elif data_type == "pcharge":
             vd = data["/Pcharge/1/TotalCharge"]
         else:
-            raise NotImplementedError("Only support rho/potential/elf/pcharge/rhoBound")
+            raise NotImplementedError(
+                f"{data_type}, {subtype}, Only support rho/potential/elf/pcharge/rhoBound"
+            )
 
     elif in_filename.endswith(".json"):
         with open(in_filename, "r") as fin:
-            data = json.load(fin)
+            from json import load
+
+            data = load(fin)
         structure = read(in_filename)[0]
         grid = data["AtomInfo"]["Grid"]  # get grid array
         if data_type == "rho" or data_type == "rhoBound":
             vd = data["Rho"]["TotalCharge"]
         elif data_type == "potential":
             if subtype is None:
                 subtype = "TotalElectrostaticPotential"
             vd = data["Potential"][subtype]
         elif data_type == "elf":
             vd = data["ELF"]["TotalELF"]
         elif data_type == "pcharge":
             vd = data["Pcharge"][0]["TotalCharge"]
         else:
-            raise NotImplementedError("Only support rho/potential/elf/pcharge/rhoBound")
+            raise NotImplementedError(
+                f"{data_type}, {subtype}, Only support rho/potential/elf/pcharge/rhoBound"
+            )
 
     else:
         raise NotImplementedError("Only support json/h5 format")
 
     _write_specific_format(
         structure,
         grid,
@@ -244,22 +251,23 @@
         gridsize,
         format=format,
         compact=compact,
         inorm=inorm,
     )
 
 
+@logger.catch
 def write_delta_rho_vesta(
-    total,
-    individuals,
-    output="delta_rho.cube",
-    format="cube",
-    compact=False,
-    inorm=False,
-    gridsize: tuple = None,
+    total: str,
+    individuals: List[str],
+    output: str = "delta_rho.cube",
+    format: str = "cube",
+    compact: bool = False,
+    inorm: bool = False,
+    gridsize: Optional[Sequence] = None,
 ):
     """电荷密度差分可视化
 
     DeviceStudio暂不支持大文件，临时写成可以用VESTA打开的格式
 
     Parameters
     ----------
@@ -284,81 +292,93 @@
         电荷差分（total-individual1-individual2-...）后的电荷密度文件，
 
     Examples
     --------
     >>> from dspawpy.io.write import write_delta_rho_vesta
     >>> write_delta_rho_vesta(total='dspawpy_proj/dspawpy_tests/inputs/supplement/AB.h5',
     ...     individuals=['dspawpy_proj/dspawpy_tests/inputs/supplement/A.h5', 'dspawpy_proj/dspawpy_tests/inputs/supplement/B.h5'],
-    ...     output='dspawpy_proj/dspawpy_tests/inputs/doctest_out/delta_rho.cube') # doctest: +ELLIPSIS
+    ...     output='dspawpy_proj/dspawpy_tests/outputs/doctest/delta_rho.cube') # doctest: +ELLIPSIS
     Reading ...dspawpy_proj/dspawpy_tests/inputs/supplement/AB.h5...
     Reading ...dspawpy_proj/dspawpy_tests/inputs/supplement/A.h5...
     Reading ...dspawpy_proj/dspawpy_tests/inputs/supplement/B.h5...
-    ==> ...dspawpy_proj/dspawpy_tests/inputs/doctest_out/delta_rho.cube
+    ==> ...dspawpy_proj/dspawpy_tests/outputs/doctest/delta_rho.cube
     """
     from dspawpy.io.structure import read
     from dspawpy.io.read import load_h5
+    import os
 
     abstotal = os.path.abspath(total)
     structure = read(abstotal)[0]
-    import numpy as np
 
     if abstotal.endswith(".h5"):
         dataAB = load_h5(abstotal)
-        rho = np.array(dataAB["/Rho/TotalCharge"])
+        rho = dataAB["/Rho/TotalCharge"]
         grid = dataAB["/AtomInfo/Grid"]
     elif abstotal.endswith(".json"):
         with open(abstotal, "r") as f1:
-            dataAB = json.load(f1)
-            rho = np.array(dataAB["Rho"]["TotalCharge"])
+            from json import load
+
+            dataAB = load(f1)
+            rho = dataAB["Rho"]["TotalCharge"]
             grid = dataAB["AtomInfo"]["Grid"]
 
     else:
         raise ValueError(f"file format must be either h5 or json: {abstotal}")
 
+    import numpy as np
+
     for individual in individuals:
         absindividual = os.path.abspath(individual)
         print(f"Reading {individual}...")
         if absindividual.endswith(".h5"):
             data_individual = load_h5(absindividual)
             rho_individual = np.array(data_individual["/Rho/TotalCharge"])
         elif absindividual.endswith(".json"):
             with open(absindividual, "r") as f2:
-                data_individual = json.load(f2)
+                from json import load
+
+                data_individual = load(f2)
                 rho_individual = np.array(data_individual["Rho"]["TotalCharge"])
         else:
             raise ValueError(f"file format must be either h5 or json: {absindividual}")
 
         rho -= rho_individual
 
-    volumetricData = np.array(rho)
     _write_specific_format(
         structure,
         grid,
-        volumetricData,
+        rho,
         output,
         gridsize,
         format=format,
         compact=compact,
         inorm=inorm,
     )
 
 
-def to_file(structure, filename: str, fmt=None, coords_are_cartesian=True):
+@logger.catch
+def to_file(
+    structure,
+    filename: str,
+    fmt: Optional[str] = None,
+    coords_are_cartesian: bool = True,
+):
     r"""Deprecated. Use :func:`dspawpy.io.structure.write` instead."""
-    warnings.warn(
+    logger.warning(
         "dspawpy.io.write.to_file is deprecated"
         "Use dspawpy.io.structure.write instead.",
         DeprecationWarning,
     )
     from .structure import write
 
     write(structure, filename, fmt, coords_are_cartesian)
 
 
-def _write_atoms(fileobj, structure, idirect=False):
+@logger.catch
+def _write_atoms(fileobj, structure, idirect: bool = False):
     fileobj.write("DS-PAW Structure\n")
     fileobj.write("  1.00\n")
     lattice = structure.lattice.matrix.reshape(-1, 1)
     fileobj.write(
         "%20.14f %20.14f %20.14f\n" % (lattice[0][0], lattice[1][0], lattice[2][0])
     )
     fileobj.write(
@@ -383,89 +403,85 @@
     fileobj.write("\n")
 
     for e in elements_set:
         fileobj.write("%5d " % (elements_number[e]))
     fileobj.write("\n")
     if idirect:
         fileobj.write("Direct\n")
-        for i, p in enumerate(structure.frac_coords):
+        for p in structure.frac_coords:
             fileobj.write("%20.14f %20.14f %20.14f\n" % (p[0], p[1], p[2]))
     else:
         fileobj.write("Cartesian\n")
-        for i, p in enumerate(structure.cart_coords):
+        for p in structure.cart_coords:
             fileobj.write("%20.14f %20.14f %20.14f\n" % (p[0], p[1], p[2]))
 
 
+@logger.catch
 def _write_specific_format(
     structure,
-    grid,
-    volumetricData,
-    filename,
-    gridsize,
-    format="cube",
-    compact=False,
-    inorm=False,
+    grid: Sequence[int],
+    volumetricData: Sequence,
+    filename: str,
+    gridsize: Optional[Sequence[int]] = None,
+    format: str = "cube",
+    compact: bool = False,
+    inorm: bool = False,
 ):
+    import os
+
     absfile = os.path.abspath(filename)
     if os.path.isfile(absfile):
-        print("Warning: %s already exists and will be overwritten!" % absfile)
+        logger.warning("%s already exists and will be overwritten!" % absfile)
     os.makedirs(os.path.dirname(absfile), exist_ok=True)
 
     import numpy as np
 
     vd = np.asarray(volumetricData)
     if inorm is True:
         vd /= np.sum(vd)
 
-    if format.lower() == "cube":
-        reshaped_vd = vd.reshape([grid[2], grid[1], grid[0]])
-    else:
-        reshaped_vd = vd.reshape([grid[0], grid[1], grid[2]])
-    ngx, ngy, ngz = reshaped_vd.shape
+    ngx, ngy, ngz = grid
+    reshaped_vd = vd.reshape(grid, order="F")  # ! dspaw output is in F order
 
     if gridsize is None:
-        nngx, nngy, nngz = ngx, ngy, ngz
+        gridsize = grid
         interp_data = reshaped_vd
-        new_grid = grid
     else:
-        nngx, nngy, nngz = gridsize
         oldngx = np.linspace(0, 1, ngx)
         oldngy = np.linspace(0, 1, ngy)
         oldngz = np.linspace(0, 1, ngz)
-        newngx = np.linspace(0, 1, nngx)
-        newngy = np.linspace(0, 1, nngy)
-        newngz = np.linspace(0, 1, nngz)
-        X, Y, Z = np.meshgrid(newngx, newngy, newngz, indexing="ij")
-        points = meshgrid2points(X, Y, Z)
-        interp_data = np.empty(
-            (nngx, nngy, nngz),
-            dtype=np.complex128,
-        )
-        print("Interpolating volumetric data...")
         from scipy.interpolate import RegularGridInterpolator
 
         rgi = RegularGridInterpolator((oldngx, oldngy, oldngz), reshaped_vd)
+
+        print("Interpolating volumetric data...")
+        newngx = np.linspace(0, 1, gridsize[0])
+        newngy = np.linspace(0, 1, gridsize[1])
+        newngz = np.linspace(0, 1, gridsize[2])
+        X, Y, Z = np.meshgrid(newngx, newngy, newngz, indexing="ij")
+        points = np.array([X.ravel(), Y.ravel(), Z.ravel()]).T
         interp_data = rgi(points).reshape(gridsize)
         print("volumetric data interpolated")
-        new_grid = gridsize
 
     if format.lower() == "cube":
         volume_in_Bohr3 = structure.volume / Bohr**3
-        reshaped_vd /= volume_in_Bohr3
+        interp_data /= volume_in_Bohr3
         with open(absfile, "w") as fileobj:
+            import time
+
             fileobj.write("Cube file written on " + time.strftime("%c"))
             fileobj.write("\nOUTER LOOP: X, MIDDLE LOOP: Y, INNER LOOP: Z\n")
 
             origin = np.zeros(3)
             fileobj.write(
                 f"{len(structure.sites):5d} {origin[0]:12.6f} {origin[1]:12.6f} {origin[2]:12.6f}\n"
             )
 
             for i in range(3):
-                n = new_grid[i]
+                n = gridsize[i]
                 d = structure.lattice.matrix[i] / n / Bohr
                 fileobj.write(f"{n:5d} {d[0]:12.6f} {d[1]:12.6f} {d[2]:12.6f}\n")
 
             positions = structure.cart_coords / Bohr
             species_string = [s.species_string for s in structure.sites]
             species_string = [
                 s.replace("+", "").replace("-", "") for s in species_string
@@ -474,83 +490,78 @@
             from dspawpy.io.utils import _symbols2numbers
 
             numbers = _symbols2numbers(symbols)
             for Z, (x, y, z) in zip(numbers, positions):
                 fileobj.write(f"{Z:5d} {0:12.6f} {x:12.6f} {y:12.6f} {z:12.6f}\n")
 
             if compact:
-                interp_data.T.flatten().tofile(fileobj, sep="\n", format="%.5e")
+                for ix in range(gridsize[0]):
+                    for iy in range(gridsize[1]):
+                        for iz in range(gridsize[2]):
+                            fileobj.write(f"{interp_data[ix, iy, iz]:12.5e}\n")
             else:
-                for iz in range(nngz):
-                    for iy in range(nngy):
-                        for ix in range(nngx):
+                for ix in range(gridsize[0]):
+                    for iy in range(gridsize[1]):
+                        for iz in range(gridsize[2]):
                             fileobj.write(f"{interp_data[ix, iy, iz]:12.5e} ")
-                            if ix % 6 == 5:
+                            if iz % 6 == 5:
                                 fileobj.write("\n")
                         fileobj.write("\n")
 
     elif format.lower() == "vesta" or format.lower() == "vasp":
         with open(absfile, "w") as file:
             _write_atoms(file, structure, idirect=True)
-            file.write("%5d %5d %5d\n" % (nngx, nngy, nngz))
+            file.write("%5d %5d %5d\n" % (gridsize[0], gridsize[1], gridsize[2]))
             count = 0
             if compact:
                 interp_data.flatten().tofile(file, sep="\n", format="%.5e")
             else:
-                for ix in range(nngx):
-                    for iy in range(nngy):
-                        for iz in range(nngz):
+                for iz in range(gridsize[2]):
+                    for iy in range(gridsize[1]):
+                        for ix in range(gridsize[0]):
                             file.write(f"{interp_data[ix, iy, iz]:12.5e} ")
                             count += 1
                             if count % 5 == 0:
                                 file.write("\n")
 
     elif format.lower() == "txt":
         with open(absfile, "w") as file:
             file.write(f"# {len(structure.sites)} atoms\n")
-            file.write(f"# {nngx} {nngy} {nngz} grid size\n")
+            file.write(f"# {gridsize[0]} {gridsize[1]} {gridsize[2]} grid size\n")
             file.write("# x y z value\n")
-            for ix in range(nngx):
-                for iy in range(nngy):
-                    for iz in range(nngz):
+            for ix in range(gridsize[0]):
+                for iy in range(gridsize[1]):
+                    for iz in range(gridsize[2]):
                         matrix = structure.lattice.matrix
-                        v_x = matrix[0] * ix / nngx
-                        v_y = matrix[1] * iy / nngy
-                        v_z = matrix[2] * iz / nngz
+                        v_x = matrix[0] * ix / gridsize[0]
+                        v_y = matrix[1] * iy / gridsize[1]
+                        v_z = matrix[2] * iz / gridsize[2]
                         v_xyz = v_x + v_y + v_z
                         x, y, z = v_xyz
                         file.write(
                             f"{x:.3f} {y:.3f} {z:.3f} {interp_data[ix, iy, iz]:14.7f}\n"
                         )
+            import time
+
             file.write(f"# {format} file written on {time.strftime('%c')}\n")
 
     else:
         raise NotImplementedError('only "cube", "vesta", "vasp", "txt" are supported.')
 
     print(f"==> {absfile}")
 
 
-def meshgrid2points(X, Y, Z):
-    import numpy as np
-
-    points = np.empty((X.shape[0] * Y.shape[1] * Z.shape[2], 3))
-    count = 0
-    for i in range(X.shape[0]):
-        for j in range(Y.shape[1]):
-            for k in range(Z.shape[2]):
-                points[count] = np.array([X[i, 0, 0], Y[0, j, 0], Z[0, 0, k]])
-                count += 1
-    return points
-
-
-def _to_dspaw_as(structure, filename: str, coords_are_cartesian=True):
+@logger.catch
+def _to_dspaw_as(structure, filename: str, coords_are_cartesian: bool = True):
     """write dspaw structure file of .as type"""
+    import os
+
     absfile = os.path.abspath(filename)
     if os.path.isfile(absfile):
-        warnings.warn("%s already exists and will be overwritten!" % absfile)
+        logger.warning("%s already exists and will be overwritten!" % absfile)
     os.makedirs(os.path.dirname(absfile), exist_ok=True)
     with open(absfile, "w", encoding="utf-8") as file:
         file.write("Total number of atoms\n")
         file.write("%d\n" % len(structure))
 
         # ^ write lattice info
         if "LatticeFixs" in structure.sites[0].properties:
@@ -641,20 +652,23 @@
                     coords[2],
                     final_strs,
                 )
             )
     print(f"==> {absfile}")
 
 
+@logger.catch
 def _to_hzw(structure, filename: str):
     """write hzw structure file of .hzw type"""
+    import os
+
     absfile = os.path.abspath(filename)
 
     if os.path.isfile(absfile):
-        warnings.warn("%s already exists and will be overwritten!" % absfile)
+        logger.warning("%s already exists and will be overwritten!" % absfile)
     os.makedirs(os.path.dirname(absfile), exist_ok=True)
     with open(absfile, "w", encoding="utf-8") as file:
         file.write("% The number of probes \n")
         file.write("0\n")
         file.write("% Uni-cell vector\n")
 
         for v in structure.lattice.matrix:
@@ -668,40 +682,48 @@
             file.write(
                 "%s %.6f %.6f %.6f\n"
                 % (site.species_string, site.coords[0], site.coords[1], site.coords[2])
             )
     print(f"==> {absfile}")
 
 
-def _to_dspaw_json(structure, filename: str, coords_are_cartesian=True):
+@logger.catch
+def _to_dspaw_json(structure, filename: str, coords_are_cartesian: bool = True):
     """write dspaw structure file of .json type"""
+    import os
+
     absfile = os.path.abspath(filename)
     lattice = structure.lattice.matrix.flatten().tolist()
     atoms = []
     for site in structure:
         coords = site.coords if coords_are_cartesian else site.frac_coords
         atoms.append({"Element": site.species_string, "Position": coords.tolist()})
 
     coordinate_type = "Cartesian" if coords_are_cartesian else "Direct"
     d = {"Lattice": lattice, "CoordinateType": coordinate_type, "Atoms": atoms}
     if os.path.isfile(absfile):
-        warnings.warn("%s already exists and will be overwritten!" % absfile)
+        logger.warning("%s already exists and will be overwritten!" % absfile)
     os.makedirs(os.path.dirname(absfile), exist_ok=True)
     with open(absfile, "w", encoding="utf-8") as file:
-        json.dump(d, file, indent=4)
+        from json import dump
+
+        dump(d, file, indent=4)
     print(f"==> {absfile}")
 
 
+@logger.catch
 def _to_pdb(structures, filename: str):
     """write pdb structure file of .pdb type"""
+    import os
+
     absfile = os.path.abspath(filename)
     if not isinstance(structures, list):
         structures = [structures]
     if os.path.isfile(absfile):
-        warnings.warn("%s already exists and will be overwritten!" % absfile)
+        logger.warning("%s already exists and will be overwritten!" % absfile)
     os.makedirs(os.path.dirname(absfile), exist_ok=True)
     with open(absfile, "w", encoding="utf-8") as file:
         for i, s in enumerate(structures):
             file.write("MODEL         %d\n" % (i + 1))
             file.write("REMARK   Converted from Structures\n")
             file.write("REMARK   Converted using dspawpy\n")
             # may lack lattice info
```

### Comparing `dspawpy-1.2.2/dspawpy/plot.py` & `dspawpy-1.3.0/dspawpy/plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # -*- coding: utf-8 -*-
-import json
-import os
-from typing import List, cast
-import matplotlib.pyplot as plt
-import numpy as np
-
-try:
-    plt.style.use("science")
-except Exception:  # install scienceplots to science style figure
-    pass  # check https://github.com/garrettj403/SciencePlots
+from loguru import logger
+from typing import List, Tuple, cast, Optional, TYPE_CHECKING
 
+if TYPE_CHECKING:
+    from pymatgen.electronic_structure.bandstructure import BandStructureSymmLine
+    from pymatgen.electronic_structure.plotter import BSDOSPlotter
+    from pymatgen.electronic_structure.dos import CompleteDos
 
+
+@logger.catch
 def average_along_axis(
-    datafile="potential.h5",
+    datafile: str = "potential.h5",
     task: str = "potential",
-    axis=2,
-    smooth=False,
-    smooth_frac=0.8,
-    raw=False,
-    subtype: str = None,
+    axis: int = 2,
+    smooth: bool = False,
+    smooth_frac: float = 0.8,
+    raw: bool = False,
+    subtype: Optional[str] = None,
     **kwargs,
 ):
     r"""绘制沿着某个轴向的物理量平均值曲线
 
     Parameters
     ----------
     datafile : str or list or np.ndarray
@@ -49,146 +47,173 @@
 
     Examples
     --------
     >>> from dspawpy.plot import average_along_axis
 
     读取 potential.h5 文件中的数据，绘图并保存原始绘图数据到csv文件
 
-    >>> average_along_axis(datafile='dspawpy_proj/dspawpy_tests/inputs/2.7/potential.h5', task='potential', axis=2, smooth=True, smooth_frac=0.8, raw=True) # doctest: +ELLIPSIS
+    >>> average_along_axis(datafile='dspawpy_proj/dspawpy_tests/inputs/2.7/potential.h5', task='potential', axis=2, smooth=True, smooth_frac=0.8) # doctest: +ELLIPSIS
     Reading .../dspawpy_proj/dspawpy_tests/inputs/2.7/potential.h5...
     <module 'matplotlib.pyplot' from '.../matplotlib/pyplot.py'>
     """
     assert task in [
         "rho",
         "potential",
         "elf",
         "pcharge",
         "rhoBound",
     ], "Only support: rho, potential, elf, pcharge, rhoBound"
 
     # only for compatibility
+    import numpy as np
+
     if isinstance(datafile, list) or isinstance(datafile, np.ndarray):
         ys = datafile  # expect np.ndarray or list
     else:
         from dspawpy.io.utils import get_absfile
 
         absfile = get_absfile(datafile, task)
+        print(f"Reading {absfile}...")
 
-    print(f"Reading {absfile}...")
-    if absfile.endswith(".h5"):
-        hfile = absfile
-        from dspawpy.io.read import load_h5
-
-        hdict = load_h5(hfile)
-        grid = hdict["/AtomInfo/Grid"]
-
-        if task == "rho":
-            if subtype is None:
-                _key = "/Rho/TotalCharge"
-            else:
+        if absfile.endswith(".h5"):
+            hfile = absfile
+            from dspawpy.io.read import load_h5
+
+            hdict = load_h5(hfile)
+            grid = hdict["/AtomInfo/Grid"]
+
+            if task == "rho":
+                if subtype is None:
+                    subtype = "TotalCharge"
                 _key = f"/Rho/{subtype}"
-        elif task == "potential":
-            if subtype is None:
-                subtype = "TotalElectrostaticPotential"
-            _key = f"/Potential/{subtype}"
-        elif task == "elf":
-            if subtype is None:
-                _key = "/ELF/TotalELF"
-            else:
+            elif task == "potential":
+                if subtype is None:
+                    if "/Potential/TotalElectrostaticPotential" in hdict:
+                        subtype = "TotalElectrostaticPotential"
+                    elif "/Potential/TotalLocalPotential" in hdict:
+                        subtype = "TotalLocalPotential"
+                    else:
+                        raise KeyError(
+                            f"Neither TotalElectrostaticPotential nor TotalLocalPotential can be found, please check your {absfile}"
+                        )
+                _key = f"/Potential/{subtype}"
+            elif task == "elf":
+                if subtype is None:
+                    subtype = "TotalELF"
                 _key = f"/ELF/{subtype}"
-        elif task == "pcharge":
-            if subtype is None:
-                _key = "/Pcharge/1/TotalCharge"
-            else:
+            elif task == "pcharge":
+                if subtype is None:
+                    subtype = "TotalCharge"
                 _key = f"/Pcharge/1/{subtype}"
-        elif task == "rhoBound":
-            if subtype is None:
-                _key = "/Rho"
+            elif task == "rhoBound":
+                if subtype is None:
+                    _key = "/Rho"
+                else:
+                    _key = subtype
             else:
-                _key = subtype
+                raise ValueError("Only support rho, potential, elf, pcharge, rhoBound")
 
-        if _key not in hdict:
-            raise KeyError(f"No {_key} key")
+            if _key not in hdict:
+                raise KeyError(f"No {_key} key")
 
-        # DS-PAW 数据写入h5 列优先
-        # h5py 从h5读取数据 默认行优先
-        # np.array(data_list) 默认行优先
-        # 所以这里先以 行优先 把 “h5 行优先 读进来的数据” 转成一维， 再以 列优先 转成 grid 对应的维度
-        tmp_pot = np.asarray(hdict[_key]).reshape([-1, 1], order="C")
-        ys = tmp_pot.reshape(grid, order="F")
+            tmp_pot = np.asarray(hdict[_key]).reshape([-1, 1], order="C")
+            ys = tmp_pot.reshape(grid, order="F")
 
-    elif absfile.endswith(".json"):
-        jfile = absfile
-        with open(jfile, "r") as f:
-            jdict = json.load(f)
-        grid = jdict["AtomInfo"]["Grid"]
+        elif absfile.endswith(".json"):
+            jfile = absfile
+            with open(jfile, "r") as f:
+                from json import load
 
-        if task == "rho":
-            if subtype is None:
-                ys = np.asarray(jdict["Rho"]["TotalCharge"]).reshape(grid, order="F")
-            else:
+                jdict = load(f)
+            grid = jdict["AtomInfo"]["Grid"]
+
+            if task == "rho":
+                if subtype is None:
+                    subtype = "TotalCharge"
                 ys = np.asarray(jdict["Rho"][subtype]).reshape(grid, order="F")
-        elif task == "potential":
-            if subtype is None:
-                subtype = "TotalElectrostaticPotential"
-            ys = np.asarray(jdict["Potential"][subtype]).reshape(grid, order="F")
-        elif task == "elf":
-            if subtype is None:
-                ys = np.asarray(jdict["ELF"]["TotalELF"]).reshape(grid, order="F")
-            else:
+            elif task == "potential":
+                if subtype is None:
+                    if "TotalElectrostaticPotential" in jdict["Potential"]:
+                        subtype = "TotalElectrostaticPotential"
+                    elif "TotalLocalPotential" in jdict["Potential"]:
+                        subtype = "TotalLocalPotential"
+                    else:
+                        raise KeyError(
+                            f"Neither TotalElectrostaticPotential nor TotalLocalPotential can be found, please check your {absfile}"
+                        )
+
+                ys = np.asarray(jdict["Potential"][subtype]).reshape(grid, order="F")
+            elif task == "elf":
+                if subtype is None:
+                    subtype = "TotalELF"
                 ys = np.asarray(jdict["ELF"][subtype]).reshape(grid, order="F")
-        elif task == "pcharge":
-            if subtype is None:
-                ys = np.asarray(jdict["Pcharge"][0]["TotalCharge"]).reshape(
-                    grid, order="F"
-                )
-            else:
+            elif task == "pcharge":
+                if subtype is None:
+                    subtype = "TotalCharge"
                 ys = np.asarray(jdict["Pcharge"][0][subtype]).reshape(grid, order="F")
-        else:
-            if subtype is None:
-                ys = np.asarray(jdict["Rho"]).reshape(grid, order="F")
             else:
+                if subtype is None:
+                    subtype = "Rho"
                 ys = np.asarray(jdict[subtype]).reshape(grid, order="F")
 
-    else:
-        raise TypeError("Only suport h5/json file")
+        else:
+            raise TypeError("Only suport h5/json file")
 
     all_axis = [0, 1, 2]
     all_axis.remove(axis)
-    y = np.mean(ys, tuple(all_axis))
+    y = np.mean(ys, tuple(all_axis))  # type: ignore
     x = np.arange(len(y))
 
+    import matplotlib.pyplot as plt
+
     if raw:
-        import pandas as pd
+        try:
+            import polars as pl
+
+            pl.DataFrame({"x": x, "y": y}).write_csv(
+                f"raw{task}_axis{axis}.csv",
+            )
+        except ModuleNotFoundError:
+            import pandas as pd
 
-        pd.DataFrame({"x": x, "y": y}).to_csv(f"raw{task}_axis{axis}.csv", index=False)
+            pd.DataFrame({"x": x, "y": y}).to_csv(
+                f"raw{task}_axis{axis}.csv",
+            )
     if smooth:
         import statsmodels.api as sm
 
         s = sm.nonparametric.lowess(y, x, frac=smooth_frac)
         if raw:
-            import pandas as pd
+            try:
+                import polars as pl
 
-            pd.DataFrame({"x": s[:, 0], "y": s[:, 1]}).to_csv(
-                f"raw{task}_axis{axis}_smooth.csv", index=False
-            )
+                pl.DataFrame({"x": s[:, 0], "y": s[:, 1]}).write_csv(
+                    f"raw{task}_axis{axis}_smooth.csv",
+                )
+            except ModuleNotFoundError:
+                import pandas as pd
+
+                pd.DataFrame({"x": s[:, 0], "y": s[:, 1]}).to_csv(
+                    f"raw{task}_axis{axis}_smooth.csv",
+                )
 
         plt.plot(s[:, 0], s[:, 1], label="macroscopic average", **kwargs)
 
     plt.plot(x, y, **kwargs)
 
     return plt
 
 
+@logger.catch
 def plot_aimd(
     datafile: str = "aimd.h5",
     show: bool = True,
     figname: str = "aimd.png",
-    flags_str="12345",
-    raw=False,
+    flags_str: str = "12345",
+    raw: bool = False,
 ):
     r"""AIMD任务完成后，绘制关键物理量的收敛过程图
 
     aimd.h5 -> aimd.png
 
     Parameters
     ----------
@@ -236,26 +261,37 @@
         flags.remove(" ")
 
     for flag in flags:
         assert flag in ["1", "2", "3", "4", "5"], "flag must be in '12345'"
 
     # 开始画组合图
     N_figs = len(flags)
+    import matplotlib.pyplot as plt
+
     fig, axes = plt.subplots(N_figs, 1, sharex=True, figsize=(6, 2 * N_figs))
     if N_figs == 1:  # 'AxesSubplot' object is not subscriptable
         axes = [axes]  # 避免上述类型错误
     fig.suptitle("DSPAW AIMD")
     for i, flag in enumerate(flags):
         print("For subfigure " + flag)
         # 读取数据
         xs, ys = _read_aimd_converge_data(datafile, flag)
         if raw:
-            import pandas as pd
+            try:
+                import polars as pl
+
+                pl.DataFrame({"x": xs, "y": ys}).write_csv(
+                    f"rawaimd_{flag}.csv",
+                )
+            except ModuleNotFoundError:
+                import pandas as pd
 
-            pd.DataFrame({"x": xs, "y": ys}).to_csv(f"rawaimd_{flag}.csv", index=False)
+                pd.DataFrame({"x": xs, "y": ys}).to_csv(
+                    f"rawaimd_{flag}.csv",
+                )
 
         axes[i].plot(xs, ys)  # 绘制坐标点
         # 子图的y轴标签
         if flag == "1":
             axes[i].set_ylabel("Kinetic Energy (eV)")
         elif flag == "2":
             axes[i].set_ylabel("Energy (eV)")
@@ -265,24 +301,31 @@
             axes[i].set_ylabel("Temperature (K)")
         else:
             axes[i].set_ylabel("Volume (Angstrom^3)")
 
     plt.tight_layout()
     # save and show
     if figname:
+        import os
+
         absfig = os.path.abspath(figname)
         os.makedirs(os.path.dirname(absfig), exist_ok=True)
         plt.savefig(absfig, dpi=300)
         print(f"==> {absfig}")
     if show:
         plt.show()
 
 
+@logger.catch
 def plot_bandunfolding(
-    datafile: str = "band.h5", ef=None, de=0.05, dele=0.06, raw=False
+    datafile: str = "band.h5",
+    ef: Optional[float] = None,
+    de: float = 0.05,
+    dele: float = 0.06,
+    raw: bool = False,
 ):
     r"""能带反折叠任务完成后，读取 h5 或 json 文件数据绘图
 
     band.h5/band.json -> bandunfolding.png
 
     Parameters
     ----------
@@ -306,33 +349,36 @@
     --------
 
     绘图并保存绘图数据到rawbandunfolding.csv
 
     >>> from dspawpy.plot import plot_bandunfolding
     >>> plot_bandunfolding("dspawpy_proj/dspawpy_tests/inputs/2.22/band.h5", raw=True) # doctest: +ELLIPSIS
     Reading .../dspawpy_proj/dspawpy_tests/inputs/2.22/band.h5...
-    <module 'matplotlib.pyplot' from '.../matplotlib/pyplot.py'>
     """
     from dspawpy.io.utils import get_absfile
 
     absfile = get_absfile(datafile, task="band")
     print(f"Reading {absfile}...")
+    import numpy as np
+
     if absfile.endswith(".h5"):
         from h5py import File
 
         f = File(absfile, "r")
         if ef is None:
             ef = np.array(f["/UnfoldingBandInfo/EFermi"])[0]
         number_of_band = np.array(f["/BandInfo/NumberOfBand"])[0]
         number_of_kpoints = np.array(f["/BandInfo/NumberOfKpoints"])[0]
         data = np.array(f["/UnfoldingBandInfo/Spin1/UnfoldingBand"])
         weight = np.array(f["/UnfoldingBandInfo/Spin1/Weight"])
     elif absfile.endswith(".json"):
         with open(absfile, "r") as f:
-            band = json.load(f)
+            from json import load
+
+            band = load(f)
         if ef is None:
             ef = band["UnfoldingBandInfo"]["EFermi"]
         number_of_band = band["BandInfo"]["NumberOfBand"]
         number_of_kpoints = band["BandInfo"]["NumberOfKpoints"]
         data = band["UnfoldingBandInfo"]["Spin1"]["UnfoldingBand"]
         weight = band["UnfoldingBandInfo"]["Spin1"]["Weight"]
     else:
@@ -341,41 +387,56 @@
     celtot = np.array(data).reshape((number_of_kpoints, number_of_band)).T
     proj_wt = np.array(weight).reshape((number_of_kpoints, number_of_band)).T
     X2, Y2, Z2, emin = getEwtData(
         number_of_kpoints, number_of_band, celtot, proj_wt, ef, de, dele
     )
 
     if raw:
-        import pandas as pd
+        try:
+            import polars as pl
 
-        pd.DataFrame({"Y": Y2, "Z": Z2}, index=X2).to_csv(
-            "rawbandunfolding.csv", header=["Y", "color"], index=True, index_label="X"
-        )
+            pl.DataFrame({"Y": Y2, "Z": Z2}).write_csv(
+                "rawbandunfolding.csv",
+                schemas=["Y", "color"],
+                index_label="X",
+            )  # type: ignore
+        except ModuleNotFoundError:
+            import pandas as pd
+
+            pd.DataFrame({"Y": Y2, "Z": Z2}).to_csv(
+                "rawbandunfolding.csv",
+                header=["Y", "color"],
+                index=True,
+                index_label="X",
+            )
+
+    import matplotlib.pyplot as plt
 
     plt.clf()
     plt.scatter(X2, Y2, c=Z2, cmap="hot")
     plt.xlim(0, 200)
     plt.ylim(emin - 0.5, 15)
     ax = plt.gca()
     plt.colorbar()
     ax.set_facecolor("black")
 
     return plt
 
 
+@logger.catch
 def plot_optical(
     datafile: str = "optical.h5",
     keys: List[str] = [
         "AbsorptionCoefficient",
         "ExtinctionCoefficient",
         "RefractiveIndex",
         "Reflectance",
     ],
     axes: List[str] = ["X", "Y", "Z", "XY", "YZ", "ZX"],
-    raw=False,
+    raw: bool = False,
     prefix: str = "",
 ):
     """光学性质计算任务完成后，读取数据并绘制预览图
 
     optical.h5/optical.json -> optical.png
 
     Parameters
@@ -385,52 +446,58 @@
     keys: List[str]
         可选 "AbsorptionCoefficient", "ExtinctionCoefficient", "RefractiveIndex", "Reflectance" 中的任意一个，默认 "AbsorptionCoefficient"
     axes : List[str]
         序号，默认"X", "Y", "Z", "XY", "YZ", "ZX"
     raw : bool
         是否保存绘图数据到csv
 
+    Exapmles
     --------
 
     绘图并保存绘图数据到rawoptical.csv
 
     >>> from dspawpy.plot import plot_optical
-    >>> plot_optical("dspawpy_proj/dspawpy_tests/inputs/2.12/scf.h5", "AbsorptionCoefficient", ['X', 'Y'], raw=True) # doctest: +ELLIPSIS
+    >>> plot_optical("dspawpy_proj/dspawpy_tests/inputs/2.12/scf.h5", "AbsorptionCoefficient", ['X', 'Y'], prefix='dspawpy_proj/dspawpy_tests/outputs/doctest') # doctest: +ELLIPSIS
     Reading .../dspawpy_proj/dspawpy_tests/inputs/2.12/scf.h5...
-    >>> plot_optical("dspawpy_proj/dspawpy_tests/inputs/2.12/optical.json", ["AbsorptionCoefficient"], ['X', 'Y'], raw=True) # doctest: +ELLIPSIS
+    >>> plot_optical("dspawpy_proj/dspawpy_tests/inputs/2.12/optical.json", ["AbsorptionCoefficient"], ['X', 'Y'], prefix='dspawpy_proj/dspawpy_tests/outputs/doctest') # doctest: +ELLIPSIS
     Reading .../dspawpy_proj/dspawpy_tests/inputs/2.12/optical.json...
     """
+    import matplotlib.pyplot as plt
+    from scipy.interpolate import interp1d
+    from dspawpy.io.utils import get_absfile
+    import numpy as np
+
     if isinstance(keys, str):
         keys = [keys]
-    from dspawpy.io.utils import get_absfile
 
     absfile = get_absfile(datafile, task="optical")
     print(f"Reading {absfile}...")
     data = {}
     if absfile.endswith("h5"):
         from dspawpy.io.read import load_h5
 
         data_all = load_h5(absfile)
         energy = data_all["/OpticalInfo/EnergyAxe"]
         for k in keys:
             data[k] = data_all["/OpticalInfo/" + k]
     elif absfile.endswith("json"):
         with open(absfile, "r") as fin:
-            data_all = json.load(fin)
+            from json import load
+
+            data_all = load(fin)
         energy = data_all["OpticalInfo"]["EnergyAxe"]
         for k in keys:
             data[k] = data_all["OpticalInfo"][k]
     else:
         raise TypeError("Only support h5/json file")
 
-    from scipy.interpolate import interp1d
-
     energy_spline = np.linspace(energy[0], energy[-1], 2001)
     dd = {"X": 0, "Y": 1, "Z": 2, "XY": 3, "YZ": 4, "ZX": 5}
     data_spline_dict = {}
+
     for k, v in data.items():
         plt.clf()
         plt.xlabel("Photon energy (eV)", fontsize=14)
         plt.ylabel(k + r" $\alpha (\omega )(cm^{-1})$", fontsize=14)
         for a in axes:
             d = np.asarray(v).reshape(len(energy), 6)[:, dd[a]]
             inter_f = interp1d(energy, d, kind="cubic")
@@ -440,33 +507,56 @@
         plt.legend()
         if prefix == "":
             plt.savefig(f"{k}.png")
         else:
             plt.savefig(f"{prefix}/{k}.png")
 
     if raw:
-        import pandas as pd
+        try:
+            import polars as pl
 
-        for k in data:
-            dictOriginal = {"energy": energy}
-            dictInterp = {"energy": energy_spline}
-            for a in axes:
-                dictOriginal.update(
-                    {k + a: np.asarray(data[k]).reshape(len(energy), 6)[:, dd[a]]}
+            for k in data:
+                dictOriginal = {"energy": energy}
+                dictInterp = {"energy": energy_spline}
+                for a in axes:
+                    dictOriginal.update(
+                        {k + a: np.asarray(data[k]).reshape(len(energy), 6)[:, dd[a]]}
+                    )
+                    dictInterp.update({k + a: data_spline_dict[k + a]})
+                pl.DataFrame(dictOriginal).write_csv(
+                    f"rawoptical{k}.csv",
+                )
+                pl.DataFrame(dictInterp).write_csv(
+                    f"rawoptical_spline{k}.csv",
+                )
+        except ModuleNotFoundError:
+            import pandas as pd
+
+            for k in data:
+                dictOriginal = {"energy": energy}
+                dictInterp = {"energy": energy_spline}
+                for a in axes:
+                    dictOriginal.update(
+                        {k + a: np.asarray(data[k]).reshape(len(energy), 6)[:, dd[a]]}
+                    )
+                    dictInterp.update({k + a: data_spline_dict[k + a]})
+                pd.DataFrame(dictOriginal).to_csv(
+                    f"rawoptical{k}.csv",
+                )
+                pd.DataFrame(dictInterp).to_csv(
+                    f"rawoptical_spline{k}.csv",
                 )
-                dictInterp.update({k + a: data_spline_dict[k + a]})
-            pd.DataFrame(dictOriginal).to_csv(f"rawoptical{k}.csv", index=False)
-            pd.DataFrame(dictInterp).to_csv(f"rawoptical_spline{k}.csv", index=False)
 
 
+@logger.catch
 def plot_phonon_thermal(
     datafile: str = "phonon.h5",
     figname: str = "phonon.png",
     show: bool = True,
-    raw=False,
+    raw: bool = False,
 ):
     """声子热力学计算任务完成后，绘制相关物理量随温度变化曲线
 
     phonon.h5/phonon.json -> phonon.png
 
     Parameters
     ----------
@@ -483,23 +573,25 @@
     ----------
     figname : str
         图片路径，默认 'phonon.png'
 
     Examples
     --------
     >>> from dspawpy.plot import plot_phonon_thermal
-    >>> plot_phonon_thermal('dspawpy_proj/dspawpy_tests/inputs/2.26/phonon.h5', figname='dspawpy_proj/dspawpy_tests/inputs/out/phonon_thermal.png', show=False) # doctest: +ELLIPSIS
+    >>> plot_phonon_thermal('dspawpy_proj/dspawpy_tests/inputs/2.26/phonon.h5', figname='dspawpy_proj/dspawpy_tests/outputs/doctest/phonon_thermal.png', show=False) # doctest: +ELLIPSIS
     Reading .../dspawpy_proj/dspawpy_tests/inputs/2.26/phonon.h5...
-    ==> .../dspawpy_proj/dspawpy_tests/inputs/out/phonon_thermal.png
+    ==> .../dspawpy_proj/dspawpy_tests/outputs/doctest/phonon_thermal.png
     """
     from dspawpy.io.utils import get_absfile
 
     absfile = get_absfile(datafile, task="phonon")
     print(f"Reading {absfile}...")
 
+    import numpy as np
+
     if absfile.endswith(".h5"):
         hfile = absfile
         from h5py import File
 
         ph = File(hfile, "r")
         if "/ThermalInfo/Temperatures" not in ph:
             raise KeyError(
@@ -508,33 +600,53 @@
         temp = np.array(ph["/ThermalInfo/Temperatures"])
         entropy = np.array(ph["/ThermalInfo/Entropy"])
         heat_capacity = np.array(ph["/ThermalInfo/HeatCapacity"])
         helmholts_free_energy = np.array(ph["/ThermalInfo/HelmholtzFreeEnergy"])
     elif absfile.endswith(".json"):
         jfile = absfile
         with open(jfile, "r") as f:
-            data = json.load(f)
+            from json import load
+
+            data = load(f)
         temp = np.array(data["ThermalInfo"]["Temperatures"])
         entropy = np.array(data["ThermalInfo"]["Entropy"])
         heat_capacity = np.array(data["ThermalInfo"]["HeatCapacity"])
         helmholts_free_energy = np.array(data["ThermalInfo"]["HelmholtzFreeEnergy"])
     else:
         raise TypeError("Only support h5/json file")
 
     if raw:
-        import pandas as pd
+        try:
+            import polars as pl
 
-        pd.DataFrame(
-            {
-                "temp": temp,
-                "entropy": entropy,
-                "heat_capacity": heat_capacity,
-                "helmholts_free_energy": helmholts_free_energy,
-            }
-        ).to_csv("rawphonon.csv", index=False)
+            pl.DataFrame(
+                {
+                    "temp": temp,
+                    "entropy": entropy,
+                    "heat_capacity": heat_capacity,
+                    "helmholts_free_energy": helmholts_free_energy,
+                }
+            ).write_csv(
+                "rawphonon.csv",
+            )
+        except ModuleNotFoundError:
+            import pandas as pd
+
+            pd.DataFrame(
+                {
+                    "temp": temp,
+                    "entropy": entropy,
+                    "heat_capacity": heat_capacity,
+                    "helmholts_free_energy": helmholts_free_energy,
+                }
+            ).to_csv(
+                "rawphonon.csv",
+            )
+
+    import matplotlib.pyplot as plt
 
     plt.plot(temp, entropy, c="red", label="Entropy (J/K/mol)")
     plt.plot(temp, heat_capacity, c="green", label="Heat Capacity (J/K/mol)")
     plt.plot(
         temp, helmholts_free_energy, c="blue", label="Helmholtz Free Energy (kJ/mol)"
     )
     plt.xlabel("Temperature(K)")
@@ -543,30 +655,33 @@
     plt.grid(alpha=0.2)
     plt.legend()
     plt.title("Thermal")
 
     plt.tight_layout()
     # save and show
     if figname:
+        import os
+
         absfig = os.path.abspath(figname)
         os.makedirs(os.path.dirname(absfig), exist_ok=True)
         plt.savefig(absfig, dpi=300)
         print(f"==> {absfig}")
     if show:
         plt.show()
 
 
+@logger.catch
 def plot_polarization_figure(
     directory: str,
     repetition: int = 2,
     annotation: bool = False,
     annotation_style: int = 1,
     show: bool = True,
     figname: str = "pol.png",
-    raw=False,
+    raw: bool = False,
 ):
     """绘制铁电极化结果图
 
     Parameters
     ----------
     directory : str
         铁电极化计算任务主目录
@@ -585,22 +700,26 @@
     -------
     axes: matplotlib.axes._subplots.AxesSubplot
         可传递给其他函数进行进一步处理
 
     Examples
     --------
     >>> from dspawpy.plot import plot_polarization_figure
-    >>> result = plot_polarization_figure(directory='dspawpy_proj/dspawpy_tests/inputs/2.20', figname='dspawpy_proj/dspawpy_tests/inputs/out/pol.png', show=False) # doctest: +ELLIPSIS
-    ==> .../dspawpy_proj/dspawpy_tests/inputs/out/pol.png
+    >>> result = plot_polarization_figure(directory='dspawpy_proj/dspawpy_tests/inputs/2.20', figname='dspawpy_proj/dspawpy_tests/outputs/doctest/pol.png', show=False) # doctest: +ELLIPSIS
+    ==> .../dspawpy_proj/dspawpy_tests/outputs/doctest/pol.png
     """
     assert repetition >= 0, "The number of repetitions must be a natural number"
     subfolders, quantum, totals = _get_subfolders_quantum_totals(directory)
     number_sfs = [int(sf) for sf in subfolders]
+    import matplotlib.pyplot as plt
+
     fig, axes = plt.subplots(1, 3, sharey=True)
     xyz = ["x", "y", "z"]
+    import numpy as np
+
     for j in range(3):  # x, y, z
         ys = np.empty(shape=(len(subfolders), repetition * 2 + 1))
         for r in range(repetition + 1):
             ys[:, repetition - r] = totals[:, j] - quantum[j] * r
             ys[:, repetition + r] = totals[:, j] + quantum[j] * r
 
         axes[j].plot(number_sfs, ys, ".")  # plot
@@ -659,31 +778,39 @@
                             ys[-1, i] - np.max(ys) / repetition / 5,
                         ),
                     )
             else:
                 raise ValueError("annotation_style must be 1 or 2")
 
         if raw:
-            import pandas as pd
+            try:
+                import polars as pl
 
-            pd.DataFrame(ys, index=subfolders).to_csv(f"pol_{xyz[j]}.csv")
+                pl.DataFrame(ys).write_csv(f"pol_{xyz[j]}.csv")
+            except ModuleNotFoundError:
+                import pandas as pd
+
+                pd.DataFrame(ys).to_csv(f"pol_{xyz[j]}.csv")
 
     plt.tight_layout()
     # save and show
     if figname:
+        import os
+
         absfig = os.path.abspath(figname)
         os.makedirs(os.path.dirname(absfig), exist_ok=True)
         plt.savefig(absfig, dpi=300)
         print(f"==> {absfig}")
     if show:
         plt.show()
 
     return axes
 
 
+@logger.catch
 def _get_subfolders_quantum_totals(directory: str):
     """返回铁电极化计算任务的子目录、量子数、极化总量；
 
     请勿创建其他子目录，否则会被错误读取
 
     Parameters
     ----------
@@ -695,14 +822,16 @@
     subfolders : list
         子目录列表
     quantum : np.ndarray
         量子数，xyz三个方向, shape=(1, 3)
     totals : np.ndarray
         极化总量，xyz三个方向, shape=(len(subfolders), 3)
     """
+    import os
+
     absdir = os.path.abspath(directory)
     raw_subfolders = next(os.walk(absdir))[1]
     subfolders = []
     for subfolder in raw_subfolders:
         assert (
             0 <= int(subfolder) < 100
         ), f"--> You should rename subfolders to 0~99, but {subfolder} found"
@@ -714,42 +843,51 @@
     subfolders.sort()  # 从小到大排序
 
     # quantum number if constant across the whole calculation, read only once
     absh5 = f"{os.path.join(absdir, subfolders[0])}/scf.h5"
     absjs = f"{os.path.join(absdir, subfolders[0])}/polarization.json"
     from h5py import File
 
+    import numpy as np
+
     if os.path.isfile(absjs):
         quantum = np.array(File(absh5).get("/PolarizationInfo/Quantum"))
     elif os.path.isfile(absjs):
         with open(absjs, "r") as f:
-            quantum = np.array(json.load(f)["PolarizationInfo"]["Quantum"])
+            from json import load
+
+            quantum = np.array(load(f)["PolarizationInfo"]["Quantum"])
     else:
         raise FileNotFoundError(f"No {absh5}/{absjs}")
 
     totals = np.empty(shape=(len(subfolders), 3))
     # the Total number is not constant, read for each subfolder
     for i, fd in enumerate(subfolders):
         absh5 = f"{os.path.join(absdir, fd)}/scf.h5"
         absjs = f"{os.path.join(absdir, fd)}/polarization.json"
         if os.path.isfile(absh5):
             data = File(f"{os.path.join(absdir, fd)}/scf.h5")
             total = np.array(data.get("/PolarizationInfo/Total"))
         elif os.path.isfile(absjs):
             with open(absjs, "r") as f:
-                data = json.load(f)
+                from json import load
+
+                data = load(f)
             total = np.array(data["PolarizationInfo"]["Total"], dtype=float)
         else:
             raise FileNotFoundError(f"No {absh5}/{absjs}")
         totals[i] = total
 
     return subfolders, quantum, totals
 
 
+@logger.catch
 def getEwtData(nk, nb, celtot, proj_wt, ef, de, dele):
+    import numpy as np
+
     emin = np.min(celtot) - de
     emax = np.max(celtot) - de
 
     emin = np.floor(emin - 0.2)
     emax = max(np.ceil(emax) * 1.0, 5.0)
 
     nps = int((emax - emin) / de)
@@ -780,15 +918,16 @@
     for i, x in enumerate(Z2):
         if x > Z2_half:
             Z2[i] = Z2_half
 
     return X2, Y2, Z2, emin
 
 
-def _read_aimd_converge_data(datafile: str, index: str = None):
+@logger.catch
+def _read_aimd_converge_data(datafile: str, index: Optional[str] = None):
     """从datafile指定的路径读取index指定的数据，返回绘图用的xs和ys两个数组
 
     Parameters
     ----------
     datafile : str or list
         hdf5文件路径，如 'aimd.h5' 或 ['aimd.h5', 'aimd2.h5']
     index : str
@@ -797,14 +936,16 @@
     Returns
     -------
     xs : np.ndarray
         x轴数据
     ys : np.ndarray
         y轴数据
     """
+    import numpy as np
+
     if isinstance(datafile, list):
         xs = []
         ys = []
         for i, df in enumerate(datafile):
             # concentrate returned np.ndarray
             x, y = _read_aimd_converge_data(df, index)
             xs.extend(x)
@@ -821,63 +962,66 @@
         hf = File(absfile)  # 加载h5文件
         print(f"Reading {absfile}...")
         Nstep = len(np.array(hf.get("/Structures"))) - 2  # 步数（可能存在未完成的）
         ys = np.full(Nstep, np.nan)  # 准备一个空数组
         # 开始读取
         if index == "5":
             for i in range(1, Nstep + 1):
-                ys[i - 1] = np.linalg.det(hf.get("/Structures/Step-%d/Lattice" % i))
+                ys[i - 1] = np.linalg.det(
+                    np.array(hf.get("/Structures/Step-%d/Lattice" % i))
+                )
         else:
             map = {
                 "1": "IonsKineticEnergy",
                 "2": "TotalEnergy0",
                 "3": "PressureKinetic",
                 "4": "Temperature",
             }
-            import warnings
-
-            if index == "3" and "PressureKinetic" not in hf.get("/AimdInfo/Step-1"):
-                warnings.warn(
+            if index == "3" and "PressureKinetic" not in np.array(
+                hf.get("/AimdInfo/Step-1")
+            ):
+                logger.warning(
                     "Ensemble is neither NPT nor NPH, no PressureKinetic found for subfigure 3!"
                 )
             else:
                 for i in range(1, Nstep + 1):
-                    # 如果计算中断，则没有PressureKinetic这个键
+                    assert index is not None
                     try:
                         ys[i - 1] = np.array(
                             hf.get("/AimdInfo/Step-%d/%s" % (i, map[index]))
                         )
                     except Exception:
                         ys[i - 1] = 0
                         ys = np.delete(ys, -1)
-                        warnings.warn(
+                        logger.warning(
                             "-> AIMD task stopped at Nstep=%s, failed to read its %s value"
                             % (Nstep, map[index])
                         )
                         break
 
         Nstep = len(ys)  # 步数更新为实际完成的步数
 
         # 返回xs，ys两个数组
         return np.linspace(1, Nstep, Nstep), np.array(ys)
 
     else:
         raise TypeError("datafile must be str or list")
 
 
+@logger.catch
 def pltbd(
-    bdp,
-    bs,
-    dos: None,
+    bdp: "BSDOSPlotter",
+    bs: "BandStructureSymmLine",
+    dos: Optional["CompleteDos"] = None,
     demax: float = 0.1,
-    ylim=None,
-    alpha=0.3,
-    colors=["red", "green", "blue"],
-    filename="banddos.png",
-    dpi=300,
+    ylim: Optional[Tuple[float, float]] = None,
+    alpha: float = 0.3,
+    colors: Optional[List[str]] = None,
+    filename: str = "banddos.png",
+    dpi: int = 300,
 ):
     """基于BSDOSPlotter类的get_plot()优化而来，可绘制（投影）能带态密度图。
 
     改进：
 
     - dos 使用半透明涂抹
     - 费米能级用虚线，左右费米能级保持在同一高度
@@ -920,24 +1064,31 @@
     ...     bs_projection=None,  # 能带的投影方式，None表示不投影
     ...     dos_projection="elements")  # 态密度的投影方式，None表示不投影
     >>> band_data = get_band_data(
     ...     band_dir='dspawpy_proj/dspawpy_tests/inputs/supplement/banddos/band.json',  # 能带数据
     ...     zero_to_efermi=True,  # 非金属体系应将零点能移动到费米能级
     ... )
     >>> dos_data = get_dos_data(dos_dir='dspawpy_proj/dspawpy_tests/inputs/supplement/banddos/dos.json')
-    >>> pltbd(bdp, band_data, dos_data, ylim=(-2,4), filename='imgs/newbd.png') # doctest: +ELLIPSIS
+    >>> pltbd(bdp, band_data, dos_data, ylim=(-2,4), filename='dspawpy_proj/dspawpy_tests/outputs/doctest/newbd.png') # doctest: +ELLIPSIS
     <module 'matplotlib.pyplot' from '.../matplotlib/pyplot.py'>
 
     与之前的版本对比:
 
     >>> bdp = BSDOSPlotter(bs_projection=None,dos_projection="elements")
     >>> plt = bdp.get_plot(bs=band_data, dos=dos_data)
 
     for old version pymatgen, it returns plt, otherwise may return axes, ref to userscripts for how to user them.
     """
+    import numpy as np
+
+    import palettable
+
+    if colors is None:
+        colors: list = palettable.colorbrewer.qualitative.Set1_9.mpl_colors  # type: ignore
+
     # self -> BSDOSPlotter
     bs_projection = bdp.bs_projection
     dos_projection = bdp.dos_projection
     vb_energy_range = bdp.vb_energy_range
     cb_energy_range = bdp.cb_energy_range
     fixed_cb_energy = bdp.fixed_cb_energy
     egrid_interval = bdp.egrid_interval
@@ -964,17 +1115,15 @@
     )
 
     if (
         bs_projection
         and bs_projection.lower() == "elements"
         and (len(elements) not in [2, 3, 4] or not bs.get_projection_on_elements())
     ):
-        import warnings
-
-        warnings.warn(
+        logger.warning(
             "Cannot get element projected data; either the projection data "
             "doesn't exist, or you don't have a compound with exactly 2 "
             "or 3 or 4 unique elements."
         )
         bs_projection = None
 
     # specify energy range of plot
@@ -1032,47 +1181,38 @@
         x_distances_list.append(x_distances)
 
     # set up bs and dos plot
     from matplotlib.gridspec import GridSpec
 
     gs = GridSpec(1, 2, width_ratios=[2, 1], wspace=0) if dos else GridSpec(1, 1)
 
+    import matplotlib.pyplot as plt
+
     fig = plt.figure(figsize=fig_size)
     fig.patch.set_facecolor("white")
     bs_ax = plt.subplot(gs[0])
-    if dos:
-        dos_ax = plt.subplot(gs[1])
-
     # set basic axes limits for the plot
     bs_ax.set_xlim(0, x_distances_list[-1][-1])
     emin = ylim[0] if ylim else emin
     emax = ylim[1] if ylim else emax
     bs_ax.set_ylim(emin, emax)
-    if dos:
-        dos_ax.set_ylim(emin, emax)
-
     # add BS xticks, labels, etc.
     bs_ax.set_xticks(xlabel_distances)
     bs_ax.set_xticklabels(xlabels, size=tick_fontsize)
     bs_ax.set_xlabel("Wavevector $k$", fontsize=axis_fontsize)
     bs_ax.set_ylabel("$E-E_F$ / eV", fontsize=axis_fontsize)
 
     # add BS fermi level line at E=0 and gridlines
     bs_ax.hlines(y=0, xmin=0, xmax=x_distances_list[-1][-1], color="k", lw=1, ls="--")
     bs_ax.set_yticks(np.arange(emin, emax + 1e-5, egrid_interval))
     bs_ax.set_yticklabels(
         np.arange(emin, emax + 1e-5, egrid_interval), size=tick_fontsize
     )
     bs_ax.set_axisbelow(True)
     bs_ax.grid(color=[0.5, 0.5, 0.5], linestyle="dotted", linewidth=1)
-    if dos:
-        dos_ax.set_yticks(np.arange(emin, emax + 1e-5, egrid_interval))
-        dos_ax.set_yticklabels([])
-        dos_ax.grid(color=[0.5, 0.5, 0.5], linestyle="dotted", linewidth=1)
-
     # renormalize the band energy to the Fermi level
     band_energies = {}
     spin_count = 0
     from pymatgen.electronic_structure.core import Spin
 
     for spin in (Spin.up, Spin.down):
         if spin in bs.bands:
@@ -1131,14 +1271,20 @@
                 loc=bs_legend,
             )
 
     # renormalize the DOS energies to Fermi level
     from pymatgen.electronic_structure.core import OrbitalType
 
     if dos:
+        dos_ax = plt.subplot(gs[1])
+        dos_ax.set_ylim(emin, emax)
+        dos_ax.set_yticks(np.arange(emin, emax + 1e-5, egrid_interval))
+        dos_ax.set_yticklabels([])
+        dos_ax.grid(color=[0.5, 0.5, 0.5], linestyle="dotted", linewidth=1)
+
         dos_energies = [e - dos.efermi for e in dos.energies]
         # Plot the DOS and projected DOS
         for spin in (Spin.up, Spin.down):
             if spin in dos.densities:
                 # plot the total DOS
                 dos_densities = dos.densities[spin] * int(spin)
                 label = "total" if spin == Spin.up else None
@@ -1219,35 +1365,38 @@
         # set up the DOS x-axis and add Fermi level line
         dos_ax.set_xlim(dos_xmin, dos_xmax)
         dos_ax.set_xticklabels([])
         dos_ax.hlines(y=0, xmin=dos_xmin, xmax=dos_xmax, color="k", lw=1, ls="--")
         dos_ax.set_xlabel("DOS", fontsize=axis_fontsize)
         dos_ax.set_ylim(emin, emax)
 
-    # add legend for DOS
-    if dos and dos_legend:
-        dos_ax.legend(
-            fancybox=True,
-            prop={"size": legend_fontsize},
-            loc=dos_legend,
-        )
+        # add legend for DOS
+        if dos_legend:
+            dos_ax.legend(
+                fancybox=True,
+                prop={"size": legend_fontsize},
+                loc=dos_legend,
+            )
 
     plt.subplots_adjust(wspace=0.1)
+    import os
+
     os.makedirs(os.path.dirname(os.path.abspath(filename)), exist_ok=True)
     plt.tight_layout()
     plt.savefig(filename, dpi=dpi)
     # plt.show()
 
     return plt
 
 
+@logger.catch
 def plot_dos(
     dosplotter,
-    xlim=None,
-    ylim=None,
+    xlim: Optional[Tuple[float, float]] = None,
+    ylim: Optional[Tuple[float, float]] = None,
     invert_axes: bool = False,
     beta_dashed: bool = False,
     raw: bool = False,
 ):
     """Get a matplotlib plot showing the DOS.
 
     Args:
@@ -1264,27 +1413,32 @@
         plt.Axes: matplotlib Axes object.
     """
     import palettable
     from pymatgen.util.plotting import pretty_plot
 
     n_colors = min(9, max(3, len(dosplotter._doses)))
 
-    colors = palettable.colorbrewer.qualitative.Set1_9.mpl_colors
+    # https://jiffyclub.github.io/palettable/colorbrewer/qualitative/
+    colors = palettable.colorbrewer.qualitative.Set1_9.mpl_colors  # type: ignore
 
     ys = None
     all_densities = []
     all_energies = []
     ax = pretty_plot(12, 8)  # may be plt for old pmg
+    import matplotlib.pyplot as plt
+
     if isinstance(ax, type(plt)):
-        ax = ax.gca()
+        ax = ax.gca()  # type: ignore
 
     # Note that this complicated processing of energies is to allow for
     # stacked plots in matplotlib.
     from pymatgen.electronic_structure.core import Spin
 
+    import numpy as np
+
     for dos in dosplotter._doses.values():
         energies = dos["energies"]
         densities = dos["densities"]
         if not ys:
             ys = {
                 Spin.up: np.zeros(energies.shape),
                 Spin.down: np.zeros(energies.shape),
@@ -1333,18 +1487,14 @@
                     ax.plot(
                         x, y, color=colors[idx % n_colors], label=str(key), linewidth=3
                     )
 
                 dd[f"key={key}_spin={spin}_x"] = x
                 dd[f"key={key}_spin={spin}_y"] = y
 
-    import pandas as pd
-
-    df = pd.DataFrame(dd)
-
     if xlim:
         ax.set_xlim(xlim)
     if ylim:
         ax.set_ylim(ylim)
     elif not invert_axes:
         xlim = ax.get_xlim()
         relevant_y = [p[1] for p in all_pts if xlim[0] < p[0] < xlim[1]]
@@ -1383,10 +1533,19 @@
     legend_text = (
         ax.get_legend().get_texts()
     )  # all the text.Text instance in the legend
     plt.setp(legend_text, fontsize=30)
     plt.tight_layout()
 
     if raw:
-        df.to_csv("dos_raw.csv", index=False)
+        try:
+            import polars as pl
+
+            df = pl.DataFrame(dd)
+            df.write_csv("dos_raw.csv")
+        except ModuleNotFoundError:
+            import pandas as pd
+
+            df = pd.DataFrame(dd)
+            df.to_csv("dos_raw.csv")
 
     return ax
```

### Comparing `dspawpy-1.2.2/dspawpy.egg-info/PKG-INFO` & `dspawpy-1.3.0/dspawpy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: dspawpy
-Version: 1.2.2
+Version: 1.3.0
 Summary: Tools for dspaw
 Home-page: http://www.hzwtech.com/
 Author: Hzwtech
 Author-email: ZhengZhilin@hzwtech.com
 License: MIT
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: pymatgen>=2022.2.7
+Requires-Dist: pymatgen
 Requires-Dist: statsmodels
 Requires-Dist: h5py
-Requires-Dist: monty
 Requires-Dist: prompt_toolkit
 Requires-Dist: loguru
+Requires-Dist: polars
+Requires-Dist: ruamel.yaml
 
 ![Pyversion](https://img.shields.io/badge/dynamic/json?query=info.requires_python&label=python&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fgeojson-rewind%2Fjson)
 ![PyPI](https://img.shields.io/pypi/v/dspawpy?label=pypi%20package)
 ![PyPI - Downloads](https://static.pepy.tech/badge/dspawpy/month)
 
 # Introduction （简介）
 
@@ -36,23 +37,44 @@
 
 ```bash
 conda install -c conda-forge dspawpy
 ```
 
 ## CHANGELOG （版本更新简述）
 
+### 1.3.0
+
+- 重要变更： 不再支持python3.8（不含）以下版本
+- 重要变更： 合并cli.py和cli_en.py，通过命令行选项 -l 或 --language 切换交互提示语言
+- 重构： 命令行交互程序增加静默运行模式，便于编程调用
+- 重构： 命令行交互程序大幅提高可读性，在等待用户输入同时多线程动态载入最终调用的函数
+- 重构： 懒导入——将导包语句从文件开头尽量移入函数中，避免导入不必要模块，减少导包耗时
+- 重构： 绝大多数参数补充类型提示，解决所有已知的静态检查问题
+- 体验优化： cli在输入部分参数时增加Tab键获取提示的功能
+- 体验优化： cli增加命令行参数帮助菜单
+- 体验优化： 全局使用 loguru 库的 catch 修饰器，控制报错信息的详细程度
+- 体验优化:  average_along_axis potential类型支持自动判断内部subtype类型为 TotalLocalPotential 的情况
+- 体验优化： 用 polars 库替换了 pandas 库，加速处理多维数据
+- BUG修复： write_vesta 插值体积数据部分变量未及时更新
+- BUG修复： rdf 修复 density 变量缺失的问题
+- BUG修复： cli 8.4 neb 
+
+
+### 1.2.2
+
+- BUG修复： dos和band读取非线性自旋算例的 h5/json 输出文件时，对自旋判断不准
+
 ### 1.2.0
 
-- 体验优化： 将导包语句从文件开头移入函数中，大幅减少python脚本的import时间
+- 体验优化： cli将导包语句从文件开头移入函数中，大幅减少python脚本的import时间
 - 体验优化： cli增加模糊匹配功能
 - 体验优化： optical绘图默认绘制全部数据以便查看
 - 体验优化： neb备份时如果目标文件夹已存在，将原先的改名成附加时间戳的文件夹
 - BUG修复： dos非线性自旋时无法读取h5/json数据
 
-
 ### 1.1.9
 
 - BUG修复： 修复cli的一些已知bug
 
 ### 1.1.8
 
 - 功能强化： 体数据（volumetric data）支持自定义网格插值（调用scipy的RegularGridInterpolator插值器）；增加 txt 格式支持，每行包含格点的 xyz 坐标和具体数值
```

### Comparing `dspawpy-1.2.2/dspawpy.egg-info/SOURCES.txt` & `dspawpy-1.3.0/dspawpy.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 dspawpy.egg-info/entry_points.txt
 dspawpy.egg-info/requires.txt
 dspawpy.egg-info/top_level.txt
 dspawpy/analysis/__init__.py
 dspawpy/analysis/aimdtools.py
 dspawpy/analysis/vacf.py
 dspawpy/cli/__init__.py
+dspawpy/cli/aux.py
 dspawpy/cli/cli.py
-dspawpy/cli/cli_en.py
+dspawpy/cli/menu_prompts.py
 dspawpy/diffusion/__init__.py
 dspawpy/diffusion/neb.py
 dspawpy/diffusion/nebtools.py
 dspawpy/diffusion/pathfinder.py
 dspawpy/io/__init__.py
 dspawpy/io/read.py
 dspawpy/io/structure.py
```

### Comparing `dspawpy-1.2.2/setup.py` & `dspawpy-1.3.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,40 @@
 # -*- coding: utf-8 -*-
 import os
-import sys
 from setuptools import find_packages, setup
 
 
 def read(fname):
     with open(
         os.path.join(os.path.abspath(os.path.dirname(__file__)), fname),
         "r",
         encoding="utf-8",
     ) as fin:
         return fin.read()
 
 
-if sys.version_info < (3, 8):
-    pmg_version = "pymatgen"
-    monty_version = "monty<=2021.12.1"  # removed os.path.which
-else:
-    pmg_version = "pymatgen >= 2022.2.7"  # removed monty os.path.which
-    monty_version = "monty"
-
 setup(
     name="dspawpy",
-    version="1.2.2",
+    version="1.3.0",
     packages=find_packages(),
     url="http://www.hzwtech.com/",
     license="MIT",
     author="Hzwtech",
     author_email="ZhengZhilin@hzwtech.com",
     description="Tools for dspaw",
     install_requires=[
-        pmg_version,
+        "pymatgen",
         "statsmodels",
-        "h5py",
-        monty_version,
-        # "statsmodels>=0.12.0",
-        # "h5py >= 3.7",
-        "prompt_toolkit",
-        "loguru",
-    ],  # numpy can be >=1.25, UserWarning about longdouble relates to WSL1, not numpy.
-    python_requires=">=3.6",
+        "h5py",  # parse h5
+        "prompt_toolkit",  # cli completer
+        "loguru",  # log
+        "polars",  # speed up pandas
+        "ruamel.yaml",  # ordered yaml
+    ],
+    python_requires=">=3.8",
     entry_points={
         "console_scripts": ["cli=dspawpy.cli.cli:main", "ecli=dspawpy.cli.cli_en:main"]
     },
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     license_files=("LICENSE.txt",),
 )
```

