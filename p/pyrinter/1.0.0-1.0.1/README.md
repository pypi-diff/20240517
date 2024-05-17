# Comparing `tmp/pyrinter-1.0.0.tar.gz` & `tmp/pyrinter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrinter-1.0.0.tar", last modified: Wed Apr 24 17:45:46 2024, max compression
+gzip compressed data, was "pyrinter-1.0.1.tar", last modified: Fri May 17 11:07:54 2024, max compression
```

## Comparing `pyrinter-1.0.0.tar` & `pyrinter-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 17:45:46.843387 pyrinter-1.0.0/
--rw-rw-rw-   0        0        0     1086 2022-10-21 07:49:12.000000 pyrinter-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1632 2024-04-24 17:45:46.841386 pyrinter-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1127 2024-04-21 20:58:12.000000 pyrinter-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 17:45:46.818788 pyrinter-1.0.0/pyrinter/
--rw-rw-rw-   0        0        0      187 2024-04-24 17:43:37.000000 pyrinter-1.0.0/pyrinter/__init__.py
--rw-rw-rw-   0        0        0     7535 2024-04-24 17:43:38.000000 pyrinter-1.0.0/pyrinter/document.py
-drwxrwxrwx   0        0        0        0 2024-04-24 17:45:46.832386 pyrinter-1.0.0/pyrinter/printers/
--rw-rw-rw-   0        0        0      234 2024-04-24 17:43:38.000000 pyrinter-1.0.0/pyrinter/printers/__init__.py
--rw-rw-rw-   0        0        0     1023 2024-04-21 20:58:12.000000 pyrinter-1.0.0/pyrinter/printers/abs_printer.py
--rw-rw-rw-   0        0        0      385 2024-04-21 20:58:12.000000 pyrinter-1.0.0/pyrinter/printers/sphinx_printer.py
--rw-rw-rw-   0        0        0     3260 2024-04-24 17:43:38.000000 pyrinter-1.0.0/pyrinter/printers/win_printer.py
-drwxrwxrwx   0        0        0        0 2024-04-24 17:45:46.840386 pyrinter-1.0.0/pyrinter/utils/
--rw-rw-rw-   0        0        0      250 2024-04-24 17:43:38.000000 pyrinter-1.0.0/pyrinter/utils/__init__.py
--rw-rw-rw-   0        0        0      315 2024-04-24 17:43:38.000000 pyrinter-1.0.0/pyrinter/utils/sphinx_utils.py
--rw-rw-rw-   0        0        0      343 2022-10-21 07:49:12.000000 pyrinter-1.0.0/pyrinter/utils/win_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-24 17:45:46.841386 pyrinter-1.0.0/pyrinter.egg-info/
--rw-rw-rw-   0        0        0     1632 2024-04-24 17:45:46.000000 pyrinter-1.0.0/pyrinter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      445 2024-04-24 17:45:46.000000 pyrinter-1.0.0/pyrinter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 17:45:46.000000 pyrinter-1.0.0/pyrinter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-04-24 17:45:46.000000 pyrinter-1.0.0/pyrinter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-24 17:45:46.000000 pyrinter-1.0.0/pyrinter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 17:45:46.843387 pyrinter-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      731 2024-04-24 17:44:13.000000 pyrinter-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 11:07:54.932667 pyrinter-1.0.1/
+-rw-rw-rw-   0        0        0     1086 2024-05-17 07:39:23.000000 pyrinter-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1632 2024-05-17 11:07:54.930667 pyrinter-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1127 2024-05-17 07:39:23.000000 pyrinter-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 11:07:54.861666 pyrinter-1.0.1/pyrinter/
+-rw-rw-rw-   0        0        0      187 2024-05-17 07:39:23.000000 pyrinter-1.0.1/pyrinter/__init__.py
+-rw-rw-rw-   0        0        0     7625 2024-05-17 11:04:06.000000 pyrinter-1.0.1/pyrinter/document.py
+drwxrwxrwx   0        0        0        0 2024-05-17 11:07:54.905667 pyrinter-1.0.1/pyrinter/printers/
+-rw-rw-rw-   0        0        0      234 2024-05-17 07:39:23.000000 pyrinter-1.0.1/pyrinter/printers/__init__.py
+-rw-rw-rw-   0        0        0     1023 2024-05-17 07:39:23.000000 pyrinter-1.0.1/pyrinter/printers/abs_printer.py
+-rw-rw-rw-   0        0        0      385 2024-05-17 07:39:23.000000 pyrinter-1.0.1/pyrinter/printers/sphinx_printer.py
+-rw-rw-rw-   0        0        0     3338 2024-05-17 07:45:50.000000 pyrinter-1.0.1/pyrinter/printers/win_printer.py
+drwxrwxrwx   0        0        0        0 2024-05-17 11:07:54.927674 pyrinter-1.0.1/pyrinter/utils/
+-rw-rw-rw-   0        0        0      250 2024-05-17 07:39:23.000000 pyrinter-1.0.1/pyrinter/utils/__init__.py
+-rw-rw-rw-   0        0        0      315 2024-05-17 07:39:23.000000 pyrinter-1.0.1/pyrinter/utils/sphinx_utils.py
+-rw-rw-rw-   0        0        0      343 2024-05-17 07:39:23.000000 pyrinter-1.0.1/pyrinter/utils/win_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-17 11:07:54.929729 pyrinter-1.0.1/pyrinter.egg-info/
+-rw-rw-rw-   0        0        0     1632 2024-05-17 11:07:54.000000 pyrinter-1.0.1/pyrinter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      445 2024-05-17 11:07:54.000000 pyrinter-1.0.1/pyrinter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 11:07:54.000000 pyrinter-1.0.1/pyrinter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-17 11:07:54.000000 pyrinter-1.0.1/pyrinter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-17 11:07:54.000000 pyrinter-1.0.1/pyrinter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 11:07:54.932667 pyrinter-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      731 2024-05-17 07:45:50.000000 pyrinter-1.0.1/setup.py
```

### Comparing `pyrinter-1.0.0/LICENSE` & `pyrinter-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrinter-1.0.0/PKG-INFO` & `pyrinter-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrinter
-Version: 1.0.0
+Version: 1.0.1
 Summary: python printer package
 Author: Hod Vaknin
 License: MIT
 Project-URL: Source, https://github.com/hodvak/py-printer
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pyrinter-1.0.0/README.md` & `pyrinter-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyrinter-1.0.0/pyrinter/document.py` & `pyrinter-1.0.1/pyrinter/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+from dataclasses import dataclass
 from enum import Enum
 from tkinter import Tk
 from tkinter.font import Font as TkFont
