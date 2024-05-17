# Comparing `tmp/dja_sepp-0.1.1.tar.gz` & `tmp/dja_sepp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dja_sepp-0.1.1.tar", last modified: Fri May 17 09:02:27 2024, max compression
+gzip compressed data, was "dja_sepp-0.1.2.tar", last modified: Fri May 17 09:24:42 2024, max compression
```

## Comparing `dja_sepp-0.1.1.tar` & `dja_sepp-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:02:27.922877 dja_sepp-0.1.1/
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     1071 2024-05-16 12:43:35.000000 dja_sepp-0.1.1/LICENSE
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2306 2024-05-17 09:02:27.920875 dja_sepp-0.1.1/PKG-INFO
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     1640 2024-05-16 12:32:24.000000 dja_sepp-0.1.1/README.md
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)      703 2024-05-17 09:02:12.000000 dja_sepp-0.1.1/pyproject.toml
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)       38 2024-05-17 09:02:27.923878 dja_sepp-0.1.1/setup.cfg
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:02:27.875066 dja_sepp-0.1.1/src/
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:02:27.909039 dja_sepp-0.1.1/src/dja_sepp/
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)      656 2024-05-17 08:37:29.000000 dja_sepp-0.1.1/src/dja_sepp/__init__.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     4778 2024-05-16 12:32:24.000000 dja_sepp-0.1.1/src/dja_sepp/psfex.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     3563 2024-05-17 08:10:03.000000 dja_sepp-0.1.1/src/dja_sepp/s3.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     9073 2024-05-17 08:36:10.000000 dja_sepp-0.1.1/src/dja_sepp/sepp.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    22764 2024-05-17 07:41:45.000000 dja_sepp-0.1.1/src/dja_sepp/sextractor.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     6936 2024-05-17 08:36:35.000000 dja_sepp-0.1.1/src/dja_sepp/tiles.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    13798 2024-05-17 09:00:08.000000 dja_sepp-0.1.1/src/dja_sepp/utils.py
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:02:27.919332 dja_sepp-0.1.1/src/dja_sepp.egg-info/
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2306 2024-05-17 09:02:27.000000 dja_sepp-0.1.1/src/dja_sepp.egg-info/PKG-INFO
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)      369 2024-05-17 09:02:27.000000 dja_sepp-0.1.1/src/dja_sepp.egg-info/SOURCES.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)        1 2024-05-17 09:02:27.000000 dja_sepp-0.1.1/src/dja_sepp.egg-info/dependency_links.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)       51 2024-05-17 09:02:27.000000 dja_sepp-0.1.1/src/dja_sepp.egg-info/requires.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)        9 2024-05-17 09:02:27.000000 dja_sepp-0.1.1/src/dja_sepp.egg-info/top_level.txt
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:24:42.315971 dja_sepp-0.1.2/
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     1071 2024-05-16 12:43:35.000000 dja_sepp-0.1.2/LICENSE
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2306 2024-05-17 09:24:42.309999 dja_sepp-0.1.2/PKG-INFO
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     1640 2024-05-16 12:32:24.000000 dja_sepp-0.1.2/README.md
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)      811 2024-05-17 09:24:29.000000 dja_sepp-0.1.2/pyproject.toml
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)       38 2024-05-17 09:24:42.316987 dja_sepp-0.1.2/setup.cfg
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:24:42.275113 dja_sepp-0.1.2/src/
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:24:42.295871 dja_sepp-0.1.2/src/dja_sepp/
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)      656 2024-05-17 08:37:29.000000 dja_sepp-0.1.2/src/dja_sepp/__init__.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     4778 2024-05-16 12:32:24.000000 dja_sepp-0.1.2/src/dja_sepp/psfex.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     3563 2024-05-17 08:10:03.000000 dja_sepp-0.1.2/src/dja_sepp/s3.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     9073 2024-05-17 08:36:10.000000 dja_sepp-0.1.2/src/dja_sepp/sepp.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    22764 2024-05-17 07:41:45.000000 dja_sepp-0.1.2/src/dja_sepp/sextractor.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     6936 2024-05-17 08:36:35.000000 dja_sepp-0.1.2/src/dja_sepp/tiles.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    14100 2024-05-17 09:21:37.000000 dja_sepp-0.1.2/src/dja_sepp/utils.py
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:24:42.306448 dja_sepp-0.1.2/src/dja_sepp.egg-info/
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2306 2024-05-17 09:24:42.000000 dja_sepp-0.1.2/src/dja_sepp.egg-info/PKG-INFO
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)      369 2024-05-17 09:24:42.000000 dja_sepp-0.1.2/src/dja_sepp.egg-info/SOURCES.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)        1 2024-05-17 09:24:42.000000 dja_sepp-0.1.2/src/dja_sepp.egg-info/dependency_links.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)       51 2024-05-17 09:24:42.000000 dja_sepp-0.1.2/src/dja_sepp.egg-info/requires.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)        9 2024-05-17 09:24:42.000000 dja_sepp-0.1.2/src/dja_sepp.egg-info/top_level.txt
```

### Comparing `dja_sepp-0.1.1/LICENSE` & `dja_sepp-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.1/PKG-INFO` & `dja_sepp-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dja_sepp
-Version: 0.1.1
+Version: 0.1.2
 Summary: Package to run SourceXtractor++ on the DAWN JWST Archive
 Author-email: Aurélien Genin <aurelien.genin@polytechnique.org>
 Project-URL: Source, https://github.com/AstroAure/DJA-SEpp
 Project-URL: DJA, https://dawn-cph.github.io/dja/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dja_sepp-0.1.1/README.md` & `dja_sepp-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.1/pyproject.toml` & `dja_sepp-0.1.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dja_sepp"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     {name="Aurélien Genin", email="aurelien.genin@polytechnique.org"}
 ]
 description = "Package to run SourceXtractor++ on the DAWN JWST Archive"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -23,8 +23,14 @@
     "matplotlib",
     "astropy",
     "scikit-learn"
 ]
 
 [project.urls]
 Source = "https://github.com/AstroAure/DJA-SEpp"
