# Comparing `tmp/torch_contour-0.0.6.tar.gz` & `tmp/torch_contour-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_contour-0.0.6.tar", last modified: Tue May 14 12:00:11 2024, max compression
+gzip compressed data, was "torch_contour-1.0.0.tar", last modified: Fri May 17 14:34:24 2024, max compression
```

## Comparing `torch_contour-0.0.6.tar` & `torch_contour-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxr-x   0 antoine   (1001) antoine   (1001)        0 2024-05-14 12:00:11.232465 torch_contour-0.0.6/
--rw-rw-r--   0 antoine   (1001) antoine   (1001)     1068 2023-12-06 15:01:07.000000 torch_contour-0.0.6/LICENSE
--rw-rw-r--   0 antoine   (1001) antoine   (1001)     3007 2024-05-14 12:00:11.232465 torch_contour-0.0.6/PKG-INFO
--rw-rw-r--   0 antoine   (1001) antoine   (1001)     1626 2024-05-14 11:54:57.000000 torch_contour-0.0.6/README.md
--rw-rw-r--   0 antoine   (1001) antoine   (1001)      138 2023-12-06 15:01:07.000000 torch_contour-0.0.6/pyproject.toml
--rw-rw-r--   0 antoine   (1001) antoine   (1001)     1054 2024-05-14 12:00:11.232465 torch_contour-0.0.6/setup.cfg
--rw-rw-r--   0 antoine   (1001) antoine   (1001)       53 2023-12-06 15:01:07.000000 torch_contour-0.0.6/setup.py
-drwxrwxr-x   0 antoine   (1001) antoine   (1001)        0 2024-05-14 12:00:11.232465 torch_contour-0.0.6/torch_contour/
--rw-rw-r--   0 antoine   (1001) antoine   (1001)      146 2024-05-14 11:57:14.000000 torch_contour-0.0.6/torch_contour/__init__.py
--rw-rw-r--   0 antoine   (1001) antoine   (1001)        0 2023-12-06 15:01:07.000000 torch_contour-0.0.6/torch_contour/py.typed
--rw-rw-r--   0 antoine   (1001) antoine   (1001)     5118 2024-05-14 11:32:18.000000 torch_contour-0.0.6/torch_contour/torch_contour copy.py
--rw-rw-r--   0 antoine   (1001) antoine   (1001)     5260 2024-05-14 11:56:48.000000 torch_contour-0.0.6/torch_contour/torch_contour.py
-drwxrwxr-x   0 antoine   (1001) antoine   (1001)        0 2024-05-14 12:00:11.232465 torch_contour-0.0.6/torch_contour.egg-info/
--rw-r--r--   0 antoine   (1001) antoine   (1001)     3007 2024-05-14 12:00:11.000000 torch_contour-0.0.6/torch_contour.egg-info/PKG-INFO
--rw-rw-r--   0 antoine   (1001) antoine   (1001)      351 2024-05-14 12:00:11.000000 torch_contour-0.0.6/torch_contour.egg-info/SOURCES.txt
--rw-rw-r--   0 antoine   (1001) antoine   (1001)        1 2024-05-14 12:00:11.000000 torch_contour-0.0.6/torch_contour.egg-info/dependency_links.txt
--rw-rw-r--   0 antoine   (1001) antoine   (1001)        6 2024-05-14 12:00:11.000000 torch_contour-0.0.6/torch_contour.egg-info/requires.txt
--rw-rw-r--   0 antoine   (1001) antoine   (1001)       14 2024-05-14 12:00:11.000000 torch_contour-0.0.6/torch_contour.egg-info/top_level.txt
+drwxrwxr-x   0 antoine   (1001) antoine   (1001)        0 2024-05-17 14:34:24.194998 torch_contour-1.0.0/
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)     1068 2023-12-06 15:01:07.000000 torch_contour-1.0.0/LICENSE
+-rw-r--r--   0 antoine   (1001) antoine   (1001)     2460 2024-05-17 14:34:24.194998 torch_contour-1.0.0/PKG-INFO
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)     1563 2024-05-17 14:31:47.000000 torch_contour-1.0.0/README.md
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)      138 2023-12-06 15:01:07.000000 torch_contour-1.0.0/pyproject.toml
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)     1054 2024-05-17 14:34:24.194998 torch_contour-1.0.0/setup.cfg
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)       53 2023-12-06 15:01:07.000000 torch_contour-1.0.0/setup.py
+drwxrwxr-x   0 antoine   (1001) antoine   (1001)        0 2024-05-17 14:34:24.190998 torch_contour-1.0.0/torch_contour/
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)      146 2024-05-17 14:34:15.000000 torch_contour-1.0.0/torch_contour/__init__.py
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)        0 2023-12-06 15:01:07.000000 torch_contour-1.0.0/torch_contour/py.typed
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)     5282 2024-05-17 14:30:46.000000 torch_contour-1.0.0/torch_contour/torch_contour.py
+drwxrwxr-x   0 antoine   (1001) antoine   (1001)        0 2024-05-17 14:34:24.194998 torch_contour-1.0.0/torch_contour.egg-info/
+-rw-r--r--   0 antoine   (1001) antoine   (1001)     2460 2024-05-17 14:34:24.000000 torch_contour-1.0.0/torch_contour.egg-info/PKG-INFO
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)      315 2024-05-17 14:34:24.000000 torch_contour-1.0.0/torch_contour.egg-info/SOURCES.txt
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)        1 2024-05-17 14:34:24.000000 torch_contour-1.0.0/torch_contour.egg-info/dependency_links.txt
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)        6 2024-05-17 14:34:24.000000 torch_contour-1.0.0/torch_contour.egg-info/requires.txt
+-rw-rw-r--   0 antoine   (1001) antoine   (1001)       14 2024-05-17 14:34:24.000000 torch_contour-1.0.0/torch_contour.egg-info/top_level.txt
```

### Comparing `torch_contour-0.0.6/LICENSE` & `torch_contour-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_contour-0.0.6/PKG-INFO` & `torch_contour-1.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,84 +1,81 @@
 Metadata-Version: 2.1
 Name: torch_contour
