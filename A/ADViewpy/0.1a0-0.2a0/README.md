# Comparing `tmp/ADViewpy-0.1a0.tar.gz` & `tmp/ADViewpy-0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ADViewpy-0.1a0.tar", last modified: Thu May 16 06:29:20 2024, max compression
+gzip compressed data, was "ADViewpy-0.2a0.tar", last modified: Fri May 17 07:38:10 2024, max compression
```

## Comparing `ADViewpy-0.1a0.tar` & `ADViewpy-0.2a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 06:29:20.483071 ADViewpy-0.1a0/
-drwxrwxrwx   0        0        0        0 2024-05-16 06:29:20.465951 ADViewpy-0.1a0/ADViewpy/
--rw-rw-rw-   0        0        0    44333 2024-05-06 09:06:33.000000 ADViewpy-0.1a0/ADViewpy/ADViewpy.py
--rw-rw-rw-   0        0        0      190 2024-05-04 05:39:18.000000 ADViewpy-0.1a0/ADViewpy/__init__.py
--rw-rw-rw-   0        0        0    18629 2024-05-06 05:26:44.000000 ADViewpy-0.1a0/ADViewpy/myCanvas.py
--rw-rw-rw-   0        0        0     3014 2024-05-06 02:28:03.000000 ADViewpy-0.1a0/ADViewpy/myUtils.py
--rw-rw-rw-   0        0        0    46111 2024-05-06 05:27:03.000000 ADViewpy-0.1a0/ADViewpy/pairwiseCanvas.py
--rw-rw-rw-   0        0        0    22890 2024-05-06 05:27:03.000000 ADViewpy-0.1a0/ADViewpy/rtCanvas.py
--rw-rw-rw-   0        0        0    64944 2024-05-06 05:27:03.000000 ADViewpy-0.1a0/ADViewpy/tcCanvas.py
--rw-rw-rw-   0        0        0    21925 2024-05-06 05:26:57.000000 ADViewpy-0.1a0/ADViewpy/treeDistributionView.py
-drwxrwxrwx   0        0        0        0 2024-05-16 06:29:20.480902 ADViewpy-0.1a0/ADViewpy.egg-info/
--rw-rw-rw-   0        0        0      995 2024-05-16 06:29:19.000000 ADViewpy-0.1a0/ADViewpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2024-05-16 06:29:20.000000 ADViewpy-0.1a0/ADViewpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 06:29:19.000000 ADViewpy-0.1a0/ADViewpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-05-16 06:29:19.000000 ADViewpy-0.1a0/ADViewpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-16 06:29:19.000000 ADViewpy-0.1a0/ADViewpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      995 2024-05-16 06:29:20.484084 ADViewpy-0.1a0/PKG-INFO
--rw-rw-rw-   0        0        0      507 2024-05-16 06:27:42.000000 ADViewpy-0.1a0/README.md
--rw-rw-rw-   0        0        0      539 2024-05-16 06:29:10.000000 ADViewpy-0.1a0/pyproject.toml
--rw-rw-rw-   0        0        0       94 2024-05-16 06:29:20.491316 ADViewpy-0.1a0/setup.cfg
--rw-rw-rw-   0        0        0     1321 2024-05-16 06:28:59.000000 ADViewpy-0.1a0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 07:38:10.086003 ADViewpy-0.2a0/
+drwxrwxrwx   0        0        0        0 2024-05-17 07:38:10.066999 ADViewpy-0.2a0/ADViewpy/
+-rw-rw-rw-   0        0        0    44333 2024-05-06 09:06:33.000000 ADViewpy-0.2a0/ADViewpy/ADViewpy.py
+-rw-rw-rw-   0        0        0      190 2024-05-04 05:39:18.000000 ADViewpy-0.2a0/ADViewpy/__init__.py
+-rw-rw-rw-   0        0        0    18629 2024-05-06 05:26:44.000000 ADViewpy-0.2a0/ADViewpy/myCanvas.py
+-rw-rw-rw-   0        0        0     3014 2024-05-06 02:28:03.000000 ADViewpy-0.2a0/ADViewpy/myUtils.py
+-rw-rw-rw-   0        0        0    46111 2024-05-06 05:27:03.000000 ADViewpy-0.2a0/ADViewpy/pairwiseCanvas.py
+-rw-rw-rw-   0        0        0    22890 2024-05-06 05:27:03.000000 ADViewpy-0.2a0/ADViewpy/rtCanvas.py
+-rw-rw-rw-   0        0        0    64944 2024-05-06 05:27:03.000000 ADViewpy-0.2a0/ADViewpy/tcCanvas.py
+-rw-rw-rw-   0        0        0    21925 2024-05-06 05:26:57.000000 ADViewpy-0.2a0/ADViewpy/treeDistributionView.py
+drwxrwxrwx   0        0        0        0 2024-05-17 07:38:10.083998 ADViewpy-0.2a0/ADViewpy.egg-info/
+-rw-rw-rw-   0        0        0     6202 2024-05-17 07:38:09.000000 ADViewpy-0.2a0/ADViewpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2024-05-17 07:38:09.000000 ADViewpy-0.2a0/ADViewpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 07:38:09.000000 ADViewpy-0.2a0/ADViewpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-05-17 07:38:09.000000 ADViewpy-0.2a0/ADViewpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-17 07:38:09.000000 ADViewpy-0.2a0/ADViewpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6202 2024-05-17 07:38:10.087002 ADViewpy-0.2a0/PKG-INFO
+-rw-rw-rw-   0        0        0     5716 2024-05-17 07:36:32.000000 ADViewpy-0.2a0/README.md
+-rw-rw-rw-   0        0        0      539 2024-05-17 07:37:43.000000 ADViewpy-0.2a0/pyproject.toml
+-rw-rw-rw-   0        0        0       94 2024-05-17 07:38:10.089000 ADViewpy-0.2a0/setup.cfg
+-rw-rw-rw-   0        0        0      904 2024-05-17 07:37:54.000000 ADViewpy-0.2a0/setup.py
```

### Comparing `ADViewpy-0.1a0/ADViewpy/ADViewpy.py` & `ADViewpy-0.2a0/ADViewpy/ADViewpy.py`

 * *Files identical despite different names*

### Comparing `ADViewpy-0.1a0/ADViewpy/myCanvas.py` & `ADViewpy-0.2a0/ADViewpy/myCanvas.py`

 * *Files identical despite different names*

### Comparing `ADViewpy-0.1a0/ADViewpy/myUtils.py` & `ADViewpy-0.2a0/ADViewpy/myUtils.py`

 * *Files identical despite different names*

### Comparing `ADViewpy-0.1a0/ADViewpy/pairwiseCanvas.py` & `ADViewpy-0.2a0/ADViewpy/pairwiseCanvas.py`

 * *Files identical despite different names*

### Comparing `ADViewpy-0.1a0/ADViewpy/rtCanvas.py` & `ADViewpy-0.2a0/ADViewpy/rtCanvas.py`

 * *Files identical despite different names*

### Comparing `ADViewpy-0.1a0/ADViewpy/tcCanvas.py` & `ADViewpy-0.2a0/ADViewpy/tcCanvas.py`

 * *Files identical despite different names*

### Comparing `ADViewpy-0.1a0/ADViewpy/treeDistributionView.py` & `ADViewpy-0.2a0/ADViewpy/treeDistributionView.py`

 * *Files identical despite different names*

### Comparing `ADViewpy-0.1a0/pyproject.toml` & `ADViewpy-0.2a0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 00000010: 3d20 2241 4456 6965 7770 7922 0d0a 7665  = "ADViewpy"..ve
-00000020: 7273 696f 6e20 3d20 2730 2e31 2e61 6c70  rsion = '0.1.alp
+00000020: 7273 696f 6e20 3d20 2730 2e32 2e61 6c70  rsion = '0.2.alp
 00000030: 6861 270d 0a64 6573 6372 6970 7469 6f6e  ha'..description
 00000040: 203d 2022 4144 5669 6577 7079 2069 7320   = "ADViewpy is 
 00000050: 5079 7468 6f6e 204c 6962 7261 7279 2074  Python Library t
 00000060: 6f20 7669 7375 616c 6c79 2063 6f6d 7061  o visually compa
 00000070: 7265 2070 6879 6c6f 6765 6e65 7469 6320  re phylogenetic 
 00000080: 7472 6565 7322 0d0a 7265 6164 6d65 203d  trees"..readme =
 00000090: 2022 5245 4144 4d45 2e6d 6422 0d0a 6465   "README.md"..de
