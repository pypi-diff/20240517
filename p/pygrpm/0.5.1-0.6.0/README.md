# Comparing `tmp/pygrpm-0.5.1.tar.gz` & `tmp/pygrpm-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrpm-0.5.1.tar", max compression
+gzip compressed data, was "pygrpm-0.6.0.tar", max compression
```

## Comparing `pygrpm-0.5.1.tar` & `pygrpm-0.6.0.tar`

### file list

```diff
@@ -1,55 +1,57 @@
--rw-r--r--   0        0        0    35185 2023-12-08 16:43:21.531063 pygrpm-0.5.1/LICENSE.txt
--rw-r--r--   0        0        0     8913 2024-01-16 17:53:16.497666 pygrpm-0.5.1/README.md
--rw-r--r--   0        0        0        0 2024-01-19 16:11:48.081745 pygrpm-0.5.1/pygrpm/__init__.py
--rw-r--r--   0        0        0      172 2023-06-27 17:10:36.561746 pygrpm-0.5.1/pygrpm/ct_utils/__init__.py
--rw-r--r--   0        0        0     8077 2024-01-12 15:38:26.608909 pygrpm-0.5.1/pygrpm/ct_utils/hounsfield_conversion.py
--rw-r--r--   0        0        0      191 2024-01-12 15:38:26.609909 pygrpm-0.5.1/pygrpm/dicom/__init__.py
--rw-r--r--   0        0        0     9407 2023-12-15 20:12:47.269732 pygrpm-0.5.1/pygrpm/dicom/reader.py
--rw-r--r--   0        0        0      152 2024-01-12 15:38:26.609909 pygrpm-0.5.1/pygrpm/dicom/sr/__init__.py
--rw-r--r--   0        0        0    19794 2024-01-12 15:38:26.609909 pygrpm-0.5.1/pygrpm/dicom/sr/builder.py
--rw-r--r--   0        0        0  1864749 2024-01-12 15:38:26.672911 pygrpm-0.5.1/pygrpm/dicom/sr/data/DCM_2023c_20230704.csv
--rw-r--r--   0        0        0     6518 2024-01-12 15:38:26.672911 pygrpm-0.5.1/pygrpm/dicom/sr/dicom_content_sequence.py
--rw-r--r--   0        0        0     5796 2024-01-19 15:47:33.552579 pygrpm-0.5.1/pygrpm/dicom/sr/sr.py
--rw-r--r--   0        0        0    11436 2024-01-12 15:38:26.673911 pygrpm-0.5.1/pygrpm/dicom/sr/sr_tags.py
--rw-r--r--   0        0        0     1340 2024-01-12 15:38:26.673911 pygrpm-0.5.1/pygrpm/dicom/sr/terminologies.py
--rw-r--r--   0        0        0      704 2024-01-12 15:38:26.673911 pygrpm-0.5.1/pygrpm/dicom/sr/utils.py
--rw-r--r--   0        0        0     5153 2023-12-15 20:12:47.269732 pygrpm-0.5.1/pygrpm/dicom/structures.py
--rw-r--r--   0        0        0     2387 2023-12-15 20:06:46.274136 pygrpm-0.5.1/pygrpm/dicom/utils.py
--rw-r--r--   0        0        0      102 2023-12-08 16:43:21.559064 pygrpm-0.5.1/pygrpm/geometry/__init__.py
--rw-r--r--   0        0        0     4964 2023-12-15 18:06:06.021945 pygrpm-0.5.1/pygrpm/geometry/data/CT01_materials.json
--rw-r--r--   0        0        0    12191 2023-12-15 20:21:33.296971 pygrpm-0.5.1/pygrpm/geometry/egsphant.py
--rw-r--r--   0        0        0     4837 2023-12-15 21:16:54.686222 pygrpm-0.5.1/pygrpm/index_tracker.py
--rw-r--r--   0        0        0      352 2023-06-27 17:10:36.564746 pygrpm-0.5.1/pygrpm/nistparser/__init__.py
--rw-r--r--   0        0        0     1436 2023-06-27 17:10:36.564746 pygrpm-0.5.1/pygrpm/nistparser/internal/data/material_lookup_key.json
--rw-r--r--   0        0        0     2216 2023-06-27 17:10:36.564746 pygrpm-0.5.1/pygrpm/nistparser/internal/enum_generator.py
--rw-r--r--   0        0        0     1685 2023-06-27 17:10:36.564746 pygrpm-0.5.1/pygrpm/nistparser/materials_enum.py
--rw-r--r--   0        0        0    16198 2024-01-12 15:38:26.673911 pygrpm-0.5.1/pygrpm/nistparser/nistparser.py
--rw-r--r--   0        0        0      123 2023-06-27 17:10:36.566746 pygrpm-0.5.1/pygrpm/tg263/__init__.py
--rw-r--r--   0        0        0      386 2023-06-27 17:10:36.567746 pygrpm-0.5.1/pygrpm/tg263/nomenclature/__init__.py
--rw-r--r--   0        0        0      475 2023-06-27 17:10:36.567746 pygrpm-0.5.1/pygrpm/tg263/nomenclature/_dictionary.py
--rw-r--r--   0        0        0      118 2023-06-27 17:10:36.567746 pygrpm-0.5.1/pygrpm/tg263/nomenclature/_exceptions.py
--rw-r--r--   0        0        0     3347 2023-12-15 20:12:47.271732 pygrpm-0.5.1/pygrpm/tg263/nomenclature/structures.py
--rwxr-xr-x   0        0        0   216046 2023-06-27 17:10:36.568746 pygrpm-0.5.1/pygrpm/tg263/nomenclature/tg263.json
--rw-r--r--   0        0        0     1258 2023-09-08 19:56:10.857811 pygrpm-0.5.1/pygrpm/tg43/README.md
--rw-r--r--   0        0        0       72 2024-01-12 15:38:26.674911 pygrpm-0.5.1/pygrpm/tg43/__init__.py
--rw-r--r--   0        0        0     3029 2023-09-08 19:56:10.857811 pygrpm-0.5.1/pygrpm/tg43/data/Flexisource/F.dat
--rw-r--r--   0        0        0        5 2023-09-08 19:56:10.857811 pygrpm-0.5.1/pygrpm/tg43/data/Flexisource/L.dat
--rw-r--r--   0        0        0        6 2023-09-08 19:56:10.858811 pygrpm-0.5.1/pygrpm/tg43/data/Flexisource/Lambda.dat
--rw-r--r--   0        0        0      141 2023-09-08 19:56:10.858811 pygrpm-0.5.1/pygrpm/tg43/data/Flexisource/gL.dat
--rw-r--r--   0        0        0     3893 2023-09-08 19:56:10.858811 pygrpm-0.5.1/pygrpm/tg43/data/MBDCA/F.dat
--rw-r--r--   0        0        0        5 2023-09-08 19:56:10.858811 pygrpm-0.5.1/pygrpm/tg43/data/MBDCA/L.dat
--rw-r--r--   0        0        0        7 2023-09-08 19:56:10.858811 pygrpm-0.5.1/pygrpm/tg43/data/MBDCA/Lambda.dat
--rw-r--r--   0        0        0      222 2023-09-08 19:56:10.858811 pygrpm-0.5.1/pygrpm/tg43/data/MBDCA/gL.dat
--rw-r--r--   0        0        0     5881 2023-09-08 19:56:10.858811 pygrpm-0.5.1/pygrpm/tg43/data/MicroSelectronV2/F.dat
--rw-r--r--   0        0        0        5 2023-09-08 19:56:10.859811 pygrpm-0.5.1/pygrpm/tg43/data/MicroSelectronV2/L.dat
--rw-r--r--   0        0        0        6 2023-09-08 19:56:10.859811 pygrpm-0.5.1/pygrpm/tg43/data/MicroSelectronV2/Lambda.dat
--rw-r--r--   0        0        0      171 2023-09-08 19:56:10.859811 pygrpm-0.5.1/pygrpm/tg43/data/MicroSelectronV2/gL.dat
--rw-r--r--   0        0        0     1800 2023-09-08 19:56:10.859811 pygrpm-0.5.1/pygrpm/tg43/data/SelectSeed/F.dat
--rw-r--r--   0        0        0        5 2023-09-08 19:56:10.859811 pygrpm-0.5.1/pygrpm/tg43/data/SelectSeed/L.dat
--rw-r--r--   0        0        0        6 2023-09-08 19:56:10.859811 pygrpm-0.5.1/pygrpm/tg43/data/SelectSeed/Lambda.dat
--rw-r--r--   0        0        0      177 2023-09-08 19:56:10.859811 pygrpm-0.5.1/pygrpm/tg43/data/SelectSeed/gL.dat
--rw-r--r--   0        0        0      177 2023-09-08 19:56:10.860811 pygrpm-0.5.1/pygrpm/tg43/data/SelectSeed/phi.dat
--rw-r--r--   0        0        0    12788 2024-01-12 15:38:26.674911 pygrpm-0.5.1/pygrpm/tg43/seed.py
--rw-r--r--   0        0        0      669 2023-09-08 19:56:10.860811 pygrpm-0.5.1/pygrpm/uid.py
--rw-r--r--   0        0        0     1937 2024-01-19 16:00:19.109668 pygrpm-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    10392 1970-01-01 00:00:00.000000 pygrpm-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    35185 2023-12-08 16:43:21.531063 pygrpm-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     8939 2024-01-19 16:15:33.885620 pygrpm-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2024-02-02 15:45:50.924793 pygrpm-0.6.0/pygrpm/__init__.py
+-rw-r--r--   0        0        0      237 2024-01-19 16:15:33.890620 pygrpm-0.6.0/pygrpm/dicom/__init__.py
+-rw-r--r--   0        0        0     9407 2023-12-15 20:12:47.269732 pygrpm-0.6.0/pygrpm/dicom/reader.py
+-rw-r--r--   0        0        0      152 2024-01-12 15:38:26.609909 pygrpm-0.6.0/pygrpm/dicom/sr/__init__.py
+-rw-r--r--   0        0        0    19805 2024-01-19 20:44:53.778339 pygrpm-0.6.0/pygrpm/dicom/sr/builder.py
+-rw-r--r--   0        0        0  1864749 2024-01-12 15:38:26.672911 pygrpm-0.6.0/pygrpm/dicom/sr/data/DCM_2023c_20230704.csv
+-rw-r--r--   0        0        0     6518 2024-01-12 15:38:26.672911 pygrpm-0.6.0/pygrpm/dicom/sr/dicom_content_sequence.py
+-rw-r--r--   0        0        0     5796 2024-01-19 15:47:33.552579 pygrpm-0.6.0/pygrpm/dicom/sr/sr.py
+-rw-r--r--   0        0        0    11436 2024-01-12 15:38:26.673911 pygrpm-0.6.0/pygrpm/dicom/sr/sr_tags.py
+-rw-r--r--   0        0        0     1340 2024-01-12 15:38:26.673911 pygrpm-0.6.0/pygrpm/dicom/sr/terminologies.py
+-rw-r--r--   0        0        0      704 2024-01-12 15:38:26.673911 pygrpm-0.6.0/pygrpm/dicom/sr/utils.py
+-rw-r--r--   0        0        0     5153 2023-12-15 20:12:47.269732 pygrpm-0.6.0/pygrpm/dicom/structures.py
+-rw-r--r--   0        0        0      669 2024-01-19 16:15:33.892620 pygrpm-0.6.0/pygrpm/dicom/uid.py
+-rw-r--r--   0        0        0     2387 2023-12-15 20:06:46.274136 pygrpm-0.6.0/pygrpm/dicom/utils.py
+-rw-r--r--   0        0        0      102 2023-12-08 16:43:21.559064 pygrpm-0.6.0/pygrpm/geometry/__init__.py
+-rw-r--r--   0        0        0     4964 2023-12-15 18:06:06.021945 pygrpm-0.6.0/pygrpm/geometry/data/CT01_materials.json
+-rw-r--r--   0        0        0    12178 2024-01-27 01:51:13.461137 pygrpm-0.6.0/pygrpm/geometry/egsphant.py
+-rw-r--r--   0        0        0      141 2024-01-19 16:15:33.892620 pygrpm-0.6.0/pygrpm/material/__init__.py
+-rw-r--r--   0        0        0     8077 2024-01-19 16:15:33.892620 pygrpm-0.6.0/pygrpm/material/hounsfield_conversion.py
+-rw-r--r--   0        0        0      398 2024-01-19 20:44:53.778339 pygrpm-0.6.0/pygrpm/material/nistparser/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-02 15:45:50.927793 pygrpm-0.6.0/pygrpm/material/nistparser/internal/__init__.py
+-rw-r--r--   0        0        0     1436 2024-01-19 16:15:33.893620 pygrpm-0.6.0/pygrpm/material/nistparser/internal/data/material_lookup_key.json
+-rw-r--r--   0        0        0     2216 2024-01-19 16:15:33.893620 pygrpm-0.6.0/pygrpm/material/nistparser/internal/enum_generator.py
+-rw-r--r--   0        0        0     1685 2024-01-19 16:15:33.893620 pygrpm-0.6.0/pygrpm/material/nistparser/materials_enum.py
+-rw-r--r--   0        0        0    16198 2024-01-19 16:15:33.894621 pygrpm-0.6.0/pygrpm/material/nistparser/nistparser.py
+-rw-r--r--   0        0        0      123 2023-06-27 17:10:36.566746 pygrpm-0.6.0/pygrpm/tg263/__init__.py
+-rw-r--r--   0        0        0      386 2023-06-27 17:10:36.567746 pygrpm-0.6.0/pygrpm/tg263/nomenclature/__init__.py
+-rw-r--r--   0        0        0      475 2023-06-27 17:10:36.567746 pygrpm-0.6.0/pygrpm/tg263/nomenclature/_dictionary.py
+-rw-r--r--   0        0        0      118 2023-06-27 17:10:36.567746 pygrpm-0.6.0/pygrpm/tg263/nomenclature/_exceptions.py
+-rw-r--r--   0        0        0     3347 2023-12-15 20:12:47.271732 pygrpm-0.6.0/pygrpm/tg263/nomenclature/structures.py
+-rwxr-xr-x   0        0        0   216046 2023-06-27 17:10:36.568746 pygrpm-0.6.0/pygrpm/tg263/nomenclature/tg263.json
+-rw-r--r--   0        0        0     1258 2023-09-08 19:56:10.857811 pygrpm-0.6.0/pygrpm/tg43/README.md
+-rw-r--r--   0        0        0       72 2024-01-12 15:38:26.674911 pygrpm-0.6.0/pygrpm/tg43/__init__.py
+-rw-r--r--   0        0        0     3029 2023-09-08 19:56:10.857811 pygrpm-0.6.0/pygrpm/tg43/data/Flexisource/F.dat
+-rw-r--r--   0        0        0        5 2023-09-08 19:56:10.857811 pygrpm-0.6.0/pygrpm/tg43/data/Flexisource/L.dat
+-rw-r--r--   0        0        0        6 2023-09-08 19:56:10.858811 pygrpm-0.6.0/pygrpm/tg43/data/Flexisource/Lambda.dat
+-rw-r--r--   0        0        0      141 2023-09-08 19:56:10.858811 pygrpm-0.6.0/pygrpm/tg43/data/Flexisource/gL.dat
+-rw-r--r--   0        0        0     3893 2023-09-08 19:56:10.858811 pygrpm-0.6.0/pygrpm/tg43/data/MBDCA/F.dat
+-rw-r--r--   0        0        0        5 2023-09-08 19:56:10.858811 pygrpm-0.6.0/pygrpm/tg43/data/MBDCA/L.dat
+-rw-r--r--   0        0        0        7 2023-09-08 19:56:10.858811 pygrpm-0.6.0/pygrpm/tg43/data/MBDCA/Lambda.dat
+-rw-r--r--   0        0        0      222 2023-09-08 19:56:10.858811 pygrpm-0.6.0/pygrpm/tg43/data/MBDCA/gL.dat
+-rw-r--r--   0        0        0     5881 2023-09-08 19:56:10.858811 pygrpm-0.6.0/pygrpm/tg43/data/MicroSelectronV2/F.dat
+-rw-r--r--   0        0        0        5 2023-09-08 19:56:10.859811 pygrpm-0.6.0/pygrpm/tg43/data/MicroSelectronV2/L.dat
+-rw-r--r--   0        0        0        6 2023-09-08 19:56:10.859811 pygrpm-0.6.0/pygrpm/tg43/data/MicroSelectronV2/Lambda.dat
+-rw-r--r--   0        0        0      171 2023-09-08 19:56:10.859811 pygrpm-0.6.0/pygrpm/tg43/data/MicroSelectronV2/gL.dat
+-rw-r--r--   0        0        0     1800 2023-09-08 19:56:10.859811 pygrpm-0.6.0/pygrpm/tg43/data/SelectSeed/F.dat
+-rw-r--r--   0        0        0        5 2023-09-08 19:56:10.859811 pygrpm-0.6.0/pygrpm/tg43/data/SelectSeed/L.dat
+-rw-r--r--   0        0        0        6 2023-09-08 19:56:10.859811 pygrpm-0.6.0/pygrpm/tg43/data/SelectSeed/Lambda.dat
+-rw-r--r--   0        0        0      177 2023-09-08 19:56:10.859811 pygrpm-0.6.0/pygrpm/tg43/data/SelectSeed/gL.dat
+-rw-r--r--   0        0        0      177 2023-09-08 19:56:10.860811 pygrpm-0.6.0/pygrpm/tg43/data/SelectSeed/phi.dat
+-rw-r--r--   0        0        0    12788 2024-01-12 15:38:26.674911 pygrpm-0.6.0/pygrpm/tg43/seed.py
+-rw-r--r--   0        0        0       84 2024-01-22 17:35:44.930763 pygrpm-0.6.0/pygrpm/visualization/__init__.py
+-rw-r--r--   0        0        0     4837 2024-01-19 16:15:33.895620 pygrpm-0.6.0/pygrpm/visualization/index_tracker.py
+-rw-r--r--   0        0        0     1937 2024-01-19 20:44:53.782339 pygrpm-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    10418 1970-01-01 00:00:00.000000 pygrpm-0.6.0/PKG-INFO
```

### Comparing `pygrpm-0.5.1/LICENSE.txt` & `pygrpm-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygrpm-0.5.1/README.md` & `pygrpm-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 
 # Index tracker
 Submodule that allows scrolling through slices of 3-D images using the matplotlib backend.
 
 ```python
 import matplotlib.pyplot as plt
 import numpy
-from pygrpm.index_tracker import IndexTracker
+from pygrpm.visualization.index_tracker import IndexTracker
 
 tracker = IndexTracker(
     *plt.subplot(),
     numpy.random.rand(512, 512, 10),
     ...
 )
 tracker.ax.set_title('My 3-D random image')
@@ -164,15 +164,15 @@
 This method retrieves the desired cross-sections of an element at given energies
 on the NIST website in (barns/electron), barn=10^-24cm^2.
 
 Simple use example:
 
 ```python
 import numpy as np
