# Comparing `tmp/slimp-0.2.0.tar.gz` & `tmp/slimp-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slimp-0.2.0.tar", last modified: Wed Feb 21 06:02:47 2024, max compression
+gzip compressed data, was "slimp-0.4.0.tar", last modified: Sat Mar 30 13:15:20 2024, max compression
```

## Comparing `slimp-0.2.0.tar` & `slimp-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,41 @@
-drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2024-02-21 06:02:47.772233 slimp-0.2.0/
--rw-r-----   0 lamy      (1265) lamy      (1265)     1087 2024-02-19 19:09:57.000000 slimp-0.2.0/LICENSE
--rw-r--r--   0 lamy      (1265) lamy      (1265)      307 2024-02-21 06:02:47.772233 slimp-0.2.0/PKG-INFO
--rw-r--r--   0 lamy      (1265) lamy      (1265)      673 2024-02-19 19:08:58.000000 slimp-0.2.0/README.md
--rw-r--r--   0 lamy      (1265) lamy      (1265)       38 2024-02-21 06:02:47.772233 slimp-0.2.0/setup.cfg
--rw-r--r--   0 lamy      (1265) lamy      (1265)     1954 2024-02-21 06:02:30.000000 slimp-0.2.0/setup.py
-drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2024-02-21 06:02:47.768233 slimp-0.2.0/slimp/
--rw-r--r--   0 lamy      (1265) lamy      (1265)      181 2024-02-19 18:57:10.000000 slimp-0.2.0/slimp/__init__.py
--rw-r--r--   0 lamy      (1265) lamy      (1265)      653 2024-02-21 05:59:07.000000 slimp-0.2.0/slimp/compile.py
--rw-r--r--   0 lamy      (1265) lamy      (1265)     5469 2024-02-19 22:13:56.000000 slimp-0.2.0/slimp/model.py
--rw-r--r--   0 lamy      (1265) lamy      (1265)     5583 2024-02-21 05:57:20.000000 slimp-0.2.0/slimp/multivariate.stan
--rw-r--r--   0 lamy      (1265) lamy      (1265)     1311 2024-02-20 06:45:02.000000 slimp-0.2.0/slimp/plots.py
--rw-r--r--   0 lamy      (1265) lamy      (1265)      954 2024-02-19 18:57:10.000000 slimp-0.2.0/slimp/predictor_mapper.py
--rw-r--r--   0 lamy      (1265) lamy      (1265)      257 2024-02-19 18:57:10.000000 slimp-0.2.0/slimp/stats.py
--rw-r--r--   0 lamy      (1265) lamy      (1265)     3161 2024-02-20 09:18:56.000000 slimp-0.2.0/slimp/univariate.stan
-drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2024-02-21 06:02:47.772233 slimp-0.2.0/slimp.egg-info/
--rw-r--r--   0 lamy      (1265) lamy      (1265)      307 2024-02-21 06:02:47.000000 slimp-0.2.0/slimp.egg-info/PKG-INFO
--rw-r--r--   0 lamy      (1265) lamy      (1265)      322 2024-02-21 06:02:47.000000 slimp-0.2.0/slimp.egg-info/SOURCES.txt
--rw-r--r--   0 lamy      (1265) lamy      (1265)        1 2024-02-21 06:02:47.000000 slimp-0.2.0/slimp.egg-info/dependency_links.txt
--rw-r--r--   0 lamy      (1265) lamy      (1265)       52 2024-02-21 06:02:47.000000 slimp-0.2.0/slimp.egg-info/requires.txt
--rw-r--r--   0 lamy      (1265) lamy      (1265)        6 2024-02-21 06:02:47.000000 slimp-0.2.0/slimp.egg-info/top_level.txt
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2024-03-30 13:15:20.604526 slimp-0.4.0/
+-rw-r-----   0 lamy      (1265) lamy      (1265)     1087 2024-02-19 19:09:57.000000 slimp-0.4.0/LICENSE
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     2092 2024-03-30 13:15:20.604526 slimp-0.4.0/PKG-INFO
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     1414 2024-03-30 13:06:18.000000 slimp-0.4.0/README.md
+-rw-r--r--   0 lamy      (1265) lamy      (1265)       38 2024-03-30 13:15:20.604526 slimp-0.4.0/setup.cfg
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     2788 2024-03-30 13:14:41.000000 slimp-0.4.0/setup.py
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2024-03-30 13:15:20.604526 slimp-0.4.0/slimp/
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     2492 2024-03-29 08:05:32.000000 slimp-0.4.0/slimp/ArrayWriter.cpp
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     1870 2024-03-29 08:05:32.000000 slimp-0.4.0/slimp/ArrayWriter.h
+-rw-r--r--   0 lamy      (1265) lamy      (1265)      900 2024-03-30 07:35:43.000000 slimp-0.4.0/slimp/Factory.cpp
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     1051 2024-03-29 08:05:32.000000 slimp-0.4.0/slimp/Factory.h
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     4464 2024-03-29 20:51:59.000000 slimp-0.4.0/slimp/VarContext.cpp
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     1853 2024-03-29 08:05:32.000000 slimp-0.4.0/slimp/VarContext.h
+-rw-r--r--   0 lamy      (1265) lamy      (1265)      199 2024-03-30 10:37:25.000000 slimp-0.4.0/slimp/__init__.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     7337 2024-03-30 08:39:54.000000 slimp-0.4.0/slimp/_slimp.cpp
+-rw-r--r--   0 lamy      (1265) lamy      (1265)      940 2024-03-29 08:05:32.000000 slimp-0.4.0/slimp/action_parameters.h
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     8252 2024-03-29 08:05:32.000000 slimp-0.4.0/slimp/actions.cpp
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     2449 2024-03-29 08:05:32.000000 slimp-0.4.0/slimp/actions.h
+-rw-r--r--   0 lamy      (1265) lamy      (1265)      487 2024-03-17 07:06:34.000000 slimp-0.4.0/slimp/functions.stan
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     7330 2024-03-30 07:04:21.000000 slimp-0.4.0/slimp/model.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     1453 2024-03-29 08:05:32.000000 slimp-0.4.0/slimp/model_data.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     1985 2024-03-17 07:09:14.000000 slimp-0.4.0/slimp/multivariate_log_likelihood.stan
+-rw-r--r--   0 lamy      (1265) lamy      (1265)      369 2024-03-16 19:45:58.000000 slimp-0.4.0/slimp/multivariate_parameters.stan
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     2824 2024-03-30 08:41:21.000000 slimp-0.4.0/slimp/multivariate_predict_posterior.stan
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     3099 2024-03-30 08:30:31.000000 slimp-0.4.0/slimp/multivariate_predict_prior.stan
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     3117 2024-03-30 08:22:44.000000 slimp-0.4.0/slimp/multivariate_sampler.stan
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     2412 2024-03-30 12:53:41.000000 slimp-0.4.0/slimp/plots.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     1477 2024-03-29 08:05:32.000000 slimp-0.4.0/slimp/predictor_mapper.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)      400 2024-03-29 08:05:32.000000 slimp-0.4.0/slimp/samples.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)      702 2024-03-30 09:02:02.000000 slimp-0.4.0/slimp/stats.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)      606 2024-03-16 19:33:30.000000 slimp-0.4.0/slimp/univariate_log_likelihood.stan
+-rw-r--r--   0 lamy      (1265) lamy      (1265)      317 2024-03-16 09:16:57.000000 slimp-0.4.0/slimp/univariate_parameters.stan
+-rw-r--r--   0 lamy      (1265) lamy      (1265)      791 2024-03-16 19:33:42.000000 slimp-0.4.0/slimp/univariate_predict_posterior.stan
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     1240 2024-03-30 08:23:44.000000 slimp-0.4.0/slimp/univariate_predict_prior.stan
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     1432 2024-03-16 19:33:53.000000 slimp-0.4.0/slimp/univariate_sampler.stan
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2024-03-30 13:15:20.604526 slimp-0.4.0/slimp.egg-info/
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     2092 2024-03-30 13:15:20.000000 slimp-0.4.0/slimp.egg-info/PKG-INFO
+-rw-r--r--   0 lamy      (1265) lamy      (1265)      872 2024-03-30 13:15:20.000000 slimp-0.4.0/slimp.egg-info/SOURCES.txt
+-rw-r--r--   0 lamy      (1265) lamy      (1265)        1 2024-03-30 13:15:20.000000 slimp-0.4.0/slimp.egg-info/dependency_links.txt
+-rw-r--r--   0 lamy      (1265) lamy      (1265)       42 2024-03-30 13:15:20.000000 slimp-0.4.0/slimp.egg-info/requires.txt
+-rw-r--r--   0 lamy      (1265) lamy      (1265)        6 2024-03-30 13:15:20.000000 slimp-0.4.0/slimp.egg-info/top_level.txt
```

### Comparing `slimp-0.2.0/LICENSE` & `slimp-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slimp-0.2.0/setup.py` & `slimp-0.4.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,95 @@
 import glob
 import os
