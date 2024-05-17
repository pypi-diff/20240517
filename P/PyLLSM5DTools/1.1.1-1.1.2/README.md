# Comparing `tmp/pyllsm5dtools-1.1.1.tar.gz` & `tmp/pyllsm5dtools-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllsm5dtools-1.1.1.tar", last modified: Thu May 16 05:35:00 2024, max compression
+gzip compressed data, was "pyllsm5dtools-1.1.2.tar", last modified: Fri May 17 21:49:10 2024, max compression
```

## Comparing `pyllsm5dtools-1.1.1.tar` & `pyllsm5dtools-1.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-16 05:35:00.584469 pyllsm5dtools-1.1.1/
--rw-rw-r--   0 matt      (1000) matt      (1000)      819 2024-03-05 21:34:03.000000 pyllsm5dtools-1.1.1/LICENSE.txt
--rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-05-16 05:35:00.584469 pyllsm5dtools-1.1.1/PKG-INFO
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-16 05:35:00.580469 pyllsm5dtools-1.1.1/PyLLSM5DTools/
--rw-rw-r--   0 matt      (1000) matt      (1000)     3645 2024-05-15 21:33:07.000000 pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_FSC_analysis_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3038 2024-05-15 21:33:07.000000 pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_MIP_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3199 2024-05-15 21:33:07.000000 pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_crop_dataset.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     5155 2024-05-15 21:33:07.000000 pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_decon_data_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     5055 2024-05-15 21:33:07.000000 pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3155 2024-05-15 21:33:07.000000 pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     6203 2024-05-15 21:33:07.000000 pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_matlab_stitching_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     6089 2024-05-15 21:33:07.000000 pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3340 2024-05-15 21:33:07.000000 pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_psf_analysis_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3136 2024-05-15 21:33:07.000000 pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3351 2024-05-15 21:33:07.000000 pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_resample_dataset.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3463 2024-05-15 21:33:07.000000 pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_tiffToZarr_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2143 2024-05-15 21:33:07.000000 pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2772 2024-05-15 21:33:07.000000 pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_zarrToTiff_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      957 2024-05-15 21:33:07.000000 pyllsm5dtools-1.1.1/PyLLSM5DTools/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     9176 2024-05-15 21:32:51.000000 pyllsm5dtools-1.1.1/PyLLSM5DTools/generatePythonWrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1122 2024-03-27 21:30:52.000000 pyllsm5dtools-1.1.1/PyLLSM5DTools/generate_config_file.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-16 05:35:00.584469 pyllsm5dtools-1.1.1/PyLLSM5DTools.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-05-16 05:35:00.000000 pyllsm5dtools-1.1.1/PyLLSM5DTools.egg-info/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)      879 2024-05-16 05:35:00.000000 pyllsm5dtools-1.1.1/PyLLSM5DTools.egg-info/SOURCES.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-05-16 05:35:00.000000 pyllsm5dtools-1.1.1/PyLLSM5DTools.egg-info/dependency_links.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       14 2024-05-16 05:35:00.000000 pyllsm5dtools-1.1.1/PyLLSM5DTools.egg-info/top_level.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)     1206 2024-03-27 20:42:06.000000 pyllsm5dtools-1.1.1/README.md
--rw-rw-r--   0 matt      (1000) matt      (1000)       38 2024-05-16 05:35:00.584469 pyllsm5dtools-1.1.1/setup.cfg
--rw-rw-r--   0 matt      (1000) matt      (1000)     3635 2024-05-16 05:32:47.000000 pyllsm5dtools-1.1.1/setup.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-17 21:49:10.980253 pyllsm5dtools-1.1.2/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      819 2024-03-05 21:34:03.000000 pyllsm5dtools-1.1.2/LICENSE.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-05-17 21:49:10.980253 pyllsm5dtools-1.1.2/PKG-INFO
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-17 21:49:10.976253 pyllsm5dtools-1.1.2/PyLLSM5DTools/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3645 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_FSC_analysis_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3038 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_MIP_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3199 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_crop_dataset.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5155 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_decon_data_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5055 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3155 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6203 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_matlab_stitching_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6089 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3340 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_psf_analysis_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3144 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3351 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_resample_dataset.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3463 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_tiffToZarr_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2143 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2772 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_zarrToTiff_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      957 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     9176 2024-05-15 21:32:51.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/generatePythonWrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1122 2024-03-27 21:30:52.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/generate_config_file.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-17 21:49:10.980253 pyllsm5dtools-1.1.2/PyLLSM5DTools.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-05-17 21:49:10.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools.egg-info/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)      879 2024-05-17 21:49:10.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools.egg-info/SOURCES.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-05-17 21:49:10.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools.egg-info/dependency_links.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       14 2024-05-17 21:49:10.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools.egg-info/top_level.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1206 2024-03-27 20:42:06.000000 pyllsm5dtools-1.1.2/README.md
+-rw-rw-r--   0 matt      (1000) matt      (1000)       38 2024-05-17 21:49:10.980253 pyllsm5dtools-1.1.2/setup.cfg
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3635 2024-05-17 21:46:11.000000 pyllsm5dtools-1.1.2/setup.py
```

### Comparing `pyllsm5dtools-1.1.1/LICENSE.txt` & `pyllsm5dtools-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_FSC_analysis_wrapper.py` & `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_FSC_analysis_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_MIP_wrapper.py` & `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_MIP_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_crop_dataset.py` & `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_crop_dataset.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_decon_data_wrapper.py` & `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_decon_data_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py` & `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py` & `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_matlab_stitching_wrapper.py` & `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_matlab_stitching_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py` & `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_psf_analysis_wrapper.py` & `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_psf_analysis_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py` & `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 def XR_psf_detection_and_analysis_wrapper(dataPaths, **kwargs):
     function_name = "XR_psf_detection_and_analysis_wrapper"
     XR_psf_detection_and_analysis_wrapper_dict = {
         "xyPixelSize": [kwargs.get("xyPixelSize", 0.108), "numericScalar"],
         "dz": [kwargs.get("dz", 0.1), "numericScalar"],
-        "angle": [kwargs.get("angle", 32.45), "numericScalar"],
+        "skewAngle": [kwargs.get("skewAngle", 32.45), "numericScalar"],
         "cropSize": [kwargs.get("cropSize", [256,128,201]), "numericArr"],
         "flipZstack": [kwargs.get("flipZstack", False), "logical"],
         "distThresh": [kwargs.get("distThresh", [256,128,201]), "numericArr"],
         "channelPatterns": [kwargs.get("channelPatterns", ['CamA_ch0','CamB_ch0']), "cell"],
         "channels": [kwargs.get("channels", [488,560]), "numericArr"],
         "RWFn": [kwargs.get("RWFn", ['/clusterfs/fiona/Gokul/RW_PSFs/PSF_RW_515em_128_128_101_100nmSteps.tif','/clusterfs/fiona/Gokul/RW_PSFs/PSF_RW_605em_128_128_101_100nmSteps.tif']), "cell"],
         "sourceStr": [kwargs.get("sourceStr", "test"), "char"],
```

### Comparing `pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_resample_dataset.py` & `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_resample_dataset.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_tiffToZarr_wrapper.py` & `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_tiffToZarr_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py` & `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.1/PyLLSM5DTools/XR_zarrToTiff_wrapper.py` & `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_zarrToTiff_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.1/PyLLSM5DTools/__init__.py` & `pyllsm5dtools-1.1.2/PyLLSM5DTools/__init__.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.1/PyLLSM5DTools/generatePythonWrapper.py` & `pyllsm5dtools-1.1.2/PyLLSM5DTools/generatePythonWrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.1/PyLLSM5DTools/generate_config_file.py` & `pyllsm5dtools-1.1.2/PyLLSM5DTools/generate_config_file.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.1/PyLLSM5DTools.egg-info/SOURCES.txt` & `pyllsm5dtools-1.1.2/PyLLSM5DTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.1/README.md` & `pyllsm5dtools-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.1/setup.py` & `pyllsm5dtools-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
 matlab_runtime_url = ("https://ssd.mathworks.com/supportfiles/downloads/R2023a/Release/6/deployment_files"
                       "/installer/complete/glnxa64/MATLAB_Runtime_R2023a_Update_6_glnxa64.zip")
 name = 'PyLLSM5DTools'
-version = '1.1.1'
+version = '1.1.2'
 
 
 class CustomInstall(install):
     def download_and_extract_matlab_runtime(self, install_dir):
         llsm5dtools_url = "https://github.com/abcucberkeley/LLSM5DTools/archive/refs/heads/main.zip"
         llsm5dtools_github_dir = os.path.join(install_dir, "LLSM5DTools-main")
         llsm5dtools_dir = os.path.join(install_dir, "LLSM5DTools")
```

