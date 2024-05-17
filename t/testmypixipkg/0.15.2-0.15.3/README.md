# Comparing `tmp/testmypixipkg-0.15.2.tar.gz` & `tmp/testmypixipkg-0.15.3.tar.gz`

## Comparing `testmypixipkg-0.15.2.tar` & `testmypixipkg-0.15.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 testmypixipkg-0.15.2/.gitattributes
--rw-r--r--   0        0        0     5841 2020-02-02 00:00:00.000000 testmypixipkg-0.15.2/CHANGELOG.md
--rw-r--r--   0        0        0   173757 2020-02-02 00:00:00.000000 testmypixipkg-0.15.2/pixi.lock
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 testmypixipkg-0.15.2/releaserc.toml
--rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 testmypixipkg-0.15.2/.github/workflows/main.yaml
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 testmypixipkg-0.15.2/src/testmypixipkg/__init__.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 testmypixipkg-0.15.2/src/testmypixipkg/__main__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 testmypixipkg-0.15.2/tests/test_say_hello.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 testmypixipkg-0.15.2/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 testmypixipkg-0.15.2/LICENSE
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 testmypixipkg-0.15.2/README.md
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 testmypixipkg-0.15.2/hatch.toml
--rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 testmypixipkg-0.15.2/pyproject.toml
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 testmypixipkg-0.15.2/PKG-INFO
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/.gitattributes
+-rw-r--r--   0        0        0     6121 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/CHANGELOG.md
+-rw-r--r--   0        0        0   173757 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/pixi.lock
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/releaserc.toml
+-rw-r--r--   0        0        0     7527 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/.github/workflows/main.yaml
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/src/testmypixipkg/__init__.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/src/testmypixipkg/__main__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/tests/test_say_hello.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/LICENSE
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/README.md
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/hatch.toml
+-rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/pyproject.toml
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/PKG-INFO
```

### Comparing `testmypixipkg-0.15.2/CHANGELOG.md` & `testmypixipkg-0.15.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # CHANGELOG
 
 
 
