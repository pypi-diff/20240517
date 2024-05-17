# Comparing `tmp/czitools-0.6.0.tar.gz` & `tmp/czitools-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "czitools-0.6.0.tar", last modified: Sun Feb 11 12:24:48 2024, max compression
+gzip compressed data, was "czitools-0.7.0.tar", last modified: Fri May 17 06:28:05 2024, max compression
```

## Comparing `czitools-0.6.0.tar` & `czitools-0.7.0.tar`

### file list

```diff
@@ -1,24 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 12:24:48.138135 czitools-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-11 12:24:36.000000 czitools-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-11 12:24:36.000000 czitools-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-02-11 12:24:48.138135 czitools-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-02-11 12:24:36.000000 czitools-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-11 12:24:37.000000 czitools-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-02-11 12:24:48.138135 czitools-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-11 12:24:37.000000 czitools-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 12:24:48.134135 czitools-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 12:24:48.134135 czitools-0.6.0/src/czitools/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-11 12:24:37.000000 czitools-0.6.0/src/czitools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-02-11 12:24:37.000000 czitools-0.6.0/src/czitools/datatreewiget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-02-11 12:24:37.000000 czitools-0.6.0/src/czitools/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    52562 2024-02-11 12:24:37.000000 czitools-0.6.0/src/czitools/metadata_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    20989 2024-02-11 12:24:37.000000 czitools-0.6.0/src/czitools/misc_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    12334 2024-02-11 12:24:37.000000 czitools-0.6.0/src/czitools/napari_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    22486 2024-02-11 12:24:37.000000 czitools-0.6.0/src/czitools/read_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-02-11 12:24:37.000000 czitools-0.6.0/src/czitools/write_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 12:24:48.134135 czitools-0.6.0/src/czitools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-02-11 12:24:48.000000 czitools-0.6.0/src/czitools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-02-11 12:24:48.000000 czitools-0.6.0/src/czitools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-11 12:24:48.000000 czitools-0.6.0/src/czitools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-02-11 12:24:48.000000 czitools-0.6.0/src/czitools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-11 12:24:48.000000 czitools-0.6.0/src/czitools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:28:05.579579 czitools-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-17 06:28:00.000000 czitools-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-17 06:28:00.000000 czitools-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8614 2024-05-17 06:28:05.579579 czitools-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-05-17 06:28:00.000000 czitools-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-17 06:28:01.000000 czitools-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-17 06:28:05.579579 czitools-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-17 06:28:01.000000 czitools-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:28:05.571579 czitools-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:28:05.575579 czitools-0.7.0/src/czitools/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:28:05.575579 czitools-0.7.0/src/czitools/metadata_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/metadata_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/metadata_tools/add_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/metadata_tools/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/metadata_tools/boundingbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/metadata_tools/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24621 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/metadata_tools/czi_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/metadata_tools/detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/metadata_tools/dimension.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/metadata_tools/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/metadata_tools/microscope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/metadata_tools/objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/metadata_tools/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/metadata_tools/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/metadata_tools/scene.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:28:05.579579 czitools-0.7.0/src/czitools/napari_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/napari_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12742 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/napari_tools/napari_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:28:05.579579 czitools-0.7.0/src/czitools/read_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/read_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22107 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/read_tools/read_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:28:05.579579 czitools-0.7.0/src/czitools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/utils/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/utils/datatreewiget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20275 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:28:05.579579 czitools-0.7.0/src/czitools/visu_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/visu_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/visu_tools/vis_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:28:05.579579 czitools-0.7.0/src/czitools/write_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/write_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-17 06:28:01.000000 czitools-0.7.0/src/czitools/write_tools/write_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:28:05.579579 czitools-0.7.0/src/czitools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8614 2024-05-17 06:28:05.000000 czitools-0.7.0/src/czitools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-17 06:28:05.000000 czitools-0.7.0/src/czitools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 06:28:05.000000 czitools-0.7.0/src/czitools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-17 06:28:05.000000 czitools-0.7.0/src/czitools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 06:28:05.000000 czitools-0.7.0/src/czitools.egg-info/top_level.txt
```

### Comparing `czitools-0.6.0/LICENSE` & `czitools-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `czitools-0.6.0/PKG-INFO` & `czitools-0.7.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: czitools
-Version: 0.6.0
+Version: 0.7.0
 Summary: Tools to simplify reading CZI (Carl Zeiss Image) meta and pixel data
 Home-page: https://github.com/sebi06/czitools
 Author: Sebastian Rhode
 Author-email: sebrhode@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Bug Tracker, https://github.com/sebi06/czitools/issues
 Project-URL: Documentation, https://github.com/sebi06/czitools/#README.md
@@ -21,93 +21,117 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: xmltodict
-Requires-Dist: aicsimageio[all]>=4.11.0
-Requires-Dist: aicspylibczi
-Requires-Dist: fsspec>=2022.8.0
-Requires-Dist: tqdm
 Requires-Dist: pylibCZIrw>=4.1.0
-Requires-Dist: napari
+Requires-Dist: aicspylibczi>=3.1.2
+Requires-Dist: tqdm
 Requires-Dist: pandas
-Requires-Dist: seaborn
-Requires-Dist: plotly
-Requires-Dist: matplotlib
-Requires-Dist: colormap
+Requires-Dist: ome-zarr
 Requires-Dist: zarr
 Requires-Dist: dask
 Requires-Dist: python-dateutil
 Requires-Dist: python-box[all]
-Requires-Dist: scikit-image>=0.19.3
 Requires-Dist: czifile
-Requires-Dist: pyqtgraph
+Provides-Extra: all
+Requires-Dist: napari[all]; extra == "all"
+Requires-Dist: seaborn; extra == "all"
+Requires-Dist: plotly; extra == "all"
+Requires-Dist: pyqtgraph; extra == "all"
+Requires-Dist: colormap; extra == "all"
 
 # czitools
 
 [![PyPI](https://img.shields.io/pypi/v/czitools.svg?color=green)](https://pypi.org/project/czitools)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/czitools)](https://pypistats.org/packages/czitools)
 [![License](https://img.shields.io/pypi/l/czitools.svg?color=green)](https://github.com/sebi06/czitools/raw/master/LICENSE)
 [![Python Version](https://img.shields.io/pypi/pyversions/czitools.svg?color=green)](https://python.org)
 [![Development Status](https://img.shields.io/pypi/status/czitools.svg)](https://en.wikipedia.org/wiki/Software_release_life_cycle#Alpha)
 
 This repository provides a collection of tools to simplify reading CZI (Carl Zeiss Image) pixel and metadata in Python. In addition it also contains other useful utilities to visualize CZI images inside Napari (needs to be installed). It is also available as a [Python Package on PyPi](https://pypi.org/project/czitools/)
 
+## Installation
+
+To install the basic functionality (will not install Napari und plotting functionality) use:
+
+```text
+pip install czitools"
+```
+
+To install the package with all optional dependencies use:
+
+```text
+pip install czitools[all]
+```
+
 ## Reading the metadata
 
 Please check [use_metadata_tools.py](https://github.com/sebi06/czitools/blob/main/demo/scripts/use_metadata_tools.py) for some examples.
 
 ```python
-# get the metadata at once as one big class
-mdata = czimd.CziMetadata(filepath)
+from czitools.metadata_tools.czi_metadata import CziMetadata, writexml
+from czitools.metadata_tools.dimension import CziDimensions
+from czitools.metadata_tools.boundingbox import CziBoundingBox
+from czitools.metadata_tools.channel import CziChannelInfo
+from czitools.metadata_tools.scaling import CziScaling
+from czitools.metadata_tools.sample import CziSampleInfo
+from czitools.metadata_tools.objective import CziObjectives
+from czitools.metadata_tools.microscope import CziMicroscope
+from czitools.metadata_tools.add_metadata import CziAddMetaData
+from czitools.metadata_tools.detector import CziDetector
+from czitools.read_tools import read_tools
+from czitools.napari_tools import napari_tools
+import napari
 
