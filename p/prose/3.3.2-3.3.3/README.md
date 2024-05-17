# Comparing `tmp/prose-3.3.2.tar.gz` & `tmp/prose-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prose-3.3.2.tar", max compression
+gzip compressed data, was "prose-3.3.3.tar", max compression
```

## Comparing `prose-3.3.2.tar` & `prose-3.3.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1097 2024-03-25 11:25:01.168869 prose-3.3.2/LICENSE
--rw-r--r--   0        0        0     3580 2024-03-25 11:25:01.168869 prose-3.3.2/README.md
--rw-r--r--   0        0        0      652 2024-03-25 11:25:01.252870 prose-3.3.2/prose/__init__.py
--rw-r--r--   0        0        0       84 2024-03-25 11:25:01.252870 prose-3.3.2/prose/archive/__init__.py
--rw-r--r--   0        0        0     2397 2024-03-25 11:25:01.252870 prose-3.3.2/prose/archive/pos1.py
--rw-r--r--   0        0        0     2071 2024-03-25 11:25:01.252870 prose-3.3.2/prose/archive/sdss.py
--rw-r--r--   0        0        0      254 2024-03-25 11:25:01.252870 prose-3.3.2/prose/blocks/__init__.py
--rw-r--r--   0        0        0     4837 2024-03-25 11:25:01.252870 prose-3.3.2/prose/blocks/alignment.py
--rw-r--r--   0        0        0     3695 2024-03-25 11:25:01.252870 prose-3.3.2/prose/blocks/background.py
--rw-r--r--   0        0        0    11053 2024-03-25 11:25:01.252870 prose-3.3.2/prose/blocks/catalogs.py
--rw-r--r--   0        0        0     8794 2024-03-25 11:25:01.252870 prose-3.3.2/prose/blocks/centroids.py
--rw-r--r--   0        0        0    13782 2024-03-25 11:25:01.252870 prose-3.3.2/prose/blocks/detection.py
--rw-r--r--   0        0        0    10729 2024-03-25 11:25:01.252870 prose-3.3.2/prose/blocks/geometry.py
--rw-r--r--   0        0        0     4332 2024-03-25 11:25:01.252870 prose-3.3.2/prose/blocks/photometry.py
--rw-r--r--   0        0        0    14031 2024-03-25 11:25:01.252870 prose-3.3.2/prose/blocks/psf.py
--rw-r--r--   0        0        0     3703 2024-03-25 11:25:01.252870 prose-3.3.2/prose/blocks/shepard.py
--rw-r--r--   0        0        0    21609 2024-03-25 11:25:01.252870 prose-3.3.2/prose/blocks/utils.py
--rw-r--r--   0        0        0     4511 2024-03-25 11:25:01.252870 prose-3.3.2/prose/blocks/visualization.py
--rw-r--r--   0        0        0     4069 2024-03-25 11:25:01.252870 prose-3.3.2/prose/builtins.py
--rw-r--r--   0        0        0    10673 2024-03-25 11:25:01.252870 prose-3.3.2/prose/citations.py
--rw-r--r--   0        0        0     5933 2024-03-25 11:25:01.252870 prose-3.3.2/prose/config.py
--rw-r--r--   0        0        0     3733 2024-03-25 11:25:01.252870 prose-3.3.2/prose/console_utils.py
--rw-r--r--   0        0        0      120 2024-03-25 11:25:01.252870 prose-3.3.2/prose/core/__init__.py
--rw-r--r--   0        0        0     4940 2024-03-25 11:25:01.252870 prose-3.3.2/prose/core/block.py
--rw-r--r--   0        0        0    25720 2024-03-25 11:25:01.252870 prose-3.3.2/prose/core/image.py
--rw-r--r--   0        0        0    10085 2024-03-25 11:25:01.252870 prose-3.3.2/prose/core/sequence.py
--rw-r--r--   0        0        0    16920 2024-03-25 11:25:01.252870 prose-3.3.2/prose/core/source.py
--rw-r--r--   0        0        0    19073 2024-03-25 11:25:01.252870 prose-3.3.2/prose/fluxes.py
--rw-r--r--   0        0        0      137 2024-03-25 11:25:01.252870 prose-3.3.2/prose/io/__init__.py
--rw-r--r--   0        0        0      686 2024-03-25 11:25:01.256870 prose-3.3.2/prose/io/create_fm_db.sql
--rw-r--r--   0        0        0    25619 2024-03-25 11:25:01.256870 prose-3.3.2/prose/io/fitsmanager.py
--rw-r--r--   0        0        0     7473 2024-03-25 11:25:01.256870 prose-3.3.2/prose/io/io.py
--rw-r--r--   0        0        0     3048 2024-03-25 11:25:01.256870 prose-3.3.2/prose/scripts/fitsmanager.py
--rw-r--r--   0        0        0    15043 2024-03-25 11:25:01.256870 prose-3.3.2/prose/simulations.py
--rw-r--r--   0        0        0     7901 2024-03-25 11:25:01.256870 prose-3.3.2/prose/telescope.py
--rw-r--r--   0        0        0    14691 2024-03-25 11:25:01.256870 prose-3.3.2/prose/utils.py
--rw-r--r--   0        0        0    29851 2024-03-25 11:25:01.256870 prose-3.3.2/prose/visualization.py
--rw-r--r--   0        0        0     1100 2024-03-25 11:25:01.256870 prose-3.3.2/pyproject.toml
--rw-r--r--   0        0        0     4668 1970-01-01 00:00:00.000000 prose-3.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1097 2024-05-17 18:43:00.027459 prose-3.3.3/LICENSE
+-rw-r--r--   0        0        0     3580 2024-05-17 18:43:00.027459 prose-3.3.3/README.md
+-rw-r--r--   0        0        0      652 2024-05-17 18:43:00.111460 prose-3.3.3/prose/__init__.py
+-rw-r--r--   0        0        0       84 2024-05-17 18:43:00.111460 prose-3.3.3/prose/archive/__init__.py
+-rw-r--r--   0        0        0     2397 2024-05-17 18:43:00.111460 prose-3.3.3/prose/archive/pos1.py
+-rw-r--r--   0        0        0     2071 2024-05-17 18:43:00.111460 prose-3.3.3/prose/archive/sdss.py
+-rw-r--r--   0        0        0      254 2024-05-17 18:43:00.111460 prose-3.3.3/prose/blocks/__init__.py
+-rw-r--r--   0        0        0     4837 2024-05-17 18:43:00.111460 prose-3.3.3/prose/blocks/alignment.py
+-rw-r--r--   0        0        0     3695 2024-05-17 18:43:00.111460 prose-3.3.3/prose/blocks/background.py
+-rw-r--r--   0        0        0    11053 2024-05-17 18:43:00.111460 prose-3.3.3/prose/blocks/catalogs.py
+-rw-r--r--   0        0        0     8794 2024-05-17 18:43:00.111460 prose-3.3.3/prose/blocks/centroids.py
+-rw-r--r--   0        0        0    13782 2024-05-17 18:43:00.111460 prose-3.3.3/prose/blocks/detection.py
+-rw-r--r--   0        0        0    10729 2024-05-17 18:43:00.111460 prose-3.3.3/prose/blocks/geometry.py
+-rw-r--r--   0        0        0     4332 2024-05-17 18:43:00.111460 prose-3.3.3/prose/blocks/photometry.py
+-rw-r--r--   0        0        0    13911 2024-05-17 18:43:00.111460 prose-3.3.3/prose/blocks/psf.py
+-rw-r--r--   0        0        0     3703 2024-05-17 18:43:00.111460 prose-3.3.3/prose/blocks/shepard.py
+-rw-r--r--   0        0        0    21609 2024-05-17 18:43:00.111460 prose-3.3.3/prose/blocks/utils.py
+-rw-r--r--   0        0        0     4511 2024-05-17 18:43:00.111460 prose-3.3.3/prose/blocks/visualization.py
+-rw-r--r--   0        0        0     4069 2024-05-17 18:43:00.111460 prose-3.3.3/prose/builtins.py
+-rw-r--r--   0        0        0    10673 2024-05-17 18:43:00.111460 prose-3.3.3/prose/citations.py
+-rw-r--r--   0        0        0     5933 2024-05-17 18:43:00.111460 prose-3.3.3/prose/config.py
+-rw-r--r--   0        0        0     3733 2024-05-17 18:43:00.111460 prose-3.3.3/prose/console_utils.py
+-rw-r--r--   0        0        0      120 2024-05-17 18:43:00.111460 prose-3.3.3/prose/core/__init__.py
+-rw-r--r--   0        0        0     4940 2024-05-17 18:43:00.111460 prose-3.3.3/prose/core/block.py
+-rw-r--r--   0        0        0    25720 2024-05-17 18:43:00.111460 prose-3.3.3/prose/core/image.py
+-rw-r--r--   0        0        0    10085 2024-05-17 18:43:00.111460 prose-3.3.3/prose/core/sequence.py
+-rw-r--r--   0        0        0    16920 2024-05-17 18:43:00.111460 prose-3.3.3/prose/core/source.py
+-rw-r--r--   0        0        0    19073 2024-05-17 18:43:00.111460 prose-3.3.3/prose/fluxes.py
+-rw-r--r--   0        0        0      137 2024-05-17 18:43:00.111460 prose-3.3.3/prose/io/__init__.py
+-rw-r--r--   0        0        0      686 2024-05-17 18:43:00.111460 prose-3.3.3/prose/io/create_fm_db.sql
+-rw-r--r--   0        0        0    25619 2024-05-17 18:43:00.111460 prose-3.3.3/prose/io/fitsmanager.py
+-rw-r--r--   0        0        0     7473 2024-05-17 18:43:00.111460 prose-3.3.3/prose/io/io.py
+-rw-r--r--   0        0        0     3048 2024-05-17 18:43:00.111460 prose-3.3.3/prose/scripts/fitsmanager.py
+-rw-r--r--   0        0        0    15043 2024-05-17 18:43:00.111460 prose-3.3.3/prose/simulations.py
+-rw-r--r--   0        0        0     7901 2024-05-17 18:43:00.111460 prose-3.3.3/prose/telescope.py
+-rw-r--r--   0        0        0    14691 2024-05-17 18:43:00.115460 prose-3.3.3/prose/utils.py
+-rw-r--r--   0        0        0    29851 2024-05-17 18:43:00.115460 prose-3.3.3/prose/visualization.py
+-rw-r--r--   0        0        0     1106 2024-05-17 18:43:00.115460 prose-3.3.3/pyproject.toml
+-rw-r--r--   0        0        0     4618 1970-01-01 00:00:00.000000 prose-3.3.3/PKG-INFO
```

### Comparing `prose-3.3.2/LICENSE` & `prose-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/README.md` & `prose-3.3.3/README.md`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/__init__.py` & `prose-3.3.3/prose/__init__.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/archive/pos1.py` & `prose-3.3.3/prose/archive/pos1.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/archive/sdss.py` & `prose-3.3.3/prose/archive/sdss.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/blocks/alignment.py` & `prose-3.3.3/prose/blocks/alignment.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/blocks/background.py` & `prose-3.3.3/prose/blocks/background.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/blocks/catalogs.py` & `prose-3.3.3/prose/blocks/catalogs.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/blocks/centroids.py` & `prose-3.3.3/prose/blocks/centroids.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/blocks/detection.py` & `prose-3.3.3/prose/blocks/detection.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/blocks/geometry.py` & `prose-3.3.3/prose/blocks/geometry.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/blocks/photometry.py` & `prose-3.3.3/prose/blocks/photometry.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/blocks/psf.py` & `prose-3.3.3/prose/blocks/psf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import numpy as np
 
 from prose import Block, Image
 
 try:
-    from jax.config import config
-
-    config.update("jax_enable_x64", True)
     import jax
+
+    jax.config.update("jax_enable_x64", True)
     import jax.numpy as jnp
     from jaxopt import ScipyMinimize
 except ModuleNotFoundError:
     pass
 
 from astropy.stats import gaussian_sigma_to_fwhm
 from scipy.optimize import minimize
@@ -287,23 +286,17 @@
         opt = minimize(nll, p0, bounds=bounds).x
         return dict(zip(keys, opt))
 
     def model_function(self):
         def model(height, xo, yo, sx, sy, theta, m):
             dx = self.x - xo
             dy = self.y - yo
-            a = (np.cos(theta) ** 2) / (2 * sx**2) + (np.sin(theta) ** 2) / (
-                2 * sy**2
-            )
-            b = -(np.sin(2 * theta)) / (4 * sx**2) + (np.sin(2 * theta)) / (
-                4 * sy**2
-            )
-            c = (np.sin(theta) ** 2) / (2 * sx**2) + (np.cos(theta) ** 2) / (
-                2 * sy**2
-            )
+            a = (np.cos(theta) ** 2) / (2 * sx**2) + (np.sin(theta) ** 2) / (2 * sy**2)
+            b = -(np.sin(2 * theta)) / (4 * sx**2) + (np.sin(2 * theta)) / (4 * sy**2)
+            c = (np.sin(theta) ** 2) / (2 * sx**2) + (np.cos(theta) ** 2) / (2 * sy**2)
             psf = height * np.exp(-(a * dx**2 + 2 * b * dx * dy + c * dy**2))
             return psf + m
 
         return model
 
     @property
     def model(self):
```

