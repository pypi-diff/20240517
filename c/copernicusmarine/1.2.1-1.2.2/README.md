# Comparing `tmp/copernicusmarine-1.2.1.tar.gz` & `tmp/copernicusmarine-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copernicusmarine-1.2.1.tar", max compression
+gzip compressed data, was "copernicusmarine-1.2.2.tar", max compression
```

## Comparing `copernicusmarine-1.2.1.tar` & `copernicusmarine-1.2.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    13827 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/LICENSE.txt
--rw-r--r--   0        0        0    31604 2024-05-13 12:42:07.892682 copernicusmarine-1.2.1/README.md
--rw-r--r--   0        0        0      972 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/__init__.py
--rw-r--r--   0        0        0     1070 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/aioretry/LICENSE
--rw-r--r--   0        0        0      225 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/aioretry/__init__.py
--rw-r--r--   0        0        0     4152 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/aioretry/retry.py
--rw-r--r--   0        0        0       10 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/catalogue_parser/__init__.py
--rw-r--r--   0        0        0    32637 2024-05-09 13:59:27.452291 copernicusmarine-1.2.1/copernicusmarine/catalogue_parser/catalogue_parser.py
--rw-r--r--   0        0        0    11593 2024-05-13 12:42:07.892682 copernicusmarine-1.2.1/copernicusmarine/catalogue_parser/request_structure.py
--rw-r--r--   0        0        0       10 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/command_line_interface/__init__.py
--rw-r--r--   0        0        0      868 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/command_line_interface/copernicus_marine.py
--rw-r--r--   0        0        0     1766 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/command_line_interface/exception_handler.py
--rw-r--r--   0        0        0     4043 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/command_line_interface/group_describe.py
--rw-r--r--   0        0        0     9849 2024-04-30 10:50:17.146536 copernicusmarine-1.2.1/copernicusmarine/command_line_interface/group_get.py
--rw-r--r--   0        0        0     3033 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/command_line_interface/group_login.py
--rw-r--r--   0        0        0    12730 2024-05-13 12:42:07.892682 copernicusmarine-1.2.1/copernicusmarine/command_line_interface/group_subset.py
--rw-r--r--   0        0        0     2339 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/command_line_interface/utils.py
--rw-r--r--   0        0        0    13437 2024-05-09 14:13:11.836107 copernicusmarine-1.2.1/copernicusmarine/core_functions/credentials_utils.py
--rw-r--r--   0        0        0     5312 2024-05-13 12:42:07.892682 copernicusmarine-1.2.1/copernicusmarine/core_functions/custom_zarr_store.py
--rw-r--r--   0        0        0     2806 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/core_functions/deprecated.py
--rw-r--r--   0        0        0     2385 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/core_functions/deprecated_options.py
--rw-r--r--   0        0        0     2174 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/core_functions/describe.py
--rw-r--r--   0        0        0     1233 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/core_functions/environment_variables.py
--rw-r--r--   0        0        0      742 2024-05-08 09:43:19.127282 copernicusmarine-1.2.1/copernicusmarine/core_functions/exceptions.py
--rw-r--r--   0        0        0     8123 2024-04-26 11:41:00.866629 copernicusmarine-1.2.1/copernicusmarine/core_functions/get.py
--rw-r--r--   0        0        0     1606 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/core_functions/login.py
--rw-r--r--   0        0        0      460 2024-05-13 12:42:07.892682 copernicusmarine-1.2.1/copernicusmarine/core_functions/models.py
--rw-r--r--   0        0        0    20227 2024-05-13 12:42:07.892682 copernicusmarine-1.2.1/copernicusmarine/core_functions/services_utils.py
--rw-r--r--   0        0        0     1984 2024-05-13 12:42:07.892682 copernicusmarine-1.2.1/copernicusmarine/core_functions/sessions.py
--rw-r--r--   0        0        0     9735 2024-05-13 12:42:07.892682 copernicusmarine-1.2.1/copernicusmarine/core_functions/subset.py
--rw-r--r--   0        0        0     6536 2024-05-13 12:42:07.892682 copernicusmarine-1.2.1/copernicusmarine/core_functions/utils.py
--rw-r--r--   0        0        0     2688 2024-05-13 12:42:07.892682 copernicusmarine-1.2.1/copernicusmarine/core_functions/versions_verifier.py
--rw-r--r--   0        0        0     2673 2024-05-07 15:20:12.688685 copernicusmarine-1.2.1/copernicusmarine/download_functions/common_download.py
--rw-r--r--   0        0        0     8027 2024-05-13 12:42:07.892682 copernicusmarine-1.2.1/copernicusmarine/download_functions/download_arco_series.py
--rw-r--r--   0        0        0     1706 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/download_functions/download_get.py
--rw-r--r--   0        0        0    20555 2024-05-13 12:42:07.892682 copernicusmarine-1.2.1/copernicusmarine/download_functions/download_original_files.py
--rw-r--r--   0        0        0      918 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/download_functions/subset_parameters.py
--rw-r--r--   0        0        0    19923 2024-05-13 12:59:26.194277 copernicusmarine-1.2.1/copernicusmarine/download_functions/subset_xarray.py
--rw-r--r--   0        0        0     5634 2024-04-30 10:50:17.146536 copernicusmarine-1.2.1/copernicusmarine/download_functions/utils.py
--rw-r--r--   0        0        0      863 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/logging_conf.json
--rw-r--r--   0        0        0     2143 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/python_interface/describe.py
--rw-r--r--   0        0        0      447 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/python_interface/exception_handler.py
--rw-r--r--   0        0        0     5817 2024-04-26 11:29:39.854618 copernicusmarine-1.2.1/copernicusmarine/python_interface/get.py
--rw-r--r--   0        0        0     3545 2024-05-13 12:42:07.896682 copernicusmarine-1.2.1/copernicusmarine/python_interface/load_utils.py
--rw-r--r--   0        0        0     1464 2024-04-30 10:50:17.146536 copernicusmarine-1.2.1/copernicusmarine/python_interface/login.py
--rw-r--r--   0        0        0     6469 2024-05-13 12:42:07.896682 copernicusmarine-1.2.1/copernicusmarine/python_interface/open_dataset.py
--rw-r--r--   0        0        0     6150 2024-05-13 12:42:07.896682 copernicusmarine-1.2.1/copernicusmarine/python_interface/read_dataframe.py
--rw-r--r--   0        0        0     6620 2024-05-13 12:42:07.896682 copernicusmarine-1.2.1/copernicusmarine/python_interface/subset.py
--rw-r--r--   0        0        0      348 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/python_interface/utils.py
--rw-r--r--   0        0        0      901 2024-05-13 12:59:26.194277 copernicusmarine-1.2.1/pyproject.toml
--rw-r--r--   0        0        0    32677 1970-01-01 00:00:00.000000 copernicusmarine-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0    13827 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/LICENSE.txt
+-rw-r--r--   0        0        0    31604 2024-05-15 11:11:24.040466 copernicusmarine-1.2.2/README.md
+-rw-r--r--   0        0        0      972 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/__init__.py
+-rw-r--r--   0        0        0     1070 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/aioretry/LICENSE
+-rw-r--r--   0        0        0      225 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/aioretry/__init__.py
+-rw-r--r--   0        0        0     4152 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/aioretry/retry.py
+-rw-r--r--   0        0        0       10 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/catalogue_parser/__init__.py
+-rw-r--r--   0        0        0    32637 2024-05-16 16:24:36.466506 copernicusmarine-1.2.2/copernicusmarine/catalogue_parser/catalogue_parser.py
+-rw-r--r--   0        0        0    11593 2024-05-16 15:20:15.365969 copernicusmarine-1.2.2/copernicusmarine/catalogue_parser/request_structure.py
+-rw-r--r--   0        0        0       10 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/command_line_interface/__init__.py
+-rw-r--r--   0        0        0      868 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/command_line_interface/copernicus_marine.py
+-rw-r--r--   0        0        0     1766 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/command_line_interface/exception_handler.py
+-rw-r--r--   0        0        0     4043 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/command_line_interface/group_describe.py
+-rw-r--r--   0        0        0     9849 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/command_line_interface/group_get.py
+-rw-r--r--   0        0        0     3033 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/command_line_interface/group_login.py
+-rw-r--r--   0        0        0    12730 2024-05-15 11:11:24.040466 copernicusmarine-1.2.2/copernicusmarine/command_line_interface/group_subset.py
+-rw-r--r--   0        0        0     2339 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/command_line_interface/utils.py
+-rw-r--r--   0        0        0    13437 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/core_functions/credentials_utils.py
+-rw-r--r--   0        0        0     5312 2024-05-15 10:48:16.757693 copernicusmarine-1.2.2/copernicusmarine/core_functions/custom_zarr_store.py
+-rw-r--r--   0        0        0     2806 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/core_functions/deprecated.py
+-rw-r--r--   0        0        0     2385 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/core_functions/deprecated_options.py
+-rw-r--r--   0        0        0     2174 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/core_functions/describe.py
+-rw-r--r--   0        0        0     1233 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/core_functions/environment_variables.py
+-rw-r--r--   0        0        0      742 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/core_functions/exceptions.py
+-rw-r--r--   0        0        0     8123 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/core_functions/get.py
+-rw-r--r--   0        0        0     1606 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/core_functions/login.py
+-rw-r--r--   0        0        0      460 2024-05-15 11:11:24.040466 copernicusmarine-1.2.2/copernicusmarine/core_functions/models.py
+-rw-r--r--   0        0        0    20227 2024-05-16 15:20:15.365969 copernicusmarine-1.2.2/copernicusmarine/core_functions/services_utils.py
+-rw-r--r--   0        0        0     1984 2024-05-15 10:48:16.757693 copernicusmarine-1.2.2/copernicusmarine/core_functions/sessions.py
+-rw-r--r--   0        0        0     9735 2024-05-16 15:20:15.365969 copernicusmarine-1.2.2/copernicusmarine/core_functions/subset.py
+-rw-r--r--   0        0        0     6536 2024-05-15 10:48:16.761693 copernicusmarine-1.2.2/copernicusmarine/core_functions/utils.py
+-rw-r--r--   0        0        0     2688 2024-05-15 10:48:16.761693 copernicusmarine-1.2.2/copernicusmarine/core_functions/versions_verifier.py
+-rw-r--r--   0        0        0     2665 2024-05-16 16:24:36.466506 copernicusmarine-1.2.2/copernicusmarine/download_functions/common_download.py
+-rw-r--r--   0        0        0     8027 2024-05-15 11:11:24.040466 copernicusmarine-1.2.2/copernicusmarine/download_functions/download_arco_series.py
+-rw-r--r--   0        0        0     1706 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/download_functions/download_get.py
+-rw-r--r--   0        0        0    20555 2024-05-15 10:48:16.761693 copernicusmarine-1.2.2/copernicusmarine/download_functions/download_original_files.py
+-rw-r--r--   0        0        0      918 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/download_functions/subset_parameters.py
+-rw-r--r--   0        0        0    19302 2024-05-16 16:24:36.466506 copernicusmarine-1.2.2/copernicusmarine/download_functions/subset_xarray.py
+-rw-r--r--   0        0        0     5634 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/download_functions/utils.py
+-rw-r--r--   0        0        0      863 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/logging_conf.json
+-rw-r--r--   0        0        0     2143 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/python_interface/describe.py
+-rw-r--r--   0        0        0      447 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/python_interface/exception_handler.py
+-rw-r--r--   0        0        0     5817 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/python_interface/get.py
+-rw-r--r--   0        0        0     3545 2024-05-16 15:20:15.369969 copernicusmarine-1.2.2/copernicusmarine/python_interface/load_utils.py
+-rw-r--r--   0        0        0     1464 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/python_interface/login.py
+-rw-r--r--   0        0        0     6469 2024-05-15 11:11:24.040466 copernicusmarine-1.2.2/copernicusmarine/python_interface/open_dataset.py
+-rw-r--r--   0        0        0     6150 2024-05-15 11:11:24.040466 copernicusmarine-1.2.2/copernicusmarine/python_interface/read_dataframe.py
+-rw-r--r--   0        0        0     6620 2024-05-15 11:11:24.040466 copernicusmarine-1.2.2/copernicusmarine/python_interface/subset.py
+-rw-r--r--   0        0        0      348 2024-05-15 09:48:12.382978 copernicusmarine-1.2.2/copernicusmarine/python_interface/utils.py
+-rw-r--r--   0        0        0      901 2024-05-17 06:04:23.143374 copernicusmarine-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0    32677 1970-01-01 00:00:00.000000 copernicusmarine-1.2.2/PKG-INFO
```

### Comparing `copernicusmarine-1.2.1/LICENSE.txt` & `copernicusmarine-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/README.md` & `copernicusmarine-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/__init__.py` & `copernicusmarine-1.2.2/copernicusmarine/__init__.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/aioretry/LICENSE` & `copernicusmarine-1.2.2/copernicusmarine/aioretry/LICENSE`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/aioretry/retry.py` & `copernicusmarine-1.2.2/copernicusmarine/aioretry/retry.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/catalogue_parser/catalogue_parser.py` & `copernicusmarine-1.2.2/copernicusmarine/catalogue_parser/catalogue_parser.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/catalogue_parser/request_structure.py` & `copernicusmarine-1.2.2/copernicusmarine/catalogue_parser/request_structure.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/command_line_interface/copernicus_marine.py` & `copernicusmarine-1.2.2/copernicusmarine/command_line_interface/copernicus_marine.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/command_line_interface/exception_handler.py` & `copernicusmarine-1.2.2/copernicusmarine/command_line_interface/exception_handler.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/command_line_interface/group_describe.py` & `copernicusmarine-1.2.2/copernicusmarine/command_line_interface/group_describe.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/command_line_interface/group_get.py` & `copernicusmarine-1.2.2/copernicusmarine/command_line_interface/group_get.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/command_line_interface/group_login.py` & `copernicusmarine-1.2.2/copernicusmarine/command_line_interface/group_login.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/command_line_interface/group_subset.py` & `copernicusmarine-1.2.2/copernicusmarine/command_line_interface/group_subset.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/command_line_interface/utils.py` & `copernicusmarine-1.2.2/copernicusmarine/command_line_interface/utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/core_functions/credentials_utils.py` & `copernicusmarine-1.2.2/copernicusmarine/core_functions/credentials_utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/core_functions/custom_zarr_store.py` & `copernicusmarine-1.2.2/copernicusmarine/core_functions/custom_zarr_store.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/core_functions/deprecated.py` & `copernicusmarine-1.2.2/copernicusmarine/core_functions/deprecated.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/core_functions/deprecated_options.py` & `copernicusmarine-1.2.2/copernicusmarine/core_functions/deprecated_options.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/core_functions/describe.py` & `copernicusmarine-1.2.2/copernicusmarine/core_functions/describe.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/core_functions/environment_variables.py` & `copernicusmarine-1.2.2/copernicusmarine/core_functions/environment_variables.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/core_functions/exceptions.py` & `copernicusmarine-1.2.2/copernicusmarine/core_functions/exceptions.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/core_functions/get.py` & `copernicusmarine-1.2.2/copernicusmarine/core_functions/get.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/core_functions/login.py` & `copernicusmarine-1.2.2/copernicusmarine/core_functions/login.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/core_functions/services_utils.py` & `copernicusmarine-1.2.2/copernicusmarine/core_functions/services_utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/core_functions/sessions.py` & `copernicusmarine-1.2.2/copernicusmarine/core_functions/sessions.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/core_functions/subset.py` & `copernicusmarine-1.2.2/copernicusmarine/core_functions/subset.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/core_functions/utils.py` & `copernicusmarine-1.2.2/copernicusmarine/core_functions/utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/core_functions/versions_verifier.py` & `copernicusmarine-1.2.2/copernicusmarine/core_functions/versions_verifier.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/download_functions/common_download.py` & `copernicusmarine-1.2.2/copernicusmarine/download_functions/common_download.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import pathlib
-from typing import Any, Optional
+from typing import Optional
 
 import xarray
 import zarr
 from dask.delayed import Delayed
 from tqdm.dask import TqdmCallback
 
 from copernicusmarine.core_functions.exceptions import (
@@ -53,30 +53,32 @@
     dataset: xarray.Dataset,
     output_path: pathlib.Path,
     netcdf_compression_enabled: bool,
     netcdf_compression_level: Optional[int],
     netcdf3_compatible: bool,
 ):
     logger.debug("Writing dataset to NetCDF")
-    encoding: dict[str, Any]
-    encoding = {f"{coord}": {"_FillValue": None} for coord in dataset.coords}
+    for coord in dataset.coords:
+        if "_FillValue" in dataset[coord].encoding:
+            dataset[coord].encoding["_FillValue"] = None
+
     if netcdf_compression_enabled:
         complevel = (
             1 if netcdf_compression_level is None else netcdf_compression_level
         )
         logger.info(f"NetCDF compression enabled with level {complevel}")
         comp = dict(
             zlib=True,
             complevel=complevel,
             contiguous=False,
             shuffle=True,
-            _FillValue=None,
         )
-        encoding_vars = {var: comp for var in dataset.data_vars}
-        encoding.update(encoding_vars)
+        encoding = {var: comp for var in dataset.data_vars}
+    else:
+        encoding = None
 
     xarray_download_format = "NETCDF3_CLASSIC" if netcdf3_compatible else None
     return dataset.to_netcdf(
         output_path,
         mode="w",
         compute=False,
         encoding=encoding,
```

