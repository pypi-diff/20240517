# Comparing `tmp/starbug2-0.7.3.tar.gz` & `tmp/starbug2-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starbug2-0.7.3.tar", last modified: Tue Mar 19 16:12:26 2024, max compression
+gzip compressed data, was "starbug2-0.7.4.tar", last modified: Fri May 17 14:03:21 2024, max compression
```

## Comparing `starbug2-0.7.3.tar` & `starbug2-0.7.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:12:26.897886 starbug2-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-19 16:12:21.000000 starbug2-0.7.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-19 16:12:21.000000 starbug2-0.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    46301 2024-03-19 16:12:26.897886 starbug2-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-03-19 16:12:21.000000 starbug2-0.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-19 16:12:21.000000 starbug2-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-19 16:12:21.000000 starbug2-0.7.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 16:12:26.897886 starbug2-0.7.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:12:26.893886 starbug2-0.7.3/starbug2/
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-03-19 16:12:21.000000 starbug2-0.7.3/starbug2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13819 2024-03-19 16:12:21.000000 starbug2-0.7.3/starbug2/artificialstars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:12:26.893886 starbug2-0.7.3/starbug2/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-19 16:12:21.000000 starbug2-0.7.3/starbug2/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-03-19 16:12:21.000000 starbug2-0.7.3/starbug2/bin/afs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15267 2024-03-19 16:12:21.000000 starbug2-0.7.3/starbug2/bin/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     8641 2024-03-19 16:12:21.000000 starbug2-0.7.3/starbug2/bin/match.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:12:26.893886 starbug2-0.7.3/starbug2/extras/
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-03-19 16:12:21.000000 starbug2-0.7.3/starbug2/extras/.default.param
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-03-19 16:12:21.000000 starbug2-0.7.3/starbug2/extras/starbug2-afs.completion
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-03-19 16:12:21.000000 starbug2-0.7.3/starbug2/extras/starbug2-match.completion
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-03-19 16:12:21.000000 starbug2-0.7.3/starbug2/extras/starbug2.completion
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-03-19 16:12:21.000000 starbug2-0.7.3/starbug2/mask.py
--rw-r--r--   0 runner    (1001) docker     (127)    32587 2024-03-19 16:12:21.000000 starbug2-0.7.3/starbug2/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-03-19 16:12:21.000000 starbug2-0.7.3/starbug2/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-03-19 16:12:21.000000 starbug2-0.7.3/starbug2/param.py
--rw-r--r--   0 runner    (1001) docker     (127)    34604 2024-03-19 16:12:21.000000 starbug2-0.7.3/starbug2/routines.py
--rw-r--r--   0 runner    (1001) docker     (127)    37832 2024-03-19 16:12:21.000000 starbug2-0.7.3/starbug2/starbug.py
--rw-r--r--   0 runner    (1001) docker     (127)    14608 2024-03-19 16:12:21.000000 starbug2-0.7.3/starbug2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:12:26.897886 starbug2-0.7.3/starbug2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    46301 2024-03-19 16:12:26.000000 starbug2-0.7.3/starbug2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-19 16:12:26.000000 starbug2-0.7.3/starbug2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 16:12:26.000000 starbug2-0.7.3/starbug2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-19 16:12:26.000000 starbug2-0.7.3/starbug2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-19 16:12:26.000000 starbug2-0.7.3/starbug2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-19 16:12:26.000000 starbug2-0.7.3/starbug2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:12:26.893886 starbug2-0.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-03-19 16:12:21.000000 starbug2-0.7.3/tests/test_match_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-03-19 16:12:21.000000 starbug2-0.7.3/tests/test_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-19 16:12:21.000000 starbug2-0.7.3/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-03-19 16:12:21.000000 starbug2-0.7.3/tests/test_param.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-03-19 16:12:21.000000 starbug2-0.7.3/tests/test_routines.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-03-19 16:12:21.000000 starbug2-0.7.3/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-19 16:12:21.000000 starbug2-0.7.3/tests/test_starbug.py
--rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-03-19 16:12:21.000000 starbug2-0.7.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:03:21.986500 starbug2-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-17 14:03:17.000000 starbug2-0.7.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-17 14:03:17.000000 starbug2-0.7.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    46301 2024-05-17 14:03:21.986500 starbug2-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-17 14:03:17.000000 starbug2-0.7.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-17 14:03:17.000000 starbug2-0.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-17 14:03:17.000000 starbug2-0.7.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 14:03:21.986500 starbug2-0.7.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:03:21.982500 starbug2-0.7.4/starbug2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-17 14:03:17.000000 starbug2-0.7.4/starbug2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14554 2024-05-17 14:03:17.000000 starbug2-0.7.4/starbug2/artificialstars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:03:21.982500 starbug2-0.7.4/starbug2/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-17 14:03:17.000000 starbug2-0.7.4/starbug2/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-05-17 14:03:17.000000 starbug2-0.7.4/starbug2/bin/afs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15267 2024-05-17 14:03:17.000000 starbug2-0.7.4/starbug2/bin/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8641 2024-05-17 14:03:17.000000 starbug2-0.7.4/starbug2/bin/match.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:03:21.986500 starbug2-0.7.4/starbug2/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-17 14:03:17.000000 starbug2-0.7.4/starbug2/extras/.default.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-17 14:03:17.000000 starbug2-0.7.4/starbug2/extras/starbug2-afs.completion
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-17 14:03:17.000000 starbug2-0.7.4/starbug2/extras/starbug2-match.completion
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-17 14:03:17.000000 starbug2-0.7.4/starbug2/extras/starbug2.completion
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-17 14:03:17.000000 starbug2-0.7.4/starbug2/mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32587 2024-05-17 14:03:17.000000 starbug2-0.7.4/starbug2/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-05-17 14:03:17.000000 starbug2-0.7.4/starbug2/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-05-17 14:03:17.000000 starbug2-0.7.4/starbug2/param.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34848 2024-05-17 14:03:17.000000 starbug2-0.7.4/starbug2/routines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38777 2024-05-17 14:03:17.000000 starbug2-0.7.4/starbug2/starbug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-05-17 14:03:17.000000 starbug2-0.7.4/starbug2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:03:21.986500 starbug2-0.7.4/starbug2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    46301 2024-05-17 14:03:21.000000 starbug2-0.7.4/starbug2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-17 14:03:21.000000 starbug2-0.7.4/starbug2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:03:21.000000 starbug2-0.7.4/starbug2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-17 14:03:21.000000 starbug2-0.7.4/starbug2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-17 14:03:21.000000 starbug2-0.7.4/starbug2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 14:03:21.000000 starbug2-0.7.4/starbug2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:03:21.986500 starbug2-0.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-17 14:03:17.000000 starbug2-0.7.4/tests/test_match_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-05-17 14:03:17.000000 starbug2-0.7.4/tests/test_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-17 14:03:17.000000 starbug2-0.7.4/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-17 14:03:17.000000 starbug2-0.7.4/tests/test_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-17 14:03:17.000000 starbug2-0.7.4/tests/test_routines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-17 14:03:17.000000 starbug2-0.7.4/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-17 14:03:17.000000 starbug2-0.7.4/tests/test_starbug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-17 14:03:17.000000 starbug2-0.7.4/tests/test_utils.py
```

### Comparing `starbug2-0.7.3/LICENSE.txt` & `starbug2-0.7.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `starbug2-0.7.3/PKG-INFO` & `starbug2-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starbug2
-Version: 0.7.3
+Version: 0.7.4
 Summary: JWST PSF photometry in complex crowded fields.
 Author-email: Conor Nally <conor.nally@ed.ac.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `starbug2-0.7.3/README.md` & `starbug2-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `starbug2-0.7.3/pyproject.toml` & `starbug2-0.7.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "starbug2"
-version = "0.7.3"
+version = "0.7.4"
 authors = [ {name = "Conor Nally", email = "conor.nally@ed.ac.uk" } ]
 readme = "README.md"
 description = "JWST PSF photometry in complex crowded fields."
 license = {file = "LICENSE.txt"}
 requires-python = ">=3.10"
 dynamic = ["dependencies"]
```

