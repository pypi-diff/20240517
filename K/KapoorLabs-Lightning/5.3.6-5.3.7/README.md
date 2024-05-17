# Comparing `tmp/kapoorlabs_lightning-5.3.6.tar.gz` & `tmp/kapoorlabs_lightning-5.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kapoorlabs_lightning-5.3.6.tar", last modified: Mon May 13 20:14:13 2024, max compression
+gzip compressed data, was "kapoorlabs_lightning-5.3.7.tar", last modified: Fri May 17 20:18:54 2024, max compression
```

## Comparing `kapoorlabs_lightning-5.3.6.tar` & `kapoorlabs_lightning-5.3.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 20:14:13.893568 kapoorlabs_lightning-5.3.6/
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 20:14:13.889568 kapoorlabs_lightning-5.3.6/.github/
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 20:14:13.889568 kapoorlabs_lightning-5.3.6/.github/workflows/
--rw-r--r--   0 debian    (1000) debian    (1000)     1068 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.6/.github/workflows/deploy.yml
--rw-r--r--   0 debian    (1000) debian    (1000)     1963 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.6/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 debian    (1000) debian    (1000)      991 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.6/.gitignore
--rw-r--r--   0 debian    (1000) debian    (1000)     1008 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.6/.pre-commit-config.yaml
--rw-r--r--   0 debian    (1000) debian    (1000)     1487 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.6/LICENSE
--rw-r--r--   0 debian    (1000) debian    (1000)       96 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.6/MANIFEST.in
--rw-r--r--   0 debian    (1000) debian    (1000)     4108 2024-05-13 20:14:13.893568 kapoorlabs_lightning-5.3.6/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)     2435 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.6/README.md
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 20:14:13.889568 kapoorlabs_lightning-5.3.6/licenses/
--rw-r--r--   0 debian    (1000) debian    (1000)    11358 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.6/licenses/Apache-2
--rw-r--r--   0 debian    (1000) debian    (1000)     1487 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.6/licenses/BSD-3
--rw-r--r--   0 debian    (1000) debian    (1000)    35148 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.6/licenses/GPL-3
--rw-r--r--   0 debian    (1000) debian    (1000)     7653 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.6/licenses/LGPL-3
--rw-r--r--   0 debian    (1000) debian    (1000)     1080 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.6/licenses/MIT
--rw-r--r--   0 debian    (1000) debian    (1000)    16726 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.6/licenses/MPL-2
--rw-r--r--   0 debian    (1000) debian    (1000)      116 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.6/pyproject.toml
--rw-r--r--   0 debian    (1000) debian    (1000)     1766 2024-05-13 20:14:13.897568 kapoorlabs_lightning-5.3.6/setup.cfg
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 20:14:13.889568 kapoorlabs_lightning-5.3.6/src/
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 20:14:13.893568 kapoorlabs_lightning-5.3.6/src/KapoorLabs_Lightning.egg-info/
--rw-r--r--   0 debian    (1000) debian    (1000)     4108 2024-05-13 20:14:13.000000 kapoorlabs_lightning-5.3.6/src/KapoorLabs_Lightning.egg-info/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)     1269 2024-05-13 20:14:13.000000 kapoorlabs_lightning-5.3.6/src/KapoorLabs_Lightning.egg-info/SOURCES.txt
--rw-r--r--   0 debian    (1000) debian    (1000)        1 2024-05-13 20:14:13.000000 kapoorlabs_lightning-5.3.6/src/KapoorLabs_Lightning.egg-info/dependency_links.txt
--rw-r--r--   0 debian    (1000) debian    (1000)      102 2024-05-13 20:14:13.000000 kapoorlabs_lightning-5.3.6/src/KapoorLabs_Lightning.egg-info/requires.txt
--rw-r--r--   0 debian    (1000) debian    (1000)       21 2024-05-13 20:14:13.000000 kapoorlabs_lightning-5.3.6/src/KapoorLabs_Lightning.egg-info/top_level.txt
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 20:14:13.893568 kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/
--rw-r--r--   0 debian    (1000) debian    (1000)     1566 2024-05-13 15:57:41.000000 kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/__init__.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 20:14:13.893568 kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/_tests/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/_tests/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)     3106 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/_tests/test_pytorch_models.py
--rw-r--r--   0 debian    (1000) debian    (1000)       78 2024-05-13 20:13:33.000000 kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/_version.py
--rw-r--r--   0 debian    (1000) debian    (1000)       75 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/caped.yaml
--rw-r--r--   0 debian    (1000) debian    (1000)     2065 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/graph_functions.py
--rw-r--r--   0 debian    (1000) debian    (1000)       68 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/kapoorlabs.yaml
--rw-r--r--   0 debian    (1000) debian    (1000)    63779 2024-05-13 17:26:48.000000 kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/lightning_trainer.py
--rw-r--r--   0 debian    (1000) debian    (1000)    13629 2024-05-13 15:18:01.000000 kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/metrics.py
--rw-r--r--   0 debian    (1000) debian    (1000)     4658 2024-05-13 15:11:51.000000 kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/optimizers.py
--rw-r--r--   0 debian    (1000) debian    (1000)    10230 2024-05-13 17:03:42.000000 kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/pytorch_callbacks.py
--rw-r--r--   0 debian    (1000) debian    (1000)    16235 2024-05-13 15:11:52.000000 kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/pytorch_datasets.py
--rw-r--r--   0 debian    (1000) debian    (1000)     2680 2024-02-23 15:21:15.000000 kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/pytorch_loggers.py
--rw-r--r--   0 debian    (1000) debian    (1000)      762 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/pytorch_losses.py
--rw-r--r--   0 debian    (1000) debian    (1000)    22962 2024-05-13 20:10:57.000000 kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/pytorch_models.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1809 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/pytorch_transforms.py
--rw-r--r--   0 debian    (1000) debian    (1000)     6283 2024-05-13 15:11:52.000000 kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/schedulers.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1340 2024-05-13 15:11:52.000000 kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/utils.py
--rw-r--r--   0 debian    (1000) debian    (1000)      615 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.6/tox.ini
--rw-r--r--   0 debian    (1000) debian    (1000)      623 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.6/update_version.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-17 20:18:54.343373 kapoorlabs_lightning-5.3.7/
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-17 20:18:54.335373 kapoorlabs_lightning-5.3.7/.github/
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-17 20:18:54.339373 kapoorlabs_lightning-5.3.7/.github/workflows/
+-rw-r--r--   0 debian    (1000) debian    (1000)     1068 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/.github/workflows/deploy.yml
+-rw-r--r--   0 debian    (1000) debian    (1000)     1963 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 debian    (1000) debian    (1000)      991 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/.gitignore
+-rw-r--r--   0 debian    (1000) debian    (1000)     1008 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/.pre-commit-config.yaml
+-rw-r--r--   0 debian    (1000) debian    (1000)     1487 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/LICENSE
+-rw-r--r--   0 debian    (1000) debian    (1000)       96 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/MANIFEST.in
+-rw-r--r--   0 debian    (1000) debian    (1000)     4108 2024-05-17 20:18:54.343373 kapoorlabs_lightning-5.3.7/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)     2435 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/README.md
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-17 20:18:54.339373 kapoorlabs_lightning-5.3.7/licenses/
+-rw-r--r--   0 debian    (1000) debian    (1000)    11358 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/licenses/Apache-2
+-rw-r--r--   0 debian    (1000) debian    (1000)     1487 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/licenses/BSD-3
+-rw-r--r--   0 debian    (1000) debian    (1000)    35148 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/licenses/GPL-3
+-rw-r--r--   0 debian    (1000) debian    (1000)     7653 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/licenses/LGPL-3
+-rw-r--r--   0 debian    (1000) debian    (1000)     1080 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/licenses/MIT
+-rw-r--r--   0 debian    (1000) debian    (1000)    16726 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/licenses/MPL-2
+-rw-r--r--   0 debian    (1000) debian    (1000)      116 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/pyproject.toml
+-rw-r--r--   0 debian    (1000) debian    (1000)     1766 2024-05-17 20:18:54.343373 kapoorlabs_lightning-5.3.7/setup.cfg
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-17 20:18:54.335373 kapoorlabs_lightning-5.3.7/src/
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-17 20:18:54.343373 kapoorlabs_lightning-5.3.7/src/KapoorLabs_Lightning.egg-info/
+-rw-r--r--   0 debian    (1000) debian    (1000)     4108 2024-05-17 20:18:54.000000 kapoorlabs_lightning-5.3.7/src/KapoorLabs_Lightning.egg-info/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)     1269 2024-05-17 20:18:54.000000 kapoorlabs_lightning-5.3.7/src/KapoorLabs_Lightning.egg-info/SOURCES.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)        1 2024-05-17 20:18:54.000000 kapoorlabs_lightning-5.3.7/src/KapoorLabs_Lightning.egg-info/dependency_links.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)      102 2024-05-17 20:18:54.000000 kapoorlabs_lightning-5.3.7/src/KapoorLabs_Lightning.egg-info/requires.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)       21 2024-05-17 20:18:54.000000 kapoorlabs_lightning-5.3.7/src/KapoorLabs_Lightning.egg-info/top_level.txt
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-17 20:18:54.343373 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/
+-rw-r--r--   0 debian    (1000) debian    (1000)     1603 2024-05-17 14:55:57.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/__init__.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-17 20:18:54.343373 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/_tests/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/_tests/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     3106 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/_tests/test_pytorch_models.py
+-rw-r--r--   0 debian    (1000) debian    (1000)       78 2024-05-17 20:17:46.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/_version.py
+-rw-r--r--   0 debian    (1000) debian    (1000)       75 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/caped.yaml
+-rw-r--r--   0 debian    (1000) debian    (1000)     2065 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/graph_functions.py
+-rw-r--r--   0 debian    (1000) debian    (1000)       68 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/kapoorlabs.yaml
+-rw-r--r--   0 debian    (1000) debian    (1000)    65851 2024-05-17 20:17:40.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/lightning_trainer.py
+-rw-r--r--   0 debian    (1000) debian    (1000)    13629 2024-05-13 15:18:01.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/metrics.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     4658 2024-05-13 15:11:51.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/optimizers.py
+-rw-r--r--   0 debian    (1000) debian    (1000)    10230 2024-05-13 17:03:42.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/pytorch_callbacks.py
+-rw-r--r--   0 debian    (1000) debian    (1000)    16235 2024-05-13 15:11:52.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/pytorch_datasets.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     2680 2024-02-23 15:21:15.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/pytorch_loggers.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      762 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/pytorch_losses.py
+-rw-r--r--   0 debian    (1000) debian    (1000)    22962 2024-05-13 20:10:57.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/pytorch_models.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1809 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/pytorch_transforms.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     6283 2024-05-13 15:11:52.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/schedulers.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     2497 2024-05-17 18:55:38.000000 kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/utils.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      615 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/tox.ini
+-rw-r--r--   0 debian    (1000) debian    (1000)      623 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.7/update_version.py
```

### Comparing `kapoorlabs_lightning-5.3.6/.github/workflows/deploy.yml` & `kapoorlabs_lightning-5.3.7/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.6/.github/workflows/test_and_deploy.yml` & `kapoorlabs_lightning-5.3.7/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.6/.gitignore` & `kapoorlabs_lightning-5.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.6/.pre-commit-config.yaml` & `kapoorlabs_lightning-5.3.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.6/LICENSE` & `kapoorlabs_lightning-5.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.6/PKG-INFO` & `kapoorlabs_lightning-5.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KapoorLabs-Lightning
-Version: 5.3.6
+Version: 5.3.7
 Summary: Lightning modules for KapoorLabs specific projects
 Home-page: https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning#README.md