-from pygrpm.nistparser import get_cross_sections
+from pygrpm.material.nistparser import get_cross_sections
 
 # Define the energies in KeV
 # Numpy array is not mandatory, can be any sequence
 energies = np.linspace(30, 200, 200)
 
 # Prints the returned list
 print(get_cross_sections("H", energies))
@@ -190,16 +190,16 @@
 
 #### get_composition
 This method is used to get and parse material composition from https://physics.nist.gov/cgi-bin/Star/compos.pl
 
 Simple use example:
 
 ```python
-from pygrpm.nistparser import get_composition
-from pygrpm.nistparser.materials_enum import NISTMaterials
+from pygrpm.material.nistparser import get_composition
+from pygrpm.material.nistparser import NISTMaterials
 
 # Prints the returned dictionary
 print(get_composition(NISTMaterials.M3_WAX))
 ```
 Note that get_composition expects the material to be of instance NISTMaterials
 
 ### Acknowledgements
```

### Comparing `pygrpm-0.5.1/pygrpm/ct_utils/hounsfield_conversion.py` & `pygrpm-0.6.0/pygrpm/material/hounsfield_conversion.py`

 * *Files identical despite different names*

### Comparing `pygrpm-0.5.1/pygrpm/dicom/reader.py` & `pygrpm-0.6.0/pygrpm/dicom/reader.py`

 * *Files identical despite different names*

### Comparing `pygrpm-0.5.1/pygrpm/dicom/sr/builder.py` & `pygrpm-0.6.0/pygrpm/dicom/sr/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 from typing import Dict, List, Union
 
 import pydicom
 from pydicom.dataset import FileMetaDataset
 from pydicom.filebase import DicomBytesIO
 from pydicom.uid import PYDICOM_IMPLEMENTATION_UID
 
