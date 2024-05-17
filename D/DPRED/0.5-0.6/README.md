# Comparing `tmp/DPRED-0.5.tar.gz` & `tmp/DPRED-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DPRED-0.5.tar", last modified: Fri May 17 15:05:25 2024, max compression
+gzip compressed data, was "DPRED-0.6.tar", last modified: Fri May 17 15:11:00 2024, max compression
```

## Comparing `DPRED-0.5.tar` & `DPRED-0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 15:05:25.815538 DPRED-0.5/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 15:05:25.337116 DPRED-0.5/DPRED/
--rwxrwxrwx   0 root         (0) root         (0)       60 2024-05-17 12:33:46.000000 DPRED-0.5/DPRED/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1166 2024-05-16 17:32:28.000000 DPRED-0.5/DPRED/blast.py
--rwxrwxrwx   0 root         (0) root         (0)     5852 2024-05-16 17:32:19.000000 DPRED-0.5/DPRED/get_pdb_data.py
--rwxrwxrwx   0 root         (0) root         (0)     2376 2024-05-17 10:04:53.000000 DPRED-0.5/DPRED/get_pdb_files.py
--rwxrwxrwx   0 root         (0) root         (0)     1257 2024-05-16 17:32:23.000000 DPRED-0.5/DPRED/get_uniprot_data.py
--rwxrwxrwx   0 root         (0) root         (0)      737 2024-05-16 17:55:59.000000 DPRED-0.5/DPRED/hmm.py
--rwxrwxrwx   0 root         (0) root         (0)     3008 2024-05-17 15:02:01.000000 DPRED-0.5/DPRED/main.py
--rwxrwxrwx   0 root         (0) root         (0)     3420 2024-05-17 10:05:34.000000 DPRED-0.5/DPRED/msa.py
--rwxrwxrwx   0 root         (0) root         (0)     1572 2024-05-16 17:32:33.000000 DPRED-0.5/DPRED/performance.py
--rwxrwxrwx   0 root         (0) root         (0)      271 2024-05-16 17:32:42.000000 DPRED-0.5/DPRED/remove.py
--rwxrwxrwx   0 root         (0) root         (0)     7659 2024-05-16 17:58:57.000000 DPRED-0.5/DPRED/validation.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 15:05:25.645844 DPRED-0.5/DPRED.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      536 2024-05-17 15:05:24.000000 DPRED-0.5/DPRED.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      440 2024-05-17 15:05:24.000000 DPRED-0.5/DPRED.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-17 15:05:24.000000 DPRED-0.5/DPRED.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       42 2024-05-17 15:05:24.000000 DPRED-0.5/DPRED.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       25 2024-05-17 15:05:24.000000 DPRED-0.5/DPRED.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        6 2024-05-17 15:05:24.000000 DPRED-0.5/DPRED.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:08.000000 DPRED-0.5/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      536 2024-05-17 15:05:25.795646 DPRED-0.5/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:02.000000 DPRED-0.5/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-17 15:05:25.818079 DPRED-0.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      872 2024-05-17 15:05:09.000000 DPRED-0.5/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 15:05:25.745031 DPRED-0.5/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:27.000000 DPRED-0.5/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:35.000000 DPRED-0.5/tests/test_main.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 15:11:00.313105 DPRED-0.6/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 15:10:59.763234 DPRED-0.6/DPRED/
+-rwxrwxrwx   0 root         (0) root         (0)       60 2024-05-17 12:33:46.000000 DPRED-0.6/DPRED/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1166 2024-05-17 15:09:50.000000 DPRED-0.6/DPRED/blast.py
+-rwxrwxrwx   0 root         (0) root         (0)     5852 2024-05-17 15:09:53.000000 DPRED-0.6/DPRED/get_pdb_data.py
+-rwxrwxrwx   0 root         (0) root         (0)     2383 2024-05-17 15:09:54.000000 DPRED-0.6/DPRED/get_pdb_files.py
+-rwxrwxrwx   0 root         (0) root         (0)     1257 2024-05-17 15:09:56.000000 DPRED-0.6/DPRED/get_uniprot_data.py
+-rwxrwxrwx   0 root         (0) root         (0)      751 2024-05-17 15:09:58.000000 DPRED-0.6/DPRED/hmm.py
+-rwxrwxrwx   0 root         (0) root         (0)     3008 2024-05-17 15:09:59.000000 DPRED-0.6/DPRED/main.py
+-rwxrwxrwx   0 root         (0) root         (0)     3434 2024-05-17 15:10:02.000000 DPRED-0.6/DPRED/msa.py
+-rwxrwxrwx   0 root         (0) root         (0)     1572 2024-05-17 15:10:04.000000 DPRED-0.6/DPRED/performance.py
+-rwxrwxrwx   0 root         (0) root         (0)      271 2024-05-17 15:10:07.000000 DPRED-0.6/DPRED/remove.py
+-rwxrwxrwx   0 root         (0) root         (0)     7687 2024-05-17 15:10:21.000000 DPRED-0.6/DPRED/validation.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 15:11:00.131422 DPRED-0.6/DPRED.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      536 2024-05-17 15:10:58.000000 DPRED-0.6/DPRED.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      440 2024-05-17 15:10:58.000000 DPRED-0.6/DPRED.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-17 15:10:58.000000 DPRED-0.6/DPRED.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       42 2024-05-17 15:10:58.000000 DPRED-0.6/DPRED.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       25 2024-05-17 15:10:58.000000 DPRED-0.6/DPRED.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        6 2024-05-17 15:10:58.000000 DPRED-0.6/DPRED.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:08.000000 DPRED-0.6/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      536 2024-05-17 15:11:00.287517 DPRED-0.6/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:02.000000 DPRED-0.6/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-17 15:11:00.318629 DPRED-0.6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      872 2024-05-17 15:10:46.000000 DPRED-0.6/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 15:11:00.228465 DPRED-0.6/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:27.000000 DPRED-0.6/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:35.000000 DPRED-0.6/tests/test_main.py
```

### Comparing `DPRED-0.5/DPRED/blast.py` & `DPRED-0.6/DPRED/blast.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.5/DPRED/get_pdb_data.py` & `DPRED-0.6/DPRED/get_pdb_data.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.5/DPRED/get_pdb_files.py` & `DPRED-0.6/DPRED/get_pdb_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from Bio.PDB import PDBList, PDBParser, PDBIO, Select
 import logging
 import os
 
