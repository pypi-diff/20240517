# Comparing `tmp/tkintertools-2.6.9.dev1.tar.gz` & `tmp/tkintertools-3.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkintertools-2.6.9.dev1.tar", last modified: Tue Aug  8 12:13:25 2023, max compression
+gzip compressed data, was "tkintertools-3.0.0b1.tar", last modified: Fri May 17 15:40:55 2024, max compression
```

## Comparing `tkintertools-2.6.9.dev1.tar` & `tkintertools-3.0.0b1.tar`

### file list

```diff
@@ -1,16 +1,107 @@
-drwxrwxrwx   0        0        0        0 2023-08-08 12:13:25.989439 tkintertools-2.6.9.dev1/
--rw-rw-rw-   0        0        0     9267 2023-06-20 19:03:57.000000 tkintertools-2.6.9.dev1/LICENSE.txt
--rw-rw-rw-   0        0        0     8374 2023-08-08 12:13:25.988438 tkintertools-2.6.9.dev1/PKG-INFO
--rw-rw-rw-   0        0        0     7740 2023-08-08 12:03:46.000000 tkintertools-2.6.9.dev1/README.md
--rw-rw-rw-   0        0        0       42 2023-08-08 12:13:25.990482 tkintertools-2.6.9.dev1/setup.cfg
--rw-rw-rw-   0        0        0     1630 2023-08-08 11:58:13.000000 tkintertools-2.6.9.dev1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-08 12:13:25.961832 tkintertools-2.6.9.dev1/tkintertools/
--rw-rw-rw-   0        0        0     2304 2023-08-08 11:57:30.000000 tkintertools-2.6.9.dev1/tkintertools/__init__.py
--rw-rw-rw-   0        0        0    75263 2023-08-08 12:11:32.000000 tkintertools-2.6.9.dev1/tkintertools/__main__.py
--rw-rw-rw-   0        0        0     3373 2023-08-08 11:38:35.000000 tkintertools-2.6.9.dev1/tkintertools/constants.py
--rw-rw-rw-   0        0        0    24186 2023-08-04 04:36:12.000000 tkintertools-2.6.9.dev1/tkintertools/tools_3d.py
-drwxrwxrwx   0        0        0        0 2023-08-08 12:13:25.986970 tkintertools-2.6.9.dev1/tkintertools.egg-info/
--rw-rw-rw-   0        0        0     8374 2023-08-08 12:13:25.000000 tkintertools-2.6.9.dev1/tkintertools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-08-08 12:13:25.000000 tkintertools-2.6.9.dev1/tkintertools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 12:13:25.000000 tkintertools-2.6.9.dev1/tkintertools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-08-08 12:13:25.000000 tkintertools-2.6.9.dev1/tkintertools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.587236 tkintertools-3.0.0b1/
+-rw-rw-rw-   0        0        0     1086 2024-05-05 00:16:47.000000 tkintertools-3.0.0b1/LICENSE.txt
+-rw-rw-rw-   0        0        0       35 2024-05-17 15:40:16.000000 tkintertools-3.0.0b1/MANIFEST.in
+-rw-rw-rw-   0        0        0     8551 2024-05-17 15:40:55.585733 tkintertools-3.0.0b1/PKG-INFO
+-rw-rw-rw-   0        0        0     6093 2024-05-17 15:04:39.000000 tkintertools-3.0.0b1/README.md
+-rw-rw-rw-   0        0        0     1633 2024-05-17 15:40:29.000000 tkintertools-3.0.0b1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 15:40:55.587236 tkintertools-3.0.0b1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.481788 tkintertools-3.0.0b1/tkintertools/
+-rw-rw-rw-   0        0        0     2091 2024-05-16 02:19:58.000000 tkintertools-3.0.0b1/tkintertools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.491806 tkintertools-3.0.0b1/tkintertools/animation/
+-rw-rw-rw-   0        0        0       86 2024-05-12 12:01:21.000000 tkintertools-3.0.0b1/tkintertools/animation/__init__.py
+-rw-rw-rw-   0        0        0     9290 2024-05-17 11:46:35.000000 tkintertools-3.0.0b1/tkintertools/animation/animations.py
+-rw-rw-rw-   0        0        0     2838 2024-05-14 13:36:12.000000 tkintertools-3.0.0b1/tkintertools/animation/controllers.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.495807 tkintertools-3.0.0b1/tkintertools/color/
+-rw-rw-rw-   0        0        0       72 2024-05-12 12:31:18.000000 tkintertools-3.0.0b1/tkintertools/color/__init__.py
+-rw-rw-rw-   0        0        0    25979 2024-05-14 13:41:15.000000 tkintertools-3.0.0b1/tkintertools/color/colormap.py
+-rw-rw-rw-   0        0        0     3475 2024-05-16 09:27:41.000000 tkintertools-3.0.0b1/tkintertools/color/rgb.py
+-rw-rw-rw-   0        0        0      466 2024-05-17 14:58:42.000000 tkintertools-3.0.0b1/tkintertools/constants.py
+-rw-rw-rw-   0        0        0    39879 2024-05-17 12:42:32.000000 tkintertools-3.0.0b1/tkintertools/core.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.503823 tkintertools-3.0.0b1/tkintertools/standard/
+-rw-rw-rw-   0        0        0       53 2024-05-15 10:30:54.000000 tkintertools-3.0.0b1/tkintertools/standard/__init__.py
+-rw-rw-rw-   0        0        0     3842 2024-05-15 10:30:36.000000 tkintertools-3.0.0b1/tkintertools/standard/dialogs.py
+-rw-rw-rw-   0        0        0     8679 2024-05-17 11:51:34.000000 tkintertools-3.0.0b1/tkintertools/standard/features.py
+-rw-rw-rw-   0        0        0       27 2024-05-15 02:38:31.000000 tkintertools-3.0.0b1/tkintertools/standard/images.py
+-rw-rw-rw-   0        0        0     9544 2024-05-17 13:03:44.000000 tkintertools-3.0.0b1/tkintertools/standard/shapes.py
+-rw-rw-rw-   0        0        0     6496 2024-05-16 13:59:22.000000 tkintertools-3.0.0b1/tkintertools/standard/texts.py
+-rw-rw-rw-   0        0        0    12748 2024-05-17 12:43:13.000000 tkintertools-3.0.0b1/tkintertools/standard/widgets.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.507327 tkintertools-3.0.0b1/tkintertools/style/
+-rw-rw-rw-   0        0        0       72 2024-05-14 13:43:42.000000 tkintertools-3.0.0b1/tkintertools/style/__init__.py
+-rw-rw-rw-   0        0        0     2823 2024-05-17 00:33:42.000000 tkintertools-3.0.0b1/tkintertools/style/parser.py
+-rw-rw-rw-   0        0        0     3189 2024-05-17 00:34:04.000000 tkintertools-3.0.0b1/tkintertools/style/theme.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.465592 tkintertools-3.0.0b1/tkintertools/theme/
+drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.514842 tkintertools-3.0.0b1/tkintertools/theme/Button/
+-rw-rw-rw-   0        0        0      158 2024-05-14 03:31:24.000000 tkintertools-3.0.0b1/tkintertools/theme/Button/Information.dark.json
+-rw-rw-rw-   0        0        0      158 2024-05-14 03:31:35.000000 tkintertools-3.0.0b1/tkintertools/theme/Button/Information.light.json
+-rw-rw-rw-   0        0        0      251 2024-05-14 03:26:27.000000 tkintertools-3.0.0b1/tkintertools/theme/Button/Rectangle.dark.json
+-rw-rw-rw-   0        0        0      251 2024-05-14 03:31:53.000000 tkintertools-3.0.0b1/tkintertools/theme/Button/Rectangle.light.json
+-rw-rw-rw-   0        0        0      251 2024-05-14 03:21:08.000000 tkintertools-3.0.0b1/tkintertools/theme/Button/RoundedRectangle.dark.json
+-rw-rw-rw-   0        0        0      251 2024-05-14 03:32:22.000000 tkintertools-3.0.0b1/tkintertools/theme/Button/RoundedRectangle.light.json
+drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.522379 tkintertools-3.0.0b1/tkintertools/theme/CheckButton/
+-rw-rw-rw-   0        0        0      158 2024-05-14 03:33:07.000000 tkintertools-3.0.0b1/tkintertools/theme/CheckButton/Information.dark.json
+-rw-rw-rw-   0        0        0      158 2024-05-14 03:33:17.000000 tkintertools-3.0.0b1/tkintertools/theme/CheckButton/Information.light.json
+-rw-rw-rw-   0        0        0      251 2024-05-14 03:33:26.000000 tkintertools-3.0.0b1/tkintertools/theme/CheckButton/Rectangle.dark.json
+-rw-rw-rw-   0        0        0      251 2024-05-14 03:33:42.000000 tkintertools-3.0.0b1/tkintertools/theme/CheckButton/Rectangle.light.json
+-rw-rw-rw-   0        0        0      251 2024-05-14 03:34:03.000000 tkintertools-3.0.0b1/tkintertools/theme/CheckButton/RoundedRectangle.dark.json
+-rw-rw-rw-   0        0        0      251 2024-05-14 03:34:34.000000 tkintertools-3.0.0b1/tkintertools/theme/CheckButton/RoundedRectangle.light.json
+drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.532932 tkintertools-3.0.0b1/tkintertools/theme/Entry/
+-rw-rw-rw-   0        0        0      251 2024-05-14 03:36:45.000000 tkintertools-3.0.0b1/tkintertools/theme/Entry/Rectangle.dark.json
+-rw-rw-rw-   0        0        0      251 2024-05-14 03:36:56.000000 tkintertools-3.0.0b1/tkintertools/theme/Entry/Rectangle.light.json
+-rw-rw-rw-   0        0        0      251 2024-05-14 03:37:17.000000 tkintertools-3.0.0b1/tkintertools/theme/Entry/RoundedRectangle.in.dark.json
+-rw-rw-rw-   0        0        0      251 2024-05-14 03:37:41.000000 tkintertools-3.0.0b1/tkintertools/theme/Entry/RoundedRectangle.in.light.json
+-rw-rw-rw-   0        0        0      251 2024-05-14 08:40:52.000000 tkintertools-3.0.0b1/tkintertools/theme/Entry/RoundedRectangle.out.dark.json
+-rw-rw-rw-   0        0        0      251 2024-05-15 11:36:08.000000 tkintertools-3.0.0b1/tkintertools/theme/Entry/RoundedRectangle.out.light.json
+-rw-rw-rw-   0        0        0      158 2024-05-14 03:38:44.000000 tkintertools-3.0.0b1/tkintertools/theme/Entry/SingleLineText.dark.json
+-rw-rw-rw-   0        0        0      158 2024-05-14 03:38:55.000000 tkintertools-3.0.0b1/tkintertools/theme/Entry/SingleLineText.light.json
+drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.535931 tkintertools-3.0.0b1/tkintertools/theme/HighlightButton/
+-rw-rw-rw-   0        0        0      155 2024-05-14 03:47:15.000000 tkintertools-3.0.0b1/tkintertools/theme/HighlightButton/Information.dark.json
+-rw-rw-rw-   0        0        0      155 2024-05-14 03:47:23.000000 tkintertools-3.0.0b1/tkintertools/theme/HighlightButton/Information.light.json
+drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.537971 tkintertools-3.0.0b1/tkintertools/theme/Information/
+-rw-rw-rw-   0        0        0       55 2024-05-14 03:39:22.000000 tkintertools-3.0.0b1/tkintertools/theme/Information/Information.dark.json
+-rw-rw-rw-   0        0        0       55 2024-05-14 03:39:26.000000 tkintertools-3.0.0b1/tkintertools/theme/Information/Information.light.json
+drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.545976 tkintertools-3.0.0b1/tkintertools/theme/Label/
+-rw-rw-rw-   0        0        0      106 2024-05-14 03:39:38.000000 tkintertools-3.0.0b1/tkintertools/theme/Label/Information.dark.json
+-rw-rw-rw-   0        0        0      106 2024-05-14 03:39:46.000000 tkintertools-3.0.0b1/tkintertools/theme/Label/Information.light.json
+-rw-rw-rw-   0        0        0      168 2024-05-14 03:39:54.000000 tkintertools-3.0.0b1/tkintertools/theme/Label/Rectangle.dark.json
+-rw-rw-rw-   0        0        0      168 2024-05-14 03:40:00.000000 tkintertools-3.0.0b1/tkintertools/theme/Label/Rectangle.light.json
+-rw-rw-rw-   0        0        0      168 2024-05-14 03:40:15.000000 tkintertools-3.0.0b1/tkintertools/theme/Label/RoundedRectangle.dark.json
+-rw-rw-rw-   0        0        0      168 2024-05-14 03:40:29.000000 tkintertools-3.0.0b1/tkintertools/theme/Label/RoundedRectangle.light.json
+drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.556897 tkintertools-3.0.0b1/tkintertools/theme/ProgressBar/
+-rw-rw-rw-   0        0        0      168 2024-05-14 03:40:59.000000 tkintertools-3.0.0b1/tkintertools/theme/ProgressBar/Rectangle.in.dark.json
+-rw-rw-rw-   0        0        0      168 2024-05-14 03:41:06.000000 tkintertools-3.0.0b1/tkintertools/theme/ProgressBar/Rectangle.in.light.json
+-rw-rw-rw-   0        0        0      168 2024-05-14 03:40:44.000000 tkintertools-3.0.0b1/tkintertools/theme/ProgressBar/Rectangle.out.dark.json
+-rw-rw-rw-   0        0        0      168 2024-05-14 03:40:51.000000 tkintertools-3.0.0b1/tkintertools/theme/ProgressBar/Rectangle.out.light.json
+-rw-rw-rw-   0        0        0      168 2024-05-14 03:41:49.000000 tkintertools-3.0.0b1/tkintertools/theme/ProgressBar/SemicircularRectangle.in.dark.json
+-rw-rw-rw-   0        0        0      168 2024-05-14 03:42:04.000000 tkintertools-3.0.0b1/tkintertools/theme/ProgressBar/SemicircularRectangle.in.light.json
+-rw-rw-rw-   0        0        0      168 2024-05-14 03:41:21.000000 tkintertools-3.0.0b1/tkintertools/theme/ProgressBar/SemicircularRectangle.out.dark.json
+-rw-rw-rw-   0        0        0      168 2024-05-14 03:41:35.000000 tkintertools-3.0.0b1/tkintertools/theme/ProgressBar/SemicircularRectangle.out.light.json
+drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.568070 tkintertools-3.0.0b1/tkintertools/theme/RadioButton/
+-rw-rw-rw-   0        0        0      251 2024-05-14 03:42:37.000000 tkintertools-3.0.0b1/tkintertools/theme/RadioButton/Oval.in.dark.json
+-rw-rw-rw-   0        0        0      251 2024-05-14 03:42:47.000000 tkintertools-3.0.0b1/tkintertools/theme/RadioButton/Oval.in.light.json
+-rw-rw-rw-   0        0        0      251 2024-05-14 03:42:18.000000 tkintertools-3.0.0b1/tkintertools/theme/RadioButton/Oval.out.dark.json
+-rw-rw-rw-   0        0        0      251 2024-05-14 03:42:27.000000 tkintertools-3.0.0b1/tkintertools/theme/RadioButton/Oval.out.light.json
+-rw-rw-rw-   0        0        0      251 2024-05-14 03:42:37.000000 tkintertools-3.0.0b1/tkintertools/theme/RadioButton/Rectangle.in.dark.json
+-rw-rw-rw-   0        0        0      251 2024-05-14 03:42:47.000000 tkintertools-3.0.0b1/tkintertools/theme/RadioButton/Rectangle.in.light.json
+-rw-rw-rw-   0        0        0      251 2024-05-15 09:23:07.000000 tkintertools-3.0.0b1/tkintertools/theme/RadioButton/Rectangle.out.dark.json
+-rw-rw-rw-   0        0        0      251 2024-05-15 09:23:20.000000 tkintertools-3.0.0b1/tkintertools/theme/RadioButton/Rectangle.out.light.json
+drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.578179 tkintertools-3.0.0b1/tkintertools/theme/Switch/
+-rw-rw-rw-   0        0        0      520 2024-05-14 03:51:34.000000 tkintertools-3.0.0b1/tkintertools/theme/Switch/Oval.dark.json
+-rw-rw-rw-   0        0        0      520 2024-05-14 03:51:45.000000 tkintertools-3.0.0b1/tkintertools/theme/Switch/Oval.light.json
+-rw-rw-rw-   0        0        0      520 2024-05-14 03:51:56.000000 tkintertools-3.0.0b1/tkintertools/theme/Switch/Rectangle.in.dark.json
+-rw-rw-rw-   0        0        0      520 2024-05-14 03:52:05.000000 tkintertools-3.0.0b1/tkintertools/theme/Switch/Rectangle.in.light.json
+-rw-rw-rw-   0        0        0      520 2024-05-14 03:52:17.000000 tkintertools-3.0.0b1/tkintertools/theme/Switch/Rectangle.out.dark.json
+-rw-rw-rw-   0        0        0      520 2024-05-14 03:52:29.000000 tkintertools-3.0.0b1/tkintertools/theme/Switch/Rectangle.out.light.json
+-rw-rw-rw-   0        0        0      520 2024-05-14 03:53:29.000000 tkintertools-3.0.0b1/tkintertools/theme/Switch/SemicircularRectangle.dark.json
+-rw-rw-rw-   0        0        0      520 2024-05-14 03:54:12.000000 tkintertools-3.0.0b1/tkintertools/theme/Switch/SemicircularRectangle.light.json
+drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.580733 tkintertools-3.0.0b1/tkintertools/theme/UnderlineButton/
+-rw-rw-rw-   0        0        0      159 2024-05-14 03:46:16.000000 tkintertools-3.0.0b1/tkintertools/theme/UnderlineButton/Information.dark.json
+-rw-rw-rw-   0        0        0      154 2024-05-14 03:46:25.000000 tkintertools-3.0.0b1/tkintertools/theme/UnderlineButton/Information.light.json
+drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.582733 tkintertools-3.0.0b1/tkintertools/three/
+-rw-rw-rw-   0        0        0       47 2024-05-14 13:48:22.000000 tkintertools-3.0.0b1/tkintertools/three/__init__.py
+-rw-rw-rw-   0        0        0    27170 2024-05-16 06:52:58.000000 tkintertools-3.0.0b1/tkintertools/three/engine.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.584732 tkintertools-3.0.0b1/tkintertools.egg-info/
+-rw-rw-rw-   0        0        0     8551 2024-05-17 15:40:55.000000 tkintertools-3.0.0b1/tkintertools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3850 2024-05-17 15:40:55.000000 tkintertools-3.0.0b1/tkintertools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 15:40:55.000000 tkintertools-3.0.0b1/tkintertools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-05-17 15:40:55.000000 tkintertools-3.0.0b1/tkintertools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-17 15:40:55.000000 tkintertools-3.0.0b1/tkintertools.egg-info/top_level.txt
```

### Comparing `tkintertools-2.6.9.dev1/tkintertools/tools_3d.py` & `tkintertools-3.0.0b1/tkintertools/three/engine.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,661 +1,716 @@
-""" 3D support """
+"""
+core codes of 3D
 
-import math  # 数学支持
-import statistics  # 数据统计
-from tkinter import Event  # 类型提示
-from typing import Iterable, overload  # 类型提示
+WARNING:
 
-from .__main__ import Canvas, Tk, Toplevel  # 继承和类型提示
-from .constants import *  # 常量
+The contents of this file are ported from tkt 2 and haven't been modified too much,
+there may be some issues!
+"""
 
