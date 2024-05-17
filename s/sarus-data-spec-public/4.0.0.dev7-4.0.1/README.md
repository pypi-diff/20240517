# Comparing `tmp/sarus_data_spec_public-4.0.0.dev7.tar.gz` & `tmp/sarus_data_spec_public-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus_data_spec_public-4.0.0.dev7.tar", last modified: Sat May 11 22:39:24 2024, max compression
+gzip compressed data, was "sarus_data_spec_public-4.0.1.tar", last modified: Fri May 17 15:57:11 2024, max compression
```

## Comparing `sarus_data_spec_public-4.0.0.dev7.tar` & `sarus_data_spec_public-4.0.1.tar`

### file list

```diff
@@ -1,223 +1,224 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.153491 sarus_data_spec_public-4.0.0.dev7/
--rw-rw-rw-   0 root         (0) root         (0)      139 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      661 2024-05-11 22:39:24.153491 sarus_data_spec_public-4.0.0.dev7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      134 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.110487 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/
--rwxrwxrwx   0 root         (0) root         (0)      947 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.112487 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/arrow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/arrow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8845 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/arrow/admin_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2178 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/arrow/array.py
--rw-rw-rw-   0 root         (0) root         (0)     7304 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/arrow/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)     2100 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/arrow/pandas_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6266 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/arrow/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    10718 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/arrow/type.py
--rw-rw-rw-   0 root         (0) root         (0)     1014 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/attribute.py
--rw-rw-rw-   0 root         (0) root         (0)     4646 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1488 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/bounds.py
--rw-rw-rw-   0 root         (0) root         (0)     4185 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.113488 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/context/
--rw-rw-rw-   0 root         (0) root         (0)      266 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/context/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/context/public.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/context/state.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/context/typing.py
--rw-rw-rw-   0 root         (0) root         (0)    21741 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.115488 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2314 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4997 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/graph_query_builder_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    22994 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/recursive_rewriter.py
--rw-rw-rw-   0 root         (0) root         (0)    11623 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)      837 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3438 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.116488 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17255 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3941 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/parameter_kind.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/privacy_limit.py
--rw-rw-rw-   0 root         (0) root         (0)     5717 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/recursive_validator.py
--rw-rw-rw-   0 root         (0) root         (0)    28906 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/signature.py
--rw-rw-rw-   0 root         (0) root         (0)     4161 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)     5355 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     8867 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/deprecation.py
--rw-rw-rw-   0 root         (0) root         (0)     1584 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     8679 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/json_serialisation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.118488 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7629 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/async_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    32029 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/base.py
--rw-rw-rw-   0 root         (0) root         (0)     6724 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/cache_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.118488 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9104 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.119488 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/local/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/local/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3892 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/local/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2583 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/local/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.119488 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/remote/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/remote/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3302 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/remote/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.120488 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/
--rw-rw-rw-   0 root         (0) root         (0)      173 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7120 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.120488 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.123489 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/
--rw-rw-rw-   0 root         (0) root         (0)     2662 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23081 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/external_op.py
--rw-rw-rw-   0 root         (0) root         (0)     3011 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/imblearn.py
--rw-rw-rw-   0 root         (0) root         (0)    10321 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/numpy.py
--rw-rw-rw-   0 root         (0) root         (0)    21505 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/optbinning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.125489 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/pandas/
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8155 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py
--rw-rw-rw-   0 root         (0) root         (0)    32015 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/pandas/groupby_dp.py
--rw-rw-rw-   0 root         (0) root         (0)    78764 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
--rw-rw-rw-   0 root         (0) root         (0)    37673 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
--rw-rw-rw-   0 root         (0) root         (0)     2807 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
--rw-rw-rw-   0 root         (0) root         (0)    34976 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/scipy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.127489 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/shap/
--rw-rw-rw-   0 root         (0) root         (0)     4162 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/shap/Explanation.py
--rw-rw-rw-   0 root         (0) root         (0)      132 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/shap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26932 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/shap/explainer.py
--rw-rw-rw-   0 root         (0) root         (0)    13453 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/shap/maskers.py
--rw-rw-rw-   0 root         (0) root         (0)    14139 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/shap/plots.py
--rw-rw-rw-   0 root         (0) root         (0)     6514 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/shap/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.130489 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/
--rw-rw-rw-   0 root         (0) root         (0)      335 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20941 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py
--rw-rw-rw-   0 root         (0) root         (0)     1931 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py
--rw-rw-rw-   0 root         (0) root         (0)     1902 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py
--rw-rw-rw-   0 root         (0) root         (0)    38069 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py
--rw-rw-rw-   0 root         (0) root         (0)     1678 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py
--rw-rw-rw-   0 root         (0) root         (0)     2084 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py
--rw-rw-rw-   0 root         (0) root         (0)     9874 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py
--rw-rw-rw-   0 root         (0) root         (0)     3294 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py
--rw-rw-rw-   0 root         (0) root         (0)    12690 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     8598 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     4340 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)     2645 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py
--rw-rw-rw-   0 root         (0) root         (0)     2884 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/skopt.py
--rw-rw-rw-   0 root         (0) root         (0)    25448 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/std.py
--rw-rw-rw-   0 root         (0) root         (0)     3011 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    14158 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/xgboost.py
--rw-rw-rw-   0 root         (0) root         (0)    13076 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/routing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.134489 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17193 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
--rw-rw-rw-   0 root         (0) root         (0)     1625 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/error_estimation.py
--rw-rw-rw-   0 root         (0) root         (0)     1474 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/extract.py
--rw-rw-rw-   0 root         (0) root         (0)    12256 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/filter.py
--rw-rw-rw-   0 root         (0) root         (0)     2922 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/generate_from_model.py
--rw-rw-rw-   0 root         (0) root         (0)    12893 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/get_item.py
--rw-rw-rw-   0 root         (0) root         (0)    11420 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/project.py
--rw-rw-rw-   0 root         (0) root         (0)     8567 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.134489 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/sampling/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/sampling/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3647 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/sampling/differentiated_sampling_sizes.py
--rw-rw-rw-   0 root         (0) root         (0)     2462 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/shuffle.py
--rw-rw-rw-   0 root         (0) root         (0)     9522 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/standard_op.py
--rw-rw-rw-   0 root         (0) root         (0)    11403 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/synthetic.py
--rw-rw-rw-   0 root         (0) root         (0)    13558 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/to_small_data.py
--rw-rw-rw-   0 root         (0) root         (0)    27871 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.135490 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/source/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/source/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/source/privacy_params.py
--rw-rw-rw-   0 root         (0) root         (0)      269 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/source/random_seed.py
--rw-rw-rw-   0 root         (0) root         (0)     3320 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/source/routing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.136490 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/sql_utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/sql_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8893 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/sql_utils/bigdata.py
--rw-rw-rw-   0 root         (0) root         (0)     5703 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/sql_utils/queries.py
--rw-rw-rw-   0 root         (0) root         (0)    10377 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/marginals.py
--rw-rw-rw-   0 root         (0) root         (0)     1548 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/multiplicity.py
--rw-rw-rw-   0 root         (0) root         (0)     3376 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/path.py
--rw-rw-rw-   0 root         (0) root         (0)     3004 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/predicate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.150491 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/
--rw-rw-rw-   0 root         (0) root         (0)     2628 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/attribute.proto
--rw-r--r--   0 root         (0) root         (0)     1507 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/attribute_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1840 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/attribute_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      251 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/bounds.proto
--rw-r--r--   0 root         (0) root         (0)     1712 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/bounds_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2160 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/bounds_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      348 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/constraint.proto
--rw-r--r--   0 root         (0) root         (0)     1964 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/constraint_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3236 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/constraint_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1340 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/dataset.proto
--rw-r--r--   0 root         (0) root         (0)     3941 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/dataset_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9653 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/dataset_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      470 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/links.proto
--rw-r--r--   0 root         (0) root         (0)     2557 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/links_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4178 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/links_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      244 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/manager.proto
--rw-r--r--   0 root         (0) root         (0)     1417 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/manager_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1638 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/manager_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      254 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/marginals.proto
--rw-r--r--   0 root         (0) root         (0)     1739 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/marginals_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2169 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/marginals_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      257 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/multiplicity.proto
--rw-r--r--   0 root         (0) root         (0)     1777 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/multiplicity_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2178 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/multiplicity_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/path.proto
--rw-r--r--   0 root         (0) root         (0)     1449 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/path_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/path_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/predicate.proto
--rw-r--r--   0 root         (0) root         (0)     2416 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/predicate_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4839 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/predicate_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      259 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/proto_container.proto
--rw-r--r--   0 root         (0) root         (0)     1634 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/proto_container_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1821 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/proto_container_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      629 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/relation.proto
--rw-r--r--   0 root         (0) root         (0)     1545 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/relation_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2606 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/relation_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1798 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/scalar.proto
--rw-r--r--   0 root         (0) root         (0)     3904 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/scalar_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9843 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/scalar_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      694 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/schema.proto
--rw-r--r--   0 root         (0) root         (0)     2611 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/schema_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4578 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/schema_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      249 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/size.proto
--rw-r--r--   0 root         (0) root         (0)     1689 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/size_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2154 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/size_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3909 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/statistics.proto
--rw-r--r--   0 root         (0) root         (0)    11222 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/statistics_pb2.py
--rw-r--r--   0 root         (0) root         (0)    32747 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/statistics_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      646 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/status.proto
--rw-r--r--   0 root         (0) root         (0)     3258 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6181 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/status_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     6970 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/transform.proto
--rw-r--r--   0 root         (0) root         (0)    16759 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/transform_pb2.py
--rw-r--r--   0 root         (0) root         (0)    48797 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/transform_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     4567 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/type.proto
--rw-r--r--   0 root         (0) root         (0)     9784 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/type_pb2.py
--rw-r--r--   0 root         (0) root         (0)    30590 2024-05-11 22:39:12.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/type_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      917 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3948 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/utilities.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    13753 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/scalar.py
--rw-rw-rw-   0 root         (0) root         (0)     4757 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1467 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/size.py
--rw-rw-rw-   0 root         (0) root         (0)    43603 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/statistics.py
--rw-rw-rw-   0 root         (0) root         (0)    17261 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.151491 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/storage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14527 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/storage/local.py
--rw-rw-rw-   0 root         (0) root         (0)     5606 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/storage/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3084 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/storage/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    40022 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/transform.py
--rw-rw-rw-   0 root         (0) root         (0)   123297 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/type.py
--rw-rw-rw-   0 root         (0) root         (0)    40869 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     4998 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/variant_constraint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 22:39:24.153491 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec_public.egg-info/
--rw-r--r--   0 root         (0) root         (0)      661 2024-05-11 22:39:24.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec_public.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9090 2024-05-11 22:39:24.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec_public.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 22:39:24.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec_public.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 22:39:24.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec_public.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      125 2024-05-11 22:39:24.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec_public.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-11 22:39:24.000000 sarus_data_spec_public-4.0.0.dev7/sarus_data_spec_public.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     6927 2024-05-11 22:39:24.154491 sarus_data_spec_public-4.0.0.dev7/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1191 2024-05-11 22:38:46.000000 sarus_data_spec_public-4.0.0.dev7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.683242 sarus_data_spec_public-4.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)      139 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      656 2024-05-17 15:57:11.683242 sarus_data_spec_public-4.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      134 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.641242 sarus_data_spec_public-4.0.1/sarus_data_spec/
+-rwxrwxrwx   0 root         (0) root         (0)      942 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.642242 sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8510 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/admin_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2354 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/array.py
+-rw-rw-rw-   0 root         (0) root         (0)     7389 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)     2100 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/pandas_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6266 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    10718 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1014 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)     4646 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/bounds.py
+-rw-rw-rw-   0 root         (0) root         (0)     4266 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.643242 sarus_data_spec_public-4.0.1/sarus_data_spec/context/
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/context/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/context/public.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/context/state.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/context/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)    21819 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.645242 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2314 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4997 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/graph_query_builder_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    22994 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/recursive_rewriter.py
+-rw-rw-rw-   0 root         (0) root         (0)    11623 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)      837 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3438 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.647242 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17255 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3941 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/parameter_kind.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/privacy_limit.py
+-rw-rw-rw-   0 root         (0) root         (0)     5717 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/recursive_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)    28910 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/signature.py
+-rw-rw-rw-   0 root         (0) root         (0)     4161 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     5355 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     8867 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/deprecation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     8679 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/json_serialisation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.648242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7629 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/async_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    32667 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6724 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/cache_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.649242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9104 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.649242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/local/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3892 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/local/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2583 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/local/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.650242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/remote/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/remote/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3302 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/remote/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.650242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7120 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.651242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.654242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/
+-rw-rw-rw-   0 root         (0) root         (0)     2662 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23600 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/external_op.py
+-rw-rw-rw-   0 root         (0) root         (0)     3011 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/imblearn.py
+-rw-rw-rw-   0 root         (0) root         (0)    10321 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/numpy.py
+-rw-rw-rw-   0 root         (0) root         (0)    21505 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/optbinning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.655242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8155 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py
+-rw-rw-rw-   0 root         (0) root         (0)    31872 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/pandas/groupby_dp.py
+-rw-rw-rw-   0 root         (0) root         (0)    78764 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
+-rw-rw-rw-   0 root         (0) root         (0)    37561 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2807 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
+-rw-rw-rw-   0 root         (0) root         (0)    34976 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/scipy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.657242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/shap/
+-rw-rw-rw-   0 root         (0) root         (0)     4162 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/shap/Explanation.py
+-rw-rw-rw-   0 root         (0) root         (0)      132 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/shap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26932 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/shap/explainer.py
+-rw-rw-rw-   0 root         (0) root         (0)    13453 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/shap/maskers.py
+-rw-rw-rw-   0 root         (0) root         (0)    14139 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/shap/plots.py
+-rw-rw-rw-   0 root         (0) root         (0)     6514 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/shap/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.660242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20941 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py
+-rw-rw-rw-   0 root         (0) root         (0)     1931 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py
+-rw-rw-rw-   0 root         (0) root         (0)    38069 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py
+-rw-rw-rw-   0 root         (0) root         (0)     1678 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2084 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py
+-rw-rw-rw-   0 root         (0) root         (0)     9874 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     3294 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    12690 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     8598 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     4340 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2645 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2884 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/skopt.py
+-rw-rw-rw-   0 root         (0) root         (0)    25448 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/std.py
+-rw-rw-rw-   0 root         (0) root         (0)     3011 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    14158 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/xgboost.py
+-rw-rw-rw-   0 root         (0) root         (0)    13273 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/routing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.664242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17193 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
+-rw-rw-rw-   0 root         (0) root         (0)     1625 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/error_estimation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1474 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/extract.py
+-rw-rw-rw-   0 root         (0) root         (0)    12256 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2922 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/generate_from_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    13308 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/get_item.py
+-rw-rw-rw-   0 root         (0) root         (0)    11420 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/push_sql.py
+-rw-rw-rw-   0 root         (0) root         (0)     8639 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.664242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/sampling/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/sampling/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3647 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/sampling/differentiated_sampling_sizes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2462 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/shuffle.py
+-rw-rw-rw-   0 root         (0) root         (0)     9522 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/standard_op.py
+-rw-rw-rw-   0 root         (0) root         (0)    11403 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/synthetic.py
+-rw-rw-rw-   0 root         (0) root         (0)    13558 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/to_small_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    27871 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.665242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/source/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/source/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/source/privacy_params.py
+-rw-rw-rw-   0 root         (0) root         (0)      269 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/source/random_seed.py
+-rw-rw-rw-   0 root         (0) root         (0)     3320 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/source/routing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.666242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/sql_utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/sql_utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8985 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/sql_utils/bigdata.py
+-rw-rw-rw-   0 root         (0) root         (0)     5703 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/sql_utils/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)    10574 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/marginals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/multiplicity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3376 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/path.py
+-rw-rw-rw-   0 root         (0) root         (0)     3004 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/predicate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.680242 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/
+-rw-rw-rw-   0 root         (0) root         (0)     2628 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/attribute.proto
+-rw-r--r--   0 root         (0) root         (0)     1507 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/attribute_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/attribute_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      251 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/bounds.proto
+-rw-r--r--   0 root         (0) root         (0)     1712 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/bounds_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2160 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/bounds_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      348 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/constraint.proto
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/constraint_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3236 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/constraint_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1340 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/dataset.proto
+-rw-r--r--   0 root         (0) root         (0)     3941 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/dataset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9653 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/dataset_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      470 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/links.proto
+-rw-r--r--   0 root         (0) root         (0)     2557 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/links_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4178 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/links_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      244 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/manager.proto
+-rw-r--r--   0 root         (0) root         (0)     1417 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/manager_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1638 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/manager_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      254 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/marginals.proto
+-rw-r--r--   0 root         (0) root         (0)     1739 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/marginals_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2169 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/marginals_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      257 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/multiplicity.proto
+-rw-r--r--   0 root         (0) root         (0)     1777 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/multiplicity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/multiplicity_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/path.proto
+-rw-r--r--   0 root         (0) root         (0)     1449 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/path_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/path_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/predicate.proto
+-rw-r--r--   0 root         (0) root         (0)     2416 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/predicate_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4839 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/predicate_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      259 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/proto_container.proto
+-rw-r--r--   0 root         (0) root         (0)     1634 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/proto_container_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1821 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/proto_container_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      629 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/relation.proto
+-rw-r--r--   0 root         (0) root         (0)     1545 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/relation_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2606 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/relation_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1798 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/scalar.proto
+-rw-r--r--   0 root         (0) root         (0)     3904 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/scalar_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9843 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/scalar_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      694 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/schema.proto
+-rw-r--r--   0 root         (0) root         (0)     2611 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/schema_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/schema_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      249 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/size.proto
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/size_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2154 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/size_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3909 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/statistics.proto
+-rw-r--r--   0 root         (0) root         (0)    11222 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/statistics_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    32747 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/statistics_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      646 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/status.proto
+-rw-r--r--   0 root         (0) root         (0)     3258 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6181 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/status_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     7135 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/transform.proto
+-rw-r--r--   0 root         (0) root         (0)    17096 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/transform_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    49955 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/transform_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     4567 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/type.proto
+-rw-r--r--   0 root         (0) root         (0)     9784 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/type_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    30590 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/type_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      917 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3948 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/utilities.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    13753 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/scalar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4757 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1467 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/size.py
+-rw-rw-rw-   0 root         (0) root         (0)    43603 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/statistics.py
+-rw-rw-rw-   0 root         (0) root         (0)    17261 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.681242 sarus_data_spec_public-4.0.1/sarus_data_spec/storage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14527 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/storage/local.py
+-rw-rw-rw-   0 root         (0) root         (0)     5606 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/storage/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3084 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/storage/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    40753 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/transform.py
+-rw-rw-rw-   0 root         (0) root         (0)   123255 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/type.py
+-rw-rw-rw-   0 root         (0) root         (0)    40943 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     4998 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/variant_constraint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.683242 sarus_data_spec_public-4.0.1/sarus_data_spec_public.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      656 2024-05-17 15:57:11.000000 sarus_data_spec_public-4.0.1/sarus_data_spec_public.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9149 2024-05-17 15:57:11.000000 sarus_data_spec_public-4.0.1/sarus_data_spec_public.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 15:57:11.000000 sarus_data_spec_public-4.0.1/sarus_data_spec_public.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 15:57:11.000000 sarus_data_spec_public-4.0.1/sarus_data_spec_public.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      125 2024-05-17 15:57:11.000000 sarus_data_spec_public-4.0.1/sarus_data_spec_public.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-17 15:57:11.000000 sarus_data_spec_public-4.0.1/sarus_data_spec_public.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     6984 2024-05-17 15:57:11.685242 sarus_data_spec_public-4.0.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1186 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/setup.py
```

### Comparing `sarus_data_spec_public-4.0.0.dev7/PKG-INFO` & `sarus_data_spec_public-4.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus_data_spec_public
-Version: 4.0.0.dev7
+Version: 4.0.1
 Summary: A library to manage Sarus datasets
 Home-page: 
 Download-URL: 
 Author: Sarus Technologies
 Author-email: 
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/__init__.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "VariantConstraint",
 ]
 
 """A library to manage Sarus datasets"""
 # pylint: disable=unused-variable
 
 PACKAGE_NAME: Final[str] = "sarus_data_spec"