```

### Comparing `kapoorlabs_lightning-5.3.6/README.md` & `kapoorlabs_lightning-5.3.7/README.md`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.6/licenses/Apache-2` & `kapoorlabs_lightning-5.3.7/licenses/Apache-2`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.6/licenses/BSD-3` & `kapoorlabs_lightning-5.3.7/licenses/BSD-3`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.6/licenses/GPL-3` & `kapoorlabs_lightning-5.3.7/licenses/GPL-3`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.6/licenses/LGPL-3` & `kapoorlabs_lightning-5.3.7/licenses/LGPL-3`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.6/licenses/MIT` & `kapoorlabs_lightning-5.3.7/licenses/MIT`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.6/licenses/MPL-2` & `kapoorlabs_lightning-5.3.7/licenses/MPL-2`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.6/setup.cfg` & `kapoorlabs_lightning-5.3.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.6/src/KapoorLabs_Lightning.egg-info/PKG-INFO` & `kapoorlabs_lightning-5.3.7/src/KapoorLabs_Lightning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KapoorLabs-Lightning
-Version: 5.3.6
+Version: 5.3.7
 Summary: Lightning modules for KapoorLabs specific projects
 Home-page: https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning#README.md
```

### Comparing `kapoorlabs_lightning-5.3.6/src/KapoorLabs_Lightning.egg-info/SOURCES.txt` & `kapoorlabs_lightning-5.3.7/src/KapoorLabs_Lightning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/__init__.py` & `kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     ShapeNetDataset,
     SingleCellDataset,
     MitosisDataset,
 )
 from .pytorch_loggers import CustomNPZLogger
 from .pytorch_models import __all__ as all_pytorch_models
 from .pytorch_transforms import Transforms
