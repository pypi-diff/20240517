# Comparing `tmp/testmypixipkg-0.13.0.tar.gz` & `tmp/testmypixipkg-0.14.0.tar.gz`

## Comparing `testmypixipkg-0.13.0.tar` & `testmypixipkg-0.14.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 testmypixipkg-0.13.0/.gitattributes
--rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 testmypixipkg-0.13.0/CHANGELOG.md
--rw-r--r--   0        0        0   173757 2020-02-02 00:00:00.000000 testmypixipkg-0.13.0/pixi.lock
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 testmypixipkg-0.13.0/releaserc.toml
--rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 testmypixipkg-0.13.0/.github/workflows/main.yaml
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 testmypixipkg-0.13.0/src/testmypixipkg/__init__.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 testmypixipkg-0.13.0/src/testmypixipkg/__main__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 testmypixipkg-0.13.0/tests/test_say_hello.py
--rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 testmypixipkg-0.13.0/.gitignore
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 testmypixipkg-0.13.0/hatch.toml
--rw-r--r--   0        0        0     3674 2020-02-02 00:00:00.000000 testmypixipkg-0.13.0/pyproject.toml
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 testmypixipkg-0.13.0/PKG-INFO
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/.gitattributes
+-rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/CHANGELOG.md
+-rw-r--r--   0        0        0   173757 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/pixi.lock
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/releaserc.toml
+-rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/.github/workflows/main.yaml
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/src/testmypixipkg/__init__.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/src/testmypixipkg/__main__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/tests/test_say_hello.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/LICENSE
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/README.md
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/hatch.toml
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/pyproject.toml
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/PKG-INFO
```

### Comparing `testmypixipkg-0.13.0/CHANGELOG.md` & `testmypixipkg-0.14.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # CHANGELOG
 
 
 
+## v0.14.0 (2024-05-16)
+
+### Feature
+
+* feat: add readme and license ([`922a78e`](https://github.com/jjjermiah/pypackage/commit/922a78e93feef2b0ee5daced1b18f461cf9a68b7))
+
+
 ## v0.13.0 (2024-05-16)
 
 ### Feature
 
 * feat: add ruff to ci ([`2b61b24`](https://github.com/jjjermiah/pypackage/commit/2b61b2461e6960c7f75177bc39527a2981a32eee))
 
 * feat: add ruff ([`3db3a38`](https://github.com/jjjermiah/pypackage/commit/3db3a3853fd2864aa31b815646c97ad11af2e599))
```

### Comparing `testmypixipkg-0.13.0/pixi.lock` & `testmypixipkg-0.14.0/pixi.lock`

 * *Files 0% similar despite different names*

```diff
@@ -3755,17 +3755,17 @@
   license_family: Apache
   purls:
   - pkg:pypi/sniffio
   size: 15064
   timestamp: 1708953086199
 - kind: pypi
   name: testmypixipkg
-  version: 0.13.0
+  version: 0.14.0
   path: .
-  sha256: 9f068bcc440364193e03614acd70d31089ec41ac5811e1c43730c889bf557ea8
+  sha256: e13ffddc5a342494e48b89ccab1b6d486fe14203503c6a0c6ad33c0430dba24d
   requires_dist:
   - rich
   - rich-click
   requires_python: '>=3.11'
   editable: true
 - kind: conda
   name: tk
```

### Comparing `testmypixipkg-0.13.0/releaserc.toml` & `testmypixipkg-0.14.0/releaserc.toml`

 * *Files identical despite different names*

### Comparing `testmypixipkg-0.13.0/.github/workflows/main.yaml` & `testmypixipkg-0.14.0/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `testmypixipkg-0.13.0/.gitignore` & `testmypixipkg-0.14.0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -159,7 +159,8 @@
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 .pixi
 
 coverage-report
 recipe.yaml
+.ruff_cache
```

### Comparing `testmypixipkg-0.13.0/pyproject.toml` & `testmypixipkg-0.14.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 [project]
 name = "testmypixipkg"
-version = "0.13.0"
+version = "0.14.0"
 description = "Add a short description here"
+license = "MIT"
+readme = "README.md"
 authors = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
 requires-python = ">= 3.11"
 dependencies = ["rich", "rich-click"]
 
 [project.scripts]
 pypkg = "testmypixipkg.__main__:say_hello"
```

