# Comparing `tmp/meshgpt_pytorch-1.2.7.tar.gz` & `tmp/meshgpt_pytorch-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshgpt_pytorch-1.2.7.tar", last modified: Thu May 16 12:38:23 2024, max compression
+gzip compressed data, was "meshgpt_pytorch-1.2.8.tar", last modified: Fri May 17 19:34:38 2024, max compression
```

## Comparing `meshgpt_pytorch-1.2.7.tar` & `meshgpt_pytorch-1.2.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:38:23.008121 meshgpt_pytorch-1.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-16 12:38:03.000000 meshgpt_pytorch-1.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-16 12:38:23.008121 meshgpt_pytorch-1.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-05-16 12:38:03.000000 meshgpt_pytorch-1.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:38:23.008121 meshgpt_pytorch-1.2.7/meshgpt_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-16 12:38:03.000000 meshgpt_pytorch-1.2.7/meshgpt_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-05-16 12:38:03.000000 meshgpt_pytorch-1.2.7/meshgpt_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    50646 2024-05-16 12:38:03.000000 meshgpt_pytorch-1.2.7/meshgpt_pytorch/meshgpt_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-05-16 12:38:03.000000 meshgpt_pytorch-1.2.7/meshgpt_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 12:38:03.000000 meshgpt_pytorch-1.2.7/meshgpt_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:38:23.008121 meshgpt_pytorch-1.2.7/meshgpt_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-16 12:38:22.000000 meshgpt_pytorch-1.2.7/meshgpt_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-16 12:38:23.000000 meshgpt_pytorch-1.2.7/meshgpt_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 12:38:22.000000 meshgpt_pytorch-1.2.7/meshgpt_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-16 12:38:23.000000 meshgpt_pytorch-1.2.7/meshgpt_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 12:38:23.000000 meshgpt_pytorch-1.2.7/meshgpt_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 12:38:23.008121 meshgpt_pytorch-1.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-16 12:38:03.000000 meshgpt_pytorch-1.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:34:38.583101 meshgpt_pytorch-1.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-17 19:34:34.000000 meshgpt_pytorch-1.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-17 19:34:38.583101 meshgpt_pytorch-1.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-05-17 19:34:34.000000 meshgpt_pytorch-1.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:34:38.583101 meshgpt_pytorch-1.2.8/meshgpt_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-17 19:34:34.000000 meshgpt_pytorch-1.2.8/meshgpt_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-05-17 19:34:34.000000 meshgpt_pytorch-1.2.8/meshgpt_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50687 2024-05-17 19:34:34.000000 meshgpt_pytorch-1.2.8/meshgpt_pytorch/meshgpt_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-05-17 19:34:34.000000 meshgpt_pytorch-1.2.8/meshgpt_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-17 19:34:34.000000 meshgpt_pytorch-1.2.8/meshgpt_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:34:38.583101 meshgpt_pytorch-1.2.8/meshgpt_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-17 19:34:38.000000 meshgpt_pytorch-1.2.8/meshgpt_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-17 19:34:38.000000 meshgpt_pytorch-1.2.8/meshgpt_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 19:34:38.000000 meshgpt_pytorch-1.2.8/meshgpt_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-17 19:34:38.000000 meshgpt_pytorch-1.2.8/meshgpt_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-17 19:34:38.000000 meshgpt_pytorch-1.2.8/meshgpt_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 19:34:38.583101 meshgpt_pytorch-1.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-17 19:34:34.000000 meshgpt_pytorch-1.2.8/setup.py
```

### Comparing `meshgpt_pytorch-1.2.7/LICENSE` & `meshgpt_pytorch-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `meshgpt_pytorch-1.2.7/PKG-INFO` & `meshgpt_pytorch-1.2.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshgpt-pytorch
-Version: 1.2.7
+Version: 1.2.8
 Summary: MeshGPT Pytorch
 Home-page: https://github.com/lucidrains/meshgpt-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanisms,transformers,mesh generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `meshgpt_pytorch-1.2.7/README.md` & `meshgpt_pytorch-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `meshgpt_pytorch-1.2.7/meshgpt_pytorch/data.py` & `meshgpt_pytorch-1.2.8/meshgpt_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `meshgpt_pytorch-1.2.7/meshgpt_pytorch/meshgpt_pytorch.py` & `meshgpt_pytorch-1.2.8/meshgpt_pytorch/meshgpt_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,16 +156,18 @@
 ):
     shifted_face_coords = torch.cat((face_coords[:, :, -1:], face_coords[:, :, :-1]), dim = 2)
 
     angles  = derive_angle(face_coords, shifted_face_coords)
 
     edge1, edge2, *_ = (face_coords - shifted_face_coords).unbind(dim = 2)
 
-    normals = l2norm(torch.cross(edge1, edge2, dim = -1))
-    area = normals.norm(dim = -1, keepdim = True) * 0.5
+    cross_product = torch.cross(edge1, edge2, dim = -1)
+
+    normals = l2norm(cross_product)
+    area = cross_product.norm(dim = -1, keepdim = True) * 0.5
 
     return dict(
         angles = angles,
         area = area,
         normals = normals
     )
```

### Comparing `meshgpt_pytorch-1.2.7/meshgpt_pytorch/trainer.py` & `meshgpt_pytorch-1.2.8/meshgpt_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `meshgpt_pytorch-1.2.7/meshgpt_pytorch.egg-info/PKG-INFO` & `meshgpt_pytorch-1.2.8/meshgpt_pytorch.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshgpt-pytorch
-Version: 1.2.7
+Version: 1.2.8
 Summary: MeshGPT Pytorch
 Home-page: https://github.com/lucidrains/meshgpt-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanisms,transformers,mesh generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `meshgpt_pytorch-1.2.7/setup.py` & `meshgpt_pytorch-1.2.8/setup.py`

 * *Files identical despite different names*