### Comparing `copernicusmarine-1.2.1/copernicusmarine/download_functions/download_arco_series.py` & `copernicusmarine-1.2.2/copernicusmarine/download_functions/download_arco_series.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/download_functions/download_get.py` & `copernicusmarine-1.2.2/copernicusmarine/download_functions/download_get.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/download_functions/download_original_files.py` & `copernicusmarine-1.2.2/copernicusmarine/download_functions/download_original_files.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/download_functions/subset_parameters.py` & `copernicusmarine-1.2.2/copernicusmarine/download_functions/subset_parameters.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/download_functions/subset_xarray.py` & `copernicusmarine-1.2.2/copernicusmarine/download_functions/subset_xarray.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from datetime import datetime
 from decimal import Decimal
 from typing import List, Literal, Optional, Union
 
 import numpy
 import xarray
 from pandas import Timestamp
-from xarray.backends import PydapDataStore
 
 from copernicusmarine.catalogue_parser.catalogue_parser import (
     CopernicusMarineDatasetServiceType,
 )
 from copernicusmarine.catalogue_parser.request_structure import (
     DatasetTimeAndGeographicalSubset,
 )
@@ -19,14 +18,15 @@
 from copernicusmarine.core_functions.exceptions import (
     CoordinatesOutOfDatasetBounds,
     MinimumLongitudeGreaterThanMaximumLongitude,
     VariableDoesNotExistInTheDataset,
 )
 from copernicusmarine.core_functions.models import SubsetMethod
 from copernicusmarine.core_functions.utils import (
+    ServiceNotSupported,
     convert_datetime64_to_netcdf_timestamp,
 )
 from copernicusmarine.download_functions.subset_parameters import (
     DepthParameters,
     GeographicalParameters,
     LatitudeParameters,
     LongitudeParameters,
@@ -39,34 +39,14 @@
     "latitude": ["latitude", "nav_lat", "x", "lat"],
     "longitude": ["longitude", "nav_lon", "y", "lon"],
     "time": ["time_counter", "time"],
     "depth": ["depth", "deptht", "elevation"],
 }
 
 