### Comparing `prose-3.3.2/prose/blocks/shepard.py` & `prose-3.3.3/prose/blocks/shepard.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/blocks/utils.py` & `prose-3.3.3/prose/blocks/utils.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/blocks/visualization.py` & `prose-3.3.3/prose/blocks/visualization.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/builtins.py` & `prose-3.3.3/prose/builtins.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/citations.py` & `prose-3.3.3/prose/citations.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/config.py` & `prose-3.3.3/prose/config.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/console_utils.py` & `prose-3.3.3/prose/console_utils.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/core/block.py` & `prose-3.3.3/prose/core/block.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/core/image.py` & `prose-3.3.3/prose/core/image.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/core/sequence.py` & `prose-3.3.3/prose/core/sequence.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/core/source.py` & `prose-3.3.3/prose/core/source.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/fluxes.py` & `prose-3.3.3/prose/fluxes.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/io/create_fm_db.sql` & `prose-3.3.3/prose/io/create_fm_db.sql`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/io/fitsmanager.py` & `prose-3.3.3/prose/io/fitsmanager.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/io/io.py` & `prose-3.3.3/prose/io/io.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/scripts/fitsmanager.py` & `prose-3.3.3/prose/scripts/fitsmanager.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/simulations.py` & `prose-3.3.3/prose/simulations.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/telescope.py` & `prose-3.3.3/prose/telescope.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/utils.py` & `prose-3.3.3/prose/utils.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/prose/visualization.py` & `prose-3.3.3/prose/visualization.py`

 * *Files identical despite different names*