-from .utils import get_most_recent_file
+from .utils import get_most_recent_file, plot_npz_files
 from .pytorch_callbacks import (
     CustomDeviceStatsMonitor,
     ExponentialDecayCallback,
     FineTuneLearningRateFinder,
     SaveFilesCallback,
     EarlyStoppingCall,
     CustomProgressBar,
@@ -59,9 +59,10 @@
     "CheckpointModel",
     "CustomVirtualMemory",
     "MitosisDataset",
     "Adam",
     "RMSprop",
     "Rprop",
     "MitosisInception",
+    "plot_npz_files"
 ]
 __all__.extend(all_pytorch_models)
```

### Comparing `kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/_tests/test_pytorch_models.py` & `kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/_tests/test_pytorch_models.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/graph_functions.py` & `kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/graph_functions.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/lightning_trainer.py` & `kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/lightning_trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,14 +89,16 @@
         gradient_clip_algorithm: str = None,
         milestones: List = None,
         factor: float = 0.1,
         patience: int = 10,
         threshold: float = 1e-4,
         t_warmup: int = 0,
         t_max: int = None,
+        weight_decay: float = 1e-5,
+        eps: float = 1e-1,
         strategy: str = "auto",
     ):
         self.npz_file = npz_file
         self.num_classes = num_classes
         self.growth_rate = growth_rate
         self.block_config = block_config
         self.num_init_features = num_init_features
