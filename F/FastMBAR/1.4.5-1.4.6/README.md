# Comparing `tmp/fastmbar-1.4.5.tar.gz` & `tmp/fastmbar-1.4.6.tar.gz`

## Comparing `fastmbar-1.4.5.tar` & `fastmbar-1.4.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastmbar-1.4.5/.readthedocs.yaml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastmbar-1.4.5/.travis.yml
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fastmbar-1.4.5/build.sh
--rw-r--r--   0        0        0    33346 2020-02-02 00:00:00.000000 fastmbar-1.4.5/energy_matrix.pdf
--rw-r--r--   0        0        0   459263 2020-02-02 00:00:00.000000 fastmbar-1.4.5/energy_matrix.png
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 fastmbar-1.4.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 fastmbar-1.4.5/.vscode/settings.json
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 fastmbar-1.4.5/FastMBAR/__init__.py
--rw-r--r--   0        0        0    30281 2020-02-02 00:00:00.000000 fastmbar-1.4.5/FastMBAR/fastmbar.py
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 fastmbar-1.4.5/FastMBAR/test_FastMBAR.py
--rw-r--r--   0        0        0     9701 2020-02-02 00:00:00.000000 fastmbar-1.4.5/FastMBAR/utils/analyzer.py
--rw-r--r--   0        0        0     8086 2020-02-02 00:00:00.000000 fastmbar-1.4.5/FastMBAR/utils/fastmbartools.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 fastmbar-1.4.5/docs/.gitignore
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastmbar-1.4.5/docs/Makefile
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 fastmbar-1.4.5/docs/requirements.txt
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 fastmbar-1.4.5/docs/source/API.rst
--rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 fastmbar-1.4.5/docs/source/butane_PMF.rst
--rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 fastmbar-1.4.5/docs/source/conf.py
--rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 fastmbar-1.4.5/docs/source/dialanine_PMF.rst
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 fastmbar-1.4.5/docs/source/examples.rst
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 fastmbar-1.4.5/docs/source/index.rst
--rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 fastmbar-1.4.5/docs/source/installation.rst
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 fastmbar-1.4.5/docs/source/references.rst
--rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 fastmbar-1.4.5/docs/source/usage.rst
--rw-r--r--   0        0        0  1201731 2020-02-02 00:00:00.000000 fastmbar-1.4.5/docs/source/_static/logo.ai
--rw-r--r--   0        0        0  1249206 2020-02-02 00:00:00.000000 fastmbar-1.4.5/docs/source/_static/logo.eps
--rw-r--r--   0        0        0   119173 2020-02-02 00:00:00.000000 fastmbar-1.4.5/docs/source/_static/logo.png
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 fastmbar-1.4.5/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 fastmbar-1.4.5/LICENSE
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 fastmbar-1.4.5/README.rst
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 fastmbar-1.4.5/pyproject.toml
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 fastmbar-1.4.5/PKG-INFO
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastmbar-1.4.6/.readthedocs.yaml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastmbar-1.4.6/.travis.yml
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fastmbar-1.4.6/build.sh
+-rw-r--r--   0        0        0    33346 2020-02-02 00:00:00.000000 fastmbar-1.4.6/energy_matrix.pdf
+-rw-r--r--   0        0        0   459263 2020-02-02 00:00:00.000000 fastmbar-1.4.6/energy_matrix.png
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 fastmbar-1.4.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 fastmbar-1.4.6/.vscode/settings.json
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 fastmbar-1.4.6/FastMBAR/__init__.py
+-rw-r--r--   0        0        0    30285 2020-02-02 00:00:00.000000 fastmbar-1.4.6/FastMBAR/fastmbar.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 fastmbar-1.4.6/FastMBAR/test_FastMBAR.py
+-rw-r--r--   0        0        0     9701 2020-02-02 00:00:00.000000 fastmbar-1.4.6/FastMBAR/utils/analyzer.py
+-rw-r--r--   0        0        0     8086 2020-02-02 00:00:00.000000 fastmbar-1.4.6/FastMBAR/utils/fastmbartools.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 fastmbar-1.4.6/docs/.gitignore
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastmbar-1.4.6/docs/Makefile
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 fastmbar-1.4.6/docs/requirements.txt
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 fastmbar-1.4.6/docs/source/API.rst
+-rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 fastmbar-1.4.6/docs/source/butane_PMF.rst
+-rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 fastmbar-1.4.6/docs/source/conf.py
+-rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 fastmbar-1.4.6/docs/source/dialanine_PMF.rst
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 fastmbar-1.4.6/docs/source/examples.rst
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 fastmbar-1.4.6/docs/source/index.rst
+-rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 fastmbar-1.4.6/docs/source/installation.rst
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 fastmbar-1.4.6/docs/source/references.rst
+-rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 fastmbar-1.4.6/docs/source/usage.rst
+-rw-r--r--   0        0        0  1201731 2020-02-02 00:00:00.000000 fastmbar-1.4.6/docs/source/_static/logo.ai
+-rw-r--r--   0        0        0  1249206 2020-02-02 00:00:00.000000 fastmbar-1.4.6/docs/source/_static/logo.eps
+-rw-r--r--   0        0        0   119173 2020-02-02 00:00:00.000000 fastmbar-1.4.6/docs/source/_static/logo.png
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 fastmbar-1.4.6/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 fastmbar-1.4.6/LICENSE
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 fastmbar-1.4.6/README.rst
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 fastmbar-1.4.6/pyproject.toml
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 fastmbar-1.4.6/PKG-INFO
```

### Comparing `fastmbar-1.4.5/.readthedocs.yaml` & `fastmbar-1.4.6/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.5/energy_matrix.pdf` & `fastmbar-1.4.6/energy_matrix.pdf`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.5/energy_matrix.png` & `fastmbar-1.4.6/energy_matrix.png`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.5/.github/workflows/python-publish.yml` & `fastmbar-1.4.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.5/FastMBAR/fastmbar.py` & `fastmbar-1.4.6/FastMBAR/fastmbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 import torch
 import numpy as np
 import scipy.optimize as optimize
 import math
 
 __version__ = "1.4.5"
 
