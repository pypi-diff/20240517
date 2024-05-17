# Comparing `tmp/par_segmentation-0.1.8.tar.gz` & `tmp/par_segmentation-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/par-segmentation/par-segmentation/dist/.tmp-zghmkziz/par_segmentation-0.1.8.tar", last modified: Thu Aug  3 14:27:10 2023, max compression
+gzip compressed data, was "/home/runner/work/par-segmentation/par-segmentation/dist/.tmp-_jddyyxs/par_segmentation-0.1.9.tar", last modified: Tue Aug  8 10:33:16 2023, max compression
```

## Comparing `par_segmentation-0.1.8.tar` & `par_segmentation-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:27:10.000000 par_segmentation-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    18650 2023-08-03 14:26:55.000000 par_segmentation-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-08-03 14:27:10.000000 par_segmentation-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-08-03 14:26:55.000000 par_segmentation-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:27:10.000000 par_segmentation-0.1.8/par_segmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-03 14:26:55.000000 par_segmentation-0.1.8/par_segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18880 2023-08-03 14:26:55.000000 par_segmentation-0.1.8/par_segmentation/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-08-03 14:26:55.000000 par_segmentation-0.1.8/par_segmentation/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)    15993 2023-08-03 14:26:55.000000 par_segmentation-0.1.8/par_segmentation/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)    16748 2023-08-03 14:26:55.000000 par_segmentation-0.1.8/par_segmentation/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10511 2023-08-03 14:26:55.000000 par_segmentation-0.1.8/par_segmentation/quantifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    14337 2023-08-03 14:26:55.000000 par_segmentation-0.1.8/par_segmentation/roi.py
--rw-r--r--   0 runner    (1001) docker     (123)    16402 2023-08-03 14:26:55.000000 par_segmentation-0.1.8/par_segmentation/tgf_interpolate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:27:10.000000 par_segmentation-0.1.8/par_segmentation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-08-03 14:27:10.000000 par_segmentation-0.1.8/par_segmentation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-03 14:27:10.000000 par_segmentation-0.1.8/par_segmentation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:27:10.000000 par_segmentation-0.1.8/par_segmentation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-03 14:27:10.000000 par_segmentation-0.1.8/par_segmentation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-03 14:27:10.000000 par_segmentation-0.1.8/par_segmentation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-03 14:27:10.000000 par_segmentation-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-03 14:26:55.000000 par_segmentation-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:27:10.000000 par_segmentation-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:26:55.000000 par_segmentation-0.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-03 14:26:55.000000 par_segmentation-0.1.8/tests/test_de_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-08-03 14:26:55.000000 par_segmentation-0.1.8/tests/test_de_correct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-08-03 14:26:55.000000 par_segmentation-0.1.8/tests/test_gd_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-03 14:26:55.000000 par_segmentation-0.1.8/tests/test_gd_correct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:33:16.000000 par_segmentation-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    18650 2023-08-08 10:33:03.000000 par_segmentation-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-08-08 10:33:16.000000 par_segmentation-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-08-08 10:33:03.000000 par_segmentation-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:33:16.000000 par_segmentation-0.1.9/par_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-08 10:33:03.000000 par_segmentation-0.1.9/par_segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-08-08 10:33:03.000000 par_segmentation-0.1.9/par_segmentation/_tgf_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20432 2023-08-08 10:33:03.000000 par_segmentation-0.1.9/par_segmentation/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16102 2023-08-08 10:33:03.000000 par_segmentation-0.1.9/par_segmentation/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16539 2023-08-08 10:33:03.000000 par_segmentation-0.1.9/par_segmentation/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17656 2023-08-08 10:33:03.000000 par_segmentation-0.1.9/par_segmentation/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11475 2023-08-08 10:33:03.000000 par_segmentation-0.1.9/par_segmentation/quantifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17645 2023-08-08 10:33:03.000000 par_segmentation-0.1.9/par_segmentation/roi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:33:16.000000 par_segmentation-0.1.9/par_segmentation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-08-08 10:33:16.000000 par_segmentation-0.1.9/par_segmentation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-08 10:33:16.000000 par_segmentation-0.1.9/par_segmentation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 10:33:16.000000 par_segmentation-0.1.9/par_segmentation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-08 10:33:16.000000 par_segmentation-0.1.9/par_segmentation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 10:33:16.000000 par_segmentation-0.1.9/par_segmentation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-08 10:33:16.000000 par_segmentation-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-08 10:33:03.000000 par_segmentation-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:33:16.000000 par_segmentation-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 10:33:03.000000 par_segmentation-0.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-08 10:33:03.000000 par_segmentation-0.1.9/tests/test_de_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-08 10:33:03.000000 par_segmentation-0.1.9/tests/test_de_correct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-08-08 10:33:03.000000 par_segmentation-0.1.9/tests/test_gd_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-08 10:33:03.000000 par_segmentation-0.1.9/tests/test_gd_correct.py
```

### Comparing `par_segmentation-0.1.8/LICENSE` & `par_segmentation-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `par_segmentation-0.1.8/PKG-INFO` & `par_segmentation-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: par_segmentation
-Version: 0.1.8
+Version: 0.1.9
 Summary: Cell cortex segmentation in C. elegans PAR protein images
 Author: Tom Bland
 Author-email: tom_bland@hotmail.co.uk
 License: CC BY 4.0
 Project-URL: Source Code, https://github.com/tsmbland/par-segmentation
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,14 +13,15 @@
 
 [![CC BY 4.0][cc-by-shield]][cc-by]
 ![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white)
 [![PyPi version](https://badgen.net/pypi/v/par-segmentation/)](https://pypi.org/project/par-segmentation)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tsmbland/par-segmentation/HEAD?filepath=%2Fscripts/Tutorial.ipynb)
 [![run with docker](https://img.shields.io/badge/run%20with-docker-0db7ed?logo=docker)](https://www.docker.com/)
 [![run with conda](http://img.shields.io/badge/run%20with-conda-3EB049?logo=anaconda)](https://docs.conda.io/en/latest/)
+[![Documentation Status](https://readthedocs.org/projects/par-segmentation/badge/?version=latest)](https://par-segmentation.readthedocs.io/en/latest/?badge=latest)
 
 Tools for segmenting, straightening and quantifying the cortex of cells.
 Works by combining spline-based segmentation with a custom quantification model, using a gradient descent optimisation procedure.
 Designed primarily for membrane-bound PAR proteins in C. elegans zygotes.
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/tsmbland/par-segmentation/master/scripts/Figs/animation.gif" width="100%" height="100%"/>
```