-from ...uid import generate_uid
+from pygrpm.dicom.uid import generate_uid
+
 from .sr_tags import (
     SR_TYPING,
     make_concept_name_code_sequence,
     make_content_sequence,
     make_referenced_instance_sequence,
 )
 from .utils import read_dicom
```

### Comparing `pygrpm-0.5.1/pygrpm/dicom/sr/data/DCM_2023c_20230704.csv` & `pygrpm-0.6.0/pygrpm/dicom/sr/data/DCM_2023c_20230704.csv`

 * *Files identical despite different names*

### Comparing `pygrpm-0.5.1/pygrpm/dicom/sr/dicom_content_sequence.py` & `pygrpm-0.6.0/pygrpm/dicom/sr/dicom_content_sequence.py`

 * *Files identical despite different names*

### Comparing `pygrpm-0.5.1/pygrpm/dicom/sr/sr.py` & `pygrpm-0.6.0/pygrpm/dicom/sr/sr.py`

 * *Files identical despite different names*

### Comparing `pygrpm-0.5.1/pygrpm/dicom/sr/sr_tags.py` & `pygrpm-0.6.0/pygrpm/dicom/sr/sr_tags.py`

 * *Files identical despite different names*

### Comparing `pygrpm-0.5.1/pygrpm/dicom/sr/terminologies.py` & `pygrpm-0.6.0/pygrpm/dicom/sr/terminologies.py`

 * *Files identical despite different names*

### Comparing `pygrpm-0.5.1/pygrpm/dicom/sr/utils.py` & `pygrpm-0.6.0/pygrpm/dicom/sr/utils.py`

 * *Files identical despite different names*

### Comparing `pygrpm-0.5.1/pygrpm/dicom/structures.py` & `pygrpm-0.6.0/pygrpm/dicom/structures.py`

 * *Files identical despite different names*

### Comparing `pygrpm-0.5.1/pygrpm/dicom/utils.py` & `pygrpm-0.6.0/pygrpm/dicom/utils.py`

 * *Files identical despite different names*

### Comparing `pygrpm-0.5.1/pygrpm/geometry/data/CT01_materials.json` & `pygrpm-0.6.0/pygrpm/geometry/data/CT01_materials.json`

 * *Files identical despite different names*

### Comparing `pygrpm-0.5.1/pygrpm/geometry/egsphant.py` & `pygrpm-0.6.0/pygrpm/geometry/egsphant.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,40 +8,41 @@
 
 import numpy as np
 
 # Global list of characters for the material assignment
 CHARACTERS = (
     r"123456789:;<=>?@ABCDEFGHIJKLMNOPQRSTUVWXYZ[\]^_`abcdefghijklmnopqrstuvwxyz"
 )
