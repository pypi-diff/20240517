# Comparing `tmp/py50-1.0.3.tar.gz` & `tmp/py50-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py50-1.0.3.tar", max compression
+gzip compressed data, was "py50-1.0.4.tar", max compression
```

## Comparing `py50-1.0.3.tar` & `py50-1.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-11-15 10:28:16.943898 py50-1.0.3/LICENSE
--rw-r--r--   0        0        0     4542 2024-05-15 04:09:24.427854 py50-1.0.3/README_pypi.md
--rw-r--r--   0        0        0     6148 2024-02-12 06:00:11.583727 py50-1.0.3/py50/.DS_Store
--rw-r--r--   0        0        0      177 2024-04-17 01:25:24.147050 py50-1.0.3/py50/__init__.py
--rw-r--r--   0        0        0    20268 2024-04-26 14:38:41.720572 py50-1.0.3/py50/calculator.py
--rw-r--r--   0        0        0     8604 2024-01-29 16:09:38.892265 py50-1.0.3/py50/plot_settings.py
--rw-r--r--   0        0        0    43460 2024-04-30 01:26:56.191290 py50-1.0.3/py50/plotcurve.py
--rw-r--r--   0        0        0    92545 2024-05-15 02:13:49.689769 py50-1.0.3/py50/stats.py
--rw-r--r--   0        0        0     6413 2024-04-20 14:15:03.007112 py50-1.0.3/py50/utils.py
--rw-r--r--   0        0        0      591 2024-05-15 04:11:36.936202 py50-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     5450 1970-01-01 00:00:00.000000 py50-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-11-15 10:28:16.943898 py50-1.0.4/LICENSE
+-rw-r--r--   0        0        0     4542 2024-05-15 04:09:24.427854 py50-1.0.4/README_pypi.md
+-rw-r--r--   0        0        0     6148 2024-02-12 06:00:11.583727 py50-1.0.4/py50/.DS_Store
+-rw-r--r--   0        0        0      177 2024-04-17 01:25:24.147050 py50-1.0.4/py50/__init__.py
+-rw-r--r--   0        0        0    20268 2024-04-26 14:38:41.720572 py50-1.0.4/py50/calculator.py
+-rw-r--r--   0        0        0     8604 2024-01-29 16:09:38.892265 py50-1.0.4/py50/plot_settings.py
+-rw-r--r--   0        0        0    43460 2024-04-30 01:26:56.191290 py50-1.0.4/py50/plotcurve.py
+-rw-r--r--   0        0        0    94182 2024-05-16 05:42:39.475829 py50-1.0.4/py50/stats.py
+-rw-r--r--   0        0        0     6413 2024-04-20 14:15:03.007112 py50-1.0.4/py50/utils.py
+-rw-r--r--   0        0        0      591 2024-05-17 01:21:25.687210 py50-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5450 1970-01-01 00:00:00.000000 py50-1.0.4/PKG-INFO
```

### Comparing `py50-1.0.3/LICENSE` & `py50-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py50-1.0.3/README_pypi.md` & `py50-1.0.4/README_pypi.md`

 * *Files identical despite different names*

### Comparing `py50-1.0.3/py50/.DS_Store` & `py50-1.0.4/py50/.DS_Store`

 * *Files identical despite different names*

### Comparing `py50-1.0.3/py50/calculator.py` & `py50-1.0.4/py50/calculator.py`

 * *Files identical despite different names*

### Comparing `py50-1.0.3/py50/plot_settings.py` & `py50-1.0.4/py50/plot_settings.py`

 * *Files identical despite different names*

### Comparing `py50-1.0.3/py50/plotcurve.py` & `py50-1.0.4/py50/plotcurve.py`

 * *Files identical despite different names*

### Comparing `py50-1.0.3/py50/stats.py` & `py50-1.0.4/py50/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -316,16 +316,16 @@
 
             # From unique items in group list, generate pairs
             pairs = list(combinations(group, 2))
 
             results_list = []
             for pair in pairs:
                 # Get items from pair list and split by hyphen
-                group1, subgroup1 = pair[0].split("-")
-                group2, subgroup2 = pair[1].split("-")
+                group1, subgroup1 = pair[0].split("-", 1)
+                group2, subgroup2 = pair[1].split("-", 1)
 
                 # # For troubleshooting
                 # print("first:", data[(data[group_col] == group1)][value_col].shape)
                 # print("second:", data[(data[group_col] == group2)][value_col].shape)
 
                 # Check length of groups
                 group1_length = self.data[self.data[group_col] == group1][value_col]
@@ -368,16 +368,16 @@
                     }
                 )
 
             # Convert the list of dictionaries to a DataFrame
             result_df = pd.DataFrame(results_list)
 
             # Split values into and separate by comma
