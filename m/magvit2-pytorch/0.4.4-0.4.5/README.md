# Comparing `tmp/magvit2_pytorch-0.4.4.tar.gz` & `tmp/magvit2_pytorch-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magvit2_pytorch-0.4.4.tar", last modified: Wed May  8 14:20:56 2024, max compression
+gzip compressed data, was "magvit2_pytorch-0.4.5.tar", last modified: Thu May 16 23:59:22 2024, max compression
```

## Comparing `magvit2_pytorch-0.4.4.tar` & `magvit2_pytorch-0.4.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:56.124939 magvit2_pytorch-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-08 14:20:52.000000 magvit2_pytorch-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-08 14:20:56.124939 magvit2_pytorch-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-05-08 14:20:52.000000 magvit2_pytorch-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:56.120939 magvit2_pytorch-0.4.4/magvit2_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-08 14:20:52.000000 magvit2_pytorch-0.4.4/magvit2_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-05-08 14:20:52.000000 magvit2_pytorch-0.4.4/magvit2_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-08 14:20:52.000000 magvit2_pytorch-0.4.4/magvit2_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    56521 2024-05-08 14:20:52.000000 magvit2_pytorch-0.4.4/magvit2_pytorch/magvit2_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-08 14:20:52.000000 magvit2_pytorch-0.4.4/magvit2_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16817 2024-05-08 14:20:52.000000 magvit2_pytorch-0.4.4/magvit2_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 14:20:52.000000 magvit2_pytorch-0.4.4/magvit2_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:56.120939 magvit2_pytorch-0.4.4/magvit2_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-08 14:20:56.000000 magvit2_pytorch-0.4.4/magvit2_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-08 14:20:56.000000 magvit2_pytorch-0.4.4/magvit2_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:20:56.000000 magvit2_pytorch-0.4.4/magvit2_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-08 14:20:56.000000 magvit2_pytorch-0.4.4/magvit2_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 14:20:56.000000 magvit2_pytorch-0.4.4/magvit2_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 14:20:56.124939 magvit2_pytorch-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-08 14:20:52.000000 magvit2_pytorch-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 23:59:22.921148 magvit2_pytorch-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-16 23:59:18.000000 magvit2_pytorch-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-16 23:59:22.921148 magvit2_pytorch-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-05-16 23:59:18.000000 magvit2_pytorch-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 23:59:22.917148 magvit2_pytorch-0.4.5/magvit2_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-16 23:59:18.000000 magvit2_pytorch-0.4.5/magvit2_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-05-16 23:59:18.000000 magvit2_pytorch-0.4.5/magvit2_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-16 23:59:18.000000 magvit2_pytorch-0.4.5/magvit2_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56521 2024-05-16 23:59:18.000000 magvit2_pytorch-0.4.5/magvit2_pytorch/magvit2_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-16 23:59:18.000000 magvit2_pytorch-0.4.5/magvit2_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16943 2024-05-16 23:59:18.000000 magvit2_pytorch-0.4.5/magvit2_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 23:59:18.000000 magvit2_pytorch-0.4.5/magvit2_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 23:59:22.921148 magvit2_pytorch-0.4.5/magvit2_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-16 23:59:22.000000 magvit2_pytorch-0.4.5/magvit2_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-16 23:59:22.000000 magvit2_pytorch-0.4.5/magvit2_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 23:59:22.000000 magvit2_pytorch-0.4.5/magvit2_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-16 23:59:22.000000 magvit2_pytorch-0.4.5/magvit2_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 23:59:22.000000 magvit2_pytorch-0.4.5/magvit2_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 23:59:22.921148 magvit2_pytorch-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-16 23:59:18.000000 magvit2_pytorch-0.4.5/setup.py
```

### Comparing `magvit2_pytorch-0.4.4/LICENSE` & `magvit2_pytorch-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `magvit2_pytorch-0.4.4/PKG-INFO` & `magvit2_pytorch-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magvit2-pytorch
-Version: 0.4.4
+Version: 0.4.5
 Summary: MagViT2 - Pytorch
 Home-page: https://github.com/lucidrains/magvit2-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformer,attention mechanisms,generative video model
 Classifier: Development Status :: 4 - Beta
```

### Comparing `magvit2_pytorch-0.4.4/README.md` & `magvit2_pytorch-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `magvit2_pytorch-0.4.4/magvit2_pytorch/attend.py` & `magvit2_pytorch-0.4.5/magvit2_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `magvit2_pytorch-0.4.4/magvit2_pytorch/data.py` & `magvit2_pytorch-0.4.5/magvit2_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `magvit2_pytorch-0.4.4/magvit2_pytorch/magvit2_pytorch.py` & `magvit2_pytorch-0.4.5/magvit2_pytorch/magvit2_pytorch.py`

 * *Files identical despite different names*

### Comparing `magvit2_pytorch-0.4.4/magvit2_pytorch/optimizer.py` & `magvit2_pytorch-0.4.5/magvit2_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `magvit2_pytorch-0.4.4/magvit2_pytorch/trainer.py` & `magvit2_pytorch-0.4.5/magvit2_pytorch/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,20 +184,24 @@
 
         # prepare for maybe distributed
 
         (
             self.model,
             self.dataloader,
             self.optimizer,
-            self.discr_optimizer
+            self.discr_optimizer,
+            self.scheduler,
+            self.discr_scheduler,
         ) = self.accelerator.prepare(
             self.model,
             self.dataloader,
             self.optimizer,
-            self.discr_optimizer
+            self.discr_optimizer,
+            self.scheduler,
+            self.discr_scheduler,
         )
 
         # only use adversarial training after a certain number of steps
 
         self.discr_start_after_step = discr_start_after_step
 
         # multiscale discr losses
```

### Comparing `magvit2_pytorch-0.4.4/magvit2_pytorch.egg-info/PKG-INFO` & `magvit2_pytorch-0.4.5/magvit2_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magvit2-pytorch
-Version: 0.4.4
+Version: 0.4.5
 Summary: MagViT2 - Pytorch
 Home-page: https://github.com/lucidrains/magvit2-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformer,attention mechanisms,generative video model
 Classifier: Development Status :: 4 - Beta
```

### Comparing `magvit2_pytorch-0.4.4/setup.py` & `magvit2_pytorch-0.4.5/setup.py`

 * *Files identical despite different names*

