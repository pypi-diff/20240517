# Comparing `tmp/znh5md-0.1.7.tar.gz` & `tmp/znh5md-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "znh5md-0.1.7.tar", max compression
+gzip compressed data, was "znh5md-0.1.9.tar", max compression
```

## Comparing `znh5md-0.1.7.tar` & `znh5md-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    13576 2023-05-16 13:50:54.924529 znh5md-0.1.7/LICENSE
--rw-r--r--   0        0        0     3004 2023-05-16 13:50:54.934529 znh5md-0.1.7/README.md
--rw-r--r--   0        0        0     1189 2023-05-16 13:50:54.934529 znh5md-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      450 2023-05-16 13:50:54.934529 znh5md-0.1.7/znh5md/__init__.py
--rw-r--r--   0        0        0     1404 2023-05-16 13:00:33.797385 znh5md-0.1.7/znh5md/cli.py
--rw-r--r--   0        0        0     3638 2023-05-16 13:00:33.807385 znh5md-0.1.7/znh5md/format/__init__.py
--rw-r--r--   0        0        0      289 2023-05-16 13:50:54.934529 znh5md-0.1.7/znh5md/io/__init__.py
--rw-r--r--   0        0        0     9759 2023-05-16 13:50:54.934529 znh5md-0.1.7/znh5md/io/base.py
--rw-r--r--   0        0        0    11166 2023-05-16 13:50:54.944529 znh5md-0.1.7/znh5md/io/reader.py
--rw-r--r--   0        0        0      179 2023-03-26 12:05:45.108922 znh5md-0.1.7/znh5md/utils.py
--rw-r--r--   0        0        0      268 2023-05-16 13:50:54.944529 znh5md-0.1.7/znh5md/znh5md/__init__.py
--rw-r--r--   0        0        0      365 2023-05-16 13:50:54.944529 znh5md-0.1.7/znh5md/znh5md/base.py
--rw-r--r--   0        0        0     4402 2023-05-16 13:50:54.944529 znh5md-0.1.7/znh5md/znh5md/h5ase.py
--rw-r--r--   0        0        0     7393 2023-05-16 13:50:54.944529 znh5md-0.1.7/znh5md/znh5md/h5dask.py
--rw-r--r--   0        0        0     3812 1970-01-01 00:00:00.000000 znh5md-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    13576 2023-05-16 13:50:54.924529 znh5md-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3004 2023-05-16 13:50:54.934529 znh5md-0.1.9/README.md
+-rw-r--r--   0        0        0     1189 2023-12-21 12:25:46.145783 znh5md-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      450 2023-09-09 08:21:07.220775 znh5md-0.1.9/znh5md/__init__.py
+-rw-r--r--   0        0        0     1404 2023-05-16 13:00:33.797385 znh5md-0.1.9/znh5md/cli.py
+-rw-r--r--   0        0        0     3638 2023-08-09 11:20:36.736216 znh5md-0.1.9/znh5md/format/__init__.py
+-rw-r--r--   0        0        0      289 2023-05-16 13:50:54.934529 znh5md-0.1.9/znh5md/io/__init__.py
+-rw-r--r--   0        0        0     9759 2023-05-16 13:50:54.934529 znh5md-0.1.9/znh5md/io/base.py
+-rw-r--r--   0        0        0    11166 2023-12-21 12:07:45.337494 znh5md-0.1.9/znh5md/io/reader.py
+-rw-r--r--   0        0        0      179 2023-12-21 12:07:45.337494 znh5md-0.1.9/znh5md/utils.py
+-rw-r--r--   0        0        0      268 2023-05-16 13:50:54.944529 znh5md-0.1.9/znh5md/znh5md/__init__.py
+-rw-r--r--   0        0        0      365 2023-05-16 13:50:54.944529 znh5md-0.1.9/znh5md/znh5md/base.py
+-rw-r--r--   0        0        0     4526 2023-12-21 12:25:46.155783 znh5md-0.1.9/znh5md/znh5md/h5ase.py
+-rw-r--r--   0        0        0     7393 2023-05-16 13:50:54.944529 znh5md-0.1.9/znh5md/znh5md/h5dask.py
+-rw-r--r--   0        0        0     3812 1970-01-01 00:00:00.000000 znh5md-0.1.9/PKG-INFO
```

### Comparing `znh5md-0.1.7/LICENSE` & `znh5md-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `znh5md-0.1.7/README.md` & `znh5md-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `znh5md-0.1.7/pyproject.toml` & `znh5md-0.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "znh5md"
-version = "0.1.7"
+version = "0.1.9"
 description = "High Performance Interface for H5MD Trajectories"
 authors = ["zincwarecode <zincwarecode@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `znh5md-0.1.7/znh5md/cli.py` & `znh5md-0.1.9/znh5md/cli.py`

 * *Files identical despite different names*

### Comparing `znh5md-0.1.7/znh5md/format/__init__.py` & `znh5md-0.1.9/znh5md/format/__init__.py`

 * *Files identical despite different names*

### Comparing `znh5md-0.1.7/znh5md/io/base.py` & `znh5md-0.1.9/znh5md/io/base.py`

 * *Files identical despite different names*

### Comparing `znh5md-0.1.7/znh5md/io/reader.py` & `znh5md-0.1.9/znh5md/io/reader.py`

 * *Files identical despite different names*

### Comparing `znh5md-0.1.7/znh5md/znh5md/h5ase.py` & `znh5md-0.1.9/znh5md/znh5md/h5ase.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,23 @@
 
 
 def _gather_value(particles_data, key, idx):
     """Helper to gather the value for a given key and index.
 
     Returns None if the key is not present in the data.
     """
-    if key in particles_data:
-        if key in [GRP.species, GRP.position, GRP.velocity, GRP.forces, GRP.momentum]:
-            # use PARTICLES_GRP
-            return rm_nan(particles_data[key][idx])
-        return particles_data[key][idx]
+    try:
+        if key in particles_data:
+            if key in [GRP.species, GRP.position, GRP.velocity, GRP.forces, GRP.momentum]:
+                # use PARTICLES_GRP
+                return rm_nan(particles_data[key][idx])
+            return particles_data[key][idx]
+    except IndexError:
+        # a property might not be available at all frames.
+        pass
     return None
 
 
 @dataclasses.dataclass
 class ASEH5MD(H5MDBase):
     """ASE interface for H5MD files.
```

### Comparing `znh5md-0.1.7/znh5md/znh5md/h5dask.py` & `znh5md-0.1.9/znh5md/znh5md/h5dask.py`

 * *Files identical despite different names*

### Comparing `znh5md-0.1.7/PKG-INFO` & `znh5md-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: znh5md
-Version: 0.1.7
+Version: 0.1.9
 Summary: High Performance Interface for H5MD Trajectories
 License: Apache-2.0
 Author: zincwarecode
 Author-email: zincwarecode@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

