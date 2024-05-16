# Comparing `tmp/testmypixipkg-0.15.0.tar.gz` & `tmp/testmypixipkg-0.15.1.tar.gz`

## Comparing `testmypixipkg-0.15.0.tar` & `testmypixipkg-0.15.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/.gitattributes
--rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/CHANGELOG.md
--rw-r--r--   0        0        0   173757 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/pixi.lock
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/releaserc.toml
--rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/.github/workflows/main.yaml
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/src/testmypixipkg/__init__.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/src/testmypixipkg/__main__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/tests/test_say_hello.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/LICENSE
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/README.md
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/hatch.toml
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/pyproject.toml
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 testmypixipkg-0.15.0/PKG-INFO
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 testmypixipkg-0.15.1/.gitattributes
+-rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 testmypixipkg-0.15.1/CHANGELOG.md
+-rw-r--r--   0        0        0   173757 2020-02-02 00:00:00.000000 testmypixipkg-0.15.1/pixi.lock
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 testmypixipkg-0.15.1/releaserc.toml
+-rw-r--r--   0        0        0     7454 2020-02-02 00:00:00.000000 testmypixipkg-0.15.1/.github/workflows/main.yaml
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 testmypixipkg-0.15.1/src/testmypixipkg/__init__.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 testmypixipkg-0.15.1/src/testmypixipkg/__main__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 testmypixipkg-0.15.1/tests/test_say_hello.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 testmypixipkg-0.15.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 testmypixipkg-0.15.1/LICENSE
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 testmypixipkg-0.15.1/README.md
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 testmypixipkg-0.15.1/hatch.toml
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 testmypixipkg-0.15.1/pyproject.toml
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 testmypixipkg-0.15.1/PKG-INFO
```

### Comparing `testmypixipkg-0.15.0/CHANGELOG.md` & `testmypixipkg-0.15.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # CHANGELOG
 
 
 
+## v0.15.1 (2024-05-16)
+
+### Fix
+
+* fix: cache prefix ([`2080a9a`](https://github.com/jjjermiah/pypackage/commit/2080a9ab5f651fdc02be1dfbae10d6c28a61727a))
+
+
 ## v0.15.0 (2024-05-16)
 
 ### Feature
 
 * feat: cache-key for envs ([`54efc26`](https://github.com/jjjermiah/pypackage/commit/54efc260ab3c5ad6ff6a1837da6d28e3e65f2f54))
```

### Comparing `testmypixipkg-0.15.0/pixi.lock` & `testmypixipkg-0.15.1/pixi.lock`

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
-  version: 0.15.0
+  version: 0.15.1
   path: .
-  sha256: 10db5f84c5f30c208f71e7151e37fcda10d78b14c4758a454a79eecb62d2a7cf
+  sha256: 92ad082e2b315d9a51edfe7c1d4f0ae3a50ffb03f1031cc6daf616893c9d9b5a
   requires_dist:
   - rich
   - rich-click
   requires_python: '>=3.11'
   editable: true
 - kind: conda
   name: tk
```

### Comparing `testmypixipkg-0.15.0/releaserc.toml` & `testmypixipkg-0.15.1/releaserc.toml`

 * *Files identical despite different names*

### Comparing `testmypixipkg-0.15.0/.github/workflows/main.yaml` & `testmypixipkg-0.15.1/.github/workflows/main.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,18 @@
   push:
     # push to any branch *
     branches: [main]
   pull_request:
     branches: [main, development]
 
 jobs:
+
+  ################################################################################################
+  # Unit-Tests: Run unit tests using pytest
+  ################################################################################################
   Unit-Tests:
     runs-on: ${{ matrix.os }}
     timeout-minutes: 15 # Consider increasing timeout
 
     strategy:
       matrix:
         os: [ubuntu-latest]
@@ -25,15 +29,15 @@
 
       - name: Install Pixi
         uses: prefix-dev/setup-pixi@v0.7.0
         with:
           environments: ${{ matrix.environments}}
           pixi-version: v0.22.0
           cache: true
-          cache-key: pixi-${{ runner.os }}-${{ matrix.environments }}
+          cache-key: pixi-ENV_${{ matrix.environments }}-
           locked: false
 
       - name: Run pytest
         run: |
           pixi run which python
           pixi run test
 
@@ -41,14 +45,17 @@
         # only upload if matrix.os is ubuntu-latest and matrix.python-version is 3.12
         if: matrix.os == 'ubuntu-latest' && matrix.python-version == '3.12'
         uses: actions/upload-artifact@v2
         with:
           name: coverage-report
           path: coverage-report
 
+  ################################################################################################
+  # Ruff: Run ruff linter
+  ################################################################################################
   Ruff:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         os: [ubuntu-latest]
         environments: [dev]
 
@@ -56,20 +63,23 @@
       - uses: actions/checkout@v4
       - name: Install Pixi
         uses: prefix-dev/setup-pixi@v0.7.0
         with:
           environments: ${{ matrix.environments}}
           pixi-version: v0.22.0
           cache: true
-          cache-key: pixi-${{ runner.os }}-${{ matrix.environments }}
+          cache-key: pixi-ENV_${{ matrix.environments }}-
           locked: false
 
       - name: Run Ruff
         run: pixi run style
 
+  ################################################################################################
+  # Semantic-Release: Run semantic-release to automate versioning and publishing
+  ################################################################################################
   Semantic-Release:
     permissions:
       contents: write
       packages: write
       issues: write
       pull-requests: write
 
@@ -110,14 +120,17 @@
       - name: Python Semantic Release
         id: release
         uses: python-semantic-release/python-semantic-release@master
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           root_options: "-v --config releaserc.toml"
 
+  ################################################################################################
+  # Publish-To-PyPi & Test-PyPi-Installation: Publish to PyPI and test installation
+  ################################################################################################
   Publish-To-PyPi:
     needs: Semantic-Release
     if: needs.Semantic-Release.outputs.released == 'true'
     strategy:
       matrix:
         os: [ubuntu-latest]
         environments: [publish]
@@ -165,14 +178,17 @@
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install using PyPI
         run: |
           pip install testmypixipkg
 
+  ################################################################################################
+  # Publish-To-Test-PyPi & Test-TestPypi-Installation: Publish to TestPyPI and test installation
+  ################################################################################################
   Publish-To-Test-PyPi:
     needs: Semantic-Release
 
     if: needs.Semantic-Release.outputs.released == 'true'
     strategy:
       matrix:
         os: [ubuntu-latest]
```

### Comparing `testmypixipkg-0.15.0/.gitignore` & `testmypixipkg-0.15.1/.gitignore`

 * *Files identical despite different names*

### Comparing `testmypixipkg-0.15.0/LICENSE` & `testmypixipkg-0.15.1/LICENSE`

 * *Files identical despite different names*

### Comparing `testmypixipkg-0.15.0/pyproject.toml` & `testmypixipkg-0.15.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "testmypixipkg"
-version = "0.15.0"
+version = "0.15.1"
 description = "Add a short description here"
 license = "MIT"
 readme = "README.md"
 authors = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
 requires-python = ">= 3.11"
 dependencies = ["rich", "rich-click"]
```