-# get only specific metadata
-czi_dimensions = czimd.CziDimensions(filepath)
+# get the metadata_tools at once as one big class
+mdata = CziMetadata(filepath)
+
+# get only specific metadata_tools
+czi_dimensions = CziDimensions(filepath)
 print("SizeS: ", czi_dimensions.SizeS)
 print("SizeT: ", czi_dimensions.SizeT)
 print("SizeZ: ", czi_dimensions.SizeZ)
 print("SizeC: ", czi_dimensions.SizeC)
 print("SizeY: ", czi_dimensions.SizeY)
 print("SizeX: ", czi_dimensions.SizeX)
 
 # try to write XML to file
-xmlfile = czimd.writexml(filepath)
+xmlfile = writexml(filepath)
 
 # get info about the channels
-czi_channels = czimd.CziChannelInfo(filepath)
+czi_channels = CziChannelInfo(filepath)
 
-# get the complete metadata from the CZI as one big object
-czimd_complete = czimd.get_metadata_as_object(filepath)
+# get the complete metadata_tools from the CZI as one big object
+czimd_complete = get_metadata_as_object(filepath)
 
 # get an object containing only the dimension information
-czi_dimensions = czimd.CziDimensions(filepath)
+czi_dimensions = CziDimensions(filepath)
 
 # get an object containing only the dimension information
-czi_scale = czimd.CziScaling(filepath)
+czi_scale = CziScaling(filepath)
 
 # get an object containing information about the sample
-czi_sample = czimd.CziSampleInfo(filepath)
+czi_sample = CziSampleInfo(filepath)
 
 # get info about the objective, the microscope and the detectors
-czi_objectives = czimd.CziObjectives(filepath)
-czi_detectors = czimd.CziDetector(filepath)
-czi_microscope = czimd.CziMicroscope(filepath)
+czi_objectives = CziObjectives(filepath)
+czi_detectors = CziDetector(filepath)
+czi_microscope = CziMicroscope(filepath)
 
 # get info about the sample carrier
-czi_sample = czimd.CziSampleInfo(filepath)
+czi_sample = CziSampleInfo(filepath)
 
 # get additional metainformation
-czi_addmd = czimd.CziAddMetaData(filepath)
+czi_addmd = CziAddMetaData(filepath)
 
 # get the complete data about the bounding boxes
-czi_bbox = czimd.CziBoundingBox(filepath)
+czi_bbox = CziBoundingBox(filepath)
 ```
 
 ## Reading CZI pixel data
 
 While the [pylibCZIrw](https://pypi.org/project/pylibCZIrw/) is focussing on reading individual planes it is also helpful to read CZI pixel data as a STCZYX(A) stack. Please check [use_read_tools.py](https://github.com/sebi06/czitools/blob/main/demo/scripts/use_read_tools.py) for some examples.
 
 ```python