### Comparing `starbug2-0.7.3/starbug2/__init__.py` & `starbug2-0.7.4/starbug2/__init__.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.7.3/starbug2/artificialstars.py` & `starbug2-0.7.4/starbug2/artificialstars.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,33 +6,34 @@
 from starbug2.utils import perror, loading, cropHDU, get_MJysr2Jy_scalefactor, warn
 from starbug2.matching import GenericMatch
 
 from astropy.io import fits
 
 from photutils.psf import FittableImageModel
 from scipy.signal import savgol_filter
+from scipy.optimize import curve_fit
 
 
 
 class Artificial_StarsIII(object):
     def __init__(self, starbug):
         ## Initialis the starbug instance
         self.starbug=starbug
         _=self.starbug.image
         _=self.starbug.load_psf()
 
         self.psf=FittableImageModel(self.starbug.psf)
 
     def __call__(self,*args,**kwargs): return self.run_auto(*args,**kwargs)
 
-    def auto_run(self, ntests, stars_per_test=1, subimage_size=-1, mag_range=(18,27)):
+    def auto_run(self, ntests, stars_per_test=1, subimage_size=-1, mag_range=(18,27),
+            loading_buffer=None):
         """
         """
 
-        load=loading(ntests)
         test_result=Table(None, names=["x_0","y_0","flux","mag","x_det","y_det","flux_det", "status"])
         scalefactor= get_MJysr2Jy_scalefactor(self.starbug.image)
         base_image=self.starbug._image.copy()
         base_shape=np.copy(self.starbug.image.shape)
         stars_per_test=int(stars_per_test)
         passed=0
 
