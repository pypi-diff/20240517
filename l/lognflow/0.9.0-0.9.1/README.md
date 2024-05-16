# Comparing `tmp/lognflow-0.9.0.tar.gz` & `tmp/lognflow-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lognflow-0.9.0.tar", last modified: Sat Aug 19 13:45:12 2023, max compression
+gzip compressed data, was "lognflow-0.9.1.tar", last modified: Wed Aug 23 12:50:07 2023, max compression
```

## Comparing `lognflow-0.9.0.tar` & `lognflow-0.9.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 13:45:12.423088 lognflow-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-19 13:45:02.000000 lognflow-0.9.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-08-19 13:45:02.000000 lognflow-0.9.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-08-19 13:45:02.000000 lognflow-0.9.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-08-19 13:45:02.000000 lognflow-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-19 13:45:02.000000 lognflow-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-08-19 13:45:12.423088 lognflow-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-08-19 13:45:02.000000 lognflow-0.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 13:45:12.419088 lognflow-0.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-19 13:45:02.000000 lognflow-0.9.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-19 13:45:02.000000 lognflow-0.9.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-08-19 13:45:02.000000 lognflow-0.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-19 13:45:02.000000 lognflow-0.9.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-19 13:45:02.000000 lognflow-0.9.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-19 13:45:02.000000 lognflow-0.9.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-19 13:45:02.000000 lognflow-0.9.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-19 13:45:02.000000 lognflow-0.9.0/docs/lognflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-19 13:45:02.000000 lognflow-0.9.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-19 13:45:02.000000 lognflow-0.9.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-19 13:45:02.000000 lognflow-0.9.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 13:45:12.419088 lognflow-0.9.0/lognflow/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-08-19 13:45:02.000000 lognflow-0.9.0/lognflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63969 2023-08-19 13:45:02.000000 lognflow-0.9.0/lognflow/lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    13438 2023-08-19 13:45:02.000000 lognflow-0.9.0/lognflow/logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-08-19 13:45:02.000000 lognflow-0.9.0/lognflow/plt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-08-19 13:45:02.000000 lognflow-0.9.0/lognflow/printprogress.py
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-08-19 13:45:02.000000 lognflow-0.9.0/lognflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 13:45:12.423088 lognflow-0.9.0/lognflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-08-19 13:45:12.000000 lognflow-0.9.0/lognflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-08-19 13:45:12.000000 lognflow-0.9.0/lognflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-19 13:45:12.000000 lognflow-0.9.0/lognflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-19 13:45:12.000000 lognflow-0.9.0/lognflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-19 13:45:12.000000 lognflow-0.9.0/lognflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-19 13:45:12.000000 lognflow-0.9.0/lognflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-19 13:45:12.423088 lognflow-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-19 13:45:02.000000 lognflow-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-19 13:45:12.423088 lognflow-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-19 13:45:02.000000 lognflow-0.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-08-19 13:45:02.000000 lognflow-0.9.0/tests/test_lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-08-19 13:45:02.000000 lognflow-0.9.0/tests/test_logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-08-19 13:45:02.000000 lognflow-0.9.0/tests/test_printprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 12:50:07.627364 lognflow-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-23 12:49:41.000000 lognflow-0.9.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-08-23 12:49:41.000000 lognflow-0.9.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-08-23 12:49:41.000000 lognflow-0.9.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-08-23 12:49:41.000000 lognflow-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-23 12:49:41.000000 lognflow-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-08-23 12:50:07.627364 lognflow-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-08-23 12:49:41.000000 lognflow-0.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 12:50:07.623364 lognflow-0.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-23 12:49:41.000000 lognflow-0.9.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-23 12:49:41.000000 lognflow-0.9.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-08-23 12:49:41.000000 lognflow-0.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-23 12:49:41.000000 lognflow-0.9.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-23 12:49:41.000000 lognflow-0.9.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-23 12:49:41.000000 lognflow-0.9.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-23 12:49:41.000000 lognflow-0.9.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-23 12:49:41.000000 lognflow-0.9.1/docs/lognflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-23 12:49:41.000000 lognflow-0.9.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-23 12:49:41.000000 lognflow-0.9.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-23 12:49:41.000000 lognflow-0.9.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 12:50:07.623364 lognflow-0.9.1/lognflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-08-23 12:49:41.000000 lognflow-0.9.1/lognflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63971 2023-08-23 12:49:41.000000 lognflow-0.9.1/lognflow/lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-08-23 12:49:41.000000 lognflow-0.9.1/lognflow/logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-08-23 12:49:41.000000 lognflow-0.9.1/lognflow/plt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-08-23 12:49:41.000000 lognflow-0.9.1/lognflow/printprogress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-08-23 12:49:41.000000 lognflow-0.9.1/lognflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 12:50:07.627364 lognflow-0.9.1/lognflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-08-23 12:50:07.000000 lognflow-0.9.1/lognflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-08-23 12:50:07.000000 lognflow-0.9.1/lognflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-23 12:50:07.000000 lognflow-0.9.1/lognflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-23 12:50:07.000000 lognflow-0.9.1/lognflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-23 12:50:07.000000 lognflow-0.9.1/lognflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-23 12:50:07.000000 lognflow-0.9.1/lognflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-23 12:50:07.627364 lognflow-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-23 12:49:41.000000 lognflow-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 12:50:07.627364 lognflow-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-23 12:49:41.000000 lognflow-0.9.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-08-23 12:49:41.000000 lognflow-0.9.1/tests/test_lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-08-23 12:49:41.000000 lognflow-0.9.1/tests/test_logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-08-23 12:49:41.000000 lognflow-0.9.1/tests/test_printprogress.py
```

### Comparing `lognflow-0.9.0/CONTRIBUTING.rst` & `lognflow-0.9.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.9.0/HISTORY.rst` & `lognflow-0.9.1/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -154,8 +154,13 @@
 
 0.9.0 (2023-08-09)
 -----------------
 * copy() is now possible from a file or a variable name into another
 * default suffix in get_flist is *
 * logviewer.get_stack_of_files is only useful for reading data.
 * more tests are added.
