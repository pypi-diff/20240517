# Comparing `tmp/testmypixipkg-0.12.0.tar.gz` & `tmp/testmypixipkg-0.13.0.tar.gz`

## Comparing `testmypixipkg-0.12.0.tar` & `testmypixipkg-0.13.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 testmypixipkg-0.12.0/.gitattributes
--rw-r--r--   0        0        0     4271 2020-02-02 00:00:00.000000 testmypixipkg-0.12.0/CHANGELOG.md
--rw-r--r--   0        0        0   154311 2020-02-02 00:00:00.000000 testmypixipkg-0.12.0/pixi.lock
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 testmypixipkg-0.12.0/releaserc.toml
--rw-r--r--   0        0        0     5910 2020-02-02 00:00:00.000000 testmypixipkg-0.12.0/.github/workflows/main.yaml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 testmypixipkg-0.12.0/src/testmypixipkg/__init__.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 testmypixipkg-0.12.0/src/testmypixipkg/__main__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 testmypixipkg-0.12.0/tests/test_say_hello.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 testmypixipkg-0.12.0/.gitignore
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 testmypixipkg-0.12.0/hatch.toml
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 testmypixipkg-0.12.0/pyproject.toml
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 testmypixipkg-0.12.0/PKG-INFO
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 testmypixipkg-0.13.0/.gitattributes
+-rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 testmypixipkg-0.13.0/CHANGELOG.md
+-rw-r--r--   0        0        0   173757 2020-02-02 00:00:00.000000 testmypixipkg-0.13.0/pixi.lock
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 testmypixipkg-0.13.0/releaserc.toml
+-rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 testmypixipkg-0.13.0/.github/workflows/main.yaml
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 testmypixipkg-0.13.0/src/testmypixipkg/__init__.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 testmypixipkg-0.13.0/src/testmypixipkg/__main__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 testmypixipkg-0.13.0/tests/test_say_hello.py
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 testmypixipkg-0.13.0/.gitignore
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 testmypixipkg-0.13.0/hatch.toml
+-rw-r--r--   0        0        0     3674 2020-02-02 00:00:00.000000 testmypixipkg-0.13.0/pyproject.toml
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 testmypixipkg-0.13.0/PKG-INFO
```

### Comparing `testmypixipkg-0.12.0/CHANGELOG.md` & `testmypixipkg-0.13.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 # CHANGELOG
 
 
 
