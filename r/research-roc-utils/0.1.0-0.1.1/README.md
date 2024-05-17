# Comparing `tmp/research_roc_utils-0.1.0.tar.gz` & `tmp/research_roc_utils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "research_roc_utils-0.1.0.tar", last modified: Wed Apr 17 15:15:53 2024, max compression
+gzip compressed data, was "research_roc_utils-0.1.1.tar", last modified: Fri May 17 09:09:42 2024, max compression
```

## Comparing `research_roc_utils-0.1.0.tar` & `research_roc_utils-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-17 15:15:53.009930 research_roc_utils-0.1.0/
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)     1080 2024-04-12 08:42:51.000000 research_roc_utils-0.1.0/LICENSE
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)    16577 2024-04-17 15:15:53.009583 research_roc_utils-0.1.0/PKG-INFO
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)    16031 2024-04-17 08:22:56.000000 research_roc_utils-0.1.0/README.md
-drwxr-xr-x   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-17 15:15:53.007869 research_roc_utils-0.1.0/research_roc_utils/
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-16 07:47:53.000000 research_roc_utils-0.1.0/research_roc_utils/__init__.py
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)    19608 2024-04-17 15:09:07.000000 research_roc_utils-0.1.0/research_roc_utils/roc_utils.py
-drwxr-xr-x   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-17 15:15:53.009220 research_roc_utils-0.1.0/research_roc_utils.egg-info/
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)    16577 2024-04-17 15:15:52.000000 research_roc_utils-0.1.0/research_roc_utils.egg-info/PKG-INFO
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      298 2024-04-17 15:15:52.000000 research_roc_utils-0.1.0/research_roc_utils.egg-info/SOURCES.txt
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        1 2024-04-17 15:15:52.000000 research_roc_utils-0.1.0/research_roc_utils.egg-info/dependency_links.txt
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      125 2024-04-17 15:15:52.000000 research_roc_utils-0.1.0/research_roc_utils.egg-info/requires.txt
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)       19 2024-04-17 15:15:52.000000 research_roc_utils-0.1.0/research_roc_utils.egg-info/top_level.txt
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)       38 2024-04-17 15:15:53.010002 research_roc_utils-0.1.0/setup.cfg
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)     1179 2024-04-17 15:11:22.000000 research_roc_utils-0.1.0/setup.py
+drwxr-xr-x   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-05-17 09:09:42.636283 research_roc_utils-0.1.1/
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)     1080 2024-04-12 08:42:51.000000 research_roc_utils-0.1.1/LICENSE
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)    16600 2024-05-17 09:09:42.636028 research_roc_utils-0.1.1/PKG-INFO
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)    16054 2024-04-17 16:01:35.000000 research_roc_utils-0.1.1/README.md
+drwxr-xr-x   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-05-17 09:09:42.634282 research_roc_utils-0.1.1/research_roc_utils/
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-16 07:47:53.000000 research_roc_utils-0.1.1/research_roc_utils/__init__.py
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)    19605 2024-05-17 08:56:56.000000 research_roc_utils-0.1.1/research_roc_utils/roc_utils.py
+drwxr-xr-x   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-05-17 09:09:42.635733 research_roc_utils-0.1.1/research_roc_utils.egg-info/
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)    16600 2024-05-17 09:09:42.000000 research_roc_utils-0.1.1/research_roc_utils.egg-info/PKG-INFO
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      298 2024-05-17 09:09:42.000000 research_roc_utils-0.1.1/research_roc_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        1 2024-05-17 09:09:42.000000 research_roc_utils-0.1.1/research_roc_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      125 2024-05-17 09:09:42.000000 research_roc_utils-0.1.1/research_roc_utils.egg-info/requires.txt
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)       19 2024-05-17 09:09:42.000000 research_roc_utils-0.1.1/research_roc_utils.egg-info/top_level.txt
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)       38 2024-05-17 09:09:42.636338 research_roc_utils-0.1.1/setup.cfg
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)     1179 2024-05-17 08:59:33.000000 research_roc_utils-0.1.1/setup.py
```

### Comparing `research_roc_utils-0.1.0/LICENSE` & `research_roc_utils-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `research_roc_utils-0.1.0/PKG-INFO` & `research_roc_utils-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: research_roc_utils
-Version: 0.1.0
+Version: 0.1.1
 Summary: Utility functions to assist in the computation of ROC curve comparisons based on academic research.
 Home-page: https://github.com/jpbruehw/research-roc-utils
 Author: J.P. Bruehwiler
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pandas>=2.2.2
 Requires-Dist: matplotlib>=3.8.4
 Requires-Dist: scikit-learn>=1.4.2
 Requires-Dist: scikits.bootstrap==1.1.0
 Requires-Dist: scipy>=1.13.0
 Requires-Dist: scikit-learn>=1.4.2
 
 <p align="center">
-    <img src="https://i.postimg.cc/265WB2yK/roc-curve-package.png"/>
+    <img src="https://i.postimg.cc/vZPgPZZz/roc-curve-package.png" style="height: 450px;"/>
 </p>
 
 # Research Utility Package for ROC Curves and AUROC Analysis
 
 <b>Fun Fact:</b> The term “Receiver Operating Characteristic” has its roots in <a href="https://www.statisticshowto.com/receiver-operating-characteristic-roc-curve/" target="_blank">World War II</a>. ROC curves were originally developed by the British as part of the <a href="https://en.wikipedia.org/wiki/Chain_Home" target="_blank">Chain Home</a> radar system. The analysis technique was used to differentiate between enemny aircraft and random noise.
 
 ## Table of Contents
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: research_roc_utils Version: 0.1.0 Summary: Utility
+Metadata-Version: 2.1 Name: research_roc_utils Version: 0.1.1 Summary: Utility
 functions to assist in the computation of ROC curve comparisons based on
 academic research. Home-page: https://github.com/jpbruehw/research-roc-utils
 Author: J.P. Bruehwiler Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: numpy>=1.26.4 Requires-Dist: pandas>=2.2.2 Requires-
 Dist: matplotlib>=3.8.4 Requires-Dist: scikit-learn>=1.4.2 Requires-Dist:
 scikits.bootstrap==1.1.0 Requires-Dist: scipy>=1.13.0 Requires-Dist: scikit-
 learn>=1.4.2
-             [https://i.postimg.cc/265WB2yK/roc-curve-package.png]
+             [https://i.postimg.cc/vZPgPZZz/roc-curve-package.png]
 # Research Utility Package for ROC Curves and AUROC Analysis FFuunn FFaacctt:: The term
 âReceiver Operating Characteristicâ has its roots in _W_o_r_l_d_ _W_a_r_ _I_I. ROC
 curves were originally developed by the British as part of the _C_h_a_i_n_ _H_o_m_e radar
 system. The analysis technique was used to differentiate between enemny
 aircraft and random noise. ## Table of Contents #### [What are ROC Curves?]
 (#what-are-roc-curves) #### [What is AUROC analysis?](#what-is-auroc-analysis)
 #### [Hanley and McNeil](#james-a-hanley-and-barbara-mcneil-methodology) ####
```

