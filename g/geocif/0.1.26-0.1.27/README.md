# Comparing `tmp/geocif-0.1.26.tar.gz` & `tmp/geocif-0.1.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geocif-0.1.26.tar", last modified: Sun May 12 15:40:29 2024, max compression
+gzip compressed data, was "geocif-0.1.27.tar", last modified: Fri May 17 00:28:41 2024, max compression
```

## Comparing `geocif-0.1.26.tar` & `geocif-0.1.27.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 15:40:29.492037 geocif-0.1.26/
--rw-rw-rw-   0        0        0     1096 2023-07-27 15:12:03.000000 geocif-0.1.26/LICENSE
--rw-rw-rw-   0        0        0      129 2023-07-27 15:12:03.000000 geocif-0.1.26/MANIFEST.in
--rw-rw-rw-   0        0        0     1586 2024-05-12 15:40:29.492037 geocif-0.1.26/PKG-INFO
--rw-rw-rw-   0        0        0      897 2024-05-12 14:58:37.000000 geocif-0.1.26/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 15:40:29.364951 geocif-0.1.26/geocif/
--rw-rw-rw-   0        0        0      155 2024-05-10 16:27:36.000000 geocif-0.1.26/geocif/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:40:29.428619 geocif-0.1.26/geocif/agmet/
--rw-rw-rw-   0        0        0        0 2024-05-09 16:19:42.000000 geocif-0.1.26/geocif/agmet/__init__.py
--rw-rw-rw-   0        0        0     6201 2024-05-09 16:20:58.000000 geocif-0.1.26/geocif/agmet/geoagmet.py
--rw-rw-rw-   0        0        0    27060 2024-05-09 16:20:58.000000 geocif-0.1.26/geocif/agmet/plot.py
--rw-rw-rw-   0        0        0     6907 2023-07-27 16:56:06.000000 geocif-0.1.26/geocif/agmet/utils.py
--rw-rw-rw-   0        0        0    34217 2024-05-11 02:14:29.000000 geocif-0.1.26/geocif/analysis.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:40:29.434889 geocif-0.1.26/geocif/backup/
--rw-rw-rw-   0        0        0        0 2024-05-09 16:19:12.000000 geocif-0.1.26/geocif/backup/__init__.py
--rw-rw-rw-   0        0        0       11 2023-07-27 15:12:03.000000 geocif-0.1.26/geocif/backup/constants.py
--rw-rw-rw-   0        0        0    10198 2024-05-10 00:43:58.000000 geocif-0.1.26/geocif/backup/features.py
--rw-rw-rw-   0        0        0     9919 2023-10-24 19:21:13.000000 geocif-0.1.26/geocif/backup/geo.py
--rw-rw-rw-   0        0        0    17693 2024-05-09 16:20:58.000000 geocif-0.1.26/geocif/backup/geocif.py
--rw-rw-rw-   0        0        0     1284 2023-10-24 19:33:45.000000 geocif-0.1.26/geocif/backup/metadata.py
--rw-rw-rw-   0        0        0       65 2023-07-27 16:50:11.000000 geocif-0.1.26/geocif/backup/models.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:40:29.444893 geocif-0.1.26/geocif/cei/
--rw-rw-rw-   0        0        0       83 2024-05-09 17:30:03.000000 geocif-0.1.26/geocif/cei/__init__.py
--rw-rw-rw-   0        0        0     5125 2024-05-09 18:11:43.000000 geocif-0.1.26/geocif/cei/definitions.py
--rw-rw-rw-   0        0        0    27358 2024-05-09 19:45:29.000000 geocif-0.1.26/geocif/cei/indices.py
--rw-rw-rw-   0        0        0    42331 2024-05-11 03:29:36.000000 geocif-0.1.26/geocif/geocif.py
--rw-rw-rw-   0        0        0     6633 2024-05-12 15:40:15.000000 geocif-0.1.26/geocif/indices_runner.py
--rw-rw-rw-   0        0        0     2274 2024-05-10 01:57:37.000000 geocif-0.1.26/geocif/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:40:29.476110 geocif-0.1.26/geocif/ml/
--rw-rw-rw-   0        0        0       83 2024-05-10 16:27:36.000000 geocif-0.1.26/geocif/ml/__init__.py
--rw-rw-rw-   0        0        0    12171 2024-05-11 02:34:09.000000 geocif-0.1.26/geocif/ml/correlations.py
--rw-rw-rw-   0        0        0     5054 2024-05-09 20:41:26.000000 geocif-0.1.26/geocif/ml/embedding.py
--rw-rw-rw-   0        0        0    12671 2024-05-12 03:53:54.000000 geocif-0.1.26/geocif/ml/feature_engineering.py
--rw-rw-rw-   0        0        0     7015 2024-05-12 03:04:01.000000 geocif-0.1.26/geocif/ml/feature_selection.py
--rw-rw-rw-   0        0        0     9769 2024-05-09 15:38:36.000000 geocif-0.1.26/geocif/ml/outliers.py
--rw-rw-rw-   0        0        0      526 2024-03-31 02:56:14.000000 geocif-0.1.26/geocif/ml/outlook.py
--rw-rw-rw-   0        0        0     3671 2024-05-10 17:25:05.000000 geocif-0.1.26/geocif/ml/output.py
--rw-rw-rw-   0        0        0     8286 2024-05-12 14:57:40.000000 geocif-0.1.26/geocif/ml/stages.py
--rw-rw-rw-   0        0        0     8119 2024-05-12 03:17:46.000000 geocif-0.1.26/geocif/ml/stats.py
--rw-rw-rw-   0        0        0     9718 2024-05-10 14:56:22.000000 geocif-0.1.26/geocif/ml/trainers.py
--rw-rw-rw-   0        0        0     3149 2024-05-09 19:24:05.000000 geocif-0.1.26/geocif/ml/trend.py
--rw-rw-rw-   0        0        0     2831 2024-05-09 19:24:05.000000 geocif-0.1.26/geocif/ml/xai.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:40:29.484703 geocif-0.1.26/geocif/playground/
--rw-rw-rw-   0        0        0        0 2024-05-10 19:03:20.000000 geocif-0.1.26/geocif/playground/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-10 18:55:55.000000 geocif-0.1.26/geocif/playground/automl.py
--rw-rw-rw-   0        0        0    13665 2024-05-11 01:04:25.000000 geocif-0.1.26/geocif/playground/misc.py
--rw-rw-rw-   0        0        0    18744 2024-05-12 14:57:40.000000 geocif-0.1.26/geocif/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:40:29.484703 geocif-0.1.26/geocif/viz/
--rw-rw-rw-   0        0        0       83 2024-05-10 16:27:36.000000 geocif-0.1.26/geocif/viz/__init__.py
--rw-rw-rw-   0        0        0    15867 2024-05-10 17:06:33.000000 geocif-0.1.26/geocif/viz/plot.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:40:29.414653 geocif-0.1.26/geocif.egg-info/
--rw-rw-rw-   0        0        0     1586 2024-05-12 15:40:28.000000 geocif-0.1.26/geocif.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1107 2024-05-12 15:40:29.000000 geocif-0.1.26/geocif.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 15:40:28.000000 geocif-0.1.26/geocif.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-10-22 16:27:17.000000 geocif-0.1.26/geocif.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2024-05-12 15:40:28.000000 geocif-0.1.26/geocif.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-05-10 01:05:13.000000 geocif-0.1.26/requirements.txt
--rw-rw-rw-   0        0        0      415 2024-05-12 15:40:29.499603 geocif-0.1.26/setup.cfg
--rw-rw-rw-   0        0        0     1617 2024-05-12 15:40:15.000000 geocif-0.1.26/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:40:29.484703 geocif-0.1.26/tests/
--rw-rw-rw-   0        0        0      355 2024-05-09 16:20:58.000000 geocif-0.1.26/tests/test_geocif.py
+drwxrwxrwx   0        0        0        0 2024-05-17 00:28:41.907815 geocif-0.1.27/
+-rw-rw-rw-   0        0        0     1096 2023-07-27 15:12:03.000000 geocif-0.1.27/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-07-27 15:12:03.000000 geocif-0.1.27/MANIFEST.in
+-rw-rw-rw-   0        0        0     1586 2024-05-17 00:28:41.903523 geocif-0.1.27/PKG-INFO
+-rw-rw-rw-   0        0        0      897 2024-05-12 14:58:37.000000 geocif-0.1.27/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 00:28:41.288003 geocif-0.1.27/geocif/
+-rw-rw-rw-   0        0        0      155 2024-05-10 16:27:36.000000 geocif-0.1.27/geocif/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 00:28:41.410964 geocif-0.1.27/geocif/agmet/
+-rw-rw-rw-   0        0        0        0 2024-05-09 16:19:42.000000 geocif-0.1.27/geocif/agmet/__init__.py
+-rw-rw-rw-   0        0        0     6201 2024-05-09 16:20:58.000000 geocif-0.1.27/geocif/agmet/geoagmet.py
+-rw-rw-rw-   0        0        0    27060 2024-05-09 16:20:58.000000 geocif-0.1.27/geocif/agmet/plot.py
+-rw-rw-rw-   0        0        0     6907 2023-07-27 16:56:06.000000 geocif-0.1.27/geocif/agmet/utils.py
+-rw-rw-rw-   0        0        0    34486 2024-05-16 01:28:20.000000 geocif-0.1.27/geocif/analysis.py
+drwxrwxrwx   0        0        0        0 2024-05-17 00:28:41.539350 geocif-0.1.27/geocif/backup/
+-rw-rw-rw-   0        0        0        0 2024-05-09 16:19:12.000000 geocif-0.1.27/geocif/backup/__init__.py
+-rw-rw-rw-   0        0        0       11 2023-07-27 15:12:03.000000 geocif-0.1.27/geocif/backup/constants.py
+-rw-rw-rw-   0        0        0    10198 2024-05-10 00:43:58.000000 geocif-0.1.27/geocif/backup/features.py
+-rw-rw-rw-   0        0        0     9919 2023-10-24 19:21:13.000000 geocif-0.1.27/geocif/backup/geo.py
+-rw-rw-rw-   0        0        0    17693 2024-05-09 16:20:58.000000 geocif-0.1.27/geocif/backup/geocif.py
+-rw-rw-rw-   0        0        0     1284 2023-10-24 19:33:45.000000 geocif-0.1.27/geocif/backup/metadata.py
+-rw-rw-rw-   0        0        0       65 2023-07-27 16:50:11.000000 geocif-0.1.27/geocif/backup/models.py
+drwxrwxrwx   0        0        0        0 2024-05-17 00:28:41.602148 geocif-0.1.27/geocif/cei/
+-rw-rw-rw-   0        0        0       83 2024-05-09 17:30:03.000000 geocif-0.1.27/geocif/cei/__init__.py
+-rw-rw-rw-   0        0        0     5125 2024-05-09 18:11:43.000000 geocif-0.1.27/geocif/cei/definitions.py
+-rw-rw-rw-   0        0        0    27358 2024-05-09 19:45:29.000000 geocif-0.1.27/geocif/cei/indices.py
+-rw-rw-rw-   0        0        0    42209 2024-05-16 14:18:55.000000 geocif-0.1.27/geocif/geocif.py
+-rw-rw-rw-   0        0        0     6633 2024-05-12 15:40:15.000000 geocif-0.1.27/geocif/indices_runner.py
+-rw-rw-rw-   0        0        0     2274 2024-05-10 01:57:37.000000 geocif-0.1.27/geocif/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-17 00:28:41.827261 geocif-0.1.27/geocif/ml/
+-rw-rw-rw-   0        0        0       83 2024-05-10 16:27:36.000000 geocif-0.1.27/geocif/ml/__init__.py
+-rw-rw-rw-   0        0        0    12360 2024-05-14 02:40:35.000000 geocif-0.1.27/geocif/ml/correlations.py
+-rw-rw-rw-   0        0        0     5054 2024-05-09 20:41:26.000000 geocif-0.1.27/geocif/ml/embedding.py
+-rw-rw-rw-   0        0        0    12671 2024-05-12 03:53:54.000000 geocif-0.1.27/geocif/ml/feature_engineering.py
+-rw-rw-rw-   0        0        0     8953 2024-05-15 14:01:01.000000 geocif-0.1.27/geocif/ml/feature_selection.py
+-rw-rw-rw-   0        0        0     9769 2024-05-09 15:38:36.000000 geocif-0.1.27/geocif/ml/outliers.py
+-rw-rw-rw-   0        0        0      526 2024-03-31 02:56:14.000000 geocif-0.1.27/geocif/ml/outlook.py
+-rw-rw-rw-   0        0        0     3671 2024-05-10 17:25:05.000000 geocif-0.1.27/geocif/ml/output.py
+-rw-rw-rw-   0        0        0     8286 2024-05-12 14:57:40.000000 geocif-0.1.27/geocif/ml/stages.py
+-rw-rw-rw-   0        0        0     8393 2024-05-13 20:11:22.000000 geocif-0.1.27/geocif/ml/stats.py
+-rw-rw-rw-   0        0        0     9433 2024-05-16 16:45:11.000000 geocif-0.1.27/geocif/ml/trainers.py
+-rw-rw-rw-   0        0        0     3149 2024-05-09 19:24:05.000000 geocif-0.1.27/geocif/ml/trend.py
+-rw-rw-rw-   0        0        0     2831 2024-05-09 19:24:05.000000 geocif-0.1.27/geocif/ml/xai.py
+drwxrwxrwx   0        0        0        0 2024-05-17 00:28:41.857837 geocif-0.1.27/geocif/playground/
+-rw-rw-rw-   0        0        0        0 2024-05-10 19:03:20.000000 geocif-0.1.27/geocif/playground/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 18:55:55.000000 geocif-0.1.27/geocif/playground/automl.py
+-rw-rw-rw-   0        0        0    13665 2024-05-11 01:04:25.000000 geocif-0.1.27/geocif/playground/misc.py
+-rw-rw-rw-   0        0        0    18744 2024-05-12 14:57:40.000000 geocif-0.1.27/geocif/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-17 00:28:41.870078 geocif-0.1.27/geocif/viz/
+-rw-rw-rw-   0        0        0       83 2024-05-10 16:27:36.000000 geocif-0.1.27/geocif/viz/__init__.py
+-rw-rw-rw-   0        0        0    15867 2024-05-15 21:02:40.000000 geocif-0.1.27/geocif/viz/plot.py
+drwxrwxrwx   0        0        0        0 2024-05-17 00:28:41.346553 geocif-0.1.27/geocif.egg-info/
+-rw-rw-rw-   0        0        0     1586 2024-05-17 00:28:36.000000 geocif-0.1.27/geocif.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1107 2024-05-17 00:28:39.000000 geocif-0.1.27/geocif.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 00:28:36.000000 geocif-0.1.27/geocif.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-10-22 16:27:17.000000 geocif-0.1.27/geocif.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2024-05-17 00:28:36.000000 geocif-0.1.27/geocif.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-05-10 01:05:13.000000 geocif-0.1.27/requirements.txt
+-rw-rw-rw-   0        0        0      415 2024-05-17 00:28:41.920358 geocif-0.1.27/setup.cfg
+-rw-rw-rw-   0        0        0     1617 2024-05-17 00:28:02.000000 geocif-0.1.27/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 00:28:41.898825 geocif-0.1.27/tests/
+-rw-rw-rw-   0        0        0      355 2024-05-09 16:20:58.000000 geocif-0.1.27/tests/test_geocif.py
```

### Comparing `geocif-0.1.26/LICENSE` & `geocif-0.1.27/LICENSE`

 * *Files identical despite different names*

### Comparing `geocif-0.1.26/PKG-INFO` & `geocif-0.1.27/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocif
-Version: 0.1.26
+Version: 0.1.27
 Summary: Models to visualize and forecast crop conditions and yields
 Home-page: https://ritviksahajpal.github.io/yield_forecasting/
 Author: Ritvik Sahajpal
 Author-email: ritvik@umd.edu
 License: MIT license
 Keywords: geocif
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `geocif-0.1.26/README.md` & `geocif-0.1.27/README.md`

 * *Files identical despite different names*