### Comparing `par_segmentation-0.1.8/README.md` & `par_segmentation-0.1.9/par_segmentation.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,27 @@
+Metadata-Version: 2.1
+Name: par-segmentation
+Version: 0.1.9
+Summary: Cell cortex segmentation in C. elegans PAR protein images
+Author: Tom Bland
+Author-email: tom_bland@hotmail.co.uk
+License: CC BY 4.0
+Project-URL: Source Code, https://github.com/tsmbland/par-segmentation
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PAR Segmentation
 
 [![CC BY 4.0][cc-by-shield]][cc-by]
 ![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white)
 [![PyPi version](https://badgen.net/pypi/v/par-segmentation/)](https://pypi.org/project/par-segmentation)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tsmbland/par-segmentation/HEAD?filepath=%2Fscripts/Tutorial.ipynb)
 [![run with docker](https://img.shields.io/badge/run%20with-docker-0db7ed?logo=docker)](https://www.docker.com/)
 [![run with conda](http://img.shields.io/badge/run%20with-conda-3EB049?logo=anaconda)](https://docs.conda.io/en/latest/)
+[![Documentation Status](https://readthedocs.org/projects/par-segmentation/badge/?version=latest)](https://par-segmentation.readthedocs.io/en/latest/?badge=latest)
 
 Tools for segmenting, straightening and quantifying the cortex of cells.
 Works by combining spline-based segmentation with a custom quantification model, using a gradient descent optimisation procedure.
 Designed primarily for membrane-bound PAR proteins in C. elegans zygotes.
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/tsmbland/par-segmentation/master/scripts/Figs/animation.gif" width="100%" height="100%"/>
```

### Comparing `par_segmentation-0.1.8/par_segmentation/funcs.py` & `par_segmentation-0.1.9/par_segmentation/funcs.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 from .roi import offset_coordinates
 from typing import Optional, Union, Tuple
 
 """
 
 """
 
+__all__ = ['load_image', 'save_img', 'save_img_jpeg', 'straighten', 'rotated_embryo', 'rotate_roi', 'norm_roi', 'interp_1d_array', 'interp_2d_array',
+           'rolling_ave_1d', 'rolling_ave_2d', 'bounded_mean_1d', 'bounded_mean_2d', 'asi', 'dosage', 'make_mask', 'readnd', 'organise_by_nd',
+           'direcslist', 'in_notebook']
 
 ########## IMAGE HANDLING ###########
 
 
 def load_image(filename: str) -> np.ndarray:
     """
     Given the filename of a TIFF, creates numpy array with pixel intensities
@@ -39,19 +42,24 @@
 
     Args:
         img: numpy array of the image to save
         direc: file path to save to (including '.tif' extension)
 
     """
 
-    io.imsave(direc, img.astype('float32'))
+    io.imsave(direc, img.astype("float32"))
 
 
-def save_img_jpeg(img: np.ndarray, direc: str, cmin: Optional[float] = None, cmax: Optional[float] = None,
-                  cmap: str = 'gray'):
+def save_img_jpeg(
+    img: np.ndarray,
+    direc: str,
+    cmin: Optional[float] = None,
+    cmax: Optional[float] = None,
+    cmap: str = "gray",
+):
     """
     Saves 2D array as jpeg, according to min and max pixel intensities
 
     Args:
         img: numpy array of the image to save
         direc: file path to save to (including '.jpeg' extension)
         cmin: optional, sets intensity scaling (along with cmax)
@@ -62,16 +70,22 @@
 
     plt.imsave(direc, img, vmin=cmin, vmax=cmax, cmap=cmap)
 
 
 ########### IMAGE OPERATIONS ###########
 
 
-def straighten(img: np.ndarray, roi: np.ndarray, thickness: int, periodic: bool = True, interp: str = 'cubic',
-               ninterp: Optional[int] = None) -> np.ndarray:
+def straighten(
+    img: np.ndarray,
+    roi: np.ndarray,
+    thickness: int,
+    periodic: bool = True,
+    interp: str = "cubic",
+    ninterp: Optional[int] = None,
+) -> np.ndarray:
     """
     Creates straightened image based on coordinates
     Todo: Doesn't work properly for non-periodic rois
 
     Args:
         img: numpy array of image to straighten
         roi: coordinates of roi (two column array with x and y coordinates), should be 1 pixel length apart in a loop
@@ -103,31 +117,49 @@
         xdiffs = np.r_[xdiffs[0], xdiffs]
 
     grad = ydiffs / xdiffs
     tangent_grad = -1 / grad
 
     # Get interpolation coordinates
     offsets = np.linspace(thickness / 2, -thickness / 2, ninterp)
-    xchange = ((offsets ** 2)[np.newaxis, :] / (1 + tangent_grad ** 2)[:, np.newaxis]) ** 0.5
+    xchange = (
+        (offsets**2)[np.newaxis, :] / (1 + tangent_grad**2)[:, np.newaxis]
+    ) ** 0.5
     ychange = xchange / abs(grad)[:, np.newaxis]
-    gridcoors_x = xcoors[:, np.newaxis] + np.sign(ydiffs)[:, np.newaxis] * np.sign(offsets)[np.newaxis, :] * xchange
-    gridcoors_y = ycoors[:, np.newaxis] - np.sign(xdiffs)[:, np.newaxis] * np.sign(offsets)[np.newaxis, :] * ychange
+    gridcoors_x = (
+        xcoors[:, np.newaxis]
+        + np.sign(ydiffs)[:, np.newaxis] * np.sign(offsets)[np.newaxis, :] * xchange
+    )
+    gridcoors_y = (
+        ycoors[:, np.newaxis]
+        - np.sign(xdiffs)[:, np.newaxis] * np.sign(offsets)[np.newaxis, :] * ychange
+    )
 
     # Interpolate
-    if interp == 'linear':
-        straight = map_coordinates(img.T, [gridcoors_x, gridcoors_y], order=1, mode='nearest')
-    elif interp == 'cubic':
-        straight = map_coordinates(img.T, [gridcoors_x, gridcoors_y], order=3, mode='nearest')
+    if interp == "linear":
+        straight = map_coordinates(
+            img.T, [gridcoors_x, gridcoors_y], order=1, mode="nearest"
+        )
+    elif interp == "cubic":
+        straight = map_coordinates(
+            img.T, [gridcoors_x, gridcoors_y], order=3, mode="nearest"
+        )
     else:
         raise ValueError('interp must be "linear" or "cubic"')
     return straight.astype(np.float64).T
 
 
-def rotated_embryo(img: np.ndarray, roi: np.ndarray, l: int, h: int, order: int = 1,
-                   return_roi: bool = False) -> Union[np.ndarray, Tuple[np.array, np.array]]:
+def rotated_embryo(
+    img: np.ndarray,
+    roi: np.ndarray,
+    l: int,
+    h: int,
+    order: int = 1,
+    return_roi: bool = False,
+) -> Union[np.ndarray, Tuple[np.array, np.array]]:
     """
     Takes an image and rotates according to coordinates so that anterior is on left, posterior on right
     Todo: some of the returned coordinates are anticlockwise
 
     Args:
         img: numpy array of image to rotate
         roi: roi of cell boundary (two columns specifying x and y coordinates)
@@ -145,32 +177,36 @@
     # PCA on ROI coordinates
     [_, coeff] = np.linalg.eig(np.cov(roi.T))
 
     # Transform ROI
     roi_transformed = np.dot(coeff.T, roi.T)
 
     # Force long axis orientation
-    x_range = (min(roi_transformed[0, :]) - max(roi_transformed[0, :]))
-    y_range = (min(roi_transformed[1, :]) - max(roi_transformed[1, :]))
+    x_range = min(roi_transformed[0, :]) - max(roi_transformed[0, :])
+    y_range = min(roi_transformed[1, :]) - max(roi_transformed[1, :])
     if x_range > y_range:
         img = img.T
         roi_transformed = np.flipud(roi_transformed)
         coeff = coeff.T
 
     # Coordinate grid
     centre_x = (min(roi_transformed[0, :]) + max(roi_transformed[0, :])) / 2
     xvals = np.arange(int(centre_x) - (l / 2), int(centre_x) + (l / 2))
     centre_y = (min(roi_transformed[1, :]) + max(roi_transformed[1, :])) // 2
     yvals = np.arange(int(centre_y) - (h / 2), int(centre_y) + (h / 2))
     xvals_grid = np.tile(xvals, [len(yvals), 1])
     yvals_grid = np.tile(yvals, [len(xvals), 1]).T
-    roi_transformed = roi_transformed - np.expand_dims([centre_x - (l / 2), centre_y - (h / 2)], -1)
+    roi_transformed = roi_transformed - np.expand_dims(
+        [centre_x - (l / 2), centre_y - (h / 2)], -1
+    )
 
     # Transform coordinate grid back
-    [xvals_back, yvals_back] = np.dot(coeff, np.array([xvals_grid.flatten(), yvals_grid.flatten()]))
+    [xvals_back, yvals_back] = np.dot(
+        coeff, np.array([xvals_grid.flatten(), yvals_grid.flatten()])
+    )
     xvals_back_grid = np.reshape(xvals_back, [len(yvals), len(xvals)])
     yvals_back_grid = np.reshape(yvals_back, [len(yvals), len(xvals)])
 
     # Map coordinates using linear interpolation
     zvals = map_coordinates(img.T, [xvals_back_grid, yvals_back_grid], order=order)
 
     # Force posterior on right
@@ -244,37 +280,43 @@
 
     return score
 
 
 ########### ARRAY OPERATIONS ###########
 
 
-def interp_1d_array(array: np.ndarray, n: int, method: str = 'cubic') -> np.ndarray:
+def interp_1d_array(array: np.ndarray, n: int, method: str = "cubic") -> np.ndarray:
     """
     Interpolates a one dimensional array into n points
 
     Args:
         array: one dimensional numpy array
         n: number of points to evaluate. Will evaluate this many points at evenly space intervals along the length of
         array
         method: 'linear' or 'cubic'
 
     Returns:
         interpolated array (one dimensional array of length n)
 
     """
     # If using linear interpolation, return the result of np.interp applied to the input array
-    if method == 'linear':
-        return np.interp(np.linspace(0, len(array) - 1, n), np.array(range(len(array))), array)
+    if method == "linear":
+        return np.interp(
+            np.linspace(0, len(array) - 1, n), np.array(range(len(array))), array
+        )
     # If using cubic interpolation, return the result of CubicSpline applied to the input array
-    elif method == 'cubic':
-        return CubicSpline(np.arange(len(array)), array)(np.linspace(0, len(array) - 1, n))
+    elif method == "cubic":
+        return CubicSpline(np.arange(len(array)), array)(
+            np.linspace(0, len(array) - 1, n)
+        )
 
 
-def interp_2d_array(array: np.ndarray, n: int, ax: int = 0, method: str = 'cubic') -> np.ndarray:
+def interp_2d_array(
+    array: np.ndarray, n: int, ax: int = 0, method: str = "cubic"
+) -> np.ndarray:
     """
     Interpolates a two dimensional array along one axis into n points
 
     Args:
         array: two dimensional numpy array
         n: number of points to evaluate along the specified axis
         ax: 0 or 1, specifies the axis to interpolate along. 0 corresponds to the rows and 1 corresponds to the columns.
@@ -295,15 +337,15 @@
     elif ax == 1:
         interped = np.zeros([len(array[:, 0]), n])
         # Loop through each row and interpolate the values along axis 1
         for x in range(len(array[:, 0])):
             interped[x, :] = interp_1d_array(array[x, :], n, method)
         return interped
     else:
-        raise ValueError('ax must be 0 or 1')
+        raise ValueError("ax must be 0 or 1")
 
 
 def rolling_ave_1d(array: np.ndarray, window: int, periodic: bool = True) -> np.ndarray:
     """
     Performs a rolling window average along a one dimensional array
 
     Args:
@@ -319,18 +361,20 @@
     """
     # If window size is 1, return the input array as is
     if window == 1:
         return array
 
     # If the array is not periodic, pad the array with its own reflected values on both ends
     if not periodic:
-        array_padded = np.r_[array[:int(window / 2)][::-1], array, array[-int(window / 2):][::-1]]
+        array_padded = np.r_[
+            array[: int(window / 2)][::-1], array, array[-int(window / 2) :][::-1]
+        ]
     # If the array is periodic, pad the array with its own values on both ends
     else:
-        array_padded = np.r_[array[-int(window / 2):], array, array[:int(window / 2)]]
+        array_padded = np.r_[array[-int(window / 2) :], array, array[: int(window / 2)]]
     # Compute the cumulative sum of the padded array
     cumsum = np.cumsum(array_padded)
     # Return the rolling average of the padded array
     return (cumsum[window:] - cumsum[:-window]) / window
 
 
 def rolling_ave_2d(array: np.ndarray, window: int, periodic: bool = True) -> np.ndarray:
@@ -346,22 +390,30 @@
         numpy array same size as input array
 
     """
 
     if window == 1:
         return array
     if not periodic:
-        array_padded = np.c_[array[:, :int(window / 2)][:, :-1], array, array[:, -int(window / 2):][:, :-1]]
-    else:
-        array_padded = np.c_[array[:, -int(np.ceil(window / 2)):], array, array[:, :int(window / 2)]]
+        array_padded = np.c_[
+            array[:, : int(window / 2)][:, :-1],
+            array,
+            array[:, -int(window / 2) :][:, :-1],
+        ]
+    else:
+        array_padded = np.c_[
+            array[:, -int(np.ceil(window / 2)) :], array, array[:, : int(window / 2)]
+        ]
     cumsum = np.cumsum(array_padded, axis=1)
     return (cumsum[:, window:] - cumsum[:, :-window]) / window
 
 
-def bounded_mean_1d(array: np.ndarray, bounds: tuple, weights: Optional[np.ndarray] = None) -> float:
+def bounded_mean_1d(
+    array: np.ndarray, bounds: tuple, weights: Optional[np.ndarray] = None
+) -> float:
     """
     Averages 1D array over region specified by bounds
     Array and weights should be same length
     Todo: Should add interpolation step first?
     Todo: combine with 2d function
 
     Args:
@@ -373,20 +425,35 @@
         single number corresponding to mean value over the bounds specified
 
     """
 
     if weights is None:
         weights = np.ones([len(array)])
     if bounds[0] < bounds[1]:
-        mean = np.average(array[int(len(array) * bounds[0]): int(len(array) * bounds[1] + 1)],
-                          weights=weights[int(len(array) * bounds[0]): int(len(array) * bounds[1] + 1)])
-    else:
-        mean = np.average(np.hstack((array[:int(len(array) * bounds[1] + 1)], array[int(len(array) * bounds[0]):])),
-                          weights=np.hstack(
-                              (weights[:int(len(array) * bounds[1] + 1)], weights[int(len(array) * bounds[0]):])))
+        mean = np.average(
+            array[int(len(array) * bounds[0]) : int(len(array) * bounds[1] + 1)],
+            weights=weights[
+                int(len(array) * bounds[0]) : int(len(array) * bounds[1] + 1)
+            ],
+        )
+    else:
+        mean = np.average(
+            np.hstack(
+                (
+                    array[: int(len(array) * bounds[1] + 1)],
+                    array[int(len(array) * bounds[0]) :],
+                )
+            ),
+            weights=np.hstack(
+                (
+                    weights[: int(len(array) * bounds[1] + 1)],
+                    weights[int(len(array) * bounds[0]) :],
+                )
+            ),
+        )
     return mean
 
 
 def bounded_mean_2d(array: np.ndarray, bounds: tuple) -> np.ndarray:
     """
     Averages 2D array in y dimension over region specified by bounds
     Todo: Should add axis parameter
@@ -398,48 +465,84 @@
 
     Returns:
         one dimensional numpy array of length array.shape[0], corresponding to mean value over the bounds specified
 
     """
 
     if bounds[0] < bounds[1]:
-        mean = np.mean(array[:, int(len(array[0, :]) * bounds[0]): int(len(array[0, :]) * bounds[1])], 1)
+        mean = np.mean(
+            array[
+                :, int(len(array[0, :]) * bounds[0]) : int(len(array[0, :]) * bounds[1])
+            ],
+            1,
+        )
     else:
         mean = np.mean(
-            np.hstack((array[:, :int(len(array[0, :]) * bounds[1])], array[:, int(len(array[0, :]) * bounds[0]):])), 1)
+            np.hstack(
+                (
+                    array[:, : int(len(array[0, :]) * bounds[1])],
+                    array[:, int(len(array[0, :]) * bounds[0]) :],
+                )
+            ),
+            1,
+        )
     return mean
 
 
 ########### MISC FUNCTIONS ###########
 
 
 def asi(mems: np.ndarray, size: float) -> float:
     """
     Calculates asymmetry index based on membrane concentration profile
 
     Args:
         mems: numpy array of membrane concentration values. Periodic array starting from extreme posterior
-        size: size of region to average over when calculating anterior and posterior concentrations (ffrom 0 to 1, where
-        1 indicates the whole embryo)
+        size: size of region to average over when calculating anterior and posterior concentrations (from 0 to 1, where 1 indicates the whole embryo)
 
     Returns:
         asymmetry index
 
     """
 
     ant = bounded_mean_1d(mems, (0.5 - size / 2, 0.5 + size / 2))
     post = bounded_mean_1d(mems, (1 - size / 2, size / 2))
     return (ant - post) / (2 * (ant + post))
 
 
 def dosage(img: np.ndarray, roi: np.ndarray, expand: float) -> np.ndarray:
+    """
+    One way of calculating protein dosage from an image
+
+    Args:
+        img: image 2D numpy array
+        roi: roi representing cell edge (two-column numpy array)
+        expand: expand the ROI by this many pixels before calculating the dosage
+
+    Returns:
+        dosage
+
+    """
+
     return np.nanmean(img * make_mask((512, 512), offset_coordinates(roi, expand)))
 
 
 def make_mask(shape: tuple, roi: np.ndarray) -> np.ndarray:
+    """
+    Create a mask for an image based on an ROI
+
+    Args:
+        shape: shape of the binary mask
+        roi: roi of the mask region
+
+    Returns:
+        binary mask
+
+    """
+
     return cv2.fillPoly(np.zeros(shape) * np.nan, [np.int32(roi)], 1)
 
 
 def readnd(path: str) -> dict:
     """
     Read an nd file
 
@@ -448,49 +551,57 @@
 
     Returns:
         dictionary containing data from nd file
 
     """
 
     nd = {}
-    f = open(path, 'r').readlines()
+    f = open(path, "r").readlines()
     for line in f[:-1]:
-        nd[line.split(', ')[0].replace('"', '')] = line.split(', ')[1].strip().replace('"', '')
+        nd[line.split(", ")[0].replace('"', "")] = (
+            line.split(", ")[1].strip().replace('"', "")
+        )
     return nd
 
 
 def organise_by_nd(path: str):
     """
     Organises images in a folder using the nd files
 
     Args:
         path: path to folder containing nd files
 
     """
-    a = glob.glob(f'{path}/*.nd')
+    a = glob.glob(f"{path}/*.nd")
     for b in a:
         name = os.path.basename(os.path.normpath(b))
-        if name[0] == '_':
+        if name[0] == "_":
             folder = name[1:-3]
         else:
             folder = name[:-3]
-        os.makedirs(f'{path}/{folder}')
-        os.rename(b, f'{path}/{folder}/{name}')
-        for file in glob.glob(f'{b[:-3]}_*'):
-            os.rename(file, f'{path}/{folder}/{os.path.basename(os.path.normpath(file))}')
+        os.makedirs(f"{path}/{folder}")
+        os.rename(b, f"{path}/{folder}/{name}")
+        for file in glob.glob(f"{b[:-3]}_*"):
+            os.rename(
+                file, f"{path}/{folder}/{os.path.basename(os.path.normpath(file))}"
+            )
 
 
-def _direcslist(dest: str, levels: int = 0, exclude: Optional[tuple] = ('!',),
-                exclusive: Optional[tuple] = None) -> list:
-    lis = sorted(glob.glob(f'{dest}/*/'))
+def _direcslist(
+    dest: str,
+    levels: int = 0,
+    exclude: Optional[tuple] = ("!",),
+    exclusive: Optional[tuple] = None,
+) -> list:
+    lis = sorted(glob.glob(f"{dest}/*/"))
 
     for level in range(levels):
         newlis = []
         for e in lis:
-            newlis.extend(sorted(glob.glob(f'{e}/*/')))
+            newlis.extend(sorted(glob.glob(f"{e}/*/")))
         lis = newlis
         lis = [x[:-1] for x in lis]
 
     # Excluded directories
     lis_copy = copy.deepcopy(lis)
     if exclude is not None:
         for x in lis:
@@ -508,16 +619,20 @@
                     lis2.append(x)
     else:
         lis2 = lis_copy
 
     return sorted(lis2)
 
 
-def direcslist(dest: str, levels: int = 0, exclude: Optional[tuple] = ('!',),
-               exclusive: Optional[tuple] = None) -> list:
+def direcslist(
+    dest: str,
+    levels: int = 0,
+    exclude: Optional[tuple] = ("!",),
+    exclusive: Optional[tuple] = None,
+) -> list:
     """
     Gives a list of directories within a given directory (full path)
     Todo: os.walk
 
     Args:
         dest: path of parent directory
         levels: number of levels to go down. E.g. if 0, only return folders within the parent folder; if 1, return
@@ -544,14 +659,15 @@
     Tests whether python is being run within a notebook
 
     https://stackoverflow.com/questions/15411967/how-can-i-check-if-code-is-executed-in-the-ipython-notebook
 
     """
     try:
         from IPython import get_ipython
-        if 'IPKernelApp' not in get_ipython().config:  # pragma: no cover
+
+        if "IPKernelApp" not in get_ipython().config:  # pragma: no cover
             return False
     except ImportError:
         return False
     except AttributeError:
         return False
     return True
```

### Comparing `par_segmentation-0.1.8/par_segmentation/interactive.py` & `par_segmentation-0.1.9/par_segmentation/interactive.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,24 @@
 import ipywidgets as widgets
 from typing import Union, Optional
 from .funcs import in_notebook
 
 
 # TODO: plot_segmentation fails if only one image
 
-def view_stack_tk(frames: Union[list, np.ndarray], start_frame: int = 0, end_frame: Optional[int] = None,
-                  show: bool = True):
+# __all__ = ['view_stack_tk', 'view_stack_jupyter', 'plot_segmentation', 'plot_segmentation_jupyter', 'plot_quantification', 
+#            'plot_quantification_jupyter', 'plot_fits', 'plot_fits_jupyter']
+
+
+def view_stack_tk(
+    frames: Union[list, np.ndarray],
+    start_frame: int = 0,
+    end_frame: Optional[int] = None,
+    show: bool = True,
+):
     """
     Interactive stack viewer
 
     Args:
         frames: either a numpy array of a 2D image or a list of 2D arrays
         start_frame: optional. If speficied only show frames after this index
         end_frame: optional. If specified only show frames before this index
@@ -29,15 +37,17 @@
         stack = True
         frames_ = frames
     elif len(frames.shape) == 3:
         stack = True
         frames_ = list(frames)
     else:
         stack = False
-        frames_ = [frames, ]
+        frames_ = [
+            frames,
+        ]
 
     # Set up figure
     plt.ion()
     fig, ax = plt.subplots()
     plt.subplots_adjust(left=0.25, bottom=0.25)
 
     # Specify ylim
@@ -45,50 +55,58 @@
     vmin = min([np.percentile(i, 0.1) for i in frames_])
 
     # Stack
     if stack:
         axframe = plt.axes([0.25, 0.1, 0.65, 0.03])
         if end_frame is None:
             end_frame = len(frames_)
-        sframe = Slider(axframe, 'Frame', start_frame, end_frame, valinit=start_frame, valfmt='%d')
+        sframe = Slider(
+            axframe, "Frame", start_frame, end_frame, valinit=start_frame, valfmt="%d"
+        )
 
         def update(i):
             ax.clear()
-            ax.imshow(frames_[int(i)], cmap='gray', vmin=vmin, vmax=vmax)
+            ax.imshow(frames_[int(i)], cmap="gray", vmin=vmin, vmax=vmax)
             ax.set_xticks([])
             ax.set_yticks([])
 
         sframe.on_changed(update)
         update(start_frame)
 
     # Single frame
     else:
-        ax.imshow(frames_[0], cmap='gray', vmin=vmin, vmax=vmax)
+        ax.imshow(frames_[0], cmap="gray", vmin=vmin, vmax=vmax)
         ax.set_xticks([])
         ax.set_yticks([])
 
-    fig.canvas.set_window_title('')
+    fig.canvas.set_window_title("")
 
     if show:
         plt.show(block=True)
 
     return fig, ax
 
 
-def view_stack_jupyter(frames: Union[list, np.ndarray], start_frame: int = 0, end_frame: Optional[int] = None):
+def view_stack_jupyter(
+    frames: Union[list, np.ndarray],
+    start_frame: int = 0,
+    end_frame: Optional[int] = None,
+):
     # Detect if single frame or stack
     if type(frames) is list:
         stack = True
         frames_ = frames
     elif len(frames.shape) == 3:
         stack = True
         frames_ = list(frames)
     else:
         stack = False
-        frames_ = [frames, ]
+        frames_ = [
+            frames,
+        ]
 
     # Set up figure
     fig, ax = plt.subplots()
 
     # Specify ylim
     vmax = max([np.percentile(i, 99.9) for i in frames_])
     vmin = min([np.percentile(i, 0.1) for i in frames_])
@@ -97,31 +115,35 @@
     if stack:
         if end_frame is None:
             end_frame = len(frames_) - 1
 
         @widgets.interact(Frame=(start_frame, end_frame, 1))
         def update(Frame=start_frame):
             ax.clear()
-            ax.imshow(frames_[int(Frame)], cmap='gray', vmin=vmin, vmax=vmax)
+            ax.imshow(frames_[int(Frame)], cmap="gray", vmin=vmin, vmax=vmax)
             ax.set_xticks([])
             ax.set_yticks([])
 
     # Single frame
     else:
-        ax.imshow(frames_[0], cmap='gray', vmin=vmin, vmax=vmax)
+        ax.imshow(frames_[0], cmap="gray", vmin=vmin, vmax=vmax)
         ax.set_xticks([])
         ax.set_yticks([])
 
     fig.set_size_inches(4, 4)
     fig.tight_layout()
 
     return fig, ax
 
 
-def view_stack(frames: Union[list, np.ndarray], start_frame: int = 0, end_frame: Optional[int] = None):
+def view_stack(
+    frames: Union[list, np.ndarray],
+    start_frame: int = 0,
+    end_frame: Optional[int] = None,
+):
     jupyter = in_notebook()
     if jupyter:
         view_stack_jupyter(frames, start_frame, end_frame)
     else:
         view_stack_tk(frames, start_frame, end_frame)
 
 
@@ -145,54 +167,57 @@
         stack = True
         frames_ = frames
     elif len(frames.shape) == 3:
         stack = True
         frames_ = list(frames)
     else:
         stack = False
-        frames_ = [frames, ]
+        frames_ = [
+            frames,
+        ]
 
     # Specify ylim
     ylim_top = max([np.percentile(i, 99.9) for i in frames_])
     ylim_bottom = min([np.percentile(i, 0.01) for i in frames_])
 
     # Single frame
     if not stack:
-        ax.imshow(frames_[0], cmap='gray', vmin=ylim_bottom, vmax=ylim_top)
-        ax.plot(rois[:, 0], rois[:, 1], c='lime')
-        ax.scatter(rois[0, 0], rois[0, 1], c='lime')
+        ax.imshow(frames_[0], cmap="gray", vmin=ylim_bottom, vmax=ylim_top)
+        ax.plot(rois[:, 0], rois[:, 1], c="lime")
+        ax.scatter(rois[0, 0], rois[0, 1], c="lime")
         ax.set_xticks([])
         ax.set_yticks([])
 
     # Stack
     else:
-
         # Add frame slider
         plt.subplots_adjust(left=0.25, bottom=0.25)
         axframe = plt.axes([0.25, 0.1, 0.65, 0.03])
-        sframe = Slider(axframe, 'Frame', 0, len(frames_), valinit=0, valfmt='%d')
+        sframe = Slider(axframe, "Frame", 0, len(frames_), valinit=0, valfmt="%d")
 
         def update(i):
             ax.clear()
-            ax.imshow(frames_[int(i)], cmap='gray', vmin=ylim_bottom, vmax=ylim_top)
-            ax.plot(rois[int(i)][:, 0], rois[int(i)][:, 1], c='lime')
-            ax.scatter(rois[int(i)][0, 0], rois[int(i)][0, 1], c='lime')
+            ax.imshow(frames_[int(i)], cmap="gray", vmin=ylim_bottom, vmax=ylim_top)
+            ax.plot(rois[int(i)][:, 0], rois[int(i)][:, 1], c="lime")
+            ax.scatter(rois[int(i)][0, 0], rois[int(i)][0, 1], c="lime")
             ax.set_xticks([])
             ax.set_yticks([])
 
         sframe.on_changed(update)
         update(0)
 
-    fig.canvas.set_window_title('Segmentation')
+    fig.canvas.set_window_title("Segmentation")
     plt.show(block=True)
 
     return fig, ax
 
 
-def plot_segmentation_jupyter(frames: Union[list, np.ndarray], rois: Union[list, np.ndarray]):
+def plot_segmentation_jupyter(
+    frames: Union[list, np.ndarray], rois: Union[list, np.ndarray]
+):
     """
     Plot segmentation results - use this function in a jupyter notebook environment
 
     Args:
         frames: either a numpy array of a 2D image or a list of 2D arrays
         rois: either a single two-column numpy array of ROI coordinates or a list of arrays
 
@@ -208,36 +233,39 @@
         stack = True
         frames_ = frames
     elif len(frames.shape) == 3:
         stack = True
         frames_ = list(frames)
     else:
         stack = False
-        frames_ = [frames, ]
+        frames_ = [
+            frames,
+        ]
 
     # Specify ylim
     ylim_top = max([np.percentile(i, 99.9) for i in frames_])
     ylim_bottom = min([np.percentile(i, 0.01) for i in frames_])
 
     # Single frame
     if not stack:
-        ax.imshow(frames_[0], cmap='gray', vmin=ylim_bottom, vmax=ylim_top)
-        ax.plot(rois[:, 0], rois[:, 1], c='lime')
-        ax.scatter(rois[0, 0], rois[0, 1], c='lime')
+        ax.imshow(frames_[0], cmap="gray", vmin=ylim_bottom, vmax=ylim_top)
+        ax.plot(rois[:, 0], rois[:, 1], c="lime")
+        ax.scatter(rois[0, 0], rois[0, 1], c="lime")
         ax.set_xticks([])
         ax.set_yticks([])
 
     # Stack
     else:
+
         @widgets.interact(Frame=(0, len(frames_) - 1, 1))
         def update(Frame=0):
             ax.clear()
-            ax.imshow(frames_[int(Frame)], cmap='gray', vmin=ylim_bottom, vmax=ylim_top)
-            ax.plot(rois[int(Frame)][:, 0], rois[int(Frame)][:, 1], c='lime')
-            ax.scatter(rois[int(Frame)][0, 0], rois[int(Frame)][0, 1], c='lime')
+            ax.imshow(frames_[int(Frame)], cmap="gray", vmin=ylim_bottom, vmax=ylim_top)
+            ax.plot(rois[int(Frame)][:, 0], rois[int(Frame)][:, 1], c="lime")
+            ax.scatter(rois[int(Frame)][0, 0], rois[int(Frame)][0, 1], c="lime")
             ax.set_xticks([])
             ax.set_yticks([])
 
     fig.set_size_inches(4, 4)
     fig.tight_layout()
 
     return fig, ax
@@ -261,48 +289,49 @@
         stack = True
         mems_ = mems
     elif len(mems.shape) == 2:
         stack = True
         mems_ = list(mems)
     else:
         stack = False
-        mems_ = [mems, ]
+        mems_ = [
+            mems,
+        ]
 
     # Single frame
     if not stack:
         ax.plot(mems_[0])
-        ax.set_xlabel('Position')
-        ax.set_ylabel('Membrane concentration')
+        ax.set_xlabel("Position")
+        ax.set_ylabel("Membrane concentration")
         ax.set_ylim(bottom=min(0, np.min(mems_[0])))
-        ax.axhline(0, c='k', linestyle='--')
+        ax.axhline(0, c="k", linestyle="--")
 
     # Stack
     else:
-
         # Specify ylim
         ylim_top = max([np.max(m) for m in mems_])
         ylim_bottom = min([np.min(m) for m in mems_])
 
         # Add frame silder
         plt.subplots_adjust(left=0.25, bottom=0.25)
         axframe = plt.axes([0.25, 0.1, 0.65, 0.03])
-        sframe = Slider(axframe, 'Frame', 0, len(mems_), valinit=0, valfmt='%d')
+        sframe = Slider(axframe, "Frame", 0, len(mems_), valinit=0, valfmt="%d")
 
         def update(i):
             ax.clear()
             ax.plot(mems_[int(i)])
-            ax.axhline(0, c='k', linestyle='--')
-            ax.set_xlabel('Position')
-            ax.set_ylabel('Membrane concentration')
+            ax.axhline(0, c="k", linestyle="--")
+            ax.set_xlabel("Position")
+            ax.set_ylabel("Membrane concentration")
             ax.set_ylim(min(ylim_bottom, 0), ylim_top)
 
         sframe.on_changed(update)
         update(0)
 
-    fig.canvas.set_window_title('Membrane Quantification')
+    fig.canvas.set_window_title("Membrane Quantification")
     plt.show(block=True)
 
     return fig, ax
 
 
 def plot_quantification_jupyter(mems: Union[list, np.ndarray]):
     """
@@ -322,64 +351,66 @@
         stack = True
         mems_ = mems
     elif len(mems.shape) == 2:
         stack = True
         mems_ = list(mems)
     else:
         stack = False
-        mems_ = [mems, ]
+        mems_ = [
+            mems,
+        ]
 
     # Single frame
     if not stack:
         ax.plot(mems_[0])
-        ax.set_xlabel('Position')
-        ax.set_ylabel('Membrane concentration')
+        ax.set_xlabel("Position")
+        ax.set_ylabel("Membrane concentration")
         ax.set_ylim(bottom=min(0, np.min(mems_[0])))
-        ax.axhline(0, c='k', linestyle='--')
+        ax.axhline(0, c="k", linestyle="--")
 
     # Stack
     else:
-
         # Specify ylim
         ylim_top = max([np.max(m) for m in mems_])
         ylim_bottom = min([np.min(m) for m in mems_] + [0])
 
         @widgets.interact(Frame=(0, len(mems_) - 1, 1))
         def update(Frame=0):
             ax.clear()
             ax.plot(mems_[int(Frame)])
-            ax.axhline(0, c='k', linestyle='--')
-            ax.set_xlabel('Position')
-            ax.set_ylabel('Membrane concentration')
+            ax.axhline(0, c="k", linestyle="--")
+            ax.set_xlabel("Position")
+            ax.set_ylabel("Membrane concentration")
             ax.set_ylim(ylim_bottom, ylim_top)
 
     fig.set_size_inches(5, 3)
     fig.tight_layout()
 
     return fig, ax
 
 
-class FitPlotter:
-    def __init__(self,
-                 target: Union[list, np.ndarray],
-                 fit: Union[list, np.ndarray]):
-
+class _FitPlotter:
+    def __init__(self, target: Union[list, np.ndarray], fit: Union[list, np.ndarray]):
         # Detect if single frame or stack
         if type(target) is list:
             self.stack = True
             target_ = target
             fit_ = fit
         elif len(target.shape) == 3:
             self.stack = True
             target_ = list(target)
             fit_ = list(fit)
         else:
             self.stack = False
-            target_ = [target, ]
-            fit_ = [fit, ]
+            target_ = [
+                target,
+            ]
+            fit_ = [
+                fit,
+            ]
 
         # Internal variables
         self.target = target_
         self.fit = fit_
         self.pos = 10
 
         # Set up figure
@@ -396,61 +427,73 @@
         self.ylim_top = max([straight_max, fit_max])
         self.ylim_bottom = min([straight_min, fit_min])
 
         # Frame slider
         if self.stack:
             plt.subplots_adjust(bottom=0.25, left=0.25)
             axframe = plt.axes([0.25, 0.1, 0.65, 0.03])
-            slider_frame = Slider(axframe, 'Frame', 0, len(self.target), valinit=0, valfmt='%d')
+            slider_frame = Slider(
+                axframe, "Frame", 0, len(self.target), valinit=0, valfmt="%d"
+            )
             slider_frame.on_changed(lambda f: self.update_frame(int(f)))
 
         # Initial plot
         self.update_frame(0)
 
         # Show
-        self.fig.canvas.set_window_title('Local fits')
+        self.fig.canvas.set_window_title("Local fits")
         plt.show(block=True)
 
     def update_pos(self, p: float):
         self.pos = int(p)
         self.ax1_update()
         self.ax2_update()
 
     def update_frame(self, i: int):
         self._target = self.target[i]
         self._fit = self.fit[i]
 
         # Position slider
-        self.slider_pos = Slider(self.ax1, '', 0, len(self._target[0, :]), valinit=self.pos, valfmt='%d',
-                                 facecolor='none', edgecolor='none')
+        self.slider_pos = Slider(
+            self.ax1,
+            "",
+            0,
+            len(self._target[0, :]),
+            valinit=self.pos,
+            valfmt="%d",
+            facecolor="none",
+            edgecolor="none",
+        )
         self.slider_pos.on_changed(self.update_pos)
 
         self.ax1_update()
         self.ax2_update()
 
     def ax1_update(self):
         self.ax1.clear()
-        self.ax1.imshow(self._target, cmap='gray', vmin=self.ylim_bottom, vmax=1.1 * self.ylim_top)
-        self.ax1.axvline(self.pos, c='r')
+        self.ax1.imshow(
+            self._target, cmap="gray", vmin=self.ylim_bottom, vmax=1.1 * self.ylim_top
+        )
+        self.ax1.axvline(self.pos, c="r")
         self.ax1.set_yticks([])
-        self.ax1.set_xlabel('Position')
-        self.ax1.xaxis.set_label_position('top')
+        self.ax1.set_xlabel("Position")
+        self.ax1.xaxis.set_label_position("top")
 
     def ax2_update(self):
         self.ax2.clear()
-        self.ax2.plot(self._target[:, self.pos], label='Actual')
-        self.ax2.plot(self._fit[:, self.pos], label='Fit')
+        self.ax2.plot(self._target[:, self.pos], label="Actual")
+        self.ax2.plot(self._fit[:, self.pos], label="Fit")
         self.ax2.set_xticks([])
-        self.ax2.set_ylabel('Intensity')
-        self.ax2.legend(frameon=False, loc='upper left', fontsize='small')
+        self.ax2.set_ylabel("Intensity")
+        self.ax2.legend(frameon=False, loc="upper left", fontsize="small")
         self.ax2.set_ylim(bottom=self.ylim_bottom, top=self.ylim_top)
 
 
 def plot_fits(target: Union[list, np.ndarray], fit_total: Union[list, np.ndarray]):
-    fp = FitPlotter(target, fit_total)
+    fp = _FitPlotter(target, fit_total)
     return fp.fig, (fp.ax1, fp.ax2)
 
 
 def plot_fits_jupyter(target: Union[list, np.ndarray], fit: Union[list, np.ndarray]):
     # Detect if single frame or stack
     if type(target) is list:
         stack = True
@@ -458,16 +501,20 @@
         fit = fit
     elif len(target.shape) == 3:
         stack = True
         target = list(target)
         fit = list(fit)
     else:
         stack = False
-        target = [target, ]
-        fit = [fit, ]
+        target = [
+            target,
+        ]
+        fit = [
+            fit,
+        ]
 
     # Set up figure
     fig = plt.figure()
     gs = fig.add_gridspec(3, 3)
     ax1 = fig.add_subplot(gs[0, :])
     ax2 = fig.add_subplot(gs[1:, :])
 
@@ -482,46 +529,48 @@
     if stack:
 
         @widgets.interact(Frame=(0, len(target) - 1, 1), Position=(0, 1, 0.01))
         def update(Frame: int = 0, Position: float = 0.1):
             position = int(Position * target[int(Frame)].shape[1] - 1)
 
             ax1.clear()
-            ax1.imshow(target[int(Frame)], cmap='gray', vmin=ylim_bottom, vmax=1.1 * ylim_top)
-            ax1.axvline(position, c='r')
+            ax1.imshow(
+                target[int(Frame)], cmap="gray", vmin=ylim_bottom, vmax=1.1 * ylim_top
+            )
+            ax1.axvline(position, c="r")
             ax1.set_yticks([])
-            ax1.set_xlabel('Position')
-            ax1.xaxis.set_label_position('top')
+            ax1.set_xlabel("Position")
+            ax1.xaxis.set_label_position("top")
 
             ax2.clear()
-            ax2.plot(target[int(Frame)][:, position], label='Actual')
-            ax2.plot(fit[int(Frame)][:, position], label='Fit')
+            ax2.plot(target[int(Frame)][:, position], label="Actual")
+            ax2.plot(fit[int(Frame)][:, position], label="Fit")
             ax2.set_xticks([])
-            ax2.set_ylabel('Intensity')
-            ax2.legend(frameon=False, loc='upper left', fontsize='small')
+            ax2.set_ylabel("Intensity")
+            ax2.legend(frameon=False, loc="upper left", fontsize="small")
             ax2.set_ylim(bottom=ylim_bottom, top=ylim_top)
 
     else:
 
         @widgets.interact(Position=(0, 1, 0.01))
         def update(Position: float = 0.1):
             position = int(Position * (target[0].shape[1] - 1))
 
             ax1.clear()
-            ax1.imshow(target[0], cmap='gray', vmin=ylim_bottom, vmax=1.1 * ylim_top)
-            ax1.axvline(position, c='r')
+            ax1.imshow(target[0], cmap="gray", vmin=ylim_bottom, vmax=1.1 * ylim_top)
+            ax1.axvline(position, c="r")
             ax1.set_yticks([])
-            ax1.set_xlabel('Position')
-            ax1.xaxis.set_label_position('top')
+            ax1.set_xlabel("Position")
+            ax1.xaxis.set_label_position("top")
 
             ax2.clear()
-            ax2.plot(target[0][:, position], label='Actual')
-            ax2.plot(fit[0][:, position], label='Fit')
+            ax2.plot(target[0][:, position], label="Actual")
+            ax2.plot(fit[0][:, position], label="Fit")
             ax2.set_xticks([])
-            ax2.set_ylabel('Intensity')
-            ax2.legend(frameon=False, loc='upper left', fontsize='small')
+            ax2.set_ylabel("Intensity")
+            ax2.legend(frameon=False, loc="upper left", fontsize="small")
             ax2.set_ylim(bottom=ylim_bottom, top=ylim_top)
 
     fig.set_size_inches(5, 3)
     fig.tight_layout()
 
     return fig, (ax1, ax2)
```

### Comparing `par_segmentation-0.1.8/par_segmentation/legacy.py` & `par_segmentation-0.1.9/par_segmentation/legacy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 import time
 import numpy as np
 from scipy.optimize import differential_evolution
 from joblib import Parallel, delayed
 import multiprocessing
-from .funcs import straighten, rolling_ave_2d, interp_1d_array, interp_2d_array, rotate_roi
+from .funcs import (
+    straighten,
+    rolling_ave_2d,
+    interp_1d_array,
+    interp_2d_array,
+    rotate_roi,
+)
 from scipy.special import erf
 from .roi import interp_roi, offset_coordinates, spline_roi
 from typing import Union, Optional, Tuple
 import cv2
 
 """
 Legacy code including differential evolution algorithm and other functions no longer used
 
 """
 
+__all__ = ['gaus', 'error_func', 'polycrop', 'bg_subtraction']
+
 
 class ImageQuantDifferentialEvolutionSingle:
     """
     Quantification works by taking cross-sections across the membrane, and fitting the resulting profile as the sum of
     a cytoplasmic signal component and a membrane signal component. Differential evolution algorithm
 
     Input data:
@@ -49,32 +57,33 @@
 
     Saving:
     save_path          destination to save results, will create if it doesn't already exist
 
 
     """
 
-    def __init__(self,
-                 img: Union[np.ndarray, list],
-                 sigma: float = 2.0,
-                 roi: Union[np.ndarray, list] = None,
-                 freedom: float = 0.5,
-                 periodic: bool = True,
-                 thickness: int = 50,
-                 itp: int = 10,
-                 rol_ave: int = 10,
-                 parallel: bool = False,
-                 cores: Optional[int] = None,
-                 rotate: bool = False,
-                 zerocap: bool = True,
-                 nfits: Optional[int] = None,
-                 iterations: int = 2,
-                 interp: str = 'cubic',
-                 bg_subtract: bool = False):
-
+    def __init__(
+        self,
+        img: Union[np.ndarray, list],
+        sigma: float = 2.0,
+        roi: Union[np.ndarray, list] = None,
+        freedom: float = 0.5,
+        periodic: bool = True,
+        thickness: int = 50,
+        itp: int = 10,
+        rol_ave: int = 10,
+        parallel: bool = False,
+        cores: Optional[int] = None,
+        rotate: bool = False,
+        zerocap: bool = True,
+        nfits: Optional[int] = None,
+        iterations: int = 2,
+        interp: str = "cubic",
+        bg_subtract: bool = False,
+    ):
         # Image / stack
         self.img = img
 
         # ROI
         self.roi_init = roi
         self.roi = roi
         self.periodic = periodic
@@ -92,19 +101,30 @@
         self.rotate = rotate
         self.zerocap = zerocap
         self.sigma = sigma
         self.nfits = nfits
         self.interp = interp
 
         # Background curves
-        self.cytbg = (1 + error_func(np.arange(thickness * 2), thickness, (self.sigma * np.sqrt(2)))) / 2
-        self.cytbg_itp = (1 + error_func(np.arange(2 * self.thickness_itp), self.thickness_itp,
-                                         (self.sigma * np.sqrt(2)) * self.itp)) / 2
+        self.cytbg = (
+            1
+            + error_func(np.arange(thickness * 2), thickness, (self.sigma * np.sqrt(2)))
+        ) / 2
+        self.cytbg_itp = (
+            1
+            + error_func(
+                np.arange(2 * self.thickness_itp),
+                self.thickness_itp,
+                (self.sigma * np.sqrt(2)) * self.itp,
+            )
+        ) / 2
         self.membg = gaus(np.arange(thickness * 2), thickness, self.sigma)
-        self.membg_itp = gaus(np.arange(2 * self.thickness_itp), self.thickness_itp, self.sigma * self.itp)
+        self.membg_itp = gaus(
+            np.arange(2 * self.thickness_itp), self.thickness_itp, self.sigma * self.itp
+        )
 
         # Computation
         self.parallel = parallel
         if cores is not None:
             self.cores = cores
         else:
             self.cores = multiprocessing.cpu_count()
@@ -127,27 +147,25 @@
             self.reset_res()
 
     """
     Run
     """
 
     def run(self):
-
         # Fitting
         for i in range(self.iterations):
             if i > 0:
                 self.adjust_roi()
                 self.reset_res()
             self.fit()
 
         # Simulate images
         self.sim_images()
 
     def fit(self):
-
         # Specify number of fits
         if self.nfits is None:
             self.nfits = len(self.roi[:, 0])
 
         # Straighten image
         self.straight = straighten(self.img, self.roi, self.thickness)
 
@@ -155,55 +173,82 @@
         if self.bg_subtract:
             bg_intensity = np.mean(self.straight[:5, :])
             self.straight -= bg_intensity
             self.img -= bg_intensity
 
         # Smoothen
         if self.rol_ave != 0:
-            self.straight_filtered = rolling_ave_2d(self.straight, self.rol_ave, self.periodic)
+            self.straight_filtered = rolling_ave_2d(
+                self.straight, self.rol_ave, self.periodic
+            )
         else:
             self.straight_filtered = self.straight
 
         # Interpolate
-        straight = interp_2d_array(self.straight_filtered, self.thickness_itp, method=self.interp)
+        straight = interp_2d_array(
+            self.straight_filtered, self.thickness_itp, method=self.interp
+        )
         straight = interp_2d_array(straight, self.nfits, ax=1, method=self.interp)
 
         # Fit
         if self.parallel:
-            results = np.array(Parallel(n_jobs=self.cores)(
-                delayed(self._fit_profile)(straight[:, x]) for x in range(len(straight[0, :]))))
+            results = np.array(
+                Parallel(n_jobs=self.cores)(
+                    delayed(self._fit_profile)(straight[:, x])
+                    for x in range(len(straight[0, :]))
+                )
+            )
             self.offsets = results[:, 0]
             self.cyts = results[:, 1]
             self.mems = results[:, 2]
         else:
             for x in range(len(straight[0, :])):
-                self.offsets[x], self.cyts[x], self.mems[x] = self._fit_profile(straight[:, x])
+                self.offsets[x], self.cyts[x], self.mems[x] = self._fit_profile(
+                    straight[:, x]
+                )
 
         # Interpolate
-        self.offsets_full = interp_1d_array(self.offsets, len(self.roi[:, 0]), method='linear')
-        self.cyts_full = interp_1d_array(self.cyts, len(self.roi[:, 0]), method='linear')
-        self.mems_full = interp_1d_array(self.mems, len(self.roi[:, 0]), method='linear')
+        self.offsets_full = interp_1d_array(
+            self.offsets, len(self.roi[:, 0]), method="linear"
+        )
+        self.cyts_full = interp_1d_array(
+            self.cyts, len(self.roi[:, 0]), method="linear"
+        )
+        self.mems_full = interp_1d_array(
+            self.mems, len(self.roi[:, 0]), method="linear"
+        )
 
     def _fit_profile(self, profile: np.ndarray) -> Tuple[float, float, float]:
         if self.zerocap:
             bounds = (
-                ((self.thickness_itp / 2) * (1 - self.freedom), (self.thickness_itp / 2) * (1 + self.freedom)),
-                (0, max(2 * max(profile), 0)), (0, max(2 * max(profile), 0)))
+                (
+                    (self.thickness_itp / 2) * (1 - self.freedom),
+                    (self.thickness_itp / 2) * (1 + self.freedom),
+                ),
+                (0, max(2 * max(profile), 0)),
+                (0, max(2 * max(profile), 0)),
+            )
         else:
             bounds = (
-                ((self.thickness_itp / 2) * (1 - self.freedom), (self.thickness_itp / 2) * (1 + self.freedom)),
-                (-0.2 * max(profile), 2 * max(profile)), (-0.2 * max(profile), 2 * max(profile)))
+                (
+                    (self.thickness_itp / 2) * (1 - self.freedom),
+                    (self.thickness_itp / 2) * (1 + self.freedom),
+                ),
+                (-0.2 * max(profile), 2 * max(profile)),
+                (-0.2 * max(profile), 2 * max(profile)),
+            )
         res = differential_evolution(self._mse, bounds=bounds, args=(profile,), tol=0.2)
         o = (res.x[0] - self.thickness_itp / 2) / self.itp
         return o, res.x[1], res.x[2]
 
     def _mse(self, l_c_m: list, profile: np.ndarray) -> np.ndarray:
         l, c, m = l_c_m
-        y = (c * self.cytbg_itp[int(l):int(l) + self.thickness_itp]) + (
-                m * self.membg_itp[int(l):int(l) + self.thickness_itp])
+        y = (c * self.cytbg_itp[int(l) : int(l) + self.thickness_itp]) + (
+            m * self.membg_itp[int(l) : int(l) + self.thickness_itp]
+        )
         return np.mean((profile - y) ** 2)
 
     """
     Misc
 
     """
 
@@ -213,16 +258,19 @@
 
         """
         for x in range(len(self.roi[:, 0])):
             c = self.cyts_full[x]
             m = self.mems_full[x]
             l = int(self.offsets_full[x] * self.itp + (self.thickness_itp / 2))
             self.straight_fit[:, x] = interp_1d_array(
-                (c * self.cytbg_itp[l:l + self.thickness_itp]) + (m * self.membg_itp[l:l + self.thickness_itp]),
-                self.thickness, method=self.interp)
+                (c * self.cytbg_itp[l : l + self.thickness_itp])
+                + (m * self.membg_itp[l : l + self.thickness_itp]),
+                self.thickness,
+                method=self.interp,
+            )
             self.straight_resids[:, x] = self.straight[:, x] - self.straight_fit[:, x]
 
     def adjust_roi(self):
         """
         Can do after a preliminary fit to refine coordinates
         Must refit after doing this
 
@@ -274,64 +322,83 @@
         self.straight = np.zeros([self.thickness, len(self.roi[:, 0])])
         self.straight_filtered = np.zeros([self.thickness, len(self.roi[:, 0])])
         self.straight_fit = np.zeros([self.thickness, len(self.roi[:, 0])])
         self.straight_resids = np.zeros([self.thickness, len(self.roi[:, 0])])
 
 
 class ImageQuantDifferentialEvolutionMulti:
-    def __init__(self,
-                 img: Union[np.ndarray, list],
-                 roi: Union[np.ndarray, list] = None,
-                 sigma: float = 2.0,
-                 periodic: bool = True,
-                 thickness: int = 50,
-                 freedom: float = 0.5,
-                 itp: int = 10,
-                 rol_ave: int = 10,
-                 parallel: bool = False,
-                 cores: Optional[int] = None,
-                 rotate: bool = False,
-                 zerocap: bool = True,
-                 nfits: Optional[int] = None,
-                 iterations: int = 1,
-                 interp: str = 'cubic',
-                 bg_subtract: bool = False,
-                 verbose: bool = True):
-
+    def __init__(
+        self,
+        img: Union[np.ndarray, list],
+        roi: Union[np.ndarray, list] = None,
+        sigma: float = 2.0,
+        periodic: bool = True,
+        thickness: int = 50,
+        freedom: float = 0.5,
+        itp: int = 10,
+        rol_ave: int = 10,
+        parallel: bool = False,
+        cores: Optional[int] = None,
+        rotate: bool = False,
+        zerocap: bool = True,
+        nfits: Optional[int] = None,
+        iterations: int = 1,
+        interp: str = "cubic",
+        bg_subtract: bool = False,
+        verbose: bool = True,
+    ):
         # Detect if single frame or stack
         if type(img) is list:
             self.stack = True
             self.img = img
         elif len(img.shape) == 3:
             self.stack = True
             self.img = list(img)
         else:
             self.stack = False
-            self.img = [img, ]
+            self.img = [
+                img,
+            ]
         self.n = len(self.img)
 
         # ROI
         if not self.stack:
-            self.roi = [roi, ]
+            self.roi = [
+                roi,
+            ]
         elif type(roi) is list:
             if len(roi) > 1:
                 self.roi = roi
             else:
                 self.roi = roi * self.n
         else:
             self.roi = [roi] * self.n
 
         # Set up list of classes
         self.iq = [
-            ImageQuantDifferentialEvolutionSingle(img=i, roi=r, sigma=sigma, periodic=periodic, thickness=thickness,
-                                                  freedom=freedom, itp=itp, rol_ave=rol_ave, parallel=parallel,
-                                                  cores=cores, rotate=rotate, zerocap=zerocap, nfits=nfits,
-                                                  iterations=iterations, interp=interp,
-                                                  bg_subtract=bg_subtract) for i, r in
-            zip(self.img, self.roi)]
+            ImageQuantDifferentialEvolutionSingle(
+                img=i,
+                roi=r,
+                sigma=sigma,
+                periodic=periodic,
+                thickness=thickness,
+                freedom=freedom,
+                itp=itp,
+                rol_ave=rol_ave,
+                parallel=parallel,
+                cores=cores,
+                rotate=rotate,
+                zerocap=zerocap,
+                nfits=nfits,
+                iterations=iterations,
+                interp=interp,
+                bg_subtract=bg_subtract,
+            )
+            for i, r in zip(self.img, self.roi)
+        ]
 
         # Initial results containers
         self.mems = [None] * self.n
         self.cyts = [None] * self.n
         self.offsets = [None] * self.n
         self.mems_full = [None] * self.n
         self.cyts_full = [None] * self.n
@@ -345,15 +412,15 @@
 
     def run(self):
         t = time.time()
 
         # Run
         for i, iq in enumerate(self.iq):
             if self.verbose:
-                print(f'Quantifying image {i + 1} of {self.n}')
+                print(f"Quantifying image {i + 1} of {self.n}")
             iq.run()
 
         # Save membrane/cytoplasmic quantification, offsets
         self.mems[:] = [iq.mems for iq in self.iq]
         self.cyts[:] = [iq.cyts for iq in self.iq]
         self.offsets[:] = [iq.offsets for iq in self.iq]
         self.mems_full[:] = [iq.mems_full for iq in self.iq]
@@ -365,15 +432,15 @@
 
         # Save target/simulated/residuals images
         self.target_full[:] = [iq.straight_filtered for iq in self.iq]
         self.sim_full[:] = [iq.straight_fit for iq in self.iq]
         self.resids_full[:] = [iq.straight_resids for iq in self.iq]
 
         if self.verbose:
-            print('Time elapsed: %.2f seconds ' % (time.time() - t))
+            print("Time elapsed: %.2f seconds " % (time.time() - t))
 
 
 def gaus(x: np.ndarray, centre: float, width: float) -> np.ndarray:
     """
     Create Gaussian curve with centre and width specified
 
     Args:
@@ -382,15 +449,15 @@
         width: width of the gaussian curve (in x units)
 
     Returns:
         Gaussian curve
 
     """
 
-    return np.exp(-((x - centre) ** 2) / (2 * width ** 2))
+    return np.exp(-((x - centre) ** 2) / (2 * width**2))
 
 
 def error_func(x: np.ndarray, centre: float, width: float) -> np.ndarray:
     """
     Create error function with centre and width specified
 
     Args:
@@ -416,22 +483,26 @@
         enlarge: amount by which to expand or contract the ROI (pixel units)
 
     Returns:
         numpy array of same shape img, with regions outside of polyline set to zero
 
     """
 
-    newcoors = np.int32(offset_coordinates(polyline, enlarge * np.ones([len(polyline[:, 0])])))
+    newcoors = np.int32(
+        offset_coordinates(polyline, enlarge * np.ones([len(polyline[:, 0])]))
+    )
     mask = np.zeros(img.shape)
     mask = cv2.fillPoly(mask, [newcoors], 1)
     newimg = img * mask
     return newimg
 
 
-def bg_subtraction(img: np.ndarray, roi: np.ndarray, band: tuple = (25, 75)) -> np.ndarray:
+def bg_subtraction(
+    img: np.ndarray, roi: np.ndarray, band: tuple = (25, 75)
+) -> np.ndarray:
     """
 
     Subtracts background intensity from an image of a cell. Background intensity calculated as the mean intensity within
     a band surronding the cell (specified by ROI)
 
     Args:
         img: numpy array of image to subtract background from
@@ -452,9 +523,9 @@
     r2 = (max(normcoors[:, 1]) - min(normcoors[:, 1])) / 2
     return (4 / 3) * np.pi * r2 * r2 * r1
 
 
 def calc_sa(normcoors: np.ndarray) -> float:
     r1 = (max(normcoors[:, 0]) - min(normcoors[:, 0])) / 2
     r2 = (max(normcoors[:, 1]) - min(normcoors[:, 1])) / 2
-    e = (1 - (r2 ** 2) / (r1 ** 2)) ** 0.5
+    e = (1 - (r2**2) / (r1**2)) ** 0.5
     return 2 * np.pi * r2 * r2 * (1 + (r1 / (r2 * e)) * np.arcsin(e))
```

### Comparing `par_segmentation-0.1.8/par_segmentation/model.py` & `par_segmentation-0.1.9/par_segmentation/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,64 +1,76 @@
 import numpy as np
 import tensorflow as tf
-from .funcs import straighten, rolling_ave_2d, interp_1d_array, interp_2d_array, rotate_roi
+from .funcs import (
+    straighten,
+    rolling_ave_2d,
+    interp_1d_array,
+    interp_2d_array,
+    rotate_roi,
+)
 from .roi import offset_coordinates, interp_roi
 from scipy.interpolate import interp1d
 from tqdm import tqdm
 import time
-from .tgf_interpolate import interpolate
+from ._tgf_interpolate import interpolate
 import matplotlib.pyplot as plt
 from typing import Union, Tuple
 
 """
 To do:
 - use a spline based method for nfits
 
 """
 
+# __all__ = ['ImageQuantGradientDescent', 'create_offsets_spline']
 
-class ImageQuantGradientDescent:
-
-    def __init__(self,
-                 img: Union[np.ndarray, list],
-                 roi: Union[np.ndarray, list],
-                 sigma: float = 3.5,
-                 periodic: bool = True,
-                 thickness: int = 50,
-                 rol_ave: int = 5,
-                 rotate: bool = False,
-                 nfits: Union[int, None] = 100,
-                 iterations: int = 2,
-                 lr: float = 0.01,
-                 descent_steps: int = 300,
-                 adaptive_sigma: bool = False,
-                 batch_norm: bool = False,
-                 freedom: float = 10,
-                 roi_knots: int = 20,
-                 fit_outer: bool = True,
-                 zerocap: bool = False,
-                 save_training: bool = False,
-                 save_sims: bool = False,
-                 verbose: bool = True):
 
+class ImageQuantGradientDescent:
+    def __init__(
+        self,
+        img: Union[np.ndarray, list],
+        roi: Union[np.ndarray, list],
+        sigma: float = 3.5,
+        periodic: bool = True,
+        thickness: int = 50,
+        rol_ave: int = 5,
+        rotate: bool = False,
+        nfits: Union[int, None] = 100,
+        iterations: int = 2,
+        lr: float = 0.01,
+        descent_steps: int = 300,
+        adaptive_sigma: bool = False,
+        batch_norm: bool = False,
+        freedom: float = 10,
+        roi_knots: int = 20,
+        fit_outer: bool = True,
+        zerocap: bool = False,
+        save_training: bool = False,
+        save_sims: bool = False,
+        verbose: bool = True,
+    ):
         # Detect if single frame or stack
         if type(img) is list:
             self.stack = True
             self.img = img
         elif len(img.shape) == 3:
             self.stack = True
             self.img = list(img)
         else:
             self.stack = False
-            self.img = [img, ]
+            self.img = [
+                img,
+            ]
         self.n = len(self.img)
 
         # ROI
         if not self.stack:
-            self.roi = [roi, ]
+            self.roi = [
+                roi,
+            ]
         elif type(roi) is list:
             if len(roi) > 1:
                 self.roi = roi
             else:
                 self.roi = roi * self.n
         else:
             self.roi = [roi] * self.n
@@ -109,53 +121,59 @@
 
     def run(self):
         t = time.time()
 
         # Fitting
         for i in range(self.iterations):
             if self.verbose:
-                print(f'Iteration {i + 1} of {self.iterations}')
+                print(f"Iteration {i + 1} of {self.iterations}")
             time.sleep(0.1)
 
             if i > 0:
                 self.adjust_roi()
             self.fit()
 
         if self.verbose:
             time.sleep(0.1)
-            print('Time elapsed: %.2f seconds \n' % (time.time() - t))
+            print("Time elapsed: %.2f seconds \n" % (time.time() - t))
 
-    def preprocess(self, frame: np.ndarray, roi: np.ndarray) -> Tuple[np.ndarray, float, np.ndarray]:
+    def preprocess(
+        self, frame: np.ndarray, roi: np.ndarray
+    ) -> Tuple[np.ndarray, float, np.ndarray]:
         """
         Preprocesses a single image with roi specified
 
         Steps:
         - Straighten according to ROI
         - Apply rolling average
         - Either interpolated to a common length (self.nfits) or pad to length of largest image if nfits is not speficied
         - Normalise images, either to themselves or globally
 
         """
 
         # Straighten
-        straight = straighten(frame, roi, thickness=self.thickness, interp='cubic', periodic=self.periodic)
+        straight = straighten(
+            frame, roi, thickness=self.thickness, interp="cubic", periodic=self.periodic
+        )
 
         # Smoothen (rolling average)
         straight = rolling_ave_2d(straight, window=self.rol_ave, periodic=self.periodic)
 
         # Interpolate to a length nfits
         if self.nfits is not None:
-            straight = interp_2d_array(straight, self.nfits, ax=1, method='cubic')
+            straight = interp_2d_array(straight, self.nfits, ax=1, method="cubic")
 
         # If nfits not specified, pad smaller images to size of largest image
         if self.nfits is None:
             pad_size = max([r.shape[0] for r in self.roi])
-            target = np.pad(straight, pad_width=((0, 0), (0, (pad_size - straight.shape[1]))))
+            target = np.pad(
+                straight, pad_width=((0, 0), (0, (pad_size - straight.shape[1])))
+            )
             mask = np.zeros(pad_size)
-            mask[:straight.shape[1]] = 1
+            mask[: straight.shape[1]] = 1
         else:
             mask = np.ones(self.nfits)
             target = straight
 
         # Normalise
         if not self.batch_norm:
             norm = np.percentile(straight, 99)
@@ -172,35 +190,37 @@
 
         """
 
         nimages = self.target.shape[0]
         self.vars = {}
 
         # Offsets
-        self.offsets_t = tf.Variable(np.zeros([nimages, self.roi_knots]), name='Offsets')
+        self.offsets_t = tf.Variable(
+            np.zeros([nimages, self.roi_knots]), name="Offsets"
+        )
         if not self.freedom == 0:
-            self.vars['offsets'] = self.offsets_t
+            self.vars["offsets"] = self.offsets_t
 
         # Cytoplasmic concentrations
         self.cyts_t = tf.Variable(0 * np.mean(self.target[:, -5:, :], axis=1))
-        self.vars['cyts'] = self.cyts_t
+        self.vars["cyts"] = self.cyts_t
 
         # Membrane concentrations
         self.mems_t = tf.Variable(0 * np.max(self.target, axis=1))
-        self.vars['mems'] = self.mems_t
+        self.vars["mems"] = self.mems_t
 
         # Outers
         if self.fit_outer:
             self.outers_t = tf.Variable(0 * np.mean(self.target[:, :5, :], axis=1))
-            self.vars['outers'] = self.outers_t
+            self.vars["outers"] = self.outers_t
 
         # Sigma
         self.sigma_t = tf.Variable(self.sigma, dtype=tf.float64)
         if self.adaptive_sigma:
-            self.vars['sigma'] = self.sigma_t
+            self.vars["sigma"] = self.sigma_t
 
     def sim_images(self) -> Tuple[tf.Tensor, tf.Tensor]:
         """
         Simulates images according to current membrane and cytoplasm concentration estimates and offsets
 
         """
 
@@ -216,73 +236,90 @@
         mems = self.mems_t
         cyts = self.cyts_t
         if self.zerocap:
             mems = mems * tf.math.sigmoid(self.swish_factor * mems)
             cyts = cyts * tf.math.sigmoid(self.swish_factor * cyts)
 
         # Create offsets spline
-        offsets_spline = create_offsets_spline(self.offsets_t, self.roi_knots, self.periodic, self.n, self.nfits,
-                                               self.roi)
+        offsets_spline = create_offsets_spline(
+            self.offsets_t, self.roi_knots, self.periodic, self.n, self.nfits, self.roi
+        )
 
         # Constrain offsets
         offsets = self.freedom * tf.math.tanh(offsets_spline)
 
         # Positions to evaluate mem and cyt curves
-        positions_ = np.arange(self.thickness, dtype=np.float64)[tf.newaxis, tf.newaxis, :]
+        positions_ = np.arange(self.thickness, dtype=np.float64)[
+            tf.newaxis, tf.newaxis, :
+        ]
         offsets_ = offsets[:, :, tf.newaxis]
         positions = tf.reshape(tf.math.add(positions_, offsets_), [-1])
 
         # Cap positions off edge
         positions = tf.minimum(positions, self.thickness - 1.000001)
         positions = tf.maximum(positions, 0)
 
         # Mask
-        mask = 1 - (tf.cast(tf.math.less(positions, 0), tf.float64) + tf.cast(
-            tf.math.greater(positions, self.thickness), tf.float64))
+        mask = 1 - (
+            tf.cast(tf.math.less(positions, 0), tf.float64)
+            + tf.cast(tf.math.greater(positions, self.thickness), tf.float64)
+        )
         mask_ = tf.reshape(mask, [nimages, nfits, self.thickness])
 
         # Mem curve
-        mem_curve = tf.math.exp(-((positions - self.thickness / 2) ** 2) / (2 * self.sigma_t ** 2))
+        mem_curve = tf.math.exp(
+            -((positions - self.thickness / 2) ** 2) / (2 * self.sigma_t**2)
+        )
         mem_curve = tf.reshape(mem_curve, [nimages, nfits, self.thickness])
 
         # Cyt curve
-        cyt_curve = (1 + tf.math.erf((positions - self.thickness / 2) / (self.sigma_t * (2 ** 0.5)))) / 2
+        cyt_curve = (
+            1
+            + tf.math.erf(
+                (positions - self.thickness / 2) / (self.sigma_t * (2**0.5))
+            )
+        ) / 2
         # self.sigma_t * (2 ** 0.5) <- this is what happens when a step is convolved with a Gaussian
         cyt_curve = tf.reshape(cyt_curve, [nimages, nfits, self.thickness])
 
         # Calculate output
         mem_total = mem_curve * tf.expand_dims(mems, axis=-1)
         if not self.fit_outer:
             cyt_total = cyt_curve * tf.expand_dims(cyts, axis=-1)
         else:
-            cyt_total = tf.expand_dims(self.outers_t, axis=-1) + cyt_curve * tf.expand_dims((cyts - self.outers_t),
-                                                                                            axis=-1)
+            cyt_total = tf.expand_dims(
+                self.outers_t, axis=-1
+            ) + cyt_curve * tf.expand_dims((cyts - self.outers_t), axis=-1)
         # Sum outputs
-        return tf.transpose(tf.math.add(mem_total, cyt_total), [0, 2, 1]), tf.transpose(mask_, [0, 2, 1])
+        return tf.transpose(tf.math.add(mem_total, cyt_total), [0, 2, 1]), tf.transpose(
+            mask_, [0, 2, 1]
+        )
 
     def losses_full(self) -> tf.Tensor:
-
         # Simulate images
         self.sim, mask = self.sim_images()
 
         # Calculate errors
         sq_errors = (self.sim - self.target) ** 2
 
         # Masking (when different size images are used)
         if self.nfits is None:
             mask *= tf.expand_dims(self.masks, axis=1)
 
         # Masked average
-        mse = tf.reduce_sum(sq_errors * mask, axis=[1, 2]) / tf.reduce_sum(mask, axis=[1, 2])
+        mse = tf.reduce_sum(sq_errors * mask, axis=[1, 2]) / tf.reduce_sum(
+            mask, axis=[1, 2]
+        )
         return mse
 
     def fit(self):
-
         # Preprocess
-        target, norms, masks = zip(*[self.preprocess(frame, roi) for frame, roi in zip(self.img, self.roi)])
+        target, norms, masks = zip(
+            *[self.preprocess(frame, roi) for frame, roi in zip(self.img, self.roi)]
+        )
         self.target = np.array(target)
         self.norms = np.array(norms)
         self.masks = np.array(masks)
 
         # Batch normalise
         if self.batch_norm:
             norm = np.percentile(self.target, 99)
@@ -312,66 +349,91 @@
             # Save trained variables
             if self.save_training:
                 newdict = {key: value.numpy() for key, value in self.vars.items()}
                 self.saved_vars.append(newdict)
 
             # Save interim simulations
             if self.save_sims:
-                self.saved_sims.append(self.sim.numpy() * self.norms[:, np.newaxis, np.newaxis])
+                self.saved_sims.append(
+                    self.sim.numpy() * self.norms[:, np.newaxis, np.newaxis]
+                )
 
         # Save and rescale sim images (rescaled)
-        self.sim_both = self.sim_images()[0].numpy() * self.norms[:, np.newaxis, np.newaxis]
+        self.sim_both = (
+            self.sim_images()[0].numpy() * self.norms[:, np.newaxis, np.newaxis]
+        )
         self.target = self.target * self.norms[:, np.newaxis, np.newaxis]
 
         # Save and rescale results
         mems = self.mems_t
         cyts = self.cyts_t
         if self.zerocap:
             mems = mems * tf.math.sigmoid(self.swish_factor * mems)
             cyts = cyts * tf.math.sigmoid(self.swish_factor * cyts)
         self.mems = mems.numpy() * self.norms[:, np.newaxis]
         self.cyts = cyts.numpy() * self.norms[:, np.newaxis]
 
         # Create offsets spline
-        offsets_spline = create_offsets_spline(self.offsets_t, self.roi_knots, self.periodic, self.n, self.nfits,
-                                               self.roi)
+        offsets_spline = create_offsets_spline(
+            self.offsets_t, self.roi_knots, self.periodic, self.n, self.nfits, self.roi
+        )
 
         # Constrain offsets
         self.offsets = self.freedom * tf.math.tanh(offsets_spline)
 
         # Crop results
         if self.nfits is None:
-            self.offsets = [offsets[mask == 1] for offsets, mask in zip(self.offsets, self.masks)]
+            self.offsets = [
+                offsets[mask == 1] for offsets, mask in zip(self.offsets, self.masks)
+            ]
             self.cyts = [cyts[mask == 1] for cyts, mask in zip(self.cyts, self.masks)]
             self.mems = [mems[mask == 1] for mems, mask in zip(self.mems, self.masks)]
 
         # Interpolated results
         if self.nfits is not None:
-            self.offsets_full = [interp_1d_array(offsets, len(roi[:, 0]), method='cubic') for offsets, roi in
-                                 zip(self.offsets, self.roi)]
-            self.cyts_full = [interp_1d_array(cyts, len(roi[:, 0]), method='linear') for cyts, roi in
-                              zip(self.cyts, self.roi)]
-            self.mems_full = [interp_1d_array(mems, len(roi[:, 0]), method='linear') for mems, roi in
-                              zip(self.mems, self.roi)]
+            self.offsets_full = [
+                interp_1d_array(offsets, len(roi[:, 0]), method="cubic")
+                for offsets, roi in zip(self.offsets, self.roi)
+            ]
+            self.cyts_full = [
+                interp_1d_array(cyts, len(roi[:, 0]), method="linear")
+                for cyts, roi in zip(self.cyts, self.roi)
+            ]
+            self.mems_full = [
+                interp_1d_array(mems, len(roi[:, 0]), method="linear")
+                for mems, roi in zip(self.mems, self.roi)
+            ]
         else:
             self.offsets_full = self.offsets
             self.cyts_full = self.cyts
             self.mems_full = self.mems
 
         # Interpolated sim images
         if self.nfits is not None:
-            self.sim_full = [interp1d(np.arange(self.nfits), sim_both, axis=-1)(
-                np.linspace(0, self.nfits - 1, len(roi[:, 0]))) for roi, sim_both in
-                zip(self.roi, self.sim_both)]
-            self.target_full = [interp1d(np.arange(self.nfits), target, axis=-1)(
-                np.linspace(0, self.nfits - 1, len(roi[:, 0]))) for roi, target in zip(self.roi, self.target)]
+            self.sim_full = [
+                interp1d(np.arange(self.nfits), sim_both, axis=-1)(
+                    np.linspace(0, self.nfits - 1, len(roi[:, 0]))
+                )
+                for roi, sim_both in zip(self.roi, self.sim_both)
+            ]
+            self.target_full = [
+                interp1d(np.arange(self.nfits), target, axis=-1)(
+                    np.linspace(0, self.nfits - 1, len(roi[:, 0]))
+                )
+                for roi, target in zip(self.roi, self.target)
+            ]
             self.resids_full = [i - j for i, j in zip(self.target_full, self.sim_full)]
         else:
-            self.sim_full = [sim_both.T[mask == 1].T for sim_both, mask in zip(self.sim_both, self.masks)]
-            self.target_full = [target.T[mask == 1].T for target, mask in zip(self.target, self.masks)]
+            self.sim_full = [
+                sim_both.T[mask == 1].T
+                for sim_both, mask in zip(self.sim_both, self.masks)
+            ]
+            self.target_full = [
+                target.T[mask == 1].T for target, mask in zip(self.target, self.masks)
+            ]
             self.resids_full = [i - j for i, j in zip(self.target_full, self.sim_full)]
 
         # Save adaptable params
         if self.sigma is not None:
             self.sigma = self.sigma_t.numpy()
 
     """
@@ -383,16 +445,18 @@
         """
         Can do after a preliminary fit to refine coordinates
         Must refit after doing this
 
         """
 
         # Offset coordinates
-        self.roi = [interp_roi(offset_coordinates(roi, offsets_full), periodic=self.periodic) for roi, offsets_full in
-                    zip(self.roi, self.offsets_full)]
+        self.roi = [
+            interp_roi(offset_coordinates(roi, offsets_full), periodic=self.periodic)
+            for roi, offsets_full in zip(self.roi, self.offsets_full)
+        ]
 
         # Rotate
         if self.periodic:
             if self.rotate:
                 self.roi = [rotate_roi(roi) for roi in self.roi]
 
     """
@@ -400,61 +464,87 @@
     
     """
 
     def plot_losses(self, log: bool = False):
         fig, ax = plt.subplots()
         if not log:
             ax.plot(self.losses.T)
-            ax.set_xlabel('Descent step')
-            ax.set_ylabel('Mean square error')
+            ax.set_xlabel("Descent step")
+            ax.set_ylabel("Mean square error")
         else:
             ax.plot(np.log10(self.losses.T))
-            ax.set_xlabel('Descent step')
-            ax.set_ylabel('log10(Mean square error)')
+            ax.set_xlabel("Descent step")
+            ax.set_ylabel("log10(Mean square error)")
         return fig, ax
 
 
-def create_offsets_spline(offsets_t, roi_knots, periodic, nimages, nfits, roi) -> tf.Tensor:
+def create_offsets_spline(
+    offsets_t, roi_knots, periodic, nimages, nfits, roi
+) -> tf.Tensor:
     if nfits is None:
         nfits = max([len(r[:, 0]) for r in roi])
 
     # Create offsets spline
     if periodic:
-        x = np.tile(np.expand_dims(np.arange(-1., roi_knots + 2), 0), (nimages, 1))
+        x = np.tile(np.expand_dims(np.arange(-1.0, roi_knots + 2), 0), (nimages, 1))
         y = tf.concat((offsets_t[:, -1:], offsets_t, offsets_t[:, :2]), axis=1)
         knots = tf.stack((x, y))
     else:
-        x = np.tile(np.expand_dims(np.arange(-1., roi_knots + 1), 0), (nimages, 1))
+        x = np.tile(np.expand_dims(np.arange(-1.0, roi_knots + 1), 0), (nimages, 1))
         y = tf.concat((offsets_t[:, :1], offsets_t, offsets_t[:, -1:]), axis=1)
         knots = tf.stack((x, y))
 
     # Evaluate offset spline
     if nfits is not None:
         if periodic:
-            positions = tf.expand_dims(tf.cast(tf.linspace(start=0.0, stop=roi_knots,
-                                                           num=nfits + 1)[:-1], dtype=tf.float64), axis=-1)
-        else:
-            positions = tf.expand_dims(tf.cast(tf.linspace(start=0.0, stop=roi_knots - 1.000001,
-                                                           num=nfits), dtype=tf.float64), axis=-1)
+            positions = tf.expand_dims(
+                tf.cast(
+                    tf.linspace(start=0.0, stop=roi_knots, num=nfits + 1)[:-1],
+                    dtype=tf.float64,
+                ),
+                axis=-1,
+            )
+        else:
+            positions = tf.expand_dims(
+                tf.cast(
+                    tf.linspace(start=0.0, stop=roi_knots - 1.000001, num=nfits),
+                    dtype=tf.float64,
+                ),
+                axis=-1,
+            )
         spline = interpolate(knots, positions, degree=3, cyclical=False)
         spline = tf.squeeze(spline, axis=1)
         offsets_spline = tf.transpose(spline[:, 1, :])
 
     else:
         offsets_spline = []
         for i in tf.range(nimages):
             if periodic:
                 positions = tf.expand_dims(
-                    tf.cast(tf.linspace(start=0.0, stop=roi_knots, num=roi[i].shape[0] + 1)[:-1],
-                            dtype=tf.float64), axis=-1)
+                    tf.cast(
+                        tf.linspace(start=0.0, stop=roi_knots, num=roi[i].shape[0] + 1)[
+                            :-1
+                        ],
+                        dtype=tf.float64,
+                    ),
+                    axis=-1,
+                )
             else:
-                positions = tf.expand_dims(tf.cast(
-                    tf.linspace(start=0.0, stop=roi_knots - 1.000001, num=roi[i].shape[0]),
-                    dtype=tf.float64), axis=-1)
-            spline = interpolate(knots[:, i:i + 1, :], positions, degree=3, cyclical=False)
+                positions = tf.expand_dims(
+                    tf.cast(
+                        tf.linspace(
+                            start=0.0, stop=roi_knots - 1.000001, num=roi[i].shape[0]
+                        ),
+                        dtype=tf.float64,
+                    ),
+                    axis=-1,
+                )
+            spline = interpolate(
+                knots[:, i : i + 1, :], positions, degree=3, cyclical=False
+            )
             spline = tf.squeeze(spline, axis=1)
             spline = tf.transpose(spline[:, 1, :])[0]
             pad = tf.zeros([nfits - roi[i].shape[0]], dtype=tf.float64)
             offsets_spline.append(tf.concat([spline, pad], axis=0))
         offsets_spline = tf.stack(offsets_spline, axis=0)
 
     return offsets_spline
```

### Comparing `par_segmentation-0.1.8/par_segmentation/quantifier.py` & `par_segmentation-0.1.9/par_segmentation/quantifier.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,121 +1,147 @@
 import numpy as np
 import os
 import pandas as pd
 from .funcs import save_img, in_notebook
-from .interactive import view_stack, view_stack_jupyter, plot_fits, plot_fits_jupyter, plot_segmentation, \
-    plot_segmentation_jupyter, plot_quantification, plot_quantification_jupyter
+from .interactive import (
+    view_stack,
+    view_stack_jupyter,
+    plot_fits,
+    plot_fits_jupyter,
+    plot_segmentation,
+    plot_segmentation_jupyter,
+    plot_quantification,
+    plot_quantification_jupyter,
+)
 from .model import ImageQuantGradientDescent
 from .legacy import ImageQuantDifferentialEvolutionMulti
 from typing import Union, Optional
 
+__all__ = ['ImageQuant']
+
 
 class ImageQuant:
     """
 
     Main class to perform image segmentation
 
-    Instructions:
-    1. (Optional) Perform SAIBR on image
-    2. Specify rough manual ROI
-    3. Initialise class
-    4. run()
-    5. New ROI coordinates will be found at self.roi
-
-    Input data:
-    img                numpy array of image or list of numpy arrays
-    roi                coordinates defining the cortex (two column numpy array of x and y coordinates at 1-pixel width
-                       intervals), or a list of arrays
-
-    ROI:
-    roi_knots          number of knots in cubic-spline fit ROI
-    freedom            amount by which the roi can move (pixel units)
-
-    Fitting parameters:
-    sigma              gaussian/error function width (pixels units)
-    periodic           True if coordinates form a closed loop
-    thickness          thickness of cross section over which to perform quantification (pixel units)
-    rol_ave            width of rolling average to apply to images prior to fitting (pixel units)
-    rotate             if True, will automatically rotate ROI so that the first/last points are at the end of the long
-                       axis
-    nfits              performs this many fits at regular intervals around ROI. If none, will fit at pixel-width
-                       intervals
-    iterations         if >1, adjusts ROI and re-fits
-    batch_norm         if True, images will be globally, rather than internally, normalised. Shouldn't affect
-                       quantification but is recommended during model optimisation
-    fit_outer          if True, will fit the outer portion of each profile to a nonzero value
-    method             'GD' for gradient descent or 'DE' for differential evolution. The former is highly recommended,
-                       the latter works but is much slower and no longer maintained
-    zerocap            if True, limits output concentrations to positive (or very weakly negative) values
-    interp             interpolation type, 'cubic' or 'linear'
-
-    Gradient descent:
-    lr                 learning rate
-    descent_steps      number of gradient descent steps
-
-    Model optimisation:
-    adaptive_sigma     if True, sigma will be trained by gradient descent
-
-    Miscellaneous:
-    verbose            False suppresses onscreen output while model is running (e.g. progress bar)
-
-    Legacy parameters (for 'DE' method):
-    parallel           if True will run in parallel on number of cores specified. NB Very buggy
-    cores              number of cores to use if parallel is True
-    itp                amount of interpolation - allows for subpixel alignment
+    Instructions:\n
+    1. (Optional) Perform SAIBR on image\n
+    2. Specify rough manual ROI\n
+    3. Initialise class\n
+    4. run()\n
+    5. New ROI coordinates will be found at self.roi\n
+    6. Save quantification results using compile_res() - returns a pandas dataframe
+
+    Args:
+        img: numpy array of image or list of numpy arrays
+        roi: coordinates defining the cortex (two column numpy array of x and y coordinates at 1-pixel width intervals), or a list of arrays
+        roi_knots: number of knots in cubic-spline fit ROI
+        freedom: amount by which the roi can move (pixel units)
+        sigma: gaussian/error function width (pixels units)
+        periodic: True if coordinates form a closed loop
+        thickness: thickness of cross section over which to perform quantification (pixel units)
+        rol_ave: width of rolling average to apply to images prior to fitting (pixel units)
+        rotate: if True, will automatically rotate ROI so that the first/last points are at the end of the long axis
+        nfits: performs this many fits at regular intervals around ROI. If none, will fit at pixel-width intervals
+        iterations: if >1, adjusts ROI and re-fits
+        batch_norm: if True, images will be globally, rather than internally, normalised. Shouldn't affect quantification but is recommended during model optimisation
+        fit_outer: if True, will fit the outer portion of each profile to a nonzero value
+        method: 'GD' for gradient descent or 'DE' for differential evolution. The former is highly recommended, the latter works but is much slower and no longer maintained
+        zerocap: if True, limits output concentrations to positive (or very weakly negative) values
+        interp: interpolation type, 'cubic' or 'linear'
+        lr: learning rate
+        descent_steps: number of gradient descent steps
+        adaptive_sigma: if True, sigma will be trained by gradient descent
+        verbose: False suppresses onscreen output while model is running (e.g. progress bar)
+        parallel: LEGACY (for DE method). If True will run in parallel on number of cores specified. NB Very buggy
+        cores:  LEGACY (for DE method). Number of cores to use if parallel is True
+        itp: LEGACY (for DE method). Amount of interpolation - allows for subpixel alignment
 
     """
 
-    def __init__(self,
-                 img: Union[np.ndarray, list],
-                 roi: Union[np.ndarray, list],
-                 sigma: float = 3.5,
-                 periodic: bool = True,
-                 thickness: int = 50,
-                 rol_ave: int = 5,
-                 rotate: bool = False,
-                 nfits: Union[int, None] = 100,
-                 iterations: int = 2,
-                 lr: float = 0.01,
-                 descent_steps: int = 400,
-                 adaptive_sigma: bool = False,
-                 batch_norm: bool = False,
-                 freedom: float = 25,
-                 roi_knots: int = 20,
-                 fit_outer: bool = True,
-                 save_training: bool = False,
-                 save_sims: bool = False,
-                 method: str = 'GD',
-                 itp: int = 10,
-                 parallel: bool = False,
-                 zerocap: bool = False,
-                 cores: Optional[float] = None,
-                 bg_subtract: bool = False,
-                 interp: str = 'cubic',
-                 verbose: bool = True):
-
+    def __init__(
+        self,
+        img: Union[np.ndarray, list],
+        roi: Union[np.ndarray, list],
+        sigma: float = 3.5,
+        periodic: bool = True,
+        thickness: int = 50,
+        rol_ave: int = 5,
+        rotate: bool = False,
+        nfits: Union[int, None] = 100,
+        iterations: int = 2,
+        lr: float = 0.01,
+        descent_steps: int = 400,
+        adaptive_sigma: bool = False,
+        batch_norm: bool = False,
+        freedom: float = 25,
+        roi_knots: int = 20,
+        fit_outer: bool = True,
+        save_training: bool = False,
+        save_sims: bool = False,
+        method: str = "GD",
+        itp: int = 10,
+        parallel: bool = False,
+        zerocap: bool = False,
+        cores: Optional[float] = None,
+        bg_subtract: bool = False,
+        interp: str = "cubic",
+        verbose: bool = True,
+    ):
         # Set up quantifier
         self.method = method
-        if self.method == 'GD':
-            self.iq = ImageQuantGradientDescent(img=img, roi=roi, sigma=sigma, periodic=periodic, thickness=thickness,
-                                                rol_ave=rol_ave, rotate=rotate, nfits=nfits, iterations=iterations,
-                                                lr=lr, descent_steps=descent_steps, adaptive_sigma=adaptive_sigma,
-                                                batch_norm=batch_norm, freedom=freedom, roi_knots=roi_knots,
-                                                fit_outer=fit_outer, zerocap=zerocap, save_training=save_training,
-                                                save_sims=save_sims, verbose=verbose)
-
-        elif self.method == 'DE':
-            self.iq = ImageQuantDifferentialEvolutionMulti(img=img, roi=roi, sigma=sigma, periodic=periodic,
-                                                           thickness=thickness, freedom=freedom, itp=itp,
-                                                           rol_ave=rol_ave, parallel=parallel, cores=cores,
-                                                           rotate=rotate, zerocap=zerocap, nfits=nfits,
-                                                           iterations=iterations, interp=interp,
-                                                           bg_subtract=bg_subtract, verbose=verbose)
+        if self.method == "GD":
+            self.iq = ImageQuantGradientDescent(
+                img=img,
+                roi=roi,
+                sigma=sigma,
+                periodic=periodic,
+                thickness=thickness,
+                rol_ave=rol_ave,
+                rotate=rotate,
+                nfits=nfits,
+                iterations=iterations,
+                lr=lr,
+                descent_steps=descent_steps,
+                adaptive_sigma=adaptive_sigma,
+                batch_norm=batch_norm,
+                freedom=freedom,
+                roi_knots=roi_knots,
+                fit_outer=fit_outer,
+                zerocap=zerocap,
+                save_training=save_training,
+                save_sims=save_sims,
+                verbose=verbose,
+            )
+
+        elif self.method == "DE":
+            self.iq = ImageQuantDifferentialEvolutionMulti(
+                img=img,
+                roi=roi,
+                sigma=sigma,
+                periodic=periodic,
+                thickness=thickness,
+                freedom=freedom,
+                itp=itp,
+                rol_ave=rol_ave,
+                parallel=parallel,
+                cores=cores,
+                rotate=rotate,
+                zerocap=zerocap,
+                nfits=nfits,
+                iterations=iterations,
+                interp=interp,
+                bg_subtract=bg_subtract,
+                verbose=verbose,
+            )
         else:
-            raise Exception('Method must be "GD" (gradient descent) or "DE" (differential evolution)')
+            raise Exception(
+                'Method must be "GD" (gradient descent) or "DE" (differential evolution)'
+            )
 
         # Input data
         self.img = self.iq.img
         self.roi = self.iq.roi
 
         # Empty results containers
         self.mems = None
@@ -131,14 +157,18 @@
 
     """
     Run
     
     """
 
     def run(self):
+        """
+        Performs segmentation/quantification and saves results
+
+        """
         self.iq.run()
 
         # Save new ROI
         self.roi = self.iq.roi
 
         # Save results
         self.mems = self.iq.mems
@@ -146,124 +176,183 @@
         self.offsets = self.iq.offsets
         self.mems_full = self.iq.mems_full
         self.cyts_full = self.iq.cyts_full
         self.offsets_full = self.iq.offsets_full
         self.target_full = self.iq.target_full
         self.sim_full = self.iq.sim_full
         self.resids_full = self.iq.resids_full
-        if self.method == 'GD':
+        if self.method == "GD":
             self.sigma = self.iq.sigma
 
     """
     Saving
     
     """
 
     def save(self, save_path: str, i: Optional[int] = None):
         """
-        Save all results to save_path
+        Save results for a single image to save_path as a series of txt files and tifs
+        I'd recommend using compile_res() instead as this will create a single pandas dataframe with all the results
 
         Args:
-            save_path:
-            i:
-
-        Returns:
+            save_path: path to save full results
+            i: index of the image to save (if quantifying multiple images in batch)
 
         """
 
         if not self.iq.stack:
             i = 0
 
         if not os.path.isdir(save_path):
             os.mkdir(save_path)
-        np.savetxt(save_path + '/offsets.txt', self.offsets[i], fmt='%.4f', delimiter='\t')
-        np.savetxt(save_path + '/cytoplasmic_concentrations.txt', self.cyts[i], fmt='%.4f', delimiter='\t')
-        np.savetxt(save_path + '/membrane_concentrations.txt', self.mems[i], fmt='%.4f', delimiter='\t')
-        np.savetxt(save_path + '/roi.txt', self.roi[i], fmt='%.4f', delimiter='\t')
-        save_img(self.target_full[i], save_path + '/target.tif')
-        save_img(self.sim_full[i], save_path + '/fit.tif')
-        save_img(self.resids_full[i], save_path + '/residuals.tif')
+        np.savetxt(
+            save_path + "/offsets.txt", self.offsets[i], fmt="%.4f", delimiter="\t"
+        )
+        np.savetxt(
+            save_path + "/cytoplasmic_concentrations.txt",
+            self.cyts[i],
+            fmt="%.4f",
+            delimiter="\t",
+        )
+        np.savetxt(
+            save_path + "/membrane_concentrations.txt",
+            self.mems[i],
+            fmt="%.4f",
+            delimiter="\t",
+        )
+        np.savetxt(save_path + "/roi.txt", self.roi[i], fmt="%.4f", delimiter="\t")
+        save_img(self.target_full[i], save_path + "/target.tif")
+        save_img(self.sim_full[i], save_path + "/fit.tif")
+        save_img(self.resids_full[i], save_path + "/residuals.tif")
 
     def compile_res(self):
+        """
+        Compile results to a pandas dataframe
+
+        Returns:
+            A pandas dataframe containing quantification results
+
+        """
+
         # Create empty dataframe
-        df = pd.DataFrame({'Frame': [],
-                           'Position': [],
-                           'Membrane signal': [],
-                           'Cytoplasmic signal': []})
+        df = pd.DataFrame(
+            {
+                "Frame": [],
+                "Position": [],
+                "Membrane signal": [],
+                "Cytoplasmic signal": [],
+            }
+        )
 
         # Fill with data
         for i, (m, c) in enumerate(zip(self.mems, self.cyts)):
-            df = df.append(pd.DataFrame({'Frame': i,
-                                         'Position': range(len(m)),
-                                         'Membrane signal': m,
-                                         'Cytoplasmic signal': c}))
-
-        df = df.reindex(columns=['Frame', 'Position', 'Membrane signal', 'Cytoplasmic signal'])
-        df = df.astype({'Frame': int, 'Position': int})
+            df = df.append(
+                pd.DataFrame(
+                    {
+                        "Frame": i,
+                        "Position": range(len(m)),
+                        "Membrane signal": m,
+                        "Cytoplasmic signal": c,
+                    }
+                )
+            )
+
+        df = df.reindex(
+            columns=["Frame", "Position", "Membrane signal", "Cytoplasmic signal"]
+        )
+        df = df.astype({"Frame": int, "Position": int})
         return df
 
     """
     Interactive
     
     """
 
     def view_frames(self):
+        """
+        Opens an interactive widget to view image(s)
+
+        """
+
         jupyter = in_notebook()
         if not jupyter:
             if self.iq.stack:
                 fig, ax = view_stack(self.img)
             else:
                 fig, ax = view_stack(self.img[0])
         else:
             if self.iq.stack:
                 fig, ax = view_stack_jupyter(self.img)
             else:
                 fig, ax = view_stack_jupyter(self.img[0])
         return fig, ax
 
     def plot_quantification(self):
+        """
+        Opens an interactive widget to plot membrane quantification results
+
+        """
+
         jupyter = in_notebook()
         if not jupyter:
             if self.iq.stack:
                 fig, ax = plot_quantification(self.mems_full)
             else:
                 fig, ax = plot_quantification(self.mems_full[0])
         else:
             if self.iq.stack:
                 fig, ax = plot_quantification_jupyter(self.mems_full)
             else:
                 fig, ax = plot_quantification_jupyter(self.mems_full[0])
         return fig, ax
 
     def plot_fits(self):
+        """
+        Opens an interactive widget to plot actual vs fit profiles
+
+        """
+
         jupyter = in_notebook()
         if not jupyter:
             if self.iq.stack:
                 fig, ax = plot_fits(self.target_full, self.sim_full)
             else:
                 fig, ax = plot_fits(self.target_full[0], self.sim_full[0])
         else:
             if self.iq.stack:
                 fig, ax = plot_fits_jupyter(self.target_full, self.sim_full)
             else:
                 fig, ax = plot_fits_jupyter(self.target_full[0], self.sim_full[0])
         return fig, ax
 
     def plot_segmentation(self):
+        """
+        Opens an interactive widget to plot segmentation results
+
+        """
+
         jupyter = in_notebook()
         if not jupyter:
             if self.iq.stack:
                 fig, ax = plot_segmentation(self.img, self.roi)
             else:
                 fig, ax = plot_segmentation(self.img[0], self.roi[0])
         else:
             if self.iq.stack:
                 fig, ax = plot_segmentation_jupyter(self.img, self.roi)
             else:
                 fig, ax = plot_segmentation_jupyter(self.img[0], self.roi[0])
         return fig, ax
 
     def plot_losses(self, log: bool = False):
-        if self.method == 'GD':
+        """
+        Plot loss curves (one line for each image)
+
+        Args:
+            log: if True, plot the logarithm of losses
+
+        """
+
+        if self.method == "GD":
             self.iq.plot_losses(log=log)
         else:
             pass
```

### Comparing `par_segmentation-0.1.8/par_segmentation/roi.py` & `par_segmentation-0.1.9/par_segmentation/roi.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,57 +9,103 @@
 
 """
 Todo: This no longer works with multiple channels - intensity ranges
 Todo: Ability to specify a directory and open all channels. Or an nd file
 
 """
 
+__all__ = ['def_roi', 'ROI_jupyter', 'spline_roi', 'interp_roi', 'offset_coordinates']
 
-def def_roi(stack: Union[np.ndarray, list], spline: bool = True, start_frame: int = 0, end_frame: Optional[int] = None,
-            periodic: bool = True, show_fit: bool = True, k: int = 3):
-    r = ROI(stack, spline=spline, start_frame=start_frame, end_frame=end_frame, periodic=periodic, show_fit=show_fit,
-            k=k)
+
+def def_roi(
+    stack: Union[np.ndarray, list],
+    spline: bool = True,
+    start_frame: int = 0,
+    end_frame: Optional[int] = None,
+    periodic: bool = True,
+    show_fit: bool = True,
+    k: int = 3,
+):
+    """
+    There are two different methods for drawing ROIs depending on if you're using normal python scripts or Jupyter notebooks.
+    This is the one to use if you're using python scripts.
+
+    Instructions:\n
+    - click to lay down points\n
+    - backspace at any time to remove last point\n
+    - press enter to select area (if spline=True will fit spline to points, otherwise will fit straight lines)\n
+    - at this point can press backspace to go back to laying points\n
+    - press enter again to close and return ROI\n
+
+    Args:
+        stack: image (2D or 3D numpy array)
+        spline: if True, will fit a spline to the user-defined points
+        start_frame: if img is a time series, this is the index of the first frame to show
+        end_frame: if img is a time series, this is the index of the last frame to show
+        periodic: set to True if drawing a periodic ROI
+        show_fit: if True, will show the spline fit (if spline=True)
+        k: degree of the spline (e.g. 3 = cubic)
+
+    Returns:
+        ROI as a numpy array\n
+        To save this in a fiji readable format:
+        np.savetxt(filename, roi, fmt='%.4f', delimiter='\t')
+
+    """
+
+    r = _ROI(
+        stack,
+        spline=spline,
+        start_frame=start_frame,
+        end_frame=end_frame,
+        periodic=periodic,
+        show_fit=show_fit,
+        k=k,
+    )
     r.run()
     return r.roi
 
 
-class ROI:
+class _ROI:
     """
-    Instructions:
-    - click to lay down points
-    - backspace at any time to remove last point
-    - press enter to select area (if spline=True will fit spline to points, otherwise will fit straight lines)
-    - at this point can press backspace to go back to laying points
-    - press enter again to close and return ROI
+    Instructions:\n
+    - click to lay down points\n
+    - backspace at any time to remove last point\n
+    - press enter to select area (if spline=True will fit spline to points, otherwise will fit straight lines)\n
+    - at this point can press backspace to go back to laying points\n
+    - press enter again to close and return ROI\n
 
     :param img: input image
     :param spline: if true, fits spline to inputted coordinates
     :return: cell boundary coordinates
     """
 
-    def __init__(self,
-                 img: Union[np.ndarray, list],
-                 spline: bool = True,
-                 start_frame: int = 0,
-                 end_frame: Optional[int] = None,
-                 periodic: bool = True,
-                 show_fit: bool = True,
-                 k: int = 3):
-
+    def __init__(
+        self,
+        img: Union[np.ndarray, list],
+        spline: bool = True,
+        start_frame: int = 0,
+        end_frame: Optional[int] = None,
+        periodic: bool = True,
+        show_fit: bool = True,
+        k: int = 3,
+    ):
         # Detect if single frame or stack
         if type(img) is list:
-            self.img_type = 'list'
+            self.img_type = "list"
             self.images = img
 
         elif len(img.shape) == 3:
-            self.img_type = 'stack'
+            self.img_type = "stack"
             self.images = list(img)
         else:
-            self.img_type = 'single'
-            self.images = [img, ]
+            self.img_type = "single"
+            self.images = [
+                img,
+            ]
 
         # Params
         self.spline = spline
         self.start_frame = start_frame
         self.end_frame = end_frame
         self.periodic = periodic
         self.show_fit = show_fit
@@ -70,166 +116,224 @@
         self._current_image = 0
         self._point0 = None
         self._points = None
         self._line = None
         self._fitted = False
 
         # Specify vlim
-        if self.img_type == 'stack' or self.img_type == 'single':
+        if self.img_type == "stack" or self.img_type == "single":
             self.vmax = max([np.percentile(i, 99.9) for i in self.images])
             self.vmin = min([np.percentile(i, 0.1) for i in self.images])
-        elif self.img_type == 'list':
+        elif self.img_type == "list":
             self.vmax = [np.percentile(i, 99.9) for i in self.images]
             self.vmin = [np.percentile(i, 0.1) for i in self.images]
 
         # Outputs
         self.xpoints = []
         self.ypoints = []
         self.roi = None
 
     def run(self):
         # Set up figure
         plt.ion()
         self.fig = plt.figure()
         self.ax = self.fig.add_subplot(111)
 
-        self.fig.canvas.mpl_connect('button_press_event', self.button_press_callback)
-        self.fig.canvas.mpl_connect('key_press_event', self.key_press_callback)
+        self.fig.canvas.mpl_connect("button_press_event", self._button_press_callback)
+        self.fig.canvas.mpl_connect("key_press_event", self._key_press_callback)
 
         # Stack
-        if self.img_type == 'stack' or self.img_type == 'list':
+        if self.img_type == "stack" or self.img_type == "list":
             plt.subplots_adjust(left=0.25, bottom=0.25)
             self.axframe = plt.axes([0.25, 0.1, 0.65, 0.03])
             if self.end_frame is None:
                 self.end_frame = len(self.images)
-            self.sframe = Slider(self.axframe, 'Frame', self.start_frame, self.end_frame, valinit=self.start_frame,
-                                 valfmt='%d')
-            self.sframe.on_changed(self.draw_frame)
+            self.sframe = Slider(
+                self.axframe,
+                "Frame",
+                self.start_frame,
+                self.end_frame,
+                valinit=self.start_frame,
+                valfmt="%d",
+            )
+            self.sframe.on_changed(self._draw_frame)
 
-        self.draw_frame(self.start_frame)
+        self._draw_frame(self.start_frame)
 
         # Show figure
-        self.fig.canvas.set_window_title('Specify ROI')
-        self.fig.canvas.mpl_connect('close_event', lambda event: self.fig.canvas.stop_event_loop())
+        self.fig.canvas.set_window_title("Specify ROI")
+        self.fig.canvas.mpl_connect(
+            "close_event", lambda event: self.fig.canvas.stop_event_loop()
+        )
         self.fig.canvas.start_event_loop(timeout=-1)
 
-    def draw_frame(self, i: int):
+    def _draw_frame(self, i: int):
         self._current_frame = i
         self.ax.clear()
 
         # Plot image
-        if self.img_type == 'stack' or self.img_type == 'single':
-            self.ax.imshow(self.images[int(i)], cmap='gray', vmin=self.vmin, vmax=self.vmax)
+        if self.img_type == "stack" or self.img_type == "single":
+            self.ax.imshow(
+                self.images[int(i)], cmap="gray", vmin=self.vmin, vmax=self.vmax
+            )
         else:
-            self.ax.imshow(self.images[int(i)], cmap='gray', vmin=self.vmin[int(i)], vmax=self.vmax[int(i)])
+            self.ax.imshow(
+                self.images[int(i)],
+                cmap="gray",
+                vmin=self.vmin[int(i)],
+                vmax=self.vmax[int(i)],
+            )
 
         # Finalise figure
         self.ax.set_xticks([])
         self.ax.set_yticks([])
-        self.ax.text(0.03, 0.97,
-                     'Specify ROI clockwise (4 points minimum)'
-                     '\nClick to lay points'
-                     '\nBACKSPACE: undo'
-                     '\nENTER: Save and continue',
-                     color='white',
-                     transform=self.ax.transAxes, fontsize=8, va='top', ha='left')
-        self.display_points()
+        self.ax.text(
+            0.03,
+            0.97,
+            "Specify ROI clockwise (4 points minimum)"
+            "\nClick to lay points"
+            "\nBACKSPACE: undo"
+            "\nENTER: Save and continue",
+            color="white",
+            transform=self.ax.transAxes,
+            fontsize=8,
+            va="top",
+            ha="left",
+        )
+        self._display_points()
         self.fig.canvas.draw()
 
-    def button_press_callback(self, event: MouseEvent):
+    def _button_press_callback(self, event: MouseEvent):
         if not self._fitted:
             if isinstance(event.inaxes, type(self.ax)):
                 # Add points to list
                 self.xpoints.extend([event.xdata])
                 self.ypoints.extend([event.ydata])
 
                 # Display points
-                self.display_points()
+                self._display_points()
                 self.fig.canvas.draw()
 
-    def key_press_callback(self, event: KeyEvent):
-        if event.key == 'backspace':
+    def _key_press_callback(self, event: KeyEvent):
+        if event.key == "backspace":
             if not self._fitted:
                 # Remove last drawn point
                 if len(self.xpoints) != 0:
                     self.xpoints = self.xpoints[:-1]
                     self.ypoints = self.ypoints[:-1]
-                self.display_points()
+                self._display_points()
                 self.fig.canvas.draw()
             else:
                 # Remove line
                 self._fitted = False
                 self._line.pop(0).remove()
                 self.roi = None
                 self.fig.canvas.draw()
 
-        if event.key == 'enter':
+        if event.key == "enter":
             if len(self.xpoints) != 0:
                 roi = np.vstack((self.xpoints, self.ypoints)).T
 
                 # Spline
                 if self.spline:
                     if not self._fitted:
                         self.roi = spline_roi(roi, periodic=self.periodic, k=self.k)
                         self._fitted = True
 
                         # Display line
                         if self.show_fit:
-                            self._line = self.ax.plot(self.roi[:, 0], self.roi[:, 1], c='b')
+                            self._line = self.ax.plot(
+                                self.roi[:, 0], self.roi[:, 1], c="b"
+                            )
                             self.fig.canvas.draw()
                         else:
                             plt.close(self.fig)
                     else:
                         plt.close(self.fig)
                 else:
                     self.roi = roi
                     plt.close(self.fig)
             else:
                 self.roi = []
                 plt.close(self.fig)
 
-    def display_points(self):
+    def _display_points(self):
         # Remove existing points
         try:
             self._point0.remove()
             self._points.remove()
         except (ValueError, AttributeError) as error:
             pass
 
         # Plot all points
         if len(self.xpoints) != 0:
-            self._points = self.ax.scatter(self.xpoints, self.ypoints, c='lime', s=10)
-            self._point0 = self.ax.scatter(self.xpoints[0], self.ypoints[0], c='r', s=10)
+            self._points = self.ax.scatter(self.xpoints, self.ypoints, c="lime", s=10)
+            self._point0 = self.ax.scatter(
+                self.xpoints[0], self.ypoints[0], c="r", s=10
+            )
 
 
 class ROI_jupyter:
+    """
+    There are two different methods for drawing ROIs depending on if you're using normal python scripts or Jupyter notebooks.
+    This is the one to use if you're using Jupyter notebooks.
+
+    Example workflow:
+
+    ### Cell 1:\n
+    r = RoiJupyter(img, periodic=True, spline=True)\n
+    r.run()\n
+    # A window will appear - draw the ROI and click save\n
+
+    ### Cell 2:\n
+    roi = r.roi\n
+    print(roi.shape)\n
+    # Confirm that the shape is not (0, 0)\n
+
+    To save this in a fiji readable format:
+    np.savetxt(filename, roi, fmt='%.4f', delimiter='\t')
+
+    Args:
+        img: image (2D or 3D numpy array)
+        spline: if True, will fit a spline to the user-defined points
+        start_frame: if img is a time series, this is the index of the first frame to show
+        end_frame: if img is a time series, this is the index of the last frame to show
+        periodic: set to True if drawing a periodic ROI
+        show_fit: if True, will show the spline fit (if spline=True)
+        k: degree of the spline (e.g. 3 = cubic)
+
 
-    def __init__(self,
-                 img: Union[np.ndarray, list],
-                 spline: bool = True,
-                 start_frame: int = 0,
-                 end_frame: Optional[int] = None,
-                 periodic: bool = True,
-                 show_fit: bool = True,
-                 k: int = 3):
+    """
 
+    def __init__(
+        self,
+        img: Union[np.ndarray, list],
+        spline: bool = True,
+        start_frame: int = 0,
+        end_frame: Optional[int] = None,
+        periodic: bool = True,
+        show_fit: bool = True,
+        k: int = 3,
+    ):
         self.fig = None
         self.ax = None
 
         # Detect if single frame or stack
         if type(img) is list:
-            self.img_type = 'list'
+            self.img_type = "list"
             self.images = img
 
         elif len(img.shape) == 3:
-            self.img_type = 'stack'
+            self.img_type = "stack"
             self.images = list(img)
         else:
-            self.img_type = 'single'
-            self.images = [img, ]
+            self.img_type = "single"
+            self.images = [
+                img,
+            ]
 
         # Params
         self.spline = spline
         self.start_frame = start_frame
         self.end_frame = end_frame
         self.periodic = periodic
         self.show_fit = show_fit
@@ -242,110 +346,123 @@
         # Outputs
         self.xpoints = []
         self.ypoints = []
         self.roi = None
 
     def run(self):
         self.fig, self.ax = plt.subplots()
-        self.fig.canvas.mpl_connect('button_press_event', self.button_press_callback)
+        self.fig.canvas.mpl_connect("button_press_event", self._button_press_callback)
 
         # Buttons
         self.ax_undo = plt.axes([0.7, 0.05, 0.1, 0.075])
-        self.b_undo = Button(self.ax_undo, 'Undo')
+        self.b_undo = Button(self.ax_undo, "Undo")
         self.b_undo.on_clicked(self._undo)
         self.ax_save = plt.axes([0.81, 0.05, 0.1, 0.075])
-        self.b_save = Button(self.ax_save, 'Save')
+        self.b_save = Button(self.ax_save, "Save")
         self.b_save.on_clicked(self._save)
 
         # Stack
-        if self.img_type == 'stack' or self.img_type == 'list':
+        if self.img_type == "stack" or self.img_type == "list":
+
             @widgets.interact(Frame=(0, len(self.images) - 1, 1))
             def update(Frame=0):
-                self.draw_frame(Frame)
+                self._draw_frame(Frame)
+
         else:
-            self.draw_frame(0)
+            self._draw_frame(0)
 
         self.fig.set_size_inches(4, 4)
 
-    def button_press_callback(self, event: MouseEvent):
+    def _button_press_callback(self, event: MouseEvent):
         if isinstance(event.inaxes, type(self.ax)):
             # Add points to list
             self.xpoints.extend([event.xdata])
             self.ypoints.extend([event.ydata])
 
             # Display points
-            self.display_points()
+            self._display_points()
             self.fig.canvas.draw()
 
     def _undo(self, _):
         # Remove last drawn point
         if len(self.xpoints) != 0:
             self.xpoints = self.xpoints[:-1]
             self.ypoints = self.ypoints[:-1]
-        self.display_points()
+        self._display_points()
         self.fig.canvas.draw()
 
     def _save(self, _):
         roi = np.vstack((self.xpoints, self.ypoints)).T
 
         # Spline
         if self.spline:
             self.roi = spline_roi(roi, periodic=self.periodic, k=self.k)
 
             # Display line
             if self.show_fit:
-                self._line = self.ax.plot(self.roi[:, 0], self.roi[:, 1], c='b')
+                self._line = self.ax.plot(self.roi[:, 0], self.roi[:, 1], c="b")
                 self.fig.canvas.draw()
         else:
             self.roi = roi
 
         plt.close()
 
-    def display_points(self):
+    def _display_points(self):
         # Remove existing points
         try:
             self._point0.remove()
             self._points.remove()
         except (ValueError, AttributeError) as error:
             pass
 
         # Plot all points
         if len(self.xpoints) != 0:
-            self._points = self.ax.scatter(self.xpoints, self.ypoints, c='lime', s=10)
-            self._point0 = self.ax.scatter(self.xpoints[0], self.ypoints[0], c='r', s=10)
+            self._points = self.ax.scatter(self.xpoints, self.ypoints, c="lime", s=10)
+            self._point0 = self.ax.scatter(
+                self.xpoints[0], self.ypoints[0], c="r", s=10
+            )
 
-    def draw_frame(self, i: int):
+    def _draw_frame(self, i: int):
         self.ax.clear()
 
         # Plot image
-        self.ax.imshow(self.images[int(i)], cmap='gray', vmin=self.vmin, vmax=self.vmax)
+        self.ax.imshow(self.images[int(i)], cmap="gray", vmin=self.vmin, vmax=self.vmax)
 
         # Finalise figure
         self.ax.set_xticks([])
         self.ax.set_yticks([])
-        self.ax.text(0.03, 0.97,
-                     'Specify ROI clockwise from posterior (4 points minimum)'
-                     '\nClick to lay points',
-                     color='white',
-                     transform=self.ax.transAxes, fontsize=8, va='top', ha='left')
-        self.display_points()
+        self.ax.text(
+            0.03,
+            0.97,
+            "Specify ROI clockwise from posterior (4 points minimum)"
+            "\nClick to lay points",
+            color="white",
+            transform=self.ax.transAxes,
+            fontsize=8,
+            va="top",
+            ha="left",
+        )
+        self._display_points()
         self.fig.canvas.draw()
 
 
-def spline_roi(roi: np.ndarray, periodic: bool = True, s: float = 0.0, k: int = 3) -> np.ndarray:
+def spline_roi(
+    roi: np.ndarray, periodic: bool = True, s: float = 0.0, k: int = 3
+) -> np.ndarray:
     """
     Fits a spline to points specifying the coordinates of the cortex, then interpolates to pixel distances
 
     Args:
-        roi:
-        periodic:
-        s:
-        k:
+        roi: two column array containing x and y coordinates. e.g. roi = np.loadtxt(filename)
+        periodic: set to True if the ROI is periodic
+        s: splprep s parameter
+        k: splprep k parameter (spline order)
 
     Returns:
+        spline ROI (numpy array)
 
     """
 
     # Append the starting x,y coordinates
     if periodic:
         x = np.r_[roi[:, 0], roi[0, 0]]
         y = np.r_[roi[:, 1], roi[0, 1]]
@@ -359,61 +476,67 @@
     # Evaluate spline
     xi, yi = splev(np.linspace(0, 1, 10000), tck)
 
     # Interpolate
     return interp_roi(np.vstack((xi, yi)).T, periodic=periodic)
 
 
-def interp_roi(roi: np.ndarray, periodic: bool = True, npoints: Optional[int] = None, gap: int = 1) -> np.ndarray:
+def interp_roi(
+    roi: np.ndarray, periodic: bool = True, npoints: Optional[int] = None, gap: int = 1
+) -> np.ndarray:
     """
-    Interpolates coordinates to one pixel distances (or as close as possible to one pixel)
-    Linear interpolation
+    Interpolates coordinates to one pixel distances (or as close as possible to one pixel). Linear interpolation
 
     Args:
-        roi:
-        periodic:
-        npoints:
-        gap:
+        roi: two column array containing x and y coordinates. e.g. roi = np.loadtxt(filename)
+        periodic: set to True if the ROI is periodic
+        npoints: number of points to interpolate to
+        gap: alternatively, specify the desired gap between succesive coordinates in pixel units
 
     Returns:
+        interpolated ROI (numpy array)
 
     """
 
     if periodic:
         c = np.append(roi, [roi[0, :]], axis=0)
     else:
         c = roi
 
     # Calculate distance between points in pixel units
     distances = ((np.diff(c[:, 0]) ** 2) + (np.diff(c[:, 1]) ** 2)) ** 0.5
     distances_cumsum = np.r_[0, np.cumsum(distances)]
     total_length = sum(distances)
 
     # Interpolate
-    fx, fy = interp1d(distances_cumsum, c[:, 0], kind='linear'), interp1d(distances_cumsum, c[:, 1], kind='linear')
+    fx, fy = interp1d(distances_cumsum, c[:, 0], kind="linear"), interp1d(
+        distances_cumsum, c[:, 1], kind="linear"
+    )
     if npoints is None:
         positions = np.linspace(0, total_length, int(round(total_length / gap)))
     else:
         positions = np.linspace(0, total_length, npoints + 1)
     xcoors, ycoors = fx(positions), fy(positions)
     newpoints = np.c_[xcoors[:-1], ycoors[:-1]]
     return newpoints
 
 
-def offset_coordinates(roi: np.ndarray, offsets: Union[np.ndarray, float], periodic: bool = True) -> np.ndarray:
+def offset_coordinates(
+    roi: np.ndarray, offsets: Union[np.ndarray, float], periodic: bool = True
+) -> np.ndarray:
     """
     Reads in coordinates, adjusts according to offsets
 
     Args:
-        roi:  two column array containing x and y coordinates. e.g. coors = np.loadtxt(filename)
+        roi:  two column array containing x and y coordinates. e.g. roi = np.loadtxt(filename)
         offsets: array the same length as coors. Direction?
-        periodic:
+        periodic: set to True if the ROI is periodic
 
     Returns:
-         array in same format as coors containing new coordinates.
+         array in same format as coors containing new coordinates.\n
          To save this in a fiji readable format:
          np.savetxt(filename, newcoors, fmt='%.4f', delimiter='\t')
 
     """
 
     # Calculate gradients
     xcoors = roi[:, 0]
@@ -427,13 +550,13 @@
         ydiffs = np.r_[ydiffs[0], ydiffs]
         xdiffs = np.r_[xdiffs[0], xdiffs]
 
     grad = ydiffs / xdiffs
     tangent_grad = -1 / grad
 
     # Offset coordinates
-    xchange = ((offsets ** 2) / (1 + tangent_grad ** 2)) ** 0.5
+    xchange = ((offsets**2) / (1 + tangent_grad**2)) ** 0.5
     ychange = xchange / abs(grad)
     newxs = xcoors + np.sign(ydiffs) * np.sign(offsets) * xchange
     newys = ycoors - np.sign(xdiffs) * np.sign(offsets) * ychange
     newcoors = np.swapaxes(np.vstack([newxs, newys]), 0, 1)
     return newcoors
```

### Comparing `par_segmentation-0.1.8/par_segmentation/tgf_interpolate.py` & `par_segmentation-0.1.9/par_segmentation/_tgf_interpolate.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,25 +7,36 @@
 import numpy as np
 import tensorflow as tf
 from absl import flags
 import enum
 
 FLAGS = flags.FLAGS
 
-Integer = Union[int, np.int8, np.int16, np.int32, np.int64, np.uint8, np.uint16,
-                np.uint32, np.uint64]
+Integer = Union[
+    int,
+    np.int8,
+    np.int16,
+    np.int32,
+    np.int64,
+    np.uint8,
+    np.uint16,
+    np.uint32,
+    np.uint64,
+]
 Float = Union[float, np.float16, np.float32, np.float64]
 TensorLike = Union[Integer, Float, Sequence, np.ndarray, tf.Tensor, tf.Variable]
 
 
-def interpolate(knots: TensorLike,
-                positions: TensorLike,
-                degree: int,
-                cyclical: bool,
-                name: str = "bspline_interpolate") -> tf.Tensor:
+def interpolate(
+    knots: TensorLike,
+    positions: TensorLike,
+    degree: int,
+    cyclical: bool,
+    name: str = "bspline_interpolate",
+) -> tf.Tensor:
     """Applies B-spline interpolation to input control points (knots).
     Note:
       In the following, A1 to An, and B1 to Bk are optional batch dimensions.
     Args:
       knots: A tensor with shape `[B1, ..., Bk, C]` containing knot values, where
         `C` is the number of knots.
       positions: Tensor with shape `[A1, .. An]`. Positions must be between
@@ -45,17 +56,18 @@
 
         num_knots = knots.get_shape().as_list()[-1]
         weights = knot_weights(positions, num_knots, degree, cyclical, False, name)
         return interpolate_with_weights(knots, weights)
 
 
 def interpolate_with_weights(
-        knots: TensorLike,
-        weights: TensorLike,
-        name: str = "bspline_interpolate_with_weights") -> tf.Tensor:
+    knots: TensorLike,
+    weights: TensorLike,
+    name: str = "bspline_interpolate_with_weights",
+) -> tf.Tensor:
     """Interpolates knots using knot weights.
     Note:
       In the following, A1 to An, and B1 to Bk are optional batch dimensions.
     Args:
       knots: A tensor with shape `[B1, ..., Bk, C]` containing knot values, where
         `C` is the number of knots.
       weights: A tensor with shape `[A1, ..., An, C]` containing dense weights for
@@ -68,15 +80,16 @@
       ValueError: If the last dimension of knots and weights is not equal.
     """
     with tf.name_scope(name):
         knots = tf.convert_to_tensor(value=knots)
         weights = tf.convert_to_tensor(value=weights)
 
         compare_dimensions(
-            tensors=(knots, weights), axes=-1, tensor_names=("knots", "weights"))
+            tensors=(knots, weights), axes=-1, tensor_names=("knots", "weights")
+        )
 
     return tf.tensordot(weights, knots, (-1, -1))
 
 
 def compare_dimensions(tensors, axes, tensor_names=None):
     """Compares dimensions of tensors with static or dynamic shapes.
     Args:
@@ -86,26 +99,29 @@
         Each entry should correspond to the axis of the tensor being compared.
       tensor_names: Names of `tensors` to be used in the error message if one is
         thrown. If left as `None`, their `Tensor.name` fields are used instead.
     Raises:
       ValueError: If inputs have unexpected types, or if given axes are out of
         bounds, or if the check fails.
     """
-    _check_tensors(tensors, 'tensors')
+    _check_tensors(tensors, "tensors")
     if isinstance(axes, int):
         axes = [axes] * len(tensors)
-    _check_tensor_axis_lists(tensors, 'tensors', axes, 'axes')
+    _check_tensor_axis_lists(tensors, "tensors", axes, "axes")
     axes = _fix_axes(tensors, axes, allow_negative=False)
     if tensor_names is None:
-        tensor_names = _give_default_names(tensors, 'tensor')
+        tensor_names = _give_default_names(tensors, "tensor")
     dimensions = [_get_dim(tensor, axis) for tensor, axis in zip(tensors, axes)]
     if not _all_are_equal(dimensions):
-        raise ValueError('Tensors {} must have the same number of dimensions in '
-                         'axes {}, but they are {}.'.format(
-            list(tensor_names), list(axes), list(dimensions)))
+        raise ValueError(
+            "Tensors {} must have the same number of dimensions in "
+            "axes {}, but they are {}.".format(
+                list(tensor_names), list(axes), list(dimensions)
+            )
+        )
 
 
 def _all_are_equal(list_of_objects):
     """Helper function to check if all the items in a list are the same."""
     if not list_of_objects:
         return True
     if isinstance(list_of_objects[0], list):
@@ -118,63 +134,72 @@
     return tf.compat.dimension_value(tensor.shape[axis])
 
 
 def _check_tensors(tensors, tensors_name):
     """Helper function to check the type and length of tensors."""
     _check_type(tensors, tensors_name, (list, tuple))
     if len(tensors) < 2:
-        raise ValueError('At least 2 tensors are required.')
+        raise ValueError("At least 2 tensors are required.")
 
 
 def _check_type(variable, variable_name, expected_type):
     """Helper function for checking that inputs are of expected types."""
     if isinstance(expected_type, (list, tuple)):
-        expected_type_name = 'list or tuple'
+        expected_type_name = "list or tuple"
     else:
         expected_type_name = expected_type.__name__
     if not isinstance(variable, expected_type):
-        raise ValueError('{} must be of type {}, but it is {}'.format(
-            variable_name, expected_type_name,
-            type(variable).__name__))
+        raise ValueError(
+            "{} must be of type {}, but it is {}".format(
+                variable_name, expected_type_name, type(variable).__name__
+            )
+        )
 
 
 def _check_tensor_axis_lists(tensors, tensors_name, axes, axes_name):
     """Helper function to check that lengths of `tensors` and `axes` match."""
     _check_type(axes, axes_name, (list, tuple))
     if len(tensors) != len(axes):
         raise ValueError(
-            '{} and {} must have the same length, but are {} and {}.'.format(
-                tensors_name, axes_name, len(tensors), len(axes)))
+            "{} and {} must have the same length, but are {} and {}.".format(
+                tensors_name, axes_name, len(tensors), len(axes)
+            )
+        )
 
 
 def _fix_axes(tensors, axes, allow_negative):
     """Makes all axes positive and checks for out of bound errors."""
     axes = [
         axis + tensor.shape.ndims if axis < 0 else axis
         for tensor, axis in zip(tensors, axes)
     ]
     if not all(
-            ((allow_negative or
-              (not allow_negative and axis >= 0)) and axis < tensor.shape.ndims)
-            for tensor, axis in zip(tensors, axes)):
-        rank_axis_pairs = list(
-            zip([tensor.shape.ndims for tensor in tensors], axes))
+        (
+            (allow_negative or (not allow_negative and axis >= 0))
+            and axis < tensor.shape.ndims
+        )
+        for tensor, axis in zip(tensors, axes)
+    ):
+        rank_axis_pairs = list(zip([tensor.shape.ndims for tensor in tensors], axes))
         raise ValueError(
-            'Some axes are out of bounds. Given rank-axes pairs: {}'.format(
-                [pair for pair in rank_axis_pairs]))
+            "Some axes are out of bounds. Given rank-axes pairs: {}".format(
+                [pair for pair in rank_axis_pairs]
+            )
+        )
     return axes
 
 
 def _give_default_names(list_of_objects, name):
     """Helper function to give default names to objects for error messages."""
