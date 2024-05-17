# Comparing `tmp/example_python_package_with_rust_backend-1.1.4.tar.gz` & `tmp/example_python_package_with_rust_backend-1.1.6.tar.gz`

## Comparing `example_python_package_with_rust_backend-1.1.4.tar` & `example_python_package_with_rust_backend-1.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      379 1970-01-01 00:00:00.000000 example_python_package_with_rust_backend-1.1.4/Cargo.toml
--rw-r--r--   0     1001      127     3752 2024-05-17 21:18:40.000000 example_python_package_with_rust_backend-1.1.4/.github/workflows/python-publish.yml
--rw-r--r--   0     1001      127     1073 2024-05-17 21:18:40.000000 example_python_package_with_rust_backend-1.1.4/LICENSE.txt
--rw-r--r--   0     1001      127      163 2024-05-17 21:18:40.000000 example_python_package_with_rust_backend-1.1.4/README.md
--rw-r--r--   0     1001      127      115 2024-05-17 21:18:40.000000 example_python_package_with_rust_backend-1.1.4/examples/usage.py
--rw-r--r--   0     1001      127      435 2024-05-17 21:18:40.000000 example_python_package_with_rust_backend-1.1.4/src/lib.rs
--rw-r--r--   0     1001      127     7686 2024-05-17 21:18:40.000000 example_python_package_with_rust_backend-1.1.4/Cargo.lock
--rw-r--r--   0     1001      127      417 2024-05-17 21:18:40.000000 example_python_package_with_rust_backend-1.1.4/pyproject.toml
--rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 example_python_package_with_rust_backend-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      379 1970-01-01 00:00:00.000000 example_python_package_with_rust_backend-1.1.6/Cargo.toml
+-rw-r--r--   0      501       20     3796 2024-05-17 21:43:36.000000 example_python_package_with_rust_backend-1.1.6/.github/workflows/python-publish.yml
+-rw-r--r--   0      501       20     1073 2024-05-17 21:43:36.000000 example_python_package_with_rust_backend-1.1.6/LICENSE.txt
+-rw-r--r--   0      501       20      999 2024-05-17 21:43:36.000000 example_python_package_with_rust_backend-1.1.6/README.md
+-rw-r--r--   0      501       20      115 2024-05-17 21:43:36.000000 example_python_package_with_rust_backend-1.1.6/examples/usage.py
+-rw-r--r--   0      501       20      759 2024-05-17 21:43:36.000000 example_python_package_with_rust_backend-1.1.6/src/lib.rs
+-rw-r--r--   0      501       20     7686 2024-05-17 21:43:36.000000 example_python_package_with_rust_backend-1.1.6/Cargo.lock
+-rw-r--r--   0      501       20      417 2024-05-17 21:43:36.000000 example_python_package_with_rust_backend-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1384 1970-01-01 00:00:00.000000 example_python_package_with_rust_backend-1.1.6/PKG-INFO
```

### Comparing `example_python_package_with_rust_backend-1.1.4/.github/workflows/python-publish.yml` & `example_python_package_with_rust_backend-1.1.6/.github/workflows/python-publish.yml`

 * *Files 6% similar despite different names*

```diff
@@ -9,46 +9,47 @@
     branches:
       - main
   release:
     types:
       - published
 
 jobs:
-  # macos:
+  macos:
     # erros on Library not loaded: /usr/local/opt/gettext/lib/libintl.8.dylib
   #   runs-on: macos-latest
-  #   steps:
-  #     - uses: actions/checkout@v4
-  #     - uses: actions/setup-python@v5
-  #       with:
-  #         python-version: 3.9
-  #         architecture: x64
-  #     - name: Build wheels - x86_64
-  #       uses: PyO3/maturin-action@v1
-  #       with:
-  #         target: x86_64
-  #         args: --release --out dist --sdist
-  #     - name: Install built wheel - x86_64
-  #       run: |
-  #         pip install example_python_package_with_rust_backend --no-index --find-links dist --force-reinstall
-  #     - name: Build wheels - universal2
-  #       uses: PyO3/maturin-action@v1
-  #       with:
-  #         target: universal2-apple-darwin
-  #         args: --release --out dist
-  #     - name: Install built wheel - universal2
-  #       run: |
-  #         pip install example_python_package_with_rust_backend --no-index --find-links dist --force-reinstall
-  #         python -c "import example_python_package_with_rust_backend"
-  #     - name: Upload wheels
-  #       uses: actions/upload-artifact@v3
-  #       uses: actions/upload-artifact@v4 breaks due to artifact names being the same3
-  #       with:
-  #         name: wheels
-  #         path: dist
+    runs-on: macos-13
+    steps:
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
+        with:
+          python-version: 3.9
+          architecture: x64
+      - name: Build wheels - x86_64
+        uses: PyO3/maturin-action@v1
+        with:
+          target: x86_64
+          args: --release --out dist --sdist
+      - name: Install built wheel - x86_64
+        run: |
+          pip install example_python_package_with_rust_backend --no-index --find-links dist --force-reinstall
+      - name: Build wheels - universal2
+        uses: PyO3/maturin-action@v1
+        with:
+          target: universal2-apple-darwin
+          args: --release --out dist
+      - name: Install built wheel - universal2
+        run: |
+          pip install example_python_package_with_rust_backend --no-index --find-links dist --force-reinstall
+          python -c "import example_python_package_with_rust_backend"
+      - name: Upload wheels
+        uses: actions/upload-artifact@v3
+        # uses: actions/upload-artifact@v4 breaks due to artifact names being the same3
+        with:
+          name: wheels
+          path: dist
 
   windows:
     runs-on: windows-latest
     strategy:
       matrix:
         target: [x64]
     steps:
@@ -100,20 +101,21 @@
       # uses: actions/upload-artifact@v4 breaks due to artifact names being the same
       with:
         name: wheels
         path: dist
 
   upload_pypi:
     runs-on: ubuntu-latest
-    needs: [ linux, windows]
+    needs: [ linux, windows, macos]
     permissions:
       contents: read
       id-token: write
     steps:
       - uses: actions/download-artifact@v3
+      # - uses: actions/download-artifact@v4 does not find the artifacts
         with:
           name: wheels
           path: dist
       - name: List artifacts
         run: ls -lhs
       - name: Publish package distributions to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `example_python_package_with_rust_backend-1.1.4/LICENSE.txt` & `example_python_package_with_rust_backend-1.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `example_python_package_with_rust_backend-1.1.4/Cargo.lock` & `example_python_package_with_rust_backend-1.1.6/Cargo.lock`

 * *Files identical despite different names*