-DJA = "https://dawn-cph.github.io/dja/"
+DJA = "https://dawn-cph.github.io/dja/"
+
+[tool.setuptools.packages.find]
+where = ["src"]
+
+[tool.setuptools.package-data]
+mypkg = ["*.txt", "*.csv"]
```

### Comparing `dja_sepp-0.1.1/src/dja_sepp/__init__.py` & `dja_sepp-0.1.2/src/dja_sepp/__init__.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.1/src/dja_sepp/psfex.py` & `dja_sepp-0.1.2/src/dja_sepp/psfex.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.1/src/dja_sepp/s3.py` & `dja_sepp-0.1.2/src/dja_sepp/s3.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.1/src/dja_sepp/sepp.py` & `dja_sepp-0.1.2/src/dja_sepp/sepp.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.1/src/dja_sepp/sextractor.py` & `dja_sepp-0.1.2/src/dja_sepp/sextractor.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.1/src/dja_sepp/tiles.py` & `dja_sepp-0.1.2/src/dja_sepp/tiles.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.1/src/dja_sepp/utils.py` & `dja_sepp-0.1.2/src/dja_sepp/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import importlib.resources
 import os
 import glob
 from typing import Union
 import numpy as np
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.font_manager import FontProperties
@@ -211,14 +212,15 @@
 
     ax : matplotlib.pyplot.Axes to plot on
     filter_list : list of the filters to plot
     scale : maximum value of the plotted throughput curves
     names : whether to display the names of the filters
     throughput_folder : folder with the throughput data downloaded from the JWST documentation
     """
+    throughput_folder = importlib.resources.files('dja_sepp').joinpath(throughput_folder)
     filter_list = [filter.lower() for filter in color_dict.keys()] if filter_list is None else filter_list
     for filter in filter_list:
         table = ascii.read(f"{throughput_folder}/{filter.upper()}_mean_system_throughput.txt")
         color = color_dict[filter.upper()] if filter.upper() in color_dict else '#000000'
         max_val = scale if 'w' in filter else scale/2
         ax.plot(table['Microns'], max_val*table['Throughput']/table['Throughput'].max(), color=color)
         ax.fill_between(table['Microns'], max_val*table['Throughput']/table['Throughput'].max(), alpha=0.4, color=color)
@@ -256,8 +258,16 @@
                     fmt='o', ms=3, c='k', capsize=3, capthick=1)
     ax.set_xlabel("Wavelength (µm)")
     if mag:
         ax.set_ylabel("AB Mag")
     else:
         ax.set_ylabel(r"$F_{\nu}$ (nJy)")
     ax.set_title(title)
-    if custom_ax is None: plt.show()
+    if custom_ax is None: plt.show()
+
+def main():
+    fig, ax = plt.subplots(figsize=(12,5))
+    plot_filters(ax, ['f090w', 'f115w', 'f200w', 'f277w', 'f356w', 'f444w'])
+    plt.show()
+
+if __name__=="__main__":
+    main()
```

### Comparing `dja_sepp-0.1.1/src/dja_sepp.egg-info/PKG-INFO` & `dja_sepp-0.1.2/src/dja_sepp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dja_sepp
-Version: 0.1.1
+Version: 0.1.2
 Summary: Package to run SourceXtractor++ on the DAWN JWST Archive
 Author-email: Aurélien Genin <aurelien.genin@polytechnique.org>
 Project-URL: Source, https://github.com/AstroAure/DJA-SEpp
 Project-URL: DJA, https://dawn-cph.github.io/dja/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

