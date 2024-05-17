# Comparing `tmp/pasqal_cloud-0.8.1.tar.gz` & `tmp/pasqal_cloud-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasqal_cloud-0.8.1.tar", last modified: Thu Apr 18 13:51:11 2024, max compression
+gzip compressed data, was "pasqal_cloud-0.9.0.tar", last modified: Fri May 17 12:48:57 2024, max compression
```

## Comparing `pasqal_cloud-0.8.1.tar` & `pasqal_cloud-0.9.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:11.512921 pasqal_cloud-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-04-18 13:51:11.512921 pasqal_cloud-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:11.508921 pasqal_cloud-0.8.1/pasqal_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)    14232 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     8941 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:11.508921 pasqal_cloud-0.8.1/pasqal_cloud/device/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:11.508921 pasqal_cloud-0.8.1/pasqal_cloud/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/device/configuration/base_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/device/configuration/emu_free.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/device/configuration/emu_tn.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/device/configuration/result_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/device/emulator_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/job.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:11.508921 pasqal_cloud-0.8.1/pasqal_cloud/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/utils/jsend.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/utils/strenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pasqal_cloud/workload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:11.512921 pasqal_cloud-0.8.1/pasqal_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-04-18 13:51:11.000000 pasqal_cloud-0.8.1/pasqal_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-18 13:51:11.000000 pasqal_cloud-0.8.1/pasqal_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:51:11.000000 pasqal_cloud-0.8.1/pasqal_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-18 13:51:11.000000 pasqal_cloud-0.8.1/pasqal_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 13:51:11.000000 pasqal_cloud-0.8.1/pasqal_cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:11.508921 pasqal_cloud-0.8.1/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:11.508921 pasqal_cloud-0.8.1/sdk/device/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/sdk/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:11.508921 pasqal_cloud-0.8.1/sdk/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/sdk/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/sdk/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:11.508921 pasqal_cloud-0.8.1/sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-18 13:51:11.512921 pasqal_cloud-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:11.512921 pasqal_cloud-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    23363 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/tests/test_cloud_sdk_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/tests/test_device_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:11.512921 pasqal_cloud-0.8.1/tests/test_doubles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/tests/test_doubles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/tests/test_doubles/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/tests/test_project_renaming_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-04-18 13:51:07.000000 pasqal_cloud-0.8.1/tests/test_workload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:48:57.490764 pasqal_cloud-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-05-17 12:48:57.490764 pasqal_cloud-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:48:57.482763 pasqal_cloud-0.9.0/pasqal_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)    14232 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/pasqal_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/pasqal_cloud/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/pasqal_cloud/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8941 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/pasqal_cloud/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/pasqal_cloud/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:48:57.482763 pasqal_cloud-0.9.0/pasqal_cloud/device/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/pasqal_cloud/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:48:57.486764 pasqal_cloud-0.9.0/pasqal_cloud/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/pasqal_cloud/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/pasqal_cloud/device/configuration/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/pasqal_cloud/device/configuration/emu_free.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/pasqal_cloud/device/configuration/emu_tn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/pasqal_cloud/device/configuration/result_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/pasqal_cloud/device/emulator_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/pasqal_cloud/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/pasqal_cloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/pasqal_cloud/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/pasqal_cloud/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:48:57.486764 pasqal_cloud-0.9.0/pasqal_cloud/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/pasqal_cloud/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/pasqal_cloud/utils/jsend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/pasqal_cloud/utils/strenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/pasqal_cloud/workload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:48:57.490764 pasqal_cloud-0.9.0/pasqal_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-05-17 12:48:57.000000 pasqal_cloud-0.9.0/pasqal_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-17 12:48:57.000000 pasqal_cloud-0.9.0/pasqal_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 12:48:57.000000 pasqal_cloud-0.9.0/pasqal_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-17 12:48:57.000000 pasqal_cloud-0.9.0/pasqal_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-17 12:48:57.000000 pasqal_cloud-0.9.0/pasqal_cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:48:57.486764 pasqal_cloud-0.9.0/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:48:57.486764 pasqal_cloud-0.9.0/sdk/device/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/sdk/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:48:57.486764 pasqal_cloud-0.9.0/sdk/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/sdk/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/sdk/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:48:57.486764 pasqal_cloud-0.9.0/sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-17 12:48:57.490764 pasqal_cloud-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:48:57.490764 pasqal_cloud-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23363 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/tests/test_cloud_sdk_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/tests/test_device_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:48:57.490764 pasqal_cloud-0.9.0/tests/test_doubles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/tests/test_doubles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/tests/test_doubles/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/tests/test_project_renaming_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-05-17 12:48:50.000000 pasqal_cloud-0.9.0/tests/test_workload.py
```

### Comparing `pasqal_cloud-0.8.1/LICENSE` & `pasqal_cloud-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.1/PKG-INFO` & `pasqal_cloud-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasqal-cloud
-Version: 0.8.1
+Version: 0.9.0
 Summary: Software development kit for Pasqal cloud platform.
 Home-page: https://github.com/pasqal-io/pasqal-cloud
 Maintainer: Pasqal Cloud Services
 Maintainer-email: pcs@pasqal.io
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -12,21 +12,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: auth0-python<4.0.0,>=3.23.1
 Requires-Dist: requests<3.0.0,>=2.25.1
 Requires-Dist: pyjwt[crypto]<3.0.0,>=2.5.0
 Requires-Dist: pydantic<3.0.0,>=2.6.0
 Provides-Extra: dev
