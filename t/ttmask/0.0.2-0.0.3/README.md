# Comparing `tmp/ttmask-0.0.2.tar.gz` & `tmp/ttmask-0.0.3.tar.gz`

## Comparing `ttmask-0.0.2.tar` & `ttmask-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 ttmask-0.0.2/.copier-answers.yml
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 ttmask-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 ttmask-0.0.2/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 ttmask-0.0.2/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 ttmask-0.0.2/.github/dependabot.yml
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 ttmask-0.0.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 ttmask-0.0.2/src/ttmask/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 ttmask-0.0.2/src/ttmask/_cli.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 ttmask-0.0.2/src/ttmask/cylinder.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 ttmask-0.0.2/src/ttmask/py.typed
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 ttmask-0.0.2/src/ttmask/sphere.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ttmask-0.0.2/tests/test_ttmask.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 ttmask-0.0.2/.gitignore
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 ttmask-0.0.2/LICENSE
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 ttmask-0.0.2/README.md
--rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 ttmask-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 ttmask-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 ttmask-0.0.3/.copier-answers.yml
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 ttmask-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 ttmask-0.0.3/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 ttmask-0.0.3/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 ttmask-0.0.3/.github/dependabot.yml
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 ttmask-0.0.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 ttmask-0.0.3/src/ttmask/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 ttmask-0.0.3/src/ttmask/_cli.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 ttmask-0.0.3/src/ttmask/cylinder.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 ttmask-0.0.3/src/ttmask/py.typed
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 ttmask-0.0.3/src/ttmask/sphere.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ttmask-0.0.3/tests/test_ttmask.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 ttmask-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 ttmask-0.0.3/LICENSE
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 ttmask-0.0.3/README.md
+-rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 ttmask-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 ttmask-0.0.3/PKG-INFO
```

### Comparing `ttmask-0.0.2/.pre-commit-config.yaml` & `ttmask-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ttmask-0.0.2/.github/workflows/ci.yml` & `ttmask-0.0.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ttmask-0.0.2/src/ttmask/cylinder.py` & `ttmask-0.0.3/src/ttmask/cylinder.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     soft_edge_size: int = typer.Option(...),
 ):
     cylinder_outer_radius = cylinder_outer_diameter / 2
     cylinder_inner_radius = cylinder_inner_diameter / 2
 
     c = boxsize // 2
     center = np.array([c, c, c])
-    mask = np.zeros(shape=(boxsize, boxsize, boxsize))
+    mask = np.zeros(shape=(boxsize, boxsize, boxsize), dtype=np.float32)
 
     # 3d positions of all voxels
     positions = np.indices([boxsize, boxsize, boxsize])
     positions = einops.rearrange(positions, 'zyx d h w -> d h w zyx')
 
     print('calculating distance')
     difference = np.abs(positions - center)  # (100, 100, 100, 3)
```

### Comparing `ttmask-0.0.2/src/ttmask/sphere.py` & `ttmask-0.0.3/src/ttmask/sphere.py`

 * *Files identical despite different names*

### Comparing `ttmask-0.0.2/.gitignore` & `ttmask-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ttmask-0.0.2/LICENSE` & `ttmask-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ttmask-0.0.2/README.md` & `ttmask-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ttmask-0.0.2/pyproject.toml` & `ttmask-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 ]
 # add your package dependencies here
 dependencies = [
     "numpy",
     "typer",
     "einops",
     "mrcfile",
+    "scipy",
 ]
 
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
 # "extras" (e.g. for `pip install .[test]`)
 [project.optional-dependencies]
 # add dependencies used for testing here
 test = ["pytest", "pytest-cov"]
```

### Comparing `ttmask-0.0.2/PKG-INFO` & `ttmask-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ttmask
-Version: 0.0.2
+Version: 0.0.3
 Summary: CLI tool for mask creation in cryo-EM/ET
 Project-URL: homepage, https://github.com/teamtomo/ttmask
 Project-URL: repository, https://github.com/teamtomo/ttmask
 Author-email: Miles Graham <miles.graham@balliol.ox.ac.uk>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: einops
 Requires-Dist: mrcfile
 Requires-Dist: numpy
+Requires-Dist: scipy
 Requires-Dist: typer
 Provides-Extra: dev
 Requires-Dist: ipython; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pdbpp; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: rich; extra == 'dev'
```

