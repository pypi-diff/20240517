# Comparing `tmp/aplotly-1.1.8.tar.gz` & `tmp/aplotly-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aplotly-1.1.8.tar", last modified: Mon Feb 12 04:14:56 2024, max compression
+gzip compressed data, was "aplotly-1.1.9.tar", last modified: Mon Feb 12 06:26:40 2024, max compression
```

## Comparing `aplotly-1.1.8.tar` & `aplotly-1.1.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2024-02-12 04:14:56.464323 aplotly-1.1.8/
--rw-r--r--   0 samuel     (501) staff       (20)     1036 2023-11-27 03:51:33.000000 aplotly-1.1.8/LICENSE
--rw-r--r--   0 samuel     (501) staff       (20)       21 2023-11-27 07:06:14.000000 aplotly-1.1.8/MANIFEST.in
--rw-r--r--   0 samuel     (501) staff       (20)     2037 2024-02-12 04:14:56.464014 aplotly-1.1.8/PKG-INFO
--rw-r--r--   0 samuel     (501) staff       (20)      594 2023-11-27 07:04:41.000000 aplotly-1.1.8/README.md
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2024-02-12 04:14:56.454917 aplotly-1.1.8/aplotly/
--rw-r--r--   0 samuel     (501) staff       (20)      237 2023-12-01 03:52:59.000000 aplotly-1.1.8/aplotly/__init__.py
--rw-r--r--   0 samuel     (501) staff       (20)     4044 2023-12-01 03:52:22.000000 aplotly-1.1.8/aplotly/colors.py
--rw-r--r--   0 samuel     (501) staff       (20)     2715 2023-12-01 03:52:22.000000 aplotly-1.1.8/aplotly/io.py
--rw-r--r--   0 samuel     (501) staff       (20)    22214 2024-02-12 04:14:16.000000 aplotly-1.1.8/aplotly/plots.py
--rw-r--r--   0 samuel     (501) staff       (20)     2532 2024-02-12 04:00:44.000000 aplotly-1.1.8/aplotly/style.py
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2024-02-12 04:14:56.457337 aplotly-1.1.8/aplotly/utils/
--rw-r--r--   0 samuel     (501) staff       (20)     1393 2024-01-26 08:46:19.000000 aplotly-1.1.8/aplotly/utils/return_breakdown.py
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2024-02-12 04:14:56.463157 aplotly-1.1.8/aplotly.egg-info/
--rw-r--r--   0 samuel     (501) staff       (20)     2037 2024-02-12 04:14:56.000000 aplotly-1.1.8/aplotly.egg-info/PKG-INFO
--rw-r--r--   0 samuel     (501) staff       (20)      625 2024-02-12 04:14:56.000000 aplotly-1.1.8/aplotly.egg-info/SOURCES.txt
--rw-r--r--   0 samuel     (501) staff       (20)        1 2024-02-12 04:14:56.000000 aplotly-1.1.8/aplotly.egg-info/dependency_links.txt
--rw-r--r--   0 samuel     (501) staff       (20)       29 2024-02-12 04:14:56.000000 aplotly-1.1.8/aplotly.egg-info/requires.txt
--rw-r--r--   0 samuel     (501) staff       (20)        8 2024-02-12 04:14:56.000000 aplotly-1.1.8/aplotly.egg-info/top_level.txt
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2024-02-12 04:14:56.461101 aplotly-1.1.8/examples/
--rw-r--r--   0 samuel     (501) staff       (20)      303 2023-12-01 03:53:03.000000 aplotly-1.1.8/examples/plot_bars.py
--rw-r--r--   0 samuel     (501) staff       (20)      443 2023-12-01 03:53:03.000000 aplotly-1.1.8/examples/plot_exposure_tree.py
--rw-r--r--   0 samuel     (501) staff       (20)      201 2024-02-12 03:59:58.000000 aplotly-1.1.8/examples/plot_gauge.py
--rw-r--r--   0 samuel     (501) staff       (20)      651 2024-02-01 03:49:15.000000 aplotly-1.1.8/examples/plot_line.py
--rw-r--r--   0 samuel     (501) staff       (20)      278 2023-12-01 03:53:03.000000 aplotly-1.1.8/examples/plot_line_and_save.py
--rw-r--r--   0 samuel     (501) staff       (20)      348 2024-02-08 06:22:44.000000 aplotly-1.1.8/examples/plot_lines.py
--rw-r--r--   0 samuel     (501) staff       (20)      354 2023-12-01 03:53:03.000000 aplotly-1.1.8/examples/plot_multiple_performance.py
--rw-r--r--   0 samuel     (501) staff       (20)      310 2023-12-01 03:53:03.000000 aplotly-1.1.8/examples/plot_performance.py
--rw-r--r--   0 samuel     (501) staff       (20)      676 2024-01-05 08:50:50.000000 aplotly-1.1.8/examples/plot_returns_tree.py
--rw-r--r--   0 samuel     (501) staff       (20)      762 2024-02-12 04:14:50.000000 aplotly-1.1.8/pyproject.toml
--rw-r--r--   0 samuel     (501) staff       (20)       38 2024-02-12 04:14:56.464378 aplotly-1.1.8/setup.cfg
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2024-02-12 04:14:56.462955 aplotly-1.1.8/tests/
--rw-r--r--   0 samuel     (501) staff       (20)     1959 2023-12-01 03:53:06.000000 aplotly-1.1.8/tests/test_colors.py
--rw-r--r--   0 samuel     (501) staff       (20)     2149 2023-12-01 03:53:06.000000 aplotly-1.1.8/tests/test_io.py
--rw-r--r--   0 samuel     (501) staff       (20)     1940 2023-12-01 03:53:06.000000 aplotly-1.1.8/tests/test_style.py
+drwxr-xr-x   0 samuel     (501) staff       (20)        0 2024-02-12 06:26:40.553066 aplotly-1.1.9/
+-rw-r--r--   0 samuel     (501) staff       (20)     1036 2023-11-27 03:51:33.000000 aplotly-1.1.9/LICENSE
+-rw-r--r--   0 samuel     (501) staff       (20)       21 2023-11-27 07:06:14.000000 aplotly-1.1.9/MANIFEST.in
+-rw-r--r--   0 samuel     (501) staff       (20)     2037 2024-02-12 06:26:40.552870 aplotly-1.1.9/PKG-INFO
+-rw-r--r--   0 samuel     (501) staff       (20)      594 2023-11-27 07:04:41.000000 aplotly-1.1.9/README.md
+drwxr-xr-x   0 samuel     (501) staff       (20)        0 2024-02-12 06:26:40.548600 aplotly-1.1.9/aplotly/
+-rw-r--r--   0 samuel     (501) staff       (20)      237 2023-12-01 03:52:59.000000 aplotly-1.1.9/aplotly/__init__.py
+-rw-r--r--   0 samuel     (501) staff       (20)     4044 2023-12-01 03:52:22.000000 aplotly-1.1.9/aplotly/colors.py
+-rw-r--r--   0 samuel     (501) staff       (20)     2715 2023-12-01 03:52:22.000000 aplotly-1.1.9/aplotly/io.py
+-rw-r--r--   0 samuel     (501) staff       (20)    22488 2024-02-12 06:26:00.000000 aplotly-1.1.9/aplotly/plots.py
+-rw-r--r--   0 samuel     (501) staff       (20)     2532 2024-02-12 04:00:44.000000 aplotly-1.1.9/aplotly/style.py
+drwxr-xr-x   0 samuel     (501) staff       (20)        0 2024-02-12 06:26:40.549775 aplotly-1.1.9/aplotly/utils/
+-rw-r--r--   0 samuel     (501) staff       (20)     1393 2024-01-26 08:46:19.000000 aplotly-1.1.9/aplotly/utils/return_breakdown.py
+drwxr-xr-x   0 samuel     (501) staff       (20)        0 2024-02-12 06:26:40.552662 aplotly-1.1.9/aplotly.egg-info/
+-rw-r--r--   0 samuel     (501) staff       (20)     2037 2024-02-12 06:26:40.000000 aplotly-1.1.9/aplotly.egg-info/PKG-INFO
+-rw-r--r--   0 samuel     (501) staff       (20)      625 2024-02-12 06:26:40.000000 aplotly-1.1.9/aplotly.egg-info/SOURCES.txt
+-rw-r--r--   0 samuel     (501) staff       (20)        1 2024-02-12 06:26:40.000000 aplotly-1.1.9/aplotly.egg-info/dependency_links.txt
+-rw-r--r--   0 samuel     (501) staff       (20)       29 2024-02-12 06:26:40.000000 aplotly-1.1.9/aplotly.egg-info/requires.txt
+-rw-r--r--   0 samuel     (501) staff       (20)        8 2024-02-12 06:26:40.000000 aplotly-1.1.9/aplotly.egg-info/top_level.txt
+drwxr-xr-x   0 samuel     (501) staff       (20)        0 2024-02-12 06:26:40.551923 aplotly-1.1.9/examples/
+-rw-r--r--   0 samuel     (501) staff       (20)      303 2023-12-01 03:53:03.000000 aplotly-1.1.9/examples/plot_bars.py
+-rw-r--r--   0 samuel     (501) staff       (20)      443 2023-12-01 03:53:03.000000 aplotly-1.1.9/examples/plot_exposure_tree.py
+-rw-r--r--   0 samuel     (501) staff       (20)      224 2024-02-12 06:24:09.000000 aplotly-1.1.9/examples/plot_gauge.py
+-rw-r--r--   0 samuel     (501) staff       (20)      651 2024-02-01 03:49:15.000000 aplotly-1.1.9/examples/plot_line.py
+-rw-r--r--   0 samuel     (501) staff       (20)      278 2023-12-01 03:53:03.000000 aplotly-1.1.9/examples/plot_line_and_save.py
+-rw-r--r--   0 samuel     (501) staff       (20)      348 2024-02-08 06:22:44.000000 aplotly-1.1.9/examples/plot_lines.py
+-rw-r--r--   0 samuel     (501) staff       (20)      354 2023-12-01 03:53:03.000000 aplotly-1.1.9/examples/plot_multiple_performance.py
+-rw-r--r--   0 samuel     (501) staff       (20)      310 2023-12-01 03:53:03.000000 aplotly-1.1.9/examples/plot_performance.py
+-rw-r--r--   0 samuel     (501) staff       (20)      676 2024-01-05 08:50:50.000000 aplotly-1.1.9/examples/plot_returns_tree.py
+-rw-r--r--   0 samuel     (501) staff       (20)      762 2024-02-12 06:26:34.000000 aplotly-1.1.9/pyproject.toml
+-rw-r--r--   0 samuel     (501) staff       (20)       38 2024-02-12 06:26:40.553106 aplotly-1.1.9/setup.cfg
+drwxr-xr-x   0 samuel     (501) staff       (20)        0 2024-02-12 06:26:40.552479 aplotly-1.1.9/tests/
+-rw-r--r--   0 samuel     (501) staff       (20)     1959 2023-12-01 03:53:06.000000 aplotly-1.1.9/tests/test_colors.py
+-rw-r--r--   0 samuel     (501) staff       (20)     2149 2023-12-01 03:53:06.000000 aplotly-1.1.9/tests/test_io.py
+-rw-r--r--   0 samuel     (501) staff       (20)     1940 2023-12-01 03:53:06.000000 aplotly-1.1.9/tests/test_style.py
```

### Comparing `aplotly-1.1.8/LICENSE` & `aplotly-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aplotly-1.1.8/PKG-INFO` & `aplotly-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aplotly
-Version: 1.1.8
+Version: 1.1.9
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `aplotly-1.1.8/README.md` & `aplotly-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `aplotly-1.1.8/aplotly/colors.py` & `aplotly-1.1.9/aplotly/colors.py`

 * *Files identical despite different names*

### Comparing `aplotly-1.1.8/aplotly/io.py` & `aplotly-1.1.9/aplotly/io.py`

 * *Files identical despite different names*

### Comparing `aplotly-1.1.8/aplotly/plots.py` & `aplotly-1.1.9/aplotly/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -570,33 +570,40 @@
     fig.data[0].customdata = colors.values
     fig.data[0].texttemplate = "%{label}<br>%{customdata:.2%}"
 
     return fig
 
 
 def plot_gauge(
-    value, threshold: Union[float, None] = None, gauge_range=(0, 100), color_palette: str = "", plot_title: str = ""
+    value,
+    previous_value: Union[float, None] = None,
+    threshold: Union[float, None] = None,
+    gauge_range=(0, 100),
+    color_palette: str = "",
+    plot_title: str = "",
 ):
     """Plot a gauge chart.
 
     Args:
         value (float): value to show on the gauge.
+        previous_value (Union[float, None]): optional previous value to use for delta. Defaults to None.
         threshold (Union[float, None], optional): threshold value. Defaults to None.
         gauge_range (tuple, optional): range of the gauge. Defaults to (0, 100).
         color_palette (str, optional): name of the color palette to use. Defaults to "" (default color palette).
         plot_title (str, optional): title for the plot. Defaults to "" (no title).
 
     """
     _, chart_colors = configure_plotly(subplots=1, color_palette=color_palette)
     fig = go.Figure(
         go.Indicator(
-            mode="gauge+number",
+            mode="gauge+number+delta" if previous_value is not None else "gauge+number",
             value=value,
             domain={"x": [0, 1], "y": [0, 1]},
             title={"text": plot_title},
+            delta={"reference": previous_value},
             gauge={
                 "axis": {"range": gauge_range},
                 "threshold": {
                     "line": {"color": chart_colors["text"]},
                     "thickness": 0.75,
                     "value": threshold if threshold is not None else None,
                 },
```

### Comparing `aplotly-1.1.8/aplotly/style.py` & `aplotly-1.1.9/aplotly/style.py`

 * *Files identical despite different names*

### Comparing `aplotly-1.1.8/aplotly/utils/return_breakdown.py` & `aplotly-1.1.9/aplotly/utils/return_breakdown.py`

 * *Files identical despite different names*

### Comparing `aplotly-1.1.8/aplotly.egg-info/PKG-INFO` & `aplotly-1.1.9/aplotly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aplotly
-Version: 1.1.8
+Version: 1.1.9
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `aplotly-1.1.8/aplotly.egg-info/SOURCES.txt` & `aplotly-1.1.9/aplotly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aplotly-1.1.8/examples/plot_line.py` & `aplotly-1.1.9/examples/plot_line.py`

 * *Files identical despite different names*

### Comparing `aplotly-1.1.8/examples/plot_returns_tree.py` & `aplotly-1.1.9/examples/plot_returns_tree.py`

 * *Files identical despite different names*

### Comparing `aplotly-1.1.8/pyproject.toml` & `aplotly-1.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aplotly"
-version = "1.1.8"
+version = "1.1.9"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "plotly >= 5.18.0",
     "pandas >= 2.1.3"
 ]
 requires-python = ">=3.10.6"
 
 [tool.bumpver]
-current_version = "1.1.8"
+current_version = "1.1.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `aplotly-1.1.8/tests/test_colors.py` & `aplotly-1.1.9/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `aplotly-1.1.8/tests/test_io.py` & `aplotly-1.1.9/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `aplotly-1.1.8/tests/test_style.py` & `aplotly-1.1.9/tests/test_style.py`

 * *Files identical despite different names*