-            result_df["A"] = result_df["A"].apply(lambda x: tuple(x.split("-")))
-            result_df["B"] = result_df["B"].apply(lambda x: tuple(x.split("-")))
+            result_df["A"] = result_df["A"].apply(lambda x: tuple(x.split("-", 1)))
+            result_df["B"] = result_df["B"].apply(lambda x: tuple(x.split("-", 1)))
 
             return result_df
         else:
             """
             No subgroups found. Tests single group and values.
             """
             # Get unique pairs from group
@@ -484,17 +484,19 @@
             elif self.data[subgroup_col].dtype != "object":
                 raise ValueError(f"Is subgroup_col: '{subgroup_col}' strings?")
             elif self.data[value_col].dtype == "object":
                 raise ValueError(f"Is value_col: '{value_col}' should be numerical?")
 
             results_list = []
             for pair in pairs:
+                # print('this is the pair:', pair)  # for troubleshooting
+                # print('this is the pairs:', pairs)
                 # Get items from pair list and split by hyphen
-                group1, subgroup1 = pair[0].split("-")
-                group2, subgroup2 = pair[1].split("-")
+                group1, subgroup1 = pair[0].split("-", 1)
+                group2, subgroup2 = pair[1].split("-", 1)
 
                 # Perform mwu
                 result = pg.mwu(
                     self.data[
                         (self.data[group_col] == group1)
                         & (self.data[subgroup_col] == subgroup1)
                     ][value_col],
@@ -522,16 +524,16 @@
                     }
                 )
 
             # Convert the list of dictionaries to a DataFrame
             df = pd.DataFrame(results_list)
 
             # Split values into and separate by comma
-            df["A"] = df["A"].apply(lambda x: tuple(x.split("-")))
-            df["B"] = df["B"].apply(lambda x: tuple(x.split("-")))
+            df["A"] = df["A"].apply(lambda x: tuple(x.split("-", 1)))
+            df["B"] = df["B"].apply(lambda x: tuple(x.split("-", 1)))
 
             return df
         else:
             """
             No subgroups found. Tests single group and values.
             """
             # Get unique pairs from group
@@ -966,19 +968,24 @@
         # If set to True, only show plots with significance
         if hide_ns is True:
             # Filter n.s. from pvalue and pairs
             hidden_sigfig_data = [
                 (item1, item2) for item1, item2 in zip(pvalue, pairs) if item1 != "n.s."
             ]
 
