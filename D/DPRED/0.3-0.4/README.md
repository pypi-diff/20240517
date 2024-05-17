# Comparing `tmp/DPRED-0.3.tar.gz` & `tmp/DPRED-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DPRED-0.3.tar", last modified: Fri May 17 14:21:19 2024, max compression
+gzip compressed data, was "DPRED-0.4.tar", last modified: Fri May 17 14:50:36 2024, max compression
```

## Comparing `DPRED-0.3.tar` & `DPRED-0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 14:21:19.973487 DPRED-0.3/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 14:21:19.616439 DPRED-0.3/DPRED/
--rwxrwxrwx   0 root         (0) root         (0)       60 2024-05-17 12:33:46.000000 DPRED-0.3/DPRED/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1166 2024-05-16 17:32:28.000000 DPRED-0.3/DPRED/blast.py
--rwxrwxrwx   0 root         (0) root         (0)     5852 2024-05-16 17:32:19.000000 DPRED-0.3/DPRED/get_pdb_data.py
--rwxrwxrwx   0 root         (0) root         (0)     2376 2024-05-17 10:04:53.000000 DPRED-0.3/DPRED/get_pdb_files.py
--rwxrwxrwx   0 root         (0) root         (0)     1257 2024-05-16 17:32:23.000000 DPRED-0.3/DPRED/get_uniprot_data.py
--rwxrwxrwx   0 root         (0) root         (0)      737 2024-05-16 17:55:59.000000 DPRED-0.3/DPRED/hmm.py
--rwxrwxrwx   0 root         (0) root         (0)     2987 2024-05-17 13:15:58.000000 DPRED-0.3/DPRED/main.py
--rwxrwxrwx   0 root         (0) root         (0)     3420 2024-05-17 10:05:34.000000 DPRED-0.3/DPRED/msa.py
--rwxrwxrwx   0 root         (0) root         (0)     1572 2024-05-16 17:32:33.000000 DPRED-0.3/DPRED/performance.py
--rwxrwxrwx   0 root         (0) root         (0)      271 2024-05-16 17:32:42.000000 DPRED-0.3/DPRED/remove.py
--rwxrwxrwx   0 root         (0) root         (0)     7659 2024-05-16 17:58:57.000000 DPRED-0.3/DPRED/validation.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 14:21:19.834567 DPRED-0.3/DPRED.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      559 2024-05-17 14:21:18.000000 DPRED-0.3/DPRED.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      440 2024-05-17 14:21:19.000000 DPRED-0.3/DPRED.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-17 14:21:18.000000 DPRED-0.3/DPRED.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       42 2024-05-17 14:21:18.000000 DPRED-0.3/DPRED.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       33 2024-05-17 14:21:18.000000 DPRED-0.3/DPRED.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       12 2024-05-17 14:21:18.000000 DPRED-0.3/DPRED.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:08.000000 DPRED-0.3/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      559 2024-05-17 14:21:19.953199 DPRED-0.3/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:02.000000 DPRED-0.3/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-17 14:21:19.977030 DPRED-0.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      863 2024-05-17 14:21:07.000000 DPRED-0.3/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 14:21:19.910806 DPRED-0.3/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:27.000000 DPRED-0.3/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:35.000000 DPRED-0.3/tests/test_main.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 14:50:36.015210 DPRED-0.4/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 14:50:35.777219 DPRED-0.4/DPRED/
+-rwxrwxrwx   0 root         (0) root         (0)       60 2024-05-17 12:33:46.000000 DPRED-0.4/DPRED/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1166 2024-05-16 17:32:28.000000 DPRED-0.4/DPRED/blast.py
+-rwxrwxrwx   0 root         (0) root         (0)     5852 2024-05-16 17:32:19.000000 DPRED-0.4/DPRED/get_pdb_data.py
+-rwxrwxrwx   0 root         (0) root         (0)     2376 2024-05-17 10:04:53.000000 DPRED-0.4/DPRED/get_pdb_files.py
+-rwxrwxrwx   0 root         (0) root         (0)     1257 2024-05-16 17:32:23.000000 DPRED-0.4/DPRED/get_uniprot_data.py
+-rwxrwxrwx   0 root         (0) root         (0)      737 2024-05-16 17:55:59.000000 DPRED-0.4/DPRED/hmm.py
+-rwxrwxrwx   0 root         (0) root         (0)     2987 2024-05-17 13:15:58.000000 DPRED-0.4/DPRED/main.py
+-rwxrwxrwx   0 root         (0) root         (0)     3420 2024-05-17 10:05:34.000000 DPRED-0.4/DPRED/msa.py
+-rwxrwxrwx   0 root         (0) root         (0)     1572 2024-05-16 17:32:33.000000 DPRED-0.4/DPRED/performance.py
+-rwxrwxrwx   0 root         (0) root         (0)      271 2024-05-16 17:32:42.000000 DPRED-0.4/DPRED/remove.py
+-rwxrwxrwx   0 root         (0) root         (0)     7659 2024-05-16 17:58:57.000000 DPRED-0.4/DPRED/validation.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 14:50:35.933572 DPRED-0.4/DPRED.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      536 2024-05-17 14:50:35.000000 DPRED-0.4/DPRED.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      440 2024-05-17 14:50:35.000000 DPRED-0.4/DPRED.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-17 14:50:35.000000 DPRED-0.4/DPRED.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       42 2024-05-17 14:50:35.000000 DPRED-0.4/DPRED.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       25 2024-05-17 14:50:35.000000 DPRED-0.4/DPRED.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       12 2024-05-17 14:50:35.000000 DPRED-0.4/DPRED.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:08.000000 DPRED-0.4/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      536 2024-05-17 14:50:36.002681 DPRED-0.4/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:35:02.000000 DPRED-0.4/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-17 14:50:36.015210 DPRED-0.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      844 2024-05-17 14:50:26.000000 DPRED-0.4/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 14:50:35.974506 DPRED-0.4/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:27.000000 DPRED-0.4/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 12:34:35.000000 DPRED-0.4/tests/test_main.py
```

### Comparing `DPRED-0.3/DPRED/blast.py` & `DPRED-0.4/DPRED/blast.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.3/DPRED/get_pdb_data.py` & `DPRED-0.4/DPRED/get_pdb_data.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.3/DPRED/get_pdb_files.py` & `DPRED-0.4/DPRED/get_pdb_files.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.3/DPRED/get_uniprot_data.py` & `DPRED-0.4/DPRED/get_uniprot_data.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.3/DPRED/hmm.py` & `DPRED-0.4/DPRED/hmm.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.3/DPRED/main.py` & `DPRED-0.4/DPRED/main.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.3/DPRED/msa.py` & `DPRED-0.4/DPRED/msa.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.3/DPRED/performance.py` & `DPRED-0.4/DPRED/performance.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.3/DPRED/validation.py` & `DPRED-0.4/DPRED/validation.py`

 * *Files identical despite different names*

### Comparing `DPRED-0.3/DPRED.egg-info/PKG-INFO` & `DPRED-0.4/DPRED.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: DPRED
-Version: 0.3
+Version: 0.4
 Summary: DPRED is a softwares package for HMM domain prediction and validation
 Home-page: https://github.com/dganci/DPRED
 Author: Daniele Ganci
 Author-email: daniele.ganci@studio.unibo.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: biopython
 Requires-Dist: requests
 Requires-Dist: numpy
-Requires-Dist: logging
```

### Comparing `DPRED-0.3/PKG-INFO` & `DPRED-0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: DPRED
-Version: 0.3
+Version: 0.4
 Summary: DPRED is a softwares package for HMM domain prediction and validation
 Home-page: https://github.com/dganci/DPRED
 Author: Daniele Ganci
 Author-email: daniele.ganci@studio.unibo.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: biopython
 Requires-Dist: requests
 Requires-Dist: numpy
-Requires-Dist: logging
```

### Comparing `DPRED-0.3/setup.py` & `DPRED-0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='DPRED',
-    version='0.3',
+    version='0.4',
     packages=find_packages(),
     install_requires=[
         'biopython',
         'requests',
         'numpy',
-        'logging'
     ],
     entry_points={
         'console_scripts': [
             'dpred=DPRED.main:main',
         ],
     },
     author='Daniele Ganci',
```

