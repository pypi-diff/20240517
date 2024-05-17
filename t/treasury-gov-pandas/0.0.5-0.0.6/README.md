# Comparing `tmp/treasury_gov_pandas-0.0.5.tar.gz` & `tmp/treasury_gov_pandas-0.0.6.tar.gz`

## Comparing `treasury_gov_pandas-0.0.5.tar` & `treasury_gov_pandas-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.5/src/treasury_gov_pandas/__init__.py
--rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.5/src/treasury_gov_pandas/load.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.5/src/treasury_gov_pandas/datasets/auctions_query/load.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.5/src/treasury_gov_pandas/datasets/auctions_query/update.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.5/src/treasury_gov_pandas/datasets/deposits_withdrawals_operating_cash/load.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.5/src/treasury_gov_pandas/datasets/deposits_withdrawals_operating_cash/update.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.5/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.5/LICENSE
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.5/README.md
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.6/src/treasury_gov_pandas/__init__.py
+-rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.6/src/treasury_gov_pandas/load.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.6/src/treasury_gov_pandas/datasets/auctions_query/load.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.6/src/treasury_gov_pandas/datasets/auctions_query/update.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.6/src/treasury_gov_pandas/datasets/deposits_withdrawals_operating_cash/load.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.6/src/treasury_gov_pandas/datasets/deposits_withdrawals_operating_cash/update.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.6/src/treasury_gov_pandas/datasets/mts/mts_table_4/load.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.6/src/treasury_gov_pandas/datasets/mts/mts_table_4/update.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.6/LICENSE
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.6/README.md
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.6/PKG-INFO
```

### Comparing `treasury_gov_pandas-0.0.5/src/treasury_gov_pandas/load.py` & `treasury_gov_pandas-0.0.6/src/treasury_gov_pandas/load.py`

 * *Files identical despite different names*

### Comparing `treasury_gov_pandas-0.0.5/LICENSE` & `treasury_gov_pandas-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `treasury_gov_pandas-0.0.5/pyproject.toml` & `treasury_gov_pandas-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "treasury_gov_pandas"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Eduardo Cavazos", email="wayo.cavazos@gmail.com" },
 ]
 description = "Library for downloading treasury.gov datasets."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `treasury_gov_pandas-0.0.5/PKG-INFO` & `treasury_gov_pandas-0.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: treasury_gov_pandas
-Version: 0.0.5
+Version: 0.0.6
 Summary: Library for downloading treasury.gov datasets.
 Project-URL: Homepage, https://github.com/dharmatech/treasury_gov_pandas.py
 Project-URL: Issues, https://github.com/dharmatech/treasury_gov_pandas.py/issues
 Author-email: Eduardo Cavazos <wayo.cavazos@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