-from collections import namedtuple
-from typing import Tuple, Generator, Optional, Union
+from typing import Literal, Tuple, Generator, Optional, Union
 from PIL import Image
 
-
-class Font(namedtuple("Font", ("font_name", "height"))):
+@dataclass
+class Font:
     """
-    class to represent font properties (font name and height)
+    class to represent font properties (font name, height and weight)
     """
 
+    font_name: str
+    height: int
+    weight: Literal["normal", "bold"] = "normal"
+
 
 class Align(Enum):
     """
     Alignment for text
     """
 
     RIGHT = 0
@@ -53,15 +57,15 @@
             page_size = page_size.value
         self.page_size = page_size
         self.name = name
 
     def add_text(
         self,
         text: str,
-        font: Font = Font(font_name="Arial", height=12),
+        font: Font = Font(font_name="Arial", height=12, weight="normal"),
         page: Optional[int] = None,
         rect: Optional[Tuple[float, float, float, float]] = None,
         align: Align = Align.LEFT,
         color: int = 0x000000,
     ):
         """
         add text to the document
@@ -221,15 +225,15 @@
         get the text size of a text (width) by the given font
 
         :param text: the text to print
         :param font: the font to use
         :return: the width of the text
         """
         root = Tk()  # Needed to estimate the width.
-        font_var = TkFont(family=font.font_name, size=font.height, weight="normal")
+        font_var = TkFont(family=font.font_name, size=font.height, weight=font.weight)
         width = font_var.measure(text) / 105
         root.destroy()  # Destroy the created window
         return width
 
     def __getitem__(self, index: int) -> Generator:
         """
         get the document data by pages (a generator)
```

### Comparing `pyrinter-1.0.0/pyrinter/printers/abs_printer.py` & `pyrinter-1.0.1/pyrinter/printers/abs_printer.py`

 * *Files identical despite different names*

### Comparing `pyrinter-1.0.0/pyrinter/printers/win_printer.py` & `pyrinter-1.0.1/pyrinter/printers/win_printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         doc.SelectObject(
             win32ui.CreateFont(
                 {
                     "name": data["font"].font_name,
                     "height": int(
                         Printer.__inch_to_printer_size(data["font"].height / 72)
                     ),
+                    "weight": 700 if data["font"].weight == "bold" else 400,
                 }
             )
         )
         doc.SetTextColor(Printer.__fix_color(data["color"]))
         align = win32con.DT_LEFT if data["align"] == Align.LEFT else win32con.DT_RIGHT
         doc.DrawText(data["text"], Printer.__get_printer_rect(data["rect"]), align)
```

### Comparing `pyrinter-1.0.0/pyrinter.egg-info/PKG-INFO` & `pyrinter-1.0.1/pyrinter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrinter
-Version: 1.0.0
+Version: 1.0.1
 Summary: python printer package
 Author: Hod Vaknin
 License: MIT
 Project-URL: Source, https://github.com/hodvak/py-printer
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pyrinter-1.0.0/setup.py` & `pyrinter-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pyrinter",
-    version="1.0.0",
+    version="1.0.1",
     packages=find_packages(include=["pyrinter", "pyrinter.*"]),
     author="Hod Vaknin",
     license="MIT",
     description="python printer package",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     project_urls={"Source": "https://github.com/hodvak/py-printer"},
```

