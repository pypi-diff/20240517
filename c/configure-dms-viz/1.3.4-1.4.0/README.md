# Comparing `tmp/configure_dms_viz-1.3.4.tar.gz` & `tmp/configure_dms_viz-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configure_dms_viz-1.3.4.tar", max compression
+gzip compressed data, was "configure_dms_viz-1.4.0.tar", max compression
```

## Comparing `configure_dms_viz-1.3.4.tar` & `configure_dms_viz-1.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1095 2024-05-15 22:23:18.834303 configure_dms_viz-1.3.4/LICENSE
--rw-r--r--   0        0        0     9172 2024-05-15 22:23:18.834303 configure_dms_viz-1.3.4/README.md
--rw-r--r--   0        0        0        0 2024-05-15 22:23:18.834303 configure_dms_viz-1.3.4/configure_dms_viz/__init__.py
--rwxr-xr-x   0        0        0    38915 2024-05-15 22:23:18.834303 configure_dms_viz-1.3.4/configure_dms_viz/configure_dms_viz.py
--rw-r--r--   0        0        0     8500 2024-05-15 22:23:18.834303 configure_dms_viz-1.3.4/configure_dms_viz/pdb_utils.py
--rw-r--r--   0        0        0     1454 2024-05-15 22:23:18.834303 configure_dms_viz-1.3.4/pyproject.toml
--rw-r--r--   0        0        0    10199 1970-01-01 00:00:00.000000 configure_dms_viz-1.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-05-17 20:09:26.922952 configure_dms_viz-1.4.0/LICENSE
+-rw-r--r--   0        0        0     9172 2024-05-17 20:09:26.922952 configure_dms_viz-1.4.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-17 20:09:26.922952 configure_dms_viz-1.4.0/configure_dms_viz/__init__.py
+-rwxr-xr-x   0        0        0    41547 2024-05-17 20:09:26.922952 configure_dms_viz-1.4.0/configure_dms_viz/configure_dms_viz.py
+-rw-r--r--   0        0        0     8500 2024-05-17 20:09:26.922952 configure_dms_viz-1.4.0/configure_dms_viz/pdb_utils.py
+-rw-r--r--   0        0        0     1454 2024-05-17 20:09:26.922952 configure_dms_viz-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    10199 1970-01-01 00:00:00.000000 configure_dms_viz-1.4.0/PKG-INFO
```

### Comparing `configure_dms_viz-1.3.4/LICENSE` & `configure_dms_viz-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `configure_dms_viz-1.3.4/README.md` & `configure_dms_viz-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `configure_dms_viz-1.3.4/configure_dms_viz/configure_dms_viz.py` & `configure_dms_viz-1.4.0/configure_dms_viz/configure_dms_viz.py`

 * *Files 3% similar despite different names*

```diff
@@ -353,14 +353,15 @@
     mut_metric_df,
     metric_col,
     sitemap_df,
     structure,
     join_data=None,
     filter_cols=None,
     filter_limits=None,
+    heatmap_limits=None,
     tooltip_cols=None,
     metric_name=None,
     condition_col=None,
     condition_name=None,
     included_chains="polymer",
     excluded_chains="none",
     alphabet="RKHDEQNSTYWFAILMVGPC-*",
@@ -392,14 +393,16 @@
         Rename or format the condition column if desired.
     join_data: list or None
         A list of pandas.dataFrames to join to the main dataframe by mutation/condition.
     filter_cols: dict or None
         A dictionary of column names and formatted names to designate as filters.
     filter_limits: dict or None
         A dictionary of the desired min and max values for each filter column slider range.
+    heatmap_limits: list or None
+        A list of the desired min, max, and center values for the metric to be used for the heatmap's color scale.
     tooltip_cols: dict or None
         A dictionary of column names and formatted names to designate as tooltips.
     included_chains: str or None
         If not mapping data to every chain, a space separated list of chain names (i.e. "C F M G J P").
     excluded_chains: str or None
         A space separated string of chains that should not be shown on the protein structure (i.e. "B L R").
     alphabet: str
@@ -439,23 +442,22 @@
     mut_metric_df = format_mutation_data(
         mut_metric_df, metric_col, condition_col, alphabet
     )
 
     # If there is no sitemap dataframe, create a default one
     if sitemap_df is None:
         click.secho(
-            message="Warning: No sitemap dataframe was provided. Creating a default sitemap.",
+            message="Warning: No sitemap dataframe was provided. Creating a default sitemap.\n If no site map is provided, the reference sites will be sorted but may appear out of order.",
             fg="yellow",
         )
+        reference_sites = sorted(list(set(mut_metric_df["reference_site"].to_list())))
         sitemap_df = pd.DataFrame(
             {
-                "reference_site": mut_metric_df["reference_site"].unique(),
-                "sequential_site": range(
-                    1, len(mut_metric_df["reference_site"].unique()) + 1
-                ),
+                "reference_site": reference_sites,
+                "sequential_site": range(1, len(reference_sites) + 1),
             }
         )
 
     # Check that the necessary columns are present in the sitemap dataframe and format
     sitemap_df = format_sitemap_data(sitemap_df, mut_metric_df, included_chains)
 
     # Keep track of the required columns to cut down on the final total data size