-import shlex
+import subprocess
 import sys
+import tempfile
 
 import setuptools
 import setuptools.command.build
 
-sys.path.insert(0, "slimp")
-import compile as slimp_compile
+here = os.path.abspath(os.path.dirname(__file__))
 
-class BuildStanModels(setuptools.Command, setuptools.command.build.SubCommand):
+class BuildCMake(setuptools.Command, setuptools.command.build.SubCommand):
     def __init__(self, *args, **kwargs):
         setuptools.Command.__init__(self, *args, **kwargs)
         setuptools.command.build.SubCommand.__init__(self, *args, **kwargs)
         self.build_lib = None
         self.editable_mode = False
         
         self.sources = []
         self.stanc_options = ""
         self.cxxflags = ""
     
     def initialize_options(self):
         pass
         
     def finalize_options(self):
-        self.sources = list(glob.glob("slimp/*.stan"))
-        self.stanc_options = shlex.split(
-            os.environ.get("SLIMP_STANC_OPTIONS", ""))
-        for option in ["STAN_CPP_OPTIMS", "STAN_THREADS", "STAN_NO_RANGE_CHECKS"]:
-            if not any(x.startswith(f"{option}=") for x in self.stanc_options):
-                self.stanc_options.append(f"{option}=TRUE")
-        self.cxxflags = os.environ.get("SLIMP_CXXFLAGS", "")
+        self.sources = [
+            *sorted(glob.glob(f"slimp/*.stan")),
+            *sorted(glob.glob(f"slimp/*.h")),
+            *sorted(glob.glob(f"slimp/*.cpp"))]
         self.set_undefined_options("build_py", ("build_lib", "build_lib"))
     
     def run(self):