-Version: 0.0.6
+Version: 1.0.0
 Summary: Differentiable contour to mask and contour to distance map implementation with PyTorch
 Home-page: https://github.com/antoinehabis/torch_contour
 Author: Antoine Habis
 Author-email: antoine.habis.tlcm@gmail.com
 License: MIT
-Description: # torch_contour
-        <figure>
-        <p align="center">
-          <img 
-          src="vary_nodes.jpg"
-          alt="Example of torch contour on a circle when varying the number of nodes"
-          width="500">
-          <figcaption>Example of torch contour on a circle when varying the number of nodes</figcaption>
-        </p>
-        </figure>
-        
-        This library contains 2 pytorch layers for performing the diferentiable operations of :
-        
-        1. contour to mask
-        2. contour to distance map. 
-        
-        It can therefore be used to transform a polygon into a binary mask or distance map in a completely differentiable way.
-        In particular, it can be used to transform the detection task into a segmentation task.
-        The two layers have no learnable weight, so all it does is apply a function in a derivative way.
-        
-        
-        
-        ## Input (Float):
-        
-        A polygon of size $2 \times n$ with \
-        with $n$ the number of nodes
-        
-        
-        ## Output (Float):
-        
-        A mask or distance map of size $1 \times H \times W$.\
-        with $H$ and $W$ respectively the Heigh and Width of the distance map or mask.
-        
-        ## Important: 
-        
-        The polygon must have values between 0 and 1. It is therefore important to apply a sigmoid function before the layer.*.
-        
-        The predicted polygon must be ordered in counter-clockwise.
-        
-        
-        
-        ## Example:
-        
-         ```
-        from torch_contour.torch_contour import Contour_to_distance_map, Contour_to_mask
-        import torch
-        import matplotlib.pyplot as plt
-        
-        x = torch.tensor([[0.1,0.1],
-                          [0.1,0.9],
-                          [0.9,0.9],
-                          [0.9,0.1]])[None]
-        
-        Dmap = Contour_to_distance_map(200)
-        Mask = Contour_to_mask(200)
-        
-        plt.imshow(Dmap(x).cpu().detach().numpy()[0,0])
-        plt.show()
-        plt.imshow(Mask(x).cpu().detach().numpy()[0,0])
-        plt.show()
-        ```
-        
-        
 Keywords: differentiable contour processing,pytorch,machine learning
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: torch
+
+# torch_contour
+<figure>
+<p align="center">
+  <img 
+  src="vary_nodes.jpg"
+  alt="Example of torch contour on a circle when varying the number of nodes"
+  width="500">
+  <figcaption>Example of torch contour on a circle when varying the number of nodes</figcaption>
+</p>
+</figure>
+
+This library contains 2 pytorch layers for performing the diferentiable operations of :
+
+1. contour to mask
+2. contour to distance map. 
+
+It can therefore be used to transform a polygon into a binary mask or distance map in a completely differentiable way.
+In particular, it can be used to transform the detection task into a segmentation task.
+The two layers have no learnable weight, so all it does is apply a function in a derivative way.
+
+
+
+## Input (Float):
+
+A polygon of size $2 \times n$ with \
+with $n$ the number of nodes
+
+
+## Output (Float):
+
+A mask or distance map of size $1 \times H \times W$.\
+with $H$ and $W$ respectively the Heigh and Width of the distance map or mask.
+
+## Important: 
+
+The polygon must have values between 0 and 1. It is therefore important to apply a sigmoid function before the layer.*.
+
+## Example:
+
+ ```
+from torch_contour.torch_contour import Contour_to_distance_map, Contour_to_mask
+import torch
+import matplotlib.pyplot as plt
+
+x = torch.tensor([[0.1,0.1],
+                  [0.1,0.9],
+                  [0.9,0.9],
+                  [0.9,0.1]])[None]
+
+Dmap = Contour_to_distance_map(200)
+Mask = Contour_to_mask(200)
+
+plt.imshow(Dmap(x).cpu().detach().numpy()[0,0])
+plt.show()
+plt.imshow(Mask(x).cpu().detach().numpy()[0,0])
+plt.show()
+```
+
```

### Comparing `torch_contour-0.0.6/README.md` & `torch_contour-1.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -31,18 +31,14 @@
 A mask or distance map of size $1 \times H \times W$.\
 with $H$ and $W$ respectively the Heigh and Width of the distance map or mask.
 
 ## Important: 
 
 The polygon must have values between 0 and 1. It is therefore important to apply a sigmoid function before the layer.*.
 
