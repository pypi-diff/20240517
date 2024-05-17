# Comparing `tmp/DPRED-0.7.tar.gz` & `tmp/DPRED-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DPRED-0.7.tar", last modified: Fri May 17 15:15:13 2024, max compression
+gzip compressed data, was "DPRED-0.8.tar", last modified: Fri May 17 21:31:41 2024, max compression
```

## Comparing `DPRED-0.7.tar` & `DPRED-0.8.tar`

### file list

```diff
@@ -1,28 +1,42 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 15:15:13.127449 DPRED-0.7/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 15:15:12.693532 DPRED-0.7/DPRED/
--rwxrwxrwx   0 root         (0) root         (0)       60 2024-05-17 12:33:46.000000 DPRED-0.7/DPRED/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1166 2024-05-17 15:09:50.000000 DPRED-0.7/DPRED/blast.py
--rwxrwxrwx   0 root         (0) root         (0)     5852 2024-05-17 15:09:53.000000 DPRED-0.7/DPRED/get_pdb_data.py
--rwxrwxrwx   0 root         (0) root         (0)     2383 2024-05-17 15:09:54.000000 DPRED-0.7/DPRED/get_pdb_files.py
--rwxrwxrwx   0 root         (0) root         (0)     1257 2024-05-17 15:09:56.000000 DPRED-0.7/DPRED/get_uniprot_data.py
--rwxrwxrwx   0 root         (0) root         (0)      751 2024-05-17 15:09:58.000000 DPRED-0.7/DPRED/hmm.py
--rwxrwxrwx   0 root         (0) root         (0)     2993 2024-05-17 15:14:35.000000 DPRED-0.7/DPRED/main.py
--rwxrwxrwx   0 root         (0) root         (0)     3434 2024-05-17 15:10:02.000000 DPRED-0.7/DPRED/msa.py
--rwxrwxrwx   0 root         (0) root         (0)     1572 2024-05-17 15:10:04.000000 DPRED-0.7/DPRED/performance.py
--rwxrwxrwx   0 root         (0) root         (0)      271 2024-05-17 15:10:07.000000 DPRED-0.7/DPRED/remove.py
--rwxrwxrwx   0 root         (0) root         (0)     7687 2024-05-17 15:10:21.000000 DPRED-0.7/DPRED/validation.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 15:15:12.973817 DPRED-0.7/DPRED.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      536 2024-05-17 15:15:11.000000 DPRED-0.7/DPRED.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      440 2024-05-17 15:15:11.000000 DPRED-0.7/DPRED.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-17 15:15:11.000000 DPRED-0.7/DPRED.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       42 2024-05-17 15:15:11.000000 DPRED-0.7/DPRED.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       25 2024-05-17 15:15:11.000000 DPRED-0.7/DPRED.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        6 2024-05-17 15:15:11.000000 DPRED-0.7/DPRED.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:08.000000 DPRED-0.7/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      536 2024-05-17 15:15:13.105505 DPRED-0.7/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:02.000000 DPRED-0.7/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-17 15:15:13.127449 DPRED-0.7/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      872 2024-05-17 15:15:07.000000 DPRED-0.7/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 15:15:13.054866 DPRED-0.7/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:27.000000 DPRED-0.7/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:35.000000 DPRED-0.7/tests/test_main.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 21:31:41.129754 DPRED-0.8/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 21:31:39.647317 DPRED-0.8/DPRED/
+-rwxrwxrwx   0 root         (0) root         (0)       60 2024-05-17 12:33:46.000000 DPRED-0.8/DPRED/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1166 2024-05-17 15:09:50.000000 DPRED-0.8/DPRED/blast.py
+-rwxrwxrwx   0 root         (0) root         (0)     5852 2024-05-17 15:09:53.000000 DPRED-0.8/DPRED/get_pdb_data.py
+-rwxrwxrwx   0 root         (0) root         (0)     2383 2024-05-17 15:09:54.000000 DPRED-0.8/DPRED/get_pdb_files.py
+-rwxrwxrwx   0 root         (0) root         (0)     1257 2024-05-17 15:09:56.000000 DPRED-0.8/DPRED/get_uniprot_data.py
+-rwxrwxrwx   0 root         (0) root         (0)      751 2024-05-17 15:09:58.000000 DPRED-0.8/DPRED/hmm.py
+-rwxrwxrwx   0 root         (0) root         (0)     2993 2024-05-17 15:14:35.000000 DPRED-0.8/DPRED/main.py
+-rwxrwxrwx   0 root         (0) root         (0)     3424 2024-05-17 21:26:13.000000 DPRED-0.8/DPRED/msa.py
+-rwxrwxrwx   0 root         (0) root         (0)     1572 2024-05-17 15:10:04.000000 DPRED-0.8/DPRED/performance.py
+-rwxrwxrwx   0 root         (0) root         (0)      271 2024-05-17 15:10:07.000000 DPRED-0.8/DPRED/remove.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 21:31:40.958786 DPRED-0.8/DPRED/src/
+-rwxrwxrwx   0 root         (0) root         (0)    11686 2018-07-26 08:18:18.000000 DPRED-0.8/DPRED/src/Kabsch.h
+-rwxrwxrwx   0 root         (0) root         (0)      109 2022-01-04 04:17:11.000000 DPRED-0.8/DPRED/src/Makefile
+-rwxrwxrwx   0 root         (0) root         (0)     6006 2018-07-26 08:18:17.000000 DPRED-0.8/DPRED/src/NW.h
+-rwxrwxrwx   0 root         (0) root         (0)    72079 2022-01-05 10:38:25.000000 DPRED-0.8/DPRED/src/TMM.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     3657 2022-01-04 06:07:35.000000 DPRED-0.8/DPRED/src/TMM.h
+-rwxrwxrwx   0 root         (0) root         (0)    36346 2018-07-26 08:18:17.000000 DPRED-0.8/DPRED/src/TMalign.h
+-rwxrwxrwx   0 root         (0) root         (0)    14228 2018-07-26 08:18:17.000000 DPRED-0.8/DPRED/src/TMalign_main.h
+-rwxrwxrwx   0 root         (0) root         (0)    14694 2018-07-26 08:18:17.000000 DPRED-0.8/DPRED/src/UPGMA.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     1973 2018-07-26 08:18:17.000000 DPRED-0.8/DPRED/src/UPGMA.h
+-rwxrwxrwx   0 root         (0) root         (0)    14990 2018-09-13 06:40:53.000000 DPRED-0.8/DPRED/src/basic_fun.h
+-rwxrwxrwx   0 root         (0) root         (0)   347960 2024-04-30 10:42:08.000000 DPRED-0.8/DPRED/src/mTM-align
+-rwxrwxrwx   0 root         (0) root         (0)     4179 2022-01-05 10:48:54.000000 DPRED-0.8/DPRED/src/main.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     7687 2024-05-17 15:10:21.000000 DPRED-0.8/DPRED/validation.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 21:31:39.932419 DPRED-0.8/DPRED.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      536 2024-05-17 21:31:38.000000 DPRED-0.8/DPRED.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      683 2024-05-17 21:31:38.000000 DPRED-0.8/DPRED.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-17 21:31:38.000000 DPRED-0.8/DPRED.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       42 2024-05-17 21:31:38.000000 DPRED-0.8/DPRED.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       25 2024-05-17 21:31:38.000000 DPRED-0.8/DPRED.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        6 2024-05-17 21:31:38.000000 DPRED-0.8/DPRED.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:08.000000 DPRED-0.8/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       19 2024-05-17 21:26:51.000000 DPRED-0.8/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)      536 2024-05-17 21:31:41.109501 DPRED-0.8/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:02.000000 DPRED-0.8/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-17 21:31:41.134278 DPRED-0.8/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      961 2024-05-17 21:25:15.000000 DPRED-0.8/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 21:31:41.054692 DPRED-0.8/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:27.000000 DPRED-0.8/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:35.000000 DPRED-0.8/tests/test_main.py
```

### Comparing `DPRED-0.7/DPRED/blast.py` & `DPRED-0.8/DPRED/blast.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.7/DPRED/get_pdb_data.py` & `DPRED-0.8/DPRED/get_pdb_data.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.7/DPRED/get_pdb_files.py` & `DPRED-0.8/DPRED/get_pdb_files.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.7/DPRED/get_uniprot_data.py` & `DPRED-0.8/DPRED/get_uniprot_data.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.7/DPRED/hmm.py` & `DPRED-0.8/DPRED/hmm.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.7/DPRED/main.py` & `DPRED-0.8/DPRED/main.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.7/DPRED/msa.py` & `DPRED-0.8/DPRED/msa.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         print(f'Done. Time = {int(round(h))}:{int(round(m))}:{int(round(s))}')
     
     def _msa(self) -> None:
         if not os.path.exists(self.pdbdir): self._download_pdb()    
         with open('pdblst', 'w') as f: f.write(self.pdbobj.get_lst())
         start = time.time()
         print('Performing multiple structural alignment...')
