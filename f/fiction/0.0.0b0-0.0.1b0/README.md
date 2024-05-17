# Comparing `tmp/fiction-0.0.0b0.tar.gz` & `tmp/fiction-0.0.1b0.tar.gz`

## Comparing `fiction-0.0.0b0.tar` & `fiction-0.0.1b0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 fiction-0.0.0b0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fiction-0.0.0b0/src/fiction/__init__.py
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 fiction-0.0.0b0/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 fiction-0.0.0b0/LICENSE.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 fiction-0.0.0b0/README.md
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 fiction-0.0.0b0/pyproject.toml
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 fiction-0.0.0b0/PKG-INFO
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 fiction-0.0.1b0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fiction-0.0.1b0/src/fiction/__init__.py
+-rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 fiction-0.0.1b0/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 fiction-0.0.1b0/LICENSE.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 fiction-0.0.1b0/README.md
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 fiction-0.0.1b0/pyproject.toml
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 fiction-0.0.1b0/PKG-INFO
```

### Comparing `fiction-0.0.0b0/.gitignore` & `fiction-0.0.1b0/.gitignore`

 * *Files identical despite different names*

### Comparing `fiction-0.0.0b0/LICENSE.txt` & `fiction-0.0.1b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fiction-0.0.0b0/pyproject.toml` & `fiction-0.0.1b0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fiction"
-version = "0.0.0-beta"
+version = "0.0.1-beta"
 requires-python = ">=3.10"
 authors = [
   {name = "Lionel Garcia"},
 ]
 description = "Astronomical image processing with jax"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
```

### Comparing `fiction-0.0.0b0/PKG-INFO` & `fiction-0.0.1b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fiction
-Version: 0.0.0b0
+Version: 0.0.1b0
 Summary: Astronomical image processing with jax
 Project-URL: Homepage, https://example.com
 Project-URL: Documentation, https://readthedocs.org
 Project-URL: Repository, https://github.com/me/spam.git
 Project-URL: Bug Tracker, https://github.com/me/spam/issues
 Project-URL: Changelog, https://github.com/me/spam/blob/master/CHANGELOG.md
 Author: Lionel Garcia
```

