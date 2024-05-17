# Comparing `tmp/bigeda-0.0.7.tar.gz` & `tmp/bigeda-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigeda-0.0.7.tar", last modified: Thu May 16 21:19:10 2024, max compression
+gzip compressed data, was "bigeda-0.0.8.tar", last modified: Fri May 17 15:05:19 2024, max compression
```

## Comparing `bigeda-0.0.7.tar` & `bigeda-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 21:19:10.394977 bigeda-0.0.7/
-drwxrwxrwx   0        0        0        0 2024-05-16 21:19:10.352593 bigeda-0.0.7/BigEDA/
--rw-rw-rw-   0        0        0      783 2024-03-31 16:22:20.000000 bigeda-0.0.7/BigEDA/__init__.py
--rw-rw-rw-   0        0        0    26808 2024-05-13 16:49:56.000000 bigeda-0.0.7/BigEDA/descriptive.py
--rw-rw-rw-   0        0        0    78541 2024-05-13 23:16:09.000000 bigeda-0.0.7/BigEDA/plots.py
--rw-rw-rw-   0        0        0    11707 2024-04-14 01:24:57.000000 bigeda-0.0.7/BigEDA/preprocessing.py
-drwxrwxrwx   0        0        0        0 2024-05-16 21:19:10.392428 bigeda-0.0.7/BigEDA.egg-info/
--rw-rw-rw-   0        0        0      870 2024-05-16 21:19:10.000000 bigeda-0.0.7/BigEDA.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2024-05-16 21:19:10.000000 bigeda-0.0.7/BigEDA.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 21:19:10.000000 bigeda-0.0.7/BigEDA.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-16 21:19:10.000000 bigeda-0.0.7/BigEDA.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-16 21:19:10.000000 bigeda-0.0.7/BigEDA.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-12-09 15:06:56.000000 bigeda-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      870 2024-05-16 21:19:10.393459 bigeda-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      301 2023-12-09 16:15:51.000000 bigeda-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 21:19:10.394977 bigeda-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      838 2024-05-16 21:18:22.000000 bigeda-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:05:19.134920 bigeda-0.0.8/
+drwxrwxrwx   0        0        0        0 2024-05-17 15:05:19.092647 bigeda-0.0.8/BigEDA/
+-rw-rw-rw-   0        0        0      783 2024-03-31 16:22:20.000000 bigeda-0.0.8/BigEDA/__init__.py
+-rw-rw-rw-   0        0        0    26812 2024-05-17 15:04:09.000000 bigeda-0.0.8/BigEDA/descriptive.py
+-rw-rw-rw-   0        0        0    78541 2024-05-13 23:16:09.000000 bigeda-0.0.8/BigEDA/plots.py
+-rw-rw-rw-   0        0        0    11707 2024-04-14 01:24:57.000000 bigeda-0.0.8/BigEDA/preprocessing.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:05:19.131989 bigeda-0.0.8/BigEDA.egg-info/
+-rw-rw-rw-   0        0        0      870 2024-05-17 15:05:18.000000 bigeda-0.0.8/BigEDA.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2024-05-17 15:05:18.000000 bigeda-0.0.8/BigEDA.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 15:05:18.000000 bigeda-0.0.8/BigEDA.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-17 15:05:18.000000 bigeda-0.0.8/BigEDA.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-17 15:05:18.000000 bigeda-0.0.8/BigEDA.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-12-09 15:06:56.000000 bigeda-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      870 2024-05-17 15:05:19.133916 bigeda-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2023-12-09 16:15:51.000000 bigeda-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-17 15:05:19.134920 bigeda-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      838 2024-05-17 15:04:39.000000 bigeda-0.0.8/setup.py
```

### Comparing `bigeda-0.0.7/BigEDA/__init__.py` & `bigeda-0.0.8/BigEDA/__init__.py`

 * *Files identical despite different names*

### Comparing `bigeda-0.0.7/BigEDA/descriptive.py` & `bigeda-0.0.8/BigEDA/descriptive.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,15 +254,15 @@
                                 'cum_rel_freq' : np.cumsum(rel_counts)})
          
 
     return freq_df
 
 ######################################################################################################################
 