@@ -63,21 +64,22 @@
                                                                     "mag":mag_range}) 
             sourcelist.add_column( 10.0 ** ( (ZP-sourcelist["mag"])/2.5 ) , name="flux")
 
             star_overlay=make_model_sources_image( shape, self.psf, sourcelist)/scalefactor
             image[self.starbug._nHDU].data+=star_overlay
             self.starbug._image=image
             
+            n=len(sourcelist)
             result=self.single_test(image, sourcelist)
             passed+=sum(result["status"])
             test_result=vstack((test_result,result))
 
-            load()
-            load.msg="recovering %d%%"%(100*passed/(test*stars_per_test))
-            load.show()
+            if loading_buffer is not None:
+                loading_buffer[0]+=1
+                loading_buffer[2]=int(100*passed/(test*stars_per_test))
         return test_result
 
     def single_test(self, image, contains):
         """
         """
         NULL=0
         DETECT=1
@@ -103,39 +105,41 @@
 
             for i, src in enumerate(contains):
                 separations=np.sqrt( (src["x_0"]-det["xcentroid"])**2 + (src["y_0"]-det["ycentroid"])**2)
                 best_match=np.argmin(separations)
                 if separations[best_match]<threshold:
                     test_result["x_det"][i]=det["xcentroid"][best_match]
                     test_result["y_det"][i]=det["ycentroid"][best_match]
-                    test_result["status"][i]=DETECT
                     test_result["flux_det"][i]=det["flux"][best_match]
+                    test_result["status"][i]=DETECT
 
                     """
                     print(best_match, len(det))
                     self.starbug.detections = Table(det[best_match])
                     self.starbug.photometry()
                     test_result["flux_det"][i]=self.starbug.psfcatalogue["flux"]
                     """
                 else: test_result["status"][i]=NULL
 
+            #test_result.remove_rows( (np.isnan(test_result["x_det"])|np.isnan(test_result["y_det"])) )
             self.starbug.detections = test_result
-            if not self.starbug.photometry():
-                self.starbug.psfcatalogue
-                #test_result["flux_det"][test_result["status"].value.astype(bool)]=self.starbug.psfcatalogue["flux"]
-
-                self.starbug.psfcatalogue.rename_columns(("x_init","y_init","xydev"),("_x_init","_y_init","_xydev"))
-                matched=GenericMatch(threshold=threshold)([contains, self.starbug.psfcatalogue], cartesian=True)
-                #print(self.starbug.psfcatalogue[["x_init","y_init","x_fit","y_fit"]])
-                #print(matched[["Catalogue_Number_2","x_0_1","y_0_1","x_fit_2","y_fit_2"]])
-                #print(len(test_result),len(matched))
-                test_result["flux_det"] = matched[:len(test_result)]["flux_2"]
-        
 
+            if sum(test_result["status"]):
 