-* moved multichannel_to_frame to utils
+* moved multichannel_to_frame to utils
+
+0.9.1 (2023-09-01)
+-----------------
+* bug removed from plt_utils numbers_as_images_4D.
+* bug removed from printprogress when number of steps is very low.
```

### Comparing `lognflow-0.9.0/LICENSE` & `lognflow-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lognflow-0.9.0/PKG-INFO` & `lognflow-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.9.0
+Version: 0.9.1
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -248,7 +248,12 @@
 0.9.0 (2023-08-09)
 -----------------
 * copy() is now possible from a file or a variable name into another
 * default suffix in get_flist is *
 * logviewer.get_stack_of_files is only useful for reading data.
 * more tests are added.
 * moved multichannel_to_frame to utils
+
+0.9.1 (2023-09-01)
+-----------------
+* bug removed from plt_utils numbers_as_images_4D.
+* bug removed from printprogress when number of steps is very low.
```

### Comparing `lognflow-0.9.0/README.rst` & `lognflow-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.9.0/docs/Makefile` & `lognflow-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lognflow-0.9.0/docs/conf.py` & `lognflow-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.9.0/docs/installation.rst` & `lognflow-0.9.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.9.0/docs/make.bat` & `lognflow-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lognflow-0.9.0/lognflow/lognflow.py` & `lognflow-0.9.1/lognflow/lognflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1469,14 +1469,33 @@
 
     def flush_all(self):
         for log_name in list(self._loggers_dict):
             self.log_text_flush(log_name, flush = True)
         for parameter_name in list(self._vars_dict):
             self.log_var_flush(parameter_name)
 