-        for source in self.sources:
-            slimp_compile.compile(
-                source, os.path.join(self.build_lib, "slimp"),
-                self.stanc_options, self.cxxflags)
+        with tempfile.TemporaryDirectory() as build_dir:
+            subprocess.check_call(
+                [
+                    "cmake", f"-DPython_EXECUTABLE={sys.executable}",
+                    "-DCMAKE_BUILD_TYPE=Release",
+                    "-DCMAKE_LIBRARY_OUTPUT_DIRECTORY="
+                        f"{os.path.join(here, self.build_lib, 'slimp')}", 
+                    "-S", here, "-B", build_dir])
+            
+            subprocess.check_call(
+                [
+                    "cmake", "--build", build_dir, "--target", "_slimp",
+                    "--config", "Release", "--parallel"])
     
     def get_source_files(self):
         return self.sources
 
-setuptools.command.build.build.sub_commands.append(("build_stan_models", None))
+setuptools.command.build.build.sub_commands.append(("build_cmake", None))
 
+long_description = open(os.path.join(here, "README.md")).read()
 setuptools.setup(
     name="slimp",
-    version="0.2.0",
+    version="0.4.0",
     
     description="Linear models with Stan and Pandas",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    
+    url="https://github.com/lamyj/slimp",
     
     author="Julien Lamy",
     author_email="lamy@unistra.fr",
     
-    cmdclass={"build_stan_models": BuildStanModels},
+    license="MIT",
+    
+    classifiers=[
+        "Development Status :: 4 - Beta",
+        "Environment :: Console",
+        "Framework :: Matplotlib",
+        "Intended Audience :: Education",
+        "Intended Audience :: Science/Research",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+        "Topic :: Scientific/Engineering",
+    ],
+    
+    keywords = [
+        "statistics", "bayesian", "linear-models", "stan", "pandas",
+        "matplotlib"],
+    
+    cmdclass={"build_cmake": BuildCMake},
 
     packages=["slimp"],
     
     install_requires=[
-        "cmdstanpy",
         "formulaic",
         "numpy",
         "matplotlib",
         "pandas",
         "seaborn"
     ],
 )
