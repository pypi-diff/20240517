# Comparing `tmp/slurm-sbalance-0.2.2.tar.gz` & `tmp/slurm-sbalance-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/lustrefs/disk/home/putt/projects/slurm-sbalance/dist/tmp9iw1pvc6/slurm-sbalance-0.2.2.tar", last modified: Tue Mar  7 07:18:07 2023, max compression
+gzip compressed data, was "/lustrefs/disk/home/putt/projects/slurm-sbalance/dist/tmp9_zmx25h/slurm-sbalance-0.2.3.tar", last modified: Fri May 17 03:59:34 2024, max compression
```

## Comparing `slurm-sbalance-0.2.2.tar` & `slurm-sbalance-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 putt     (1980400009) putt     (1980400009)        0 2023-03-07 07:18:07.000000 slurm-sbalance-0.2.2/
--rw-r--r--   0 putt     (1980400009) putt     (1980400009)     1105 2023-02-20 04:23:15.000000 slurm-sbalance-0.2.2/LICENSE
--rw-r--r--   0 putt     (1980400009) putt     (1980400009)     2298 2023-03-07 07:18:07.000000 slurm-sbalance-0.2.2/PKG-INFO
--rw-r--r--   0 putt     (1980400009) putt     (1980400009)     1438 2023-02-20 04:23:15.000000 slurm-sbalance-0.2.2/README.md
--rw-r--r--   0 putt     (1980400009) putt     (1980400009)      649 2023-03-01 07:45:45.000000 slurm-sbalance-0.2.2/pyproject.toml
-drwxr-xr-x   0 putt     (1980400009) putt     (1980400009)        0 2023-03-07 07:18:07.000000 slurm-sbalance-0.2.2/sbalance/
--rw-r--r--   0 putt     (1980400009) putt     (1980400009)      166 2023-02-27 13:33:48.000000 slurm-sbalance-0.2.2/sbalance/__init__.py
--rw-r--r--   0 putt     (1980400009) putt     (1980400009)       58 2023-02-20 04:23:15.000000 slurm-sbalance-0.2.2/sbalance/__main__.py
--rw-r--r--   0 putt     (1980400009) putt     (1980400009)      283 2023-03-07 07:13:31.000000 slurm-sbalance-0.2.2/sbalance/config.py
--rw-r--r--   0 putt     (1980400009) putt     (1980400009)     3962 2023-03-07 06:58:10.000000 slurm-sbalance-0.2.2/sbalance/fields.py
--rwxr-xr-x   0 putt     (1980400009) putt     (1980400009)     8990 2023-03-07 07:12:05.000000 slurm-sbalance-0.2.2/sbalance/sbalance.py
--rw-r--r--   0 putt     (1980400009) putt     (1980400009)    10240 2023-03-03 08:50:02.000000 slurm-sbalance-0.2.2/sbalance/slurm.py
--rw-r--r--   0 putt     (1980400009) putt     (1980400009)      497 2023-02-28 07:15:39.000000 slurm-sbalance-0.2.2/sbalance/utils.py
--rw-r--r--   0 putt     (1980400009) putt     (1980400009)       38 2023-03-07 07:18:07.000000 slurm-sbalance-0.2.2/setup.cfg
--rw-r--r--   0 putt     (1980400009) putt     (1980400009)     1611 2023-03-07 07:07:32.000000 slurm-sbalance-0.2.2/setup.py
-drwxr-xr-x   0 putt     (1980400009) putt     (1980400009)        0 2023-03-07 07:18:07.000000 slurm-sbalance-0.2.2/slurm_sbalance.egg-info/
--rw-r--r--   0 putt     (1980400009) putt     (1980400009)     2298 2023-03-07 07:18:07.000000 slurm-sbalance-0.2.2/slurm_sbalance.egg-info/PKG-INFO
--rw-r--r--   0 putt     (1980400009) putt     (1980400009)      371 2023-03-07 07:18:07.000000 slurm-sbalance-0.2.2/slurm_sbalance.egg-info/SOURCES.txt
--rw-r--r--   0 putt     (1980400009) putt     (1980400009)        1 2023-03-07 07:18:07.000000 slurm-sbalance-0.2.2/slurm_sbalance.egg-info/dependency_links.txt
--rw-r--r--   0 putt     (1980400009) putt     (1980400009)       44 2023-03-07 07:18:07.000000 slurm-sbalance-0.2.2/slurm_sbalance.egg-info/entry_points.txt
--rw-r--r--   0 putt     (1980400009) putt     (1980400009)        9 2023-03-07 07:18:07.000000 slurm-sbalance-0.2.2/slurm_sbalance.egg-info/top_level.txt
+drwxr-xr-x   0 putt     (1980400009) putt     (1980400009)        0 2024-05-17 03:59:34.000000 slurm-sbalance-0.2.3/
+-rw-r-----   0 putt     (1980400009) putt     (1980400009)     1105 2023-02-20 04:23:15.000000 slurm-sbalance-0.2.3/LICENSE
+-rw-r--r--   0 putt     (1980400009) putt     (1980400009)     2298 2024-05-17 03:59:34.000000 slurm-sbalance-0.2.3/PKG-INFO
+-rw-r-----   0 putt     (1980400009) putt     (1980400009)     1438 2023-02-20 04:23:15.000000 slurm-sbalance-0.2.3/README.md
+-rw-r-----   0 putt     (1980400009) putt     (1980400009)      649 2023-03-01 07:45:45.000000 slurm-sbalance-0.2.3/pyproject.toml
+drwxr-xr-x   0 putt     (1980400009) putt     (1980400009)        0 2024-05-17 03:59:34.000000 slurm-sbalance-0.2.3/sbalance/
+-rw-r-----   0 putt     (1980400009) putt     (1980400009)      166 2023-02-27 13:33:48.000000 slurm-sbalance-0.2.3/sbalance/__init__.py
+-rw-r-----   0 putt     (1980400009) putt     (1980400009)       58 2023-02-20 04:23:15.000000 slurm-sbalance-0.2.3/sbalance/__main__.py
+-rw-r-----   0 putt     (1980400009) putt     (1980400009)      283 2024-05-17 03:49:30.000000 slurm-sbalance-0.2.3/sbalance/config.py
+-rw-r-----   0 putt     (1980400009) putt     (1980400009)     3962 2023-03-07 06:58:10.000000 slurm-sbalance-0.2.3/sbalance/fields.py
+-rwxr-x---   0 putt     (1980400009) putt     (1980400009)     8990 2023-03-07 07:12:05.000000 slurm-sbalance-0.2.3/sbalance/sbalance.py
+-rw-r-----   0 putt     (1980400009) putt     (1980400009)    10237 2024-05-17 03:40:05.000000 slurm-sbalance-0.2.3/sbalance/slurm.py
+-rw-r-----   0 putt     (1980400009) putt     (1980400009)      497 2023-02-28 07:15:39.000000 slurm-sbalance-0.2.3/sbalance/utils.py
+-rw-r--r--   0 putt     (1980400009) putt     (1980400009)       38 2024-05-17 03:59:34.000000 slurm-sbalance-0.2.3/setup.cfg
+-rw-r-----   0 putt     (1980400009) putt     (1980400009)     1611 2024-05-17 03:49:09.000000 slurm-sbalance-0.2.3/setup.py
+drwxr-xr-x   0 putt     (1980400009) putt     (1980400009)        0 2024-05-17 03:59:34.000000 slurm-sbalance-0.2.3/slurm_sbalance.egg-info/
+-rw-r-----   0 putt     (1980400009) putt     (1980400009)     2298 2024-05-17 03:59:34.000000 slurm-sbalance-0.2.3/slurm_sbalance.egg-info/PKG-INFO
+-rw-r-----   0 putt     (1980400009) putt     (1980400009)      371 2024-05-17 03:59:34.000000 slurm-sbalance-0.2.3/slurm_sbalance.egg-info/SOURCES.txt
+-rw-r-----   0 putt     (1980400009) putt     (1980400009)        1 2024-05-17 03:59:34.000000 slurm-sbalance-0.2.3/slurm_sbalance.egg-info/dependency_links.txt
+-rw-r-----   0 putt     (1980400009) putt     (1980400009)       44 2024-05-17 03:59:34.000000 slurm-sbalance-0.2.3/slurm_sbalance.egg-info/entry_points.txt
+-rw-r-----   0 putt     (1980400009) putt     (1980400009)        9 2024-05-17 03:59:34.000000 slurm-sbalance-0.2.3/slurm_sbalance.egg-info/top_level.txt
```

### Comparing `slurm-sbalance-0.2.2/LICENSE` & `slurm-sbalance-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `slurm-sbalance-0.2.2/PKG-INFO` & `slurm-sbalance-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurm-sbalance
-Version: 0.2.2
+Version: 0.2.3
 Summary: Slurm utility for checking account balance
 Home-page: https://github.com/puttsk/slurm-sbalance
 Author: Putt Sakdhnagool
 Author-email: putt.sakdhnagool@nectec.or.th
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/puttsk/slurm-sbalance/issues
 Project-URL: Source, https://github.com/puttsk/slurm-sbalance/
```

