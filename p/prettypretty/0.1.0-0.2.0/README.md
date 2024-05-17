# Comparing `tmp/prettypretty-0.1.0.tar.gz` & `tmp/prettypretty-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettypretty-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "prettypretty-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `prettypretty-0.1.0.tar` & `prettypretty-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,40 @@
--rw-r--r--   0        0        0     2793 2024-05-02 16:16:46.878000 prettypretty-0.1.0/.gitignore
--rw-r--r--   0        0        0      351 2024-05-08 11:44:14.092903 prettypretty-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0    11358 2024-05-10 23:06:53.590972 prettypretty-0.1.0/LICENSE
--rw-r--r--   0        0        0      342 2024-05-16 13:10:04.823502 prettypretty-0.1.0/README.md
--rw-r--r--   0        0        0      634 2024-05-06 06:14:58.399937 prettypretty-0.1.0/docs/Makefile
--rw-r--r--   0        0        0     1522 2024-05-15 04:37:26.443031 prettypretty-0.1.0/docs/apidocs/color.rst
--rw-r--r--   0        0        0      168 2024-05-16 12:39:37.821220 prettypretty-0.1.0/docs/apidocs/prettypretty.rst
--rw-r--r--   0        0        0     1837 2024-05-16 12:45:08.223904 prettypretty-0.1.0/docs/conf.py
--rw-r--r--   0        0        0     5390 2024-05-15 17:10:11.260351 prettypretty-0.1.0/docs/conversions.rst
--rw-r--r--   0        0        0     4210 2024-05-13 23:07:43.595548 prettypretty-0.1.0/docs/formats-and-spaces.rst
--rw-r--r--   0        0        0     1411 2024-05-16 12:50:50.029771 prettypretty-0.1.0/docs/index.rst
--rw-r--r--   0        0        0      800 2024-05-06 06:14:58.400754 prettypretty-0.1.0/docs/make.bat
--rw-r--r--   0        0        0      208 2024-05-15 12:03:02.707612 prettypretty-0.1.0/docs/tools.rst
--rw-r--r--   0        0        0     1091 2024-05-02 16:16:18.007588 prettypretty-0.1.0/package-lock.json
--rw-r--r--   0        0        0       54 2024-05-02 16:16:09.342077 prettypretty-0.1.0/package.json
--rw-r--r--   0        0        0       22 2024-05-16 14:14:34.401618 prettypretty-0.1.0/prettypretty/__init__.py
--rw-r--r--   0        0        0       53 2024-05-15 19:10:56.836768 prettypretty-0.1.0/prettypretty/api/__init__.py
--rw-r--r--   0        0        0     7459 2024-05-16 12:50:10.098721 prettypretty-0.1.0/prettypretty/api/color.py
--rw-r--r--   0        0        0        0 2024-05-10 20:14:19.249777 prettypretty-0.1.0/prettypretty/color/__init__.py
--rw-r--r--   0        0        0     3643 2024-05-15 04:46:14.229875 prettypretty-0.1.0/prettypretty/color/apca.py
--rw-r--r--   0        0        0    12151 2024-05-16 04:08:42.955500 prettypretty-0.1.0/prettypretty/color/conversion.py
--rw-r--r--   0        0        0     1865 2024-05-15 03:43:07.902917 prettypretty-0.1.0/prettypretty/color/difference.py
--rw-r--r--   0        0        0     7658 2024-05-16 04:36:18.294816 prettypretty-0.1.0/prettypretty/color/grid.py
--rw-r--r--   0        0        0     8302 2024-05-16 12:57:08.461118 prettypretty-0.1.0/prettypretty/color/lores.py
--rw-r--r--   0        0        0     6109 2024-05-15 23:55:49.255258 prettypretty-0.1.0/prettypretty/color/serde.py
--rw-r--r--   0        0        0     7174 2024-05-15 03:48:44.497474 prettypretty-0.1.0/prettypretty/color/space.py
--rw-r--r--   0        0        0     2773 2024-05-16 04:27:39.507626 prettypretty-0.1.0/prettypretty/color/spec.py
--rw-r--r--   0        0        0      634 2024-05-05 17:58:20.659244 prettypretty-0.1.0/prettypretty/color/style.py
--rw-r--r--   0        0        0     4631 2024-05-16 04:45:02.880375 prettypretty-0.1.0/prettypretty/color/theme.py
--rw-r--r--   0        0        0      746 2024-05-16 13:06:20.940095 prettypretty-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0     1507 2024-05-10 00:55:29.680752 prettypretty-0.1.0/runtest.py
--rw-r--r--   0        0        0       49 2024-05-10 01:03:55.934703 prettypretty-0.1.0/test/__init__.py
--rw-r--r--   0        0        0     9112 2024-05-02 16:13:52.778390 prettypretty-0.1.0/test/runtime.py
--rw-r--r--   0        0        0    10106 2024-05-16 13:01:21.356843 prettypretty-0.1.0/test/test_color.py
--rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 prettypretty-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1891 2024-05-16 19:41:31.436717 prettypretty-0.2.0/.github/workflows/gh-pages.yml
+-rw-r--r--   0        0        0     2793 2024-05-02 16:16:46.878000 prettypretty-0.2.0/.gitignore
+-rw-r--r--   0        0        0      351 2024-05-08 11:44:14.092903 prettypretty-0.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0    11358 2024-05-10 23:06:53.590972 prettypretty-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2644 2024-05-17 00:06:53.091896 prettypretty-0.2.0/README.md
+-rw-r--r--   0        0        0      634 2024-05-06 06:14:58.399937 prettypretty-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0     1459 2024-05-16 22:39:39.714324 prettypretty-0.2.0/docs/apidocs/color.rst
+-rw-r--r--   0        0        0      299 2024-05-16 19:27:36.542585 prettypretty-0.2.0/docs/apidocs/prettypretty.rst
+-rw-r--r--   0        0        0     1837 2024-05-16 12:45:08.223904 prettypretty-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0     5390 2024-05-15 17:10:11.260351 prettypretty-0.2.0/docs/conversions.rst
+-rw-r--r--   0        0        0   205416 2024-05-16 23:49:30.072296 prettypretty-0.2.0/docs/figures/rgb6-ansi-iterm2.png
+-rw-r--r--   0        0        0   402258 2024-05-16 23:49:17.744169 prettypretty-0.2.0/docs/figures/rgb6-ansi-macos.png
+-rw-r--r--   0        0        0   459630 2024-05-16 23:49:27.026617 prettypretty-0.2.0/docs/figures/rgb6-background.png
+-rw-r--r--   0        0        0   451366 2024-05-16 23:49:25.445383 prettypretty-0.2.0/docs/figures/rgb6-text.png
+-rw-r--r--   0        0        0     4210 2024-05-13 23:07:43.595548 prettypretty-0.2.0/docs/formats-and-spaces.rst
+-rw-r--r--   0        0        0     3500 2024-05-17 00:07:11.716839 prettypretty-0.2.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-05-06 06:14:58.400754 prettypretty-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0      319 2024-05-16 22:40:04.066388 prettypretty-0.2.0/docs/tools.rst
+-rw-r--r--   0        0        0     1091 2024-05-02 16:16:18.007588 prettypretty-0.2.0/package-lock.json
+-rw-r--r--   0        0        0       54 2024-05-02 16:16:09.342077 prettypretty-0.2.0/package.json
+-rw-r--r--   0        0        0       22 2024-05-17 00:10:25.518484 prettypretty-0.2.0/prettypretty/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 20:14:19.249777 prettypretty-0.2.0/prettypretty/color/__init__.py
+-rw-r--r--   0        0        0     3643 2024-05-15 04:46:14.229875 prettypretty-0.2.0/prettypretty/color/apca.py
+-rw-r--r--   0        0        0    12096 2024-05-16 22:58:18.351293 prettypretty-0.2.0/prettypretty/color/conversion.py
+-rw-r--r--   0        0        0     1865 2024-05-15 03:43:07.902917 prettypretty-0.2.0/prettypretty/color/difference.py
+-rw-r--r--   0        0        0     8633 2024-05-16 22:58:25.188032 prettypretty-0.2.0/prettypretty/color/lores.py
+-rw-r--r--   0        0        0     6109 2024-05-15 23:55:49.255258 prettypretty-0.2.0/prettypretty/color/serde.py
+-rw-r--r--   0        0        0     7174 2024-05-15 03:48:44.497474 prettypretty-0.2.0/prettypretty/color/space.py
+-rw-r--r--   0        0        0     2773 2024-05-16 04:27:39.507626 prettypretty-0.2.0/prettypretty/color/spec.py
+-rw-r--r--   0        0        0      634 2024-05-05 17:58:20.659244 prettypretty-0.2.0/prettypretty/color/style.py
+-rw-r--r--   0        0        0     4631 2024-05-16 04:45:02.880375 prettypretty-0.2.0/prettypretty/color/theme.py
+-rw-r--r--   0        0        0     7453 2024-05-16 19:25:15.223741 prettypretty-0.2.0/prettypretty/color_object.py
+-rw-r--r--   0        0        0     7796 2024-05-16 23:06:50.625401 prettypretty-0.2.0/prettypretty/grid.py
+-rw-r--r--   0        0        0    15321 2024-05-16 19:34:53.347084 prettypretty-0.2.0/prettypretty/termio.py
+-rw-r--r--   0        0        0      856 2024-05-16 19:44:38.278771 prettypretty-0.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0     1507 2024-05-10 00:55:29.680752 prettypretty-0.2.0/runtest.py
+-rw-r--r--   0        0        0       49 2024-05-10 01:03:55.934703 prettypretty-0.2.0/test/__init__.py
+-rw-r--r--   0        0        0     9112 2024-05-02 16:13:52.778390 prettypretty-0.2.0/test/runtime.py
+-rw-r--r--   0        0        0    10115 2024-05-16 19:30:16.747923 prettypretty-0.2.0/test/test_color.py
+-rw-r--r--   0        0        0     3411 1970-01-01 00:00:00.000000 prettypretty-0.2.0/PKG-INFO
```

### Comparing `prettypretty-0.1.0/.gitignore` & `prettypretty-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `prettypretty-0.1.0/LICENSE` & `prettypretty-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prettypretty-0.1.0/docs/Makefile` & `prettypretty-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `prettypretty-0.1.0/docs/apidocs/color.rst` & `prettypretty-0.2.0/docs/apidocs/color.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-prettypretty.color.core
-=======================
+prettypretty.color
+==================
 