-# Built-in dictionaries of values
-material_dictionaries = {"CT01": "data/CT01_materials.json"}
+
+MATERIAL_DICTIONARIES = {
+    "CT01": Path(os.path.dirname(__file__)) / "data/CT01_materials.json"
+}
 
 
 class Egsphant:
     """
     Class used to take a volumetric numpy array along with physical center coordinates and
     voxel spacing values to generate an egsphant file of the volume
     """
 
     # pylint: disable=R0913, R0902
     def __init__(
             self,
             volume: np.ndarray,
             spacings: np.ndarray,
             center: np.ndarray,
-            materials: Union[str, Dict],
+            materials: Dict,
     ) -> None:
         """
         Class used to convert a provided 3D numpy array into an egsphant volume
         @param volume: A 3D numpy array who's values dictate material information
         @param spacings: A sequence three values representing spacing in each axis
         @param center: A sequence of three values representing the volume's center, such as
         (0, 0, 0), (-21, -39, 256), etc...
-        @param materials: Either a string representing predefined material assignments
-                or a custom dictionary with material name, value ranges, and density
+        @param materials: Dictionary with material name, value ranges, and density
         @param slice_axis: Axis where slices are located for a 3-D image (usually 0 or 2).
             Defaults to 0.
         """
         self.volume: np.ndarray = volume
         self.spacings: np.ndarray = spacings
         self.center: np.ndarray = center
         self.materials: Dict = materials