-VERSION: Final[str] = "4.0.0.dev7"
+VERSION: Final[str] = "4.0.1"
 
 try:
     import sarus_data_spec.context.worker as sw
 
     push_global_context(sw.WorkerContext())
 except ModuleNotFoundError as exception:
     if exception.name == "sarus_data_spec.context.worker":
```

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/arrow/admin_utils.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/admin_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import typing as t
 
 import pandas as pd
 import pyarrow as pa
 
-from sarus_data_spec.arrow.array import fit_array_to_schema_type_async_gen
 from sarus_data_spec.arrow.pandas_utils import (
     convert_pandas_metadata_to_admin_columns,
     pandas_index_columns,
     remove_pandas_index_columns,
 )
 from sarus_data_spec.constants import DATA, PU_COLUMN, PUBLIC, WEIGHTS
 import sarus_data_spec.typing as st
@@ -15,15 +14,15 @@
 
 async def async_to_arrow_extract_admin(
     dataset: st.Dataset, batch_size: int = 10000
 ) -> t.Optional[t.AsyncIterator[pa.RecordBatch]]:
     """This function return an async iterator record batches of the
     admin data if there is administrative columns.
     """
-    # TODO: Why not all admin columns?
+
     schema = await dataset.async_schema()
     if not schema.has_admin_columns():
         return None
 
     # Extract admin data from DATA
     batches_async_it = await dataset.async_to_arrow(batch_size)
     pe_field_names = [PUBLIC, PU_COLUMN, WEIGHTS]
@@ -49,25 +48,20 @@
 
 async def async_to_arrow_extract_data_only(
     dataset: st.Dataset, batch_size: int = 10000
 ) -> t.AsyncIterator[pa.RecordBatch]:
     """This function return an async iterator of record batches.
 
     The RecordBatches contain the data only, without the admin columns.
-    Index columns are admin columns
     """
     batches_async_it = await dataset.async_to_arrow(batch_size)
     schema = await dataset.async_schema()
 
-    valid_batches_async_it = fit_array_to_schema_type_async_gen(
-        batches_async_it, schema.type()
-    )
-
     if not schema.has_admin_columns():
-        return valid_batches_async_it
+        return batches_async_it
 
     # Extract PE from DATA
     data_cols = list(schema.type().data_type().children().keys())
 
     async def extract_data(
         batches_async_it: t.AsyncIterator[pa.RecordBatch],
     ) -> t.AsyncIterator[pa.RecordBatch]:
@@ -97,30 +91,28 @@
             new_struct_array = pa.StructArray.from_arrays(arrays, names)
             data_batch = pa.RecordBatch.from_struct_array(new_struct_array)
             data_batch = data_batch.replace_schema_metadata(
                 batch.schema.metadata
             )
             yield data_batch
 
-    return extract_data(valid_batches_async_it)
+    return extract_data(batches_async_it)
 
 
 async def async_admin_data(dataset: st.Dataset) -> t.Optional[pa.Table]:
     """Return the privacy unit as a pa.Table if it exists."""
     pe_batches_async_it = await async_to_arrow_extract_admin(dataset)
     if pe_batches_async_it is None:
         return None
     pe_batches = [batch async for batch in pe_batches_async_it]
     return pa.Table.from_batches(pe_batches)
 
 
 def merge_schemas_metadata(schema1: pa.Schema, schema2: pa.Schema) -> dict:
     """Merge metadata from two PyArrow schemas."""
-    # TODO: if both schemas have the same metadata e.g. pandas: {..}
-    # the final merged_metadata will contain the metadata of schema2 only
     metadata1 = schema1.metadata or {}
     metadata2 = schema2.metadata or {}
 
     # Combine metadata from both schemas
     merged_metadata = {**metadata1, **metadata2}
 
     return merged_metadata
@@ -136,14 +128,16 @@
     """
     if admin_data is None:
         # TODO also wrap the data in an empty protection
         return data
 
     data_index_columns = pandas_index_columns(data.schema)
     if len(data_index_columns) > 0:
+        # There are some pandas metadata
+        assert data_index_columns == pandas_index_columns(admin_data.schema)
         data = remove_pandas_index_columns(data)
 
     merged_metadata = merge_schemas_metadata(data.schema, admin_data.schema)
 
     # We merge the privacy unit and data in Pyarrow
     data_arrays = [
         chunked_array.combine_chunks() for chunked_array in data.columns
@@ -163,16 +157,15 @@
     # We guarantee that the data.index is a reliable way to trace how
     # the rows were rearranged using PyArrow's  internal implementation
     # See: https://arrow.apache.org/docs/python/pandas.html#handling-pandas-indexes
 
     if type(result) == pd.DataFrame:
         df = t.cast(pd.DataFrame, result)
         input_pe_df = input_admin_data.to_pandas()
-        filtered = input_pe_df.loc[df.index]
-        output_admin_data = pa.Table.from_pandas(filtered)
+        output_admin_data = pa.Table.from_pandas(input_pe_df.loc[df.index])
     elif type(result) == pd.Series:
         sr = t.cast(pd.Series, result)
         input_pe_df = input_admin_data.to_pandas()
         output_admin_data = pa.Table.from_pandas(input_pe_df.loc[sr.index])
     elif type(result) == pd.core.groupby.DataFrameGroupBy:
         df_grouped_by = t.cast(pd.core.groupby.DataFrameGroupBy, result)
         combined_df = df_grouped_by.obj
@@ -203,39 +196,39 @@
             i = output_admin_data.schema.get_field_index(col)
             column = output_admin_data.column(col).cast(field.type)
             output_admin_data = output_admin_data.set_column(i, field, column)
 
     return output_admin_data
 
 
-def validate_admin_data(
+def validate_privacy_unit(
     admin_data: t.List[pa.Table],
 ) -> pa.Table:
-    """Check that admin_data (tables with administrative columns) have the
-    the same PUs and same weights."""
+    """Check privacy unit related administrative data are equal across several
+    tables."""
     if len(admin_data) == 0:
         raise ValueError("The list of input admin data is empty.")
 
-    pe = next(iter(admin_data), None)
-    if pe is None:
+    pu = next(iter(admin_data), None)
+    if pu is None:
         raise ValueError(
             "The dataset was infered PUP but has no input admin data"
         )
 
-    cols_to_check = [PU_COLUMN, WEIGHTS]
+    cols_to_check = [PU_COLUMN, WEIGHTS, PUBLIC]
 
     if not all(
         [
-            candidate.select(cols_to_check).equals(pe.select(cols_to_check))
+            candidate.select(cols_to_check).equals(pu.select(cols_to_check))
             for candidate in admin_data
         ]
     ):
         raise ValueError(
             "The dataset is PUP but has several differing input admin "
             "data values"
         )
-    return pe
+    return pu
 
 
 def create_admin_columns(table: pa.Table) -> pa.Table:
     """Isolate special columns to admin columns."""
     return convert_pandas_metadata_to_admin_columns(table)
```

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/arrow/array.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/array.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,26 +26,31 @@
     """
     async for batch in batch_async_iterator:
         if schema_type.has_admin_columns():
             assert DATA in batch.schema.names
 
         # retrieve pandas index that may not be present in the schema type
         field_names = list(batch.schema.names)
-        index_cols = pandas_index_columns(batch.schema)
-        index_arrays = [
-            batch.columns[field_names.index(col)] for col in index_cols
-        ]
 
-        # select columns present in the schema type
+        # select columns present in the schema type.
+        # it fails if columns in the schema are not in the array
         updated_array = select_columns(
             schema_type,
             convert_record_batch(record_batch=batch, _type=schema_type),
         )
         updated_batch = pa.RecordBatch.from_struct_array(updated_array)
 
+        index_cols = [
+            col
+            for col in pandas_index_columns(batch.schema)
+            if col not in list(updated_batch.schema.names)
+        ]
+        index_arrays = [
+            batch.columns[field_names.index(col)] for col in index_cols
+        ]
         if len(index_cols) > 0:
             # add index cols
             updated_field_names = list(updated_batch.schema.names)
             arrays = index_arrays + updated_batch.columns
             names = index_cols + updated_field_names
             new_struct_array = pa.StructArray.from_arrays(arrays, names)
             updated_batch = pa.RecordBatch.from_struct_array(new_struct_array)
```

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/arrow/conversion.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 async def async_cast_arrow_batches(
     batches_async_iterator: t.AsyncIterator[pa.RecordBatch],
     kind: st.DatasetCastable,
 ) -> st.DatasetCastable:
     """Convert an async record batches iterator to another Python type."""
     if kind not in t.get_args(st.DatasetCastable):
         raise TypeError(f"Cannot cast a Dataset to type {kind}")
-
+    if kind == t.AsyncIterator[pa.RecordBatch]:
+        return batches_async_iterator
     if kind == t.Iterator[pa.RecordBatch]:
         return sync_iterator_from_async_iterator(batches_async_iterator)
     if kind == pd.DataFrame:
         return await async_arrow_batches_to_dataframe(batches_async_iterator)
     elif kind == pd.Series:
         return await async_arrow_batches_to_series(batches_async_iterator)
     elif kind == pd.core.groupby.DataFrameGroupBy:
```

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/arrow/pandas_utils.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/arrow/schema.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/arrow/type.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/type.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/attribute.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/attribute.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/base.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/bounds.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/bounds.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/constants.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,25 +51,27 @@
 DATETIME_MONTH = "month"
 DATETIME_DAY = "day"
 DATETIME_HOUR = "hour"
 DATETIME_MINUTES = "minutes"
 DATETIME_SECONDS = "seconds"
 
 
-# sql, to_sql status
+# sql, to_sql, push_sql status
 TO_SQL_TASK = "sql_preparation"
 SQL_TASK = "sql"
+PUSH_SQL_TASK = "push_sql"
 
 # Big Data Status
 BIG_DATA_TASK = "big_data_dataset"
 BIG_DATA_THRESHOLD = "threshold"
 IS_BIG_DATA = "is_big_data"
 DATASET_N_LINES = "dataset_n_lines"
 DATASET_N_BYTES = "dataset_n_bytes"
 THRESHOLD_TYPE = "threshold_type"
+SAMPLE_SIZE_N_LINES = "sample_size_n_lines"
 
 # Caching Status
 TO_PARQUET_TASK = "to_parquet"
 CACHE = TO_PARQUET_TASK
 CACHE_PATH = "path"
 COMPUTATION_QUEUED = "computation_queued"
 TO_SQL_CACHING_TASK = "to_sql_caching"
```

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/context/public.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/context/public.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/context/typing.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/context/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataset.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,14 +230,17 @@
         self, batch_size: int = 10000
     ) -> AsyncIterator[pa.RecordBatch]:
         return await self.manager().async_to_arrow(self, batch_size)
 
     def to_sql(self) -> None:
         return self.manager().to_sql(self)
 
+    def push_sql(self) -> None:
+        return self.manager().push_sql(self)
+
     def parents(
         self,
     ) -> Tuple[
         List[Union[st.DataSpec, st.Transform]],
         Dict[str, Union[st.DataSpec, st.Transform]],
     ]:
         if not self.is_transformed():
```

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/base.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/graph_query_builder_utils.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/graph_query_builder_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/recursive_rewriter.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/recursive_rewriter.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/simple_rules.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/simple_rules.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/typing.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_rewriter/utils.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/base.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/parameter_kind.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/parameter_kind.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/privacy_limit.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/privacy_limit.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/recursive_validator.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/recursive_validator.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/signature.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/signature.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import time
 import typing as t
 
 import pyarrow as pa
 
 from sarus_data_spec.arrow.admin_utils import (
     async_admin_data,
-    validate_admin_data,
+    validate_privacy_unit,
 )
 from sarus_data_spec.dataspec_validator.parameter_kind import (
     DATASET,
     DATASPEC,
     PUP_DATASET,
     SCALAR,
     STATIC,
@@ -704,15 +704,15 @@
         ]
         if len(admin_data) == 0:
             raise ValueError(
                 "The list of input admin data is empty "
                 f"among arguments {self.arguments}"
             )
 
-        return validate_admin_data(admin_data)
+        return validate_privacy_unit(admin_data)
 
     def callable(
         self,
     ) -> t.Callable[..., SarusSignatureValue]:
         """Returns a callable that will compute the signature's value given
         variables' values."""
         # Build callables here