-## A small diagonal matrix with __EPS__ as its diagonal elements is added 
-## to the Hessian matrix to avoid the case where the Hessian matrix is singular 
+## A small diagonal matrix with __EPS__ as its diagonal elements is added
+## to the Hessian matrix to avoid the case where the Hessian matrix is singular
 ## due to underflow.
 __EPS__ = 1e-16
 
+
 class FastMBAR:
     """
     The FastMBAR class is initialized with an energy matrix and an array
     of num of conformations. The corresponding MBAR equation is solved
     in the constructor. Therefore, the relative free energies of states
     used in the energy matrix is calculated in the constructor. The
     method **calculate_free_energies_for_perturbed_states**
@@ -301,46 +302,46 @@
             self._log_prob_mix = torch.stack(log_prob_mix, dim=0)
             DeltaF = self._F_bootstrap[None, :, :] - self._F_bootstrap[:, None, :]
             self._DeltaF = torch.mean(DeltaF, dim=2)
             self._DeltaF_std = torch.std(DeltaF, dim=2)
 
     @property
     def F(self) -> np.ndarray:
-        """Free energies of the states under the constraint :math:`\sum_{k=1}^{M} N_k * F_k = 0`,
+        r"""Free energies of the states under the constraint :math:`\sum_{k=1}^{M} N_k * F_k = 0`,
         where :math:`N_k` is the number of conformations sampled from state k.
         """
         return self._F.cpu().numpy()
 
     @property
     def F_std(self) -> np.ndarray:
-        """Standard deviation of the free energies of the states under the constraint
+        r"""Standard deviation of the free energies of the states under the constraint
         :math:`\sum_{k=1}^{M} N_k * F_k = 0`,
         where :math:`N_k` is the number of conformations sampled from state k.
         """
         return self._F_std.cpu().numpy()
 
     @property
     def F_cov(self) -> np.ndarray:
-        """Covariance matrix of the free energies of the states under the constraint
+        r"""Covariance matrix of the free energies of the states under the constraint
         :math:`\sum_{k=1}^{M} N_k * F_k = 0`,
         where :math:`N_k` is the number of conformations sampled from state k.
         """
         return self._F_cov.cpu().numpy()
 
     @property
     def DeltaF(self) -> np.ndarray:
