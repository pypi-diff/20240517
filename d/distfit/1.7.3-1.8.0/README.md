# Comparing `tmp/distfit-1.7.3.tar.gz` & `tmp/distfit-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distfit-1.7.3.tar", last modified: Fri Dec  8 19:41:56 2023, max compression
+gzip compressed data, was "distfit-1.8.0.tar", last modified: Fri May 17 11:17:38 2024, max compression
```

## Comparing `distfit-1.7.3.tar` & `distfit-1.8.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-12-08 19:41:56.150240 distfit-1.7.3/
--rw-rw-rw-   0        0        0     1181 2023-09-30 18:07:42.000000 distfit-1.7.3/LICENSE
--rw-rw-rw-   0        0        0        0 2023-09-30 18:07:42.000000 distfit-1.7.3/MANIFEST.in
--rw-rw-rw-   0        0        0    11755 2023-12-08 19:41:56.150240 distfit-1.7.3/PKG-INFO
--rw-rw-rw-   0        0        0    11214 2023-09-30 18:07:42.000000 distfit-1.7.3/README.md
-drwxrwxrwx   0        0        0        0 2023-12-08 19:41:56.118975 distfit-1.7.3/distfit/
--rw-rw-rw-   0        0        0     2141 2023-12-08 19:36:21.000000 distfit-1.7.3/distfit/__init__.py
--rw-rw-rw-   0        0        0   121964 2023-12-08 19:35:55.000000 distfit-1.7.3/distfit/distfit.py
--rw-rw-rw-   0        0        0    29312 2023-12-02 11:13:47.000000 distfit-1.7.3/distfit/examples.py
-drwxrwxrwx   0        0        0        0 2023-12-08 19:41:56.150240 distfit-1.7.3/distfit/tests/
--rw-rw-rw-   0        0        0        0 2023-09-30 18:07:42.000000 distfit-1.7.3/distfit/tests/__init__.py
--rw-rw-rw-   0        0        0    14023 2023-09-30 18:07:42.000000 distfit-1.7.3/distfit/tests/test_distfit.py
-drwxrwxrwx   0        0        0        0 2023-12-08 19:41:56.150240 distfit-1.7.3/distfit.egg-info/
--rw-rw-rw-   0        0        0    11755 2023-12-08 19:41:55.000000 distfit-1.7.3/distfit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-12-08 19:41:56.000000 distfit-1.7.3/distfit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-08 19:41:55.000000 distfit-1.7.3/distfit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2023-12-08 19:41:55.000000 distfit-1.7.3/distfit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-12-08 19:41:55.000000 distfit-1.7.3/distfit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-08 19:41:56.150240 distfit-1.7.3/setup.cfg
--rw-rw-rw-   0        0        0     1933 2023-10-19 20:38:32.000000 distfit-1.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 11:17:38.374820 distfit-1.8.0/
+-rw-rw-rw-   0        0        0     1181 2023-09-30 18:07:42.000000 distfit-1.8.0/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-09-30 18:07:42.000000 distfit-1.8.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    11992 2024-05-17 11:17:38.359202 distfit-1.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11214 2023-09-30 18:07:42.000000 distfit-1.8.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 11:17:38.331854 distfit-1.8.0/distfit/
+-rw-rw-rw-   0        0        0     2141 2024-05-04 09:25:32.000000 distfit-1.8.0/distfit/__init__.py
+-rw-rw-rw-   0        0        0   122875 2024-05-04 12:30:34.000000 distfit-1.8.0/distfit/distfit.py
+-rw-rw-rw-   0        0        0    31633 2024-05-04 12:32:59.000000 distfit-1.8.0/distfit/examples.py
+drwxrwxrwx   0        0        0        0 2024-05-17 11:17:38.359202 distfit-1.8.0/distfit/tests/
+-rw-rw-rw-   0        0        0        0 2023-09-30 18:07:42.000000 distfit-1.8.0/distfit/tests/__init__.py
+-rw-rw-rw-   0        0        0    14023 2023-09-30 18:07:42.000000 distfit-1.8.0/distfit/tests/test_distfit.py
+drwxrwxrwx   0        0        0        0 2024-05-17 11:17:38.359202 distfit-1.8.0/distfit.egg-info/
+-rw-rw-rw-   0        0        0    11992 2024-05-17 11:17:38.000000 distfit-1.8.0/distfit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2024-05-17 11:17:38.000000 distfit-1.8.0/distfit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 11:17:38.000000 distfit-1.8.0/distfit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2024-05-17 11:17:38.000000 distfit-1.8.0/distfit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-17 11:17:38.000000 distfit-1.8.0/distfit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 11:17:38.374820 distfit-1.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     1933 2023-10-19 20:38:32.000000 distfit-1.8.0/setup.py
```

### Comparing `distfit-1.7.3/LICENSE` & `distfit-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `distfit-1.7.3/PKG-INFO` & `distfit-1.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: distfit
-Version: 1.7.3
-Summary: distfit is a python library for probability density fitting.
-Home-page: https://erdogant.github.io/distfit
-Download-URL: https://github.com/erdogant/distfit/archive/1.7.3.tar.gz
-Author: Erdogan Taskesen
-Author-email: erdogant@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
   <a href="https://erdogant.github.io/pca/">
   <img src="https://github.com/erdogant/distfit/blob/master/docs/figs/logo.png" width="600" />
   </a>
 </p>
 
 [![Python](https://img.shields.io/pypi/pyversions/distfit)](https://img.shields.io/pypi/pyversions/distfit)
```