-The predicted polygon must be ordered in counter-clockwise.
-
-
-
 ## Example:
 
  ```
 from torch_contour.torch_contour import Contour_to_distance_map, Contour_to_mask
 import torch
 import matplotlib.pyplot as plt
```

### Comparing `torch_contour-0.0.6/setup.cfg` & `torch_contour-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `torch_contour-0.0.6/torch_contour/torch_contour copy.py` & `torch_contour-1.0.0/torch_contour/torch_contour.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,170 +1,170 @@
 import torch
 import torch.nn as nn
 
 
-
-
 class Contour_to_mask(nn.Module):
-
     """This layer transform a polygon into a mask
-    
+
     ...
-    
+
     Attributes
     ----------
     size: int
-        the size of the output image 
+        the size of the output image
     k: float
         the control parameter to approximate the sign function
     eps: float
         a parameter to smooth the function and avoid division by 0
-    
+
     Methods
     -------
     forward(contour)
         forward function that turns the contour into a mask
     """
 
     def __init__(self, size, k=1e5, eps=1e-5):
-
         """
         Parameters
         ----------
         size: int
-            the size of the output image 
+            the size of the output image
         k: float
             the control parameter to approximate the sign function
         eps: float
             a parameter to smooth the function and avoid division by 0
 
         """
         super().__init__()
         self.k = k
         self.eps = eps
         self.size = size
