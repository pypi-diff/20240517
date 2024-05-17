# Comparing `tmp/fairchem_data_oc-0.0.1.tar.gz` & `tmp/fairchem_data_oc-0.0.1b0.tar.gz`

## Comparing `fairchem_data_oc-0.0.1.tar` & `fairchem_data_oc-0.0.1b0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/src/fairchem/data/oc/.flake8
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/src/fairchem/data/oc/LICENSE.md
--rw-r--r--   0        0        0    10040 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/src/fairchem/data/oc/README.md
--rw-r--r--   0        0        0     8795 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/src/fairchem/data/oc/README_legacy_OC20.md
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/src/fairchem/data/oc/__init__.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/src/fairchem/data/oc/codecov.yml
--rw-r--r--   0        0        0    64730 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/src/fairchem/data/oc/ocdata_workflow.png
--rw-r--r--   0        0        0    14359 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/src/fairchem/data/oc/structure_generator.py
--rw-r--r--   0        0        0    58230 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/src/fairchem/data/oc/workflow_image.png
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/src/fairchem/data/oc/core/__init__.py
--rw-r--r--   0        0        0     6431 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/src/fairchem/data/oc/core/adsorbate.py
--rw-r--r--   0        0        0    21903 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/src/fairchem/data/oc/core/adsorbate_slab_config.py
--rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/src/fairchem/data/oc/core/bulk.py
--rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/src/fairchem/data/oc/core/multi_adsorbate_slab_config.py
--rw-r--r--   0        0        0    21698 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/src/fairchem/data/oc/core/slab.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/src/fairchem/data/oc/databases/__init__.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/src/fairchem/data/oc/databases/update.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/src/fairchem/data/oc/databases/pkls/__init__.py
--rw-r--r--   0        0        0    52517 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/src/fairchem/data/oc/databases/pkls/adsorbates.pkl
--rw-r--r--   0        0        0 36088635 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/src/fairchem/data/oc/databases/pkls/bulks.pkl
--rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/src/fairchem/data/oc/scripts/precompute_sample_structures.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/src/fairchem/data/oc/tests/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/src/fairchem/data/oc/utils/__init__.py
--rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/src/fairchem/data/oc/utils/flag_anomaly.py
--rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/src/fairchem/data/oc/utils/vasp.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/.gitignore
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/.flake8
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/LICENSE.md
+-rw-r--r--   0        0        0    10383 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/README.md
+-rw-r--r--   0        0        0     8795 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/README_legacy_OC20.md
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/__init__.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/codecov.yml
+-rw-r--r--   0        0        0    64730 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/ocdata_workflow.png
+-rw-r--r--   0        0        0    14359 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/structure_generator.py
+-rw-r--r--   0        0        0    58230 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/workflow_image.png
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/core/__init__.py
+-rw-r--r--   0        0        0     6431 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/core/adsorbate.py
+-rw-r--r--   0        0        0    21903 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/core/adsorbate_slab_config.py
+-rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/core/bulk.py
+-rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/core/multi_adsorbate_slab_config.py
+-rw-r--r--   0        0        0    21698 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/core/slab.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/databases/__init__.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/databases/update.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/databases/pkls/__init__.py
+-rw-r--r--   0        0        0    52517 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/databases/pkls/adsorbates.pkl
+-rw-r--r--   0        0        0 36088635 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/databases/pkls/bulks.pkl
+-rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/scripts/precompute_sample_structures.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/tests/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/utils/__init__.py
+-rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/utils/flag_anomaly.py
+-rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/utils/vasp.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/.gitignore
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/pyproject.toml
+-rw-r--r--   0        0        0    10670 2020-02-02 00:00:00.000000 fairchem_data_oc-0.0.1b0/PKG-INFO
```

### Comparing `fairchem_data_oc-0.0.1/src/fairchem/data/oc/LICENSE.md` & `fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fairchem_data_oc-0.0.1/src/fairchem/data/oc/README.md` & `fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/Open-Catalyst-Project/Open-Catalyst-Dataset/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/Open-Catalyst-Project/Open-Catalyst-Dataset/tree/main)
 [![codecov](https://codecov.io/gh/Open-Catalyst-Project/Open-Catalyst-Dataset/branch/main/graph/badge.svg?token=IZ7J729L6S)](https://codecov.io/gh/Open-Catalyst-Project/Open-Catalyst-Dataset/tree/main)
 
 # Open-Catalyst-Dataset
 
 This repository hosts the adsorbate-catalyst input generation workflow used in the [Open Catalyst Project](https://opencatalystproject.org/).
 
-## Install
+## Setup
 
-To install just run in your favorite environment with python >= 3.9
-* `pip install fairchem-data-oc`
+The easiest way to install prerequisites is via [conda](https://conda.io/docs/index.html). After installing [conda](http://conda.pydata.org/), run the following commands:
+
+* Create a new environment: `conda create -n ocp python=3.9`
+* Activate the newly created environment: `conda activate ocp`
+* Install specific versions of Pymatgen and ASE: `pip install pymatgen==2023.5.10 ase==3.22.1`
+* Clone this repo and install with: `pip install -e .`
 
 ## Workflow
 
 The codebase supports the following workflow to generate adsorbate-catalyst input configurations.
 
 1. Initialize a bulk:
     - By providing an atoms object, or
```

### Comparing `fairchem_data_oc-0.0.1/src/fairchem/data/oc/README_legacy_OC20.md` & `fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/README_legacy_OC20.md`

 * *Files identical despite different names*

### Comparing `fairchem_data_oc-0.0.1/src/fairchem/data/oc/ocdata_workflow.png` & `fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/ocdata_workflow.png`

 * *Files identical despite different names*

### Comparing `fairchem_data_oc-0.0.1/src/fairchem/data/oc/structure_generator.py` & `fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/structure_generator.py`

 * *Files identical despite different names*

### Comparing `fairchem_data_oc-0.0.1/src/fairchem/data/oc/workflow_image.png` & `fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/workflow_image.png`

 * *Files identical despite different names*

### Comparing `fairchem_data_oc-0.0.1/src/fairchem/data/oc/core/adsorbate.py` & `fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/core/adsorbate.py`

 * *Files identical despite different names*

### Comparing `fairchem_data_oc-0.0.1/src/fairchem/data/oc/core/adsorbate_slab_config.py` & `fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/core/adsorbate_slab_config.py`

 * *Files identical despite different names*

### Comparing `fairchem_data_oc-0.0.1/src/fairchem/data/oc/core/bulk.py` & `fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/core/bulk.py`

 * *Files identical despite different names*

### Comparing `fairchem_data_oc-0.0.1/src/fairchem/data/oc/core/multi_adsorbate_slab_config.py` & `fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/core/multi_adsorbate_slab_config.py`

 * *Files identical despite different names*

### Comparing `fairchem_data_oc-0.0.1/src/fairchem/data/oc/core/slab.py` & `fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/core/slab.py`

 * *Files identical despite different names*

### Comparing `fairchem_data_oc-0.0.1/src/fairchem/data/oc/databases/update.py` & `fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/databases/update.py`

 * *Files identical despite different names*

### Comparing `fairchem_data_oc-0.0.1/src/fairchem/data/oc/databases/pkls/adsorbates.pkl` & `fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/databases/pkls/adsorbates.pkl`

 * *Files identical despite different names*

### Comparing `fairchem_data_oc-0.0.1/src/fairchem/data/oc/databases/pkls/bulks.pkl` & `fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/databases/pkls/bulks.pkl`

 * *Files identical despite different names*

### Comparing `fairchem_data_oc-0.0.1/src/fairchem/data/oc/scripts/precompute_sample_structures.py` & `fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/scripts/precompute_sample_structures.py`

 * *Files identical despite different names*

### Comparing `fairchem_data_oc-0.0.1/src/fairchem/data/oc/utils/flag_anomaly.py` & `fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/utils/flag_anomaly.py`

 * *Files identical despite different names*

### Comparing `fairchem_data_oc-0.0.1/src/fairchem/data/oc/utils/vasp.py` & `fairchem_data_oc-0.0.1b0/src/fairchem/data/oc/utils/vasp.py`

 * *Files identical despite different names*

### Comparing `fairchem_data_oc-0.0.1/.gitignore` & `fairchem_data_oc-0.0.1b0/.gitignore`

 * *Files identical despite different names*

### Comparing `fairchem_data_oc-0.0.1/pyproject.toml` & `fairchem_data_oc-0.0.1b0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -3,26 +3,17 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "fairchem-data-oc"
 dynamic = ["version", "readme"]
 description = "Code for generating adsorbate-catalyst input configurations"
 license = {text = "MIT License"}
-dependencies = [
-    "numpy>=1.25.0",
-    "scipy",
-    "matplotlib",
-    "ase",  #  this was pinned to 3.22.1
-    "pymatgen>=2023.10.3",  # this was pinned to 2023.5.10
-    "tqdm"
-]
 
 [project.urls]
 repository = "https://github.com/FAIR-Chem/fairchem/tree/main/src/fairchem/data/oc"
-documentation = "https://fair-chem.github.io/"
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.version.raw-options]
 root = "../../"
 git_describe_command = 'git describe --tags --match  fairchem_data_oc-*'
```

### Comparing `fairchem_data_oc-0.0.1/PKG-INFO` & `fairchem_data_oc-0.0.1b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 Metadata-Version: 2.3
 Name: fairchem-data-oc
-Version: 0.0.1
+Version: 0.0.1b0
 Summary: Code for generating adsorbate-catalyst input configurations
 Project-URL: repository, https://github.com/FAIR-Chem/fairchem/tree/main/src/fairchem/data/oc
-Project-URL: documentation, https://fair-chem.github.io/
 License: MIT License
-Requires-Dist: ase
-Requires-Dist: matplotlib
-Requires-Dist: numpy>=1.25.0
-Requires-Dist: pymatgen>=2023.10.3
-Requires-Dist: scipy
-Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/Open-Catalyst-Project/Open-Catalyst-Dataset/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/Open-Catalyst-Project/Open-Catalyst-Dataset/tree/main)
 [![codecov](https://codecov.io/gh/Open-Catalyst-Project/Open-Catalyst-Dataset/branch/main/graph/badge.svg?token=IZ7J729L6S)](https://codecov.io/gh/Open-Catalyst-Project/Open-Catalyst-Dataset/tree/main)
 
 # Open-Catalyst-Dataset
 
 This repository hosts the adsorbate-catalyst input generation workflow used in the [Open Catalyst Project](https://opencatalystproject.org/).
 
-## Install
+## Setup
 
-To install just run in your favorite environment with python >= 3.9
-* `pip install fairchem-data-oc`
+The easiest way to install prerequisites is via [conda](https://conda.io/docs/index.html). After installing [conda](http://conda.pydata.org/), run the following commands:
+
+* Create a new environment: `conda create -n ocp python=3.9`
+* Activate the newly created environment: `conda activate ocp`
+* Install specific versions of Pymatgen and ASE: `pip install pymatgen==2023.5.10 ase==3.22.1`
+* Clone this repo and install with: `pip install -e .`
 
 ## Workflow
 
 The codebase supports the following workflow to generate adsorbate-catalyst input configurations.
 
 1. Initialize a bulk:
     - By providing an atoms object, or
```