@@ -126,14 +128,16 @@
         self.gradient_clip_algorithm = gradient_clip_algorithm
         self.milestones = milestones
         self.factor = factor
         self.patience = patience
         self.threshold = threshold
         self.t_warmup = t_warmup
         self.strategy = strategy
+        self.weight_decay = weight_decay
+        self.eps = eps
         self.scheduler = None
         if self.loss_function not in self.LOSS_CHOICES:
             raise ValueError(
                 f"Invalid loss function choice, must be one of {self.LOSS_CHOICES}"
             )
         if self.scheduler_choice not in self.SCHEDULER_CHOICES:
             raise ValueError(
@@ -148,15 +152,17 @@
         train_non_dividing_arrays = training_data["non_dividing_train_arrays"]
         train_non_dividing_labels = training_data["non_dividing_train_labels"]
 
         val_dividing_arrays = training_data["dividing_val_arrays"]
         val_dividing_labels = training_data["dividing_val_labels"]
         val_non_dividing_arrays = training_data["non_dividing_val_arrays"]
         val_non_dividing_labels = training_data["non_dividing_val_labels"]
-
+        print(
+            f"Dividing labels in training {len(train_dividing_labels)}, Non Dividing labels in training {len(train_non_dividing_labels)}"
+        )
         train_arrays = np.concatenate(
             (train_dividing_arrays, train_non_dividing_arrays)
         )
         train_labels = np.concatenate(
             (train_dividing_labels, train_non_dividing_labels)
         )
 
@@ -185,14 +191,15 @@
             self.num_classes,
             growth_rate=self.growth_rate,
             block_config=self.block_config,
             num_init_features=self.num_init_features,
             bottleneck_size=self.bottleneck_size,
             kernel_size=self.kernel_size,
         )
+        print(f"Training Mitosis Inception Model {self.model}")
 
     def setup_mitosisnet_model(self):
         self.model = MitosisNet(
             self.input_channels,
             self.num_classes,
         )
 
@@ -203,15 +210,17 @@
         self.logger = self.npz_logger
 
     def setup_checkpoint(self):
         self.ckpt_path = load_checkpoint_model(self.log_path)
         self.modelcheckpoint = CheckpointModel(save_dir=self.log_path)
 
     def setup_adam(self):
