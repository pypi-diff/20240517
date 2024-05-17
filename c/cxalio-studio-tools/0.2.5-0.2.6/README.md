# Comparing `tmp/cxalio_studio_tools-0.2.5.tar.gz` & `tmp/cxalio_studio_tools-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cxalio_studio_tools-0.2.5.tar", max compression
+gzip compressed data, was "cxalio_studio_tools-0.2.6.tar", max compression
```

## Comparing `cxalio_studio_tools-0.2.5.tar` & `cxalio_studio_tools-0.2.6.tar`

### file list

```diff
@@ -1,44 +1,52 @@
--rw-r--r--   0        0        0    35821 2024-04-16 07:18:25.822233 cxalio_studio_tools-0.2.5/LICENSE
--rw-r--r--   0        0        0     1064 2024-05-16 01:05:40.939683 cxalio_studio_tools-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1619 2024-05-16 04:20:46.686740 cxalio_studio_tools-0.2.5/README.md
--rw-r--r--   0        0        0      188 2024-05-15 04:56:11.320786 cxalio_studio_tools-0.2.5/src/cx_core/__init__.py
--rw-r--r--   0        0        0      145 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.5/src/cx_core/abstract_app.py
--rw-r--r--   0        0        0      838 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.5/src/cx_core/abstract_env.py
--rw-r--r--   0        0        0     1286 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.5/src/cx_core/app_logger.py
--rw-r--r--   0        0        0     2024 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.5/src/cx_core/datapackage.py
--rw-r--r--   0        0        0     1826 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.5/src/cx_core/ffmpeg_progress_parser.py
--rw-r--r--   0        0        0     1462 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.5/src/cx_core/folder_expander.py
--rw-r--r--   0        0        0      465 2024-05-15 04:56:11.320786 cxalio_studio_tools-0.2.5/src/cx_core/osinfo.py
--rw-r--r--   0        0        0     1421 2024-05-15 04:56:11.321788 cxalio_studio_tools-0.2.5/src/cx_core/tag_replacer.py
--rw-r--r--   0        0        0     2991 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.5/src/cx_core/timecode.py
--rw-r--r--   0        0        0     1640 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.5/src/cx_core/timepoint.py
--rw-r--r--   0        0        0      466 2024-05-15 04:56:11.321788 cxalio_studio_tools-0.2.5/src/cx_core/tui_elements.py
--rw-r--r--   0        0        0     2835 2024-05-16 01:10:01.334550 cxalio_studio_tools-0.2.5/src/cx_core/utils.py
--rw-r--r--   0        0        0      101 2024-05-15 04:56:11.321788 cxalio_studio_tools-0.2.5/src/cx_subtitle/__init__.py
--rw-r--r--   0        0        0     4752 2024-05-16 01:11:55.820388 cxalio_studio_tools-0.2.5/src/cx_subtitle/loader.py
--rw-r--r--   0        0        0     5394 2024-05-15 04:56:11.322788 cxalio_studio_tools-0.2.5/src/cx_subtitle/saver.py
--rw-r--r--   0        0        0      731 2024-05-15 04:56:11.322788 cxalio_studio_tools-0.2.5/src/cx_subtitle/subtitle.py
--rw-r--r--   0        0        0     2858 2024-05-15 04:56:11.322788 cxalio_studio_tools-0.2.5/src/cx_subtitle/subtitle_formatter.py
--rw-r--r--   0        0        0       35 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.5/src/media_killer/__init__.py
--rw-r--r--   0        0        0     1312 2024-05-15 04:56:11.322788 cxalio_studio_tools-0.2.5/src/media_killer/env.py
--rw-r--r--   0        0        0     2958 2024-05-15 04:56:11.323789 cxalio_studio_tools-0.2.5/src/media_killer/example_project.toml
--rw-r--r--   0        0        0      364 2024-05-15 04:56:11.323789 cxalio_studio_tools-0.2.5/src/media_killer/exceptions.py
--rw-r--r--   0        0        0     5453 2024-05-15 04:56:11.323789 cxalio_studio_tools-0.2.5/src/media_killer/help.md
--rw-r--r--   0        0        0     7970 2024-05-16 01:03:50.246599 cxalio_studio_tools-0.2.5/src/media_killer/media_killer_app.py
--rw-r--r--   0        0        0     6865 2024-05-16 01:03:50.254603 cxalio_studio_tools-0.2.5/src/media_killer/mission.py
--rw-r--r--   0        0        0     1269 2024-05-15 04:56:11.324789 cxalio_studio_tools-0.2.5/src/media_killer/option_package.py
--rw-r--r--   0        0        0     3827 2024-05-15 04:56:11.324789 cxalio_studio_tools-0.2.5/src/media_killer/planner.py
--rw-r--r--   0        0        0     3484 2024-05-16 01:03:50.263052 cxalio_studio_tools-0.2.5/src/media_killer/profile_loader.py
--rw-r--r--   0        0        0     1762 2024-05-15 04:56:11.325789 cxalio_studio_tools-0.2.5/src/media_killer/script_writer.py
--rw-r--r--   0        0        0     2793 2024-05-15 04:56:11.325789 cxalio_studio_tools-0.2.5/src/media_killer/source_adapter.py
--rw-r--r--   0        0        0     4092 2024-05-16 01:03:50.278075 cxalio_studio_tools-0.2.5/src/media_killer/transcoder.py
--rw-r--r--   0        0        0       30 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.5/src/sub_conv/__init__.py
--rw-r--r--   0        0        0     1132 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.5/src/sub_conv/env.py
--rw-r--r--   0        0        0       44 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.5/src/sub_conv/exceptions.py
--rw-r--r--   0        0        0     3539 2024-05-16 04:22:39.006788 cxalio_studio_tools-0.2.5/src/sub_conv/help.md
--rw-r--r--   0        0        0    10199 2024-05-16 01:15:56.196910 cxalio_studio_tools-0.2.5/src/sub_conv/subconv_app.py
--rw-r--r--   0        0        0     1624 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.5/src/sub_conv/subtitle_translator.py
--rw-r--r--   0        0        0        0 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.5/src/systools/__init__.py
--rw-r--r--   0        0        0      278 2024-05-15 04:56:11.328045 cxalio_studio_tools-0.2.5/src/systools/env.py
--rw-r--r--   0        0        0     3722 2024-05-15 04:56:11.328045 cxalio_studio_tools-0.2.5/src/systools/update_githubhosts.py
--rw-r--r--   0        0        0     2507 1970-01-01 00:00:00.000000 cxalio_studio_tools-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    35821 2024-04-16 07:18:25.822233 cxalio_studio_tools-0.2.6/LICENSE
+-rw-r--r--   0        0        0     1084 2024-05-17 07:44:23.221828 cxalio_studio_tools-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1996 2024-05-17 07:51:54.561308 cxalio_studio_tools-0.2.6/README.md
+-rw-r--r--   0        0        0       21 2024-05-17 05:39:34.544036 cxalio_studio_tools-0.2.6/src/cx_core/__init__.py
+-rw-r--r--   0        0        0      108 2024-05-17 05:53:09.833669 cxalio_studio_tools-0.2.6/src/cx_core/app/__init__.py
+-rw-r--r--   0        0        0      139 2024-05-17 05:39:34.578319 cxalio_studio_tools-0.2.6/src/cx_core/app/abstract_app.py
+-rw-r--r--   0        0        0      839 2024-05-17 05:39:34.512687 cxalio_studio_tools-0.2.6/src/cx_core/app/abstract_env.py
+-rw-r--r--   0        0        0     1286 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.6/src/cx_core/app/app_logger.py
+-rw-r--r--   0        0        0      489 2024-05-17 05:39:34.572394 cxalio_studio_tools-0.2.6/src/cx_core/app/osinfo.py
+-rw-r--r--   0        0        0       57 2024-05-17 05:39:34.584785 cxalio_studio_tools-0.2.6/src/cx_core/filesystem/__init__.py
+-rw-r--r--   0        0        0     7184 2024-05-17 05:34:42.314821 cxalio_studio_tools-0.2.6/src/cx_core/filesystem/path_expander.py
+-rw-r--r--   0        0        0     1011 2024-05-17 05:34:42.337608 cxalio_studio_tools-0.2.6/src/cx_core/filesystem/path_utils.py
+-rw-r--r--   0        0        0      106 2024-05-17 05:39:34.566406 cxalio_studio_tools-0.2.6/src/cx_core/misc/__init__.py
+-rw-r--r--   0        0        0     2024 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.6/src/cx_core/misc/datapackage.py
+-rw-r--r--   0        0        0      185 2024-05-17 05:39:34.595553 cxalio_studio_tools-0.2.6/src/cx_core/misc/misc_utils.py
+-rw-r--r--   0        0        0     2991 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.6/src/cx_core/misc/timecode.py
+-rw-r--r--   0        0        0     1640 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.6/src/cx_core/misc/timepoint.py
+-rw-r--r--   0        0        0      111 2024-05-17 05:39:34.560433 cxalio_studio_tools-0.2.6/src/cx_core/text/__init__.py
+-rw-r--r--   0        0        0      490 2024-05-17 05:34:42.309485 cxalio_studio_tools-0.2.6/src/cx_core/text/code_detecting.py
+-rw-r--r--   0        0        0     1421 2024-05-15 04:56:11.321788 cxalio_studio_tools-0.2.6/src/cx_core/text/tag_replacer.py
+-rw-r--r--   0        0        0     1641 2024-05-17 05:34:42.341609 cxalio_studio_tools-0.2.6/src/cx_core/text/text_utils.py
+-rw-r--r--   0        0        0       29 2024-05-17 05:39:34.534426 cxalio_studio_tools-0.2.6/src/cx_core/tui/__init__.py
+-rw-r--r--   0        0        0      465 2024-05-17 05:39:34.507134 cxalio_studio_tools-0.2.6/src/cx_core/tui/tui_elements.py
+-rw-r--r--   0        0        0      102 2024-05-17 05:50:00.631930 cxalio_studio_tools-0.2.6/src/cx_subtitle/__init__.py
+-rw-r--r--   0        0        0     4872 2024-05-17 05:34:42.333077 cxalio_studio_tools-0.2.6/src/cx_subtitle/loader.py
+-rw-r--r--   0        0        0     5739 2024-05-17 05:58:33.996192 cxalio_studio_tools-0.2.6/src/cx_subtitle/saver.py
+-rw-r--r--   0        0        0      736 2024-05-17 05:34:42.324075 cxalio_studio_tools-0.2.6/src/cx_subtitle/subtitle.py
+-rw-r--r--   0        0        0     2854 2024-05-17 05:50:00.614878 cxalio_studio_tools-0.2.6/src/cx_subtitle/subtitle_formatter.py
+-rw-r--r--   0        0        0       35 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.6/src/media_killer/__init__.py
+-rw-r--r--   0        0        0     1554 2024-05-17 07:31:58.553596 cxalio_studio_tools-0.2.6/src/media_killer/env.py
+-rw-r--r--   0        0        0     2958 2024-05-15 04:56:11.323789 cxalio_studio_tools-0.2.6/src/media_killer/example_project.toml
+-rw-r--r--   0        0        0      783 2024-05-17 05:24:05.584096 cxalio_studio_tools-0.2.6/src/media_killer/exceptions.py
+-rw-r--r--   0        0        0     5453 2024-05-15 04:56:11.323789 cxalio_studio_tools-0.2.6/src/media_killer/help.md
+-rw-r--r--   0        0        0     7390 2024-05-17 05:53:09.817424 cxalio_studio_tools-0.2.6/src/media_killer/media_killer_app.py
+-rw-r--r--   0        0        0     6958 2024-05-17 05:39:34.548120 cxalio_studio_tools-0.2.6/src/media_killer/mission.py
+-rw-r--r--   0        0        0     1324 2024-05-17 07:28:17.427659 cxalio_studio_tools-0.2.6/src/media_killer/option_package.py
+-rw-r--r--   0        0        0     3489 2024-05-17 07:33:38.885945 cxalio_studio_tools-0.2.6/src/media_killer/profile_loader.py
+-rw-r--r--   0        0        0     1772 2024-05-17 05:34:42.300925 cxalio_studio_tools-0.2.6/src/media_killer/script_writer.py
+-rw-r--r--   0        0        0     3075 2024-05-17 05:50:00.619892 cxalio_studio_tools-0.2.6/src/media_killer/source_adapter.py
+-rw-r--r--   0        0        0     4368 2024-05-17 05:34:42.329076 cxalio_studio_tools-0.2.6/src/media_killer/task_inspector.py
+-rw-r--r--   0        0        0     4246 2024-05-17 07:27:24.724480 cxalio_studio_tools-0.2.6/src/media_killer/transcoder.py
+-rw-r--r--   0        0        0       30 2024-04-16 07:18:25.837859 cxalio_studio_tools-0.2.6/src/sub_conv/__init__.py
+-rw-r--r--   0        0        0     1286 2024-05-17 05:53:09.821355 cxalio_studio_tools-0.2.6/src/sub_conv/env.py
+-rw-r--r--   0        0        0      360 2024-05-17 05:50:00.658714 cxalio_studio_tools-0.2.6/src/sub_conv/exceptions.py
+-rw-r--r--   0        0        0     3548 2024-05-17 05:58:34.029805 cxalio_studio_tools-0.2.6/src/sub_conv/help.md
+-rw-r--r--   0        0        0     5503 2024-05-17 05:53:09.789294 cxalio_studio_tools-0.2.6/src/sub_conv/subconv_app.py
+-rw-r--r--   0        0        0     1857 2024-05-17 07:49:03.803106 cxalio_studio_tools-0.2.6/src/sub_conv/subtitle_translator.py
+-rw-r--r--   0        0        0     6762 2024-05-17 05:50:00.650915 cxalio_studio_tools-0.2.6/src/sub_conv/worker.py
+-rw-r--r--   0        0        0        0 2024-05-15 04:56:11.326789 cxalio_studio_tools-0.2.6/src/systools/__init__.py
+-rw-r--r--   0        0        0      282 2024-05-17 05:53:09.839811 cxalio_studio_tools-0.2.6/src/systools/env.py
+-rw-r--r--   0        0        0     3750 2024-05-17 05:58:34.010735 cxalio_studio_tools-0.2.6/src/systools/update_githubhosts.py
+-rw-r--r--   0        0        0     2912 1970-01-01 00:00:00.000000 cxalio_studio_tools-0.2.6/PKG-INFO
```

### Comparing `cxalio_studio_tools-0.2.5/LICENSE` & `cxalio_studio_tools-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.5/pyproject.toml` & `cxalio_studio_tools-0.2.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cxalio-studio-tools"
-version = "0.2.5"
+version = "0.2.6"
 description = "Scripts for po studio made by cxalio"
 authors = ["xiii_1991 <xiii_1991@163.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [
     { include = "cx_core", from = "src" },
     { include = "media_killer", from = "src" },
@@ -22,14 +22,15 @@
 rich = "^13.7.0"
 chardet = "^5.2.0"
 rich-argparse = '^1.4.0'
 python-ffmpeg = "^2.0.10"
 python-docx = "^1.1.0"
 openpyxl = "^3.1.2"
 translators = "^5.9.2"
+xpinyin = "^0.7.6"
 
 [tool.poetry.scripts]
 mediakiller = 'media_killer:run'
 subconv = 'sub_conv:run'
 update_githubhosts = 'systools.update_githubhosts:run'
 
 [build-system]
```

### Comparing `cxalio_studio_tools-0.2.5/README.md` & `cxalio_studio_tools-0.2.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -34,24 +34,36 @@
 
 ## To-do
 
 - media-inspector 解析媒体信息
 
 ## Change-log
 
+### 0.2.6
+
+- 统一设计可迭代的 PathExpander 代替 FolderExpander
+- 重新构造更健壮的 subconv
+- 更新 mediakiller 的逻辑与结构
+- 修改了cx_core库的结构，优化了全部代码
+- 优化了 mediakiller 和 subconv 的状态显示布局
+- 修复了 mediakiller 无数值选项传递失败的 bug
+- 为 subconv 增加了备选翻译方案
+
 ### 0.2.5
+
 mediakiller:
 
 - 修复了 duration 无法解析时崩溃的 bug。
 - 修复了目标目录解析为当前目录的错误。
 - 增加了扩展名检查，强制生成的配置文件扩展名为`toml`。
 - 修改了当前任务进度条的样式，减少闪烁。
 - 修复了不可覆盖输出文件时，转码卡住的问题。
 
 subconv:
+
 - 增加了强制设置读取文件编码的选项。
 
 ### 0.2.0
 
 重新构建现有工具。
 
 #### MediaKiller
```

### Comparing `cxalio_studio_tools-0.2.5/src/cx_core/abstract_env.py` & `cxalio_studio_tools-0.2.6/src/cx_core/app/abstract_env.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,9 +24,9 @@
         self._logger.print(*objs, level=LogLevel.CRITICAL)
 
     @property
     def log_level(self):
         return self._logger.level
 
     @log_level.setter
-    def log_level(self,level):
+    def log_level(self, level):
         self._logger.level = level
```

### Comparing `cxalio_studio_tools-0.2.5/src/cx_core/app_logger.py` & `cxalio_studio_tools-0.2.6/src/cx_core/app/app_logger.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.5/src/cx_core/datapackage.py` & `cxalio_studio_tools-0.2.6/src/cx_core/misc/datapackage.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.5/src/cx_core/tag_replacer.py` & `cxalio_studio_tools-0.2.6/src/cx_core/text/tag_replacer.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.5/src/cx_core/timecode.py` & `cxalio_studio_tools-0.2.6/src/cx_core/misc/timecode.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.5/src/cx_core/timepoint.py` & `cxalio_studio_tools-0.2.6/src/cx_core/misc/timepoint.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.5/src/cx_subtitle/loader.py` & `cxalio_studio_tools-0.2.6/src/cx_subtitle/loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import re
 from abc import abstractmethod
+from functools import cached_property
 from os import PathLike
 from pathlib import Path
 
 from docx import Document
-from functools import cached_property
 
-from cx_core.timepoint import TimePoint
-from cx_core.utils import detect_encoding
+from cx_core.misc.timepoint import TimePoint
+from cx_core.text.code_detecting import detect_encoding
 from .subtitle import Subtitle
 
 
 class AbstractSubtitleLoader:
-    def __init__(self, source: str | PathLike,encoding=None):
+    def __init__(self, source: str | PathLike, encoding=None):
         self.source = Path(source)
         self.file = None
         self._encoding = encoding
 
     @cached_property
     def encoding(self):
         if self._encoding and self._encoding != 'auto':
@@ -37,16 +37,16 @@
 
 
 class TxtLoader(AbstractSubtitleLoader):
     MILLISECOND_PER_CHAR = 120
     MIN_DURATION_PER_LINE = 2000
     TS_PATTERN = r'\s*\d{2}:\d{2}:\d{2}.\d{3}\s*'
 
-    def __init__(self, filename):
-        super(TxtLoader, self).__init__(filename)
+    def __init__(self, filename, encoding=None):
+        super(TxtLoader, self).__init__(filename, encoding)
         self.__last_point = TimePoint(0)
 
     def subtitles(self):
         for a in self.file:
             content = re.sub(self.TS_PATTERN, '', a)
             duration = len(content) * TxtLoader.MILLISECOND_PER_CHAR
             if duration < TxtLoader.MIN_DURATION_PER_LINE:
@@ -57,16 +57,16 @@
             self.__last_point = end
 
 
 class SrtLoader(AbstractSubtitleLoader):
     HEAD_LINE = re.compile(r'^\d+$')
     TIME_LINE = re.compile(r'^(\d\d:\d\d:\d\d[,.]\d\d\d) --> (\d\d:\d\d:\d\d[,.]\d\d\d)$')
 
-    def __int__(self, filename):
-        super(SrtLoader, self).__init__(filename)
+    def __int__(self, filename, encoding=None):
+        super(SrtLoader, self).__init__(filename, encoding)
 
     def subtitles(self):
         content, start, end = '', None, None
         state = None
         for a in self.file:
             line = a.strip()
             if not state:
@@ -90,16 +90,16 @@
 
 
 class WordLoader(AbstractSubtitleLoader):
     MILLISECOND_PER_CHAR = 120
     MIN_DURATION_PER_LINE = 2000
     TS_PATTERN = r'\s*\d{2}:\d{2}:\d{2}.\d{3}\s*'
 
-    def __init__(self, filename):
-        super(WordLoader, self).__init__(filename)
+    def __init__(self, filename, encoding=None):
+        super(WordLoader, self).__init__(filename, encoding)
         self.__last_point = TimePoint(0)
         self.document = None
 
     def __enter__(self):
         self.document = Document(str(self.source.absolute()))
         return self
 
@@ -121,16 +121,16 @@
 class TTMLLoader(AbstractSubtitleLoader):
     PATTERN = r'<p begin=\"(\d\d:\d\d:\d\d.\d\d\d)\" end=\"(\d\d:\d\d:\d\d.\d\d\d)\">(.*?)</p>\s'
     REPLACEMENTS = {
         '<br/>': '\n',
         '&quot;': '"'
     }
 
-    def __init__(self, filename):
-        super(TTMLLoader, self).__init__(filename)
+    def __init__(self, filename, encoding=None):
+        super(TTMLLoader, self).__init__(filename, encoding)
 
     def subtitles(self):
         total = self.file.read()
         pat = re.compile(self.PATTERN, re.DOTALL)
         for match in pat.finditer(total):
             start = TimePoint.from_timestamp(match.group(1))
             end = TimePoint.from_timestamp(match.group(2))
```

### Comparing `cxalio_studio_tools-0.2.5/src/cx_subtitle/saver.py` & `cxalio_studio_tools-0.2.6/src/cx_subtitle/saver.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 import csv
 from abc import abstractmethod
 from copy import deepcopy
+from functools import cached_property
 from pathlib import Path
 
 from docx import Document
 from openpyxl import Workbook
 
 from .subtitle import Subtitle, SubtitleProcessor
 
 
 class AbstractSubtitleSaver:
-    def __init__(self, filename, keep_time=False):
+    def __init__(self, filename, keep_time=False, encoding=None):
         self.target = Path(filename)
         self.keep_time = keep_time
         self.file = None
-        self.encoding = 'utf-8'
+        self._encoding = encoding
         self.processors: [SubtitleProcessor] = []
-        self.parent_folder=None
+        self._target_parent = None
+
+    @cached_property
+    def encoding(self):
+        if self._encoding == 'auto':
+            return None
+        return self._encoding
 
     def __enter__(self):
-        self.parent_folder = self.target.absolute().parent
-        self.parent_folder.mkdir(parents=True, exist_ok=True)
+        self._target_parent = self.target.absolute().parent
+        self._target_parent.mkdir(parents=True, exist_ok=True)
         self.file = open(self.target, 'w', encoding=self.encoding)
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.file.flush()
         self.file.close()
         return False
@@ -47,28 +54,28 @@
 
 class TxtSaver(AbstractSubtitleSaver):
     LINE_TEMPLATE = {
         True: '{start}\t{content}\n',
         False: '{content}\n'
     }
 
-    def __init__(self, target, keep_time=False):
-        super(TxtSaver, self).__init__(target, keep_time)
+    def __init__(self, target, keep_time=False, encoding=None):
+        super(TxtSaver, self).__init__(target, keep_time, encoding)
 
     def write(self, subtitle: Subtitle):
         sub = self.process_subtitle(subtitle)
         line = TxtSaver.LINE_TEMPLATE[self.keep_time].format(start=sub.start.timestamp, content=sub.content)
         self.file.write(line)
 
 
 class SrtSaver(AbstractSubtitleSaver):
     LINE_TEMPLATE = '{number}\n{start} --> {end}\n{content}\n\n'
 
-    def __init__(self, target, keep_time=True):
-        super(SrtSaver, self).__init__(target, keep_time)
+    def __init__(self, target, keep_time=True, encoding=None):
+        super(SrtSaver, self).__init__(target, keep_time, encoding)
         self.__count = 1
 
     def write(self, subtitle: Subtitle):
         sub = self.process_subtitle(subtitle)
         line = SrtSaver.LINE_TEMPLATE.format(
             number=self.__count,
             start=sub.start.timestamp,
@@ -81,24 +88,24 @@
 
 class WordSaver(AbstractSubtitleSaver):
     LINE_TEMPLATE = {
         True: '{start}\t{content}',
         False: '{content}'
     }
 
-    def __init__(self, target, keep_time=False):
-        super(WordSaver, self).__init__(target, keep_time)
+    def __init__(self, target, keep_time=False, encoding=None):
+        super(WordSaver, self).__init__(target, keep_time, encoding)
         self.document = Document()
 
     def __enter__(self):
         self.document.add_heading(Path(self.target.stem).name, level=1)
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        self.document.save(self.target)
+        self.document.save(str(self.target.absolute()))
         return False
 
     def write(self, subtitle: Subtitle):
         sub = self.process_subtitle(subtitle)
         line = self.LINE_TEMPLATE[self.keep_time].format(
             start=sub.start.timestamp,
             content=sub.content
@@ -109,16 +116,16 @@
 class ExcelSaver(AbstractSubtitleSaver):
     """如果 keep_time 为 True，则会追加秒数队列"""
     HEADERS = {
         True: ['开始', '结束', '开始（秒）', '结束（秒）', '台词'],
         False: ['开始', '结束', '台词']
     }
 
-    def __init__(self, target, keep_time=True):
-        super(ExcelSaver, self).__init__(target, keep_time)
+    def __init__(self, target, keep_time=True, encoding=None):
+        super(ExcelSaver, self).__init__(target, keep_time, encoding)
         self.workbook = Workbook()
         self.table = self.workbook.active
 
     def __enter__(self):
         self.table.title = '字幕表格'
         self.table.append(self.HEADERS[self.keep_time])
         return self
@@ -140,16 +147,16 @@
 class CsvSaver(AbstractSubtitleSaver):
     """如果 keep_time 为 True，则会追加秒数队列"""
     HEADERS = {
         True: ['开始', '结束', '开始（秒）', '结束（秒）', '台词'],
         False: ['开始', '结束', '台词']
     }
 
-    def __init__(self, target, keep_time=False):
-        super(CsvSaver, self).__init__(target, keep_time)
+    def __init__(self, target, keep_time=False, encoding=None):
+        super(CsvSaver, self).__init__(target, keep_time, encoding)
         self.__saver = None
 
     def __enter__(self):
         self.file = open(self.target, 'w', newline='', encoding=self.encoding)
         self.__saver = csv.DictWriter(self.file, self.HEADERS[self.keep_time], extrasaction='ignore')
         self.__saver.writeheader()
         return self
```

### Comparing `cxalio_studio_tools-0.2.5/src/cx_subtitle/subtitle.py` & `cxalio_studio_tools-0.2.6/src/cx_subtitle/subtitle.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 from functools import cached_property
 
-from cx_core.timepoint import TimePoint
+from cx_core.misc.timepoint import TimePoint
 
 
 @dataclass(order=True)
 class Subtitle:
     start: TimePoint
     end: TimePoint
     content: str
```

### Comparing `cxalio_studio_tools-0.2.5/src/cx_subtitle/subtitle_formatter.py` & `cxalio_studio_tools-0.2.6/src/cx_subtitle/subtitle_formatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 
-from .subtitle import Subtitle,SubtitleProcessor
+from .subtitle import Subtitle, SubtitleProcessor
 
 
 class SubtitleFormatter(SubtitleProcessor):
     def __init__(self, **kwargs):
-        super(SubtitleFormatter,self).__init__()
+        super(SubtitleFormatter, self).__init__()
         self.replacements = {'\t': ' '}
         self.remove_tags = True
 
         self.normal_strip = True
         self.strip_quotes = True
         self.extra_strips = ''
 
@@ -83,10 +83,7 @@
 
     def is_subtitle_legal(self, subtitle: Subtitle):
         if self.remove_empty_subtitles and not subtitle.content:
             return False
         if self.remove_zero_duration_subtitles and subtitle.duration == 0:
             return False
         return True
-
-
-
```

### Comparing `cxalio_studio_tools-0.2.5/src/media_killer/env.py` & `cxalio_studio_tools-0.2.6/src/media_killer/env.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import signal
 
-from rich.progress import Progress, SpinnerColumn
+from rich.progress import Progress, SpinnerColumn, TextColumn, BarColumn, TaskProgressColumn, TimeRemainingColumn
+from rich.table import Column
 
-from cx_core import AppLogger, AbstractEnv, LogLevel
+from cx_core.app import AppLogger, AbstractEnv, LogLevel
 
 
 class Env(AbstractEnv):
     def __init__(self):
         super(Env, self).__init__()
         self._progress = Progress(
             SpinnerColumn(),
-            # MofNCompleteColumn(),
-            *Progress.get_default_columns(),
+            TextColumn("[progress.description]{task.description}", table_column=Column(ratio=50)),
+            BarColumn(table_column=Column(ratio=20)),
+            TaskProgressColumn(),
+            TimeRemainingColumn(),
             expand=True,
             transient=True)
 
         self._logger = AppLogger(console=self._progress.console)
         self._logger.level = LogLevel.WARNING
 
         self.args = None
```

### Comparing `cxalio_studio_tools-0.2.5/src/media_killer/example_project.toml` & `cxalio_studio_tools-0.2.6/src/media_killer/example_project.toml`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.5/src/media_killer/help.md` & `cxalio_studio_tools-0.2.6/src/media_killer/help.md`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.5/src/media_killer/media_killer_app.py` & `cxalio_studio_tools-0.2.6/src/media_killer/media_killer_app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import pkgutil
 from argparse import ArgumentParser, ArgumentError
-from pathlib import Path
 
-from rich.columns import Columns
 from rich.markdown import Markdown
 from rich.panel import Panel
 from rich_argparse import RichHelpFormatter
 
-from cx_core import AbstractApp
 from cx_core import DataPackage
-from cx_core.app_logger import LogLevel
-from cx_core.tui_elements import JobCounter
-from cx_core.utils import normalize_path
+from cx_core.app import AbstractApp
+from cx_core.app import LogLevel
+from cx_core.filesystem import normalize_path, force_suffix
+from cx_core.tui import JobCounter
 from .env import env
+from .exceptions import *
 from .mission import MissionMaker
-from .planner import Planner
-from .profile_loader import ProfileLoader, ProfileNoFoundError
+from .profile_loader import ProfileLoader
 from .script_writer import ScriptWriter
+from .task_inspector import TaskInspector
 from .transcoder import Transcoder
 
 
 class MediaKillerApp(AbstractApp):
-    APP_VERSION = '0.2.4'
+    APP_VERSION = '0.2.6'
     APP_NAME = 'mediakiller'
 
     def __init__(self):
         super(MediaKillerApp, self).__init__()
         self.global_task = None
 
         parser = ArgumentParser(prog=MediaKillerApp.APP_NAME, formatter_class=RichHelpFormatter,
@@ -59,16 +58,15 @@
         data = pkgutil.get_data('media_killer', 'help.md').decode('utf_8')
         panel = Panel(Markdown(data), width=80)
         env.console.print(panel)
 
     @staticmethod
     def copy_example_profile(tgt):
         tgt = normalize_path(tgt)
-        if tgt.suffix != '.toml':
-            tgt = tgt.with_suffix('.toml')
+        tgt = force_suffix(tgt, '.toml')
         data = pkgutil.get_data('media_killer', 'example_project.toml')
         try:
             with open(tgt, 'xb') as file:
                 file.write(data)
             env.print(f'模板配置文件已保存到 {env.args.profile} ，[red]请在修改后运行！[/red]')
         except FileExistsError:
             env.error('文件 {0} 已存在，[red]请手动删除它，或指定其它的目标文件[/red]'.format(tgt))
@@ -99,82 +97,75 @@
             pass
         elif issubclass(exc_type, ProfileNoFoundError):
             env.critical(exc_val)
             result = True
         elif issubclass(exc_type, ArgumentError):
             env.error('参数输入有误:', exc_val)
             result = True
+        elif issubclass(exc_type, MediaKillerError):
+            env.error(f'[red]{exc_val}[/red]')
+            result = True
 
         env.stop()
         return result
 
     def run(self):
         if env.args.full_help:
             env.info('检测到 full_help 设置，打印帮助文件并退出')
             MediaKillerApp.show_full_help()
             return
 
         if not env.args.profile:
             env.info('未检测到项目文件选项')
-            raise ProfileNoFoundError
+            raise ProfileNoFoundError()
 
         if env.args.generate_example:
             env.info('检测到 "--generate-example" 参数，将拷贝配置文件模板')
             env.progress.update(task_id=self.global_task, description='正在输出配置文件', visible=True)
             self.copy_example_profile(env.args.profile)
             return
 
         with ProfileLoader(env.args.profile) as profile_loader:
             datas = profile_loader.load()
             self.profile = datas
         env.info('配置信息已初始化')
 
         if not self.profile.source.files:
-            env.error('[red]未指定任何来源信息，无事可做[/red]')
-            return
+            raise NoSourceError()
 
-        planner = Planner(self.profile)
-        env.progress.update(task_id=self.global_task, description='正在将来源信息加入计划', visible=True)
-        planner.load_sources(self.profile.source.files)
-        env.info('已发现 {0} 项来源'.format(len(planner)))
-
-        env.progress.update(task_id=self.global_task, description='正在整理来源信息', visible=True)
-        planner.arrange()
-        env.print(f'整理结束，已添加 {len(planner)} 项计划')
-        if env.args.debug:
-            col = Columns(
-                (Panel(Path(str(x)).name, style='yellow', border_style='green', safe_box=True,
-                       title=f'#{i}', title_align='left')
-                 for i, x in enumerate(planner)),
-                expand=True, equal=False, column_first=True
-            )
-            env.debug(col)
+        plans = []
+        with TaskInspector(self.profile) as inspector:
+            plans = inspector.make_plans(self.profile.source.files)
+
+        if not plans:
+            raise NoPlansError()
+        env.print(f'探测到 {len(plans)} 个源文件')
 
         env.debug('构建 mission maker')
-        missions = MissionMaker(self.profile)
+        mission_maker = MissionMaker(self.profile)
 
         if env.args.script_output is not None:
             env.progress.update(task_id=self.global_task, description='输出脚本文件', visible=True)
             env.info('检测到 "--make-script" 参数，将进行脚本输出')
             output_file = normalize_path(env.args.script_output)
             with ScriptWriter(output_file) as writer:
-                for mission in env.progress.track(missions(planner.plans), description=env.args.script_output):
+                for mission in env.progress.track(mission_maker(plans), description=env.args.script_output):
                     writer.write_mission(mission)
             env.print(f'已输出脚本文件 "{env.args.script_output}"')
             return
 
-        env.progress.update(self.global_task, description='总体进度', visible=True, total=len(planner))
+        env.progress.update(self.global_task, description='总体进度', visible=True, total=len(plans))
         env.progress.start_task(self.global_task)
 
-        job_counter = JobCounter(len(planner))
-        for mission in missions(planner):
+        job_counter = JobCounter(len(plans))
+        for mission in mission_maker(plans):
             job_counter.advance()
             if env.wanna_quit:
                 env.print('正在取消未完成的任务...')
-                break
+                raise UserCanceledError()
             if env.args.pretend_mode:
                 env.print(f'模拟运行: [yellow]{mission.source.name}[/yellow] 完毕')
             else:
                 with Transcoder(mission) as coder:
                     coder.run()
             env.progress.advance(self.global_task)
             env.print(f'[yellow]{job_counter}[/yellow] [cyan]{mission.source.name}[/cyan] 转换完成')
```

### Comparing `cxalio_studio_tools-0.2.5/src/media_killer/mission.py` & `cxalio_studio_tools-0.2.6/src/media_killer/mission.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from functools import cache
 from pathlib import Path
 
 from cx_core import DataPackage
-from cx_core.tag_replacer import TagReplacer
-from cx_core.utils import limit_number, split_at_unquoted_spaces, normalize_path
+from cx_core.filesystem.path_utils import normalize_path
+from cx_core.misc.misc_utils import limit_number
+from cx_core.text.tag_replacer import TagReplacer
+from cx_core.text.text_utils import split_at_unquoted_spaces
 from .env import env
 from .option_package import OptionPackage
 
 
 class OptionParser:
     def __init__(self, options):
         self._options = options
```

### Comparing `cxalio_studio_tools-0.2.5/src/media_killer/option_package.py` & `cxalio_studio_tools-0.2.6/src/media_killer/option_package.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections import defaultdict
 from pathlib import Path
 
-from cx_core.utils import unquote_text
+from cx_core.text.text_utils import unquote_text
 
 
 class OptionPackage:
 
     @staticmethod
     def __format_key(k: str):
         key = str(k).strip()
@@ -29,17 +29,19 @@
             self.raw_data[k].append(v)
         elif k not in self.raw_data:
             self.raw_data[k] = []
         return self
 
     def iter_options(self):
         for k, vs in self.raw_data.items():
-            for v in vs:
-                value = v or ''
-                yield k, value
+            if not vs:
+                yield k, None
+            else:
+                for v in vs:
+                    yield k, v
 
     def iter_arguments(self):
         for k, v in self.iter_options():
             yield '-' + k
             yield v
 
     def __rich_repr__(self):
```

### Comparing `cxalio_studio_tools-0.2.5/src/media_killer/planner.py` & `cxalio_studio_tools-0.2.6/src/media_killer/task_inspector.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,94 +1,107 @@
 import itertools
-from itertools import groupby
-from pathlib import Path
 
-from cx_core.folder_expander import FolderExpander
+from cx_core import DataPackage
+from cx_core.filesystem.path_expander import *
+from cx_core.filesystem.path_utils import normalize_path, normalize_suffix
 from .env import env
 from .source_adapter import adapters
 
 
-class Planner:
+class TaskInspector:
+    """处理输入的队列，并解析可接受的文件"""
+
     DEFAULT_SUFFIXES = ("mov mkv mp4 flv 3gp 3gpp rmvb mp3 aac"
                         " mxf mxf_op1a vob wmv wma srt ass aas ttml ogg oga ogv m4a"
                         " m4v 3g2 mpeg mpg ts lrc h264 flac ast asf gif")
 
-    def __init__(self, profile):
-        self._loaded_file = set()
-        self.plans = []
-        self.profile = profile
-        env.debug('初始化任务调度器')
-
-    def __len__(self):
-        return len(self.plans)
-
-    def __iter__(self):
-        return self.plans.__iter__()
-
-    def load_source(self, filename):
-        source = Path(filename)
-        if not source.is_absolute():
-            source = self.profile.general.working_folder / source
-        suffix = source.suffix.lower().strip('.')
-        env.debug(f'文件 "{source}" 的扩展名为 "{suffix}"')
+    def __init__(self, profile: DataPackage):
+        self._profile = profile
+        self.task = None
+        self._expander_settings = None
+
+    def __enter__(self):
+        env.info('计算扩展名白名单...')
+        _suffixes = {str(x).strip('.') for x in
+                     itertools.chain(
+                         TaskInspector.DEFAULT_SUFFIXES.split(),
+                         self.profile.source.suffix_includes)
+                     if x not in {str(x).strip('.')
+                                  for x in self.profile.source.suffix_excludes}
+                     }
+        env.debug(f'计划接受的扩展名: [green]{' '.join(_suffixes)}[/green]')
+
+        self._expander_settings = PathExpander.Settings(
+            accept_dir=False,
+            file_validator=SuffixValidator(_suffixes),
+            anchor_dir=self.profile.general.working_folder
+        )
+        env.info('已构建 PathExpander.Settings')
+
+        self.task = env.progress.add_task(description='任务探测器', total=None)
+        env.info('任务探测器启动')
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        env.progress.remove_task(self.task)
+        return False
+
+    @property
+    def profile(self):
+        return self._profile
+
+    def _expand_source(self, source: Path) -> []:
+        """
+        检查来源文件是否是列表文件并展开
+        """
+        source = normalize_path(source, self.profile.general.working_folder)
+        suffix = normalize_suffix(source.suffix, False)
+        result = []
         if suffix in adapters:
-            env.debug(f'已识别 "{source}" 为列表文件')
-            try:
-                with adapters[suffix](source) as adp:
-                    for item in adp.items():
-                        env.debug(f'发现文件路径 "{item}"')
-                        self.plans.append(item)
-            except FileNotFoundError:
-                env.error(f'文件 {source} 不存在，无法读取')
-            finally:
-                self._loaded_file.add(source)
+            env.print(f'[cyan]{source.name}[/cyan] 为列表文件，将会展开')
+            env.progress.update(self.task, description=f'正在展开 [cyan]{source.name}[/cyan] 中包含的媒体信息')
+            with adapters[suffix](source) as adapter:
+                for item in adapter.items():
+                    k = Path(item)
+                    env.debug(f'发现新的文件路径: [cyan]{k}[/cyan]')
+                    result.append(k)
         else:
-            self.plans.append(source)
-            self._loaded_file.add(source)
-            env.debug(f'文件 "{source}" 无法识别为列表文件，将直接添加进入计划')
-
-    def load_sources(self, filenames):
-        task = env.progress.add_task(description='读取来源文件...')
-        for f in env.progress.track(filenames, task_id=task):
-            self.load_source(f)
-        env.progress.remove_task(task)
-
-    def make_suffix_whitelist(self):
-        env.debug('开始构建扩展名白名单')
-        _basic_suffixes = {str(x).strip('.') for x in
-                           itertools.chain(Planner.DEFAULT_SUFFIXES.split(), self.profile.source.suffix_includes)}
-        _blacklist = {str(x).strip('.') for x in self.profile.source.suffix_excludes}
-        w_list = _basic_suffixes - _blacklist
-        env.debug(f'生成扩展名白名单 [cyan]{" ".join(w_list)}[/cyan]')
-        return w_list
-
-    def arrange(self):
-        env.info('开始整理计划列表')
-
-        env.debug('构建 Expander ...')
-        expander = FolderExpander()
-        expander.working_directory = self.profile.general.working_folder
-
-        w_list = self.make_suffix_whitelist()
-        expander.suffixes_whitelist = ['.' + x for x in w_list]
-
-        env.info('开始展开文件夹')
-        new_files = [Path(x) for x in expander.expand(*self.plans)]
-        env.info('正在根据路径进行排序')
-        new_files = sorted(new_files, key=lambda a: a.absolute())
-
-        env.info('开始逐个检查文件')
-        arranged_files = []
-        task = env.progress.add_task(description='检查文件列表...')
-        for k, v in env.progress.track(groupby(new_files), task_id=task):
-            kk = Path(k)
+            result.append(source)
+        return result
+
+    def _arrange(self, sources: []) -> []:
+        env.progress.update(self.task, description='检查计划列表…')
+        env.info('开始根据路径进行排序…')
+        sources = sorted(sources, key=lambda a: Path(a).absolute())
+
+        env.info('开始逐个检查…')
+        result = []
+        for k, v in env.progress.track(itertools.groupby(sources), task_id=self.task):
+            kk = Path(k).absolute()
+            env.progress.update(self.task,
+                                description=f'检查项目: [cyan]{kk.name}[/cyan] …')
             if not kk.exists():
-                env.warning(f'文件 "{kk}" 不存在，将从任务列表中去除')
+                env.warning(f'[red]文件 [cyan]{kk.name}[/cyan] 不存在，将从任务列表中去除[/red]')
                 continue
-            arranged_files.append(kk)
-            env.debug(f'重新添加 "{kk}"')
+            result.append(kk)
+            env.debug(f'添加任务 [cyan]{kk}[/cyan]')
+
             count = len(list(v))
             if count > 1:
-                env.warning(f'发现 {count} 个重复的 "{k}" ，已经去除')
-        env.progress.remove_task(task)
-        self.plans = arranged_files
-        env.info('计划列表自动整理完毕')
+                env.warning(
+                    f'[yellow][cyan]{kk.name}[/cyan]有 [red]{count - 1}[/red] 个重复项，已从任务列表中去除[/yellow]')
+
+        env.info('计划列表整理完毕')
+        return result
+
+    def make_plans(self, sources) -> [Path]:
+        env.print(f'检测到 {len(sources)} 个输入，正在展开路径…')
+        env.progress.update(self.task, description='构建路径展开器…')
+        expander = PathExpander(sources, self._expander_settings)
+
+        result = []
+
+        for source in expander:
+            env.progress.update(self.task, description=f'检测 [cyan]{source.name}[/cyan]')
+            result += self._expand_source(source)
+
+        return self._arrange(result)
```

### Comparing `cxalio_studio_tools-0.2.5/src/media_killer/profile_loader.py` & `cxalio_studio_tools-0.2.6/src/media_killer/profile_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 import tomllib
 from collections.abc import Iterable
 from pathlib import Path
 
 from cx_core import DataPackage
-from cx_core.utils import normalize_path
+from cx_core.filesystem.path_utils import normalize_path, force_suffix
 from .env import env
-from .exceptions import ProfileNoFoundError
 
 
 class ProfileLoader:
     def __init__(self, filename):
         self.task_id = None
-        self.filename = Path(filename)
+        self.filename = force_suffix(filename, 'toml')
 
     def __enter__(self):
         env.info('进入配置解析器环境')
-        self.task_id = env.progress.add_task(description='初始化配置解析器', start=False)
+        self.task_id = env.progress.add_task(description='初始化配置解析器', total=None)
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
+        result = False
+        if exc_type is None:
+            pass
+        elif issubclass(exc_type, FileNotFoundError):
+            env.critical(f'未找到配置文件: {self.filename.name}')
+            result = True
+
         env.progress.remove_task(self.task_id)
         self.task_id = None
         env.info('配置解析器已关闭')
 
+        return result
+
     @staticmethod
     def __make_sure_list(a=None):
         if not a:
             return []
         if isinstance(a, str):
             return a.split(' ')
         if isinstance(a, Iterable):
@@ -34,31 +42,32 @@
         return [x for x in str(a).split(' ')]
 
     def __check_data_package(self, package):
         env.progress.update(self.task_id, description='解析配置文件数据', completed=1, total=2)
         env.info('开始检查配置数据...')
 
         result = DataPackage(**package)
-        env.print(f'开始解析配置文件：[cyan]{result.general.name}[/cyan]:[yellow]{result.general.description}[/yellow]')
+        env.print(f'配置文件：[cyan]{result.general.name}[/cyan] : [yellow]{result.general.description}[/yellow]')
 
         if not result.general.ffmpeg:
             result.general.ffmpeg = 'ffmpeg'
             env.print('未指定 ffmpeg ，将调用系统环境中的 ffmpeg')
 
         profile_folder = normalize_path('.' if not result.profile_path else result.profile_path.parent)
         result.profile_folder = profile_folder
         if not result.general.working_folder:
             env.debug('配置文件未指定工作目录')
             result.general.working_folder = profile_folder
         else:
             result.general.working_folder = normalize_path(result.general.working_folder, profile_folder)
         env.debug(f'general.working_folder 已设置为 {result.general.working_folder}')
 
-        result.source.files.extend(ProfileLoader.__make_sure_list(env.args.sources))
-        env.print(f'增加 {len(env.args.sources)} 个手动指定的来源文件')
+        if env.args.sources:
+            result.source.files.extend(ProfileLoader.__make_sure_list(env.args.sources))
+            env.print(f'增加 {len(env.args.sources)} 个手动指定的来源文件')
 
         if not result.target.folder:
             env.debug('未设置目标文件夹')
             result.target.folder = Path('.')
         result.target.folder = normalize_path(result.target.folder, result.general.working_folder)
         env.debug(f'target.folder 已设置为 {result.target.folder}')
 
@@ -68,19 +77,13 @@
 
         env.debug(f'参数解析结果：{result}')
 
         return result
 
     def load(self):
         result = {}
-        env.progress.start_task(self.task_id)
-        env.progress.update(self.task_id, completed=0, total=2)
-        task = env.progress.add_task(description=f'读取{self.filename}...')
-        try:
-            with env.progress.open(self.filename, 'rb', task_id=task) as fp:
-                result.update(tomllib.load(fp))
-            result['profile_path'] = Path(self.filename).absolute()
-            return self.__check_data_package(result)
-        except FileNotFoundError:
-            raise ProfileNoFoundError(self.filename)
-        finally:
-            env.progress.remove_task(task)
+        env.progress.update(self.task_id, description=f'读取{self.filename}…')
+
+        with env.progress.open(self.filename, 'rb', task_id=self.task_id) as fp:
+            result.update(tomllib.load(fp))
+        result['profile_path'] = Path(self.filename).absolute()
+        return self.__check_data_package(result)
```

### Comparing `cxalio_studio_tools-0.2.5/src/media_killer/script_writer.py` & `cxalio_studio_tools-0.2.6/src/media_killer/script_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 
-from cx_core.utils import quote_text
+from cx_core.text.text_utils import quote_text
 from .env import env
 from .mission import Mission
 
 
 class ScriptWriter:
     def __init__(self, target):
         self.target = Path(target).absolute()
```

### Comparing `cxalio_studio_tools-0.2.5/src/media_killer/source_adapter.py` & `cxalio_studio_tools-0.2.6/src/media_killer/source_adapter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import csv
 import urllib.parse
-import xml.etree.ElementTree as ET
+import xml.etree.ElementTree as eTree
 from abc import abstractmethod
 from pathlib import Path
 
-from cx_core.utils import detect_encoding
+from cx_core.text.code_detecting import detect_encoding
 from .env import env
 
 
 class AbstractAdapter:
     def __init__(self):
         self.filename = None
         self.file = None
@@ -22,19 +22,25 @@
         self.task = env.progress.add_task(description=f'读取 {self.filename} ...')
         env.progress.wrap_file(self.file, task_id=self.task)
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.file.close()
         env.progress.remove_task(self.task)
-        return False
+        result = False
+        if exc_type is None:
+            env.debug('展开结束')
+        elif issubclass(exc_type, FileNotFoundError):
+            env.error(f'文件 [cyan]{self.filename}[/cyan] 无法读取！')
+            result = True
+        return result
 
     @abstractmethod
     def items(self):
-        pass
+        yield ''
 
 
 class CSVAdapter(AbstractAdapter):
     suffix = 'csv'
 
     def __init__(self, filename):
         super(AbstractAdapter, self).__init__()
@@ -66,15 +72,15 @@
     suffix = 'xml'
 
     def __init__(self, filename):
         super(AbstractAdapter, self).__init__()
         self.filename = filename
 
     def items(self):
-        et = ET.parse(self.file)
+        et = eTree.parse(self.file)
         for e in et.iter('pathurl'):
             url = urllib.parse.unquote_plus(e.text)
             if not url.startswith('file:'):
                 continue
             path = url.removeprefix('file:')
             yield Path(path)
 
@@ -83,15 +89,15 @@
     suffix = 'fcpxml'
 
     def __init__(self, filename):
         super(AbstractAdapter, self).__init__()
         self.filename = filename
 
     def items(self):
-        et = ET.parse(self.file)
+        et = eTree.parse(self.file)
         for e in et.iter('media-rep'):
             url = urllib.parse.unquote_plus(e.attrib['src'])
             if not url.startswith('file:'):
                 continue
             path = url.removeprefix('file:')
             yield Path(path)
```

### Comparing `cxalio_studio_tools-0.2.5/src/media_killer/transcoder.py` & `cxalio_studio_tools-0.2.6/src/media_killer/transcoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,41 +46,43 @@
                 folder.mkdir(parents=True, exist_ok=True)
 
         ffmpeg = FFmpeg(self.mission.profile.general.ffmpeg)
         env.debug(f'创建 ffmpeg 对象: {self.mission.profile.general.ffmpeg}')
 
         env.progress.update(self.task, description=f'写入全局参数')
         for k, v in self.mission.general_options.iter_options():
-            ffmpeg.option(k, v)
             env.debug(f'写入全局选项： [green]{k}[/green] : [yellow]{v}[/yellow]')
+            ffmpeg.option(k, v)
 
         for input_ in self.mission.inputs:
             env.progress.update(self.task, description=f'为 {input_.filename.name} 写入输入参数')
             ffmpeg.input(input_.filename.absolute(), input_.raw_data)
             env.debug(f'添加输入选项： {input_.raw_data}')
 
         for output_ in self.mission.outputs:
             env.progress.update(self.task, description=f'为 {output_.filename.name} 写入输出参数')
             ffmpeg.output(output_.filename.absolute(), output_.raw_data)
             env.debug(f'添加输出选项： {output_.raw_data}')
 
         env.debug(f'全部任务选项输入完毕， ffmpeg 对象构建完成')
+        env.progress.update(self.task, description=f'全部参数已写入')
 
         @ffmpeg.on('progress')
         def on_progress(progress: Progress):
             desc = '{0} [yellow]x{1:.2f}[/yellow]'.format(self.mission.source.name, progress.speed)
             curr = progress.time.seconds
             env.progress.update(self.task, description=desc, completed=curr)
 
         @ffmpeg.on('stderr')
         def on_stderr(line):
             env.debug(f'[grey]FFMPEG输出：[/grey] {line}')
 
         @ffmpeg.on('start')
         def on_start(arguments):
+            env.progress.update(self.task, description='ffmpeg 已启动')
             env.debug(f'开始执行任务: {' '.join(arguments)}')
 
         @ffmpeg.on('completed')
         def on_completed():
             env.debug(f'[green]{self.mission.source.name}[/green] [yellow]执行完毕，顺利退出[/yellow]')
 
         @ffmpeg.on('terminated')
```

### Comparing `cxalio_studio_tools-0.2.5/src/sub_conv/env.py` & `cxalio_studio_tools-0.2.6/src/sub_conv/env.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import signal
 
-from rich.progress import Progress, SpinnerColumn
+from rich.progress import Progress, SpinnerColumn, TextColumn, TimeElapsedColumn
+from rich.table import Column
 
-from cx_core import AbstractEnv, AppLogger, LogLevel
+from cx_core.app import AbstractEnv, AppLogger, LogLevel
 
 
 class Env(AbstractEnv):
     def __init__(self):
         super(Env, self).__init__()
         self.wanna_quit = False
 
         self._progress = Progress(
             SpinnerColumn(),
-            *Progress.get_default_columns(),
+            TextColumn('[progress.description]{task.description}', table_column=Column(ratio=50)),
+            TimeElapsedColumn(),
             expand=True,
             transient=True)
 
         self._logger = AppLogger(console=self._progress.console)
         self._logger.level = LogLevel.WARNING
 
     def start(self):
```

### Comparing `cxalio_studio_tools-0.2.5/src/sub_conv/help.md` & `cxalio_studio_tools-0.2.6/src/sub_conv/help.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # SubConv
 
 version: 0.2.5
 
 SubConv 用于批量转换字幕文件为台词本文档，
 附加地，也可以转换成其它格式的字幕文件，但**不保证完整性**。
 
->subconv 不能当做一个完备的字幕文件转换器
+> subconv 不能当做一个完备的字幕文件转换器
 
 subconv 有以下特点：
+
 - 可以批量地对文件进行处理，可以自动展开文件夹
 - 目标文件自动放置在源文件旁边，最大化减少参数指定
 - 也可以手动指定集中的输出文件夹
 - 支持`srt`、`ttml` 等多种字幕格式
 - 输出台词本可以选择是否尽量保留时间信息
 - 内置一个简单的字幕内容检查器，将会自动进行简单的格式化处理
 - 内置台词英文翻译功能(需要网络)
@@ -67,35 +68,38 @@
 # -f 是 --format 的缩写
 # -c 是 --encoding 的缩写
 ```
 
 具体支持的输出格式，可以用`--help`参数打印帮助信息查看
 
 ### 关于源文件的编码
+
 subconv 将会自动识别源文件的编码，但是有时这会有一些问题。
 
 通过使用`--force-decoding`选项强制指定读取源文件时的编码可以解决一些问题。
 
 ### 关于自动格式化器
 
 subconv 内置了一个简单的格式化器，默认启用。它将会对字幕内容进行这些检查：
+
 - 自动去除字幕文件中携带的格式化标签（Davinci Resolve 输出的字幕通常都有）
 - 自动删除开头结尾的空格或回车
 - 自动缩减连续的多个空格或引号
 - 自动将连续的多个回车合并为一个
 
 如果不希望进行这些处理，可以使用 `--bypass-formatter` 参数禁用它。
 
 ### 自动翻译
 
 启用了 `--translate` 参数后，输出的字幕文本将自动转换为英文。
 
 英文翻译使用 bing 翻译服务完成，需要确保网络通畅。
 
 ## 测试运行
+
 指定 `--dry-run` 参数可以启用干转模式，
 subconv 将会处理所有的内容，但是不会真的输出文件。
 
 也可以使用 `--debug` 参数，将会输出所有工作过程的信息，方便查看。
 
 两个选项可以一起使用。
```

### Comparing `cxalio_studio_tools-0.2.5/src/sub_conv/subtitle_translator.py` & `cxalio_studio_tools-0.2.6/src/sub_conv/subtitle_translator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 import time
 
-from translators.server import TranslatorError
+import translators
+from xpinyin import Pinyin as pinYin
 
 from cx_subtitle import Subtitle, SubtitleProcessor
-import translators
 from .env import env
 
 
 class SubtitleTranslator(SubtitleProcessor):
     MAX_SEQUENCE = 120
     SLEEP_SECOND = 15
 
     def __init__(self, target_lang='en'):
         super(SubtitleTranslator, self).__init__()
         env.debug('初始化翻译器')
         self.target_lang = target_lang
         self.ts = translators
-        # _ = self.ts.preaccelerate_and_speedtest()
         self._count = 0
+        self._pin_yin = None
+
+    def _fallback_translate(self, s: str):
+        if not self._pin_yin:
+            self._pin_yin = pinYin()
+        return self._pin_yin.get_pinyin(s, ' ')
 
-    def __call__(self, s):
+    def __call__(self, s: Subtitle):
         translated_content = s.content
         for i in range(10):
             if env.wanna_quit:
                 break
             try:
                 translated_content = str(self.ts.translate_text(s.content, to_language=self.target_lang))
                 env.debug(f'翻译文本 "{s.content}" 为 "{translated_content}" ')
@@ -31,15 +36,16 @@
             except KeyboardInterrupt:
                 env.error(f'用户终止服务')
                 break
             except Exception as e:
                 env.error(f'ERROR {i}: [red]{e}[/red]')
                 time.sleep(2)
         if translated_content == s.content:
-            env.debug(f'翻译失败，将保持原样: [yellow]{translated_content}[/yellow]')
+            env.debug(f'[yellow]{translated_content}[/yellow]，在线翻译失败，将启动备用方案')
+            translated_content = self._fallback_translate(translated_content)
 
         self._count += 1
         if self._count >= SubtitleTranslator.MAX_SEQUENCE:
             env.info('[cyan]达到连续最大请求数，正在等待……[/cyan]')
             time.sleep(SubtitleTranslator.SLEEP_SECOND)
             self._count = 0
```

### Comparing `cxalio_studio_tools-0.2.5/src/systools/update_githubhosts.py` & `cxalio_studio_tools-0.2.6/src/systools/update_githubhosts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-import urllib.request
 import os
+import urllib.request
 from argparse import ArgumentParser
 
-from cx_core import OSInfo, AbstractApp, DataPackage
 from rich_argparse import RichHelpFormatter
+
+from cx_core import DataPackage
+from cx_core.app import OSInfo, AbstractApp
 from .env import env
 
 
 class GithubHostsUpdaterApp(AbstractApp):
     URL = "https://gitlab.com/ineo6/hosts/-/raw/master/next-hosts"
 
     def __init__(self):
@@ -58,15 +60,15 @@
         self.status.update('开始解析...')
         github_hosts = []
         with open(local_filename, encoding='utf-8') as new_hosts:
             for line in new_hosts:
                 github_hosts.append(line)
 
         old_hosts = []
-        with open(self.osinfo.hosts_file,encoding='utf-8') as host_file:
+        with open(self.osinfo.hosts_file, encoding='utf-8') as host_file:
             inside_github_section = False
             for line in host_file:
                 if line == github_hosts[0]:
                     inside_github_section = True
                     continue
                 if line == github_hosts[-1]:
                     inside_github_section = False
@@ -83,15 +85,15 @@
 
         self.status.update('正在写入...')
         target = self.osinfo.hosts_file
         if self.args.side_save:
             target = self.args.side_save[0]
             env.print(f'修改输出目标为 {target}')
 
-        with open(target, "w",encoding='utf-8') as new_host:
+        with open(target, "w", encoding='utf-8') as new_host:
             new_host.writelines(old_hosts)
             new_host.writelines(github_hosts)
             env.print('写入完毕。')
 
         self.refresh_dns()
```

### Comparing `cxalio_studio_tools-0.2.5/PKG-INFO` & `cxalio_studio_tools-0.2.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cxalio-studio-tools
-Version: 0.2.5
+Version: 0.2.6
 Summary: Scripts for po studio made by cxalio
 Home-page: https://gitee.com/xiii_1991/cxalio-studio-tools
 License: GPL-3.0-or-later
 Keywords: ffmpeg,tool
 Author: xiii_1991
 Author-email: xiii_1991@163.com
 Requires-Python: >=3.11,<4.0
@@ -15,14 +15,15 @@
 Requires-Dist: chardet (>=5.2.0,<6.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: python-docx (>=1.1.0,<2.0.0)
 Requires-Dist: python-ffmpeg (>=2.0.10,<3.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: rich-argparse (>=1.4.0,<2.0.0)
 Requires-Dist: translators (>=5.9.2,<6.0.0)
+Requires-Dist: xpinyin (>=0.7.6,<0.8.0)
 Project-URL: Repository, https://gitee.com/xiii_1991/cxalio-studio-tools.git
 Description-Content-Type: text/markdown
 
 # cxalio-studio-tools
 
 ## 介绍
 
@@ -58,24 +59,36 @@
 
 ## To-do
 
 - media-inspector 解析媒体信息
 
 ## Change-log
 
+### 0.2.6
+
+- 统一设计可迭代的 PathExpander 代替 FolderExpander
+- 重新构造更健壮的 subconv
+- 更新 mediakiller 的逻辑与结构
+- 修改了cx_core库的结构，优化了全部代码
+- 优化了 mediakiller 和 subconv 的状态显示布局
+- 修复了 mediakiller 无数值选项传递失败的 bug
+- 为 subconv 增加了备选翻译方案
+
 ### 0.2.5
+
 mediakiller:
 
 - 修复了 duration 无法解析时崩溃的 bug。
 - 修复了目标目录解析为当前目录的错误。
 - 增加了扩展名检查，强制生成的配置文件扩展名为`toml`。
 - 修改了当前任务进度条的样式，减少闪烁。
 - 修复了不可覆盖输出文件时，转码卡住的问题。
 
 subconv:
+
 - 增加了强制设置读取文件编码的选项。
 
 ### 0.2.0
 
 重新构建现有工具。
 
 #### MediaKiller
```

