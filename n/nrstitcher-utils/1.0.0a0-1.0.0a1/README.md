# Comparing `tmp/nrstitcher_utils-1.0.0a0.tar.gz` & `tmp/nrstitcher_utils-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrstitcher_utils-1.0.0a0.tar", last modified: Thu May 16 09:29:15 2024, max compression
+gzip compressed data, was "nrstitcher_utils-1.0.0a1.tar", last modified: Fri May 17 08:54:04 2024, max compression
```

## Comparing `nrstitcher_utils-1.0.0a0.tar` & `nrstitcher_utils-1.0.0a1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-05-16 09:29:15.867238 nrstitcher_utils-1.0.0a0/
--rw-r--r--   0 payno     (1000) payno     (1000)     1241 2024-05-16 07:38:25.000000 nrstitcher_utils-1.0.0a0/LICENSE
--rw-r--r--   0 payno     (1000) payno     (1000)     3770 2024-05-16 09:29:15.867238 nrstitcher_utils-1.0.0a0/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)      411 2024-05-16 07:38:25.000000 nrstitcher_utils-1.0.0a0/README.md
--rw-r--r--   0 payno     (1000) payno     (1000)     2179 2024-05-16 07:38:25.000000 nrstitcher_utils-1.0.0a0/pyproject.toml
--rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-05-16 09:29:15.867238 nrstitcher_utils-1.0.0a0/setup.cfg
--rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-05-16 07:38:25.000000 nrstitcher_utils-1.0.0a0/setup.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-05-16 09:29:15.863238 nrstitcher_utils-1.0.0a0/src/
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-05-16 09:29:15.863238 nrstitcher_utils-1.0.0a0/src/nrstitcher_utils/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-05-16 07:38:25.000000 nrstitcher_utils-1.0.0a0/src/nrstitcher_utils/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-05-16 09:29:15.867238 nrstitcher_utils-1.0.0a0/src/nrstitcher_utils/app/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-05-16 07:38:25.000000 nrstitcher_utils-1.0.0a0/src/nrstitcher_utils/app/__init__.py
--rwxr-xr-x   0 payno     (1000) payno     (1000)     8527 2024-05-16 07:38:25.000000 nrstitcher_utils-1.0.0a0/src/nrstitcher_utils/app/nrs_config_id16a_ht.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-05-16 09:29:15.867238 nrstitcher_utils-1.0.0a0/src/nrstitcher_utils/core/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-05-16 07:38:25.000000 nrstitcher_utils-1.0.0a0/src/nrstitcher_utils/core/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3144 2024-05-16 07:38:25.000000 nrstitcher_utils-1.0.0a0/src/nrstitcher_utils/core/h5_settings.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8310 2024-05-16 07:38:25.000000 nrstitcher_utils-1.0.0a0/src/nrstitcher_utils/core/ht_vol.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3460 2024-05-16 07:38:25.000000 nrstitcher_utils-1.0.0a0/src/nrstitcher_utils/core/utils.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-05-16 09:29:15.867238 nrstitcher_utils-1.0.0a0/src/nrstitcher_utils/resources/
--rw-r--r--   0 payno     (1000) payno     (1000)      282 2024-05-16 07:38:25.000000 nrstitcher_utils-1.0.0a0/src/nrstitcher_utils/resources/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-05-16 09:29:15.867238 nrstitcher_utils-1.0.0a0/src/nrstitcher_utils/resources/config_files/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-05-16 07:38:25.000000 nrstitcher_utils-1.0.0a0/src/nrstitcher_utils/resources/config_files/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3660 2024-05-16 07:38:25.000000 nrstitcher_utils-1.0.0a0/src/nrstitcher_utils/resources/config_files/slurm_config_id16a.txt
--rw-r--r--   0 payno     (1000) payno     (1000)       43 2024-05-16 09:28:17.000000 nrstitcher_utils-1.0.0a0/src/nrstitcher_utils/version.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-05-16 09:29:15.867238 nrstitcher_utils-1.0.0a0/src/nrstitcher_utils.egg-info/
--rw-r--r--   0 payno     (1000) payno     (1000)     3770 2024-05-16 09:29:15.000000 nrstitcher_utils-1.0.0a0/src/nrstitcher_utils.egg-info/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)      773 2024-05-16 09:29:15.000000 nrstitcher_utils-1.0.0a0/src/nrstitcher_utils.egg-info/SOURCES.txt
--rw-r--r--   0 payno     (1000) payno     (1000)        1 2024-05-16 09:29:15.000000 nrstitcher_utils-1.0.0a0/src/nrstitcher_utils.egg-info/dependency_links.txt
--rw-r--r--   0 payno     (1000) payno     (1000)       86 2024-05-16 09:29:15.000000 nrstitcher_utils-1.0.0a0/src/nrstitcher_utils.egg-info/entry_points.txt
--rw-r--r--   0 payno     (1000) payno     (1000)      138 2024-05-16 09:29:15.000000 nrstitcher_utils-1.0.0a0/src/nrstitcher_utils.egg-info/requires.txt
--rw-r--r--   0 payno     (1000) payno     (1000)       17 2024-05-16 09:29:15.000000 nrstitcher_utils-1.0.0a0/src/nrstitcher_utils.egg-info/top_level.txt
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-05-17 08:54:04.419379 nrstitcher_utils-1.0.0a1/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1241 2024-04-26 11:40:31.000000 nrstitcher_utils-1.0.0a1/LICENSE
+-rw-r--r--   0 payno     (1000) payno     (1000)     3770 2024-05-17 08:54:04.419379 nrstitcher_utils-1.0.0a1/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)      411 2024-05-15 07:05:10.000000 nrstitcher_utils-1.0.0a1/README.md
+-rw-r--r--   0 payno     (1000) payno     (1000)     2245 2024-05-17 08:23:20.000000 nrstitcher_utils-1.0.0a1/pyproject.toml
+-rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-05-17 08:54:04.419379 nrstitcher_utils-1.0.0a1/setup.cfg
+-rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-04-26 11:40:31.000000 nrstitcher_utils-1.0.0a1/setup.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-05-17 08:54:04.415379 nrstitcher_utils-1.0.0a1/src/
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-05-17 08:54:04.415379 nrstitcher_utils-1.0.0a1/src/nrstitcher_utils/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-26 11:40:31.000000 nrstitcher_utils-1.0.0a1/src/nrstitcher_utils/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-05-17 08:54:04.415379 nrstitcher_utils-1.0.0a1/src/nrstitcher_utils/app/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-26 11:40:31.000000 nrstitcher_utils-1.0.0a1/src/nrstitcher_utils/app/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2261 2024-05-17 08:30:07.000000 nrstitcher_utils-1.0.0a1/src/nrstitcher_utils/app/nrs_clean_scories.py
+-rwxr-xr-x   0 payno     (1000) payno     (1000)     8527 2024-05-15 07:05:10.000000 nrstitcher_utils-1.0.0a1/src/nrstitcher_utils/app/nrs_config_id16a_ht.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-05-17 08:54:04.415379 nrstitcher_utils-1.0.0a1/src/nrstitcher_utils/core/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-26 11:40:31.000000 nrstitcher_utils-1.0.0a1/src/nrstitcher_utils/core/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3144 2024-05-15 07:05:10.000000 nrstitcher_utils-1.0.0a1/src/nrstitcher_utils/core/h5_settings.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8310 2024-05-15 07:05:10.000000 nrstitcher_utils-1.0.0a1/src/nrstitcher_utils/core/ht_vol.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3460 2024-05-15 07:05:10.000000 nrstitcher_utils-1.0.0a1/src/nrstitcher_utils/core/utils.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-05-17 08:54:04.415379 nrstitcher_utils-1.0.0a1/src/nrstitcher_utils/resources/
+-rw-r--r--   0 payno     (1000) payno     (1000)      282 2024-04-26 11:40:31.000000 nrstitcher_utils-1.0.0a1/src/nrstitcher_utils/resources/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-05-17 08:54:04.419379 nrstitcher_utils-1.0.0a1/src/nrstitcher_utils/resources/config_files/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-26 11:40:31.000000 nrstitcher_utils-1.0.0a1/src/nrstitcher_utils/resources/config_files/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3660 2024-05-15 11:49:19.000000 nrstitcher_utils-1.0.0a1/src/nrstitcher_utils/resources/config_files/slurm_config_id16a.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       43 2024-05-17 08:51:27.000000 nrstitcher_utils-1.0.0a1/src/nrstitcher_utils/version.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-05-17 08:54:04.419379 nrstitcher_utils-1.0.0a1/src/nrstitcher_utils.egg-info/
+-rw-r--r--   0 payno     (1000) payno     (1000)     3770 2024-05-17 08:54:04.000000 nrstitcher_utils-1.0.0a1/src/nrstitcher_utils.egg-info/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)      819 2024-05-17 08:54:04.000000 nrstitcher_utils-1.0.0a1/src/nrstitcher_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)        1 2024-05-17 08:54:04.000000 nrstitcher_utils-1.0.0a1/src/nrstitcher_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)      150 2024-05-17 08:54:04.000000 nrstitcher_utils-1.0.0a1/src/nrstitcher_utils.egg-info/entry_points.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)      138 2024-05-17 08:54:04.000000 nrstitcher_utils-1.0.0a1/src/nrstitcher_utils.egg-info/requires.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       17 2024-05-17 08:54:04.000000 nrstitcher_utils-1.0.0a1/src/nrstitcher_utils.egg-info/top_level.txt
```

### Comparing `nrstitcher_utils-1.0.0a0/LICENSE` & `nrstitcher_utils-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `nrstitcher_utils-1.0.0a0/PKG-INFO` & `nrstitcher_utils-1.0.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrstitcher_utils
-Version: 1.0.0a0
+Version: 1.0.0a1
 Summary: NRStitcher utils for esrf usage
 Author: Arttu Miettenen, Yervand Azatian
 Author-email: Jayde Livingstone <jayde.livingstone@gmail.com>, Henri Payno <henri.payno@esrf.fr>
 License: The nrstitcher_utils library goal is to ease usage of nrstitcher at esrf
         
         nrstitcher_utils is distributed under the MIT license.
```

