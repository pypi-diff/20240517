# Comparing `tmp/bitlinear-1.2.0.tar.gz` & `tmp/bitlinear-1.2.1.tar.gz`

## Comparing `bitlinear-1.2.0.tar` & `bitlinear-1.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 bitlinear-1.2.0/bitlinear/__init__.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 bitlinear-1.2.0/bitlinear/bitlinear.py
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 bitlinear-1.2.0/bitlinear/kernels.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bitlinear-1.2.0/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bitlinear-1.2.0/LICENSE
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bitlinear-1.2.0/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bitlinear-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 bitlinear-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 bitlinear-1.2.1/bitlinear/__init__.py
+-rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 bitlinear-1.2.1/bitlinear/bitlinear.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 bitlinear-1.2.1/bitlinear/kernels.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bitlinear-1.2.1/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bitlinear-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bitlinear-1.2.1/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bitlinear-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 bitlinear-1.2.1/PKG-INFO
```

### Comparing `bitlinear-1.2.0/bitlinear/bitlinear.py` & `bitlinear-1.2.1/bitlinear/bitlinear.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,16 @@
             bias=bias,
             device=device,
             dtype=dtype,
         )
         self.eps = eps
         self.kernel = kernel
         self.measure = measure
+        self.activation_bits = activation_bits
+        self.weight_bits = weight_bits
         self.x_max = x_max if x_max is not None else ceil(2**(activation_bits-1)-1)
         self.x_min = x_min if x_min is not None else ceil(-2**(activation_bits-1))
         self.w_max = w_max if w_max is not None else ceil(2**(weight_bits-1)-1)
         self.w_min = w_min if w_min is not None else ceil(-2**(weight_bits-1))
 
     def __repr__(self):
         return f"BitLinear(in_features={self.in_features}, out_features={self.out_features}, bias={self.bias is not None}, eps={self.eps}, weight_bits={self.weight_bits}, activation_bits={self.activation_bits}, x_max={self.x_max}, x_min={self.x_min}, w_max={self.w_max}, w_min={self.w_min}, kernel={self.kernel}, measure={self.measure})"
```

### Comparing `bitlinear-1.2.0/bitlinear/kernels.py` & `bitlinear-1.2.1/bitlinear/kernels.py`

 * *Files identical despite different names*

### Comparing `bitlinear-1.2.0/LICENSE` & `bitlinear-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bitlinear-1.2.0/README.md` & `bitlinear-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `bitlinear-1.2.0/pyproject.toml` & `bitlinear-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bitlinear"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name = "Peter Schneider-Kamp" }
 ]
 
 description = "An production-ready implementation of 1.58 bit quantization-aware training and inference."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `bitlinear-1.2.0/PKG-INFO` & `bitlinear-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bitlinear
-Version: 1.2.0
+Version: 1.2.1
 Summary: An production-ready implementation of 1.58 bit quantization-aware training and inference.
 Project-URL: Homepage, https://github.com/schneiderkamplab/bitlinear
 Project-URL: Bug Tracker, https://github.com/schneiderkamplab/bitlinear/issues
 Author: Peter Schneider-Kamp
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