@@ -56,22 +57,22 @@
         self.density_string: str = ""
 
         self.built: bool = False
 
     def __str__(self):
         return self.content
 
-    def build(self):
+    def build(self, precision=3):
         """
         Generic build method to generate and format the egsphant string as desired
         @return: None
         """
         self._trim_materials()
         self.generate_headers()
-        self.generate_voxel_positions()
+        self.generate_voxel_positions(precision)
         self.generate_volumes_string()
 
         self.built = True
 
     @property
     def content(self) -> str:
         """
@@ -262,45 +263,45 @@
     """
     Helper method to ensure proper materials assignment to the Egsphant class
     @param materials: The desired materials dictionary, or filename
     @return: The associated materials dictionary
     """
     # Assign the proper values to internal self.materials dictionary
     if isinstance(materials, str):
-        if materials in material_dictionaries:
+        if materials in MATERIAL_DICTIONARIES:
             # Open the jsons with the materials and open it in dictionary
-            path_to_dict = (
-                    Path(os.path.dirname(__file__)) / material_dictionaries[materials]
-            )
-            with open(path_to_dict, "r", encoding="utf8") as json_file:
+            with open(MATERIAL_DICTIONARIES[materials], "r", encoding="utf8") as json_file:
                 return json.load(json_file)
         else:
             raise ValueError(
                 f"Provided dictionary name was not an accepted value."
-                f"Current values are {material_dictionaries.keys()}"
+                f"Current values are {MATERIAL_DICTIONARIES.keys()}"
             )
     elif isinstance(materials, dict):
         return materials
     else:
         raise ValueError("Provided materials was neither a string nor dictionary.")
 
 
+# pylint: disable=too-many-arguments
 def make_egsphant_from_numpy(volume: np.ndarray,
                              spacings: Sequence,
                              center: Sequence,
                              materials: Union[str, Dict],
+                             precision: int = 3,
                              slice_axis: int = 0) -> Egsphant:
     """
     Utility method to build an Egsphant class given numpy content
     @param volume: A 3D numpy array who's values dictate material information
     @param spacings: A sequence three values representing spacing in each axis
     @param center: A sequence of three values representing the volume's center, such as
     (0, 0, 0), (-21, -39, 256), etc...
     @param materials: Either a string representing predefined material assignments
             or a custom dictionary with material name, value ranges, and density