+    def save(self, parameter_name: str, 
+                   parameter_value,
+                   suffix = None,
+                   mat_field = None,
+                   time_tag: bool = None):
+        return self.log_single(parameter_name = parameter_name, 
+                               parameter_value = parameter_value,
+                               suffix = suffix,
+                               mat_field = mat_field,
+                               time_tag = time_tag)
+
+    def savez(self, parameter_name: str, 
+                    parameter_value,
+                    time_tag: bool = None):
+        return self.log_single(parameter_name = parameter_name, 
+                               parameter_value = parameter_value,
+                               suffix = 'npz',
+                               time_tag = time_tag)
+
     def __call__(self, *args, **kwargs):
         """calling the object
             In the case of the following code::
                 logger = lognflow()
                 logger('Hello lognflow')
             The text (str(...)) will be passed to the main log text file.
         """
@@ -1488,27 +1507,8 @@
         except:
             pass
         
     def __repr__(self):
         return f'{self.log_dir}'
 
     def __bool__(self):
-        return self.log_dir.is_dir()
-
-    def save(self, parameter_name: str, 
-                   parameter_value,
-                   suffix = None,
-                   mat_field = None,
-                   time_tag: bool = None):
-        return self.log_single(parameter_name = parameter_name, 
-                               parameter_value = parameter_value,
-                               suffix = suffix,
-                               mat_field = mat_field,
-                               time_tag = time_tag)
-
-    def savez(self, parameter_name: str, 
-                   parameter_value,
-                   time_tag: bool = None):
-        return self.log_single(parameter_name = parameter_name, 
-                               parameter_value = parameter_value,
-                               suffix = 'npz',
-                               time_tag = time_tag)
+        return self.log_dir.is_dir()
```

### Comparing `lognflow-0.9.0/lognflow/logviewer.py` & `lognflow-0.9.1/lognflow/logviewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,14 +273,18 @@
             ----------
            
                 It returns a list of data in all files or a numpy array if 
                 concatenation of all is possible.
         """
         if not flist:
             flist = self.get_flist(var_name, suffix)
+        else:
+            flist = list(flist)
+            assert pathlib.Path(flist[0]).is_file(), \
+                f'File not found: {flist[0]}. You can use logviewer get_flist'
         
         if flist:
             n_files = len(flist)
             if(read_func is None):
                 try:
                     fdata = np.load(flist[0])
                     read_func = np.load
```

### Comparing `lognflow-0.9.0/lognflow/plt_utils.py` & `lognflow-0.9.1/lognflow/plt_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from .printprogress import printprogress
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 import numpy as np
 import matplotlib.pyplot as plt
 
 def plt_colorbar(mappable):
     """ Add colobar to the current axis 
         This is specially useful in plt.subplots
@@ -37,18 +38,20 @@
     """ from https://www.icare.univ-lille.fr/how-to-
                     convert-a-matplotlib-figure-to-a-numpy-array-or-a-pil-image/
     """
     fig.canvas.draw()
     w,h = fig.canvas.get_width_height()
     buf = np.frombuffer(fig.canvas.tostring_argb(), dtype=np.ubyte)
     buf.shape = (w, h, 4)
-    buf = np.roll (buf, 3, axis = 2)
-    return buf
+    return buf.sum(2)
 
-def numbers_as_images_3D(dataset_shape: tuple, fontsize, verbose = False):
+def numbers_as_images_3D(data3D_shape: tuple[int, int, int],
+                         fontsize: int, 
+                         text_loc: tuple[int, int] = None,
+                         verbose: bool = True):
     """ Numbers3D
     This function generates a 4D dataset of images with shape
     (n_x, n_r, n_c) where in each image the value "x" is written as a text
     that fills the image. As such, later when working with such a dataset you can
     look at the image and know which index it had before you use it.
     
     Follow this recipe to make good images:
@@ -57,40 +60,45 @@
     2- find fontsize that is the largest and still fits
     3- Increase n_x to desired size.
     
     You can provide a logs_root, log_dir or simply select a directory to save the
     output 3D array.
     
     """
