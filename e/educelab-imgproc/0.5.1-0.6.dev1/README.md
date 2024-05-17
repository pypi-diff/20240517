# Comparing `tmp/educelab-imgproc-0.5.1.tar.gz` & `tmp/educelab_imgproc-0.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "educelab-imgproc-0.5.1.tar", last modified: Wed Nov  8 18:45:28 2023, max compression
+gzip compressed data, was "educelab_imgproc-0.6.dev1.tar", last modified: Fri May 17 17:06:25 2024, max compression
```

## Comparing `educelab-imgproc-0.5.1.tar` & `educelab_imgproc-0.6.dev1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-11-08 18:45:28.626155 educelab-imgproc-0.5.1/
--rw-r--r--   0 seth       (501) staff       (20)    34458 2023-03-30 17:42:22.000000 educelab-imgproc-0.5.1/LICENSE
--rw-r--r--   0 seth       (501) staff       (20)     1604 2023-11-08 18:45:28.626099 educelab-imgproc-0.5.1/PKG-INFO
--rw-r--r--   0 seth       (501) staff       (20)      653 2023-04-06 00:38:08.000000 educelab-imgproc-0.5.1/README.md
--rw-r--r--   0 seth       (501) staff       (20)      103 2023-03-30 17:42:22.000000 educelab-imgproc-0.5.1/pyproject.toml
--rw-r--r--   0 seth       (501) staff       (20)       68 2023-06-02 14:26:57.000000 educelab-imgproc-0.5.1/requirements.txt
--rw-r--r--   0 seth       (501) staff       (20)      918 2023-11-08 18:45:28.626410 educelab-imgproc-0.5.1/setup.cfg
-drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-11-08 18:45:28.623252 educelab-imgproc-0.5.1/src/
-drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-11-08 18:45:28.623180 educelab-imgproc-0.5.1/src/educelab/
-drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-11-08 18:45:28.625247 educelab-imgproc-0.5.1/src/educelab/imgproc/
--rw-r--r--   0 seth       (501) staff       (20)      364 2023-06-02 14:26:57.000000 educelab-imgproc-0.5.1/src/educelab/imgproc/__init__.py
--rw-r--r--   0 seth       (501) staff       (20)     2071 2023-06-02 14:26:57.000000 educelab-imgproc-0.5.1/src/educelab/imgproc/adjust.py
--rw-r--r--   0 seth       (501) staff       (20)      715 2023-04-06 00:33:44.000000 educelab-imgproc-0.5.1/src/educelab/imgproc/conversion.py
--rw-r--r--   0 seth       (501) staff       (20)      835 2023-04-06 00:33:44.000000 educelab-imgproc-0.5.1/src/educelab/imgproc/correction.py
--rw-r--r--   0 seth       (501) staff       (20)     3910 2023-05-10 17:49:06.000000 educelab-imgproc-0.5.1/src/educelab/imgproc/enhance.py
--rw-r--r--   0 seth       (501) staff       (20)     2673 2023-11-08 18:44:06.000000 educelab-imgproc-0.5.1/src/educelab/imgproc/exiftool.py
--rw-r--r--   0 seth       (501) staff       (20)      241 2023-05-10 16:08:03.000000 educelab-imgproc-0.5.1/src/educelab/imgproc/filters.py
--rw-r--r--   0 seth       (501) staff       (20)     2048 2023-04-06 00:33:44.000000 educelab-imgproc-0.5.1/src/educelab/imgproc/pca.py
--rw-r--r--   0 seth       (501) staff       (20)     5316 2023-06-02 14:26:57.000000 educelab-imgproc-0.5.1/src/educelab/imgproc/pipeline.py
--rw-r--r--   0 seth       (501) staff       (20)      718 2023-06-02 14:26:57.000000 educelab-imgproc-0.5.1/src/educelab/imgproc/properties.py
--rw-r--r--   0 seth       (501) staff       (20)     1027 2023-04-06 00:33:44.000000 educelab-imgproc-0.5.1/src/educelab/imgproc/roi.py
-drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-11-08 18:45:28.625784 educelab-imgproc-0.5.1/src/educelab_imgproc.egg-info/
--rw-r--r--   0 seth       (501) staff       (20)     1604 2023-11-08 18:45:28.000000 educelab-imgproc-0.5.1/src/educelab_imgproc.egg-info/PKG-INFO
--rw-r--r--   0 seth       (501) staff       (20)      633 2023-11-08 18:45:28.000000 educelab-imgproc-0.5.1/src/educelab_imgproc.egg-info/SOURCES.txt
--rw-r--r--   0 seth       (501) staff       (20)        1 2023-11-08 18:45:28.000000 educelab-imgproc-0.5.1/src/educelab_imgproc.egg-info/dependency_links.txt
--rw-r--r--   0 seth       (501) staff       (20)      101 2023-11-08 18:45:28.000000 educelab-imgproc-0.5.1/src/educelab_imgproc.egg-info/requires.txt
--rw-r--r--   0 seth       (501) staff       (20)        9 2023-11-08 18:45:28.000000 educelab-imgproc-0.5.1/src/educelab_imgproc.egg-info/top_level.txt
+drwxr-xr-x   0 seth       (501) staff       (20)        0 2024-05-17 17:06:25.474931 educelab_imgproc-0.6.dev1/
+-rw-r--r--   0 seth       (501) staff       (20)    34458 2023-03-30 17:42:22.000000 educelab_imgproc-0.6.dev1/LICENSE
+-rw-r--r--   0 seth       (501) staff       (20)     1607 2024-05-17 17:06:25.474860 educelab_imgproc-0.6.dev1/PKG-INFO
+-rw-r--r--   0 seth       (501) staff       (20)      653 2023-04-06 00:38:08.000000 educelab_imgproc-0.6.dev1/README.md
+-rw-r--r--   0 seth       (501) staff       (20)      103 2023-03-30 17:42:22.000000 educelab_imgproc-0.6.dev1/pyproject.toml
+-rw-r--r--   0 seth       (501) staff       (20)       68 2023-06-02 14:26:57.000000 educelab_imgproc-0.6.dev1/requirements.txt
+-rw-r--r--   0 seth       (501) staff       (20)      921 2024-05-17 17:06:25.475180 educelab_imgproc-0.6.dev1/setup.cfg
+drwxr-xr-x   0 seth       (501) staff       (20)        0 2024-05-17 17:06:25.470655 educelab_imgproc-0.6.dev1/src/
+drwxr-xr-x   0 seth       (501) staff       (20)        0 2024-05-17 17:06:25.470584 educelab_imgproc-0.6.dev1/src/educelab/
+drwxr-xr-x   0 seth       (501) staff       (20)        0 2024-05-17 17:06:25.473845 educelab_imgproc-0.6.dev1/src/educelab/imgproc/
+-rw-r--r--   0 seth       (501) staff       (20)      364 2023-06-02 14:26:57.000000 educelab_imgproc-0.6.dev1/src/educelab/imgproc/__init__.py
+-rw-r--r--   0 seth       (501) staff       (20)     2071 2023-06-02 14:26:57.000000 educelab_imgproc-0.6.dev1/src/educelab/imgproc/adjust.py
+-rw-r--r--   0 seth       (501) staff       (20)      715 2023-04-06 00:33:44.000000 educelab_imgproc-0.6.dev1/src/educelab/imgproc/conversion.py
+-rw-r--r--   0 seth       (501) staff       (20)      835 2023-04-06 00:33:44.000000 educelab_imgproc-0.6.dev1/src/educelab/imgproc/correction.py
+-rw-r--r--   0 seth       (501) staff       (20)     3910 2023-05-10 17:49:06.000000 educelab_imgproc-0.6.dev1/src/educelab/imgproc/enhance.py
+-rw-r--r--   0 seth       (501) staff       (20)     2702 2023-11-08 18:57:38.000000 educelab_imgproc-0.6.dev1/src/educelab/imgproc/exiftool.py
+-rw-r--r--   0 seth       (501) staff       (20)      241 2023-05-10 16:08:03.000000 educelab_imgproc-0.6.dev1/src/educelab/imgproc/filters.py
+-rw-r--r--   0 seth       (501) staff       (20)     2048 2023-04-06 00:33:44.000000 educelab_imgproc-0.6.dev1/src/educelab/imgproc/pca.py
+-rw-r--r--   0 seth       (501) staff       (20)     5566 2024-05-16 21:05:06.000000 educelab_imgproc-0.6.dev1/src/educelab/imgproc/pipeline.py
+-rw-r--r--   0 seth       (501) staff       (20)      718 2023-06-02 14:26:57.000000 educelab_imgproc-0.6.dev1/src/educelab/imgproc/properties.py
+-rw-r--r--   0 seth       (501) staff       (20)     1027 2023-04-06 00:33:44.000000 educelab_imgproc-0.6.dev1/src/educelab/imgproc/roi.py
+drwxr-xr-x   0 seth       (501) staff       (20)        0 2024-05-17 17:06:25.474530 educelab_imgproc-0.6.dev1/src/educelab_imgproc.egg-info/
+-rw-r--r--   0 seth       (501) staff       (20)     1607 2024-05-17 17:06:25.000000 educelab_imgproc-0.6.dev1/src/educelab_imgproc.egg-info/PKG-INFO
+-rw-r--r--   0 seth       (501) staff       (20)      633 2024-05-17 17:06:25.000000 educelab_imgproc-0.6.dev1/src/educelab_imgproc.egg-info/SOURCES.txt
+-rw-r--r--   0 seth       (501) staff       (20)        1 2024-05-17 17:06:25.000000 educelab_imgproc-0.6.dev1/src/educelab_imgproc.egg-info/dependency_links.txt
+-rw-r--r--   0 seth       (501) staff       (20)      101 2024-05-17 17:06:25.000000 educelab_imgproc-0.6.dev1/src/educelab_imgproc.egg-info/requires.txt
+-rw-r--r--   0 seth       (501) staff       (20)        9 2024-05-17 17:06:25.000000 educelab_imgproc-0.6.dev1/src/educelab_imgproc.egg-info/top_level.txt
```

### Comparing `educelab-imgproc-0.5.1/LICENSE` & `educelab_imgproc-0.6.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `educelab-imgproc-0.5.1/PKG-INFO` & `educelab_imgproc-0.6.dev1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: educelab-imgproc
-Version: 0.5.1
+Version: 0.6.dev1
 Summary: EduceLab image processing module
 Home-page: https://educelab.gitlab.io/educelab-imgproc/
 Download-URL: https://gitlab.com/educelab/educelab-imgproc
 Author: Seth Parker
 Author-email: c.seth.parker@uky.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `educelab-imgproc-0.5.1/README.md` & `educelab_imgproc-0.6.dev1/README.md`

 * *Files identical despite different names*

### Comparing `educelab-imgproc-0.5.1/setup.cfg` & `educelab_imgproc-0.6.dev1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = educelab-imgproc
-version = 0.5.1
+version = 0.6.dev1
 author = Seth Parker
 author_email = c.seth.parker@uky.edu
 description = EduceLab image processing module
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://educelab.gitlab.io/educelab-imgproc/
 download_url = https://gitlab.com/educelab/educelab-imgproc