+import array
+import math
+import platform
+import statistics
+import tkinter
+import typing
 
-class Canvas_3D(Canvas):
-    """ 3D 画布基类 """
+from .. import constants, core
+
+
+class Canvas3D(core.Canvas):
+    """3D 画布基类"""
 
     def __init__(
         self,
-        master,  # type: Tk | Toplevel
-        width,  # type: int
-        height,  # type: int
-        x=None,  # type: int | None
-        y=None,  # type: int | None
+        master: core.Tk | core.Toplevel | core.NestedToplevel | core.Canvas,
         *,
-        lock=True,  # type: bool
-        expand=True,  # type: bool
-        keep=True,  # type: bool
-        camera_distance=CAMERA_DISTANCE,  # type: float
-        **kw
-    ):  # type: (...) -> None
-        """
-        `master`: 父控件 \ 
-        `width`: 画布宽度 \ 
-        `height`: 画布高度 \ 
-        `x`: 画布左上角的横坐标 \ 
-        `y`: 画布左上角的纵坐标 \ 
-        `lock`: 画布内控件的功能锁，为 False 时功能暂时失效 \ 
-        `expand`: 画布内控件是否能缩放 \ 
-        `keep`: 画布比例是否保持不变 \ 
-        `camera_distance`: 相机位置与原点间的距离，默认值为 1000 \ 
-        `**kw`: 与 tkinter.Canvas 类的参数相同
-        """
-        Canvas.__init__(
-            self, master, width, height, x, y, lock=lock, expand=expand, keep=keep, **kw)
-        self.distance = camera_distance
-        self._items_3d = []  # type: list[Point | Line | Side]
-        self._geos = []  # type: list[Geometry]
-        self._zoom()  # 更新画布视野
-
-    def _zoom(self, rate_x=None, rate_y=None):  # type: (float | None, float | None) -> None
-        # override: 保持画布视野居中
-        Canvas._zoom(self, rate_x, rate_y)
-        half_width, half_height = self.width[1] / 2, self.height[1] / 2
-        self.configure(
-            scrollregion=(-half_width, -half_height, half_width, half_height))
+        expand: typing.Literal["", "x", "y", "xy"] = "xy",
+        zoom_item: bool = False,
+        keep_ratio: typing.Literal["min", "max", "full"] | None = None,
+        free_anchor: bool = False,
+        **kw,
+    ) -> None:
+        """"""
+        core.Canvas.__init__(
+            self, master, expand=expand, zoom_item=zoom_item,
+            keep_ratio=keep_ratio, free_anchor=free_anchor, **kw)
+        self._items_3d: list[Point | Line | Side] = []
+        self._geos: list[Point | Line | Side] = []
+        self._distance: int = 1000
+
+    def distance(self, value: int | None = None) -> int | None:
+        """"""
+        if value is None:
+            return self._distance
+        self._distance = value
 