### Comparing `prose-3.3.2/pyproject.toml` & `prose-3.3.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "prose"
-version = "3.3.2"
+version = "3.3.3"
 description = "Modular image processing pipelines for Astronomy"
 authors = ["Lionel Garcia"]
 license = "MIT"
 readme = "README.md"
 include = ["prose/io/*.sql"]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.9,<3.12"
 numpy = "^1.23.5"
 astropy = "^5.1.1"
 astroquery = "^0.4.6"
 requests = "^2.31.0"
 ipython = "*"
 scipy = "*"
 matplotlib = "*"
@@ -30,15 +30,15 @@
 imageio = { version = "*", extras = ["ffmpeg"] }
 
 [tool.poetry.group.dev.dependencies]
 pytest = "*"
 black = "*"
 
 [tool.poetry.group.jax.dependencies]
-jax = "*"
+jax = "^0.4.26"
 jaxopt = "*"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "*"
 docutils = "*"
 jupyterlab = "*"
 myst-parser = "*"
```

### Comparing `prose-3.3.2/PKG-INFO` & `prose-3.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: prose
-Version: 3.3.2
+Version: 3.3.3
 Summary: Modular image processing pipelines for Astronomy
 License: MIT
 Author: Lionel Garcia
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: astropy (>=5.1.1,<6.0.0)
 Requires-Dist: astroquery (>=0.4.6,<0.5.0)
 Requires-Dist: celerite2
 Requires-Dist: imageio[ffmpeg]
