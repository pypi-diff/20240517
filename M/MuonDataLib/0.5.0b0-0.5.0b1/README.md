# Comparing `tmp/muondatalib-0.5.0b0.tar.gz` & `tmp/muondatalib-0.5.0b1.tar.gz`

## Comparing `muondatalib-0.5.0b0.tar` & `muondatalib-0.5.0b1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/.readthedocs.yaml
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/MuonDataLib-dev.yml
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/MuonDataLib.yml
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/.github/release.yml
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/.github/workflows/flake8.yml
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/.github/workflows/label_merge_conflicts.yml
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/.github/workflows/merge.yml
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/.github/workflows/release_next.yml
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/.github/workflows/run_tests.yml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/docs/source/api.rst
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/docs/source/conf.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/docs/source/index.rst
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/docs/source/intro.rst
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/docs/source/loaders.rst
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/docs/source/dev/index.rst
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/docs/source/dev/setup.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/data/__init__.py
--rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/data/detector1.py
--rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/data/hdf5.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/data/muon_data.py
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/data/periods.py
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/data/raw_data.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/data/sample.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/data/source.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/data/user.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/data/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/data/loader/__init__.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/data/loader/load_nxs2.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/test_helpers/__init__.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/src/MuonDataLib/test_helpers/nexus.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data/__init__.py
--rw-r--r--   0        0        0    10577 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data/detector1_test.py
--rw-r--r--   0        0        0     9592 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data/hdf5_test.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data/muon_data_test.py
--rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data/periods_test.py
--rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data/raw_data_test.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data/sample_test.py
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data/source_test.py
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data/user_test.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data/utils_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data/loader/__init__.py
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data/loader/load_nxs2_test.py
--rw-r--r--   0        0        0  1370476 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data_files/HIFI00180594.nxs
--rw-r--r--   0        0        0  1977434 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data_files/HIFI00183810.nxs
--rw-r--r--   0        0        0   560372 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data_files/HIFI42.nxs
--rw-r--r--   0        0        0  1084660 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data_files/HIFI51.nxs
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/data_files/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/system_tests/__init__.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/system_tests/multiperiod_test.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/system_tests/single_period_test.py
--rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/test/test_helpers/nexus_test.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/tools/conda_dict_to_yml.py
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/tools/create_conda_yml.py
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/tools/setup_helper.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/tools/version.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/README.md
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/pyproject.toml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 muondatalib-0.5.0b0/PKG-INFO
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/.readthedocs.yaml
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/MuonDataLib-dev.yml
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/MuonDataLib.yml
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/.github/release.yml
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/.github/workflows/flake8.yml
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/.github/workflows/label_merge_conflicts.yml
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/.github/workflows/merge.yml
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/.github/workflows/release_next.yml
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/.github/workflows/run_tests.yml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/docs/source/api.rst
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/docs/source/conf.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/docs/source/index.rst
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/docs/source/intro.rst
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/docs/source/loaders.rst
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/docs/source/dev/index.rst
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/docs/source/dev/setup.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/src/MuonDataLib/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/src/MuonDataLib/data/__init__.py
+-rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/src/MuonDataLib/data/detector1.py
+-rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/src/MuonDataLib/data/hdf5.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/src/MuonDataLib/data/muon_data.py
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/src/MuonDataLib/data/periods.py
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/src/MuonDataLib/data/raw_data.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/src/MuonDataLib/data/sample.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/src/MuonDataLib/data/source.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/src/MuonDataLib/data/user.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/src/MuonDataLib/data/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/src/MuonDataLib/data/loader/__init__.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/src/MuonDataLib/data/loader/load_nxs2.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/src/MuonDataLib/test_helpers/__init__.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/src/MuonDataLib/test_helpers/nexus.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/test/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/test/data/__init__.py
+-rw-r--r--   0        0        0    10577 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/test/data/detector1_test.py
+-rw-r--r--   0        0        0     9592 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/test/data/hdf5_test.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/test/data/muon_data_test.py
+-rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/test/data/periods_test.py
+-rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/test/data/raw_data_test.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/test/data/sample_test.py
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/test/data/source_test.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/test/data/user_test.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/test/data/utils_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/test/data/loader/__init__.py
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/test/data/loader/load_nxs2_test.py
+-rw-r--r--   0        0        0  1370476 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/test/data_files/HIFI00180594.nxs
+-rw-r--r--   0        0        0  1977434 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/test/data_files/HIFI00183810.nxs
+-rw-r--r--   0        0        0   560372 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/test/data_files/HIFI42.nxs
+-rw-r--r--   0        0        0  1084660 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/test/data_files/HIFI51.nxs
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/test/data_files/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/test/system_tests/__init__.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/test/system_tests/multiperiod_test.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/test/system_tests/single_period_test.py
+-rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/test/test_helpers/nexus_test.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/tools/conda_dict_to_yml.py
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/tools/create_conda_yml.py
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/tools/setup_helper.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/tools/version.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/README.md
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/pyproject.toml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 muondatalib-0.5.0b1/PKG-INFO
```

### Comparing `muondatalib-0.5.0b0/.pre-commit-config.yaml` & `muondatalib-0.5.0b1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/.github/PULL_REQUEST_TEMPLATE.md` & `muondatalib-0.5.0b1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/.github/workflows/label_merge_conflicts.yml` & `muondatalib-0.5.0b1/.github/workflows/label_merge_conflicts.yml`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/.github/workflows/merge.yml` & `muondatalib-0.5.0b1/.github/workflows/merge.yml`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/.github/workflows/release_next.yml` & `muondatalib-0.5.0b1/.github/workflows/release_next.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 name: Build and upload release to PyPI
 
 on:
   push:
     branches:
-    - 'main'
-  pull_request:
-    branches:
-      - 'main'
+      - 'release-next'
 
 permissions:
   contents: write
 
 jobs:
   update_version:
     name: update version
```

### Comparing `muondatalib-0.5.0b0/.github/workflows/run_tests.yml` & `muondatalib-0.5.0b1/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/docs/source/conf.py` & `muondatalib-0.5.0b1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/docs/source/index.rst` & `muondatalib-0.5.0b1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/docs/source/dev/setup.rst` & `muondatalib-0.5.0b1/docs/source/dev/setup.rst`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/src/MuonDataLib/data/detector1.py` & `muondatalib-0.5.0b1/src/MuonDataLib/data/detector1.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/src/MuonDataLib/data/hdf5.py` & `muondatalib-0.5.0b1/src/MuonDataLib/data/hdf5.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/src/MuonDataLib/data/muon_data.py` & `muondatalib-0.5.0b1/src/MuonDataLib/data/muon_data.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/src/MuonDataLib/data/periods.py` & `muondatalib-0.5.0b1/src/MuonDataLib/data/periods.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/src/MuonDataLib/data/raw_data.py` & `muondatalib-0.5.0b1/src/MuonDataLib/data/raw_data.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/src/MuonDataLib/data/sample.py` & `muondatalib-0.5.0b1/src/MuonDataLib/data/sample.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/src/MuonDataLib/data/source.py` & `muondatalib-0.5.0b1/src/MuonDataLib/data/source.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/src/MuonDataLib/data/user.py` & `muondatalib-0.5.0b1/src/MuonDataLib/data/user.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/src/MuonDataLib/data/utils.py` & `muondatalib-0.5.0b1/src/MuonDataLib/data/utils.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/src/MuonDataLib/data/loader/load_nxs2.py` & `muondatalib-0.5.0b1/src/MuonDataLib/data/loader/load_nxs2.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/src/MuonDataLib/test_helpers/nexus.py` & `muondatalib-0.5.0b1/src/MuonDataLib/test_helpers/nexus.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/test/data/detector1_test.py` & `muondatalib-0.5.0b1/test/data/detector1_test.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/test/data/hdf5_test.py` & `muondatalib-0.5.0b1/test/data/hdf5_test.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/test/data/muon_data_test.py` & `muondatalib-0.5.0b1/test/data/muon_data_test.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/test/data/periods_test.py` & `muondatalib-0.5.0b1/test/data/periods_test.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/test/data/raw_data_test.py` & `muondatalib-0.5.0b1/test/data/raw_data_test.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/test/data/sample_test.py` & `muondatalib-0.5.0b1/test/data/sample_test.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/test/data/source_test.py` & `muondatalib-0.5.0b1/test/data/source_test.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/test/data/user_test.py` & `muondatalib-0.5.0b1/test/data/user_test.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/test/data/utils_test.py` & `muondatalib-0.5.0b1/test/data/utils_test.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/test/data/loader/load_nxs2_test.py` & `muondatalib-0.5.0b1/test/data/loader/load_nxs2_test.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/test/data_files/HIFI00180594.nxs` & `muondatalib-0.5.0b1/test/data_files/HIFI00180594.nxs`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/test/data_files/HIFI00183810.nxs` & `muondatalib-0.5.0b1/test/data_files/HIFI00183810.nxs`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/test/data_files/HIFI42.nxs` & `muondatalib-0.5.0b1/test/data_files/HIFI42.nxs`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/test/data_files/HIFI51.nxs` & `muondatalib-0.5.0b1/test/data_files/HIFI51.nxs`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/test/system_tests/multiperiod_test.py` & `muondatalib-0.5.0b1/test/system_tests/multiperiod_test.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/test/system_tests/single_period_test.py` & `muondatalib-0.5.0b1/test/system_tests/single_period_test.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/test/test_helpers/nexus_test.py` & `muondatalib-0.5.0b1/test/test_helpers/nexus_test.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/tools/conda_dict_to_yml.py` & `muondatalib-0.5.0b1/tools/conda_dict_to_yml.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/tools/create_conda_yml.py` & `muondatalib-0.5.0b1/tools/create_conda_yml.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/tools/setup_helper.py` & `muondatalib-0.5.0b1/tools/setup_helper.py`

 * *Files identical despite different names*

### Comparing `muondatalib-0.5.0b0/tools/version.py` & `muondatalib-0.5.0b1/tools/version.py`

 * *Files identical despite different names*