-    def items_3d(self):  # type: () -> tuple[Point | Line | Side]
-        """ 返回 `Canvas_3d` 类全部的基本 3D 对象 """
+    def items_3d(self) -> tuple["Point | Line | Side", ...]:
+        """返回 `Canvas3D` 类全部的基本 3D 对象"""
         return tuple(self._items_3d)
 
-    def geos(self):  # type: () -> tuple[Geometry]
-        """ 返回 `Canvas_3d` 类全部的几何体对象 """
+    def geos(self) -> tuple["Geometry", ...]:
+        """返回 `Canvas3D` 类全部的几何体对象"""
         return tuple(self._geos)
 
-    def space_sort(self):  # type: () -> None
-        """ 空间位置排序 """  # BUG: 在距离比较近的两个对象时，仍会显示不正确
+    def space_sort(self) -> None:
+        """空间位置排序"""
         self._items_3d.sort(key=lambda item: item._camera_distance())
         for item in self._items_3d:
             self.lower(item.item)
 
 
-class Space(Canvas_3D):
-    """ 三维空间 """
+class Space(Canvas3D):
+    """三维空间"""
 
     def __init__(
         self,
-        master,  # type: Tk | Toplevel
-        width,  # type: int
-        height,  # type: int
-        x=None,  # type: int | None
-        y=None,  # type: int | None
+        master: core.Tk | core.Toplevel | core.NestedToplevel | core.Canvas,
         *,
-        lock=True,  # type: bool
-        expand=True,  # type: bool
-        keep=True,  # type: bool
-        camera_distance=CAMERA_DISTANCE,  # type: float
-        origin_size=ORIGIN_SIZE,  # type: float
-        origin_width=ORIGIN_WIDTH,  # type: float
-        origin_fill=ORIGIN_FILL,  # type: str
-        origin_outline=ORIGIN_OUTLINE,  # type: str
-        **kw
-    ):  # type: (...) -> None
-        """
-        `master`: 父控件 \ 
-        `width`: 画布宽度 \ 
-        `height`: 画布高度 \ 
-        `x`: 画布左上角的横坐标 \ 
-        `y`: 画布左上角的纵坐标 \ 
-        `lock`: 画布内控件的功能锁，为 False 时功能暂时失效 \ 
-        `expand`: 画布内控件是否能缩放 \ 
-        `keep`: 画布比例是否保持不变 \ 
-        `camera_distance`: 相机位置与原点间的距离，默认值为 1000 \ 
-        `origin_size`: 原点大小，默认值为 1 \ 
-        `origin_width`: 原点轮廓宽度，默认值为 1 \ 
-        `origin_fill`: 原点填充颜色，默认为无色 \ 
-        `origin_outline`: 原点轮廓颜色，默认为无色 \ 
-        `**kw`: 与 tkinter.Canvas 类的参数相同
-        """
-        Canvas_3D.__init__(
-            self, master, width, height, x, y, lock=lock, expand=expand, keep=keep, camera_distance=camera_distance, **kw)
-        self._origin = Point(
-            self, ORIGIN_COORDINATE, size=origin_size, width=origin_width, fill=origin_fill, outline=origin_outline)
+        expand: typing.Literal["", "x", "y", "xy"] = "xy",
+        zoom_item: bool = False,
+        keep_ratio: typing.Literal["min", "max", "full"] | None = None,
+        free_anchor: bool = False,
+        **kw,
+    ) -> None:
+        """"""
+        Canvas3D.__init__(
+            self, master, expand=expand, zoom_item=zoom_item,
+            keep_ratio=keep_ratio, free_anchor=free_anchor, **kw)
+        self._bind_event()
+
+    def _zoom_init(self) -> None:
+        Canvas3D._zoom_init(self)
+        self._origin = Point(self, (0, 0, 0), size=1,
+                             width=1, fill="", outline="")
         self._items_3d.clear()
