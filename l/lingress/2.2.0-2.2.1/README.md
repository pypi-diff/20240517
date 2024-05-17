# Comparing `tmp/lingress-2.2.0.tar.gz` & `tmp/lingress-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lingress-2.2.0.tar", last modified: Fri Apr 19 05:00:21 2024, max compression
+gzip compressed data, was "lingress-2.2.1.tar", last modified: Fri Apr 19 09:12:17 2024, max compression
```

## Comparing `lingress-2.2.0.tar` & `lingress-2.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 aeiwz      (501) staff       (20)        0 2024-04-19 05:00:21.979332 lingress-2.2.0/
--rw-r--r--   0 aeiwz      (501) staff       (20)     1066 2024-02-28 15:01:52.000000 lingress-2.2.0/LICENSE
--rw-r--r--   0 aeiwz      (501) staff       (20)     3165 2024-04-19 05:00:21.979253 lingress-2.2.0/PKG-INFO
--rw-r--r--   0 aeiwz      (501) staff       (20)     2220 2024-02-28 15:12:10.000000 lingress-2.2.0/README.rst
-drwxr-xr-x   0 aeiwz      (501) staff       (20)        0 2024-04-19 05:00:21.977167 lingress-2.2.0/lingress/
--rw-r--r--   0 aeiwz      (501) staff       (20)      119 2024-04-18 08:39:34.000000 lingress-2.2.0/lingress/__init__.py
--rw-r--r--   0 aeiwz      (501) staff       (20)    42166 2024-03-29 03:04:47.000000 lingress-2.2.0/lingress/lingress.py
--rw-r--r--   0 aeiwz      (501) staff       (20)     5919 2024-04-19 04:58:25.000000 lingress-2.2.0/lingress/utility.py
-drwxr-xr-x   0 aeiwz      (501) staff       (20)        0 2024-04-19 05:00:21.978899 lingress-2.2.0/lingress.egg-info/
--rw-r--r--   0 aeiwz      (501) staff       (20)     3165 2024-04-19 05:00:21.000000 lingress-2.2.0/lingress.egg-info/PKG-INFO
--rw-r--r--   0 aeiwz      (501) staff       (20)      258 2024-04-19 05:00:21.000000 lingress-2.2.0/lingress.egg-info/SOURCES.txt
--rw-r--r--   0 aeiwz      (501) staff       (20)        1 2024-04-19 05:00:21.000000 lingress-2.2.0/lingress.egg-info/dependency_links.txt
--rw-r--r--   0 aeiwz      (501) staff       (20)       90 2024-04-19 05:00:21.000000 lingress-2.2.0/lingress.egg-info/requires.txt
--rw-r--r--   0 aeiwz      (501) staff       (20)        9 2024-04-19 05:00:21.000000 lingress-2.2.0/lingress.egg-info/top_level.txt
--rw-r--r--   0 aeiwz      (501) staff       (20)       80 2024-04-19 05:00:21.979777 lingress-2.2.0/setup.cfg
--rw-r--r--   0 aeiwz      (501) staff       (20)     1378 2024-04-19 04:59:18.000000 lingress-2.2.0/setup.py
+drwxr-xr-x   0 aeiwz      (501) staff       (20)        0 2024-04-19 09:12:17.657855 lingress-2.2.1/
+-rw-r--r--   0 aeiwz      (501) staff       (20)     1066 2024-02-28 15:01:52.000000 lingress-2.2.1/LICENSE
+-rw-r--r--   0 aeiwz      (501) staff       (20)     3165 2024-04-19 09:12:17.657792 lingress-2.2.1/PKG-INFO
+-rw-r--r--   0 aeiwz      (501) staff       (20)     2220 2024-02-28 15:12:10.000000 lingress-2.2.1/README.rst
+drwxr-xr-x   0 aeiwz      (501) staff       (20)        0 2024-04-19 09:12:17.656543 lingress-2.2.1/lingress/
+-rw-r--r--   0 aeiwz      (501) staff       (20)      119 2024-04-18 08:39:34.000000 lingress-2.2.1/lingress/__init__.py
+-rw-r--r--   0 aeiwz      (501) staff       (20)    42166 2024-03-29 03:04:47.000000 lingress-2.2.1/lingress/lingress.py
+-rw-r--r--   0 aeiwz      (501) staff       (20)     5899 2024-04-19 09:11:37.000000 lingress-2.2.1/lingress/utility.py
+drwxr-xr-x   0 aeiwz      (501) staff       (20)        0 2024-04-19 09:12:17.657559 lingress-2.2.1/lingress.egg-info/
+-rw-r--r--   0 aeiwz      (501) staff       (20)     3165 2024-04-19 09:12:17.000000 lingress-2.2.1/lingress.egg-info/PKG-INFO
+-rw-r--r--   0 aeiwz      (501) staff       (20)      258 2024-04-19 09:12:17.000000 lingress-2.2.1/lingress.egg-info/SOURCES.txt
+-rw-r--r--   0 aeiwz      (501) staff       (20)        1 2024-04-19 09:12:17.000000 lingress-2.2.1/lingress.egg-info/dependency_links.txt
+-rw-r--r--   0 aeiwz      (501) staff       (20)       90 2024-04-19 09:12:17.000000 lingress-2.2.1/lingress.egg-info/requires.txt
+-rw-r--r--   0 aeiwz      (501) staff       (20)        9 2024-04-19 09:12:17.000000 lingress-2.2.1/lingress.egg-info/top_level.txt
+-rw-r--r--   0 aeiwz      (501) staff       (20)       80 2024-04-19 09:12:17.658051 lingress-2.2.1/setup.cfg
+-rw-r--r--   0 aeiwz      (501) staff       (20)     1378 2024-04-19 09:11:20.000000 lingress-2.2.1/setup.py
```

### Comparing `lingress-2.2.0/LICENSE` & `lingress-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lingress-2.2.0/PKG-INFO` & `lingress-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lingress
-Version: 2.2.0
+Version: 2.2.1
 Summary: Metabolomics data analysis with univariate (linear regression) and visualization tools.
 Home-page: https://github.com/aeiwz/lingress.git
