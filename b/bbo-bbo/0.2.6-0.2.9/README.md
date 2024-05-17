# Comparing `tmp/bbo_bbo-0.2.6.tar.gz` & `tmp/bbo_bbo-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbo_bbo-0.2.6.tar", last modified: Tue Dec 12 10:54:25 2023, max compression
+gzip compressed data, was "bbo_bbo-0.2.9.tar", last modified: Thu Apr 18 13:32:22 2024, max compression
```

## Comparing `bbo_bbo-0.2.6.tar` & `bbo_bbo-0.2.9.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2023-12-12 10:54:25.543892 bbo_bbo-0.2.6/
--rw-rw-r--   0 voit     (86501) voit     (86501)    26526 2023-11-14 18:07:18.000000 bbo_bbo-0.2.6/LICENSE
--rw-rw-r--   0 voit     (86501) voit     (86501)      426 2023-12-12 10:54:25.543892 bbo_bbo-0.2.6/PKG-INFO
--rw-rw-r--   0 voit     (86501) voit     (86501)        0 2023-11-14 18:07:18.000000 bbo_bbo-0.2.6/README.md
-drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2023-12-12 10:54:25.539892 bbo_bbo-0.2.6/bbo/
--rw-rw-r--   0 voit     (86501) voit     (86501)       48 2023-11-14 18:07:18.000000 bbo_bbo-0.2.6/bbo/__init__.py
--rw-rw-r--   0 voit     (86501) voit     (86501)       43 2023-11-14 18:07:18.000000 bbo_bbo-0.2.6/bbo/exceptions.py
--rw-rw-r--   0 voit     (86501) voit     (86501)    23782 2023-12-12 10:53:27.000000 bbo_bbo-0.2.6/bbo/label_lib.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     1794 2023-11-14 18:07:18.000000 bbo_bbo-0.2.6/bbo/path_management.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     3869 2023-11-14 18:07:18.000000 bbo_bbo-0.2.6/bbo/yaml.py
-drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2023-12-12 10:54:25.539892 bbo_bbo-0.2.6/bbo_bbo.egg-info/
--rw-rw-r--   0 voit     (86501) voit     (86501)      426 2023-12-12 10:54:25.000000 bbo_bbo-0.2.6/bbo_bbo.egg-info/PKG-INFO
--rw-rw-r--   0 voit     (86501) voit     (86501)      266 2023-12-12 10:54:25.000000 bbo_bbo-0.2.6/bbo_bbo.egg-info/SOURCES.txt
--rw-rw-r--   0 voit     (86501) voit     (86501)        1 2023-12-12 10:54:25.000000 bbo_bbo-0.2.6/bbo_bbo.egg-info/dependency_links.txt
--rw-rw-r--   0 voit     (86501) voit     (86501)        7 2023-12-12 10:54:25.000000 bbo_bbo-0.2.6/bbo_bbo.egg-info/requires.txt
--rw-rw-r--   0 voit     (86501) voit     (86501)        4 2023-12-12 10:54:25.000000 bbo_bbo-0.2.6/bbo_bbo.egg-info/top_level.txt
--rw-rw-r--   0 voit     (86501) voit     (86501)       38 2023-12-12 10:54:25.543892 bbo_bbo-0.2.6/setup.cfg
--rw-rw-r--   0 voit     (86501) voit     (86501)      827 2023-12-12 10:54:05.000000 bbo_bbo-0.2.6/setup.py
+drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-04-18 13:32:22.797442 bbo_bbo-0.2.9/
+-rw-rw-r--   0 voit     (86501) voit     (86501)    26526 2023-11-14 18:07:18.000000 bbo_bbo-0.2.9/LICENSE
+-rw-rw-r--   0 voit     (86501) voit     (86501)      426 2024-04-18 13:32:22.797442 bbo_bbo-0.2.9/PKG-INFO
+-rw-rw-r--   0 voit     (86501) voit     (86501)        0 2023-11-14 18:07:18.000000 bbo_bbo-0.2.9/README.md
+drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-04-18 13:32:22.797442 bbo_bbo-0.2.9/bbo/
+-rw-rw-r--   0 voit     (86501) voit     (86501)       48 2023-11-14 18:07:18.000000 bbo_bbo-0.2.9/bbo/__init__.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)       43 2023-11-14 18:07:18.000000 bbo_bbo-0.2.9/bbo/exceptions.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)    19512 2024-04-18 13:14:02.000000 bbo_bbo-0.2.9/bbo/geometry.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)    24762 2024-04-18 13:14:02.000000 bbo_bbo-0.2.9/bbo/label_lib.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     1794 2023-11-14 18:07:18.000000 bbo_bbo-0.2.9/bbo/path_management.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     7134 2024-04-18 13:14:02.000000 bbo_bbo-0.2.9/bbo/test_geometry.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     3869 2023-11-14 18:07:18.000000 bbo_bbo-0.2.9/bbo/yaml.py
+drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-04-18 13:32:22.797442 bbo_bbo-0.2.9/bbo_bbo.egg-info/
+-rw-rw-r--   0 voit     (86501) voit     (86501)      426 2024-04-18 13:32:22.000000 bbo_bbo-0.2.9/bbo_bbo.egg-info/PKG-INFO
+-rw-rw-r--   0 voit     (86501) voit     (86501)      303 2024-04-18 13:32:22.000000 bbo_bbo-0.2.9/bbo_bbo.egg-info/SOURCES.txt
+-rw-rw-r--   0 voit     (86501) voit     (86501)        1 2024-04-18 13:32:22.000000 bbo_bbo-0.2.9/bbo_bbo.egg-info/dependency_links.txt
+-rw-rw-r--   0 voit     (86501) voit     (86501)       19 2024-04-18 13:32:22.000000 bbo_bbo-0.2.9/bbo_bbo.egg-info/requires.txt
+-rw-rw-r--   0 voit     (86501) voit     (86501)        4 2024-04-18 13:32:22.000000 bbo_bbo-0.2.9/bbo_bbo.egg-info/top_level.txt
+-rw-rw-r--   0 voit     (86501) voit     (86501)       38 2024-04-18 13:32:22.797442 bbo_bbo-0.2.9/setup.cfg
+-rw-rw-r--   0 voit     (86501) voit     (86501)      843 2024-04-18 13:31:59.000000 bbo_bbo-0.2.9/setup.py
```

### Comparing `bbo_bbo-0.2.6/LICENSE` & `bbo_bbo-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bbo_bbo-0.2.6/bbo/label_lib.py` & `bbo_bbo-0.2.9/bbo/label_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,16 +151,19 @@
         # and should not be used in any circumstance except for emergencies with the yml files.
         np.savez(file_path.with_suffix(".npz").as_posix(), labels)
 
     with open(file_path.with_suffix(".yml").as_posix(), 'w') as f:
         write_label_yaml(f, labels)
 
 