+## v0.15.3 (2024-05-16)
+
+### Fix
+
+* fix: nice env ([`3d81d90`](https://github.com/jjjermiah/pypackage/commit/3d81d90ce34fae0a9fef133202290725a5ddc24e))
+
+### Unknown
+
+* add dev ([`6d5d10e`](https://github.com/jjjermiah/pypackage/commit/6d5d10ed69e74d8cbd4e3770d2462f73d99f1b0d))
+
+
 ## v0.15.2 (2024-05-16)
 
 ### Chore
 
 * chore: lock ([`79ca798`](https://github.com/jjjermiah/pypackage/commit/79ca7989542568d1dbcce0795552c09801f98704))
 
 ### Fix
```

### Comparing `testmypixipkg-0.15.2/pixi.lock` & `testmypixipkg-0.15.3/pixi.lock`

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
-  version: 0.15.2
+  version: 0.15.3
   path: .
-  sha256: 4b9c9b1400f47fd34b9c3806a4119a8d1939f26fa9820cb5e62728461155f8f0
+  sha256: 99c2416a18a1cc9404e634fd14593e2f4463c26cca18bbf5bfa3a054fc48be11
   requires_dist:
   - rich
   - rich-click
   requires_python: '>=3.11'
   editable: true
 - kind: conda
   name: tk
```

### Comparing `testmypixipkg-0.15.2/releaserc.toml` & `testmypixipkg-0.15.3/releaserc.toml`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,19 @@
 logging_use_named_masks = false
 major_on_zero = true
 allow_zero_version = true
 tag_format = "v{version}"
 
 [semantic_release.branches.main]
 match = "(main|master)"
+
+[semantic_release.branches.develop]
+match = "(dev|develop)"
 prerelease_token = "rc"
-prerelease = false
+prerelease = true
 
 [semantic_release.changelog]
 template_dir = "templates"
 changelog_file = "CHANGELOG.md"
 exclude_commit_patterns = []
 
 [semantic_release.changelog.environment]
```

### Comparing `testmypixipkg-0.15.2/.github/workflows/main.yaml` & `testmypixipkg-0.15.3/.github/workflows/main.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -5,39 +5,38 @@
   push:
     # push to any branch *
     branches: [main]
   pull_request:
     branches: [main, development]
 
 jobs:
-
   ################################################################################################
   # Unit-Tests: Run unit tests using pytest
   ################################################################################################
   Unit-Tests:
     runs-on: ${{ matrix.os }}
     timeout-minutes: 15 # Consider increasing timeout
-
+    env:
+      PIXI_ENV: "dev"
     strategy:
       matrix:
         os: [ubuntu-latest]
-        environments: [dev]
         # os: [ubuntu-latest, macos-latest, macos-14, windows-latest]
         # python-version: ["3.12", "3.11", "3.10"]
 
     steps:
       - uses: actions/checkout@v4
 
       - name: Install Pixi
         uses: prefix-dev/setup-pixi@v0.7.0
         with:
-          environments: ${{ matrix.environments}}
+          environments: ${{ env.PIXI_ENV }}
           pixi-version: v0.22.0
           cache: true
-          cache-key: pixi-ENV_${{ matrix.environments }}-
+          cache-key: pixi-ENV_${{ env.PIXI_ENV }}-
           locked: false
 
       - name: Run pytest
         run: |
           pixi run which python
           pixi run test
 
@@ -50,28 +49,29 @@
           path: coverage-report
 
   ################################################################################################
   # Ruff: Run ruff linter
   ################################################################################################
   Ruff:
     runs-on: ubuntu-latest
+    env:
+      PIXI_ENV: "dev"
     strategy:
       matrix:
         os: [ubuntu-latest]
-        environments: [dev]
 
     steps:
       - uses: actions/checkout@v4
       - name: Install Pixi
         uses: prefix-dev/setup-pixi@v0.7.0
         with:
-          environments: ${{ matrix.environments}}
+          environments: ${{ env.PIXI_ENV }}
           pixi-version: v0.22.0
           cache: true
-          cache-key: pixi-ENV_${{ matrix.environments }}-
+          cache-key: pixi-ENV_${{ env.PIXI_ENV }}-
           locked: false
 
       - name: Run Ruff
         run: pixi run style
 
   ################################################################################################
   # Semantic-Release: Run semantic-release to automate versioning and publishing
@@ -125,33 +125,34 @@
           root_options: "-v --config releaserc.toml"
 
   ################################################################################################
   # Publish-To-PyPi & Test-PyPi-Installation: Publish to PyPI and test installation
   ################################################################################################
   Publish-To-PyPi:
     needs: Semantic-Release
+    env:
+      PIXI_ENV: "publish"
     if: needs.Semantic-Release.outputs.released == 'true'
     strategy:
       matrix:
         os: [ubuntu-latest]
-        environments: [publish]
 
     runs-on: ${{ matrix.os }}
     steps:
       - name: Checkout the code with tag ${{ needs.Semantic-Release.outputs.tag }}
         uses: actions/checkout@v4
         with:
           ref: ${{ needs.Semantic-Release.outputs.tag }}
 
       - name: Install Pixi
         uses: prefix-dev/setup-pixi@v0.7.0
         with:
-          environments: ${{ matrix.environments}}
+          environments: ${{ env.PIXI_ENV }}
           pixi-version: v0.22.0
-          cache-key: pixi-ENV_${{ matrix.environments }}-
+          cache-key: pixi-ENV_${{ env.PIXI_ENV }}-
           cache: true
           locked: false
 
       - name: Publish to PyPI
         env:
           HATCH_INDEX_USER: __token__
           HATCH_INDEX_AUTH: ${{ secrets.PYPI_API_TOKEN }}
@@ -184,35 +185,35 @@
           pip install testmypixipkg
 
   ################################################################################################
   # Publish-To-Test-PyPi & Test-TestPypi-Installation: Publish to TestPyPI and test installation
   ################################################################################################
   Publish-To-Test-PyPi:
     needs: Semantic-Release
-
+    env:
+      PIXI_ENV: "publish"
     if: needs.Semantic-Release.outputs.released == 'true'
     strategy:
       matrix:
         os: [ubuntu-latest]
-        environments: [publish]
 
     runs-on: ${{ matrix.os }}
 
     steps:
       - name: Checkout the code with tag ${{ needs.Semantic-Release.outputs.tag }}
         uses: actions/checkout@v4
         with:
           ref: ${{ needs.Semantic-Release.outputs.tag }}
 
       - name: Install Pixi
         uses: prefix-dev/setup-pixi@v0.7.0
         with:
-          environments: ${{ matrix.environments}}
+          environments: ${{ env.PIXI_ENV }}
           pixi-version: v0.22.0
-          cache-key: pixi-ENV_${{ matrix.environments }}-
+          cache-key: pixi-ENV_${{ env.PIXI_ENV }}-
           cache: true
           locked: false
 
       - name: Publish to TestPyPI
         env:
           HATCH_INDEX_USER: __token__
           HATCH_INDEX_AUTH: ${{ secrets.TEST_PYPI_API_TOKEN }}
```

### Comparing `testmypixipkg-0.15.2/.gitignore` & `testmypixipkg-0.15.3/.gitignore`

 * *Files identical despite different names*

### Comparing `testmypixipkg-0.15.2/LICENSE` & `testmypixipkg-0.15.3/LICENSE`

 * *Files identical despite different names*

### Comparing `testmypixipkg-0.15.2/pyproject.toml` & `testmypixipkg-0.15.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "testmypixipkg"
-version = "0.15.2"
+version = "0.15.3"
 description = "Add a short description here"
 license = "MIT"
 readme = "README.md"
 authors = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
 requires-python = ">= 3.11"
 dependencies = ["rich", "rich-click"]
 
@@ -68,17 +68,16 @@
 
 ####################################################################################################
 #################################### RELEASE & BUILD ###############################################
 [tool.pixi.feature.release.dependencies]
 python-semantic-release = ">=8.5.1"
 
 [tool.pixi.feature.release.tasks]
-semver = { cmd = "echo 'Next Version is: $(semantic-release -c releaserc.toml version --print)'", inputs = [
-  "src",
-] }
+# Semver task will only work on the main or dev/develop branch (see releaserc.toml:branches)
+semver = { cmd = 'echo "Next Version is: $(semantic-release -c releaserc.toml version --print)"' }
 
 [tool.pixi.feature.build.dependencies]
 hatch = "*"
 
 [tool.pixi.feature.build.tasks]
 # Builds the package and publishes it to the test.pypi.org repository
 build = { cmd = "hatch build --clean", inputs = ["src"], outputs = ["dist/*"] }
```

