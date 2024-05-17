# Comparing `tmp/snewpy-1.5.tar.gz` & `tmp/snewpy-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snewpy-1.5.tar", last modified: Fri May  3 14:21:56 2024, max compression
+gzip compressed data, was "snewpy-1.5.1.tar", last modified: Fri May 17 09:21:37 2024, max compression
```

## Comparing `snewpy-1.5.tar` & `snewpy-1.5.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:21:56.966618 snewpy-1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-03 14:21:25.000000 snewpy-1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-03 14:21:56.966618 snewpy-1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-03 14:21:25.000000 snewpy-1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:21:56.958618 snewpy-1.5/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:21:56.962618 snewpy-1.5/python/snewpy/
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/_git.py
--rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/_model_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    54158 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/flavor_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)    15744 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/flux.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/from_snowglobes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:21:56.966618 snewpy-1.5/python/snewpy/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11026 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    25596 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/models/ccsn.py
--rw-r--r--   0 runner    (1001) docker     (127)    34393 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/models/ccsn_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/models/model_files.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/models/presn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/models/presn_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    21931 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/models/registry_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8258 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/neutrino.py
--rw-r--r--   0 runner    (1001) docker     (127)    17477 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/rate_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/run_snowglobes.py
--rw-r--r--   0 runner    (1001) docker     (127)    19106 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/snowglobes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14103 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/snowglobes_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:21:56.966618 snewpy-1.5/python/snewpy/test/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/test/_rate_crosscheck_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/test/simplerate_integrationtest.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/test/snewpy_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/test/test_00_init.py
--rw-r--r--   0 runner    (1001) docker     (127)    17150 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/test/test_01_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    13490 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/test/test_02_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/test/test_03_neutrino.py
--rw-r--r--   0 runner    (1001) docker     (127)    33885 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/test/test_04_xforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/test/test_05_snowglobes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/test/test_flux_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/test/test_presn_rates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/test/test_rate_calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-03 14:21:25.000000 snewpy-1.5/python/snewpy/to_snowglobes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:21:56.962618 snewpy-1.5/python/snewpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-03 14:21:56.000000 snewpy-1.5/python/snewpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-03 14:21:56.000000 snewpy-1.5/python/snewpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 14:21:56.000000 snewpy-1.5/python/snewpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 14:21:39.000000 snewpy-1.5/python/snewpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-03 14:21:56.000000 snewpy-1.5/python/snewpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 14:21:56.000000 snewpy-1.5/python/snewpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 14:21:56.966618 snewpy-1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-03 14:21:25.000000 snewpy-1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:21:37.689344 snewpy-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-17 09:21:03.000000 snewpy-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-05-17 09:21:37.685344 snewpy-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-17 09:21:03.000000 snewpy-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:21:37.681344 snewpy-1.5.1/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:21:37.681344 snewpy-1.5.1/python/snewpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/_model_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54158 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/flavor_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15744 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/flux.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/from_snowglobes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:21:37.685344 snewpy-1.5.1/python/snewpy/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11026 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25596 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/models/ccsn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34393 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/models/ccsn_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/models/model_files.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/models/presn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/models/presn_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21930 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/models/registry_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8258 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/neutrino.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17477 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/rate_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/run_snowglobes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19106 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/snowglobes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14103 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/snowglobes_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:21:37.685344 snewpy-1.5.1/python/snewpy/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/test/_rate_crosscheck_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/test/simplerate_integrationtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/test/snewpy_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/test/test_00_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17150 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/test/test_01_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13490 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/test/test_02_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/test/test_03_neutrino.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33885 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/test/test_04_xforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/test/test_05_snowglobes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/test/test_flux_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/test/test_presn_rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/test/test_rate_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-17 09:21:03.000000 snewpy-1.5.1/python/snewpy/to_snowglobes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:21:37.685344 snewpy-1.5.1/python/snewpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-05-17 09:21:37.000000 snewpy-1.5.1/python/snewpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-17 09:21:37.000000 snewpy-1.5.1/python/snewpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 09:21:37.000000 snewpy-1.5.1/python/snewpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 09:21:19.000000 snewpy-1.5.1/python/snewpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-17 09:21:37.000000 snewpy-1.5.1/python/snewpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 09:21:37.000000 snewpy-1.5.1/python/snewpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 09:21:37.689344 snewpy-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-17 09:21:03.000000 snewpy-1.5.1/setup.py
```

### Comparing `snewpy-1.5/LICENSE` & `snewpy-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/PKG-INFO` & `snewpy-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snewpy
-Version: 1.5
+Version: 1.5.1
 Summary: A Python package for working with supernova neutrinos
 Home-page: https://github.com/SNEWS2/snewpy
 Author: SNEWS Collaboration
 Author-email: snews2.0@lists.bnl.gov
 License: BSD
 Provides: snewpy
 Requires-Python: >=3.8