### Comparing `slurm-sbalance-0.2.2/README.md` & `slurm-sbalance-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `slurm-sbalance-0.2.2/pyproject.toml` & `slurm-sbalance-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `slurm-sbalance-0.2.2/sbalance/fields.py` & `slurm-sbalance-0.2.3/sbalance/fields.py`

 * *Files identical despite different names*

### Comparing `slurm-sbalance-0.2.2/sbalance/sbalance.py` & `slurm-sbalance-0.2.3/sbalance/sbalance.py`

 * *Files identical despite different names*

### Comparing `slurm-sbalance-0.2.2/sbalance/slurm.py` & `slurm-sbalance-0.2.3/sbalance/slurm.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 SCONTROL_CLI = 'scontrol'
 
 SU_UNLIMITED = 'unlimited'
 SERVICE_HOUR_FACTOR = 7680.0 
 
 PARTITION_CONFIGS = [
     {"name":"compute", "factor": 128 * 1 * 60},
-    {"name":"gpu", "factor": 4 * 112 * 60},
-    {"name":"memory", "factor": 128 * 4.5 * 60}
+    {"name":"gpu", "factor": 4 * 96 * 60},
+    {"name":"memory", "factor": 128 * 4 * 60}
 ]
 
 class Slurm:
 
     @classmethod
     def get_qos(cls) -> dict:
         """get_slurm_qos returns a dictionary containing QoS data."""
```

### Comparing `slurm-sbalance-0.2.2/setup.py` & `slurm-sbalance-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='slurm-sbalance',
-    version="0.2.2",  
+    version="0.2.3",  
     description='Slurm utility for checking account balance',  
     long_description=long_description, 
     long_description_content_type='text/markdown', 
     url='https://github.com/puttsk/slurm-sbalance',  
     author='Putt Sakdhnagool',
     author_email='putt.sakdhnagool@nectec.or.th', 
     classifiers=[
```

### Comparing `slurm-sbalance-0.2.2/slurm_sbalance.egg-info/PKG-INFO` & `slurm-sbalance-0.2.3/slurm_sbalance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurm-sbalance
-Version: 0.2.2
+Version: 0.2.3
 Summary: Slurm utility for checking account balance
 Home-page: https://github.com/puttsk/slurm-sbalance
 Author: Putt Sakdhnagool
 Author-email: putt.sakdhnagool@nectec.or.th
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/puttsk/slurm-sbalance/issues
 Project-URL: Source, https://github.com/puttsk/slurm-sbalance/
```

