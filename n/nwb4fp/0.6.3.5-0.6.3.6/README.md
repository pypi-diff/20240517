# Comparing `tmp/nwb4fp-0.6.3.5.tar.gz` & `tmp/nwb4fp-0.6.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwb4fp-0.6.3.5.tar", last modified: Thu May 16 12:40:17 2024, max compression
+gzip compressed data, was "nwb4fp-0.6.3.6.tar", last modified: Fri May 17 14:28:30 2024, max compression
```

## Comparing `nwb4fp-0.6.3.5.tar` & `nwb4fp-0.6.3.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 12:40:18.068521 nwb4fp-0.6.3.5/
--rw-rw-rw-   0        0        0     1089 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.5/LICENSE
--rw-rw-rw-   0        0        0     5732 2024-05-16 12:40:18.061518 nwb4fp-0.6.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     6901 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 12:40:18.090531 nwb4fp-0.6.3.5/setup.cfg
--rw-rw-rw-   0        0        0      888 2024-05-16 12:39:56.000000 nwb4fp-0.6.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:40:17.316520 nwb4fp-0.6.3.5/src/
-drwxrwxrwx   0        0        0        0 2024-05-16 12:40:17.337520 nwb4fp-0.6.3.5/src/nwb4fp/
-drwxrwxrwx   0        0        0        0 2024-05-16 12:40:17.474525 nwb4fp-0.6.3.5/src/nwb4fp/main/
--rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.5/src/nwb4fp/main/__init__.py
--rw-rw-rw-   0        0        0     3846 2024-05-16 11:52:07.000000 nwb4fp-0.6.3.5/src/nwb4fp/main/main_create_nwb.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:40:17.642518 nwb4fp-0.6.3.5/src/nwb4fp/postprocess/
--rw-rw-rw-   0        0        0    15551 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.5/src/nwb4fp/postprocess/Get_positions.py
--rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.5/src/nwb4fp/postprocess/__init__.py
--rw-rw-rw-   0        0        0     1844 2024-05-16 11:18:45.000000 nwb4fp-0.6.3.5/src/nwb4fp/postprocess/add_wfcor.py
--rw-rw-rw-   0        0        0      470 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.5/src/nwb4fp/postprocess/dlc_kinematic.py
--rw-rw-rw-   0        0        0     2485 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.5/src/nwb4fp/postprocess/extract_wf.py
--rw-rw-rw-   0        0        0     1343 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.5/src/nwb4fp/postprocess/get_potential_merge.py
--rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.5/src/nwb4fp/postprocess/lfp_channel.py
--rw-rw-rw-   0        0        0    17455 2024-05-16 12:39:49.000000 nwb4fp-0.6.3.5/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
--rw-rw-rw-   0        0        0    14469 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.5/src/nwb4fp/postprocess/quality_metrix.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:40:17.843530 nwb4fp-0.6.3.5/src/nwb4fp/preprocess/
--rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.5/src/nwb4fp/preprocess/__init__.py
--rw-rw-rw-   0        0        0      459 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.5/src/nwb4fp/preprocess/copy_file.py
--rw-rw-rw-   0        0        0      620 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.5/src/nwb4fp/preprocess/down_sample.py
--rw-rw-rw-   0        0        0     8249 2024-05-13 14:58:38.000000 nwb4fp-0.6.3.5/src/nwb4fp/preprocess/down_sample_lfp.py
--rw-rw-rw-   0        0        0     3712 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.5/src/nwb4fp/preprocess/extract_lfp.py
--rw-rw-rw-   0        0        0      148 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.5/src/nwb4fp/preprocess/get_path.py
--rw-rw-rw-   0        0        0     1203 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.5/src/nwb4fp/preprocess/load_data.py
--rw-rw-rw-   0        0        0      244 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.5/src/nwb4fp/preprocess/run_phy.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:40:17.339525 nwb4fp-0.6.3.5/src/nwb4fp/test/
-drwxrwxrwx   0        0        0        0 2024-05-16 12:40:17.339525 nwb4fp-0.6.3.5/src/nwb4fp/test/run_scripts/
--rw-rw-rw-   0        0        0     1525 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.5/src/nwb4fp/test/run_scripts/readnwb.py
--rw-rw-rw-   0        0        0     1028 2024-05-13 13:05:19.000000 nwb4fp-0.6.3.5/src/nwb4fp/test/run_scripts/readnwb_0283.py
--rw-rw-rw-   0        0        0     1108 2024-05-16 11:52:09.000000 nwb4fp-0.6.3.5/src/nwb4fp/test/run_scripts/readnwb_09PC.py
--rw-rw-rw-   0        0        0     1448 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.5/src/nwb4fp/test/run_scripts/readnwb_09PD.py
--rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.5/src/nwb4fp/test/run_scripts/test.py
--rw-rw-rw-   0        0        0     5828 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.5/src/nwb4fp/test/run_scripts/test_lfp.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:40:17.453525 nwb4fp-0.6.3.5/src/nwb4fp.egg-info/
--rw-rw-rw-   0        0        0     5732 2024-05-16 12:40:17.000000 nwb4fp-0.6.3.5/src/nwb4fp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1143 2024-05-16 12:40:17.000000 nwb4fp-0.6.3.5/src/nwb4fp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 12:40:17.000000 nwb4fp-0.6.3.5/src/nwb4fp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2885 2024-05-16 12:40:17.000000 nwb4fp-0.6.3.5/src/nwb4fp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-16 12:40:17.000000 nwb4fp-0.6.3.5/src/nwb4fp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 14:28:30.548142 nwb4fp-0.6.3.6/
+-rw-rw-rw-   0        0        0     1089 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.6/LICENSE
+-rw-rw-rw-   0        0        0     5732 2024-05-17 14:28:30.540149 nwb4fp-0.6.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6901 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-17 14:28:30.562149 nwb4fp-0.6.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      888 2024-05-17 14:28:24.000000 nwb4fp-0.6.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 14:28:29.743147 nwb4fp-0.6.3.6/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 14:28:29.759143 nwb4fp-0.6.3.6/src/nwb4fp/
+drwxrwxrwx   0        0        0        0 2024-05-17 14:28:29.917143 nwb4fp-0.6.3.6/src/nwb4fp/main/
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.6/src/nwb4fp/main/__init__.py
+-rw-rw-rw-   0        0        0     3846 2024-05-16 11:52:07.000000 nwb4fp-0.6.3.6/src/nwb4fp/main/main_create_nwb.py
+drwxrwxrwx   0        0        0        0 2024-05-17 14:28:29.749142 nwb4fp-0.6.3.6/src/nwb4fp/postprocess/
+-rw-rw-rw-   0        0        0    15551 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.6/src/nwb4fp/postprocess/Get_positions.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.6/src/nwb4fp/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     1981 2024-05-17 14:28:05.000000 nwb4fp-0.6.3.6/src/nwb4fp/postprocess/add_wfcor.py
+-rw-rw-rw-   0        0        0      470 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.6/src/nwb4fp/postprocess/dlc_kinematic.py
+-rw-rw-rw-   0        0        0     2485 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.6/src/nwb4fp/postprocess/extract_wf.py
+-rw-rw-rw-   0        0        0     1343 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.6/src/nwb4fp/postprocess/get_potential_merge.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.6/src/nwb4fp/postprocess/lfp_channel.py
+-rw-rw-rw-   0        0        0    17455 2024-05-16 12:39:49.000000 nwb4fp-0.6.3.6/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
+-rw-rw-rw-   0        0        0    14469 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.6/src/nwb4fp/postprocess/quality_metrix.py
+drwxrwxrwx   0        0        0        0 2024-05-17 14:28:29.754139 nwb4fp-0.6.3.6/src/nwb4fp/preprocess/
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.6/src/nwb4fp/preprocess/__init__.py
+-rw-rw-rw-   0        0        0      459 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.6/src/nwb4fp/preprocess/copy_file.py
+-rw-rw-rw-   0        0        0      620 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.6/src/nwb4fp/preprocess/down_sample.py
+-rw-rw-rw-   0        0        0     8249 2024-05-13 14:58:38.000000 nwb4fp-0.6.3.6/src/nwb4fp/preprocess/down_sample_lfp.py
+-rw-rw-rw-   0        0        0     3712 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.6/src/nwb4fp/preprocess/extract_lfp.py
+-rw-rw-rw-   0        0        0      148 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.6/src/nwb4fp/preprocess/get_path.py
+-rw-rw-rw-   0        0        0     1203 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.6/src/nwb4fp/preprocess/load_data.py
+-rw-rw-rw-   0        0        0      244 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.6/src/nwb4fp/preprocess/run_phy.py
+drwxrwxrwx   0        0        0        0 2024-05-17 14:28:29.761142 nwb4fp-0.6.3.6/src/nwb4fp/test/
+drwxrwxrwx   0        0        0        0 2024-05-17 14:28:30.486148 nwb4fp-0.6.3.6/src/nwb4fp/test/run_scripts/
+-rw-rw-rw-   0        0        0     1525 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.6/src/nwb4fp/test/run_scripts/readnwb.py
+-rw-rw-rw-   0        0        0     1028 2024-05-13 13:05:19.000000 nwb4fp-0.6.3.6/src/nwb4fp/test/run_scripts/readnwb_0283.py
+-rw-rw-rw-   0        0        0     1108 2024-05-16 11:52:09.000000 nwb4fp-0.6.3.6/src/nwb4fp/test/run_scripts/readnwb_09PC.py
+-rw-rw-rw-   0        0        0     1448 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.6/src/nwb4fp/test/run_scripts/readnwb_09PD.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.6/src/nwb4fp/test/run_scripts/test.py
+-rw-rw-rw-   0        0        0     5828 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.6/src/nwb4fp/test/run_scripts/test_lfp.py
+drwxrwxrwx   0        0        0        0 2024-05-17 14:28:29.885143 nwb4fp-0.6.3.6/src/nwb4fp.egg-info/
+-rw-rw-rw-   0        0        0     5732 2024-05-17 14:28:29.000000 nwb4fp-0.6.3.6/src/nwb4fp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1143 2024-05-17 14:28:29.000000 nwb4fp-0.6.3.6/src/nwb4fp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 14:28:29.000000 nwb4fp-0.6.3.6/src/nwb4fp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2885 2024-05-17 14:28:29.000000 nwb4fp-0.6.3.6/src/nwb4fp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-17 14:28:29.000000 nwb4fp-0.6.3.6/src/nwb4fp.egg-info/top_level.txt
```

### Comparing `nwb4fp-0.6.3.5/LICENSE` & `nwb4fp-0.6.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.5/PKG-INFO` & `nwb4fp-0.6.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.3.5
+Version: 0.6.3.6
 Summary: Description of my package
 Home-page: https://github.com/sachuriga/QuattrocoloLab-nwb4fp
 Author: sachuriga
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.6.3.5/README.md` & `nwb4fp-0.6.3.6/README.md`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.5/setup.py` & `nwb4fp-0.6.3.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         with open('requirements.txt', encoding='utf-8-sig') as req:
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
     except UnicodeDecodeError:
         with open('requirements.txt', encoding='utf-16') as req:
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
 setup(
     name='nwb4fp',
-    version='0.6.3.5',
+    version='0.6.3.6',
     url='https://github.com/sachuriga/QuattrocoloLab-nwb4fp',
     author='sachuriga',
     author_email='sachuriga.sachuriga@ntnu.no',
     description='Description of my package',
     #packages=find_packages(./src/),    
     install_requires=read_requirements(),
 )
```