-        self.mesh = (
-            torch.unsqueeze(
-                torch.stack(
-                    torch.meshgrid(torch.arange(self.size), torch.arange(self.size)),
-                    dim=-1,
-                ).reshape(-1, 2),
-                dim=1,
-            )
-            / self.size
-        )
 
-    def forward(self, contour):
 
+    def forward(self, contour):
         """Return the distance map of the given size given the contour.
 
         Raises
         ------
         ValueError
             If the values of the contour or not between 0 and 1.
         """
 
+        b = contour.shape[0]
+        mesh = (
+            torch.unsqueeze(
+                torch.stack(
+                    torch.meshgrid(torch.arange(self.size), torch.arange(self.size)),
+                    dim=-1,
+                ).reshape(-1, 2),
+                dim=1,
+            )
+            / self.size
+        )
+        mesh = mesh.unsqueeze(0).repeat(b,1,1,1)
+
         if (contour < 0).any() or (contour > 1).any():
             raise ValueError("Tensor values should be in the range [0, 1]")
 
-        contours = torch.unsqueeze(contour, dim=0)
-        diff = -self.mesh + contours
-        roll_diff = torch.roll(diff, -1, dims=1)
-        sign = diff * torch.roll(roll_diff, 1, dims=2)
-        sign = sign[:, :, 1] - sign[:, :, 0]
+        contour = torch.unsqueeze(contour, dim=1)
+        diff = -mesh + contour
+        roll_diff = torch.roll(diff, -1, dims=2)
+        sign = diff * torch.roll(roll_diff, 1, dims=3)
+        sign = sign[:, :, :, 1] - sign[:, :, :, 0]
         sign = torch.tanh(self.k * sign)
-        norm_diff = torch.linalg.vector_norm(diff, dim=2)
-        norm_roll = torch.linalg.vector_norm(roll_diff, dim=2)
-        scalar_product = torch.sum(diff * roll_diff, dim=2)
+        norm_diff = torch.linalg.vector_norm(diff, dim=3)
+        norm_roll = torch.linalg.vector_norm(roll_diff, dim=3)
+        scalar_product = torch.sum(diff * roll_diff, dim=3)
+
         clip = torch.clamp(scalar_product / (norm_diff * norm_roll), -1 + self.eps, 1 - self.eps)
         angles = torch.acos(clip)
         torch.pi = torch.acos(torch.zeros(1)).item() * 2
-        sum_angles = torch.clamp(torch.sum(sign * angles, dim=1) / (2 * torch.pi), 0, 1)
-        out0 = sum_angles.reshape(1, self.size, self.size)
+        sum_angles = torch.clamp(torch.abs(torch.sum(sign * angles, dim=2) / (2 * torch.pi)), 0, 1)
+        out0 = sum_angles.reshape(b, self.size, self.size)
         mask = torch.unsqueeze(out0, dim=0)
-
+        
         return mask
-    
-
-
 
 
 class Contour_to_distance_map(nn.Module):
     """This layer transform a polygon into a distance map
-    
+
     ...
-    
+
     Attributes
     ----------
     size: int
-        the size of the output image 
+        the size of the output image
     k: float
         the control parameter to approximate the sign function
     eps: float
         a parameter to smooth the function and avoid division by 0
-    
+
     Methods
     -------
     forward(contour)
         forward function that turns the contour into a distance map
     """
 
     def __init__(self, size, k=1e5, eps=1e-5):
-
-
         """
         Parameters
         ----------
         size: int
-            the size of the output image 
+            the size of the output image
         k: float
             the control parameter to approximate the sign function
         eps: float
             a parameter to smooth the function and avoid division by 0
 
         """
         super().__init__()
         self.k = k
         self.eps = eps
         self.size = size
