# Comparing `tmp/lionz-0.6.tar.gz` & `tmp/lionz-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lionz-0.6.tar", last modified: Fri Mar 15 19:10:55 2024, max compression
+gzip compressed data, was "lionz-0.7.tar", last modified: Fri May 17 08:47:49 2024, max compression
```

## Comparing `lionz-0.6.tar` & `lionz-0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:10:55.148354 lionz-0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-03-15 19:10:55.148354 lionz-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-03-15 19:10:49.000000 lionz-0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:10:55.148354 lionz-0.6/lionz/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-15 19:10:49.000000 lionz-0.6/lionz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-15 19:10:49.000000 lionz-0.6/lionz/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-03-15 19:10:49.000000 lionz-0.6/lionz/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-03-15 19:10:49.000000 lionz-0.6/lionz/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-03-15 19:10:49.000000 lionz-0.6/lionz/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     9126 2024-03-15 19:10:49.000000 lionz-0.6/lionz/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    26289 2024-03-15 19:10:49.000000 lionz-0.6/lionz/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-03-15 19:10:49.000000 lionz-0.6/lionz/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16353 2024-03-15 19:10:49.000000 lionz-0.6/lionz/lionz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:10:55.148354 lionz-0.6/lionz/nnUNet_custom_trainer/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-15 19:10:49.000000 lionz-0.6/lionz/nnUNet_custom_trainer/LION_custom_trainers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 19:10:49.000000 lionz-0.6/lionz/nnUNet_custom_trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-03-15 19:10:49.000000 lionz-0.6/lionz/nnUNet_custom_trainer/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-03-15 19:10:49.000000 lionz-0.6/lionz/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)    11072 2024-03-15 19:10:49.000000 lionz-0.6/lionz/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:10:55.148354 lionz-0.6/lionz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-03-15 19:10:55.000000 lionz-0.6/lionz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-15 19:10:55.000000 lionz-0.6/lionz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 19:10:55.000000 lionz-0.6/lionz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-15 19:10:55.000000 lionz-0.6/lionz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-15 19:10:55.000000 lionz-0.6/lionz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-15 19:10:55.000000 lionz-0.6/lionz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 19:10:55.148354 lionz-0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-03-15 19:10:49.000000 lionz-0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:47:49.168953 lionz-0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-17 08:47:49.168953 lionz-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12295 2024-05-17 08:47:33.000000 lionz-0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:47:49.168953 lionz-0.7/lionz/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-17 08:47:33.000000 lionz-0.7/lionz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-17 08:47:33.000000 lionz-0.7/lionz/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-05-17 08:47:33.000000 lionz-0.7/lionz/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-17 08:47:33.000000 lionz-0.7/lionz/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-05-17 08:47:33.000000 lionz-0.7/lionz/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9126 2024-05-17 08:47:33.000000 lionz-0.7/lionz/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26289 2024-05-17 08:47:33.000000 lionz-0.7/lionz/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-17 08:47:33.000000 lionz-0.7/lionz/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16353 2024-05-17 08:47:33.000000 lionz-0.7/lionz/lionz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:47:49.168953 lionz-0.7/lionz/nnUNet_custom_trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-17 08:47:33.000000 lionz-0.7/lionz/nnUNet_custom_trainer/LION_custom_trainers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:47:33.000000 lionz-0.7/lionz/nnUNet_custom_trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-17 08:47:33.000000 lionz-0.7/lionz/nnUNet_custom_trainer/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-05-17 08:47:33.000000 lionz-0.7/lionz/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11399 2024-05-17 08:47:33.000000 lionz-0.7/lionz/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:47:49.168953 lionz-0.7/lionz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-17 08:47:49.000000 lionz-0.7/lionz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-17 08:47:49.000000 lionz-0.7/lionz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 08:47:49.000000 lionz-0.7/lionz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-17 08:47:49.000000 lionz-0.7/lionz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-17 08:47:49.000000 lionz-0.7/lionz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-17 08:47:49.000000 lionz-0.7/lionz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 08:47:49.168953 lionz-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-17 08:47:33.000000 lionz-0.7/setup.py
```

### Comparing `lionz-0.6/PKG-INFO` & `lionz-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lionz
-Version: 0.6
+Version: 0.7
 Summary: A toolkit for precise segmentation of tumors in PET/CT scans.
 Home-page: https://github.com/QIMP-Team/lionz
 Download-URL: https://github.com/QIMP-Team/lionz/archive/v0.1.tar.gz
 Author: Lalith Kumar Shiyam Sundar, Sebastian Gutschmayer, Manuel Pires, Zacharias Chalampalakis
 Author-email: lalith.shiyamsundar@meduniwien.ac.at, sebastian.gutschmayer@meduniwien.ac.at, manuel.pires@meduniwien.ac.at, Zacharias.Chalampalakis@meduniwien.ac.at
 Project-URL: Bug Tracker, https://github.com/QIMP-Team/lionz/issues
 Project-URL: Documentation, https://lionz.readthedocs.io/en/latest/
