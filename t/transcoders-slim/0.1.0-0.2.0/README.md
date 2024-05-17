# Comparing `tmp/transcoders_slim-0.1.0.tar.gz` & `tmp/transcoders_slim-0.2.0.tar.gz`

## Comparing `transcoders_slim-0.1.0.tar` & `transcoders_slim-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 transcoders_slim-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 transcoders_slim-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0   161756 2020-02-02 00:00:00.000000 transcoders_slim-0.1.0/pdm.lock
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 transcoders_slim-0.1.0/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 transcoders_slim-0.1.0/.github/workflows/tests.yaml
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 transcoders_slim-0.1.0/docs/setup.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transcoders_slim-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 transcoders_slim-0.1.0/tests/test_init.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 transcoders_slim-0.1.0/tests/test_load_pretrained.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 transcoders_slim-0.1.0/transcoders_slim/__init__.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 transcoders_slim-0.1.0/transcoders_slim/load_pretrained.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 transcoders_slim-0.1.0/transcoders_slim/transcoder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transcoders_slim-0.1.0/transcoders_slim/sae_training/__init__.py
--rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 transcoders_slim-0.1.0/transcoders_slim/sae_training/config.py
--rw-r--r--   0        0        0    28830 2020-02-02 00:00:00.000000 transcoders_slim-0.1.0/transcoders_slim/sae_training/sparse_autoencoder.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 transcoders_slim-0.1.0/.gitignore
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 transcoders_slim-0.1.0/README.md
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 transcoders_slim-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 transcoders_slim-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0   161756 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/pdm.lock
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/docs/setup.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/tests/test_init.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/tests/test_load_pretrained.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/transcoders_slim/__init__.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/transcoders_slim/load_pretrained.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/transcoders_slim/transcoder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/transcoders_slim/sae_training/__init__.py
+-rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/transcoders_slim/sae_training/config.py
+-rw-r--r--   0        0        0    28830 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/transcoders_slim/sae_training/sparse_autoencoder.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/README.md
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/PKG-INFO
```

### Comparing `transcoders_slim-0.1.0/CHANGELOG.md` & `transcoders_slim-0.2.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # CHANGELOG
 
 
 