@@ -171,7 +195,21 @@
 
 The basic usage can be inferred from this sample notebook:&nbsp;
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sebi06/czitools/blob/main/demo/notebooks/read_czi_segment_voroni_otsu.ipynb)
 
 ## Remarks
 
 The code to read multi-dimensional with delayed reading using Dask array was heavily inspired by input from: [Pradeep Rajasekhar](https://github.com/pr4deepr).
+
+Local installation (base functionality only):
+
+```text
+pip install -e .
+```
+
+### Local Installation
+
+Local installation (full functionality):
+
+```text
+pip install -e ".[all]"
+```
```

### Comparing `czitools-0.6.0/README.md` & `czitools-0.7.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -4,62 +4,90 @@
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/czitools)](https://pypistats.org/packages/czitools)
 [![License](https://img.shields.io/pypi/l/czitools.svg?color=green)](https://github.com/sebi06/czitools/raw/master/LICENSE)
 [![Python Version](https://img.shields.io/pypi/pyversions/czitools.svg?color=green)](https://python.org)
 [![Development Status](https://img.shields.io/pypi/status/czitools.svg)](https://en.wikipedia.org/wiki/Software_release_life_cycle#Alpha)
 
 This repository provides a collection of tools to simplify reading CZI (Carl Zeiss Image) pixel and metadata in Python. In addition it also contains other useful utilities to visualize CZI images inside Napari (needs to be installed). It is also available as a [Python Package on PyPi](https://pypi.org/project/czitools/)
 
+## Installation
+
+To install the basic functionality (will not install Napari und plotting functionality) use:
+
+```text
+pip install czitools"
+```
+
+To install the package with all optional dependencies use:
+
+```text
+pip install czitools[all]
+```
+
 ## Reading the metadata
 
 Please check [use_metadata_tools.py](https://github.com/sebi06/czitools/blob/main/demo/scripts/use_metadata_tools.py) for some examples.
 
 ```python
-# get the metadata at once as one big class
-mdata = czimd.CziMetadata(filepath)
+from czitools.metadata_tools.czi_metadata import CziMetadata, writexml
+from czitools.metadata_tools.dimension import CziDimensions
+from czitools.metadata_tools.boundingbox import CziBoundingBox
+from czitools.metadata_tools.channel import CziChannelInfo
+from czitools.metadata_tools.scaling import CziScaling
+from czitools.metadata_tools.sample import CziSampleInfo
+from czitools.metadata_tools.objective import CziObjectives
+from czitools.metadata_tools.microscope import CziMicroscope
+from czitools.metadata_tools.add_metadata import CziAddMetaData
+from czitools.metadata_tools.detector import CziDetector
+from czitools.read_tools import read_tools
+from czitools.napari_tools import napari_tools
+import napari
+
+# get the metadata_tools at once as one big class
+mdata = CziMetadata(filepath)
 
-# get only specific metadata
-czi_dimensions = czimd.CziDimensions(filepath)
+# get only specific metadata_tools
+czi_dimensions = CziDimensions(filepath)
 print("SizeS: ", czi_dimensions.SizeS)
 print("SizeT: ", czi_dimensions.SizeT)
 print("SizeZ: ", czi_dimensions.SizeZ)
 print("SizeC: ", czi_dimensions.SizeC)
 print("SizeY: ", czi_dimensions.SizeY)
 print("SizeX: ", czi_dimensions.SizeX)
 
 # try to write XML to file
-xmlfile = czimd.writexml(filepath)
+xmlfile = writexml(filepath)
 
 # get info about the channels
-czi_channels = czimd.CziChannelInfo(filepath)
+czi_channels = CziChannelInfo(filepath)
 
-# get the complete metadata from the CZI as one big object
-czimd_complete = czimd.get_metadata_as_object(filepath)
+# get the complete metadata_tools from the CZI as one big object
+czimd_complete = get_metadata_as_object(filepath)
 
 # get an object containing only the dimension information
-czi_dimensions = czimd.CziDimensions(filepath)
+czi_dimensions = CziDimensions(filepath)
 
 # get an object containing only the dimension information
-czi_scale = czimd.CziScaling(filepath)
+czi_scale = CziScaling(filepath)
 
 # get an object containing information about the sample
-czi_sample = czimd.CziSampleInfo(filepath)
+czi_sample = CziSampleInfo(filepath)
 
 # get info about the objective, the microscope and the detectors
-czi_objectives = czimd.CziObjectives(filepath)
-czi_detectors = czimd.CziDetector(filepath)
-czi_microscope = czimd.CziMicroscope(filepath)
+czi_objectives = CziObjectives(filepath)
+czi_detectors = CziDetector(filepath)
+czi_microscope = CziMicroscope(filepath)
 
 # get info about the sample carrier
-czi_sample = czimd.CziSampleInfo(filepath)
+czi_sample = CziSampleInfo(filepath)
 
 # get additional metainformation
-czi_addmd = czimd.CziAddMetaData(filepath)
+czi_addmd = CziAddMetaData(filepath)
 
 # get the complete data about the bounding boxes
-czi_bbox = czimd.CziBoundingBox(filepath)
+czi_bbox = CziBoundingBox(filepath)
 ```
 
 ## Reading CZI pixel data
 
 While the [pylibCZIrw](https://pypi.org/project/pylibCZIrw/) is focussing on reading individual planes it is also helpful to read CZI pixel data as a STCZYX(A) stack. Please check [use_read_tools.py](https://github.com/sebi06/czitools/blob/main/demo/scripts/use_read_tools.py) for some examples.
 
 ```python
@@ -123,7 +151,21 @@
 
 The basic usage can be inferred from this sample notebook:&nbsp;
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sebi06/czitools/blob/main/demo/notebooks/read_czi_segment_voroni_otsu.ipynb)
 
 ## Remarks
 
 The code to read multi-dimensional with delayed reading using Dask array was heavily inspired by input from: [Pradeep Rajasekhar](https://github.com/pr4deepr).
+
+Local installation (base functionality only):
+
+```text
+pip install -e .
+```
+
+### Local Installation
+
+Local installation (full functionality):
+
+```text
+pip install -e ".[all]"
+```
```

### Comparing `czitools-0.6.0/setup.cfg` & `czitools-0.7.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = czitools
-version = 0.6.0
+version = 0.7.0
 author = Sebastian Rhode
 author_email = sebrhode@gmail.com
 url = https://github.com/sebi06/czitools
 license = GNU General Public License v3 (GPLv3)
 description = Tools to simplify reading CZI (Carl Zeiss Image) meta and pixel data
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -29,34 +29,32 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.9
 install_requires = 
-	numpy
-	xmltodict
-	aicsimageio[all]>=4.11.0
-	aicspylibczi
-	fsspec>=2022.8.0
-	tqdm
 	pylibCZIrw>=4.1.0
-	napari
+	aicspylibczi>=3.1.2
+	tqdm
 	pandas
-	seaborn
-	plotly
-	matplotlib
-	colormap
+	ome-zarr
 	zarr
 	dask
 	python-dateutil
 	python-box[all]
-	scikit-image>=0.19.3
 	czifile
+
+[options.extras_require]
+all = 
+	napari[all] # will install PyQt5
+	seaborn
+	plotly
 	pyqtgraph
+	colormap
 
 [options.packages.find]
 where = src
 exclude = 
 	data*
 	docs*
 	demo*
```

### Comparing `czitools-0.6.0/src/czitools/datatreewiget.py` & `czitools-0.7.0/src/czitools/utils/datatreewiget.py`

 * *Files identical despite different names*

### Comparing `czitools-0.6.0/src/czitools/logger.py` & `czitools-0.7.0/src/czitools/utils/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 def get_logger(log_to_file: bool = False):
     """
     Creates a custom logger with two handlers:
     - stdout_handler: logging to console (logs all five levels)
     - file_handler: logging to a file (logs all five levels) if `log_to_file` is True
 
     Args:
-        log_to_file (bool): Whether or not to log to file. Defaults to False.
+        log_to_file (bool): Whether to log to file. Defaults to False.
 
     Returns:
         logging.Logger: A custom logger with two handlers.
     """
 
     # Create custom logger logging all five levels
     logger = logging.getLogger(__name__)
```

### Comparing `czitools-0.6.0/src/czitools/misc_tools.py` & `czitools-0.7.0/src/czitools/utils/misc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 #################################################################
-# File        : misc_tools.py
+# File        : misc.py
 # Author      : sebi06
 #
 # Disclaimer: The code is purely experimental. Feel free to
 # use it at your own risk.
 #
 #################################################################
 
@@ -15,24 +15,22 @@
 import zarr
 import pandas as pd
 import dask.array as da
 import numpy as np
 import time
 from pathlib import Path
 import dateutil.parser as dt
-from itertools import product
-from czitools import metadata_tools as czimd
-from typing import List, Dict, Tuple, Optional, Type, Any, Union, Mapping
-from dataclasses import make_dataclass, fields, dataclass
-from czitools import logger as LOGGER
+from tqdm.contrib.itertools import product
+from typing import Dict, Tuple, Any, Union
 import validators
-import re
-#from urllib.parse import urlparse
+from aicspylibczi import CziFile
+from czitools.utils import logger
 
-logger = LOGGER.get_logger()
+
+logger = logger.get_logger()
 
 
 def openfile(
     directory: Union[str, os.PathLike[str]],
     title: str = "Open CZI Image File",
     ftypename: str = "CZI Files",
     extension: str = "*.czi",
@@ -141,23 +139,23 @@
 
     return minvalue, maxvalue
 
 
 def md2dataframe(
     md_dict: Dict, paramcol: str = "Parameter", keycol: str = "Value"
 ) -> pd.DataFrame:
-    """Converts the given metadata dictionary to a Pandas DataFrame.
+    """Converts the given metadata_tools dictionary to a Pandas DataFrame.
 
     Args:
-        md_dict (dict): A dictionary containing metadata.
-        paramcol (str, optional): The name of the column for metadata parameters. Defaults to "Parameter".
-        keycol (str, optional): The name of the column for metadata values. Defaults to "Value".
+        md_dict (dict): A dictionary containing metadata_tools.
+        paramcol (str, optional): The name of the column for metadata_tools parameters. Defaults to "Parameter".
+        keycol (str, optional): The name of the column for metadata_tools values. Defaults to "Value".
 
     Returns:
-        pd.DataFrame: A Pandas DataFrame containing all the metadata.
+        pd.DataFrame: A Pandas DataFrame containing all the metadata_tools.
     """
     mdframe = pd.DataFrame(columns=[paramcol, keycol])
 
     for k in md_dict.keys():
         d = {"Parameter": k, "Value": md_dict[k]}
         df = pd.DataFrame([d], index=[0])
         mdframe = pd.concat([mdframe, df], ignore_index=True)
@@ -249,232 +247,257 @@
     if mdata_entry is not None:
         return mdata_entry
 
 
 def get_planetable(
     czifile: Union[str, os.PathLike[str]],
     norm_time: bool = True,
-    savetable: bool = False,
-    separator: str = ",",
-    read_one_only: bool = False,
-    index: bool = True,
-) -> Tuple[pd.DataFrame, Optional[str]]:
+    pt_complete: bool = True,
+    t: int = 0,
+    c: int = 0,
+    z: int = 0,
+) -> pd.DataFrame:
     """Get the planetable from the individual subblocks
     Args:
         czifile: the source for the CZI image file
         norm_time: normalize the timestamps
-        savetable: option save the planetable as CSV file
-        separator: specify the separator for the CSV file
-        read_one_only: option to read only the first entry
-        index: option to save CSV file with an index
-
-    Returns:
-        Planetable as pd.DataFrame or np.recarray and the location of the CSV file
-    """
-
-    try:
-        from aicspylibczi import CziFile
-
-        if isinstance(czifile, Path):
-            # convert to string
-            czifile = str(czifile)
-
-        if validators.url(czifile):
-            logger.warning("Reading PlaneTable from CZI via a link is not supported.")
-
-        # get the czi metadata
-        czi_dimensions = czimd.CziDimensions(czifile)
-        aicsczi = CziFile(czifile)
-
-        # initialize the plane table
-        df_czi = pd.DataFrame(
-            columns=[
-                "Subblock",
-                "Scene",
-                "Tile",
-                "T",
-                "Z",
-                "C",
-                "X[micron]",
-                "Y[micron]",
-                "Z[micron]",
-                "Time[s]",
-                "xstart",
-                "ystart",
-                "width",
-                "height",
-            ]
-        )
-
-        # define subblock counter
-        sbcount = -1
-
-        # check if dimensions are None (because they do not exist for that image)
-        size_c = check_dimsize(czi_dimensions.SizeC, set2value=1)
-        size_z = check_dimsize(czi_dimensions.SizeZ, set2value=1)
-        size_t = check_dimsize(czi_dimensions.SizeT, set2value=1)
-        size_s = check_dimsize(czi_dimensions.SizeS, set2value=1)
-        size_m = check_dimsize(czi_dimensions.SizeM, set2value=1)
-
-        def getsbinfo(subblock: Any) -> Tuple[float, float, float, float]:
-            try:
-                time = subblock.findall(".//AcquisitionTime")[0].text
-                timestamp = dt.parse(time).timestamp()
-            except IndexError as e:
-                timestamp = 0.0
-
-            try:
-                xpos = np.double(subblock.findall(".//StageXPosition")[0].text)
-            except IndexError as e:
-                xpos = 0.0
-
-            try:
-                ypos = np.double(subblock.findall(".//StageYPosition")[0].text)
-            except IndexError as e:
-                ypos = 0.0
-
-            try:
-                zpos = np.double(subblock.findall(".//FocusPosition")[0].text)
-            except IndexError as e:
-                zpos = 0.0
-
-            return timestamp, xpos, ypos, zpos
-
-        # do if the data is not a mosaic
-        if size_m > 1:
-            for s, m, t, z, c in product(
-                range(size_s),
-                range(size_m),
-                range(size_t),
-                range(size_z),
-                range(size_c),
-            ):
-                sbcount += 1
-
-                # get x, y, width and height for a specific tile
-                tilebbox = aicsczi.get_mosaic_tile_bounding_box(S=s, M=m, T=t, Z=z, C=c)
-
-                # read information from subblock
-                sb = aicsczi.read_subblock_metadata(
-                    unified_xml=True, B=0, S=s, M=m, T=t, Z=z, C=c
-                )
-
-                # get information from subblock
-                timestamp, xpos, ypos, zpos = getsbinfo(sb)
-
-                plane = pd.DataFrame(
-                    {
-                        "Subblock": sbcount,
-                        "Scene": s,
-                        "Tile": m,
-                        "T": t,
-                        "Z": z,
-                        "C": c,
-                        "X[micron]": xpos,
-                        "Y[micron]": ypos,
-                        "Z[micron]": zpos,
-                        "Time[s]": timestamp,
-                        "xstart": tilebbox.x,
-                        "ystart": tilebbox.y,
-                        "width": tilebbox.w,
-                        "height": tilebbox.h,
-                    },
-                    index=[0],
-                )
-
-                # df_czi = pd.concat([df_czi, plane], ignore_index=True)
-
-                df_czi = pd.concat([df_czi if not df_czi.empty else None, plane])
-
-                if read_one_only:
-                    break
-
-        # do if the data is not a mosaic
-        if size_m == 1:
-            for s, t, z, c in product(
-                range(size_s), range(size_t), range(size_z), range(size_c)
-            ):
-                sbcount += 1
-
-                # get x, y, width and height for a specific tile
-                tilebbox = aicsczi.get_tile_bounding_box(S=s, T=t, Z=z, C=c)
-
-                # read information from subblocks
-                sb = aicsczi.read_subblock_metadata(
-                    unified_xml=True, B=0, S=s, T=t, Z=z, C=c
-                )
-
-                # get information from subblock
-                timestamp, xpos, ypos, zpos = getsbinfo(sb)
-
-                plane = pd.DataFrame(
-                    {
-                        "Subblock": sbcount,
-                        "Scene": s,
-                        "Tile": 0,
-                        "T": t,
-                        "Z": z,
-                        "C": c,
-                        "X[micron]": xpos,
-                        "Y[micron]": ypos,
-                        "Z[micron]": zpos,
-                        "Time[s]": timestamp,
-                        "xstart": tilebbox.x,
-                        "ystart": tilebbox.y,
-                        "width": tilebbox.w,
-                        "height": tilebbox.h,
-                    },
-                    index=[0],
-                )
-
-                # df_czi = pd.concat([df_czi, plane], ignore_index=True)
-
-                df_czi = pd.concat([df_czi if not df_czi.empty else None, plane])
-
-                if read_one_only:
-                    break
-
-        # cast data  types
-        df_czi = df_czi.astype(
-            {
-                "Subblock": "int32",
-                "Scene": "int32",
-                "Tile": "int32",
-                "T": "int32",
-                "Z": "int32",
-                "C": "int16",
-                "X[micron]": "float",
-                "Y[micron]": "float",
-                "Z[micron]": "float",
-                "xstart": "int32",
-                "ystart": "int32",
-                "width": "int32",
-                "height": "int32",
-            },
-            copy=False,
-            errors="ignore",
-        )
-
-        # normalize time stamps
-        if norm_time:
-            df_czi = norm_columns(df_czi, colname="Time[s]", mode="min")
-
-        # save planetable as CSV file
-        if savetable:
-            csvfile = save_planetable(df_czi, czifile, separator=separator, index=index)
-            logger.info(f"PlaneTable saved as CSV file: {csvfile}")
-        if not savetable:
-            csvfile = None
-
-    except ImportError as e:
-        # print("Package aicspylibczi not found. Use Fallback values.")
-        logger.warning("Package aicspylibczi not found. Cannot extract planetable.")
+        pt_complete: Read data from all subblocks or only use the ones to be shown in the plot
+
+    Returns:
+        Planetable as pd.DataFrame
+    """
+
+    if isinstance(czifile, Path):
+        # convert to string
+        czifile = str(czifile)
+
+    if validators.url(czifile):
+        logger.warning("Reading PlaneTable from CZI via a link is not supported.")
         return None, None
 
-    return df_czi, csvfile
+    # initialize the plane table
+    df_czi = pd.DataFrame(
+        columns=[
+            "Subblock",
+            "Scene",
+            "Tile",
+            "T",
+            "Z",
+            "C",
+            "X[micron]",
+            "Y[micron]",
+            "Z[micron]",
+            "Time[s]",
+            "xstart",
+            "ystart",
+            "width",
+            "height",
+        ]
+    )
+
+    # define subblock counter
+    sbcount = -1
+
+    aicsczi = CziFile(czifile)
+    dims = aicsczi.get_dims_shape()
+
+    if "S" in dims[0].keys():
+        size_s = dims[0]["S"][1]
+    else:
+        size_s = 1
+
+    if "M" in dims[0].keys():
+        size_m = dims[0]["M"][1]
+    else:
+        size_m = 1
+
+    if "T" in dims[0].keys():
+        size_t = dims[0]["T"][1]
+    else:
+        size_t = 1
+
+    if "C" in dims[0].keys():
+        size_c = dims[0]["C"][1]
+    else:
+        size_c = 1
+
+    if "Z" in dims[0].keys():
+        size_z = dims[0]["Z"][1]
+    else:
+        size_z = 1
+
+    def getsbinfo(subblock: Any) -> Tuple[float, float, float, float]:
+        try:
+            time = subblock.findall(".//AcquisitionTime")[0].text
+            timestamp = dt.parse(time).timestamp()
+        except IndexError as e:
+            timestamp = 0.0
+
+        try:
+            xpos = np.double(subblock.findall(".//StageXPosition")[0].text)
+        except IndexError as e:
+            xpos = 0.0
+
+        try:
+            ypos = np.double(subblock.findall(".//StageYPosition")[0].text)
+        except IndexError as e:
+            ypos = 0.0
+
+        try:
+            zpos = np.double(subblock.findall(".//FocusPosition")[0].text)
+        except IndexError as e:
+            zpos = 0.0
+
+        return timestamp, xpos, ypos, zpos
+
+    if pt_complete:
+        t_start = 0
+        t_end = size_t
+        c_start = 0
+        c_end = size_c
+        z_start = 0
+        z_end = size_z
+
+    elif not pt_complete:
+        t_start = t
+        t_end = t + 1
+        c_start = c
+        c_end = c + 1
+        z_start = 0
+        z_end = z + 1
+
+    # do if the data is not a mosaic
+    if size_m > 1:
+        # for s, m, t, z, c in product(
+        #    range(size_s),
+        #    range(size_m),
+        #    range(size_t),
+        #    range(size_z),
+        #    range(size_c),
+        # ):
+        for s, m, t, c, z in product(
+            range(size_s),
+            range(size_m),
+            enumerate(range(t_start, t_end)),
+            enumerate(range(c_start, c_end)),
+            enumerate(range(z_start, z_end)),
+            desc="Reading sublocks planes",
+            unit=" 2Dplanes",
+        ):
+            sbcount += 1
+
+            # get x, y, width and height for a specific tile
+            tilebbox = aicsczi.get_mosaic_tile_bounding_box(
+                S=s, M=m, T=t[1], Z=z[1], C=c[1]
+            )
+
+            # read information from subblock
+            sb = aicsczi.read_subblock_metadata(
+                unified_xml=True, B=0, S=s, M=m, T=t[1], Z=z[1], C=c[1]
+            )
+
+            # get information from subblock
+            timestamp, xpos, ypos, zpos = getsbinfo(sb)
+
+            plane = pd.DataFrame(
+                {
+                    "Subblock": sbcount,
+                    "Scene": s,
+                    "Tile": m,
+                    "T": t[1],
+                    "Z": z[1],
+                    "C": c[1],
+                    "X[micron]": xpos,
+                    "Y[micron]": ypos,
+                    "Z[micron]": zpos,
+                    "Time[s]": timestamp,
+                    "xstart": tilebbox.x,
+                    "ystart": tilebbox.y,
+                    "width": tilebbox.w,
+                    "height": tilebbox.h,
+                },
+                index=[0],
+            )
+
+            df_czi = pd.concat([df_czi if not df_czi.empty else None, plane])
+
+    # do if the data is not a mosaic
+    if size_m == 1:
+        # for s, t, z, c in product(
+        #    range(size_s), range(size_t), range(size_z), range(size_c)
+        # ):
+        for s, t, c, z in product(
+            range(size_s),
+            enumerate(range(t_start, t_end)),
+            enumerate(range(c_start, c_end)),
+            enumerate(range(z_start, z_end)),
+            desc="Reading sublocks planes",
+            unit=" 2Dplanes",
+        ):
+            sbcount += 1
+
+            # get x, y, width and height for a specific tile
+            tilebbox = aicsczi.get_tile_bounding_box(S=s, T=t[1], Z=z[1], C=c[1])
+
+            # read information from subblocks
+            sb = aicsczi.read_subblock_metadata(
+                unified_xml=True, B=0, S=s, T=t[1], Z=z[1], C=c[1]
+            )
+
+            # get information from subblock
+            timestamp, xpos, ypos, zpos = getsbinfo(sb)
+
+            plane = pd.DataFrame(
+                {
+                    "Subblock": sbcount,
+                    "Scene": s,
+                    "Tile": 0,
+                    "T": t[1],
+                    "Z": z[1],
+                    "C": c[1],
+                    "X[micron]": xpos,
+                    "Y[micron]": ypos,
+                    "Z[micron]": zpos,
+                    "Time[s]": timestamp,
+                    "xstart": tilebbox.x,
+                    "ystart": tilebbox.y,
+                    "width": tilebbox.w,
+                    "height": tilebbox.h,
+                },
+                index=[0],
+            )
+
+            df_czi = pd.concat([df_czi if not df_czi.empty else None, plane])
+
+    # cast data  types
+    df_czi = df_czi.astype(
+        {
+            "Subblock": "int32",
+            "Scene": "int32",
+            "Tile": "int32",
+            "T": "int32",
+            "Z": "int32",
+            "C": "int16",
+            "X[micron]": "float",
+            "Y[micron]": "float",
+            "Z[micron]": "float",
+            "xstart": "int32",
+            "ystart": "int32",
+            "width": "int32",
+            "height": "int32",
+        },
+        copy=False,
+        errors="ignore",
+    )
+
+    # normalize time stamps
+    if norm_time:
+        df_czi = norm_columns(df_czi, colname="Time[s]", mode="min")
+
+    return df_czi
 
 
 def norm_columns(
     df: pd.DataFrame, colname: str = "Time [s]", mode: str = "min"
 ) -> pd.DataFrame:
     """Normalize a specific column inside a Pandas dataframe
     Args:
@@ -655,25 +678,17 @@
     if not validators.url(source_link):
         logger.warning("Not a valid link.")
         return ""
 
     import io
     import zipfile
 
-    compressed_data = os .path.join(os.getcwd(), os.path.basename(source_link))
+    compressed_data = os.path.join(os.getcwd(), os.path.basename(source_link))
 
     if not os.path.isfile(compressed_data):
         response = requests.get(GITHUB_IMAGES_PATH, stream=True)
         compressed_data = io.BytesIO(response.content)
 
-    with zipfile.ZipFile(compressed_data, 'r') as zip_accessor:
-        zip_accessor.extractall('./')
+    with zipfile.ZipFile(compressed_data, "r") as zip_accessor:
+        zip_accessor.extractall("./")
 
     return compressed_data[:-4]
-
-
-
-    
-
-    
-
-
```

### Comparing `czitools-0.6.0/src/czitools/napari_tools.py` & `czitools-0.7.0/src/czitools/napari_tools/napari_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,55 +5,59 @@
 # Author      : sebi06
 #
 # Disclaimer: This code is purely experimental. Feel free to
 # use it at your own risk.
 #
 #################################################################
 
-import napari
-
-from PyQt5.QtWidgets import (
-    QVBoxLayout,
-    QWidget,
-    QTableWidget,
-    QTableWidgetItem,
-)
-
-from PyQt5.QtCore import Qt
-from PyQt5 import QtWidgets
-from PyQt5.QtGui import QFont
-from czitools import metadata_tools as czimd
-from czitools import misc_tools
-from czitools.datatreewiget import DataTreeWidget
-import numpy as np
-from typing import (
-    List,
-    Dict,
-    Tuple,
-    Optional,
-    Type,
-    Any,
-    Union,
-    Literal,
-    Mapping,
-    Annotated,
-)
-from napari.utils.colormaps import Colormap
-from napari.utils import resize_dask_cache
-import dask.array as da
-from dataclasses import dataclass
-from czitools import logger as LOGGER
-
-logger = LOGGER.get_logger()
-
-
-@dataclass
-class ValueRange:
-    lo: float
-    hi: float
+import sys
+from czitools.utils import logger
+from czitools.metadata_tools.helper import ValueRange
+
+logger = logger.get_logger()
+
+# check if Napari is actually installed
+try:
+    import napari
+except (ImportError, ModuleNotFoundError) as error:
+    # Output expected ImportErrors.
+    logger.error(error.__class__.__name__ + ": " + error.msg)
+    sys.exit(1)
+else:
+
+    from PyQt5.QtWidgets import (
+        QVBoxLayout,
+        QWidget,
+        QTableWidget,
+        QTableWidgetItem,
+    )
+
+    from PyQt5.QtCore import Qt
+    from PyQt5 import QtWidgets
+    from PyQt5.QtGui import QFont
+    from czitools.metadata_tools import czi_metadata as czimd
+    from czitools.utils import misc
+    from czitools.utils.datatreewiget import DataTreeWidget
+    import numpy as np
+    from typing import (
+        List,
+        Dict,
+        Tuple,
+        Optional,
+        Type,
+        Any,
+        Union,
+        Literal,
+        Mapping,
+        Annotated,
+    )
+    from napari.utils.colormaps import Colormap
+    from napari.utils import resize_dask_cache
+    import dask.array as da
+    from dataclasses import dataclass
 
 
 class MdTableWidget(QWidget):
     def __init__(self) -> None:
         super(QWidget, self).__init__()
 
         self.layout = QVBoxLayout(self)
@@ -61,29 +65,29 @@
         self.layout.addWidget(self.mdtable)
         self.mdtable.setShowGrid(True)
         self.mdtable.setHorizontalHeaderLabels(["Parameter", "Value"])
         header = self.mdtable.horizontalHeader()
         header.setDefaultAlignment(Qt.AlignLeft)
 
     def update_metadata(self, md_dict: Dict) -> None:
-        """Update the table with the metadata from the dictionary
+        """Update the table with the metadata_tools from the dictionary
 
         Args:
             md_dict (Dict): Metadata dictionary
         """
 
-        # number of rows is set to number of metadata entries
+        # number of rows is set to number of metadata_tools entries
         row_count = len(md_dict)
         col_count = 2
         self.mdtable.setColumnCount(col_count)
         self.mdtable.setRowCount(row_count)
 
         row = 0
 
-        # update the table with the entries from metadata dictionary
+        # update the table with the entries from metadata_tools dictionary
         for key, value in md_dict.items():
             newkey = QTableWidgetItem(key)
             self.mdtable.setItem(row, 0, newkey)
             newvalue = QTableWidgetItem(str(value))
             self.mdtable.setItem(row, 1, newvalue)
             row += 1
 
@@ -133,29 +137,29 @@
     contrast: Literal["calc", "napari_auto", "from_czi"] = "calc",
     gamma: float = 0.85,
     show_metadata: Literal["none", "tree", "table"] = "tree",
     name_sliders: bool = False,
     dask_cache_size: Annotated[float, ValueRange(0.5, 0.9)] = 0.5,
 ) -> List:
     """Display the multidimensional array inside the Napari viewer.
-    Optionally the CziMetadata class will be used show a table with the metadata.
+    Optionally the CziMetadata class will be used show a table with the metadata_tools.
     Every channel will be added as a new layer to the viewer.
 
     Args:
         viewer (Any): Napari viewer object
         array (Union[np.ndarray, List[da.Array], da.Array]): multi-dimensional array containing the pixel data (Numpy, List of Dask Array or Dask array.
         metadata (czimd.CziMetadata): CziMetadata class
         dim_string (str): dimension string for the array to be shown
         blending (str, optional): blending mode for viewer. Defaults to "additive".
         contrast (Literal[str], optional): method to be used to calculate an appropriate display scaling.
             - "calc" : real min & max calculation (might be slow) be calculated (slow)
             - "napari_auto" : Let Napari figure out a display scaling. Will look in the center of an image!
-            - "from_czi" : use the display scaling from ZEN stored inside the CZI metadata. Defaults to "calc".
+            - "from_czi" : use the display scaling from ZEN stored inside the CZI metadata_tools. Defaults to "calc".
         gamma (float, optional): gamma value for the Viewer for all layers Defaults to 0.85.
-        show_metadata (mdviewoption, optional): Option to show metadata as tree or table. Defaults to "tree".
+        show_metadata (mdviewoption, optional): Option to show metadata_tools as tree or table. Defaults to "tree".
         name_sliders (bool, optional): option to use the dimension letters as slider labels for the viewer. Defaults to False.
         dask_cache_size(float, optional): option to resize the dask cache used for opportunistic caching. Range [0 - 1]
 
     Returns:
         List: List of napari layers
     """
 
@@ -172,32 +176,32 @@
     # create empty list for the napari layers
     napari_layers = []
 
     # create scale factor with all ones
     scalefactors = [1.0] * len(array.shape)
 
     # testing
-    #scalefactors = [1.0] * 6
+    # scalefactors = [1.0] * 6
 
     # modify the tuple for the scales for napari
 
     # the "strange factor" is added due to an open (rounding) bug on the Napari side:
     # https://github.com/napari/napari/issues/4861
     # https://forum.image.sc/t/image-layer-in-napari-showing-the-wrong-dimension-size-one-plane-is-missing/69939/12
 
     scalefactors[dim_order["Z"]] = metadata.scale.ratio["zx_sf"] * 1.001
 
     if show_metadata.lower != "none":
-        # add PyQTGraph DataTreeWidget to Napari viewer to show the metadata
+        # add PyQTGraph DataTreeWidget to Napari viewer to show the metadata_tools
         if show_metadata == "tree":
             md_dict = czimd.create_md_dict_nested(metadata, sort=True, remove_none=True)
             mdtree = MdTreeWidget(data=md_dict, expandlevel=1)
             viewer.window.add_dock_widget(mdtree, name="MetadataTree", area="right")
 
-        # add QTableWidget DataTreeWidget to Napari viewer to show the metadata
+        # add QTableWidget DataTreeWidget to Napari viewer to show the metadata_tools
         if show_metadata == "table":
             md_dict = czimd.create_md_dict_red(metadata, sort=True, remove_none=True)
             mdtable = MdTableWidget()
             mdtable.update_metadata(md_dict)
             mdtable.update_style()
             viewer.window.add_dock_widget(mdtable, name="MetadataTable", area="right")
 
@@ -208,37 +212,37 @@
         size_c = metadata.image.SizeC
 
     # loop over all channels and add them as layers
     for ch in range(size_c):
         try:
             # get the channel name
             chname = metadata.channelinfo.names[ch]
-            # inside the CZI metadata colors are defined as ARGB hexstring
+            # inside the CZI metadata_tools colors are defined as ARGB hexstring
             rgb = "#" + metadata.channelinfo.colors[ch][3:]
             ncmap = Colormap(["#000000", rgb], name="cm_" + chname)
         except (KeyError, IndexError) as e:
             logger.warning(e)
             # or use CH1 etc. as string for the name
             chname = "CH" + str(ch + 1)
             ncmap = Colormap(["#000000", "#ffffff"], name="cm_" + chname)
 
         # cut out channel
         if metadata.image.SizeC is not None:
-            channel = misc_tools.slicedim(array, ch, dim_order["C"])
+            channel = misc.slicedim(array, ch, dim_order["C"])
         if metadata.image.SizeC is None:
             channel = array
 
         # actually show the image array
         logger.info(f"Adding Channel: {chname}")
         logger.info(f"Shape Channel: {ch} , {channel.shape}")
         logger.info(f"Scaling Factors: {scalefactors}")
 
         if contrast == "calc":
             # really calculate the min and max values - might be slow
-            sc = misc_tools.calc_scaling(channel, corr_min=1.1, corr_max=0.9)
+            sc = misc.calc_scaling(channel, corr_min=1.1, corr_max=0.9)
             logger.info(f"Calculated Display Scaling (min & max): {sc}")
 
             # add channel to napari viewer
             new_layer = viewer.add_image(
                 channel,
                 name=chname,
                 scale=scalefactors,
@@ -313,15 +317,15 @@
     #     od[dim_order["C"]], od[dim_order["Z"]] = od[dim_order["Z"]], od[dim_order["C"]]
     #     viewer.dims.order = tuple(od)
 
     return napari_layers
 
 
 def rename_sliders(sliders: Tuple, dim_order: Dict) -> Tuple:
-    """Rename the sliders inside the Napari viewer based on the metadata
+    """Rename the sliders inside the Napari viewer based on the metadata_tools
 
 
     Args:
         sliders (Tuple): labels of sliders from viewer
         dim_order (Dict): dictionary indication the dimension string and its position inside the array
 
     Returns:
```

### Comparing `czitools-0.6.0/src/czitools/read_tools.py` & `czitools-0.7.0/src/czitools/read_tools/read_tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,70 +6,39 @@
 #
 # Disclaimer: This code is purely experimental. Feel free to
 # use it at your own risk.
 #
 #################################################################
 
 from typing import (
-    List,
     Dict,
     Tuple,
     Optional,
-    Type,
-    Any,
     Union,
-    Mapping,
-    Literal,
-    Annotated,
-)
-from typing import (
-    List,
-    Dict,
-    Tuple,
-    Optional,
-    Type,
-    Any,
-    Union,
-    Mapping,
-    Literal,
     Annotated,
 )
 from pylibCZIrw import czi as pyczi
-from czitools import metadata_tools as czimd
-from czitools import misc_tools
-from dataclasses import dataclass, field, fields, Field
+from czitools.metadata_tools import czi_metadata as czimd
+from czitools.utils import misc
 import numpy as np
 from pathlib import Path
-import dask
 import dask.array as da
 import dask.delayed
 import os
 from tqdm import tqdm
 from tqdm.contrib.itertools import product
 import tempfile
 import shutil
-from czitools import logger as LOGGER
-from enum import Enum
-from dataclasses import dataclass
+from czitools.utils import logger
+from czitools.metadata_tools.helper import ValueRange
+from czitools.metadata_tools.helper import AttachmentType
 
 # from memory_profiler import profile
 
-logger = LOGGER.get_logger()
-
-
-class AttachmentType(Enum):
-    SlidePreview = 1
-    Label = 2
-    Prescan = 3
-
-
-@dataclass
-class ValueRange:
-    lo: float
-    hi: float
+logger = logger.get_logger()
 
 
 # code for which memory has to be monitored
 # instantiating the decorator
 # @profile
 def read_6darray(
     filepath: Union[str, os.PathLike[str]],
@@ -89,15 +58,15 @@
         zoom (float, optional): Downscale images using a factor [0.01 - 1.0]. Defaults to 1.0
         planes (dict, optional): Allowed keys S, T, Z, C and their start and end values must be >=0 (zero-based).
                                  planes = {"Z":(0, 2)} will return 3 z-plane with indices (0, 1, 2).
                                  Respectively {"Z":(5, 5)} will return a single z-plane with index 5.
         zoom (float, options): Downsample CZI image by a factor [0.01 - 1.0]. Defaults to 1.0.
 
     Returns:
-        Tuple[array6d, mdata]: output as 6D dask array and metadata
+        Tuple[array6d, mdata]: output as 6D dask array and metadata_tools
     """
 
     if isinstance(filepath, Path):
         # convert to string
         filepath = str(filepath)
 
     # check zoom factor
@@ -108,15 +77,15 @@
         zoom = 1.0
     if zoom < 0.01:
         logger.warning(
             f"Zoom factor f{zoom} is not in valid range [0.01 - 1.0]. Using 0.01 instead."
         )
         zoom = 0.01
 
-    # get the complete metadata at once as one big class
+    # get the complete metadata_tools at once as one big class
     mdata = czimd.CziMetadata(filepath)
 
     if not mdata.consistent_pixeltypes:
         logger.info("Detected PixelTypes ar not consistent. Cannot create array6d")
         return None, mdata
 
     # check zoomlevels
@@ -164,18 +133,18 @@
 
         # if mdata.image.SizeS is None:
         #     # use the size of the total_bounding_rectangle
         #     size_x = czidoc.total_bounding_rectangle.w
         #     size_y = czidoc.total_bounding_rectangle.h
 
         # check if dimensions are None (because they do not exist for that image)
-        size_c = misc_tools.check_dimsize(mdata.image.SizeC, set2value=1)
-        size_z = misc_tools.check_dimsize(mdata.image.SizeZ, set2value=1)
-        size_t = misc_tools.check_dimsize(mdata.image.SizeT, set2value=1)
-        size_s = misc_tools.check_dimsize(mdata.image.SizeS, set2value=1)
+        size_c = misc.check_dimsize(mdata.image.SizeC, set2value=1)
+        size_z = misc.check_dimsize(mdata.image.SizeZ, set2value=1)
+        size_t = misc.check_dimsize(mdata.image.SizeT, set2value=1)
+        size_s = misc.check_dimsize(mdata.image.SizeS, set2value=1)
 
         s_start = 0
         s_end = size_s
         t_start = 0
         t_end = size_t
         c_start = 0
         c_end = size_c
@@ -274,15 +243,15 @@
                 array6d = array6d.rechunk(chunks=(1, 1, 1, size_z, image2d.shape[0], image2d.shape[1]))
 
         if not remove_adim:
             if use_dask and chunk_zyx:
                 # for testing
                 array6d = array6d.rechunk(chunks=(1, 1, 1, size_z, image2d.shape[0], image2d.shape[1], 3))
 
-    # update metadata
+    # update metadata_tools
     mdata.array6d_size = array6d.shape
 
     return array6d, mdata
 
 
 # code for which memory has to be monitored
 # instantiating the decorator
@@ -300,37 +269,37 @@
         filepath (str | Path): filepath for the CZI image
         chunk_zyx (bool, optional): Option to chunk dask array along z-stacks. Defaults to False.
         planes (dict, optional): Allowed keys S, T, Z, C and their start and end values must be >=0 (zero-based).
                                  planes = {"Z":(0, 2)} will return 3 z-plane with indices (0, 1, 2).
                                  Respectively {"Z":(5, 5)} will return a single z-plane with index 5.
 
     Returns:
-        Tuple[array6d, mdata]: output as 6D dask array and metadata
+        Tuple[array6d, mdata]: output as 6D dask array and metadata_tools
     """
 
     if isinstance(filepath, Path):
         # convert to string
         filepath = str(filepath)
 
-    # get the complete metadata at once as one big class
+    # get the complete metadata_tools at once as one big class
     mdata = czimd.CziMetadata(filepath)
 
     if not mdata.consistent_pixeltypes:
         logger.info("Detected PixelTypes ar not consistent. Cannot create array6d")
-        return None, mdata, ""
+        return None, mdata
 
     # check planes
     if not planes is False:
         for k in ["S", "T", "C", "Z"]:
             if k in planes.keys() and k in mdata.bbox.total_bounding_box.keys():
                 if mdata.bbox.total_bounding_box[k][1] - 1 < planes[k][1]:
                     logger.info(
                         f"Planes indices (zero-based) for {planes[k]} are invalid. BBox for {[k]}: {mdata.bbox.total_bounding_box[k]}"
                     )
-                    return None, mdata, ""
+                    return None, mdata
 
     if not mdata.scene_shape_is_consistent and not "S" in planes.keys():
         logger.info("Scenes have inconsistent shape. Cannot read 6D array")
         return None, mdata
 
     # open the CZI document to read the
     with pyczi.open_czi(filepath, mdata.pyczi_readertype) as czidoc:
@@ -344,18 +313,18 @@
 
         if mdata.image.SizeS is None:
             # use the size of the total_bounding_rectangle
             size_x = czidoc.total_bounding_rectangle.w
             size_y = czidoc.total_bounding_rectangle.h
 
         # check if dimensions are None (because they do not exist for that image)
-        size_c = misc_tools.check_dimsize(mdata.image.SizeC, set2value=1)
-        size_z = misc_tools.check_dimsize(mdata.image.SizeZ, set2value=1)
-        size_t = misc_tools.check_dimsize(mdata.image.SizeT, set2value=1)
-        size_s = misc_tools.check_dimsize(mdata.image.SizeS, set2value=1)
+        size_c = misc.check_dimsize(mdata.image.SizeC, set2value=1)
+        size_z = misc.check_dimsize(mdata.image.SizeZ, set2value=1)
+        size_t = misc.check_dimsize(mdata.image.SizeT, set2value=1)
+        size_s = misc.check_dimsize(mdata.image.SizeS, set2value=1)
 
         s_start = 0
         s_end = size_s
         t_start = 0
         t_end = size_t
         c_start = 0
         c_end = size_c
@@ -484,15 +453,15 @@
                 array6d = array6d.rechunk(chunks=(1, 1, 1, size_z, size_y, size_x))
 
         if not remove_adim:
             if chunk_zyx:
                 # for testing
                 array6d = array6d.rechunk(chunks=(1, 1, 1, size_z, size_y, size_x, 3))
 
-    return array6d, mdata  # , dim_string
+    return array6d, mdata
 
 
 @dask.delayed
 def read_2dplane(
     czidoc: pyczi.CziReader,
     s: int = 0,
     t: int = 0,
```

### Comparing `czitools-0.6.0/src/czitools/write_tools.py` & `czitools-0.7.0/src/czitools/write_tools/write_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,21 +12,22 @@
 # the ome_zarr imports we require
 from pathlib import Path
 import dask.array as da
 import zarr
 import ome_zarr.reader
 import ome_zarr.scale
 import ome_zarr.writer
+import ome_zarr.format
 from ome_zarr.io import parse_url
-from typing import List, Dict, Tuple, Optional, Type, Any, Union, Mapping
+from typing import Union
 import shutil
 import numpy as np
-from czitools import logger as LOGGER
+from czitools.utils import logger
 
-logger = LOGGER.get_logger()
+logger = logger.get_logger()
 
 
 def write_omezarr(
     array5d: Union[np.ndarray, da.Array],
     zarr_path: str,
     axes: str = "tczyx",
     overwrite: bool = False,
@@ -34,23 +35,23 @@
     """
     Simple function to write OME-ZARR from an 5D numpy yor dask array
 
     Args:
         array5d (Union[np.ndarary, da.Array]): Up-to 5 dimensional array to be written as OME-ZARR
         zarr_path (str): Path for the OME-ZARR folder to be created
         axes (str): Defines the dimension order (lower case string). Defaults to "STCZYX"
-        overwrite (False): If True, than an existing folder will be overwritten.Defaults to False
+        overwrite (False): If True, then an existing folder will be overwritten. Defaults to False
 
     Returns:
         str: Path for location of OME-ZARR folder
     """
 
     # check number of dimension of input array
     if len(array5d.shape) > 5:
-        LOGGER.warning("Input array as more than 5 dimensions.")
+        logger.warning("Input array as more than 5 dimensions.")
         return None
 
     # make sure lower case is use for axes order
     axes = axes.lower()
 
     # check for invalid dimensions and clean up
     for character in ["b", "h", "s", "i", "v", "a"]:
@@ -67,15 +68,15 @@
     # write the image data
     store = parse_url(zarr_path, mode="w").store
     root = zarr.group(store=store)
     # root.info
 
     # TODO: Add Channel information etc. to the root along those lines
     """
-    # add omero metadata: the napari ome-zarr plugin uses this to pass rendering
+    # add omero metadata_tools: the napari ome-zarr plugin uses this to pass rendering
     # options to napari.
     root.attrs['omero'] = {
         'channels': [{
                 'color': 'ffffff',
                 'label': 'LS-data',
                 'active': True,
                 }]
```

### Comparing `czitools-0.6.0/src/czitools.egg-info/PKG-INFO` & `czitools-0.7.0/src/czitools.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: czitools
-Version: 0.6.0
+Version: 0.7.0
 Summary: Tools to simplify reading CZI (Carl Zeiss Image) meta and pixel data
 Home-page: https://github.com/sebi06/czitools
 Author: Sebastian Rhode
 Author-email: sebrhode@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Bug Tracker, https://github.com/sebi06/czitools/issues
 Project-URL: Documentation, https://github.com/sebi06/czitools/#README.md
@@ -21,93 +21,117 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: xmltodict
-Requires-Dist: aicsimageio[all]>=4.11.0
-Requires-Dist: aicspylibczi
-Requires-Dist: fsspec>=2022.8.0
-Requires-Dist: tqdm
 Requires-Dist: pylibCZIrw>=4.1.0
-Requires-Dist: napari
+Requires-Dist: aicspylibczi>=3.1.2
+Requires-Dist: tqdm
 Requires-Dist: pandas
-Requires-Dist: seaborn
-Requires-Dist: plotly
-Requires-Dist: matplotlib
-Requires-Dist: colormap
+Requires-Dist: ome-zarr
 Requires-Dist: zarr
 Requires-Dist: dask
 Requires-Dist: python-dateutil
 Requires-Dist: python-box[all]
-Requires-Dist: scikit-image>=0.19.3
 Requires-Dist: czifile
-Requires-Dist: pyqtgraph
+Provides-Extra: all
+Requires-Dist: napari[all]; extra == "all"
+Requires-Dist: seaborn; extra == "all"
+Requires-Dist: plotly; extra == "all"
+Requires-Dist: pyqtgraph; extra == "all"
+Requires-Dist: colormap; extra == "all"
 
 # czitools
 
 [![PyPI](https://img.shields.io/pypi/v/czitools.svg?color=green)](https://pypi.org/project/czitools)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/czitools)](https://pypistats.org/packages/czitools)
 [![License](https://img.shields.io/pypi/l/czitools.svg?color=green)](https://github.com/sebi06/czitools/raw/master/LICENSE)
 [![Python Version](https://img.shields.io/pypi/pyversions/czitools.svg?color=green)](https://python.org)
 [![Development Status](https://img.shields.io/pypi/status/czitools.svg)](https://en.wikipedia.org/wiki/Software_release_life_cycle#Alpha)
 
 This repository provides a collection of tools to simplify reading CZI (Carl Zeiss Image) pixel and metadata in Python. In addition it also contains other useful utilities to visualize CZI images inside Napari (needs to be installed). It is also available as a [Python Package on PyPi](https://pypi.org/project/czitools/)
 
+## Installation
+
+To install the basic functionality (will not install Napari und plotting functionality) use:
+
+```text
+pip install czitools"
+```
+
+To install the package with all optional dependencies use:
+
+```text
+pip install czitools[all]
+```
+
 ## Reading the metadata
 
 Please check [use_metadata_tools.py](https://github.com/sebi06/czitools/blob/main/demo/scripts/use_metadata_tools.py) for some examples.
 
 ```python
-# get the metadata at once as one big class
-mdata = czimd.CziMetadata(filepath)
+from czitools.metadata_tools.czi_metadata import CziMetadata, writexml
+from czitools.metadata_tools.dimension import CziDimensions
+from czitools.metadata_tools.boundingbox import CziBoundingBox
+from czitools.metadata_tools.channel import CziChannelInfo
+from czitools.metadata_tools.scaling import CziScaling
+from czitools.metadata_tools.sample import CziSampleInfo
+from czitools.metadata_tools.objective import CziObjectives
+from czitools.metadata_tools.microscope import CziMicroscope
+from czitools.metadata_tools.add_metadata import CziAddMetaData
+from czitools.metadata_tools.detector import CziDetector
+from czitools.read_tools import read_tools
+from czitools.napari_tools import napari_tools
+import napari
 
-# get only specific metadata
-czi_dimensions = czimd.CziDimensions(filepath)
+# get the metadata_tools at once as one big class
+mdata = CziMetadata(filepath)
+
+# get only specific metadata_tools
+czi_dimensions = CziDimensions(filepath)
 print("SizeS: ", czi_dimensions.SizeS)
 print("SizeT: ", czi_dimensions.SizeT)
 print("SizeZ: ", czi_dimensions.SizeZ)
 print("SizeC: ", czi_dimensions.SizeC)
 print("SizeY: ", czi_dimensions.SizeY)
 print("SizeX: ", czi_dimensions.SizeX)
 
 # try to write XML to file
-xmlfile = czimd.writexml(filepath)
+xmlfile = writexml(filepath)
 
 # get info about the channels
-czi_channels = czimd.CziChannelInfo(filepath)
+czi_channels = CziChannelInfo(filepath)
 
-# get the complete metadata from the CZI as one big object
-czimd_complete = czimd.get_metadata_as_object(filepath)
+# get the complete metadata_tools from the CZI as one big object
+czimd_complete = get_metadata_as_object(filepath)
 
 # get an object containing only the dimension information
-czi_dimensions = czimd.CziDimensions(filepath)
+czi_dimensions = CziDimensions(filepath)
 
 # get an object containing only the dimension information
-czi_scale = czimd.CziScaling(filepath)
+czi_scale = CziScaling(filepath)
 
 # get an object containing information about the sample
-czi_sample = czimd.CziSampleInfo(filepath)
+czi_sample = CziSampleInfo(filepath)
 
 # get info about the objective, the microscope and the detectors
-czi_objectives = czimd.CziObjectives(filepath)
-czi_detectors = czimd.CziDetector(filepath)
-czi_microscope = czimd.CziMicroscope(filepath)
+czi_objectives = CziObjectives(filepath)
+czi_detectors = CziDetector(filepath)
+czi_microscope = CziMicroscope(filepath)
 
 # get info about the sample carrier
-czi_sample = czimd.CziSampleInfo(filepath)
+czi_sample = CziSampleInfo(filepath)
 
 # get additional metainformation
-czi_addmd = czimd.CziAddMetaData(filepath)
+czi_addmd = CziAddMetaData(filepath)
 
 # get the complete data about the bounding boxes
-czi_bbox = czimd.CziBoundingBox(filepath)
+czi_bbox = CziBoundingBox(filepath)
 ```
 
 ## Reading CZI pixel data
 
 While the [pylibCZIrw](https://pypi.org/project/pylibCZIrw/) is focussing on reading individual planes it is also helpful to read CZI pixel data as a STCZYX(A) stack. Please check [use_read_tools.py](https://github.com/sebi06/czitools/blob/main/demo/scripts/use_read_tools.py) for some examples.
 
 ```python
@@ -171,7 +195,21 @@
 
 The basic usage can be inferred from this sample notebook:&nbsp;
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sebi06/czitools/blob/main/demo/notebooks/read_czi_segment_voroni_otsu.ipynb)
 
 ## Remarks
 
 The code to read multi-dimensional with delayed reading using Dask array was heavily inspired by input from: [Pradeep Rajasekhar](https://github.com/pr4deepr).
+
+Local installation (base functionality only):
+
+```text
+pip install -e .
+```
+
+### Local Installation
+
+Local installation (full functionality):
+
+```text
+pip install -e ".[all]"
+```
```