### Comparing `nwb4fp-0.6.3.5/src/nwb4fp/main/main_create_nwb.py` & `nwb4fp-0.6.3.6/src/nwb4fp/main/main_create_nwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.5/src/nwb4fp/postprocess/Get_positions.py` & `nwb4fp-0.6.3.6/src/nwb4fp/postprocess/Get_positions.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.5/src/nwb4fp/postprocess/add_wfcor.py` & `nwb4fp-0.6.3.6/src/nwb4fp/postprocess/add_wfcor.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,12 +33,19 @@
     for file in cluster_files:
         file_path = os.path.join(path, file)
         df = pd.read_csv(file_path, sep='\t')
         merged_df = pd.concat([merged_df,df], axis=1)
         
     df5 =  pd.concat([df4,merged_df], axis=1)
     print(df0)
-    df5.to_csv(Path(fr"{path}/cluster_info.tsv"), 
+    file_path = Path(fr"{path}/cluster_info.tsv")
+
+    # 如果文件已经存在，删除它
+    if file_path.exists():
+        file_path.unlink()
+
+    df5.to_csv(file_path, 
                sep="\t", header=True, 
                index=True)
+    
 if __name__== "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nwb4fp-0.6.3.5/src/nwb4fp/postprocess/extract_wf.py` & `nwb4fp-0.6.3.6/src/nwb4fp/postprocess/extract_wf.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.5/src/nwb4fp/postprocess/get_potential_merge.py` & `nwb4fp-0.6.3.6/src/nwb4fp/postprocess/get_potential_merge.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.5/src/nwb4fp/postprocess/nwbPHYnOPHYS.py` & `nwb4fp-0.6.3.6/src/nwb4fp/postprocess/nwbPHYnOPHYS.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.5/src/nwb4fp/postprocess/quality_metrix.py` & `nwb4fp-0.6.3.6/src/nwb4fp/postprocess/quality_metrix.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.5/src/nwb4fp/preprocess/down_sample.py` & `nwb4fp-0.6.3.6/src/nwb4fp/preprocess/down_sample.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.5/src/nwb4fp/preprocess/down_sample_lfp.py` & `nwb4fp-0.6.3.6/src/nwb4fp/preprocess/down_sample_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.5/src/nwb4fp/preprocess/extract_lfp.py` & `nwb4fp-0.6.3.6/src/nwb4fp/preprocess/extract_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.5/src/nwb4fp/preprocess/load_data.py` & `nwb4fp-0.6.3.6/src/nwb4fp/preprocess/load_data.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.5/src/nwb4fp/test/run_scripts/readnwb.py` & `nwb4fp-0.6.3.6/src/nwb4fp/test/run_scripts/readnwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.5/src/nwb4fp/test/run_scripts/readnwb_0283.py` & `nwb4fp-0.6.3.6/src/nwb4fp/test/run_scripts/readnwb_0283.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.5/src/nwb4fp/test/run_scripts/readnwb_09PC.py` & `nwb4fp-0.6.3.6/src/nwb4fp/test/run_scripts/readnwb_09PC.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.5/src/nwb4fp/test/run_scripts/readnwb_09PD.py` & `nwb4fp-0.6.3.6/src/nwb4fp/test/run_scripts/readnwb_09PD.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.5/src/nwb4fp/test/run_scripts/test_lfp.py` & `nwb4fp-0.6.3.6/src/nwb4fp/test/run_scripts/test_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.5/src/nwb4fp.egg-info/PKG-INFO` & `nwb4fp-0.6.3.6/src/nwb4fp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.3.5
+Version: 0.6.3.6
 Summary: Description of my package
 Home-page: https://github.com/sachuriga/QuattrocoloLab-nwb4fp
 Author: sachuriga
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.6.3.5/src/nwb4fp.egg-info/SOURCES.txt` & `nwb4fp-0.6.3.6/src/nwb4fp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.5/src/nwb4fp.egg-info/requires.txt` & `nwb4fp-0.6.3.6/src/nwb4fp.egg-info/requires.txt`

 * *Files identical despite different names*

