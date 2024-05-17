# Comparing `tmp/mc_shapley-0.0.5.tar.gz` & `tmp/mc_shapley-0.0.6.tar.gz`

## Comparing `mc_shapley-0.0.5.tar` & `mc_shapley-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 mc_shapley-0.0.5/src/mc_shapley/__init__.py
--rw-r--r--   0        0        0    15303 2020-02-02 00:00:00.000000 mc_shapley-0.0.5/src/mc_shapley/mc_shapley.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 mc_shapley-0.0.5/src/mc_shapley/temporal_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mc_shapley-0.0.5/tests_mc_shapley/__init__.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mc_shapley-0.0.5/tests_mc_shapley/temp_test_file2.csv
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 mc_shapley-0.0.5/tests_mc_shapley/temp_test_file3.csv
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 mc_shapley-0.0.5/tests_mc_shapley/test_file1.txt
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 mc_shapley-0.0.5/tests_mc_shapley/test_file2.txt
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 mc_shapley-0.0.5/tests_mc_shapley/test_file3.csv
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 mc_shapley-0.0.5/tests_mc_shapley/test_file4.csv
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 mc_shapley-0.0.5/tests_mc_shapley/test_file5.csv
--rw-r--r--   0        0        0  2347336 2020-02-02 00:00:00.000000 mc_shapley-0.0.5/tests_mc_shapley/test_file_park.csv
--rw-r--r--   0        0        0     9447 2020-02-02 00:00:00.000000 mc_shapley-0.0.5/tests_mc_shapley/test_mc_shapley.py
--rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 mc_shapley-0.0.5/tutorials/short_tutorial.md
--rw-r--r--   0        0        0   373728 2020-02-02 00:00:00.000000 mc_shapley-0.0.5/tutorials/references/Quantifying Algorithmic Improvements over Time.pdf
--rw-r--r--   0        0        0  1690563 2020-02-02 00:00:00.000000 mc_shapley-0.0.5/tutorials/references/Using the Shapley Value to Analyze Algorithm Portfolios.pdf
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 mc_shapley-0.0.5/tutorials/references/references.md
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mc_shapley-0.0.5/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mc_shapley-0.0.5/LICENSE
--rw-r--r--   0        0        0     7288 2020-02-02 00:00:00.000000 mc_shapley-0.0.5/README.md
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 mc_shapley-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     8187 2020-02-02 00:00:00.000000 mc_shapley-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 mc_shapley-0.0.6/src/mc_shapley/__init__.py
+-rw-r--r--   0        0        0    15303 2020-02-02 00:00:00.000000 mc_shapley-0.0.6/src/mc_shapley/mc_shapley.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 mc_shapley-0.0.6/src/mc_shapley/temporal_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mc_shapley-0.0.6/tests_mc_shapley/__init__.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mc_shapley-0.0.6/tests_mc_shapley/temp_test_file2.csv
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 mc_shapley-0.0.6/tests_mc_shapley/temp_test_file3.csv
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 mc_shapley-0.0.6/tests_mc_shapley/test_file1.txt
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 mc_shapley-0.0.6/tests_mc_shapley/test_file2.txt
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 mc_shapley-0.0.6/tests_mc_shapley/test_file3.csv
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 mc_shapley-0.0.6/tests_mc_shapley/test_file4.csv
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 mc_shapley-0.0.6/tests_mc_shapley/test_file5.csv
+-rw-r--r--   0        0        0  2347336 2020-02-02 00:00:00.000000 mc_shapley-0.0.6/tests_mc_shapley/test_file_park.csv
+-rw-r--r--   0        0        0     9447 2020-02-02 00:00:00.000000 mc_shapley-0.0.6/tests_mc_shapley/test_mc_shapley.py
+-rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 mc_shapley-0.0.6/tutorials/short_tutorial.md
+-rw-r--r--   0        0        0   373728 2020-02-02 00:00:00.000000 mc_shapley-0.0.6/tutorials/references/Quantifying Algorithmic Improvements over Time.pdf
+-rw-r--r--   0        0        0  1690563 2020-02-02 00:00:00.000000 mc_shapley-0.0.6/tutorials/references/Using the Shapley Value to Analyze Algorithm Portfolios.pdf
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 mc_shapley-0.0.6/tutorials/references/references.md
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mc_shapley-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mc_shapley-0.0.6/LICENSE
+-rw-r--r--   0        0        0     7288 2020-02-02 00:00:00.000000 mc_shapley-0.0.6/README.md
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mc_shapley-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     8168 2020-02-02 00:00:00.000000 mc_shapley-0.0.6/PKG-INFO
```

### Comparing `mc_shapley-0.0.5/src/mc_shapley/mc_shapley.py` & `mc_shapley-0.0.6/src/mc_shapley/mc_shapley.py`

 * *Files identical despite different names*

### Comparing `mc_shapley-0.0.5/src/mc_shapley/temporal_utils.py` & `mc_shapley-0.0.6/src/mc_shapley/temporal_utils.py`

 * *Files identical despite different names*

### Comparing `mc_shapley-0.0.5/tests_mc_shapley/test_file_park.csv` & `mc_shapley-0.0.6/tests_mc_shapley/test_file_park.csv`

 * *Files identical despite different names*

### Comparing `mc_shapley-0.0.5/tests_mc_shapley/test_mc_shapley.py` & `mc_shapley-0.0.6/tests_mc_shapley/test_mc_shapley.py`

 * *Files identical despite different names*

### Comparing `mc_shapley-0.0.5/tutorials/short_tutorial.md` & `mc_shapley-0.0.6/tutorials/short_tutorial.md`

 * *Files identical despite different names*

### Comparing `mc_shapley-0.0.5/tutorials/references/Quantifying Algorithmic Improvements over Time.pdf` & `mc_shapley-0.0.6/tutorials/references/Quantifying Algorithmic Improvements over Time.pdf`

 * *Files identical despite different names*

### Comparing `mc_shapley-0.0.5/tutorials/references/Using the Shapley Value to Analyze Algorithm Portfolios.pdf` & `mc_shapley-0.0.6/tutorials/references/Using the Shapley Value to Analyze Algorithm Portfolios.pdf`

 * *Files identical despite different names*

### Comparing `mc_shapley-0.0.5/tutorials/references/references.md` & `mc_shapley-0.0.6/tutorials/references/references.md`

 * *Files identical despite different names*

### Comparing `mc_shapley-0.0.5/LICENSE` & `mc_shapley-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mc_shapley-0.0.5/README.md` & `mc_shapley-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mc_shapley-0.0.5/pyproject.toml` & `mc_shapley-0.0.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
-name = "mc_shapley"
-version = "0.0.5"
+name = "mc-shapley"
+version = "0.0.6"
 authors = [
   { name="Nikita A. Gallegos", email="nikitaagallegos@gmail.com" },
 ]
 description = "A package that is used to run Shapley value variations useful for research on CSV file. The package includes MC-Net Shapley which runs in polynomial time and Temporal Shapley which gives favor to coalition members on both performance and precedents. Both rely on certain assumptions, to learn more check the references."
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research"
 ]
 dependencies = [
   'csv',
   'scipy',
-  'numpy',
-  'copy'
+  'numpy'
 ]
 
 [project.optional-dependencies]
 tests = [
   'pytest'
 ]
```

### Comparing `mc_shapley-0.0.5/PKG-INFO` & `mc_shapley-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.3
-Name: mc_shapley
-Version: 0.0.5
+Name: mc-shapley
+Version: 0.0.6
 Summary: A package that is used to run Shapley value variations useful for research on CSV file. The package includes MC-Net Shapley which runs in polynomial time and Temporal Shapley which gives favor to coalition members on both performance and precedents. Both rely on certain assumptions, to learn more check the references.
 Project-URL: Homepage, https://github.com/uwyo-mallet/Shapley-CVS--Gallegos-
 Project-URL: Issues, https://github.com/uwyo-mallet/Shapley-CVS--Gallegos-/issues
 Author-email: "Nikita A. Gallegos" <nikitaagallegos@gmail.com>
 License-File: LICENSE
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Requires-Dist: copy
+Requires-Python: >=3.10
 Requires-Dist: csv
 Requires-Dist: numpy
 Requires-Dist: scipy
 Provides-Extra: tests
 Requires-Dist: pytest; extra == 'tests'
 Description-Content-Type: text/markdown
```

