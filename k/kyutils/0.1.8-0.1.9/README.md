# Comparing `tmp/kyutils-0.1.8.tar.gz` & `tmp/kyutils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kyutils-0.1.8.tar", max compression
+gzip compressed data, was "kyutils-0.1.9.tar", max compression
```

## Comparing `kyutils-0.1.8.tar` & `kyutils-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1069 2023-09-11 06:06:00.272770 kyutils-0.1.8/LICENSE
--rw-r--r--   0        0        0      799 2023-09-11 06:06:00.272770 kyutils-0.1.8/README.md
--rw-r--r--   0        0        0      367 2023-09-11 06:06:21.440631 kyutils-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      321 2023-09-11 06:06:00.272770 kyutils-0.1.8/src/kyutils/__init__.py
--rw-r--r--   0        0        0        0 2023-09-11 06:06:00.272770 kyutils-0.1.8/src/kyutils/behavior/__init__.py
--rw-r--r--   0        0        0     1344 2023-09-11 06:06:00.272770 kyutils-0.1.8/src/kyutils/behavior/position.py
--rw-r--r--   0        0        0     3449 2023-09-11 06:06:00.272770 kyutils-0.1.8/src/kyutils/behavior/reward.py
--rw-r--r--   0        0        0        0 2023-09-11 06:06:00.272770 kyutils-0.1.8/src/kyutils/probe/__init__.py
--rw-r--r--   0        0        0     4378 2023-09-11 06:06:00.272770 kyutils-0.1.8/src/kyutils/probe/generate_probe.py
--rw-r--r--   0        0        0        0 2023-09-11 06:06:00.272770 kyutils-0.1.8/src/kyutils/spikegadgets/__init__.py
--rw-r--r--   0        0        0     2717 2023-09-11 06:06:00.272770 kyutils-0.1.8/src/kyutils/spikegadgets/header.py
--rw-r--r--   0        0        0    34162 2023-09-11 06:06:00.272770 kyutils-0.1.8/src/kyutils/spikegadgets/spike_config_15.xml
--rw-r--r--   0        0        0    34168 2023-09-11 06:06:00.272770 kyutils-0.1.8/src/kyutils/spikegadgets/spike_config_20.xml
--rw-r--r--   0        0        0    18909 2023-09-11 06:06:00.272770 kyutils-0.1.8/src/kyutils/spikegadgets/trode_conf_base.xml
--rw-r--r--   0        0        0     8847 2023-09-11 06:06:00.272770 kyutils-0.1.8/src/kyutils/spikegadgets/trodesconf.py
--rw-r--r--   0        0        0     1349 1970-01-01 00:00:00.000000 kyutils-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-09-11 06:20:27.249519 kyutils-0.1.9/LICENSE
+-rw-r--r--   0        0        0      799 2023-09-11 06:20:27.249519 kyutils-0.1.9/README.md
+-rw-r--r--   0        0        0      389 2023-09-11 06:20:57.615234 kyutils-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-09-11 06:20:27.253519 kyutils-0.1.9/src/kyutils/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-11 06:20:27.253519 kyutils-0.1.9/src/kyutils/behavior/__init__.py
+-rw-r--r--   0        0        0     1758 2023-09-11 06:20:27.253519 kyutils-0.1.9/src/kyutils/behavior/position.py
+-rw-r--r--   0        0        0     3449 2023-09-11 06:20:27.253519 kyutils-0.1.9/src/kyutils/behavior/reward.py
+-rw-r--r--   0        0        0        0 2023-09-11 06:20:27.253519 kyutils-0.1.9/src/kyutils/probe/__init__.py
+-rw-r--r--   0        0        0     4378 2023-09-11 06:20:27.253519 kyutils-0.1.9/src/kyutils/probe/generate_probe.py
+-rw-r--r--   0        0        0        0 2023-09-11 06:20:27.253519 kyutils-0.1.9/src/kyutils/spikegadgets/__init__.py
+-rw-r--r--   0        0        0     2717 2023-09-11 06:20:27.253519 kyutils-0.1.9/src/kyutils/spikegadgets/header.py
+-rw-r--r--   0        0        0    34162 2023-09-11 06:20:27.253519 kyutils-0.1.9/src/kyutils/spikegadgets/spike_config_15.xml
+-rw-r--r--   0        0        0    34168 2023-09-11 06:20:27.253519 kyutils-0.1.9/src/kyutils/spikegadgets/spike_config_20.xml
+-rw-r--r--   0        0        0    18909 2023-09-11 06:20:27.253519 kyutils-0.1.9/src/kyutils/spikegadgets/trode_conf_base.xml
+-rw-r--r--   0        0        0     8847 2023-09-11 06:20:27.253519 kyutils-0.1.9/src/kyutils/spikegadgets/trodesconf.py
+-rw-r--r--   0        0        0     1392 1970-01-01 00:00:00.000000 kyutils-0.1.9/PKG-INFO
```

### Comparing `kyutils-0.1.8/LICENSE` & `kyutils-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kyutils-0.1.8/README.md` & `kyutils-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `kyutils-0.1.8/src/kyutils/behavior/position.py` & `kyutils-0.1.9/src/kyutils/behavior/position.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import numpy as np
 from ..spikegadgets.trodesconf import readTrodesExtractedDataFile
+import matplotlib.pyplot as plt
 
 def load_position_from_rec(rec_directory):
 
     online_tracking_file = find_file_with_extension(rec_directory, 'videoPositionTracking')
     online_tracking_timestamps_file = find_file_with_extension(rec_directory, 'videoTimeStamps.cameraHWSync')
 
     position = readTrodesExtractedDataFile(online_tracking_file)
@@ -14,14 +15,26 @@
     position_array[:,0] = position['data']['xloc']
     position_array[:,1] = position['data']['yloc']
     
     position_timestamps_ptp = t_position['data']['HWTimestamp']
     
     return (position_array, position_timestamps_ptp)
 
+def plot_spatial_raster(spike_times, position, t_position, ax=None):
+    if ax is None:
+        fig, ax = plt.subplots()
+        
+    ind = np.searchsorted(t_position, spike_times)
+    ind = ind[ind<len(position)]
+    
+    ax.plot(position[:,0], position[:,1], 'k', alpha=0.1)
+    ax.plot(position[ind,0], position[ind,1], 'r.', markersize=2., alpha=0.7)
+    
+    return (fig, ax)
+
 def find_file_with_extension(directory, extension):
     """
     Searches for a file with a particular extension in a directory and returns its path.
 
     Parameters:
     - directory (str): The directory to search in.
     - extension (str): The extension to look for (e.g., '.txt').
```