+## v0.13.0 (2024-05-16)
+
+### Feature
+
+* feat: add ruff to ci ([`2b61b24`](https://github.com/jjjermiah/pypackage/commit/2b61b2461e6960c7f75177bc39527a2981a32eee))
+
+* feat: add ruff ([`3db3a38`](https://github.com/jjjermiah/pypackage/commit/3db3a3853fd2864aa31b815646c97ad11af2e599))
+
+### Fix
+
+* fix: rename CD to semantic release ([`c264e7b`](https://github.com/jjjermiah/pypackage/commit/c264e7bbd209520ae8db086855d9a2d66c029cab))
+
+* fix: add recipe to ignore ([`7acb290`](https://github.com/jjjermiah/pypackage/commit/7acb2906473d8f0d331890be4bed85264b05d7e0))
+
+
 ## v0.12.0 (2024-05-16)
 
 ### Feature
 
 * feat: add pypi ([`12f3f55`](https://github.com/jjjermiah/pypackage/commit/12f3f5500b19e722a7ed8c2d2e7c4a0d16d08784))
 
 * feat: add publish-pypi ([`b261e14`](https://github.com/jjjermiah/pypackage/commit/b261e145d97a42a1cc348af5db868920aae97a28))
```

### Comparing `testmypixipkg-0.12.0/pixi.lock` & `testmypixipkg-0.13.0/pixi.lock`

 * *Files 10% similar despite different names*

```diff
@@ -117,152 +117,227 @@
       - conda: https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2024.2.2-hbcca054_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/coverage-7.5.1-py312h9a8786e_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/execnet-2.1.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ghp-import-2.1.0-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h55db66e_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.6.2-h59595ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-h77fa898_7.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-h77fa898_7.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.3-h2797004_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-hc0a3c3a_7.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/markdown-3.6-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.5-py312h98912ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mergedeep-1.3.4-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-1.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-get-deps-0.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.5-h59595ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.3.0-hd590300_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.3-hab00c5b_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.12-4_cp312.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0.1-py312h98912ed_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pyyaml-env-tag-0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/ruff-0.4.4-py312h5715c7c_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/watchdog-4.0.0-py312h7900ff3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
       - pypi: .
       osx-64:
       - conda: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2024.2.2-h8857fd0_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/coverage-7.5.1-py312h520dd33_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/execnet-2.1.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ghp-import-2.1.0-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libcxx-17.0.6-h88467a6_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libexpat-2.6.2-h73e2aa4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.3-h92b6c6a_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/markdown-3.6-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.5-py312h41838bb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mergedeep-1.3.4-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-1.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-get-deps-0.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.5-h5846eda_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.3.0-hd75f5a5_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.3-h1411813_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.12-4_cp312.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0.1-py312h104f124_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pyyaml-env-tag-0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/ruff-0.4.4-py312h675b354_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/watchdog-4.0.0-py312hc2c2f20_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
       - pypi: .
       osx-arm64:
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/bzip2-1.0.8-h93a5062_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ca-certificates-2024.2.2-hf0a4a13_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/coverage-7.5.1-py312h7e5086c_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/execnet-2.1.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ghp-import-2.1.0-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libcxx-17.0.6-h5f092b4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libexpat-2.6.2-hebf3989_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libffi-3.4.2-h3422bc3_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libsqlite-3.45.3-h091b4b1_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libzlib-1.2.13-h53f4e23_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/markdown-3.6-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/markupsafe-2.1.5-py312he37b823_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mergedeep-1.3.4-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-1.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-get-deps-0.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ncurses-6.5-hb89a1cb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.3.0-h0d3ecfb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.3-h4a7b5fc_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.12-4_cp312.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/pyyaml-6.0.1-py312h02f2b3b_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pyyaml-env-tag-0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/readline-8.2-h92ec313_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ruff-0.4.4-py312h3402d49_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/watchdog-4.0.0-py312he37b823_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/yaml-0.2.5-h3422bc3_2.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
       - pypi: .
       win-64:
       - conda: https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-hcfcfb64_5.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-win_pyh7428d3b_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/coverage-7.5.1-py312h4389bb4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/execnet-2.1.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ghp-import-2.1.0-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libexpat-2.6.2-h63175ca_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.3-hcfcfb64_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/markdown-3.6-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.5-py312he70551f_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mergedeep-1.3.4-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-1.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-get-deps-0.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/openssl-3.3.0-hcfcfb64_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.12.3-h2628c8c_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.12-4_cp312.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0.1-py312he70551f_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pyyaml-env-tag-0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/ruff-0.4.4-py312h7a6832a_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hcf57466_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.38.33130-h82b7239_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.38.33130-hcb4865c_18.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/watchdog-4.0.0-py312h2e8e312_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
       - pypi: .
   publish:
     channels:
     - url: https://conda.anaconda.org/conda-forge/
     indexes:
     - https://pypi.org/simple
@@ -1373,14 +1448,31 @@
   - python >=3.7
   license: Unlicense
   purls:
   - pkg:pypi/filelock
   size: 15902
   timestamp: 1714422911808
 - kind: conda
+  name: ghp-import
+  version: 2.1.0
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/ghp-import-2.1.0-pyhd8ed1ab_0.tar.bz2
+  sha256: 097d9b4c946b195800bc68f68393370049238509b08ef828c06fbf481bbc139c
+  md5: 6d8d61116031a3f5b1f32e7899785866
+  depends:
+  - python >=3.6
+  - python-dateutil >=2.8.1
+  license: LicenseRef-Tumbolia-Public
+  purls:
+  - pkg:pypi/ghp-import
+  size: 15504
+  timestamp: 1651585848291
+- kind: conda
   name: gitdb
   version: 4.0.11
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/gitdb-4.0.11-pyhd8ed1ab_0.conda
   sha256: 52ab2798be31b8f509eeec458712f447ced4f96ecb672c6c9a42778f47e07b1b
@@ -2264,14 +2356,32 @@
   - libgcc-ng >=12
   constrains:
   - zlib 1.2.13 *_5
   license: Zlib
   license_family: Other
   size: 61588
   timestamp: 1686575217516
+- kind: conda
+  name: markdown
+  version: '3.6'
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/markdown-3.6-pyhd8ed1ab_0.conda
+  sha256: fce1fde00359696983989699c00f9891194c4ebafea647a8d21b7e2e3329b56e
+  md5: 06e9bebf748a0dea03ecbe1f0e27e909
+  depends:
+  - importlib-metadata >=4.4
+  - python >=3.6
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/markdown
+  size: 78331
+  timestamp: 1710435316163
 - kind: pypi
   name: markdown-it-py
   version: 3.0.0
   url: https://files.pythonhosted.org/packages/42/d7/1ec15b46af6af88f19b8e5ffea08fa375d433c998b8a7639e76935c14f1f/markdown_it_py-3.0.0-py3-none-any.whl
   sha256: 355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1
   requires_dist:
   - mdurl~=0.1
@@ -2419,14 +2529,85 @@
   license: MIT
   license_family: MIT
   purls:
   - pkg:pypi/mdurl
   size: 14680
   timestamp: 1704317789138
 - kind: conda
+  name: mergedeep
+  version: 1.3.4
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/mergedeep-1.3.4-pyhd8ed1ab_0.tar.bz2
+  sha256: 41ad8c16876820981adfc6e17a62935c950214bd9a9bb092e6aaefdc89a33f0b
+  md5: 1a160a3cab5cb6bd46264b52cd6f69a2
+  depends:
+  - python >=3.6
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/mergedeep
+  size: 9598
+  timestamp: 1612711404414
+- kind: conda
+  name: mkdocs
+  version: 1.6.0
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/mkdocs-1.6.0-pyhd8ed1ab_0.conda
+  sha256: d15180924550ece7ef30c1868af23b4a3a02d650533c72977a27ba4fca3cc3a3
+  md5: e938f734bcc0cfdccf85e5f7ed573c8e
+  depends:
+  - click >=7.0
+  - colorama >=0.4
+  - ghp-import >=1.0
+  - importlib-metadata >=4.4
+  - jinja2 >=2.11.1
+  - markdown >=3.3.6
+  - markupsafe >=2.0.1
+  - mergedeep >=1.3.4
+  - mkdocs-get-deps >=0.2.0
+  - packaging >=20.5
+  - pathspec >=0.11.1
+  - python >=3.8
+  - pyyaml >=5.1
+  - pyyaml-env-tag >=0.1
+  - watchdog >=2.0
+  constrains:
+  - babel >=2.9.0
+  license: BSD-2-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/mkdocs
+  size: 3523311
+  timestamp: 1714253186566
+- kind: conda
+  name: mkdocs-get-deps
+  version: 0.2.0
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/mkdocs-get-deps-0.2.0-pyhd8ed1ab_0.conda
+  sha256: aa6207994b15a15b5f82a442804c279bf78f6c4680f0903fb015294c41e34b30
+  md5: 0365c9a6e4e41732bde159112b0aef4d
+  depends:
+  - importlib-metadata >=4.3
+  - mergedeep >=1.3.4
+  - platformdirs >=2.2.0
+  - python >=3.8
+  - pyyaml >=5.1
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/mkdocs-get-deps
+  size: 14733
+  timestamp: 1713710951974
+- kind: conda
   name: more-itertools
   version: 10.2.0
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/more-itertools-10.2.0-pyhd8ed1ab_0.conda
   sha256: 9e49e9484ff279453f0b55323a3f0c7cb97440c74f69eecda1f4ad29fae5cd3c
@@ -3014,14 +3195,32 @@
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.12.* *_cp312
   license: Python-2.0
   size: 31991381
   timestamp: 1713208036041
 - kind: conda
+  name: python-dateutil
+  version: 2.9.0
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
+  sha256: f3ceef02ac164a8d3a080d0d32f8e2ebe10dd29e3a685d240e38b3599e146320
+  md5: 2cf4264fffb9e6eff6031c5b6884d61c
+  depends:
+  - python >=3.7
+  - six >=1.5
+  license: Apache-2.0
+  license_family: APACHE
+  purls:
+  - pkg:pypi/python-dateutil
+  size: 222742
+  timestamp: 1709299922152
+- kind: conda
   name: python-gitlab
   version: 4.5.0
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/python-gitlab-4.5.0-pyhd8ed1ab_0.conda
   sha256: 48a5592e592b4f78d6aa509a0045d384e581622975ad1d34d2d0660f6252a5a4
@@ -3140,14 +3339,113 @@
   license: BSD-3-Clause
   license_family: BSD
   purls:
   - pkg:pypi/pywin32-ctypes
   size: 55871
   timestamp: 1695395307212
 - kind: conda
+  name: pyyaml
+  version: 6.0.1
+  build: py312h02f2b3b_1
+  build_number: 1
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/pyyaml-6.0.1-py312h02f2b3b_1.conda
+  sha256: b6b4027b89c17b9bbd8089aec3e44bc29f802a7d5668d5a75b5358d7ed9705ca
+  md5: a0c843e52a1c4422d8657dd76e9eb994
+  depends:
+  - python >=3.12.0rc3,<3.13.0a0
+  - python >=3.12.0rc3,<3.13.0a0 *_cpython
+  - python_abi 3.12.* *_cp312
+  - yaml >=0.2.5,<0.3.0a0
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/pyyaml
+  size: 182705
+  timestamp: 1695373895409
+- kind: conda
+  name: pyyaml
+  version: 6.0.1
+  build: py312h104f124_1
+  build_number: 1
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0.1-py312h104f124_1.conda
+  sha256: 04aa180782cb675b960c0bf4aad439b4a7a08553c6af74d0b8e5df9a0c7cc4f4
+  md5: 260ed90aaf06061edabd7209638cf03b
+  depends:
+  - python >=3.12.0rc3,<3.13.0a0
+  - python_abi 3.12.* *_cp312
+  - yaml >=0.2.5,<0.3.0a0
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/pyyaml
+  size: 185636
+  timestamp: 1695373742454
+- kind: conda
+  name: pyyaml
+  version: 6.0.1
+  build: py312h98912ed_1
+  build_number: 1
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0.1-py312h98912ed_1.conda
+  sha256: 7f347a10a7121b08d79d21cd4f438c07c23479ea0c74dfb89d6dc416f791bb7f
+  md5: e3fd78d8d490af1d84763b9fe3f2e552
+  depends:
+  - libgcc-ng >=12
+  - python >=3.12.0rc3,<3.13.0a0
+  - python_abi 3.12.* *_cp312
+  - yaml >=0.2.5,<0.3.0a0
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/pyyaml
+  size: 196583
+  timestamp: 1695373632212
+- kind: conda
+  name: pyyaml
+  version: 6.0.1
+  build: py312he70551f_1
+  build_number: 1
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0.1-py312he70551f_1.conda
+  sha256: a72fa8152791b4738432f270e70b3a9a4d583ef059a78aa1c62f4b4ab7b15494
+  md5: f91e0baa89ba21166916624ba7bfb422
+  depends:
+  - python >=3.12.0rc3,<3.13.0a0
+  - python_abi 3.12.* *_cp312
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
+  - yaml >=0.2.5,<0.3.0a0
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/pyyaml
+  size: 167932
+  timestamp: 1695374097139
+- kind: conda
+  name: pyyaml-env-tag
+  version: '0.1'
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/pyyaml-env-tag-0.1-pyhd8ed1ab_0.tar.bz2
+  sha256: 900319483135730d9836855a807822f0500b1a239520749103e9ef9b7ba9f246
+  md5: 626ed9060ddeb681ddc42bcad89156ab
+  depends:
+  - python >=3.6
+  - pyyaml
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/pyyaml-env-tag
+  size: 7473
+  timestamp: 1624389117412
+- kind: conda
   name: readline
   version: '8.2'
   build: h8228510_1
   build_number: 1
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
   sha256: 5435cf39d039387fbdc977b0a762357ea909a7694d9528ab40f005e9208744d7
@@ -3285,14 +3583,96 @@
   - mkdocs-material[imaging]~=9.5.18 ; extra == 'docs'
   - mkdocs-material-extensions ; extra == 'docs'
   - mkdocs-rss-plugin ; extra == 'docs'
   - mkdocstrings[python] ; extra == 'docs'
   - rich-codex ; extra == 'docs'
   requires_python: '>=3.7'
 - kind: conda
+  name: ruff
+  version: 0.4.4
+  build: py312h3402d49_0
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/ruff-0.4.4-py312h3402d49_0.conda
+  sha256: 09f47bd451076a28db84ceb9552d9c318402d8768b12a466cb503a39600da905
+  md5: ed152476a82a8ebae71ce4eb335cb725
+  depends:
+  - __osx >=11.0
+  - libcxx >=16
+  - python >=3.12,<3.13.0a0
+  - python >=3.12,<3.13.0a0 *_cpython
+  - python_abi 3.12.* *_cp312
+  constrains:
+  - __osx >=11.0
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/ruff
+  size: 5808812
+  timestamp: 1715290154581
+- kind: conda
+  name: ruff
+  version: 0.4.4
+  build: py312h5715c7c_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/ruff-0.4.4-py312h5715c7c_0.conda
+  sha256: 23795ee023595be9e5c52736b280de4a2adb2082993615ee05e71e563628b266
+  md5: b217a3a08f3cc3275822367a0a9abb54
+  depends:
+  - libgcc-ng >=12
+  - libstdcxx-ng >=12
+  - python >=3.12,<3.13.0a0
+  - python_abi 3.12.* *_cp312
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/ruff
+  size: 6280363
+  timestamp: 1715289943071
+- kind: conda
+  name: ruff
+  version: 0.4.4
+  build: py312h675b354_0
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/ruff-0.4.4-py312h675b354_0.conda
+  sha256: fae26e6e28e84cfedaca5612b43bde8e80b459ec6db246f43d9e493254d693c2
+  md5: 36d393eb2de35b8bbd0175fe893355bc
+  depends:
+  - __osx >=10.13
+  - libcxx >=16
+  - python >=3.12,<3.13.0a0
+  - python_abi 3.12.* *_cp312
+  constrains:
+  - __osx >=10.12
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/ruff
+  size: 6079492
+  timestamp: 1715290168569
+- kind: conda
+  name: ruff
+  version: 0.4.4
+  build: py312h7a6832a_0
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/ruff-0.4.4-py312h7a6832a_0.conda
+  sha256: ca264b4933ccc0d4d24c07960415d82c68776d56313cd5a95731e6a0d07984b7
+  md5: 445d9c0ed18d9dc2521c87a4d723189c
+  depends:
+  - python >=3.12,<3.13.0a0
+  - python_abi 3.12.* *_cp312
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/ruff
+  size: 6170392
+  timestamp: 1715291305605
+- kind: conda
   name: secretstorage
   version: 3.3.3
   build: py312h7900ff3_2
   build_number: 2
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/secretstorage-3.3.3-py312h7900ff3_2.conda
   sha256: 0479e3f8c8e90049a6d92d4c7e67916c6d6cdafd11a1a31c54c785cce44aeb20
@@ -3323,14 +3703,31 @@
   license: MIT
   license_family: MIT
   purls:
   - pkg:pypi/shellingham
   size: 14568
   timestamp: 1698144516278
 - kind: conda
+  name: six
+  version: 1.16.0
+  build: pyh6c4a22f_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
+  sha256: a85c38227b446f42c5b90d9b642f2c0567880c15d72492d8da074a59c8f91dd6
+  md5: e5f25f8dbc060e9a8d912e432202afc2
+  depends:
+  - python
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/six
+  size: 14259
+  timestamp: 1620240338595
+- kind: conda
   name: smmap
   version: 5.0.0
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/smmap-5.0.0-pyhd8ed1ab_0.tar.bz2
   sha256: 23011cb3e064525bdb8787c75126a2e78d2344a72cd6773922006d1da1f2af16
@@ -3358,17 +3755,17 @@
   license_family: Apache
   purls:
   - pkg:pypi/sniffio
   size: 15064
   timestamp: 1708953086199
 - kind: pypi
   name: testmypixipkg
-  version: 0.12.0
+  version: 0.13.0
   path: .
-  sha256: 5f7ebba804bbe1e4aed09bbcdda1d47036b22f7a73fac7c6fd9a327d127fd9a3
+  sha256: 9f068bcc440364193e03614acd70d31089ec41ac5811e1c43730c889bf557ea8
   requires_dist:
   - rich
   - rich-click
   requires_python: '>=3.11'
   editable: true
 - kind: conda
   name: tk
@@ -3746,14 +4143,87 @@
   depends:
   - vc14_runtime >=14.38.33130
   license: BSD-3-Clause
   license_family: BSD
   size: 16988
   timestamp: 1702511261442
 - kind: conda
+  name: watchdog
+  version: 4.0.0
+  build: py312h2e8e312_0
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/watchdog-4.0.0-py312h2e8e312_0.conda
+  sha256: 4b1eeaecccadf55a5c322e25290d75c8bed7b0d5e25fa6dfa03fc16fc9919fc4
+  md5: 186ec4486a2c5d738c002067665b50be
+  depends:
+  - python >=3.12,<3.13.0a0
+  - python_abi 3.12.* *_cp312
+  - pyyaml >=3.10
+  license: Apache-2.0
+  license_family: APACHE
+  purls:
+  - pkg:pypi/watchdog
+  size: 152911
+  timestamp: 1707295573907
+- kind: conda
+  name: watchdog
+  version: 4.0.0
+  build: py312h7900ff3_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/watchdog-4.0.0-py312h7900ff3_0.conda
+  sha256: db3ef9753934826c008216b198f04a6637150e1d91d72733148c0822e4a042a2
+  md5: 1b87b82dd803565550e6358c0790f3d2
+  depends:
+  - python >=3.12,<3.13.0a0
+  - python_abi 3.12.* *_cp312
+  - pyyaml >=3.10
+  license: Apache-2.0
+  license_family: APACHE
+  purls:
+  - pkg:pypi/watchdog
+  size: 136845
+  timestamp: 1707295261797
+- kind: conda
+  name: watchdog
+  version: 4.0.0
+  build: py312hc2c2f20_0
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/watchdog-4.0.0-py312hc2c2f20_0.conda
+  sha256: f333e1f11d60e096d8b0f2b7dbe313fc9ee22d6c09f0a0cc7d3c9fed56ee48dd
+  md5: ebd7ea0d23052393f0a62efe8a508e99
+  depends:
+  - python >=3.12,<3.13.0a0
+  - python_abi 3.12.* *_cp312
+  - pyyaml >=3.10
+  license: Apache-2.0
+  license_family: APACHE
+  purls:
+  - pkg:pypi/watchdog
+  size: 144711
+  timestamp: 1707295580304
+- kind: conda
+  name: watchdog
+  version: 4.0.0
+  build: py312he37b823_0
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/watchdog-4.0.0-py312he37b823_0.conda
+  sha256: 3e7486e161e4478a1bb63cb124a446b21b0af113458522d215ba76eebb1a473a
+  md5: c483c04540c229b50564201c5432667c
+  depends:
+  - python >=3.12,<3.13.0a0
+  - python >=3.12,<3.13.0a0 *_cpython
+  - python_abi 3.12.* *_cp312
+  - pyyaml >=3.10
+  license: Apache-2.0
+  license_family: APACHE
+  purls:
+  - pkg:pypi/watchdog
+  size: 145347
+  timestamp: 1707295575866
+- kind: conda
   name: win_inet_pton
   version: 1.1.0
   build: pyhd8ed1ab_6
   build_number: 6
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2
@@ -3813,14 +4283,71 @@
   depends:
   - vc >=14.1,<15
   - vs2015_runtime >=14.16.27033
   license: LGPL-2.1 and GPL-2.0
   size: 217804
   timestamp: 1660346976440
 - kind: conda
+  name: yaml
+  version: 0.2.5
+  build: h0d85af4_2
+  build_number: 2
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2
+  sha256: 5301417e2c8dea45b401ffee8df3957d2447d4ce80c83c5ff151fc6bfe1c4148
+  md5: d7e08fcf8259d742156188e8762b4d20
+  license: MIT
+  license_family: MIT
+  size: 84237
+  timestamp: 1641347062780
+- kind: conda
+  name: yaml
+  version: 0.2.5
+  build: h3422bc3_2
+  build_number: 2
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/yaml-0.2.5-h3422bc3_2.tar.bz2
+  sha256: 93181a04ba8cfecfdfb162fc958436d868cc37db504c58078eab4c1a3e57fbb7
+  md5: 4bb3f014845110883a3c5ee811fd84b4
+  license: MIT
+  license_family: MIT
+  size: 88016
+  timestamp: 1641347076660
+- kind: conda
+  name: yaml
+  version: 0.2.5
+  build: h7f98852_2
+  build_number: 2
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2
+  sha256: a4e34c710eeb26945bdbdaba82d3d74f60a78f54a874ec10d373811a5d217535
+  md5: 4cb3ad778ec2d5a7acbdf254eb1c42ae
+  depends:
+  - libgcc-ng >=9.4.0
+  license: MIT
+  license_family: MIT
+  size: 89141
+  timestamp: 1641346969816
+- kind: conda
+  name: yaml
+  version: 0.2.5
+  build: h8ffe710_2
+  build_number: 2
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2
+  sha256: 4e2246383003acbad9682c7c63178e2e715ad0eb84f03a8df1fbfba455dfedc5
+  md5: adbfb9f45d1004a26763652246a33764
+  depends:
+  - vc >=14.1,<15.0a0
+  - vs2015_runtime >=14.16.27012
+  license: MIT
+  license_family: MIT
+  size: 63274
+  timestamp: 1641347623319
+- kind: conda
   name: zipp
   version: 3.17.0
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
   sha256: bced1423fdbf77bca0a735187d05d9b9812d2163f60ab426fc10f11f92ecbe26
```

### Comparing `testmypixipkg-0.12.0/releaserc.toml` & `testmypixipkg-0.13.0/releaserc.toml`

 * *Files identical despite different names*

### Comparing `testmypixipkg-0.12.0/.github/workflows/main.yaml` & `testmypixipkg-0.13.0/.github/workflows/main.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         os: [ubuntu-latest]
         python-version: ["3.12"]
         environments: [dev]
         # os: [ubuntu-latest, macos-latest, macos-14, windows-latest]
         # python-version: ["3.12", "3.11", "3.10"]
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install Pixi
@@ -46,22 +46,36 @@
         # only upload if matrix.os is ubuntu-latest and matrix.python-version is 3.12
         if: matrix.os == 'ubuntu-latest' && matrix.python-version == '3.12'
         uses: actions/upload-artifact@v2
         with:
           name: coverage-report
           path: coverage-report
 
-  Continuous-Deployment:
+  Ruff:
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v4
+      - name: Install Pixi
+        uses: prefix-dev/setup-pixi@v0.7.0
+        with:
+          environments: dev
+          pixi-version: v0.22.0
+          cache: true
+          locked: false
+      - name: Run Ruff
+        run: pixi run style
+
+  Semantic-Release:
     permissions:
       contents: write
       packages: write
       issues: write
       pull-requests: write
 
-    # needs: [Unit-Tests]
+    needs: [Unit-Tests, Ruff]
 
     # if pulling to main, deploy to PyPI
     if: github.ref == 'refs/heads/main'
 
     strategy:
       matrix:
         os: [ubuntu-latest]
@@ -95,28 +109,28 @@
         id: release
         uses: python-semantic-release/python-semantic-release@master
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           root_options: "-v --config releaserc.toml"
 
   Publish-To-PyPi:
-    needs: Continuous-Deployment
-    if: needs.Continuous-Deployment.outputs.released == 'true'
+    needs: Semantic-Release
+    if: needs.Semantic-Release.outputs.released == 'true'
     strategy:
       matrix:
         os: [ubuntu-latest]
         python-version: ["3.12"]
         environments: [publish]
 
     runs-on: ${{ matrix.os }}
     steps:
-      - name: Checkout the code with tag ${{ needs.Continuous-Deployment.outputs.tag }}
-        uses: actions/checkout@v3
+      - name: Checkout the code with tag ${{ needs.Semantic-Release.outputs.tag }}
+        uses: actions/checkout@v4
         with:
-          ref: ${{ needs.Continuous-Deployment.outputs.tag }}
+          ref: ${{ needs.Semantic-Release.outputs.tag }}
 
       - name: Install Pixi
         uses: prefix-dev/setup-pixi@v0.7.0
         with:
           environments: ${{ matrix.environments}}
           pixi-version: v0.22.0
           cache: true
@@ -136,45 +150,45 @@
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest]
         python-version: ["3.12"]
         environments: [publish]
 
     steps:
-      - name: Checkout the code with tag ${{ needs.Continuous-Deployment.outputs.tag }}
-        uses: actions/checkout@v3
+      - name: Checkout the code with tag ${{ needs.Semantic-Release.outputs.tag }}
+        uses: actions/checkout@v4
         with:
-          ref: ${{ needs.Continuous-Deployment.outputs.tag }}
+          ref: ${{ needs.Semantic-Release.outputs.tag }}
 
       - name: setup python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install using PyPI
         run: |
           pip install testmypixipkg
 
   Publish-To-Test-PyPi:
-    needs: Continuous-Deployment
+    needs: Semantic-Release
 
-    if: needs.Continuous-Deployment.outputs.released == 'true'
+    if: needs.Semantic-Release.outputs.released == 'true'
     strategy:
       matrix:
         os: [ubuntu-latest]
         python-version: ["3.12"]
         environments: [publish]
 
     runs-on: ${{ matrix.os }}
 
     steps:
-      - name: Checkout the code with tag ${{ needs.Continuous-Deployment.outputs.tag }}
-        uses: actions/checkout@v3
+      - name: Checkout the code with tag ${{ needs.Semantic-Release.outputs.tag }}
+        uses: actions/checkout@v4
         with:
-          ref: ${{ needs.Continuous-Deployment.outputs.tag }}
+          ref: ${{ needs.Semantic-Release.outputs.tag }}
 
       - name: Install Pixi
         uses: prefix-dev/setup-pixi@v0.7.0
         with:
           environments: ${{ matrix.environments}}
           pixi-version: v0.22.0
           cache: true
@@ -193,18 +207,18 @@
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest]
         python-version: ["3.12"]
         environments: [publish]
 
     steps:
-      - name: Checkout the code with tag ${{ needs.Continuous-Deployment.outputs.tag }}
-        uses: actions/checkout@v3
+      - name: Checkout the code with tag ${{ needs.Semantic-Release.outputs.tag }}
+        uses: actions/checkout@v4
         with:
-          ref: ${{ needs.Continuous-Deployment.outputs.tag }}
+          ref: ${{ needs.Semantic-Release.outputs.tag }}
 
       - name: setup python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install using TestPyPI
```

### Comparing `testmypixipkg-0.12.0/.gitignore` & `testmypixipkg-0.13.0/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -157,8 +157,9 @@
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 .pixi
 
-coverage-report
+coverage-report
+recipe.yaml
```

