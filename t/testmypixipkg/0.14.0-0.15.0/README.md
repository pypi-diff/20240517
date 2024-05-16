# Comparing `tmp/testmypixipkg-0.14.0.tar.gz` & `tmp/testmypixipkg-0.15.0.tar.gz`

## Comparing `testmypixipkg-0.14.0.tar` & `testmypixipkg-0.15.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/.gitattributes
--rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/CHANGELOG.md
--rw-r--r--   0        0        0   173757 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/pixi.lock
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/releaserc.toml
--rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/.github/workflows/main.yaml
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/src/testmypixipkg/__init__.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/src/testmypixipkg/__main__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/tests/test_say_hello.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/LICENSE
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/README.md
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/hatch.toml
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/pyproject.toml
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 testmypixipkg-0.14.0/PKG-INFO
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/.gitattributes
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/CHANGELOG.md
+-rw-r--r--   0        0        0   173757 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/pixi.lock
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/releaserc.toml
+-rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/.github/workflows/main.yaml
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/src/testmypixipkg/__init__.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/src/testmypixipkg/__main__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/tests/test_say_hello.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/LICENSE
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/README.md
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/hatch.toml
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/pyproject.toml
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/PKG-INFO
```

### Comparing `testmypixipkg-0.14.0/CHANGELOG.md` & `testmypixipkg-0.15.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # CHANGELOG
 
 
 
+## v0.15.0 (2024-05-16)
+
+### Feature
+
+* feat: cache-key for envs ([`54efc26`](https://github.com/jjjermiah/pypackage/commit/54efc260ab3c5ad6ff6a1837da6d28e3e65f2f54))
+
+
 ## v0.14.0 (2024-05-16)
 
 ### Feature
 
 * feat: add readme and license ([`922a78e`](https://github.com/jjjermiah/pypackage/commit/922a78e93feef2b0ee5daced1b18f461cf9a68b7))
```

### Comparing `testmypixipkg-0.14.0/pixi.lock` & `testmypixipkg-0.15.0/pixi.lock`

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
-  version: 0.14.0
+  version: 0.15.0
   path: .
-  sha256: e13ffddc5a342494e48b89ccab1b6d486fe14203503c6a0c6ad33c0430dba24d
+  sha256: 10db5f84c5f30c208f71e7151e37fcda10d78b14c4758a454a79eecb62d2a7cf
   requires_dist:
   - rich
   - rich-click
   requires_python: '>=3.11'
   editable: true
 - kind: conda
   name: tk
```

### Comparing `testmypixipkg-0.14.0/releaserc.toml` & `testmypixipkg-0.15.0/releaserc.toml`

 * *Files identical despite different names*

### Comparing `testmypixipkg-0.14.0/.github/workflows/main.yaml` & `testmypixipkg-0.15.0/.github/workflows/main.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -12,33 +12,28 @@
   Unit-Tests:
     runs-on: ${{ matrix.os }}
     timeout-minutes: 15 # Consider increasing timeout
 
     strategy:
       matrix:
         os: [ubuntu-latest]
-        python-version: ["3.12"]
         environments: [dev]
         # os: [ubuntu-latest, macos-latest, macos-14, windows-latest]
         # python-version: ["3.12", "3.11", "3.10"]
 
     steps:
       - uses: actions/checkout@v4
 
-      - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
-        with:
-          python-version: ${{ matrix.python-version }}
-
       - name: Install Pixi
         uses: prefix-dev/setup-pixi@v0.7.0
         with:
           environments: ${{ matrix.environments}}
           pixi-version: v0.22.0
           cache: true
+          cache-key: pixi-${{ runner.os }}-${{ matrix.environments }}
           locked: false
 
       - name: Run pytest
         run: |
           pixi run which python
           pixi run test
 
@@ -48,23 +43,30 @@
         uses: actions/upload-artifact@v2
         with:
           name: coverage-report
           path: coverage-report
 
   Ruff:
     runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        os: [ubuntu-latest]
+        environments: [dev]
+
     steps:
       - uses: actions/checkout@v4
       - name: Install Pixi
         uses: prefix-dev/setup-pixi@v0.7.0
         with:
-          environments: dev
+          environments: ${{ matrix.environments}}
           pixi-version: v0.22.0
           cache: true
+          cache-key: pixi-${{ runner.os }}-${{ matrix.environments }}
           locked: false
+
       - name: Run Ruff
         run: pixi run style
 
   Semantic-Release:
     permissions:
       contents: write
       packages: write
@@ -114,15 +116,14 @@
 
   Publish-To-PyPi:
     needs: Semantic-Release
     if: needs.Semantic-Release.outputs.released == 'true'
     strategy:
       matrix:
         os: [ubuntu-latest]
-        python-version: ["3.12"]
         environments: [publish]
 
     runs-on: ${{ matrix.os }}
     steps:
       - name: Checkout the code with tag ${{ needs.Semantic-Release.outputs.tag }}
         uses: actions/checkout@v4
         with:
@@ -171,15 +172,14 @@
   Publish-To-Test-PyPi:
     needs: Semantic-Release
 
     if: needs.Semantic-Release.outputs.released == 'true'
     strategy:
       matrix:
         os: [ubuntu-latest]
-        python-version: ["3.12"]
         environments: [publish]
 
     runs-on: ${{ matrix.os }}
 
     steps:
       - name: Checkout the code with tag ${{ needs.Semantic-Release.outputs.tag }}
         uses: actions/checkout@v4
```

### Comparing `testmypixipkg-0.14.0/.gitignore` & `testmypixipkg-0.15.0/.gitignore`

 * *Files identical despite different names*

### Comparing `testmypixipkg-0.14.0/LICENSE` & `testmypixipkg-0.15.0/LICENSE`

 * *Files identical despite different names*

### Comparing `testmypixipkg-0.14.0/pyproject.toml` & `testmypixipkg-0.15.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "testmypixipkg"
-version = "0.14.0"
+version = "0.15.0"
 description = "Add a short description here"
 license = "MIT"
 readme = "README.md"
 authors = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
 requires-python = ">= 3.11"
 dependencies = ["rich", "rich-click"]
```