-def _nearest_neighbor_coordinates(
-    dataset: xarray.Dataset,
-    dimension: str,
-    target_value: Union[float, datetime],
-):
-    if isinstance(target_value, datetime):
-        target_value = numpy.datetime64(target_value)
-    coordinates = dataset[dimension].values
-    index = numpy.searchsorted(coordinates, target_value)
-    index = numpy.clip(index, 0, len(coordinates) - 1)
-    if index > 0 and (
-        index == len(coordinates)
-        or abs(target_value - coordinates[index - 1])
-        < abs(target_value - coordinates[index])
-    ):
-        return coordinates[index - 1]
-    else:
-        return coordinates[index]
-
-
 def _dataset_custom_sel(
     dataset: xarray.Dataset,
     coord_type: Literal["latitude", "longitude", "depth", "time"],
     coord_selection: Union[float, slice, datetime, None],
     method: Union[str, None] = None,
 ) -> xarray.Dataset:
     for coord_label in COORDINATES_LABEL[coord_type]:
@@ -78,17 +58,22 @@
                 coord_label not in tmp_dataset.sizes
             ):
                 target = (
                     coord_selection.start
                     if isinstance(coord_selection, slice)
                     else coord_selection
                 )
-                nearest_neighbor_value = _nearest_neighbor_coordinates(
-                    dataset, coord_label, target
-                )
+                nearest_neighbor_value = dataset.sel(
+                    {coord_label: target}, method="nearest"
+                )[coord_label].values
+                if coord_label == "time":
+                    nanosecond = 1e-9
+                    nearest_neighbor_value = datetime.fromtimestamp(
+                        nearest_neighbor_value.astype(int) * nanosecond
+                    )
                 dataset = dataset.sel(
                     {
                         coord_label: slice(
                             nearest_neighbor_value, nearest_neighbor_value
                         )
                     }
                 )