-Requires-Dist: types-requests==2.31.0.1; extra == "dev"
-Requires-Dist: requests-mock==1.11.0; extra == "dev"
 Requires-Dist: pytest-cov==4.1.0; extra == "dev"
+Requires-Dist: pytest==7.4.0; extra == "dev"
 Requires-Dist: mypy==1.9.0; extra == "dev"
+Requires-Dist: types-requests==2.31.0.1; extra == "dev"
 Requires-Dist: flake8==6.0.0; extra == "dev"
-Requires-Dist: pytest==7.4.0; extra == "dev"
 Requires-Dist: black==23.3.0; extra == "dev"
+Requires-Dist: requests-mock==1.11.0; extra == "dev"
 Requires-Dist: isort==5.12.0; extra == "dev"
 
 # PASQAL Cloud
 
 SDK to be used to access Pasqal Cloud Services.
 
 ## Installation
```

### Comparing `pasqal_cloud-0.8.1/README.md` & `pasqal_cloud-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.1/pasqal_cloud/__init__.py` & `pasqal_cloud-0.9.0/pasqal_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.1/pasqal_cloud/_version.py` & `pasqal_cloud-0.9.0/pasqal_cloud/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = "0.8.1"
+__version__ = "0.9.0"
```

### Comparing `pasqal_cloud-0.8.1/pasqal_cloud/authentication.py` & `pasqal_cloud-0.9.0/pasqal_cloud/authentication.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.1/pasqal_cloud/batch.py` & `pasqal_cloud-0.9.0/pasqal_cloud/batch.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.1/pasqal_cloud/client.py` & `pasqal_cloud-0.9.0/pasqal_cloud/client.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.1/pasqal_cloud/device/configuration/base_config.py` & `pasqal_cloud-0.9.0/pasqal_cloud/device/configuration/base_config.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.1/pasqal_cloud/device/configuration/emu_tn.py` & `pasqal_cloud-0.9.0/pasqal_cloud/device/configuration/emu_tn.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.1/pasqal_cloud/endpoints.py` & `pasqal_cloud-0.9.0/pasqal_cloud/endpoints.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,23 +34,23 @@
 class Endpoints:
     core: str = CORE_API_URL
 
 
 # ---- Auth0 ----
 
 # Prod Auth0 configuration
-AUTH0_DOMAIN: Final[str] = "pasqal.eu.auth0.com"
+AUTH0_DOMAIN: Final[str] = "authenticate.pasqal.cloud"
 PUBLIC_CLIENT_ID: Final[str] = "PeZvo7Atx7IVv3iel59asJSb4Ig7vuSB"
 AUDIENCE: Final[str] = "https://apis.pasqal.cloud/account/api/v1"
 
-PREPROD_AUTH0_DOMAIN: Final[str] = "pasqal-preprod.eu.auth0.com"
+PREPROD_AUTH0_DOMAIN: Final[str] = "authenticate.preprod.pasqal.cloud"
 PREPROD_PUBLIC_CLIENT_ID: Final[str] = "2l6A2ldvwJE5sdkghu40BTYLm7sSUAv9"
 PREPROD_AUDIENCE: Final[str] = "https://apis.preprod.pasqal.cloud/account/api/v1"
 