-Download-URL: https://github.com/aeiwz/lingress/archive/refs/tags/v2.2.0.tar.gz
+Download-URL: https://github.com/aeiwz/lingress/archive/refs/tags/v2.2.1.tar.gz
 Author: aeiwz
 Author-email: theerayut_aeiw_123@hotmail.com
 License: MIT
 Keywords: Omics,Chemometrics,Visualization,Data Analysis,Univariate,Linear Regression
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `lingress-2.2.0/README.rst` & `lingress-2.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `lingress-2.2.0/lingress/lingress.py` & `lingress-2.2.1/lingress/lingress.py`

 * *Files identical despite different names*

### Comparing `lingress-2.2.0/lingress/utility.py` & `lingress-2.2.1/lingress/utility.py`

 * *Files 6% similar despite different names*

```diff
@@ -124,15 +124,15 @@
                 color_map = color_map
 
         
 
         #plot spectra
         fig = go.Figure()
         for i in df_spectra.index:
-            fig.add_trace(go.Scatter(x=ppm, y=df_spectra.loc[i,:], mode='lines', name=i, line=dict(color=color_map[i], width=line_width)))
+            fig.add_trace(go.Scatter(x=ppm, y=df_spectra.loc[i,:], mode='lines', name=i, line=dict(width=line_width)))
 
         fig.update_layout(
             autosize=False,
             width=fig_width,
             height=fig_height,
             margin=dict(
                 l=50,
```

### Comparing `lingress-2.2.0/lingress.egg-info/PKG-INFO` & `lingress-2.2.1/lingress.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lingress
-Version: 2.2.0
+Version: 2.2.1
 Summary: Metabolomics data analysis with univariate (linear regression) and visualization tools.
 Home-page: https://github.com/aeiwz/lingress.git
-Download-URL: https://github.com/aeiwz/lingress/archive/refs/tags/v2.2.0.tar.gz
+Download-URL: https://github.com/aeiwz/lingress/archive/refs/tags/v2.2.1.tar.gz
 Author: aeiwz
 Author-email: theerayut_aeiw_123@hotmail.com
 License: MIT
 Keywords: Omics,Chemometrics,Visualization,Data Analysis,Univariate,Linear Regression
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `lingress-2.2.0/setup.py` & `lingress-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 DESCRIPTION = '\n\n'.join(LOAD_TEXT(_) for _ in [
     'README.rst'
 ])
 
 setup(
   name = 'lingress',      
   packages = ['lingress'], 
-  version = '2.2.0',  
+  version = '2.2.1',  
   license='MIT', 
   description = 'Metabolomics data analysis with univariate (linear regression) and visualization tools.',
   long_description=DESCRIPTION,
   author = 'aeiwz',                 
   author_email = 'theerayut_aeiw_123@hotmail.com',     
   url = 'https://github.com/aeiwz/lingress.git',  
-  download_url = 'https://github.com/aeiwz/lingress/archive/refs/tags/v2.2.0.tar.gz',  
+  download_url = 'https://github.com/aeiwz/lingress/archive/refs/tags/v2.2.1.tar.gz',  
   keywords = ['Omics', 'Chemometrics', 'Visualization', 'Data Analysis', 'Univariate', 'Linear Regression'],
   install_requires=[            
           'scikit-learn',
           'pandas',
           'numpy',
           'matplotlib',
           'seaborn',
```