-The modules in ``prettypretty.color`` implement the low-level color API. Most
-modules have limited dependencies on the standard library but otherwise stand on
-their own. A few modules pull in :mod:`prettypretty.color.spec`, which provides
-common type definitions. But :mod:`prettypretty.color.grid` and
-:mod:`prettypretty.color.lores` pull in several other color modules.
+Prettypretty's low-level color API. Much of the functionality is implemented
+through a simple procedural API and different modules are largely independent
+from each other. The one exception is :mod:`prettypretty.color.lores`, which
+implements support for low-resolution terminal colors with help of the
+:mod:`prettypretty.color.conversion`, :mod:`prettypretty.color.difference`, and
+:mod:`prettypretty.color.theme` modules.
 
 
 prettypretty.color.apca
 -----------------------
 
 .. automodule:: prettypretty.color.apca
     :members:
@@ -25,21 +26,14 @@
 prettypretty.color.difference
 -----------------------------
 
 .. automodule:: prettypretty.color.difference
     :members:
 
 
-prettypretty.color.grid
------------------------
-
-.. automodule:: prettypretty.color.grid
-    :members:
-
-
 prettypretty.color.lores
 ------------------------
 
 .. automodule:: prettypretty.color.lores
     :members:
```

### Comparing `prettypretty-0.1.0/docs/conf.py` & `prettypretty-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `prettypretty-0.1.0/docs/conversions.rst` & `prettypretty-0.2.0/docs/conversions.rst`

 * *Files identical despite different names*

