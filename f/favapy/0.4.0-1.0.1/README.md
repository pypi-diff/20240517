# Comparing `tmp/favapy-0.4.0.tar.gz` & `tmp/favapy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "favapy-0.4.0.tar", last modified: Fri Nov  3 01:29:53 2023, max compression
+gzip compressed data, was "favapy-1.0.1.tar", last modified: Fri May 17 04:38:13 2024, max compression
```

## Comparing `favapy-0.4.0.tar` & `favapy-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 01:29:53.735249 favapy-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-11-03 01:29:41.000000 favapy-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2023-11-03 01:29:53.735249 favapy-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2023-11-03 01:29:41.000000 favapy-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-11-03 01:29:41.000000 favapy-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-11-03 01:29:53.735249 favapy-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2023-11-03 01:29:41.000000 favapy-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 01:29:53.731249 favapy-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 01:29:53.735249 favapy-0.4.0/src/favapy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 01:29:41.000000 favapy-0.4.0/src/favapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14592 2023-11-03 01:29:41.000000 favapy-0.4.0/src/favapy/fava.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 01:29:53.735249 favapy-0.4.0/src/favapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2023-11-03 01:29:53.000000 favapy-0.4.0/src/favapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      318 2023-11-03 01:29:53.000000 favapy-0.4.0/src/favapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 01:29:53.000000 favapy-0.4.0/src/favapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-11-03 01:29:53.000000 favapy-0.4.0/src/favapy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-11-03 01:29:53.000000 favapy-0.4.0/src/favapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-03 01:29:53.000000 favapy-0.4.0/src/favapy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 01:29:53.735249 favapy-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-11-03 01:29:41.000000 favapy-0.4.0/tests/test_fava.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:38:13.060004 favapy-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-17 04:38:03.000000 favapy-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-17 04:38:13.060004 favapy-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-17 04:38:03.000000 favapy-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-17 04:38:03.000000 favapy-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-17 04:38:13.060004 favapy-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-17 04:38:03.000000 favapy-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:38:13.056004 favapy-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:38:13.060004 favapy-1.0.1/src/favapy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 04:38:03.000000 favapy-1.0.1/src/favapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17587 2024-05-17 04:38:03.000000 favapy-1.0.1/src/favapy/fava.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:38:13.060004 favapy-1.0.1/src/favapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-17 04:38:13.000000 favapy-1.0.1/src/favapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 04:38:13.000000 favapy-1.0.1/src/favapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 04:38:13.000000 favapy-1.0.1/src/favapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-17 04:38:13.000000 favapy-1.0.1/src/favapy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-17 04:38:13.000000 favapy-1.0.1/src/favapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 04:38:13.000000 favapy-1.0.1/src/favapy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 04:38:13.060004 favapy-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-17 04:38:03.000000 favapy-1.0.1/tests/test_fava.py
```

### Comparing `favapy-0.4.0/LICENSE` & `favapy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `favapy-0.4.0/PKG-INFO` & `favapy-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: favapy
-Version: 0.4.0
+Version: 1.0.1
 Summary: Infer Functional Associations using Variational Autoencoders on -Omics data.
 Home-page: https://github.com/mikelkou/VAE_Functional_associations
 Author: Mikaela Koutrouli
 Author-email: mikaela.koutrouli@cpr.ku.dk
 Project-URL: Bug Tracker, https://github.com/mikelkou/VAE_Functional_associations/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `favapy-0.4.0/README.md` & `favapy-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `favapy-0.4.0/setup.cfg` & `favapy-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = favapy
-version = 0.4.0
+version = 1.0.1
 author = Mikaela Koutrouli
 author_email = mikaela.koutrouli@cpr.ku.dk
 description = Infer Functional Associations using Variational Autoencoders on -Omics data.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mikelkou/VAE_Functional_associations
 project_urls =
```