-        """Free energy difference between states.
+        r"""Free energy difference between states.
         :math:`\mathrm{DeltaF}[i,j]` is the free energy difference between state j and state i,
         i.e., :math:`\mathrm{DeltaF}[i,j] = F[j] - F[i]` .
         """
         return self._DeltaF.cpu().numpy()
 
     @property
     def DeltaF_std(self) -> np.ndarray:
-        """Standard deviation of the free energy difference between states.
+        r"""Standard deviation of the free energy difference between states.
         :math:`\mathrm{DeltaF_std}[i,j]` is the standard deviation of the free energy
         difference :math:`\mathrm{DeltaF}[i,j]`.
         """
         return self._DeltaF_std.cpu().numpy()
 
     @property
     def log_prob_mix(self) -> np.ndarray:
@@ -351,23 +352,23 @@
         ## Initilize dF by self-consistent iteration
         ## this is only required by the Newton's method, becuase when the inital guess
         ## is far away from the true solution, the Hessian matrix can be very close to
         ## singular due to underflow. This can be avoided by using a good initial guess.
         dF_init = energy.new_zeros(self.M - 1)
         for _ in range(10):
             F_init = torch.cat([dF_init.new_zeros(1), dF_init])
-            b = - F_init - torch.log(num_conf)
+            b = -F_init - torch.log(num_conf)
             log_prob_mix = torch.logsumexp(-(energy + b[:, None]), dim=0)
             du = energy + log_prob_mix
             F = -torch.logsumexp(-du, dim=1)
             dF_init = F[1:] - F[0]
         return dF_init
 
     def calculate_free_energies_of_perturbed_states(self, energy_perturbed):
-        """calculate free energies for perturbed states.
+        r"""calculate free energies for perturbed states.
 
         Parameters
         -----------
         energy_perturbed: 2-D float ndarray with size of (L,N)
             each row of the energy_perturbed matrix represents a state and
             the value energy_perturbed[l,n] represents the reduced energy
             of the n'th conformation in the l'th perturbed state.
```

### Comparing `fastmbar-1.4.5/FastMBAR/test_FastMBAR.py` & `fastmbar-1.4.6/FastMBAR/test_FastMBAR.py`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.5/FastMBAR/utils/analyzer.py` & `fastmbar-1.4.6/FastMBAR/utils/analyzer.py`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.5/FastMBAR/utils/fastmbartools.py` & `fastmbar-1.4.6/FastMBAR/utils/fastmbartools.py`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.5/docs/Makefile` & `fastmbar-1.4.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.5/docs/source/butane_PMF.rst` & `fastmbar-1.4.6/docs/source/butane_PMF.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.5/docs/source/conf.py` & `fastmbar-1.4.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.5/docs/source/dialanine_PMF.rst` & `fastmbar-1.4.6/docs/source/dialanine_PMF.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.5/docs/source/examples.rst` & `fastmbar-1.4.6/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.5/docs/source/index.rst` & `fastmbar-1.4.6/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.5/docs/source/installation.rst` & `fastmbar-1.4.6/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.5/docs/source/references.rst` & `fastmbar-1.4.6/docs/source/references.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.5/docs/source/usage.rst` & `fastmbar-1.4.6/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.5/docs/source/_static/logo.ai` & `fastmbar-1.4.6/docs/source/_static/logo.ai`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.5/docs/source/_static/logo.eps` & `fastmbar-1.4.6/docs/source/_static/logo.eps`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.5/docs/source/_static/logo.png` & `fastmbar-1.4.6/docs/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.5/LICENSE` & `fastmbar-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.5/README.rst` & `fastmbar-1.4.6/README.rst`

 * *Files identical despite different names*

### Comparing `fastmbar-1.4.5/pyproject.toml` & `fastmbar-1.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "FastMBAR"
-version = "1.4.5"
+version = "1.4.6"
 authors = [
   { name="Xinqiang Ding", email="Xinqiang.Ding@tufts.edu" }
 ]
 description = "A fast solver for large scale MBAR/UWHAM equations"
 readme = "README.rst"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `fastmbar-1.4.5/PKG-INFO` & `fastmbar-1.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: FastMBAR
-Version: 1.4.5
+Version: 1.4.6
 Summary: A fast solver for large scale MBAR/UWHAM equations
 Project-URL: Homepage, https://fastmbar.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/BrooksResearchGroup-UM/FastMBAR/issues
 Author-email: Xinqiang Ding <Xinqiang.Ding@tufts.edu>
 License: MIT License
         
         Copyright (c) 2018 Xinqiang Ding, Charles L. Brooks III
```

