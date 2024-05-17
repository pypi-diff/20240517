# Comparing `tmp/DPRED-0.6.tar.gz` & `tmp/DPRED-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DPRED-0.6.tar", last modified: Fri May 17 15:11:00 2024, max compression
+gzip compressed data, was "DPRED-0.7.tar", last modified: Fri May 17 15:15:13 2024, max compression
```

## Comparing `DPRED-0.6.tar` & `DPRED-0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 15:11:00.313105 DPRED-0.6/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 15:10:59.763234 DPRED-0.6/DPRED/
--rwxrwxrwx   0 root         (0) root         (0)       60 2024-05-17 12:33:46.000000 DPRED-0.6/DPRED/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1166 2024-05-17 15:09:50.000000 DPRED-0.6/DPRED/blast.py
--rwxrwxrwx   0 root         (0) root         (0)     5852 2024-05-17 15:09:53.000000 DPRED-0.6/DPRED/get_pdb_data.py
--rwxrwxrwx   0 root         (0) root         (0)     2383 2024-05-17 15:09:54.000000 DPRED-0.6/DPRED/get_pdb_files.py
--rwxrwxrwx   0 root         (0) root         (0)     1257 2024-05-17 15:09:56.000000 DPRED-0.6/DPRED/get_uniprot_data.py
--rwxrwxrwx   0 root         (0) root         (0)      751 2024-05-17 15:09:58.000000 DPRED-0.6/DPRED/hmm.py
--rwxrwxrwx   0 root         (0) root         (0)     3008 2024-05-17 15:09:59.000000 DPRED-0.6/DPRED/main.py
--rwxrwxrwx   0 root         (0) root         (0)     3434 2024-05-17 15:10:02.000000 DPRED-0.6/DPRED/msa.py
--rwxrwxrwx   0 root         (0) root         (0)     1572 2024-05-17 15:10:04.000000 DPRED-0.6/DPRED/performance.py
--rwxrwxrwx   0 root         (0) root         (0)      271 2024-05-17 15:10:07.000000 DPRED-0.6/DPRED/remove.py
--rwxrwxrwx   0 root         (0) root         (0)     7687 2024-05-17 15:10:21.000000 DPRED-0.6/DPRED/validation.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 15:11:00.131422 DPRED-0.6/DPRED.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      536 2024-05-17 15:10:58.000000 DPRED-0.6/DPRED.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      440 2024-05-17 15:10:58.000000 DPRED-0.6/DPRED.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-17 15:10:58.000000 DPRED-0.6/DPRED.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       42 2024-05-17 15:10:58.000000 DPRED-0.6/DPRED.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       25 2024-05-17 15:10:58.000000 DPRED-0.6/DPRED.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        6 2024-05-17 15:10:58.000000 DPRED-0.6/DPRED.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:08.000000 DPRED-0.6/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      536 2024-05-17 15:11:00.287517 DPRED-0.6/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:02.000000 DPRED-0.6/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-17 15:11:00.318629 DPRED-0.6/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      872 2024-05-17 15:10:46.000000 DPRED-0.6/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 15:11:00.228465 DPRED-0.6/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:27.000000 DPRED-0.6/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:35.000000 DPRED-0.6/tests/test_main.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 15:15:13.127449 DPRED-0.7/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 15:15:12.693532 DPRED-0.7/DPRED/
+-rwxrwxrwx   0 root         (0) root         (0)       60 2024-05-17 12:33:46.000000 DPRED-0.7/DPRED/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1166 2024-05-17 15:09:50.000000 DPRED-0.7/DPRED/blast.py
+-rwxrwxrwx   0 root         (0) root         (0)     5852 2024-05-17 15:09:53.000000 DPRED-0.7/DPRED/get_pdb_data.py
+-rwxrwxrwx   0 root         (0) root         (0)     2383 2024-05-17 15:09:54.000000 DPRED-0.7/DPRED/get_pdb_files.py
+-rwxrwxrwx   0 root         (0) root         (0)     1257 2024-05-17 15:09:56.000000 DPRED-0.7/DPRED/get_uniprot_data.py
+-rwxrwxrwx   0 root         (0) root         (0)      751 2024-05-17 15:09:58.000000 DPRED-0.7/DPRED/hmm.py
+-rwxrwxrwx   0 root         (0) root         (0)     2993 2024-05-17 15:14:35.000000 DPRED-0.7/DPRED/main.py
+-rwxrwxrwx   0 root         (0) root         (0)     3434 2024-05-17 15:10:02.000000 DPRED-0.7/DPRED/msa.py
+-rwxrwxrwx   0 root         (0) root         (0)     1572 2024-05-17 15:10:04.000000 DPRED-0.7/DPRED/performance.py
+-rwxrwxrwx   0 root         (0) root         (0)      271 2024-05-17 15:10:07.000000 DPRED-0.7/DPRED/remove.py
+-rwxrwxrwx   0 root         (0) root         (0)     7687 2024-05-17 15:10:21.000000 DPRED-0.7/DPRED/validation.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 15:15:12.973817 DPRED-0.7/DPRED.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      536 2024-05-17 15:15:11.000000 DPRED-0.7/DPRED.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      440 2024-05-17 15:15:11.000000 DPRED-0.7/DPRED.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-17 15:15:11.000000 DPRED-0.7/DPRED.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       42 2024-05-17 15:15:11.000000 DPRED-0.7/DPRED.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       25 2024-05-17 15:15:11.000000 DPRED-0.7/DPRED.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        6 2024-05-17 15:15:11.000000 DPRED-0.7/DPRED.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:08.000000 DPRED-0.7/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      536 2024-05-17 15:15:13.105505 DPRED-0.7/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:02.000000 DPRED-0.7/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-17 15:15:13.127449 DPRED-0.7/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      872 2024-05-17 15:15:07.000000 DPRED-0.7/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 15:15:13.054866 DPRED-0.7/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:27.000000 DPRED-0.7/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:35.000000 DPRED-0.7/tests/test_main.py
```

### Comparing `DPRED-0.6/DPRED/blast.py` & `DPRED-0.7/DPRED/blast.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.6/DPRED/get_pdb_data.py` & `DPRED-0.7/DPRED/get_pdb_data.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.6/DPRED/get_pdb_files.py` & `DPRED-0.7/DPRED/get_pdb_files.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.6/DPRED/get_uniprot_data.py` & `DPRED-0.7/DPRED/get_uniprot_data.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.6/DPRED/hmm.py` & `DPRED-0.7/DPRED/hmm.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.6/DPRED/main.py` & `DPRED-0.7/DPRED/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     validation.KCrossVal(pdbobj, pfam, k, db).validation(bid, l, chunks, sets, n) # validate the model through a K-fold CV
     print('Finished!')
     lap = time.time()-start
     h, rem = divmod(lap, 3600)
     m, s = divmod(rem, 60)
     print(f'Total execution time = {int(round(h))}:{int(round(m))}:{int(round(s))}')
 