```

### Comparing `lionz-0.6/README.md` & `lionz-0.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-![Lion-logo.png](/Images/Lion-logo.png)
+![Lion-logo.png](/Images/lion.png)
 ## LION (Lesion segmentatION): Loud. Proud. Unbounded. 🦁
 [![Recommended Version](https://img.shields.io/badge/Recommended-pip%20install%20lionz%3D%3D0.4.0-9400D3.svg)](https://pypi.org/project/lionz/0.4.0/) 
 [![Monthly Downloads](https://img.shields.io/pypi/dm/lionz?label=Downloads%20(Monthly)&color=9400D3&style=flat-square&logo=python)](https://pypi.org/project/lionz/) 
 [![Daily Downloads](https://img.shields.io/pypi/dd/lionz?label=Downloads%20(Daily)&color=9400D3&style=flat-square&logo=python)](https://pypi.org/project/lionz/)
-[![DOI](https://zenodo.org/badge/685935027.svg)](https://zenodo.org/badge/latestdoi/685935027)
+[![DOI](https://zenodo.org/badge/685935027.svg)](https://zenodo.org/badge/latestdoi/685935027)<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
+[![All Contributors](https://img.shields.io/badge/all_contributors-3-orange.svg?style=flat-square)](#contributors-)
+<!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 
 
 
-LION has roared onto the scene, revolutionizing the way we view lesion segmentation. Born from the same lineage as MOOSE 2.0, LION is laser-focused on PET tumor segmentation. Our curated models, each crafted with precision, cater to various tracers, setting the gold standard in lesion detection.
 
-✨ **Exclusive Engineering Paradigm**: With LION, segmentation is not just a task; it's an orchestrated dance of models. Define workflows for each model, mix and match channels as some models thrive on PET/CT while others are optimized for just PET. Run them in a sequence that maximizes output and efficiency. This unique trait of LION lets you tailor the process to your exact needs, making lesion segmentation an art of precision.
+LION has roared onto the scene, revolutionizing the way we view lesion segmentation. Born from the same lineage as MOOSE 2.0, LION is laser-focused on tumor segmentation. Our curated models, each crafted with precision, cater to various tracers, setting the gold standard in lesion detection.
+
+✨ **Exclusive Engineering Paradigm**: With LION, segmentation is not just a task; it's an orchestrated dance of models. Define workflows for each model, mix and match channels as some models thrive on PET/CT while others are optimized for just PET or CT. Run them in a sequence that maximizes output and efficiency. This unique trait of LION lets you tailor the process to your exact needs, making lesion segmentation an art of precision.
 
-🌐 **Autopet-fueled Power**: LION has been trained on 1014 Autopet datasets. This vast and focused dataset empowers LION to spot and segment lesions with exceptional accuracy.
 
 🔔 **Flexibility Unleashed**: Whether you're looking for a command-line tool for batch processing or a library package for your Python projects, LION has you covered. Seamlessly integrate it into your work environment and watch it shine.
 
 Dive into the exciting world of PET tumor segmentation with LION and experience the future today!
 
 🔔 **Important Notification:** As of now, the LION tool is optimized and validated for FDG imaging. Development for PSMA imaging is ongoing and will be available soon. We appreciate your patience and understanding. Stay tuned for updates! 🔔
 
@@ -251,7 +253,31 @@
 Take, for instance, our LION package, dubbed 'lionz', pronounced "lion-zee". Now, one might wonder, why append a 'Z'?
 
 In the expansive realm of science and mathematics, 'Z' is frequently invoked as a representation of the unexplored, the variables that are shrouded in mystery, or the ultimate point in a sequence. This mirrors our ethos at QIMP perfectly. We're inveterate boundary-pushers, ever eager to trek into the uncharted, always aligning ourselves with the vanguard of technological advancement. The 'Z' is a testament to this ethos. It symbolizes our ceaseless endeavor to transcend the conventional, to journey into the untouched, and to be the torchbearers of the future in medical imaging.
 
 So, the next time you stumble upon a 'Z' in any of our package names, let it serve as a reminder of the zest for exploration and the spirit of discovery that fuels us. With QIMP, you're not merely downloading a tool; you're aligning yourself with a movement that aims to redefine the landscape of medical image processing. Let's soar into the realms of the 'Z' dimension, side by side! 🚀
 
 ---
+
+## Contributors ✨
+
+Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/LalithShiyam"><img src="https://avatars.githubusercontent.com/u/48599863?v=4?s=100" width="100px;" alt="Lalith Kumar Shiyam Sundar"/><br /><sub><b>Lalith Kumar Shiyam Sundar</b></sub></a><br /><a href="https://github.com/LalithShiyam/LION/commits?author=LalithShiyam" title="Code">💻</a></td>  
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mprires"><img src="https://avatars.githubusercontent.com/u/48754309?v=4?s=100" width="100px;" alt="Manuel Pires"/><br /><sub><b>Manuel Pires</b></sub></a><br /><a href="https://github.com/LalithShiyam/LION/commits?author=mprires" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Keyn34"><img src="https://avatars.githubusercontent.com/u/87951050?v=4?s=100" width="100px;" alt="Sebastian Gutschmayer"/><br /><sub><b>Sebastian Gutschmayer</b></sub></a><br /><a href="https://github.com/LalithShiyam/LION/commits?author=Keyn34" title="Code">💻</a></td>
+    </tr>
+  </tbody>
+</table>
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+
+This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
```

### Comparing `lionz-0.6/lionz/constants.py` & `lionz-0.7/lionz/constants.py`

 * *Files identical despite different names*

### Comparing `lionz-0.6/lionz/display.py` & `lionz-0.7/lionz/display.py`

 * *Files identical despite different names*

### Comparing `lionz-0.6/lionz/download.py` & `lionz-0.7/lionz/download.py`

 * *Files identical despite different names*

### Comparing `lionz-0.6/lionz/file_utilities.py` & `lionz-0.7/lionz/file_utilities.py`

 * *Files identical despite different names*

### Comparing `lionz-0.6/lionz/image_conversion.py` & `lionz-0.7/lionz/image_conversion.py`

 * *Files identical despite different names*

### Comparing `lionz-0.6/lionz/image_processing.py` & `lionz-0.7/lionz/image_processing.py`

 * *Files identical despite different names*

### Comparing `lionz-0.6/lionz/input_validation.py` & `lionz-0.7/lionz/input_validation.py`

 * *Files identical despite different names*

### Comparing `lionz-0.6/lionz/lionz.py` & `lionz-0.7/lionz/lionz.py`

 * *Files identical despite different names*

### Comparing `lionz-0.6/lionz/nnUNet_custom_trainer/utility.py` & `lionz-0.7/lionz/nnUNet_custom_trainer/utility.py`

 * *Files identical despite different names*

### Comparing `lionz-0.6/lionz/predict.py` & `lionz-0.7/lionz/predict.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,18 +83,21 @@
 
     mask_path = None
 
     for workflow_name, task_number in workflow_to_task_map.items():
         # Predict using the current workflow
         current_workflow_dir = os.path.join(workflow_dir, f"{model_name}_{workflow_name}")
         trainer = [model["trainer"] for model in MODELS[model_name] if task_number in model["directory"]][0]
-        command = f'nnUNetv2_predict -i {current_workflow_dir} -o {output_dir} -d {task_number} -c 3d_fullres' \
-                  f' -f all -tr {trainer} --disable_tta -device {accelerator}'
+        plans = [model["plans"] for model in MODELS[model_name] if task_number in model["directory"]][0]
+        configuration = [model["configuration"] for model in MODELS[model_name] if task_number in model["directory"]][0]
+        command = f'nnUNetv2_predict -i {current_workflow_dir} -o {output_dir} -d {task_number} -c {configuration}' \
+                  f' -f all -tr {trainer} --disable_tta -device {accelerator} -p {plans}'
         os.environ["nnUNet_results"] = NNUNET_RESULTS_FOLDER
-        subprocess.run(command, shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL, env=os.environ)
+        subprocess.run(command, shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+
 
         mask_path = get_files(output_dir, '.nii.gz')[0]
 
         # Retain only the tumor label
         tumor_label = TRACER_WORKFLOWS[model_name]['workflows'][workflow_name]["tumor_label"]
         prediction = nib.load(mask_path)
         prediction_data = prediction.get_fdata()
```

### Comparing `lionz-0.6/lionz/resources.py` & `lionz-0.7/lionz/resources.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,32 +71,33 @@
             'pet_ct': {
                 'tumor_label': 11,
                 'channels': {
                     'PT': '0000.nii.gz',
                     'CT': '0001.nii.gz'
                 }
             },
-            'pet': {
-                'tumor_label': 11,  # Adjust this if the tumor label is different for the 'pet' workflow
-                'channels': {
-                    'PT': '0000.nii.gz'
-                }
-            }
+             'pet': {
+                 'tumor_label': 11,  # Adjust this if the tumor label is different for the 'pet' workflow
+                 'channels': {
+                     'PT': '0000.nii.gz'
+                 }
+             }
         }
     },
     'psma': {
         'reference_modality': 'PT',  # You can change this for psma if needed
         'workflows': {
             'pet': {
+                'tumor_label': 6,
                 'channels': {
                     'PT': '0000.nii.gz'
                 }
             }
         }
-    },  
+    },
     'mpx': {
         'reference_modality': 'PT',  # You can change this for psma if needed
         'workflows': {
             'pet': {
                 'tumor_label': 11,  # Adjust this if the tumor label is different for the 'pet' workflow
                 'channels': {
                     'PT': '0000.nii.gz'
@@ -119,50 +120,60 @@
 #    - multilabel_prefix: A prefix to distinguish between different types of labels in multi-label models.
 #
 # To include your own model, add a new entry to this dictionary following the above format.
 
 MODELS = {
     "fdg": [
         {
-            "url": "https://ucd-emic-muv.s3.us-west-2.amazonaws.com/lion/clin_pt_fdg_ct_2000epochs.zip",
-            "filename": "Dataset789_Tumors_all_organs_LION.zip",
-            "directory": "Dataset789_Tumors_all_organs_LION",
+            "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/lion/clin_pt_fdg_ct_2000epochs.zip",
+            "filename": "Dataset804_Tumors_all_organs_LION.zip",
+            "directory": "Dataset804_Tumors_all_organs_LION",
             "trainer": "nnUNetTrainerDA5_2000epochs",
             "voxel_spacing": [3, 3, 3],
-            "multilabel_prefix": "fdg_tumor_01_"
+            "multilabel_prefix": "fdg_tumor_01_",
+            "plans": "nnUNetPlans",
+            "configuration": "3d_fullres"
         },
         {
-            "url": "https://ucd-emic-muv.s3.us-west-2.amazonaws.com/lion/clin_pt_fdg_tumor_16082023.zip",
-            "filename": "Dataset804_Tumors_all_organs.zip",
-            "directory": "Dataset804_Tumors_all_organs",
+            "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/lion/clin_pt_fdg_cancer_only_DA_30102023.zip",
+            "filename": "Dataset789_Tumors.zip",
+            "directory": "Dataset789_Tumors",
             "trainer": "nnUNetTrainerDA5",
             "voxel_spacing": [3, 3, 3],
-            "multilabel_prefix": "fdg_tumor_"
+            "multilabel_prefix": "fdg_tumor_",
+            "plans": "nnUNetPlans",
+            "configuration": "3d_fullres"
         }
     ],
     "psma": [
         {
-            "url": "PLACEHOLDER_URL_FOR_MODEL",
-            "filename": "PLACEHOLDER_FILENAME",
-            "directory": "PLACEHOLDER_DIRECTORY",
-            "trainer": "PLACEHOLDER_TRAINER",
-            "voxel_spacing": ["PLACEHOLDER_X", "PLACEHOLDER_Y", "PLACEHOLDER_Z"],
-            "multilabel_prefix": "PLACEHOLDER_PREFIX"
+            "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/lion/clin_pt_resenc_PSMA550_30042024.zip",
+            "filename": "Dataset711_PSMA.zip",
+            "directory": "Dataset711_PSMA",
+            "trainer": "nnUNetTrainer",
+            "voxel_spacing": [3, 3, 3],
+            "multilabel_prefix": "psma_tumor",
+            "plans": "nnUNetResEncUNetLPlans",
+            "configuration": "3d_fullres"
         }
     ],
-    "mpx": [  
+"mpx": [
         {
-            "url": "https://ucd-emic-muv.s3.us-west-2.amazonaws.com/lion/clin_pt_fdg_tumor_16082023.zip",
-            "filename": "Dataset804_Tumors_all_organs.zip",
-            "directory": "Dataset804_Tumors_all_organs",
+            "url": "https://enhance-pet.s3.eu-central-1.amazonaws.com/lion/clin_pt_fdg_cancer_only_DA_30102023.zip",
+            "filename": "Dataset789_Tumors.zip",
+            "directory": "Dataset789_Tumors",
             "trainer": "nnUNetTrainerDA5",
             "voxel_spacing": [3, 3, 3],
-            "multilabel_prefix": "fdg_tumor_"
+            "multilabel_prefix": "fdg_tumor_",
+            "plans": "nnUNetPlans",
+            "configuration": "3d_fullres"
         }
     ],
+
+    # Add more tracers as needed, following the same structure
 }
 
 
 def check_cuda() -> str:
     """
     This function checks if CUDA is available on the device and prints the device name and number of CUDA devices
     available on the device.
@@ -191,19 +202,21 @@
 def map_model_name_to_task_number(model_name: str) -> dict:
     """
     Maps the model name to the task number based on the workflow.
     :param model_name: The name of the model.
     :return: A dictionary of workflows and their associated task numbers.
     """
     if model_name == "fdg":
-        return {'pet_ct': '789', 'pet': '804'}
-    elif model_name == "mpx":
-        return {'pet': '804'}
+        return {'pet_ct': '804', 'pet': '789'}
     elif model_name == "psma":
-        return {'workflow_name_placeholder': '444'}  # replace 'workflow_name_placeholder' with the actual workflow name
+        return {'pet': '711'}
+    elif model_name == 'mpx':
+        return {'pet': '789'}
+    elif model_name == "tracer":
+        return {'workflow_name_place_holder': '444'} # replace 'workflow_name_placeholder' with the actual workflow name
     else:
         raise Exception(f"Error: The model name '{model_name}' is not valid.")
 
 
 def has_label_above_threshold(mask_path: str, threshold: int = 10) -> bool:
     """
     Check if the mask has non-zero voxels above a certain threshold after clearing a margin of the same size.
@@ -273,18 +286,10 @@
             'action_on_false': 'stop'
         },
         'pet': {
             'rule_func': (has_label_above_threshold, {"threshold": 10}),
             'action_on_true': 'continue',
             'action_on_false': 'continue'
         }
-    },
-  
-    "mpx": {
-        'pet': {
-            'rule_func': (has_label_above_threshold, {"threshold": 10}),
-            'action_on_true': 'continue',
-            'action_on_false': 'continue'
-        }
     }
-    
+    # Add more rules for different tracers and workflows as necessary.
 }
```

### Comparing `lionz-0.6/lionz.egg-info/PKG-INFO` & `lionz-0.7/lionz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lionz
-Version: 0.6
+Version: 0.7
 Summary: A toolkit for precise segmentation of tumors in PET/CT scans.
 Home-page: https://github.com/QIMP-Team/lionz
 Download-URL: https://github.com/QIMP-Team/lionz/archive/v0.1.tar.gz
 Author: Lalith Kumar Shiyam Sundar, Sebastian Gutschmayer, Manuel Pires, Zacharias Chalampalakis
 Author-email: lalith.shiyamsundar@meduniwien.ac.at, sebastian.gutschmayer@meduniwien.ac.at, manuel.pires@meduniwien.ac.at, Zacharias.Chalampalakis@meduniwien.ac.at
 Project-URL: Bug Tracker, https://github.com/QIMP-Team/lionz/issues
 Project-URL: Documentation, https://lionz.readthedocs.io/en/latest/
```

### Comparing `lionz-0.6/lionz.egg-info/SOURCES.txt` & `lionz-0.7/lionz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lionz-0.6/setup.py` & `lionz-0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Convert the authors to a formatted string
 authors_string = ", ".join([name for name, email in AUTHORS])
 emails_string = ", ".join([email for name, email in AUTHORS])
 
 setup(
     name='lionz',
-    version='0.6',
+    version='0.7',
     packages=find_packages(),
     install_requires=[
         'nnunetv2',
         'nibabel',
         'halo',
         'pandas',
         'SimpleITK',
```

