# Comparing `tmp/cesped-24.5.0.tar.gz` & `tmp/cesped-24.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cesped-24.5.0.tar", last modified: Thu May  2 00:12:20 2024, max compression
+gzip compressed data, was "cesped-24.5.2.tar", last modified: Fri May 17 09:53:20 2024, max compression
```

## Comparing `cesped-24.5.0.tar` & `cesped-24.5.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:20.241055 cesped-24.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-02 00:05:43.000000 cesped-24.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-02 00:05:43.000000 cesped-24.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-05-02 00:12:20.241055 cesped-24.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10067 2024-05-02 00:05:43.000000 cesped-24.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:20.233055 cesped-24.5.0/cesped/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:20.233055 cesped-24.5.0/cesped/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/configs/defaultDataAugmentation.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/configs/defaultDataConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/configs/defaultInferenceConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/configs/defaultModelConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/configs/defaultOptimizerConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/configs/defaultRelionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/configs/defaultTrainerConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:20.237055 cesped-24.5.0/cesped/datamanager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/datamanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13527 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/datamanager/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/datamanager/ctf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/datamanager/plDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    22438 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/evaluateEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/inferEntry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:20.237055 cesped-24.5.0/cesped/network/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/network/featureExtractors.py
--rw-r--r--   0 runner    (1001) docker     (127)    24563 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/network/image2sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/network/plModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    28525 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/particlesDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/trainEntry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:20.237055 cesped-24.5.0/cesped/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/utils/angles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/utils/anglesStats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/utils/cliBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/utils/fsc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/utils/gaussianFilters.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/utils/tensors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/utils/volumeStats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:20.237055 cesped-24.5.0/cesped/zenodo/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/zenodo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/zenodo/bechmarkUrls.py
--rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/zenodo/downloadFromZenodo.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/zenodo/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-05-02 00:05:43.000000 cesped-24.5.0/cesped/zenodo/uploadToZenodo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:20.237055 cesped-24.5.0/cesped.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-05-02 00:12:20.000000 cesped-24.5.0/cesped.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-02 00:12:20.000000 cesped-24.5.0/cesped.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 00:12:20.000000 cesped-24.5.0/cesped.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-02 00:12:20.000000 cesped-24.5.0/cesped.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 00:12:20.000000 cesped-24.5.0/cesped.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-02 00:05:43.000000 cesped-24.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 00:12:20.241055 cesped-24.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-02 00:05:43.000000 cesped-24.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:12:20.237055 cesped-24.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:05:43.000000 cesped-24.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-02 00:05:43.000000 cesped-24.5.0/tests/test_anglesStats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-02 00:05:43.000000 cesped-24.5.0/tests/test_particlesDataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:53:20.710270 cesped-24.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-17 09:46:38.000000 cesped-24.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-17 09:46:38.000000 cesped-24.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-05-17 09:53:20.710270 cesped-24.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10067 2024-05-17 09:46:38.000000 cesped-24.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:53:20.702270 cesped-24.5.2/cesped/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:53:20.702270 cesped-24.5.2/cesped/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/configs/defaultDataAugmentation.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/configs/defaultDataConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/configs/defaultInferenceConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/configs/defaultModelConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/configs/defaultOptimizerConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/configs/defaultRelionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/configs/defaultTrainerConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:53:20.702270 cesped-24.5.2/cesped/datamanager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/datamanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13527 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/datamanager/augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/datamanager/ctf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/datamanager/plDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22438 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/evaluateEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/inferEntry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:53:20.706270 cesped-24.5.2/cesped/network/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/network/featureExtractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24563 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/network/image2sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/network/plModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28525 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/particlesDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/trainEntry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:53:20.706270 cesped-24.5.2/cesped/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/utils/angles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/utils/anglesStats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/utils/cliBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/utils/fsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/utils/gaussianFilters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/utils/tensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/utils/volumeStats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:53:20.706270 cesped-24.5.2/cesped/zenodo/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/zenodo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/zenodo/bechmarkUrls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/zenodo/downloadFromZenodo.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/zenodo/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-05-17 09:46:38.000000 cesped-24.5.2/cesped/zenodo/uploadToZenodo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:53:20.706270 cesped-24.5.2/cesped.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-05-17 09:53:20.000000 cesped-24.5.2/cesped.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-17 09:53:20.000000 cesped-24.5.2/cesped.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 09:53:20.000000 cesped-24.5.2/cesped.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-17 09:53:20.000000 cesped-24.5.2/cesped.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-17 09:53:20.000000 cesped-24.5.2/cesped.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-17 09:46:38.000000 cesped-24.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 09:53:20.710270 cesped-24.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-17 09:46:38.000000 cesped-24.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:53:20.706270 cesped-24.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:46:38.000000 cesped-24.5.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-17 09:46:38.000000 cesped-24.5.2/tests/test_anglesStats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-17 09:46:38.000000 cesped-24.5.2/tests/test_particlesDataset.py
```

### Comparing `cesped-24.5.0/LICENSE` & `cesped-24.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/PKG-INFO` & `cesped-24.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesped
-Version: 24.5.0
+Version: 24.5.2
 Summary: Code utilities for the CESPED (Cryo-EM Supervised Pose Estimation Dataset) benchmark
 Home-page: https://github.com/rsanchezgarc/cesped
 Author: Ruben Sanchez-Garcia
 Author-email: ruben.sanchez-garcia@stats.ox.ac.uk
 Keywords: deep learning cryoem pose estimation
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cesped-24.5.0/README.md` & `cesped-24.5.2/README.md`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/cesped/configs/defaultDataAugmentation.yaml` & `cesped-24.5.2/cesped/configs/defaultDataAugmentation.yaml`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/cesped/configs/defaultDataConfig.yaml` & `cesped-24.5.2/cesped/configs/defaultDataConfig.yaml`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/cesped/configs/defaultTrainerConfig.yaml` & `cesped-24.5.2/cesped/configs/defaultTrainerConfig.yaml`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/cesped/constants.py` & `cesped-24.5.2/cesped/constants.py`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/cesped/datamanager/augmentations.py` & `cesped-24.5.2/cesped/datamanager/augmentations.py`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/cesped/datamanager/ctf.py` & `cesped-24.5.2/cesped/datamanager/ctf.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,16 +7,16 @@
               wiener_parameter=0.15):
     '''
     Apply the 2D CTF through a Wiener filter
 
     Input:
         image (Tensor) the DxD image in real space
         sampling_rate: in A/pixel
-        dfu (float or Bx1 tensor): DefocusU (Angstrom)
-        dfv (float or Bx1 tensor): DefocusV (Angstrom)
+        dfu (float or Bx1 tensor): DefocusU (Angstrom). Positive for underfocus
+        dfv (float or Bx1 tensor): DefocusV (Angstrom). Positive for underfocus
         dfang (float or Bx1 tensor): DefocusAngle (degrees)
         volt (float or Bx1 tensor): accelerating voltage (kV)
         cs (float or Bx1 tensor): spherical aberration (mm)
         w (float or Bx1 tensor): amplitude contrast ratio
         phase_shift (float or Bx1 tensor): degrees
         bfactor (float or Bx1 tensor): envelope fcn B-factor (Angstrom^2)
         mode (string): CTF correction: 'phase_flip' or 'wiener'
@@ -43,16 +43,16 @@
 
 def _compute_ctf(freqs, dfu, dfv, dfang, volt, cs, w, phase_shift=0, bfactor=None):
     '''
     Compute the 2D CTF
 
     Input:
         freqs (Tensor) Nx2 or BxNx2 tensor of 2D spatial frequencies