+    @param precision: The decimal precision for voxel positions
     @param slice_axis: Axis where slices are located for a 3-D image (usually 0 or 2).
         Defaults to 0.
     @return: The Egsphant class structured on the provided input
     """
     # ValueError will be raised here if inputs are unacceptable
     _validate_inputs(volume, spacings, center)
 
@@ -308,10 +309,10 @@
     volume = volume.swapaxes(0, slice_axis)
     center = np.array(center)
     spacings = np.array(spacings)
 
     materials = _ensure_materials_dict(materials)
 
     egsphant = Egsphant(volume, spacings, center, materials)
-    egsphant.build()
+    egsphant.build(precision=precision)
 
     return egsphant
```

### Comparing `pygrpm-0.5.1/pygrpm/index_tracker.py` & `pygrpm-0.6.0/pygrpm/visualization/index_tracker.py`

 * *Files identical despite different names*

### Comparing `pygrpm-0.5.1/pygrpm/nistparser/internal/data/material_lookup_key.json` & `pygrpm-0.6.0/pygrpm/material/nistparser/internal/data/material_lookup_key.json`

 * *Files identical despite different names*

### Comparing `pygrpm-0.5.1/pygrpm/nistparser/internal/enum_generator.py` & `pygrpm-0.6.0/pygrpm/material/nistparser/internal/enum_generator.py`

 * *Files identical despite different names*

### Comparing `pygrpm-0.5.1/pygrpm/nistparser/materials_enum.py` & `pygrpm-0.6.0/pygrpm/material/nistparser/materials_enum.py`

 * *Files identical despite different names*

### Comparing `pygrpm-0.5.1/pygrpm/nistparser/nistparser.py` & `pygrpm-0.6.0/pygrpm/material/nistparser/nistparser.py`

 * *Files identical despite different names*

### Comparing `pygrpm-0.5.1/pygrpm/tg263/nomenclature/structures.py` & `pygrpm-0.6.0/pygrpm/tg263/nomenclature/structures.py`

 * *Files identical despite different names*

### Comparing `pygrpm-0.5.1/pygrpm/tg263/nomenclature/tg263.json` & `pygrpm-0.6.0/pygrpm/tg263/nomenclature/tg263.json`

 * *Files identical despite different names*

### Comparing `pygrpm-0.5.1/pygrpm/tg43/README.md` & `pygrpm-0.6.0/pygrpm/tg43/README.md`

 * *Files identical despite different names*

### Comparing `pygrpm-0.5.1/pygrpm/tg43/data/Flexisource/F.dat` & `pygrpm-0.6.0/pygrpm/tg43/data/Flexisource/F.dat`

 * *Files identical despite different names*

### Comparing `pygrpm-0.5.1/pygrpm/tg43/data/MBDCA/F.dat` & `pygrpm-0.6.0/pygrpm/tg43/data/MBDCA/F.dat`

 * *Files identical despite different names*

### Comparing `pygrpm-0.5.1/pygrpm/tg43/data/MicroSelectronV2/F.dat` & `pygrpm-0.6.0/pygrpm/tg43/data/MicroSelectronV2/F.dat`

 * *Files identical despite different names*

### Comparing `pygrpm-0.5.1/pygrpm/tg43/data/SelectSeed/F.dat` & `pygrpm-0.6.0/pygrpm/tg43/data/SelectSeed/F.dat`

 * *Files identical despite different names*

### Comparing `pygrpm-0.5.1/pygrpm/tg43/seed.py` & `pygrpm-0.6.0/pygrpm/tg43/seed.py`

 * *Files identical despite different names*

### Comparing `pygrpm-0.5.1/pygrpm/uid.py` & `pygrpm-0.6.0/pygrpm/dicom/uid.py`

 * *Files identical despite different names*

### Comparing `pygrpm-0.5.1/pyproject.toml` & `pygrpm-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygrpm"
-version = "0.5.1"
+version = "0.6.0"
 description = "Medical physics library containing many utilty functions"
 readme = "README.md"
 maintainers = ["Yannick Lemaréchal <yannick.lemarechal.1@ulaval.ca>"]
 homepage = "https://paradim.science/"
 repository = "https://git.valeria.science/YALEM10/pygrpm"
 keywords = ["Medical physics", "dicom", "tg43"]
 authors = [
```

### Comparing `pygrpm-0.5.1/PKG-INFO` & `pygrpm-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrpm
-Version: 0.5.1
+Version: 0.6.0
 Summary: Medical physics library containing many utilty functions
 Home-page: https://paradim.science/
 License: AGPL
 Keywords: Medical physics,dicom,tg43
 Author: Pierre-Luc Asselin
 Author-email: pierre-luc.asselin.2@ulaval.ca
 Maintainer: Yannick Lemaréchal
@@ -172,15 +172,15 @@
 
 # Index tracker
 Submodule that allows scrolling through slices of 3-D images using the matplotlib backend.
 
 ```python
 import matplotlib.pyplot as plt
 import numpy
-from pygrpm.index_tracker import IndexTracker
+from pygrpm.visualization.index_tracker import IndexTracker
 
 tracker = IndexTracker(
     *plt.subplot(),
     numpy.random.rand(512, 512, 10),
     ...
 )
 tracker.ax.set_title('My 3-D random image')
@@ -199,15 +199,15 @@
 This method retrieves the desired cross-sections of an element at given energies
 on the NIST website in (barns/electron), barn=10^-24cm^2.
 
 Simple use example:
 
 ```python
 import numpy as np
-from pygrpm.nistparser import get_cross_sections
+from pygrpm.material.nistparser import get_cross_sections
 
 # Define the energies in KeV
 # Numpy array is not mandatory, can be any sequence
 energies = np.linspace(30, 200, 200)
 
 # Prints the returned list
 print(get_cross_sections("H", energies))
@@ -225,16 +225,16 @@
 
 #### get_composition
 This method is used to get and parse material composition from https://physics.nist.gov/cgi-bin/Star/compos.pl
 
 Simple use example:
 
 ```python
-from pygrpm.nistparser import get_composition
-from pygrpm.nistparser.materials_enum import NISTMaterials
+from pygrpm.material.nistparser import get_composition
+from pygrpm.material.nistparser import NISTMaterials
 
 # Prints the returned dictionary
 print(get_composition(NISTMaterials.M3_WAX))
 ```
 Note that get_composition expects the material to be of instance NISTMaterials
 
 ### Acknowledgements
```