-    n_x, n_r, n_c = dataset_shape
-    dataset = np.zeros(dataset_shape)    
+    n_x, n_r, n_c = data3D_shape
+    
+    if text_loc is None:
+        text_loc = (n_r//2 - fontsize, n_c//2 - fontsize)
+    
+    dataset = np.zeros(data3D_shape)    
     txt_width = int(np.log(n_x)/np.log(n_x)) + 1
     number_text_base = '{ind_x:0{width}}}'
     if(verbose):
         pBar = printprogress(n_x)
     for ind_x in range(n_x):
         mat = np.ones((n_r, n_c))
         number_text = number_text_base.format(ind_x = ind_x, 
                                               width = txt_width)
-        fig = plt.figure(figsize = (1, 1))
+        fig = plt.figure(figsize = (n_rr, n_cc), dpi = n_rc)
         ax = fig.add_subplot(111)
         ax.imshow(mat, cmap = 'gray', vmin = 0, vmax = 1)
-        ax.text(mat.shape[0]//2 - fontsize, mat.shape[1]//2 ,
+        ax.text(text_loc[0], text_loc[1],
                 number_text, fontsize = fontsize)
         ax.axis('off')
         buf = pltfig_to_numpy(fig)
         plt.close()
-        buf2 = buf[::buf.shape[0]//n_r, ::buf.shape[1]//n_c, :3].mean(2)
-        buf2 = buf2[:n_r, :n_c]
-        dataset[ind_x] = buf2.copy()
+        dataset[ind_x] = buf.copy()
         if(verbose):
             pBar()
     return dataset
 
-def numbers_as_images_4D(dataset_shape: tuple, fontsize, verbose = False):
+def numbers_as_images_4D(data4D_shape: tuple[int, int, int, int],
+                         fontsize: int, 
+                         text_loc: tuple[int, int] = None,
+                         verbose: bool = True):
     """ Numbers4D
     This function generates a 4D dataset of images with shape
     (n_x, n_y, n_r, n_c) where in each image the value "x, y" is written as a text
     that fills the image. As such, later when working with such a dataset you can
     look at the image and know which index it had before you use it.
     
     Follow this recipe to make good images:
@@ -98,35 +106,42 @@
     1- set n_x, n_y to 10, Set the desired n_r, n_c and width. 
     2- try fontsize that is the largest
     3- Increase n_x and n_y to desired size.
     
     You can provide a logs_root, log_dir or simply select a directory to save the
     output 4D array.
     
+    :param text__loc:
+        text_loc should be a tuple of the location of bottom left corner of the
+        text in the image.
+    
     """
-    n_x, n_y, n_r, n_c = dataset_shape
+    n_x, n_y, n_r, n_c = data4D_shape
+
+    if text_loc is None:
+        text_loc = (n_r//2 - fontsize, n_c//2 - fontsize)
+    
     dataset = np.zeros((n_x, n_y, n_r, n_c))    
     txt_width = int(np.log(np.maximum(n_x, n_y))
-                    /np.log(np.maximum(n_x, n_y))) + 1
+                    / np.log(np.maximum(n_x, n_y))) + 1
     number_text_base = '{ind_x:0{width}}, {ind_y:0{width}}'
     if(verbose):
         pBar = printprogress(n_x * n_y)
     for ind_x in range(n_x):
         for ind_y in range(n_y):
             mat = np.ones((n_r, n_c))
-            number_text = number_text_base.format(ind_x = ind_x, 
-                                                  ind_y = ind_y,
-                                                  width = txt_width)
-            fig = plt.figure(figsize = (1, 1))
+            number_text = number_text_base.format(
+                ind_x = ind_x, ind_y = ind_y, width = txt_width)
+            n_rc = np.minimum(n_r, n_c)
+            n_rr = n_r / n_rc
+            n_cc = n_c / n_rc
+            fig = plt.figure(figsize = (n_rr, n_cc), dpi = n_rc)
             ax = fig.add_subplot(111)
             ax.imshow(mat, cmap = 'gray', vmin = 0, vmax = 1)
-            ax.text(mat.shape[0]//2 - fontsize, mat.shape[1]//2 ,
-                    number_text, fontsize = fontsize)
+            ax.text(text_loc[0], text_loc[1], number_text, fontsize = fontsize)
             ax.axis('off')
             buf = pltfig_to_numpy(fig)
             plt.close()
-            buf2 = buf[::buf.shape[0]//n_r, ::buf.shape[1]//n_c, :3].mean(2)
-            buf2 = buf2[:n_r, :n_c]
-            dataset[ind_x, ind_y] = buf2.copy()
+            dataset[ind_x, ind_y] = buf.copy()
             if(verbose):
                 pBar()
     return dataset
```

### Comparing `lognflow-0.9.0/lognflow/printprogress.py` & `lognflow-0.9.1/lognflow/printprogress.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,16 @@
                 more options to come
         """
         assert method in ['linear', 'linear_robust']
         self.print_function_kwargs = print_function_kwargs
         self.method = method
         self.in_print_function = print_function
         if(n_steps != int(n_steps)):
-            self._print_func('textProgBar takes integers no less than 2 ')
+            self._print_func(
+                r'printprogress takes integers no less than 2 as n_steps.')
             n_steps = int(n_steps)
         if(n_steps<2):
             n_steps = 2
         if (title is None):
             title = f'Progress for {n_steps} steps'
         self.FLAG_ended = False
         self.FLAG_warning = False
@@ -71,14 +72,15 @@
         self._print_func('/', end='')
         self._print_func(' '*int((self.numTicks - len(title))/2), end='')
         self._print_func(title, end='')
         self._print_func(' '*int(ceil((self.numTicks-len(title))/2)-1), end='')
         self._print_func(' \\')
         
         self._print_func(' ', end = '')
+        self.len_prog_text = 0
     
     def _print_func(self, text, end='\n'):
         if (self.in_print_function is not None):
             if (self.in_print_function == print):
                 print(text, end = end, flush = True)
             else:
                 self.in_print_function(text, end = end,
@@ -89,56 +91,63 @@
             passedTime = time() - self.startTime
             remTimeS = passedTime * ( self.n_steps / self.ck - 1)
         
         return remTimeS
     
     def __call__(self, ck=1):
         """ ticking the progress bar
-            just call the object and the progress bar moves one ahead when ready.
+            just call the object and the progress bar moves ck steps
+            ahead when ready.
             
             output
             ~~~~~~
             :param ETA:
                 the remaining time in seconds will be provided at the output
         """
         remTimeS = 0
         if(self.FLAG_ended):
             if(not self.FLAG_warning):
                 self.FLAG_warning = True
-                self._print_func('-' * self.numTicks)
+                self._print_func('-' * (self.numTicks + 2))
         else:
             self.ck += ck
             if(self.ck <= self.n_steps):
                 remTimeS = self._calc_ETA() # useful when print_function is None
-                cProg = int(self.numTicks*self.ck/(self.n_steps-1)/3)    
+                cProg = int(self.numTicks*self.ck/(self.n_steps-1)/3)
                 #3: because 3 charachters are used
                 while((self.prog < cProg) & (not self.FLAG_ended)):
                     self.prog += 1
                     remTimeS = self._calc_ETA()
                     if(remTimeS>356400): # less than 99d and more than 99h
                         progStr = "%02d" % int(ceil(remTimeS/86400))
                         self._print_func(progStr, end='')
                         self._print_func('d', end='')
+                        self.len_prog_text += 3
                     elif(remTimeS>5940): # less than 99h and more than 99m
                         progStr = "%02d" % int(ceil(remTimeS/3600))
                         self._print_func(progStr, end='')
                         self._print_func('h', end='')
+                        self.len_prog_text += 3
                     elif(remTimeS>99): # less than 99m and more than 99s
                         progStr = "%02d" % int(ceil(remTimeS/60))
                         self._print_func(progStr, end='')
                         self._print_func('m', end='')
+                        self.len_prog_text += 3
                     elif(remTimeS>=0): # less than 99s and more than 0
                         progStr = "%02d" % int(ceil(remTimeS))
                         self._print_func(progStr, end='')
                         self._print_func('s', end='')
+                        self.len_prog_text += 3
                     else:
-                        self.end()
-            if(self.ck >= self.n_steps):
-                self.end()
+                        self._end()
+            if((self.ck >= self.n_steps) | 
+               (self.len_prog_text >= self.numTicks)):
+                self._end()
         return remTimeS
-    def end(self):
+
+    def _end(self):
         if(not self.FLAG_ended):
             self._print_func('')
             self.FLAG_ended = True
             
     def __del__(self):
-        self.end()
+        self._end()
```

### Comparing `lognflow-0.9.0/lognflow/utils.py` & `lognflow-0.9.1/lognflow/utils.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.9.0/lognflow.egg-info/PKG-INFO` & `lognflow-0.9.1/lognflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.9.0
+Version: 0.9.1
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -248,7 +248,12 @@
 0.9.0 (2023-08-09)
 -----------------
 * copy() is now possible from a file or a variable name into another
 * default suffix in get_flist is *
 * logviewer.get_stack_of_files is only useful for reading data.
 * more tests are added.
 * moved multichannel_to_frame to utils
+
+0.9.1 (2023-09-01)
+-----------------
+* bug removed from plt_utils numbers_as_images_4D.
+* bug removed from printprogress when number of steps is very low.
```

### Comparing `lognflow-0.9.0/lognflow.egg-info/SOURCES.txt` & `lognflow-0.9.1/lognflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lognflow-0.9.0/setup.py` & `lognflow-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """The setup script for lognflow."""
 
 from setuptools import setup, find_packages
 
 __author__ = 'Alireza Sadri'
 __email__ = 'arsadri@gmail.com'
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
```

### Comparing `lognflow-0.9.0/tests/test_lognflow.py` & `lognflow-0.9.1/tests/test_lognflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,15 +325,14 @@
 def test_log_multichannel_by_subplots():
     logger = lognflow(temp_dir)
     logger('Well this is a test for log_multichannel_by_subplots')
     images = np.random.rand(100, 100, 20)
     logger.log_multichannel_by_subplots('images', images, (4, 5))
 
 if __name__ == '__main__':
-    
     #-----IF RUN BY PYTHON------#
     temp_dir = select_directory()
     #---------------------------#
     test_log_multichannel_by_subplots()
     test_replace_time_with_index()
     test_log_hist()
     test_copy_list_of_files()
```

### Comparing `lognflow-0.9.0/tests/test_logviewer.py` & `lognflow-0.9.1/tests/test_logviewer.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.9.0/tests/test_printprogress.py` & `lognflow-0.9.1/tests/test_printprogress.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,34 +7,19 @@
 from lognflow import lognflow, select_directory, logviewer, printprogress
 
 import numpy as np
 
 import tempfile
 temp_dir = tempfile.gettempdir()
 
-@pytest.fixture
-def response():
-    """Sample pytest fixture.
-
-    See more at: http://doc.pytest.org/en/latest/fixture.html
-    """
-    # import requests
-    # return requests.get('https://github.com/audreyr/cookiecutter-pypackage')
-
-def test_content(response):
-    """Sample pytest test function with the pytest fixture as an argument."""
-    # from bs4 import BeautifulSoup
-    # assert 'GitHub' in BeautifulSoup(response.content).title.string
-
 def test_printprogress():
-    N = 3000000
-    pprog = printprogress(N)
-    for _ in range(N):
-        pprog()
-    # assert input('Did it show you a progress bar? (y for yes)')=='y'
+    for N in list([2, 4, 8, 10, 20, 200, 2000, 20000, 20000000]):
+        pprog = printprogress(N)
+        for _ in range(N):
+            pprog()
 
 def test_printprogress_with_logger():
     logger = lognflow(temp_dir)
     N = 1500000
     pprog = printprogress(N, print_function = logger, log_time_stamp = False)
     for _ in range(N):
         pprog()
@@ -58,12 +43,12 @@
             counter += 1
         pprog()
 
 if __name__ == '__main__':
     #-----IF RUN BY PYTHON------#
     temp_dir = select_directory()
     #---------------------------#
+    test_printprogress()
     test_printprogress_ETA()
     test_specific_timing()
     test_printprogress_with_logger()
-    test_printprogress()
-    exit()
+    exit()
```