### Comparing `prettypretty-0.1.0/docs/formats-and-spaces.rst` & `prettypretty-0.2.0/docs/formats-and-spaces.rst`

 * *Files identical despite different names*

### Comparing `prettypretty-0.1.0/docs/make.bat` & `prettypretty-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `prettypretty-0.1.0/package-lock.json` & `prettypretty-0.2.0/package-lock.json`

 * *Files identical despite different names*

### Comparing `prettypretty-0.1.0/prettypretty/api/color.py` & `prettypretty-0.2.0/prettypretty/color_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from collections.abc import Iterable
 from typing import cast, Literal, overload, Self
 
-from ..color.apca import contrast, use_black_text, use_black_background
-from ..color.conversion import get_converter
-from ..color.difference import deltaE_oklab, closest_oklab
-from ..color.serde import (
+from .color.apca import contrast, use_black_text, use_black_background
+from .color.conversion import get_converter
+from .color.difference import deltaE_oklab, closest_oklab
+from .color.serde import (
     parse_format_spec,
     parse_hex,
     parse_x_rgb,
     parse_x_rgbi,
     stringify,
 )
-from ..color.space import EPSILON, is_tag, resolve, Space
-from ..color.spec import ColorSpec, CoordinateSpec, FloatCoordinateSpec
+from .color.space import EPSILON, is_tag, resolve, Space
+from .color.spec import ColorSpec, CoordinateSpec, FloatCoordinateSpec
 
 
 class Color(ColorSpec):
     """
     A color object.
 
     This class implements the high-level, object-oriented API for colors.
```

### Comparing `prettypretty-0.1.0/prettypretty/color/apca.py` & `prettypretty-0.2.0/prettypretty/color/apca.py`

 * *Files identical despite different names*

### Comparing `prettypretty-0.1.0/prettypretty/color/conversion.py` & `prettypretty-0.2.0/prettypretty/color/conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 import itertools
 import math
 from typing import cast, TypeAlias
 
 from .spec import ConverterSpec, CoordinateSpec
 
 
-_RGB6_TO_RGB256 = (0, 0x5F, 0x87, 0xAF, 0xD7, 0xFF)
-
 # See https://github.com/color-js/color.js/blob/a77e080a070039c534dda3965a769675aac5f75e/src/spaces/srgb-linear.js
 
 _XYZ_TO_LINEAR_SRGB = (
 	(  3.2409699419045226,  -1.537383177570094,   -0.4986107602930034  ),
 	( -0.9692436362808796,   1.8759675015077202,   0.04155505740717559 ),
 	(  0.05563007969699366, -0.20397695888897652,  1.0569715142428786  ),
 )
@@ -324,15 +322,15 @@
         _collect_conversions(vars(mod), _converter_cache)
         _collected_mod_lores = True
 
     # Determine route. Only the first and/or last node can be lo-res.
     route: list[str] = [source] if is_source_lores else []
 
     route.extend(_elaborate_route(
-        'rgb256' if is_source_lores else source,
+        'srgb' if is_source_lores else source,
         'oklab' if is_target_lores else target,
     ))
 
     if is_target_lores:
         route.append(target)
 
     # Turn list of nodes into list of functions into converter function
```

### Comparing `prettypretty-0.1.0/prettypretty/color/difference.py` & `prettypretty-0.2.0/prettypretty/color/difference.py`

 * *Files identical despite different names*

### Comparing `prettypretty-0.1.0/prettypretty/color/grid.py` & `prettypretty-0.2.0/prettypretty/grid.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """
 A script to visualize 8-bit terminal colors as well as prettypretty's support
 for down-sampling colors and maximizing contrast.
 """
 import argparse
 import os
 
-from .conversion import rgb256_to_srgb, get_converter
-from .apca import use_black_text, use_black_background
-from .lores import (
+from .color.conversion import get_converter
+from .color.apca import use_black_text, use_black_background
+from .color.lores import (
     rgb6_to_eight_bit,
-    rgb6_to_rgb256,
-    eight_bit_to_rgb256,
+    rgb6_to_srgb,
+    eight_bit_to_srgb,
     oklab_to_ansi,
     oklab_to_eight_bit,
 )
-from .theme import MACOS_TERMINAL, VGA, XTERM, current_theme
-from .style import eight_bit_to_sgr_params, Layer, sgr
+from .color.theme import MACOS_TERMINAL, VGA, XTERM, current_theme
+from .color.style import eight_bit_to_sgr_params, Layer, sgr
+from .termio import TermIO
+
 
 class FramedBoxes:
     """
     Boxes in a frame.
 
     This class helps with incrementally formatting a grid of boxes with a
     surrounding frame (or border). Each box has the same width and a height of
@@ -134,29 +136,28 @@
     frame.top(
         layer.name.capitalize()
         + ': '
         + ('Downsampled ' if ansi_only else '')
         + '6•6•6 RGB Cube'
     )
 
-    rgb256_to_oklab = get_converter('rgb256', 'oklab')
+    srgb_to_oklab = get_converter('srgb', 'oklab')
 
     for r in range(6):
         for b in range(6):
             frame.left()
 
             for g in range(6):
-                rgb256 = rgb6_to_rgb256(r, g, b)
+                srgb = rgb6_to_srgb(r, g, b)
 
                 if ansi_only:
-                    eight_bit = oklab_to_ansi(*rgb256_to_oklab(*rgb256))
-                    srgb = rgb256_to_srgb(*eight_bit_to_rgb256(*eight_bit))
+                    eight_bit = oklab_to_ansi(*srgb_to_oklab(*srgb))
+                    srgb = eight_bit_to_srgb(*eight_bit)
                 else:
                     eight_bit = rgb6_to_eight_bit(r, g, b)
-                    srgb = rgb256_to_srgb(*rgb256)
 
                 # Pick black or white for other color based on contrast
                 if layer is Layer.BACKGROUND:
                     foreground = (232 if use_black_text(*srgb) else 255),
                     background = eight_bit
                 else:
                     foreground = eight_bit
@@ -234,15 +235,23 @@
     return parser
 
 
 if __name__ == '__main__':
     options = create_parser().parse_args()
     width, _ = os.get_terminal_size()
 
-    with current_theme(options.theme or VGA):
+    theme = options.theme
+    if theme is None:
+        termio = TermIO()
+        with termio.cbread_mode():
+            theme = TermIO().extract_theme()
+    if theme is None:
+        theme = VGA
+
+    with current_theme(theme):
         print(f'\n{format_color_cube(width)}')
         print(f'\n{format_color_cube(width, ansi_only=True)}')
         print(f'\n{format_color_cube(width, layer=Layer.TEXT)}')
 
         if os.getenv('COLORTERM') == 'truecolor':
             print(f'\n{format_hires_slice(width)}')
             print(f'\n{format_hires_slice(width, eight_bit_only=True)}')
```

### Comparing `prettypretty-0.1.0/prettypretty/color/lores.py` & `prettypretty-0.2.0/prettypretty/color/lores.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 """
 Support for low-resolution terminal colors
 """
 from itertools import chain
 from typing import Callable, cast
 
-# Rename basic conversion to prevent it from tripping up module scan
-from .conversion import get_converter, rgb256_to_srgb as rgb256_into_srgb
+# Make imported conversion private so that it won't be collected a second time
+from .conversion import get_converter, rgb256_to_srgb as _rgb256_to_srgb
 from .difference import closest_oklab
 from .spec import CoordinateVectorSpec
 from .theme import current_theme, Theme
 
 
 _RGB6_TO_RGB256 = (0, 0x5F, 0x87, 0xAF, 0xD7, 0xFF)
 
 
+def ansi_to_eight_bit(color: int) -> tuple[int]:
+    """
+    Convert the given ANSI color to 8-bit format. This function implements the
+    identity transform for the color value.
+    """
+    return color,
+
+
 def rgb6_to_eight_bit(r: int, g: int, b: int) -> tuple[int]:
     """
     Convert the given color from the 6x6x6 RGB cube of 8-bit terminal colors to
     an actual 8-bit terminal color.
     """
     assert 0 <= r <= 5 and 0 <= g <= 5 and 0 <= b <= 5
     return 16 + 36 * r + 6 * g + b,
@@ -70,19 +78,14 @@
             return index if level - value < value - previous_level else index - 1
 
         assert False, 'unreachable statement'
 
     return convert(r), convert(g), convert(b)
 
 
-def ansi_to_eight_bit(color: int) -> tuple[int]:
-    """Convert the given ANSI color to 8-bit format."""
-    return color,
-
-
 def ansi_to_rgb256(color: int) -> tuple[int, int, int]:
     """
     :bdg-warning:`Lossy conversion` Convert the given ANSI color to RGB256
     format.
 
     .. warning::
         The result of this function critically depends on the current color
@@ -92,40 +95,14 @@
     assert 0 <= color <= 15
     c = current_theme().ansi(color)
 
     assert c.tag == 'rgb256'
     return c.coordinates  # type: ignore
 
 
-def ansi_to_srgb(color: int) -> tuple[float, float, float]:
-    """
-    Convert the ANSI color to sRGB. Directly converting to sRGB and avoiding
-    RGB256 is the more conservative conversion because most terminals, when
-    queried with OSC-4, report color values with four hexadecimal digits per
-    coordinate. RGB256 obviously cannot preserve that resolution, though sRGB
-    can.
-
-    .. warning::
-        The result of this function critically depends on the current color
-        theme. After all, the current theme determines the RGB256 values for all
-        extended ANSI colors.
-    """
-    assert 0 <= color <= 15
-    c = current_theme().ansi(color)
-
-    if c.tag == 'rg256':
-        coordinates = rgb256_into_srgb(*cast(tuple[int, int, int], c.coordinates))
-    elif c.tag == 'srgb':
-        coordinates = c.coordinates
-    else:
-        coordinates = get_converter(c.tag, 'srgb')(*c.coordinates)
-
-    return cast(tuple[float, float, float], coordinates)
-
-
 def _eight_bit_gray_to_rgb256(color: int) -> tuple[int, int, int]:
     """Convert the given 8-bit gray to RGB256 format."""
     assert 232 <= color <= 255
     c = 10 * (color - 232) + 8
     return c, c, c
 
 
@@ -145,29 +122,61 @@
         return rgb6_to_rgb256(*eight_bit_to_rgb6(color))
     if 232 <= color <= 255:
         return _eight_bit_gray_to_rgb256(color)
 
     raise ValueError(f'{color} is not a valid 8-bit terminal color')
 
 
+def ansi_to_srgb(color: int) -> tuple[float, float, float]:
+    """
+    Convert the ANSI color to sRGB. Directly converting to sRGB and avoiding
+    RGB256 is the more conservative conversion because most terminals, when
+    queried with OSC-4, report color values with four hexadecimal digits per
+    coordinate. RGB256 obviously cannot preserve that resolution, though sRGB
+    can.
+
+    .. warning::
+        The result of this function critically depends on the current color
+        theme. After all, the current theme determines the RGB256 values for all
+        extended ANSI colors.
+    """
+    assert 0 <= color <= 15
+    c = current_theme().ansi(color)
+
+    if c.tag == 'rg256':
+        coordinates = _rgb256_to_srgb(*cast(tuple[int, int, int], c.coordinates))
+    elif c.tag == 'srgb':
+        coordinates = c.coordinates
+    else:
+        coordinates = get_converter(c.tag, 'srgb')(*c.coordinates)
+
+    return cast(tuple[float, float, float], coordinates)
+
+
+def rgb6_to_srgb(r: int, g: int, b: int) -> tuple[float, float, float]:
+    """Convert the given color in RGB6 format to sRGB format."""
+    assert 0 <= r <= 5 and 0 <= g <= 5 and 0 <= b <= 5
+    return _rgb256_to_srgb(*rgb6_to_rgb256(r, g, b))
+
+
 def eight_bit_to_srgb(color: int) -> tuple[float, float, float]:
     """
     Convert the given 8-bit terminal color to sRGB.
 
     .. warning::
         The result of this function may depend on the current color theme.
         It provides RGB256 color values for 8-bit colors 0–15, i.e., the
         extended ANSI colors.
     """
     if 0 <= color <= 15:
         return ansi_to_srgb(color)
     if 16 <= color <= 231:
-        return rgb256_into_srgb(*rgb6_to_rgb256(*eight_bit_to_rgb6(color)))
+        return _rgb256_to_srgb(*rgb6_to_rgb256(*eight_bit_to_rgb6(color)))
     if 232 <= color <= 255:
-        return rgb256_into_srgb(*_eight_bit_gray_to_rgb256(color))
+        return _rgb256_to_srgb(*_eight_bit_gray_to_rgb256(color))
 
     raise ValueError(f'{color} is not a valid 8-bit terminal color')
 
 
 # --------------------------------------------------------------------------------------
 
 
@@ -180,24 +189,24 @@
         self._rgb: None | CoordinateVectorSpec = None
         self._gray: None | CoordinateVectorSpec = None
         self._convert: None | _RGB256_TO_OKLAB = None
 
     @property
     def convert(self) -> _RGB256_TO_OKLAB:
         if self._convert is None:
-            setattr(self, '_convert', get_converter('rgb256', 'oklab'))
+            setattr(self, '_convert', get_converter('srgb', 'oklab'))
         assert self._convert is not None
         return self._convert
 
     @property
     def ansi(self) -> CoordinateVectorSpec:
         theme = current_theme()
         if theme not in self._ansi:
             self._ansi[theme] = tuple(
-                (self.convert if c.tag == 'srgb256' else get_converter(c.tag, 'oklab'))
+                (self.convert if c.tag == 'srgb' else get_converter(c.tag, 'oklab'))
                 (*c.coordinates)  # type: ignore
                 for n, c in theme.colors() if n not in ('text', 'background')
             )
         return self._ansi[theme]
 
     @property
     def rgb(self) -> CoordinateVectorSpec:
```

### Comparing `prettypretty-0.1.0/prettypretty/color/serde.py` & `prettypretty-0.2.0/prettypretty/color/serde.py`

 * *Files identical despite different names*

### Comparing `prettypretty-0.1.0/prettypretty/color/space.py` & `prettypretty-0.2.0/prettypretty/color/space.py`

 * *Files identical despite different names*

### Comparing `prettypretty-0.1.0/prettypretty/color/spec.py` & `prettypretty-0.2.0/prettypretty/color/spec.py`

 * *Files identical despite different names*

### Comparing `prettypretty-0.1.0/prettypretty/color/style.py` & `prettypretty-0.2.0/prettypretty/color/style.py`

 * *Files identical despite different names*

### Comparing `prettypretty-0.1.0/prettypretty/color/theme.py` & `prettypretty-0.2.0/prettypretty/color/theme.py`

 * *Files identical despite different names*

### Comparing `prettypretty-0.1.0/pyproject.toml` & `prettypretty-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     "sphinxcontrib-autoprogram",
     "sphinx_design",
     "sphinx-rtd-theme",
 ]
 
 [project.urls]
 repository = "https://github.com/apparebit/prettypretty"
+package = "https://pypi.org/project/prettypretty/"
+documentation= "https://apparebit.github.io/prettypretty/"
 
 [build-system]
 requires = ["flit_core >=3.4"]
 build-backend = "flit_core.buildapi"
 
 [tool.pyright]
 include = ["prettypretty/**/*.py", "test/*.py", "runtest.py"]
```

### Comparing `prettypretty-0.1.0/runtest.py` & `prettypretty-0.2.0/runtest.py`

 * *Files identical despite different names*

### Comparing `prettypretty-0.1.0/test/runtime.py` & `prettypretty-0.2.0/test/runtime.py`

 * *Files identical despite different names*

### Comparing `prettypretty-0.1.0/test/test_color.py` & `prettypretty-0.2.0/test/test_color.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from prettypretty.color.serde import (
     parse_hex,
     parse_x_rgb,
     parse_x_rgbi,
 )
 
 from prettypretty.color.theme import VGA
-from prettypretty.api import Color
+from prettypretty.color_object import Color
 
 
 @dataclass(frozen=True)
 class ColorValues:
     spec: str
     parsed: tuple[int, int, int]
     srgb: tuple[float, float, float]
```

