# Comparing `tmp/example_python_package_with_rust_backend-0.1.0.tar.gz` & `tmp/example_python_package_with_rust_backend-1.1.2.tar.gz`

## Comparing `example_python_package_with_rust_backend-0.1.0.tar` & `example_python_package_with_rust_backend-1.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      379 1970-01-01 00:00:00.000000 example_python_package_with_rust_backend-0.1.0/Cargo.toml
--rw-r--r--   0     1001      127     2084 2024-05-17 16:51:01.000000 example_python_package_with_rust_backend-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0     1001      127     1073 2024-05-17 16:51:01.000000 example_python_package_with_rust_backend-0.1.0/LICENSE.txt
--rw-r--r--   0     1001      127      163 2024-05-17 16:51:01.000000 example_python_package_with_rust_backend-0.1.0/README.md
--rw-r--r--   0     1001      127      115 2024-05-17 16:51:01.000000 example_python_package_with_rust_backend-0.1.0/examples/usage.py
--rw-r--r--   0     1001      127      435 2024-05-17 16:51:01.000000 example_python_package_with_rust_backend-0.1.0/src/lib.rs
--rw-r--r--   0     1001      127     7686 2024-05-17 16:51:01.000000 example_python_package_with_rust_backend-0.1.0/Cargo.lock
--rw-r--r--   0     1001      127      452 2024-05-17 16:51:01.000000 example_python_package_with_rust_backend-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 example_python_package_with_rust_backend-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      379 1970-01-01 00:00:00.000000 example_python_package_with_rust_backend-1.1.2/Cargo.toml
+-rw-r--r--   0     1001      127     2121 2024-05-17 18:19:19.000000 example_python_package_with_rust_backend-1.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0     1001      127     1073 2024-05-17 18:19:19.000000 example_python_package_with_rust_backend-1.1.2/LICENSE.txt
+-rw-r--r--   0     1001      127      163 2024-05-17 18:19:19.000000 example_python_package_with_rust_backend-1.1.2/README.md
+-rw-r--r--   0     1001      127      115 2024-05-17 18:19:19.000000 example_python_package_with_rust_backend-1.1.2/examples/usage.py
+-rw-r--r--   0     1001      127      435 2024-05-17 18:19:19.000000 example_python_package_with_rust_backend-1.1.2/src/lib.rs
+-rw-r--r--   0     1001      127     7686 2024-05-17 18:19:19.000000 example_python_package_with_rust_backend-1.1.2/Cargo.lock
+-rw-r--r--   0     1001      127      417 2024-05-17 18:19:19.000000 example_python_package_with_rust_backend-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 example_python_package_with_rust_backend-1.1.2/PKG-INFO
```

### Comparing `example_python_package_with_rust_backend-0.1.0/.github/workflows/python-publish.yml` & `example_python_package_with_rust_backend-1.1.2/.github/workflows/python-publish.yml`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,16 @@
         with:
           name: wheels
           path: dist
       - name: List artifacts
         run: ls -lhs
       - name: Publish package distributions to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
-
+        with:
+          verbose: true
 
 
       # name: PyPI Python Package
 
 # on:
 #   release:
 #     types: [published]
```

### Comparing `example_python_package_with_rust_backend-0.1.0/LICENSE.txt` & `example_python_package_with_rust_backend-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `example_python_package_with_rust_backend-0.1.0/Cargo.lock` & `example_python_package_with_rust_backend-1.1.2/Cargo.lock`

 * *Files identical despite different names*

### Comparing `example_python_package_with_rust_backend-0.1.0/PKG-INFO` & `example_python_package_with_rust_backend-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: example_python_package_with_rust_backend
-Version: 0.1.0
+Version: 1.1.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE.txt
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