-        self.bind('<B3-Motion>', self._translate)
-        self.bind('<Button-3>', lambda _: self._translate(_, True))
-        self.bind('<ButtonRelease-3>', lambda _: self._translate(_, False))
-        self.bind('<B1-Motion>', self._rotate)
-        self.bind('<Button-1>', lambda _: self._rotate(_, True))
-        self.bind('<ButtonRelease-1>', lambda _: self._rotate(_, False))
-        if SYSTEM == 'Linux':  # 兼容 Linux 系统
-            self.bind('<Button-4>', lambda _: self._scale(_, True))
-            self.bind('<Button-5>', lambda _: self._scale(_, False))
+
+    def _zoom(self) -> None:
+        """"""
+        Canvas3D._zoom(self)
+        self.update_idletasks()
+        for item in self._items_3d:
+            item.update()
+        self.space_sort()
+
+    def _bind_event(self) -> None:
+        """"""
+        self.bind("<B3-Motion>", self._translate, "+")
+        self.bind("<Button-3>", lambda event: self._translate(event, True), "+")
+        self.bind("<ButtonRelease-3>",
+                  lambda event: self._translate(event, False), "+")
+        self.bind("<B1-Motion>", self._rotate, "+")
+        self.bind("<Button-1>", lambda event: self._rotate(event, True), "+")
+        self.bind("<ButtonRelease-1>",
+                  lambda event: self._rotate(event, False), "+")
+        if platform.system() == "Linux":  # 兼容 Linux 系统
+            self.bind("<Button-4>", lambda event: self._scale(event, True), "+")
+            self.bind("<Button-5>", lambda event: self._scale(event, False), "+")
         else:
-            self.bind('<MouseWheel>', self._scale)
+            self.bind("<MouseWheel>", self._scale, "+")
 
-    def _translate(self, event, flag=None, _cache=[]):
-        # type: (Event, bool | None, list[float]) -> None
-        """ 平移事件 """
+    def _translate(self, event: tkinter.Event, flag: bool | None = None, _cache: list[float] = []) -> None:
+        """平移事件"""
         if flag is True:  # 按下
             _cache[:] = [event.x, event.y]
-            return self.configure(cursor='fleur')
+            self.configure(cursor="fleur")
+            return
         elif flag is False:  # 松开
-            return self.configure(cursor='arrow')
-        dx, dy = event.x-_cache[0], event.y-_cache[1]
+            self.configure(cursor="arrow")
+            return
+        dx, dy = event.x - _cache[0], event.y - _cache[1]
         _cache[:] = [event.x, event.y]
-        for item in self._items_3d+[self._origin]:
+        for item in self._items_3d + [self._origin]:
             item.translate(
-                0, dx*self.width[0]/self.width[1], dy*self.height[0]/self.height[1])
+                0, dx*self._initial_size[0]/self._size[0], -dy*self._initial_size[1]/self._size[1])
             item.update()
         self.space_sort()
 
     def _rotate(self, event, flag=None, _cache=[]):
-        # type: (Event, bool | None, list[float]) -> None
-        """ 旋转事件 """
-        if flag is True:
-            _cache[:] = [event.x, event.y]
-            return self.configure(cursor='fleur')
-        elif flag is False:
-            return self.configure(cursor='arrow')
-        dx, dy = event.x-_cache[0], event.y-_cache[1]
+        # type: (tkinter.Event, bool | None, list[float]) -> None
+        """旋转事件"""
+        if flag is False:
+            # if self._release(event):  # 兼容原 core.Canvas
+            #     return
+            self.configure(cursor="arrow")
+            return
+        else:
+            if flag is True:
+                _cache[:] = [event.x, event.y]
+            # if self._click(event):
+            #     return
+            if flag is True:
+                self.configure(cursor="fleur")
+                return
+        dx, dy = event.x - _cache[0], event.y - _cache[1]
         _cache[:] = [event.x, event.y]
         for item in self._items_3d:
-            item.rotate(0, -2*dy/self.width[1]*math.tau, 2*dx /
-                        self.height[1]*math.tau, center=self._origin.coordinates[0])
+            item.rotate(0, 2*dy/self._size[0]*math.tau, 2*dx/self._size[1]*math.tau,
+                        center=self._origin.coordinates[0])
             item.update()
         self.space_sort()
 
-    def _scale(self, event, flag=None):  # type: (Event, bool | None) -> None
-        """ 缩放事件 """
+    def _scale(self, event: tkinter.Event, flag: bool | None = None) -> None:
+        """缩放事件"""
         if flag is not None:
             event.delta = flag
         k = 1.1 if event.delta > 0 else 0.9
         for item in self._items_3d:
             item.scale(k, k, k, center=self._origin.coordinates[0])
             item.update()
         self.space_sort()
 
 
-def translate(coordinate, dx=0, dy=0, dz=0):
-    # type: (list[float], float, float, float) -> None
-    """
-    ### 平移
-    将一个三维空间中的点进行平移 \n
-    ---
-    `coordinate`: 点的空间坐标 \ 
-    `dx`: x 方向位移长度 \ 
-    `dy`: y 方向位移长度 \ 
-    `dz`: z 方向位移长度
+def translate(coordinate: tuple[float, float, float], dx: float = 0, dy: float = 0, dz: float = 0) -> None:
+    """将一个三维空间中的点进行平移
+
+    * `coordinate`: 点的空间坐标
+    * `dx`: x 方向位移长度
+    * `dy`: y 方向位移长度
+    * `dz`: z 方向位移长度
     """
     for i, delta in enumerate((dx, dy, dz)):
         coordinate[i] += delta
 
 
-@overload
+@typing.overload
 def rotate(coordinate, dx=0, dy=0, dz=0, *, center):
-    # type: (list[float], float, float, float, ..., Iterable[float]) -> None
+    # type: (tuple[float, float, float], float, float, float, ..., tuple[float, float, float]) -> None
     ...
 
 
-@overload
+@typing.overload
 def rotate(coordinate, dx=0, *, axis):
-    # type: (list[float], float,  ..., Iterable[Iterable[float]]) -> None
+    # type: (tuple[float, float, float], float,  ..., tuple[tuple[float, float, float], tuple[float, float, float]]) -> None
     ...
 
 
 def rotate(coordinate, dx=0, dy=0, dz=0, *, center, axis=None):
-    # type: (list[float], float, float, float, ..., Iterable[float], Iterable[Iterable[float]] | None) -> None
-    """
-    ### 旋转
-    将一个三维空间中的点以一个点或线为参照进行旋转 \n
-    ---
-    `coordinate`: 点的空间坐标 \ 
-    `dx`: x 方向旋转弧度，或者绕旋转轴线的旋转弧度 \ 
-    `dy`: y 方向旋转弧度 \ 
-    `dz`: z 方向旋转弧度 \ 
-    `center`: 旋转中心的空间坐标 \ 
-    `axis`: 旋转轴线的空间坐标
+    # type: (tuple[float, float, float], float, float, float, ..., tuple[float, float, float], tuple[tuple[float, float, float], tuple[float, float, float]] | None) -> None
+    """将一个三维空间中的点以一个点或线为参照进行旋转（实现方式为欧拉角）
+
+    * `coordinate`: 点的空间坐标
+    * `dx`: x 方向逆时针旋转弧度，或者绕旋转轴线的旋转弧度
+    * `dy`: y 方向逆时针旋转弧度
+    * `dz`: z 方向逆时针旋转弧度
+    * `center`: 旋转中心的空间坐标
+    * `axis`: 旋转轴线的空间坐标
     """
     if axis is not None:  # 参照为线（定轴转动）