### Comparing `favapy-0.4.0/setup.py` & `favapy-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="favapy",
-    version="0.4.0",
+    version="1.0.1",
     author="Mikaela Koutrouli",
     author_email="mikaela.koutrouli@cpr.ku.dk",
     description="Infer Functional Associations using Variational Autoencoders on -Omics data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mikelkou/VAE_Functional_associations",
     project_urls={
```

### Comparing `favapy-0.4.0/src/favapy/fava.py` & `favapy-1.0.1/src/favapy/fava.py`

 * *Files 10% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         help="Type of correlation to use (Pearson or Spearman).",
     )
 
     args = parser.parse_args()
     return args
 
 
-def load_data(input_file, data_type):
+def _load_data(input_file, data_type):
     """
     Loads and preprocesses data from a file.
 
     Parameters
     ----------
     input_file : str
         Path to the input file.
@@ -185,15 +185,16 @@
         def sampling(args):
             z_mean, z_log_sigma = args
             epsilon = K.random_normal(
                 shape=(K.shape(z_mean)[0], latent_dim), mean=0.0, stddev=0.1
             )
             return z_mean + K.exp(z_log_sigma) * epsilon
 
-        z = layers.Lambda(sampling)([z_mean, z_log_sigma])
+        # z = layers.Lambda(sampling)([z_mean, z_log_sigma])
+        z = layers.Lambda(sampling, output_shape=(latent_dim,))([z_mean, z_log_sigma])
 
         # Create encoder
         encoder = keras.Model(inputs, [z_mean, z_log_sigma, z], name="encoder")
         self.encoder = encoder
         # Create decoder
         latent_inputs = keras.Input(shape=(latent_dim,), name="z_sampling")
         x = layers.Dense(hidden_layer, activation="relu")(latent_inputs)  # relu
@@ -221,15 +222,94 @@
             x_train,
             batch_size=batch_size,
             epochs=epochs,
             validation_data=(x_test, x_test),
         )
 
 
-def create_protein_pairs(x_test_encoded, row_names, correlation_type="pearson"):
+######### Code for multiprocessing correlations --> slower #########
+import multiprocessing as mp
+import time
+
+
+def _calculate_correlation(sub_df, correlation_type):
+    if correlation_type == "spearman":
+        corr = sub_df.corr(method="spearman")
+    else:
+        corr_matrix = np.corrcoef(sub_df)
+        corr = pd.DataFrame(corr_matrix, index=sub_df.index, columns=sub_df.index)
+    return corr
+
+
+def _create_protein_pairs_parallel(
+    x_test_encoded, row_names, correlation_type="pearson", num_processes=4
+):
+    start_time = time.time()
+
+    df_x_test_encoded = pd.concat(
+        [pd.DataFrame(x_test_encoded[i, :, :]) for i in range(x_test_encoded.shape[0])],
+        axis=1,
+    )
+    df_x_test_encoded.index = row_names
+
+    # Split DataFrame into chunks for parallel processing
+    chunks = [df_x_test_encoded.iloc[i::num_processes] for i in range(num_processes)]
+    print(chunks)
+    # Create a pool of processes
+    pool = mp.Pool(processes=num_processes)
+
+    # Calculate correlations in parallel
+    results = [
+        pool.apply_async(_calculate_correlation, args=(chunk, correlation_type))
+        for chunk in chunks
+    ]
+
+    correlations = pd.DataFrame(columns=row_names, index=row_names)
+    for r in results:
+        corr_chunk = r.get()
+        for idx in corr_chunk.index:
+            correlations.loc[idx, corr_chunk.columns] = corr_chunk.loc[idx, :]
+
+    pool.close()
+    pool.join()
+
+    threshold = 0.85
+    threshold_decrement = 0.05
+    max_iterations = 5
+
+    for _ in range(max_iterations):
+        high_corr = correlations.where(
+            (np.abs(correlations) > threshold) & (np.abs(correlations) < 1)
+        )
+
+        if high_corr.stack().empty:
+            threshold -= threshold_decrement  # Decrease the threshold
+            print(
+                f"No correlations above threshold. Decreasing threshold to {threshold}"
+            )
+            if threshold <= 0:
+                print("Threshold reached 0. No further reduction possible.")
+                break
+        else:
+            correlation_df = high_corr.stack().reset_index()
+            print(f"Correlations found above threshold {threshold}.")
+            end_time = time.time()
+            break
+
+    total_time = end_time - start_time
+    print(f"Total time taken: {total_time} seconds")
+    correlation_df.columns = ["Protein_1", "Protein_2", "Score"]
+
+    return correlation_df
+
+
+###################################################################################################
+
+
+def _create_protein_pairs(x_test_encoded, row_names, correlation_type="pearson"):
     """
     Create pairs of proteins based on their encoded latent spaces.
 
     Parameters
     ----------
     x_test_encoded : np.ndarray
         Encoded latent spaces.
@@ -239,14 +319,15 @@
         Type of correlation to use (Pearson or Spearman).
 
     Returns
     -------
     correlation_df : pd.DataFrame
         DataFrame containing protein pairs and correlation scores.
     """
+    start_time = time.time()
     # Concatenate latent spaces
     df_x_test_encoded_0 = pd.DataFrame(x_test_encoded[0, :, :])
     df_x_test_encoded_1 = pd.DataFrame(x_test_encoded[1, :, :])
     df_x_test_encoded_2 = pd.DataFrame(x_test_encoded[2, :, :])
 
     df_x_test_encoded_01 = pd.merge(
         df_x_test_encoded_0, df_x_test_encoded_1, left_index=True, right_index=True
@@ -263,20 +344,22 @@
         corr.columns = corr.index = row_names
     else:
         corr = np.corrcoef(df_x_test_encoded)
         corr = pd.DataFrame(corr, columns=row_names, index=row_names)
 
     correlation_df = corr.stack().reset_index()
 
-    # set column names
+    end_time = time.time()
+    total_time = end_time - start_time
+    print(f"Total time taken OLD: {total_time} seconds")
     correlation_df.columns = ["Protein_1", "Protein_2", "Score"]
     return correlation_df
 
 
-def pairs_after_cutoff(correlation, interaction_count=100000, CC_cutoff=None):
+def _pairs_after_cutoff(correlation, interaction_count=100000, CC_cutoff=None):
     """
     Filter protein pairs based on correlation scores and cutoffs.
 
     Parameters
     ----------
     correlation : pd.DataFrame
         DataFrame containing protein pairs and correlation scores.
@@ -339,15 +422,20 @@
         Correlation Coefficient cutoff, by default None.
 
     Returns
     -------
     final_pairs : pd.DataFrame
         Filtered protein pairs based on correlation and cutoffs.
     """
+    from scipy.sparse import issparse
+
     if type(data) == anndata._core.anndata.AnnData:
+        # if issparse(data.X):
+        data.X = data.X.toarray()
+        data.var.index.name = None
         x = data.X.T
         row_names = data.var.index
     else:
         x = np.asarray(data, dtype=np.float32)
         row_names = data.index
 
     if np.any(x < 0):
@@ -382,18 +470,20 @@
 
     opt = tf.keras.optimizers.Adam(learning_rate=0.001, clipnorm=0.001)
     x_train = x_test = np.array(x)
     vae = VAE(
         opt, x_train, x_test, batch_size, original_dim, hidden_layer, latent_dim, epochs
     )
     x_test_encoded = np.array(vae.encoder.predict(x_test, batch_size=batch_size))
-    correlation = create_protein_pairs(x_test_encoded, row_names, correlation_type)
+    correlation = _create_protein_pairs(x_test_encoded, row_names, correlation_type)
+    # correlation = _create_protein_pairs_parallel(x_test_encoded, row_names, correlation_type, num_processes=6)
+
     final_pairs = correlation[correlation.iloc[:, 0] != correlation.iloc[:, 1]]
     final_pairs = final_pairs.sort_values(by=["Score"], ascending=False)
-    final_pairs = pairs_after_cutoff(
+    final_pairs = _pairs_after_cutoff(
         correlation=final_pairs,
         interaction_count=interaction_count,
         CC_cutoff=CC_cutoff,
     )
     return final_pairs
 
 
@@ -403,15 +493,15 @@
 
     This function loads data, applies preprocessing, trains a Variational Autoencoder (VAE),
     calculates correlation scores between encoded latent spaces, filters protein pairs based
     on correlation and cutoffs, and finally saves the results to a file.
     """
     args = argument_parser()
 
-    x, row_names = load_data(args.input_file, args.data_type)
+    x, row_names = _load_data(args.input_file, args.data_type)
     original_dim = x.shape[1]
 
     if args.hidden_layer == None:
         if original_dim >= 2000:
             args.hidden_layer = 1000
         if original_dim > 500 and original_dim < 2000:
             args.hidden_layer = 500
@@ -437,19 +527,21 @@
         args.hidden_layer,
         args.latent_dim,
         args.epochs,
     )
     x_test_encoded = np.array(vae.encoder.predict(x_test, batch_size=args.batch_size))
 
     logging.info(f" Calculating {args.correlation_type} correlation scores.")
-    correlation = create_protein_pairs(x_test_encoded, row_names, args.correlation_type)
+    correlation = _create_protein_pairs(
+        x_test_encoded, row_names, args.correlation_type
+    )
 
     final_pairs = correlation[correlation.iloc[:, 0] != correlation.iloc[:, 1]]
     final_pairs = final_pairs.sort_values(by=["Score"], ascending=False)
-    final_pairs = pairs_after_cutoff(
+    final_pairs = _pairs_after_cutoff(
         correlation=final_pairs,
         interaction_count=args.interaction_count,
         CC_cutoff=args.CC_cutoff,
     )
     final_pairs.Score = final_pairs.Score.astype(float).round(5)
     logging.warn(
         " If it is not the desired cut-off, please check again the value assigned to the related parameter (-n or interaction_count | -c or CC_cutoff)."
```

### Comparing `favapy-0.4.0/src/favapy.egg-info/PKG-INFO` & `favapy-1.0.1/src/favapy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: favapy
-Version: 0.4.0
+Version: 1.0.1
 Summary: Infer Functional Associations using Variational Autoencoders on -Omics data.
 Home-page: https://github.com/mikelkou/VAE_Functional_associations
 Author: Mikaela Koutrouli
 Author-email: mikaela.koutrouli@cpr.ku.dk
 Project-URL: Bug Tracker, https://github.com/mikelkou/VAE_Functional_associations/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `favapy-0.4.0/tests/test_fava.py` & `favapy-1.0.1/tests/test_fava.py`

 * *Files identical despite different names*

