# Comparing `tmp/fig2sketch-0.3.0.tar.gz` & `tmp/fig2sketch-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fig2sketch-0.3.0.tar", last modified: Thu May 16 15:25:49 2024, max compression
+gzip compressed data, was "fig2sketch-0.3.1.tar", last modified: Thu May 16 16:22:34 2024, max compression
```

## Comparing `fig2sketch-0.3.0.tar` & `fig2sketch-0.3.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:25:49.288202 fig2sketch-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-05-16 15:25:49.288202 fig2sketch-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 15:25:49.288202 fig2sketch-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:25:49.280202 fig2sketch-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:25:49.284202 fig2sketch-0.3.0/src/converter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/artboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/component.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/document.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/font.py
--rw-r--r--   0 runner    (1001) docker     (127)    34002 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/font_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11428 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/positioning.py
--rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/prototype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/shape.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/shape_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    12579 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/shape_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/slice.py
--rw-r--r--   0 runner    (1001) docker     (127)    12979 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)    12487 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/converter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:25:49.288202 fig2sketch-0.3.0/src/fig2sketch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-05-16 15:25:49.000000 fig2sketch-0.3.0/src/fig2sketch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-16 15:25:49.000000 fig2sketch-0.3.0/src/fig2sketch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:25:49.000000 fig2sketch-0.3.0/src/fig2sketch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-16 15:25:49.000000 fig2sketch-0.3.0/src/fig2sketch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-16 15:25:49.000000 fig2sketch-0.3.0/src/fig2sketch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-16 15:25:49.000000 fig2sketch-0.3.0/src/fig2sketch.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     3382 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/fig2sketch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:25:49.284202 fig2sketch-0.3.0/src/figformat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/figformat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/figformat/decodefig.py
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/figformat/fig2tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/figformat/kiwi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/figformat/vector_network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:25:49.288202 fig2sketch-0.3.0/src/sketchformat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/sketchformat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/sketchformat/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/sketchformat/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/sketchformat/layer_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/sketchformat/layer_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/sketchformat/layer_shape.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/sketchformat/prototype.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:25:49.288202 fig2sketch-0.3.0/src/sketchformat/serialize/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/sketchformat/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/sketchformat/serialize/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/sketchformat/serialize/orjson.py
--rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/sketchformat/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-16 15:25:45.000000 fig2sketch-0.3.0/src/sketchformat/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:22:34.068167 fig2sketch-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-05-16 16:22:34.068167 fig2sketch-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 16:22:34.068167 fig2sketch-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:22:34.060166 fig2sketch-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:22:34.064166 fig2sketch-0.3.1/src/converter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/artboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/font.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34002 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/font_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11428 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/positioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/prototype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/shape_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12579 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/shape_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12979 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12487 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/converter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:22:34.068167 fig2sketch-0.3.1/src/fig2sketch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-05-16 16:22:34.000000 fig2sketch-0.3.1/src/fig2sketch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-16 16:22:34.000000 fig2sketch-0.3.1/src/fig2sketch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 16:22:34.000000 fig2sketch-0.3.1/src/fig2sketch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-16 16:22:34.000000 fig2sketch-0.3.1/src/fig2sketch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-16 16:22:34.000000 fig2sketch-0.3.1/src/fig2sketch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-16 16:22:34.000000 fig2sketch-0.3.1/src/fig2sketch.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3382 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/fig2sketch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:22:34.068167 fig2sketch-0.3.1/src/figformat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/figformat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/figformat/decodefig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/figformat/fig2tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/figformat/kiwi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/figformat/vector_network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:22:34.068167 fig2sketch-0.3.1/src/sketchformat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/sketchformat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/sketchformat/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/sketchformat/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/sketchformat/layer_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/sketchformat/layer_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/sketchformat/layer_shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/sketchformat/prototype.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:22:34.068167 fig2sketch-0.3.1/src/sketchformat/serialize/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/sketchformat/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/sketchformat/serialize/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/sketchformat/serialize/orjson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/sketchformat/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-16 16:22:30.000000 fig2sketch-0.3.1/src/sketchformat/text.py
```

### Comparing `fig2sketch-0.3.0/LICENSE` & `fig2sketch-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/PKG-INFO` & `fig2sketch-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fig2sketch
-Version: 0.3.0
+Version: 0.3.1
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Pillow==10.3.0
 Requires-Dist: fonttools==4.43.0
 Requires-Dist: appdirs==1.4.4
 Provides-Extra: fast
