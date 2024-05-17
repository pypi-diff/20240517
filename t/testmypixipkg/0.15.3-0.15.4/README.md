# Comparing `tmp/testmypixipkg-0.15.3.tar.gz` & `tmp/testmypixipkg-0.15.4.tar.gz`

## Comparing `testmypixipkg-0.15.3.tar` & `testmypixipkg-0.15.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/.gitattributes
--rw-r--r--   0        0        0     6121 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/CHANGELOG.md
--rw-r--r--   0        0        0   173757 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/pixi.lock
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/releaserc.toml
--rw-r--r--   0        0        0     7527 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/.github/workflows/main.yaml
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/src/testmypixipkg/__init__.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/src/testmypixipkg/__main__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/tests/test_say_hello.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/LICENSE
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/README.md
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/hatch.toml
--rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/pyproject.toml
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 testmypixipkg-0.15.3/PKG-INFO
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/.gitattributes
+-rw-r--r--   0        0        0     6274 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/CHANGELOG.md
+-rw-r--r--   0        0        0   173757 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/pixi.lock
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/releaserc.toml
+-rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/.github/workflows/main.yaml
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/src/testmypixipkg/__init__.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/src/testmypixipkg/__main__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/tests/test_say_hello.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/LICENSE
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/README.md
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/hatch.toml
+-rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/pyproject.toml
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 testmypixipkg-0.15.4/PKG-INFO
```

### Comparing `testmypixipkg-0.15.3/CHANGELOG.md` & `testmypixipkg-0.15.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # CHANGELOG
 
 
 
+## v0.15.4 (2024-05-17)
+
+### Fix
+
+* fix: verbose ([`e1015a1`](https://github.com/jjjermiah/pypackage/commit/e1015a10269a7efd97340b232e911fd9035386bf))
+
+
 ## v0.15.3 (2024-05-16)
 
 ### Fix
 
 * fix: nice env ([`3d81d90`](https://github.com/jjjermiah/pypackage/commit/3d81d90ce34fae0a9fef133202290725a5ddc24e))
 
 ### Unknown
```

### Comparing `testmypixipkg-0.15.3/pixi.lock` & `testmypixipkg-0.15.4/pixi.lock`

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
-  version: 0.15.3
+  version: 0.15.4
   path: .
-  sha256: 99c2416a18a1cc9404e634fd14593e2f4463c26cca18bbf5bfa3a054fc48be11
+  sha256: 11efb66ee6dbb8a4a6e067c1922837f27a18f910d3d0a61214db960065f90b59
   requires_dist:
   - rich
   - rich-click
   requires_python: '>=3.11'
   editable: true
 - kind: conda
   name: tk
```

### Comparing `testmypixipkg-0.15.3/releaserc.toml` & `testmypixipkg-0.15.4/releaserc.toml`

 * *Files identical despite different names*

### Comparing `testmypixipkg-0.15.3/.github/workflows/main.yaml` & `testmypixipkg-0.15.4/.github/workflows/main.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     steps:
       - uses: actions/checkout@v4
 
       - name: Install Pixi
         uses: prefix-dev/setup-pixi@v0.7.0
         with:
           environments: ${{ env.PIXI_ENV }}
+          log-level: "vv"
           pixi-version: v0.22.0
           cache: true
           cache-key: pixi-ENV_${{ env.PIXI_ENV }}-
           locked: false
 
       - name: Run pytest
         run: |
```

### Comparing `testmypixipkg-0.15.3/.gitignore` & `testmypixipkg-0.15.4/.gitignore`

 * *Files identical despite different names*

### Comparing `testmypixipkg-0.15.3/LICENSE` & `testmypixipkg-0.15.4/LICENSE`

 * *Files identical despite different names*

### Comparing `testmypixipkg-0.15.3/pyproject.toml` & `testmypixipkg-0.15.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "testmypixipkg"
-version = "0.15.3"
+version = "0.15.4"
 description = "Add a short description here"
 license = "MIT"
 readme = "README.md"
 authors = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
 requires-python = ">= 3.11"
 dependencies = ["rich", "rich-click"]
```

