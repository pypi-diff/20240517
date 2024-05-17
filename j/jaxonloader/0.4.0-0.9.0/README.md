# Comparing `tmp/jaxonloader-0.4.0.tar.gz` & `tmp/jaxonloader-0.9.0.tar.gz`

## Comparing `jaxonloader-0.4.0.tar` & `jaxonloader-0.9.0.tar`

### file list

```diff
@@ -1,27 +1,19 @@
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/mkdocs.yml
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/noxfile.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/.github/workflows/nox.yaml
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/.github/workflows/pre_commit.yaml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/docs/api.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/docs/future.md
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/docs/getting-started.md
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/docs/index.md
--rw-r--r--   0        0        0   126325 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/docs/images/performance.png
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/jaxonloader/__init__.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/jaxonloader/boto_client.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/jaxonloader/config.py
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/jaxonloader/dataloader.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/jaxonloader/dataset.py
--rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/jaxonloader/utils.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/jaxonloader/datasets/__init__.py
--rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/jaxonloader/datasets/_datasets.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/jaxonloader/datasets/download.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/tests/test_mnist.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/tests/test_slicing.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/tests/test_tinyshakespeare.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/LICENSE
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/README.md
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonloader-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jaxonloader-0.9.0/mkdocs.yml
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jaxonloader-0.9.0/noxfile.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jaxonloader-0.9.0/.github/workflows/nox.yaml
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 jaxonloader-0.9.0/.github/workflows/pre_commit.yaml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jaxonloader-0.9.0/docs/api.md
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jaxonloader-0.9.0/docs/future.md
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 jaxonloader-0.9.0/docs/getting-started.md
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jaxonloader-0.9.0/docs/index.md
+-rw-r--r--   0        0        0   126325 2020-02-02 00:00:00.000000 jaxonloader-0.9.0/docs/images/performance.png
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 jaxonloader-0.9.0/jaxonloader/__init__.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 jaxonloader-0.9.0/jaxonloader/dataloader.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 jaxonloader-0.9.0/jaxonloader/dataset.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jaxonloader-0.9.0/jaxonloader/utils.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jaxonloader-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonloader-0.9.0/LICENSE
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jaxonloader-0.9.0/README.md
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 jaxonloader-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 jaxonloader-0.9.0/PKG-INFO
```

### Comparing `jaxonloader-0.4.0/.github/workflows/nox.yaml` & `jaxonloader-0.9.0/.github/workflows/nox.yaml`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.4.0/docs/getting-started.md` & `jaxonloader-0.9.0/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.4.0/docs/index.md` & `jaxonloader-0.9.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.4.0/docs/images/performance.png` & `jaxonloader-0.9.0/docs/images/performance.png`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.4.0/jaxonloader/dataloader.py` & `jaxonloader-0.9.0/jaxonloader/dataloader.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.4.0/jaxonloader/dataset.py` & `jaxonloader-0.9.0/jaxonloader/dataset.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.4.0/.gitignore` & `jaxonloader-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.4.0/LICENSE` & `jaxonloader-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.4.0/pyproject.toml` & `jaxonloader-0.9.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,18 @@
 [project]
 name = "jaxonloader"
-version = "0.4.0"
+version = "0.9.0"
 description = "A dataloader, but for JAX/Numpy"
 readme = "README.md"
-requires-python ="~=3.10"
-license = {file = "LICENSE"}
-authors = [
-  {name = "Artur A. Galstyan", email = "mail@arturgalstyan.dev"},
-]
-dependencies=[
-  "jaxtyping",
-  "progressbar2",
-  "polars",
-  "beartype",
-  "typing_extensions",
-  "loguru",
-  "pyarrow",
-  "boto3",
-  "boto3-stubs",
-  "jax",
-  "jaxlib"
-]
+requires-python = "~=3.10"
+license = { file = "LICENSE" }
+authors = [{ name = "Artur A. Galstyan", email = "mail@arturgalstyan.dev" }]
+dependencies = ["jaxtyping", "beartype", "typing_extensions", "jax", "jaxlib"]
 [project.optional-dependencies]
-dev = [
-    "nox",
-    "pre-commit",
-    "pytest",
-    "mkdocs",
-]
-
+dev = ["nox", "pre-commit", "pytest", "mkdocs"]
 
 
 [tool.ruff]
 extend-include = ["*.ipynb"]
 src = []
 
 [tool.ruff.lint]
```