### Comparing `research_roc_utils-0.1.0/README.md` & `research_roc_utils-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-    <img src="https://i.postimg.cc/265WB2yK/roc-curve-package.png"/>
+    <img src="https://i.postimg.cc/vZPgPZZz/roc-curve-package.png" style="height: 450px;"/>
 </p>
 
 # Research Utility Package for ROC Curves and AUROC Analysis
 
 <b>Fun Fact:</b> The term “Receiver Operating Characteristic” has its roots in <a href="https://www.statisticshowto.com/receiver-operating-characteristic-roc-curve/" target="_blank">World War II</a>. ROC curves were originally developed by the British as part of the <a href="https://en.wikipedia.org/wiki/Chain_Home" target="_blank">Chain Home</a> radar system. The analysis technique was used to differentiate between enemny aircraft and random noise.
 
 ## Table of Contents
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-             [https://i.postimg.cc/265WB2yK/roc-curve-package.png]
+             [https://i.postimg.cc/vZPgPZZz/roc-curve-package.png]
 # Research Utility Package for ROC Curves and AUROC Analysis FFuunn FFaacctt:: The term
 âReceiver Operating Characteristicâ has its roots in _W_o_r_l_d_ _W_a_r_ _I_I. ROC
 curves were originally developed by the British as part of the _C_h_a_i_n_ _H_o_m_e radar
 system. The analysis technique was used to differentiate between enemny
 aircraft and random noise. ## Table of Contents #### [What are ROC Curves?]
 (#what-are-roc-curves) #### [What is AUROC analysis?](#what-is-auroc-analysis)
 #### [Hanley and McNeil](#james-a-hanley-and-barbara-mcneil-methodology) ####
```

### Comparing `research_roc_utils-0.1.0/research_roc_utils/roc_utils.py` & `research_roc_utils-0.1.1/research_roc_utils/roc_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,15 +206,15 @@
 # BOOTSTRAP RESAMPLING P-VALUE
 #----------------------------#
 
 def calculate_roc_score(y_true, y_pred, indices, score_fun, sample_weight):
     if sample_weight is not None:
         return score_fun(y_true[indices], y_pred[indices], sample_weight=sample_weight[indices])
     else:
-      return score_fun(y_true[indices], y_pred[indices])
+        return score_fun(y_true[indices], y_pred[indices])
   
 def convert_np_array(list_like):
     if isinstance(list_like, np.ndarray):
         return list_like
     else:
         return np.array(list_like)
   
@@ -226,36 +226,36 @@
     score_fun=roc_auc_score,
     sample_weight=None,
     n_resamples=5000,
     two_tailed=True,
     seed=None,
     reject_one_class_samples=True,
 ):
-    l = []
+    z = []
     
     # ensure that lists are array like object that have shape
     y_true = convert_np_array(y_true)
     y_pred_1 = convert_np_array(y_pred_1)
     y_pred_2 = convert_np_array(y_pred_2)
     
     indices = list(boot.bootstrap_indices(y_true, n_samples=n_resamples, seed=seed))
     
     for idx_vals in indices:
         if reject_one_class_samples and len(np.unique(y_true[idx_vals])) < 2:
             continue
         score_1 = calculate_roc_score(y_true, y_pred_1, idx_vals, score_fun, sample_weight)
         score_2 = calculate_roc_score(y_true, y_pred_2, idx_vals, score_fun, sample_weight)
-        l.append(compare_fun(score_1, score_2))
+        z.append(compare_fun(score_1, score_2))
 
-    p = percentileofscore(l, 0.0, kind="mean") / 100.0
+    p = percentileofscore(z, 0.0, kind="mean") / 100.0
 
     if two_tailed:
         p = 2 * min(p, 1-p)
         
-    return p, l
+    return p, z
 
 ##############################################################################
 # p4: Binary Model comparison functions that provide functionality
 # provides methods for t-stat, z-score, threshold calculations, as well as
 # creating stacked ROC curve plot to visualize multiple models
 # based on the academic research cited above 
 
@@ -339,16 +339,16 @@
     
     return z_score
 
 # calculate p-value with bootstrapping
 # method for comparing two models using 
 # at a given significance level with bootstrapping
 # 1 - p hypothesis test:
-# H0: Model 1 performance is significantly different from Model 2
-# H1: Model 1 is not significantly different from Model 2
+# H0: Model 1 and Model 2 have no difference in performance
+# H1: Model 2's performance is better than Model 1
 # returns p-val and list of the differences between models
 def boot_p_val(
     y_true,
     y_pred_1,
     y_pred_2,
     compare_fun=np.subtract,
     score_fun=roc_auc_score,
@@ -477,25 +477,25 @@
 # the original implementation of this 
 # methodology was to compare two investment strategies
 # paper link: https://shorturl.at/oEORV
 def auroc_non_parametric(y_true, y_pred):
     # get true neg and pos counts
     n_1 = sum(1 for y in y_true if y == 1)
     n_0 = sum(1 for y in y_true if y == 0)
-    # get geometric mean
-    g_mean = 1 / (n_1 * n_0)
+    # get reciprocal product
+    rec_prod = 1 / (n_1 * n_0)
     # create df and seperate
     df = pd.DataFrame({'y_true': y_true, 'y_pred': y_pred})
     # get predictions at 0 and 1
     y_pred_true = df[df['y_true'] == 1]['y_pred']
     y_pred_false = df[df['y_true'] == 0]['y_pred']
     # find sum
     total_sum = 0
     for zi in y_pred_true:
         for xj in y_pred_false:
             if zi > xj:
                 total_sum += 1
             elif zi == xj:
                 total_sum += 0.5
-    auroc = g_mean * total_sum
+    auroc = rec_prod * total_sum
     
     return auroc
```

### Comparing `research_roc_utils-0.1.0/research_roc_utils.egg-info/PKG-INFO` & `research_roc_utils-0.1.1/research_roc_utils.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: research-roc-utils
-Version: 0.1.0
+Version: 0.1.1
 Summary: Utility functions to assist in the computation of ROC curve comparisons based on academic research.
 Home-page: https://github.com/jpbruehw/research-roc-utils
 Author: J.P. Bruehwiler
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pandas>=2.2.2
 Requires-Dist: matplotlib>=3.8.4
 Requires-Dist: scikit-learn>=1.4.2
 Requires-Dist: scikits.bootstrap==1.1.0
 Requires-Dist: scipy>=1.13.0
 Requires-Dist: scikit-learn>=1.4.2
 
 <p align="center">
-    <img src="https://i.postimg.cc/265WB2yK/roc-curve-package.png"/>
+    <img src="https://i.postimg.cc/vZPgPZZz/roc-curve-package.png" style="height: 450px;"/>
 </p>
 
 # Research Utility Package for ROC Curves and AUROC Analysis
 
 <b>Fun Fact:</b> The term “Receiver Operating Characteristic” has its roots in <a href="https://www.statisticshowto.com/receiver-operating-characteristic-roc-curve/" target="_blank">World War II</a>. ROC curves were originally developed by the British as part of the <a href="https://en.wikipedia.org/wiki/Chain_Home" target="_blank">Chain Home</a> radar system. The analysis technique was used to differentiate between enemny aircraft and random noise.
 
 ## Table of Contents
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: research-roc-utils Version: 0.1.0 Summary: Utility
+Metadata-Version: 2.1 Name: research-roc-utils Version: 0.1.1 Summary: Utility
 functions to assist in the computation of ROC curve comparisons based on
 academic research. Home-page: https://github.com/jpbruehw/research-roc-utils
 Author: J.P. Bruehwiler Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: numpy>=1.26.4 Requires-Dist: pandas>=2.2.2 Requires-
 Dist: matplotlib>=3.8.4 Requires-Dist: scikit-learn>=1.4.2 Requires-Dist:
 scikits.bootstrap==1.1.0 Requires-Dist: scipy>=1.13.0 Requires-Dist: scikit-
 learn>=1.4.2
-             [https://i.postimg.cc/265WB2yK/roc-curve-package.png]
+             [https://i.postimg.cc/vZPgPZZz/roc-curve-package.png]
 # Research Utility Package for ROC Curves and AUROC Analysis FFuunn FFaacctt:: The term
 âReceiver Operating Characteristicâ has its roots in _W_o_r_l_d_ _W_a_r_ _I_I. ROC
 curves were originally developed by the British as part of the _C_h_a_i_n_ _H_o_m_e radar
 system. The analysis technique was used to differentiate between enemny
 aircraft and random noise. ## Table of Contents #### [What are ROC Curves?]
 (#what-are-roc-curves) #### [What is AUROC analysis?](#what-is-auroc-analysis)
 #### [Hanley and McNeil](#james-a-hanley-and-barbara-mcneil-methodology) ####
```

### Comparing `research_roc_utils-0.1.0/setup.py` & `research_roc_utils-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Python setup.py for project_name package"""
 import io
 import os
 from setuptools import find_packages, setup
 
 def read(*paths, **kwargs):
     """Read the contents of a text file safely.
-    >>> read("research_roc_utils", "0.1.0")
-    '0.1.0'
+    >>> read("research_roc_utils", "0.1.1")
+    '0.1.1'
     >>> read("README.md")
     ...
     """
 
     content = ""
     with io.open(
         os.path.join(os.path.dirname(__file__), *paths),
@@ -22,15 +22,15 @@
 def read_requirements(path):
     return [
         line.strip()
         for line in read(path).split("\n")
         if not line.startswith(('"', "#", "-", "git+"))
     ]
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 
 setup(
     name="research_roc_utils",
     version=VERSION,
     description="Utility functions to assist in the computation of ROC curve comparisons based on academic research.",
     url="https://github.com/jpbruehw/research-roc-utils",
     long_description=read("README.md"),
```

