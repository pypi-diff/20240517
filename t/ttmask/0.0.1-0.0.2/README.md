# Comparing `tmp/ttmask-0.0.1.tar.gz` & `tmp/ttmask-0.0.2.tar.gz`

## Comparing `ttmask-0.0.1.tar` & `ttmask-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 ttmask-0.0.1/.copier-answers.yml
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 ttmask-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 ttmask-0.0.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 ttmask-0.0.1/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 ttmask-0.0.1/.github/dependabot.yml
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 ttmask-0.0.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 ttmask-0.0.1/src/ttmask/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 ttmask-0.0.1/src/ttmask/_cli.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 ttmask-0.0.1/src/ttmask/py.typed
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 ttmask-0.0.1/src/ttmask/sphere.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ttmask-0.0.1/tests/test_ttmask.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 ttmask-0.0.1/.gitignore
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 ttmask-0.0.1/LICENSE
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 ttmask-0.0.1/README.md
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 ttmask-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 ttmask-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 ttmask-0.0.2/.copier-answers.yml
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 ttmask-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 ttmask-0.0.2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 ttmask-0.0.2/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 ttmask-0.0.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 ttmask-0.0.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 ttmask-0.0.2/src/ttmask/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 ttmask-0.0.2/src/ttmask/_cli.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 ttmask-0.0.2/src/ttmask/cylinder.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 ttmask-0.0.2/src/ttmask/py.typed
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 ttmask-0.0.2/src/ttmask/sphere.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ttmask-0.0.2/tests/test_ttmask.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 ttmask-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 ttmask-0.0.2/LICENSE
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 ttmask-0.0.2/README.md
+-rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 ttmask-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 ttmask-0.0.2/PKG-INFO
```

### Comparing `ttmask-0.0.1/.pre-commit-config.yaml` & `ttmask-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ttmask-0.0.1/.github/workflows/ci.yml` & `ttmask-0.0.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ttmask-0.0.1/src/ttmask/sphere.py` & `ttmask-0.0.2/src/ttmask/sphere.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from ._cli import cli
 import numpy as np
 import einops
-import napari
 import typer
 from scipy.ndimage import distance_transform_edt
 import mrcfile
 
 
 @cli.command(name='sphere')
 def sphere(
@@ -35,9 +34,8 @@
 
     distance_from_edge = distance_transform_edt(mask == 0)
     boundary_pixels = (distance_from_edge <= soft_edge_size) & (distance_from_edge != 0)
     normalised_distance_from_edge = (distance_from_edge[boundary_pixels] / soft_edge_size) * np.pi
 
     mask[boundary_pixels] = (0.5 * np.cos(normalised_distance_from_edge) + 0.5)
 
-    #   mrcfile.read("bla.mrc")
     mrcfile.write("sphere.mrc", mask, voxel_size=4, overwrite=True)
```

### Comparing `ttmask-0.0.1/.gitignore` & `ttmask-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ttmask-0.0.1/LICENSE` & `ttmask-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ttmask-0.0.1/README.md` & `ttmask-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ttmask-0.0.1/pyproject.toml` & `ttmask-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     "Typing :: Typed",
 ]
 # add your package dependencies here
 dependencies = [
     "numpy",
     "typer",
     "einops",
-    "napari",
+    "mrcfile",
 ]
 
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
 # "extras" (e.g. for `pip install .[test]`)
 [project.optional-dependencies]
 # add dependencies used for testing here
 test = ["pytest", "pytest-cov"]
```

### Comparing `ttmask-0.0.1/PKG-INFO` & `ttmask-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ttmask
-Version: 0.0.1
+Version: 0.0.2
 Summary: CLI tool for mask creation in cryo-EM/ET
 Project-URL: homepage, https://github.com/teamtomo/ttmask
 Project-URL: repository, https://github.com/teamtomo/ttmask
 Author-email: Miles Graham <miles.graham@balliol.ox.ac.uk>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: einops
-Requires-Dist: napari
+Requires-Dist: mrcfile
 Requires-Dist: numpy
 Requires-Dist: typer
 Provides-Extra: dev
 Requires-Dist: ipython; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pdbpp; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
```