-        self.mesh = (
-            torch.unsqueeze(
-                torch.stack(
-                    torch.meshgrid(torch.arange(self.size), torch.arange(self.size)),
-                    dim=-1,
-                ).reshape(-1, 2),
-                dim=1,
-            )
-            / self.size
-        )
 
-    def forward(self, contour):
 
+    def forward(self, contour):
         """Return the distance map of the given size given the contour.
 
         Raises
         ------
         ValueError
             If the values of the contour or not between 0 and 1.
         """
+        b = contour.shape[0]
+        mesh = (
+            torch.unsqueeze(
+                torch.stack(
+                    torch.meshgrid(torch.arange(self.size), torch.arange(self.size)),
+                    dim=-1,
+                ).reshape(-1, 2),
+                dim=1,
+            )
+            / self.size
+        )
+        mesh = mesh.unsqueeze(0).repeat(b,1,1,1)
 
         if (contour < 0).any() or (contour > 1).any():
             raise ValueError("Tensor values should be in the range [0, 1]")
-                
-        contour = torch.unsqueeze(contour, dim=0)
-        diff = -self.mesh + contour
-        min_diff = torch.min(torch.norm(diff, dim=-1), dim=1)[0]
-        min_diff = min_diff.reshape((self.size, self.size))
-        roll_diff = torch.roll(diff, -1, dims=1)
-        sign = diff * torch.roll(roll_diff, 1, dims=2)
-        sign = sign[:, :, 1] - sign[:, :, 0]
+        
+
+
+        contour = torch.unsqueeze(contour, dim=1)
+        diff = - mesh + contour
+        min_diff = torch.min(torch.norm(diff, dim=-1), dim=2)[0]
+        print(min_diff.shape)
+        min_diff = min_diff.reshape((b,self.size, self.size))
+        roll_diff = torch.roll(diff, -1, dims=2)
+        sign = diff * torch.roll(roll_diff, 1, dims=3)
+        sign = sign[:, :, :, 1] - sign[:, :, :, 0]
         sign = torch.tanh(self.k * sign)
-        norm_diff = torch.clip(torch.norm(diff, dim=2), self.eps, None)
-        norm_roll = torch.clip(torch.norm(roll_diff, dim=2), self.eps, None)
-        scalar_product = torch.sum(diff * roll_diff, dim=2)
+        norm_diff = torch.clip(torch.norm(diff, dim=3), self.eps, None)
+        norm_roll = torch.clip(torch.norm(roll_diff, dim=3), self.eps, None)
+        scalar_product = torch.sum(diff * roll_diff, dim=3)
         clip = torch.clip(scalar_product / (norm_diff * norm_roll), -1 + self.eps, 1 - self.eps)
         angles = torch.arccos(clip)
         torch.pi = torch.acos(torch.zeros(1)).item() * 2
-        sum_angles = torch.sum(sign * angles, dim=1) / (2 * torch.pi)
-        resize = sum_angles.reshape(1, self.size, self.size)
+        sum_angles = torch.abs(torch.sum(sign * angles, dim=2) / (2 * torch.pi))
+        resize = sum_angles.reshape(b, self.size, self.size)
         dmap = torch.unsqueeze((resize * min_diff) / torch.max(resize * min_diff), 0)
         return dmap
```

### Comparing `torch_contour-0.0.6/torch_contour.egg-info/PKG-INFO` & `torch_contour-1.0.0/torch_contour.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,84 +1,81 @@
 Metadata-Version: 2.1
-Name: torch-contour
-Version: 0.0.6
+Name: torch_contour
+Version: 1.0.0
 Summary: Differentiable contour to mask and contour to distance map implementation with PyTorch
 Home-page: https://github.com/antoinehabis/torch_contour
 Author: Antoine Habis
 Author-email: antoine.habis.tlcm@gmail.com
 License: MIT