```

### Comparing `fig2sketch-0.3.0/README.md` & `fig2sketch-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/pyproject.toml` & `fig2sketch-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/converter/artboard.py` & `fig2sketch-0.3.1/src/converter/artboard.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/converter/base.py` & `fig2sketch-0.3.1/src/converter/base.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/converter/component.py` & `fig2sketch-0.3.1/src/converter/component.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/converter/context.py` & `fig2sketch-0.3.1/src/converter/context.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/converter/convert.py` & `fig2sketch-0.3.1/src/converter/convert.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/converter/document.py` & `fig2sketch-0.3.1/src/converter/document.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/converter/font.py` & `fig2sketch-0.3.1/src/converter/font.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,18 @@
     raise FontNotFoundError(f"Could not find font {family} {subfamily}")
 
 
 def convert(
     name: Tuple[str, str], font_file: IO[bytes], postscript: str, output_zip: ZipFile
 ) -> FontReference:
     family, subfamily = name
+
+    font_file.seek(0)
     data = font_file.read()
+
     sha = utils.generate_file_ref(data)
     path = f"fonts/{sha}"
     output_zip.open(path, "w").write(data)
 
     return FontReference(
         do_objectID=utils.gen_object_id((0, 0), bytes.fromhex(sha)),
         fontData=JsonFileReference(_ref_class="MSFontData", _ref=path),
```

### Comparing `fig2sketch-0.3.0/src/converter/font_features.py` & `fig2sketch-0.3.1/src/converter/font_features.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/converter/group.py` & `fig2sketch-0.3.1/src/converter/group.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/converter/instance.py` & `fig2sketch-0.3.1/src/converter/instance.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/converter/meta.py` & `fig2sketch-0.3.1/src/converter/meta.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/converter/page.py` & `fig2sketch-0.3.1/src/converter/page.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/converter/positioning.py` & `fig2sketch-0.3.1/src/converter/positioning.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/converter/prototype.py` & `fig2sketch-0.3.1/src/converter/prototype.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/converter/rectangle.py` & `fig2sketch-0.3.1/src/converter/rectangle.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/converter/shape_group.py` & `fig2sketch-0.3.1/src/converter/shape_group.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/converter/shape_path.py` & `fig2sketch-0.3.1/src/converter/shape_path.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/converter/style.py` & `fig2sketch-0.3.1/src/converter/style.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/converter/symbol.py` & `fig2sketch-0.3.1/src/converter/symbol.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/converter/text.py` & `fig2sketch-0.3.1/src/converter/text.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/converter/tree.py` & `fig2sketch-0.3.1/src/converter/tree.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/converter/user.py` & `fig2sketch-0.3.1/src/converter/user.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/converter/utils.py` & `fig2sketch-0.3.1/src/converter/utils.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/fig2sketch.egg-info/PKG-INFO` & `fig2sketch-0.3.1/src/fig2sketch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fig2sketch
-Version: 0.3.0
+Version: 0.3.1
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Pillow==10.3.0
 Requires-Dist: fonttools==4.43.0
 Requires-Dist: appdirs==1.4.4
 Provides-Extra: fast
```

### Comparing `fig2sketch-0.3.0/src/fig2sketch.egg-info/SOURCES.txt` & `fig2sketch-0.3.1/src/fig2sketch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/fig2sketch.py` & `fig2sketch-0.3.1/src/fig2sketch.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/figformat/decodefig.py` & `fig2sketch-0.3.1/src/figformat/decodefig.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/figformat/fig2tree.py` & `fig2sketch-0.3.1/src/figformat/fig2tree.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/figformat/kiwi.py` & `fig2sketch-0.3.1/src/figformat/kiwi.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/figformat/vector_network.py` & `fig2sketch-0.3.1/src/figformat/vector_network.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/sketchformat/common.py` & `fig2sketch-0.3.1/src/sketchformat/common.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/sketchformat/document.py` & `fig2sketch-0.3.1/src/sketchformat/document.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/sketchformat/layer_common.py` & `fig2sketch-0.3.1/src/sketchformat/layer_common.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/sketchformat/layer_group.py` & `fig2sketch-0.3.1/src/sketchformat/layer_group.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/sketchformat/layer_shape.py` & `fig2sketch-0.3.1/src/sketchformat/layer_shape.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/sketchformat/prototype.py` & `fig2sketch-0.3.1/src/sketchformat/prototype.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/sketchformat/serialize/json.py` & `fig2sketch-0.3.1/src/sketchformat/serialize/json.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/sketchformat/serialize/orjson.py` & `fig2sketch-0.3.1/src/sketchformat/serialize/orjson.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/sketchformat/style.py` & `fig2sketch-0.3.1/src/sketchformat/style.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.3.0/src/sketchformat/text.py` & `fig2sketch-0.3.1/src/sketchformat/text.py`

 * *Files identical despite different names*