```

### Comparing `snewpy-1.5/README.md` & `snewpy-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/__init__.py` & `snewpy-1.5.1/python/snewpy/__init__.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/_git.py` & `snewpy-1.5.1/python/snewpy/_git.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/_model_downloader.py` & `snewpy-1.5.1/python/snewpy/_model_downloader.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/flavor_transformation.py` & `snewpy-1.5.1/python/snewpy/flavor_transformation.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/flux.py` & `snewpy-1.5.1/python/snewpy/flux.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/from_snowglobes.py` & `snewpy-1.5.1/python/snewpy/from_snowglobes.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/models/__init__.py` & `snewpy-1.5.1/python/snewpy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/models/base.py` & `snewpy-1.5.1/python/snewpy/models/base.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/models/ccsn.py` & `snewpy-1.5.1/python/snewpy/models/ccsn.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/models/ccsn_loaders.py` & `snewpy-1.5.1/python/snewpy/models/ccsn_loaders.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/models/model_files.yml` & `snewpy-1.5.1/python/snewpy/models/model_files.yml`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/models/presn.py` & `snewpy-1.5.1/python/snewpy/models/presn.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/models/presn_loaders.py` & `snewpy-1.5.1/python/snewpy/models/presn_loaders.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/models/registry_model.py` & `snewpy-1.5.1/python/snewpy/models/registry_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -469,15 +469,15 @@
         _loader_class = c.__mro__[2] #store the loader class for later use
 
         def __init__(self, filename:str=None, *args, **kwargs):
             if filename is not None:
                 if not hasattr(self,'metadata'):
                     self.metadata = {}
                 if hasattr(self,'_metadata_from_filename'):
-                    self.metadata.update(*self._metadata_from_filename(filename))
+                    self.metadata.update(self._metadata_from_filename(filename))
                 self._loader_class.__init__(self, filename=os.path.abspath(filename), metadata=self.metadata)
             else:
                 super().__init__(*args, **kwargs)
 
     #generate the docstring
     c1.__doc__ = c.__doc__
     c1._doc_params_ = {'Parameters':
```

### Comparing `snewpy-1.5/python/snewpy/neutrino.py` & `snewpy-1.5.1/python/snewpy/neutrino.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/rate_calculator.py` & `snewpy-1.5.1/python/snewpy/rate_calculator.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/snowglobes.py` & `snewpy-1.5.1/python/snewpy/snowglobes.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/snowglobes_interface.py` & `snewpy-1.5.1/python/snewpy/snowglobes_interface.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/test/_rate_crosscheck_table.py` & `snewpy-1.5.1/python/snewpy/test/_rate_crosscheck_table.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/test/simplerate_integrationtest.py` & `snewpy-1.5.1/python/snewpy/test/simplerate_integrationtest.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/test/snewpy_test_suite.py` & `snewpy-1.5.1/python/snewpy/test/snewpy_test_suite.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/test/test_01_registry.py` & `snewpy-1.5.1/python/snewpy/test/test_01_registry.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/test/test_02_models.py` & `snewpy-1.5.1/python/snewpy/test/test_02_models.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/test/test_03_neutrino.py` & `snewpy-1.5.1/python/snewpy/test/test_03_neutrino.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/test/test_04_xforms.py` & `snewpy-1.5.1/python/snewpy/test/test_04_xforms.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/test/test_05_snowglobes.py` & `snewpy-1.5.1/python/snewpy/test/test_05_snowglobes.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/test/test_flux_container.py` & `snewpy-1.5.1/python/snewpy/test/test_flux_container.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/test/test_presn_rates.py` & `snewpy-1.5.1/python/snewpy/test/test_presn_rates.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/test/test_rate_calculation.py` & `snewpy-1.5.1/python/snewpy/test/test_rate_calculation.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy/to_snowglobes.py` & `snewpy-1.5.1/python/snewpy/to_snowglobes.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/python/snewpy.egg-info/PKG-INFO` & `snewpy-1.5.1/python/snewpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snewpy
-Version: 1.5
+Version: 1.5.1
 Summary: A Python package for working with supernova neutrinos
 Home-page: https://github.com/SNEWS2/snewpy
 Author: SNEWS Collaboration
 Author-email: snews2.0@lists.bnl.gov
 License: BSD
 Provides: snewpy
 Requires-Python: >=3.8
```

### Comparing `snewpy-1.5/python/snewpy.egg-info/SOURCES.txt` & `snewpy-1.5.1/python/snewpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `snewpy-1.5/setup.py` & `snewpy-1.5.1/setup.py`

 * *Files identical despite different names*