-            # Unzip the hidden_sigfig_data and separate into pvalue and pairs variables
-            pvalue, pairs = zip(*hidden_sigfig_data)
-            # # to trouble shoot
-            # print(pvalue)
-            # print(pairs)
+            try:
+                # Unzip the hidden_sigfig_data and separate into pvalue and pairs variables
+                pvalue, pairs = zip(*hidden_sigfig_data)
+                # # to troubleshoot
+                # print(pvalue)
+                # print(pairs)
+            except:
+                warnings.warn("No Significant Values. hide_ns will be set to False!")
+                if all(sigfig == "n.s." for sigfig in pvalue):
+                    hide_ns = False
 
         # set orientation for plot and Annotator
         orient = orient.lower()
         if orient == "v":
             ax = sns.boxplot(
                 data=self.data,
                 x=group_col,
@@ -1157,19 +1164,24 @@
         # If set to True, only show plots with significance
         if hide_ns is True:
             # Filter n.s. from pvalue and pairs
             hidden_sigfig_data = [
                 (item1, item2) for item1, item2 in zip(pvalue, pairs) if item1 != "n.s."
             ]
 
-            # Unzip the hidden_sigfig_data and separate into pvalue and pairs variables
-            pvalue, pairs = zip(*hidden_sigfig_data)
-            # # to trouble shoot
-            # print(pvalue)
-            # print(pairs)
+            try:
+                # Unzip the hidden_sigfig_data and separate into pvalue and pairs variables
+                pvalue, pairs = zip(*hidden_sigfig_data)
+                # # to troubleshoot
+                # print(pvalue)
+                # print(pairs)
+            except:
+                warnings.warn("No Significant Values. hide_ns will be set to False!")
+                if all(sigfig == "n.s." for sigfig in pvalue):
+                    hide_ns = False
 
         # set orientation for plot and Annotator
         orient = orient.lower()
         if orient == "v":
             ax = sns.barplot(
                 data=self.data,
                 x=group_col,
@@ -1346,19 +1358,24 @@
         # If set to True, only show plots with significance
         if hide_ns is True:
             # Filter n.s. from pvalue and pairs
             hidden_sigfig_data = [
                 (item1, item2) for item1, item2 in zip(pvalue, pairs) if item1 != "n.s."
             ]
 
-            # Unzip the hidden_sigfig_data and separate into pvalue and pairs
-            pvalue, pairs = zip(*hidden_sigfig_data)
-            # # to trouble shoot
-            # print(pvalue)
-            # print(pairs)
+            try:
+                # Unzip the hidden_sigfig_data and separate into pvalue and pairs variables
+                pvalue, pairs = zip(*hidden_sigfig_data)
+                # # to troubleshoot
+                # print(pvalue)
+                # print(pairs)
+            except:
+                warnings.warn("No Significant Values. hide_ns will be set to False!")
+                if all(sigfig == "n.s." for sigfig in pvalue):
+                    hide_ns = False
 
         # set orientation for plot and Annotator
         orient = orient.lower()
         if orient == "v":
             ax = sns.violinplot(
                 data=self.data,
                 x=group_col,
@@ -1534,19 +1551,24 @@
         # If set to True, only show plots with significance
         if hide_ns is True:
             # Filter n.s. from pvalue and pairs
             hidden_sigfig_data = [
                 (item1, item2) for item1, item2 in zip(pvalue, pairs) if item1 != "n.s."
             ]
 
-            # Unzip the hidden_sigfig_data and separate into pvalue and pairs
-            pvalue, pairs = zip(*hidden_sigfig_data)
-            # # to trouble shoot
-            # print(pvalue)
-            # print(pairs)
+            try:
+                # Unzip the hidden_sigfig_data and separate into pvalue and pairs variables
+                pvalue, pairs = zip(*hidden_sigfig_data)
+                # # to troubleshoot
+                # print(pvalue)
+                # print(pairs)
+            except:
+                warnings.warn("No Significant Values. hide_ns will be set to False!")
+                if all(sigfig == "n.s." for sigfig in pvalue):
+                    hide_ns = False
 
         # To color code plots:
         subgroup_col_plot = None
         if subgroup_col is None:
             subgroup_col_plot = group_col
 
         # set orientation for plot and Annotator
@@ -1734,19 +1756,24 @@
         # If set to True, only show plots with significance
         if hide_ns is True:
             # Filter n.s. from pvalue and pairs
             hidden_sigfig_data = [
                 (item1, item2) for item1, item2 in zip(pvalue, pairs) if item1 != "n.s."
             ]
 
-            # Unzip the hidden_sigfig_data and separate into pvalue and pairs
-            pvalue, pairs = zip(*hidden_sigfig_data)
-            # # to trouble shoot
-            # print(pvalue)
-            # print(pairs)
+            try:
+                # Unzip the hidden_sigfig_data and separate into pvalue and pairs variables
+                pvalue, pairs = zip(*hidden_sigfig_data)
+                # # to troubleshoot
+                # print(pvalue)
+                # print(pairs)
+            except:
+                warnings.warn("No Significant Values. hide_ns will be set to False!")
+                if all(sigfig == "n.s." for sigfig in pvalue):
+                    hide_ns = False
 
         # To color code plots:
         subgroup_col_plot = None
         if subgroup_col is None:
             subgroup_col_plot = group_col
 
         # set orientation for plot and Annotator
@@ -1931,19 +1958,24 @@
         # If set to True, only show plots with significance
         if hide_ns is True:
             # Filter n.s. from pvalue and pairs
             hidden_sigfig_data = [
                 (item1, item2) for item1, item2 in zip(pvalue, pairs) if item1 != "n.s."
             ]
 
-            # Unzip the hidden_sigfig_data and separate into pvalue and pairs
-            pvalue, pairs = zip(*hidden_sigfig_data)
-            # # to trouble shoot
-            # print(pvalue)
-            # print(pairs)
+            try:
+                # Unzip the hidden_sigfig_data and separate into pvalue and pairs variables
+                pvalue, pairs = zip(*hidden_sigfig_data)
+                # # to troubleshoot
+                # print(pvalue)
+                # print(pairs)
+            except:
+                warnings.warn("No Significant Values. hide_ns will be set to False!")
+                if all(sigfig == "n.s." for sigfig in pvalue):
+                    hide_ns = False
 
         # set orientation for plot and Annotator
         orient = orient.lower()
         if orient == "v":
             ax = sns.boxenplot(
                 data=self.data,
                 x=group_col,
```

### Comparing `py50-1.0.3/py50/utils.py` & `py50-1.0.4/py50/utils.py`

 * *Files identical despite different names*

### Comparing `py50-1.0.3/pyproject.toml` & `py50-1.0.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py50"
-version = "1.0.3"
+version = "1.0.4"
 description = "Generate Dose-Response Curves"
 documentation = "https://py50.readthedocs.io/en/latest/"
 authors = ["Tony Eight Lin <tonyelin@tmu.edu.tw>"]
 license = "GPL-3.0"
 readme = "README_pypi.md"
 packages = [{ include = "py50"}]
```

### Comparing `py50-1.0.3/PKG-INFO` & `py50-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py50
-Version: 1.0.3
+Version: 1.0.4
 Summary: Generate Dose-Response Curves
 License: GPL-3.0
 Author: Tony Eight Lin
 Author-email: tonyelin@tmu.edu.tw
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