```

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/simple_rules.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/simple_rules.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/dataspec_validator/typing.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/deprecation.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/deprecation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/factory.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/factory.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/json_serialisation.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/json_serialisation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/async_utils.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/async_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/base.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     BIG_DATA_TASK,
     BIG_DATA_THRESHOLD,
     DATASET_N_BYTES,
     DATASET_N_LINES,
     IS_BIG_DATA,
     IS_REMOTE,
     THRESHOLD_TYPE,
+    SAMPLE_SIZE_N_LINES,
 )
 from sarus_data_spec.dataspec_rewriter.recursive_rewriter import (
     RecursiveDataspecRewriter,
 )
 from sarus_data_spec.dataspec_validator.recursive_validator import (
     RecursiveDataspecValidator,
 )
@@ -323,21 +324,25 @@
                     status = stt.last_status(
                         dataspec=ds_args[0], task=BIG_DATA_TASK
                     )
                 assert status
                 big_data_threshold = int(
                     status.task(BIG_DATA_TASK).properties()[BIG_DATA_THRESHOLD]  # type:ignore
                 )
+                sample_size_n_lines = status.task(BIG_DATA_TASK).properties()[  # type:ignore
+                    SAMPLE_SIZE_N_LINES
+                ]
                 # write status
                 stt.ready(
                     dataset,
                     task=BIG_DATA_TASK,
                     properties={
                         IS_BIG_DATA: str(is_big_data),
                         BIG_DATA_THRESHOLD: str(big_data_threshold),
+                        SAMPLE_SIZE_N_LINES: str(sample_size_n_lines),
                         DATASET_N_LINES: str(number_lines),
                         DATASET_N_BYTES: str(number_bytes),
                         THRESHOLD_TYPE: threshold_kind,
                     },
                 )
                 return is_big_data
 
@@ -367,15 +372,15 @@
         raise NotImplementedError
 
     # -------CACHING POLICY/UTILS ----
 
     def is_cached(self, dataspec: st.DataSpec) -> bool:
         raise NotImplementedError
 
-    def is_pushed_to_sql(self, dataspec: st.DataSpec) -> bool:
+    def is_cached_to_sql(self, dataspec: st.DataSpec) -> bool:
         raise NotImplementedError
 
     def parquet_dir(self) -> str:
         return self._parquet_dir
 
     def sql_pushing_schema_prefix(self, dataset: st.Dataset) -> str:
         raise NotImplementedError
@@ -445,48 +450,58 @@
 
     def to_parquet(self, dataset: st.Dataset) -> None:
         sync(self.async_to_parquet(dataset=dataset))
 
     def to_sql(self, dataset: st.Dataset) -> None:
         sync(self.async_to_sql(dataset=dataset))
 
+    def push_sql(self, dataset: st.Dataset) -> None:
+        sync(self.async_push_sql(dataset=dataset))
+
     def to_tensorflow(self, dataset: st.Dataset) -> tf.data.Dataset:
         return sync(self.async_to_tensorflow(dataset=dataset))
 
     def value(self, scalar: st.Scalar) -> st.DataSpecValue:
         return sync(self.async_value(scalar=scalar))
 
     def composed_callable(
         self, transform: st.Transform
     ) -> t.Callable[..., t.Any]:
         implementation = get_implementation(transform.transform_to_apply())
         return implementation.callable(transform)
 
     # ------ASYNC COMPUTATIONS--------
     async def async_to(
-        self, dataset: st.Dataset, kind: t.Type, drop_admin: bool = True
+        self,
+        dataset: st.Dataset,
+        kind: t.Type,
+        drop_admin: bool = True,
+        batch_size: t.Optional[int] = None,
     ) -> st.DatasetCastable:
         """Convert a Dataset's to a Python type."""
+        if batch_size is None:
+            batch_size = BATCH_SIZE
         if drop_admin:
             batches_async_it = await async_to_arrow_extract_data_only(
-                dataset=dataset, batch_size=BATCH_SIZE
+                dataset=dataset, batch_size=batch_size
             )
         else:
             if kind not in [
                 pd.DataFrame,
                 t.Iterator[pa.RecordBatch],
+                t.AsyncIterator[pa.RecordBatch],
                 pd.core.groupby.DataFrameGroupBy,
                 pd.core.groupby.SeriesGroupBy,
             ]:
                 raise TypeError(
                     f"The target type {kind} is not compatible"
                     " with the protection."
                 )
             batches_async_it = await dataset.async_to_arrow(
-                batch_size=BATCH_SIZE
+                batch_size=batch_size
             )
 
         return await async_cast_arrow_batches(batches_async_it, kind)
 
     async def async_bounds(self, dataset: st.Dataset) -> st.Bounds:
         raise NotImplementedError
 
@@ -745,14 +760,17 @@
 
     async def async_schema_op(self, dataset: st.Dataset) -> st.Schema:
         raise NotImplementedError
 
     async def async_to_sql(self, dataset: st.Dataset) -> None:
         raise NotImplementedError
 
+    async def async_push_sql(self, dataset: st.Dataset) -> None:
+        raise NotImplementedError
+
     async def async_sql_op(
         self,
         dataset: st.Dataset,
         query: t.Union[str, t.Dict[str, t.Any]],
         dialect: t.Optional[st.SQLDialect] = None,
         batch_size: int = 10000,
         result_type: t.Optional[st.Type] = None,
```

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/cache_utils.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/cache_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/base.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/local/base.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/local/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/local/schema.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/local/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/computations/remote/base.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/remote/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/base.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/__init__.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/external_op.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/external_op.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import pyarrow as pa
 
 from sarus_data_spec.arrow.admin_utils import (
     compute_admin_data,
     create_admin_columns,
     merge_data_and_admin,
 )