-    return [name + '_' + str(index) for index in range(len(list_of_objects))]
+    return [name + "_" + str(index) for index in range(len(list_of_objects))]
 
 
 class Degree(enum.IntEnum):
     """Defines valid degrees for B-spline interpolation."""
+
     CONSTANT = 0
     LINEAR = 1
     QUADRATIC = 2
     CUBIC = 3
     QUARTIC = 4
 
 
@@ -192,60 +217,75 @@
 
 def _quadratic(position: tf.Tensor) -> tf.Tensor:
     """B-Spline basis functions of degree 2 for positions in the range [0, 1]."""
     # We pre-calculate the terms that are used multiple times.
     pos_sq = tf.pow(position, 2.0)
 
     # Piecewise quadratic splines are C1 smooth.
-    return tf.stack((tf.pow(1.0 - position, 2.0) / 2.0, -pos_sq + position + 0.5,
-                     pos_sq / 2.0),
-                    axis=-1)
+    return tf.stack(
+        (tf.pow(1.0 - position, 2.0) / 2.0, -pos_sq + position + 0.5, pos_sq / 2.0),
+        axis=-1,
+    )
 
 
 def _cubic(position: tf.Tensor) -> tf.Tensor:
     """B-Spline basis functions of degree 3 for positions in the range [0, 1]."""
     # We pre-calculate the terms that are used multiple times.
     neg_pos = 1.0 - position
     pos_sq = tf.pow(position, 2.0)
     pos_cb = tf.pow(position, 3.0)
 
     # Piecewise cubic splines are C2 smooth.
     return tf.stack(
-        (tf.pow(neg_pos, 3.0) / 6.0, (3.0 * pos_cb - 6.0 * pos_sq + 4.0) / 6.0,
-         (-3.0 * pos_cb + 3.0 * pos_sq + 3.0 * position + 1.0) / 6.0,
-         pos_cb / 6.0),
-        axis=-1)
+        (
+            tf.pow(neg_pos, 3.0) / 6.0,
+            (3.0 * pos_cb - 6.0 * pos_sq + 4.0) / 6.0,
+            (-3.0 * pos_cb + 3.0 * pos_sq + 3.0 * position + 1.0) / 6.0,
+            pos_cb / 6.0,
+        ),
+        axis=-1,
+    )
 
 
 def _quartic(position: tf.Tensor) -> tf.Tensor:
     """B-Spline basis functions of degree 4 for positions in the range [0, 1]."""
     # We pre-calculate the terms that are used multiple times.
     neg_pos = 1.0 - position
     pos_sq = tf.pow(position, 2.0)
     pos_cb = tf.pow(position, 3.0)
     pos_qt = tf.pow(position, 4.0)
 
     # Piecewise quartic splines are C3 smooth.
     return tf.stack(
-        (tf.pow(neg_pos, 4.0) / 24.0,
-         (-4.0 * tf.pow(neg_pos, 4.0) + 4.0 * tf.pow(neg_pos, 3.0) +
-          6.0 * tf.pow(neg_pos, 2.0) + 4.0 * neg_pos + 1.0) / 24.0,
-         (pos_qt - 2.0 * pos_cb - pos_sq + 2.0 * position) / 4.0 + 11.0 / 24.0,
-         (-4.0 * pos_qt + 4.0 * pos_cb + 6.0 * pos_sq + 4.0 * position + 1.0) /
-         24.0, pos_qt / 24.0),
-        axis=-1)
+        (
+            tf.pow(neg_pos, 4.0) / 24.0,
+            (
+                -4.0 * tf.pow(neg_pos, 4.0)
+                + 4.0 * tf.pow(neg_pos, 3.0)
+                + 6.0 * tf.pow(neg_pos, 2.0)
+                + 4.0 * neg_pos
+                + 1.0
+            )
+            / 24.0,
+            (pos_qt - 2.0 * pos_cb - pos_sq + 2.0 * position) / 4.0 + 11.0 / 24.0,
+            (-4.0 * pos_qt + 4.0 * pos_cb + 6.0 * pos_sq + 4.0 * position + 1.0) / 24.0,
+            pos_qt / 24.0,
+        ),
+        axis=-1,
+    )
 
 
 def knot_weights(
-        positions: TensorLike,
-        num_knots: TensorLike,
-        degree: int,
-        cyclical: bool,
-        sparse_mode: bool = False,
-        name: str = "bspline_knot_weights") -> Union[tf.Tensor, Tuple[tf.Tensor, tf.Tensor]]:
+    positions: TensorLike,
+    num_knots: TensorLike,
+    degree: int,
+    cyclical: bool,
+    sparse_mode: bool = False,
+    name: str = "bspline_knot_weights",
+) -> Union[tf.Tensor, Tuple[tf.Tensor, tf.Tensor]]:
     """Function that converts cardinal B-spline positions to knot weights.
     Note:
       In the following, A1 to An are optional batch dimensions.
     Args:
       positions: A tensor with shape `[A1, .. An]`. Positions must be between
         `[0, C - D)` for non-cyclical and `[0, C)` for cyclical splines, where `C`
         is the number of knots and `D` is the spline degree.
@@ -275,24 +315,23 @@
         if degree > 4 or degree < 0:
             raise ValueError("Degree should be between 0 and 4.")
         if degree > num_knots - 1:
             raise ValueError("Degree cannot be >= number of knots.")
         if cyclical:
             positions = assert_all_in_range(positions, 0.0, float(num_knots))
         else:
-            positions = assert_all_in_range(positions, 0.0,
-                                            float(num_knots - degree))
+            positions = assert_all_in_range(positions, 0.0, float(num_knots - degree))
 
         all_basis_functions = {
             # Maps valid degrees to functions.
             Degree.CONSTANT: _constant,
             Degree.LINEAR: _linear,
             Degree.QUADRATIC: _quadratic,
             Degree.CUBIC: _cubic,
-            Degree.QUARTIC: _quartic
+            Degree.QUARTIC: _quartic,
         }
         basis_functions = all_basis_functions[degree]
 
         if not cyclical and num_knots - degree == 1:
             # In this case all weights are non-zero and we can just return them.
             if not sparse_mode:
                 return basis_functions(positions)
@@ -309,54 +348,63 @@
         sparse_weights = basis_functions(positions - shift)
         shift = tf.cast(shift, tf.int32)
 
         if sparse_mode:
             # Returns just the weights and the shift amounts, so that tf.gather_nd on
             # the knots can be used to sparsely activate knots if needed.
             shape_weights = tf.concat(
-                (shape_batch, tf.constant((degree + 1,), dtype=tf.int32)), axis=0)
+                (shape_batch, tf.constant((degree + 1,), dtype=tf.int32)), axis=0
+            )
             sparse_weights = tf.reshape(sparse_weights, shape=shape_weights)
             shift = tf.reshape(shift, shape=shape_batch)
             return sparse_weights, shift
 
         num_positions = tf.size(input=positions)
         ind_row, ind_col = tf.meshgrid(
             tf.range(num_positions, dtype=tf.int32),
             tf.range(degree + 1, dtype=tf.int32),
-            indexing="ij")
+            indexing="ij",
+        )
 
         tiled_shifts = tf.reshape(
             tf.tile(tf.expand_dims(shift, axis=-1), multiples=(1, degree + 1)),
-            shape=(-1,))
+            shape=(-1,),
+        )
         ind_col = tf.reshape(ind_col, shape=(-1,)) + tiled_shifts
         if cyclical:
             ind_col = tf.math.mod(ind_col, num_knots)
         indices = tf.stack((tf.reshape(ind_row, shape=(-1,)), ind_col), axis=-1)
-        shape_indices = tf.concat((tf.reshape(
-            num_positions, shape=(1,)), tf.constant(
-            (degree + 1, 2), dtype=tf.int32)),
-            axis=0)
+        shape_indices = tf.concat(
+            (
+                tf.reshape(num_positions, shape=(1,)),
+                tf.constant((degree + 1, 2), dtype=tf.int32),
+            ),
+            axis=0,
+        )
         indices = tf.reshape(indices, shape=shape_indices)
-        shape_scatter = tf.concat((tf.reshape(
-            num_positions, shape=(1,)), tf.constant((num_knots,), dtype=tf.int32)),
-            axis=0)
+        shape_scatter = tf.concat(
+            (
+                tf.reshape(num_positions, shape=(1,)),
+                tf.constant((num_knots,), dtype=tf.int32),
+            ),
+            axis=0,
+        )
         weights = tf.scatter_nd(indices, sparse_weights, shape_scatter)
         shape_weights = tf.concat(
-            (shape_batch, tf.constant((num_knots,), dtype=tf.int32)), axis=0)
+            (shape_batch, tf.constant((num_knots,), dtype=tf.int32)), axis=0
+        )
         return tf.reshape(weights, shape=shape_weights)
 
 
-TFG_ADD_ASSERTS_TO_GRAPH = 'tfg_add_asserts_to_graph'
+TFG_ADD_ASSERTS_TO_GRAPH = "tfg_add_asserts_to_graph"
 
 
-def assert_all_in_range(vector,
-                        minval,
-                        maxval,
-                        open_bounds=False,
-                        name='assert_all_in_range'):
+def assert_all_in_range(
+    vector, minval, maxval, open_bounds=False, name="assert_all_in_range"
+):
     """Checks whether all values of vector are between minval and maxval.
     This function checks if all the values in the given vector are in an interval
     `[minval, maxval]` if `open_bounds` is `False`, or in `]minval, maxval[` if it
     is set to `True`.
     Note:
       In the following, A1 to An are optional batch dimensions.
     Args:
@@ -381,14 +429,18 @@
 
     with tf.name_scope(name):
         vector = tf.convert_to_tensor(value=vector)
         minval = tf.convert_to_tensor(value=minval, dtype=vector.dtype)
         maxval = tf.convert_to_tensor(value=maxval, dtype=vector.dtype)
 
         if open_bounds:
-            assert_ops = (tf.debugging.assert_less(vector, maxval),
-                          tf.debugging.assert_greater(vector, minval))
+            assert_ops = (
+                tf.debugging.assert_less(vector, maxval),
+                tf.debugging.assert_greater(vector, minval),
+            )
         else:
-            assert_ops = (tf.debugging.assert_less_equal(vector, maxval),
-                          tf.debugging.assert_greater_equal(vector, minval))
+            assert_ops = (
+                tf.debugging.assert_less_equal(vector, maxval),
+                tf.debugging.assert_greater_equal(vector, minval),
+            )
         with tf.control_dependencies(assert_ops):
             return tf.identity(vector)
```

### Comparing `par_segmentation-0.1.8/par_segmentation.egg-info/PKG-INFO` & `par_segmentation-0.1.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,16 @@
-Metadata-Version: 2.1
-Name: par-segmentation
-Version: 0.1.8
-Summary: Cell cortex segmentation in C. elegans PAR protein images
-Author: Tom Bland
-Author-email: tom_bland@hotmail.co.uk
-License: CC BY 4.0
-Project-URL: Source Code, https://github.com/tsmbland/par-segmentation
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PAR Segmentation
 
 [![CC BY 4.0][cc-by-shield]][cc-by]
 ![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white)
 [![PyPi version](https://badgen.net/pypi/v/par-segmentation/)](https://pypi.org/project/par-segmentation)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tsmbland/par-segmentation/HEAD?filepath=%2Fscripts/Tutorial.ipynb)
 [![run with docker](https://img.shields.io/badge/run%20with-docker-0db7ed?logo=docker)](https://www.docker.com/)
 [![run with conda](http://img.shields.io/badge/run%20with-conda-3EB049?logo=anaconda)](https://docs.conda.io/en/latest/)
+[![Documentation Status](https://readthedocs.org/projects/par-segmentation/badge/?version=latest)](https://par-segmentation.readthedocs.io/en/latest/?badge=latest)
 
 Tools for segmenting, straightening and quantifying the cortex of cells.
 Works by combining spline-based segmentation with a custom quantification model, using a gradient descent optimisation procedure.
 Designed primarily for membrane-bound PAR proteins in C. elegans zygotes.
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/tsmbland/par-segmentation/master/scripts/Figs/animation.gif" width="100%" height="100%"/>
```

### Comparing `par_segmentation-0.1.8/par_segmentation.egg-info/SOURCES.txt` & `par_segmentation-0.1.9/par_segmentation.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 par_segmentation/__init__.py
+par_segmentation/_tgf_interpolate.py
 par_segmentation/funcs.py
 par_segmentation/interactive.py
 par_segmentation/legacy.py
 par_segmentation/model.py
 par_segmentation/quantifier.py
 par_segmentation/roi.py
-par_segmentation/tgf_interpolate.py
 par_segmentation.egg-info/PKG-INFO
 par_segmentation.egg-info/SOURCES.txt
 par_segmentation.egg-info/dependency_links.txt
 par_segmentation.egg-info/requires.txt
 par_segmentation.egg-info/top_level.txt
 tests/__init__.py
 tests/test_de_completion.py
```

### Comparing `par_segmentation-0.1.8/setup.py` & `par_segmentation-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='par_segmentation',
-    version='0.1.8',
+    version='0.1.9',
     license="CC BY 4.0",
     author='Tom Bland',
     author_email='tom_bland@hotmail.co.uk',
     packages=find_packages(),
     install_requires=['numpy',
                       'matplotlib',
                       'scipy',
```

### Comparing `par_segmentation-0.1.8/tests/test_de_completion.py` & `par_segmentation-0.1.9/tests/test_de_completion.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from par_segmentation import *
-
+import os
+import numpy as np
 
 class TestDeCompletion:
     """
     Testing that the differential evolution optimiser runs to completion
     NOT testing that any results are as expected
 
     """
```

### Comparing `par_segmentation-0.1.8/tests/test_de_correct.py` & `par_segmentation-0.1.9/tests/test_de_correct.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from par_segmentation import *
 import pytest
+import os
+import numpy as np
 
 class TestDeCorrectTests:
     """
     Making sure results from differential evolution optimiser are as expected
     Note: if underlying algorithm is changed, or default parameters are changed, tests may fail
 
     """
```

### Comparing `par_segmentation-0.1.8/tests/test_gd_completion.py` & `par_segmentation-0.1.9/tests/test_gd_completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from par_segmentation import *
+import os
+import numpy as np
 
 
 
 class TestGdCompletion:
     """
 
     GRADIENT DESCENT COMPLETION TESTS
```

### Comparing `par_segmentation-0.1.8/tests/test_gd_correct.py` & `par_segmentation-0.1.9/tests/test_gd_correct.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from par_segmentation import *
 import pytest
+import os
+import numpy as np
 
 
 class TestGdCorrect:
     """
     Making sure results from gradient descent optimiser are as expected
     Note: if underlying algorithm is changed, or default parameters are changed, tests may fail
```