+                #if not self.starbug.bgd_estimate() and not self.starbug.photometry():
+                if not self.starbug.photometry():
+                    #self.starbug.psfcatalogue
+                    #test_result["flux_det"][test_result["status"].value.astype(bool)]=self.starbug.psfcatalogue["flux"]
+
+                    self.starbug.psfcatalogue.rename_columns(("x_init","y_init","xydev"),("_x_init","_y_init","_xydev"))
+                    matched=GenericMatch(threshold=threshold)([contains, self.starbug.psfcatalogue], cartesian=True)
+                    #print(self.starbug.psfcatalogue[["x_init","y_init","x_fit","y_fit"]])
+                    #print(matched[["Catalogue_Number_2","x_0_1","y_0_1","x_fit_2","y_fit_2"]])
+                    #print(len(test_result),len(matched))
+                    test_result["flux_det"] = matched[:len(test_result)]["flux_2"]
 
         return hstack((contains,test_result))
 
 
     def create_subimage(self, image, size, position=(0,0), hdu=1, buffer=0):
         """
         """
@@ -154,57 +158,65 @@
         y_end =  int(min( position[1]+(size/2), imshape[1]-buffer))
 
         return cropHDU(image,xlim=(x_edge,x_end),ylim=(y_edge,y_end)), x_edge, y_edge
 
     def get_magerr(self, test_result):
         return None
 
-    def get_completeness(self, test_result):
+    @staticmethod
+    def get_completeness(test_result):
         """
 
         Returns:
         --------
         result : astropy Table
             Table containing percent completeness as a function of magnitude
         """
 
-        bins = np.arange( min(test_result["mag"]), max(test_result["mag"]), 0.1)
+        bins = np.arange( np.floor(min(test_result["mag"])), np.ceil(max(test_result["mag"])), 0.1)
         percs= np.zeros(len(bins))
         errors=np.zeros(len(bins))
         means =np.zeros(len(bins))
         
         ibins = np.digitize( test_result["mag"], bins=bins)
         for i in range(max(ibins)):
             binned=test_result[ (ibins==i) ]
-            if binned: percs[i]=sum(binned["status"])/len(binned)
+            if binned: percs[i]=float(sum(binned["status"]))/len(binned)
 
             mag_inj= -2.5*np.log10( binned["flux"])
             mag_det= -2.5*np.log10( binned["flux_det"])
             errors[i]=np.nanstd( mag_inj-mag_det )
             means[i]=np.nanmean( mag_inj-mag_det )
 
-        import matplotlib.pyplot as plt
-        fig,(ax1,ax2)=plt.subplots(1,2)
-        ax1.scatter(bins,percs,c='k')
-        y=savgol_filter( percs, window_length=10, polyorder=2)
-        ax1.plot(bins,y, c='cyan')
-
-        ax2.scatter( -2.5 * np.log10( test_result["flux"]/test_result["flux_det"] ), test_result["mag"], c='k')
-        ax2.errorbar( means, bins , xerr=errors, lw=0)
-        ax2.invert_yaxis()
 
+        #_s=curve_fit(fnxep,bins,percs)
+        #a,b,c=_s[0]
 
-
-        plt.show()
+        out=Table( [bins,percs,errors], names=("mag","rec","err"), dtype=(float,float,float))
+        return out
 
 
+        """
+        mask= np.isnan(test_result["flux_det"])
+        test_result=test_result[~mask]
+        m,c=np.polyfit(test_result["flux_inj"], test_result["flux_det"],1)
 
+        import matplotlib.pyplot as plt
+        fig,(ax1,ax2)=plt.subplots(1,2)
+        ax1.plot(bins,percs,c='k')
+        x=np.linspace(min(bins),max(bins),100)
+        ax1.plot(x,fnxep(x,a,b,c))
+        #y=savgol_filter( percs, window_length=10, polyorder=2)
+        #ax1.plot(bins,y, c='cyan')
 
+        ax2.plot(bins,errors)
 
-        return None
+        plt.tight_layout()
+        plt.show()
+        """
 
 
 
 class Artificial_Stars(object):
 
     def __init__(self, psf=None, detector=None, photometry=None):
         self.psf=psf
@@ -371,7 +383,9 @@
         subimage=image[ x_edge:x_end,y_edge:y_end]
         return subimage, x_edge, y_edge
         
     def periodic_export(self,fname=""):
         return 0
 
 
