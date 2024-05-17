# Comparing `tmp/fairchem_demo_ocpapi-0.0.1.tar.gz` & `tmp/fairchem_demo_ocpapi-0.0.1b0.tar.gz`

## Comparing `fairchem_demo_ocpapi-0.0.1.tar` & `fairchem_demo_ocpapi-0.0.1b0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1/src/fairchem/demo/ocpapi/.isort.cfg
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1/src/fairchem/demo/ocpapi/LICENSE
--rw-r--r--   0        0        0     8515 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1/src/fairchem/demo/ocpapi/README.md
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1/src/fairchem/demo/ocpapi/__init__.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1/src/fairchem/demo/ocpapi/version.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1/src/fairchem/demo/ocpapi/client/__init__.py
--rw-r--r--   0        0        0    16402 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1/src/fairchem/demo/ocpapi/client/client.py
--rw-r--r--   0        0        0    12676 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1/src/fairchem/demo/ocpapi/client/models.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1/src/fairchem/demo/ocpapi/client/ui.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1/src/fairchem/demo/ocpapi/workflows/__init__.py
--rw-r--r--   0        0        0    28890 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1/src/fairchem/demo/ocpapi/workflows/adsorbates.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1/src/fairchem/demo/ocpapi/workflows/context.py
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1/src/fairchem/demo/ocpapi/workflows/filter.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1/src/fairchem/demo/ocpapi/workflows/log.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1/src/fairchem/demo/ocpapi/workflows/retry.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1/.gitignore
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     9444 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/.isort.cfg
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/LICENSE
+-rw-r--r--   0        0        0     8515 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/README.md
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/__init__.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/version.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/client/__init__.py
+-rw-r--r--   0        0        0    16402 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/client/client.py
+-rw-r--r--   0        0        0    12676 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/client/models.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/client/ui.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/workflows/__init__.py
+-rw-r--r--   0        0        0    28890 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/workflows/adsorbates.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/workflows/context.py
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/workflows/filter.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/workflows/log.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/workflows/retry.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/.gitignore
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/pyproject.toml
+-rw-r--r--   0        0        0     9389 2020-02-02 00:00:00.000000 fairchem_demo_ocpapi-0.0.1b0/PKG-INFO
```

### Comparing `fairchem_demo_ocpapi-0.0.1/src/fairchem/demo/ocpapi/LICENSE` & `fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/LICENSE`

 * *Files identical despite different names*

### Comparing `fairchem_demo_ocpapi-0.0.1/src/fairchem/demo/ocpapi/README.md` & `fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/README.md`

 * *Files identical despite different names*

### Comparing `fairchem_demo_ocpapi-0.0.1/src/fairchem/demo/ocpapi/client/client.py` & `fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/client/client.py`

 * *Files identical despite different names*

### Comparing `fairchem_demo_ocpapi-0.0.1/src/fairchem/demo/ocpapi/client/models.py` & `fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/client/models.py`

 * *Files identical despite different names*

### Comparing `fairchem_demo_ocpapi-0.0.1/src/fairchem/demo/ocpapi/client/ui.py` & `fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/client/ui.py`

 * *Files identical despite different names*

### Comparing `fairchem_demo_ocpapi-0.0.1/src/fairchem/demo/ocpapi/workflows/__init__.py` & `fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `fairchem_demo_ocpapi-0.0.1/src/fairchem/demo/ocpapi/workflows/adsorbates.py` & `fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/workflows/adsorbates.py`

 * *Files identical despite different names*

### Comparing `fairchem_demo_ocpapi-0.0.1/src/fairchem/demo/ocpapi/workflows/context.py` & `fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/workflows/context.py`

 * *Files identical despite different names*

### Comparing `fairchem_demo_ocpapi-0.0.1/src/fairchem/demo/ocpapi/workflows/filter.py` & `fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/workflows/filter.py`

 * *Files identical despite different names*

### Comparing `fairchem_demo_ocpapi-0.0.1/src/fairchem/demo/ocpapi/workflows/retry.py` & `fairchem_demo_ocpapi-0.0.1b0/src/fairchem/demo/ocpapi/workflows/retry.py`

 * *Files identical despite different names*

### Comparing `fairchem_demo_ocpapi-0.0.1/.gitignore` & `fairchem_demo_ocpapi-0.0.1b0/.gitignore`

 * *Files identical despite different names*

### Comparing `fairchem_demo_ocpapi-0.0.1/pyproject.toml` & `fairchem_demo_ocpapi-0.0.1b0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     "tenacity == 8.2.3",
     "tqdm == 4.66.1",
 ]
 
 [project.urls]
 repository = "https://github.com/FAIR-Chem/fairchem/tree/main/src/fairchem/demo/ocpapi"
 home = "https://open-catalyst.metademolab.com/"
-documentation = "https://fair-chem.github.io/"
 
 [project.optional-dependencies]
 dev = [
     "ase == 3.22.1",
     "readchar == 4.0.5",
 ]
```

### Comparing `fairchem_demo_ocpapi-0.0.1/PKG-INFO` & `fairchem_demo_ocpapi-0.0.1b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.3
 Name: fairchem-demo-ocpapi
-Version: 0.0.1
+Version: 0.0.1b0
 Summary: Python client library for the Open Catalyst API
 Project-URL: repository, https://github.com/FAIR-Chem/fairchem/tree/main/src/fairchem/demo/ocpapi
 Project-URL: home, https://open-catalyst.metademolab.com/
-Project-URL: documentation, https://fair-chem.github.io/
 Author-email: Open Catalyst Project <opencatalyst@meta.com>
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Requires-Dist: dataclasses-json==0.6.0
```