### Comparing `nrstitcher_utils-1.0.0a0/pyproject.toml` & `nrstitcher_utils-1.0.0a1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     "pandoc",
     "sphinx_autodoc_typehints",
     "pydata_sphinx_theme",
 ]
 
 [project.scripts]
 nrs-config-id16a-ht = "nrstitcher_utils.app.nrs_config_id16a_ht:main"
+nrs-clean-scories = "nrstitcher_utils.app.nrs_clean_scories:main"
 
 [build_sphinx]
 source_dir = "doc"
 build_dir = "build/sphinx"
 
 [tool.setuptools.dynamic]
 version = {attr = "nrstitcher_utils.version.version"}
```

### Comparing `nrstitcher_utils-1.0.0a0/src/nrstitcher_utils/app/nrs_config_id16a_ht.py` & `nrstitcher_utils-1.0.0a1/src/nrstitcher_utils/app/nrs_config_id16a_ht.py`

 * *Files identical despite different names*

### Comparing `nrstitcher_utils-1.0.0a0/src/nrstitcher_utils/core/h5_settings.py` & `nrstitcher_utils-1.0.0a1/src/nrstitcher_utils/core/h5_settings.py`

 * *Files identical despite different names*

### Comparing `nrstitcher_utils-1.0.0a0/src/nrstitcher_utils/core/ht_vol.py` & `nrstitcher_utils-1.0.0a1/src/nrstitcher_utils/core/ht_vol.py`

 * *Files identical despite different names*

### Comparing `nrstitcher_utils-1.0.0a0/src/nrstitcher_utils/core/utils.py` & `nrstitcher_utils-1.0.0a1/src/nrstitcher_utils/core/utils.py`

 * *Files identical despite different names*

### Comparing `nrstitcher_utils-1.0.0a0/src/nrstitcher_utils/resources/config_files/slurm_config_id16a.txt` & `nrstitcher_utils-1.0.0a1/src/nrstitcher_utils/resources/config_files/slurm_config_id16a.txt`

 * *Files identical despite different names*

### Comparing `nrstitcher_utils-1.0.0a0/src/nrstitcher_utils.egg-info/PKG-INFO` & `nrstitcher_utils-1.0.0a1/src/nrstitcher_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrstitcher_utils
-Version: 1.0.0a0
+Version: 1.0.0a1
 Summary: NRStitcher utils for esrf usage
 Author: Arttu Miettenen, Yervand Azatian
 Author-email: Jayde Livingstone <jayde.livingstone@gmail.com>, Henri Payno <henri.payno@esrf.fr>
 License: The nrstitcher_utils library goal is to ease usage of nrstitcher at esrf
         
         nrstitcher_utils is distributed under the MIT license.
```

### Comparing `nrstitcher_utils-1.0.0a0/src/nrstitcher_utils.egg-info/SOURCES.txt` & `nrstitcher_utils-1.0.0a1/src/nrstitcher_utils.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/nrstitcher_utils.egg-info/PKG-INFO
 src/nrstitcher_utils.egg-info/SOURCES.txt
 src/nrstitcher_utils.egg-info/dependency_links.txt
 src/nrstitcher_utils.egg-info/entry_points.txt
 src/nrstitcher_utils.egg-info/requires.txt
 src/nrstitcher_utils.egg-info/top_level.txt
 src/nrstitcher_utils/app/__init__.py
+src/nrstitcher_utils/app/nrs_clean_scories.py
 src/nrstitcher_utils/app/nrs_config_id16a_ht.py
 src/nrstitcher_utils/core/__init__.py
 src/nrstitcher_utils/core/h5_settings.py
 src/nrstitcher_utils/core/ht_vol.py
 src/nrstitcher_utils/core/utils.py
 src/nrstitcher_utils/resources/__init__.py
 src/nrstitcher_utils/resources/config_files/__init__.py
```