-def get_labels(labels):
-    return [lm for lm in labels["labels"] if len(labels["labels"][lm].keys()) > 0]
+def get_labels(labels, allow_empty=False):
+    if allow_empty:
+        return list(labels["labels"].keys())
+    else:
+        return [lm for lm in labels["labels"] if len(labels["labels"][lm].keys()) > 0]
 
 
 def get_labeled_frame_idxs(labels):
     frames = set()
     for ln in labels["labels"]:
         frames.update(set(labels["labels"][ln].keys()))
 
@@ -261,28 +264,25 @@
                     labels["point_times"][ln][fr_idx][i_cam] = 0
 
 
 def combine_cams(labels_list: list, target_file=None, yml_only=False):
     # Normalize path of target_file
     if isinstance(target_file, str):
         target_file = Path(target_file).expanduser().resolve()
-
     # Load data from files
     for i_l, label in enumerate(labels_list):
         if isinstance(label, str):
             if label == "None":
                 labels_list[i_l] = None
                 continue
             labels_list[i_l] = Path(label)
         if isinstance(label, Path):
             labels_list[i_l] = labels_list[i_l].expanduser().resolve()
             labels_list[i_l] = load(labels_list[i_l].as_posix())
 
-    make_global_labeler_list(labels_list)
-
     target_labels = get_empty_labels()
     target_labels['labeler_list'] = make_global_labeler_list(labels_list)
 
     data_shape = (len(labels_list), 2)
 
     for cam_idx, labels in enumerate(labels_list):
         if labels is None:
@@ -300,14 +300,38 @@
     sort_dictionaries(target_labels)
 
     if target_file is not None:
         save(target_file, target_labels, yml_only=yml_only)
     return target_labels
 
 
+def reorder_cams(labels, new_order: tuple, target_file=None, yml_only=False, reorder_times=True):
+    # Normalize path of target_file
+    if isinstance(target_file, str):
+        target_file = Path(target_file).expanduser().resolve()
+
+    # Load data from files
+    if isinstance(labels, str):
+        labels = Path(labels)
+    if isinstance(labels, Path):
+        labels = labels.expanduser().resolve()
+        labels = load(labels.as_posix())
+
+    for ln in labels["labels"]:
+        for fr_idx in labels["labels"][ln]:
+            labels["labels"][ln][fr_idx] = labels["labels"][ln][fr_idx][new_order,]
+            labels["labeler"][ln][fr_idx] = labels["labeler"][ln][fr_idx][new_order,]
+            if reorder_times:
+                labels["point_times"][ln][fr_idx] = labels["point_times"][ln][fr_idx][new_order,]
+
+    if target_file is not None:
+        save(target_file, labels, yml_only=yml_only)
+    return labels
+
+
 def initialize_target(labels, target_labels, data_shape):
     # Walk through frames
     for ln in labels["labels"]:
         # Initialize label key
         initialize_label_name(target_labels, ln)
         for fr_idx in labels["labels"][ln]:
             # Initialize frame index
```

### Comparing `bbo_bbo-0.2.6/bbo/path_management.py` & `bbo_bbo-0.2.9/bbo/path_management.py`

 * *Files identical despite different names*

### Comparing `bbo_bbo-0.2.6/bbo/yaml.py` & `bbo_bbo-0.2.9/bbo/yaml.py`

 * *Files identical despite different names*

### Comparing `bbo_bbo-0.2.6/setup.py` & `bbo_bbo-0.2.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="bbo_bbo",
-    version="0.2.6",
+    version="0.2.9",
     description="Base tools for MPINB BBO group",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/bbo-lab/bbo",
     author="BBO-lab @ caesar",
     author_email="kay-michael.voit@caesar.de",
     license="BSD",
     classifiers=[
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     packages=['bbo'],
     include_package_data=True,
-    install_requires=["pyyaml"],
+    install_requires=["pyyaml","numpy","scipy"],
 )
```

