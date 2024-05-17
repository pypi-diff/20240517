# Comparing `tmp/DPRED-0.4.tar.gz` & `tmp/DPRED-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DPRED-0.4.tar", last modified: Fri May 17 14:50:36 2024, max compression
+gzip compressed data, was "DPRED-0.5.tar", last modified: Fri May 17 15:05:25 2024, max compression
```

## Comparing `DPRED-0.4.tar` & `DPRED-0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 14:50:36.015210 DPRED-0.4/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 14:50:35.777219 DPRED-0.4/DPRED/
--rwxrwxrwx   0 root         (0) root         (0)       60 2024-05-17 12:33:46.000000 DPRED-0.4/DPRED/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1166 2024-05-16 17:32:28.000000 DPRED-0.4/DPRED/blast.py
--rwxrwxrwx   0 root         (0) root         (0)     5852 2024-05-16 17:32:19.000000 DPRED-0.4/DPRED/get_pdb_data.py
--rwxrwxrwx   0 root         (0) root         (0)     2376 2024-05-17 10:04:53.000000 DPRED-0.4/DPRED/get_pdb_files.py
--rwxrwxrwx   0 root         (0) root         (0)     1257 2024-05-16 17:32:23.000000 DPRED-0.4/DPRED/get_uniprot_data.py
--rwxrwxrwx   0 root         (0) root         (0)      737 2024-05-16 17:55:59.000000 DPRED-0.4/DPRED/hmm.py
--rwxrwxrwx   0 root         (0) root         (0)     2987 2024-05-17 13:15:58.000000 DPRED-0.4/DPRED/main.py
--rwxrwxrwx   0 root         (0) root         (0)     3420 2024-05-17 10:05:34.000000 DPRED-0.4/DPRED/msa.py
--rwxrwxrwx   0 root         (0) root         (0)     1572 2024-05-16 17:32:33.000000 DPRED-0.4/DPRED/performance.py
--rwxrwxrwx   0 root         (0) root         (0)      271 2024-05-16 17:32:42.000000 DPRED-0.4/DPRED/remove.py
--rwxrwxrwx   0 root         (0) root         (0)     7659 2024-05-16 17:58:57.000000 DPRED-0.4/DPRED/validation.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 14:50:35.933572 DPRED-0.4/DPRED.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      536 2024-05-17 14:50:35.000000 DPRED-0.4/DPRED.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      440 2024-05-17 14:50:35.000000 DPRED-0.4/DPRED.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-17 14:50:35.000000 DPRED-0.4/DPRED.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       42 2024-05-17 14:50:35.000000 DPRED-0.4/DPRED.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       25 2024-05-17 14:50:35.000000 DPRED-0.4/DPRED.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       12 2024-05-17 14:50:35.000000 DPRED-0.4/DPRED.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:08.000000 DPRED-0.4/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      536 2024-05-17 14:50:36.002681 DPRED-0.4/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:02.000000 DPRED-0.4/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-17 14:50:36.015210 DPRED-0.4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      844 2024-05-17 14:50:26.000000 DPRED-0.4/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 14:50:35.974506 DPRED-0.4/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:27.000000 DPRED-0.4/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:35.000000 DPRED-0.4/tests/test_main.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 15:05:25.815538 DPRED-0.5/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 15:05:25.337116 DPRED-0.5/DPRED/
+-rwxrwxrwx   0 root         (0) root         (0)       60 2024-05-17 12:33:46.000000 DPRED-0.5/DPRED/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1166 2024-05-16 17:32:28.000000 DPRED-0.5/DPRED/blast.py
+-rwxrwxrwx   0 root         (0) root         (0)     5852 2024-05-16 17:32:19.000000 DPRED-0.5/DPRED/get_pdb_data.py
+-rwxrwxrwx   0 root         (0) root         (0)     2376 2024-05-17 10:04:53.000000 DPRED-0.5/DPRED/get_pdb_files.py
+-rwxrwxrwx   0 root         (0) root         (0)     1257 2024-05-16 17:32:23.000000 DPRED-0.5/DPRED/get_uniprot_data.py
+-rwxrwxrwx   0 root         (0) root         (0)      737 2024-05-16 17:55:59.000000 DPRED-0.5/DPRED/hmm.py
+-rwxrwxrwx   0 root         (0) root         (0)     3008 2024-05-17 15:02:01.000000 DPRED-0.5/DPRED/main.py
+-rwxrwxrwx   0 root         (0) root         (0)     3420 2024-05-17 10:05:34.000000 DPRED-0.5/DPRED/msa.py
+-rwxrwxrwx   0 root         (0) root         (0)     1572 2024-05-16 17:32:33.000000 DPRED-0.5/DPRED/performance.py
+-rwxrwxrwx   0 root         (0) root         (0)      271 2024-05-16 17:32:42.000000 DPRED-0.5/DPRED/remove.py
+-rwxrwxrwx   0 root         (0) root         (0)     7659 2024-05-16 17:58:57.000000 DPRED-0.5/DPRED/validation.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 15:05:25.645844 DPRED-0.5/DPRED.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      536 2024-05-17 15:05:24.000000 DPRED-0.5/DPRED.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      440 2024-05-17 15:05:24.000000 DPRED-0.5/DPRED.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-17 15:05:24.000000 DPRED-0.5/DPRED.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       42 2024-05-17 15:05:24.000000 DPRED-0.5/DPRED.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       25 2024-05-17 15:05:24.000000 DPRED-0.5/DPRED.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        6 2024-05-17 15:05:24.000000 DPRED-0.5/DPRED.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:08.000000 DPRED-0.5/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      536 2024-05-17 15:05:25.795646 DPRED-0.5/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:02.000000 DPRED-0.5/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-17 15:05:25.818079 DPRED-0.5/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      872 2024-05-17 15:05:09.000000 DPRED-0.5/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 15:05:25.745031 DPRED-0.5/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:27.000000 DPRED-0.5/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:35.000000 DPRED-0.5/tests/test_main.py
```

### Comparing `DPRED-0.4/DPRED/blast.py` & `DPRED-0.5/DPRED/blast.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.4/DPRED/get_pdb_data.py` & `DPRED-0.5/DPRED/get_pdb_data.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.4/DPRED/get_pdb_files.py` & `DPRED-0.5/DPRED/get_pdb_files.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.4/DPRED/get_uniprot_data.py` & `DPRED-0.5/DPRED/get_uniprot_data.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.4/DPRED/hmm.py` & `DPRED-0.5/DPRED/hmm.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.4/DPRED/main.py` & `DPRED-0.5/DPRED/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 import time
 