-Description: # torch_contour
-        <figure>
-        <p align="center">
-          <img 
-          src="vary_nodes.jpg"
-          alt="Example of torch contour on a circle when varying the number of nodes"
-          width="500">
-          <figcaption>Example of torch contour on a circle when varying the number of nodes</figcaption>
-        </p>
-        </figure>
-        
-        This library contains 2 pytorch layers for performing the diferentiable operations of :
-        
-        1. contour to mask
-        2. contour to distance map. 
-        
-        It can therefore be used to transform a polygon into a binary mask or distance map in a completely differentiable way.
-        In particular, it can be used to transform the detection task into a segmentation task.
-        The two layers have no learnable weight, so all it does is apply a function in a derivative way.
-        
-        
-        
-        ## Input (Float):
-        
-        A polygon of size $2 \times n$ with \
-        with $n$ the number of nodes
-        
-        
-        ## Output (Float):
-        
-        A mask or distance map of size $1 \times H \times W$.\
-        with $H$ and $W$ respectively the Heigh and Width of the distance map or mask.
-        
-        ## Important: 
-        
-        The polygon must have values between 0 and 1. It is therefore important to apply a sigmoid function before the layer.*.
-        
-        The predicted polygon must be ordered in counter-clockwise.
-        
-        
-        
-        ## Example:
-        
-         ```
-        from torch_contour.torch_contour import Contour_to_distance_map, Contour_to_mask
-        import torch
-        import matplotlib.pyplot as plt
-        
-        x = torch.tensor([[0.1,0.1],
-                          [0.1,0.9],
-                          [0.9,0.9],
-                          [0.9,0.1]])[None]
-        
-        Dmap = Contour_to_distance_map(200)
-        Mask = Contour_to_mask(200)
-        
-        plt.imshow(Dmap(x).cpu().detach().numpy()[0,0])
-        plt.show()
-        plt.imshow(Mask(x).cpu().detach().numpy()[0,0])
-        plt.show()
-        ```
-        
-        
 Keywords: differentiable contour processing,pytorch,machine learning
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: torch
+
+# torch_contour
+<figure>
+<p align="center">
+  <img 
+  src="vary_nodes.jpg"
+  alt="Example of torch contour on a circle when varying the number of nodes"
+  width="500">
+  <figcaption>Example of torch contour on a circle when varying the number of nodes</figcaption>
+</p>
+</figure>
+
+This library contains 2 pytorch layers for performing the diferentiable operations of :
+
+1. contour to mask
+2. contour to distance map. 
+
+It can therefore be used to transform a polygon into a binary mask or distance map in a completely differentiable way.
+In particular, it can be used to transform the detection task into a segmentation task.
+The two layers have no learnable weight, so all it does is apply a function in a derivative way.
+
+
+
+## Input (Float):
+
+A polygon of size $2 \times n$ with \
+with $n$ the number of nodes
+
+
+## Output (Float):
+
+A mask or distance map of size $1 \times H \times W$.\
+with $H$ and $W$ respectively the Heigh and Width of the distance map or mask.
+
+## Important: 
+
+The polygon must have values between 0 and 1. It is therefore important to apply a sigmoid function before the layer.*.
+
+## Example:
+
+ ```
+from torch_contour.torch_contour import Contour_to_distance_map, Contour_to_mask
+import torch
+import matplotlib.pyplot as plt
+
+x = torch.tensor([[0.1,0.1],
+                  [0.1,0.9],
+                  [0.9,0.9],
+                  [0.9,0.1]])[None]
+
+Dmap = Contour_to_distance_map(200)
+Mask = Contour_to_mask(200)
+
+plt.imshow(Dmap(x).cpu().detach().numpy()[0,0])
+plt.show()
+plt.imshow(Mask(x).cpu().detach().numpy()[0,0])
+plt.show()
+```
+
```