+## v0.2.0 (2024-05-12)
+
+### Feature
+
+* feat: bump version ([`1c5da65`](https://github.com/dtch1997/transcoders-slim/commit/1c5da65a8d542b313c2f360b6f09262a35db3479))
+
+
 ## v0.1.0 (2024-05-12)
 
 ### Chore
 
 * chore: fix github badge ([`1cb5552`](https://github.com/dtch1997/transcoders-slim/commit/1cb55529c49bcc19acee8df35298a18bf06937e2))
 
 * chore: update readme, tests ([`2188dc3`](https://github.com/dtch1997/transcoders-slim/commit/2188dc36e03be98adb719bf6ace31bf789e1ad6f))
```

### Comparing `transcoders_slim-0.1.0/pdm.lock` & `transcoders_slim-0.2.0/pdm.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # This file is @generated by PDM.
 # It is not intended for manual editing.
 
 [metadata]
 groups = ["default", "test"]
 strategy = ["cross_platform", "inherit_metadata"]
 lock_version = "4.4.1"
-content_hash = "sha256:4a5335ae1f42369770824c6ed267e0f1b733d0f71f119b1e8315b5b403ffad6a"
+content_hash = "sha256:58e4698f3647a8f1ad33ab4f7f7e5edb0e2d98e779cc9f9dc8f7f73c3ec15771"
 
 [[package]]
 name = "accelerate"
-version = "0.30.0"
+version = "0.30.1"
 requires_python = ">=3.8.0"
 summary = "Accelerate"
 groups = ["default"]
 dependencies = [
     "huggingface-hub",
     "numpy>=1.17",
     "packaging>=20.0",
     "psutil",
     "pyyaml",
     "safetensors>=0.3.1",
     "torch>=1.10.0",
 ]
 files = [
-    {file = "accelerate-0.30.0-py3-none-any.whl", hash = "sha256:cd93902dc37a49952b4b8b324c5d53776c936fcd77b4b0162cf5ce55a4fc2721"},
-    {file = "accelerate-0.30.0.tar.gz", hash = "sha256:0f8e103a6ced54cd40af6bb2331ec922e42269d2778038dc564d53047b1386d2"},
+    {file = "accelerate-0.30.1-py3-none-any.whl", hash = "sha256:8dd4edd532a4dac72558c5fe6fe8cb70d0c8ec9e8733f48db97d51ee41cbe763"},
+    {file = "accelerate-0.30.1.tar.gz", hash = "sha256:96779c618889646b86dc928c9e55e86e50a7ccab59e1692e22096481977ae682"},
 ]
 
 [[package]]
 name = "aiohttp"
 version = "3.9.5"
 requires_python = ">=3.8"
 summary = "Async http client/server framework (asyncio)"
@@ -1001,21 +1001,21 @@
     {file = "pandas-2.2.2-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:43498c0bdb43d55cb162cdc8c06fac328ccb5d2eabe3cadeb3529ae6f0517c32"},
     {file = "pandas-2.2.2-cp312-cp312-win_amd64.whl", hash = "sha256:d187d355ecec3629624fccb01d104da7d7f391db0311145817525281e2804d23"},
     {file = "pandas-2.2.2.tar.gz", hash = "sha256:9e79019aba43cb4fda9e4d983f8e88ca0373adbb697ae9c6c43093218de28b54"},
 ]
 
 [[package]]
 name = "platformdirs"
-version = "4.2.1"
+version = "4.2.2"
 requires_python = ">=3.8"
 summary = "A small Python package for determining appropriate platform-specific dirs, e.g. a `user data dir`."
 groups = ["default", "test"]
 files = [
-    {file = "platformdirs-4.2.1-py3-none-any.whl", hash = "sha256:17d5a1161b3fd67b390023cb2d3b026bbd40abde6fdb052dfbd3a29c3ba22ee1"},
-    {file = "platformdirs-4.2.1.tar.gz", hash = "sha256:031cd18d4ec63ec53e82dceaac0417d218a6863f7745dfcc9efe7793b7039bdf"},
+    {file = "platformdirs-4.2.2-py3-none-any.whl", hash = "sha256:2d7a1657e36a80ea911db832a8a6ece5ee53d8de21edd5cc5879af6530b1bfee"},
+    {file = "platformdirs-4.2.2.tar.gz", hash = "sha256:38b7b51f512eed9e84a22788b4bce1de17c0adb134d6becb09836e37d8654cd3"},
 ]
 
 [[package]]
 name = "pluggy"
 version = "1.5.0"
 requires_python = ">=3.8"
 summary = "plugin and hook calling mechanisms for python"
@@ -1023,28 +1023,28 @@
 files = [
     {file = "pluggy-1.5.0-py3-none-any.whl", hash = "sha256:44e1ad92c8ca002de6377e165f3e0f1be63266ab4d554740532335b9d75ea669"},
     {file = "pluggy-1.5.0.tar.gz", hash = "sha256:2cffa88e94fdc978c4c574f15f9e59b7f4201d439195c3715ca9e2486f1d0cf1"},
 ]
 
 [[package]]
 name = "pre-commit"
-version = "3.7.0"
+version = "3.7.1"
 requires_python = ">=3.9"
 summary = "A framework for managing and maintaining multi-language pre-commit hooks."
 groups = ["test"]
 dependencies = [
     "cfgv>=2.0.0",
     "identify>=1.0.0",
     "nodeenv>=0.11.1",
     "pyyaml>=5.1",
     "virtualenv>=20.10.0",
 ]
 files = [
-    {file = "pre_commit-3.7.0-py2.py3-none-any.whl", hash = "sha256:5eae9e10c2b5ac51577c3452ec0a490455c45a0533f7960f993a0d01e59decab"},
-    {file = "pre_commit-3.7.0.tar.gz", hash = "sha256:e209d61b8acdcf742404408531f0c37d49d2c734fd7cff2d6076083d191cb060"},
+    {file = "pre_commit-3.7.1-py2.py3-none-any.whl", hash = "sha256:fae36fd1d7ad7d6a5a1c0b0d5adb2ed1a3bda5a21bf6c3e5372073d7a11cd4c5"},
+    {file = "pre_commit-3.7.1.tar.gz", hash = "sha256:8ca3ad567bc78a4972a3f1a477e94a79d4597e8140a6e0b651c5e33899c3654a"},
 ]
 
 [[package]]
 name = "protobuf"
 version = "4.25.3"
 requires_python = ">=3.8"
 summary = ""
@@ -1074,44 +1074,44 @@
     {file = "psutil-5.9.8-cp37-abi3-win_amd64.whl", hash = "sha256:8db4c1b57507eef143a15a6884ca10f7c73876cdf5d51e713151c1236a0e68cf"},
     {file = "psutil-5.9.8-cp38-abi3-macosx_11_0_arm64.whl", hash = "sha256:d16bbddf0693323b8c6123dd804100241da461e41d6e332fb0ba6058f630f8c8"},
     {file = "psutil-5.9.8.tar.gz", hash = "sha256:6be126e3225486dff286a8fb9a06246a5253f4c7c53b475ea5f5ac934e64194c"},
 ]
 
 [[package]]
 name = "pyarrow"
-version = "16.0.0"
+version = "16.1.0"
 requires_python = ">=3.8"
 summary = "Python library for Apache Arrow"
 groups = ["default"]
 dependencies = [
     "numpy>=1.16.6",
 ]
 files = [
-    {file = "pyarrow-16.0.0-cp310-cp310-macosx_10_15_x86_64.whl", hash = "sha256:22a1fdb1254e5095d629e29cd1ea98ed04b4bbfd8e42cc670a6b639ccc208b60"},
-    {file = "pyarrow-16.0.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:574a00260a4ed9d118a14770edbd440b848fcae5a3024128be9d0274dbcaf858"},
-    {file = "pyarrow-16.0.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c0815d0ddb733b8c1b53a05827a91f1b8bde6240f3b20bf9ba5d650eb9b89cdf"},
-    {file = "pyarrow-16.0.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:df0080339387b5d30de31e0a149c0c11a827a10c82f0c67d9afae3981d1aabb7"},
-    {file = "pyarrow-16.0.0-cp310-cp310-manylinux_2_28_aarch64.whl", hash = "sha256:edf38cce0bf0dcf726e074159c60516447e4474904c0033f018c1f33d7dac6c5"},
-    {file = "pyarrow-16.0.0-cp310-cp310-manylinux_2_28_x86_64.whl", hash = "sha256:91d28f9a40f1264eab2af7905a4d95320ac2f287891e9c8b0035f264fe3c3a4b"},
-    {file = "pyarrow-16.0.0-cp310-cp310-win_amd64.whl", hash = "sha256:99af421ee451a78884d7faea23816c429e263bd3618b22d38e7992c9ce2a7ad9"},
-    {file = "pyarrow-16.0.0-cp311-cp311-macosx_10_15_x86_64.whl", hash = "sha256:d22d0941e6c7bafddf5f4c0662e46f2075850f1c044bf1a03150dd9e189427ce"},
-    {file = "pyarrow-16.0.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:266ddb7e823f03733c15adc8b5078db2df6980f9aa93d6bb57ece615df4e0ba7"},
-    {file = "pyarrow-16.0.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5cc23090224b6594f5a92d26ad47465af47c1d9c079dd4a0061ae39551889efe"},
-    {file = "pyarrow-16.0.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:56850a0afe9ef37249d5387355449c0f94d12ff7994af88f16803a26d38f2016"},
-    {file = "pyarrow-16.0.0-cp311-cp311-manylinux_2_28_aarch64.whl", hash = "sha256:705db70d3e2293c2f6f8e84874b5b775f690465798f66e94bb2c07bab0a6bb55"},
-    {file = "pyarrow-16.0.0-cp311-cp311-manylinux_2_28_x86_64.whl", hash = "sha256:5448564754c154997bc09e95a44b81b9e31ae918a86c0fcb35c4aa4922756f55"},
-    {file = "pyarrow-16.0.0-cp311-cp311-win_amd64.whl", hash = "sha256:729f7b262aa620c9df8b9967db96c1575e4cfc8c25d078a06968e527b8d6ec05"},
-    {file = "pyarrow-16.0.0-cp312-cp312-macosx_10_15_x86_64.whl", hash = "sha256:fb8065dbc0d051bf2ae2453af0484d99a43135cadabacf0af588a3be81fbbb9b"},
-    {file = "pyarrow-16.0.0-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:20ce707d9aa390593ea93218b19d0eadab56390311cb87aad32c9a869b0e958c"},
-    {file = "pyarrow-16.0.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5823275c8addbbb50cd4e6a6839952682a33255b447277e37a6f518d6972f4e1"},
-    {file = "pyarrow-16.0.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1ab8b9050752b16a8b53fcd9853bf07d8daf19093533e990085168f40c64d978"},
-    {file = "pyarrow-16.0.0-cp312-cp312-manylinux_2_28_aarch64.whl", hash = "sha256:42e56557bc7c5c10d3e42c3b32f6cff649a29d637e8f4e8b311d334cc4326730"},
-    {file = "pyarrow-16.0.0-cp312-cp312-manylinux_2_28_x86_64.whl", hash = "sha256:2a7abdee4a4a7cfa239e2e8d721224c4b34ffe69a0ca7981354fe03c1328789b"},
-    {file = "pyarrow-16.0.0-cp312-cp312-win_amd64.whl", hash = "sha256:ef2f309b68396bcc5a354106741d333494d6a0d3e1951271849787109f0229a6"},
-    {file = "pyarrow-16.0.0.tar.gz", hash = "sha256:59bb1f1edbbf4114c72415f039f1359f1a57d166a331c3229788ccbfbb31689a"},
+    {file = "pyarrow-16.1.0-cp310-cp310-macosx_10_15_x86_64.whl", hash = "sha256:17e23b9a65a70cc733d8b738baa6ad3722298fa0c81d88f63ff94bf25eaa77b9"},
+    {file = "pyarrow-16.1.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:4740cc41e2ba5d641071d0ab5e9ef9b5e6e8c7611351a5cb7c1d175eaf43674a"},
+    {file = "pyarrow-16.1.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:98100e0268d04e0eec47b73f20b39c45b4006f3c4233719c3848aa27a03c1aef"},
+    {file = "pyarrow-16.1.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f68f409e7b283c085f2da014f9ef81e885d90dcd733bd648cfba3ef265961848"},
+    {file = "pyarrow-16.1.0-cp310-cp310-manylinux_2_28_aarch64.whl", hash = "sha256:a8914cd176f448e09746037b0c6b3a9d7688cef451ec5735094055116857580c"},
+    {file = "pyarrow-16.1.0-cp310-cp310-manylinux_2_28_x86_64.whl", hash = "sha256:48be160782c0556156d91adbdd5a4a7e719f8d407cb46ae3bb4eaee09b3111bd"},
+    {file = "pyarrow-16.1.0-cp310-cp310-win_amd64.whl", hash = "sha256:9cf389d444b0f41d9fe1444b70650fea31e9d52cfcb5f818b7888b91b586efff"},
+    {file = "pyarrow-16.1.0-cp311-cp311-macosx_10_15_x86_64.whl", hash = "sha256:d0ebea336b535b37eee9eee31761813086d33ed06de9ab6fc6aaa0bace7b250c"},
+    {file = "pyarrow-16.1.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:2e73cfc4a99e796727919c5541c65bb88b973377501e39b9842ea71401ca6c1c"},
+    {file = "pyarrow-16.1.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:bf9251264247ecfe93e5f5a0cd43b8ae834f1e61d1abca22da55b20c788417f6"},
+    {file = "pyarrow-16.1.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ddf5aace92d520d3d2a20031d8b0ec27b4395cab9f74e07cc95edf42a5cc0147"},
+    {file = "pyarrow-16.1.0-cp311-cp311-manylinux_2_28_aarch64.whl", hash = "sha256:25233642583bf658f629eb230b9bb79d9af4d9f9229890b3c878699c82f7d11e"},
+    {file = "pyarrow-16.1.0-cp311-cp311-manylinux_2_28_x86_64.whl", hash = "sha256:a33a64576fddfbec0a44112eaf844c20853647ca833e9a647bfae0582b2ff94b"},
+    {file = "pyarrow-16.1.0-cp311-cp311-win_amd64.whl", hash = "sha256:185d121b50836379fe012753cf15c4ba9638bda9645183ab36246923875f8d1b"},
+    {file = "pyarrow-16.1.0-cp312-cp312-macosx_10_15_x86_64.whl", hash = "sha256:2e51ca1d6ed7f2e9d5c3c83decf27b0d17bb207a7dea986e8dc3e24f80ff7d6f"},
+    {file = "pyarrow-16.1.0-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:06ebccb6f8cb7357de85f60d5da50e83507954af617d7b05f48af1621d331c9a"},
+    {file = "pyarrow-16.1.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b04707f1979815f5e49824ce52d1dceb46e2f12909a48a6a753fe7cafbc44a0c"},
+    {file = "pyarrow-16.1.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0d32000693deff8dc5df444b032b5985a48592c0697cb6e3071a5d59888714e2"},
+    {file = "pyarrow-16.1.0-cp312-cp312-manylinux_2_28_aarch64.whl", hash = "sha256:8785bb10d5d6fd5e15d718ee1d1f914fe768bf8b4d1e5e9bf253de8a26cb1628"},
+    {file = "pyarrow-16.1.0-cp312-cp312-manylinux_2_28_x86_64.whl", hash = "sha256:e1369af39587b794873b8a307cc6623a3b1194e69399af0efd05bb202195a5a7"},
+    {file = "pyarrow-16.1.0-cp312-cp312-win_amd64.whl", hash = "sha256:febde33305f1498f6df85e8020bca496d0e9ebf2093bab9e0f65e2b4ae2b3444"},
+    {file = "pyarrow-16.1.0.tar.gz", hash = "sha256:15fbb22ea96d11f0b5768504a3f961edab25eaf4197c341720c4a387f6c60315"},
 ]
 
 [[package]]
 name = "pyarrow-hotfix"
 version = "0.6"
 requires_python = ">=3.5"
 summary = ""
@@ -1130,24 +1130,24 @@
 files = [
     {file = "pygments-2.18.0-py3-none-any.whl", hash = "sha256:b8e6aca0523f3ab76fee51799c488e38782ac06eafcf95e7ba832985c8e7b13a"},
     {file = "pygments-2.18.0.tar.gz", hash = "sha256:786ff802f32e91311bff3889f6e9a86e81505fe99f2735bb6d60ae0c5004f199"},
 ]
 
 [[package]]
 name = "pyright"
-version = "1.1.361"
+version = "1.1.363"
 requires_python = ">=3.7"
 summary = "Command line wrapper for pyright"
 groups = ["test"]
 dependencies = [
     "nodeenv>=1.6.0",
 ]
 files = [
-    {file = "pyright-1.1.361-py3-none-any.whl", hash = "sha256:c50fc94ce92b5c958cfccbbe34142e7411d474da43d6c14a958667e35b9df7ea"},
-    {file = "pyright-1.1.361.tar.gz", hash = "sha256:1d67933315666b05d230c85ea8fb97aaa2056e4092a13df87b7765bb9e8f1a8d"},
+    {file = "pyright-1.1.363-py3-none-any.whl", hash = "sha256:d3b8d73c8d230e26cc3523862f3398032a0c39a00d7bb69dc0f595f8e888fd01"},
+    {file = "pyright-1.1.363.tar.gz", hash = "sha256:00a8f0ae0e339473bb0488f8a2a2dcdf574e94a16cd7b4390d49d144714d8db2"},
 ]
 
 [[package]]
 name = "pytest"
 version = "8.2.0"
 requires_python = ">=3.8"
 summary = "pytest: simple powerful testing with Python"
@@ -1220,66 +1220,66 @@
     {file = "PyYAML-6.0.1-cp312-cp312-win32.whl", hash = "sha256:d483d2cdf104e7c9fa60c544d92981f12ad66a457afae824d146093b8c294c54"},
     {file = "PyYAML-6.0.1-cp312-cp312-win_amd64.whl", hash = "sha256:0d3304d8c0adc42be59c5f8a4d9e3d7379e6955ad754aa9d6ab7a398b59dd1df"},
     {file = "PyYAML-6.0.1.tar.gz", hash = "sha256:bfdf460b1736c775f2ba9f6a92bca30bc2095067b8a9d77876d1fad6cc3b4a43"},
 ]
 
 [[package]]
 name = "regex"
-version = "2024.4.28"
+version = "2024.5.15"
 requires_python = ">=3.8"
 summary = "Alternative regular expression module, to replace re."
 groups = ["default"]
 files = [
-    {file = "regex-2024.4.28-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:cd196d056b40af073d95a2879678585f0b74ad35190fac04ca67954c582c6b61"},
-    {file = "regex-2024.4.28-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:8bb381f777351bd534462f63e1c6afb10a7caa9fa2a421ae22c26e796fe31b1f"},
-    {file = "regex-2024.4.28-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:47af45b6153522733aa6e92543938e97a70ce0900649ba626cf5aad290b737b6"},
-    {file = "regex-2024.4.28-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:99d6a550425cc51c656331af0e2b1651e90eaaa23fb4acde577cf15068e2e20f"},
-    {file = "regex-2024.4.28-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:bf29304a8011feb58913c382902fde3395957a47645bf848eea695839aa101b7"},
-    {file = "regex-2024.4.28-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:92da587eee39a52c91aebea8b850e4e4f095fe5928d415cb7ed656b3460ae79a"},
-    {file = "regex-2024.4.28-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6277d426e2f31bdbacb377d17a7475e32b2d7d1f02faaecc48d8e370c6a3ff31"},
-    {file = "regex-2024.4.28-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:28e1f28d07220c0f3da0e8fcd5a115bbb53f8b55cecf9bec0c946eb9a059a94c"},
-    {file = "regex-2024.4.28-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:aaa179975a64790c1f2701ac562b5eeb733946eeb036b5bcca05c8d928a62f10"},
-    {file = "regex-2024.4.28-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:6f435946b7bf7a1b438b4e6b149b947c837cb23c704e780c19ba3e6855dbbdd3"},
-    {file = "regex-2024.4.28-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:19d6c11bf35a6ad077eb23852827f91c804eeb71ecb85db4ee1386825b9dc4db"},
-    {file = "regex-2024.4.28-cp310-cp310-musllinux_1_1_ppc64le.whl", hash = "sha256:fdae0120cddc839eb8e3c15faa8ad541cc6d906d3eb24d82fb041cfe2807bc1e"},
-    {file = "regex-2024.4.28-cp310-cp310-musllinux_1_1_s390x.whl", hash = "sha256:e672cf9caaf669053121f1766d659a8813bd547edef6e009205378faf45c67b8"},
-    {file = "regex-2024.4.28-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:f57515750d07e14743db55d59759893fdb21d2668f39e549a7d6cad5d70f9fea"},
-    {file = "regex-2024.4.28-cp310-cp310-win32.whl", hash = "sha256:a1409c4eccb6981c7baabc8888d3550df518add6e06fe74fa1d9312c1838652d"},
-    {file = "regex-2024.4.28-cp310-cp310-win_amd64.whl", hash = "sha256:1f687a28640f763f23f8a9801fe9e1b37338bb1ca5d564ddd41619458f1f22d1"},
-    {file = "regex-2024.4.28-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:84077821c85f222362b72fdc44f7a3a13587a013a45cf14534df1cbbdc9a6796"},
-    {file = "regex-2024.4.28-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:b45d4503de8f4f3dc02f1d28a9b039e5504a02cc18906cfe744c11def942e9eb"},
-    {file = "regex-2024.4.28-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:457c2cd5a646dd4ed536c92b535d73548fb8e216ebee602aa9f48e068fc393f3"},
-    {file = "regex-2024.4.28-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:2b51739ddfd013c6f657b55a508de8b9ea78b56d22b236052c3a85a675102dc6"},
-    {file = "regex-2024.4.28-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:459226445c7d7454981c4c0ce0ad1a72e1e751c3e417f305722bbcee6697e06a"},
-    {file = "regex-2024.4.28-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:670fa596984b08a4a769491cbdf22350431970d0112e03d7e4eeaecaafcd0fec"},
-    {file = "regex-2024.4.28-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:fe00f4fe11c8a521b173e6324d862ee7ee3412bf7107570c9b564fe1119b56fb"},
-    {file = "regex-2024.4.28-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:36f392dc7763fe7924575475736bddf9ab9f7a66b920932d0ea50c2ded2f5636"},
-    {file = "regex-2024.4.28-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:23a412b7b1a7063f81a742463f38821097b6a37ce1e5b89dd8e871d14dbfd86b"},
-    {file = "regex-2024.4.28-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:f1d6e4b7b2ae3a6a9df53efbf199e4bfcff0959dbdb5fd9ced34d4407348e39a"},
-    {file = "regex-2024.4.28-cp311-cp311-musllinux_1_1_ppc64le.whl", hash = "sha256:499334ad139557de97cbc4347ee921c0e2b5e9c0f009859e74f3f77918339257"},
-    {file = "regex-2024.4.28-cp311-cp311-musllinux_1_1_s390x.whl", hash = "sha256:0940038bec2fe9e26b203d636c44d31dd8766abc1fe66262da6484bd82461ccf"},
-    {file = "regex-2024.4.28-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:66372c2a01782c5fe8e04bff4a2a0121a9897e19223d9eab30c54c50b2ebeb7f"},
-    {file = "regex-2024.4.28-cp311-cp311-win32.whl", hash = "sha256:c77d10ec3c1cf328b2f501ca32583625987ea0f23a0c2a49b37a39ee5c4c4630"},
-    {file = "regex-2024.4.28-cp311-cp311-win_amd64.whl", hash = "sha256:fc0916c4295c64d6890a46e02d4482bb5ccf33bf1a824c0eaa9e83b148291f90"},
-    {file = "regex-2024.4.28-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:08a1749f04fee2811c7617fdd46d2e46d09106fa8f475c884b65c01326eb15c5"},
-    {file = "regex-2024.4.28-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:b8eb28995771c087a73338f695a08c9abfdf723d185e57b97f6175c5051ff1ae"},
-    {file = "regex-2024.4.28-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:dd7ef715ccb8040954d44cfeff17e6b8e9f79c8019daae2fd30a8806ef5435c0"},
-    {file = "regex-2024.4.28-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:fb0315a2b26fde4005a7c401707c5352df274460f2f85b209cf6024271373013"},
-    {file = "regex-2024.4.28-cp312-cp312-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:f2fc053228a6bd3a17a9b0a3f15c3ab3cf95727b00557e92e1cfe094b88cc662"},
-    {file = "regex-2024.4.28-cp312-cp312-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:7fe9739a686dc44733d52d6e4f7b9c77b285e49edf8570754b322bca6b85b4cc"},
-    {file = "regex-2024.4.28-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a74fcf77d979364f9b69fcf8200849ca29a374973dc193a7317698aa37d8b01c"},
-    {file = "regex-2024.4.28-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:965fd0cf4694d76f6564896b422724ec7b959ef927a7cb187fc6b3f4e4f59833"},
-    {file = "regex-2024.4.28-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:2fef0b38c34ae675fcbb1b5db760d40c3fc3612cfa186e9e50df5782cac02bcd"},
-    {file = "regex-2024.4.28-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:bc365ce25f6c7c5ed70e4bc674f9137f52b7dd6a125037f9132a7be52b8a252f"},
-    {file = "regex-2024.4.28-cp312-cp312-musllinux_1_1_ppc64le.whl", hash = "sha256:ac69b394764bb857429b031d29d9604842bc4cbfd964d764b1af1868eeebc4f0"},
-    {file = "regex-2024.4.28-cp312-cp312-musllinux_1_1_s390x.whl", hash = "sha256:144a1fc54765f5c5c36d6d4b073299832aa1ec6a746a6452c3ee7b46b3d3b11d"},
-    {file = "regex-2024.4.28-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:2630ca4e152c221072fd4a56d4622b5ada876f668ecd24d5ab62544ae6793ed6"},
-    {file = "regex-2024.4.28-cp312-cp312-win32.whl", hash = "sha256:7f3502f03b4da52bbe8ba962621daa846f38489cae5c4a7b5d738f15f6443d17"},
-    {file = "regex-2024.4.28-cp312-cp312-win_amd64.whl", hash = "sha256:0dd3f69098511e71880fb00f5815db9ed0ef62c05775395968299cb400aeab82"},
-    {file = "regex-2024.4.28.tar.gz", hash = "sha256:83ab366777ea45d58f72593adf35d36ca911ea8bd838483c1823b883a121b0e4"},
+    {file = "regex-2024.5.15-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:a81e3cfbae20378d75185171587cbf756015ccb14840702944f014e0d93ea09f"},
+    {file = "regex-2024.5.15-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:7b59138b219ffa8979013be7bc85bb60c6f7b7575df3d56dc1e403a438c7a3f6"},
+    {file = "regex-2024.5.15-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:a0bd000c6e266927cb7a1bc39d55be95c4b4f65c5be53e659537537e019232b1"},
+    {file = "regex-2024.5.15-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5eaa7ddaf517aa095fa8da0b5015c44d03da83f5bd49c87961e3c997daed0de7"},
+    {file = "regex-2024.5.15-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:ba68168daedb2c0bab7fd7e00ced5ba90aebf91024dea3c88ad5063c2a562cca"},
+    {file = "regex-2024.5.15-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:6e8d717bca3a6e2064fc3a08df5cbe366369f4b052dcd21b7416e6d71620dca1"},
+    {file = "regex-2024.5.15-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1337b7dbef9b2f71121cdbf1e97e40de33ff114801263b275aafd75303bd62b5"},
+    {file = "regex-2024.5.15-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:f9ebd0a36102fcad2f03696e8af4ae682793a5d30b46c647eaf280d6cfb32796"},
+    {file = "regex-2024.5.15-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:9efa1a32ad3a3ea112224897cdaeb6aa00381627f567179c0314f7b65d354c62"},
+    {file = "regex-2024.5.15-cp310-cp310-musllinux_1_2_aarch64.whl", hash = "sha256:1595f2d10dff3d805e054ebdc41c124753631b6a471b976963c7b28543cf13b0"},
+    {file = "regex-2024.5.15-cp310-cp310-musllinux_1_2_i686.whl", hash = "sha256:b802512f3e1f480f41ab5f2cfc0e2f761f08a1f41092d6718868082fc0d27143"},
+    {file = "regex-2024.5.15-cp310-cp310-musllinux_1_2_ppc64le.whl", hash = "sha256:a0981022dccabca811e8171f913de05720590c915b033b7e601f35ce4ea7019f"},
+    {file = "regex-2024.5.15-cp310-cp310-musllinux_1_2_s390x.whl", hash = "sha256:19068a6a79cf99a19ccefa44610491e9ca02c2be3305c7760d3831d38a467a6f"},
+    {file = "regex-2024.5.15-cp310-cp310-musllinux_1_2_x86_64.whl", hash = "sha256:1b5269484f6126eee5e687785e83c6b60aad7663dafe842b34691157e5083e53"},
+    {file = "regex-2024.5.15-cp310-cp310-win32.whl", hash = "sha256:ada150c5adfa8fbcbf321c30c751dc67d2f12f15bd183ffe4ec7cde351d945b3"},
+    {file = "regex-2024.5.15-cp310-cp310-win_amd64.whl", hash = "sha256:ac394ff680fc46b97487941f5e6ae49a9f30ea41c6c6804832063f14b2a5a145"},
+    {file = "regex-2024.5.15-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:f5b1dff3ad008dccf18e652283f5e5339d70bf8ba7c98bf848ac33db10f7bc7a"},
+    {file = "regex-2024.5.15-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:c6a2b494a76983df8e3d3feea9b9ffdd558b247e60b92f877f93a1ff43d26656"},
+    {file = "regex-2024.5.15-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:a32b96f15c8ab2e7d27655969a23895eb799de3665fa94349f3b2fbfd547236f"},
+    {file = "regex-2024.5.15-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:10002e86e6068d9e1c91eae8295ef690f02f913c57db120b58fdd35a6bb1af35"},
+    {file = "regex-2024.5.15-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:ec54d5afa89c19c6dd8541a133be51ee1017a38b412b1321ccb8d6ddbeb4cf7d"},
+    {file = "regex-2024.5.15-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:10e4ce0dca9ae7a66e6089bb29355d4432caed736acae36fef0fdd7879f0b0cb"},
+    {file = "regex-2024.5.15-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:3e507ff1e74373c4d3038195fdd2af30d297b4f0950eeda6f515ae3d84a1770f"},
+    {file = "regex-2024.5.15-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d1f059a4d795e646e1c37665b9d06062c62d0e8cc3c511fe01315973a6542e40"},
+    {file = "regex-2024.5.15-cp311-cp311-musllinux_1_2_aarch64.whl", hash = "sha256:0721931ad5fe0dda45d07f9820b90b2148ccdd8e45bb9e9b42a146cb4f695649"},
+    {file = "regex-2024.5.15-cp311-cp311-musllinux_1_2_i686.whl", hash = "sha256:833616ddc75ad595dee848ad984d067f2f31be645d603e4d158bba656bbf516c"},
+    {file = "regex-2024.5.15-cp311-cp311-musllinux_1_2_ppc64le.whl", hash = "sha256:287eb7f54fc81546346207c533ad3c2c51a8d61075127d7f6d79aaf96cdee890"},
+    {file = "regex-2024.5.15-cp311-cp311-musllinux_1_2_s390x.whl", hash = "sha256:19dfb1c504781a136a80ecd1fff9f16dddf5bb43cec6871778c8a907a085bb3d"},
+    {file = "regex-2024.5.15-cp311-cp311-musllinux_1_2_x86_64.whl", hash = "sha256:119af6e56dce35e8dfb5222573b50c89e5508d94d55713c75126b753f834de68"},
+    {file = "regex-2024.5.15-cp311-cp311-win32.whl", hash = "sha256:1c1c174d6ec38d6c8a7504087358ce9213d4332f6293a94fbf5249992ba54efa"},
+    {file = "regex-2024.5.15-cp311-cp311-win_amd64.whl", hash = "sha256:9e717956dcfd656f5055cc70996ee2cc82ac5149517fc8e1b60261b907740201"},
+    {file = "regex-2024.5.15-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:632b01153e5248c134007209b5c6348a544ce96c46005d8456de1d552455b014"},
+    {file = "regex-2024.5.15-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:e64198f6b856d48192bf921421fdd8ad8eb35e179086e99e99f711957ffedd6e"},
+    {file = "regex-2024.5.15-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:68811ab14087b2f6e0fc0c2bae9ad689ea3584cad6917fc57be6a48bbd012c49"},
+    {file = "regex-2024.5.15-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f8ec0c2fea1e886a19c3bee0cd19d862b3aa75dcdfb42ebe8ed30708df64687a"},
+    {file = "regex-2024.5.15-cp312-cp312-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:d0c0c0003c10f54a591d220997dd27d953cd9ccc1a7294b40a4be5312be8797b"},
+    {file = "regex-2024.5.15-cp312-cp312-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:2431b9e263af1953c55abbd3e2efca67ca80a3de8a0437cb58e2421f8184717a"},
+    {file = "regex-2024.5.15-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4a605586358893b483976cffc1723fb0f83e526e8f14c6e6614e75919d9862cf"},
+    {file = "regex-2024.5.15-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:391d7f7f1e409d192dba8bcd42d3e4cf9e598f3979cdaed6ab11288da88cb9f2"},
+    {file = "regex-2024.5.15-cp312-cp312-musllinux_1_2_aarch64.whl", hash = "sha256:9ff11639a8d98969c863d4617595eb5425fd12f7c5ef6621a4b74b71ed8726d5"},
+    {file = "regex-2024.5.15-cp312-cp312-musllinux_1_2_i686.whl", hash = "sha256:4eee78a04e6c67e8391edd4dad3279828dd66ac4b79570ec998e2155d2e59fd5"},
+    {file = "regex-2024.5.15-cp312-cp312-musllinux_1_2_ppc64le.whl", hash = "sha256:8fe45aa3f4aa57faabbc9cb46a93363edd6197cbc43523daea044e9ff2fea83e"},
+    {file = "regex-2024.5.15-cp312-cp312-musllinux_1_2_s390x.whl", hash = "sha256:d0a3d8d6acf0c78a1fff0e210d224b821081330b8524e3e2bc5a68ef6ab5803d"},
+    {file = "regex-2024.5.15-cp312-cp312-musllinux_1_2_x86_64.whl", hash = "sha256:c486b4106066d502495b3025a0a7251bf37ea9540433940a23419461ab9f2a80"},
+    {file = "regex-2024.5.15-cp312-cp312-win32.whl", hash = "sha256:c49e15eac7c149f3670b3e27f1f28a2c1ddeccd3a2812cba953e01be2ab9b5fe"},
+    {file = "regex-2024.5.15-cp312-cp312-win_amd64.whl", hash = "sha256:673b5a6da4557b975c6c90198588181029c60793835ce02f497ea817ff647cb2"},
+    {file = "regex-2024.5.15.tar.gz", hash = "sha256:d3ee02d9e5f482cc8309134a91eeaacbdd2261ba111b0fef3748eeb4913e6a2c"},
 ]
 
 [[package]]
 name = "requests"
 version = "2.31.0"
 requires_python = ">=3.7"
 summary = "Python HTTP for Humans."
@@ -1308,36 +1308,36 @@
 files = [
     {file = "rich-13.7.1-py3-none-any.whl", hash = "sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222"},
     {file = "rich-13.7.1.tar.gz", hash = "sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432"},
 ]
 
 [[package]]
 name = "ruff"
-version = "0.4.3"
+version = "0.4.4"
 requires_python = ">=3.7"
 summary = "An extremely fast Python linter and code formatter, written in Rust."
 groups = ["test"]
 files = [
-    {file = "ruff-0.4.3-py3-none-macosx_10_12_x86_64.whl", hash = "sha256:b70800c290f14ae6fcbb41bbe201cf62dfca024d124a1f373e76371a007454ce"},
-    {file = "ruff-0.4.3-py3-none-macosx_11_0_arm64.whl", hash = "sha256:08a0d6a22918ab2552ace96adeaca308833873a4d7d1d587bb1d37bae8728eb3"},
-    {file = "ruff-0.4.3-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:eba1f14df3c758dd7de5b55fbae7e1c8af238597961e5fb628f3de446c3c40c5"},
-    {file = "ruff-0.4.3-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:819fb06d535cc76dfddbfe8d3068ff602ddeb40e3eacbc90e0d1272bb8d97113"},
-    {file = "ruff-0.4.3-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:0bfc9e955e6dc6359eb6f82ea150c4f4e82b660e5b58d9a20a0e42ec3bb6342b"},
-    {file = "ruff-0.4.3-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:510a67d232d2ebe983fddea324dbf9d69b71c4d2dfeb8a862f4a127536dd4cfb"},
-    {file = "ruff-0.4.3-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:dc9ff11cd9a092ee7680a56d21f302bdda14327772cd870d806610a3503d001f"},
-    {file = "ruff-0.4.3-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:29efff25bf9ee685c2c8390563a5b5c006a3fee5230d28ea39f4f75f9d0b6f2f"},
-    {file = "ruff-0.4.3-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:18b00e0bcccf0fc8d7186ed21e311dffd19761cb632241a6e4fe4477cc80ef6e"},
-    {file = "ruff-0.4.3-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:262f5635e2c74d80b7507fbc2fac28fe0d4fef26373bbc62039526f7722bca1b"},
-    {file = "ruff-0.4.3-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:7363691198719c26459e08cc17c6a3dac6f592e9ea3d2fa772f4e561b5fe82a3"},
-    {file = "ruff-0.4.3-py3-none-musllinux_1_2_i686.whl", hash = "sha256:eeb039f8428fcb6725bb63cbae92ad67b0559e68b5d80f840f11914afd8ddf7f"},
-    {file = "ruff-0.4.3-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:927b11c1e4d0727ce1a729eace61cee88a334623ec424c0b1c8fe3e5f9d3c865"},
-    {file = "ruff-0.4.3-py3-none-win32.whl", hash = "sha256:25cacda2155778beb0d064e0ec5a3944dcca9c12715f7c4634fd9d93ac33fd30"},
-    {file = "ruff-0.4.3-py3-none-win_amd64.whl", hash = "sha256:7a1c3a450bc6539ef00da6c819fb1b76b6b065dec585f91456e7c0d6a0bbc725"},
-    {file = "ruff-0.4.3-py3-none-win_arm64.whl", hash = "sha256:71ca5f8ccf1121b95a59649482470c5601c60a416bf189d553955b0338e34614"},
-    {file = "ruff-0.4.3.tar.gz", hash = "sha256:ff0a3ef2e3c4b6d133fbedcf9586abfbe38d076041f2dc18ffb2c7e0485d5a07"},
+    {file = "ruff-0.4.4-py3-none-macosx_10_12_x86_64.whl", hash = "sha256:29d44ef5bb6a08e235c8249294fa8d431adc1426bfda99ed493119e6f9ea1bf6"},
+    {file = "ruff-0.4.4-py3-none-macosx_11_0_arm64.whl", hash = "sha256:c4efe62b5bbb24178c950732ddd40712b878a9b96b1d02b0ff0b08a090cbd891"},
+    {file = "ruff-0.4.4-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4c8e2f1e8fc12d07ab521a9005d68a969e167b589cbcaee354cb61e9d9de9c15"},
+    {file = "ruff-0.4.4-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:60ed88b636a463214905c002fa3eaab19795679ed55529f91e488db3fe8976ab"},
+    {file = "ruff-0.4.4-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:b90fc5e170fc71c712cc4d9ab0e24ea505c6a9e4ebf346787a67e691dfb72e85"},
+    {file = "ruff-0.4.4-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:8e7e6ebc10ef16dcdc77fd5557ee60647512b400e4a60bdc4849468f076f6eef"},
+    {file = "ruff-0.4.4-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:b9ddb2c494fb79fc208cd15ffe08f32b7682519e067413dbaf5f4b01a6087bcd"},
+    {file = "ruff-0.4.4-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:c51c928a14f9f0a871082603e25a1588059b7e08a920f2f9fa7157b5bf08cfe9"},
+    {file = "ruff-0.4.4-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b5eb0a4bfd6400b7d07c09a7725e1a98c3b838be557fee229ac0f84d9aa49c36"},
+    {file = "ruff-0.4.4-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:b1867ee9bf3acc21778dcb293db504692eda5f7a11a6e6cc40890182a9f9e595"},
+    {file = "ruff-0.4.4-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:1aecced1269481ef2894cc495647392a34b0bf3e28ff53ed95a385b13aa45768"},
+    {file = "ruff-0.4.4-py3-none-musllinux_1_2_i686.whl", hash = "sha256:9da73eb616b3241a307b837f32756dc20a0b07e2bcb694fec73699c93d04a69e"},
+    {file = "ruff-0.4.4-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:958b4ea5589706a81065e2a776237de2ecc3e763342e5cc8e02a4a4d8a5e6f95"},
+    {file = "ruff-0.4.4-py3-none-win32.whl", hash = "sha256:cb53473849f011bca6e754f2cdf47cafc9c4f4ff4570003a0dad0b9b6890e876"},
+    {file = "ruff-0.4.4-py3-none-win_amd64.whl", hash = "sha256:424e5b72597482543b684c11def82669cc6b395aa8cc69acc1858b5ef3e5daae"},
+    {file = "ruff-0.4.4-py3-none-win_arm64.whl", hash = "sha256:39df0537b47d3b597293edbb95baf54ff5b49589eb7ff41926d8243caa995ea6"},
+    {file = "ruff-0.4.4.tar.gz", hash = "sha256:f87ea42d5cdebdc6a69761a9d0bc83ae9b3b30d0ad78952005ba6568d6c022af"},
 ]
 
 [[package]]
 name = "safetensors"
 version = "0.4.3"
 requires_python = ">=3.7"
 summary = ""
@@ -1440,25 +1440,25 @@
     {file = "sentencepiece-0.2.0-cp312-cp312-win32.whl", hash = "sha256:fb89f811e5efd18bab141afc3fea3de141c3f69f3fe9e898f710ae7fe3aab251"},
     {file = "sentencepiece-0.2.0-cp312-cp312-win_amd64.whl", hash = "sha256:7a673a72aab81fef5ebe755c6e0cc60087d1f3a4700835d40537183c1703a45f"},
     {file = "sentencepiece-0.2.0.tar.gz", hash = "sha256:a52c19171daaf2e697dc6cbe67684e0fa341b1248966f6aebb541de654d15843"},
 ]
 
 [[package]]
 name = "sentry-sdk"
-version = "2.1.1"
+version = "2.2.0"
 requires_python = ">=3.6"
 summary = "Python client for Sentry (https://sentry.io)"
 groups = ["default"]
 dependencies = [
     "certifi",
     "urllib3>=1.26.11",
 ]
 files = [
-    {file = "sentry_sdk-2.1.1-py2.py3-none-any.whl", hash = "sha256:99aeb78fb76771513bd3b2829d12613130152620768d00cd3e45ac00cb17950f"},
-    {file = "sentry_sdk-2.1.1.tar.gz", hash = "sha256:95d8c0bb41c8b0bc37ab202c2c4a295bb84398ee05f4cdce55051cd75b926ec1"},
+    {file = "sentry_sdk-2.2.0-py2.py3-none-any.whl", hash = "sha256:674f58da37835ea7447fe0e34c57b4a4277fad558b0a7cb4a6c83bcb263086be"},
+    {file = "sentry_sdk-2.2.0.tar.gz", hash = "sha256:70eca103cf4c6302365a9d7cf522e7ed7720828910eb23d43ada8e50d1ecda9d"},
 ]
 
 [[package]]
 name = "setproctitle"
 version = "1.3.3"
 requires_python = ">=3.7"
 summary = "A Python module to customize the process title"
@@ -1834,26 +1834,26 @@
 files = [
     {file = "urllib3-2.2.1-py3-none-any.whl", hash = "sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d"},
     {file = "urllib3-2.2.1.tar.gz", hash = "sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19"},
 ]
 
 [[package]]
 name = "virtualenv"
-version = "20.26.1"
+version = "20.26.2"
 requires_python = ">=3.7"
 summary = "Virtual Python Environment builder"
 groups = ["test"]
 dependencies = [
     "distlib<1,>=0.3.7",
     "filelock<4,>=3.12.2",
     "platformdirs<5,>=3.9.1",
 ]
 files = [
-    {file = "virtualenv-20.26.1-py3-none-any.whl", hash = "sha256:7aa9982a728ae5892558bff6a2839c00b9ed145523ece2274fad6f414690ae75"},
-    {file = "virtualenv-20.26.1.tar.gz", hash = "sha256:604bfdceaeece392802e6ae48e69cec49168b9c5f4a44e483963f9242eb0e78b"},
+    {file = "virtualenv-20.26.2-py3-none-any.whl", hash = "sha256:a624db5e94f01ad993d476b9ee5346fdf7b9de43ccaee0e0197012dc838a0e9b"},
+    {file = "virtualenv-20.26.2.tar.gz", hash = "sha256:82bf0f4eebbb78d36ddaee0283d43fe5736b53880b8a8cdcd37390a07ac3741c"},
 ]
 
 [[package]]
 name = "wandb"
 version = "0.17.0"
 requires_python = ">=3.7"
 summary = "A CLI and library for interacting with the Weights & Biases API."
```

### Comparing `transcoders_slim-0.1.0/.github/workflows/release.yaml` & `transcoders_slim-0.2.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `transcoders_slim-0.1.0/.github/workflows/tests.yaml` & `transcoders_slim-0.2.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `transcoders_slim-0.1.0/tests/test_load_pretrained.py` & `transcoders_slim-0.2.0/tests/test_load_pretrained.py`

 * *Files identical despite different names*

### Comparing `transcoders_slim-0.1.0/transcoders_slim/load_pretrained.py` & `transcoders_slim-0.2.0/transcoders_slim/load_pretrained.py`

 * *Files identical despite different names*

### Comparing `transcoders_slim-0.1.0/transcoders_slim/sae_training/config.py` & `transcoders_slim-0.2.0/transcoders_slim/sae_training/config.py`

 * *Files identical despite different names*

### Comparing `transcoders_slim-0.1.0/transcoders_slim/sae_training/sparse_autoencoder.py` & `transcoders_slim-0.2.0/transcoders_slim/sae_training/sparse_autoencoder.py`

 * *Files identical despite different names*

### Comparing `transcoders_slim-0.1.0/.gitignore` & `transcoders_slim-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `transcoders_slim-0.1.0/README.md` & `transcoders_slim-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `transcoders_slim-0.1.0/pyproject.toml` & `transcoders_slim-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 [project]
 name = "transcoders-slim"
-version = "0.1.0"
+version = "0.2.0"
 description = "A template for python projects in PDM"
 authors = [
-    {name = "Daniel Tan", email = "dtch1997@users.noreply.github.com"},
-    {name = "Daniel CH Tan", email = "dtch1997@users.noreply.github.com"},
+    { name = "Daniel Tan", email = "dtch1997@users.noreply.github.com" },
+    { name = "Daniel CH Tan", email = "dtch1997@users.noreply.github.com" },
 ]
 dependencies = [
     "huggingface-hub>=0.23.0",
     "torch>=2.3.0",
-    "transformer-lens>=1.17.0",
-    "einops>=0.8.0",
+    "transformer-lens>=1.14.0",
+    "einops>=0.7.0",
     "jaxtyping>=0.2.28",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
-license = {text = "MIT"}
+license = { text = "MIT" }
 
 [project.optional-dependencies]
-test = [
-    "ruff>=0.4.3",
-    "pytest>=8.2.0",
-    "pyright>=1.1.361",
-    "pre-commit>=3.7.0",
-]
+test = ["ruff>=0.4.3", "pytest>=8.2.0", "pyright>=1.1.361", "pre-commit>=3.7.0"]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.pdm]
 distribution = true
@@ -37,8 +32,8 @@
 venv = ".venv"
 
 [tool.semantic_release]
 version_variables = [
     "transcoders_slim/__init__.py:__version__",
     "pyproject.toml:version",
 ]
-branch = "main"
+branch = "main"
```

### Comparing `transcoders_slim-0.1.0/PKG-INFO` & `transcoders_slim-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: transcoders-slim
-Version: 0.1.0
+Version: 0.2.0
 Summary: A template for python projects in PDM
 Author-email: Daniel Tan <dtch1997@users.noreply.github.com>, Daniel CH Tan <dtch1997@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.10
-Requires-Dist: einops>=0.8.0
+Requires-Dist: einops>=0.7.0
 Requires-Dist: huggingface-hub>=0.23.0
 Requires-Dist: jaxtyping>=0.2.28
 Requires-Dist: torch>=2.3.0
-Requires-Dist: transformer-lens>=1.17.0
+Requires-Dist: transformer-lens>=1.14.0
 Provides-Extra: test
 Requires-Dist: pre-commit>=3.7.0; extra == 'test'
 Requires-Dist: pyright>=1.1.361; extra == 'test'
 Requires-Dist: pytest>=8.2.0; extra == 'test'
 Requires-Dist: ruff>=0.4.3; extra == 'test'
 Description-Content-Type: text/markdown
```