#### html2text {}

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1 Name: distfit Version: 1.7.3 Summary: distfit is a python
-library for probability density fitting. Home-page: https://erdogant.github.io/
-distfit Download-URL: https://github.com/erdogant/distfit/archive/1.7.3.tar.gz
-Author: Erdogan Taskesen Author-email: erdogant@gmail.com Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3
-Description-Content-Type: text/markdown License-File: LICENSE
      _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_e_r_d_o_g_a_n_t_/_d_i_s_t_f_i_t_/_b_l_o_b_/_m_a_s_t_e_r_/_d_o_c_s_/_f_i_g_s_/_l_o_g_o_._p_n_g_]
 [![Python](https://img.shields.io/pypi/pyversions/distfit)](https://
 img.shields.io/pypi/pyversions/distfit) [![Pypi](https://img.shields.io/pypi/v/
 distfit)](https://pypi.org/project/distfit/) [![Docs](https://img.shields.io/
 badge/Sphinx-Docs-Green)](https://erdogant.github.io/distfit/) [![LOC](https://
 sloc.xyz/github/erdogant/distfit/?category=code)](https://github.com/erdogant/
 distfit/) [![Downloads](https://static.pepy.tech/personalized-badge/
```

### Comparing `distfit-1.7.3/README.md` & `distfit-1.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: distfit
+Version: 1.8.0
+Summary: distfit is a python library for probability density fitting.
+Home-page: https://erdogant.github.io/distfit
+Download-URL: https://github.com/erdogant/distfit/archive/1.8.0.tar.gz
+Author: Erdogan Taskesen
+Author-email: erdogant@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: packaging
+Requires-Dist: matplotlib>=3.5.2
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: statsmodels
+Requires-Dist: scipy
+Requires-Dist: pypickle
+Requires-Dist: colourmap>=1.1.10
+Requires-Dist: joblib
+
 <p align="center">
   <a href="https://erdogant.github.io/pca/">
   <img src="https://github.com/erdogant/distfit/blob/master/docs/figs/logo.png" width="600" />
   </a>
 </p>
 
 [![Python](https://img.shields.io/pypi/pyversions/distfit)](https://img.shields.io/pypi/pyversions/distfit)
```

#### html2text {}

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1 Name: distfit Version: 1.8.0 Summary: distfit is a python
+library for probability density fitting. Home-page: https://erdogant.github.io/
+distfit Download-URL: https://github.com/erdogant/distfit/archive/1.8.0.tar.gz
+Author: Erdogan Taskesen Author-email: erdogant@gmail.com Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Requires-Python: >=3
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+packaging Requires-Dist: matplotlib>=3.5.2 Requires-Dist: numpy Requires-Dist:
+pandas Requires-Dist: statsmodels Requires-Dist: scipy Requires-Dist: pypickle
+Requires-Dist: colourmap>=1.1.10 Requires-Dist: joblib
      _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_e_r_d_o_g_a_n_t_/_d_i_s_t_f_i_t_/_b_l_o_b_/_m_a_s_t_e_r_/_d_o_c_s_/_f_i_g_s_/_l_o_g_o_._p_n_g_]
 [![Python](https://img.shields.io/pypi/pyversions/distfit)](https://
 img.shields.io/pypi/pyversions/distfit) [![Pypi](https://img.shields.io/pypi/v/
 distfit)](https://pypi.org/project/distfit/) [![Docs](https://img.shields.io/
 badge/Sphinx-Docs-Green)](https://erdogant.github.io/distfit/) [![LOC](https://
 sloc.xyz/github/erdogant/distfit/?category=code)](https://github.com/erdogant/
 distfit/) [![Downloads](https://static.pepy.tech/personalized-badge/
```

### Comparing `distfit-1.7.3/distfit/__init__.py` & `distfit-1.8.0/distfit/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distfit.distfit import distfit
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '1.7.3'
+__version__ = '1.8.0'
 
 
 # module level doc-string
 __doc__ = """
 distfit
 =====================================================================
 distfit is a python package for probability density fitting of univariate distributions for random variables.
```

### Comparing `distfit-1.7.3/distfit/distfit.py` & `distfit-1.8.0/distfit/distfit.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
                  weighted: bool = True,
                  f: float = 1.5,
                  mhist: str = 'numpy',
                  cmap: str = 'Set1',
                  random_state: int = None,
                  verbose: [str, int] = 'info',
                  multtest=None,
-                 n_jobs=1,
+                 n_jobs: int = 1,
                  ):
         """Initialize distfit with user-defined parameters.
 
         Parameters
         ----------
         method : str, default: 'parametric'
             Specify the method type.
@@ -149,16 +149,16 @@
         f : float, (default: 1.5)
             Only used in discrete fitting. It uses n in range n0/f to n0*f where n0 is the initial estimate.
         cmap : String, optional (default: 'Set1')
             Colormap when plotting multiple the CDF. The used colors are stored in dfit.summary['colors'].
         random_state : int, optional
             Random state.
         n_jobs : int, optional (default: 1)
-            Number of cpu cores that are used to compute the bootstrap.
-            Note that the use of multiple cores accacionally causes a RuntimeWarning: invalid value encountered in log. The results can then be unriable. It is better to set n_jobs=1.
+            Number of cpu cores that are used for the computations.
+            Note that the use of multiple cores occasionally causes a RuntimeWarning: invalid value encountered in log. The results can then be unriable. It is better to set n_jobs=1.
             -1: Use all cores
         verbose : [str, int], default is 'info' or 20
             Set the verbose messages using string or integer values.
                 * 0, 60, None, 'silent', 'off', 'no']: No message.
                 * 10, 'debug': Messages from debug level and higher.
                 * 20, 'info': Messages from info level and higher.
                 * 30, 'warning': Messages from warning level and higher.
@@ -212,14 +212,17 @@
         >>>
 
         References
         ----------
             * https://erdogant.github.io/distfit
 
         """
+        # Set the logger
+        set_logger(verbose=verbose)
+
         if (alpha is None): alpha=1
         self.method = method
         self.alpha = alpha
         self.bins = bins
         self.bound = bound
         self.distr = distr
         self.n_boots = n_boots
@@ -230,17 +233,25 @@
         self.stats = stats
         self.f = f  # Only for discrete
         self.weighted = weighted  # Only for discrete
         self.mhist = mhist
         self.cmap = cmap
         self.random_state = random_state
         self.verbose = verbose
-        self.n_jobs = n_jobs
-        # Set the logger
-        set_logger(verbose=verbose)
+
+        # Set n_jobs
+        if n_boots is not None:
+            # Allocate the cores to bootstrapping
+            self.n_jobs_dist = 1
+            self.n_jobs = n_jobs
+        else:
+            # Allocate the cores to general proces
+            self.n_jobs_dist = n_jobs
+            self.n_jobs = 1
+
         if multtest is not None: logger.warning('multtest will be removed from initialization in a future release. Please set this parameter when using the predict function. Example: dfit.predict(multtest="holm")')
         # Check versions
         check_version()
 
     # Fit
     def fit(self, verbose=None):
         """Collect the required distribution functions.
@@ -324,15 +335,15 @@
         X_bins, y_obs = self.density(X, self.bins, mhist=self.mhist)
         # Smoothing by interpolation
         X_bins, y_obs = smoothline(X_bins, y_obs, interpol=1, window=self.smooth)
         self.histdata = (y_obs, X_bins)
 
         if self.method=='parametric':
             # Compute best distribution fit on the empirical X
-            out_summary, model = _compute_score_distribution(X, X_bins, y_obs, self.distributions, self.stats, cmap=self.cmap, n_boots=self.n_boots, random_state=self.random_state, n_jobs=self.n_jobs)
+            out_summary, model = _compute_score_distribution(X, X_bins, y_obs, self.distributions, self.stats, cmap=self.cmap, n_boots=self.n_boots, random_state=self.random_state, n_jobs=self.n_jobs, n_jobs_dist=self.n_jobs_dist)
             # Determine confidence intervals on the best fitting distribution
             model = compute_cii(self, model, logger=logger)
             # Store
             self.model = model
             self.summary = out_summary
         elif self.method=='discrete':
             # Compute best distribution fit on the empirical X
@@ -2204,26 +2215,23 @@
     out['f'] = f
     out['n_boots'] = n_boots
     out['random_state'] = random_state
     # Return
     return out
 
 
-# %% Compute score for each distribution
-def _compute_score_distribution(data, X, y_obs, DISTRIBUTIONS, stats, cmap='Set1', n_boots=None, random_state=None, n_jobs=1):
+# %% Compute score for each distribution - in parallel when n_jobs_dist != 1
+def _compute_score_distribution(data, X, y_obs, DISTRIBUTIONS, stats, cmap='Set1', n_boots=None, random_state=None, n_jobs=1, n_jobs_dist=1):
     df = pd.DataFrame(index=range(0, len(DISTRIBUTIONS)), columns=['name', 'score', 'loc', 'scale', 'arg', 'params', 'model', 'bootstrap_score', 'bootstrap_pass'])
     max_name_len = np.max(list(map(lambda x: len(x.name) if isinstance(x.name, str) else len(x.name()), DISTRIBUTIONS)))
 
-    # Estimate distribution parameters
-    for i, distribution in enumerate(DISTRIBUTIONS):
-
-        # Fit the distribution. However this can result in an error. I need the try-except.
+    def fit_distribution(i, distribution):
         try:
             start_time = time.time()
-
+            # Fit the distribution. However, this can result in an error. I need the try-except.
             # Ignore warnings from data that can't be fit
             with warnings.catch_warnings():
                 # fit dist to data
                 params = distribution.fit(data)
                 logger.debug(params)
 
                 # Separate parts of parameters
@@ -2238,35 +2246,41 @@
                 # Get name of the distribution
                 distr_name = distribution.name if isinstance(distribution.name, str) else distribution.name()
                 # Fitted model
                 distribution_fit = distribution(*arg, loc, scale) if arg else distribution(loc, scale)  # Store the fitted model
                 # Bootstrapping
                 bootstrap_score, bootstrap_pass = _bootstrap(distribution, distribution_fit, data, n_boots=n_boots, random_state=random_state, n_jobs=n_jobs)
 
-                # Store results
-                df.values[i, 0] = distr_name
-                df.values[i, 1] = score
-                df.values[i, 2] = loc
-                df.values[i, 3] = scale
-                df.values[i, 4] = arg
-                df.values[i, 5] = params
-                df.values[i, 6] = distribution_fit
-                df.values[i, 7] = bootstrap_score
-                df.values[i, 8] = bootstrap_pass
+                # Setup for the logger - when not Parallel executed
+                spaces_1 = ' ' * (max_name_len - len(distr_name))
+                scores = ('[%s: %g] [loc=%.3f scale=%.3f]' % (stats, score, loc, scale))
+                time_spent = time.time() - start_time
+                logger.info("[%s%s] [%.4s sec] %s" % (distr_name, spaces_1, time_spent, scores))
+
+                return (i, distr_name, score, loc, scale, arg, params, distribution_fit, bootstrap_score, bootstrap_pass, start_time)
+
+        except Exception as e:
+            return None
+
+    # Parallelize the loop over distributions
+    results = Parallel(n_jobs=n_jobs_dist)(
+        delayed(fit_distribution)(i, distribution) for i, distribution in enumerate(DISTRIBUTIONS)
+    )
+
+    # Fill the DataFrame with the results
+    for result in results:
+        if result is not None:
+            i, distr_name, score, loc, scale, arg, params, distribution_fit, bootstrap_score, bootstrap_pass, start_time = result
+            df.values[i] = [distr_name, score, loc, scale, arg, params, distribution_fit, bootstrap_score, bootstrap_pass]
 
             # Setup for the logger
             spaces_1 = ' ' * (max_name_len - len(distr_name))
-            scores = ('[%s: %g] [loc=%.3f scale=%.3f]' %(stats, score, loc, scale))
+            scores = ('[%s: %g] [loc=%.3f scale=%.3f]' % (stats, score, loc, scale))
             time_spent = time.time() - start_time
-            logger.info("[%s%s] [%.4s sec] %s" %(distr_name, spaces_1, time_spent, scores))
-
-        except Exception:
-            pass
-            # e = sys.exc_info()[0]
-            # logger.error(e)
+            logger.info("[%s%s] [%.4s sec] %s" % (distr_name, spaces_1, time_spent, scores))
 
     # Sort the output
     df, model = _sort_dataframe(df, cmap=cmap)
     # Return
     return df, model
 
 
@@ -2277,14 +2291,15 @@
     df.reset_index(drop=True, inplace=True)
     df = set_colors(df, cmap=cmap)
     # Get best model
     model = df.iloc[0,:].to_dict()
 
     return df, model
 
+
 # %% Compute fit score
 def _compute_fit_score(stats, y_obs, pdf):
     if stats=='RSS':
         score = np.sum(np.power(y_obs - pdf, 2.0))
         # score = (((y_obs - pdf) / sigmas)**2).sum()
     elif stats=='wasserstein':
         score = st.wasserstein_distance(y_obs, pdf)
```

### Comparing `distfit-1.7.3/distfit/examples.py` & `distfit-1.8.0/distfit/examples.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,85 @@
+import numpy as np
+import matplotlib.pyplot as plt
+from distfit import distfit
+import time
+from tqdm import tqdm
+import colourmap
+
+X = np.random.normal(163, 10, 10000)
+
+def run_prog_bootstrap(n_jobs: int, n_boots: int):
+    dfit = distfit(distr='popular', n_boots=n_boots, n_jobs=n_jobs, verbose='warning')
+    results = dfit.fit_transform(X)
+    return results
+
+def compute_performance(n_boots_list):
+    # combinations = [(1, 1)] + [(i, 8 - i) for i in range(1, 8)]
+    combinations = np.arange(1, 14)
+    timings = {}
+
+    for comb in tqdm(combinations):
+        timings[(comb)] = []
+        for n_boots in tqdm(n_boots_list, ):
+            start_time = time.time()
+            _ = run_prog_bootstrap(comb, n_boots)
+            elapsed_time = time.time() - start_time
+            timings[(comb)].append((n_boots, elapsed_time))
+
+    return timings
+
+def plot_performance(timings):
+    fig, ax = plt.subplots(figsize=(10, 6))
+
+    colors = ['r', 'g', 'b', 'm', 'c', 'y', 'k']  # Define colors for different n_jobs values
+    colors = colourmap.fromlist(np.arange(1, 14), scheme='hex')[0]
+    markers = ['o', '^', 's', 'd', 'x', 'v', 'h']  # Define markers for different n_jobs values
+
+    for n_jobs, results in timings.items():
+        x, y = zip(*results)
+        label = f"n_jobs={n_jobs}"
+        # Ensure indexing within range of available colors and markers
+        idx = min(n_jobs - 1, len(colors) - 1)
+        ax.plot(x, y, label=label, color=colors[idx], marker='o', linestyle='-')
+
+    ax.set_xlabel('n_boots')
+    ax.set_ylabel('Time (s)')
+    ax.set_title('Performance Comparison')
+    ax.legend()
+    plt.grid(True)
+    plt.show()
+
+
+# Define the n_boots_list
+n_boots_list = [0, 10, 50, 100]
+# Compute performance
+timings = compute_performance(n_boots_list)
+# Plot performance
+plot_performance(timings)
+
+
+
+# %% Parrellel computing
+import time
+from distfit import distfit
+
+X = np.random.normal(163, 10, 10000)
+
+start_time = time.time()
+
+# dfit = distfit(distr='full', n_boots=50, n_jobs=-1, verbose='info')
+dfit = distfit(distr='popular', n_jobs=20, n_boots=50, verbose='info')
+dfit.fit_transform(X)
+
+elapsed_time = time.time() - start_time
+print(elapsed_time)
+# n_jobs=-1 > 79.834397315979
+# n_jobs=1 >  64 sec
+# n_jobs=2 >  58 sec
+
 # %% Issue 45
 # https://github.com/erdogant/distfit/issues/45
 
 import numpy as np
 from distfit import distfit
 
 data = np.array([ 56.518556,  54.803739,  57.424846,  54.254221,  63.235301,
@@ -31,25 +109,25 @@
               'burr',
               'johnsonsb',
               'loggamma',
               'norminvgauss']
 
 dfit = distfit(distr=marg_dists)
 dfit.fit_transform(data)
-dfit.plot()
+dfit.plot(bar_properties={'width':10})
 
 # %% Issue xx
 
 from distfit import distfit
 import numpy as np
-
-dfit = distfit(distr='full',stats='energy',todf=True, n_jobs=-1)
 X = np.random.normal(0, 2, 10000)
+
+dfit = distfit()
 dfit.fit_transform(X)
-dfit.plot(chart='pdf')
+dfit.plot(bar_properties={'width':0.1})
 
 
 
 # %% Import libraries
 import time
 import numpy as np
 from distfit import distfit
```

### Comparing `distfit-1.7.3/distfit/tests/test_distfit.py` & `distfit-1.8.0/distfit/tests/test_distfit.py`

 * *Files identical despite different names*

### Comparing `distfit-1.7.3/distfit.egg-info/PKG-INFO` & `distfit-1.8.0/distfit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 Metadata-Version: 2.1
 Name: distfit
-Version: 1.7.3
+Version: 1.8.0
 Summary: distfit is a python library for probability density fitting.
 Home-page: https://erdogant.github.io/distfit
-Download-URL: https://github.com/erdogant/distfit/archive/1.7.3.tar.gz
+Download-URL: https://github.com/erdogant/distfit/archive/1.8.0.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: packaging
+Requires-Dist: matplotlib>=3.5.2
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: statsmodels
+Requires-Dist: scipy
+Requires-Dist: pypickle
+Requires-Dist: colourmap>=1.1.10
+Requires-Dist: joblib
 
 <p align="center">
   <a href="https://erdogant.github.io/pca/">
   <img src="https://github.com/erdogant/distfit/blob/master/docs/figs/logo.png" width="600" />
   </a>
 </p>
```

#### html2text {}

```diff
@@ -1,14 +1,17 @@
-Metadata-Version: 2.1 Name: distfit Version: 1.7.3 Summary: distfit is a python
+Metadata-Version: 2.1 Name: distfit Version: 1.8.0 Summary: distfit is a python
 library for probability density fitting. Home-page: https://erdogant.github.io/
-distfit Download-URL: https://github.com/erdogant/distfit/archive/1.7.3.tar.gz
+distfit Download-URL: https://github.com/erdogant/distfit/archive/1.8.0.tar.gz
 Author: Erdogan Taskesen Author-email: erdogant@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3
-Description-Content-Type: text/markdown License-File: LICENSE
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+packaging Requires-Dist: matplotlib>=3.5.2 Requires-Dist: numpy Requires-Dist:
+pandas Requires-Dist: statsmodels Requires-Dist: scipy Requires-Dist: pypickle
+Requires-Dist: colourmap>=1.1.10 Requires-Dist: joblib
      _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_e_r_d_o_g_a_n_t_/_d_i_s_t_f_i_t_/_b_l_o_b_/_m_a_s_t_e_r_/_d_o_c_s_/_f_i_g_s_/_l_o_g_o_._p_n_g_]
 [![Python](https://img.shields.io/pypi/pyversions/distfit)](https://
 img.shields.io/pypi/pyversions/distfit) [![Pypi](https://img.shields.io/pypi/v/
 distfit)](https://pypi.org/project/distfit/) [![Docs](https://img.shields.io/
 badge/Sphinx-Docs-Green)](https://erdogant.github.io/distfit/) [![LOC](https://
 sloc.xyz/github/erdogant/distfit/?category=code)](https://github.com/erdogant/
 distfit/) [![Downloads](https://static.pepy.tech/personalized-badge/
```

### Comparing `distfit-1.7.3/setup.py` & `distfit-1.8.0/setup.py`

 * *Files identical despite different names*