-        self.optimizer = Adam(lr=self.learning_rate)
+        self.optimizer = Adam(
+            lr=self.learning_rate, weight_decay=self.weight_decay, eps=self.eps
+        )
 
     def setup_rmsprop(self):
         self.optimizer = RMSprop(
             lr=self.learning_rate,
             momentum=self.momentum,
             weight_decay=self.decay,
             eps=self.epsilon,
@@ -303,35 +312,37 @@
 
 class LightningData(LightningDataModule):
     def __init__(
         self,
         data_train,
         data_val,
         batch_size=1,
-        num_workers=4,
+        num_workers=0,
     ):
         super().__init__()
         self.save_hyperparameters()
         self.data_train = data_train
         self.data_val = data_val
         self.batch_size = batch_size
         self.num_workers = num_workers
 
     def train_dataloader(self):
         return DataLoader(
             self.data_train,
             batch_size=self.batch_size,
             num_workers=self.num_workers,
+            shuffle=True,
         )
 
     def val_dataloader(self):
         return DataLoader(
             self.data_val,
             batch_size=self.batch_size,
             num_workers=self.num_workers,
+            shuffle=False,
         )
 
 
 class LightningModel(LightningModule):
     def __init__(
         self,
         network: torch.nn.Module,
@@ -339,15 +350,15 @@
         optim_func: optim,
         scheduler: schedulers = None,
         automatic_optimization: bool = True,
         on_step: bool = True,
         on_epoch: bool = True,
         sync_dist: bool = True,
         rank_zero_only: bool = False,
-        num_classes = 2
+        num_classes=2,
     ):
         super().__init__()
         self.save_hyperparameters(
             logger=False,
             ignore=["network", "loss_func", "optim_func", "scheduler"],
         )
 
@@ -359,25 +370,25 @@
         self.on_step = on_step
         self.on_epoch = on_epoch
         self.sync_dist = sync_dist
         self.rank_zero_only = rank_zero_only
         self.num_classes = num_classes
 
     @classmethod
-    def extract_json(cls, backbone_model_json):
-        if backbone_model_json is not None:
+    def extract_json(cls, checkpoint_model_json):
+        if checkpoint_model_json is not None:
             assert isinstance(
-                backbone_model_json, (str, dict)
-            ), "backbone_model_json must be a json or dict"
+                checkpoint_model_json, (str, dict)
+            ), "checkpoint_model_json must be a json or dict"
 
-            if isinstance(backbone_model_json, str):
-                with open(backbone_model_json) as file:
+            if isinstance(checkpoint_model_json, str):
+                with open(checkpoint_model_json) as file:
                     mitosis_data = json.load(file)
             else:
-                mitosis_data = backbone_model_json
+                mitosis_data = checkpoint_model_json
             return mitosis_data
 
     @classmethod
     def extract_mitosis_model(
         cls,
         mitosis_model,
         mitosis_model_json,
@@ -386,15 +397,15 @@
         scheduler=None,
         ckpt_model_path=None,
         map_location="cuda",
     ):
         if mitosis_model_json is not None:
             assert isinstance(
                 mitosis_model_json, (str, dict)
-            ), "backbone_model_json must be a json or dict"
+            ), "checkpoint_model_json must be a json or dict"
 
             if isinstance(mitosis_model_json, str):
                 with open(mitosis_model_json) as file:
                     mitosis_data = json.load(file)
             else:
                 mitosis_data = mitosis_model_json
 
@@ -404,61 +415,64 @@
                 growth_rate = mitosis_data["growth_rate"]
                 block_config = tuple(mitosis_data["block_config"])
                 num_init_features = mitosis_data["num_init_features"]
                 bottleneck_size = mitosis_data["bottleneck_size"]
                 kernel_size = mitosis_data["kernel_size"]
 
             if ckpt_model_path is None:
