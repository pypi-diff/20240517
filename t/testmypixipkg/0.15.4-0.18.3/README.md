# Comparing `tmp/testmypixipkg-0.15.4.tar.gz` & `tmp/testmypixipkg-0.18.3.tar.gz`

## Comparing `testmypixipkg-0.15.4.tar` & `testmypixipkg-0.18.3.tar`

### file list

```diff
@@ -1,14 +1,19 @@
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/.gitattributes
--rw-r--r--   0        0        0     6274 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/CHANGELOG.md
--rw-r--r--   0        0        0   173757 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/pixi.lock
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/releaserc.toml
--rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/.github/workflows/main.yaml
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/src/testmypixipkg/__init__.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/src/testmypixipkg/__main__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/tests/test_say_hello.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/LICENSE
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/README.md
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/hatch.toml
--rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/pyproject.toml
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/PKG-INFO
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 testmypixipkg-0.18.3/.gitattributes
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 testmypixipkg-0.18.3/mkdocs.yaml
+-rw-r--r--   0        0        0   173757 2020-02-02 00:00:00.000000 testmypixipkg-0.18.3/pixi.lock
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 testmypixipkg-0.18.3/releaserc.toml
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 testmypixipkg-0.18.3/ruff.toml
+-rw-r--r--   0        0        0     8698 2020-02-02 00:00:00.000000 testmypixipkg-0.18.3/.github/workflows/main.yaml
+-rw-r--r--   0        0        0    10446 2020-02-02 00:00:00.000000 testmypixipkg-0.18.3/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 testmypixipkg-0.18.3/docs/about.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 testmypixipkg-0.18.3/docs/index.md
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 testmypixipkg-0.18.3/src/testmypixipkg/__init__.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 testmypixipkg-0.18.3/src/testmypixipkg/__main__.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 testmypixipkg-0.18.3/src/testmypixipkg/cli.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 testmypixipkg-0.18.3/tests/test_say_hello.py
+-rw-r--r--   0        0        0     3215 2020-02-02 00:00:00.000000 testmypixipkg-0.18.3/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 testmypixipkg-0.18.3/LICENSE
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 testmypixipkg-0.18.3/README.md
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 testmypixipkg-0.18.3/hatch.toml
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 testmypixipkg-0.18.3/pyproject.toml
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 testmypixipkg-0.18.3/PKG-INFO
```

### Comparing `testmypixipkg-0.15.4/CHANGELOG.md` & `testmypixipkg-0.18.3/docs/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,115 @@
 # CHANGELOG
 
 
 