-def summary(df, auto_col=True, quant_col_names=[], cat_col_names=[]) :
+def summary(df, auto_col=False, quant_col_names=[], cat_col_names=[]) :
 
     if auto_col == True :
         quant_col_names = columns_names(df, types=[pl.Float64, pl.Int64])
         cat_col_names = columns_names(df, types=[pl.Boolean, pl.Utf8])
 
     elif auto_col == False : 
         # colnames debe ser un objeto tipo colnames = [list_quant_columns , list_cat_columns]
@@ -585,15 +585,15 @@
                                            'abs_freq' : counts, 
                                            'rel_freq' : np.round(rel_counts, 4)})     
     
     return contigency_table_df
 
 ######################################################################################################################
 
-def cov_matrix(df, auto_col=True, quant_col_names=None) :
+def cov_matrix(df, auto_col=False, quant_col_names=None) :
 
     if auto_col == True :
         quant_col_names = columns_names(df, types=[pl.Float64, pl.Int64])
 
     p_quant = len(quant_col_names)
     cov_matrix_ = np.zeros((p_quant,p_quant))
 
@@ -606,15 +606,15 @@
 
     cov_matrix_df = pd.DataFrame(cov_matrix_, columns=quant_col_names, index=quant_col_names)
     
     return cov_matrix_df
 
 ######################################################################################################################
 
-def corr_matrix(df, auto_col=True, quant_col_names=None, response=None, predictors=None, method='pearson') :
+def corr_matrix(df, auto_col=False, quant_col_names=None, response=None, predictors=None, method='pearson') :
 
     if response != None and predictors != None : 
 
         corr_list = []
         for col in predictors:
             corr_list.append(np.round(df.select(pl.corr(response, col, method=method)).to_numpy()[0][0], 2))
 
@@ -639,15 +639,15 @@
 
         corr_matrix_df = pd.DataFrame(corr_matrix_, columns=quant_col_names, index=quant_col_names) 
        
         return corr_matrix_df
 
 ######################################################################################################################
     
-def high_corr(df, upper, lower, auto_col=True, quant_col_names=None, method='pearson'):
+def high_corr(df, upper, lower, auto_col=False, quant_col_names=None, method='pearson'):
 
     if auto_col == True :
         quant_col_names = columns_names(df, types=[pl.Float64, pl.Int64])
 
     corr_dict = dict()
 
     for (col1,col2) in combinations(quant_col_names, 2) :
```

### Comparing `bigeda-0.0.7/BigEDA/plots.py` & `bigeda-0.0.8/BigEDA/plots.py`

 * *Files identical despite different names*

### Comparing `bigeda-0.0.7/BigEDA/preprocessing.py` & `bigeda-0.0.8/BigEDA/preprocessing.py`

 * *Files identical despite different names*

### Comparing `bigeda-0.0.7/BigEDA.egg-info/PKG-INFO` & `bigeda-0.0.8/BigEDA.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BigEDA
-Version: 0.0.7
+Version: 0.0.8
 Summary: This is a package to carry out Exploratory Data Analysis, allowing to work with Big Data.
 Home-page: https://github.com/FabioScielzoOrtiz/EDA_Package
 Author: Fabio Scielzo Ortiz
 Author-email: fabioscielzo98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bigeda-0.0.7/LICENSE` & `bigeda-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bigeda-0.0.7/PKG-INFO` & `bigeda-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BigEDA
-Version: 0.0.7
+Version: 0.0.8
 Summary: This is a package to carry out Exploratory Data Analysis, allowing to work with Big Data.
 Home-page: https://github.com/FabioScielzoOrtiz/EDA_Package
 Author: Fabio Scielzo Ortiz
 Author-email: fabioscielzo98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bigeda-0.0.7/setup.py` & `bigeda-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="BigEDA",
-    version="0.0.7",
+    version="0.0.8",
     author="Fabio Scielzo Ortiz",
     author_email="fabioscielzo98@gmail.com",
     description="This is a package to carry out Exploratory Data Analysis, allowing to work with Big Data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/FabioScielzoOrtiz/EDA_Package",  # add your project URL here
     packages=find_packages(),
```