```

#### html2text {}

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 2.1 Name: prose Version: 3.3.2 Summary: Modular image
+Metadata-Version: 2.1 Name: prose Version: 3.3.3 Summary: Modular image
 processing pipelines for Astronomy License: MIT Author: Lionel Garcia Requires-
-Python: >=3.8,<3.12 Classifier: License :: OSI Approved :: MIT License
+Python: >=3.9,<3.12 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: astropy (>=5.1.1,<6.0.0) Requires-
-Dist: astroquery (>=0.4.6,<0.5.0) Requires-Dist: celerite2 Requires-Dist:
-imageio[ffmpeg] Requires-Dist: ipython Requires-Dist: matplotlib Requires-Dist:
-multiprocess Requires-Dist: numpy (>=1.23.5,<2.0.0) Requires-Dist: pandas
-(>1.1) Requires-Dist: photutils (>=1.6.0,<2.0.0) Requires-Dist: pytest
-Requires-Dist: pyyaml Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist:
-scikit-image (>=0.21.0,<0.22.0) Requires-Dist: scipy Requires-Dist: sep
-Requires-Dist: tabulate Requires-Dist: tqdm Requires-Dist: twirl (==0.4.0)
-Description-Content-Type: text/markdown # prose
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: astropy
+(>=5.1.1,<6.0.0) Requires-Dist: astroquery (>=0.4.6,<0.5.0) Requires-Dist:
+celerite2 Requires-Dist: imageio[ffmpeg] Requires-Dist: ipython Requires-Dist:
+matplotlib Requires-Dist: multiprocess Requires-Dist: numpy (>=1.23.5,<2.0.0)
+Requires-Dist: pandas (>1.1) Requires-Dist: photutils (>=1.6.0,<2.0.0)
+Requires-Dist: pytest Requires-Dist: pyyaml Requires-Dist: requests
+(>=2.31.0,<3.0.0) Requires-Dist: scikit-image (>=0.21.0,<0.22.0) Requires-Dist:
+scipy Requires-Dist: sep Requires-Dist: tabulate Requires-Dist: tqdm Requires-
+Dist: twirl (==0.4.0) Description-Content-Type: text/markdown # prose
                            [docs/_static/prose3.png]
                Modular image processing pipelines for Astronomy
                     _[_g_i_t_h_u_b_]_[_l_i_c_e_n_s_e_]_[_p_a_p_e_r_]_[_d_o_c_u_m_e_n_t_a_t_i_o_n_]
 *prose* is a Python package to build modular image processing pipelines for
 Astronomy. *powered by [astropy](https://www.astropy.org/) and [photutils]
 (https://photutils.readthedocs.io)*! ## Example Here is a quick example
 pipeline to characterize the point-spread-function (PSF) of an example image
```