### Comparing `kyutils-0.1.8/src/kyutils/behavior/reward.py` & `kyutils-0.1.9/src/kyutils/behavior/reward.py`

 * *Files identical despite different names*

### Comparing `kyutils-0.1.8/src/kyutils/probe/generate_probe.py` & `kyutils-0.1.9/src/kyutils/probe/generate_probe.py`

 * *Files identical despite different names*

### Comparing `kyutils-0.1.8/src/kyutils/spikegadgets/header.py` & `kyutils-0.1.9/src/kyutils/spikegadgets/header.py`

 * *Files identical despite different names*

### Comparing `kyutils-0.1.8/src/kyutils/spikegadgets/spike_config_15.xml` & `kyutils-0.1.9/src/kyutils/spikegadgets/spike_config_15.xml`

 * *Files identical despite different names*

### Comparing `kyutils-0.1.8/src/kyutils/spikegadgets/spike_config_20.xml` & `kyutils-0.1.9/src/kyutils/spikegadgets/spike_config_20.xml`

 * *Files identical despite different names*

### Comparing `kyutils-0.1.8/src/kyutils/spikegadgets/trode_conf_base.xml` & `kyutils-0.1.9/src/kyutils/spikegadgets/trode_conf_base.xml`

 * *Files identical despite different names*

### Comparing `kyutils-0.1.8/src/kyutils/spikegadgets/trodesconf.py` & `kyutils-0.1.9/src/kyutils/spikegadgets/trodesconf.py`

 * *Files identical despite different names*

### Comparing `kyutils-0.1.8/PKG-INFO` & `kyutils-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: kyutils
-Version: 0.1.8
+Version: 0.1.9
 Summary: kyu's utils
 License: MIT
 Author: Kyu Hyun Lee
 Author-email: kyuhyun9056@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
 Requires-Dist: numpy (>=1.25.2,<2.0.0)
 Requires-Dist: probeinterface (>=0.2.17,<0.3.0)
 Requires-Dist: spikeinterface (>=0.98.2,<0.99.0)
 Description-Content-Type: text/markdown
 
 # kyutils
```