-                backbone_model_path = mitosis_data["model_path"]
-                most_recent_backbone_ckpt = get_most_recent_file(
-                    backbone_model_path, ".ckpt"
+                checkpoint_model_path = mitosis_data["model_path"]
+                most_recent_checkpoint_ckpt = get_most_recent_file(
+                    checkpoint_model_path, ".ckpt"
                 )
             else:
-                most_recent_backbone_ckpt = ckpt_model_path
+                most_recent_checkpoint_ckpt = ckpt_model_path
             checkpoint = torch.load(
-                most_recent_backbone_ckpt, map_location=map_location
+                most_recent_checkpoint_ckpt, map_location=map_location
             )
-            learning_rate = checkpoint["lr_schedulers"][0]["_last_lr"][0]
+            learning_rate = 1.0e-3
             if isinstance(scheduler, CosineAnnealingScheduler):
                 t_max = checkpoint["lr_schedulers"][0]["T_max"]
                 eta_min = checkpoint["lr_schedulers"][0]["eta_min"]
                 scheduler = scheduler(t_max=t_max, eta_min=eta_min)
+                learning_rate = checkpoint["lr_schedulers"][0]["_last_lr"][0]
             if isinstance(scheduler, ExponentialLR):
                 gamma = checkpoint["lr_schedulers"][0]["gamma"]
                 scheduler = scheduler(gamma=gamma)
+                learning_rate = checkpoint["lr_schedulers"][0]["_last_lr"][0]
             if isinstance(scheduler, MultiStepLR):
                 milestones = checkpoint["lr_schedulers"][0]["milestones"]
                 gamma = checkpoint["lr_schedulers"][0]["gamma"]
                 scheduler = scheduler(milestones=milestones, gamma=gamma)
+                learning_rate = checkpoint["lr_schedulers"][0]["_last_lr"][0]
 
             optimizer = optim_func(lr=learning_rate)
             network = mitosis_model(input_channels, num_classes)
             if "growth_rate" in mitosis_data.keys():
                 network = mitosis_model(
                     input_channels,
                     num_classes,
                     growth_rate=growth_rate,
                     block_config=block_config,
                     num_init_features=num_init_features,
                     bottleneck_size=bottleneck_size,
                     kernel_size=kernel_size,
                 )
 
-            backbone_lightning_model = cls.load_from_checkpoint(
-                most_recent_backbone_ckpt,
+            checkpoint_lightning_model = cls.load_from_checkpoint(
+                most_recent_checkpoint_ckpt,
                 network=network,
                 loss_func=loss_func,
                 optim_func=optimizer,
                 scheduler=scheduler,
                 map_location=map_location,
             )
 
-            backbone_torch_model = backbone_lightning_model.network
+            checkpoint_torch_model = checkpoint_lightning_model.network
 
-            return backbone_lightning_model, backbone_torch_model
+            return checkpoint_lightning_model, checkpoint_torch_model
 
     def load_pretrained(self, pretrained_file, strict=True, verbose=True):
         if isinstance(pretrained_file, (list, tuple)):
             pretrained_file = pretrained_file[0]
 
         # Load the state dict
         state_dict = torch.load(pretrained_file)["state_dict"]
@@ -493,40 +507,49 @@
     def loss(self, y_hat, y):
 
         return self.loss_func(y_hat, y)
 
     def training_step(self, batch, batch_idx):
         x, y = batch
         y_hat = self(x)
-        if not self.automatic_optimization:
-            opt = self.optimizers()
-            opt.zero_grad()
 
         if not self.automatic_optimization:
             opt = self.optimizers()
             loss = self.loss(y_hat, y)
             opt.zero_grad()
             self.manual_backward(loss)
             opt.step()
         else:
             loss = self.loss(y_hat, y)
 
-        accuracy = self.compute_accuracy(y_hat, y)
-
         self.log(
             "train_loss",
             loss,
             on_step=self.on_step,
             on_epoch=self.on_epoch,
             prog_bar=True,
             logger=True,
             sync_dist=self.sync_dist,
             rank_zero_only=self.rank_zero_only,
         )
 
+        current_lr = self.optimizers().param_groups[0]["lr"]
+        self.log(
+            "learning_rate",
+            current_lr,
+            on_step=self.on_step,
+            on_epoch=self.on_epoch,
+            prog_bar=True,
+            logger=True,
+            sync_dist=self.sync_dist,
+            rank_zero_only=self.rank_zero_only,
+        )
+
+        accuracy = self.compute_accuracy(y_hat, y)
+
         self.log(
             "train_accuracy",
             accuracy,
             on_step=self.on_step,
             on_epoch=self.on_epoch,
             prog_bar=True,
             logger=True,
@@ -543,40 +566,56 @@
         x, y = batch
         y_hat = self(x)
         loss = self.loss(y_hat, y)
         accuracy = self.compute_accuracy(y_hat, y)
         self.log(
             f"{prefix}_loss",
             loss,
-            on_step=self.on_step,
             on_epoch=self.on_epoch,
             prog_bar=True,
             logger=True,
             sync_dist=self.sync_dist,
             rank_zero_only=self.rank_zero_only,
         )
 
         self.log(
             f"{prefix}_accuracy",
             accuracy,
-            on_step=self.on_step,
             on_epoch=self.on_epoch,
             prog_bar=True,
             logger=True,
             sync_dist=self.sync_dist,
             rank_zero_only=self.rank_zero_only,
         )
 
     def validation_step(self, batch, batch_idx):
         self._shared_eval(batch, batch_idx, "validation")
 
+    def on_train_epoch_end(self) -> None:
+        """Actions to perform at the end of each training epoch."""
+
+        sch = self.lr_schedulers()
+        learning_rate = self.optimizers().param_groups[0]["lr"]
+        self.log(
+            "learning_rate",
+            learning_rate,
+            prog_bar=True,
+            logger=False,
+            sync_dist=self.sync_dist,
+            rank_zero_only=self.rank_zero_only,
+        )
+        if isinstance(sch, torch.optim.lr_scheduler.ReduceLROnPlateau):
+            sch.step(self.trainer.callback_metrics[self.reduce_lr_metric])
+
     def compute_accuracy(self, outputs, labels):
 
         predicted = outputs.data
-        accuracy = Accuracy(task="multiclass", num_classes=self.num_classes).to(self.device)
+        accuracy = Accuracy(task="multiclass", num_classes=self.num_classes).to(
+            self.device
+        )
         accuracies = accuracy(predicted, labels)
 
         return accuracies
 
     def configure_optimizers(self):
         optimizer = self.optim_func(self.parameters())
 
@@ -1058,15 +1097,16 @@
     def callback_metrics(self):
         return self.trainer.callback_metrics
 
 
 class LightningTrain:
     def __init__(
         self,
-        dataset: Dataset,
+        dataset_train: Dataset,
+        dataset_val: Dataset,
         loss_func: torch.nn.Module,
         model_func: torch.nn.Module,
         optim_func: optimizers._Optimizer,
         model_save_file: str,
         ckpt_file: str = None,
         train_val_test_split: List = [95, 2.5, 2.5],
         batch_size: int = 64,
@@ -1079,15 +1119,17 @@
         num_workers: int = 4,
         enable_checkpointing: bool = True,
         callbacks: List[Callback] = None,
         scheduler: schedulers = None,
         logger: Logger = None,
         **kwargs,
     ):
-        self.dataset = dataset
+        self.dataset_train = dataset_train
+
+        self.dataset_val = dataset_val
 
         self.loss_func = loss_func
 
         self.model_func = model_func
 
         self.optim_func = optim_func
 
@@ -1126,25 +1168,29 @@
             "model_func": self.model_func,
             "min_epochs": self.min_epochs,
             "epochs": self.epochs,
             "optim_func": self.optim_func,
             "scheduler": self.scheduler,
             "train_val_test_split": self.train_val_test_split,
             "batch_size": self.batch_size,
-            "dataset": self.dataset,
+            "dataset_train": self.dataset_train,
+            "dataset_val": self.dataset_val,
         }
         self.hparams.update(kwargs=kwargs)
 
     def _train_model(self):
         self.model = LightningModel(
             self.model_func, self.loss_func, self.optim_func, self.scheduler
         )
 
-        self.datas = LightningData(hparams=self.hparams, num_workers=self.num_workers)
-        self.datas.setup("fit")
+        self.datas = LightningData(
+            data_train=self.dataset_train,
+            data_val=self.dataset_val,
+            num_workers=self.num_workers,
+        )
         self.default_root_dir = Path(self.model_save_file).absolute().parent.as_posix()
         self.default_root_dir = os.path.join(
             self.default_root_dir, Path(self.model_save_file).stem
         )
         Path(self.default_root_dir).mkdir(exist_ok=True)
 
         self.trainer = Trainer(
@@ -1178,15 +1224,16 @@
     def callback_metrics(self):
         return self.trainer.callback_metrics
 
 
 class AutoLightningTrain:
     def __init__(
         self,
-        dataset: Dataset,
+        dataset_train: Dataset,
+        dataset_val: Dataset,
         loss_func: torch.nn.Module,
         model_func: torch.nn.Module,
         optim_func: optimizers._Optimizer,
         model_save_file: str,
         ckpt_file: str = None,
         train_val_test_split: List = [95, 2.5, 2.5],
         batch_size: int = 64,
@@ -1199,15 +1246,17 @@
         num_workers: int = 4,
         enable_checkpointing: bool = True,
         callbacks: List[Callback] = None,
         scheduler: schedulers = None,
         logger: Logger = None,
         **kwargs,
     ):
-        self.dataset = dataset
+        self.dataset_train = dataset_train
+
+        self.dataset_val = dataset_val
 
         self.loss_func = loss_func
 
         self.model_func = model_func
 
         self.optim_func = optim_func
 
@@ -1246,25 +1295,29 @@
             "model_func": self.model_func,
             "min_epochs": self.min_epochs,
             "epochs": self.epochs,
             "optim_func": self.optim_func,
             "scheduler": self.scheduler,
             "train_val_test_split": self.train_val_test_split,
             "batch_size": self.batch_size,
-            "dataset": self.dataset,
+            "dataset_train": self.dataset_train,
+            "dataset_val": self.dataset_val,
         }
         self.hparams.update(kwargs=kwargs)
 
     def _train_model(self):
         self.model = AutoLightningModel(
             self.model_func, self.loss_func, self.optim_func, self.scheduler
         )
 
-        self.datas = LightningData(hparams=self.hparams, num_workers=self.num_workers)
-        self.datas.setup("fit")
+        self.datas = LightningData(
+            data_train=self.dataset_train,
+            data_val=self.dataset_val,
+            num_workers=self.num_workers,
+        )
         self.default_root_dir = Path(self.model_save_file).absolute().parent.as_posix()
         self.default_root_dir = os.path.join(
             self.default_root_dir, Path(self.model_save_file).stem
         )
         Path(self.default_root_dir).mkdir(exist_ok=True)
 
         self.trainer = Trainer(
@@ -1310,15 +1363,16 @@
     def callback_metrics(self):
         return self.trainer.callback_metrics
 
 
 class ClusterLightningTrain:
     def __init__(
         self,
-        dataset: Dataset,
+        dataset_train: Dataset,
+        dataset_val: Dataset,
         loss_func: torch.nn.Module,
         cluster_loss_func: torch.nn.Module,
         network: DeepEmbeddedClustering,
         optim_func: optimizers._Optimizer,
         model_save_file: str,
         ckpt_file: str = None,
         train_val_test_split: List = [95, 2.5, 2.5],
@@ -1334,15 +1388,17 @@
         enable_checkpointing: bool = True,
         callbacks: List[Callback] = None,
         scheduler: schedulers = None,
         logger: Logger = None,
         mem_percent: int = 20,
         **kwargs,
     ):
-        self.dataset = dataset
+        self.dataset_train = dataset_train
+
+        self.dataset_val = dataset_val
 
         self.loss_func = loss_func
 
         self.cluster_loss_func = cluster_loss_func
 
         self.gamma = gamma
 
@@ -1387,15 +1443,16 @@
             "network": self.network,
             "min_epochs": self.min_epochs,
             "epochs": self.epochs,
             "optim_func": self.optim_func,
             "scheduler": self.scheduler,
             "train_val_test_split": self.train_val_test_split,
             "batch_size": self.batch_size,
-            "dataset": self.dataset,
+            "dataset_train": self.dataset_train,
+            "dataset_val": self.dataset_val,
         }
         self.hparams.update(kwargs=kwargs)
 
     def _train_model(self):
         self.default_root_dir = Path(self.model_save_file).absolute().parent.as_posix()
         self.default_root_dir = os.path.join(
             self.default_root_dir, Path(self.model_save_file).stem
@@ -1410,16 +1467,19 @@
             min_epochs=self.min_epochs,
             max_epochs=self.epochs,
             default_root_dir=self.default_root_dir,
             enable_checkpointing=self.enable_checkpointing,
             num_nodes=self.num_nodes,
         )
 
-        self.datas = LightningData(hparams=self.hparams, num_workers=self.num_workers)
-        self.datas.setup("fit")
+        self.datas = LightningData(
+            data_train=self.dataset_train,
+            data_val=self.dataset_val,
+            num_workers=self.num_workers,
+        )
         train_dataloaders = self.datas.train_dataloader()
         predict_loader = self.datas.predict_dataloader()
 
         if self.ckpt_file is None:
             get_kmeans = True
         else:
             get_kmeans = False
```

### Comparing `kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/metrics.py` & `kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/metrics.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/optimizers.py` & `kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/optimizers.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/pytorch_callbacks.py` & `kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/pytorch_callbacks.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/pytorch_datasets.py` & `kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/pytorch_datasets.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/pytorch_loggers.py` & `kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/pytorch_loggers.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/pytorch_losses.py` & `kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/pytorch_losses.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/pytorch_models.py` & `kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/pytorch_models.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/pytorch_transforms.py` & `kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/pytorch_transforms.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.6/src/kapoorlabs_lightning/schedulers.py` & `kapoorlabs_lightning-5.3.7/src/kapoorlabs_lightning/schedulers.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.6/tox.ini` & `kapoorlabs_lightning-5.3.7/tox.ini`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.6/update_version.py` & `kapoorlabs_lightning-5.3.7/update_version.py`

 * *Files identical despite different names*

