# Comparing `tmp/pygff-1.1.0.tar.gz` & `tmp/pygff-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygff-1.1.0.tar", last modified: Sat Jul  8 18:06:19 2023, max compression
+gzip compressed data, was "pygff-1.2.0.tar", last modified: Fri May 17 08:17:25 2024, max compression
```

## Comparing `pygff-1.1.0.tar` & `pygff-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 18:06:19.494035 pygff-1.1.0/
--rw-rw-rw-   0        0        0     1090 2022-06-02 08:09:31.000000 pygff-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     4353 2023-07-08 18:06:19.494035 pygff-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3791 2023-07-08 18:02:39.000000 pygff-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 18:06:19.475034 pygff-1.1.0/pygff/
--rw-rw-rw-   0        0        0     8378 2023-06-27 11:46:47.000000 pygff-1.1.0/pygff/GFF.py
--rw-rw-rw-   0        0        0       89 2022-06-28 20:30:20.000000 pygff-1.1.0/pygff/__init__.py
--rw-rw-rw-   0        0        0     1851 2022-06-28 20:30:20.000000 pygff-1.1.0/pygff/_util.py
--rw-rw-rw-   0        0        0    13294 2023-06-21 14:45:36.000000 pygff-1.1.0/pygff/load.py
--rw-rw-rw-   0        0        0    11314 2023-06-27 10:49:44.000000 pygff-1.1.0/pygff/save.py
-drwxrwxrwx   0        0        0        0 2023-07-08 18:06:19.486034 pygff-1.1.0/pygff.egg-info/
--rw-rw-rw-   0        0        0     4353 2023-07-08 18:06:19.000000 pygff-1.1.0/pygff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-07-08 18:06:19.000000 pygff-1.1.0/pygff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 18:06:19.000000 pygff-1.1.0/pygff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-07-08 18:06:19.000000 pygff-1.1.0/pygff.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-08 18:06:19.000000 pygff-1.1.0/pygff.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      101 2022-07-18 10:13:50.000000 pygff-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      684 2023-07-08 18:06:19.496032 pygff-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      176 2022-07-18 10:13:22.000000 pygff-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 18:06:19.492033 pygff-1.1.0/tests/
--rw-rw-rw-   0        0        0      724 2023-06-27 09:24:49.000000 pygff-1.1.0/tests/test_load.py
--rw-rw-rw-   0        0        0      856 2023-06-27 08:53:06.000000 pygff-1.1.0/tests/test_metadata.py
--rw-rw-rw-   0        0        0     2088 2023-06-27 11:42:02.000000 pygff-1.1.0/tests/test_save.py
+drwxr-xr-x   0 nicholas   (501) staff       (20)        0 2024-05-17 08:17:25.732460 pygff-1.2.0/
+-rw-r--r--   0 nicholas   (501) staff       (20)     1070 2023-09-04 09:56:18.000000 pygff-1.2.0/LICENSE
+-rw-r--r--   0 nicholas   (501) staff       (20)     4749 2024-05-17 08:17:25.732375 pygff-1.2.0/PKG-INFO
+-rw-r--r--   0 nicholas   (501) staff       (20)     4146 2024-05-17 08:05:42.000000 pygff-1.2.0/README.md
+drwxr-xr-x   0 nicholas   (501) staff       (20)        0 2024-05-17 08:17:25.729937 pygff-1.2.0/pygff/
+-rw-r--r--   0 nicholas   (501) staff       (20)     8734 2024-05-17 08:01:56.000000 pygff-1.2.0/pygff/GFF.py
+-rw-r--r--   0 nicholas   (501) staff       (20)       86 2023-09-04 09:56:18.000000 pygff-1.2.0/pygff/__init__.py
+-rw-r--r--   0 nicholas   (501) staff       (20)     1447 2024-05-16 12:40:00.000000 pygff-1.2.0/pygff/_util.py
+-rw-r--r--   0 nicholas   (501) staff       (20)    13410 2024-05-16 16:42:32.000000 pygff-1.2.0/pygff/load.py
+-rw-r--r--   0 nicholas   (501) staff       (20)    11175 2024-05-16 16:28:39.000000 pygff-1.2.0/pygff/save.py
+drwxr-xr-x   0 nicholas   (501) staff       (20)        0 2024-05-17 08:17:25.732081 pygff-1.2.0/pygff.egg-info/
+-rw-r--r--   0 nicholas   (501) staff       (20)     4749 2024-05-17 08:17:25.000000 pygff-1.2.0/pygff.egg-info/PKG-INFO
+-rw-r--r--   0 nicholas   (501) staff       (20)      330 2024-05-17 08:17:25.000000 pygff-1.2.0/pygff.egg-info/SOURCES.txt
+-rw-r--r--   0 nicholas   (501) staff       (20)        1 2024-05-17 08:17:25.000000 pygff-1.2.0/pygff.egg-info/dependency_links.txt
+-rw-r--r--   0 nicholas   (501) staff       (20)       28 2024-05-17 08:17:25.000000 pygff-1.2.0/pygff.egg-info/requires.txt
+-rw-r--r--   0 nicholas   (501) staff       (20)        6 2024-05-17 08:17:25.000000 pygff-1.2.0/pygff.egg-info/top_level.txt
+-rw-r--r--   0 nicholas   (501) staff       (20)       99 2023-09-04 09:56:18.000000 pygff-1.2.0/pyproject.toml
+-rw-r--r--   0 nicholas   (501) staff       (20)      657 2024-05-17 08:17:25.732757 pygff-1.2.0/setup.cfg
+-rw-r--r--   0 nicholas   (501) staff       (20)      172 2023-09-04 09:56:18.000000 pygff-1.2.0/setup.py
+drwxr-xr-x   0 nicholas   (501) staff       (20)        0 2024-05-17 08:17:25.731754 pygff-1.2.0/tests/
+-rw-r--r--   0 nicholas   (501) staff       (20)      701 2023-09-04 09:56:18.000000 pygff-1.2.0/tests/test_load.py
+-rw-r--r--   0 nicholas   (501) staff       (20)      831 2023-09-04 09:56:18.000000 pygff-1.2.0/tests/test_metadata.py
+-rw-r--r--   0 nicholas   (501) staff       (20)     2014 2023-09-04 09:56:18.000000 pygff-1.2.0/tests/test_save.py
```

### Comparing `pygff-1.1.0/PKG-INFO` & `pygff-1.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,108 +1,118 @@
-Metadata-Version: 2.1
-Name: pygff
-Version: 1.1.0
-Summary: A package to read and write Grace Format files (.gff/.segff)
-Home-page: https://bitbucket.org/felixgremse/gff_file_format/src/master/
-Author: Gremse-IT GmbH
-Author-email: info@gremse-it.com
-Maintainer: Nicholas Book
-Maintainer-email: nbook@gremse-it.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# PyGFF
----
-A Python package to read and write Grace Format files (*.gff / .segff*).
-
-## Easiest way to install PyGFF
----
-```bash
-$ pip install pygff
-```
-
-## Basic usage
----
-- Loading a *.gff* file:
-	```python
-	>>> from pygff import load
-	>>> data = load("image.gff")
-	```
-- Saving a numpy ndarray `np_array` as a *.gff* file:
-	```python
-	>>> from pygff import GFF, save
-	>>> save("image.gff", GFF(np_arr))
-	```
-- Saving a numpy array `seg_array` as a *.segff* (segmentation) file with class names, indices, and colors:
-	```python
-	>>> from pygff import GFF, save
-	>>> segff = GFF(seg_array)
-	>>> segff.info.set_class_dict(
-        {"Heart": {"index": 1, "color": (255, 0, 0, 255)},
-          "Liver": {"index": 2, "color": (0, 255, 0, 255)}})
-	>>> save("segmentation.segff", segff)
-	```
-	Note that `seg_array` is converted to `np.uint8` before saving. Colors are specified as RGBA, and class index 0 is reserved for "unclassified" data.
-
-## Tutorials
----
-Tutorial notebooks can be found in the `/tutorials/` directory of [this](https://bitbucket.org/felixgremse/gff_file_format/src/master/) repository. They are not included with the PyGFF package. We recommed that you to start with `01_load_and_save.ipynb` to learn more about loading, saving, and GFF objects. More tutorials will be added in the future.
-
-Running the examples requires the packages `jupyter`, `matplotlib`, `numpy`, and `scipy` to be installed. Also, please download the required example datasets if you have not cloned the repository yet.
-
-## What is GFF?
----
-GFF is an open source file format for multimodal biomedical images (*.gff*) and segmentations (*.segff*). The format supports datasets with up to five dimensions (three spatial dimensions, time-variant, and multi-channel) and a rich set of metadata key-value pairs. By default, the implementation uses a lossless compression algorithm to reduce file size and cryptographic hashing for secure writing. Multithreading is also used if possible to speed up reading and writing of GFF files.
-
-The PyGFF package is developed by [Gremse-IT GmbH](https://gremse-it.com/) (Aachen, Germany) as a Python interface for [Imalytics Preclinical 3.0](https://gremse-it.com/imalytics-preclinical/) which utilizes *.gff* by default for underlay, overlay, segmentation (*.segff*), and project files (*.imaproj*). 
-
-For more details, please refer to this publication:
-
-> Yamoah, Grace Gyamfuah et al. “Data Curation for Preclinical and Clinical Multimodal Imaging Studies.” 
-> Molecular imaging and biology vol. 21,6 (2019): 1034-1043. doi:10.1007/s11307-019-01339-0
-
-Full text: https://pubmed.ncbi.nlm.nih.gov/30868426/
-
-## How to build the package yourself
----
-1. Clone the repository
-	```bash
-	$ git clone git@bitbucket.org:felixgremse/gff_file_format.git
-	```
-2. (Optional) Create a virtual environment, e.g. with `venv`
-	```bash
-	$ python -m venv env
-	...
-	$ source env/bin/activate
-	```
-	or using `conda`
-	```bash
-	$ conda env create --file environment.yml
-	...
-	$ conda activate pygff
-	```
-3. Then, install `pygff` in editable mode, e.g. using `build`
-	```bash
-	$ python -m pip install --upgrade build
-	...
-	$ python -m pip install -e .
-	```
-	or `conda-build`
-	```bash
-	$ conda develop .
-	```
-## How to run package tests
----
-Make sure that `pytest` is installed and then simply call it from a shell in the main directory.
-```bash
-$ pytest
-```
-
-## License
----
-The PyGFF package is licensed under the terms of the [MIT license](https://opensource.org/licenses/MIT).
-
-All *.gff* files, *.segff* files, and Jupyter notebooks contained in the `/tutorials/` directory of the repository are licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode).
+Metadata-Version: 2.1
+Name: pygff
+Version: 1.2.0
+Summary: A package to read and write Grace Format files (.gff/.segff)
+Home-page: https://bitbucket.org/felixgremse/gff_file_format/src/master/
+Author: Gremse-IT GmbH
+Author-email: info@gremse-it.com
+Maintainer: Nicholas Book
+Maintainer-email: nbook@gremse-it.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy>=1.13.3
+Requires-Dist: pytest>=4.4.1
+
+# PyGFF
+---
+A Python package to read and write Grace Format files (*.gff / .segff*).
+
+## Easiest Way To Install PyGFF
+---
+```bash
+$ pip install pygff
+```
+
+## Basic Usage
+---
+1) **Loading** a *.gff* file:
+	```python
+	>>> from pygff import load
+	>>> img5D = load("tutorials/CT140.gff")
+	>>> img5D.shape
+	(1, 1, 429, 211, 290)
+	>>> img5D.info.voxel_sizes
+	[0.14 0.14 0.14]
+	```
+	GFF objects are five-dimensional [numpy arrays](https://numpy.org/doc/stable/reference/arrays.html) with additional customizable metadata such as voxel sizes and channel units. The shape / indexing convention used is (channel, time, z, y, x).
+
+2) **Saving** a numpy ndarray `np_array` as a *.gff* file:
+	```python
+	>>> from pygff import GFF, save
+	>>> save("image.gff", GFF(np_array))
+	```
+	The required metadata is automatically added by the `GFF` constructor.
+	
+3) Saving a numpy array `seg_array` as a *.segff* (**segmentation**) file with metadata for class names, indices, and colors:
+	```python
+	>>> from pygff import GFF, save
+	>>> segff = GFF(seg_array)
+	>>> segff.info.set_class_dict(
+        {"Heart": {"index": 1, "color": (255, 0, 0, 255)},
+          "Liver": {"index": 2, "color": (0, 255, 0, 255)}})
+	>>> save("segmentation.segff", segff)
+	```
+	Note that `seg_array` is converted to `np.uint8` before saving. Colors are specified as RGBA, and class index 0 is reserved for "unclassified" data.
+
+## Tutorials
+---
+Tutorial notebooks can be found in the `/tutorials/` directory of [this](https://bitbucket.org/felixgremse/gff_file_format/src/master/) repository. They are not included with the PyGFF package. We recommed that you to start with `01_load_and_save.ipynb` to learn more about loading, saving, and GFF objects. More tutorials will be added in the future.
+
+Running the examples requires the packages `jupyter`, `matplotlib`, `numpy`, and `scipy` to be installed. Also, please download the required example datasets if you have not cloned the repository yet.
+
+## What is GFF?
+---
+GFF is an open source file format for multimodal biomedical images (*.gff*) and segmentations (*.segff*). The format supports datasets with up to five dimensions (three spatial dimensions, time-variant, and multi-channel) and a rich set of metadata key-value pairs. By default, the implementation uses a lossless compression algorithm to reduce file size and cryptographic hashing for secure writing. Multithreading is also used if possible to speed up reading and writing of GFF files.
+
+The PyGFF package is developed by [Gremse-IT GmbH](https://gremse-it.com/) (Aachen, Germany) as a Python interface for [Imalytics Preclinical 3.0](https://gremse-it.com/imalytics-preclinical/) which utilizes *.gff* by default for underlay, overlay, segmentation (*.segff*), and project files (*.imaproj*). 
+
+For more details, please refer to this publication:
+
+> Yamoah, Grace Gyamfuah et al. “Data Curation for Preclinical and Clinical Multimodal Imaging Studies.” 
+> Molecular imaging and biology vol. 21,6 (2019): 1034-1043. doi:10.1007/s11307-019-01339-0
+
+Full text: https://pubmed.ncbi.nlm.nih.gov/30868426/
+
+## How to build the package yourself
+---
+1. Clone the repository
+	```bash
+	$ git clone git@bitbucket.org:felixgremse/gff_file_format.git
+	```
+2. (Optional) Create a virtual environment, e.g. with `venv`
+	```bash
+	$ python -m venv env
+	...
+	$ source env/bin/activate
+	```
+	or using `conda`
+	```bash
+	$ conda env create --file environment.yml
+	...
+	$ conda activate pygff
+	```
+3. Then, install `pygff` in editable mode, e.g. using `build`
+	```bash
+	$ python -m pip install --upgrade build
+	...
+	$ python -m pip install -e .
+	```
+	or `conda-build`
+	```bash
+	$ conda develop .
+	```
+## How to run package tests
+---
+Make sure that `pytest` is installed and then simply call it from a shell in the main directory.
+```bash
+$ pytest
+```
+
+## License
+---
+The PyGFF package is licensed under the terms of the [MIT license](https://opensource.org/licenses/MIT).
+
+All *.gff* files, *.segff* files, and Jupyter notebooks contained in the `/tutorials/` directory of the repository are licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode).
```

### Comparing `pygff-1.1.0/README.md` & `pygff-1.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,92 +1,100 @@
-# PyGFF
----
-A Python package to read and write Grace Format files (*.gff / .segff*).
-
-## Easiest way to install PyGFF
----
-```bash
-$ pip install pygff
-```
-
-## Basic usage
----
-- Loading a *.gff* file:
-	```python
-	>>> from pygff import load
-	>>> data = load("image.gff")
-	```
-- Saving a numpy ndarray `np_array` as a *.gff* file:
-	```python
-	>>> from pygff import GFF, save
-	>>> save("image.gff", GFF(np_arr))
-	```
-- Saving a numpy array `seg_array` as a *.segff* (segmentation) file with class names, indices, and colors:
-	```python
-	>>> from pygff import GFF, save
-	>>> segff = GFF(seg_array)
-	>>> segff.info.set_class_dict(
-        {"Heart": {"index": 1, "color": (255, 0, 0, 255)},
-          "Liver": {"index": 2, "color": (0, 255, 0, 255)}})
-	>>> save("segmentation.segff", segff)
-	```
-	Note that `seg_array` is converted to `np.uint8` before saving. Colors are specified as RGBA, and class index 0 is reserved for "unclassified" data.
-
-## Tutorials
----
-Tutorial notebooks can be found in the `/tutorials/` directory of [this](https://bitbucket.org/felixgremse/gff_file_format/src/master/) repository. They are not included with the PyGFF package. We recommed that you to start with `01_load_and_save.ipynb` to learn more about loading, saving, and GFF objects. More tutorials will be added in the future.
-
-Running the examples requires the packages `jupyter`, `matplotlib`, `numpy`, and `scipy` to be installed. Also, please download the required example datasets if you have not cloned the repository yet.
-
-## What is GFF?
----
-GFF is an open source file format for multimodal biomedical images (*.gff*) and segmentations (*.segff*). The format supports datasets with up to five dimensions (three spatial dimensions, time-variant, and multi-channel) and a rich set of metadata key-value pairs. By default, the implementation uses a lossless compression algorithm to reduce file size and cryptographic hashing for secure writing. Multithreading is also used if possible to speed up reading and writing of GFF files.
-
-The PyGFF package is developed by [Gremse-IT GmbH](https://gremse-it.com/) (Aachen, Germany) as a Python interface for [Imalytics Preclinical 3.0](https://gremse-it.com/imalytics-preclinical/) which utilizes *.gff* by default for underlay, overlay, segmentation (*.segff*), and project files (*.imaproj*). 
-
-For more details, please refer to this publication:
-
-> Yamoah, Grace Gyamfuah et al. “Data Curation for Preclinical and Clinical Multimodal Imaging Studies.” 
-> Molecular imaging and biology vol. 21,6 (2019): 1034-1043. doi:10.1007/s11307-019-01339-0
-
-Full text: https://pubmed.ncbi.nlm.nih.gov/30868426/
-
-## How to build the package yourself
----
-1. Clone the repository
-	```bash
-	$ git clone git@bitbucket.org:felixgremse/gff_file_format.git
-	```
-2. (Optional) Create a virtual environment, e.g. with `venv`
-	```bash
-	$ python -m venv env
-	...
-	$ source env/bin/activate
-	```
-	or using `conda`
-	```bash
-	$ conda env create --file environment.yml
-	...
-	$ conda activate pygff
-	```
-3. Then, install `pygff` in editable mode, e.g. using `build`
-	```bash
-	$ python -m pip install --upgrade build
-	...
-	$ python -m pip install -e .
-	```
-	or `conda-build`
-	```bash
-	$ conda develop .
-	```
-## How to run package tests
----
-Make sure that `pytest` is installed and then simply call it from a shell in the main directory.
-```bash
-$ pytest
-```
-
-## License
----
-The PyGFF package is licensed under the terms of the [MIT license](https://opensource.org/licenses/MIT).
-
+# PyGFF
+---
+A Python package to read and write Grace Format files (*.gff / .segff*).
+
+## Easiest Way To Install PyGFF
+---
+```bash
+$ pip install pygff
+```
+
+## Basic Usage
+---
+1) **Loading** a *.gff* file:
+	```python
+	>>> from pygff import load
+	>>> img5D = load("tutorials/CT140.gff")
+	>>> img5D.shape
+	(1, 1, 429, 211, 290)
+	>>> img5D.info.voxel_sizes
+	[0.14 0.14 0.14]
+	```
+	GFF objects are five-dimensional [numpy arrays](https://numpy.org/doc/stable/reference/arrays.html) with additional customizable metadata such as voxel sizes and channel units. The shape / indexing convention used is (channel, time, z, y, x).
+
+2) **Saving** a numpy ndarray `np_array` as a *.gff* file:
+	```python
+	>>> from pygff import GFF, save
+	>>> save("image.gff", GFF(np_array))
+	```
+	The required metadata is automatically added by the `GFF` constructor.
+	
+3) Saving a numpy array `seg_array` as a *.segff* (**segmentation**) file with metadata for class names, indices, and colors:
+	```python
+	>>> from pygff import GFF, save
+	>>> segff = GFF(seg_array)
+	>>> segff.info.set_class_dict(
+        {"Heart": {"index": 1, "color": (255, 0, 0, 255)},
+          "Liver": {"index": 2, "color": (0, 255, 0, 255)}})
+	>>> save("segmentation.segff", segff)
+	```
+	Note that `seg_array` is converted to `np.uint8` before saving. Colors are specified as RGBA, and class index 0 is reserved for "unclassified" data.
+
+## Tutorials
+---
+Tutorial notebooks can be found in the `/tutorials/` directory of [this](https://bitbucket.org/felixgremse/gff_file_format/src/master/) repository. They are not included with the PyGFF package. We recommed that you to start with `01_load_and_save.ipynb` to learn more about loading, saving, and GFF objects. More tutorials will be added in the future.
+
+Running the examples requires the packages `jupyter`, `matplotlib`, `numpy`, and `scipy` to be installed. Also, please download the required example datasets if you have not cloned the repository yet.
+
+## What is GFF?
+---
+GFF is an open source file format for multimodal biomedical images (*.gff*) and segmentations (*.segff*). The format supports datasets with up to five dimensions (three spatial dimensions, time-variant, and multi-channel) and a rich set of metadata key-value pairs. By default, the implementation uses a lossless compression algorithm to reduce file size and cryptographic hashing for secure writing. Multithreading is also used if possible to speed up reading and writing of GFF files.
+
+The PyGFF package is developed by [Gremse-IT GmbH](https://gremse-it.com/) (Aachen, Germany) as a Python interface for [Imalytics Preclinical 3.0](https://gremse-it.com/imalytics-preclinical/) which utilizes *.gff* by default for underlay, overlay, segmentation (*.segff*), and project files (*.imaproj*). 
+
+For more details, please refer to this publication:
+
+> Yamoah, Grace Gyamfuah et al. “Data Curation for Preclinical and Clinical Multimodal Imaging Studies.” 
+> Molecular imaging and biology vol. 21,6 (2019): 1034-1043. doi:10.1007/s11307-019-01339-0
+
+Full text: https://pubmed.ncbi.nlm.nih.gov/30868426/
+
+## How to build the package yourself
+---
+1. Clone the repository
+	```bash
+	$ git clone git@bitbucket.org:felixgremse/gff_file_format.git
+	```
+2. (Optional) Create a virtual environment, e.g. with `venv`
+	```bash
+	$ python -m venv env
+	...
+	$ source env/bin/activate
+	```
+	or using `conda`
+	```bash
+	$ conda env create --file environment.yml
+	...
+	$ conda activate pygff
+	```
+3. Then, install `pygff` in editable mode, e.g. using `build`
+	```bash
+	$ python -m pip install --upgrade build
+	...
+	$ python -m pip install -e .
+	```
+	or `conda-build`
+	```bash
+	$ conda develop .
+	```
+## How to run package tests
+---
+Make sure that `pytest` is installed and then simply call it from a shell in the main directory.
+```bash
+$ pytest
+```
+
+## License
+---
+The PyGFF package is licensed under the terms of the [MIT license](https://opensource.org/licenses/MIT).
+
 All *.gff* files, *.segff* files, and Jupyter notebooks contained in the `/tutorials/` directory of the repository are licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode).
```

### Comparing `pygff-1.1.0/pygff.egg-info/PKG-INFO` & `pygff-1.2.0/pygff.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,108 +1,118 @@
-Metadata-Version: 2.1
-Name: pygff
-Version: 1.1.0
-Summary: A package to read and write Grace Format files (.gff/.segff)
-Home-page: https://bitbucket.org/felixgremse/gff_file_format/src/master/
-Author: Gremse-IT GmbH
-Author-email: info@gremse-it.com
-Maintainer: Nicholas Book
-Maintainer-email: nbook@gremse-it.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# PyGFF
----
-A Python package to read and write Grace Format files (*.gff / .segff*).
-
-## Easiest way to install PyGFF
----
-```bash
-$ pip install pygff
-```
-
-## Basic usage
----
-- Loading a *.gff* file:
-	```python
-	>>> from pygff import load
-	>>> data = load("image.gff")
-	```
-- Saving a numpy ndarray `np_array` as a *.gff* file:
-	```python
-	>>> from pygff import GFF, save
-	>>> save("image.gff", GFF(np_arr))
-	```
-- Saving a numpy array `seg_array` as a *.segff* (segmentation) file with class names, indices, and colors:
-	```python
-	>>> from pygff import GFF, save
-	>>> segff = GFF(seg_array)
-	>>> segff.info.set_class_dict(
-        {"Heart": {"index": 1, "color": (255, 0, 0, 255)},
-          "Liver": {"index": 2, "color": (0, 255, 0, 255)}})
-	>>> save("segmentation.segff", segff)
-	```
-	Note that `seg_array` is converted to `np.uint8` before saving. Colors are specified as RGBA, and class index 0 is reserved for "unclassified" data.
-
-## Tutorials
----
-Tutorial notebooks can be found in the `/tutorials/` directory of [this](https://bitbucket.org/felixgremse/gff_file_format/src/master/) repository. They are not included with the PyGFF package. We recommed that you to start with `01_load_and_save.ipynb` to learn more about loading, saving, and GFF objects. More tutorials will be added in the future.
-
-Running the examples requires the packages `jupyter`, `matplotlib`, `numpy`, and `scipy` to be installed. Also, please download the required example datasets if you have not cloned the repository yet.
-
-## What is GFF?
----
-GFF is an open source file format for multimodal biomedical images (*.gff*) and segmentations (*.segff*). The format supports datasets with up to five dimensions (three spatial dimensions, time-variant, and multi-channel) and a rich set of metadata key-value pairs. By default, the implementation uses a lossless compression algorithm to reduce file size and cryptographic hashing for secure writing. Multithreading is also used if possible to speed up reading and writing of GFF files.
-
-The PyGFF package is developed by [Gremse-IT GmbH](https://gremse-it.com/) (Aachen, Germany) as a Python interface for [Imalytics Preclinical 3.0](https://gremse-it.com/imalytics-preclinical/) which utilizes *.gff* by default for underlay, overlay, segmentation (*.segff*), and project files (*.imaproj*). 
-
-For more details, please refer to this publication:
-
-> Yamoah, Grace Gyamfuah et al. “Data Curation for Preclinical and Clinical Multimodal Imaging Studies.” 
-> Molecular imaging and biology vol. 21,6 (2019): 1034-1043. doi:10.1007/s11307-019-01339-0
-
-Full text: https://pubmed.ncbi.nlm.nih.gov/30868426/
-
-## How to build the package yourself
----
-1. Clone the repository
-	```bash
-	$ git clone git@bitbucket.org:felixgremse/gff_file_format.git
-	```
-2. (Optional) Create a virtual environment, e.g. with `venv`
-	```bash
-	$ python -m venv env
-	...
-	$ source env/bin/activate
-	```
-	or using `conda`
-	```bash
-	$ conda env create --file environment.yml
-	...
-	$ conda activate pygff
-	```
-3. Then, install `pygff` in editable mode, e.g. using `build`
-	```bash
-	$ python -m pip install --upgrade build
-	...
-	$ python -m pip install -e .
-	```
-	or `conda-build`
-	```bash
-	$ conda develop .
-	```
-## How to run package tests
----
-Make sure that `pytest` is installed and then simply call it from a shell in the main directory.
-```bash
-$ pytest
-```
-
-## License
----
-The PyGFF package is licensed under the terms of the [MIT license](https://opensource.org/licenses/MIT).
-
-All *.gff* files, *.segff* files, and Jupyter notebooks contained in the `/tutorials/` directory of the repository are licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode).
+Metadata-Version: 2.1
+Name: pygff
+Version: 1.2.0
+Summary: A package to read and write Grace Format files (.gff/.segff)
+Home-page: https://bitbucket.org/felixgremse/gff_file_format/src/master/
+Author: Gremse-IT GmbH
+Author-email: info@gremse-it.com
+Maintainer: Nicholas Book
+Maintainer-email: nbook@gremse-it.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy>=1.13.3
+Requires-Dist: pytest>=4.4.1
+
+# PyGFF
+---
+A Python package to read and write Grace Format files (*.gff / .segff*).
+
+## Easiest Way To Install PyGFF
+---
+```bash
+$ pip install pygff
+```
+
+## Basic Usage
+---
+1) **Loading** a *.gff* file:
+	```python
+	>>> from pygff import load
+	>>> img5D = load("tutorials/CT140.gff")
+	>>> img5D.shape
+	(1, 1, 429, 211, 290)
+	>>> img5D.info.voxel_sizes
+	[0.14 0.14 0.14]
+	```
+	GFF objects are five-dimensional [numpy arrays](https://numpy.org/doc/stable/reference/arrays.html) with additional customizable metadata such as voxel sizes and channel units. The shape / indexing convention used is (channel, time, z, y, x).
+
+2) **Saving** a numpy ndarray `np_array` as a *.gff* file:
+	```python
+	>>> from pygff import GFF, save
+	>>> save("image.gff", GFF(np_array))
+	```
+	The required metadata is automatically added by the `GFF` constructor.
+	
+3) Saving a numpy array `seg_array` as a *.segff* (**segmentation**) file with metadata for class names, indices, and colors:
+	```python
+	>>> from pygff import GFF, save
+	>>> segff = GFF(seg_array)
+	>>> segff.info.set_class_dict(
+        {"Heart": {"index": 1, "color": (255, 0, 0, 255)},
+          "Liver": {"index": 2, "color": (0, 255, 0, 255)}})
+	>>> save("segmentation.segff", segff)
+	```
+	Note that `seg_array` is converted to `np.uint8` before saving. Colors are specified as RGBA, and class index 0 is reserved for "unclassified" data.
+
+## Tutorials
+---
+Tutorial notebooks can be found in the `/tutorials/` directory of [this](https://bitbucket.org/felixgremse/gff_file_format/src/master/) repository. They are not included with the PyGFF package. We recommed that you to start with `01_load_and_save.ipynb` to learn more about loading, saving, and GFF objects. More tutorials will be added in the future.
+
+Running the examples requires the packages `jupyter`, `matplotlib`, `numpy`, and `scipy` to be installed. Also, please download the required example datasets if you have not cloned the repository yet.
+
+## What is GFF?
+---
+GFF is an open source file format for multimodal biomedical images (*.gff*) and segmentations (*.segff*). The format supports datasets with up to five dimensions (three spatial dimensions, time-variant, and multi-channel) and a rich set of metadata key-value pairs. By default, the implementation uses a lossless compression algorithm to reduce file size and cryptographic hashing for secure writing. Multithreading is also used if possible to speed up reading and writing of GFF files.
+
+The PyGFF package is developed by [Gremse-IT GmbH](https://gremse-it.com/) (Aachen, Germany) as a Python interface for [Imalytics Preclinical 3.0](https://gremse-it.com/imalytics-preclinical/) which utilizes *.gff* by default for underlay, overlay, segmentation (*.segff*), and project files (*.imaproj*). 
+
+For more details, please refer to this publication:
+
+> Yamoah, Grace Gyamfuah et al. “Data Curation for Preclinical and Clinical Multimodal Imaging Studies.” 
+> Molecular imaging and biology vol. 21,6 (2019): 1034-1043. doi:10.1007/s11307-019-01339-0
+
+Full text: https://pubmed.ncbi.nlm.nih.gov/30868426/
+
+## How to build the package yourself
+---
+1. Clone the repository
+	```bash
+	$ git clone git@bitbucket.org:felixgremse/gff_file_format.git
+	```
+2. (Optional) Create a virtual environment, e.g. with `venv`
+	```bash
+	$ python -m venv env
+	...
+	$ source env/bin/activate
+	```
+	or using `conda`
+	```bash
+	$ conda env create --file environment.yml
+	...
+	$ conda activate pygff
+	```
+3. Then, install `pygff` in editable mode, e.g. using `build`
+	```bash
+	$ python -m pip install --upgrade build
+	...
+	$ python -m pip install -e .
+	```
+	or `conda-build`
+	```bash
+	$ conda develop .
+	```
+## How to run package tests
+---
+Make sure that `pytest` is installed and then simply call it from a shell in the main directory.
+```bash
+$ pytest
+```
+
+## License
+---
+The PyGFF package is licensed under the terms of the [MIT license](https://opensource.org/licenses/MIT).
+
+All *.gff* files, *.segff* files, and Jupyter notebooks contained in the `/tutorials/` directory of the repository are licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode).
```

### Comparing `pygff-1.1.0/setup.cfg` & `pygff-1.2.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,42 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2070 7967 6666 0d0a 7665 7273 696f   = pygff..versio
-00000020: 6e20 3d20 312e 312e 300d 0a61 7574 686f  n = 1.1.0..autho
-00000030: 7220 3d20 4772 656d 7365 2d49 5420 476d  r = Gremse-IT Gm
-00000040: 6248 0d0a 6175 7468 6f72 5f65 6d61 696c  bH..author_email
-00000050: 203d 2069 6e66 6f40 6772 656d 7365 2d69   = info@gremse-i
-00000060: 742e 636f 6d0d 0a6d 6169 6e74 6169 6e65  t.com..maintaine
-00000070: 7220 3d20 4e69 6368 6f6c 6173 2042 6f6f  r = Nicholas Boo
-00000080: 6b0d 0a6d 6169 6e74 6169 6e65 725f 656d  k..maintainer_em
-00000090: 6169 6c20 3d20 6e62 6f6f 6b40 6772 656d  ail = nbook@grem
-000000a0: 7365 2d69 742e 636f 6d0d 0a64 6573 6372  se-it.com..descr
-000000b0: 6970 7469 6f6e 203d 2041 2070 6163 6b61  iption = A packa
-000000c0: 6765 2074 6f20 7265 6164 2061 6e64 2077  ge to read and w
-000000d0: 7269 7465 2047 7261 6365 2046 6f72 6d61  rite Grace Forma
-000000e0: 7420 6669 6c65 7320 282e 6766 662f 2e73  t files (.gff/.s
-000000f0: 6567 6666 290d 0a6c 6f6e 675f 6465 7363  egff)..long_desc
-00000100: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
-00000110: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
-00000120: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
-00000130: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
-00000140: 6d61 726b 646f 776e 0d0a 7572 6c20 3d20  markdown..url = 
-00000150: 6874 7470 733a 2f2f 6269 7462 7563 6b65  https://bitbucke
-00000160: 742e 6f72 672f 6665 6c69 7867 7265 6d73  t.org/felixgrems
-00000170: 652f 6766 665f 6669 6c65 5f66 6f72 6d61  e/gff_file_forma
-00000180: 742f 7372 632f 6d61 7374 6572 2f0d 0a63  t/src/master/..c
-00000190: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
-000001a0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000001b0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000001c0: 3a20 330d 0a09 4c69 6365 6e73 6520 3a3a  : 3...License ::
-000001d0: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
-000001e0: 204d 4954 204c 6963 656e 7365 0d0a 094f   MIT License...O
-000001f0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00000200: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
-00000210: 740d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  t....[options]..
-00000220: 7061 636b 6167 6573 203d 2070 7967 6666  packages = pygff
-00000230: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
-00000240: 7320 3d20 3e3d 332e 360d 0a69 6e73 7461  s = >=3.6..insta
-00000250: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
-00000260: 096e 756d 7079 3e3d 312e 3133 2e33 0d0a  .numpy>=1.13.3..
-00000270: 0970 7974 6573 743e 3d34 2e34 2e31 0d0a  .pytest>=4.4.1..
-00000280: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-00000290: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-000002a0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 7079 6766 660a 7665 7273 696f 6e20  = pygff.version 
+00000020: 3d20 312e 322e 300a 6175 7468 6f72 203d  = 1.2.0.author =
+00000030: 2047 7265 6d73 652d 4954 2047 6d62 480a   Gremse-IT GmbH.
+00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2069  author_email = i
+00000050: 6e66 6f40 6772 656d 7365 2d69 742e 636f  nfo@gremse-it.co
+00000060: 6d0a 6d61 696e 7461 696e 6572 203d 204e  m.maintainer = N
+00000070: 6963 686f 6c61 7320 426f 6f6b 0a6d 6169  icholas Book.mai
+00000080: 6e74 6169 6e65 725f 656d 6169 6c20 3d20  ntainer_email = 
+00000090: 6e62 6f6f 6b40 6772 656d 7365 2d69 742e  nbook@gremse-it.
+000000a0: 636f 6d0a 6465 7363 7269 7074 696f 6e20  com.description 
+000000b0: 3d20 4120 7061 636b 6167 6520 746f 2072  = A package to r
+000000c0: 6561 6420 616e 6420 7772 6974 6520 4772  ead and write Gr
+000000d0: 6163 6520 466f 726d 6174 2066 696c 6573  ace Format files
+000000e0: 2028 2e67 6666 2f2e 7365 6766 6629 0a6c   (.gff/.segff).l
+000000f0: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
+00000100: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
+00000110: 640a 6c6f 6e67 5f64 6573 6372 6970 7469  d.long_descripti
+00000120: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
+00000130: 3d20 7465 7874 2f6d 6172 6b64 6f77 6e0a  = text/markdown.
+00000140: 7572 6c20 3d20 6874 7470 733a 2f2f 6269  url = https://bi
+00000150: 7462 7563 6b65 742e 6f72 672f 6665 6c69  tbucket.org/feli
+00000160: 7867 7265 6d73 652f 6766 665f 6669 6c65  xgremse/gff_file
+00000170: 5f66 6f72 6d61 742f 7372 632f 6d61 7374  _format/src/mast
+00000180: 6572 2f0a 636c 6173 7369 6669 6572 7320  er/.classifiers 
+00000190: 3d20 0a09 5072 6f67 7261 6d6d 696e 6720  = ..Programming 
+000001a0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000001b0: 6f6e 203a 3a20 330a 094c 6963 656e 7365  on :: 3..License
+000001c0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+000001d0: 203a 3a20 4d49 5420 4c69 6365 6e73 650a   :: MIT License.
+000001e0: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
+000001f0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
+00000200: 656e 740a 0a5b 6f70 7469 6f6e 735d 0a70  ent..[options].p
+00000210: 6163 6b61 6765 7320 3d20 7079 6766 660a  ackages = pygff.
+00000220: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
+00000230: 3d20 3e3d 332e 360a 696e 7374 616c 6c5f  = >=3.6.install_
+00000240: 7265 7175 6972 6573 203d 200a 096e 756d  requires = ..num
+00000250: 7079 3e3d 312e 3133 2e33 0a09 7079 7465  py>=1.13.3..pyte
+00000260: 7374 3e3d 342e 342e 310a 0a5b 6567 675f  st>=4.4.1..[egg_
+00000270: 696e 666f 5d0a 7461 675f 6275 696c 6420  info].tag_build 
+00000280: 3d20 0a74 6167 5f64 6174 6520 3d20 300a  = .tag_date = 0.
+00000290: 0a                                       .
```

### Comparing `pygff-1.1.0/tests/test_load.py` & `pygff-1.2.0/tests/test_load.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from pygff import load
-from .datadir import datadir
-
-
-def test_loading(datadir):
-    path = datadir / "minimal.gff"
-
-    with open(path, "rb") as f:
-        gff = load(f)
-        assert gff[0] == 0
-
-
-def test_loading_segmentation(datadir):
-    path = datadir / "minimal_seg.segff"
-    with open(path, "rb") as f:
-        segff = load(f)
-        assert segff[0] == 0
-        assert segff.info is not None
-        meta_dict = segff.info.meta
-        assert meta_dict["Project info"] is not None
-        assert meta_dict["Project info"]["ClassColors"] == "0 0 0 255"
-        assert meta_dict["Project info"]["ClassIndices"] == "0"
-        assert meta_dict["Project info"]["ClassNames"] == "unclassified"
+from pygff import load
+from .datadir import datadir
+
+
+def test_loading(datadir):
+    path = datadir / "minimal.gff"
+
+    with open(path, "rb") as f:
+        gff = load(f)
+        assert gff[0] == 0
+
+
+def test_loading_segmentation(datadir):
+    path = datadir / "minimal_seg.segff"
+    with open(path, "rb") as f:
+        segff = load(f)
+        assert segff[0] == 0
+        assert segff.info is not None
+        meta_dict = segff.info.meta
+        assert meta_dict["Project info"] is not None
+        assert meta_dict["Project info"]["ClassColors"] == "0 0 0 255"
+        assert meta_dict["Project info"]["ClassIndices"] == "0"
+        assert meta_dict["Project info"]["ClassNames"] == "unclassified"
```

### Comparing `pygff-1.1.0/tests/test_save.py` & `pygff-1.2.0/tests/test_save.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-from pygff import load, save, GFF, GFFInfo
-import numpy as np
-import pathlib
-import pytest
-from tests.datadir import datadir
-
-
-def test_saving(datadir):
-    path = datadir / "minimal.gff"
-    gff = load(path)
-
-    output_path = datadir / "minimal_out.gff"
-
-    with open(output_path, "wb") as f:
-        save(f, gff)
-
-    gff_new = load(output_path)
-
-    assert np.array_equal(gff, gff_new)
-
-
-def test_saving_array(datadir):
-    test_array = np.ndarray((1, 1, 1, 1, 1))
-    test_info = GFFInfo()
-    test_gff = GFF(test_array, test_info)
-    arr_path = datadir / "minimal_arr.gff"
-    save(open(arr_path, "wb"), test_gff)
-    assert np.array_equal(test_gff, load(arr_path))
-
-
-def test_empty_segff(datadir):
-    gff = GFF()
-    metadata = gff.info
-
-    with pytest.raises(ValueError):  # no "ProjectInfo" set
-        metadata.get_class_dict()
-
-    save(datadir / "minimal_out.segff", gff)
-
-    segff = load(datadir / "minimal_out.segff")
-    # assert np.array_equal(gff, segff) # fails as GFF is always loaded as 5D
-
-    assert segff.info.get_class_dict() == {
-        "unclassified": {"index": 0, "color": (0, 0, 0, 255)}
-    }
-
-
-def test_add_class(datadir):
-    gff = GFF()
-    gff.info.set_class_dict({"test": {"index": 1, "color": (255, 0, 0, 255)}})
-    class_dict = gff.info.get_class_dict()
-    assert class_dict == {
-        "unclassified": {"index": 0, "color": (0, 0, 0, 255)},
-        "test": {"index": 1, "color": (255, 0, 0, 255)},
-    }
-
-    gff.info.add_class(
-        new_class={"name": "test2", "index": 2, "color": (0, 255, 0, 255)}
-    )
-    assert gff.info.get_class_dict() == {
-        "unclassified": {"index": 0, "color": (0, 0, 0, 255)},
-        "test": {"index": 1, "color": (255, 0, 0, 255)},
-        "test2": {"index": 2, "color": (0, 255, 0, 255)},
-    }
-
-    save(datadir / "add_class.segff", gff)
-
-
-if __name__ == "__main__":
-    tmp_dir = pathlib.Path("tests/testdata")
-    test_saving(tmp_dir)
-    test_saving_array(tmp_dir)
-    test_empty_segff(tmp_dir)
-    test_add_class(tmp_dir)
+from pygff import load, save, GFF, GFFInfo
+import numpy as np
+import pathlib
+import pytest
+from tests.datadir import datadir
+
+
+def test_saving(datadir):
+    path = datadir / "minimal.gff"
+    gff = load(path)
+
+    output_path = datadir / "minimal_out.gff"
+
+    with open(output_path, "wb") as f:
+        save(f, gff)
+
+    gff_new = load(output_path)
+
+    assert np.array_equal(gff, gff_new)
+
+
+def test_saving_array(datadir):
+    test_array = np.ndarray((1, 1, 1, 1, 1))
+    test_info = GFFInfo()
+    test_gff = GFF(test_array, test_info)
+    arr_path = datadir / "minimal_arr.gff"
+    save(open(arr_path, "wb"), test_gff)
+    assert np.array_equal(test_gff, load(arr_path))
+
+
+def test_empty_segff(datadir):
+    gff = GFF()
+    metadata = gff.info
+
+    with pytest.raises(ValueError):  # no "ProjectInfo" set
+        metadata.get_class_dict()
+
+    save(datadir / "minimal_out.segff", gff)
+
+    segff = load(datadir / "minimal_out.segff")
+    # assert np.array_equal(gff, segff) # fails as GFF is always loaded as 5D
+
+    assert segff.info.get_class_dict() == {
+        "unclassified": {"index": 0, "color": (0, 0, 0, 255)}
+    }
+
+
+def test_add_class(datadir):
+    gff = GFF()
+    gff.info.set_class_dict({"test": {"index": 1, "color": (255, 0, 0, 255)}})
+    class_dict = gff.info.get_class_dict()
+    assert class_dict == {
+        "unclassified": {"index": 0, "color": (0, 0, 0, 255)},
+        "test": {"index": 1, "color": (255, 0, 0, 255)},
+    }
+
+    gff.info.add_class(
+        new_class={"name": "test2", "index": 2, "color": (0, 255, 0, 255)}
+    )
+    assert gff.info.get_class_dict() == {
+        "unclassified": {"index": 0, "color": (0, 0, 0, 255)},
+        "test": {"index": 1, "color": (255, 0, 0, 255)},
+        "test2": {"index": 2, "color": (0, 255, 0, 255)},
+    }
+
+    save(datadir / "add_class.segff", gff)
+
+
+if __name__ == "__main__":
+    tmp_dir = pathlib.Path("tests/testdata")
+    test_saving(tmp_dir)
+    test_saving_array(tmp_dir)
+    test_empty_segff(tmp_dir)
+    test_add_class(tmp_dir)
```

