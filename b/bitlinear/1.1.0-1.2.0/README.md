# Comparing `tmp/bitlinear-1.1.0.tar.gz` & `tmp/bitlinear-1.2.0.tar.gz`

## Comparing `bitlinear-1.1.0.tar` & `bitlinear-1.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 bitlinear-1.1.0/bitlinear/__init__.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 bitlinear-1.1.0/bitlinear/bitlinear.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 bitlinear-1.1.0/bitlinear/kernels.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bitlinear-1.1.0/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bitlinear-1.1.0/LICENSE
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bitlinear-1.1.0/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bitlinear-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 bitlinear-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 bitlinear-1.2.0/bitlinear/__init__.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 bitlinear-1.2.0/bitlinear/bitlinear.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 bitlinear-1.2.0/bitlinear/kernels.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bitlinear-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bitlinear-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bitlinear-1.2.0/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bitlinear-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 bitlinear-1.2.0/PKG-INFO
```

### Comparing `bitlinear-1.1.0/bitlinear/bitlinear.py` & `bitlinear-1.2.0/bitlinear/bitlinear.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from math import ceil
 import torch
 import torch.nn as nn
 
 from .kernels import TorchLinear
 
 def round_clamp(input, min, max):
     return (input.round().clamp(min, max) - input).detach() + input
@@ -11,40 +12,47 @@
             self,
             in_features,
             out_features,
             bias=True,
             device=None,
             dtype=None,
             eps=1e-5,
+            weight_bits=1.58,
             activation_bits=8,
+            x_max=None,
+            x_min=None,
+            w_max=None,
+            w_min=None,
             kernel=TorchLinear(),
             measure=torch.median,
         ):
         super(BitLinear, self).__init__(
             in_features=in_features,
             out_features=out_features,
             bias=bias,
             device=device,
             dtype=dtype,
         )
         self.eps = eps
-        self.activation_bits = activation_bits
         self.kernel = kernel
         self.measure = measure
-        self.Q_b = 2**(activation_bits-1)-1
+        self.x_max = x_max if x_max is not None else ceil(2**(activation_bits-1)-1)
+        self.x_min = x_min if x_min is not None else ceil(-2**(activation_bits-1))
+        self.w_max = w_max if w_max is not None else ceil(2**(weight_bits-1)-1)
+        self.w_min = w_min if w_min is not None else ceil(-2**(weight_bits-1))
 
     def __repr__(self):
-        return f"BitLinear(in_features={self.in_features}, out_features={self.out_features}, bias={self.bias is not None}, eps={self.eps}, activation_bits={self.activation_bits}, kernel={self.kernel})"
+        return f"BitLinear(in_features={self.in_features}, out_features={self.out_features}, bias={self.bias is not None}, eps={self.eps}, weight_bits={self.weight_bits}, activation_bits={self.activation_bits}, x_max={self.x_max}, x_min={self.x_min}, w_max={self.w_max}, w_min={self.w_min}, kernel={self.kernel}, measure={self.measure})"
 
     def forward(self, x):
         x_norm = torch.layer_norm(x, x.size()[1:])
         x_scale = self.Q_b / x_norm.detach().abs().max(dim=-1, keepdim=True).values.clamp_(min=self.eps)
-        x_quant = round_clamp(x_norm * x_scale, -self.Q_b-1, self.Q_b)
+        x_quant = round_clamp(x_norm * x_scale, -self.x_min, self.x_max)
         w_scale = 1 / self.measure(self.weight.detach().abs()).clamp_(min=self.eps)
-        w_quant = round_clamp(self.weight * w_scale, -1, 1)
+        w_quant = round_clamp(self.weight * w_scale, self.y_min, self.y_max)
         y_quant = self.kernel(x_quant, w_quant, self.bias)
         y = y_quant / (w_scale * x_scale)
         return y
 
 def replace_modules(model, old_class=nn.Linear, new_class=BitLinear, new_class_kwargs={}):
     for name, module in model.named_children():
         if isinstance(module, old_class):
```

### Comparing `bitlinear-1.1.0/bitlinear/kernels.py` & `bitlinear-1.2.0/bitlinear/kernels.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         output = [[sum(input[i][k] * weight[j][k] for k in range(m)) + (bias[j] if bias is not None else 0) for j in range(p)] for i in range(n)]
         return torch.Tensor(output)
 
 class TernaryNaive(Kernel):
     def __call__(input, weight, bias=None):
         input = input.tolist()
         weight = weight.tolist()
+        assert all(all(x in {-1, 0, 1} for x in row) for row in input)
         if bias is not None:
             bias = bias.tolist()
         output = []
         n = len(input)
         m = len(input[0])
         p = len(weight)
         for i in range(n):
```

### Comparing `bitlinear-1.1.0/LICENSE` & `bitlinear-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bitlinear-1.1.0/README.md` & `bitlinear-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bitlinear-1.1.0/pyproject.toml` & `bitlinear-1.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bitlinear"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
   { name = "Peter Schneider-Kamp" }
 ]
 
 description = "An production-ready implementation of 1.58 bit quantization-aware training and inference."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `bitlinear-1.1.0/PKG-INFO` & `bitlinear-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bitlinear
-Version: 1.1.0
+Version: 1.2.0
 Summary: An production-ready implementation of 1.58 bit quantization-aware training and inference.
 Project-URL: Homepage, https://github.com/schneiderkamplab/bitlinear
 Project-URL: Bug Tracker, https://github.com/schneiderkamplab/bitlinear/issues
 Author: Peter Schneider-Kamp
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

