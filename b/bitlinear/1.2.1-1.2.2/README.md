# Comparing `tmp/bitlinear-1.2.1.tar.gz` & `tmp/bitlinear-1.2.2.tar.gz`

## Comparing `bitlinear-1.2.1.tar` & `bitlinear-1.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 bitlinear-1.2.1/bitlinear/__init__.py
--rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 bitlinear-1.2.1/bitlinear/bitlinear.py
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 bitlinear-1.2.1/bitlinear/kernels.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bitlinear-1.2.1/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bitlinear-1.2.1/LICENSE
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bitlinear-1.2.1/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bitlinear-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 bitlinear-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 bitlinear-1.2.2/bitlinear/__init__.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 bitlinear-1.2.2/bitlinear/bitlinear.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 bitlinear-1.2.2/bitlinear/kernels.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bitlinear-1.2.2/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bitlinear-1.2.2/LICENSE
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bitlinear-1.2.2/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bitlinear-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 bitlinear-1.2.2/PKG-INFO
```

### Comparing `bitlinear-1.2.1/bitlinear/bitlinear.py` & `bitlinear-1.2.2/bitlinear/bitlinear.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         self.w_min = w_min if w_min is not None else ceil(-2**(weight_bits-1))
 
     def __repr__(self):
         return f"BitLinear(in_features={self.in_features}, out_features={self.out_features}, bias={self.bias is not None}, eps={self.eps}, weight_bits={self.weight_bits}, activation_bits={self.activation_bits}, x_max={self.x_max}, x_min={self.x_min}, w_max={self.w_max}, w_min={self.w_min}, kernel={self.kernel}, measure={self.measure})"
 
     def forward(self, x):
         x_norm = torch.layer_norm(x, x.size()[1:])
-        x_scale = self.Q_b / x_norm.detach().abs().max(dim=-1, keepdim=True).values.clamp_(min=self.eps)
+        x_scale = self.x_max / x_norm.detach().abs().max(dim=-1, keepdim=True).values.clamp_(min=self.eps)
         x_quant = round_clamp(x_norm * x_scale, -self.x_min, self.x_max)
         w_scale = 1 / self.measure(self.weight.detach().abs()).clamp_(min=self.eps)
         w_quant = round_clamp(self.weight * w_scale, self.y_min, self.y_max)
         y_quant = self.kernel(x_quant, w_quant, self.bias)
         y = y_quant / (w_scale * x_scale)
         return y
```

### Comparing `bitlinear-1.2.1/bitlinear/kernels.py` & `bitlinear-1.2.2/bitlinear/kernels.py`

 * *Files identical despite different names*

### Comparing `bitlinear-1.2.1/LICENSE` & `bitlinear-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bitlinear-1.2.1/README.md` & `bitlinear-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `bitlinear-1.2.1/pyproject.toml` & `bitlinear-1.2.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bitlinear"
-version = "1.2.1"
+version = "1.2.2"
 authors = [
   { name = "Peter Schneider-Kamp" }
 ]
 
 description = "An production-ready implementation of 1.58 bit quantization-aware training and inference."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `bitlinear-1.2.1/PKG-INFO` & `bitlinear-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bitlinear
-Version: 1.2.1
+Version: 1.2.2
 Summary: An production-ready implementation of 1.58 bit quantization-aware training and inference.
 Project-URL: Homepage, https://github.com/schneiderkamplab/bitlinear
 Project-URL: Bug Tracker, https://github.com/schneiderkamplab/bitlinear/issues
 Author: Peter Schneider-Kamp
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