-import remove
+from . import remove
 
 logging.getLogger("Bio").setLevel(logging.ERROR)
 
 class ChainSelector(Select):
     '''A chain selector for Bio.PDB'''
     def __init__(self, target_chain: str) -> None:
         self.target_chain = target_chain
```

### Comparing `DPRED-0.5/DPRED/get_uniprot_data.py` & `DPRED-0.6/DPRED/get_uniprot_data.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.5/DPRED/hmm.py` & `DPRED-0.6/DPRED/hmm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import subprocess
 import time
 
-import msa
-import remove
+from . import msa
+from . import remove
 
 class HMM:
     def __init__(self, pdbobj: object, pfam: str, mtm: bool, pdb: bool) -> None:
         self.msa = 'msa'
         if not os.path.exists(self.msa): msa.MSA(pdbobj, pfam, mtm, pdb).write_msa()
         
     def hmm(self, name: str, msa: bool) -> None:
```

### Comparing `DPRED-0.5/DPRED/main.py` & `DPRED-0.6/DPRED/main.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.5/DPRED/msa.py` & `DPRED-0.6/DPRED/msa.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import subprocess
 from collections import Counter
 import time
 
-import get_pdb_files as pdbfiles
-import remove
+from . import get_pdb_files as pdbfiles
+from . import remove
 
 class MSA:
     def __init__(self, pdbobj: object, pfam: str, mtm, pdb) -> None: 
         self.msadir = os.path.join(os.getcwd(), "mTM_result")
         self.pdbdir = os.path.join(os.getcwd(), "input_pdb")
         self.pdbobj, self.pfam, self.mtm, self.pdb = pdbobj, pfam, mtm, pdb
         self.ids = []
```

### Comparing `DPRED-0.5/DPRED/performance.py` & `DPRED-0.6/DPRED/performance.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.5/DPRED/validation.py` & `DPRED-0.6/DPRED/validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import subprocess
 import random
 import os
 import time
 
-import blast
-import remove
-import get_uniprot_data as updata
-import performance as pf
+from . import blast
+from . import remove
+from . import get_uniprot_data as updata
+from . import performance as pf
 
 class KCrossVal:
     
     def __init__(self, pdbobj: object, pfam: str, k: int, db: bool) -> None:
         self.k = k
         # UniProt data
         start = time.time()
```

### Comparing `DPRED-0.5/DPRED.egg-info/PKG-INFO` & `DPRED-0.6/DPRED.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DPRED
-Version: 0.5
+Version: 0.6
 Summary: DPRED is a softwares package for HMM domain prediction and validation
 Home-page: https://github.com/dganci/DPRED
 Author: Daniele Ganci
 Author-email: daniele.ganci@studio.unibo.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DPRED-0.5/PKG-INFO` & `DPRED-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DPRED
-Version: 0.5
+Version: 0.6
 Summary: DPRED is a softwares package for HMM domain prediction and validation
 Home-page: https://github.com/dganci/DPRED
 Author: Daniele Ganci
 Author-email: daniele.ganci@studio.unibo.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DPRED-0.5/setup.py` & `DPRED-0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='DPRED',
-    version='0.5',
+    version='0.6',
     packages=find_packages(include=['DPRED', 'DPRED.*']),
     install_requires=[
         'biopython',
         'requests',
         'numpy',
     ],
     entry_points={
```