```

### Comparing `ADViewpy-0.1a0/setup.py` & `ADViewpy-0.2a0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,22 @@
 import codecs
 import os
 from setuptools import setup, find_packages
 
-# here = os.path.abspath(os.path.dirname(__file__))
-#
-# with codecs.open(("./README.md"), encoding="utf-8") as f:
-#     long_description = "\n" + f.read()
-
-here = os.path.abspath(os.path.dirname(__file__))
-with open(os.path.join(here, "README.md"),"r" ,encoding='utf-8') as f:
-    long_description = f.read()
-
-VERSION = '0.1.alpha'
+VERSION = '0.2.alpha'
 DESCRIPTION = ('ADViewpy is Python Library to visually compare phylogenetic trees')
 LONG_DESCRIPTION = 'ADViewpy is Python Library to visually compare phylogenetic trees, utilizing Aggregated Dendrogram for phylogenetic tree visualization. '
 
 
-
 setup(
     name="ADViewpy",
     version=VERSION,
     author="Ng Weng Shan",
     author_email="ngwengshan025@hotmail.com",
     description=DESCRIPTION,
-    # long_description_content_type="text/markdown",
-    # long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[
         'dendropy',
         'ipycanvas',
         'ipywidgets',
         'scikit-learn',
         'numpy',
```

