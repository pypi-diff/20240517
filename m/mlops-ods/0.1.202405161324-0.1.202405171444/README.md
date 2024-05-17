# Comparing `tmp/mlops_ods-0.1.202405161324.tar.gz` & `tmp/mlops_ods-0.1.202405171444.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlops_ods-0.1.202405161324.tar", max compression
+gzip compressed data, was "mlops_ods-0.1.202405171444.tar", max compression
```

## Comparing `mlops_ods-0.1.202405161324.tar` & `mlops_ods-0.1.202405171444.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1015 2024-05-16 13:23:42.767181 mlops_ods-0.1.202405161324/README.md
--rw-r--r--   0        0        0      944 2024-05-16 13:24:12.195270 mlops_ods-0.1.202405161324/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/app/__init__.py
--rw-r--r--   0        0        0       50 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/app/example.py
--rw-r--r--   0        0        0       69 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/conf/config.yaml
--rw-r--r--   0        0        0      287 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/conf/features/features.yaml
--rw-r--r--   0        0        0      103 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/conf/model/fast.yaml
--rw-r--r--   0        0        0      103 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/conf/model/slow.yaml
--rw-r--r--   0        0        0      146 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/conf/settings/predict.yaml
--rw-r--r--   0        0        0      183 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/conf/settings/train.yaml
--rw-r--r--   0        0        0      702 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/config.py
--rw-r--r--   0        0        0      113 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/dataset/.gitignore
--rw-r--r--   0        0        0      122 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/dataset/2015-street-tree-census-tree-data.csv.dvc
--rw-r--r--   0        0        0       21 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/dataset/features/.gitignore
--rw-r--r--   0        0        0       74 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/dataset/prepared/.gitignore
--rw-r--r--   0        0        0       11 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/dataset/processed/.gitignore
--rw-r--r--   0        0        0       47 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/dvc_functions/__init__.py
--rw-r--r--   0        0        0      127 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/dvc_functions/__main__.py
--rw-r--r--   0        0        0       50 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/dvc_functions/cli.py
--rw-r--r--   0        0        0     1845 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/dvc_functions/dvc-research.md
--rw-r--r--   0        0        0     2585 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/dvc_functions/models.py
--rw-r--r--   0        0        0      500 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/dvc_functions/preprocessing.py
--rw-r--r--   0        0        0     2013 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/dvc_functions/scaler.py
--rw-r--r--   0        0        0       49 2024-05-16 13:23:42.807181 mlops_ods-0.1.202405161324/src/mlops_ods/models/.gitignore
--rw-r--r--   0        0        0  9730898 2024-05-16 13:23:42.831181 mlops_ods-0.1.202405161324/src/mlops_ods/notebooks/eda.ipynb
--rw-r--r--   0        0        0    51114 2024-05-16 13:23:42.835181 mlops_ods-0.1.202405161324/src/mlops_ods/notebooks/model.ipynb
--rw-r--r--   0        0        0     7740 2024-05-16 13:23:42.835181 mlops_ods-0.1.202405161324/src/mlops_ods/snakemake_scripts/dag.svg
--rw-r--r--   0        0        0      647 2024-05-16 13:23:42.835181 mlops_ods-0.1.202405161324/src/mlops_ods/snakemake_scripts/model_fit.py
--rw-r--r--   0        0        0      624 2024-05-16 13:23:42.835181 mlops_ods-0.1.202405161324/src/mlops_ods/snakemake_scripts/model_fit_bigger.py
--rw-r--r--   0        0        0      268 2024-05-16 13:23:42.835181 mlops_ods-0.1.202405161324/src/mlops_ods/snakemake_scripts/preprocess_data_base.py
--rw-r--r--   0        0        0     1046 2024-05-16 13:23:42.835181 mlops_ods-0.1.202405161324/src/mlops_ods/snakemake_scripts/preprocess_data_research.py
--rw-r--r--   0        0        0      628 2024-05-16 13:23:42.835181 mlops_ods-0.1.202405161324/src/mlops_ods/snakemake_scripts/snakemake_steps.md
--rw-r--r--   0        0        0     2364 2024-05-16 13:23:42.835181 mlops_ods-0.1.202405161324/src/mlops_ods/train_predict.py
--rw-r--r--   0        0        0        0 2024-05-16 13:23:42.835181 mlops_ods-0.1.202405161324/src/mlops_ods/utils/__init__.py
--rw-r--r--   0        0        0     2262 2024-05-16 13:23:42.835181 mlops_ods-0.1.202405161324/src/mlops_ods/utils/utils_etl.py
--rw-r--r--   0        0        0     2138 2024-05-16 13:23:42.835181 mlops_ods-0.1.202405161324/src/mlops_ods/utils/utils_model.py
--rw-r--r--   0        0        0     2183 1970-01-01 00:00:00.000000 mlops_ods-0.1.202405161324/PKG-INFO
+-rw-r--r--   0        0        0     1015 2024-05-17 14:43:57.826703 mlops_ods-0.1.202405171444/README.md
+-rw-r--r--   0        0        0      968 2024-05-17 14:44:32.455098 mlops_ods-0.1.202405171444/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-17 14:43:57.862704 mlops_ods-0.1.202405171444/src/mlops_ods/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-17 14:43:57.862704 mlops_ods-0.1.202405171444/src/mlops_ods/app/__init__.py
+-rw-r--r--   0        0        0       50 2024-05-17 14:43:57.862704 mlops_ods-0.1.202405171444/src/mlops_ods/app/example.py
+-rw-r--r--   0        0        0       69 2024-05-17 14:43:57.862704 mlops_ods-0.1.202405171444/src/mlops_ods/conf/config.yaml
+-rw-r--r--   0        0        0      287 2024-05-17 14:43:57.862704 mlops_ods-0.1.202405171444/src/mlops_ods/conf/features/features.yaml
+-rw-r--r--   0        0        0      103 2024-05-17 14:43:57.862704 mlops_ods-0.1.202405171444/src/mlops_ods/conf/model/fast.yaml
+-rw-r--r--   0        0        0      103 2024-05-17 14:43:57.862704 mlops_ods-0.1.202405171444/src/mlops_ods/conf/model/slow.yaml
+-rw-r--r--   0        0        0      146 2024-05-17 14:43:57.862704 mlops_ods-0.1.202405171444/src/mlops_ods/conf/settings/predict.yaml
+-rw-r--r--   0        0        0      183 2024-05-17 14:43:57.862704 mlops_ods-0.1.202405171444/src/mlops_ods/conf/settings/train.yaml
+-rw-r--r--   0        0        0      702 2024-05-17 14:43:57.862704 mlops_ods-0.1.202405171444/src/mlops_ods/config.py
+-rw-r--r--   0        0        0      113 2024-05-17 14:43:57.862704 mlops_ods-0.1.202405171444/src/mlops_ods/dataset/.gitignore
+-rw-r--r--   0        0        0      122 2024-05-17 14:43:57.862704 mlops_ods-0.1.202405171444/src/mlops_ods/dataset/2015-street-tree-census-tree-data.csv.dvc
+-rw-r--r--   0        0        0       21 2024-05-17 14:43:57.862704 mlops_ods-0.1.202405171444/src/mlops_ods/dataset/features/.gitignore
+-rw-r--r--   0        0        0       74 2024-05-17 14:43:57.862704 mlops_ods-0.1.202405171444/src/mlops_ods/dataset/prepared/.gitignore
+-rw-r--r--   0        0        0       11 2024-05-17 14:43:57.862704 mlops_ods-0.1.202405171444/src/mlops_ods/dataset/processed/.gitignore
+-rw-r--r--   0        0        0       47 2024-05-17 14:43:57.862704 mlops_ods-0.1.202405171444/src/mlops_ods/dvc_functions/__init__.py
+-rw-r--r--   0        0        0      127 2024-05-17 14:43:57.862704 mlops_ods-0.1.202405171444/src/mlops_ods/dvc_functions/__main__.py
+-rw-r--r--   0        0        0       50 2024-05-17 14:43:57.862704 mlops_ods-0.1.202405171444/src/mlops_ods/dvc_functions/cli.py
+-rw-r--r--   0        0        0     1845 2024-05-17 14:43:57.862704 mlops_ods-0.1.202405171444/src/mlops_ods/dvc_functions/dvc-research.md
+-rw-r--r--   0        0        0     2585 2024-05-17 14:43:57.862704 mlops_ods-0.1.202405171444/src/mlops_ods/dvc_functions/models.py
+-rw-r--r--   0        0        0      500 2024-05-17 14:43:57.862704 mlops_ods-0.1.202405171444/src/mlops_ods/dvc_functions/preprocessing.py
+-rw-r--r--   0        0        0     2013 2024-05-17 14:43:57.862704 mlops_ods-0.1.202405171444/src/mlops_ods/dvc_functions/scaler.py
+-rw-r--r--   0        0        0       49 2024-05-17 14:43:57.862704 mlops_ods-0.1.202405171444/src/mlops_ods/models/.gitignore
+-rw-r--r--   0        0        0  9730898 2024-05-17 14:43:57.890704 mlops_ods-0.1.202405171444/src/mlops_ods/notebooks/eda.ipynb
+-rw-r--r--   0        0        0    51114 2024-05-17 14:43:57.890704 mlops_ods-0.1.202405171444/src/mlops_ods/notebooks/model.ipynb
+-rw-r--r--   0        0        0     7740 2024-05-17 14:43:57.890704 mlops_ods-0.1.202405171444/src/mlops_ods/snakemake_scripts/dag.svg
+-rw-r--r--   0        0        0      647 2024-05-17 14:43:57.890704 mlops_ods-0.1.202405171444/src/mlops_ods/snakemake_scripts/model_fit.py
+-rw-r--r--   0        0        0      624 2024-05-17 14:43:57.890704 mlops_ods-0.1.202405171444/src/mlops_ods/snakemake_scripts/model_fit_bigger.py
+-rw-r--r--   0        0        0      268 2024-05-17 14:43:57.890704 mlops_ods-0.1.202405171444/src/mlops_ods/snakemake_scripts/preprocess_data_base.py
+-rw-r--r--   0        0        0     1046 2024-05-17 14:43:57.890704 mlops_ods-0.1.202405171444/src/mlops_ods/snakemake_scripts/preprocess_data_research.py
+-rw-r--r--   0        0        0      628 2024-05-17 14:43:57.890704 mlops_ods-0.1.202405171444/src/mlops_ods/snakemake_scripts/snakemake_steps.md
+-rw-r--r--   0        0        0     2364 2024-05-17 14:43:57.890704 mlops_ods-0.1.202405171444/src/mlops_ods/train_predict.py
+-rw-r--r--   0        0        0        0 2024-05-17 14:43:57.890704 mlops_ods-0.1.202405171444/src/mlops_ods/utils/__init__.py
+-rw-r--r--   0        0        0     2262 2024-05-17 14:43:57.890704 mlops_ods-0.1.202405171444/src/mlops_ods/utils/utils_etl.py
+-rw-r--r--   0        0        0     2165 2024-05-17 14:43:57.890704 mlops_ods-0.1.202405171444/src/mlops_ods/utils/utils_model.py
+-rw-r--r--   0        0        0     2183 1970-01-01 00:00:00.000000 mlops_ods-0.1.202405171444/PKG-INFO
```

### Comparing `mlops_ods-0.1.202405161324/README.md` & `mlops_ods-0.1.202405171444/README.md`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405161324/pyproject.toml` & `mlops_ods-0.1.202405171444/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlops_ods"
-version = "0.1.202405161324"
+version = "0.1.202405171444"
 description = ""
 authors = ["Iuliia Fokina"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "^2.2.2"
@@ -30,14 +30,15 @@
 [tool.poetry.group.dev.dependencies]
 flake8 = "^7.0.0"
 black = "^24.3.0"
 isort = "^5.13.2"
 mypy = "^1.9.0"
 pytest = "^8.1.1"
 pre-commit = "^3.7.0"
+hypothesis = "^6.102.4"
 
 [tool.black]
 line-length = 88
 
 [tool.isort]
 profile = "black"
```