+from sarus_data_spec.arrow.array import fit_array_to_schema_type_async_gen
 from sarus_data_spec.arrow.conversion import to_pyarrow_table
 from sarus_data_spec.arrow.schema import type_from_arrow_schema
 from sarus_data_spec.constants import MAX_MAX_MULT, MULTIPLICITY
 from sarus_data_spec.dataset import Dataset
 from sarus_data_spec.dataspec_validator.signature import (
     SarusBoundSignature,
     SarusSignature,
@@ -249,15 +250,17 @@
         converting the Pyarrow schema to a Sarus schema.q
         """
         syn_variant = self.dataset.variant(kind=st.ConstraintKind.SYNTHETIC)
         assert syn_variant is not None
         assert syn_variant.prototype() == sp.Dataset
 
         syn_dataset = t.cast(st.Dataset, syn_variant)
-        arrow_iterator = await syn_dataset.async_to_arrow(batch_size=1000)
+        arrow_iterator = await compute_external_to_arrow(
+            syn_dataset, batch_size=1000
+        )
         first_batch = await arrow_iterator.__anext__()
         schema = first_batch.schema
 
         schema_type = type_from_arrow_schema(schema)
 
         # retrieve max_mul from parent
         parents_args, parents_kwargs = self.dataset.parents()
@@ -312,41 +315,22 @@
         )
 
 
 class ExternalDatasetOp(DatasetImplementation):
     async def to_arrow(
         self, batch_size: int
     ) -> t.AsyncIterator[pa.RecordBatch]:
-        transform = self.dataset.transform()
-        implementation = external_implementation(transform)
-        bound_signature = implementation.signature().bind_dataspec(
-            self.dataset
+        batches_async_it = await compute_external_to_arrow(
+            self.dataset, batch_size
+        )
+        schema = await self.dataset.async_schema()
+        # make sure the arrow array is conform to its schema.
+        return fit_array_to_schema_type_async_gen(
+            batches_async_it, schema.type()
         )
-        bound_signature.static_validation()
-
-        if self.dataset.is_pup():
-            result = await implementation.compute(bound_signature)
-            if (
-                isinstance(result, pd.Series)
-                and implementation.pup_kind(bound_signature) == PUPKind.ROW
-            ):
-                # Reformat the series as a dataframe with a single row
-                result = result.to_frame().transpose()
-            ds_result = t.cast(st.DatasetCastable, result)
-            admin_data = await bound_signature.admin_data()
-            output_admin_data = compute_admin_data(admin_data, ds_result)
-            data_table = to_pyarrow_table(ds_result)
-            table = merge_data_and_admin(data_table, output_admin_data)
-
-        else:
-            result = await implementation.compute(bound_signature)
-            data_table = to_pyarrow_table(result)
-            table = create_admin_columns(data_table)
-
-        return async_iter(table.to_batches(max_chunksize=batch_size))
 
     async def size(self) -> st.Size:
         implementation = external_implementation(self.dataset.transform())
         bound_signature = implementation.signature().bind_dataspec(
             self.dataset
         )
         pup_kind = implementation.pup_kind(bound_signature)
@@ -608,7 +592,38 @@
                 .statistics()
                 .multiplicity()
             )
         except Exception:
             # this is for the mock, not very nice
             max_mult = ""
     return max_mult
+
+
+async def compute_external_to_arrow(
+    dataset: st.Dataset, batch_size: int
+) -> t.AsyncIterator[pa.RecordBatch]:
+    """It computes arrow record batches of a dataset from the external op implementation"""
+    transform = dataset.transform()
+    implementation = external_implementation(transform)
+    bound_signature = implementation.signature().bind_dataspec(dataset)
+    bound_signature.static_validation()
+
+    if dataset.is_pup():
+        result = await implementation.compute(bound_signature)
+        if (
+            isinstance(result, pd.Series)
+            and implementation.pup_kind(bound_signature) == PUPKind.ROW
+        ):
+            # Reformat the series as a dataframe with a single row
+            result = result.to_frame().transpose()
+        ds_result = t.cast(st.DatasetCastable, result)
+        admin_data = await bound_signature.admin_data()
+        output_admin_data = compute_admin_data(admin_data, ds_result)
+        data_table = to_pyarrow_table(ds_result)
+        table = merge_data_and_admin(data_table, output_admin_data)
+
+    else:
+        result = await implementation.compute(bound_signature)
+        data_table = to_pyarrow_table(result)
+        table = create_admin_columns(data_table)
+
+    return async_iter(table.to_batches(max_chunksize=batch_size))
```

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/imblearn.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/imblearn.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/numpy.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/numpy.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/optbinning.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/optbinning.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/pandas/groupby_dp.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/pandas/groupby_dp.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,25 +34,22 @@
     from sarus_data_spec.sarus_statistics.ops.mean.op import GroupByMeanOp
     from sarus_data_spec.sarus_statistics.ops.median.op import GroupbyMedianOp
     from sarus_data_spec.sarus_statistics.ops.std.op import GroupByStdOp
     from sarus_data_spec.sarus_statistics.ops.sum.op import GroupBySumOp
     from sarus_data_spec.sarus_statistics.ops.tau_thresholding.op import (
         TauThresholdingOp,
     )
-except ModuleNotFoundError:
-    pass
-    # TODO properly: from sarus_data_spec.sarus_statistics.ops.bounds.op
-    # imports sarus_differential_privacy
-    # if "sarus_data_spec.sarus_statistics" not in str(e_pandas_dp):
-    #     raise
+except ModuleNotFoundError as e_groupby_dp:
+    if "sarus_data_spec.sarus_statistics" not in str(e_groupby_dp):
+        raise
 
 try:
     from sarus_differential_privacy.query import ComposedPrivateQuery
-except ModuleNotFoundError as e_pandas_dp:
-    if "sarus_differential_privacy" not in str(e_pandas_dp):
+except ModuleNotFoundError as e_groupby_dp:
+    if "sarus_differential_privacy" not in str(e_groupby_dp):
         raise
 
 try:
     from sarus_data_spec.sarus_query_builder.builders.bounds_builder import (
         simple_bounds_builder,
     )
     from sarus_data_spec.sarus_query_builder.builders.composed_builder import (
@@ -224,19 +221,20 @@
         for index, column_name in enumerate(dataframegroupby.nth(0).columns):
             count_parameters = shape_task[index]
             dataframes_with_counts[column_name] = GroupByCountOp(
                 parent_ds,
                 count_parameters.parameters["noise"],
             ).value(column_name, max_mul, random_generator, keys_values)
 
+        for col_name, df in dataframes_with_counts.items():
+            df.columns = [col_name]
+
         if len(dataframes_with_counts.keys()) == 1:
             return list(dataframes_with_counts.values())[0]
         else:
-            for col_name, df in dataframes_with_counts.items():
-                df.columns = [col_name]
             return pd.concat(dataframes_with_counts.values(), axis=1)
 
 
 class pd_mean_groupby_dp(ExternalOpImplementation):
     _transform_id = "pandas.PD_MEAN_GROUPBY_DP"
     _non_dp_equivalent_id = "pandas.PD_MEAN_GROUPBY"
 
@@ -379,19 +377,20 @@
                 parent_ds,
                 mean_parameters.parameters["noise"],
             )
             dataframes_with_dp_means[column_name] = mean_op.value(
                 column_name, max_mul, bounds, random_generator, keys_values
             )
 
+        for col_name, df in dataframes_with_dp_means.items():
+            df.columns = [col_name]
+
         if len(dataframes_with_dp_means.keys()) == 1:
             return list(dataframes_with_dp_means.values())[0]
         else:
-            for col_name, df in dataframes_with_dp_means.items():
-                df.columns = [col_name]
             return pd.concat(dataframes_with_dp_means.values(), axis=1)
 
 
 class pd_median_groupby_dp(ExternalOpImplementation):
     _transform_id = "pandas.PD_MEDIAN_GROUPBY_DP"
     _non_dp_equivalent_id = "pandas.PD_MEDIAN_GROUPBY"
 
@@ -535,19 +534,20 @@
                 parent_ds,
                 median_parameters.parameters["noise"],
             )
             dataframes_with_dp_median[column_name] = median_op.value(
                 column_name, max_mul, bounds, random_generator, keys_values
             )
 
+        for col_name, df in dataframes_with_dp_median.items():
+            df.columns = [col_name]
+
         if len(dataframes_with_dp_median.keys()) == 1:
             return list(dataframes_with_dp_median.values())[0]
         else:
-            for col_name, df in dataframes_with_dp_median.items():
-                df.columns = [col_name]
             return pd.concat(dataframes_with_dp_median.values(), axis=1)
 
 
 class pd_std_groupby_dp(ExternalOpImplementation):
     _transform_id = "pandas.PD_STD_GROUPBY_DP"
     _non_dp_equivalent_id = "pandas.PD_STD_GROUPBY"
 
@@ -690,19 +690,20 @@
                 std_parameters.parameters["noise_square"],
                 std_parameters.parameters["noise_count"],
             )
             dataframes_with_dp_std[column_name] = std_op.value(
                 column_name, max_mul, bounds, random_generator, keys_values
             )
 
+        for col_name, df in dataframes_with_dp_std.items():
+            df.columns = [col_name]
+
         if len(dataframes_with_dp_std.keys()) == 1:
             return list(dataframes_with_dp_std.values())[0]
         else:
-            for col_name, df in dataframes_with_dp_std.items():
-                df.columns = [col_name]
             return pd.concat(dataframes_with_dp_std.values(), axis=1)
 
 
 class pd_sum_groupby_dp(ExternalOpImplementation):
     _transform_id = "pandas.PD_SUM_GROUPBY_DP"
     _non_dp_equivalent_id = "pandas.PD_SUM_GROUPBY"
 
@@ -844,13 +845,14 @@
                 parent_ds,
                 sum_parameters.parameters["noise"],
             )
             dataframes_with_dp_sum[column_name] = sum_op.value(
                 column_name, max_mul, bounds, random_generator, keys_values
             )
 
+        for col_name, df in dataframes_with_dp_sum.items():
+            df.columns = [col_name]
+
         if len(dataframes_with_dp_sum.keys()) == 1:
             return list(dataframes_with_dp_sum.values())[0]
         else:
-            for col_name, df in dataframes_with_dp_sum.items():
-                df.columns = [col_name]
             return pd.concat(dataframes_with_dp_sum.values(), axis=1)
```

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,20 +31,17 @@
     from sarus_data_spec.sarus_statistics.ops.mean.op import MeanOp
     from sarus_data_spec.sarus_statistics.ops.median.op import MedianOp
     from sarus_data_spec.sarus_statistics.ops.std.op import StdOp
     from sarus_data_spec.sarus_statistics.ops.sum.op import SumOp
     from sarus_data_spec.sarus_statistics.protobuf.multiplicity_pb2 import (
         MultiplicityParameters,
     )
-except ModuleNotFoundError:
-    pass
-    # TODO properly: from sarus_data_spec.sarus_statistics.ops.bounds.op
-    # imports sarus_differential_privacy
-    # if "sarus_data_spec.sarus_statistics" not in str(e_pandas_dp):
-    #     raise
+except ModuleNotFoundError as e_pandas_dp:
+    if "sarus_data_spec.sarus_statistics" not in str(e_pandas_dp):
+        raise
 
 try:
     from sarus_differential_privacy.query import ComposedPrivateQuery
 except ModuleNotFoundError as e_pandas_dp:
     if "sarus_differential_privacy" not in str(e_pandas_dp):
         raise
```

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/scipy.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/scipy.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/shap/Explanation.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/shap/Explanation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/shap/explainer.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/shap/explainer.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/shap/maskers.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/shap/maskers.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/shap/plots.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/shap/plots.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/shap/utils.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/shap/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/skopt.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/skopt.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/std.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/std.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/typing.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/utils.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/external/xgboost.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/xgboost.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/routing.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/routing.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,18 @@
     Project,
     ProjectStaticChecker,
 )
 from sarus_data_spec.manager.ops.processor.standard.to_small_data import (
     ToSmallData,
     ToSmallDataStaticChecker,
 )
+from sarus_data_spec.manager.ops.processor.standard.push_sql import (
+    PushSQL,
+    PushSQLStaticChecker,
+)
 
 try:
     from sarus_data_spec.manager.ops.processor.standard.sample import (
         Sample,
         SampleStaticChecker,
     )
 
@@ -251,14 +255,16 @@
         return Transcode, TranscodeStaticChecker
     elif transform.spec() == "select_sql":
         return SelectSQL, SelectSQLStaticChecker
     elif transform.spec() == "dp_select_sql":
         return DPSelectSQL, DPSelectSQLStaticChecker
     elif transform.spec() == "extract":
         return Extract, ExtractStaticChecker
+    elif transform.spec() == "push_sql":
+        return PushSQL, PushSQLStaticChecker
     elif transform.spec() == "generate_from_model":
         return GenerateFromModel, GenerateFromModelStaticChecker
     else:
         raise NotImplementedError(transform.spec())
 
 
 def get_scalar_op(
```

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/error_estimation.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/error_estimation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/extract.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/extract.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/filter.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/filter.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/generate_from_model.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/generate_from_model.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/get_item.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/get_item.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,24 +87,34 @@
             array = convert_record_batch(
                 record_batch=batch, _type=parent_schema.type()
             )
             # VERY UGLY SHOULD BE REMOVED WHEN WE HAVE PROTECTED TYPE
             if DATA in parent_schema.type().children():
                 old_arrays = array.flatten()
                 idx_data = array.type.get_field_index(DATA)
+                list_col_names = list(parent_schema.type().children().keys())
+                list_idx = [
+                    array.type.get_field_index(col) for col in list_col_names
+                ]
+                reordered_list_col_names = [
+                    list_col_names[i]
+                    for i in sorted(
+                        range(len(list_idx)), key=lambda k: list_idx[k]
+                    )
+                ]
                 array = old_arrays[idx_data]
                 updated_array = get_items(
                     _type=parent_schema.data_type(),
                     array=array,
                     path=path,
                 )
                 old_arrays[idx_data] = updated_array
                 return pa.StructArray.from_arrays(
                     old_arrays,
-                    names=list(parent_schema.type().children().keys()),
+                    names=reordered_list_col_names,
                 )
 
             updated_array = get_items(
                 _type=parent_schema.data_type(),
                 array=array,
                 path=path,
             )
```

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/project.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/project.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/sample.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import AsyncIterator, List, Union
 import typing as t
 import warnings
 
 import numpy as np
 import pyarrow as pa
+import gc
 
 from sarus_data_spec.bounds import bounds as bounds_builder
 from sarus_data_spec.constants import DATA, DATASET_SLUGNAME
 from sarus_data_spec.dataset import Dataset
 from sarus_data_spec.manager.async_utils import async_iter
 from sarus_data_spec.manager.ops.processor.standard.standard_op import (  # noqa: E501
     StandardDatasetImplementation,
@@ -225,14 +226,16 @@
     if sampling_spec.HasField("fraction"):
         new_size = int(sampling_spec.fraction * parent_table.num_rows)
     else:
         new_size = sampling_spec.size
 
     parent_size = await op.parent_size()
     if new_size >= parent_size.statistics().size():
+        del parent_batches, parent_table
+        gc.collect()
         return await op.parent_to_arrow(batch_size)
 
     indices = generator.choice(
         parent_table.num_rows,
         replace=False,
         size=new_size,
     )
```

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/sampling/differentiated_sampling_sizes.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/sampling/differentiated_sampling_sizes.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/shuffle.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/shuffle.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/standard_op.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/standard_op.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/synthetic.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/synthetic.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/to_small_data.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/to_small_data.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/source/routing.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/source/routing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/sql_utils/bigdata.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/sql_utils/bigdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,18 @@
         for grouped_queries in grouped(self.queries, self.group_by):
             queries = [query for query in grouped_queries if query]
             result_types: t.List[t.Optional[st.Type]] = [
                 query[1] for query in queries
             ]
             assert len(set(result_types)) == 1
             union_query = sa.union_all(
-                *[statement for statement, result_type in queries]
+                *[
+                    t.cast(sa.sql.selectable.Select, statement)
+                    for statement, result_type in queries
+                ]
             )
 
             rendered = sqlalchemy_query_to_string(union_query)
             query_result = await dataset.manager().async_sql(
                 dataset, rendered, result_type=result_types[0]
             )
             results.extend(
```

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/ops/sql_utils/queries.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/sql_utils/queries.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/manager/typing.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,19 @@
     ) -> st.Multiplicity: ...
 
     def to_pandas(self, dataset: st.Dataset) -> pd.DataFrame: ...
 
     async def async_to_pandas(self, dataset: st.Dataset) -> pd.DataFrame: ...
 
     async def async_to(
-        self, dataset: st.Dataset, kind: t.Type, drop_admin: bool = True
+        self,
+        dataset: st.Dataset,
+        kind: t.Type,
+        drop_admin: bool = True,
+        batch_size: t.Optional[int] = None,
     ) -> st.DatasetCastable:
         """Casts a Dataset to a Python type passed as argument."""
         ...
 
     def to(
         self, dataset: st.Dataset, kind: t.Type, drop_admin: bool = True
     ) -> st.DatasetCastable: ...
@@ -163,16 +167,20 @@
 
     async def async_to_tensorflow(
         self, dataset: st.Dataset
     ) -> tf.data.Dataset: ...
 
     def to_sql(self, dataset: st.Dataset) -> None: ...
 
+    def push_sql(self, dataset: st.Dataset) -> None: ...
+
     async def async_to_sql(self, dataset: st.Dataset) -> None: ...
 
+    async def async_push_sql(self, dataset: st.Dataset) -> None: ...
+
     def status(
         self, dataspec: st.DataSpec, task_name: t.Optional[str] = None
     ) -> t.Optional[st.Status]: ...
 
     def dataspec_rewriter(self) -> sdrt.DataspecRewriter: ...
 
     def dataspec_validator(self) -> sdvt.DataspecValidator: ...
@@ -241,15 +249,15 @@
     def caches(self) -> t.Any: ...
 
     def is_cached(self, dataspec: st.DataSpec) -> bool:
         """Returns whether a dataspec should be cached
         or not"""
         ...
 
-    def is_pushed_to_sql(self, dataspec: st.DataSpec) -> bool:
+    def is_cached_to_sql(self, dataspec: st.DataSpec) -> bool:
         """Returns whether a dataspec should be pushed to sql
         or not"""
         ...
 
     def attribute(
         self, name: str, dataspec: st.DataSpec
     ) -> t.Optional[st.Attribute]: ...
```

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/marginals.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/marginals.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/multiplicity.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/multiplicity.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/path.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/path.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/predicate.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/predicate.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/__init__.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/attribute_pb2.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/attribute_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/attribute_pb2.pyi` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/attribute_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/bounds_pb2.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/bounds_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/bounds_pb2.pyi` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/bounds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/constraint_pb2.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/constraint_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/constraint_pb2.pyi` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/constraint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/dataset.proto` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/dataset.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/dataset_pb2.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/dataset_pb2.pyi` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/links_pb2.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/links_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/links_pb2.pyi` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/links_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/manager_pb2.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/manager_pb2.pyi` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/marginals_pb2.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/marginals_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/marginals_pb2.pyi` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/marginals_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/multiplicity_pb2.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/multiplicity_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/multiplicity_pb2.pyi` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/multiplicity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/path_pb2.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/path_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/path_pb2.pyi` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/path_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/predicate.proto` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/predicate.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/predicate_pb2.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/predicate_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/predicate_pb2.pyi` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/predicate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/proto_container_pb2.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/proto_container_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/proto_container_pb2.pyi` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/proto_container_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/relation.proto` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/relation.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/relation_pb2.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/relation_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/relation_pb2.pyi` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/relation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/scalar.proto` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/scalar.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/scalar_pb2.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/scalar_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/scalar_pb2.pyi` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/scalar_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/schema.proto` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/schema.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/schema_pb2.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/schema_pb2.pyi` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/schema_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/size_pb2.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/size_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/size_pb2.pyi` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/size_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/statistics.proto` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/statistics.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/statistics_pb2.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/statistics_pb2.pyi` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/statistics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/status.proto` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/status.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/status_pb2.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/status_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/status_pb2.pyi` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/transform.proto` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/transform.proto`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,15 @@
       ValidatedUserType validated_user_type = 31;
       DPSelectSql dp_select_sql = 32;
       ErrorEstimation error_estimation = 33;
       FitModel fit_model = 34;
       FitModelDP fit_model_dp = 35;
       GenerateFromModel generate_from_model = 36;
       ToSmallData to_small_data = 37;
+      PushSQL push_sql = 38;
     }
   }
 
   message External {
     bytes arguments = 1;
     bytes named_arguments = 2;
     OpIdentifier op_identifier = 3;
@@ -187,14 +188,21 @@
 
   message ToSmallData {
     int32 size = 1;
     bool random_sampling = 2;
     sarus_data_spec.Scalar seed = 3;
   }
 
+  message PushSQL {
+    string dataconnection_name = 1;
+    string schema_name = 2;
+    string table_name = 3;
+    string uri = 4;
+  }
+
   message Synthetic {
   }
 
   message UserSettings {
   }
 
   message AutomaticUserSettings {
```

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/transform_pb2.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/transform_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,143 +12,145 @@
 
 
 from sarus_data_spec.protobuf import type_pb2 as sarus__data__spec_dot_protobuf_dot_type__pb2
 from sarus_data_spec.protobuf import path_pb2 as sarus__data__spec_dot_protobuf_dot_path__pb2
 from sarus_data_spec.protobuf import scalar_pb2 as sarus__data__spec_dot_protobuf_dot_scalar__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(sarus_data_spec/protobuf/transform.proto\x1a#sarus_data_spec/protobuf/type.proto\x1a#sarus_data_spec/protobuf/path.proto\x1a%sarus_data_spec/protobuf/scalar.proto\"\xd1)\n\tTransform\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0b\n\x03\x64oc\x18\x03 \x01(\t\x12\x1d\n\x04spec\x18\x04 \x01(\x0b\x32\x0f.Transform.Spec\x12.\n\nproperties\x18\x05 \x03(\x0b\x32\x1a.Transform.PropertiesEntry\x12\x12\n\ninversible\x18\x06 \x01(\x08\x12\x19\n\x11schema_preserving\x18\x07 \x01(\x08\x1a\x31\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x92\x0e\n\x04Spec\x12\'\n\x08identity\x18\x01 \x01(\x0b\x32\x13.Transform.IdentityH\x00\x12\'\n\x08variable\x18\x02 \x01(\x0b\x32\x13.Transform.VariableH\x00\x12\'\n\x08\x63omposed\x18\x03 \x01(\x0b\x32\x13.Transform.ComposedH\x00\x12%\n\x07project\x18\x04 \x01(\x0b\x32\x12.Transform.ProjectH\x00\x12#\n\x06\x66ilter\x18\x05 \x01(\x0b\x32\x11.Transform.FilterH\x00\x12%\n\x07shuffle\x18\x06 \x01(\x0b\x32\x12.Transform.ShuffleH\x00\x12\x1f\n\x04join\x18\x07 \x01(\x0b\x32\x0f.Transform.JoinH\x00\x12\x1f\n\x04\x63\x61st\x18\x08 \x01(\x0b\x32\x0f.Transform.CastH\x00\x12#\n\x06sample\x18\t \x01(\x0b\x32\x11.Transform.SampleH\x00\x12\x30\n\ruser_settings\x18\n \x01(\x0b\x32\x17.Transform.UserSettingsH\x00\x12?\n\x15privacy_unit_tracking\x18\x0b \x01(\x0b\x32\x1e.Transform.PrivacyUnitTrackingH\x00\x12\'\n\x08\x65xternal\x18\x0c \x01(\x0b\x32\x13.Transform.ExternalH\x00\x12)\n\tsynthetic\x18\r \x01(\x0b\x32\x14.Transform.SyntheticH\x00\x12)\n\ttranscode\x18\x0e \x01(\x0b\x32\x14.Transform.TranscodeH\x00\x12\x38\n\x11inverse_transcode\x18\x0f \x01(\x0b\x32\x1b.Transform.InverseTranscodeH\x00\x12&\n\x08get_item\x18\x10 \x01(\x0b\x32\x12.Transform.GetItemH\x00\x12J\n\x1bprivacy_unit_tracking_paths\x18\x11 \x01(\x0b\x32#.Transform.PrivacyUnitTrackingPathsH\x00\x12\x43\n\x17\x61utomatic_user_settings\x18\x12 \x01(\x0b\x32 .Transform.AutomaticUserSettingsH\x00\x12.\n\x0cpublic_paths\x18\x13 \x01(\x0b\x32\x16.Transform.PublicPathsH\x00\x12\x30\n\rassign_budget\x18\x14 \x01(\x0b\x32\x17.Transform.AssignBudgetH\x00\x12\x36\n\x10\x61utomatic_budget\x18\x15 \x01(\x0b\x32\x1a.Transform.AutomaticBudgetH\x00\x12\x37\n\x10\x61ttribute_budget\x18\x16 \x01(\x0b\x32\x1b.Transform.AttributesBudgetH\x00\x12(\n\tsd_budget\x18\x17 \x01(\x0b\x32\x13.Transform.SDBudgetH\x00\x12,\n\x0b\x64\x65rive_seed\x18\x18 \x01(\x0b\x32\x15.Transform.DeriveSeedH\x00\x12+\n\x0bgroup_by_pe\x18\x19 \x01(\x0b\x32\x14.Transform.GroupByPEH\x00\x12\x34\n\x0fsampling_ratios\x18\x1a \x01(\x0b\x32\x19.Transform.SamplingRatiosH\x00\x12*\n\nselect_sql\x18\x1b \x01(\x0b\x32\x14.Transform.SelectSqlH\x00\x12%\n\x07\x65xtract\x18\x1c \x01(\x0b\x32\x12.Transform.ExtractH\x00\x12\x38\n\x11relationship_spec\x18\x1d \x01(\x0b\x32\x1b.Transform.RelationshipSpecH\x00\x12@\n\x15\x64ifferentiated_sample\x18\x1e \x01(\x0b\x32\x1f.Transform.DifferentiatedSampleH\x00\x12;\n\x13validated_user_type\x18\x1f \x01(\x0b\x32\x1c.Transform.ValidatedUserTypeH\x00\x12/\n\rdp_select_sql\x18  \x01(\x0b\x32\x16.Transform.DPSelectSqlH\x00\x12\x36\n\x10\x65rror_estimation\x18! \x01(\x0b\x32\x1a.Transform.ErrorEstimationH\x00\x12(\n\tfit_model\x18\" \x01(\x0b\x32\x13.Transform.FitModelH\x00\x12-\n\x0c\x66it_model_dp\x18# \x01(\x0b\x32\x15.Transform.FitModelDPH\x00\x12;\n\x13generate_from_model\x18$ \x01(\x0b\x32\x1c.Transform.GenerateFromModelH\x00\x12/\n\rto_small_data\x18% \x01(\x0b\x32\x16.Transform.ToSmallDataH\x00\x42\x06\n\x04spec\x1a\xf6\x07\n\x08\x45xternal\x12\x11\n\targuments\x18\x01 \x01(\x0c\x12\x17\n\x0fnamed_arguments\x18\x02 \x01(\x0c\x12\x37\n\rop_identifier\x18\x03 \x01(\x0b\x32 .Transform.External.OpIdentifier\x1a\xd7\x04\n\x0cOpIdentifier\x12&\n\x03std\x18\x01 \x01(\x0b\x32\x17.Transform.External.StdH\x00\x12,\n\x06pandas\x18\x02 \x01(\x0b\x32\x1a.Transform.External.PandasH\x00\x12*\n\x05numpy\x18\x03 \x01(\x0b\x32\x19.Transform.External.NumpyH\x00\x12\x34\n\ntensorflow\x18\x04 \x01(\x0b\x32\x1e.Transform.External.TensorflowH\x00\x12.\n\x07sklearn\x18\x05 \x01(\x0b\x32\x1b.Transform.External.SklearnH\x00\x12?\n\x10pandas_profiling\x18\x06 \x01(\x0b\x32#.Transform.External.PandasProfilingH\x00\x12.\n\x07xgboost\x18\x07 \x01(\x0b\x32\x1b.Transform.External.XGBoostH\x00\x12*\n\x05skopt\x18\x08 \x01(\x0b\x32\x19.Transform.External.SkoptH\x00\x12\x30\n\x08imblearn\x18\t \x01(\x0b\x32\x1c.Transform.External.ImblearnH\x00\x12(\n\x04shap\x18\n \x01(\x0b\x32\x18.Transform.External.ShapH\x00\x12*\n\x05scipy\x18\x0b \x01(\x0b\x32\x19.Transform.External.ScipyH\x00\x12\x34\n\noptbinning\x18\x0c \x01(\x0b\x32\x1e.Transform.External.OptBinningH\x00\x42\x04\n\x02op\x1a\x13\n\x03Std\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x16\n\x06Pandas\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x15\n\x05Numpy\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x1a\n\nTensorflow\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x17\n\x07Sklearn\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x1f\n\x0fPandasProfiling\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x17\n\x07XGBoost\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x15\n\x05Skopt\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x18\n\x08Imblearn\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x14\n\x04Shap\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x15\n\x05Scipy\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x1a\n\nOptBinning\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\n\n\x08Identity\x1a*\n\x08Variable\x12\x10\n\x08position\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x1a\xa9\x01\n\x08\x43omposed\x12\x11\n\ttransform\x18\x01 \x01(\t\x12\x11\n\targuments\x18\x02 \x03(\t\x12@\n\x0fnamed_arguments\x18\x03 \x03(\x0b\x32\'.Transform.Composed.NamedArgumentsEntry\x1a\x35\n\x13NamedArgumentsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x34\n\x07Project\x12)\n\nprojection\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a/\n\x06\x46ilter\x12%\n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a\t\n\x07Shuffle\x1a)\n\x04Join\x12!\n\x02on\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a+\n\x04\x43\x61st\x12#\n\x04type\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a\x61\n\x06Sample\x12\x12\n\x08\x66raction\x18\x01 \x01(\x01H\x00\x12\x0e\n\x04size\x18\x02 \x01(\x03H\x00\x12%\n\x04seed\x18\x03 \x01(\x0b\x32\x17.sarus_data_spec.ScalarB\x0c\n\nproportion\x1av\n\x0fSchemaInference\x12:\n\x0b\x63\x61st_policy\x18\x01 \x01(\x0e\x32%.Transform.SchemaInference.CastPolicy\"\'\n\nCastPolicy\x12\x08\n\x04NONE\x10\x00\x12\x0f\n\x0bMOST_LIKELY\x10\x01\x1a\x16\n\x07GroupBy\x12\x0b\n\x03key\x18\x01 \x01(\t\x1a[\n\x0bToSmallData\x12\x0c\n\x04size\x18\x01 \x01(\x05\x12\x17\n\x0frandom_sampling\x18\x02 \x01(\x08\x12%\n\x04seed\x18\x03 \x01(\x0b\x32\x17.sarus_data_spec.Scalar\x1a\x0b\n\tSynthetic\x1a\x0e\n\x0cUserSettings\x1a/\n\x15\x41utomaticUserSettings\x12\x16\n\x0emax_categories\x18\x01 \x01(\x03\x1a\x15\n\x13PrivacyUnitTracking\x1a\x0b\n\tTranscode\x1a\x12\n\x10InverseTranscode\x1ao\n\x14\x44ifferentiatedSample\x12\x12\n\x08\x66raction\x18\x01 \x01(\x01H\x00\x12\x0e\n\x04size\x18\x02 \x01(\x03H\x00\x12%\n\x04seed\x18\x03 \x01(\x0b\x32\x17.sarus_data_spec.ScalarB\x0c\n\nproportion\x1a\x1a\n\x18PrivacyUnitTrackingPaths\x1a\r\n\x0bPublicPaths\x1a.\n\x07GetItem\x12#\n\x04path\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Path\x1a\x0e\n\x0c\x41ssignBudget\x1a\x11\n\x0f\x41utomaticBudget\x1a\x12\n\x10\x41ttributesBudget\x1a\n\n\x08SDBudget\x1a$\n\nDeriveSeed\x12\x16\n\x0erandom_integer\x18\x01 \x01(\x03\x1a\x0b\n\tGroupByPE\x1a\x10\n\x0eSamplingRatios\x1a\x12\n\x10RelationshipSpec\x1a\x88\x01\n\tSelectSql\x12\x0f\n\x05query\x18\x01 \x01(\tH\x00\x12\x34\n\x0f\x61liased_queries\x18\x02 \x01(\x0b\x32\x19.Transform.AliasedQueriesH\x00\x12*\n\x0bsql_dialect\x18\x03 \x01(\x0e\x32\x15.Transform.SQLDialectB\x08\n\x06select\x1a\x8a\x01\n\x0b\x44PSelectSql\x12\x0f\n\x05query\x18\x01 \x01(\tH\x00\x12\x34\n\x0f\x61liased_queries\x18\x02 \x01(\x0b\x32\x19.Transform.AliasedQueriesH\x00\x12*\n\x0bsql_dialect\x18\x03 \x01(\x0e\x32\x15.Transform.SQLDialectB\x08\n\x06select\x1a@\n\x0e\x41liasedQueries\x12.\n\raliased_query\x18\x01 \x03(\x0b\x32\x17.Transform.AliasedQuery\x1a\x42\n\x0c\x41liasedQuery\x12#\n\x04path\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Path\x12\r\n\x05query\x18\x02 \x01(\t\x1a\x17\n\x07\x45xtract\x12\x0c\n\x04size\x18\x01 \x01(\x05\x1a\x13\n\x11ValidatedUserType\x1a\x11\n\x0f\x45rrorEstimation\x1aV\n\x08\x46itModel\x12\x12\n\nbatch_size\x18\x01 \x01(\x05\x12\x0e\n\x06\x65pochs\x18\x02 \x01(\x05\x12&\n\ttext_kind\x18\x03 \x01(\x0b\x32\x13.Transform.TextKind\x1aN\n\x08TextKind\x12\x14\n\ntext_field\x18\x01 \x01(\tH\x00\x12\x1f\n\x04\x63hat\x18\x02 \x01(\x0b\x32\x0f.Transform.ChatH\x00\x42\x0b\n\ttext_kind\x1a\x34\n\x04\x43hat\x12\x16\n\x0equestion_field\x18\x01 \x01(\t\x12\x14\n\x0c\x61nswer_field\x18\x02 \x01(\t\x1an\n\nFitModelDP\x12\x12\n\nbatch_size\x18\x01 \x01(\x05\x12\x0e\n\x06\x65pochs\x18\x03 \x01(\x05\x12\x14\n\x0cl2_norm_clip\x18\x04 \x01(\x01\x12&\n\ttext_kind\x18\x05 \x01(\x0b\x32\x13.Transform.TextKind\x1a@\n\x11GenerateFromModel\x12\x16\n\x0emax_new_tokens\x18\x01 \x01(\x05\x12\x13\n\x0btemperature\x18\x02 \x01(\x01\"\x80\x01\n\nSQLDialect\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08POSTGRES\x10\x01\x12\x0e\n\nSQL_SERVER\x10\x02\x12\n\n\x06MY_SQL\x10\x03\x12\x0b\n\x07SQLLITE\x10\x04\x12\n\n\x06ORACLE\x10\x05\x12\r\n\tBIG_QUERY\x10\x06\x12\x0c\n\x08REDSHIFT\x10\x07\x12\x08\n\x04HIVE\x10\x08\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(sarus_data_spec/protobuf/transform.proto\x1a#sarus_data_spec/protobuf/type.proto\x1a#sarus_data_spec/protobuf/path.proto\x1a%sarus_data_spec/protobuf/scalar.proto\"\xd7*\n\tTransform\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0b\n\x03\x64oc\x18\x03 \x01(\t\x12\x1d\n\x04spec\x18\x04 \x01(\x0b\x32\x0f.Transform.Spec\x12.\n\nproperties\x18\x05 \x03(\x0b\x32\x1a.Transform.PropertiesEntry\x12\x12\n\ninversible\x18\x06 \x01(\x08\x12\x19\n\x11schema_preserving\x18\x07 \x01(\x08\x1a\x31\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xba\x0e\n\x04Spec\x12\'\n\x08identity\x18\x01 \x01(\x0b\x32\x13.Transform.IdentityH\x00\x12\'\n\x08variable\x18\x02 \x01(\x0b\x32\x13.Transform.VariableH\x00\x12\'\n\x08\x63omposed\x18\x03 \x01(\x0b\x32\x13.Transform.ComposedH\x00\x12%\n\x07project\x18\x04 \x01(\x0b\x32\x12.Transform.ProjectH\x00\x12#\n\x06\x66ilter\x18\x05 \x01(\x0b\x32\x11.Transform.FilterH\x00\x12%\n\x07shuffle\x18\x06 \x01(\x0b\x32\x12.Transform.ShuffleH\x00\x12\x1f\n\x04join\x18\x07 \x01(\x0b\x32\x0f.Transform.JoinH\x00\x12\x1f\n\x04\x63\x61st\x18\x08 \x01(\x0b\x32\x0f.Transform.CastH\x00\x12#\n\x06sample\x18\t \x01(\x0b\x32\x11.Transform.SampleH\x00\x12\x30\n\ruser_settings\x18\n \x01(\x0b\x32\x17.Transform.UserSettingsH\x00\x12?\n\x15privacy_unit_tracking\x18\x0b \x01(\x0b\x32\x1e.Transform.PrivacyUnitTrackingH\x00\x12\'\n\x08\x65xternal\x18\x0c \x01(\x0b\x32\x13.Transform.ExternalH\x00\x12)\n\tsynthetic\x18\r \x01(\x0b\x32\x14.Transform.SyntheticH\x00\x12)\n\ttranscode\x18\x0e \x01(\x0b\x32\x14.Transform.TranscodeH\x00\x12\x38\n\x11inverse_transcode\x18\x0f \x01(\x0b\x32\x1b.Transform.InverseTranscodeH\x00\x12&\n\x08get_item\x18\x10 \x01(\x0b\x32\x12.Transform.GetItemH\x00\x12J\n\x1bprivacy_unit_tracking_paths\x18\x11 \x01(\x0b\x32#.Transform.PrivacyUnitTrackingPathsH\x00\x12\x43\n\x17\x61utomatic_user_settings\x18\x12 \x01(\x0b\x32 .Transform.AutomaticUserSettingsH\x00\x12.\n\x0cpublic_paths\x18\x13 \x01(\x0b\x32\x16.Transform.PublicPathsH\x00\x12\x30\n\rassign_budget\x18\x14 \x01(\x0b\x32\x17.Transform.AssignBudgetH\x00\x12\x36\n\x10\x61utomatic_budget\x18\x15 \x01(\x0b\x32\x1a.Transform.AutomaticBudgetH\x00\x12\x37\n\x10\x61ttribute_budget\x18\x16 \x01(\x0b\x32\x1b.Transform.AttributesBudgetH\x00\x12(\n\tsd_budget\x18\x17 \x01(\x0b\x32\x13.Transform.SDBudgetH\x00\x12,\n\x0b\x64\x65rive_seed\x18\x18 \x01(\x0b\x32\x15.Transform.DeriveSeedH\x00\x12+\n\x0bgroup_by_pe\x18\x19 \x01(\x0b\x32\x14.Transform.GroupByPEH\x00\x12\x34\n\x0fsampling_ratios\x18\x1a \x01(\x0b\x32\x19.Transform.SamplingRatiosH\x00\x12*\n\nselect_sql\x18\x1b \x01(\x0b\x32\x14.Transform.SelectSqlH\x00\x12%\n\x07\x65xtract\x18\x1c \x01(\x0b\x32\x12.Transform.ExtractH\x00\x12\x38\n\x11relationship_spec\x18\x1d \x01(\x0b\x32\x1b.Transform.RelationshipSpecH\x00\x12@\n\x15\x64ifferentiated_sample\x18\x1e \x01(\x0b\x32\x1f.Transform.DifferentiatedSampleH\x00\x12;\n\x13validated_user_type\x18\x1f \x01(\x0b\x32\x1c.Transform.ValidatedUserTypeH\x00\x12/\n\rdp_select_sql\x18  \x01(\x0b\x32\x16.Transform.DPSelectSqlH\x00\x12\x36\n\x10\x65rror_estimation\x18! \x01(\x0b\x32\x1a.Transform.ErrorEstimationH\x00\x12(\n\tfit_model\x18\" \x01(\x0b\x32\x13.Transform.FitModelH\x00\x12-\n\x0c\x66it_model_dp\x18# \x01(\x0b\x32\x15.Transform.FitModelDPH\x00\x12;\n\x13generate_from_model\x18$ \x01(\x0b\x32\x1c.Transform.GenerateFromModelH\x00\x12/\n\rto_small_data\x18% \x01(\x0b\x32\x16.Transform.ToSmallDataH\x00\x12&\n\x08push_sql\x18& \x01(\x0b\x32\x12.Transform.PushSQLH\x00\x42\x06\n\x04spec\x1a\xf6\x07\n\x08\x45xternal\x12\x11\n\targuments\x18\x01 \x01(\x0c\x12\x17\n\x0fnamed_arguments\x18\x02 \x01(\x0c\x12\x37\n\rop_identifier\x18\x03 \x01(\x0b\x32 .Transform.External.OpIdentifier\x1a\xd7\x04\n\x0cOpIdentifier\x12&\n\x03std\x18\x01 \x01(\x0b\x32\x17.Transform.External.StdH\x00\x12,\n\x06pandas\x18\x02 \x01(\x0b\x32\x1a.Transform.External.PandasH\x00\x12*\n\x05numpy\x18\x03 \x01(\x0b\x32\x19.Transform.External.NumpyH\x00\x12\x34\n\ntensorflow\x18\x04 \x01(\x0b\x32\x1e.Transform.External.TensorflowH\x00\x12.\n\x07sklearn\x18\x05 \x01(\x0b\x32\x1b.Transform.External.SklearnH\x00\x12?\n\x10pandas_profiling\x18\x06 \x01(\x0b\x32#.Transform.External.PandasProfilingH\x00\x12.\n\x07xgboost\x18\x07 \x01(\x0b\x32\x1b.Transform.External.XGBoostH\x00\x12*\n\x05skopt\x18\x08 \x01(\x0b\x32\x19.Transform.External.SkoptH\x00\x12\x30\n\x08imblearn\x18\t \x01(\x0b\x32\x1c.Transform.External.ImblearnH\x00\x12(\n\x04shap\x18\n \x01(\x0b\x32\x18.Transform.External.ShapH\x00\x12*\n\x05scipy\x18\x0b \x01(\x0b\x32\x19.Transform.External.ScipyH\x00\x12\x34\n\noptbinning\x18\x0c \x01(\x0b\x32\x1e.Transform.External.OptBinningH\x00\x42\x04\n\x02op\x1a\x13\n\x03Std\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x16\n\x06Pandas\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x15\n\x05Numpy\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x1a\n\nTensorflow\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x17\n\x07Sklearn\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x1f\n\x0fPandasProfiling\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x17\n\x07XGBoost\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x15\n\x05Skopt\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x18\n\x08Imblearn\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x14\n\x04Shap\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x15\n\x05Scipy\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x1a\n\nOptBinning\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\n\n\x08Identity\x1a*\n\x08Variable\x12\x10\n\x08position\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x1a\xa9\x01\n\x08\x43omposed\x12\x11\n\ttransform\x18\x01 \x01(\t\x12\x11\n\targuments\x18\x02 \x03(\t\x12@\n\x0fnamed_arguments\x18\x03 \x03(\x0b\x32\'.Transform.Composed.NamedArgumentsEntry\x1a\x35\n\x13NamedArgumentsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x34\n\x07Project\x12)\n\nprojection\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a/\n\x06\x46ilter\x12%\n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a\t\n\x07Shuffle\x1a)\n\x04Join\x12!\n\x02on\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a+\n\x04\x43\x61st\x12#\n\x04type\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a\x61\n\x06Sample\x12\x12\n\x08\x66raction\x18\x01 \x01(\x01H\x00\x12\x0e\n\x04size\x18\x02 \x01(\x03H\x00\x12%\n\x04seed\x18\x03 \x01(\x0b\x32\x17.sarus_data_spec.ScalarB\x0c\n\nproportion\x1av\n\x0fSchemaInference\x12:\n\x0b\x63\x61st_policy\x18\x01 \x01(\x0e\x32%.Transform.SchemaInference.CastPolicy\"\'\n\nCastPolicy\x12\x08\n\x04NONE\x10\x00\x12\x0f\n\x0bMOST_LIKELY\x10\x01\x1a\x16\n\x07GroupBy\x12\x0b\n\x03key\x18\x01 \x01(\t\x1a[\n\x0bToSmallData\x12\x0c\n\x04size\x18\x01 \x01(\x05\x12\x17\n\x0frandom_sampling\x18\x02 \x01(\x08\x12%\n\x04seed\x18\x03 \x01(\x0b\x32\x17.sarus_data_spec.Scalar\x1a\\\n\x07PushSQL\x12\x1b\n\x13\x64\x61taconnection_name\x18\x01 \x01(\t\x12\x13\n\x0bschema_name\x18\x02 \x01(\t\x12\x12\n\ntable_name\x18\x03 \x01(\t\x12\x0b\n\x03uri\x18\x04 \x01(\t\x1a\x0b\n\tSynthetic\x1a\x0e\n\x0cUserSettings\x1a/\n\x15\x41utomaticUserSettings\x12\x16\n\x0emax_categories\x18\x01 \x01(\x03\x1a\x15\n\x13PrivacyUnitTracking\x1a\x0b\n\tTranscode\x1a\x12\n\x10InverseTranscode\x1ao\n\x14\x44ifferentiatedSample\x12\x12\n\x08\x66raction\x18\x01 \x01(\x01H\x00\x12\x0e\n\x04size\x18\x02 \x01(\x03H\x00\x12%\n\x04seed\x18\x03 \x01(\x0b\x32\x17.sarus_data_spec.ScalarB\x0c\n\nproportion\x1a\x1a\n\x18PrivacyUnitTrackingPaths\x1a\r\n\x0bPublicPaths\x1a.\n\x07GetItem\x12#\n\x04path\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Path\x1a\x0e\n\x0c\x41ssignBudget\x1a\x11\n\x0f\x41utomaticBudget\x1a\x12\n\x10\x41ttributesBudget\x1a\n\n\x08SDBudget\x1a$\n\nDeriveSeed\x12\x16\n\x0erandom_integer\x18\x01 \x01(\x03\x1a\x0b\n\tGroupByPE\x1a\x10\n\x0eSamplingRatios\x1a\x12\n\x10RelationshipSpec\x1a\x88\x01\n\tSelectSql\x12\x0f\n\x05query\x18\x01 \x01(\tH\x00\x12\x34\n\x0f\x61liased_queries\x18\x02 \x01(\x0b\x32\x19.Transform.AliasedQueriesH\x00\x12*\n\x0bsql_dialect\x18\x03 \x01(\x0e\x32\x15.Transform.SQLDialectB\x08\n\x06select\x1a\x8a\x01\n\x0b\x44PSelectSql\x12\x0f\n\x05query\x18\x01 \x01(\tH\x00\x12\x34\n\x0f\x61liased_queries\x18\x02 \x01(\x0b\x32\x19.Transform.AliasedQueriesH\x00\x12*\n\x0bsql_dialect\x18\x03 \x01(\x0e\x32\x15.Transform.SQLDialectB\x08\n\x06select\x1a@\n\x0e\x41liasedQueries\x12.\n\raliased_query\x18\x01 \x03(\x0b\x32\x17.Transform.AliasedQuery\x1a\x42\n\x0c\x41liasedQuery\x12#\n\x04path\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Path\x12\r\n\x05query\x18\x02 \x01(\t\x1a\x17\n\x07\x45xtract\x12\x0c\n\x04size\x18\x01 \x01(\x05\x1a\x13\n\x11ValidatedUserType\x1a\x11\n\x0f\x45rrorEstimation\x1aV\n\x08\x46itModel\x12\x12\n\nbatch_size\x18\x01 \x01(\x05\x12\x0e\n\x06\x65pochs\x18\x02 \x01(\x05\x12&\n\ttext_kind\x18\x03 \x01(\x0b\x32\x13.Transform.TextKind\x1aN\n\x08TextKind\x12\x14\n\ntext_field\x18\x01 \x01(\tH\x00\x12\x1f\n\x04\x63hat\x18\x02 \x01(\x0b\x32\x0f.Transform.ChatH\x00\x42\x0b\n\ttext_kind\x1a\x34\n\x04\x43hat\x12\x16\n\x0equestion_field\x18\x01 \x01(\t\x12\x14\n\x0c\x61nswer_field\x18\x02 \x01(\t\x1an\n\nFitModelDP\x12\x12\n\nbatch_size\x18\x01 \x01(\x05\x12\x0e\n\x06\x65pochs\x18\x03 \x01(\x05\x12\x14\n\x0cl2_norm_clip\x18\x04 \x01(\x01\x12&\n\ttext_kind\x18\x05 \x01(\x0b\x32\x13.Transform.TextKind\x1a@\n\x11GenerateFromModel\x12\x16\n\x0emax_new_tokens\x18\x01 \x01(\x05\x12\x13\n\x0btemperature\x18\x02 \x01(\x01\"\x80\x01\n\nSQLDialect\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08POSTGRES\x10\x01\x12\x0e\n\nSQL_SERVER\x10\x02\x12\n\n\x06MY_SQL\x10\x03\x12\x0b\n\x07SQLLITE\x10\x04\x12\n\n\x06ORACLE\x10\x05\x12\r\n\tBIG_QUERY\x10\x06\x12\x0c\n\x08REDSHIFT\x10\x07\x12\x08\n\x04HIVE\x10\x08\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sarus_data_spec.protobuf.transform_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _TRANSFORM_PROPERTIESENTRY._options = None
   _TRANSFORM_PROPERTIESENTRY._serialized_options = b'8\001'
   _TRANSFORM_COMPOSED_NAMEDARGUMENTSENTRY._options = None
   _TRANSFORM_COMPOSED_NAMEDARGUMENTSENTRY._serialized_options = b'8\001'
   _TRANSFORM._serialized_start=158
-  _TRANSFORM._serialized_end=5487
+  _TRANSFORM._serialized_end=5621
   _TRANSFORM_PROPERTIESENTRY._serialized_start=338
   _TRANSFORM_PROPERTIESENTRY._serialized_end=387
   _TRANSFORM_SPEC._serialized_start=390
-  _TRANSFORM_SPEC._serialized_end=2200
-  _TRANSFORM_EXTERNAL._serialized_start=2203
-  _TRANSFORM_EXTERNAL._serialized_end=3217
-  _TRANSFORM_EXTERNAL_OPIDENTIFIER._serialized_start=2317
-  _TRANSFORM_EXTERNAL_OPIDENTIFIER._serialized_end=2916
-  _TRANSFORM_EXTERNAL_STD._serialized_start=2918
-  _TRANSFORM_EXTERNAL_STD._serialized_end=2937
-  _TRANSFORM_EXTERNAL_PANDAS._serialized_start=2939
-  _TRANSFORM_EXTERNAL_PANDAS._serialized_end=2961
-  _TRANSFORM_EXTERNAL_NUMPY._serialized_start=2963
-  _TRANSFORM_EXTERNAL_NUMPY._serialized_end=2984
-  _TRANSFORM_EXTERNAL_TENSORFLOW._serialized_start=2986
-  _TRANSFORM_EXTERNAL_TENSORFLOW._serialized_end=3012
-  _TRANSFORM_EXTERNAL_SKLEARN._serialized_start=3014
-  _TRANSFORM_EXTERNAL_SKLEARN._serialized_end=3037
-  _TRANSFORM_EXTERNAL_PANDASPROFILING._serialized_start=3039
-  _TRANSFORM_EXTERNAL_PANDASPROFILING._serialized_end=3070
-  _TRANSFORM_EXTERNAL_XGBOOST._serialized_start=3072
-  _TRANSFORM_EXTERNAL_XGBOOST._serialized_end=3095
-  _TRANSFORM_EXTERNAL_SKOPT._serialized_start=3097
-  _TRANSFORM_EXTERNAL_SKOPT._serialized_end=3118
-  _TRANSFORM_EXTERNAL_IMBLEARN._serialized_start=3120
-  _TRANSFORM_EXTERNAL_IMBLEARN._serialized_end=3144
-  _TRANSFORM_EXTERNAL_SHAP._serialized_start=3146
-  _TRANSFORM_EXTERNAL_SHAP._serialized_end=3166
-  _TRANSFORM_EXTERNAL_SCIPY._serialized_start=3168
-  _TRANSFORM_EXTERNAL_SCIPY._serialized_end=3189
-  _TRANSFORM_EXTERNAL_OPTBINNING._serialized_start=3191
-  _TRANSFORM_EXTERNAL_OPTBINNING._serialized_end=3217
-  _TRANSFORM_IDENTITY._serialized_start=3219
-  _TRANSFORM_IDENTITY._serialized_end=3229
-  _TRANSFORM_VARIABLE._serialized_start=3231
-  _TRANSFORM_VARIABLE._serialized_end=3273
-  _TRANSFORM_COMPOSED._serialized_start=3276
-  _TRANSFORM_COMPOSED._serialized_end=3445
-  _TRANSFORM_COMPOSED_NAMEDARGUMENTSENTRY._serialized_start=3392
-  _TRANSFORM_COMPOSED_NAMEDARGUMENTSENTRY._serialized_end=3445
-  _TRANSFORM_PROJECT._serialized_start=3447
-  _TRANSFORM_PROJECT._serialized_end=3499
-  _TRANSFORM_FILTER._serialized_start=3501
-  _TRANSFORM_FILTER._serialized_end=3548
-  _TRANSFORM_SHUFFLE._serialized_start=3550
-  _TRANSFORM_SHUFFLE._serialized_end=3559
-  _TRANSFORM_JOIN._serialized_start=3561
-  _TRANSFORM_JOIN._serialized_end=3602
-  _TRANSFORM_CAST._serialized_start=3604
-  _TRANSFORM_CAST._serialized_end=3647
-  _TRANSFORM_SAMPLE._serialized_start=3649
-  _TRANSFORM_SAMPLE._serialized_end=3746
-  _TRANSFORM_SCHEMAINFERENCE._serialized_start=3748
-  _TRANSFORM_SCHEMAINFERENCE._serialized_end=3866
-  _TRANSFORM_SCHEMAINFERENCE_CASTPOLICY._serialized_start=3827
-  _TRANSFORM_SCHEMAINFERENCE_CASTPOLICY._serialized_end=3866
-  _TRANSFORM_GROUPBY._serialized_start=3868
-  _TRANSFORM_GROUPBY._serialized_end=3890
-  _TRANSFORM_TOSMALLDATA._serialized_start=3892
-  _TRANSFORM_TOSMALLDATA._serialized_end=3983
-  _TRANSFORM_SYNTHETIC._serialized_start=3985
-  _TRANSFORM_SYNTHETIC._serialized_end=3996
-  _TRANSFORM_USERSETTINGS._serialized_start=3998
-  _TRANSFORM_USERSETTINGS._serialized_end=4012
-  _TRANSFORM_AUTOMATICUSERSETTINGS._serialized_start=4014
-  _TRANSFORM_AUTOMATICUSERSETTINGS._serialized_end=4061
-  _TRANSFORM_PRIVACYUNITTRACKING._serialized_start=4063
-  _TRANSFORM_PRIVACYUNITTRACKING._serialized_end=4084
-  _TRANSFORM_TRANSCODE._serialized_start=4086
-  _TRANSFORM_TRANSCODE._serialized_end=4097
-  _TRANSFORM_INVERSETRANSCODE._serialized_start=4099
-  _TRANSFORM_INVERSETRANSCODE._serialized_end=4117
-  _TRANSFORM_DIFFERENTIATEDSAMPLE._serialized_start=4119
-  _TRANSFORM_DIFFERENTIATEDSAMPLE._serialized_end=4230
-  _TRANSFORM_PRIVACYUNITTRACKINGPATHS._serialized_start=4232
-  _TRANSFORM_PRIVACYUNITTRACKINGPATHS._serialized_end=4258
-  _TRANSFORM_PUBLICPATHS._serialized_start=4260
-  _TRANSFORM_PUBLICPATHS._serialized_end=4273
-  _TRANSFORM_GETITEM._serialized_start=4275
-  _TRANSFORM_GETITEM._serialized_end=4321
-  _TRANSFORM_ASSIGNBUDGET._serialized_start=4323
-  _TRANSFORM_ASSIGNBUDGET._serialized_end=4337
-  _TRANSFORM_AUTOMATICBUDGET._serialized_start=4339
-  _TRANSFORM_AUTOMATICBUDGET._serialized_end=4356
-  _TRANSFORM_ATTRIBUTESBUDGET._serialized_start=4358
-  _TRANSFORM_ATTRIBUTESBUDGET._serialized_end=4376
-  _TRANSFORM_SDBUDGET._serialized_start=4378
-  _TRANSFORM_SDBUDGET._serialized_end=4388
-  _TRANSFORM_DERIVESEED._serialized_start=4390
-  _TRANSFORM_DERIVESEED._serialized_end=4426
-  _TRANSFORM_GROUPBYPE._serialized_start=4428
-  _TRANSFORM_GROUPBYPE._serialized_end=4439
-  _TRANSFORM_SAMPLINGRATIOS._serialized_start=4441
-  _TRANSFORM_SAMPLINGRATIOS._serialized_end=4457
-  _TRANSFORM_RELATIONSHIPSPEC._serialized_start=4459
-  _TRANSFORM_RELATIONSHIPSPEC._serialized_end=4477
-  _TRANSFORM_SELECTSQL._serialized_start=4480
-  _TRANSFORM_SELECTSQL._serialized_end=4616
-  _TRANSFORM_DPSELECTSQL._serialized_start=4619
-  _TRANSFORM_DPSELECTSQL._serialized_end=4757
-  _TRANSFORM_ALIASEDQUERIES._serialized_start=4759
-  _TRANSFORM_ALIASEDQUERIES._serialized_end=4823
-  _TRANSFORM_ALIASEDQUERY._serialized_start=4825
-  _TRANSFORM_ALIASEDQUERY._serialized_end=4891
-  _TRANSFORM_EXTRACT._serialized_start=4893
-  _TRANSFORM_EXTRACT._serialized_end=4916
-  _TRANSFORM_VALIDATEDUSERTYPE._serialized_start=4918
-  _TRANSFORM_VALIDATEDUSERTYPE._serialized_end=4937
-  _TRANSFORM_ERRORESTIMATION._serialized_start=4939
-  _TRANSFORM_ERRORESTIMATION._serialized_end=4956
-  _TRANSFORM_FITMODEL._serialized_start=4958
-  _TRANSFORM_FITMODEL._serialized_end=5044
-  _TRANSFORM_TEXTKIND._serialized_start=5046
-  _TRANSFORM_TEXTKIND._serialized_end=5124
-  _TRANSFORM_CHAT._serialized_start=5126
-  _TRANSFORM_CHAT._serialized_end=5178
-  _TRANSFORM_FITMODELDP._serialized_start=5180
-  _TRANSFORM_FITMODELDP._serialized_end=5290
-  _TRANSFORM_GENERATEFROMMODEL._serialized_start=5292
-  _TRANSFORM_GENERATEFROMMODEL._serialized_end=5356
-  _TRANSFORM_SQLDIALECT._serialized_start=5359
-  _TRANSFORM_SQLDIALECT._serialized_end=5487
+  _TRANSFORM_SPEC._serialized_end=2240
+  _TRANSFORM_EXTERNAL._serialized_start=2243
+  _TRANSFORM_EXTERNAL._serialized_end=3257
+  _TRANSFORM_EXTERNAL_OPIDENTIFIER._serialized_start=2357
+  _TRANSFORM_EXTERNAL_OPIDENTIFIER._serialized_end=2956
+  _TRANSFORM_EXTERNAL_STD._serialized_start=2958
+  _TRANSFORM_EXTERNAL_STD._serialized_end=2977
+  _TRANSFORM_EXTERNAL_PANDAS._serialized_start=2979
+  _TRANSFORM_EXTERNAL_PANDAS._serialized_end=3001
+  _TRANSFORM_EXTERNAL_NUMPY._serialized_start=3003
+  _TRANSFORM_EXTERNAL_NUMPY._serialized_end=3024
+  _TRANSFORM_EXTERNAL_TENSORFLOW._serialized_start=3026
+  _TRANSFORM_EXTERNAL_TENSORFLOW._serialized_end=3052
+  _TRANSFORM_EXTERNAL_SKLEARN._serialized_start=3054
+  _TRANSFORM_EXTERNAL_SKLEARN._serialized_end=3077
+  _TRANSFORM_EXTERNAL_PANDASPROFILING._serialized_start=3079
+  _TRANSFORM_EXTERNAL_PANDASPROFILING._serialized_end=3110
+  _TRANSFORM_EXTERNAL_XGBOOST._serialized_start=3112
+  _TRANSFORM_EXTERNAL_XGBOOST._serialized_end=3135
+  _TRANSFORM_EXTERNAL_SKOPT._serialized_start=3137
+  _TRANSFORM_EXTERNAL_SKOPT._serialized_end=3158
+  _TRANSFORM_EXTERNAL_IMBLEARN._serialized_start=3160
+  _TRANSFORM_EXTERNAL_IMBLEARN._serialized_end=3184
+  _TRANSFORM_EXTERNAL_SHAP._serialized_start=3186
+  _TRANSFORM_EXTERNAL_SHAP._serialized_end=3206
+  _TRANSFORM_EXTERNAL_SCIPY._serialized_start=3208
+  _TRANSFORM_EXTERNAL_SCIPY._serialized_end=3229
+  _TRANSFORM_EXTERNAL_OPTBINNING._serialized_start=3231
+  _TRANSFORM_EXTERNAL_OPTBINNING._serialized_end=3257
+  _TRANSFORM_IDENTITY._serialized_start=3259
+  _TRANSFORM_IDENTITY._serialized_end=3269
+  _TRANSFORM_VARIABLE._serialized_start=3271
+  _TRANSFORM_VARIABLE._serialized_end=3313
+  _TRANSFORM_COMPOSED._serialized_start=3316
+  _TRANSFORM_COMPOSED._serialized_end=3485
+  _TRANSFORM_COMPOSED_NAMEDARGUMENTSENTRY._serialized_start=3432
+  _TRANSFORM_COMPOSED_NAMEDARGUMENTSENTRY._serialized_end=3485
+  _TRANSFORM_PROJECT._serialized_start=3487
+  _TRANSFORM_PROJECT._serialized_end=3539
+  _TRANSFORM_FILTER._serialized_start=3541
+  _TRANSFORM_FILTER._serialized_end=3588
+  _TRANSFORM_SHUFFLE._serialized_start=3590
+  _TRANSFORM_SHUFFLE._serialized_end=3599
+  _TRANSFORM_JOIN._serialized_start=3601
+  _TRANSFORM_JOIN._serialized_end=3642
+  _TRANSFORM_CAST._serialized_start=3644
+  _TRANSFORM_CAST._serialized_end=3687
+  _TRANSFORM_SAMPLE._serialized_start=3689
+  _TRANSFORM_SAMPLE._serialized_end=3786
+  _TRANSFORM_SCHEMAINFERENCE._serialized_start=3788
+  _TRANSFORM_SCHEMAINFERENCE._serialized_end=3906
+  _TRANSFORM_SCHEMAINFERENCE_CASTPOLICY._serialized_start=3867
+  _TRANSFORM_SCHEMAINFERENCE_CASTPOLICY._serialized_end=3906
+  _TRANSFORM_GROUPBY._serialized_start=3908
+  _TRANSFORM_GROUPBY._serialized_end=3930
+  _TRANSFORM_TOSMALLDATA._serialized_start=3932
+  _TRANSFORM_TOSMALLDATA._serialized_end=4023
+  _TRANSFORM_PUSHSQL._serialized_start=4025
+  _TRANSFORM_PUSHSQL._serialized_end=4117
+  _TRANSFORM_SYNTHETIC._serialized_start=4119
+  _TRANSFORM_SYNTHETIC._serialized_end=4130
+  _TRANSFORM_USERSETTINGS._serialized_start=4132
+  _TRANSFORM_USERSETTINGS._serialized_end=4146
+  _TRANSFORM_AUTOMATICUSERSETTINGS._serialized_start=4148
+  _TRANSFORM_AUTOMATICUSERSETTINGS._serialized_end=4195
+  _TRANSFORM_PRIVACYUNITTRACKING._serialized_start=4197
+  _TRANSFORM_PRIVACYUNITTRACKING._serialized_end=4218
+  _TRANSFORM_TRANSCODE._serialized_start=4220
+  _TRANSFORM_TRANSCODE._serialized_end=4231
+  _TRANSFORM_INVERSETRANSCODE._serialized_start=4233
+  _TRANSFORM_INVERSETRANSCODE._serialized_end=4251
+  _TRANSFORM_DIFFERENTIATEDSAMPLE._serialized_start=4253
+  _TRANSFORM_DIFFERENTIATEDSAMPLE._serialized_end=4364
+  _TRANSFORM_PRIVACYUNITTRACKINGPATHS._serialized_start=4366
+  _TRANSFORM_PRIVACYUNITTRACKINGPATHS._serialized_end=4392
+  _TRANSFORM_PUBLICPATHS._serialized_start=4394
+  _TRANSFORM_PUBLICPATHS._serialized_end=4407
+  _TRANSFORM_GETITEM._serialized_start=4409
+  _TRANSFORM_GETITEM._serialized_end=4455
+  _TRANSFORM_ASSIGNBUDGET._serialized_start=4457
+  _TRANSFORM_ASSIGNBUDGET._serialized_end=4471
+  _TRANSFORM_AUTOMATICBUDGET._serialized_start=4473
+  _TRANSFORM_AUTOMATICBUDGET._serialized_end=4490
+  _TRANSFORM_ATTRIBUTESBUDGET._serialized_start=4492
+  _TRANSFORM_ATTRIBUTESBUDGET._serialized_end=4510
+  _TRANSFORM_SDBUDGET._serialized_start=4512
+  _TRANSFORM_SDBUDGET._serialized_end=4522
+  _TRANSFORM_DERIVESEED._serialized_start=4524
+  _TRANSFORM_DERIVESEED._serialized_end=4560
+  _TRANSFORM_GROUPBYPE._serialized_start=4562
+  _TRANSFORM_GROUPBYPE._serialized_end=4573
+  _TRANSFORM_SAMPLINGRATIOS._serialized_start=4575
+  _TRANSFORM_SAMPLINGRATIOS._serialized_end=4591
+  _TRANSFORM_RELATIONSHIPSPEC._serialized_start=4593
+  _TRANSFORM_RELATIONSHIPSPEC._serialized_end=4611
+  _TRANSFORM_SELECTSQL._serialized_start=4614
+  _TRANSFORM_SELECTSQL._serialized_end=4750
+  _TRANSFORM_DPSELECTSQL._serialized_start=4753
+  _TRANSFORM_DPSELECTSQL._serialized_end=4891
+  _TRANSFORM_ALIASEDQUERIES._serialized_start=4893
+  _TRANSFORM_ALIASEDQUERIES._serialized_end=4957
+  _TRANSFORM_ALIASEDQUERY._serialized_start=4959
+  _TRANSFORM_ALIASEDQUERY._serialized_end=5025
+  _TRANSFORM_EXTRACT._serialized_start=5027
+  _TRANSFORM_EXTRACT._serialized_end=5050
+  _TRANSFORM_VALIDATEDUSERTYPE._serialized_start=5052
+  _TRANSFORM_VALIDATEDUSERTYPE._serialized_end=5071
+  _TRANSFORM_ERRORESTIMATION._serialized_start=5073
+  _TRANSFORM_ERRORESTIMATION._serialized_end=5090
+  _TRANSFORM_FITMODEL._serialized_start=5092
+  _TRANSFORM_FITMODEL._serialized_end=5178
+  _TRANSFORM_TEXTKIND._serialized_start=5180
+  _TRANSFORM_TEXTKIND._serialized_end=5258
+  _TRANSFORM_CHAT._serialized_start=5260
+  _TRANSFORM_CHAT._serialized_end=5312
+  _TRANSFORM_FITMODELDP._serialized_start=5314
+  _TRANSFORM_FITMODELDP._serialized_end=5424
+  _TRANSFORM_GENERATEFROMMODEL._serialized_start=5426
+  _TRANSFORM_GENERATEFROMMODEL._serialized_end=5490
+  _TRANSFORM_SQLDIALECT._serialized_start=5493
+  _TRANSFORM_SQLDIALECT._serialized_end=5621
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/transform_pb2.pyi` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/transform_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,15 @@
         VALIDATED_USER_TYPE_FIELD_NUMBER: builtins.int
         DP_SELECT_SQL_FIELD_NUMBER: builtins.int
         ERROR_ESTIMATION_FIELD_NUMBER: builtins.int
         FIT_MODEL_FIELD_NUMBER: builtins.int
         FIT_MODEL_DP_FIELD_NUMBER: builtins.int
         GENERATE_FROM_MODEL_FIELD_NUMBER: builtins.int
         TO_SMALL_DATA_FIELD_NUMBER: builtins.int
+        PUSH_SQL_FIELD_NUMBER: builtins.int
         @property
         def identity(self) -> global___Transform.Identity: ...
         @property
         def variable(self) -> global___Transform.Variable: ...
         @property
         def composed(self) -> global___Transform.Composed: ...
         @property
@@ -171,14 +172,16 @@
         def fit_model(self) -> global___Transform.FitModel: ...
         @property
         def fit_model_dp(self) -> global___Transform.FitModelDP: ...
         @property
         def generate_from_model(self) -> global___Transform.GenerateFromModel: ...
         @property
         def to_small_data(self) -> global___Transform.ToSmallData: ...
+        @property
+        def push_sql(self) -> global___Transform.PushSQL: ...
         def __init__(self,
             *,
             identity : typing.Optional[global___Transform.Identity] = ...,
             variable : typing.Optional[global___Transform.Variable] = ...,
             composed : typing.Optional[global___Transform.Composed] = ...,
             project : typing.Optional[global___Transform.Project] = ...,
             filter : typing.Optional[global___Transform.Filter] = ...,
@@ -210,18 +213,19 @@
             validated_user_type : typing.Optional[global___Transform.ValidatedUserType] = ...,
             dp_select_sql : typing.Optional[global___Transform.DPSelectSql] = ...,
             error_estimation : typing.Optional[global___Transform.ErrorEstimation] = ...,
             fit_model : typing.Optional[global___Transform.FitModel] = ...,
             fit_model_dp : typing.Optional[global___Transform.FitModelDP] = ...,
             generate_from_model : typing.Optional[global___Transform.GenerateFromModel] = ...,
             to_small_data : typing.Optional[global___Transform.ToSmallData] = ...,
+            push_sql : typing.Optional[global___Transform.PushSQL] = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["assign_budget",b"assign_budget","attribute_budget",b"attribute_budget","automatic_budget",b"automatic_budget","automatic_user_settings",b"automatic_user_settings","cast",b"cast","composed",b"composed","derive_seed",b"derive_seed","differentiated_sample",b"differentiated_sample","dp_select_sql",b"dp_select_sql","error_estimation",b"error_estimation","external",b"external","extract",b"extract","filter",b"filter","fit_model",b"fit_model","fit_model_dp",b"fit_model_dp","generate_from_model",b"generate_from_model","get_item",b"get_item","group_by_pe",b"group_by_pe","identity",b"identity","inverse_transcode",b"inverse_transcode","join",b"join","privacy_unit_tracking",b"privacy_unit_tracking","privacy_unit_tracking_paths",b"privacy_unit_tracking_paths","project",b"project","public_paths",b"public_paths","relationship_spec",b"relationship_spec","sample",b"sample","sampling_ratios",b"sampling_ratios","sd_budget",b"sd_budget","select_sql",b"select_sql","shuffle",b"shuffle","spec",b"spec","synthetic",b"synthetic","to_small_data",b"to_small_data","transcode",b"transcode","user_settings",b"user_settings","validated_user_type",b"validated_user_type","variable",b"variable"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["assign_budget",b"assign_budget","attribute_budget",b"attribute_budget","automatic_budget",b"automatic_budget","automatic_user_settings",b"automatic_user_settings","cast",b"cast","composed",b"composed","derive_seed",b"derive_seed","differentiated_sample",b"differentiated_sample","dp_select_sql",b"dp_select_sql","error_estimation",b"error_estimation","external",b"external","extract",b"extract","filter",b"filter","fit_model",b"fit_model","fit_model_dp",b"fit_model_dp","generate_from_model",b"generate_from_model","get_item",b"get_item","group_by_pe",b"group_by_pe","identity",b"identity","inverse_transcode",b"inverse_transcode","join",b"join","privacy_unit_tracking",b"privacy_unit_tracking","privacy_unit_tracking_paths",b"privacy_unit_tracking_paths","project",b"project","public_paths",b"public_paths","relationship_spec",b"relationship_spec","sample",b"sample","sampling_ratios",b"sampling_ratios","sd_budget",b"sd_budget","select_sql",b"select_sql","shuffle",b"shuffle","spec",b"spec","synthetic",b"synthetic","to_small_data",b"to_small_data","transcode",b"transcode","user_settings",b"user_settings","validated_user_type",b"validated_user_type","variable",b"variable"]) -> None: ...
-        def WhichOneof(self, oneof_group: typing_extensions.Literal["spec",b"spec"]) -> typing.Optional[typing_extensions.Literal["identity","variable","composed","project","filter","shuffle","join","cast","sample","user_settings","privacy_unit_tracking","external","synthetic","transcode","inverse_transcode","get_item","privacy_unit_tracking_paths","automatic_user_settings","public_paths","assign_budget","automatic_budget","attribute_budget","sd_budget","derive_seed","group_by_pe","sampling_ratios","select_sql","extract","relationship_spec","differentiated_sample","validated_user_type","dp_select_sql","error_estimation","fit_model","fit_model_dp","generate_from_model","to_small_data"]]: ...
+        def HasField(self, field_name: typing_extensions.Literal["assign_budget",b"assign_budget","attribute_budget",b"attribute_budget","automatic_budget",b"automatic_budget","automatic_user_settings",b"automatic_user_settings","cast",b"cast","composed",b"composed","derive_seed",b"derive_seed","differentiated_sample",b"differentiated_sample","dp_select_sql",b"dp_select_sql","error_estimation",b"error_estimation","external",b"external","extract",b"extract","filter",b"filter","fit_model",b"fit_model","fit_model_dp",b"fit_model_dp","generate_from_model",b"generate_from_model","get_item",b"get_item","group_by_pe",b"group_by_pe","identity",b"identity","inverse_transcode",b"inverse_transcode","join",b"join","privacy_unit_tracking",b"privacy_unit_tracking","privacy_unit_tracking_paths",b"privacy_unit_tracking_paths","project",b"project","public_paths",b"public_paths","push_sql",b"push_sql","relationship_spec",b"relationship_spec","sample",b"sample","sampling_ratios",b"sampling_ratios","sd_budget",b"sd_budget","select_sql",b"select_sql","shuffle",b"shuffle","spec",b"spec","synthetic",b"synthetic","to_small_data",b"to_small_data","transcode",b"transcode","user_settings",b"user_settings","validated_user_type",b"validated_user_type","variable",b"variable"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["assign_budget",b"assign_budget","attribute_budget",b"attribute_budget","automatic_budget",b"automatic_budget","automatic_user_settings",b"automatic_user_settings","cast",b"cast","composed",b"composed","derive_seed",b"derive_seed","differentiated_sample",b"differentiated_sample","dp_select_sql",b"dp_select_sql","error_estimation",b"error_estimation","external",b"external","extract",b"extract","filter",b"filter","fit_model",b"fit_model","fit_model_dp",b"fit_model_dp","generate_from_model",b"generate_from_model","get_item",b"get_item","group_by_pe",b"group_by_pe","identity",b"identity","inverse_transcode",b"inverse_transcode","join",b"join","privacy_unit_tracking",b"privacy_unit_tracking","privacy_unit_tracking_paths",b"privacy_unit_tracking_paths","project",b"project","public_paths",b"public_paths","push_sql",b"push_sql","relationship_spec",b"relationship_spec","sample",b"sample","sampling_ratios",b"sampling_ratios","sd_budget",b"sd_budget","select_sql",b"select_sql","shuffle",b"shuffle","spec",b"spec","synthetic",b"synthetic","to_small_data",b"to_small_data","transcode",b"transcode","user_settings",b"user_settings","validated_user_type",b"validated_user_type","variable",b"variable"]) -> None: ...
+        def WhichOneof(self, oneof_group: typing_extensions.Literal["spec",b"spec"]) -> typing.Optional[typing_extensions.Literal["identity","variable","composed","project","filter","shuffle","join","cast","sample","user_settings","privacy_unit_tracking","external","synthetic","transcode","inverse_transcode","get_item","privacy_unit_tracking_paths","automatic_user_settings","public_paths","assign_budget","automatic_budget","attribute_budget","sd_budget","derive_seed","group_by_pe","sampling_ratios","select_sql","extract","relationship_spec","differentiated_sample","validated_user_type","dp_select_sql","error_estimation","fit_model","fit_model_dp","generate_from_model","to_small_data","push_sql"]]: ...
 
     class External(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         class OpIdentifier(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             STD_FIELD_NUMBER: builtins.int
             PANDAS_FIELD_NUMBER: builtins.int
@@ -594,14 +598,33 @@
             size : builtins.int = ...,
             random_sampling : builtins.bool = ...,
             seed : typing.Optional[sarus_data_spec.protobuf.scalar_pb2.Scalar] = ...,
             ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["seed",b"seed"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["random_sampling",b"random_sampling","seed",b"seed","size",b"size"]) -> None: ...
 
+    class PushSQL(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+        DATACONNECTION_NAME_FIELD_NUMBER: builtins.int
+        SCHEMA_NAME_FIELD_NUMBER: builtins.int
+        TABLE_NAME_FIELD_NUMBER: builtins.int
+        URI_FIELD_NUMBER: builtins.int
+        dataconnection_name: typing.Text = ...
+        schema_name: typing.Text = ...
+        table_name: typing.Text = ...
+        uri: typing.Text = ...
+        def __init__(self,
+            *,
+            dataconnection_name : typing.Text = ...,
+            schema_name : typing.Text = ...,
+            table_name : typing.Text = ...,
+            uri : typing.Text = ...,
+            ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["dataconnection_name",b"dataconnection_name","schema_name",b"schema_name","table_name",b"table_name","uri",b"uri"]) -> None: ...
+
     class Synthetic(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         def __init__(self,
             ) -> None: ...
 
     class UserSettings(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
```

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/type.proto` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/type.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/type_pb2.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/type_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/type_pb2.pyi` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/typing.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/protobuf/utilities.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/utilities.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/scalar.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/scalar.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/schema.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/size.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/size.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/statistics.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/statistics.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/status.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/status.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/storage/local.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/storage/local.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/storage/typing.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/storage/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/storage/utils.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/storage/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/transform.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import datetime
 import json
 import typing as t
 
 from sarus_data_spec.base import Referrable
 from sarus_data_spec.constants import (
     BIG_DATA_TASK,
-    BIG_DATA_THRESHOLD,
+    SAMPLE_SIZE_N_LINES,
     MODEL_PROPERTIES,
 )
 from sarus_data_spec.context import global_context
 from sarus_data_spec.json_serialisation import SarusJSONEncoder
 from sarus_data_spec.path import straight_path
 import sarus_data_spec.dataset as sd
 import sarus_data_spec.protobuf as sp
@@ -494,21 +494,20 @@
     return msg
 
 
 def transform_id(transform: st.Transform) -> str:
     """Return the transform id."""
     spec = transform.protobuf().spec
     spec_type = str(spec.WhichOneof("spec"))
-
-    if spec_type != "external":
-        return spec_type
-    else:
+    if spec_type == "external":
         library = str(spec.external.op_identifier.WhichOneof("op"))
         op_name = getattr(spec.external.op_identifier, library).name
         return f"{library}.{op_name}"
+    else:
+        return spec_type
 
 
 def external(
     id: str,
     py_args: t.Optional[t.Dict[int, t.Any]] = None,
     py_kwargs: t.Optional[t.Dict[str, t.Any]] = None,
     ds_args_pos: t.Optional[t.List[int]] = None,
@@ -898,14 +897,34 @@
             ),
             inversible=False,
             schema_preserving=True,
         )
     )
 
 
+def push_sql(
+    dataconnection_name: str, schema_name: str, table_name: str, uri: str
+) -> Transform:
+    return Transform(
+        sp.Transform(
+            name="push_sql",
+            spec=sp.Transform.Spec(
+                push_sql=sp.Transform.PushSQL(
+                    dataconnection_name=dataconnection_name,
+                    schema_name=schema_name,
+                    table_name=table_name,
+                    uri=uri,
+                )
+            ),
+            inversible=True,
+            schema_preserving=True,
+        )
+    )
+
+
 def handle_big_data_from_name(code_name: str) -> bool:
     """
     Check if the transform with name codename can handle bigdata in SQL.
     """
     if code_name in [
         "assign_budget",
         "differentiated_sample",
@@ -940,22 +959,25 @@
     manager = dataspec.manager()
 
     if manager.is_big_data(dataspec) and (
         code_name is None or not handle_big_data_from_name(code_name)
     ):
         status = manager.status(dataspec, task_name=BIG_DATA_TASK)
         assert status
-        big_data_threshold = int(
-            status.task(BIG_DATA_TASK).properties()[BIG_DATA_THRESHOLD]  # type:ignore
+        # This could be improved by taking the threshold in bytes,
+        # measuring the size of one row and
+        # guessing the numbers of rows we can fetch.
+        big_data_threshold_lines = int(
+            status.task(BIG_DATA_TASK).properties()[SAMPLE_SIZE_N_LINES]  # type:ignore
         )
         seed = global_context().generate_seed()
         small_dataspec = t.cast(
             st.DataSpec,
             to_small_data(
-                size=big_data_threshold,
+                size=big_data_threshold_lines,
                 random_sampling=random_sampling,
                 seed=seed,
             )(dataspec),
         )
     else:
         small_dataspec = dataspec
     return small_dataspec
```

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/type.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/type.py`

 * *Files 0% similar despite different names*

```diff
@@ -2798,16 +2798,16 @@
             ),
             properties=properties,
         )
     )
 
 
 def Float(
-    min: t.Optional[float] = np.finfo(np.float64).min,  # type:ignore
-    max: t.Optional[float] = np.finfo(np.float64).max,  # type:ignore
+    min: t.Optional[float] = None,
+    max: t.Optional[float] = None,
     base: t.Optional[st.FloatBase] = None,
     possible_values: t.Optional[t.Iterable[float]] = None,
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Type:
     if base is None:
         base = st.FloatBase.FLOAT64
     if min is None:
@@ -3374,20 +3374,22 @@
             **protection_fields,
         }
         return Struct(fields=fields)
 
 
 def to_numeric_string(
     sds_type: st.Type,
-) -> t.Literal["int64", "int32", "int16", "int8", "float32", "float64"]:
+) -> t.Literal[
+    "int64", "int32", "int16", "int8", "float32", "float64", "boolean"
+]:
     class ToNumericString(st.TypeVisitor):
         """Visitor that converts sarus type to a string"""
 
         str_type: t.Literal[
-            "int64", "int32", "int16", "int8", "float32", "float64"
+            "int64", "int32", "int16", "int8", "float32", "float64", "boolean"
         ]
 
         def Integer(
             self,
             min: int,
             max: int,
             base: st.IntegerBase,
@@ -3462,15 +3464,15 @@
             properties: t.Optional[t.Mapping[str, str]] = None,
         ) -> None:
             raise NotImplementedError
 
         def Boolean(
             self, properties: t.Optional[t.Mapping[str, str]] = None
         ) -> None:
-            raise NotImplementedError
+            self.str_type = "boolean"
 
         def Bytes(
             self, properties: t.Optional[t.Mapping[str, str]] = None
         ) -> None:
             raise NotImplementedError
 
         def Unit(
```

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/typing.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/typing.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 
 
 # List of types a Dataset can be converted to
 DatasetCastable = t.Union[
     pd.DataFrame,
     pd.Series,
     t.Iterator[pa.RecordBatch],
+    t.AsyncIterator[pa.RecordBatch],
     pd.core.groupby.DataFrameGroupBy,
     pd.core.groupby.SeriesGroupBy,
 ]
 
 
 P = t.TypeVar("P", bound=Protobuf, covariant=True)
 
@@ -361,14 +362,16 @@
 
     async def async_to_arrow(
         self, batch_size: int = 10000
     ) -> t.AsyncIterator[pa.RecordBatch]: ...
 
     def to_sql(self) -> None: ...
 
+    def push_sql(self) -> None: ...
+
     def spec(self) -> str: ...
 
     def __iter__(self) -> t.Iterator[pa.RecordBatch]: ...
 
     def to_pandas(self) -> pd.DataFrame: ...
 
     async def async_to_pandas(self) -> pd.DataFrame: ...
```

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec/variant_constraint.py` & `sarus_data_spec_public-4.0.1/sarus_data_spec/variant_constraint.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec_public.egg-info/PKG-INFO` & `sarus_data_spec_public-4.0.1/sarus_data_spec_public.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus_data_spec_public
-Version: 4.0.0.dev7
+Version: 4.0.1
 Summary: A library to manage Sarus datasets
 Home-page: 
 Download-URL: 
 Author: Sarus Technologies
 Author-email: 
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sarus_data_spec_public-4.0.0.dev7/sarus_data_spec_public.egg-info/SOURCES.txt` & `sarus_data_spec_public-4.0.1/sarus_data_spec_public.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,15 @@
 sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
 sarus_data_spec/manager/ops/processor/standard/error_estimation.py
 sarus_data_spec/manager/ops/processor/standard/extract.py
 sarus_data_spec/manager/ops/processor/standard/filter.py
 sarus_data_spec/manager/ops/processor/standard/generate_from_model.py
 sarus_data_spec/manager/ops/processor/standard/get_item.py
 sarus_data_spec/manager/ops/processor/standard/project.py
+sarus_data_spec/manager/ops/processor/standard/push_sql.py
 sarus_data_spec/manager/ops/processor/standard/sample.py
 sarus_data_spec/manager/ops/processor/standard/shuffle.py
 sarus_data_spec/manager/ops/processor/standard/standard_op.py
 sarus_data_spec/manager/ops/processor/standard/synthetic.py
 sarus_data_spec/manager/ops/processor/standard/to_small_data.py
 sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
 sarus_data_spec/manager/ops/processor/standard/sampling/__init__.py
```

### Comparing `sarus_data_spec_public-4.0.0.dev7/setup.cfg` & `sarus_data_spec_public-4.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 	sarus_data_spec.manager.ops.processor.standard.differentiated_sample
 	sarus_data_spec.manager.ops.processor.standard.extract
 	sarus_data_spec.manager.ops.processor.standard.shuffle
 	sarus_data_spec.manager.ops.processor.standard.synthetic
 	sarus_data_spec.manager.ops.processor.standard.generate_from_model
 	sarus_data_spec.manager.ops.processor.standard.error_estimation
 	sarus_data_spec.manager.ops.processor.standard.to_small_data
+	sarus_data_spec.manager.ops.processor.standard.push_sql
 	sarus_data_spec.manager.ops.processor.external.external_op
 	sarus_data_spec.manager.ops.processor.external.imblearn
 	sarus_data_spec.manager.ops.processor.external.numpy
 	sarus_data_spec.manager.ops.processor.external.pandas.groupby
 	sarus_data_spec.manager.ops.processor.external.pandas.groupby_dp
 	sarus_data_spec.manager.ops.processor.external.pandas.pandas
 	sarus_data_spec.manager.ops.processor.external.pandas.pandas_dp
```

### Comparing `sarus_data_spec_public-4.0.0.dev7/setup.py` & `sarus_data_spec_public-4.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 
     def run(self):
         generate_proto_code()
         build_py.run(self)
 
 
 if __name__ == "__main__":
-    setup(version="4.0.0.dev7")
+    setup(version="4.0.1")
```