```

### Comparing `educelab-imgproc-0.5.1/src/educelab/imgproc/adjust.py` & `educelab_imgproc-0.6.dev1/src/educelab/imgproc/adjust.py`

 * *Files identical despite different names*

### Comparing `educelab-imgproc-0.5.1/src/educelab/imgproc/conversion.py` & `educelab_imgproc-0.6.dev1/src/educelab/imgproc/conversion.py`

 * *Files identical despite different names*

### Comparing `educelab-imgproc-0.5.1/src/educelab/imgproc/correction.py` & `educelab_imgproc-0.6.dev1/src/educelab/imgproc/correction.py`

 * *Files identical despite different names*

### Comparing `educelab-imgproc-0.5.1/src/educelab/imgproc/enhance.py` & `educelab_imgproc-0.6.dev1/src/educelab/imgproc/enhance.py`

 * *Files identical despite different names*

### Comparing `educelab-imgproc-0.5.1/src/educelab/imgproc/exiftool.py` & `educelab_imgproc-0.6.dev1/src/educelab/imgproc/exiftool.py`

 * *Files 11% similar despite different names*

```diff
@@ -56,19 +56,20 @@
     cmd.append(str(dest))
 
     # Run exiftool
     subprocess.run(cmd, check=True)
 
 
 def read_tags(file: Union[str, Path, List[Path]], tags: List[str] = None) -> \