### Comparing `geocif-0.1.26/geocif/agmet/geoagmet.py` & `geocif-0.1.27/geocif/agmet/geoagmet.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.26/geocif/agmet/plot.py` & `geocif-0.1.27/geocif/agmet/plot.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.26/geocif/agmet/utils.py` & `geocif-0.1.27/geocif/agmet/utils.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.26/geocif/analysis.py` & `geocif-0.1.27/geocif/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -370,25 +370,26 @@
                 (df_model["% of total Area (ha)"] < 1)
                 & (df_model["Mean Absolute Percentage Error"] > 50)
                 & (df_model["Country"].isin(["Angola", "United Republic Of Tanzania"]))
             ]
 
             # Remove df_tmp from df_model
             df_model = df_model.drop(df_tmp.index)
-
             # Plot the histogram of MAPE
             # Create bins for '% of total Area (ha)' and 'MAPE'
+            bin_edges = np.linspace(0, df_model["% of total Area (ha)"].max() + 1, 5 + 1)
+
             df_model["Area Bins"] = pd.cut(
                 df_model["% of total Area (ha)"],
-                bins=[0, 2, 4, 6, 8, 10, 20, max(df_model["% of total Area (ha)"])],
+                bins=bin_edges,
                 precision=0,
             )
             df_model["MAPE Bins"] = pd.cut(
                 df_model["Mean Absolute Percentage Error"],
-                bins=6,  # [0, 5, 10, 15, 20, 25, 30, 50, max(df_model["Mean Absolute Percentage Error"])],
+                bins=5,  # [0, 5, 10, 15, 20, 25, 30, 50, max(df_model["Mean Absolute Percentage Error"])],
                 right=False,
                 precision=1,
             )
 
             # Count occurrences of MAPE values for each area bin
             area_mape_counts = (
                 df_model.groupby(["Area Bins", "MAPE Bins"])
@@ -440,15 +441,14 @@
             # Setting the title and labels
             plt.title(
                 f"Kernel Density Estimation of Mean Absolute Percentage Error by Country - {model}"
             )
             plt.xlabel("Mean Absolute Percentage Error (%)")
             plt.ylabel("Density")
             plt.legend(title="Country", title_fontsize="13")
-
             plt.savefig(self.dir_analysis / f"mape_histogram_{model}.png", dpi=250)
             plt.close()
 
             # Map MAPE at regional level
             df_model["Country Region"] = (
                 df_model["Country"].str.lower().str.replace("_", " ")
                 + " "
@@ -456,25 +456,28 @@
             )
 
             fname = f"mape_{self.crop}_{model}.png"
             col = "Mean Absolute Percentage Error"
             countries = df_model["Country"].unique().tolist()
             # make it title case and replace _ with space
             countries = [country.title().replace("_", " ") for country in countries]
+            countries = ["Malawi"]
+            df_model = df_model[df_model["Country"].isin(countries)]
+            self.dg = self.dg[self.dg["ADM0_NAME"].isin(countries)]
             plot.plot_df_shpfile(
                 self.dg,  # dataframe containing adm1 name and polygon
                 df_model,  # dataframe containing information that will be mapped
                 merge_col="Country Region",  # Column on which to merge
                 name_country=countries,
                 name_col=col,  # Which column to plot
                 dir_out=self.dir_analysis,  # Output directory
                 fname=fname,  # Output file name
-                label=f"Mean Absolute Percentage Error",
+                label=f"MAPE (%)",
                 vmin=df_model[col].min(),
-                vmax=50,  # df_model[col].max(),
+                vmax=df_model[col].max(),
                 cmap=pal.scientific.sequential.Bamako_20_r,
                 series="sequential",
                 show_bg=False,
                 annotate_regions=False,
                 loc_legend="lower left",
             )
 
@@ -484,28 +487,33 @@
     def map(self, df_plot):
         # df_plot = self.df_analysis.copy()
         models = df_plot["Model"].unique()
 
         for model in models:
             df_model = df_plot[df_plot["Model"] == model]
 
+            countries = ["malawi"]
+            df_model = df_model[df_model["Country"].isin(countries)]
+            self.dg = self.dg[self.dg["ADM0_NAME"].isin(["Malawi", "malawi"])]
+
             countries = df_model["Country"].unique().tolist()
             if len(countries) > 1:
                 self.dir_plot = self.dir_analysis
                 fname_prefix = f"{len(countries)}_countries"
             else:
                 self.dir_plot = self.dir_analysis / self.country / self.crop
                 fname_prefix = f"{self.country}"
             countries = [country.title().replace("_", " ") for country in countries]
             df_model["Country Region"] = (
                 df_model["Country"].str.lower().str.replace("_", " ")
                 + " "
                 + df_model["Region"].str.lower().str.replace("_", " ")
             )
 
+
             # Change Harvest year to type int
             df_model["Harvest Year"] = df_model["Harvest Year"].astype(int)
             annotate_region_column = (
                 "ADM1_NAME" if self.admin_zone == "admin_1" else "ADM2_NAME"
             )
             analysis_years = df_model["Harvest Year"].unique()
             for idx, year in enumerate(tqdm(analysis_years, desc="Map")):
@@ -513,103 +521,104 @@
 
                 for time_period in tqdm(
                     df_harvest_year["Stage Name"].unique(), desc="Map"
                 ):
                     df_time_period = df_harvest_year[
                         df_harvest_year["Stage Name"] == time_period
                     ]
-
-                    """ % of total area """
-                    # if idx == 0:
-                    #     fname = f"{self.country}_{self.crop}_perc_area.png"
-                    #     col = "% of total Area (ha)"
-                    #     plot.plot_df_shpfile(
-                    #         self.dg,  # dataframe containing adm1 name and polygon
-                    #         df_model,  # dataframe containing information that will be mapped
-                    #         merge_col="Country Region",  # Column on which to merge
-                    #         name_country=countries,  # Plot global map
-                    #         name_col=col,  # Which column to plot
-                    #         dir_out=self.plot_dir / str(year),  # Output directory
-                    #         fname=fname,  # Output file name
-                    #         label=f"% of Total Area (ha)\n{self.crop.title()}",
-                    #         vmin=df_model[col].min(),
-                    #         vmax=df_model[col].max(),
-                    #         cmap=pal.scientific.sequential.Bamako_20_r,
-                    #         series="sequential",
-                    #         show_bg=False,
-                    #         annotate_regions=True,
-                    #         annotate_region_column=annotate_region_column,
-                    #         loc_legend="lower left",
-                    #     )
-                    #
-                    #     """ Unique regions """
-                    #     fname = f"{self.country}_{self.crop}_region_ID.png"
-                    #     col = "Region_ID"
-                    #     df_model[col] = df_model[col].astype(int) + 1
-                    #     if len(df_model["Region_ID"].unique() > 1):
-                    #         # Create a dictionary with each region assigned a unique integer identifier and name
-                    #         dict_region = {
-                    #             int(key): key for key in df_time_period["Region_ID"].unique()
-                    #         }
-                    #         plot.plot_df_shpfile(
-                    #             self.dg,  # dataframe containing adm1 name and polygon
-                    #             df_model,  # dataframe containing information that will be mapped
-                    #             dict_lup=dict_region,
-                    #             merge_col="Country Region",  # Column on which to merge
-                    #             name_country=countries,  # Plot global map
-                    #             name_col=col,  # Which column to plot
-                    #             dir_out=self.plot_dir / str(year),  # Output directory
-                    #             fname=fname,  # Output file name
-                    #             label=f"Region Cluster\n{self.crop.title()}",
-                    #             vmin=df_model[col].min(),
-                    #             vmax=df_model[col].max(),
-                    #             cmap=pal.tableau.Tableau_20.mpl_colors,
-                    #             series="qualitative",
-                    #             show_bg=False,
-                    #             alpha_feature=1,
-                    #             use_key=True,
-                    #             annotate_regions=True,
-                    #             annotate_region_column=annotate_region_column,
-                    #             loc_legend="lower left",
-                    #         )
-
-                    """ Anomaly """
-                    fname = (
-                        f"{fname_prefix}_{self.crop}_{time_period}_{year}_anomaly.png"
-                    )
-                    plot.plot_df_shpfile(
-                        self.dg,  # dataframe containing adm1 name and polygon
-                        df_harvest_year,  # dataframe containing information that will be mapped
-                        merge_col="Country Region",  # Column on which to merge
-                        name_country=countries,  # Plot global map
-                        name_col="Anomaly",  # Which column to plot
-                        dir_out=self.dir_plot / str(year),  # Output directory
-                        fname=fname,  # Output file name
-                        label=f"% of {self.number_lag_years}-year Median Yield\n{self.crop.title()}, {year}",
-                        vmin=df_harvest_year["Anomaly"].min(),
-                        vmax=110,  # df_harvest_year["Anomaly"].max(),
-                        cmap=pal.cartocolors.diverging.Geyser_5_r,
-                        series="sequential",
-                        show_bg=False,
-                        annotate_regions=False,
-                        annotate_region_column=annotate_region_column,
-                        loc_legend="lower left",
-                    )
+    #
+    #                 """ % of total area """
+                    if idx == 0:
+                        fname = f"{self.country}_{self.crop}_perc_area.png"
+                        col = "% of total Area (ha)"
+                        plot.plot_df_shpfile(
+                            self.dg,  # dataframe containing adm1 name and polygon
+                            df_model,  # dataframe containing information that will be mapped
+                            merge_col="Country Region",  # Column on which to merge
+                            name_country=countries,  # Plot global map
+                            name_col=col,  # Which column to plot
+                            dir_out=self.dir_plot / str(year),  # Output directory
+                            fname=fname,  # Output file name
+                            label=f"% of Total Area (ha)\n{self.crop.title()}",
+                            vmin=df_model[col].min(),
+                            vmax=df_model[col].max(),
+                            cmap=pal.scientific.sequential.Bamako_20_r,
+                            series="sequential",
+                            show_bg=False,
+                            annotate_regions=False,
+                            annotate_region_column=annotate_region_column,
+                            loc_legend="lower left",
+                        )
+    #
+    #                 #     """ Unique regions """
+                    fname = f"{self.country}_{self.crop}_region_ID.png"
+                    col = "Region_ID"
+                    df_model[col] = df_model[col].astype(int) + 1
+                    if len(df_model["Region_ID"].unique() > 1):
+                        # Create a dictionary with each region assigned a unique integer identifier and name
+                        dict_region = {
+                            int(key): key for key in df_time_period["Region_ID"].unique()
+                        }
+                        plot.plot_df_shpfile(
+                            self.dg,  # dataframe containing adm1 name and polygon
+                            df_model,  # dataframe containing information that will be mapped
+                            dict_lup=dict_region,
+                            merge_col="Country Region",  # Column on which to merge
+                            name_country=countries,  # Plot global map
+                            name_col=col,  # Which column to plot
+                            dir_out=self.dir_plot / str(year),  # Output directory
+                            fname=fname,  # Output file name
+                            label=f"Region Cluster\n{self.crop.title()}",
+                            vmin=df_model[col].min(),
+                            vmax=df_model[col].max(),
+                            cmap=pal.tableau.Tableau_20.mpl_colors,
+                            series="qualitative",
+                            show_bg=False,
+                            alpha_feature=1,
+                            use_key=True,
+                            annotate_regions=False,
+                            annotate_region_column=annotate_region_column,
+                            loc_legend="lower left",
+                        )
+    #                     breakpoint()
+
+                    # """ Anomaly """
+                    # fname = (
+                    #     f"{fname_prefix}_{self.crop}_{time_period}_{year}_anomaly.png"
+                    # )
+                    # plot.plot_df_shpfile(
+                    #     self.dg,  # dataframe containing adm1 name and polygon
+                    #     df_harvest_year,  # dataframe containing information that will be mapped
+                    #     merge_col="Country Region",  # Column on which to merge
+                    #     name_country=countries,  # Plot global map
+                    #     name_col="Anomaly",  # Which column to plot
+                    #     dir_out=self.dir_plot / str(year),  # Output directory
+                    #     fname=fname,  # Output file name
+                    #     label=f"% of {self.number_lag_years}-year Median Yield\n{self.crop.title()}, {year}",
+                    #     vmin=df_harvest_year["Anomaly"].min(),
+                    #     vmax=110,  # df_harvest_year["Anomaly"].max(),
+                    #     cmap=pal.cartocolors.diverging.Geyser_5_r,
+                    #     series="sequential",
+                    #     show_bg=False,
+                    #     annotate_regions=False,
+                    #     annotate_region_column=annotate_region_column,
+                    #     loc_legend="lower left",
+                    # )
 
                     """ Predicted Yield """
                     fname = f"{fname_prefix}_{self.crop}_{time_period}_{year}_predicted_yield.png"
                     plot.plot_df_shpfile(
                         self.dg,  # dataframe containing adm1 name and polygon
                         df_harvest_year,  # dataframe containing information that will be mapped
                         merge_col="Country Region",  # Column on which to merge
                         name_country=countries,  # Plot global map
                         name_col="Predicted Yield (tn per ha)",  # Which column to plot
                         dir_out=self.dir_plot / str(year),  # Output directory
                         fname=fname,  # Output file name
-                        label=f"{self.predicted}\n{self.crop.title()}, {year}",
+                        label=f"Predicted Yield (Mg/ha)\n{self.crop.title()}, {year}",
                         vmin=df_harvest_year[self.predicted].min(),
                         vmax=df_harvest_year[self.predicted].max(),
                         cmap=pal.scientific.sequential.Bamako_20_r,
                         series="sequential",
                         show_bg=False,
                         annotate_regions=False,
                         annotate_region_column=annotate_region_column,
@@ -745,18 +754,18 @@
             method = df[df["Option"] == "method"]["Value"].values[0]
             crops = ast.literal_eval(df[df["Option"] == "crops"]["Value"].values[0])
             models = ast.literal_eval(df[df["Option"] == "models"]["Value"].values[0])
             admin_zone = df[df["Option"] == "admin_zone"]["Value"].values[0]
             name_shapefile = df[df["Option"] == "boundary_file"]["Value"].values[0]
 
             for crop in crops:
-                # Does a table with the name {country}-{crop} exist in the database?
-                table = f"{country}-{crop}"
+                # Does a table with the name {country}_{crop} exist in the database?
+                table = f"{country}_{crop}"
                 if self.table_exists(self.db_path, table):
-                    self.dict_config[f"{country}-{crop}"] = {
+                    self.dict_config[f"{country}_{crop}"] = {
                         "method": method,
                         "crops": crop,
                         "models": models,
                         "admin_zone": admin_zone,
                         "name_shapefile": name_shapefile,
                     }
 
@@ -785,35 +794,35 @@
         self.dg["Country Region"] = self.dg["Country Region"].str.cat(
             self.dg["ADM1_NAME"], sep=" "
         )
         self.dg.loc[self.dg["ADM2_NAME"].notna(), "Country Region"] = (
             self.dg["ADM0_NAME"] + " " + self.dg["ADM2_NAME"]
         )
         # Make it lower case
-        self.dg["Country Region"] = self.dg["Country Region"].str.lower()
+        self.dg["Country Region"] = self.dg["Country Region"].str.lower().replace("_", " ")
 
 
 def run(path_config_files=[Path("../config/geocif.txt")]):
     logger, parser = log.setup_logger_parser(path_config_files)
     obj = Geoanalysis(path_config_files, logger, parser)
     obj.setup()
 
     """ Loop over each country, crop, model combination in dict_config """
     frames = []
     for country_crop, value in obj.dict_config.items():
-        obj.country = country_crop.split("-")[0]
-        obj.crop = country_crop.split("-")[1]
+        obj.crop = value["crops"]
+        # to get country, remove obj.crops from country_crop
+        obj.country = country_crop.replace(f"_{obj.crop}", "")
 
         obj.admin_zone = value["admin_zone"]
         obj.boundary_file = value["name_shapefile"]
         obj.method = value["method"]
-        obj.number_lag_years = value["number_lag_years"]
+        obj.number_lag_years = 5
 
-        obj.table = f"{obj.country}-{obj.crop}"
-        breakpoint()
+        obj.table = f"{obj.country}_{obj.crop}"
         models = value["models"]
         for model in models:
             obj.model = model
 
             df_tmp = obj.execute()
             frames.append(df_tmp)
```

### Comparing `geocif-0.1.26/geocif/backup/features.py` & `geocif-0.1.27/geocif/backup/features.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.26/geocif/backup/geo.py` & `geocif-0.1.27/geocif/backup/geo.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.26/geocif/backup/geocif.py` & `geocif-0.1.27/geocif/backup/geocif.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.26/geocif/backup/metadata.py` & `geocif-0.1.27/geocif/backup/metadata.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.26/geocif/cei/definitions.py` & `geocif-0.1.27/geocif/cei/definitions.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.26/geocif/cei/indices.py` & `geocif-0.1.27/geocif/cei/indices.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.26/geocif/geocif.py` & `geocif-0.1.27/geocif/geocif.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,15 @@
         ====================================================================
         """
         self.method = self.parser.get("DEFAULT", "method")
         self.db_forecasts = self.parser.get("DEFAULT", "db")
         self.countries = ast.literal_eval(self.parser.get("DEFAULT", "countries"))
         self.do_parallel = self.parser.getboolean("DEFAULT", "do_parallel")
         self.update_input_file = self.parser.getboolean("DEFAULT", "update_input_file")
+        self.correlation_plots = self.parser.getboolean("DEFAULT", "correlation_plots")
         self.national_correlation = self.parser.getboolean(
             "DEFAULT", "national_correlation"
         )
         self.correlation_plot_groupby = self.parser.get(
             "DEFAULT", "correlation_plot_groupby"
         )
         self.run_ml = self.parser.getboolean("DEFAULT", "run_ml")
@@ -260,40 +261,29 @@
                     self.model.fit(
                         X_train,
                         y_train,
                         cat_features=self.cat_features,
                         verbose=False,
                         # callbacks=[TQDMCallback(self.best_hyperparams["iterations"])],
                     )
+                elif self.model_name == "merf":
+                    Z_train = np.ones((len(X_train), 1))
+                    clusters_train = df_region["Region"]
+                    clusters_train.reset_index(drop=True, inplace=True)
+
+                    self.model.fit(X_train, Z_train, clusters_train.astype("object"), y_train.values)
                 elif self.model_name == "linear":
                     self.model.fit(X_train_scaled, y_train)
                 elif self.model_name == "gam":
                     self.model.fit(X_train_scaled.values, y_train.values)
                     self.best_hyperparams = {}
                 elif self.model_name in ["cubist"]:
                     self.model.fit(X_train, y_train)
             except:
                 self.logger.error(f"Error fitting model for {self.country} {self.crop}")
-            # if self.cluster_strategy == "individual" or len(X_train) == 1:
-            #     self.model.fit(
-            #         X_train,
-            #         y_train,
-            #         cat_features=self.cat_features,
-            #         verbose=False,
-            #         # callbacks=[TQDMCallback(self.best_hyperparams["iterations"])],
-            #     )
-            # elif self.cluster_strategy in ["auto_detect", "single"]:
-            #     # Use MERF
-            #     Z_train = np.ones((len(X_train), 1))
-            #     clusters_train = df_region["Region"]
-            #     clusters_train.reset_index(drop=True, inplace=True)
-            #
-            #     self.model.fit(X_train, Z_train, clusters_train.astype("object"), y_train.values)
-            #     # change clusters_train to object dtype
-            #     # clusters_train = clusters_train.astype("object")
 
     def predict(self, df_region, scaler=None):
         """
         Predict yield for the current stage
         :param df_region:
         :param scaler:
         """
@@ -309,34 +299,38 @@
             elif self.model_name == "median":
                 y_pred = np.full(len(X_test), df_region[f"Median {self.target}"].values)
             elif self.model_name == "last_year":
                 y_pred = np.full(
                     len(X_test), df_region[f"Last Year {self.target}"].values
                 )
         else:
-            best_hyperparameters = self.model.get_params().copy()
             if self.model_name in ["linear", "gam"]:
                 # Drop cat_features from X_test
                 X_test = X_test.drop(
                     columns=[
                         item for item in self.cat_features if item != "Harvest Year"
                     ]
                 )
                 X_test = scaler.transform(X_test)
                 best_hyperparameters = {}
 
             if self.estimate_ci:
                 if self.estimate_ci_for_all or self.forecast_season == self.today_year:
                     y_pred, y_pred_ci = self.model.predict(X_test, alpha=0.1)
+                    best_hyperparameters = self.model.get_params().copy()
+            elif self.model_name == "merf":
+                Z_test = np.ones((len(X_test), 1))
+                clusters_test = df_region["Region"]
+                clusters_test.reset_index(drop=True, inplace=True)
+
+                y_pred = self.model.predict(X_test, Z_test, clusters_test.astype("object"))
+                best_hyperparameters = self.model.fe_model.get_params().copy()
             else:
                 y_pred = self.model.predict(X_test)
-            # Z_test = np.ones((len(X_test), 1))
-            # clusters_test = df_region["Region"]
-            # clusters_test.reset_index(drop=True, inplace=True)
-            # y_pred = self.model.predict(X_test, Z_test, clusters_test.astype("object"))
+                best_hyperparameters = self.model.get_params().copy()
 
         if self.check_yield_trend:
             # Get information for retrending
             for idx, region in enumerate(df_region["Region"].unique()):
                 mask_region = self.df_train["Region"] == df_region["Region"].unique()[0]
                 df_tmp = self.df_train[mask_region]
 
@@ -349,15 +343,15 @@
                 # Retrend the predicted yield
                 y_pred[idx] += trend.compute_trend(
                     obj_trend, df_region.iloc[idx][["Harvest Year"]]
                 )[0]
 
         # Create a dataframe with forecast results
         shp = len(X_test)
-        experiment_id = f"{self.country}-{self.crop}"
+        experiment_id = f"{self.country}_{self.crop}"
         now = ar.utcnow().to("America/New_York").format("MMMM-DD-YYYY HH:mm:ss")
         selected_features = self.selected_features + self.cat_features
         df = pd.DataFrame(
             {
                 "Experiment_ID": np.full(shp, experiment_id),
                 "Date": np.full(shp, self.today),
                 "Time": np.full(shp, now),
@@ -460,15 +454,15 @@
         self.feature_names = []
 
         """ Select stages that will be used for ML
          1. method = "latest" - Select the latest stage
          2. method = "fraction" - Select a fraction (1-100) of all stages
         """
         stages_features = stages.select_stages_for_ml(
-            stages_features, method="fraction", n=30
+            stages_features, method="fraction", n=60
         )
 
         for stage in stages_features:
             # Convert each element of stage to str and join with _
             _stage = "_".join([str(x) for x in stage])
 
             # Create a list appending _stage to each element of combined_keys
@@ -739,38 +733,39 @@
         # Only use geometry column from self.dg
         self.dg_country = self.dg_country[["Country Region", "geometry"]].merge(
             df[["Country Region", self.correlation_plot_groupby]],
             on="Country Region",
             how="outer",
         )
 
-        dict_kwargs = {}
-        dict_kwargs["all_stages"] = self.all_stages
-        dict_kwargs["target_col"] = self.target
-        dict_kwargs["country"] = self.country
-        dict_kwargs["crop"] = self.crop
-        dict_kwargs["dir_output"] = (
-            self.dir_analysis
-            / self.country
-            / self.crop
-            / self.model_name
-            / str(self.forecast_season)
-        )
-        dict_kwargs["forecast_season"] = self.forecast_season
-        dict_kwargs["method"] = self.method
-        dict_kwargs["national_correlation"] = self.national_correlation
-        dict_kwargs["groupby"] = self.correlation_plot_groupby
-        dict_kwargs["dg_country"] = self.dg_country
-        dict_kwargs["combined_dict"] = self.combined_dict
-
-        self.logger.info(f"Correlation plot for {self.country} {self.crop}")
-        (
-            dict_selected_features,
-            dict_best_cei,
-        ) = correlations.all_correlated_feature_by_time(df, **dict_kwargs)
+        if self.correlation_plots:
+            dict_kwargs = {}
+            dict_kwargs["all_stages"] = self.all_stages
+            dict_kwargs["target_col"] = self.target
+            dict_kwargs["country"] = self.country
+            dict_kwargs["crop"] = self.crop
+            dict_kwargs["dir_output"] = (
+                self.dir_analysis
+                / self.country
+                / self.crop
+                / self.model_name
+                / str(self.forecast_season)
+            )
+            dict_kwargs["forecast_season"] = self.forecast_season
+            dict_kwargs["method"] = self.method
+            dict_kwargs["national_correlation"] = self.national_correlation
+            dict_kwargs["groupby"] = self.correlation_plot_groupby
+            dict_kwargs["dg_country"] = self.dg_country
+            dict_kwargs["combined_dict"] = self.combined_dict
+
+            self.logger.info(f"Correlation plot for {self.country} {self.crop}")
+            (
+                dict_selected_features,
+                dict_best_cei,
+            ) = correlations.all_correlated_feature_by_time(df, **dict_kwargs)
 
         """ Separate into train and test datasets based on forecast_season """
         mask = df["Harvest Year"] == self.forecast_season
         self.df_train = df[~mask]
         self.df_test = df[mask]
 
         # Drop rows with missing values for self.target_col in df_train
@@ -837,15 +832,15 @@
         self.ml_model = self.parser.getboolean(self.model_name, "ML_model")
         self.model_names = ast.literal_eval(self.parser.get(self.country, "models"))
         self.optimize = self.parser.getboolean(self.country, "optimize")
         self.fraction_loocv = self.parser.getfloat(self.country, "fraction_loocv")
         self.all_seasons = self.df_results["Harvest Year"].unique()
 
         """ If not using a ML model then set XAI and CI to False """
-        if not self.ml_model or self.model_name in ["linear", "gam"]:
+        if not self.ml_model or self.model_name in ["linear", "gam", "merf"]:
             self.do_xai = False
             self.estimate_ci = False
             self.check_yield_trend = False
             self.estimate_ci_for_all = False
         else:
             self.do_xai = self.parser.getboolean("ML", "do_xai")
             self.estimate_ci = self.parser.getboolean("ML", "estimate_ci")
```

### Comparing `geocif-0.1.26/geocif/indices_runner.py` & `geocif-0.1.27/geocif/indices_runner.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.26/geocif/logger.py` & `geocif-0.1.27/geocif/logger.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.26/geocif/ml/correlations.py` & `geocif-0.1.27/geocif/ml/correlations.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,16 +270,20 @@
                 )
 
                 kwargs["region_id"] = region_id
                 plot_feature_corr_by_time(df_tmp, **kwargs)
                 # For each element in dict_best_cei, add the type of the cei
             else:
                 # HACK
-                dict_selected_features[region_id] = dict_selected_features[0]
-                dict_best_cei[region_id] = dict_best_cei[0]
+                df_corr = _all_correlated_feature_by_time(df, **kwargs)
+                dict_selected_features[region_id] = df_corr.columns
+                dict_best_cei[region_id] = {}
+
+                #dict_selected_features[region_id] = dict_selected_features[0]
+                #dict_best_cei[region_id] = dict_best_cei[0]
                 # Combine all unique values from the existing dictionary elements
                 # combined_metrics = set()
                 # for key in dict_selected_features:
                 #     breakpoint()
                 #     combined_metrics.update(dict_selected_features[key])
                 #
                 # # Add the combined set as a new element with key 3
```

### Comparing `geocif-0.1.26/geocif/ml/embedding.py` & `geocif-0.1.27/geocif/ml/embedding.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.26/geocif/ml/feature_engineering.py` & `geocif-0.1.27/geocif/ml/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.26/geocif/ml/outliers.py` & `geocif-0.1.27/geocif/ml/outliers.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.26/geocif/ml/outlook.py` & `geocif-0.1.27/geocif/ml/outlook.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.26/geocif/ml/output.py` & `geocif-0.1.27/geocif/ml/output.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.26/geocif/ml/stages.py` & `geocif-0.1.27/geocif/ml/stages.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.26/geocif/ml/stats.py` & `geocif-0.1.27/geocif/ml/stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -201,14 +201,19 @@
                 mask_yield & mask_region & (df_fewsnet["indicator"] == "area"), "value"
             ]
             prod_value = df_fewsnet.loc[
                 mask_yield & mask_region & (df_fewsnet["indicator"] == "production"),
                 "value",
             ]
 
+            # Replace any inf or 0 values by NaN
+            yield_value = yield_value.replace([0, np.inf, -np.inf], np.nan)
+            area_value = area_value.replace([0, np.inf, -np.inf], np.nan)
+            prod_value = prod_value.replace([0, np.inf, -np.inf], np.nan)
+
             if not yield_value.empty:
                 group.loc[:, target_col] = yield_value.values[0]
                 group.loc[:, "Area (ha)"] = area_value.values[0]
                 group.loc[:, "Production (tn)"] = prod_value.values[0]
 
             return group
```

### Comparing `geocif-0.1.26/geocif/ml/trainers.py` & `geocif-0.1.27/geocif/ml/trainers.py`

 * *Files 3% similar despite different names*

```diff
@@ -248,38 +248,35 @@
             fraction_loocv,
             cat_features,
             seed,
         )
     else:
         hyperparams = {}
 
-        if model_name == "catboost":
+        if model_name in ["catboost", "merf"]:
             hyperparams = {
                 "depth": 6,
                 "learning_rate": 0.01,
                 "iterations": 5000,
                 "subsample": 1.0,
                 "random_strength": 0.5,
                 "reg_lambda": 0.001,
                 "loss_function": "MAPE",
                 "early_stopping_rounds": 50,
                 "random_seed": seed,
                 "verbose": False,
             }
-            model = CatBoostRegressor(**hyperparams, cat_features=cat_features)
-            # if cluster_strategy in ["auto_detect", "single"]:
-            #     from merf import MERF
-            #
-            #     regr = CatBoostRegressor(**hyperparams, cat_features=cat_features)
-            #
-            #     model = MERF(regr, max_iterations=5)
-            # elif cluster_strategy == "individual":
-            #     # For all features with AUC in name, set monotone_constraints to 1, rest are 0
-            #     # monotone_constraints = [1 if "AUC_" in ftr else 0 for ftr in feature_names]
-            #     model = CatBoostRegressor(**hyperparams, cat_features=cat_features)
+            if model_name == "catboost":
+                model = CatBoostRegressor(**hyperparams, cat_features=cat_features)
+            elif model_name == "merf":
+                from merf import MERF
+
+                hyperparams["iterations"] = 1000
+                regr = CatBoostRegressor(**hyperparams, cat_features=cat_features)
+                model = MERF(regr, max_iterations=10)
         elif model_name == "linear":
             from sklearn.linear_model import LassoCV
 
             model = LassoCV(cv=5, random_state=42)
         elif model_name == "gam":
             from pygam import LinearGAM
```

### Comparing `geocif-0.1.26/geocif/ml/trend.py` & `geocif-0.1.27/geocif/ml/trend.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.26/geocif/ml/xai.py` & `geocif-0.1.27/geocif/ml/xai.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.26/geocif/playground/misc.py` & `geocif-0.1.27/geocif/playground/misc.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.26/geocif/utils.py` & `geocif-0.1.27/geocif/utils.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.26/geocif/viz/plot.py` & `geocif-0.1.27/geocif/viz/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,15 +328,15 @@
             # plt.setp(cb.ax.xaxis.get_ticklines(), alpha=0.6)
             # Do not show first and last tick label
             ticks[0] = ""
             ticks[-1] = ""
             cb.ax.set_title(
                 label, fontsize=8, fontweight="semibold", fontfamily="Arial"
             )
-            cb.ax.set_xticklabels(ticks, fontsize=6, fontfamily="Arial")
+            cb.ax.set_xticklabels(ticks, fontsize=4, fontfamily="Arial")
 
             # Use BoundaryNorm to create discrete levels
             # sm = plt.cm.ScalarMappable(cmap=cmap.mpl_colormap, norm=norm)
             # sm._A = []  # This is a hack to make sure the ScalarMappable is aware of the colormap
 
             # Adjust format based on the step size
             # step_size = (vmax - vmin) / number_of_intervals
```

### Comparing `geocif-0.1.26/geocif.egg-info/PKG-INFO` & `geocif-0.1.27/geocif.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocif
-Version: 0.1.26
+Version: 0.1.27
 Summary: Models to visualize and forecast crop conditions and yields
 Home-page: https://ritviksahajpal.github.io/yield_forecasting/
 Author: Ritvik Sahajpal
 Author-email: ritvik@umd.edu
 License: MIT license
 Keywords: geocif
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `geocif-0.1.26/geocif.egg-info/SOURCES.txt` & `geocif-0.1.27/geocif.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geocif-0.1.26/setup.py` & `geocif-0.1.27/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,10 +46,10 @@
     keywords="geocif",
     name="geocif",
     packages=find_packages(include=["geocif", "geocif.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://ritviksahajpal.github.io/yield_forecasting/",
-    version="0.1.26",
+    version="0.1.27",
     zip_safe=False,
 )
```