-if __name__ == '__main__':
+def main():
     parser = argparse.ArgumentParser(prog='DPRED', description='Domain prediction and validation using HMM.')
     
     # mandatory
     parser.add_argument('--pfam', type=str, required=True, help='Pfam ID for domain prediction')
     parser.add_argument('-k', type=int, required=True, help='Number of folds for cross-validation')
     parser.add_argument('-l', type=str, required=True, help='Domain length range (upper incl.)')
```

### Comparing `DPRED-0.6/DPRED/msa.py` & `DPRED-0.7/DPRED/msa.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.6/DPRED/performance.py` & `DPRED-0.7/DPRED/performance.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.6/DPRED/validation.py` & `DPRED-0.7/DPRED/validation.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.6/DPRED.egg-info/PKG-INFO` & `DPRED-0.7/DPRED.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DPRED
-Version: 0.6
+Version: 0.7
 Summary: DPRED is a softwares package for HMM domain prediction and validation
 Home-page: https://github.com/dganci/DPRED
 Author: Daniele Ganci
 Author-email: daniele.ganci@studio.unibo.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DPRED-0.6/PKG-INFO` & `DPRED-0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DPRED
-Version: 0.6
+Version: 0.7
 Summary: DPRED is a softwares package for HMM domain prediction and validation
 Home-page: https://github.com/dganci/DPRED
 Author: Daniele Ganci
 Author-email: daniele.ganci@studio.unibo.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DPRED-0.6/setup.py` & `DPRED-0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='DPRED',
-    version='0.6',
+    version='0.7',
     packages=find_packages(include=['DPRED', 'DPRED.*']),
     install_requires=[
         'biopython',
         'requests',
         'numpy',
     ],
     entry_points={
```