-        center = _Line(*axis).center()  # 旋转轴中点
+        center = _Object3D(*axis).center()  # 旋转轴中点
         n = list(axis[0])
         for i in range(3):
             n[i] -= axis[1][i]
             coordinate[i] -= center[i]
         n_m = math.hypot(*n)
         for i in range(3):
             n[i] /= n_m
-        x_2, y_2, z_2 = map(lambda _: _**2, n)
+        x_2, y_2, z_2 = map(lambda _: _*_, n)
         zx, xy, yz = [n[i-1]*v for i, v in enumerate(n)]
         s_θ, c_θ = math.sin(dx), math.cos(dx)
         _c_θ = 1 - c_θ
 
-        matrix = [[x_2*_c_θ + c_θ, xy*_c_θ + n[2]*s_θ, zx*_c_θ - n[1]*s_θ],
-                  [xy*_c_θ - n[2]*s_θ, y_2*_c_θ + c_θ, yz*_c_θ + n[0]*s_θ],
-                  [zx*_c_θ + n[1]*s_θ, yz*_c_θ - n[0]*s_θ, z_2*_c_θ + c_θ]]
+        matrix = [
+            [x_2*_c_θ + c_θ, xy*_c_θ + n[2]*s_θ, zx*_c_θ - n[1]*s_θ],
+            [xy*_c_θ - n[2]*s_θ, y_2*_c_θ + c_θ, yz*_c_θ + n[0]*s_θ],
+            [zx*_c_θ + n[1]*s_θ, yz*_c_θ - n[0]*s_θ, z_2*_c_θ + c_θ]
+        ]
 
         for i, δ in enumerate(center):
             matrix[i] = δ + sum(matrix[i][j]*coordinate[j] for j in range(3))
 
     else:  # 参照为点（定点转动）
         sx, sy, sz = math.sin(dx), math.sin(dy), math.sin(dz)
         cx, cy, cz = math.cos(dx), math.cos(dy), math.cos(dz)
 
-        matrix = [[cz * cy, cz * sy * sx - sz * cx, cz * sy * cx + sz * sx],
-                  [sz * cy, sz * sy * sx + cz * cx, sz * sy * cx - cz * sx],
-                  [-sy,     cy * sx,                cy * cx]]
+        matrix = [
+            [cz*cy, cz*sy*sx - sz*cx, cz*sy*cx + sz*sx],
+            [sz*cy, sz*sy*sx + cz*cx, sz*sy*cx - cz*sx],
+            [-sy, cy*sx, cy*cx]
+        ]
 
         for i, δ in enumerate(center):
-            matrix[i] = δ + sum(
-                matrix[i][j] * (coordinate[j] - center[j]) for j in range(3))
+            matrix[i] = δ + sum(matrix[i][j] * (coordinate[j]-center[j])
+                                for j in range(3))
 
-    coordinate[:] = matrix
+    for i, mat in enumerate(matrix):
+        coordinate[i] = mat
 
 
 def scale(coordinate, kx=1, ky=1, kz=1, *, center):
-    # type: (list[float], float, float, float, ..., Iterable[float]) -> None
-    """
-    ### 缩放
-    将一个三维空间中的点以另一个点为缩放中心进行缩放 \n
-    ---
-    `coordinate`: 点的空间坐标 \ 
-    `kx`: x 方向缩放比例 \ 
-    `ky`: y 方向缩放比例 \ 
-    `kz`: z 方向缩放比例 \ 
-    `center`: 缩放中心的空间坐标
+    # type: (tuple[float, float, float], float, float, float, ..., tuple[float, float, float]) -> None
+    """将一个三维空间中的点以另一个点为缩放中心进行缩放
+
+    * `coordinate`: 点的空间坐标
+    * `kx`: x 方向缩放比例
+    * `ky`: y 方向缩放比例
+    * `kz`: z 方向缩放比例
+    * `center`: 缩放中心的空间坐标
     """
-    if kx <= 0 or ky <= 0 or kz <= 0:  # 限制缩放比例的范围
-        raise ValueError('invalid scaling factor')
     for i, k in enumerate((kx, ky, kz)):
-        coordinate[i] += (coordinate[i] - center[i]) * (k - 1)
+        coordinate[i] += (coordinate[i] - center[i]) * (k-1)
 
 
-class _3D_Object:
-    """ 3D 对象基类 """
+def project(coordinate, distance):
+    # type: (tuple[float, float, float], float) -> tuple[float, float]
+    """将一个三维空间中的点投影到指定距离的正向平面上，并返回在该平面上的坐标
 
-    def __init__(self, *coordinates):  # type: (list[float]) -> None
-        self.coordinates = list(coordinates)  # 所有点的坐标
+    * `coordinate`: 点的空间坐标
+    * `distance`: 正向平面的距离（平面正对着我们）
+    """
+    relative_dis = distance - coordinate[0]
+    if relative_dis <= 1e-16:
+        return [math.inf]*2
+    k = distance / relative_dis
+    return coordinate[1]*k, coordinate[2]*k
+
+
+class _Object3D:
+    """3D 对象基类"""
+
+    def __init__(self, *coordinates):
+        # type: (tuple[float, float, float]) -> None
+        self.coordinates = [array.array("f", lst) for lst in coordinates]
 
     def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
-        """
-        ### 平移
-        `dx`: x 方向位移长度 \ 
-        `dy`: y 方向位移长度 \ 
-        `dz`: z 方向位移长度
+        """平移对象本身
+
+        * `dx`: x 方向位移长度
+        * `dy`: y 方向位移长度
+        * `dz`: z 方向位移长度
         """
         for coordinate in self.coordinates:
             translate(coordinate, dx, dy, dz)
 
-    @overload
-    def rotate(self, dx=0, dy=0, dz=0, *, center=ROTATE_CENTER):
-        # type: (float, float, float, ..., Iterable[float]) -> None
+    @typing.overload
+    def rotate(self, dx=0, dy=0, dz=0, *, center=(0, 0, 0)):
+        # type: (float, float, float, ..., tuple[float, float, float]) -> None
         ...
 
-    @overload
+    @typing.overload
     def rotate(self, dx=0, *, axis):
-        # type: (float, ..., Iterable[Iterable[float]]) -> None
+        # type: (float, ..., tuple[tuple[float, float, float], tuple[float, float, float]]) -> None
         ...
 
-    def rotate(self, dx=0, dy=0, dz=0, *, center=ROTATE_CENTER, axis=None):
-        # type: (float, float, float, ..., Iterable[float], Iterable[Iterable[float]] | None) -> None
-        """
-        ### 旋转
-        `dx`: x 方向旋转弧度，或者绕旋转轴线的旋转弧度 \ 
-        `dy`: y 方向旋转弧度 \ 
-        `dz`: z 方向旋转弧度 \ 
-        `center`: 旋转中心，默认为原点 \ 
-        `axis`: 旋转轴线，无默认值
+    def rotate(self, dx=0, dy=0, dz=0, *, center=(0, 0, 0), axis=None):
+        # type: (float, float, float, ..., tuple[float, float, float], tuple[tuple[float, float, float], tuple[float, float, float]] | None) -> None
+        """旋转对象本身
+
+        * `dx`: x 方向逆时针旋转弧度，或者绕旋转轴线的旋转弧度
+        * `dy`: y 方向逆时针旋转弧度
+        * `dz`: z 方向逆时针旋转弧度
+        * `center`: 旋转中心，默认为原点
+        * `axis`: 旋转轴线，无默认值
         """
         for coordinate in self.coordinates:
             rotate(coordinate, dx, dy, dz, center=center, axis=axis)
 
     def scale(self, kx=1, ky=1, kz=1, *, center=None):
-        # type: (float, float, float, ..., Iterable[float] | None) -> None
-        """
-        ### 缩放
-        `kx`: x 方向缩放比例 \ 
-        `ky`: y 方向缩放比例 \ 
-        `kz`: z 方向缩放比例 \ 
-        `center`: 缩放中心，默认为几何中心
+        # type: (float, float, float, ..., tuple[float, float, float] | None) -> None
+        """缩放对象本身
+
+        * `kx`: x 方向缩放比例
+        * `ky`: y 方向缩放比例
+        * `kz`: z 方向缩放比例
+        * `center`: 缩放中心，默认为几何中心
         """
         if center is None:
             center = self.center()
         for coordinate in self.coordinates:
             scale(coordinate, kx, ky, kz, center=center)
 
     def center(self):  # type: () -> tuple[float, float, float]
