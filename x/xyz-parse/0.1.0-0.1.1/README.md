# Comparing `tmp/xyz_parse-0.1.0.tar.gz` & `tmp/xyz_parse-0.1.1.tar.gz`

## Comparing `xyz_parse-0.1.0.tar` & `xyz_parse-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 xyz_parse-0.1.0/Cargo.toml
--rw-r--r--   0     1001      127     2674 2024-05-17 14:26:01.000000 xyz_parse-0.1.0/.github/workflows/cd.yaml
--rw-r--r--   0     1001      127      583 2024-05-17 14:26:01.000000 xyz_parse-0.1.0/.github/workflows/ci.yaml
--rw-r--r--   0     1001      127      697 2024-05-17 14:26:01.000000 xyz_parse-0.1.0/.gitignore
--rw-r--r--   0     1001      127      308 2024-05-17 14:26:01.000000 xyz_parse-0.1.0/README.md
--rw-r--r--   0     1001      127     3214 2024-05-17 14:26:01.000000 xyz_parse-0.1.0/src/atom.rs
--rw-r--r--   0     1001      127      572 2024-05-17 14:26:01.000000 xyz_parse-0.1.0/src/lib.rs
--rw-r--r--   0     1001      127     4699 2024-05-17 14:26:01.000000 xyz_parse-0.1.0/src/molecule.rs
--rw-r--r--   0     1001      127     4664 2024-05-17 14:26:01.000000 xyz_parse-0.1.0/src/python.rs
--rw-r--r--   0     1001      127     8048 2024-05-17 14:26:01.000000 xyz_parse-0.1.0/src/xyz.rs
--rw-r--r--   0     1001      127     8787 2024-05-17 14:26:04.000000 xyz_parse-0.1.0/Cargo.lock
--rw-r--r--   0     1001      127      390 2024-05-17 14:26:01.000000 xyz_parse-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 xyz_parse-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 xyz_parse-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      127     2674 2024-05-17 14:38:45.000000 xyz_parse-0.1.1/.github/workflows/cd.yaml
+-rw-r--r--   0     1001      127      583 2024-05-17 14:38:45.000000 xyz_parse-0.1.1/.github/workflows/ci.yaml
+-rw-r--r--   0     1001      127      697 2024-05-17 14:38:45.000000 xyz_parse-0.1.1/.gitignore
+-rw-r--r--   0     1001      127      308 2024-05-17 14:38:45.000000 xyz_parse-0.1.1/README.md
+-rw-r--r--   0     1001      127     3214 2024-05-17 14:38:45.000000 xyz_parse-0.1.1/src/atom.rs
+-rw-r--r--   0     1001      127      572 2024-05-17 14:38:45.000000 xyz_parse-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      127     4699 2024-05-17 14:38:45.000000 xyz_parse-0.1.1/src/molecule.rs
+-rw-r--r--   0     1001      127     4664 2024-05-17 14:38:45.000000 xyz_parse-0.1.1/src/python.rs
+-rw-r--r--   0     1001      127     8048 2024-05-17 14:38:45.000000 xyz_parse-0.1.1/src/xyz.rs
+-rw-r--r--   0     1001      127     8787 2024-05-17 14:38:49.000000 xyz_parse-0.1.1/Cargo.lock
+-rw-r--r--   0     1001      127      375 2024-05-17 14:38:45.000000 xyz_parse-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 xyz_parse-0.1.1/PKG-INFO
```

### Comparing `xyz_parse-0.1.0/Cargo.toml` & `xyz_parse-0.1.1/Cargo.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "xyz-parse"
-version = "0.1.0"
+version = "0.1.1"
 edition = "2021"
 authors = ["Julian Popescu <jpopesculian@gmail.com>"]
 license = "MIT OR Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/aqora-io/xyz-parse"
 documentation = "https://docs.rs/xyz-parse/"
 repository = "https://github.com/aqora-io/xyz-parse"
```

### Comparing `xyz_parse-0.1.0/.github/workflows/cd.yaml` & `xyz_parse-0.1.1/.github/workflows/cd.yaml`

 * *Files identical despite different names*

### Comparing `xyz_parse-0.1.0/.github/workflows/ci.yaml` & `xyz_parse-0.1.1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `xyz_parse-0.1.0/.gitignore` & `xyz_parse-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `xyz_parse-0.1.0/src/atom.rs` & `xyz_parse-0.1.1/src/atom.rs`

 * *Files identical despite different names*

### Comparing `xyz_parse-0.1.0/src/lib.rs` & `xyz_parse-0.1.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `xyz_parse-0.1.0/src/molecule.rs` & `xyz_parse-0.1.1/src/molecule.rs`

 * *Files identical despite different names*

### Comparing `xyz_parse-0.1.0/src/python.rs` & `xyz_parse-0.1.1/src/python.rs`

 * *Files identical despite different names*

### Comparing `xyz_parse-0.1.0/src/xyz.rs` & `xyz_parse-0.1.1/src/xyz.rs`

 * *Files identical despite different names*

### Comparing `xyz_parse-0.1.0/Cargo.lock` & `xyz_parse-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -311,12 +311,12 @@
 name = "windows_x86_64_msvc"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "xyz-parse"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "pyo3",
  "rust_decimal",
 ]
```

### Comparing `xyz_parse-0.1.0/PKG-INFO` & `xyz_parse-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: xyz-parse
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Simple parser for the XYZ file format
 Keywords: xyz,chemistry,parser,parse
 Home-Page: https://github.com/aqora-io/xyz-parse
 Author: Julian Popescu <jpopesculian@gmail.com>
```