-List[Dict]:
+        List[Dict]:
     """Get metadata tags for a file or list of files.
 
     :param file: Path or list of Paths to image files
-    :param tags: List of ExifTool tag strings, e.g. '[-ExposureTime, -ISO]'
+    :param tags: List of ExifTool tag strings, e.g.
+           :code:`['-ExposureTime', '-ISO']`
     :return: List of dicts containing tag values, one dict for each input path
     """
     # Setup metadata request
     cmd = ['exiftool', '-J']
 
     # Append all the other tags
     if tags is not None:
```

### Comparing `educelab-imgproc-0.5.1/src/educelab/imgproc/pca.py` & `educelab_imgproc-0.6.dev1/src/educelab/imgproc/pca.py`

 * *Files identical despite different names*

### Comparing `educelab-imgproc-0.5.1/src/educelab/imgproc/pipeline.py` & `educelab_imgproc-0.6.dev1/src/educelab/imgproc/pipeline.py`

 * *Files 13% similar despite different names*

```diff
@@ -36,16 +36,16 @@
     return textwrap.dedent("""\
     -brightness-contrast=BRIGHTNESS{,CONTRAST}
     \t\t\tBrightness/contrast adjustment
     -clahe{=KERNEL{,BINS}}
     \t\t\tContrast Limited Adaptive Histogram Equalization
     -clip{=MIN{,MAX}}
     \t\t\tClip values to range
-    -curves
-    \t\t\tCurves enhancement. Currently a preset enhancement curve.
+    -curves{=X0,Y0:X1,Y1:...:Xn,Yn}
+    \t\t\tCurves enhancement. Provide a series of semicolon separated XY pairs.
     -exposure{=VAL}
     \t\t\tAdjust image exposure
     -gamma{=GAMMA{,GAIN}}
     \t\t\tGamma correction
     -normalize
     \t\t\tLinear contrast stretch to data min/max
     -shadows=VAL
@@ -79,18 +79,25 @@
     def clip(sep, val):
         defaults = {'a_min': 0., 'a_max': 1.}
         parsed = parse_parameter_list(val, ['a_min', 'a_max'], [float, float])
         return defaults | parsed
 
     @staticmethod
     def curves(sep, val):
-        if sep != '' or val != '':
-            raise ValueError('-curves does not take parameters')
-        # TODO: currently a hardcoded enhancement curve
-        return {'x': [[0., 0.], [0.207, 0.118], [0.513, 0.473], [1., 1.]]}
+        if val == '':
+            return {'x': [[0., 0.], [0.207, 0.118], [0.513, 0.473], [1., 1.]]}
+
+        node_list = val.split(':')
+        node_list = [n.split(',') for n in node_list]
+        for idx, n in enumerate(node_list):
+            if len(n) != 2:
+                raise ValueError(f'Unsupported curves parameter: {",".join(n)}')
+        node_list = [[float(n[0]), float(n[1])] for n in node_list]
+
+        return {'x': node_list}
 
     @staticmethod
     def exposure(sep, val):
         defaults = {'val': 1.}
         parsed = parse_parameter_list(val, ['val'], [float])
         return defaults | parsed
```

### Comparing `educelab-imgproc-0.5.1/src/educelab/imgproc/properties.py` & `educelab_imgproc-0.6.dev1/src/educelab/imgproc/properties.py`

 * *Files identical despite different names*

### Comparing `educelab-imgproc-0.5.1/src/educelab/imgproc/roi.py` & `educelab_imgproc-0.6.dev1/src/educelab/imgproc/roi.py`

 * *Files identical despite different names*

### Comparing `educelab-imgproc-0.5.1/src/educelab_imgproc.egg-info/PKG-INFO` & `educelab_imgproc-0.6.dev1/src/educelab_imgproc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: educelab-imgproc
-Version: 0.5.1
+Version: 0.6.dev1
 Summary: EduceLab image processing module
 Home-page: https://educelab.gitlab.io/educelab-imgproc/
 Download-URL: https://gitlab.com/educelab/educelab-imgproc
 Author: Seth Parker
 Author-email: c.seth.parker@uky.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `educelab-imgproc-0.5.1/src/educelab_imgproc.egg-info/SOURCES.txt` & `educelab_imgproc-0.6.dev1/src/educelab_imgproc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