-        """ 几何中心 """
+        """几何中心"""
         return tuple(statistics.mean(xyz) for xyz in zip(*self.coordinates))
 
-    def _project(self, distance):
-        """
-        ### 投影
-        `distance`: 对象与观察者的距离
-        """
-        # NOTE: 这里可能需要一些优化
-
-
-class _Point(_3D_Object):
-    """ 点（基类） """
-
-    def __init__(self, coordinate):  # type: (list[float]) -> None
-        _3D_Object.__init__(self, coordinate)
+    def _project(self, distance, canvas=None):
+        # type: (float, Canvas3D | Space | None) -> list[tuple[float, float]]
+        """投影对象自身
+
+        * `distance`: 对象与观察者的距离
+        * `canvas`: 投影到的画布
+        """
+        lst = [project(point, distance) for point in self.coordinates]
+        if canvas is not None:
+            lst = [(pos[0] + canvas._initial_size[0]/2, canvas._initial_size[1]/2 - pos[1])
+                   for pos in lst]
+        return lst
 
-    def _project(self, distance):  # type: (float) -> list[float]
-        # override: 具体的实现
-        relative_dis = distance - self.coordinates[0][0]
-        if relative_dis <= 1e-16:
-            return [float('inf')]*2  # BUG: 目前超出范围只能让其消失
-        k = distance/relative_dis
-        return [self.coordinates[0][1]*k, self.coordinates[0][2]*k]
 
-
-class _Line(_3D_Object):
-    """ 线（基类） """
+class Point(_Object3D):
+    """点"""
 
     def __init__(
         self,
-        start,  # type: list[float]
-        end,  # type: list[float]
+        canvas,  # type: Canvas3D | Space
+        coords,  # type: tuple[float, float, float]
+        *,
+        size=1,  # type: float
+        width=1,  # type: float
+        fill="#000000",  # type: str
+        outline="#000000",  # type: str
+        markuptext="",  # type: str
+        markupdelta=(0, 0),  # type: tuple[float, float]
+        markupfont=(constants.FONT, constants.SIZE),
+        # type: tuple[str, int, str]
+        markupfill="#000000",  # type: str
+        markupjustify="center",  # type: str
     ):  # type: (...) -> None
-        _3D_Object.__init__(self, start, end)
-        self.points = [_Point(start), _Point(end)]
-
-    def _project(self, distance):  # type: (float) -> list[list[float]]
-        # override: 具体的实现
-        return [point._project(distance) for point in self.points]
-
-
-class _Side(_3D_Object):
-    """ 面（基类） """
+        """
+        * `canvas`: 父画布
+        * `coords`: 点的空间坐标
+        * `size`: 点的大小
+        * `width`: 点轮廓的宽度
+        * `fill`: 点内部的填充颜色
+        * `outline`: 点轮廓的颜色
+        * `markuptext`: 标记文本
+        * `markupdelta`: 标记文本显示位置的偏移量
+        * `markupfont`: 标记文本字体
+        * `markupfill`: 标记文本颜色
+        * `markupjustify`: 标记文本多行对齐方式
+        """
+        _Object3D.__init__(self, list(coords))
+        canvas._items_3d.append(self)
+        self.canvas = canvas
+        self.size = size
+        self.width = width
+        self.fill = fill
+        self.item = canvas.create_oval(-1, -1, -1, -1,
+                                       fill=fill, outline=outline, width=width)
+        self.text = None
+        if markuptext:
+            self.text = canvas.create_text(-1, -1, text=markuptext,
+                                           font=markupfont, fill=markupfill, justify=markupjustify)
+            self.delta = markupdelta
+        self.update()
 
-    def __init__(self, *coordinates):  # type: (list[float]) -> None
-        _3D_Object.__init__(self, *coordinates)
-        self.lines = [_Line(coordinates[index-1], coordinate)
-                      for index, coordinate in enumerate(coordinates)]
+    def update(self):  # type: () -> None
+        """更新对象的显示"""
+        x, y = self._project(self.canvas._distance, self.canvas)[0]
+        self.canvas.coords(self.item, (x-self.size) * self.canvas._ratio[0], (y-self.size) *
+                           self.canvas._ratio[1], (x+self.size) * self.canvas._ratio[0], (y+self.size) * self.canvas._ratio[1])
+        if self.text is not None:
+            self.canvas.coords(
+                self.text, (x+self.delta[0]) * self.canvas._ratio[0], (y-self.delta[1]) * self.canvas._ratio[1])
 
-    def _project(self, distance):  # type: (float) -> list[list[list[float]]]
-        # override: 具体的实现
-        return [line._project(distance) for line in self.lines]
+    def _camera_distance(self):  # type: () -> float
+        """与相机距离"""
+        sign = math.copysign(1, self.canvas._distance - self.coordinates[0][0])
+        return sign * math.dist([self.canvas._distance, 0, 0], self.coordinates[0])
 
 
-class Point(_Point):
-    """ 点 """
+class Line(_Object3D):
+    """线"""
 
     def __init__(
         self,
-        canvas,  # type: Canvas_3D | Space
-        coords,  # type: Iterable[float]
+        canvas,  # type: Canvas3D | Space
+        point_start,  # type: tuple[float, float, float]
+        point_end,  # type: tuple[float, float, float]
         *,
-        size=POINT_SIZE,  # type: float
-        width=POINT_WIDTH,  # type: float
-        fill=COLOR_POINT_FILL,  # type: str
-        outline=COLOR_POINT_OUTLINE,  # type: str
+        width=1,  # type: float
+        fill="#000000",  # type: str
     ):  # type: (...) -> None
         """
-        `canvas`: 父画布 \ 
-        `coords`: 点的空间坐标 \ 
-        `size`: 点的大小 \ 
-        `width`: 点轮廓的宽度 \ 
-        `fill`: 点内部的填充颜色 \ 
-        `outline`: 点轮廓的颜色
+        * `canvas`: 父画布
+        * `point_start`: 起点坐标
+        * `point_end`: 终点坐标
+        * `width`: 线的宽度
+        * `fill`: 线的颜色
         """
-        _Point.__init__(self, list(coords))
+        _Object3D.__init__(self, list(point_start), list(point_end))
         canvas._items_3d.append(self)
         self.canvas = canvas
-        self.size = size
         self.width = width
         self.fill = fill
-        self.item = canvas.create_oval(
-            -1, -1, -1, -1, fill=fill, outline=outline, width=width)
+        self.item = canvas.create_line(-1, -1, -1, -1, width=width, fill=fill)
         self.update()
 
     def update(self):  # type: () -> None
-        """ 更新对象的显示 """
-        x, y = self._project(self.canvas.distance)
-        self.canvas.coords(self.item, (x-self.size)*self.canvas.rx, (y-self.size) *
-                           self.canvas.ry, (x+self.size)*self.canvas.rx, (y+self.size)*self.canvas.ry)
+        """更新对象的显示"""
+        self.canvas.coords(self.item, *[coord * self.canvas._ratio[i]
+                           for point in self._project(self.canvas._distance, self.canvas) for i, coord in enumerate(point)])
 
     def _camera_distance(self):  # type: () -> float