-        subprocess.run(["./mTM-align/src/mTM-align", "-i", "pdblst"], stdout=subprocess.DEVNULL)
+        subprocess.run(["./src/mTM-align", "-i", "pdblst"], stdout=subprocess.DEVNULL)
         lap = time.time()-start
         h, rem = divmod(lap, 3600)
         m, s = divmod(rem, 60)
         print(f'Done. Time = {int(round(h))}:{int(round(m))}:{int(round(s))}')
         if self.pdb is False: remove.Remove(self.pdbdir).remove() # remove input_pdb
         if self.mtm is False: remove.Remove('pdblst').remove() # remove pdblst
```

### Comparing `DPRED-0.7/DPRED/performance.py` & `DPRED-0.8/DPRED/performance.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.7/DPRED/validation.py` & `DPRED-0.8/DPRED/validation.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.7/DPRED.egg-info/PKG-INFO` & `DPRED-0.8/DPRED.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DPRED
-Version: 0.7
+Version: 0.8
 Summary: DPRED is a softwares package for HMM domain prediction and validation
 Home-page: https://github.com/dganci/DPRED
 Author: Daniele Ganci
 Author-email: daniele.ganci@studio.unibo.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DPRED-0.7/PKG-INFO` & `DPRED-0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DPRED
-Version: 0.7
+Version: 0.8
 Summary: DPRED is a softwares package for HMM domain prediction and validation
 Home-page: https://github.com/dganci/DPRED
 Author: Daniele Ganci
 Author-email: daniele.ganci@studio.unibo.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DPRED-0.7/setup.py` & `DPRED-0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='DPRED',
-    version='0.7',
+    version='0.8',
     packages=find_packages(include=['DPRED', 'DPRED.*']),
     install_requires=[
         'biopython',
         'requests',
         'numpy',
     ],
     entry_points={
@@ -22,8 +22,12 @@
     url='https://github.com/dganci/DPRED',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
+    include_package_data=True,
+    package_data={
+        'DPRED': ['src/*'],
+    },
 )
```

