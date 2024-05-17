# Comparing `tmp/fairchem_applications_cattsunami-0.0.1.tar.gz` & `tmp/fairchem_applications_cattsunami-0.0.1b0.tar.gz`

## Comparing `fairchem_applications_cattsunami-0.0.1.tar` & `fairchem_applications_cattsunami-0.0.1b0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/DATASET.md
--rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/README.md
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/__init__.py
--rw-r--r--   0        0        0   771334 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/summary_fig.png
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/core/__init__.py
--rw-r--r--   0        0        0    69388 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/core/autoframe.py
--rw-r--r--   0        0        0    11428 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/core/ocpneb.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/core/reaction.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/databases/__init__.py
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/databases/desorptions_9Aug23.pkl
--rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/databases/dissociation_reactions_20Oct23.pkl
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/databases/transfers_5Sept23.pkl
--rw-r--r--   0        0        0    14572 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/run_validation/run_validation.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/run_validation/run_validation.sh
--rw-r--r--   0        0        0    35873 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/run_validation/mapping_files/desorption_mapping.pkl
--rw-r--r--   0        0        0    41063 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/run_validation/mapping_files/dissociation_mapping.pkl
--rw-r--r--   0        0        0    50571 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/run_validation/mapping_files/transfer_mapping.pkl
--rw-r--r--   0        0        0    82245 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/tutorial/dissociation_scheme.png
--rw-r--r--   0        0        0    10757 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/tutorial/workbook.ipynb
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1/.gitignore
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     6143 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/DATASET.md
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/README.md
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/__init__.py
+-rw-r--r--   0        0        0   771334 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/summary_fig.png
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/core/__init__.py
+-rw-r--r--   0        0        0    69388 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/core/autoframe.py
+-rw-r--r--   0        0        0    11428 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/core/ocpneb.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/core/reaction.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/databases/__init__.py
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/databases/desorptions_9Aug23.pkl
+-rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/databases/dissociation_reactions_20Oct23.pkl
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/databases/transfers_5Sept23.pkl
+-rw-r--r--   0        0        0    14572 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/run_validation/run_validation.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/run_validation/run_validation.sh
+-rw-r--r--   0        0        0    35873 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/run_validation/mapping_files/desorption_mapping.pkl
+-rw-r--r--   0        0        0    41063 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/run_validation/mapping_files/dissociation_mapping.pkl
+-rw-r--r--   0        0        0    50571 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/run_validation/mapping_files/transfer_mapping.pkl
+-rw-r--r--   0        0        0    82245 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/tutorial/dissociation_scheme.png
+-rw-r--r--   0        0        0    10757 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/tutorial/workbook.ipynb
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/pyproject.toml
+-rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 fairchem_applications_cattsunami-0.0.1b0/PKG-INFO
```

### Comparing `fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/DATASET.md` & `fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/DATASET.md`

 * *Files identical despite different names*

### Comparing `fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/README.md` & `fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,25 @@
 ## CatTSunami: Accelerating Transition State Energy Calculations with Pre-trained Graph Neural Networks
 