+## v0.18.3 (2024-05-17)
+
+### Fix
+
+* fix: lock ([`26dba1d`](https://github.com/jjjermiah/pypackage/commit/26dba1d47c1bb8085c010ea616040598932dac22))
+
+* fix: idk ([`c7603a4`](https://github.com/jjjermiah/pypackage/commit/c7603a436f4a2decfb1d35b2508ad715a5face2a))
+
+
+## v0.18.2 (2024-05-17)
+
+### Ci
+
+* ci: no needs ([`21b4659`](https://github.com/jjjermiah/pypackage/commit/21b465996fbc5085e5feedea3d0b22ad654b4817))
+
+### Fix
+
+* fix: no key ([`a730baf`](https://github.com/jjjermiah/pypackage/commit/a730baf6358c5e94b936f33f84ba954ee381a348))
+
+* fix: token ([`edd4e0f`](https://github.com/jjjermiah/pypackage/commit/edd4e0fea74ba473ce7bb9c08379b6e598136f0a))
+
+* fix: add token? ([`58f3c26`](https://github.com/jjjermiah/pypackage/commit/58f3c2638fa7e756e2e7ac4f078ee8303fb1f6b7))
+
+
+## v0.18.1 (2024-05-17)
+
+### Fix
+
+* fix: no pixi cache ([`f6bc401`](https://github.com/jjjermiah/pypackage/commit/f6bc401594d3d4f2e80622c65dbab60620216352))
+
+* fix: locks ([`a4f45c4`](https://github.com/jjjermiah/pypackage/commit/a4f45c4fae353ee684ef1050c37fbeb63f752c7c))
+
+* fix: token i think ([`12bf904`](https://github.com/jjjermiah/pypackage/commit/12bf904d6479b8ab575e99bfc616aae9f0d2c3c0))
+
+
+## v0.18.0 (2024-05-17)
+
+### Ci
+
+* ci: add permissions for docs ([`e399e91`](https://github.com/jjjermiah/pypackage/commit/e399e919e993a883dfbc9923bf443a2921bd57cc))
+
+* ci: revert ([`664ce2d`](https://github.com/jjjermiah/pypackage/commit/664ce2d84c812350920212784b69829440fe12a7))
+
+* ci: fix ([`7a29926`](https://github.com/jjjermiah/pypackage/commit/7a2992661be1292428bd1bb701a069b60f1808f7))
+
+* ci: test env version ref ([`4ac0388`](https://github.com/jjjermiah/pypackage/commit/4ac03881965008633bf4ae017946550e401c58f4))
+
+### Documentation
+
+* docs(config): update paths and refs for CHANGELOG.md ([`d53b9dd`](https://github.com/jjjermiah/pypackage/commit/d53b9ddd0c7bed293ddafcad1f9755f996f2a46b))
+
+### Feature
+
+* feat: looking good ([`2cc4ad0`](https://github.com/jjjermiah/pypackage/commit/2cc4ad0fa4e0ef91650bcfc5153729aa059a84e1))
+
+* feat: fix release ([`8e34988`](https://github.com/jjjermiah/pypackage/commit/8e349886fb0ff2acba5a68185573896183fbb208))
+
+* feat(project): expand README, clean dependencies, and update metadata ([`a409819`](https://github.com/jjjermiah/pypackage/commit/a409819b34141bb856bb83030569a5ba41d4f5b6))
+
+* feat: add docs ([`68b20ef`](https://github.com/jjjermiah/pypackage/commit/68b20ef0e35364e59a21d453718efd6bbce72e52))
+
+### Fix
+
+* fix: lock ([`2e48cc6`](https://github.com/jjjermiah/pypackage/commit/2e48cc63caf9e704d929c188e22e06da90670970))
+
+* fix: actually release ([`abd3250`](https://github.com/jjjermiah/pypackage/commit/abd325041562c2efaa65e756b9ae075d042b934a))
+
+* fix: force deploy docs ([`017b775`](https://github.com/jjjermiah/pypackage/commit/017b775dfb3c39f2817cbbb33353ed8a41b4ec38))
+
+* fix: publish nolock ([`756c4bc`](https://github.com/jjjermiah/pypackage/commit/756c4bc72ac53ca32658bc0046ab84b974ccfb16))
+
+* fix: lock ([`d3df023`](https://github.com/jjjermiah/pypackage/commit/d3df023154a21a59a7ea3ecf5ebd4516ff8968bf))
+
+### Unknown
+
+* fix:update lock ([`5c831fd`](https://github.com/jjjermiah/pypackage/commit/5c831fd80fd81e518601868cea5c161609685749))
+
+* `ci(github-actions): standardize env variable syntax` ([`ca14640`](https://github.com/jjjermiah/pypackage/commit/ca146401e0f58518066aadafcaf2863a835ae210))
+
+
+## v0.17.0 (2024-05-17)
+
+### Feature
+
+* feat: add cli module and separate ruff.toml ([`76190ff`](https://github.com/jjjermiah/pypackage/commit/76190ffd9f25207ced1d7e1502b459f65ae85e1e))
+
+### Unknown
+
+* chore (pixi.lock): upgrade testmypixipkg version from 0.15.4 to 0.16.0 and update sha256 checksum to match new version ([`0bc4889`](https://github.com/jjjermiah/pypackage/commit/0bc48893ca5f02882a8ec7aafc6b7638d19dbafe))
+
+
+## v0.16.0 (2024-05-17)
+
+### Feature
+
+* feat: debug ([`90b11cb`](https://github.com/jjjermiah/pypackage/commit/90b11cba1355a310bf830e1d6e542ac62cf009fb))
+
+### Fix
+
+* fix: lock ([`4806afc`](https://github.com/jjjermiah/pypackage/commit/4806afc6b7c9ec0e5f2febd98705e3ca690829d3))
+
+* fix: no lock ([`f7a3ca9`](https://github.com/jjjermiah/pypackage/commit/f7a3ca9b17490fd1087d68b6ae4f5c5fb29cf123))
+
+
 ## v0.15.4 (2024-05-17)
 
 ### Fix
 
 * fix: verbose ([`e1015a1`](https://github.com/jjjermiah/pypackage/commit/e1015a10269a7efd97340b232e911fd9035386bf))
```

### Comparing `testmypixipkg-0.15.4/pixi.lock` & `testmypixipkg-0.18.3/pixi.lock`

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
-  version: 0.15.4
+  version: 0.18.3
   path: .
-  sha256: 11efb66ee6dbb8a4a6e067c1922837f27a18f910d3d0a61214db960065f90b59
+  sha256: eae0d029bdbfae961384e9840ea287ed72d9b42201754f9da504d9259f8942b3
   requires_dist:
   - rich
   - rich-click
   requires_python: '>=3.11'
   editable: true
 - kind: conda
   name: tk
```

### Comparing `testmypixipkg-0.15.4/releaserc.toml` & `testmypixipkg-0.18.3/releaserc.toml`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [semantic_release.branches.develop]
 match = "(dev|develop)"
 prerelease_token = "rc"
 prerelease = true
 
 [semantic_release.changelog]
 template_dir = "templates"
-changelog_file = "CHANGELOG.md"
+changelog_file = "docs/CHANGELOG.md"
 exclude_commit_patterns = []
 
 [semantic_release.changelog.environment]
 block_start_string = "{%"
 block_end_string = "%}"
 variable_start_string = "{{"
 variable_end_string = "}}"
@@ -54,13 +54,13 @@
 minor_tags = ["feat"]
 patch_tags = ["fix", "perf"]
 default_bump_level = 0
 
 [semantic_release.remote]
 name = "origin"
 type = "github"
-ignore_token_for_push = true
+ignore_token_for_push = false
 insecure = false
 
 [semantic_release.publish]
 dist_glob_patterns = ["dist/*"]
 upload_to_vcs_release = true
```

### Comparing `testmypixipkg-0.15.4/.github/workflows/main.yaml` & `testmypixipkg-0.18.3/.github/workflows/main.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -26,19 +26,17 @@
     steps:
       - uses: actions/checkout@v4
 
       - name: Install Pixi
         uses: prefix-dev/setup-pixi@v0.7.0
         with:
           environments: ${{ env.PIXI_ENV }}
-          log-level: "vv"
           pixi-version: v0.22.0
-          cache: true
-          cache-key: pixi-ENV_${{ env.PIXI_ENV }}-
-          locked: false
+          cache: false
+          # cache-key: pixi-ENV_${{ env.PIXI_ENV }}-
 
       - name: Run pytest
         run: |
           pixi run which python
           pixi run test
 
       - name: Upload coverage report artifact to be used by Codecov
@@ -63,41 +61,79 @@
     steps:
       - uses: actions/checkout@v4
       - name: Install Pixi
         uses: prefix-dev/setup-pixi@v0.7.0
         with:
           environments: ${{ env.PIXI_ENV }}
           pixi-version: v0.22.0
-          cache: true
-          cache-key: pixi-ENV_${{ env.PIXI_ENV }}-
-          locked: false
+          cache: false
+          # cache-key: pixi-ENV_${{ env.PIXI_ENV }}-
 
       - name: Run Ruff
         run: pixi run style
 
   ################################################################################################
+  # Docs: Build and deploy mkdocs documentation
+  ################################################################################################
+  Docs:
+    runs-on: ubuntu-latest
+    env:
+      PIXI_ENV: "dev"
+
+    permissions:
+      # Need to give the action permission to write to the repository to deploy the docs
+      contents: write
+
+    strategy:
+      matrix:
+        os: [ubuntu-latest]
+
+    steps:
+      - name: Check-out repository
+        uses: actions/checkout@v4
+
+      - name: Configure Git Credentials
+        run: |
+          git config user.name github-actions[bot]
+          git config user.email github-actions[bot]@users.noreply.github.com
+
+      - name: Install Pixi
+        uses: prefix-dev/setup-pixi@v0.7.0
+        with:
+          environments: ${{ env.PIXI_ENV }}
+          pixi-version: v0.22.0
+          cache: false
+          # cache-key: pixi-ENV_${{ env.PIXI_ENV }}-
+
+      - name: Build and deploy documentation
+        run: pixi run doc-deploy
+
+  ################################################################################################
   # Semantic-Release: Run semantic-release to automate versioning and publishing
   ################################################################################################
   Semantic-Release:
     permissions:
+      # Read releases read-all
       contents: write
       packages: write
       issues: write
       pull-requests: write
 
-    needs: [Unit-Tests, Ruff]
+    # needs: [Unit-Tests, Ruff]
 
     # if pulling to main, deploy to PyPI
     if: github.ref == 'refs/heads/main'
 
+    env:
+      PIXI_ENV: "publish"
+
     strategy:
       matrix:
         os: [ubuntu-latest]
         python-version: ["3.12"]
-        environments: [publish]
 
     # Set up operating system
     runs-on: ${{ matrix.os }}
 
     # Concurrency is for preventing multiple runs of the same workflow
     concurrency: release
 
@@ -109,25 +145,29 @@
     # Define job steps
     steps:
       - name: Check-out repository
         uses: actions/checkout@v2
         with:
           fetch-depth: 0
 
-      - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+      - name: Install Pixi
+        uses: prefix-dev/setup-pixi@v0.7.0
+        env:
+          RUNNER_DEBUG: true
         with:
-          python-version: ${{ matrix.python-version }}
+          environments: ${{ env.PIXI_ENV }}
+          pixi-version: v0.22.0
+          cache: false
+          # cache-key: pixi-ENV_${{ env.PIXI_ENV }}-
 
-      - name: Python Semantic Release
+      - name: Run semantic-release
+        env:
+          GH_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         id: release
-        uses: python-semantic-release/python-semantic-release@master
-        with:
-          github_token: ${{ secrets.GITHUB_TOKEN }}
-          root_options: "-v --config releaserc.toml"
+        run: pixi run release
 
   ################################################################################################
   # Publish-To-PyPi & Test-PyPi-Installation: Publish to PyPI and test installation
   ################################################################################################
   Publish-To-PyPi:
     needs: Semantic-Release
     env:
@@ -145,17 +185,17 @@
           ref: ${{ needs.Semantic-Release.outputs.tag }}
 
       - name: Install Pixi
         uses: prefix-dev/setup-pixi@v0.7.0
         with:
           environments: ${{ env.PIXI_ENV }}
           pixi-version: v0.22.0
-          cache-key: pixi-ENV_${{ env.PIXI_ENV }}-
-          cache: true
-          locked: false
+          # cache-key: pixi-ENV_${{ env.PIXI_ENV }}-
+          cache: false
+          locked: false # wont be the same because of the tag
 
       - name: Publish to PyPI
         env:
           HATCH_INDEX_USER: __token__
           HATCH_INDEX_AUTH: ${{ secrets.PYPI_API_TOKEN }}
           HATCH_INDEX_REPO: https://upload.pypi.org/legacy/
         run: |
@@ -206,17 +246,17 @@
           ref: ${{ needs.Semantic-Release.outputs.tag }}
 
       - name: Install Pixi
         uses: prefix-dev/setup-pixi@v0.7.0
         with:
           environments: ${{ env.PIXI_ENV }}
           pixi-version: v0.22.0
-          cache-key: pixi-ENV_${{ env.PIXI_ENV }}-
-          cache: true
-          locked: false
+          # cache-key: pixi-ENV_${{ env.PIXI_ENV }}-
+          cache: false
+          locked: false # wont be the same because of the tag
 
       - name: Publish to TestPyPI
         env:
           HATCH_INDEX_USER: __token__
           HATCH_INDEX_AUTH: ${{ secrets.TEST_PYPI_API_TOKEN }}
         run: |
           pixi run publish-test
```

### Comparing `testmypixipkg-0.15.4/.gitignore` & `testmypixipkg-0.18.3/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -159,8 +159,12 @@
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 .pixi
 
 coverage-report
 recipe.yaml
-.ruff_cache
+.ruff_cache
+src/testmypixipkg/__pycache__/__init__.cpython-312.pyc
+**/__pycache__/*
+*./**/.pyc
+**.pyc
```

### Comparing `testmypixipkg-0.15.4/LICENSE` & `testmypixipkg-0.18.3/LICENSE`

 * *Files identical despite different names*