-        dfu (float or Bx1 tensor): DefocusU (Angstrom)
-        dfv (float or Bx1 tensor): DefocusV (Angstrom)
+        dfu (float or Bx1 tensor): DefocusU (Angstrom). Positive for underfocus
+        dfv (float or Bx1 tensor): DefocusV (Angstrom). Positive for underfocus
         dfang (float or Bx1 tensor): DefocusAngle (degrees)
         volt (float or Bx1 tensor): accelerating voltage (kV)
         cs (float or Bx1 tensor): spherical aberration (mm)
         w (float or Bx1 tensor): amplitude contrast ratio
         phase_shift (float or Bx1 tensor): degrees
         bfactor (float or Bx1 tensor): envelope fcn B-factor (Angstrom^2)
     '''
@@ -70,19 +70,19 @@
     ang = torch.atan2(y, x)
     s2 = x ** 2 + y ** 2
     df = .5 * (dfu + dfv + (dfu - dfv) * torch.cos(2 * (ang - dfang)))
     gamma = 2 * torch.pi * (-.5 * df * lam * s2 + .25 * cs * lam ** 3 * s2 ** 2) - phase_shift
     ctf = (1 - w ** 2) ** .5 * torch.sin(gamma) - w * torch.cos(gamma)
     if bfactor is not None:
         ctf *= torch.exp(-bfactor / 4 * s2)
-    return ctf
+    return -ctf
 
 @functools.lru_cache(1)
 def _get2DFreqs(imageSize, sampling_rate, device=None):
     freqs = torch.stack(torch.meshgrid(
         torch.linspace(-.5, .5, imageSize),
         torch.linspace(-.5, .5, imageSize), indexing='ij'), -1)\
             / sampling_rate
     freqs = freqs.reshape(-1,2)
     if device is not None:
         freqs = freqs.to(device)
-    return freqs
+    return freqs
```

### Comparing `cesped-24.5.0/cesped/datamanager/plDataset.py` & `cesped-24.5.2/cesped/datamanager/plDataset.py`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/cesped/evaluateEntry.py` & `cesped-24.5.2/cesped/evaluateEntry.py`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/cesped/inferEntry.py` & `cesped-24.5.2/cesped/inferEntry.py`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/cesped/network/featureExtractors.py` & `cesped-24.5.2/cesped/network/featureExtractors.py`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/cesped/network/image2sphere.py` & `cesped-24.5.2/cesped/network/image2sphere.py`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/cesped/network/plModule.py` & `cesped-24.5.2/cesped/network/plModule.py`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/cesped/particlesDataset.py` & `cesped-24.5.2/cesped/particlesDataset.py`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/cesped/trainEntry.py` & `cesped-24.5.2/cesped/trainEntry.py`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/cesped/utils/angles.py` & `cesped-24.5.2/cesped/utils/angles.py`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/cesped/utils/anglesStats.py` & `cesped-24.5.2/cesped/utils/anglesStats.py`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/cesped/utils/cliBuilder.py` & `cesped-24.5.2/cesped/utils/cliBuilder.py`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/cesped/utils/fsc.py` & `cesped-24.5.2/cesped/utils/fsc.py`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/cesped/utils/gaussianFilters.py` & `cesped-24.5.2/cesped/utils/gaussianFilters.py`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/cesped/utils/tensors.py` & `cesped-24.5.2/cesped/utils/tensors.py`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/cesped/utils/volumeStats.py` & `cesped-24.5.2/cesped/utils/volumeStats.py`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/cesped/zenodo/bechmarkUrls.py` & `cesped-24.5.2/cesped/zenodo/bechmarkUrls.py`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/cesped/zenodo/downloadFromZenodo.py` & `cesped-24.5.2/cesped/zenodo/downloadFromZenodo.py`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/cesped/zenodo/uploadToZenodo.py` & `cesped-24.5.2/cesped/zenodo/uploadToZenodo.py`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/cesped.egg-info/PKG-INFO` & `cesped-24.5.2/cesped.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesped
-Version: 24.5.0
+Version: 24.5.2
 Summary: Code utilities for the CESPED (Cryo-EM Supervised Pose Estimation Dataset) benchmark
 Home-page: https://github.com/rsanchezgarc/cesped
 Author: Ruben Sanchez-Garcia
 Author-email: ruben.sanchez-garcia@stats.ox.ac.uk
 Keywords: deep learning cryoem pose estimation
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cesped-24.5.0/cesped.egg-info/SOURCES.txt` & `cesped-24.5.2/cesped.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/setup.py` & `cesped-24.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/tests/test_anglesStats.py` & `cesped-24.5.2/tests/test_anglesStats.py`

 * *Files identical despite different names*

### Comparing `cesped-24.5.0/tests/test_particlesDataset.py` & `cesped-24.5.2/tests/test_particlesDataset.py`

 * *Files identical despite different names*