-        """ 与相机距离 """
-        sign = math.copysign(1, self.canvas.distance - self.coordinates[0][0])
-        return sign*math.dist([self.canvas.distance, 0, 0], self.coordinates[0])
+        """与相机距离"""
+        center = self.center()
+        sign = math.copysign(1, self.canvas._distance - center[0])
+        return sign * math.dist([self.canvas._distance, 0, 0], center)
 
 
-class Line(_Line):
-    """ 线 """
+class Side(_Object3D):
+    """面"""
 
     def __init__(
         self,
-        canvas,  # type: Canvas_3D | Space
-        point_start,  # type: Iterable[float]
-        point_end,  # type: Iterable[float]
-        *,
-        width=LINE_WDITH,  # type: float
-        fill=COLOR_LINE_FILL,  # type: str
+        canvas,  # type: Canvas3D | Space
+        *points,  # type: tuple[float, float, float]
+        width=1,  # type: float
+        fill="",  # type: str
+        outline="#000000",  # type: str
     ):  # type: (...) -> None
         """
-        `canvas`: 父画布 \ 
-        `point_start`: 起点坐标 \ 
-        `point_end`: 终点坐标 \ 
-        `width`: 线的宽度 \ 
-        `fill`: 线的颜色
+        * `canvas`: 父画布
+        * `points`: 各点的空间坐标
+        * `width`: 面轮廓的宽度
+        * `fill`: 面内部的填充颜色
+        * `outline`: 面轮廓的颜色
         """
-        _Line.__init__(self, list(point_start), list(point_end))
+        _Object3D.__init__(self, *[list(point) for point in points])
         canvas._items_3d.append(self)
         self.canvas = canvas
         self.width = width
         self.fill = fill
-        self.item = canvas.create_line(-1, -1, -1, -1, width=width, fill=fill)
+        self.outline = outline
+        self.item = canvas.create_polygon(-1, -1, -1, -1,
+                                          width=width, fill=fill, outline=outline)
         self.update()
 
     def update(self):  # type: () -> None
-        """ 更新对象的显示 """
-        self.canvas.coords(self.item, *[coord*(self.canvas.ry if i else self.canvas.rx)
-                           for point in self._project(self.canvas.distance) for i, coord in enumerate(point)])
+        """更新对象的显示"""
+        self.canvas.coords(
+            self.item, *[coord * self.canvas._ratio[i] for point in self._project(self.canvas._distance, self.canvas) for i, coord in enumerate(point)])
 
     def _camera_distance(self):  # type: () -> float
-        """ 与相机距离 """
+        """与相机距离"""
         center = self.center()
-        sign = math.copysign(1, self.canvas.distance - center[0])
-        return sign*math.dist([self.canvas.distance, 0, 0], center)
+        sign = math.copysign(1, self.canvas._distance - center[0])
+        return sign * math.dist([self.canvas._distance, 0, 0], center)
 
 
-class Side(_Side):
-    """ 面 """
+class Text3D(_Object3D):
+    """三维文本"""
 
     def __init__(
         self,
-        canvas,  # type: Canvas_3D | Space
-        *points,  # type: Iterable[float]
-        width=SIDE_WIDTH,  # type: float
-        fill=COLOR_SIDE_FILL,  # type: str
-        outline=COLOR_SIDE_OUTLINE,  # type: str
+        canvas,  # type: Canvas3D | Space
+        coords,  # type: tuple[float, float, float]
+        text="",  # type: str
+        *,
+        # type: tuple[str, int, str]
+        font=(constants.FONT, constants.SIZE),
+        justify="center",  # type: typing.Literal["center", "left", "right"]
+        fill="#000000",  # type: str
     ):  # type: (...) -> None
         """
-        `canvas`: 父画布 \ 
-        `points`: 各点的空间坐标 \ 
-        `width`: 面轮廓的宽度 \ 
-        `fill`: 面内部的填充颜色 \ 
-        `outline`: 面轮廓的颜色
+        * `canvas`: 父画布
+        * `coords`: 点的空间坐标
+        * `text`: 显示的文本
+        * `size`: 点的大小
+        * `font`: 点轮廓的宽度
+        * `justify`: 多行文本对齐方式
+        * `fill`: 点内部的填充颜色
         """
-        _Side.__init__(self, *[list(point) for point in points])
+        _Object3D.__init__(self, list(coords))
         canvas._items_3d.append(self)
         self.canvas = canvas
-        self.width = width
+        self.font = font
         self.fill = fill
-        self.outline = outline
-        self.item = canvas.create_polygon(
-            -1, -1, -1, -1, width=width, fill=fill, outline=outline)
+        self.text = text
+        self.item = canvas.create_text(-1, -1,
+                                       text=text, fill=fill, justify=justify)
         self.update()
 
     def update(self):  # type: () -> None
-        """ 更新对象的显示 """
-        self.canvas.coords(self.item, *[coord*(self.canvas.ry if i else self.canvas.rx)
-                           for line in self._project(self.canvas.distance) for point in line for i, coord in enumerate(point)])
+        """更新对象的显示"""
+        x, y = self._project(self.canvas._distance, self.canvas)[0]
+        self.canvas.coords(
+            self.item, x*self.canvas._ratio[0], y*self.canvas._ratio[1])
+        font = list(self.font)
+        font[1] = round(font[1] * self.canvas._distance *
+                        math.sqrt(self.canvas._ratio[0]*self.canvas._ratio[1]) / self._camera_distance())
+        self.canvas.itemconfigure(self.item, font=font)
 
     def _camera_distance(self):  # type: () -> float
-        """ 与相机距离 """
-        center = self.center()
-        sign = math.copysign(1, self.canvas.distance - center[0])
-        return sign*math.dist([self.canvas.distance, 0, 0], center)
+        """与相机距离"""
+        sign = math.copysign(1, self.canvas._distance - self.coordinates[0][0])
+        return sign * math.dist([self.canvas._distance, 0, 0], self.coordinates[0])
 
 
 class Geometry:
-    """ 几何体 """
+    """几何体"""
 
     def __init__(
         self,
-        canvas,  # type: Canvas_3D | Space
+        canvas,  # type: Canvas3D | Space
         *sides,  # type: Side
     ):  # type: (...) -> None
         """
-        `canvas`: 父画布 \ 
-        `sides`: 组成几何体的面
+        * `canvas`: 父画布
+        * `sides`: 组成几何体的面
         """
         canvas._geos.append(self)
         self.canvas = canvas
         self.sides = list(sides)
 
     def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
-        """
-        ### 平移
-        `dx`: x 方向位移长度 \ 
-        `dy`: y 方向位移长度 \ 
-        `dz`: z 方向位移长度
+        """平移几何体中的所有 3D 对象
+
+        * `dx`: x 方向位移长度
+        * `dy`: y 方向位移长度
+        * `dz`: z 方向位移长度
         """
         for side in self.sides:
             side.translate(dx, dy, dz)
 
-    @overload
-    def rotate(self, dx=0, dy=0, dz=0, *, center=ROTATE_CENTER):
-        # type: (float, float, float, ..., Iterable[float]) -> None
+    @typing.overload
+    def rotate(self, dx=0, dy=0, dz=0, *, center=(0, 0, 0)):
+        # type: (float, float, float, ..., tuple[float, float, float]) -> None
         ...
 
-    @overload
+    @typing.overload
     def rotate(self, dx=0, *, axis):
-        # type: (float, ..., Iterable[Iterable[float]]) -> None
+        # type: (float, ..., tuple[tuple[float, float, float], tuple[float, float, float]]) -> None
         ...
 
-    def rotate(self, dx=0, dy=0, dz=0, *, center=ROTATE_CENTER, axis=None):
-        # type: (float, float, float, ..., Iterable[float], Iterable[Iterable[float]] | None) -> None
-        """
-        ### 旋转
-        `dx`: x 方向旋转弧度，或者绕旋转轴线的旋转弧度 \ 
-        `dy`: y 方向旋转弧度 \ 
-        `dz`: z 方向旋转弧度 \ 
-        `center`: 旋转中心，默认为原点 \ 
-        `axis`: 旋转轴线，无默认值
+    def rotate(self, dx=0, dy=0, dz=0, *, center=(0, 0, 0), axis=None):
+        # type: (float, float, float, ..., tuple[float, float, float], tuple[tuple[float, float, float], tuple[float, float, float]] | None) -> None
+        """旋转几何体中的所有 3D 对象
+
+        * `dx`: x 方向逆时针旋转弧度，或者绕旋转轴线的旋转弧度
+        * `dy`: y 方向逆时针旋转弧度
+        * `dz`: z 方向逆时针旋转弧度
+        * `center`: 旋转中心，默认为原点
+        * `axis`: 旋转轴线，无默认值
         """
         for side in self.sides:
             side.rotate(dx, dy, dz, center=center, axis=axis)
 
     def scale(self, kx=1, ky=1, kz=1, *, center=None):