```

### Comparing `slimp-0.2.0/slimp/univariate.stan` & `slimp-0.4.0/slimp/univariate_sampler.stan`

 * *Files 24% similar despite different names*

```diff
@@ -6,20 +6,18 @@
 intercept after centering the predictors around 0; let Xbar_i be the mean of the
 i-th predictors value, we then have:
 
 µ = α_c + Σ (X_i - Xbar_i) β_i
 α_c = α_0 + Σ Xbar_i β_i ~ Student(3, μ_α, σ_α)
 βᵢ ~ Student(3, 0, σ_βᵢ)
 σ ~ Exp(λ_σ)
+*/
 
-Note than when predicting data, the new predictors must be offset by the mean of
-the *original* predictors.
+#include functions.stan
 
-*/
-    
 data
 {
     // Number of outcomes and predictors
     int<lower=1> N, K;
     
     // Outcomes
     vector[N] y;
@@ -30,94 +28,32 @@
     real mu_alpha, sigma_alpha;
     
     // Scale of the non-intercept priors (location is 0)
     vector<lower=0>[K-1] sigma_beta;
     
     // Scale of the variance prior
     real<lower=0> lambda_sigma;
-    
-    // Number of new outcomes to predict
-    int<lower=0> N_new;
-    // New predictors
-    matrix[N_new, K] X_new;
-    // Whether to generate data from prior or posterior distribution
-    int use_prior;
 }
 
 transformed data
 {
     // Center the predictors
-    vector[K-1] X_bar;
-    matrix[N, K-1] X_c;
-    for(k in 2:K)
-    {
-        X_bar[k-1] = mean(X[, k]);
-        X_c[, k-1] = X[, k] - X_bar[k-1];
-    }
-    
-    // Center the new predictors, if given, around the *original* predictors
-    matrix[N_new, K-1] X_c_new;
-    if(N_new > 0)
-    {
-        for(k in 2:K)
-        {
-            X_c_new[, k-1] = X_new[, k] - X_bar[k-1];
-        }
-    }
-}
- 
-parameters
-{
-    // Centered intercept
-    real alpha_c;
-    
-    // Non-intercept parameters
-    vector[K-1] beta;
-    
-    // Variance. NOTE: it cannot be 0 or infinity, this causes warnings in the
-    // likelihood. Values are taken from std::numeric_limits<float>.
-    real<lower=1.2e-38, upper=3.4e+38> sigma;
+    vector[K-1] X_bar = center_columns(X, N, K);
+    matrix[N, K-1] X_c = center(X, X_bar, N, K);
 }
 
+#include univariate_parameters.stan
+
 model
 {
     alpha_c ~ student_t(3, mu_alpha, sigma_alpha);
     beta ~ student_t(3, 0, sigma_beta);
     sigma ~ exponential(lambda_sigma);
     
     y ~ normal_id_glm(X_c, alpha_c, beta, sigma);
 }
 
 generated quantities
 {
     // Non-centered intercept
     real alpha = alpha_c - dot_product(X_bar, beta);
-    
-    // Expected Value of the prior-or-posterior predictive distribution
-    vector[N_new] mu_rep;
-    // Draw from the prior-or-posterior predictive distribution
-    vector[N_new] y_rep;
-    if(N_new > 0)
-    {
-        real alpha_c_;
-        vector[K-1] beta_;
-        real sigma_;
-        
-        if(use_prior == 1)
-        {
-            // WARNING: the RNG must match the prior
-            alpha_c_ = student_t_rng(3, mu_alpha, sigma_alpha);
-            beta_ = to_vector(student_t_rng(3, 0, sigma_beta));
-            sigma_ = exponential_rng(lambda_sigma);
-        }
-        else
-        {
-            alpha_c_ = alpha_c;
-            beta_ = beta;
-            sigma_ = sigma;
-        }
-        
-        // WARNING: must match the likelihood
-        mu_rep = alpha_c_ + X_c_new*beta_;
-        y_rep = to_vector(normal_rng(mu_rep, sigma_));
-    }
 }
```