@@ -414,19 +399,15 @@
         CopernicusMarineDatasetServiceType.STATIC_ARCO,
     ]:
         dataset = sessions.open_zarr(
             dataset_url, copernicus_marine_username=username
         )
         dataset_coordinates = dataset.coords
     else:
-        session = sessions.get_configured_request_session()
-        session.auth = (username, password)
-        store = PydapDataStore.open(dataset_url, session=session, timeout=300)
-        dataset = xarray.open_dataset(store)
-        dataset_coordinates = dataset.coords
+        raise ServiceNotSupported(service_type)
     for coordinate_label in COORDINATES_LABEL["latitude"]:
         if coordinate_label in dataset.sizes:
             latitudes = dataset_coordinates[coordinate_label].values
             user_minimum_coordinate_value = (
                 dataset_subset.minimum_latitude
                 if dataset_subset.minimum_latitude is not None
                 else latitudes.min()
```

### Comparing `copernicusmarine-1.2.1/copernicusmarine/download_functions/utils.py` & `copernicusmarine-1.2.2/copernicusmarine/download_functions/utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/logging_conf.json` & `copernicusmarine-1.2.2/copernicusmarine/logging_conf.json`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/python_interface/describe.py` & `copernicusmarine-1.2.2/copernicusmarine/python_interface/describe.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/python_interface/get.py` & `copernicusmarine-1.2.2/copernicusmarine/python_interface/get.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/python_interface/load_utils.py` & `copernicusmarine-1.2.2/copernicusmarine/python_interface/load_utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/python_interface/login.py` & `copernicusmarine-1.2.2/copernicusmarine/python_interface/login.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/python_interface/open_dataset.py` & `copernicusmarine-1.2.2/copernicusmarine/python_interface/open_dataset.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/python_interface/read_dataframe.py` & `copernicusmarine-1.2.2/copernicusmarine/python_interface/read_dataframe.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/copernicusmarine/python_interface/subset.py` & `copernicusmarine-1.2.2/copernicusmarine/python_interface/subset.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.1/pyproject.toml` & `copernicusmarine-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "copernicusmarine"
-version = "1.2.1"
+version = "1.2.2"
 description = ""
 authors = ["Copernicus Marine User Support <servicedesk.cmems@mercator-ocean.eu>"]
 readme = "README.md"
 packages = [{include = "copernicusmarine"}]
 license = "EUPL-1.2"
 
 [tool.poetry.dependencies]
```

### Comparing `copernicusmarine-1.2.1/PKG-INFO` & `copernicusmarine-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copernicusmarine
-Version: 1.2.1
+Version: 1.2.2
 Summary: 
 License: EUPL-1.2
 Author: Copernicus Marine User Support
 Author-email: servicedesk.cmems@mercator-ocean.eu
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: copernicusmarine Version: 1.2.1 Summary: License:
+Metadata-Version: 2.1 Name: copernicusmarine Version: 1.2.2 Summary: License:
 EUPL-1.2 Author: Copernicus Marine User Support Author-email:
 servicedesk.cmems@mercator-ocean.eu Requires-Python: >=3.9,<3.13 Classifier:
 License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: aiohttp (>=3.9.4) Requires-Dist:
```