+def fnxep(x,a,b,c):
+    return a*np.exp(b*x+c)
```

### Comparing `starbug2-0.7.3/starbug2/bin/main.py` & `starbug2-0.7.4/starbug2/bin/main.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.7.3/starbug2/bin/match.py` & `starbug2-0.7.4/starbug2/bin/match.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.7.3/starbug2/extras/.default.param` & `starbug2-0.7.4/starbug2/extras/.default.param`

 * *Files identical despite different names*

### Comparing `starbug2-0.7.3/starbug2/extras/starbug2-afs.completion` & `starbug2-0.7.4/starbug2/extras/starbug2-afs.completion`

 * *Files identical despite different names*

### Comparing `starbug2-0.7.3/starbug2/extras/starbug2-match.completion` & `starbug2-0.7.4/starbug2/extras/starbug2-match.completion`

 * *Files identical despite different names*

### Comparing `starbug2-0.7.3/starbug2/extras/starbug2.completion` & `starbug2-0.7.4/starbug2/extras/starbug2.completion`

 * *Files identical despite different names*

### Comparing `starbug2-0.7.3/starbug2/mask.py` & `starbug2-0.7.4/starbug2/mask.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.7.3/starbug2/matching.py` & `starbug2-0.7.4/starbug2/matching.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.7.3/starbug2/misc.py` & `starbug2-0.7.4/starbug2/misc.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.7.3/starbug2/param.py` & `starbug2-0.7.4/starbug2/param.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,75 +4,77 @@
 
 default="""## STARBUG CONFIG FILE
 # Generated with starbug2-v%s
 PARAM       =  STARBUGII PARAMETERS     //COMMENT
 
 
 ## GENERIC
-VERBOSE     = 0          // (0:false 1:true)
+VERBOSE     = 0          //(0:false 1:true)
 OUTPUT      = .          //Directory or filename to output to 
 HDUNAME     =            //If using a non standard HDU name, name it here (str or int)
 FILTER      =            //Set a custom filter for the image
 
 ## DETECTETION 
-FWHM        = -1         // Custom FWHM for image (-1 to use WEBBPSF)
-SIGSKY      = 2.0        // (float>0) 
-SIGSRC      = 5.0        // (float>0) Source value mininmum N sigma above background
-DOBGD2D     = 1          // Run background2D step (usually finds more sources but takes time)
-DOCONVL     = 1          // Run convolution step (usually finds more sources)
-CLEANSRC    = 1          // Run source cleaning after detection (removes likely contaminants)
-SHARP_LO    = 0.4        // cutoff in detection
-SHARP_HI    = 0.9        // cutoff in detection
-ROUND1_HI   = 1.0        // cutoff in detection
-ROUND2_HI   = 1.0        // cutoff in detection
-SMOOTH_LO   =            //.
-SMOOTH_HI   =            //.
-RICKER_R    = 1.0        // Radius (pix) of ricker wavelet 
+FWHM        = -1         //Custom FWHM for image (-1 to use WEBBPSF)
+SIGSKY      = 2.0        //(float>0) 
+SIGSRC      = 5.0        //Source value mininmum N sigma above background
+DOBGD2D     = 1          //Run background2D step (usually finds more sources but takes time)
+DOCONVL     = 1          //Run convolution step (usually finds more sources)
+CLEANSRC    = 1          //Run source cleaning after detection (removes likely contaminants)
+SHARP_LO    = 0.4        //Cutoff in detection
+SHARP_HI    = 0.9        //Cutoff in detection
+ROUND1_HI   = 1.0        //Cutoff in detection
+ROUND2_HI   = 1.0        //Cutoff in detection
+SMOOTH_LO   =            //Cutoff in detection
+SMOOTH_HI   =            //Cutoff in detection 
+RICKER_R    = 1.0        //Radius (pix) of ricker wavelet 
 
 ## APERTURE PHOTOMOETRY
 APPHOT_R    = 1.5        //Radius in number of pixels
 ENCENERGY   = -1         //Fraction encircled energy (mutually exclusive with APPHOT_R)
 SKY_RIN     = 3          //Sky annulus inner radius
 SKY_ROUT    = 4.5        //Sky annulus outer radius
 APCORR_FILE =            //Aperture correction file. See full manual for details
 
 ## BACKGROUND ESTIMATION
-BGD_R       = 0          //.
-BOX_SIZE    = 2          // (int>0) Background estimation kernal size (pix)
+BGD_R       = 0          //Aperture masking fixed radius (if zero, starbug will scale radii)
+BOX_SIZE    = 2          //Background estimation kernal size (pix)
 
 ## PHOTOMETRY
 AP_FILE     =            //Detection file to use instead of detecting
 BGD_FILE    =            //Background estimation file
 PSF_FILE    =            //Non default PSF file
 USE_WCS     = 1          //When loading an AP_FILE, do you want to use WCS or xy values (if available)
 ZP_MAG      = 8.9        //Zero point (mag) to add to the magnitude columns 
 
 CRIT_SEP    =            //minimum distance for grouping (pixels) between two sources
 FORCE_POS   = 0          //Force centroid position (1) or allow psf fitting to fit position too (0)
 DPOS_THRESH = -1         //If allowed to fit position, max separation (arcsec) from source list centroid
-MAX_XYDEV   = 3p         //.
+MAX_XYDEV   = 3p         //Maximum deviation from initial guess centroid position
 PSF_SIZE    = -1         //Set fit size of psf (>0) or -1 to take PSF file dimensions
-GEN_RESIDUAL= 0          //generate a residual image
+GEN_RESIDUAL= 0          //Generate a residual image
 
 ## SOURCE STATS
 CALC_CROWD  = 1          //Run crowding metric calculation (execution time scales N^2)
 
 ## CATALOGUE MATCHING
-MATCH_THRESH= 0.1        // when combining background subtraction catalogue, minimum separation (arcsec) of centroids to be considered separate sources
+MATCH_THRESH= 0.1        // matching separation threshold in units arcsec
 MATCH_COLS  =            // EXTRA columns to include in output matched table i.e sharpness
 NEXP_THRESH = -1         // Keep sources that appear in NUM >= NEXP_THRESH (if -1 keep everything)
 SN_THRESH   = -1         // Remove sources with SN ratio < SN_THRESH before matching (default -1 to not apply this cut)
 BRIDGE_COL  =            // Bridge --band matching NIRCam and MIRI catalogues by ensuring NIRCam catalogue has a match in BRIDGE_COL
 
 ## ARTIFICAL STAR TESTS
-NTESTS      = 100        // Number of artificial star tests
-NSTARS      = 1          // Number of stars per artifical test
+NTESTS      = 100        //Number of artificial star tests
+NSTARS      = 1          //Number of stars per artifical test
 SUBIMAGE    = 500        //number of pixels ? to crop around artificial star
-MIN_FLUX    = 0.00001      //minimun flux for artificial star
-MAX_FLUX    = 100.0      //maximum flux for artificial star
+#MIN_FLUX    = 0.00001    //minimun flux for artificial star
+#MAX_FLUX    = 100.0      //maximum flux for artificial star
+MIN_MAG     = 18.0       //Bright limit of test magnitude
+MAX_MAG     = 28.0       //Faint limit of test magnitude
 
 ## MISC EXTRAS
 REGION_COL  = green      //DS9 region colour
 REGION_SCAL = 1          //Scale region to flux if possible
 REGION_RAD  = 3          //Region radius default
 REGION_XCOL = RA         //X column name to use for region
 REGION_YCOL = DEC        //Y column name to use for region
```

### Comparing `starbug2-0.7.3/starbug2/routines.py` & `starbug2-0.7.4/starbug2/routines.py`

 * *Files 2% similar despite different names*

```diff
@@ -710,17 +710,24 @@
         """
         """ 
 
         if init_params is None or len(init_params)==0:
             perror("Must include source list\n")
             return None
 
+        
+
+        ### Removing completely masked sources
+        apertures=CircularAperture([(l["x_init"],l["y_init"]) for l in init_params],self.aperture_radius)
+        apmasks=aperture_photometry(~mask,apertures)
+        init_params.remove_rows(apmasks["aperture_sum"]==0)
+
+        error[error==0]=sys.maxsize ## bad errors should be big not small
+
         if self.background is not None: image=image-self.background
-        from astropy.io import fits
-        fits.PrimaryHDU( image).writeto("/tmp/out.fits",overwrite=True)
         if self.verbose: printf("-> fitting %d sources\n"%len(init_params))
         cat=super().__call__(image, mask=mask, init_params=init_params, error=error)
 
         d=np.sqrt((cat["x_init"]-cat["x_fit"])**2.0 + (cat["y_init"]-cat["y_fit"])**2.0)
         cat.add_column(Column(d,name="xydev"))
 
         if "flux_err" not in cat.colnames:
```

### Comparing `starbug2-0.7.3/starbug2/starbug.py` & `starbug2-0.7.4/starbug2/starbug.py`

 * *Files 3% similar despite different names*

```diff
@@ -244,15 +244,15 @@
                     #self.options["USE_WCS"]=0
 
             elif len( set(("x_0","y_0"))&cn)==2:
                 self.detections.rename_columns(("x_0","y_0"),("xcentroid","ycentroid"))
             elif len( set(("x_init","y_init"))&cn)==2:
                 self.detections.rename_columns(("x_init","y_init"),("xcentroid","ycentroid"))
 
-            if len( set(("xcentroid","ycentroid"))&cn)==2:
+            if len( set(("xcentroid","ycentroid"))&set(self.detections.colnames))==2:
                 mask=(self.detections["xcentroid"]>=0) & (self.detections["xcentroid"]<self.image.shape[1]) & (self.detections["ycentroid"]>=0) & (self.detections["ycentroid"]<self.image.shape[0])
                 self.detections.remove_rows(~mask)
                 self.log("-> loaded %d sources from AP_FILE\n"%len(self.detections))
             else:
                 warn("Unable to determine physical coordinates from detections table\n")
         else: perror("AP_FILE='%s' does not exists\n"%fname)
 
@@ -345,15 +345,16 @@
             error=self._image["ERR"].data.copy() * scalefactor
         else: error=np.sqrt(np.abs(image))
         
         # create mask
         if "DQ" in extnames(self._image):
             mask=self._image["DQ"].data & (DQ_DO_NOT_USE|DQ_SATURATED) #|DQ_JUMP_DET)
             mask=mask.astype(bool)
-        else:mask=np.isnan(image)
+        else:mask=(np.isnan(image) | np.isnan(error))
+        #fits.PrimaryHDU(data=mask.astype(int)).writeto("/tmp/out.fits",overwrite=True)
 
         # collect and scale background array
         if self.background is not None:
             bgd=self.background.data.copy() * scalefactor
         else: bgd=None
 
         return image, error, bgd, mask
@@ -528,35 +529,49 @@
 
     def bgd_estimate(self):
         """
         Estimate the background of the active image
         Saves the result as an ImageHDU self.background
         """
         self.log("\nEstimating Diffuse Background\n")
+        status=1
         if self.detections:
+            sourcelist=self.detections.copy()
 
             _f=starbug2.filters.get(self.filter)
             if self.options["FWHM"]>0: FWHM=self.options["FWHM"]
             elif _f: FWHM=_f.pFWHM
             else: FWHM=2
 
-            bgd=BackGround_Estimate_Routine(self.detections,
+            if "x_init" in sourcelist.colnames: sourcelist.rename_column("x_init", "xcentroid")
+            if "y_init" in sourcelist.colnames: sourcelist.rename_column("y_init", "ycentroid")
+            if "x_det" in sourcelist.colnames: sourcelist.rename_column("x_det", "xcentroid")
+            if "y_det" in sourcelist.colnames: sourcelist.rename_column("y_det", "ycentroid")
+            if "flux_det" in sourcelist.colnames: sourcelist.rename_column("flux_det", "flux")
+            mask=~(np.isnan(sourcelist["xcentroid"])|np.isnan(sourcelist["ycentroid"]))
+
+
+            bgd=BackGround_Estimate_Routine(sourcelist[mask],
                                             boxsize=int(self.options["BOX_SIZE"]),
                                             fwhm=FWHM,
                                             sigsky=self.options["SIGSKY"],
                                             bgd_r=self.options["BGD_R"],
                                             verbose=self.options["VERBOSE"])
             header=self.header
             header.update(self.wcs.to_header())
             self.background=fits.ImageHDU(data=bgd(self.image.data.copy()), header=header)
-            _fname="%s/%s-bgd.fits"%(self.outdir, self.bname)
-            self.log("--> %s\n"%_fname)
-            self.background.writeto(_fname,overwrite=True)
+            if not self.options.get("QUIETMODE"):
+                _fname="%s/%s-bgd.fits"%(self.outdir, self.bname)
+                self.log("--> %s\n"%_fname)
+                self.background.writeto(_fname,overwrite=True)
+
         else:
             perror("unable to estimate background, no source list loaded\n")
+            status=1
+        return status
 
 
 
     def bgd_subtraction(self):
         """
         Internally subtract a background array from an image array
         """
@@ -638,25 +653,30 @@
             else: size=psf_model.shape[0]
             if not size%2: size-=1
             self.log("-> psf size: %d\n"%size)
 
             #########################
             # Sort out Init guesses #
             #########################
+            apphot_r=self.options.get("APPHOT_R")
+            if not apphot_r or apphot_r <=0: apphot_r=3
 
             init_guesses=self.detections.copy()
+            #print(init_guesses, end="")
             if "xcentroid" in init_guesses.colnames: init_guesses.rename_column("xcentroid", "x_init")
             if "ycentroid" in init_guesses.colnames: init_guesses.rename_column("ycentroid", "y_init")
             if "x_det" in init_guesses.colnames: init_guesses.rename_column("x_det", "x_init")
             if "y_det" in init_guesses.colnames: init_guesses.rename_column("y_det", "y_init")
 
             init_guesses=init_guesses[ init_guesses["x_init"]>=0 ]
             init_guesses=init_guesses[ init_guesses["y_init"]>=0 ]
             init_guesses=init_guesses[ init_guesses["x_init"]<self.image.header["NAXIS1"]]
             init_guesses=init_guesses[ init_guesses["y_init"]<self.image.header["NAXIS2"]]
+            #print(init_guesses)
+
 
             ######
             # Allow tables that dont have the correct columns through
             ######
             required=["x_init","y_init","flux",self.filter, "flag"]
             for notfound in  set(required)-set(init_guesses.colnames):
                 dtype=np.uint16 if notfound=="flag" else float
@@ -669,16 +689,14 @@
             #init_guesses=init_guesses[init_guesses["flux_0"]>0]
             #init_guesses.remove_column("flux_0")
 
             
             ###########
             # Run Fit #
             ###########
-            apphot_r=self.options.get("APPHOT_R")
-            if not apphot_r or apphot_r <=0: apphot_r=3
 
             min_separation=self.options.get("CRIT_SEP")
             if not min_separation:
                 min_separation = min(5, 2.5*self.options.get("FWHM"))
 
             if self.options["FORCE_POS"]:
                 phot=PSFPhot_Routine(psf_model, size, min_separation=min_separation, apphot_r=apphot_r, background=bgd, force_fit=1, verbose=self.options["VERBOSE"])
```

### Comparing `starbug2-0.7.3/starbug2/utils.py` & `starbug2-0.7.4/starbug2/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     """
     Returns the contents of the table as a notmal 2D numpy array
     NB: this is different from Table.asarray(), which returns an array of numpy.voids
 
     if colnames not None, return the subset of the table corresponding to this list
     """
     if not colnames: colnames=tab.colnames
-    else: colnames=list( set(colnames)&set(tab.colnames) )
+    else: colnames=rmduplicates(colnames)#list( set(colnames)&set(tab.colnames) ) ####BBAAAAD
     return np.array( tab[colnames].as_array().tolist() )
 
 def collapse_header(header):
     """
     Convert a dictionary to a Header. 
     Parameters in PARAMFILES have keys longer than 8 chars
     which can cause issues in the fits format. This function turns
```

### Comparing `starbug2-0.7.3/starbug2.egg-info/PKG-INFO` & `starbug2-0.7.4/starbug2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starbug2
-Version: 0.7.3
+Version: 0.7.4
 Summary: JWST PSF photometry in complex crowded fields.
 Author-email: Conor Nally <conor.nally@ed.ac.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `starbug2-0.7.3/starbug2.egg-info/SOURCES.txt` & `starbug2-0.7.4/starbug2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `starbug2-0.7.3/tests/test_match_run.py` & `starbug2-0.7.4/tests/test_match_run.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.7.3/tests/test_matching.py` & `starbug2-0.7.4/tests/test_matching.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.7.3/tests/test_param.py` & `starbug2-0.7.4/tests/test_param.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.7.3/tests/test_routines.py` & `starbug2-0.7.4/tests/test_routines.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.7.3/tests/test_run.py` & `starbug2-0.7.4/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.7.3/tests/test_utils.py` & `starbug2-0.7.4/tests/test_utils.py`

 * *Files identical despite different names*