-        # type: (float, float, float, ..., Iterable[float] | None) -> None
-        """
-        ### 缩放
-        `kx`: x 方向缩放比例 \ 
-        `ky`: y 方向缩放比例 \ 
-        `kz`: z 方向缩放比例 \ 
-        `center`: 缩放中心，默认为几何中心
+        # type: (float, float, float, ..., tuple[float, float, float] | None) -> None
+        """缩放几何体中的所有 3D 对象
+
+        * `kx`: x 方向缩放比例
+        * `ky`: y 方向缩放比例
+        * `kz`: z 方向缩放比例
+        * `center`: 缩放中心，默认为几何中心
         """
         if center is None:
             center = self.center()
         for side in self.sides:
             side.scale(kx, ky, kz, center=center)
 
     def center(self):  # type: () -> tuple[float, float, float]
-        """ 几何中心 """
+        """几何中心"""
         return tuple(statistics.mean(axis) for axis in zip(*set(tuple(coord) for side in self.sides for coord in side.coordinates)))
 
     def update(self):  # type: () -> None
-        """ 更新几何体 """
+        """更新几何体"""
         for side in self.sides:
             side.update()
 
     def append(self, *sides):  # type: (Side) -> None
-        """
-        ### 添加面
-        `sides`: `Side` 类
+        """给几何体添加更多新的面
+
+        * `sides`: `Side` 类
         """
         for side in sides:
             self.sides.append(side)
 
 
 class Cuboid(Geometry):
-    """ 长方体 """
+    """长方体"""
 
     def __init__(
         self,
-        canvas,  # type: Canvas_3D | Space
+        canvas,  # type: Canvas3D | Space
         x,  # type: float
         y,  # type: float
         z,  # type: float
         length,  # type: float
         width,  # type: float
         height,  # type: float
         *,
-        color_up='',  # type: str
-        color_down='',  # type: str
-        color_left='',  # type: str
-        color_right='',  # type: str
-        color_front='',  # type: str
-        color_back='',  # type: str
+        boardwidth=1,  # type: int
+        color_fill_up="",  # type: str
+        color_fill_down="",  # type: str
+        color_fill_left="",  # type: str
+        color_fill_right="",  # type: str
+        color_fill_front="",  # type: str
+        color_fill_back="",  # type: str
+        color_outline_up="#000000",  # type: str
+        color_outline_down="#000000",  # type: str
+        color_outline_left="#000000",  # type: str
+        color_outline_right="#000000",  # type: str
+        color_outline_front="#000000",  # type: str
+        color_outline_back="#000000",  # type: str
     ):  # type: (...) -> None
         """
-        `canvas`: 父画布 \ 
-        `x`: 左上角 x 坐标 \ 
-        `y`: 左上角 y 坐标 \ 
-        `z`: 左上角 z 坐标 \ 
-        `length`: 长度 \ 
-        `width`: 宽度 \ 
-        `height`: 高度 \ 
-        `color_up`: 上表面颜色 \ 
-        `color_down`: 下表面颜色 \ 
-        `color_left`: 左侧面颜色 \ 
-        `color_right`: 右侧面颜色 \ 
-        `color_front`: 正面颜色 \ 
-        `color_back`: 后面颜色
+        * `canvas`: 父画布
+        * `x`: 左上角 x 坐标
+        * `y`: 左上角 y 坐标
+        * `z`: 左上角 z 坐标
+        * `length`: 长度
+        * `width`: 宽度
+        * `height`: 高度
+        * `boardwidth`: 边框线条宽度
+        * `color_fill_up`: 上表面内部颜色
+        * `color_fill_down`: 下表面内部颜色
+        * `color_fill_left`: 左侧面内部颜色
+        * `color_fill_right`: 右侧面内部颜色
+        * `color_fill_front`: 正面内部颜色
+        * `color_fill_back`: 后面内部颜色
+        * `color_outline_up`: 上表面边框颜色
+        * `color_outline_down`: 下表面边框颜色
+        * `color_outline_left`: 左侧面边框颜色
+        * `color_outline_right`: 右侧面边框颜色
+        * `color_outline_front`: 正面边框颜色
+        * `color_outline_back`: 后面边框颜色
         """
         canvas._geos.append(self)
         self.canvas = canvas
-        coords = [[x+l, y+w, z+h]
-                  for l in (0, length)
-                  for w in (0, width)
-                  for h in (0, height)]
+        coords = [[x + l, y + w, z + h]
+                  for l in (0, length) for w in (0, width) for h in (0, height)]
         self.sides = [
-            Side(canvas, coords[0], coords[1],
-                 coords[3], coords[2], fill=color_back),
-            Side(canvas, coords[0], coords[1],
-                 coords[5], coords[4], fill=color_left),
-            Side(canvas, coords[0], coords[2],
-                 coords[6], coords[4], fill=color_up),
-            Side(canvas, coords[1], coords[3],
-                 coords[7], coords[5], fill=color_down),
-            Side(canvas, coords[2], coords[3],
-                 coords[7], coords[6], fill=color_right),
-            Side(canvas, coords[4], coords[5],
-                 coords[7], coords[6], fill=color_front),
+            Side(canvas, coords[0], coords[1], coords[3], coords[2],
+                 width=boardwidth, fill=color_fill_back, outline=color_outline_back),
+            Side(canvas, coords[0], coords[1], coords[5], coords[4],
+                 width=boardwidth, fill=color_fill_left, outline=color_outline_left),
+            Side(canvas, coords[0], coords[2], coords[6], coords[4],
+                 width=boardwidth, fill=color_fill_down, outline=color_outline_down),
+            Side(canvas, coords[1], coords[3], coords[7], coords[5],
+                 width=boardwidth, fill=color_fill_up, outline=color_outline_up),
+            Side(canvas, coords[2], coords[3], coords[7], coords[6],
+                 width=boardwidth, fill=color_fill_right, outline=color_outline_right),
+            Side(canvas, coords[4], coords[5], coords[7], coords[6],
+                 width=boardwidth, fill=color_fill_front, outline=color_outline_front),
         ]
 
 
 class Tetrahedron(Geometry):
-    """ 四面体 """
+    """四面体"""
 
     def __init__(
         self,
-        canvas,  # type: Canvas_3D | Space
-        point_1,  # type: Iterable[float]
-        point_2,  # type: Iterable[float]
-        point_3,  # type: Iterable[float]
-        point_4,  # type: Iterable[float]
+        canvas,  # type: Canvas3D | Space
+        point_1,  # type: tuple[float, float, float]
+        point_2,  # type: tuple[float, float, float]
+        point_3,  # type: tuple[float, float, float]
+        point_4,  # type: tuple[float, float, float]
         *,
-        colors=('',)*4  # type: Iterable[str]
+        boardwidth=1,  # type: int
+        color_fill=("", "", "", ""),  # type: tuple[str, str, str, str]
+        color_outline=("#000000", "#000000", "#000000", "#000000")
+        # type: tuple[str, str, str, str]
     ):  # type: (...) -> None
         """
-        `canvas`: 父画布 \ 
-        `point_1`: 第一个顶点 \ 
-        `point_2`: 第二个顶点 \ 
-        `point_3`: 第三个顶点 \ 
-        `point_4`: 第四个顶点 \ 
-        `colors`: 颜色序列
+        * `canvas`: 父画布
+        * `point_1`: 第一个顶点
+        * `point_2`: 第二个顶点
+        * `point_3`: 第三个顶点
+        * `point_4`: 第四个顶点
+        * `boardwidth`: 边框线条宽度
+        * `color_fill`: 内部颜色序列
+        * `color_outline`: 边框颜色序列
         """
         canvas._geos.append(self)
         self.canvas = canvas
         self.sides = [
-            Side(canvas, point_1, point_2, point_3, fill=colors[0]),
-            Side(canvas, point_1, point_2, point_4, fill=colors[1]),
-            Side(canvas, point_1, point_3, point_4, fill=colors[2]),
-            Side(canvas, point_2, point_3, point_4, fill=colors[3]),
+            Side(canvas, point_1, point_2, point_3, width=boardwidth,
+                 fill=color_fill[0], outline=color_outline[0]),
+            Side(canvas, point_1, point_2, point_4, width=boardwidth,
+                 fill=color_fill[1], outline=color_outline[0]),
+            Side(canvas, point_1, point_3, point_4, width=boardwidth,
+                 fill=color_fill[2], outline=color_outline[0]),
+            Side(canvas, point_2, point_3, point_4, width=boardwidth,
+                 fill=color_fill[3], outline=color_outline[0]),
         ]
-
-
-__all__ = list(filter(lambda name: '__' not in name, globals()))
```