-DEV_AUTH0_DOMAIN: Final[str] = "pasqal-dev.eu.auth0.com"
+DEV_AUTH0_DOMAIN: Final[str] = "authenticate.dev.pasqal.cloud"
 DEV_PUBLIC_CLIENT_ID: Final[str] = "5QtfSu1UV118Iz6By6IJRSNoDrLbAiOv"
 DEV_AUDIENCE: Final[str] = "https://apis.dev.pasqal.cloud/account/api/v1"
 
 REALM: Final[str] = "pcs-users"
 
 
 @dataclass
```

### Comparing `pasqal_cloud-0.8.1/pasqal_cloud/errors.py` & `pasqal_cloud-0.9.0/pasqal_cloud/errors.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.1/pasqal_cloud/job.py` & `pasqal_cloud-0.9.0/pasqal_cloud/job.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.1/pasqal_cloud/utils/jsend.py` & `pasqal_cloud-0.9.0/pasqal_cloud/utils/jsend.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.1/pasqal_cloud/workload.py` & `pasqal_cloud-0.9.0/pasqal_cloud/workload.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.1/pasqal_cloud.egg-info/PKG-INFO` & `pasqal_cloud-0.9.0/pasqal_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasqal-cloud
-Version: 0.8.1
+Version: 0.9.0
 Summary: Software development kit for Pasqal cloud platform.
 Home-page: https://github.com/pasqal-io/pasqal-cloud
 Maintainer: Pasqal Cloud Services
 Maintainer-email: pcs@pasqal.io
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -12,21 +12,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: auth0-python<4.0.0,>=3.23.1
 Requires-Dist: requests<3.0.0,>=2.25.1
 Requires-Dist: pyjwt[crypto]<3.0.0,>=2.5.0
 Requires-Dist: pydantic<3.0.0,>=2.6.0
 Provides-Extra: dev
-Requires-Dist: types-requests==2.31.0.1; extra == "dev"
-Requires-Dist: requests-mock==1.11.0; extra == "dev"
 Requires-Dist: pytest-cov==4.1.0; extra == "dev"
+Requires-Dist: pytest==7.4.0; extra == "dev"
 Requires-Dist: mypy==1.9.0; extra == "dev"
+Requires-Dist: types-requests==2.31.0.1; extra == "dev"
 Requires-Dist: flake8==6.0.0; extra == "dev"
-Requires-Dist: pytest==7.4.0; extra == "dev"
 Requires-Dist: black==23.3.0; extra == "dev"
+Requires-Dist: requests-mock==1.11.0; extra == "dev"
 Requires-Dist: isort==5.12.0; extra == "dev"
 
 # PASQAL Cloud
 
 SDK to be used to access Pasqal Cloud Services.
 
 ## Installation
```

### Comparing `pasqal_cloud-0.8.1/pasqal_cloud.egg-info/SOURCES.txt` & `pasqal_cloud-0.9.0/pasqal_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.1/sdk/setup.py` & `pasqal_cloud-0.9.0/sdk/setup.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.1/setup.py` & `pasqal_cloud-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.1/tests/conftest.py` & `pasqal_cloud-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.1/tests/test_batch.py` & `pasqal_cloud-0.9.0/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.1/tests/test_client.py` & `pasqal_cloud-0.9.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.1/tests/test_cloud_sdk_import.py` & `pasqal_cloud-0.9.0/tests/test_cloud_sdk_import.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.1/tests/test_config.py` & `pasqal_cloud-0.9.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.1/tests/test_device_specs.py` & `pasqal_cloud-0.9.0/tests/test_device_specs.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.1/tests/test_doubles/authentication.py` & `pasqal_cloud-0.9.0/tests/test_doubles/authentication.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.1/tests/test_errors.py` & `pasqal_cloud-0.9.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.1/tests/test_job.py` & `pasqal_cloud-0.9.0/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.1/tests/test_project_renaming_compatibility.py` & `pasqal_cloud-0.9.0/tests/test_project_renaming_compatibility.py`

 * *Files identical despite different names*

### Comparing `pasqal_cloud-0.8.1/tests/test_workload.py` & `pasqal_cloud-0.9.0/tests/test_workload.py`

 * *Files identical despite different names*