-![summary](https://github.com/FAIR-Chem/fairchem/blob/main/src/fairchem/applications/cattsunami/summary_fig.png)
+![summary](https://github.com/Open-Catalyst-Project/CatTSunami/blob/master/summary_fig.png)
 
 CatTSunami is a framework for high-throughput enumeration of nudged elastic band (NEB) frame sets. It was built for use with machine learned (ML) models trained on [OC20](https://arxiv.org/abs/2010.09990), which were demonstrated to be performant on this auxiliary task. To train your own model or obtain pre-trained checkpoints, please see [`fairchem-core`](https://github.com/FAIR-Chem/fairchem/tree/cattsunami-package/src/fairchem/core).
 
 This repository contains the validation dataset, framework for enumeration, and accompanying code to run ML-accelerated NEBs and validate new models. For more information, please read the manuscript [paper](https://arxiv.org/abs/2405.02078).
 
 ### Getting started
-Configured for use:
-1. Install fairchem-core and fairchem-data-oc [instructions](https://fair-chem.github.io/core/install.html)
-2. Pip innstall fairchem-applications-cattsunami 
-3. Check out the [tutorial notebook](https://github.com/FAIR-Chem/fairchem/tree/main/src/fairchem/applications/cattsunami/tutorial/workbook.ipynb)
-```
-pip install fairchem-applications-cattsunami
-```
-
-Configured for local development:
-1. Clone the [fairchem repo](https://github.com/FAIR-Chem/fairchem/tree/main) 
-2. Install `fairchem-data-oc` and `fairchem-core`:  [instructions](https://fair-chem.github.io/core/install.html)
+Configured for local development
+1. Clone the [`fairchem repo`](https://github.com/FAIR-Chem/fairchem/tree/main) 
+2. Install `fairchem-data-oc` and `fairchem-core`:  [`instructions`](https://fair-chem.github.io/core/install.html)
 3. Install this repository `pip install -e packages/fairchem-applications-cattsunami`
 4. Check out the [tutorial notebook](https://github.com/FAIR-Chem/fairchem/tree/main/src/fairchem/applications/cattsunami/tutorial/workbook.ipynb)
 
 
 ### Validation Dataset
-The validation dataset is comprised of 932 DFT NEB calculations to assess model performance on this important task. There are 3 different reaction classes considered: desorptions, dissociations, and transfers. For more information see the [dataset markdown file](https://github.com/FAIR-Chem/fairchem/blob/main/src/fairchem/applications/cattsunami/DATASET.md).
+The validation dataset is comprised of 932 DFT NEB calculations to assess model performance on this important task. There are 3 different reaction classes considered: desorptions, dissociations, and transfers. For more information see the [dataset markdown file](https://github.com/Open-Catalyst-Project/CatTSunami/blob/master/DATASET.md).
 
 |Splits |Size of compressed version (in bytes)  |Size of uncompressed version (in bytes)    | MD5 checksum (download link)   |
 |---    |---    |---    |---    |
 |ASE Trajectories   |1.5G  |6.3G   | [52af34a93758c82fae951e52af445089](https://dl.fbaipublicfiles.com/opencatalystproject/data/oc20neb/oc20neb_dft_trajectories_04_23_24.tar.gz)   |
```

### Comparing `fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/summary_fig.png` & `fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/summary_fig.png`

 * *Files identical despite different names*

### Comparing `fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/core/autoframe.py` & `fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/core/autoframe.py`

 * *Files identical despite different names*

### Comparing `fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/core/ocpneb.py` & `fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/core/ocpneb.py`

 * *Files identical despite different names*

### Comparing `fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/core/reaction.py` & `fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/core/reaction.py`

 * *Files identical despite different names*

### Comparing `fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/databases/desorptions_9Aug23.pkl` & `fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/databases/desorptions_9Aug23.pkl`

 * *Files identical despite different names*

### Comparing `fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/databases/dissociation_reactions_20Oct23.pkl` & `fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/databases/dissociation_reactions_20Oct23.pkl`

 * *Files identical despite different names*

### Comparing `fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/databases/transfers_5Sept23.pkl` & `fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/databases/transfers_5Sept23.pkl`

 * *Files identical despite different names*

### Comparing `fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/run_validation/run_validation.py` & `fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/run_validation/run_validation.py`

 * *Files identical despite different names*

### Comparing `fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/run_validation/mapping_files/desorption_mapping.pkl` & `fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/run_validation/mapping_files/desorption_mapping.pkl`

 * *Files identical despite different names*

### Comparing `fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/run_validation/mapping_files/dissociation_mapping.pkl` & `fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/run_validation/mapping_files/dissociation_mapping.pkl`

 * *Files identical despite different names*

### Comparing `fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/run_validation/mapping_files/transfer_mapping.pkl` & `fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/run_validation/mapping_files/transfer_mapping.pkl`

 * *Files identical despite different names*

### Comparing `fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/tutorial/dissociation_scheme.png` & `fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/tutorial/dissociation_scheme.png`

 * *Files identical despite different names*

### Comparing `fairchem_applications_cattsunami-0.0.1/src/fairchem/applications/cattsunami/tutorial/workbook.ipynb` & `fairchem_applications_cattsunami-0.0.1b0/src/fairchem/applications/cattsunami/tutorial/workbook.ipynb`

 * *Files identical despite different names*

### Comparing `fairchem_applications_cattsunami-0.0.1/.gitignore` & `fairchem_applications_cattsunami-0.0.1b0/.gitignore`

 * *Files identical despite different names*

### Comparing `fairchem_applications_cattsunami-0.0.1/pyproject.toml` & `fairchem_applications_cattsunami-0.0.1b0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -3,27 +3,17 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "fairchem-applications-cattsunami"
 dynamic = ["version", "readme"]
 description = "Accelerating Transition State Energy Calculations with Pre-trained Graph Neural Networks"
 license = {text = "MIT License"}
-dependencies = [
-    "torch>=2.2",
-    "numpy>=1.25.0",
-    "scipy",
-    "ase",
-    "networkx",
-    "fairchem-core",
-    "fairchem-data-oc"
-]
 
 [project.urls]
 repository = "http://github.com/Fair-Chem/src/fairchem/applications/cattsunami"
-documentation = "https://fair-chem.github.io/"
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.version.raw-options]
 root = "../../"
 git_describe_command = 'git describe --tags --match fairchem_applications_cattsunami-*'
```

### Comparing `fairchem_applications_cattsunami-0.0.1/PKG-INFO` & `fairchem_applications_cattsunami-0.0.1b0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,33 @@
 Metadata-Version: 2.3
 Name: fairchem-applications-cattsunami
-Version: 0.0.1
+Version: 0.0.1b0
 Summary: Accelerating Transition State Energy Calculations with Pre-trained Graph Neural Networks
 Project-URL: repository, http://github.com/Fair-Chem/src/fairchem/applications/cattsunami
-Project-URL: documentation, https://fair-chem.github.io/
 License: MIT License
-Requires-Dist: ase
-Requires-Dist: fairchem-core
-Requires-Dist: fairchem-data-oc
-Requires-Dist: networkx
-Requires-Dist: numpy>=1.25.0
-Requires-Dist: scipy
-Requires-Dist: torch>=2.2
 Description-Content-Type: text/markdown
 
 ## CatTSunami: Accelerating Transition State Energy Calculations with Pre-trained Graph Neural Networks
 
-![summary](https://github.com/FAIR-Chem/fairchem/blob/main/src/fairchem/applications/cattsunami/summary_fig.png)
+![summary](https://github.com/Open-Catalyst-Project/CatTSunami/blob/master/summary_fig.png)
 
 CatTSunami is a framework for high-throughput enumeration of nudged elastic band (NEB) frame sets. It was built for use with machine learned (ML) models trained on [OC20](https://arxiv.org/abs/2010.09990), which were demonstrated to be performant on this auxiliary task. To train your own model or obtain pre-trained checkpoints, please see [`fairchem-core`](https://github.com/FAIR-Chem/fairchem/tree/cattsunami-package/src/fairchem/core).
 
 This repository contains the validation dataset, framework for enumeration, and accompanying code to run ML-accelerated NEBs and validate new models. For more information, please read the manuscript [paper](https://arxiv.org/abs/2405.02078).
 
 ### Getting started
-Configured for use:
-1. Install fairchem-core and fairchem-data-oc [instructions](https://fair-chem.github.io/core/install.html)
-2. Pip innstall fairchem-applications-cattsunami 
-3. Check out the [tutorial notebook](https://github.com/FAIR-Chem/fairchem/tree/main/src/fairchem/applications/cattsunami/tutorial/workbook.ipynb)
-```
-pip install fairchem-applications-cattsunami
-```
-
-Configured for local development:
-1. Clone the [fairchem repo](https://github.com/FAIR-Chem/fairchem/tree/main) 
-2. Install `fairchem-data-oc` and `fairchem-core`:  [instructions](https://fair-chem.github.io/core/install.html)
+Configured for local development
+1. Clone the [`fairchem repo`](https://github.com/FAIR-Chem/fairchem/tree/main) 
+2. Install `fairchem-data-oc` and `fairchem-core`:  [`instructions`](https://fair-chem.github.io/core/install.html)
 3. Install this repository `pip install -e packages/fairchem-applications-cattsunami`
 4. Check out the [tutorial notebook](https://github.com/FAIR-Chem/fairchem/tree/main/src/fairchem/applications/cattsunami/tutorial/workbook.ipynb)
 
 
 ### Validation Dataset
-The validation dataset is comprised of 932 DFT NEB calculations to assess model performance on this important task. There are 3 different reaction classes considered: desorptions, dissociations, and transfers. For more information see the [dataset markdown file](https://github.com/FAIR-Chem/fairchem/blob/main/src/fairchem/applications/cattsunami/DATASET.md).
+The validation dataset is comprised of 932 DFT NEB calculations to assess model performance on this important task. There are 3 different reaction classes considered: desorptions, dissociations, and transfers. For more information see the [dataset markdown file](https://github.com/Open-Catalyst-Project/CatTSunami/blob/master/DATASET.md).
 
 |Splits |Size of compressed version (in bytes)  |Size of uncompressed version (in bytes)    | MD5 checksum (download link)   |
 |---    |---    |---    |---    |
 |ASE Trajectories   |1.5G  |6.3G   | [52af34a93758c82fae951e52af445089](https://dl.fbaipublicfiles.com/opencatalystproject/data/oc20neb/oc20neb_dft_trajectories_04_23_24.tar.gz)   |
```