-import get_pdb_data as pdbdata
-import hmm
-import validation
+from . import get_pdb_data as pdbdata
+from . import hmm
+from . import validation
 
 def PDBobj(pfam: str, l: list, res: int, mut: int, iden: int): return pdbdata.GetPDB(pfam, l, res, mut, iden)
 
 def DPRED(pdbobj: object, pfam: str, k: int, l: int, bid: int, n: str, mtm: bool, msa: bool, pdb: bool, chunks: bool, sets: bool, db: bool) -> None:
     start = time.time()
     hmm.HMM(pdbobj, pfam, mtm, pdb).hmm(n, msa) # generates a HMM model for domain prediction
     validation.KCrossVal(pdbobj, pfam, k, db).validation(bid, l, chunks, sets, n) # validate the model through a K-fold CV
```

### Comparing `DPRED-0.4/DPRED/msa.py` & `DPRED-0.5/DPRED/msa.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.4/DPRED/performance.py` & `DPRED-0.5/DPRED/performance.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.4/DPRED/validation.py` & `DPRED-0.5/DPRED/validation.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.4/DPRED.egg-info/PKG-INFO` & `DPRED-0.5/DPRED.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DPRED
-Version: 0.4
+Version: 0.5
 Summary: DPRED is a softwares package for HMM domain prediction and validation
 Home-page: https://github.com/dganci/DPRED
 Author: Daniele Ganci
 Author-email: daniele.ganci@studio.unibo.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DPRED-0.4/PKG-INFO` & `DPRED-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DPRED
-Version: 0.4
+Version: 0.5
 Summary: DPRED is a softwares package for HMM domain prediction and validation
 Home-page: https://github.com/dganci/DPRED
 Author: Daniele Ganci
 Author-email: daniele.ganci@studio.unibo.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DPRED-0.4/setup.py` & `DPRED-0.5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='DPRED',
-    version='0.4',
-    packages=find_packages(),
+    version='0.5',
+    packages=find_packages(include=['DPRED', 'DPRED.*']),
     install_requires=[
         'biopython',
         'requests',
         'numpy',
     ],
     entry_points={
         'console_scripts': [
```