@@ -465,14 +467,57 @@
     if join_data:
         mut_metric_df = join_additional_data(mut_metric_df, join_data)
 
     # Add the condition column to the required columns if it's not None
     if condition_col:
         cols_to_keep.append(condition_col)
 
+    # Check that the heatmap limits are in the correct format
+    if heatmap_limits:
+        # Check that the values are all able to be coerced into numbers
+        for value in heatmap_limits:
+            try:
+                pd.to_numeric(value)
+            except ValueError as err:
+                raise ValueError(
+                    f"The heatmap limit '{value}' cannot be coerced into a number."
+                ) from err
+        # Only the center of the scale is provided
+        if len(heatmap_limits) == 1:
+            click.secho(
+                message="One value was provided for heatmap limits, this will be the center value of the scale.\n",
+                fg="green",
+            )
+        # The min and max are provided
+        elif len(heatmap_limits) == 2:
+            click.secho(
+                message="Two values were provided for heatmap limits, these will be the min and max of the scale.\n",
+                fg="green",
+            )
+            # Check that the values are in the correct order
+            if heatmap_limits[0] > heatmap_limits[1]:
+                raise ValueError(
+                    "The heatmap limits are not specified correctly. The min value must be less than the max value."
+                )
+        # The min, center, and max are provided
+        elif len(heatmap_limits) == 3:
+            click.secho(
+                message="Three values were provided for heatmap limits, these will be the min, center, and max of the scale.\n",
+                fg="green",
+            )
+            # Check that the values are in the correct order
+            if not heatmap_limits[0] < heatmap_limits[1] < heatmap_limits[2]:
+                raise ValueError(
+                    "The heatmap limits are not specified correctly. The min value must be less than the max value and the center value must be in between."
+                )
+        else:
+            raise ValueError(
+                "The heatmap limits must be a list of one, two, or three values."
+            )
+
     # Add the filter columns to the required columns
     if filter_cols:
         cols = check_filter_columns(mut_metric_df, filter_cols)
         cols_to_keep += cols
         if filter_limits:
             filter_limits_cols = [col for col in filter_limits.keys()]
             # Check that the columns are in the filter columns
@@ -653,14 +698,15 @@
         "negative_condition_colors": negative_condition_colors,
         "alphabet": [aa for aa in alphabet],
         "pdb": pdb,
         "dataChains": included_chains.split(" "),
         "excludeChains": excluded_chains.split(" "),
         "filter_cols": filter_cols,
         "filter_limits": filter_limits,
+        "heatmap_limits": heatmap_limits,
         "tooltip_cols": tooltip_cols,
         "excludedAminoAcids": exclude_amino_acids,
         "description": description,
         "title": title,
     }
 
     return experiment_dict
@@ -767,14 +813,21 @@
     "--filter-limits",
     type=DictParamType(),
     required=False,
     default=None,
     help="Optionally, a space separated list of columns to use as filters in the visualization. Example: \"{'effect': [min, max], 'times_seen': [min, max]}\"",
 )
 @click.option(
+    "--heatmap-limits",
+    type=ListParamType(),
+    required=False,
+    default=None,
+    help='Optionally, a list of the min, center, and max values for the metric to be used for the heatmap\'s color scale. Example: "[min, center, max]"',
+)
+@click.option(
     "--tooltip-cols",
     type=DictParamType(),
     required=False,
     default=None,
     help="Optionally, a space separated list of columns to use as tooltips in the visualization. Example: \"{'times_seen': '# Obsv', 'effect': 'Func Eff.'}\"",
 )
 @click.option(
@@ -855,14 +908,15 @@
     structure,
     name,
     output,
     metric_name,
     condition_name,
     filter_cols,
     filter_limits,
+    heatmap_limits,
     tooltip_cols,
     join_data,
     included_chains,
     excluded_chains,
     alphabet,
     colors,
     negative_colors,
@@ -901,14 +955,15 @@
         mut_metric_df,
         metric,
         sitemap_df,
         structure,
         join_data_dfs,
         filter_cols,
         filter_limits,
+        heatmap_limits,
         tooltip_cols,
         metric_name,
         condition,
         condition_name,
         included_chains,
         excluded_chains,
         alphabet,
```

### Comparing `configure_dms_viz-1.3.4/configure_dms_viz/pdb_utils.py` & `configure_dms_viz-1.4.0/configure_dms_viz/pdb_utils.py`

 * *Files identical despite different names*

### Comparing `configure_dms_viz-1.3.4/pyproject.toml` & `configure_dms_viz-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configure-dms-viz"
-version = "1.3.4"
+version = "1.4.0"
 description = "Configure your data for visualization with dms-viz.github.io"
 authors = ["Will Hannon <hannonww@gmail.com>"]
 maintainers = ["Will Hannon <hannonww@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dms-viz"
 repository = "https://github.com/dms-viz/configure_dms_viz"
```

### Comparing `configure_dms_viz-1.3.4/PKG-INFO` & `configure_dms_viz-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configure-dms-viz
-Version: 1.3.4
+Version: 1.4.0
 Summary: Configure your data for visualization with dms-viz.github.io
 Home-page: https://github.com/dms-viz
 License: MIT
 Keywords: deep mutational scanning,interactive protein structure,dms-viz,dms,protein
 Author: Will Hannon
 Author-email: hannonww@gmail.com
 Maintainer: Will Hannon
```