### Comparing `mlops_ods-0.1.202405161324/src/mlops_ods/config.py` & `mlops_ods-0.1.202405171444/src/mlops_ods/config.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405161324/src/mlops_ods/dvc_functions/dvc-research.md` & `mlops_ods-0.1.202405171444/src/mlops_ods/dvc_functions/dvc-research.md`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405161324/src/mlops_ods/dvc_functions/models.py` & `mlops_ods-0.1.202405171444/src/mlops_ods/dvc_functions/models.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405161324/src/mlops_ods/dvc_functions/scaler.py` & `mlops_ods-0.1.202405171444/src/mlops_ods/dvc_functions/scaler.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405161324/src/mlops_ods/notebooks/eda.ipynb` & `mlops_ods-0.1.202405171444/src/mlops_ods/notebooks/eda.ipynb`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405161324/src/mlops_ods/notebooks/model.ipynb` & `mlops_ods-0.1.202405171444/src/mlops_ods/notebooks/model.ipynb`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405161324/src/mlops_ods/snakemake_scripts/dag.svg` & `mlops_ods-0.1.202405171444/src/mlops_ods/snakemake_scripts/dag.svg`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405161324/src/mlops_ods/snakemake_scripts/model_fit.py` & `mlops_ods-0.1.202405171444/src/mlops_ods/snakemake_scripts/model_fit.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405161324/src/mlops_ods/snakemake_scripts/model_fit_bigger.py` & `mlops_ods-0.1.202405171444/src/mlops_ods/snakemake_scripts/model_fit_bigger.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405161324/src/mlops_ods/snakemake_scripts/preprocess_data_research.py` & `mlops_ods-0.1.202405171444/src/mlops_ods/snakemake_scripts/preprocess_data_research.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405161324/src/mlops_ods/snakemake_scripts/snakemake_steps.md` & `mlops_ods-0.1.202405171444/src/mlops_ods/snakemake_scripts/snakemake_steps.md`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405161324/src/mlops_ods/train_predict.py` & `mlops_ods-0.1.202405171444/src/mlops_ods/train_predict.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405161324/src/mlops_ods/utils/utils_etl.py` & `mlops_ods-0.1.202405171444/src/mlops_ods/utils/utils_etl.py`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.202405161324/src/mlops_ods/utils/utils_model.py` & `mlops_ods-0.1.202405171444/src/mlops_ods/utils/utils_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,8 +78,10 @@
         df["guards"]
         .map({"Harmful": 1, "Unsure": 2, "Helpful": 3})
         .fillna(0)
         .astype(int)
     )
     df["spc_common"] = df["spc_common"].fillna("n/d")
     df["problems"] = df["problems"].fillna("").apply(lambda x: len(x.split(",")))
-    df["health"] = df["health"].map({"Poor": 0, "Fair": 1, "Good": 2}).astype(int)
+    df["health"] = (
+        df["health"].map({"Poor": 0, "Fair": 1, "Good": 2}).fillna(-1).astype(int)
+    )
```

### Comparing `mlops_ods-0.1.202405161324/PKG-INFO` & `mlops_ods-0.1.202405171444/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlops_ods
-Version: 0.1.202405161324
+Version: 0.1.202405171444
 Summary: 
 Author: Iuliia Fokina
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

