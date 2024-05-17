# Comparing `tmp/skpro-2.2.2.tar.gz` & `tmp/skpro-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skpro-2.2.2.tar", last modified: Sat Apr 20 18:35:59 2024, max compression
+gzip compressed data, was "skpro-2.3.0.tar", last modified: Thu May 16 22:42:03 2024, max compression
```

## Comparing `skpro-2.2.2.tar` & `skpro-2.3.0.tar`

### file list

```diff
@@ -1,273 +1,284 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.235070 skpro-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-20 18:35:52.000000 skpro-2.2.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-20 18:35:52.000000 skpro-2.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15900 2024-04-20 18:35:59.235070 skpro-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12298 2024-04-20 18:35:52.000000 skpro-2.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.207069 skpro-2.2.2/build_tools/
--rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-04-20 18:35:52.000000 skpro-2.2.2/build_tools/changelog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.199069 skpro-2.2.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.207069 skpro-2.2.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     9914 2024-04-20 18:35:52.000000 skpro-2.2.2/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.207069 skpro-2.2.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-20 18:35:52.000000 skpro-2.2.2/examples/custom_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.207069 skpro-2.2.2/examples/parametric/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-20 18:35:52.000000 skpro-2.2.2/examples/parametric/bagging.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-20 18:35:52.000000 skpro-2.2.2/examples/parametric/hyperparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-20 18:35:52.000000 skpro-2.2.2/examples/parametric/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-20 18:35:52.000000 skpro-2.2.2/examples/parametric/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-20 18:35:52.000000 skpro-2.2.2/examples/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.207069 skpro-2.2.2/examples/vendors/
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-20 18:35:52.000000 skpro-2.2.2/examples/vendors/pymc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-20 18:35:52.000000 skpro-2.2.2/examples/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.207069 skpro-2.2.2/extension_templates/
--rw-r--r--   0 runner    (1001) docker     (127)    15039 2024-04-20 18:35:52.000000 skpro-2.2.2/extension_templates/regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    14400 2024-04-20 18:35:52.000000 skpro-2.2.2/extension_templates/survival.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-20 18:35:52.000000 skpro-2.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-20 18:35:59.235070 skpro-2.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.207069 skpro-2.2.2/skpro/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.207069 skpro-2.2.2/skpro/base/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/base/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    22066 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/base/old_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.207069 skpro-2.2.2/skpro/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/benchmarking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/benchmarking/evaluate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.211069 skpro-2.2.2/skpro/benchmarking/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/benchmarking/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/benchmarking/tests/test_evaluate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.211069 skpro-2.2.2/skpro/datatypes/
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.211069 skpro-2.2.2/skpro/datatypes/_adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_adapter/polars.py
--rw-r--r--   0 runner    (1001) docker     (127)    20992 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11557 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.211069 skpro-2.2.2/skpro/datatypes/_convert_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_convert_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_convert_utils/_coerce.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_convert_utils/_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.211069 skpro-2.2.2/skpro/datatypes/_proba/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_proba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_proba/_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_proba/_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_proba/_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_proba/_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.211069 skpro-2.2.2/skpro/datatypes/_table/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9939 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_table/_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_table/_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_table/_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/_table/_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.211069 skpro-2.2.2/skpro/datatypes/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/tests/test_convert_to.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/datatypes/tests/test_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.215069 skpro-2.2.2/skpro/distributions/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.215069 skpro-2.2.2/skpro/distributions/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.215069 skpro-2.2.2/skpro/distributions/adapters/scipy/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/adapters/scipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/adapters/scipy/_empirical.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.215069 skpro-2.2.2/skpro/distributions/adapters/scipy/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/adapters/scipy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/adapters/scipy/tests/test_scipy_adapters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.215069 skpro-2.2.2/skpro/distributions/adapters/statsmodels/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/adapters/statsmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/adapters/statsmodels/_empirical.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.215069 skpro-2.2.2/skpro/distributions/base/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27660 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/base/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/base/_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14689 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/empirical.py
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/fisk.py
--rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/laplace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/logistic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/lognormal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6595 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/mixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/poisson.py
--rw-r--r--   0 runner    (1001) docker     (127)    24128 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/qpd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6288 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/qpd_empirical.py
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/t.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.215069 skpro-2.2.2/skpro/distributions/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/tests/test_all_distrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/tests/test_base_default_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/tests/test_proba_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/tests/test_qpd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/distributions/weibull.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.215069 skpro-2.2.2/skpro/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16917 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/metrics/_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/metrics/_coerce.py
--rw-r--r--   0 runner    (1001) docker     (127)    18539 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/metrics/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.219069 skpro-2.2.2/skpro/metrics/survival/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/metrics/survival/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/metrics/survival/_c_harrell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/metrics/survival/_spll.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.219069 skpro-2.2.2/skpro/metrics/survival/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/metrics/survival/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/metrics/survival/tests/test_c_harrell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.219069 skpro-2.2.2/skpro/metrics/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/metrics/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/metrics/tests/test_distr_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/metrics/tests/test_probabilistic_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.219069 skpro-2.2.2/skpro/model_selection/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30439 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/model_selection/_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.219069 skpro-2.2.2/skpro/registry/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12805 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/registry/_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/registry/_scitype.py
--rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/registry/_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.219069 skpro-2.2.2/skpro/registry/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/registry/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/registry/tests/test_scitype.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/registry/tests/test_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.219069 skpro-2.2.2/skpro/regression/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.219069 skpro-2.2.2/skpro/regression/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.219069 skpro-2.2.2/skpro/regression/adapters/sklearn/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/adapters/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/adapters/sklearn/_sklearn_proba.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.219069 skpro-2.2.2/skpro/regression/base/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30706 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/base/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/base/_delegate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.223070 skpro-2.2.2/skpro/regression/base/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/base/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/base/adapters/_sklearn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.223070 skpro-2.2.2/skpro/regression/baselines/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/baselines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/baselines/density.py
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.223070 skpro-2.2.2/skpro/regression/compose/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/compose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21530 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/compose/_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    16701 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/cyclic_boosting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/density.py
--rw-r--r--   0 runner    (1001) docker     (127)     8251 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.223070 skpro-2.2.2/skpro/regression/gp/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/gp/_sklearn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.223070 skpro-2.2.2/skpro/regression/linear/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14211 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/linear/_glm.py
--rw-r--r--   0 runner    (1001) docker     (127)    11986 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/linear/_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14030 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/mapie.py
--rw-r--r--   0 runner    (1001) docker     (127)    13604 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/multiquantile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.223070 skpro-2.2.2/skpro/regression/parametric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/parametric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/parametric/estimators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8750 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/parametric/parametric.py
--rw-r--r--   0 runner    (1001) docker     (127)    14702 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/residual.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.223070 skpro-2.2.2/skpro/regression/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/tests/test_all_regressors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/tests/test_cyclic_boosting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.223070 skpro-2.2.2/skpro/regression/vendors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/vendors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/regression/vendors/pymc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.223070 skpro-2.2.2/skpro/survival/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.223070 skpro-2.2.2/skpro/survival/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/adapters/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/adapters/lifelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/adapters/sksurv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.223070 skpro-2.2.2/skpro/survival/additive/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/additive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/additive/_aalen_lifelines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.227069 skpro-2.2.2/skpro/survival/aft/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/aft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/aft/_aft_lifelines_fisk.py
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/aft/_aft_lifelines_lognormal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7636 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/aft/_aft_lifelines_weibull.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.227069 skpro-2.2.2/skpro/survival/compose/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/compose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/compose/_reduce_cond_unc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/compose/_reduce_uncensored.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.227069 skpro-2.2.2/skpro/survival/coxph/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/coxph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/coxph/_coxnet_sksurv.py
--rw-r--r--   0 runner    (1001) docker     (127)     8646 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/coxph/_coxph_lifelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/coxph/_coxph_sksurv.py
--rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/coxph/_coxph_statsmodels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.227069 skpro-2.2.2/skpro/survival/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19654 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/ensemble/_grad_boost_sksurv.py
--rw-r--r--   0 runner    (1001) docker     (127)    16778 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/ensemble/_survforest_sksurv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.227069 skpro-2.2.2/skpro/survival/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/survival/tree/_tree_sksurv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.227069 skpro-2.2.2/skpro/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.227069 skpro-2.2.2/skpro/tests/scenarios/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/scenarios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10341 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/scenarios/scenarios.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/scenarios/scenarios_getter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/scenarios/scenarios_regressor_proba.py
--rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/test_all_estimators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/test_baselines.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/test_class_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/test_density.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/test_vendors.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.231070 skpro-2.2.2/skpro/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.231070 skpro-2.2.2/skpro/utils/_maint/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/_maint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/_maint/_show_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.231070 skpro-2.2.2/skpro/utils/_maint/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/_maint/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/_maint/tests/test_show_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.231070 skpro-2.2.2/skpro/utils/deep_equals/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/deep_equals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/deep_equals/_deep_equals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/estimator_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/git_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/index.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/random_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/sklearn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.231070 skpro-2.2.2/skpro/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/tests/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.231070 skpro-2.2.2/skpro/utils/validation/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14906 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/utils/validation/_dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.231070 skpro-2.2.2/skpro/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/workflow/cross_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.231070 skpro-2.2.2/skpro/workflow/manager/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/workflow/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/workflow/manager/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/workflow/manager/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.231070 skpro-2.2.2/skpro/workflow/table/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/workflow/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/workflow/table/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-20 18:35:52.000000 skpro-2.2.2/skpro/workflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:35:59.231070 skpro-2.2.2/skpro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15900 2024-04-20 18:35:59.000000 skpro-2.2.2/skpro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-04-20 18:35:59.000000 skpro-2.2.2/skpro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:35:59.000000 skpro-2.2.2/skpro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-20 18:35:59.000000 skpro-2.2.2/skpro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-20 18:35:59.000000 skpro-2.2.2/skpro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:35:56.000000 skpro-2.2.2/skpro.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.415758 skpro-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-16 22:41:53.000000 skpro-2.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-16 22:41:53.000000 skpro-2.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16220 2024-05-16 22:42:03.415758 skpro-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-05-16 22:41:53.000000 skpro-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.383757 skpro-2.3.0/build_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-16 22:41:53.000000 skpro-2.3.0/build_tools/changelog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.379757 skpro-2.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.383757 skpro-2.3.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     9914 2024-05-16 22:41:53.000000 skpro-2.3.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.383757 skpro-2.3.0/extension_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    15567 2024-05-16 22:41:53.000000 skpro-2.3.0/extension_templates/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14948 2024-05-16 22:41:53.000000 skpro-2.3.0/extension_templates/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14309 2024-05-16 22:41:53.000000 skpro-2.3.0/extension_templates/survival.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-16 22:41:53.000000 skpro-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-16 22:42:03.419757 skpro-2.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.383757 skpro-2.3.0/skpro/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.387757 skpro-2.3.0/skpro/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/base/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22066 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/base/old_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.387757 skpro-2.3.0/skpro/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/benchmarking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/benchmarking/evaluate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.387757 skpro-2.3.0/skpro/benchmarking/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/benchmarking/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/benchmarking/tests/test_evaluate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.387757 skpro-2.3.0/skpro/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.387757 skpro-2.3.0/skpro/datatypes/_adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_adapter/polars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20992 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11559 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.387757 skpro-2.3.0/skpro/datatypes/_convert_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_convert_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_convert_utils/_coerce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_convert_utils/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.391757 skpro-2.3.0/skpro/datatypes/_proba/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_proba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_proba/_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_proba/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_proba/_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_proba/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.391757 skpro-2.3.0/skpro/datatypes/_table/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9939 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_table/_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_table/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_table/_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/_table/_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.391757 skpro-2.3.0/skpro/datatypes/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/tests/test_convert_to.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/datatypes/tests/test_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.391757 skpro-2.3.0/skpro/distributions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.395757 skpro-2.3.0/skpro/distributions/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.395757 skpro-2.3.0/skpro/distributions/adapters/scipy/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/adapters/scipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/adapters/scipy/_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/adapters/scipy/_empirical.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.395757 skpro-2.3.0/skpro/distributions/adapters/scipy/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/adapters/scipy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/adapters/scipy/tests/test_scipy_adapters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.395757 skpro-2.3.0/skpro/distributions/adapters/statsmodels/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/adapters/statsmodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/adapters/statsmodels/_empirical.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.395757 skpro-2.3.0/skpro/distributions/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68328 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/base/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/base/_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/beta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/chi_squared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21324 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/empirical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/exponential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/fisk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/laplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/logistic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/lognormal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/poisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25929 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/qpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6288 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/qpd_empirical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6955 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/t.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.395757 skpro-2.3.0/skpro/distributions/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/tests/test_all_distrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/tests/test_base_default_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/tests/test_base_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/tests/test_proba_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/tests/test_qpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/distributions/weibull.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.395757 skpro-2.3.0/skpro/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16917 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/metrics/_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/metrics/_coerce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22237 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/metrics/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.395757 skpro-2.3.0/skpro/metrics/survival/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/metrics/survival/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/metrics/survival/_c_harrell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/metrics/survival/_spll.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.395757 skpro-2.3.0/skpro/metrics/survival/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/metrics/survival/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/metrics/survival/tests/test_c_harrell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.395757 skpro-2.3.0/skpro/metrics/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/metrics/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/metrics/tests/test_distr_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/metrics/tests/test_probabilistic_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.399757 skpro-2.3.0/skpro/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30439 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/model_selection/_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.399757 skpro-2.3.0/skpro/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12805 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/registry/_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/registry/_scitype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/registry/_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.399757 skpro-2.3.0/skpro/registry/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/registry/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/registry/tests/test_scitype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/registry/tests/test_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.399757 skpro-2.3.0/skpro/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.399757 skpro-2.3.0/skpro/regression/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.399757 skpro-2.3.0/skpro/regression/adapters/ngboost/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/adapters/ngboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/adapters/ngboost/_ngboost_proba.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.399757 skpro-2.3.0/skpro/regression/adapters/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/adapters/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/adapters/sklearn/_sklearn_proba.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.399757 skpro-2.3.0/skpro/regression/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30706 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/base/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/base/_delegate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.399757 skpro-2.3.0/skpro/regression/base/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/base/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/base/adapters/_sklearn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.399757 skpro-2.3.0/skpro/regression/baselines/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/baselines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/baselines/density.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.403757 skpro-2.3.0/skpro/regression/compose/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/compose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21530 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/compose/_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20226 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/cyclic_boosting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/density.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.403757 skpro-2.3.0/skpro/regression/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8251 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/ensemble/_bagging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9237 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/ensemble/_ngboost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.403757 skpro-2.3.0/skpro/regression/gp/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/gp/_sklearn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.403757 skpro-2.3.0/skpro/regression/linear/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14211 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/linear/_glm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/linear/_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/linear/_sklearn_poisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14030 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/mapie.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13604 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/multiquantile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.403757 skpro-2.3.0/skpro/regression/parametric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/parametric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/parametric/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8750 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/parametric/parametric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14702 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/residual.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.403757 skpro-2.3.0/skpro/regression/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/tests/test_all_regressors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/tests/test_cyclic_boosting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.403757 skpro-2.3.0/skpro/regression/vendors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/vendors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/regression/vendors/pymc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.403757 skpro-2.3.0/skpro/survival/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.403757 skpro-2.3.0/skpro/survival/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/adapters/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/adapters/lifelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/adapters/sksurv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.403757 skpro-2.3.0/skpro/survival/additive/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/additive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/additive/_aalen_lifelines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.403757 skpro-2.3.0/skpro/survival/aft/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/aft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/aft/_aft_lifelines_fisk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/aft/_aft_lifelines_lognormal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7636 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/aft/_aft_lifelines_weibull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.407757 skpro-2.3.0/skpro/survival/compose/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/compose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/compose/_reduce_cond_unc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/compose/_reduce_uncensored.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.407757 skpro-2.3.0/skpro/survival/coxph/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/coxph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/coxph/_coxnet_sksurv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8646 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/coxph/_coxph_lifelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/coxph/_coxph_sksurv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/coxph/_coxph_statsmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.407757 skpro-2.3.0/skpro/survival/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19654 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/ensemble/_grad_boost_sksurv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8914 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/ensemble/_ngboost_surv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/ensemble/_survforest_sksurv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.407757 skpro-2.3.0/skpro/survival/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/survival/tree/_tree_sksurv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.407757 skpro-2.3.0/skpro/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/_config_test_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.407757 skpro-2.3.0/skpro/tests/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/scenarios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10341 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/scenarios/scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/scenarios/scenarios_getter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/scenarios/scenarios_regressor_proba.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16275 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/test_all_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/test_baselines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/test_class_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/test_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/test_vendors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.411758 skpro-2.3.0/skpro/tests/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/tests/test_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.411758 skpro-2.3.0/skpro/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.411758 skpro-2.3.0/skpro/utils/_maint/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/_maint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/_maint/_show_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.411758 skpro-2.3.0/skpro/utils/_maint/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/_maint/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/_maint/tests/test_show_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.411758 skpro-2.3.0/skpro/utils/deep_equals/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/deep_equals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/deep_equals/_deep_equals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/estimator_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/git_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/random_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/sklearn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.411758 skpro-2.3.0/skpro/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/tests/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.411758 skpro-2.3.0/skpro/utils/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14906 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/utils/validation/_dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.411758 skpro-2.3.0/skpro/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/workflow/cross_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.411758 skpro-2.3.0/skpro/workflow/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/workflow/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/workflow/manager/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/workflow/manager/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.415758 skpro-2.3.0/skpro/workflow/table/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/workflow/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/workflow/table/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-16 22:41:53.000000 skpro-2.3.0/skpro/workflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:42:03.415758 skpro-2.3.0/skpro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16220 2024-05-16 22:42:03.000000 skpro-2.3.0/skpro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-05-16 22:42:03.000000 skpro-2.3.0/skpro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 22:42:03.000000 skpro-2.3.0/skpro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-16 22:42:03.000000 skpro-2.3.0/skpro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 22:42:03.000000 skpro-2.3.0/skpro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 22:42:00.000000 skpro-2.3.0/skpro.egg-info/zip-safe
```

### Comparing `skpro-2.2.2/LICENSE.txt` & `skpro-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/PKG-INFO` & `skpro-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skpro
-Version: 2.2.2
+Version: 2.3.0
 Summary: A unified framework for probability distributions and probabilistic supervised regression
 Author: Franz Király, Frithjof Gressmann, Vitaly Davydov
 Author-email: skpro developers <sktime.toolbox@gmail.com>
 Maintainer: Franz Király, Frithjof Gressmann
 Maintainer-email: skpro developers <sktime.toolbox@gmail.com>
 Project-URL: Homepage, https://github.com/sktime/skpro
 Project-URL: Repository, https://github.com/sktime/skpro
@@ -36,26 +36,26 @@
 Requires-Dist: pandas<2.3.0,>=1.1.0
 Requires-Dist: packaging
 Requires-Dist: scikit-base<0.8.0,>=0.6.1
 Requires-Dist: scikit-learn<1.5.0,>=0.24.0
 Requires-Dist: scipy<2.0.0,>=1.2.0
 Provides-Extra: all-extras
 Requires-Dist: attrs; extra == "all-extras"
+Requires-Dist: cyclic-boosting>=1.4.0; python_version < "3.12" and extra == "all-extras"
 Requires-Dist: distfit; extra == "all-extras"
 Requires-Dist: lifelines<0.29.0; extra == "all-extras"
 Requires-Dist: mapie; extra == "all-extras"
 Requires-Dist: matplotlib>=3.3.2; extra == "all-extras"
-Requires-Dist: ngboost; extra == "all-extras"
+Requires-Dist: ngboost<0.6.0; extra == "all-extras"
 Requires-Dist: polars<0.21.0; extra == "all-extras"
 Requires-Dist: pyarrow<14.0.0; python_version < "3.12" and extra == "all-extras"
 Requires-Dist: scikit-survival<0.23.0; extra == "all-extras"
 Requires-Dist: statsmodels>=0.12.1; extra == "all-extras"
 Requires-Dist: tabulate; extra == "all-extras"
 Requires-Dist: uncertainties; extra == "all-extras"
-Requires-Dist: cyclic-boosting>=1.2.5; python_version < "3.12" and extra == "all-extras"
 Provides-Extra: dev
 Requires-Dist: backoff; extra == "dev"
 Requires-Dist: httpx; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-randomly; extra == "dev"
@@ -69,21 +69,21 @@
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: nbsphinx>=0.8.6; extra == "docs"
 Requires-Dist: numpydoc; extra == "docs"
 Requires-Dist: pydata-sphinx-theme; extra == "docs"
 Requires-Dist: sphinx!=7.2.0,<8.0.0; extra == "docs"
 Requires-Dist: sphinx-design<0.6.0; extra == "docs"
 Requires-Dist: sphinx-issues<5.0.0; extra == "docs"
-Requires-Dist: sphinx-gallery<0.16.0; extra == "docs"
+Requires-Dist: sphinx-gallery<0.17.0; extra == "docs"
 Requires-Dist: sphinx-panels; extra == "docs"
 Requires-Dist: tabulate; extra == "docs"
 
 <a href="https://skpro.readthedocs.io/en/latest"><img src="https://github.com/sktime/skpro/blob/main/docs/source/images/skpro-banner.png" width="500" align="right" /></a>
 
-:rocket: **Version 2.2.2 out now!** [Read the release notes here.](https://skpro.readthedocs.io/en/latest/changelog.html).
+:rocket: **Version 2.3.0 out now!** [Read the release notes here.](https://skpro.readthedocs.io/en/latest/changelog.html).
 
 `skpro` is a library for supervised probabilistic prediction in python.
 It provides `scikit-learn`-like, `scikit-base` compatible interfaces to:
 
 * tabular **supervised regressors for probabilistic prediction** - interval, quantile and distribution predictions
 * tabular **probabilistic time-to-event and survival prediction** - instance-individual survival distributions
 * **metrics to evaluate probabilistic predictions**, e.g., pinball loss, empirical coverage, CRPS, survival losses
@@ -94,15 +94,16 @@
 | Overview | |
 |---|---|
 | **Open Source** |  [![BSD 3-clause](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://github.com/sktime/sktime/blob/main/LICENSE) |
 | **Tutorials** | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sktime/skpro/main?filepath=examples) [![!youtube](https://img.shields.io/static/v1?logo=youtube&label=YouTube&message=tutorials&color=red)](https://www.youtube.com/playlist?list=PLKs3UgGjlWHqNzu0LEOeLKvnjvvest2d0) |
 | **Community** | [![!discord](https://img.shields.io/static/v1?logo=discord&label=discord&message=chat&color=lightgreen)](https://discord.com/invite/54ACzaFsn7) [![!slack](https://img.shields.io/static/v1?logo=linkedin&label=LinkedIn&message=news&color=lightblue)](https://www.linkedin.com/company/scikit-time/) |
 | **CI/CD** | [![github-actions](https://img.shields.io/github/actions/workflow/status/sktime/sktime/wheels.yml?logo=github)](https://github.com/sktime/skpro/actions/workflows/wheels.yml) [![!codecov](https://img.shields.io/codecov/c/github/sktime/skpro?label=codecov&logo=codecov)](https://codecov.io/gh/sktime/skpro) [![readthedocs](https://img.shields.io/readthedocs/skpro?logo=readthedocs)](https://skpro.readthedocs.io/en/latest/) [![platform](https://img.shields.io/conda/pn/conda-forge/skpro)](https://github.com/sktime/skpro) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/skpro?color=orange)](https://pypi.org/project/skpro/) [![!conda](https://img.shields.io/conda/vn/conda-forge/skpro)](https://anaconda.org/conda-forge/skpro) [![!python-versions](https://img.shields.io/pypi/pyversions/skpro)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) |
-| **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/skpro) |
+| **Downloads** | [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/skpro) |
+| **Citation** | [![DOI](https://zenodo.org/badge/103107372.svg)](https://zenodo.org/doi/10.5281/zenodo.11002671) |
 
 ## :books: Documentation
 
 | Documentation              |                                                                |
 | -------------------------- | -------------------------------------------------------------- |
 | :star: **[Tutorials]**        | New to skpro? Here's everything you need to know!              |
 | :clipboard: **[Binder Notebooks]** | Example notebooks to play with in your browser.              |
@@ -133,15 +134,15 @@
 | Type                            | Platforms                               |
 | ------------------------------- | --------------------------------------- |
 | :bug: **Bug Reports**              | [GitHub Issue Tracker]                  |
 | :sparkles: **Feature Requests & Ideas** | [GitHub Issue Tracker]                       |
 | :woman_technologist: **Usage Questions**          | [GitHub Discussions] · [Stack Overflow] |
 | :speech_balloon: **General Discussion**        | [GitHub Discussions] |
 | :factory: **Contribution & Development** | `dev-chat` channel · [Discord] |
-| :globe_with_meridians: **Community collaboration session** | [Discord] - Fridays 3 pm UTC, dev/meet-ups channel |
+| :globe_with_meridians: **Community collaboration session** | [Discord] - Fridays 13 UTC, dev/meet-ups channel |
 
 [github issue tracker]: https://github.com/sktime/skpro/issues
 [github discussions]: https://github.com/sktime/skpro/discussions
 [stack overflow]: https://stackoverflow.com/questions/tagged/sktime
 [discord]: https://discord.com/invite/54ACzaFsn7
 
 
@@ -163,15 +164,15 @@
 ``skpro`` curates libraries of components of the following types:
 
 | Module | Status | Links |
 |---|---|---|
 | **[Probabilistic tabular regression]** | maturing | [Tutorial](https://github.com/sktime/skpro/blob/main/examples/01_skpro_intro.ipynb) · [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/regression.html) · [Extension Template](https://github.com/sktime/skpro/blob/main/extension_templates/regression.py) |
 | **[Time-to-event (survival) prediction]** | experimental | [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/survival.html) · [Extension Template](https://github.com/sktime/skpro/blob/main/extension_templates/survival.py) |
 | **[Performance metrics]** | maturing | [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/metrics.html) |
-| **[Probability distributions]** | maturing | [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/distributions.html) |
+| **[Probability distributions]** | maturing | [Tutorial](https://github.com/sktime/skpro/blob/main/examples/03_skpro_distributions.ipynb) · [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/distributions.html) · [Extension Template](https://github.com/sktime/skpro/blob/main/extension_templates/distributions.py) |
 
 [Probabilistic tabular regression]: https://github.com/sktime/skpro/tree/main/skpro/regression
 [Time-to-event (survival) prediction]: https://github.com/sktime/skpro/tree/main/skpro/survival
 [Performance metrics]: https://github.com/sktime/skpro/tree/main/skpro/metrics
 [Probability distributions]: https://github.com/sktime/skpro/tree/main/skpro/distributions
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skpro Version: 2.2.2 Summary: A unified framework
+Metadata-Version: 2.1 Name: skpro Version: 2.3.0 Summary: A unified framework
 for probability distributions and probabilistic supervised regression Author:
 Franz KirÃ¡ly, Frithjof Gressmann, Vitaly Davydov Author-email: skpro
 developers
 gmail.com> Maintainer: Franz KirÃ¡ly, Frithjof Gressmann Maintainer-email:
 skpro developers
 gmail.com> Project-URL: Homepage, https://github.com/sktime/skpro Project-URL:
 Repository, https://github.com/sktime/skpro Project-URL: Documentation, https:/
@@ -20,55 +20,55 @@
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
 Python: <3.13,>=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.txt License-File: AUTHORS.rst Requires-Dist: numpy<1.27,>=1.21.0
 Requires-Dist: pandas<2.3.0,>=1.1.0 Requires-Dist: packaging Requires-Dist:
 scikit-base<0.8.0,>=0.6.1 Requires-Dist: scikit-learn<1.5.0,>=0.24.0 Requires-
 Dist: scipy<2.0.0,>=1.2.0 Provides-Extra: all-extras Requires-Dist: attrs;
-extra == "all-extras" Requires-Dist: distfit; extra == "all-extras" Requires-
-Dist: lifelines<0.29.0; extra == "all-extras" Requires-Dist: mapie; extra ==
-"all-extras" Requires-Dist: matplotlib>=3.3.2; extra == "all-extras" Requires-
-Dist: ngboost; extra == "all-extras" Requires-Dist: polars<0.21.0; extra ==
-"all-extras" Requires-Dist: pyarrow<14.0.0; python_version < "3.12" and extra
-== "all-extras" Requires-Dist: scikit-survival<0.23.0; extra == "all-extras"
-Requires-Dist: statsmodels>=0.12.1; extra == "all-extras" Requires-Dist:
-tabulate; extra == "all-extras" Requires-Dist: uncertainties; extra == "all-
-extras" Requires-Dist: cyclic-boosting>=1.2.5; python_version < "3.12" and
-extra == "all-extras" Provides-Extra: dev Requires-Dist: backoff; extra ==
-"dev" Requires-Dist: httpx; extra == "dev" Requires-Dist: pre-commit; extra ==
-"dev" Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-cov; extra ==
-"dev" Requires-Dist: pytest-randomly; extra == "dev" Requires-Dist: pytest-
-timeout; extra == "dev" Requires-Dist: pytest-xdist; extra == "dev" Requires-
-Dist: wheel; extra == "dev" Provides-Extra: binder Requires-Dist: jupyter;
-extra == "binder" Provides-Extra: docs Requires-Dist: jupyter; extra == "docs"
-Requires-Dist: myst-parser; extra == "docs" Requires-Dist: nbsphinx>=0.8.6;
-extra == "docs" Requires-Dist: numpydoc; extra == "docs" Requires-Dist: pydata-
-sphinx-theme; extra == "docs" Requires-Dist: sphinx!=7.2.0,<8.0.0; extra ==
-"docs" Requires-Dist: sphinx-design<0.6.0; extra == "docs" Requires-Dist:
-sphinx-issues<5.0.0; extra == "docs" Requires-Dist: sphinx-gallery<0.16.0;
-extra == "docs" Requires-Dist: sphinx-panels; extra == "docs" Requires-Dist:
-tabulate; extra == "docs" _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_s_k_t_i_m_e_/_s_k_p_r_o_/_b_l_o_b_/_m_a_i_n_/_d_o_c_s_/
-_s_o_u_r_c_e_/_i_m_a_g_e_s_/_s_k_p_r_o_-_b_a_n_n_e_r_._p_n_g_]:rocket: **Version 2.2.2 out now!** [Read the
-release notes here.](https://skpro.readthedocs.io/en/latest/changelog.html).
-`skpro` is a library for supervised probabilistic prediction in python. It
-provides `scikit-learn`-like, `scikit-base` compatible interfaces to: * tabular
-**supervised regressors for probabilistic prediction** - interval, quantile and
-distribution predictions * tabular **probabilistic time-to-event and survival
-prediction** - instance-individual survival distributions * **metrics to
-evaluate probabilistic predictions**, e.g., pinball loss, empirical coverage,
-CRPS, survival losses * **reductions** to turn `scikit-learn` regressors into
-probabilistic `skpro` regressors, such as bootstrap or conformal * building
-**pipelines and composite models**, including tuning via probabilistic
-performance metrics * symbolic **probability distributions** with value domain
-of `pandas.DataFrame`-s and `pandas`-like interface | Overview | | |---|---| |
-**Open Source** | [![BSD 3-clause](https://img.shields.io/badge/License-
-BSD%203--Clause-blue.svg)](https://github.com/sktime/sktime/blob/main/LICENSE)
-| | **Tutorials** | [![Binder](https://mybinder.org/badge_logo.svg)](https://
-mybinder.org/v2/gh/sktime/skpro/main?filepath=examples) [![!youtube](https://
-img.shields.io/static/
+extra == "all-extras" Requires-Dist: cyclic-boosting>=1.4.0; python_version <
+"3.12" and extra == "all-extras" Requires-Dist: distfit; extra == "all-extras"
+Requires-Dist: lifelines<0.29.0; extra == "all-extras" Requires-Dist: mapie;
+extra == "all-extras" Requires-Dist: matplotlib>=3.3.2; extra == "all-extras"
+Requires-Dist: ngboost<0.6.0; extra == "all-extras" Requires-Dist:
+polars<0.21.0; extra == "all-extras" Requires-Dist: pyarrow<14.0.0;
+python_version < "3.12" and extra == "all-extras" Requires-Dist: scikit-
+survival<0.23.0; extra == "all-extras" Requires-Dist: statsmodels>=0.12.1;
+extra == "all-extras" Requires-Dist: tabulate; extra == "all-extras" Requires-
+Dist: uncertainties; extra == "all-extras" Provides-Extra: dev Requires-Dist:
+backoff; extra == "dev" Requires-Dist: httpx; extra == "dev" Requires-Dist:
+pre-commit; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-Dist:
+pytest-cov; extra == "dev" Requires-Dist: pytest-randomly; extra == "dev"
+Requires-Dist: pytest-timeout; extra == "dev" Requires-Dist: pytest-xdist;
+extra == "dev" Requires-Dist: wheel; extra == "dev" Provides-Extra: binder
+Requires-Dist: jupyter; extra == "binder" Provides-Extra: docs Requires-Dist:
+jupyter; extra == "docs" Requires-Dist: myst-parser; extra == "docs" Requires-
+Dist: nbsphinx>=0.8.6; extra == "docs" Requires-Dist: numpydoc; extra == "docs"
+Requires-Dist: pydata-sphinx-theme; extra == "docs" Requires-Dist:
+sphinx!=7.2.0,<8.0.0; extra == "docs" Requires-Dist: sphinx-design<0.6.0; extra
+== "docs" Requires-Dist: sphinx-issues<5.0.0; extra == "docs" Requires-Dist:
+sphinx-gallery<0.17.0; extra == "docs" Requires-Dist: sphinx-panels; extra ==
+"docs" Requires-Dist: tabulate; extra == "docs" _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_s_k_t_i_m_e_/
+_s_k_p_r_o_/_b_l_o_b_/_m_a_i_n_/_d_o_c_s_/_s_o_u_r_c_e_/_i_m_a_g_e_s_/_s_k_p_r_o_-_b_a_n_n_e_r_._p_n_g_]:rocket: **Version 2.3.0
+out now!** [Read the release notes here.](https://skpro.readthedocs.io/en/
+latest/changelog.html). `skpro` is a library for supervised probabilistic
+prediction in python. It provides `scikit-learn`-like, `scikit-base` compatible
+interfaces to: * tabular **supervised regressors for probabilistic prediction**
+- interval, quantile and distribution predictions * tabular **probabilistic
+time-to-event and survival prediction** - instance-individual survival
+distributions * **metrics to evaluate probabilistic predictions**, e.g.,
+pinball loss, empirical coverage, CRPS, survival losses * **reductions** to
+turn `scikit-learn` regressors into probabilistic `skpro` regressors, such as
+bootstrap or conformal * building **pipelines and composite models**, including
+tuning via probabilistic performance metrics * symbolic **probability
+distributions** with value domain of `pandas.DataFrame`-s and `pandas`-like
+interface | Overview | | |---|---| | **Open Source** | [![BSD 3-clause](https:/
+/img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://github.com/
+sktime/sktime/blob/main/LICENSE) | | **Tutorials** | [![Binder](https://
+mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sktime/skpro/
+main?filepath=examples) [![!youtube](https://img.shields.io/static/
 v1?logo=youtube&label=YouTube&message=tutorials&color=red)](https://
 www.youtube.com/playlist?list=PLKs3UgGjlWHqNzu0LEOeLKvnjvvest2d0) | |
 **Community** | [![!discord](https://img.shields.io/static/
 v1?logo=discord&label=discord&message=chat&color=lightgreen)](https://
 discord.com/invite/54ACzaFsn7) [![!slack](https://img.shields.io/static/
 v1?logo=linkedin&label=LinkedIn&message=news&color=lightblue)](https://
 www.linkedin.com/company/scikit-time/) | | **CI/CD** | [![github-actions]
@@ -80,54 +80,55 @@
 (https://skpro.readthedocs.io/en/latest/) [![platform](https://img.shields.io/
 conda/pn/conda-forge/skpro)](https://github.com/sktime/skpro) | | **Code** | [!
 [!pypi](https://img.shields.io/pypi/v/skpro?color=orange)](https://pypi.org/
 project/skpro/) [![!conda](https://img.shields.io/conda/vn/conda-forge/skpro)]
 (https://anaconda.org/conda-forge/skpro) [![!python-versions](https://
 img.shields.io/pypi/pyversions/skpro)](https://www.python.org/) [![!black]
 (https://img.shields.io/badge/code%20style-black-000000.svg)](https://
-github.com/psf/black) | | **Downloads**| [![Downloads](https://
+github.com/psf/black) | | **Downloads** | [![Downloads](https://
 static.pepy.tech/personalized-badge/
 skpro?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20
 (pypi))](https://pepy.tech/project/skpro) [![Downloads](https://
 static.pepy.tech/personalized-badge/
 skpro?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20
 (pypi))](https://pepy.tech/project/skpro) [![Downloads](https://
 static.pepy.tech/personalized-badge/
 skpro?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20
-(pypi))](https://pepy.tech/project/skpro) | ## :books: Documentation |
-Documentation | | | -------------------------- | ------------------------------
--------------------------------- | | :star: **[Tutorials]** | New to skpro?
-Here's everything you need to know! | | :clipboard: **[Binder Notebooks]** |
-Example notebooks to play with in your browser. | | :woman_technologist: **
-[User Guides]** | How to use skpro and its features. | | :scissors: **
-[Extension Templates]** | How to build your own estimator using skpro's API. |
-| :control_knobs: **[API Reference]** | The detailed reference for skpro's API.
-| | :hammer_and_wrench: **[Changelog]** | Changes and version history. | | :
-deciduous_tree: **[Roadmap]** | skpro's software and community development
-plan. | | :pencil: **[Related Software]** | A list of related software. |
-[tutorials]: https://skpro.readthedocs.io/en/latest/tutorials.html [binder
-notebooks]: https://mybinder.org/v2/gh/sktime/skpro/main?filepath=examples
-[user guides]: https://skpro.readthedocs.io/en/latest/user_guide.html
-[extension templates]: https://github.com/sktime/skpro/tree/main/
-extension_templates [api reference]: https://skpro.readthedocs.io/en/latest/
-api_reference.html [changelog]: https://skpro.readthedocs.io/en/latest/
+(pypi))](https://pepy.tech/project/skpro) | | **Citation** | [![DOI](https://
+zenodo.org/badge/103107372.svg)](https://zenodo.org/doi/10.5281/
+zenodo.11002671) | ## :books: Documentation | Documentation | | | -------------
+------------- | -------------------------------------------------------------
+- | | :star: **[Tutorials]** | New to skpro? Here's everything you need to
+know! | | :clipboard: **[Binder Notebooks]** | Example notebooks to play with
+in your browser. | | :woman_technologist: **[User Guides]** | How to use skpro
+and its features. | | :scissors: **[Extension Templates]** | How to build your
+own estimator using skpro's API. | | :control_knobs: **[API Reference]** | The
+detailed reference for skpro's API. | | :hammer_and_wrench: **[Changelog]** |
+Changes and version history. | | :deciduous_tree: **[Roadmap]** | skpro's
+software and community development plan. | | :pencil: **[Related Software]** |
+A list of related software. | [tutorials]: https://skpro.readthedocs.io/en/
+latest/tutorials.html [binder notebooks]: https://mybinder.org/v2/gh/sktime/
+skpro/main?filepath=examples [user guides]: https://skpro.readthedocs.io/en/
+latest/user_guide.html [extension templates]: https://github.com/sktime/skpro/
+tree/main/extension_templates [api reference]: https://skpro.readthedocs.io/en/
+latest/api_reference.html [changelog]: https://skpro.readthedocs.io/en/latest/
 changelog.html [roadmap]: https://skpro.readthedocs.io/en/latest/roadmap.html
 [related software]: https://skpro.readthedocs.io/en/latest/
 related_software.html ## :speech_balloon: Where to ask questions Questions and
 feedback are extremely welcome! We strongly believe in the value of sharing
 help publicly, as it allows a wider audience to benefit from it. `skpro` is
 maintained by the `sktime` community, we use the same social channels. | Type |
 Platforms | | ------------------------------- | -------------------------------
 -------- | | :bug: **Bug Reports** | [GitHub Issue Tracker] | | :sparkles:
 **Feature Requests & Ideas** | [GitHub Issue Tracker] | | :woman_technologist:
 **Usage Questions** | [GitHub Discussions] Â· [Stack Overflow] | | :
 speech_balloon: **General Discussion** | [GitHub Discussions] | | :factory:
 **Contribution & Development** | `dev-chat` channel Â· [Discord] | | :
 globe_with_meridians: **Community collaboration session** | [Discord] - Fridays
-3 pm UTC, dev/meet-ups channel | [github issue tracker]: https://github.com/
+13 UTC, dev/meet-ups channel | [github issue tracker]: https://github.com/
 sktime/skpro/issues [github discussions]: https://github.com/sktime/skpro/
 discussions [stack overflow]: https://stackoverflow.com/questions/tagged/sktime
 [discord]: https://discord.com/invite/54ACzaFsn7 ## :dizzy: Features Our
 objective is to enhance the interoperability and usability of the AI model
 ecosystem: * ``skpro`` is compatible with [scikit-learn] and [sktime], e.g., an
 ``sktime`` proba forecaster can be built with an ``skpro`` proba regressor
 which in an ``sklearn`` regressor with proba mode added by ``skpro`` *
@@ -144,21 +145,24 @@
 regression.html) Â· [Extension Template](https://github.com/sktime/skpro/blob/
 main/extension_templates/regression.py) | | **[Time-to-event (survival)
 prediction]** | experimental | [API Reference](https://skpro.readthedocs.io/en/
 latest/api_reference/survival.html) Â· [Extension Template](https://github.com/
 sktime/skpro/blob/main/extension_templates/survival.py) | | **[Performance
 metrics]** | maturing | [API Reference](https://skpro.readthedocs.io/en/latest/
 api_reference/metrics.html) | | **[Probability distributions]** | maturing |
-[API Reference](https://skpro.readthedocs.io/en/latest/api_reference/
-distributions.html) | [Probabilistic tabular regression]: https://github.com/
-sktime/skpro/tree/main/skpro/regression [Time-to-event (survival) prediction]:
-https://github.com/sktime/skpro/tree/main/skpro/survival [Performance metrics]:
-https://github.com/sktime/skpro/tree/main/skpro/metrics [Probability
-distributions]: https://github.com/sktime/skpro/tree/main/skpro/distributions
-## :hourglass_flowing_sand: Installing `skpro` To install `skpro`, use `pip`:
+[Tutorial](https://github.com/sktime/skpro/blob/main/examples/
+03_skpro_distributions.ipynb) Â· [API Reference](https://skpro.readthedocs.io/
+en/latest/api_reference/distributions.html) Â· [Extension Template](https://
+github.com/sktime/skpro/blob/main/extension_templates/distributions.py) |
+[Probabilistic tabular regression]: https://github.com/sktime/skpro/tree/main/
+skpro/regression [Time-to-event (survival) prediction]: https://github.com/
+sktime/skpro/tree/main/skpro/survival [Performance metrics]: https://
+github.com/sktime/skpro/tree/main/skpro/metrics [Probability distributions]:
+https://github.com/sktime/skpro/tree/main/skpro/distributions ## :
+hourglass_flowing_sand: Installing `skpro` To install `skpro`, use `pip`:
 ```bash pip install skpro ``` or, with maximum dependencies, ```bash pip
 install skpro[all_extras] ``` Releases are available as source packages and
 binary wheels. You can see all available wheels [here](https://pypi.org/simple/
 skpro/). ## :zap: Quickstart ### Making probabilistic predictions ``` python
 from sklearn.datasets import load_diabetes from sklearn.ensemble import
 RandomForestRegressor from sklearn.linear_model import LinearRegression from
 sklearn.model_selection import train_test_split from skpro.regression.residual
```

### Comparing `skpro-2.2.2/README.md` & `skpro-2.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <a href="https://skpro.readthedocs.io/en/latest"><img src="https://github.com/sktime/skpro/blob/main/docs/source/images/skpro-banner.png" width="500" align="right" /></a>
 
-:rocket: **Version 2.2.2 out now!** [Read the release notes here.](https://skpro.readthedocs.io/en/latest/changelog.html).
+:rocket: **Version 2.3.0 out now!** [Read the release notes here.](https://skpro.readthedocs.io/en/latest/changelog.html).
 
 `skpro` is a library for supervised probabilistic prediction in python.
 It provides `scikit-learn`-like, `scikit-base` compatible interfaces to:
 
 * tabular **supervised regressors for probabilistic prediction** - interval, quantile and distribution predictions
 * tabular **probabilistic time-to-event and survival prediction** - instance-individual survival distributions
 * **metrics to evaluate probabilistic predictions**, e.g., pinball loss, empirical coverage, CRPS, survival losses
@@ -15,15 +15,16 @@
 | Overview | |
 |---|---|
 | **Open Source** |  [![BSD 3-clause](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://github.com/sktime/sktime/blob/main/LICENSE) |
 | **Tutorials** | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sktime/skpro/main?filepath=examples) [![!youtube](https://img.shields.io/static/v1?logo=youtube&label=YouTube&message=tutorials&color=red)](https://www.youtube.com/playlist?list=PLKs3UgGjlWHqNzu0LEOeLKvnjvvest2d0) |
 | **Community** | [![!discord](https://img.shields.io/static/v1?logo=discord&label=discord&message=chat&color=lightgreen)](https://discord.com/invite/54ACzaFsn7) [![!slack](https://img.shields.io/static/v1?logo=linkedin&label=LinkedIn&message=news&color=lightblue)](https://www.linkedin.com/company/scikit-time/) |
 | **CI/CD** | [![github-actions](https://img.shields.io/github/actions/workflow/status/sktime/sktime/wheels.yml?logo=github)](https://github.com/sktime/skpro/actions/workflows/wheels.yml) [![!codecov](https://img.shields.io/codecov/c/github/sktime/skpro?label=codecov&logo=codecov)](https://codecov.io/gh/sktime/skpro) [![readthedocs](https://img.shields.io/readthedocs/skpro?logo=readthedocs)](https://skpro.readthedocs.io/en/latest/) [![platform](https://img.shields.io/conda/pn/conda-forge/skpro)](https://github.com/sktime/skpro) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/skpro?color=orange)](https://pypi.org/project/skpro/) [![!conda](https://img.shields.io/conda/vn/conda-forge/skpro)](https://anaconda.org/conda-forge/skpro) [![!python-versions](https://img.shields.io/pypi/pyversions/skpro)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) |
-| **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/skpro) |
+| **Downloads** | [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/skpro) |
+| **Citation** | [![DOI](https://zenodo.org/badge/103107372.svg)](https://zenodo.org/doi/10.5281/zenodo.11002671) |
 
 ## :books: Documentation
 
 | Documentation              |                                                                |
 | -------------------------- | -------------------------------------------------------------- |
 | :star: **[Tutorials]**        | New to skpro? Here's everything you need to know!              |
 | :clipboard: **[Binder Notebooks]** | Example notebooks to play with in your browser.              |
@@ -54,15 +55,15 @@
 | Type                            | Platforms                               |
 | ------------------------------- | --------------------------------------- |
 | :bug: **Bug Reports**              | [GitHub Issue Tracker]                  |
 | :sparkles: **Feature Requests & Ideas** | [GitHub Issue Tracker]                       |
 | :woman_technologist: **Usage Questions**          | [GitHub Discussions] · [Stack Overflow] |
 | :speech_balloon: **General Discussion**        | [GitHub Discussions] |
 | :factory: **Contribution & Development** | `dev-chat` channel · [Discord] |
-| :globe_with_meridians: **Community collaboration session** | [Discord] - Fridays 3 pm UTC, dev/meet-ups channel |
+| :globe_with_meridians: **Community collaboration session** | [Discord] - Fridays 13 UTC, dev/meet-ups channel |
 
 [github issue tracker]: https://github.com/sktime/skpro/issues
 [github discussions]: https://github.com/sktime/skpro/discussions
 [stack overflow]: https://stackoverflow.com/questions/tagged/sktime
 [discord]: https://discord.com/invite/54ACzaFsn7
 
 
@@ -84,15 +85,15 @@
 ``skpro`` curates libraries of components of the following types:
 
 | Module | Status | Links |
 |---|---|---|
 | **[Probabilistic tabular regression]** | maturing | [Tutorial](https://github.com/sktime/skpro/blob/main/examples/01_skpro_intro.ipynb) · [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/regression.html) · [Extension Template](https://github.com/sktime/skpro/blob/main/extension_templates/regression.py) |
 | **[Time-to-event (survival) prediction]** | experimental | [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/survival.html) · [Extension Template](https://github.com/sktime/skpro/blob/main/extension_templates/survival.py) |
 | **[Performance metrics]** | maturing | [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/metrics.html) |
-| **[Probability distributions]** | maturing | [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/distributions.html) |
+| **[Probability distributions]** | maturing | [Tutorial](https://github.com/sktime/skpro/blob/main/examples/03_skpro_distributions.ipynb) · [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/distributions.html) · [Extension Template](https://github.com/sktime/skpro/blob/main/extension_templates/distributions.py) |
 
 [Probabilistic tabular regression]: https://github.com/sktime/skpro/tree/main/skpro/regression
 [Time-to-event (survival) prediction]: https://github.com/sktime/skpro/tree/main/skpro/survival
 [Performance metrics]: https://github.com/sktime/skpro/tree/main/skpro/metrics
 [Probability distributions]: https://github.com/sktime/skpro/tree/main/skpro/distributions
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_s_k_t_i_m_e_/_s_k_p_r_o_/_b_l_o_b_/_m_a_i_n_/_d_o_c_s_/_s_o_u_r_c_e_/_i_m_a_g_e_s_/_s_k_p_r_o_-
-_b_a_n_n_e_r_._p_n_g_]:rocket: **Version 2.2.2 out now!** [Read the release notes here.]
+_b_a_n_n_e_r_._p_n_g_]:rocket: **Version 2.3.0 out now!** [Read the release notes here.]
 (https://skpro.readthedocs.io/en/latest/changelog.html). `skpro` is a library
 for supervised probabilistic prediction in python. It provides `scikit-learn`-
 like, `scikit-base` compatible interfaces to: * tabular **supervised regressors
 for probabilistic prediction** - interval, quantile and distribution
 predictions * tabular **probabilistic time-to-event and survival prediction** -
 instance-individual survival distributions * **metrics to evaluate
 probabilistic predictions**, e.g., pinball loss, empirical coverage, CRPS,
@@ -32,54 +32,55 @@
 (https://skpro.readthedocs.io/en/latest/) [![platform](https://img.shields.io/
 conda/pn/conda-forge/skpro)](https://github.com/sktime/skpro) | | **Code** | [!
 [!pypi](https://img.shields.io/pypi/v/skpro?color=orange)](https://pypi.org/
 project/skpro/) [![!conda](https://img.shields.io/conda/vn/conda-forge/skpro)]
 (https://anaconda.org/conda-forge/skpro) [![!python-versions](https://
 img.shields.io/pypi/pyversions/skpro)](https://www.python.org/) [![!black]
 (https://img.shields.io/badge/code%20style-black-000000.svg)](https://
-github.com/psf/black) | | **Downloads**| [![Downloads](https://
+github.com/psf/black) | | **Downloads** | [![Downloads](https://
 static.pepy.tech/personalized-badge/
 skpro?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20
 (pypi))](https://pepy.tech/project/skpro) [![Downloads](https://
 static.pepy.tech/personalized-badge/
 skpro?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20
 (pypi))](https://pepy.tech/project/skpro) [![Downloads](https://
 static.pepy.tech/personalized-badge/
 skpro?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20
-(pypi))](https://pepy.tech/project/skpro) | ## :books: Documentation |
-Documentation | | | -------------------------- | ------------------------------
--------------------------------- | | :star: **[Tutorials]** | New to skpro?
-Here's everything you need to know! | | :clipboard: **[Binder Notebooks]** |
-Example notebooks to play with in your browser. | | :woman_technologist: **
-[User Guides]** | How to use skpro and its features. | | :scissors: **
-[Extension Templates]** | How to build your own estimator using skpro's API. |
-| :control_knobs: **[API Reference]** | The detailed reference for skpro's API.
-| | :hammer_and_wrench: **[Changelog]** | Changes and version history. | | :
-deciduous_tree: **[Roadmap]** | skpro's software and community development
-plan. | | :pencil: **[Related Software]** | A list of related software. |
-[tutorials]: https://skpro.readthedocs.io/en/latest/tutorials.html [binder
-notebooks]: https://mybinder.org/v2/gh/sktime/skpro/main?filepath=examples
-[user guides]: https://skpro.readthedocs.io/en/latest/user_guide.html
-[extension templates]: https://github.com/sktime/skpro/tree/main/
-extension_templates [api reference]: https://skpro.readthedocs.io/en/latest/
-api_reference.html [changelog]: https://skpro.readthedocs.io/en/latest/
+(pypi))](https://pepy.tech/project/skpro) | | **Citation** | [![DOI](https://
+zenodo.org/badge/103107372.svg)](https://zenodo.org/doi/10.5281/
+zenodo.11002671) | ## :books: Documentation | Documentation | | | -------------
+------------- | -------------------------------------------------------------
+- | | :star: **[Tutorials]** | New to skpro? Here's everything you need to
+know! | | :clipboard: **[Binder Notebooks]** | Example notebooks to play with
+in your browser. | | :woman_technologist: **[User Guides]** | How to use skpro
+and its features. | | :scissors: **[Extension Templates]** | How to build your
+own estimator using skpro's API. | | :control_knobs: **[API Reference]** | The
+detailed reference for skpro's API. | | :hammer_and_wrench: **[Changelog]** |
+Changes and version history. | | :deciduous_tree: **[Roadmap]** | skpro's
+software and community development plan. | | :pencil: **[Related Software]** |
+A list of related software. | [tutorials]: https://skpro.readthedocs.io/en/
+latest/tutorials.html [binder notebooks]: https://mybinder.org/v2/gh/sktime/
+skpro/main?filepath=examples [user guides]: https://skpro.readthedocs.io/en/
+latest/user_guide.html [extension templates]: https://github.com/sktime/skpro/
+tree/main/extension_templates [api reference]: https://skpro.readthedocs.io/en/
+latest/api_reference.html [changelog]: https://skpro.readthedocs.io/en/latest/
 changelog.html [roadmap]: https://skpro.readthedocs.io/en/latest/roadmap.html
 [related software]: https://skpro.readthedocs.io/en/latest/
 related_software.html ## :speech_balloon: Where to ask questions Questions and
 feedback are extremely welcome! We strongly believe in the value of sharing
 help publicly, as it allows a wider audience to benefit from it. `skpro` is
 maintained by the `sktime` community, we use the same social channels. | Type |
 Platforms | | ------------------------------- | -------------------------------
 -------- | | :bug: **Bug Reports** | [GitHub Issue Tracker] | | :sparkles:
 **Feature Requests & Ideas** | [GitHub Issue Tracker] | | :woman_technologist:
 **Usage Questions** | [GitHub Discussions] Â· [Stack Overflow] | | :
 speech_balloon: **General Discussion** | [GitHub Discussions] | | :factory:
 **Contribution & Development** | `dev-chat` channel Â· [Discord] | | :
 globe_with_meridians: **Community collaboration session** | [Discord] - Fridays
-3 pm UTC, dev/meet-ups channel | [github issue tracker]: https://github.com/
+13 UTC, dev/meet-ups channel | [github issue tracker]: https://github.com/
 sktime/skpro/issues [github discussions]: https://github.com/sktime/skpro/
 discussions [stack overflow]: https://stackoverflow.com/questions/tagged/sktime
 [discord]: https://discord.com/invite/54ACzaFsn7 ## :dizzy: Features Our
 objective is to enhance the interoperability and usability of the AI model
 ecosystem: * ``skpro`` is compatible with [scikit-learn] and [sktime], e.g., an
 ``sktime`` proba forecaster can be built with an ``skpro`` proba regressor
 which in an ``sklearn`` regressor with proba mode added by ``skpro`` *
@@ -96,21 +97,24 @@
 regression.html) Â· [Extension Template](https://github.com/sktime/skpro/blob/
 main/extension_templates/regression.py) | | **[Time-to-event (survival)
 prediction]** | experimental | [API Reference](https://skpro.readthedocs.io/en/
 latest/api_reference/survival.html) Â· [Extension Template](https://github.com/
 sktime/skpro/blob/main/extension_templates/survival.py) | | **[Performance
 metrics]** | maturing | [API Reference](https://skpro.readthedocs.io/en/latest/
 api_reference/metrics.html) | | **[Probability distributions]** | maturing |
-[API Reference](https://skpro.readthedocs.io/en/latest/api_reference/
-distributions.html) | [Probabilistic tabular regression]: https://github.com/
-sktime/skpro/tree/main/skpro/regression [Time-to-event (survival) prediction]:
-https://github.com/sktime/skpro/tree/main/skpro/survival [Performance metrics]:
-https://github.com/sktime/skpro/tree/main/skpro/metrics [Probability
-distributions]: https://github.com/sktime/skpro/tree/main/skpro/distributions
-## :hourglass_flowing_sand: Installing `skpro` To install `skpro`, use `pip`:
+[Tutorial](https://github.com/sktime/skpro/blob/main/examples/
+03_skpro_distributions.ipynb) Â· [API Reference](https://skpro.readthedocs.io/
+en/latest/api_reference/distributions.html) Â· [Extension Template](https://
+github.com/sktime/skpro/blob/main/extension_templates/distributions.py) |
+[Probabilistic tabular regression]: https://github.com/sktime/skpro/tree/main/
+skpro/regression [Time-to-event (survival) prediction]: https://github.com/
+sktime/skpro/tree/main/skpro/survival [Performance metrics]: https://
+github.com/sktime/skpro/tree/main/skpro/metrics [Probability distributions]:
+https://github.com/sktime/skpro/tree/main/skpro/distributions ## :
+hourglass_flowing_sand: Installing `skpro` To install `skpro`, use `pip`:
 ```bash pip install skpro ``` or, with maximum dependencies, ```bash pip
 install skpro[all_extras] ``` Releases are available as source packages and
 binary wheels. You can see all available wheels [here](https://pypi.org/simple/
 skpro/). ## :zap: Quickstart ### Making probabilistic predictions ``` python
 from sklearn.datasets import load_diabetes from sklearn.ensemble import
 RandomForestRegressor from sklearn.linear_model import LinearRegression from
 sklearn.model_selection import train_test_split from skpro.regression.residual
```

### Comparing `skpro-2.2.2/build_tools/changelog.py` & `skpro-2.3.0/build_tools/changelog.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 HEADERS = {
     "Accept": "application/vnd.github.v3+json",
 }
 
 if os.getenv("GITHUB_TOKEN") is not None:
     HEADERS["Authorization"] = f"token {os.getenv('GITHUB_TOKEN')}"
 
-OWNER = "skpro"
+OWNER = "sktime"
 REPO = "skpro"
 GITHUB_REPOS = "https://api.github.com/repos"
 
 
 def fetch_merged_pull_requests(page: int = 1) -> List[Dict]:  # noqa
     "Fetch a page of pull requests"
     params = {
```

### Comparing `skpro-2.2.2/docs/source/conf.py` & `skpro-2.3.0/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,15 @@
 copybutton_prompt_is_regexp = True
 
 # -- Options for nbsphinx extension ------------------------------------------
 nbsphinx_execute = "never"  # always  # whether to run notebooks
 nbsphinx_allow_errors = False  # False
 nbsphinx_timeout = 600  # seconds, set to -1 to disable timeout
 
-# add Binder launch buttom at the top
+# add Binder launch button at the top
 current_file = "{{ env.doc2path( env.docname, base=None) }}"
 
 # make sure Binder points to latest stable release, not main
 binder_base = "https://mybinder.org/v2/gh//skpro/"
 binder_url = binder_base + f"{version_match}?filepath={current_file}"
 nbsphinx_prolog = f"""
 .. |binder| image:: https://mybinder.org/badge_logo.svg
```

### Comparing `skpro-2.2.2/extension_templates/regression.py` & `skpro-2.3.0/extension_templates/regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 # todo: uncomment the following line, enter authors' GitHub IDs
 # __author__ = [authorGitHubID, anotherAuthorGitHubID]
 
 from skpro.regression.base import BaseProbaRegressor
 
 # todo: add any necessary imports here
 
-# todo: if any imports are skpro soft dependencies:
+# todo: for imports of skpro soft dependencies:
 # make sure to fill in the "python_dependencies" tag with the package import name
+# import soft dependencies only inside methods of the class, not at the top of the file
 
 
 # todo: change class name and write docstring
 class ClassName(BaseProbaRegressor):
     """Custom probabilistic supervised regressor. todo: write docstring.
 
     todo: describe your custom regressor here
@@ -65,19 +66,19 @@
 
     # todo: fill init
     # params should be written to self and never changed
     # super call must not be removed, change class name
     # parameter checks can go after super call
     def __init__(self, paramname, paramname2="paramname2default"):
         # estimators should precede parameters
-        #  if estimators have default values, set None and initalize below
+        #  if estimators have default values, set None and initialize below
 
         # todo: write any hyper-parameters and components to self
         self.paramname = paramname
-        self.paramname2 = "paramname2default"
+        self.paramname2 = paramname2
 
         # leave this as is
         super().__init__()
 
         # todo: optional, parameter checking logic (if applicable) should happen here
         # if writes derived values to self, should *not* overwrite self.parama etc
         # instead, write to self._parama, self._newparam (starting with _)
@@ -314,16 +315,14 @@
         #   class properties (e.g., inherited); parent class test case
         #   imported objects such as estimators from skpro or sklearn
         # important: all such imports should be *inside get_test_params*, not at the top
         #            since imports are used only at testing time
         #
         # The parameter_set argument is not used for most automated, module level tests.
         #   It can be used in custom, estimator specific tests, for "special" settings.
-        #   For classification, this is also used in tests for reference settings,
-        #       such as published in benchmarking studies, or for identity testing.
         # A parameter dictionary must be returned *for all values* of parameter_set,
         #   i.e., "parameter_set not available" errors should never be raised.
         #
         # A good parameter set should primarily satisfy two criteria,
         #   1. Chosen set of parameters should have a low testing time,
         #      ideally in the magnitude of few seconds for the entire test suite.
         #       This is vital for the cases where default values result in
```

### Comparing `skpro-2.2.2/extension_templates/survival.py` & `skpro-2.3.0/extension_templates/survival.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 # todo: uncomment the following line, enter authors' GitHub IDs
 # __author__ = [authorGitHubID, anotherAuthorGitHubID]
 
 from skpro.survival.base import BaseSurvReg
 
 # todo: add any necessary imports here
 
-# todo: if any imports are skpro soft dependencies:
+# todo: for imports of skpro soft dependencies:
 # make sure to fill in the "python_dependencies" tag with the package import name
+# import soft dependencies only inside methods of the class, not at the top of the file
 
 
 # todo: change class name and write docstring
 class ClassName(BaseSurvReg):
     """Custom probabilistic survival regressor. todo: write docstring.
 
     todo: describe your custom regressor here
@@ -44,19 +45,19 @@
 
     # todo: fill init
     # params should be written to self and never changed
     # super call must not be removed, change class name
     # parameter checks can go after super call
     def __init__(self, paramname, paramname2="paramname2default"):
         # estimators should precede parameters
-        #  if estimators have default values, set None and initalize below
+        #  if estimators have default values, set None and initialize below
 
         # todo: write any hyper-parameters and components to self
         self.paramname = paramname
-        self.paramname2 = "paramname2default"
+        self.paramname2 = paramname2
 
         # leave this as is
         super().__init__()
 
         # todo: optional, parameter checking logic (if applicable) should happen here
         # if writes derived values to self, should *not* overwrite self.parama etc
         # instead, write to self._parama, self._newparam (starting with _)
@@ -301,16 +302,14 @@
         #   class properties (e.g., inherited); parent class test case
         #   imported objects such as estimators from skpro or sklearn
         # important: all such imports should be *inside get_test_params*, not at the top
         #            since imports are used only at testing time
         #
         # The parameter_set argument is not used for most automated, module level tests.
         #   It can be used in custom, estimator specific tests, for "special" settings.
-        #   For classification, this is also used in tests for reference settings,
-        #       such as published in benchmarking studies, or for identity testing.
         # A parameter dictionary must be returned *for all values* of parameter_set,
         #   i.e., "parameter_set not available" errors should never be raised.
         #
         # A good parameter set should primarily satisfy two criteria,
         #   1. Chosen set of parameters should have a low testing time,
         #      ideally in the magnitude of few seconds for the entire test suite.
         #       This is vital for the cases where default values result in
```

### Comparing `skpro-2.2.2/pyproject.toml` & `skpro-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "skpro"
-version = "2.2.2"
+version = "2.3.0"
 description = "A unified framework for probability distributions and probabilistic supervised regression"
 authors = [
     {name = "skpro developers", email = "sktime.toolbox@gmail.com"},
     {name = "Franz Király"},
     {name = "Frithjof Gressmann"},
     {name = "Vitaly Davydov"},
 ]
@@ -48,26 +48,26 @@
     "scikit-learn>=0.24.0,<1.5.0",
     "scipy<2.0.0,>=1.2.0",
 ]
 
 [project.optional-dependencies]
 all_extras = [
     "attrs",
+    "cyclic-boosting>=1.4.0; python_version < '3.12'",
     "distfit",
     "lifelines<0.29.0",
     "mapie",
     "matplotlib>=3.3.2",
-    "ngboost",
+    "ngboost<0.6.0",
     "polars<0.21.0",
     "pyarrow<14.0.0; python_version < '3.12'",
     "scikit-survival<0.23.0",
     "statsmodels>=0.12.1",
     "tabulate",
     "uncertainties",
-    "cyclic-boosting>=1.2.5; python_version < '3.12'"
 ]
 
 dev = [
     "backoff",
     "httpx",
     "pre-commit",
     "pytest",
@@ -87,15 +87,15 @@
     "myst-parser",
     "nbsphinx>=0.8.6",
     "numpydoc",
     "pydata-sphinx-theme",
     "sphinx<8.0.0,!=7.2.0",
     "sphinx-design<0.6.0",
     "sphinx-issues<5.0.0",
-    "sphinx-gallery<0.16.0",
+    "sphinx-gallery<0.17.0",
     "sphinx-panels",
     "tabulate",
 ]
 
 [project.urls]
 Homepage = "https://github.com/sktime/skpro"
 Repository = "https://github.com/sktime/skpro"
```

### Comparing `skpro-2.2.2/setup.cfg` & `skpro-2.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/base/_base.py` & `skpro-2.3.0/skpro/base/_base.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/base/old_base.py` & `skpro-2.3.0/skpro/base/old_base.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/benchmarking/evaluate.py` & `skpro-2.3.0/skpro/benchmarking/evaluate.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/benchmarking/tests/test_evaluate.py` & `skpro-2.3.0/skpro/benchmarking/tests/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/datatypes/__init__.py` & `skpro-2.3.0/skpro/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/datatypes/_adapter/polars.py` & `skpro-2.3.0/skpro/datatypes/_adapter/polars.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/datatypes/_check.py` & `skpro-2.3.0/skpro/datatypes/_check.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/datatypes/_common.py` & `skpro-2.3.0/skpro/datatypes/_common.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/datatypes/_convert.py` & `skpro-2.3.0/skpro/datatypes/_convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # copyright: skpro developers, BSD-3-Clause License (see LICENSE file)
 """Machine type converters for scitypes.
 
 Exports
 -------
 convert_to(obj, to_type: str, as_scitype: str, store=None)
-    converts object "obj" to type "to_type", considerd as "as_scitype"
+    converts object "obj" to type "to_type", considered as "as_scitype"
 
 convert(obj, from_type: str, to_type: str, as_scitype: str, store=None)
     same as convert_to, without automatic identification of "from_type"
 
 mtype(obj, as_scitype: str)
     returns "from_type" of obj, considered as "as_scitype"
 ---
@@ -155,23 +155,23 @@
         store.clear()
     elif store_behaviour == "update":
         # store is passed to convert_obj by reference, unchanged
         # this "elif" is here for clarity, to cover all three values
         pass
     else:
         raise ValueError(
-            "bug: unrechable condition error, store_behaviour has unexpected value"
+            "bug: unreachable condition error, store_behaviour has unexpected value"
         )
 
     converted_obj = convert_dict[key](obj, store=store)
 
     return converted_obj
 
 
-# conversion based on queriable type to specified target
+# conversion based on queryable type to specified target
 def convert_to(
     obj,
     to_type: str,
     as_scitype: str = None,
     store=None,
     store_behaviour: str = None,
 ):
```

### Comparing `skpro-2.2.2/skpro/datatypes/_convert_utils/_coerce.py` & `skpro-2.3.0/skpro/datatypes/_convert_utils/_coerce.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/datatypes/_convert_utils/_convert.py` & `skpro-2.3.0/skpro/datatypes/_convert_utils/_convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,20 +48,20 @@
 
     Parameters
     ----------
     mtype : mtype string in convert_dict
     anchor_mtype : mtype string in convert_dict
     convert_dict : conversion dictionary with entries of converter signature
         see docstring of datatypes._convert
-    mtype_universe : iterable of mtype strings in convert_dict, coercable to list or set
+    mtype_universe : iterable of mtype strings in convert_dict, coercible to list or set
 
     Returns
     -------
     reference to convert_dict
-    CAVEAT: convert_dict passed to this function gets mutated, this is a referene
+    CAVEAT: convert_dict passed to this function gets mutated, this is a reference
     """
     keys = convert_dict.keys()
     scitype = list(keys)[0][2]
 
     if mtype_universe is None:
         mtype_universe = {x[1] for x in list(keys)}
         mtype_universe = mtype_universe.union([x[0] for x in list(keys)])
```

### Comparing `skpro-2.2.2/skpro/datatypes/_examples.py` & `skpro-2.3.0/skpro/datatypes/_examples.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/datatypes/_proba/__init__.py` & `skpro-2.3.0/skpro/datatypes/_proba/__init__.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/datatypes/_proba/_check.py` & `skpro-2.3.0/skpro/datatypes/_proba/_check.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/datatypes/_proba/_convert.py` & `skpro-2.3.0/skpro/datatypes/_proba/_convert.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/datatypes/_proba/_examples.py` & `skpro-2.3.0/skpro/datatypes/_proba/_examples.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/datatypes/_proba/_registry.py` & `skpro-2.3.0/skpro/datatypes/_proba/_registry.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/datatypes/_registry.py` & `skpro-2.3.0/skpro/datatypes/_registry.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/datatypes/_table/__init__.py` & `skpro-2.3.0/skpro/datatypes/_table/__init__.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/datatypes/_table/_check.py` & `skpro-2.3.0/skpro/datatypes/_table/_check.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/datatypes/_table/_convert.py` & `skpro-2.3.0/skpro/datatypes/_table/_convert.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/datatypes/_table/_examples.py` & `skpro-2.3.0/skpro/datatypes/_table/_examples.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/datatypes/_table/_registry.py` & `skpro-2.3.0/skpro/datatypes/_table/_registry.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/datatypes/tests/test_check.py` & `skpro-2.3.0/skpro/datatypes/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/datatypes/tests/test_convert.py` & `skpro-2.3.0/skpro/datatypes/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/datatypes/tests/test_convert_to.py` & `skpro-2.3.0/skpro/datatypes/tests/test_convert_to.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Testing machine type converters for scitypes - covert_to utility."""
+"""Testing machine type converters for scitypes - convert_to utility."""
 
 __author__ = ["fkiraly"]
 
 from skpro.datatypes._convert import convert_to
 from skpro.datatypes._examples import get_examples
 from skpro.utils import deep_equals
```

### Comparing `skpro-2.2.2/skpro/datatypes/tests/test_lookup.py` & `skpro-2.3.0/skpro/datatypes/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/distributions/__init__.py` & `skpro-2.3.0/skpro/distributions/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,45 @@
 """Probability distribution objects."""
+
 # copyright: skpro developers, BSD-3-Clause License (see LICENSE file)
 # adapted from sktime
 
 __all__ = [
+    "Beta",
+    "ChiSquared",
+    "Delta",
     "Empirical",
+    "Exponential",
     "Fisk",
     "Laplace",
     "Logistic",
     "LogNormal",
     "Mixture",
     "Normal",
     "Poisson",
     "QPD_Empirical",
     "QPD_S",
     "QPD_B",
     "QPD_U",
+    "QPD_Johnson",
     "TDistribution",
+    "Uniform",
     "Weibull",
 ]
 
+from skpro.distributions.beta import Beta
+from skpro.distributions.chi_squared import ChiSquared
+from skpro.distributions.delta import Delta
 from skpro.distributions.empirical import Empirical
+from skpro.distributions.exponential import Exponential
 from skpro.distributions.fisk import Fisk
 from skpro.distributions.laplace import Laplace
 from skpro.distributions.logistic import Logistic
 from skpro.distributions.lognormal import LogNormal
 from skpro.distributions.mixture import Mixture
 from skpro.distributions.normal import Normal
 from skpro.distributions.poisson import Poisson
-from skpro.distributions.qpd import QPD_B, QPD_S, QPD_U
+from skpro.distributions.qpd import QPD_B, QPD_S, QPD_U, QPD_Johnson
 from skpro.distributions.qpd_empirical import QPD_Empirical
 from skpro.distributions.t import TDistribution
+from skpro.distributions.uniform import Uniform
 from skpro.distributions.weibull import Weibull
```

### Comparing `skpro-2.2.2/skpro/distributions/adapters/scipy/_empirical.py` & `skpro-2.3.0/skpro/distributions/adapters/scipy/_empirical.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/distributions/adapters/statsmodels/_empirical.py` & `skpro-2.3.0/skpro/distributions/adapters/statsmodels/_empirical.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 __author__ = ["fkiraly"]
 
 import numpy as np
 import pandas as pd
 
 
 def empirical_from_rvdf(dist, index=None, columns=None):
-    """Convert a statsmodels rv_discrte_float to an skpro Empirical object.
+    """Convert a statsmodels rv_discrete_float to an skpro Empirical object.
 
     Parameters
     ----------
     dist : rv_discrte_float object
         Instance of rv_discrete.
     index : pd.Index or coercible, optional
         Index of the resulting empirical distribution.
```

### Comparing `skpro-2.2.2/skpro/distributions/base/_delegate.py` & `skpro-2.3.0/skpro/distributions/base/_delegate.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/distributions/empirical.py` & `skpro-2.3.0/skpro/distributions/empirical.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,21 +6,38 @@
 import numpy as np
 import pandas as pd
 
 from skpro.distributions.base import BaseDistribution
 
 
 class Empirical(BaseDistribution):
-    """Empirical distribution (skpro native).
+    r"""Empirical distribution, or weighted sum of delta distributions.
+
+    This distribution represents an empirical distribution, or, more generally,
+    a weighted sum of delta distributions.
+
+    The distribution is parameterized by support in ``spl``, and optionally
+    weights in ``weights``.
+
+    For the scalar case, the distribution is parameterized as follows:
+    let :math:`s_i, i = 1 \dots N` the entries of ``spl``,
+    and :math:`w_i, i = 1 \dots N` the entries of ``weights``; if ``weights=None``,
+    by default we define :math:`p_i = \frac{1}{N}`, otherwise we
+    define :math:`p_i := \frac{w_i}{\sum_{i=1}^N w_i}`
+
+    The distribution is the unique distribution that takes value :math:`s_i` with
+    probability :math:`p_i`. In particluar, if ``weights`` was ``None``,
+    the distribution is the uniform distribution supported on the :math:`s_i`.
 
     Parameters
     ----------
-    spl : pd.DataFrame with pd.MultiIndex
-        empirical sample
-        last (highest) index is instance, first (lowest) index is sample
+    spl : pd.DataFrame
+        empirical sample; for scalar distributions, rows are samples;
+        for dataframe-like distributions,
+        first (lowest) index is sample, further indices are instance indices
     weights : pd.Series, with same index and length as spl, optional, default=None
         if not passed, ``spl`` is assumed to be unweighted
     time_indep : bool, optional, default=True
         if True, ``sample`` will sample individual instance indices independently
         if False, ``sample`` will sample entire instances from ``spl``
     index : pd.Index, optional, default = RangeIndex
     columns : pd.Index, optional, default = RangeIndex
@@ -36,64 +53,108 @@
     >>> spl = pd.DataFrame(
     ...     [[0, 1], [2, 3], [10, 11], [6, 7], [8, 9], [4, 5]],
     ...     index=spl_idx,
     ...     columns=["a", "b"],
     ... )
     >>> dist = Empirical(spl)
     >>> empirical_sample = dist.sample(3)
+
+    scalar distribution:
+    >>> spl = pd.Series([1, 2, 3, 4, 3])
+    >>> dist = Empirical(spl)
+    >>> empirical_sample = dist.sample(3)
     """
 
     _tags = {
         "capabilities:approx": [],
         "capabilities:exact": ["mean", "var", "energy", "cdf", "ppf"],
         "distr:measuretype": "discrete",
+        "distr:paramtype": "nonparametric",
     }
 
     def __init__(self, spl, weights=None, time_indep=True, index=None, columns=None):
         self.spl = spl
         self.weights = weights
         self.time_indep = time_indep
-        self.index = index
-        self.columns = columns
 
-        _timestamps = spl.index.droplevel(0).unique()
-        _spl_instances = spl.index.get_level_values(0).unique()
-        self._timestamps = _timestamps
-        self._spl_instances = _spl_instances
-        self._N = len(_spl_instances)
+        index, columns = self._init_index(index, columns)
 
-        if index is None:
-            index = pd.Index(_timestamps)
+        super().__init__(index=index, columns=columns)
+
+        # initialized sorted samples
+        self._init_sorted()
+
+    def _init_index(self, index, columns):
+        """Initialize index and columns.
+
+        Sets the following attributes:
+
+        * ``_spl_indices`` - unique index for samples
+        * ``_shape`` - shape of self - 0D or 2D
+        * ``_N`` - number of samples
+        * only if array distribution: ``_instances``,
+          coerced index of ``self``, from ``spl`` index
+        """
+        spl = self.spl
 
+        is_scalar = not isinstance(spl.index, pd.MultiIndex)
+        is_scalar = is_scalar and (spl.ndim <= 1 or spl.shape[1] == 1)
+
+        if is_scalar:
+            self._shape = ()
+            _spl_indices = spl.index
+            self._spl_indices = _spl_indices
+            self._N = len(_spl_indices)
+            return None, None
+
+        _instances = spl.index.droplevel(0).unique()
+        _spl_indices = spl.index.get_level_values(0).unique()
+        self._instances = _instances
+        self._spl_indices = _spl_indices
+        self._N = len(_spl_indices)
+
+        if index is None:
+            index = _instances
         if columns is None:
             columns = spl.columns
 
-        super().__init__(index=index, columns=columns)
+        self._shape = (len(index), len(columns))
 
-        # initialized sorted samples
-        self._init_sorted()
+        return index, columns
 
     def _init_sorted(self):
         """Initialize sorted version of spl."""
-        times = self._timestamps
+        if self.ndim == 0:
+            spl = self.spl.values.flatten()
+            sorter = np.argsort(spl)
+            spl_sorted = spl[sorter]
+            if self.weights is not None:
+                weights_sorted = self.weights.values.flatten()[sorter]
+            else:
+                weights_sorted = np.ones_like(spl)
+            self._sorted = spl_sorted
+            self._weights = weights_sorted
+            return None
+
+        times = self._instances
         cols = self.columns
 
         sorted = {}
         weights = {}
         for t in times:
             sorted[t] = {}
             weights[t] = {}
             for col in cols:
                 sl = (slice(None),) + self._coerce_tuple(t)
                 spl_t = self.spl.loc[sl, col].values
                 sorter = np.argsort(spl_t)
                 spl_t_sorted = spl_t[sorter]
                 sorted[t][col] = spl_t_sorted
                 if self.weights is not None:
-                    weights_t = self.weights.loc[(slice(None), t)].values
+                    weights_t = self.weights.loc[sl].values
                     weights_t_sorted = weights_t[sorter]
                     weights[t][col] = weights_t_sorted
                 else:
                     ones = np.ones(len(spl_t_sorted))
                     weights[t][col] = ones
 
         self._sorted = sorted
@@ -105,50 +166,93 @@
         return x
 
     def _apply_per_ix(self, func, params, x=None):
         """Apply function per index."""
         sorted = self._sorted
         weights = self._weights
 
-        if x is not None and hasattr(x, "index"):
-            index = x.index
-        else:
-            index = self.index
-        if x is not None and hasattr(x, "columns"):
-            cols = x.columns
-        else:
-            cols = self.columns
+        if self.ndim == 0:
+            return func(spl=sorted, weights=weights, x=x, **params)
+
+        index = self.index
+        cols = self.columns
 
         res = pd.DataFrame(index=index, columns=cols)
-        for ix in index:
-            for col in cols:
+        for i, ix in enumerate(index):
+            for j, col in enumerate(cols):
                 spl_t = sorted[ix][col]
                 weights_t = weights[ix][col]
                 if x is None:
                     x_t = None
                 elif hasattr(x, "loc"):
                     x_t = x.loc[ix, col]
                 else:
-                    x_t = x
+                    x_t = x[i, j]
                 res.at[ix, col] = func(spl=spl_t, weights=weights_t, x=x_t, **params)
         return res.apply(pd.to_numeric)
 
+    def _slice_ix(self, obj, ix):
+        """Slice obj by index ix, applied to MultiIndex levels 1 ... last.
+
+        obj is assumed to have MultiIndex, and slicing occurs on the
+        last levels, 1 ... last.
+
+        ix can be a simple index or MultiIndex,
+        same number of levels as obj.index.droplevel(0).
+
+        This utility function is needed since pandas cannot do this?
+
+        Parameters
+        ----------
+        obj : pd.DataFrame or pd.Series, with pd.MultiIndex
+            object to slice
+        ix : pd.Index or pd.MultiIndex
+            index to slice by, loc references
+
+        Returns
+        -------
+        pd.DataFrame or pd.Series, same type as obj
+            obj sliced by levels 1 ... last, subset to levels in ix
+        """
+        if not isinstance(ix, pd.MultiIndex):
+            if isinstance(obj, pd.DataFrame):
+                return obj.loc[(slice(None), ix), :]
+            else:
+                return obj.loc[(slice(None), ix)]
+
+        obj_ix = obj.index
+        obj_vals = obj_ix.get_level_values(0).unique()
+        if isinstance(ix, pd.MultiIndex):
+            prod_ix = [(v,) + i for v in obj_vals for i in ix]
+        else:
+            prod_ix = [(v,) + (i,) for v in obj_vals for i in ix]
+        prod_ix = pd.MultiIndex.from_tuples(prod_ix)
+
+        return obj.loc[prod_ix]
+
     def _iloc(self, rowidx=None, colidx=None):
+        if is_scalar_notnone(rowidx) and is_scalar_notnone(colidx):
+            return self._iat(rowidx, colidx)
+        if is_scalar_notnone(rowidx):
+            rowidx = pd.Index([rowidx])
+        if is_scalar_notnone(colidx):
+            colidx = pd.Index([colidx])
+
         index = self.index
         columns = self.columns
         weights = self.weights
 
         spl_subset = self.spl
 
         if rowidx is not None:
             rowidx_loc = index[rowidx]
             # subset multiindex to rowidx by last level
-            spl_subset = self.spl.loc[(slice(None), rowidx_loc), :]
+            spl_subset = self._slice_ix(self.spl, rowidx_loc)
             if weights is not None:
-                weights_subset = weights.loc[(slice(None), rowidx_loc)]
+                weights_subset = self._slice_ix(weights, rowidx_loc)
             else:
                 weights_subset = None
             subs_rowidx = index[rowidx]
         else:
             subs_rowidx = index
             weights_subset = weights
 
@@ -162,15 +266,28 @@
             spl_subset,
             weights=weights_subset,
             time_indep=self.time_indep,
             index=subs_rowidx,
             columns=subs_colidx,
         )
 
-    def energy(self, x=None):
+    def _iat(self, rowidx=None, colidx=None):
+        if rowidx is None or colidx is None:
+            raise ValueError("iat method requires both row and column index")
+        self_subset = self.iloc[[rowidx], [colidx]]
+        spl_subset = self_subset.spl.droplevel(0)
+        if self.weights is not None:
+            wts_subset = self_subset.weights.droplevel(0)
+        else:
+            wts_subset = None
+
+        subset_params = {"spl": spl_subset, "weights": wts_subset}
+        return type(self)(**subset_params)
+
+    def _energy_default(self, x=None):
         r"""Energy of self, w.r.t. self or a constant frame x.
 
         Let :math:`X, Y` be i.i.d. random variables with the distribution of `self`.
 
         If `x` is `None`, returns :math:`\mathbb{E}[|X-Y|]` (per row), "self-energy".
         If `x` is passed, returns :math:`\mathbb{E}[|X-x|]` (per row), "energy wrt x".
 
@@ -180,77 +297,105 @@
             if pd.DataFrame, must have same rows and columns as `self`
 
         Returns
         -------
         pd.DataFrame with same rows as `self`, single column `"energy"`
         each row contains one float, self-energy/energy as described above.
         """
-        energy = self._apply_per_ix(_energy_np, {"assume_sorted": True}, x=x)
-        res = pd.DataFrame(energy.sum(axis=1), columns=["energy"])
-        return res
+        energy_arr = self._apply_per_ix(_energy_np, {"assume_sorted": True}, x=x)
+        if energy_arr.ndim > 0:
+            energy_arr = np.sum(energy_arr, axis=1)
+        return energy_arr
 
-    def mean(self):
+    def _mean(self):
         r"""Return expected value of the distribution.
 
         Let :math:`X` be a random variable with the distribution of `self`.
         Returns the expectation :math:`\mathbb{E}[X]`
 
         Returns
         -------
         pd.DataFrame with same rows, columns as `self`
         expected value of distribution (entry-wise)
         """
         spl = self.spl
+
+        # scalar case
+        if self.ndim == 0:
+            spl = spl.values.flatten()
+            if self.weights is None:
+                return np.mean(spl)
+            else:
+                return np.average(spl, weights=self.weights)
+
+        # dataframe case
+        groupby_levels = list(range(1, spl.index.nlevels))
         if self.weights is None:
-            mean_df = spl.groupby(level=-1, sort=False).mean()
+            mean_df = spl.groupby(level=groupby_levels, sort=False).mean()
         else:
-            mean_df = spl.groupby(level=-1, sort=False).apply(
+            mean_df = spl.groupby(level=groupby_levels, sort=False).apply(
                 lambda x: np.average(x, weights=self.weights.loc[x.index], axis=0)
             )
             mean_df = pd.DataFrame(mean_df.tolist(), index=mean_df.index)
             mean_df.columns = spl.columns
 
+        mean_df = mean_df.loc[self.index]  # ensure consistent sorting
         return mean_df
 
-    def var(self):
+    def _var(self):
         r"""Return element/entry-wise variance of the distribution.
 
         Let :math:`X` be a random variable with the distribution of `self`.
         Returns :math:`\mathbb{V}[X] = \mathbb{E}\left(X - \mathbb{E}[X]\right)^2`
 
         Returns
         -------
         pd.DataFrame with same rows, columns as `self`
         variance of distribution (entry-wise)
         """
         spl = self.spl
         N = self._N
+
+        # scalar case
+        if self.ndim == 0:
+            spl = spl.values.flatten()
+            if self.weights is None:
+                return np.var(spl, ddof=0)
+            else:
+                mean = self.mean()
+                var = np.average((spl - mean) ** 2, weights=self.weights)
+                return var
+
+        # dataframe case
+        groupby_levels = list(range(1, spl.index.nlevels))
         if self.weights is None:
-            var_df = spl.groupby(level=-1, sort=False).var(ddof=0)
+            var_df = spl.groupby(level=groupby_levels, sort=False).var(ddof=0)
         else:
             mean = self.mean()
-            means = pd.concat([mean] * N, axis=0, keys=self._spl_instances)
-            var_df = spl.groupby(level=-1, sort=False).apply(
+            means = pd.concat([mean] * N, axis=0, keys=self._spl_indices)
+            var_df = spl.groupby(level=groupby_levels, sort=False).apply(
                 lambda x: np.average(
                     (x - means.loc[x.index]) ** 2,
                     weights=self.weights.loc[x.index],
                     axis=0,
                 )
             )
             var_df = pd.DataFrame(
                 var_df.tolist(), index=var_df.index, columns=spl.columns
             )
+
+        var_df = var_df.loc[self.index]  # ensure consistent sorting
         return var_df
 
-    def cdf(self, x):
+    def _cdf(self, x):
         """Cumulative distribution function."""
         cdf_val = self._apply_per_ix(_cdf_np, {"assume_sorted": True}, x=x)
         return cdf_val
 
-    def ppf(self, p):
+    def _ppf(self, p):
         """Quantile function = percent point function = inverse cdf."""
         ppf_val = self._apply_per_ix(_ppf_np, {"assume_sorted": True}, x=p)
         return ppf_val
 
     def sample(self, n_samples=None):
         """Sample from the distribution.
 
@@ -264,16 +409,21 @@
         returns a sample that contains a single sample from `self`,
         in `pd.DataFrame` mtype format convention, with `index` and `columns` as `self`
         if n_samples is `int`:
         returns a `pd.DataFrame` that contains `n_samples` i.i.d. samples from `self`,
         in `pd-multiindex` mtype format convention, with same `columns` as `self`,
         and `MultiIndex` that is product of `RangeIndex(n_samples)` and `self.index`
         """
+        # for now, always defaulting to the standard logic
+        # todo: address issue #283
+        if self.ndim >= 0:
+            return super().sample(n_samples=n_samples)
+
         spl = self.spl
-        timestamps = self._timestamps
+        timestamps = self._instances
         weights = self.weights
 
         if n_samples is None:
             n_samples = 1
             n_samples_was_none = True
         else:
             n_samples_was_none = False
@@ -323,15 +473,39 @@
         params2 = {
             "spl": spl,
             "weights": pd.Series([0.5, 0.5, 0.5, 1, 1, 1.1], index=spl_idx),
             "time_indep": False,
             "index": pd.RangeIndex(3),
             "columns": pd.Index(["a", "b"]),
         }
-        return [params1, params2]
+
+        # params3 is scalar, unweighted
+        spl_scalar = pd.Series([1, 2, 3, 4, 3])
+        params3 = {"spl": spl_scalar}
+
+        # params4 is scalar, weighted
+        spl_scalar = pd.DataFrame([1, 2, 3, 4, 3])
+        wts_scalar = pd.Series([0.2, 0.2, 0.3, 0.3, 0.1])
+        params4 = {"spl": spl_scalar, "weights": wts_scalar}
+
+        # hierarchical MultiIndex, important for sktime
+        spl_idx = pd.MultiIndex.from_product(
+            [[0, 1], [0, 1, 2], [0, 1]], names=["sample", "instance", "time"]
+        )
+        param5 = {"spl": pd.DataFrame(np.random.rand(12, 2), index=spl_idx)}
+
+        # hierarchical MultiIndex, important for sktime, weighted
+        spl_idx = pd.MultiIndex.from_product(
+            [[0, 1], [0, 1, 2], [0, 1]], names=["sample", "instance", "time"]
+        )
+        weights = pd.Series(list(range(1, 13)), index=spl_idx)
+        spl = pd.DataFrame(np.random.rand(12, 2), index=spl_idx)
+        param6 = {"spl": spl, "weights": weights}
+
+        return [params1, params2, params3, params4, param5, param6]
 
 
 def _energy_np(spl, x=None, weights=None, assume_sorted=False):
     r"""Compute sample energy, fast numpy based subroutine.
 
     Let :math:`X` be the random variable with support being
     values of `spl`, with probability weights `weights`.
@@ -451,7 +625,12 @@
     weights = weights / w_sum
 
     cum_weights = np.cumsum(weights)
     ix_val = np.searchsorted(cum_weights, x)
     ppf_val = spl[ix_val]
 
     return ppf_val
+
+
+def is_scalar_notnone(obj):
+    """Check if obj is scalar and not None."""
+    return obj is not None and np.isscalar(obj)
```

### Comparing `skpro-2.2.2/skpro/distributions/fisk.py` & `skpro-2.3.0/skpro/distributions/logistic.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,126 +1,171 @@
 # copyright: skpro developers, BSD-3-Clause License (see LICENSE file)
-"""Log-logistic aka Fisk probability distribution."""
+"""Logistic probability distribution."""
 
-__author__ = ["fkiraly"]
+__author__ = ["malikrafsan"]
 
+import numpy as np
 import pandas as pd
-from scipy.stats import fisk
 
 from skpro.distributions.base import BaseDistribution
 
 
-class Fisk(BaseDistribution):
-    r"""Fisk distribution, aka log-logistic distribution.
+class Logistic(BaseDistribution):
+    r"""Logistic distribution.
 
-    The Fisk distibution is parametrized by a scale parameter :math:`\alpha`
-    and a shape parameter :math:`\beta`, such that the cumulative distribution
-    function (CDF) is given by:
+    The logistic distribution is parametrized by a mean parameter :math:`\mu`,
+    and scale parameter :math:`s`, such that the cdf is given by:
 
-    .. math:: F(x) = 1 - \left(1 + \frac{x}{\alpha}\right)^{-\beta}\right)^{-1}
+    .. math:: F(x) = \frac{1}{1 + \exp\left(\frac{x - \mu}{s}\right)}
+
+    The scale parameter :math:`s` is represented by the parameter ``scale``,
+    and the mean parameter :math:`\mu` by the parameter ``mu``.
 
     Parameters
     ----------
-    alpha : float or array of float (1D or 2D), must be positive
+    mu : float or array of float (1D or 2D)
+        mean of the logistic distribution
+    scale : float or array of float (1D or 2D), must be positive
         scale parameter of the distribution
-    beta : float or array of float (1D or 2D), must be positive
-        shape parameter of the distribution
     index : pd.Index, optional, default = RangeIndex
     columns : pd.Index, optional, default = RangeIndex
 
     Example
     -------
-    >>> from skpro.distributions.fisk import Fisk
+    >>> from skpro.distributions.logistic import Logistic
 
-    >>> d = Fisk(beta=[[1, 1], [2, 3], [4, 5]], alpha=2)
+    >>> l = Logistic(mu=[[0, 1], [2, 3], [4, 5]], scale=1)
     """
 
     _tags = {
-        "capabilities:approx": ["energy", "pdfnorm"],
+        "capabilities:approx": ["pdfnorm", "energy"],
         "capabilities:exact": ["mean", "var", "pdf", "log_pdf", "cdf", "ppf"],
         "distr:measuretype": "continuous",
+        "distr:paramtype": "parametric",
+        "broadcast_init": "on",
     }
 
-    def __init__(self, alpha=1, beta=1, index=None, columns=None):
-        self.alpha = alpha
-        self.beta = beta
-        self.index = index
-        self.columns = columns
-
-        # todo: untangle index handling
-        # and broadcast of parameters.
-        # move this functionality to the base class
-        # important: if only one argument, it is a lenght-1-tuple, deal with this
-        self._alpha, self._beta = self._get_bc_params(self.alpha, self.beta)
-        shape = self._alpha.shape
+    def __init__(self, mu, scale, index=None, columns=None):
+        self.mu = mu
+        self.scale = scale
 
-        if index is None:
-            index = pd.RangeIndex(shape[0])
+        super().__init__(index=index, columns=columns)
 
-        if columns is None:
-            columns = pd.RangeIndex(shape[1])
+    def _mean(self):
+        """Return expected value of the distribution.
 
-        super().__init__(index=index, columns=columns)
+        Returns
+        -------
+        2D np.ndarray, same shape as ``self``
+            expected value of distribution (entry-wise)
+        """
+        return self._bc_params["mu"]
 
-    def mean(self):
-        r"""Return expected value of the distribution.
+    def _var(self):
+        r"""Return variance of the distribution.
 
         Let :math:`X` be a random variable with the distribution of `self`.
-        Returns the expectation :math:`\mathbb{E}[X]`
+        Returns the variance :math:`\mathbb{V}[X] = \frac{\mathbb{S}^2 \times \pi^3}{3}`
 
         Returns
         -------
         pd.DataFrame with same rows, columns as `self`
-        expected value of distribution (entry-wise)
+        variance of distribution (entry-wise)
         """
-        mean_arr = fisk.mean(scale=self._alpha, c=self._beta)
-        return pd.DataFrame(mean_arr, index=self.index, columns=self.columns)
+        scale = self._bc_params["scale"]
+        var_arr = (scale**2 * np.pi**2) / 3
+        return var_arr
+
+    def _pdf(self, x):
+        """Probability density function.
+
+        Parameters
+        ----------
+        x : 2D np.ndarray, same shape as ``self``
+            values to evaluate the pdf at
 
-    def var(self):
-        r"""Return element/entry-wise variance of the distribution.
+        Returns
+        -------
+        2D np.ndarray, same shape as ``self``
+            pdf values at the given points
+        """
+        mu = self._bc_params["mu"]
+        scale = self._bc_params["scale"]
 
-        Let :math:`X` be a random variable with the distribution of `self`.
-        Returns :math:`\mathbb{V}[X] = \mathbb{E}\left(X - \mathbb{E}[X]\right)^2`
+        numerator = np.exp(-(x - mu) / scale)
+        denominator = scale * ((1 + np.exp(-(x - mu) / scale)) ** 2)
+        pdf_arr = numerator / denominator
+        return pdf_arr
+
+    def _log_pdf(self, x):
+        """Logarithmic probability density function.
+
+        Parameters
+        ----------
+        x : 2D np.ndarray, same shape as ``self``
+            values to evaluate the pdf at
 
         Returns
         -------
-        pd.DataFrame with same rows, columns as `self`
-        variance of distribution (entry-wise)
+        2D np.ndarray, same shape as ``self``
+            log pdf values at the given points
         """
-        var_arr = fisk.var(scale=self._alpha, c=self._beta)
-        return pd.DataFrame(var_arr, index=self.index, columns=self.columns)
+        mu = self._bc_params["mu"]
+        scale = self._bc_params["scale"]
 
-    def pdf(self, x):
-        """Probability density function."""
-        d = self.loc[x.index, x.columns]
-        pdf_arr = fisk.pdf(x.values, scale=d.alpha, c=d.beta)
-        return pd.DataFrame(pdf_arr, index=x.index, columns=x.columns)
-
-    def log_pdf(self, x):
-        """Logarithmic probability density function."""
-        d = self.loc[x.index, x.columns]
-        lpdf_arr = fisk.logpdf(x.values, scale=d.alpha, c=d.beta)
-        return pd.DataFrame(lpdf_arr, index=x.index, columns=x.columns)
-
-    def cdf(self, x):
-        """Cumulative distribution function."""
-        d = self.loc[x.index, x.columns]
-        cdf_arr = fisk.cdf(x.values, scale=d.alpha, c=d.beta)
-        return pd.DataFrame(cdf_arr, index=x.index, columns=x.columns)
-
-    def ppf(self, p):
-        """Quantile function = percent point function = inverse cdf."""
-        d = self.loc[p.index, p.columns]
-        icdf_arr = fisk.ppf(p.values, scale=d.alpha, c=d.beta)
-        return pd.DataFrame(icdf_arr, index=p.index, columns=p.columns)
+        y = -(x - mu) / scale
+        lpdf_arr = y - np.log(scale) - 2 * np.logaddexp(0, y)
+        return lpdf_arr
+
+    def _cdf(self, x):
+        """Cumulative distribution function.
+
+        Parameters
+        ----------
+        x : 2D np.ndarray, same shape as ``self``
+            values to evaluate the cdf at
+
+        Returns
+        -------
+        2D np.ndarray, same shape as ``self``
+            cdf values at the given points
+        """
+        mu = self._bc_params["mu"]
+        scale = self._bc_params["scale"]
+
+        cdf_arr = (1 + np.tanh((x - mu) / (2 * scale))) / 2
+        return cdf_arr
+
+    def _ppf(self, p):
+        """Quantile function = percent point function = inverse cdf.
+
+        Parameters
+        ----------
+        p : 2D np.ndarray, same shape as ``self``
+            values to evaluate the ppf at
+
+        Returns
+        -------
+        2D np.ndarray, same shape as ``self``
+            ppf values at the given points
+        """
+        mu = self._bc_params["mu"]
+        scale = self._bc_params["scale"]
+
+        ppf_arr = mu + scale * np.log(p / (1 - p))
+        return ppf_arr
 
     @classmethod
     def get_test_params(cls, parameter_set="default"):
         """Return testing parameter settings for the estimator."""
-        params1 = {"alpha": [[1, 1], [2, 3], [4, 5]], "beta": 3}
+        # array case examples
+        params1 = {"mu": [[0, 1], [2, 3], [4, 5]], "scale": 1}
         params2 = {
-            "alpha": 2,
-            "beta": 3,
+            "mu": 0,
+            "scale": 1,
             "index": pd.Index([1, 2, 5]),
             "columns": pd.Index(["a", "b"]),
         }
-        return [params1, params2]
+        # scalar case examples
+        params3 = {"mu": -2, "scale": 2}
+
+        return [params1, params2, params3]
```

### Comparing `skpro-2.2.2/skpro/distributions/laplace.py` & `skpro-2.3.0/skpro/distributions/weibull.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,155 +1,182 @@
 # copyright: skpro developers, BSD-3-Clause License (see LICENSE file)
-"""Laplace probability distribution."""
+"""Weibull probability distribution."""
 
-__author__ = ["fkiraly"]
+__author__ = ["malikrafsan"]
 
 import numpy as np
 import pandas as pd
+from scipy.special import gamma
 
 from skpro.distributions.base import BaseDistribution
 
 
-class Laplace(BaseDistribution):
-    """Laplace distribution.
+class Weibull(BaseDistribution):
+    r"""Weibull distribution.
+
+    The Weibull distribution is parametrized by scale parameter :math:`\lambda`,
+    and shape parameter :math:`k`, such that the cdf is given by:
+
+    .. math:: F(x) = 1 - \exp\left(-\left(\frac{x}{\lambda}\right)^k\right)
+
+    The scale parameter :math:`\lambda` is represented by the parameter ``scale``,
+    and the shape parameter :math:`k` by the parameter ``k``.
 
     Parameters
     ----------
-    mean : float or array of float (1D or 2D)
-        mean of the distribution
     scale : float or array of float (1D or 2D), must be positive
-        scale parameter of the distribution, same as standard deviation / sqrt(2)
+        scale parameter of the distribution
+    k : float or array of float (1D or 2D), must be positive
+        shape parameter of the distribution
     index : pd.Index, optional, default = RangeIndex
     columns : pd.Index, optional, default = RangeIndex
 
     Example
     -------
-    >>> from skpro.distributions import Laplace
+    >>> from skpro.distributions.weibull import Weibull
 
-    >>> n = Laplace(mu=[[0, 1], [2, 3], [4, 5]], scale=1)
+    >>> w = Weibull(scale=[[1, 1], [2, 3], [4, 5]], k=1)
     """
 
     _tags = {
-        "capabilities:approx": ["pdfnorm"],
-        "capabilities:exact": ["mean", "var", "energy", "pdf", "log_pdf", "cdf", "ppf"],
+        "capabilities:approx": ["pdfnorm", "energy"],
+        "capabilities:exact": ["mean", "var", "pdf", "log_pdf", "cdf", "ppf"],
         "distr:measuretype": "continuous",
+        "distr:paramtype": "parametric",
+        "broadcast_init": "on",
     }
 
-    def __init__(self, mu, scale, index=None, columns=None):
-        self.mu = mu
+    def __init__(self, scale, k, index=None, columns=None):
         self.scale = scale
-        self.index = index
-        self.columns = columns
+        self.k = k
 
-        # todo: untangle index handling
-        # and broadcast of parameters.
-        # move this functionality to the base class
-        self._mu, self._scale = self._get_bc_params(self.mu, self.scale)
-        shape = self._mu.shape
+        super().__init__(index=index, columns=columns)
 
-        if index is None:
-            index = pd.RangeIndex(shape[0])
+    def _mean(self):
+        r"""Return expected value of the distribution.
 
-        if columns is None:
-            columns = pd.RangeIndex(shape[1])
+        For Weibull distribution, expectation is given by,
+        :math:`\lambda \Gamma (1+\frac{1}{k})`
 
-        super().__init__(index=index, columns=columns)
+        Returns
+        -------
+        2D np.ndarray, same shape as ``self``
+            expected value of distribution (entry-wise)
+        """
+        scale = self._bc_params["scale"]
+        k = self._bc_params["k"]
+        mean_arr = scale * gamma(1 + 1 / k)
+        return mean_arr
 
-    def energy(self, x=None):
-        r"""Energy of self, w.r.t. self or a constant frame x.
+    def _var(self):
+        r"""Return element/entry-wise variance of the distribution.
+
+        For Weibull distribution, variance is given by
+        :math:`\lambda^2 \left( \Gamma(1+\frac{2}{k}) - \Gamma^2(1+\frac{1}{k}) \right)`
+
+        Returns
+        -------
+        2D np.ndarray, same shape as ``self``
+            pdf values at the given points
+        """
+        scale = self._bc_params["scale"]
+        k = self._bc_params["k"]
 
-        Let :math:`X, Y` be i.i.d. random variables with the distribution of `self`.
+        left_gamma = gamma(1 + 2 / k)
+        right_gamma = gamma(1 + 1 / k) ** 2
+        var_arr = scale**2 * (left_gamma - right_gamma)
+        return var_arr
 
-        If `x` is `None`, returns :math:`\mathbb{E}[|X-Y|]` (per row), "self-energy".
-        If `x` is passed, returns :math:`\mathbb{E}[|X-x|]` (per row), "energy wrt x".
+    def _pdf(self, x):
+        """Probability density function.
 
         Parameters
         ----------
-        x : None or pd.DataFrame, optional, default=None
-            if pd.DataFrame, must have same rows and columns as `self`
+        x : 2D np.ndarray, same shape as ``self``
+            values to evaluate the pdf at
 
         Returns
         -------
-        pd.DataFrame with same rows as `self`, single column `"energy"`
-        each row contains one float, self-energy/energy as described above.
+        2D np.ndarray, same shape as ``self``
+            pdf values at the given points
         """
-        if x is None:
-            sc_arr = self._scale
-            energy_arr = np.sum(sc_arr, axis=1) * 1.5
-            energy = pd.DataFrame(energy_arr, index=self.index, columns=["energy"])
-        else:
-            d = self.loc[x.index, x.columns]
-            mu_arr, sc_arr = d.mu, d.scale
-            y_arr = np.abs((x.values - mu_arr) / sc_arr)
-            c_arr = y_arr + np.exp(-y_arr)
-            energy_arr = np.sum(sc_arr * c_arr, axis=1)
-            energy = pd.DataFrame(energy_arr, index=self.index, columns=["energy"])
-        return energy
+        k = self._bc_params["k"]
+        scale = self._bc_params["scale"]
 
-    def mean(self):
-        r"""Return expected value of the distribution.
+        pdf_arr = (k / scale) * (x / scale) ** (k - 1) * np.exp(-((x / scale) ** k))
+        pdf_arr = pdf_arr * (x >= 0)  # if x < 0, pdf = 0
+        return pdf_arr
+
+    def _log_pdf(self, x):
+        """Logarithmic probability density function.
 
-        Let :math:`X` be a random variable with the distribution of `self`.
-        Returns the expectation :math:`\mathbb{E}[X]`
+        Parameters
+        ----------
+        x : 2D np.ndarray, same shape as ``self``
+            values to evaluate the pdf at
 
         Returns
         -------
-        pd.DataFrame with same rows, columns as `self`
-        expected value of distribution (entry-wise)
+        2D np.ndarray, same shape as ``self``
+            log pdf values at the given points
         """
-        mean_arr = self._mu
-        return pd.DataFrame(mean_arr, index=self.index, columns=self.columns)
+        k = self._bc_params["k"]
+        scale = self._bc_params["scale"]
 
-    def var(self):
-        r"""Return element/entry-wise variance of the distribution.
+        lpdf_arr = np.log(k / scale) + (k - 1) * np.log(x / scale) - (x / scale) ** k
+        lpdf_arr = lpdf_arr + np.log(x >= 0)  # if x < 0, pdf = 0, so log pdf = -inf
+        return lpdf_arr
 
-        Let :math:`X` be a random variable with the distribution of `self`.
-        Returns :math:`\mathbb{V}[X] = \mathbb{E}\left(X - \mathbb{E}[X]\right)^2`
+    def _cdf(self, x):
+        """Cumulative distribution function.
+
+        Parameters
+        ----------
+        x : 2D np.ndarray, same shape as ``self``
+            values to evaluate the cdf at
 
         Returns
         -------
-        pd.DataFrame with same rows, columns as `self`
-        variance of distribution (entry-wise)
+        2D np.ndarray, same shape as ``self``
+            cdf values at the given points
         """
-        sd_arr = self._scale / np.sqrt(2)
-        return pd.DataFrame(sd_arr, index=self.index, columns=self.columns) ** 2
-
-    def pdf(self, x):
-        """Probability density function."""
-        d = self.loc[x.index, x.columns]
-        pdf_arr = np.exp(-np.abs((x.values - d.mu) / d.scale))
-        pdf_arr = pdf_arr / (2 * d.scale)
-        return pd.DataFrame(pdf_arr, index=x.index, columns=x.columns)
-
-    def log_pdf(self, x):
-        """Logarithmic probability density function."""
-        d = self.loc[x.index, x.columns]
-        lpdf_arr = -np.abs((x.values - d.mu) / d.scale)
-        lpdf_arr = lpdf_arr - np.log(2 * d.scale)
-        return pd.DataFrame(lpdf_arr, index=x.index, columns=x.columns)
-
-    def cdf(self, x):
-        """Cumulative distribution function."""
-        d = self.loc[x.index, x.columns]
-        sgn_arr = np.sign(x.values - d.mu)
-        exp_arr = np.exp(-np.abs((x.values - d.mu) / d.scale))
-        cdf_arr = 0.5 + 0.5 * sgn_arr * (1 - exp_arr)
-        return pd.DataFrame(cdf_arr, index=x.index, columns=x.columns)
-
-    def ppf(self, p):
-        """Quantile function = percent point function = inverse cdf."""
-        d = self.loc[p.index, p.columns]
-        sgn_arr = np.sign(p.values - 0.5)
-        icdf_arr = d.mu - d.scale * sgn_arr * np.log(1 - 2 * np.abs(p.values - 0.5))
-        return pd.DataFrame(icdf_arr, index=p.index, columns=p.columns)
+        k = self._bc_params["k"]
+        scale = self._bc_params["scale"]
+
+        cdf_arr = 1 - np.exp(-((x / scale) ** k))
+        cdf_arr = cdf_arr * (x >= 0)  # if x < 0, cdf = 0
+        return cdf_arr
+
+    def _ppf(self, p):
+        """Quantile function = percent point function = inverse cdf.
+
+        Parameters
+        ----------
+        p : 2D np.ndarray, same shape as ``self``
+            values to evaluate the ppf at
+
+        Returns
+        -------
+        2D np.ndarray, same shape as ``self``
+            ppf values at the given points
+        """
+        k = self._bc_params["k"]
+        scale = self._bc_params["scale"]
+
+        ppf_arr = scale * (-np.log(1 - p)) ** (1 / k)
+        return ppf_arr
 
     @classmethod
     def get_test_params(cls, parameter_set="default"):
         """Return testing parameter settings for the estimator."""
-        params1 = {"mu": [[0, 1], [2, 3], [4, 5]], "scale": 1}
+        # array case examples
+        params1 = {"scale": [[1, 1], [2, 3], [4, 5]], "k": 1}
         params2 = {
-            "mu": 0,
             "scale": 1,
+            "k": 1,
             "index": pd.Index([1, 2, 5]),
             "columns": pd.Index(["a", "b"]),
         }
-        return [params1, params2]
+        # scalar case examples
+        params3 = {"scale": 2, "k": 3}
+
+        return [params1, params2, params3]
```

### Comparing `skpro-2.2.2/skpro/distributions/lognormal.py` & `skpro-2.3.0/skpro/distributions/lognormal.py`

 * *Files 26% similar despite different names*

```diff
@@ -32,36 +32,24 @@
     >>> from skpro.distributions.lognormal import LogNormal
 
     >>> n = LogNormal(mu=[[0, 1], [2, 3], [4, 5]], sigma=1)
     """
 
     _tags = {
         "authors": ["bhavikar04", "fkiraly"],
-        "capabilities:approx": ["pdflognorm"],
-        "capabilities:exact": ["mean", "var", "energy", "pdf", "log_pdf", "cdf", "ppf"],
+        "capabilities:approx": ["energy", "pdfnorm"],
+        "capabilities:exact": ["mean", "var", "pdf", "log_pdf", "cdf", "ppf"],
         "distr:measuretype": "continuous",
+        "distr:paramtype": "parametric",
+        "broadcast_init": "on",
     }
 
     def __init__(self, mu, sigma, index=None, columns=None):
         self.mu = mu
         self.sigma = sigma
-        self.index = index
-        self.columns = columns
-
-        # todo: untangle index handling
-        # and broadcast of parameters.
-        # move this functionality to the base class
-        self._mu, self._sigma = self._get_bc_params()
-        shape = self._mu.shape
-
-        if index is None:
-            index = pd.RangeIndex(shape[0])
-
-        if columns is None:
-            columns = pd.RangeIndex(shape[1])
 
         super().__init__(index=index, columns=columns)
 
     # commented out, seems incorrect
     # def energy(self, x=None):
     #     r"""Energy of self, w.r.t. self or a constant frame x.
 
@@ -95,75 +83,129 @@
     #         c_arr2 = c_arr2 * c_arr3
     #         c_arr = c_arr + c_arr2
 
     #         energy_arr = np.sum(c_arr, axis=1)
     #         energy = pd.DataFrame(energy_arr, index=self.index, columns=["energy"])
     #     return energy
 
-    def mean(self):
-        r"""Return expected value of the distribution.
-
-        Let :math:`X` be a random variable with the distribution of `self`.
-        Returns the expectation :math:`\mathbb{E}[X]`
+    def _mean(self):
+        """Return expected value of the distribution.
 
         Returns
         -------
-        pd.DataFrame with same rows, columns as `self`
-        expected value of distribution (entry-wise)
+        2D np.ndarray, same shape as ``self``
+            expected value of distribution (entry-wise)
         """
-        mean_arr = np.exp(self._mu + self._sigma**2 / 2)
-        return pd.DataFrame(mean_arr, index=self.index, columns=self.columns)
+        mu = self._bc_params["mu"]
+        sigma = self._bc_params["sigma"]
 
-    def var(self):
-        r"""Return element/entry-wise variance of the distribution.
+        mean_arr = np.exp(mu + sigma**2 / 2)
+        return mean_arr
 
-        Let :math:`X` be a random variable with the distribution of `self`.
-        Returns :math:`\mathbb{V}[X] = \mathbb{E}\left(X - \mathbb{E}[X]\right)^2`
+    def _var(self):
+        r"""Return element/entry-wise variance of the distribution.
 
         Returns
         -------
-        pd.DataFrame with same rows, columns as `self`
-        variance of distribution (entry-wise)
+        2D np.ndarray, same shape as ``self``
+            variance of the distribution (entry-wise)
         """
-        mu = self._mu
-        sigma = self._sigma
+        mu = self._bc_params["mu"]
+        sigma = self._bc_params["sigma"]
+
         sd_arr = np.exp(2 * mu + 2 * sigma**2) - np.exp(2 * mu + sigma**2)
-        return pd.DataFrame(sd_arr, index=self.index, columns=self.columns) ** 2
+        return sd_arr
+
+    def _pdf(self, x):
+        """Probability density function.
 
-    def pdf(self, x):
-        """Probability density function."""
-        d = self.loc[x.index, x.columns]
-        pdf_arr = np.exp(-0.5 * ((np.log(x.values) - d.mu) / d.sigma) ** 2)
-        pdf_arr = pdf_arr / (x.values * d.sigma * np.sqrt(2 * np.pi))
-        return pd.DataFrame(pdf_arr, index=x.index, columns=x.columns)
-
-    def log_pdf(self, x):
-        """Logarithmic probability density function."""
-        d = self.loc[x.index, x.columns]
-        lpdf_arr = -0.5 * ((np.log(x.values) - d.mu) / d.sigma) ** 2
-        lpdf_arr = lpdf_arr - np.log(x.values * d.sigma * np.sqrt(2 * np.pi))
-        return pd.DataFrame(lpdf_arr, index=x.index, columns=x.columns)
-
-    def cdf(self, x):
-        """Cumulative distribution function."""
-        d = self.loc[x.index, x.columns]
-        cdf_arr = 0.5 + 0.5 * erf((np.log(x.values) - d.mu) / (d.sigma * np.sqrt(2)))
-        return pd.DataFrame(cdf_arr, index=x.index, columns=x.columns)
-
-    def ppf(self, p):
-        """Quantile function = percent point function = inverse cdf."""
-        d = self.loc[p.index, p.columns]
-        icdf_arr = d.mu + d.sigma * np.sqrt(2) * erfinv(2 * p.values - 1)
+        Parameters
+        ----------
+        x : 2D np.ndarray, same shape as ``self``
+            values to evaluate the pdf at
+
+        Returns
+        -------
+        2D np.ndarray, same shape as ``self``
+            pdf values at the given points
+        """
+        mu = self._bc_params["mu"]
+        sigma = self._bc_params["sigma"]
+
+        pdf_arr = np.exp(-0.5 * ((np.log(x) - mu) / sigma) ** 2)
+        pdf_arr = pdf_arr / (x * sigma * np.sqrt(2 * np.pi))
+        return pdf_arr
+
+    def _log_pdf(self, x):
+        """Logarithmic probability density function.
+
+        Parameters
+        ----------
+        x : 2D np.ndarray, same shape as ``self``
+            values to evaluate the pdf at
+
+        Returns
+        -------
+        2D np.ndarray, same shape as ``self``
+            log pdf values at the given points
+        """
+        mu = self._bc_params["mu"]
+        sigma = self._bc_params["sigma"]
+
+        lpdf_arr = -0.5 * ((np.log(x) - mu) / sigma) ** 2
+        lpdf_arr = lpdf_arr - np.log(x * sigma * np.sqrt(2 * np.pi))
+        return lpdf_arr
+
+    def _cdf(self, x):
+        """Cumulative distribution function.
+
+        Parameters
+        ----------
+        x : 2D np.ndarray, same shape as ``self``
+            values to evaluate the cdf at
+
+        Returns
+        -------
+        2D np.ndarray, same shape as ``self``
+            cdf values at the given points
+        """
+        mu = self._bc_params["mu"]
+        sigma = self._bc_params["sigma"]
+
+        cdf_arr = 0.5 + 0.5 * erf((np.log(x) - mu) / (sigma * np.sqrt(2)))
+        return cdf_arr
+
+    def _ppf(self, p):
+        """Quantile function = percent point function = inverse cdf.
+
+        Parameters
+        ----------
+        p : 2D np.ndarray, same shape as ``self``
+            values to evaluate the ppf at
+
+        Returns
+        -------
+        2D np.ndarray, same shape as ``self``
+            ppf values at the given points
+        """
+        mu = self._bc_params["mu"]
+        sigma = self._bc_params["sigma"]
+
+        icdf_arr = mu + sigma * np.sqrt(2) * erfinv(2 * p - 1)
         icdf_arr = np.exp(icdf_arr)
-        return pd.DataFrame(icdf_arr, index=p.index, columns=p.columns)
+        return icdf_arr
 
     @classmethod
     def get_test_params(cls, parameter_set="default"):
         """Return testing parameter settings for the estimator."""
+        # array case examples
         params1 = {"mu": [[0, 1], [2, 3], [4, 5]], "sigma": 1}
         params2 = {
             "mu": 0,
             "sigma": 1,
             "index": pd.Index([1, 2, 5]),
             "columns": pd.Index(["a", "b"]),
         }
-        return [params1, params2]
+        # scalar case examples
+        params3 = {"mu": -2, "sigma": 2}
+
+        return [params1, params2, params3]
```

### Comparing `skpro-2.2.2/skpro/distributions/mixture.py` & `skpro-2.3.0/skpro/distributions/delta.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,194 +1,204 @@
 # copyright: skpro developers, BSD-3-Clause License (see LICENSE file)
-"""Mixture distribution."""
+"""Delta (constant/certain) probability distribution."""
 
 __author__ = ["fkiraly"]
 
 import numpy as np
 import pandas as pd
-from skbase.base import BaseMetaObject
 
 from skpro.distributions.base import BaseDistribution
 
 
-class Mixture(BaseMetaObject, BaseDistribution):
-    """Mixture of distributions.
+class Delta(BaseDistribution):
+    r"""Delta distribution aka constant distribution aka certain distribution.
+
+    This distribution always produces the same value when sampling - ``c``.
+    It it useful to represent a constant value as a distribution, e.g., as a baseline
+    method to create a probabilistic prediction from a point prediction.
+
+    The delta distribution is parametrized by a constant value :math:`c`.
+    For the cdf, we have:
+
+    .. math:: F(x) = 0 \text{ if } x < c, 1 \text{ if } x \geq c
+
+    The constant value :math:`c` is represented by the parameter ``c``.
 
     Parameters
     ----------
-    distributions : list of tuples (str, BaseDistribution) or BaseDistribution
-        list of mixture components
-    weights : list of float, optional, default = None
-        list of mixture weights, will be normalized to sum to 1
-        if not provided, uniform mixture is assumed
-    index : pd.Index, optional, default = inferred from component distributions
-    columns : pd.Index, optional, default = inferred from component distributions
+    c : float or array of float (1D or 2D)
+        support of the delta distribution
+    index : pd.Index, optional, default = RangeIndex
+    columns : pd.Index, optional, default = RangeIndex
 
     Example
     -------
-    >>> from skpro.distributions.mixture import Mixture
-    >>> from skpro.distributions.normal import Normal
+    >>> from skpro.distributions.delta import Delta
 
-    >>> n1 = Normal(mu=[[0, 1], [2, 3], [4, 5]], sigma=1)
-    >>> n2 = Normal(mu=3, sigma=2, index=n1.index, columns=n1.columns)
-    >>> m = Mixture(distributions=[("n1", n1), ("n2", n2)], weights=[0.3, 0.7])
-    >>> mixture_sample = m.sample(n_samples=10)
+    >>> delta = Delta(c=[[0, 1], [2, 3], [4, 5]])
+    >>> this_is_always_c = delta.sample()
     """
 
     _tags = {
-        "capabilities:approx": ["pdfnorm", "energy", "ppf"],
-        "capabilities:exact": ["mean", "var", "pdf", "log_pdf", "cdf"],
-        "distr:measuretype": "mixed",
-        "named_object_parameters": "_distributions",
+        "capabilities:approx": [],
+        "capabilities:exact": ["mean", "var", "energy", "pmf", "log_pmf", "cdf", "ppf"],
+        "distr:measuretype": "discrete",
+        "distr:paramtype": "nonparametric",
+        "broadcast_init": "on",
     }
 
-    def __init__(self, distributions, weights=None, index=None, columns=None):
-        self.distributions = distributions
-        self.weights = weights
-        self.index = index
-        self.columns = columns
-
-        self._distributions = self._coerce_to_named_object_tuples(distributions)
-        n_dists = len(self._distributions)
-
-        if weights is None:
-            self._weights = np.ones(n_dists) / n_dists
-        else:
-            self._weights = np.array(weights) / np.sum(weights)
+    def __init__(self, c, index=None, columns=None):
+        self.c = c
+        if index is None and hasattr(c, "index") and isinstance(c.index, pd.Index):
+            index = c.index
+        if columns is None and hasattr(c, "columns"):
+            if isinstance(c.columns, pd.Index):
+                columns = c.columns
 
-        if index is None:
-            index = self._distributions[0][1].index
+        super().__init__(index=index, columns=columns)
 
-        if columns is None:
-            columns = self._distributions[0][1].columns
+    def _energy_self(self):
+        r"""Energy of self, w.r.t. self.
 
-        super().__init__(index=index, columns=columns)
+        :math:`\mathbb{E}[|X-Y|]`, where :math:`X, Y` are i.i.d. copies of self.
 
-    def _iloc(self, rowidx=None, colidx=None):
-        dists = self._distributions
-        weights = self.weights
+        Private method, to be implemented by subclasses.
 
-        dists_subset = [(x[0], x[1].iloc[rowidx, colidx]) for x in dists]
+        Returns
+        -------
+        2D np.ndarray, same shape as ``self``
+            energy values w.r.t. the given points
+        """
+        # energy of self w.r.t. self is always 0
+        energy_arr = self._coerce_to_self_index_np(0)
+        if energy_arr.ndim > 0:
+            energy_arr = np.sum(energy_arr, axis=1)
+        return energy_arr
 
-        index_subset = dists_subset[0][1].index
-        columns_subset = dists_subset[0][1].columns
+    def _energy_x(self, x):
+        r"""Energy of self, w.r.t. a constant frame x.
 
-        return Mixture(
-            distributions=dists_subset,
-            weights=weights,
-            index=index_subset,
-            columns=columns_subset,
-        )
+        :math:`\mathbb{E}[|X-x|]`, where :math:`X` is a copy of self,
+        and :math:`x` is a constant.
 
-    def mean(self):
-        r"""Return expected value of the distribution.
+        Private method, to be implemented by subclasses.
 
-        Let :math:`X` be a random variable with the distribution of `self`.
-        Returns the expectation :math:`\mathbb{E}[X]`
+        Parameters
+        ----------
+        x : 2D np.ndarray, same shape as ``self``
+            values to compute energy w.r.t. to
 
         Returns
         -------
-        pd.DataFrame with same rows, columns as `self`
-        expected value of distribution (entry-wise)
+        2D np.ndarray, same shape as ``self``
+            energy values w.r.t. the given points
         """
-        return self._average("mean")
+        c = self._bc_params["c"]
 
-    def var(self):
-        r"""Return element/entry-wise variance of the distribution.
+        energy_arr = np.abs(c - x)
+        if energy_arr.ndim > 0:
+            energy_arr = np.sum(energy_arr, axis=1)
+        return energy_arr
 
-        Let :math:`X` be a random variable with the distribution of `self`.
-        Returns :math:`\mathbb{V}[X] = \mathbb{E}\left(X - \mathbb{E}[X]\right)^2`
+    def _mean(self):
+        """Return expected value of the distribution.
 
         Returns
         -------
-        pd.DataFrame with same rows, columns as `self`
-        variance of distribution (entry-wise)
+        2D np.ndarray, same shape as ``self``
+            expected value of distribution (entry-wise)
         """
-        weights = self._weights
-        var_mean = self._average("var")
-        mixture_mean = self._average("mean")
-
-        means = [d.mean() for _, d in self._distributions]
-        mean_var = [(m - mixture_mean) ** 2 for m in means]
-        var_mean_var = self._average_df(mean_var, weights=weights)
+        return self._bc_params["c"]
 
-        return var_mean + var_mean_var
+    def _var(self):
+        r"""Return element/entry-wise variance of the distribution.
 
-    def _average(self, method, x=None, weights=None):
-        """Average a method over the mixture components."""
-        if x is None:
-            args = ()
-        else:
-            args = (x,)
+        Returns
+        -------
+        2D np.ndarray, same shape as ``self``
+            variance of the distribution (entry-wise)
+        """
+        # variance of a constant is always 0
+        return self._coerce_to_self_index_np(0)
 
-        vals = [getattr(d, method)(*args) for _, d in self._distributions]
+    def _pmf(self, x):
+        """Probability mass function.
 
-        return self._average_df(vals, weights=weights)
+        Parameters
+        ----------
+        x : 2D np.ndarray, same shape as ``self``
+            values to evaluate the pmf at
 
-    def _average_df(self, df_list, weights=None):
-        """Average a list of `pd.DataFrame` objects, with weights."""
-        if weights is None and hasattr(self, "_weights"):
-            weights = self._weights
-        elif weights is None:
-            weights = np.ones(len(df_list)) / len(df_list)
+        Returns
+        -------
+        2D np.ndarray, same shape as ``self``
+            pmf values at the given points
+        """
+        c = self._bc_params["c"]
+        pmf_arr = np.where(x == c, 1, 0)
+        return pmf_arr
 
-        n_df = len(df_list)
-        df_weighted = [df * w for df, w in zip(df_list, weights)]
-        df_concat = pd.concat(df_weighted, axis=1, keys=range(n_df))
-        df_res = df_concat.T.groupby(level=-1).sum().T
-        return df_res
+    def _log_pmf(self, x):
+        """Logarithmic probability mass function.
 
-    def pdf(self, x):
-        """Probability density function."""
-        return self._average("pdf", x)
+        Parameters
+        ----------
+        x : 2D np.ndarray, same shape as ``self``
+            values to evaluate the pmf at
 
-    def cdf(self, x):
-        """Cumulative distribution function."""
-        return self._average("cdf", x)
+        Returns
+        -------
+        2D np.ndarray, same shape as ``self``
+            log pmf values at the given points
+        """
+        c = self._bc_params["c"]
+        lpmf_arr = np.where(x == c, 0, -np.inf)
+        return lpmf_arr
 
-    def sample(self, n_samples=None):
-        """Sample from the distribution.
+    def _cdf(self, x):
+        """Cumulative distribution function.
 
         Parameters
         ----------
-        n_samples : int, optional, default = None
+        x : 2D np.ndarray, same shape as ``self``
+            values to evaluate the cdf at
 
         Returns
         -------
-        if `n_samples` is `None`:
-        returns a sample that contains a single sample from `self`,
-        in `pd.DataFrame` mtype format convention, with `index` and `columns` as `self`
-        if n_samples is `int`:
-        returns a `pd.DataFrame` that contains `n_samples` i.i.d. samples from `self`,
-        in `pd-multiindex` mtype format convention, with same `columns` as `self`,
-        and `MultiIndex` that is product of `RangeIndex(n_samples)` and `self.index`
+        2D np.ndarray, same shape as ``self``
+            cdf values at the given points
         """
-        if n_samples is None:
-            N = 1
-        else:
-            N = n_samples
+        c = self._bc_params["c"]
+
+        cdf_arr = np.where(x < c, 0, 1)
+        return cdf_arr
 
-        n_dist = len(self._distributions)
-        selector = np.random.choice(n_dist, size=N, p=self._weights)
+    def _ppf(self, p):
+        """Quantile function = percent point function = inverse cdf.
 
-        samples = [self._distributions[i][1].sample() for i in selector]
+        Parameters
+        ----------
+        p : 2D np.ndarray, same shape as ``self``
+            values to evaluate the ppf at
 
-        if n_samples is None:
-            return samples[0]
-        else:
-            return pd.concat(samples, axis=0, keys=range(N))
+        Returns
+        -------
+        2D np.ndarray, same shape as ``self``
+            ppf values at the given points
+        """
+        c = self._bc_params["c"]
+        icdf_arr = c
+        return icdf_arr
 
     @classmethod
     def get_test_params(cls, parameter_set="default"):
         """Return testing parameter settings for the estimator."""
-        from skpro.distributions.normal import Normal
-
-        index = pd.RangeIndex(3)
-        columns = pd.Index(["a", "b"])
-        normal1 = Normal(mu=0, sigma=1, index=index, columns=columns)
-        normal2 = Normal(mu=[[0, 1], [2, 3], [4, 5]], sigma=1, columns=columns)
-
-        dists = [("normal1", normal1), ("normal2", normal2)]
-
-        params1 = {"distributions": dists}
-        params2 = {"distributions": dists, "weights": [0.3, 0.7]}
-        return [params1, params2]
+        # array case examples
+        params1 = {"c": [[0, 1], [2, 3], [4, 5]]}
+        params2 = {
+            "c": 42,
+            "index": pd.Index([1, 2, 5]),
+            "columns": pd.Index(["a", "b"]),
+        }
+        # scalar case examples
+        params3 = {"c": 42}
+        return [params1, params2, params3]
```

### Comparing `skpro-2.2.2/skpro/distributions/normal.py` & `skpro-2.3.0/skpro/distributions/chi_squared.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,151 +1,162 @@
 # copyright: skpro developers, BSD-3-Clause License (see LICENSE file)
-"""Normal/Gaussian probability distribution."""
+"""Chi-Squared probability distribution."""
 
-__author__ = ["fkiraly"]
+__author__ = ["sukjingitsit"]
 
-import numpy as np
 import pandas as pd
-from scipy.special import erf, erfinv
+from scipy.stats.distributions import chi2
 
 from skpro.distributions.base import BaseDistribution
 
 
-class Normal(BaseDistribution):
-    """Normal distribution (skpro native).
+class ChiSquared(BaseDistribution):
+    """Chi-Squared distribution (skpro native).
 
     Parameters
     ----------
-    mu : float or array of float (1D or 2D)
-        mean of the normal distribution
-    sigma : float or array of float (1D or 2D), must be positive
-        standard deviation of the normal distribution
+    dof : float or array of float (1D or 2D)
+        degrees of freedom of the chi-squared distribution
     index : pd.Index, optional, default = RangeIndex
     columns : pd.Index, optional, default = RangeIndex
 
     Example
     -------
-    >>> from skpro.distributions.normal import Normal
-
-    >>> n = Normal(mu=[[0, 1], [2, 3], [4, 5]], sigma=1)
+    >>> from skpro.distributions.chi_squared import ChiSquared
+    >>> chi = ChiSquared(dof=[[1, 2], [3, 4], [5, 6]])
     """
 
     _tags = {
-        "capabilities:approx": ["pdfnorm"],
-        "capabilities:exact": ["mean", "var", "energy", "pdf", "log_pdf", "cdf", "ppf"],
+        # packaging info
+        # --------------
+        "authors": "sukjingitsit",
+        # estimator tags
+        # --------------
+        "capabilities:exact": ["mean", "var", "pdf", "log_pdf", "cdf", "ppf"],
         "distr:measuretype": "continuous",
+        "distr:paramtype": "parametric",
+        "broadcast_init": "on",
     }
 
-    def __init__(self, mu, sigma, index=None, columns=None):
-        self.mu = mu
-        self.sigma = sigma
-        self.index = index
-        self.columns = columns
-
-        # todo: untangle index handling
-        # and broadcast of parameters.
-        # move this functionality to the base class
-        self._mu, self._sigma = self._get_bc_params(self.mu, self.sigma)
-        shape = self._mu.shape
+    def __init__(self, dof, index=None, columns=None):
+        self.dof = dof
 
-        if index is None:
-            index = pd.RangeIndex(shape[0])
+        super().__init__(index=index, columns=columns)
 
-        if columns is None:
-            columns = pd.RangeIndex(shape[1])
+    r"""Energy implementation issues:
 
-        super().__init__(index=index, columns=columns)
+    The self-energy is mathematically difficult to calculate due to
+    their being no proper closed form. As discussed with fkiraly,
+    using E(d.energy(x)) is one possible way, but the question arises
+    on how to approximate the integral. The other alternative is to use
+    sampling to estimate the self-energy.
+
+    The closed form version for cross-energy can be framed as follows:
+    Here, :math:`k=dof`
+    :math:`x <= 0, \operatorname{energy}(x) = k + \vert x \vert`
+    :math:`x > 0, \operatorname{energy}(x) =
+    x*(2*\operatorname{CDF}(k,x)-1)+k-2k*\operatorname{CDF}(k+1,x)`
+    where :math:`\operatorname{CDF}(k,x)` represents the CDF of x
+    for a chi-square distribution with k degrees of freedom.
+    """
+
+    def _mean(self):
+        """Return expected value of the distribution.
+
+        Returns
+        -------
+        2D np.ndarray, same shape as ``self``
+            expected value of distribution (entry-wise)
+        """
+        return self._bc_params["dof"]
+
+    def _var(self):
+        r"""Return element/entry-wise variance of the distribution.
+
+        Returns
+        -------
+        2D np.ndarray, same shape as ``self``
+            variance of the distribution (entry-wise)
+        """
+        return 2 * self._bc_params["dof"]
 
-    def energy(self, x=None):
-        r"""Energy of self, w.r.t. self or a constant frame x.
+    def _pdf(self, x):
+        """Probability density function.
 
-        Let :math:`X, Y` be i.i.d. random variables with the distribution of `self`.
+        Parameters
+        ----------
+        x : 2D np.ndarray, same shape as ``self``
+            values to evaluate the pdf at
 
-        If `x` is `None`, returns :math:`\mathbb{E}[|X-Y|]` (per row), "self-energy".
-        If `x` is passed, returns :math:`\mathbb{E}[|X-x|]` (per row), "energy wrt x".
+        Returns
+        -------
+        2D np.ndarray, same shape as ``self``
+            pdf values at the given points
+        """
+        dof = self._bc_params["dof"]
+        pdf_arr = chi2.pdf(x, dof)
+        return pdf_arr
+
+    def _log_pdf(self, x):
+        """Logarithmic probability density function.
 
         Parameters
         ----------
-        x : None or pd.DataFrame, optional, default=None
-            if pd.DataFrame, must have same rows and columns as `self`
+        x : 2D np.ndarray, same shape as ``self``
+            values to evaluate the pdf at
 
         Returns
         -------
-        pd.DataFrame with same rows as `self`, single column `"energy"`
-        each row contains one float, self-energy/energy as described above.
+        2D np.ndarray, same shape as ``self``
+            log pdf values at the given points
         """
-        if x is None:
-            sd_arr = self._sigma
-            energy_arr = 2 * np.sum(sd_arr, axis=1) / np.sqrt(np.pi)
-            energy = pd.DataFrame(energy_arr, index=self.index, columns=["energy"])
-        else:
-            mu_arr, sd_arr = self._mu, self._sigma
-            c_arr = (x - mu_arr) * (2 * self.cdf(x) - 1) + 2 * sd_arr**2 * self.pdf(x)
-            energy_arr = np.sum(c_arr, axis=1)
-            energy = pd.DataFrame(energy_arr, index=self.index, columns=["energy"])
-        return energy
+        dof = self._bc_params["dof"]
+        lpdf_arr = chi2.logpdf(x, dof)
+        return lpdf_arr
 
-    def mean(self):
-        r"""Return expected value of the distribution.
+    def _cdf(self, x):
+        """Cumulative distribution function.
 
-        Let :math:`X` be a random variable with the distribution of `self`.
-        Returns the expectation :math:`\mathbb{E}[X]`
+        Parameters
+        ----------
+        x : 2D np.ndarray, same shape as ``self``
+            values to evaluate the cdf at
 
         Returns
         -------
-        pd.DataFrame with same rows, columns as `self`
-        expected value of distribution (entry-wise)
+        2D np.ndarray, same shape as ``self``
+            cdf values at the given points
         """
-        mean_arr = self._mu
-        return pd.DataFrame(mean_arr, index=self.index, columns=self.columns)
+        dof = self._bc_params["dof"]
+        cdf_arr = chi2.cdf(x, dof)
+        return cdf_arr
 
-    def var(self):
-        r"""Return element/entry-wise variance of the distribution.
+    def _ppf(self, p):
+        """Quantile function = percent point function = inverse cdf.
 
-        Let :math:`X` be a random variable with the distribution of `self`.
-        Returns :math:`\mathbb{V}[X] = \mathbb{E}\left(X - \mathbb{E}[X]\right)^2`
+        Parameters
+        ----------
+        p : 2D np.ndarray, same shape as ``self``
+            values to evaluate the ppf at
 
         Returns
         -------
-        pd.DataFrame with same rows, columns as `self`
-        variance of distribution (entry-wise)
+        2D np.ndarray, same shape as ``self``
+            ppf values at the given points
         """
-        sd_arr = self._sigma
-        return pd.DataFrame(sd_arr, index=self.index, columns=self.columns) ** 2
-
-    def pdf(self, x):
-        """Probability density function."""
-        d = self.loc[x.index, x.columns]
-        pdf_arr = np.exp(-0.5 * ((x.values - d.mu) / d.sigma) ** 2)
-        pdf_arr = pdf_arr / (d.sigma * np.sqrt(2 * np.pi))
-        return pd.DataFrame(pdf_arr, index=x.index, columns=x.columns)
-
-    def log_pdf(self, x):
-        """Logarithmic probability density function."""
-        d = self.loc[x.index, x.columns]
-        lpdf_arr = -0.5 * ((x.values - d.mu) / d.sigma) ** 2
-        lpdf_arr = lpdf_arr - np.log(d.sigma * np.sqrt(2 * np.pi))
-        return pd.DataFrame(lpdf_arr, index=x.index, columns=x.columns)
-
-    def cdf(self, x):
-        """Cumulative distribution function."""
-        d = self.loc[x.index, x.columns]
-        cdf_arr = 0.5 + 0.5 * erf((x.values - d.mu) / (d.sigma * np.sqrt(2)))
-        return pd.DataFrame(cdf_arr, index=x.index, columns=x.columns)
-
-    def ppf(self, p):
-        """Quantile function = percent point function = inverse cdf."""
-        d = self.loc[p.index, p.columns]
-        icdf_arr = d.mu + d.sigma * np.sqrt(2) * erfinv(2 * p.values - 1)
-        return pd.DataFrame(icdf_arr, index=p.index, columns=p.columns)
+        dof = self._bc_params["dof"]
+        icdf_arr = chi2.ppf(p, dof)
+        return icdf_arr
 
     @classmethod
     def get_test_params(cls, parameter_set="default"):
         """Return testing parameter settings for the estimator."""
-        params1 = {"mu": [[0, 1], [2, 3], [4, 5]], "sigma": 1}
+        # array case examples
+        params1 = {"dof": [[1, 2], [3, 4], [5, 6]]}
         params2 = {
-            "mu": 0,
-            "sigma": 1,
+            "dof": 10,
             "index": pd.Index([1, 2, 5]),
             "columns": pd.Index(["a", "b"]),
         }
-        return [params1, params2]
+        # scalar case examples
+        params3 = {"dof": 3}
+        return [params1, params2, params3]
```

### Comparing `skpro-2.2.2/skpro/distributions/qpd_empirical.py` & `skpro-2.3.0/skpro/distributions/qpd_empirical.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/distributions/t.py` & `skpro-2.3.0/skpro/distributions/t.py`

 * *Files 22% similar despite different names*

```diff
@@ -33,55 +33,47 @@
 
     _tags = {
         "authors": ["Alex-JG3"],
         "maintainers": ["Alex-JG3"],
         "capabilities:approx": ["pdfnorm", "energy"],
         "capabilities:exact": ["mean", "var", "pdf", "log_pdf", "cdf", "ppf"],
         "distr:measuretype": "continuous",
+        "distr:paramtype": "parametric",
+        "broadcast_init": "on",
     }
 
     def __init__(self, mu, sigma, df=1, index=None, columns=None):
         self.mu = mu
         self.sigma = sigma
         self.df = df
-        self.index = index
-        self.columns = columns
-
-        self._mu, self._sigma, self._df = self._get_bc_params(
-            self.mu, self.sigma, self.df
-        )
-        shape = self._mu.shape
-
-        if index is None:
-            index = pd.RangeIndex(shape[0])
-
-        if columns is None:
-            columns = pd.RangeIndex(shape[1])
 
         super().__init__(index=index, columns=columns)
 
-    def mean(self):
-        r"""Return expected value of the distribution.
-
-        Let :math:`X` be a random variable with the distribution of `self`.
-        Returns the expectation :math:`\mathbb{E}[X]`. The expectation,
-        :math:`\mathbb{E}[X]`, as infinite if :math:`\nu \le 1`.
+    def _mean(self):
+        """Return expected value of the distribution.
 
         Returns
         -------
-        pd.DataFrame with same rows, columns as `self`
-        expected value of distribution (entry-wise)
+        2D np.ndarray, same shape as ``self``
+            expected value of distribution (entry-wise)
         """
-        mean_arr = self._mu.copy()
-        if (self._df <= 1).any():
+        mean_arr = self._bc_params["mu"]
+        df = self._bc_params["df"]
+
+        if self.ndim == 0:
+            if df <= 1:
+                return np.inf
+            return mean_arr
+
+        if (df <= 1).any():
             mean_arr = mean_arr.astype(np.float32)
-            mean_arr[self._df <= 1] = np.inf
-        return pd.DataFrame(mean_arr, index=self.index, columns=self.columns)
+            mean_arr[df <= 1] = np.inf
+        return mean_arr
 
-    def var(self):
+    def _var(self):
         r"""Return element/entry-wise variance of the distribution.
 
         Let :math:`X` be a random variable with the distribution of `self`.
         Returns,
 
         .. math::
             \mathbb{V}[X] = \begin{cases}
@@ -92,77 +84,142 @@
         Where :math:`\nu` is the degrees of freedom of the t-distribution.
 
         Returns
         -------
         pd.DataFrame with same rows, columns as `self`
         variance of distribution (entry-wise)
         """
-        df_arr = self._df.copy()
-        df_arr = df_arr.astype(np.float32)
+        sigma = self._bc_params["sigma"]
+        df = self._bc_params["df"]
+        df_arr = df.astype(np.float32)
+
+        if self.ndim == 0:
+            if df <= 2:
+                return np.inf
+            return sigma**2 * df / (df - 2)
+
         df_arr[df_arr <= 2] = np.inf
         mask = (df_arr > 2) & (df_arr != np.inf)
-        df_arr[mask] = self._sigma[mask] ** 2 * df_arr[mask] / (df_arr[mask] - 2)
-        return pd.DataFrame(df_arr, index=self.index, columns=self.columns)
+        df_arr[mask] = sigma[mask] ** 2 * df_arr[mask] / (df_arr[mask] - 2)
+        return df_arr
+
+    def _pdf(self, x):
+        """Probability density function.
+
+        Parameters
+        ----------
+        x : 2D np.ndarray, same shape as ``self``
+            values to evaluate the pdf at
+
+        Returns
+        -------
+        2D np.ndarray, same shape as ``self``
+            pdf values at the given points
+        """
+        df = self._bc_params["df"]
+        mu = self._bc_params["mu"]
+        sigma = self._bc_params["sigma"]
+
+        pdf_arr = gamma((df + 1) / 2)
+        pdf_arr = pdf_arr / (np.sqrt(np.pi * df) * gamma(df / 2))
+        pdf_arr = pdf_arr * (1 + ((x - mu) / sigma) ** 2 / df) ** (-(df + 1) / 2)
+        pdf_arr = pdf_arr / sigma
+        return pdf_arr
+
+    def _log_pdf(self, x):
+        """Logarithmic probability density function.
+
+        Parameters
+        ----------
+        x : 2D np.ndarray, same shape as ``self``
+            values to evaluate the pdf at
 
-    def pdf(self, x):
-        """Probability density function."""
-        d = self.loc[x.index, x.columns]
-        pdf_arr = gamma((d._df + 1) / 2)
-        pdf_arr = pdf_arr / (np.sqrt(np.pi * d._df) * gamma(d._df / 2))
-        pdf_arr = pdf_arr * (1 + ((x - d._mu) / d._sigma) ** 2 / d._df) ** (
-            -(d._df + 1) / 2
-        )
-        pdf_arr = pdf_arr / d._sigma
-        return pd.DataFrame(pdf_arr, index=x.index, columns=x.columns)
-
-    def log_pdf(self, x):
-        """Logarithmic probability density function."""
-        d = self.loc[x.index, x.columns]
-        lpdf_arr = loggamma((d._df + 1) / 2)
-        lpdf_arr = lpdf_arr - 0.5 * np.log(d._df * np.pi)
-        lpdf_arr = lpdf_arr - loggamma(d._df / 2)
-        lpdf_arr = lpdf_arr - ((d._df + 1) / 2) * np.log(
-            1 + ((x - d._mu) / d._sigma) ** 2 / d._df
-        )
-        lpdf_arr = lpdf_arr - np.log(d._sigma)
-        return pd.DataFrame(lpdf_arr, index=x.index, columns=x.columns)
-
-    def cdf(self, x):
-        """Cumulative distribution function."""
-        d = self.loc[x.index, x.columns]
-        x_ = (x - d._mu) / d._sigma
-        cdf_arr = x_ * gamma((d._df + 1) / 2)
-        cdf_arr = cdf_arr * hyp2f1(0.5, (d._df + 1) / 2, 3 / 2, -(x_**2) / d._df)
-        cdf_arr = 0.5 + cdf_arr / (np.sqrt(np.pi * d._df) * gamma(d._df / 2))
-        return pd.DataFrame(cdf_arr, index=x.index, columns=x.columns)
-
-    def ppf(self, p):
-        """Quantile function = percent point function = inverse cdf."""
-        d = self.loc[p.index, p.columns]
-        ppf_arr = p.to_numpy(copy=True)
-        ppf_arr[p.values == 0.5] = 0.0
-        ppf_arr[p.values <= 0] = -np.inf
-        ppf_arr[p.values >= 1] = np.inf
-
-        mask1 = (p.values < 0.5) & (p.values > 0)
-        mask2 = (p.values < 1) & (p.values > 0.5)
-        ppf_arr[mask1] = 1 / betaincinv(0.5 * d._df[mask1], 0.5, 2 * ppf_arr[mask1])
-        ppf_arr[mask2] = 1 / betaincinv(
-            0.5 * d._df[mask2], 0.5, 2 * (1 - ppf_arr[mask2])
-        )
+        Returns
+        -------
+        2D np.ndarray, same shape as ``self``
+            log pdf values at the given points
+        """
+        df = self._bc_params["df"]
+        mu = self._bc_params["mu"]
+        sigma = self._bc_params["sigma"]
+
+        lpdf_arr = loggamma((df + 1) / 2)
+        lpdf_arr = lpdf_arr - 0.5 * np.log(df * np.pi)
+        lpdf_arr = lpdf_arr - loggamma(df / 2)
+        lpdf_arr = lpdf_arr - ((df + 1) / 2) * np.log(1 + ((x - mu) / sigma) ** 2 / df)
+        lpdf_arr = lpdf_arr - np.log(sigma)
+        return lpdf_arr
+
+    def _cdf(self, x):
+        """Cumulative distribution function.
+
+        Parameters
+        ----------
+        x : 2D np.ndarray, same shape as ``self``
+            values to evaluate the cdf at
+
+        Returns
+        -------
+        2D np.ndarray, same shape as ``self``
+            cdf values at the given points
+        """
+        df = self._bc_params["df"]
+        mu = self._bc_params["mu"]
+        sigma = self._bc_params["sigma"]
+
+        x_ = (x - mu) / sigma
+        cdf_arr = x_ * gamma((df + 1) / 2)
+        cdf_arr = cdf_arr * hyp2f1(0.5, (df + 1) / 2, 3 / 2, -(x_**2) / df)
+        cdf_arr = 0.5 + cdf_arr / (np.sqrt(np.pi * df) * gamma(df / 2))
+        return cdf_arr
+
+    def _ppf(self, p):
+        """Quantile function = percent point function = inverse cdf.
+
+        Parameters
+        ----------
+        p : 2D np.ndarray, same shape as ``self``
+            values to evaluate the ppf at
+
+        Returns
+        -------
+        2D np.ndarray, same shape as ``self``
+            ppf values at the given points
+        """
+        df = self._bc_params["df"]
+        mu = self._bc_params["mu"]
+        sigma = self._bc_params["sigma"]
+
+        ppf_arr = p.copy()
+        ppf_arr[p == 0.5] = 0.0
+        ppf_arr[p <= 0] = -np.inf
+        ppf_arr[p >= 1] = np.inf
+
+        mask1 = (p < 0.5) & (p > 0)
+        mask2 = (p < 1) & (p > 0.5)
+        ppf_arr[mask1] = 1 / betaincinv(0.5 * df[mask1], 0.5, 2 * ppf_arr[mask1])
+        ppf_arr[mask2] = 1 / betaincinv(0.5 * df[mask2], 0.5, 2 * (1 - ppf_arr[mask2]))
         ppf_arr[mask1 | mask2] = np.sqrt(ppf_arr[mask1 | mask2] - 1)
-        ppf_arr[mask1 | mask2] = np.sqrt(d._df[mask1 | mask2]) * ppf_arr[mask1 | mask2]
+        ppf_arr[mask1 | mask2] = np.sqrt(df[mask1 | mask2]) * ppf_arr[mask1 | mask2]
         ppf_arr[mask1] = -ppf_arr[mask1]
-        ppf_arr = d._sigma * ppf_arr + d._mu
-        return pd.DataFrame(ppf_arr, index=p.index, columns=p.columns)
+        ppf_arr = sigma * ppf_arr + mu
+        return ppf_arr
 
     @classmethod
     def get_test_params(cls, parameter_set="default"):
         """Return testing parameter settings for the estimator."""
-        params1 = {"mu": [[0, 1], [2, 3], [4, 5]], "sigma": 1}
+        # array case examples
+        params1 = {
+            "mu": [[0, 1], [2, 3], [4, 5]],
+            "sigma": 1,
+            "df": [2, 3],
+        }
         params2 = {
             "mu": 0,
             "sigma": 1,
             "index": pd.Index([1, 2, 5]),
             "columns": pd.Index(["a", "b"]),
         }
-        return [params1, params2]
+        # scalar case examples
+        params3 = {"mu": -2, "sigma": 3, "df": 4}
+
+        return [params1, params2, params3]
```

### Comparing `skpro-2.2.2/skpro/distributions/tests/test_all_distrs.py` & `skpro-2.3.0/skpro/distributions/tests/test_all_distrs.py`

 * *Files 18% similar despite different names*

```diff
@@ -46,16 +46,16 @@
     approx_methods = distr.get_tag("capabilities:approx")
     exact_methods = distr.get_tag("capabilities:exact")
     return method in approx_methods or method in exact_methods
 
 
 METHODS_SCALAR = ["mean", "var", "energy"]
 METHODS_SCALAR_POS = ["var", "energy"]  # result always non-negative?
-METHODS_X = ["energy", "pdf", "log_pdf", "cdf"]
-METHODS_X_POS = ["energy", "pdf", "cdf"]  # result always non-negative?
+METHODS_X = ["energy", "pdf", "log_pdf", "pmf", "log_pmf", "cdf"]
+METHODS_X_POS = ["energy", "pdf", "pmf", "cdf", "surv", "haz"]  # result non-negative?
 METHODS_P = ["ppf"]
 METHODS_ROWWISE = ["energy"]  # results in one column
 
 
 class TestAllDistributions(PackageConfig, DistributionFixtureGenerator, QuickTester):
     """Module level tests for all skpro parameter fitters."""
 
@@ -64,42 +64,59 @@
     exclude_objects = ["QPD_B"]
     # remove this when fixing failures to re-enable testing
 
     def test_shape(self, object_instance):
         """Test index, columns, len and shape of distribution."""
         d = object_instance
 
-        assert isinstance(d.index, pd.Index)
-        assert isinstance(d.columns, pd.Index)
-
+        assert hasattr(d, "shape")
         assert isinstance(d.shape, tuple)
-        assert len(d.shape) == 2
+        assert len(d.shape) in [0, 2]
+
+        if len(d.shape) == 2:
+            assert all(isinstance(n, int) for n in d.shape)
+
+            assert isinstance(d.index, pd.Index)
+            assert isinstance(d.columns, pd.Index)
 
-        assert d.shape[0] == len(d.index)
-        assert d.shape[1] == len(d.columns)
+            assert d.shape[0] == len(d.index)
+            assert d.shape[1] == len(d.columns)
 
         assert isinstance(len(d), int)
-        assert len(d) == d.shape[0]
+
+        if len(d.shape) == 2:
+            assert len(d) == d.shape[0]
+        else:
+            assert len(d) == 1
+
+        assert hasattr(d, "ndim")
+        assert d.ndim == len(d.shape)
 
     @pytest.mark.parametrize("shuffled", [False, True])
     def test_sample(self, object_instance, shuffled):
         """Test sample expected return."""
         d = object_instance
 
         if shuffled:
             d = _shuffle_distr(d)
 
         res = d.sample()
 
-        assert d.shape == res.shape
-        assert (res.index == d.index).all()
-        assert (res.columns == d.columns).all()
+        if d.ndim > 0:
+            assert d.shape == res.shape
+            assert (res.index == d.index).all()
+            assert (res.columns == d.columns).all()
+        else:  # d.ndim = 0
+            assert np.isscalar(res)
 
         res_panel = d.sample(3)
-        dummy_panel = pd.concat([res, res, res], keys=range(3))
+        if d.ndim > 0:
+            dummy_panel = pd.concat([res, res, res], keys=range(3))
+        else:
+            dummy_panel = pd.DataFrame(index=range(3), columns=range(1))
         assert dummy_panel.shape == res_panel.shape
         assert (res_panel.index == dummy_panel.index).all()
         assert (res_panel.columns == dummy_panel.columns).all()
 
     @pytest.mark.parametrize("shuffled", [False, True])
     @pytest.mark.parametrize("method", METHODS_SCALAR, ids=METHODS_SCALAR)
     def test_methods_scalar(self, object_instance, method, shuffled):
@@ -141,15 +158,19 @@
 
         d = object_instance
 
         if shuffled:
             d = _shuffle_distr(d)
 
         np_unif = np.random.uniform(size=d.shape)
-        p = pd.DataFrame(np_unif, index=d.index, columns=d.columns)
+        if d.ndim > 0:
+            p = pd.DataFrame(np_unif, index=d.index, columns=d.columns)
+        else:
+            p = np_unif
+
         res = getattr(object_instance, method)(p)
 
         _check_output_format(res, d, method)
 
     @pytest.mark.parametrize("q", [0.7, [0.1, 0.3, 0.9]])
     def test_quantile(self, object_instance, q):
         """Test expected return of quantile method."""
@@ -158,29 +179,38 @@
 
         d = object_instance
 
         def _check_quantile_output(obj, q):
             assert check_is_mtype(
                 obj, "pred_quantiles", "Proba", msg_return_dict="list"
             )
-            assert (obj.index == d.index).all()
+            if d.ndim == 0:
+                expected_index = pd.RangeIndex(1)
+                vars = [d.__class__.__name__]
+            else:
+                expected_index = d.index
+                vars = d.columns
+
+            assert (obj.index == expected_index).all()
 
             if not isinstance(q, list):
                 q = [q]
-            expected_columns = pd.MultiIndex.from_product([d.columns, q])
+            expected_columns = pd.MultiIndex.from_product([vars, q])
             assert (obj.columns == expected_columns).all()
 
         res = d.quantile(q)
         _check_quantile_output(res, q)
 
     @pytest.mark.parametrize("subset_row", [True, False])
     @pytest.mark.parametrize("subset_col", [True, False])
     def test_subsetting(self, object_instance, subset_row, subset_col):
         """Test subsetting of distribution."""
         d = object_instance
+        if d.ndim == 0:  # no subsetting to test if example is scalar
+            return None
 
         if subset_row:
             ix_loc = random_ss_ix(d.index, 3)
             ix_iloc = d.index.get_indexer(ix_loc)
         else:
             ix_loc = d.index
             ix_iloc = pd.RangeIndex(len(d.index))
@@ -214,28 +244,52 @@
         if "log_pdf" not in capabilities_exact or "pdf" not in capabilities_exact:
             return
         x = d.sample()
         pdf = d.pdf(x)
         log_pdf = d.log_pdf(x)
         assert np.allclose(np.log(pdf), log_pdf)
 
+    def test_log_pmf_and_pmf(self, object_instance):
+        """Test that the log of the pmf and log_pmf function are similar."""
+        d = object_instance
+        capabilities_exact = d.get_tags()["capabilities:exact"]
+
+        if "log_pmf" not in capabilities_exact or "pmf" not in capabilities_exact:
+            return
+        x = d.sample()
+        pmf = d.pmf(x)
+        log_pmf = d.log_pmf(x)
+        assert np.allclose(np.log(pmf), log_pmf)
+
     def test_ppf_and_cdf(self, object_instance):
         """Test that the ppf is the inverse of the cdf."""
         d = object_instance
         capabilities_exact = d.get_tags()["capabilities:exact"]
 
         if "ppf" not in capabilities_exact or "cdf" not in capabilities_exact:
             return
         x = d.sample()
         x_approx = d.ppf(d.cdf(x))
-        assert np.allclose(x.values, x_approx.values)
+        if d.ndim > 0:
+            assert np.allclose(x.values, x_approx.values)
+        else:
+            assert np.allclose(x, x_approx)
 
 
 def _check_output_format(res, dist, method):
     """Check output format expectations for BaseDistribution tests."""
+    if dist.shape == ():  # scalar distribution case
+        # check if numpy float
+        assert np.isscalar(res)
+        assert np.isreal(res)
+        if method in METHODS_SCALAR_POS or method in METHODS_X_POS:
+            assert res >= 0
+        return None
+
+    # array distribution case
     if method in METHODS_ROWWISE:
         exp_shape = (dist.shape[0], 1)
     else:
         exp_shape = dist.shape
     assert res.shape == exp_shape
     assert (res.index == dist.index).all()
     if method not in METHODS_ROWWISE:
@@ -250,9 +304,13 @@
         assert pd.api.types.is_numeric_dtype(res)
     else:
         raise TypeError("res must be a pandas DataFrame or Series.")
 
 
 def _shuffle_distr(d):
     """Shuffle distribution row index."""
-    shuffled_index = pd.DataFrame(d.index).sample(frac=1).index
+    if d.shape == ():  # nothing to shuffle if scalar
+        return d
+    # shuffle rows otherwise
+    shuffled_df = pd.DataFrame(d.index).sample(frac=1)
+    shuffled_index = pd.Index(shuffled_df.values.flatten())
     return d.loc[shuffled_index]
```

### Comparing `skpro-2.2.2/skpro/distributions/tests/test_base_default_methods.py` & `skpro-2.3.0/skpro/distributions/tests/test_base_default_methods.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,48 +13,91 @@
 __author__ = ["fkiraly"]
 
 import numpy as np
 import pandas as pd
 from scipy.special import erfinv
 
 from skpro.distributions.base import BaseDistribution
+from skpro.utils.estimator_checks import check_estimator
 
 
 # normal distribution with exact implementations removed
 class _DistrDefaultMethodTester(BaseDistribution):
     """Tester distribution for default methods."""
 
     _tags = {
         "capabilities:approx": ["pdfnorm", "mean", "var", "energy", "log_pdf", "cdf"],
         "capabilities:exact": ["pdf", "ppf"],
         "distr:measuretype": "continuous",
+        "broadcast_init": "on",
     }
 
     def __init__(self, mu, sigma, index=None, columns=None):
         self.mu = mu
         self.sigma = sigma
-        self.index = index
-        self.columns = columns
-
-        self._mu, self._sigma = self._get_bc_params(self.mu, self.sigma)
-        shape = self._mu.shape
-
-        if index is None:
-            index = pd.RangeIndex(shape[0])
-
-        if columns is None:
-            columns = pd.RangeIndex(shape[1])
 
         super().__init__(index=index, columns=columns)
 
-    def ppf(self, p):
-        """Quantile function = percent point function = inverse cdf."""
-        d = self.loc[p.index, p.columns]
-        icdf_arr = d.mu + d.sigma * np.sqrt(2) * erfinv(2 * p.values - 1)
-        return pd.DataFrame(icdf_arr, index=p.index, columns=p.columns)
-
-    def pdf(self, x):
-        """Probability density function."""
-        d = self.loc[x.index, x.columns]
-        pdf_arr = np.exp(-0.5 * ((x.values - d.mu) / d.sigma) ** 2)
-        pdf_arr = pdf_arr / (d.sigma * np.sqrt(2 * np.pi))
-        return pd.DataFrame(pdf_arr, index=x.index, columns=x.columns)
+    def _ppf(self, p):
+        """Quantile function = percent point function = inverse cdf.
+
+        Parameters
+        ----------
+        p : 2D np.ndarray, same shape as ``self``
+            values to evaluate the ppf at
+
+        Returns
+        -------
+        2D np.ndarray, same shape as ``self``
+            ppf values at the given points
+        """
+        mu = self._bc_params["mu"]
+        sigma = self._bc_params["sigma"]
+
+        icdf_arr = mu + sigma * np.sqrt(2) * erfinv(2 * p - 1)
+        return icdf_arr
+
+    def _pdf(self, x):
+        """Probability density function.
+
+        Parameters
+        ----------
+        x : 2D np.ndarray, same shape as ``self``
+            values to evaluate the pdf at
+
+        Returns
+        -------
+        2D np.ndarray, same shape as ``self``
+            pdf values at the given points
+        """
+        mu = self._bc_params["mu"]
+        sigma = self._bc_params["sigma"]
+
+        pdf_arr = np.exp(-0.5 * ((x - mu) / sigma) ** 2)
+        pdf_arr = pdf_arr / (sigma * np.sqrt(2 * np.pi))
+        return pdf_arr
+
+    @classmethod
+    def get_test_params(cls, parameter_set="default"):
+        """Return testing parameter settings for the estimator."""
+        # array case examples
+        params1 = {"mu": [[0, 1], [2, 3], [4, 5]], "sigma": 1}
+        params2 = {
+            "mu": 0,
+            "sigma": 1,
+            "index": pd.Index([1, 2, 5]),
+            "columns": pd.Index(["a", "b"]),
+        }
+        # scalar case examples
+        params3 = {"mu": 1, "sigma": 2}
+        return [params1, params2, params3]
+
+
+def test_base_default():
+    """Test default methods.
+
+    The _DistributionDefaultMethodTester class is not detected
+    by TestAllDistributions (it is private), so we need to test it explicitly.
+
+    check_estimator invokes a TestAllDistributions call.
+    """
+    check_estimator(_DistrDefaultMethodTester, raise_exceptions=True)
```

### Comparing `skpro-2.2.2/skpro/distributions/tests/test_qpd.py` & `skpro-2.3.0/skpro/distributions/tests/test_qpd.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,56 @@
 """Tests for quantile-parameterized distributions."""
 
+import numpy as np
 import pytest
 
 from skpro.distributions.qpd import QPD_B, QPD_S, QPD_U
 from skpro.tests.test_switch import run_test_for_class
 
 
 @pytest.mark.skipif(
     not run_test_for_class(QPD_B),
-    reason="run test only if softdeps are present and incrementally (if requested)",
+    reason="run test only if softdeps are present and incrementally (if requested)",  #
 )
 def test_qpd_b_simple_use():
     """Test simple use of qpd with bounded mode."""
-    from skpro.distributions.qpd import QPD_B
-
     qpd = QPD_B(
         alpha=0.2,
         qv_low=[1, 2],
         qv_median=[3, 4],
         qv_high=[5, 6],
         lower=0,
         upper=10,
     )
 
     qpd.mean()
 
 
+def test_qpd_b_pdf():
+    """Test pdf of qpd with bounded mode."""
+    # these parameters should produce a uniform on -0.5, 0.5
+    qpd_linear = QPD_B(
+        alpha=0.2,
+        qv_low=-0.3,
+        qv_median=0,
+        qv_high=0.3,
+        lower=-0.5,
+        upper=0.5,
+    )
+    x = np.linspace(-0.45, 0.45, 100)
+    pdf_vals = [qpd_linear.pdf(x_) for x_ in x]
+    np.testing.assert_allclose(pdf_vals, 1.0, rtol=1e-5)
+
+
 @pytest.mark.skipif(
     not run_test_for_class(QPD_S),
     reason="run test only if softdeps are present and incrementally (if requested)",
 )
 def test_qpd_s_simple_use():
     """Test simple use of qpd with semi-bounded mode."""
-    from skpro.distributions.qpd import QPD_S
-
     qpd = QPD_S(
         alpha=0.2,
         qv_low=[1, 2],
         qv_median=[3, 4],
         qv_high=[5, 6],
         lower=0,
     )
@@ -46,17 +59,15 @@
 
 
 @pytest.mark.skipif(
     not run_test_for_class(QPD_U),
     reason="run test only if softdeps are present and incrementally (if requested)",
 )
 def test_qpd_u_simple_use():
-    """Test simple use of qpd with unbounded mode."""
-    from skpro.distributions.qpd import QPD_U
-
+    """Test simple use of qpd with un-bounded mode."""
     qpd = QPD_U(
         alpha=0.2,
         qv_low=[1, 2],
         qv_median=[3, 4],
         qv_high=[5, 6],
     )
```

### Comparing `skpro-2.2.2/skpro/metrics/__init__.py` & `skpro-2.3.0/skpro/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/metrics/_classes.py` & `skpro-2.3.0/skpro/metrics/_classes.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/metrics/_coerce.py` & `skpro-2.3.0/skpro/metrics/_coerce.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/metrics/base.py` & `skpro-2.3.0/skpro/metrics/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -56,23 +56,24 @@
         y_pred : return object of probabilistic predictition method scitype:y_pred
             must have same index and columns as y_true
             Predicted values, i-th row is prediction for i-th row of ``y_true``.
 
         Returns
         -------
         loss : float or 1-column pd.DataFrame with calculated metric value(s)
-            metric is always averaged (arithmetic) over fh values
-            if multioutput = "raw_values",
-                will have a column level corresponding to variables in y_true
-            if multioutput = multioutput = "uniform_average" or or array-like
-                entries will be averaged over output variable column
-            if score_average = False,
-                will have column levels corresponding to quantiles/intervals
-            if score_average = True,
-                entries will be averaged over quantiles/interval column
+            metric is always averaged (arithmetic) over instances
+
+            * if ``multioutput = "raw_values"``,
+              will have a column level corresponding to variables in ``y_true``
+            * if ``multioutput = multioutput = "uniform_average"`` or or array-like
+              entries will be averaged over output variable column
+            * if ``score_average = False``,
+              will have column levels corresponding to quantiles/intervals
+            * if ``score_average = True``,
+              entries will be averaged over quantiles/interval column
         """
         return self.evaluate(y_true, y_pred, **kwargs)
 
     def evaluate(self, y_true, y_pred, **kwargs):
         """Evaluate the metric on given inputs.
 
         Parameters
@@ -83,23 +84,24 @@
         y_pred : return object of probabilistic predictition method scitype:y_pred
             must have same index and columns as y_true
             Predicted values, i-th row is prediction for i-th row of ``y_true``.
 
         Returns
         -------
         loss : float or 1-column pd.DataFrame with calculated metric value(s)
-            metric is always averaged (arithmetic) over fh values
-            if multioutput = "raw_values",
-                will have a column level corresponding to variables in y_true
-            if multioutput = multioutput = "uniform_average" or or array-like
-                entries will be averaged over output variable column
-            if score_average = False,
-                will have column levels corresponding to quantiles/intervals
-            if score_average = True,
-                entries will be averaged over quantiles/interval column
+            metric is always averaged (arithmetic) over instances
+
+            * if ``multioutput = "raw_values"``,
+              will have a column level corresponding to variables in ``y_true``
+            * if ``multioutput = multioutput = "uniform_average"`` or or array-like
+              entries will be averaged over output variable column
+            * if ``score_average = False``,
+              will have column levels corresponding to quantiles/intervals
+            * if ``score_average = True``,
+              entries will be averaged over quantiles/interval column
         """
         # Input checks and conversions
         y_true_inner, y_pred_inner, multioutput = self._check_ys(
             y_true, y_pred, self.multioutput
         )
 
         # Don't want to include scores for 0 width intervals, makes no sense
@@ -168,24 +170,27 @@
 
         y_pred : return object of probabilistic predictition method scitype:y_pred
             must have same index and columns as y_true
             Predicted values, i-th row is prediction for i-th row of ``y_true``.
 
         Returns
         -------
-        loss : pd.DataFrame of length len(fh), with calculated metric value(s)
+        loss : pd.DataFrame of same length as ``y_true``,
+            calculated metric value(s).
+
             i-th column contains metric value(s) for prediction at i-th fh element
-            if multioutput = "raw_values",
-                will have a column level corresponding to variables in y_true
-            if multioutput = multioutput = "uniform_average" or or array-like
-                entries will be averaged over output variable column
-            if score_average = False,
-                will have column levels corresponding to quantiles/intervals
-            if score_average = True,
-                entries will be averaged over quantiles/interval column
+
+            * if multioutput = "raw_values",
+              will have a column level corresponding to variables in y_true
+            * if multioutput = multioutput = "uniform_average" or or array-like
+              entries will be averaged over output variable column
+            * if score_average = False,
+              will have column levels corresponding to quantiles/intervals
+            * if score_average = True,
+              entries will be averaged over quantiles/interval column
         """
         # Input checks and conversions
         y_true_inner, y_pred_inner, multioutput = self._check_ys(
             y_true, y_pred, self.multioutput
         )
 
         # Don't want to include scores for 0 width intervals, makes no sense
@@ -220,15 +225,15 @@
 
         Parameters
         ----------
         y_true : pd.Series, pd.DataFrame, 1D np.array, or 2D np.ndarray
             Ground truth (correct) target values.
 
         y_pred : return object of probabilistic predictition method scitype:y_pred
-            must have same index and columns as y_true
+            must have same index and columns as ``y_true``.
             Predicted values, i-th row is prediction for i-th row of ``y_true``.
         """
         n = y_true.shape[0]
         out_series = pd.Series(index=y_pred.index)
         try:
             x_bar = self.evaluate(y_true, y_pred, self.multioutput, **kwargs)
             for i in range(n):
@@ -334,15 +339,15 @@
 
         if not all((alpha > 0) & (alpha < 1)):
             raise ValueError("Alpha must be between 0 and 1.")
 
         return alpha
 
     def _handle_multioutput(self, loss, multioutput):
-        """Specificies how multivariate outputs should be handled.
+        """Handle output according to multioutput parameter.
 
         Parameters
         ----------
         loss : float, np.ndarray the evaluated metric value.
 
         multioutput : string "uniform_average" or "raw_values" determines how \
             multioutput results will be treated.
@@ -392,15 +397,17 @@
         y_pred : return object of probabilistic predictition method scitype:y_pred
             must have same index and columns as y_true
             Predicted values, i-th row is prediction for i-th row of ``y_true``.
 
         Returns
         -------
         loss : float or 1-column pd.DataFrame with calculated metric value(s)
+
             float if multioutput = "uniform_average" or multivariate = True
+
             1-column df if multioutput = "raw_values" and metric is not multivariate
             metric is always averaged (arithmetic) over rows
         """
         multioutput = self.multioutput
         multivariate = self.multivariate
 
         index_df = self.evaluate_by_index(y_true, y_pred, **kwargs)
@@ -424,29 +431,46 @@
             Object to coerce
 
         Returns
         -------
         obj : object
             Coerced object
         """
+        if obj is None:
+            return None
         obj = convert_to(obj, to_type="pd_DataFrame_Table", as_scitype="Table")
         obj = _coerce_to_df(obj)
         return obj
 
     def evaluate_by_index(self, y_true, y_pred, **kwargs):
         """Evaluate the metric by instance index (row).
 
         Parameters
         ----------
         y_true : pd.Series, pd.DataFrame, 1D np.array, or 2D np.ndarray
             Ground truth (correct) target values.
 
         y_pred : skpro BaseDistribution of same shape as y_true
             Predictive distribution.
-            Must have same index and columns as y_true.
+            Must have same index and columns as ``y_true``.
+
+        Returns
+        -------
+        loss : ``pd.Series`` or ``pd.DataFrame``
+            Calculated metric, by time point (default=jackknife pseudo-values).
+
+            ``pd.Series`` if ``self.multioutput="uniform_average"`` or array-like
+
+            * index is equal to index of ``y_true``
+            * entry at index i is metric at time i, averaged over variables
+
+            ``pd.DataFrame`` if ``self.multioutput="raw_values"``
+
+            * index and columns equal to those of ``y_true``
+            * i,j-th entry is metric at time i, at variable j
         """
         multioutput = self.multioutput
 
         if hasattr(self, "multivariate"):
             multivariate = self.multivariate
         else:
             multivariate = False
@@ -478,7 +502,81 @@
                     **kwargs_inner,
                 )
                 res_for_col.columns = [col]
                 res_by_col += [res_for_col]
             res = pd.concat(res_by_col, axis=1)
 
         return res
+
+
+class BaseSurvDistrMetric(BaseDistrMetric):
+    """Intermediate base class for distributional prediction metrics/scores.
+
+    Developer note:
+    Same as BaseSurvDistrMetric, except for tag set and docstring overrides.
+    """
+
+    _tags = {"capability:survival": True}
+
+    def evaluate(self, y_true, y_pred, **kwargs):
+        """Evaluate the  metric on given inputs.
+
+        Parameters
+        ----------
+        y_true : pd.Series, pd.DataFrame, 1D np.array, or 2D np.ndarray
+            Ground truth (correct) target values.
+
+        y_pred : return object of probabilistic predictition method scitype:y_pred
+            must have same index and columns as y_true
+            Predicted values, i-th row is prediction for i-th row of ``y_true``.
+
+        C_true : pd.Series, pd.DataFrame, np.ndarray, optional (default=None)
+            censoring information for survival analysis,
+            should have same column name as y, same length as X and y
+            should have entries 0 and 1 (float or int)
+            0 = uncensored, 1 = (right) censored
+            if None, all observations are assumed to be uncensored
+
+        Returns
+        -------
+        loss : float or 1-column pd.DataFrame with calculated metric value(s)
+            float if multioutput = "uniform_average" or multivariate = True
+            1-column df if multioutput = "raw_values" and metric is not multivariate
+            metric is always averaged (arithmetic) over rows
+        """
+        return super().evaluate(y_true=y_true, y_pred=y_pred, **kwargs)
+
+    def evaluate_by_index(self, y_true, y_pred, **kwargs):
+        """Evaluate the metric by instance index (row).
+
+        Parameters
+        ----------
+        y_true : pd.Series, pd.DataFrame, 1D np.array, or 2D np.ndarray
+            Ground truth (correct) target values.
+
+        y_pred : skpro BaseDistribution of same shape as y_true
+            Predictive distribution.
+            Must have same index and columns as y_true.
+
+        C_true : pd.Series, pd.DataFrame, np.ndarray, optional (default=None)
+            censoring information for survival analysis,
+            should have same column name as y, same length as X and y
+            should have entries 0 and 1 (float or int)
+            0 = uncensored, 1 = (right) censored
+            if None, all observations are assumed to be uncensored
+
+        Returns
+        -------
+        loss : ``pd.Series`` or ``pd.DataFrame``
+            Calculated metric, by time point (default=jackknife pseudo-values).
+
+            ``pd.Series`` if ``self.multioutput="uniform_average"`` or array-like
+
+            * index is equal to index of ``y_true``
+            * entry at index i is metric at time i, averaged over variables
+
+            ``pd.DataFrame`` if ``self.multioutput="raw_values"``
+
+            * index and columns equal to those of ``y_true``
+            * i,j-th entry is metric at time i, at variable j
+        """
+        return super().evaluate_by_index(y_true=y_true, y_pred=y_pred, **kwargs)
```

### Comparing `skpro-2.2.2/skpro/metrics/survival/_c_harrell.py` & `skpro-2.3.0/skpro/metrics/survival/_c_harrell.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Concordance index, Harrell's."""
 # copyright: skpro developers, BSD-3-Clause License (see LICENSE file)
 
 import numpy as np
 import pandas as pd
 
-from skpro.metrics.base import BaseDistrMetric
+from skpro.metrics.base import BaseSurvDistrMetric
 
 
-class ConcordanceHarrell(BaseDistrMetric):
+class ConcordanceHarrell(BaseSurvDistrMetric):
     r"""Concordance index (Harrell).
 
     Fraction of concordant test index pairs among all comparale pairs,
     as proposed in [1]_, commonly known as Harrell's C-index, Harrell's C,
     or simply concordance index,
     if not in delination of other C-indices (e.g., Uno's C-index).
 
@@ -163,15 +163,16 @@
             nCj = ~Cj
             rj = risk_scores[:, j]
             for i in range(y_true.shape[0]):
                 yij = yj[i]
                 rij = rj[i]
                 Cij = Cj[i]
                 nCij = ~Cij
-                one_unc = ~(Cj & Cij)
+                one_unc = ~(Cj & Cij)  # at least one uncensored in the pair
+                xone_unc = ~(Cj & Cij) & (Cj | Cij)  # exactly one uncensored
 
                 # mark concordant pairs (no ties)
                 comp1 = nCij & (yj > yij)  # comparable, > type
                 conc1 = comp1 & (rj > rij)
                 comp2 = nCj & (yj < yij)  # comparable, < type
                 conc2 = comp2 & (rj < rij)
 
@@ -183,15 +184,15 @@
                 nconc = conc.sum() - nCij  # sum, subtract i=j if counted above
                 # i=j was counted iff it was not censored
 
                 # handle ties in total of concordant pairs
                 if tie_score != 0:
                     nconc = nconc.astype(float)
                     nconc += np.sum((yj != yij) & (rj == rij)) * tie_score
-                    nconc += np.sum(one_unc & (yj == yij) & (rj == rij)) * tie_score
+                    nconc += np.sum(xone_unc & (yj == yij) & (rj == rij)) * tie_score
 
                 # count comparable pairs
                 comp3 = one_unc & (yj == yij)
                 comp = comp1 | comp2 | comp3
                 ncomp = comp.sum() - nCij  # subtract i=j, but only if counted above
 
                 nconc_mat[i, j] = nconc
@@ -204,15 +205,17 @@
             ncomp_total = ncomp_mat.sum(axis=0)
             nspl = len(ncomp_mat)
             result = (nspl / ncomp_total) * nconc_mat
         else:  # normalization == "index"
             # weighting is such that rows contain simple fractions
             # but the average over rows is not the overall C-index,
             # as number of comparable pairs is in general not the same for each index
+            ncomp_mat[ncomp_mat == 0] = 1  # handling of case 0 / 0, avoid nans
             result = nconc_mat / ncomp_mat
+            result[ncomp_mat == 1] = tie_score  # handling of case 0 / 0
 
         res_df = pd.DataFrame(result, index=ix, columns=cols)
 
         if self.multivariate:
             return pd.DataFrame(res_df.mean(axis=1), columns=["C_Harrell"])
         else:
             return res_df
```

### Comparing `skpro-2.2.2/skpro/metrics/survival/_spll.py` & `skpro-2.3.0/skpro/metrics/survival/_spll.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Survival Process Logarithmic Loss for distributional predictions."""
 # copyright: skpro developers, BSD-3-Clause License (see LICENSE file)
 
 import numpy as np
 import pandas as pd
 
-from skpro.metrics.base import BaseDistrMetric
+from skpro.metrics.base import BaseSurvDistrMetric
 
 
-class SPLL(BaseDistrMetric):
+class SPLL(BaseSurvDistrMetric):
     r"""Survival Process Logarithmic Loss for distributional predictions.
 
     Same as the negative log-likelihood of the survival process (see [1]_),
     and therefore a proper scoring rule for survival predictions.
 
     For a predictive distribution :math:`d` with pdf :math:`d.p`,
     survival function :math:`d.S`, a ground truth value :math:`y`
```

### Comparing `skpro-2.2.2/skpro/metrics/survival/tests/test_c_harrell.py` & `skpro-2.3.0/skpro/metrics/survival/tests/test_c_harrell.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 # copyright: skpro developers, BSD-3-Clause License (see LICENSE file)
 
 import pandas as pd
 import pytest
 
 
 @pytest.mark.parametrize("concordant", [True, False])
-@pytest.mark.parametrize("pass_c", [True, False])
+@pytest.mark.parametrize("pass_c", ["True", "False", "None"])
 @pytest.mark.parametrize("normalization", ["overall", "index"])
 def test_charrell_logic(concordant, pass_c, normalization):
     """Test the logic of the Harrell's C-index metric.
 
     Parameters
     ----------
     concordant : bool, optional, default=True
         If True, the test examples are fully concordant.
         If False, the test examples are fully discordant.
     pass_c : bool, optional, default=True
-        If True, the `c_true` argument is passed to the metric.
-        If False, the `c_true` argument is not passed to the metric.
+        If True, the ``C_true`` argument is passed to the metric, with censoring data.
+        If None, the ``C_true`` argument is passed to the metric, with value None.
+        If False, the ``C_true`` argument is not passed to the metric.
     normalization : str, optional, default="overall"
         The normalization method for the metric.
     """
     from skpro.distributions import Normal
     from skpro.metrics.survival._c_harrell import ConcordanceHarrell
 
     # examples are constructed to be fully concordant or discordant,
@@ -32,21 +33,26 @@
     y_pred_mean = pd.DataFrame({"a": [2, 3, 4, 5], "b": [6, 5, 4, 3]})
 
     if not concordant:
         y_pred_mean = -y_pred_mean
     y_pred = Normal(y_pred_mean, sigma=1, columns=pd.Index(["a", "b"]))
 
     # evaluate the metric
-    metric = ConcordanceHarrell(normalization=normalization)
+    metric = ConcordanceHarrell(normalization=normalization, tie_score=int(concordant))
     metric_args = {"y_true": y_true, "y_pred": y_pred}
-    if pass_c:
-        metric_args["c_true"] = c_true
+    if pass_c == "True":
+        metric_args["C_true"] = c_true
+    elif pass_c == "None":
+        metric_args["C_true"] = c_true
 
     res = metric(**metric_args)
     res_by_index = metric.evaluate_by_index(**metric_args)
 
+    assert res_by_index.shape == y_true.shape
+
     # test assumptions
     # if concordant, the result should be 1
     # if discordant, the result should be 0
     assert res == concordant
-    assert res_by_index.shape == y_true.shape
-    assert (res_by_index == concordant).all().all()
+
+    if normalization == "index":
+        assert (res_by_index == concordant).all().all()
```

### Comparing `skpro-2.2.2/skpro/metrics/tests/test_distr_metrics.py` & `skpro-2.3.0/skpro/metrics/tests/test_distr_metrics.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/metrics/tests/test_probabilistic_metrics.py` & `skpro-2.3.0/skpro/metrics/tests/test_probabilistic_metrics.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/model_selection/_tuning.py` & `skpro-2.3.0/skpro/model_selection/_tuning.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/registry/_lookup.py` & `skpro-2.3.0/skpro/registry/_lookup.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/registry/_scitype.py` & `skpro-2.3.0/skpro/registry/_scitype.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/registry/_tags.py` & `skpro-2.3.0/skpro/registry/_tags.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,14 +158,20 @@
     (
         "distr:measuretype",
         "distribution",
         ("str", ["continuous", "discrete", "mixed"]),
         "measure type of distr",
     ),
     (
+        "distr:paramtype",
+        "distribution",
+        ("str", ["general", "parametric", "nonparametric", "composite"]),
+        "parametrization type of distribution",
+    ),
+    (
         "approx_mean_spl",
         "distribution",
         "int",
         "sample size used in MC estimates of mean",
     ),
     (
         "approx_var_spl",
@@ -187,14 +193,32 @@
     ),
     (
         "bisect_iter",
         "distribution",
         "int",
         "max iters for bisection method in ppf",
     ),
+    (
+        "broadcast_params",
+        "distribution",
+        ("list", "str"),
+        "distribution parameters to broadcast, complement is not broadcast",
+    ),
+    (
+        "broadcast_init",
+        "distribution",
+        ("str", ["on", "off"]),
+        "whether to initialize broadcast parameters in __init__, 'on' or 'off'",
+    ),
+    (
+        "broadcast_inner",
+        "distribution",
+        ("str", ["array", "scalar"]),
+        "if inner logic is vectorized ('array') or scalar ('scalar')",
+    ),
     # ---------------
     # BaseProbaMetric
     # ---------------
     (
         "scitype:y_pred",
         "metric",
         "str",
```

### Comparing `skpro-2.2.2/skpro/registry/tests/test_scitype.py` & `skpro-2.3.0/skpro/registry/tests/test_scitype.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/registry/tests/test_tags.py` & `skpro-2.3.0/skpro/registry/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/regression/adapters/sklearn/_sklearn_proba.py` & `skpro-2.3.0/skpro/regression/adapters/sklearn/_sklearn_proba.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/regression/base/_base.py` & `skpro-2.3.0/skpro/regression/base/_base.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/regression/base/_delegate.py` & `skpro-2.3.0/skpro/regression/base/_delegate.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/regression/base/adapters/_sklearn.py` & `skpro-2.3.0/skpro/regression/base/adapters/_sklearn.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/regression/baselines/density.py` & `skpro-2.3.0/skpro/regression/baselines/density.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/regression/bootstrap.py` & `skpro-2.3.0/skpro/regression/bootstrap.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/regression/compose/_pipeline.py` & `skpro-2.3.0/skpro/regression/compose/_pipeline.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/regression/cyclic_boosting.py` & `skpro-2.3.0/skpro/regression/cyclic_boosting.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,35 +2,50 @@
 
 This is a interface for Cyclic boosting, it contains efficient,
 off-the-shelf, general-purpose supervised machine learning methods
 for both regression and classification tasks.
 Please read the official document for its detail
 https://cyclic-boosting.readthedocs.io/en/latest/
 """
+
 # copyright: skpro developers, BSD-3-Clause License (see LICENSE file)
 
 __author__ = [
     "setoguchi-naoki"
 ]  # interface only. Cyclic boosting authors in cyclic_boosting package
 
 import warnings
+from typing import Union
 
 import numpy as np
 import pandas as pd
 
-from skpro.distributions.qpd import QPD_B, QPD_S, QPD_U
+from skpro.distributions.qpd import QPD_Johnson
 from skpro.regression.base import BaseProbaRegressor
 
 
 class CyclicBoosting(BaseProbaRegressor):
-    """Cyclic boosting regressor.
+    """Cyclic boosting regressor from ``cyclic-boosting`` library.
+
+    Direct interface to ``pipeline_CBAdditiveQuantileRegressor``
+    and ``pipeline_CBMultiplicativeQuantileRegressor`` from ``cyclic-boosting``.
+
+    The algorithms use boosting to create conditional distribution predictions
+    that are Johnson Quantile-Parameterized Distributions (JQPD),
+    with parameters estimated by quantile regression at quantile nodes.
 
-    Estimates the parameters of Johnson Quantile-Parameterized Distributions
-    (JQPD) by quantile regression, which is one of the Cyclic boosting's functions
-    this method can more accurately approximate to the distribution of observed data
+    The quantile nodes are ``[alpha, 0.5, 1-alpha]``, where ``alpha``
+    is a parameter of the model.
+
+    The cyclic boosting model performs boosted quantile regression for the quantiles
+    at the nodes, and then substitutes the quantile predictions into the paramtric
+    form of the Johnson QPD.
+
+    The model allows to select unbounded, left semi-bounded, and bounded
+    predictive distribution support.
 
     Parameters
     ----------
     feature_groups : list, default=None
         Explanatory variables and interaction terms in the model,
         For each feature or feature tuple in the sequence, a
         one- or multidimensional factor profile will be determined,
@@ -40,27 +55,46 @@
     feature_properties : dict, default=None
         name and characteristic of train dataset by `flags` from cyclic boosting library
         it is able to set multiple characteristic by OR operator
         e.g. {sample1: flags.IS_CONTINUOUS | flags.IS_LINEAR, sample2: flags.IS_ORDERED}
         for basic options, see https://cyclic-boosting.readthedocs.io/en/latest/\
         tutorial.html#set-feature-properties
     alpha : float, default=0.2
-        lower quantile for QPD's parameter alpha
+        lower quantile QPD parameter.
+        The three quantile nodes are uniquely determined by this parameter,
+        as ``[alpha, 0.5, 1-alpha]``.
     mode : str, default='multiplicative'
         the type of quantile regressor. 'multiplicative' or 'additive'
-    bound : str, default='U'
-        Different modes defined by supported target range, options are ``S``
-            (semi-bound), ``B`` (bound), and ``U`` (unbound).
-    lower : float, default=0.0
-        lower bound of supported range (only active for bound and semi-bound
-        modes)
-    upper : float, default=1.0
-        upper bound of supported range (only active for bound mode)
+    bound : str, default='U', one of ``'S'``, ``'B'``, ``'U'``
+        Mode for the predictive distribution support, options are ``S``
+        (semi-bounded), ``B`` (bounded), and ``U`` (unbounded).
+    lower : float, default=None
+        lower bound of predictive distribution support.
+        If ``None`` (default), ``upper`` should also be ``None``, and the
+        predictive distribution will have unbounded support, i.e., the entire reals.
+        If a float, and ``upper`` is ``None``, prediction will be of
+        semi-bounded support, with support between ``lower`` and infinity.
+        If a float, and ``upper`` is also a float, prediction will be on a bounded
+        interval, with support between ``lower`` and ``upper``.
+    upper : float, default=None
+        upper bound of predictive distribution support.
+        If ``None`` (default), will use semi-bounded mode if ``lower`` is a float,
+        and unbounded if ``lower`` is ``None``.
+        If a float, assumes that ``lower`` is also a float, and prediction will
+        be on a bounded interval, with support between ``lower`` and ``upper``.
     maximal_iterations : int, default=10
-        number of iterations
+        maximum number of iterations for the cyclic boosting algorithm
+    dist_type: str, one of ``'normal'`` (default), ``'logistic'``
+        inner base distribution to use for the Johnson QPD, i.e., before
+        arcosh and similar transformations.
+        Available options are ``'normal'`` (default), ``'logistic'``,
+        or ``'sinhlogistic'``.
+    dist_shape: float, optional, default=0.0
+        parameter modifying the logistic base distribution via
+        sinh/arcsinh-scaling - only relevant for ``dist_type='sinhlogistic'``
 
     Attributes
     ----------
     estimators_ : list of skpro regressors
         clones of regressor in `estimator` fitted in the ensemble
     quantiles : list, default=[0.2, 0.5, 0.8]
         targets of quantile prediction for j-qpd's param
@@ -68,15 +102,15 @@
         quantile prediction results
     quantile_est: list
         estimators, each estimator predicts point in the value of quantiles attribute
     qpd: skpro.distributions.J_QPD_S
         Johnson Quantile-Parameterized Distributions instance
 
     Example
-    --------
+    -------
     >>> from skpro.regression.cyclic_boosting import CyclicBoosting
     >>> from sklearn.datasets import load_diabetes  # doctest: +SKIP
     >>> from sklearn.model_selection import train_test_split  # doctest: +SKIP
     >>> X, y = load_diabetes(return_X_y=True, as_frame=True)  # doctest: +SKIP
     >>> X_train, X_test, y_train, y_test = train_test_split(X, y)  # doctest: +SKIP
 
     >>> reg_proba = CyclicBoosting()  # doctest: +SKIP
@@ -86,49 +120,84 @@
 
     _tags = {
         # packaging info
         # --------------
         "authors": ["setoguchi-naoki", "felix-wick"],
         "maintainers": ["setoguchi-naoki"],
         "estimator_type": "regressor_proba",
-        "python_dependencies": "cyclic_boosting>=1.2.5",
+        "python_dependencies": "cyclic_boosting>=1.4.0",
         # estimator tags
         # --------------
         "capability:multioutput": False,
         "capability:missing": True,
         "X_inner_mtype": "pd_DataFrame_Table",
         "y_inner_mtype": "pd_DataFrame_Table",
     }
 
     def __init__(
         self,
         feature_groups=None,
         feature_properties=None,
         alpha=0.2,
         mode="multiplicative",
-        bound="U",
-        lower=0.0,
-        upper=1.0,
+        bound="deprecated",
+        lower=None,
+        upper=None,
         maximal_iterations=10,
+        dist_type: Union[str, None] = "normal",
+        dist_shape: Union[float, None] = 0.0,
     ):
         self.feature_groups = feature_groups
         self.feature_properties = feature_properties
         self.alpha = alpha
-        self.quantiles = [self.alpha, 0.5, 1 - self.alpha]
-        self.quantile_values = list()
-        self.quantile_est = list()
-        self.qpd = None
         self.mode = mode
         self.bound = bound
         self.lower = lower
         self.upper = upper
         self.maximal_iterations = maximal_iterations
+        self.dist_type = dist_type
+        self.dist_shape = dist_shape
 
         super().__init__()
 
+        self.quantiles = [self.alpha, 0.5, 1 - self.alpha]
+        self.quantile_values = list()
+        self.quantile_est = list()
+        self.qpd = None
+
+        # todo 2.4.0: remove bound parameter and this deprecation warning
+        if bound == "deprecated":
+            warnings.warn(
+                "In CyclicBoosting, the 'bound' parameter is deprecated, "
+                "and will be removed in skpro version 2.4.0. "
+                "To retain the current behavior, and silence this warning, "
+                "do not set the 'bound' parameter "
+                "and set 'lower' and 'upper' parameters instead, "
+                "as follows: for unbounded mode, previously bound='U', "
+                "set 'lower' and 'upper' to None; "
+                "for semi-bounded mode, previously bound='S', "
+                "set 'lower' to lower bound and 'upper' to None; "
+                "for bounded mode, previously bound='B', "
+                "set 'lower' to lower bound and 'upper' to upper bound.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+
+        # todo 2.4.0: remove this block
+        # translate bound to lower and upper
+        if lower is None and bound in ["S", "B"]:
+            self._lower = 0.0
+        else:
+            self._lower = None
+        if upper is None and bound == "B":
+            self._upper = 1.0
+        else:
+            self._upper = upper
+        # end block
+
         # check parameters
         if (not isinstance(feature_groups, list)) and feature_groups is not None:
             raise ValueError("feature_groups needs to be list")
         if (
             not isinstance(feature_properties, dict)
         ) and feature_properties is not None:
             raise ValueError("feature_properties needs to be dict")
@@ -269,34 +338,29 @@
 
         # predict quantiles
         self.quantile_values = list()
         for est in self.quantile_est:
             yhat = est.predict(X.copy())
             self.quantile_values.append(yhat)
 
+        # todo 2.4.0: replace self._lower and self._upper with self.lower and self.upper
         # Johnson Quantile-Parameterized Distributions
         params = {
             "alpha": self.alpha,
-            "qv_low": self.quantile_values[0],
-            "qv_median": self.quantile_values[1],
-            "qv_high": self.quantile_values[2],
+            "qv_low": self.quantile_values[0].reshape(-1, 1),
+            "qv_median": self.quantile_values[1].reshape(-1, 1),
+            "qv_high": self.quantile_values[2].reshape(-1, 1),
+            "lower": self.lower,
+            "upper": self.upper,
+            "version": self.dist_type,
+            "dist_shape": self.dist_shape,
             "index": index,
             "columns": y_cols,
         }
-        if self.bound == "U":
-            qpd = QPD_U(**params)
-        elif self.bound == "S":
-            params["lower"] = self.lower
-            qpd = QPD_S(**params)
-        elif self.bound == "B":
-            params["lower"] = self.lower
-            params["upper"] = self.upper
-            qpd = QPD_B(**params)
-        else:
-            raise ValueError("bound need to be 'U' or 'S' or 'B'")
+        qpd = QPD_Johnson(**params)
 
         return qpd
 
     def _predict_interval(self, X, coverage):
         """Compute/return interval predictions.
 
         private _predict_interval containing the core logic,
@@ -412,19 +476,16 @@
             [y_cols, quantiles],
         )
 
         # predict quantiles
         self.quantile_values = list()
         if is_given_proba:
             qpd = self.predict_proba(X.copy())
-            if isinstance(quantiles, list):
-                quantile = [quantiles]
-
-            p = pd.DataFrame(quantile, index=X.index, columns=columns)
-            quantiles = qpd.ppf(p)
+            pred = np.asarray([np.squeeze(qpd.ppf(q)) for q in quantiles]).T
+            quantiles = pd.DataFrame(pred, index=X.index, columns=columns)
 
         else:
             for est in self.quantile_est:
                 yhat = est.predict(X.copy())
                 self.quantile_values.append(yhat)
 
             quantiles = pd.DataFrame(
@@ -447,9 +508,21 @@
         -------
         params : dict or list of dict, default = {}
             Parameters to create testing instances of the class
             Each dict are parameters to construct an "interesting" test instance, i.e.,
             `MyClass(**params)` or `MyClass(**params[i])` creates a valid test instance.
             `create_test_instance` uses the first (or only) dictionary in `params`
         """
-        param1 = {"alpha": 0.3, "mode": "additive", "bound": "S", "lower": 0.0}
-        return [param1]
+        param1 = {
+            "alpha": 0.2,
+            "mode": "additive",
+            "lower": 0.0,
+            "maximal_iterations": 5,
+        }
+        param2 = {
+            "alpha": 0.2,
+            "mode": "additive",
+            "lower": 0.0,
+            "upper": 1000,
+            "maximal_iterations": 5,
+        }
+        return [param1, param2]
```

### Comparing `skpro-2.2.2/skpro/regression/density.py` & `skpro-2.3.0/skpro/regression/density.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         return ys[index]
 
     return func
 
 
 class DensityAdapter(BaseEstimator, metaclass=abc.ABCMeta):
     """
-    Abtract base class for density adapter
+    Abstract base class for density adapter
     that transform an input into an
     density cdf/pdf interface
     """
 
     @abc.abstractmethod
     def __call__(self, inlet):
         """
```

### Comparing `skpro-2.2.2/skpro/regression/ensemble.py` & `skpro-2.3.0/skpro/regression/ensemble/_bagging.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/regression/gp/_sklearn.py` & `skpro-2.3.0/skpro/regression/gp/_sklearn.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/regression/linear/_glm.py` & `skpro-2.3.0/skpro/regression/linear/_glm.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/regression/linear/_sklearn.py` & `skpro-2.3.0/skpro/regression/linear/_sklearn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Adapters to sklearnn linear regressors with probabilistic components."""
+"""Adapters to sklearn linear regressors with probabilistic components."""
 # copyright: skpro developers, BSD-3-Clause License (see LICENSE file)
 # based on sktime pipelines
 
 __author__ = ["fkiraly"]
 
 from skpro.regression.adapters.sklearn import SklearnProbaReg
 from skpro.regression.base.adapters import _DelegateWithFittedParamForwarding
```

### Comparing `skpro-2.2.2/skpro/regression/mapie.py` & `skpro-2.3.0/skpro/regression/mapie.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/regression/multiquantile.py` & `skpro-2.3.0/skpro/regression/multiquantile.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/regression/parametric/estimators.py` & `skpro-2.3.0/skpro/regression/parametric/estimators.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/regression/parametric/parametric.py` & `skpro-2.3.0/skpro/regression/parametric/parametric.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/regression/residual.py` & `skpro-2.3.0/skpro/regression/residual.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/regression/tests/test_all_regressors.py` & `skpro-2.3.0/skpro/regression/tests/test_all_regressors.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/regression/tests/test_cyclic_boosting.py` & `skpro-2.3.0/skpro/regression/tests/test_cyclic_boosting.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,72 +16,65 @@
     from sklearn.datasets import load_diabetes
     from sklearn.model_selection import train_test_split
 
     X, y = load_diabetes(return_X_y=True, as_frame=True)
     y = pd.DataFrame(y)
     X = X.iloc[:200]
     y = y.iloc[:200]
-    X_train, X_test, y_train, y_test = train_test_split(X, y)
+    X_train, X_test, y_train, y_test = train_test_split(X, y, random_state=0)
 
     reg_proba = CyclicBoosting()
     reg_proba.fit(X_train, y_train)
     y_pred = reg_proba.predict_proba(X_test)
 
     assert y_pred.shape == y_test.shape
 
 
 @pytest.mark.skipif(
     not run_test_for_class(CyclicBoosting),
     reason="run test only if softdeps are present and incrementally (if requested)",
 )
-def test_cyclic_boosting_with_manual_paramaters():
-    """Test use of cyclic boosting regressor with_manual_paramaters."""
+def test_cyclic_boosting_with_manual_parameters():
+    """Test use of cyclic boosting regressor with_manual_parameters."""
     from cyclic_boosting import flags
     from sklearn.datasets import load_diabetes
     from sklearn.model_selection import train_test_split
 
     X, y = load_diabetes(return_X_y=True, as_frame=True)
     y = pd.DataFrame(y)
     X = X.iloc[:200]
     y = y.iloc[:200]
-    X_train, X_test, y_train, y_test = train_test_split(X, y)
+    X_train, X_test, y_train, y_test = train_test_split(X, y, random_state=0)
 
     features = [
         "age",
         "sex",
         "bmi",
         "bp",
         "s1",
         "s2",
         "s3",
-        "s4",
-        "s5",
-        "s6",
         ("age", "sex"),
     ]
 
     fp = {
-        "age": flags.IS_CONTINUOUS,
-        "sex": flags.IS_CONTINUOUS,
+        "age": flags.IS_UNORDERED,
+        "sex": flags.IS_UNORDERED,
         "bmi": flags.IS_CONTINUOUS,
         "bp": flags.IS_CONTINUOUS,
         "s1": flags.IS_CONTINUOUS,
         "s2": flags.IS_CONTINUOUS,
         "s3": flags.IS_CONTINUOUS,
-        "s4": flags.IS_CONTINUOUS,
-        "s5": flags.IS_CONTINUOUS,
-        "s6": flags.IS_CONTINUOUS,
     }
 
     reg_proba = CyclicBoosting(
         feature_groups=features,
         feature_properties=fp,
         maximal_iterations=5,
         alpha=0.25,
         mode="additive",
-        bound="S",
         lower=0.0,
     )
     reg_proba.fit(X_train, y_train)
     y_pred = reg_proba.predict_proba(X_test)
 
     assert y_pred.shape == y_test.shape
```

### Comparing `skpro-2.2.2/skpro/regression/vendors/pymc.py` & `skpro-2.3.0/skpro/regression/vendors/pymc.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/survival/adapters/_common.py` & `skpro-2.3.0/skpro/survival/adapters/_common.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/survival/adapters/lifelines.py` & `skpro-2.3.0/skpro/survival/adapters/lifelines.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/survival/adapters/sksurv.py` & `skpro-2.3.0/skpro/survival/adapters/sksurv.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/survival/additive/_aalen_lifelines.py` & `skpro-2.3.0/skpro/survival/additive/_aalen_lifelines.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/survival/aft/_aft_lifelines_fisk.py` & `skpro-2.3.0/skpro/survival/aft/_aft_lifelines_fisk.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,21 +27,21 @@
     as being equal to the *median* lifetime. The
     :math:`\beta` parameter influences the shape of the hazard.
 
     Parameters
     ----------
     alpha_cols: pd.Index or coercible, optional, default=None
         Columns of the input data frame to be used as covariates for
-        the mean parameter :math:`\mu`.
+        the scale parameter :math:`\alpha`.
         If None, all columns are used.
 
     beta_cols: string "all", pd.Index or coercible, optional, default=None
         Columns of the input data frame to be used as covariates for
-        the standard deviation parameter :math:`\sigma`.
-        If None, no covariates are used, the standard deviation parameter
+        the shape parameter :math:`\beta`.
+        If None, no covariates are used, the shape parameter
         is estimated as a constant. If "all", all columns are used.
 
     fit_intercept: boolean, optional (default=True)
         Whether to fit an intercept term in the model.
 
     alpha: float, optional (default=0.05)
       the level in the confidence intervals around the estimated survival function,
```

### Comparing `skpro-2.2.2/skpro/survival/aft/_aft_lifelines_lognormal.py` & `skpro-2.3.0/skpro/survival/aft/_aft_lifelines_lognormal.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/survival/aft/_aft_lifelines_weibull.py` & `skpro-2.3.0/skpro/survival/aft/_aft_lifelines_weibull.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/survival/base.py` & `skpro-2.3.0/skpro/survival/base.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/survival/compose/_reduce_cond_unc.py` & `skpro-2.3.0/skpro/survival/compose/_reduce_cond_unc.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         X = X.copy()
         columns = self._y_cols
         index = X.index
 
         if C is None:
             C = pd.DataFrame(0, index=index, columns=columns)
         else:
-            C = C.copy()
+            C = C.copy().astype("float")
         X_and_C = pd.concat([X, C], axis=1)
         return X_and_C
 
     def _predict(self, X):
         """Predict labels for data from features.
 
         State required:
```

### Comparing `skpro-2.2.2/skpro/survival/compose/_reduce_uncensored.py` & `skpro-2.3.0/skpro/survival/compose/_reduce_uncensored.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/survival/coxph/_coxnet_sksurv.py` & `skpro-2.3.0/skpro/survival/coxph/_coxnet_sksurv.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/survival/coxph/_coxph_lifelines.py` & `skpro-2.3.0/skpro/survival/coxph/_coxph_lifelines.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/survival/coxph/_coxph_sksurv.py` & `skpro-2.3.0/skpro/survival/coxph/_coxph_sksurv.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/survival/coxph/_coxph_statsmodels.py` & `skpro-2.3.0/skpro/survival/coxph/_coxph_statsmodels.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         """
         from statsmodels.duration.hazard_regression import PHReg
 
         self._y_cols = y.columns
 
         endog = y.to_numpy().flatten()
         exog = X
-        status = C.to_numpy().flatten() if C is not None else None
+        status = 1 - C.to_numpy().flatten() if C is not None else None
 
         params = {
             "ties": self.ties,
             "missing": self.missing,
         }
 
         if self.strata is not None:
```

### Comparing `skpro-2.2.2/skpro/survival/ensemble/_grad_boost_sksurv.py` & `skpro-2.3.0/skpro/survival/ensemble/_grad_boost_sksurv.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/survival/ensemble/_survforest_sksurv.py` & `skpro-2.3.0/skpro/survival/ensemble/_survforest_sksurv.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     max_leaf_nodes : int or None, optional, default: None
         Grow a tree with ``max_leaf_nodes`` in best-first fashion.
         Best nodes are defined as relative reduction in impurity.
         If None then unlimited number of leaf nodes.
 
     bootstrap : boolean, optional, default: True
         Whether bootstrap samples are used when building trees. If False, the
-        whole datset is used to build each tree.
+        whole dataset is used to build each tree.
 
     oob_score : bool, default: False
         Whether to use out-of-bag samples to estimate
         the generalization accuracy.
 
     n_jobs : int or None, optional, default: None
         The number of jobs to run in parallel. :meth:`fit`, :meth:`predict`,
@@ -289,15 +289,15 @@
     max_leaf_nodes : int or None, optional, default: None
         Grow a tree with ``max_leaf_nodes`` in best-first fashion.
         Best nodes are defined as relative reduction in impurity.
         If None then unlimited number of leaf nodes.
 
     bootstrap : boolean, optional, default: True
         Whether bootstrap samples are used when building trees. If False, the
-        whole datset is used to build each tree.
+        whole dataset is used to build each tree.
 
     oob_score : bool, default: False
         Whether to use out-of-bag samples to estimate
         the generalization accuracy.
 
     n_jobs : int or None, optional, default: None
         The number of jobs to run in parallel. :meth:`fit`, :meth:`predict`,
```

### Comparing `skpro-2.2.2/skpro/survival/tree/_tree_sksurv.py` & `skpro-2.3.0/skpro/survival/tree/_tree_sksurv.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/tests/scenarios/scenarios.py` & `skpro-2.3.0/skpro/tests/scenarios/scenarios.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/tests/scenarios/scenarios_getter.py` & `skpro-2.3.0/skpro/tests/scenarios/scenarios_getter.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     ----------
     obj : class or object, or string, or list of str.
         Which kind of estimator/object to retrieve scenarios for.
         If object, must be a class or object inheriting from BaseObject.
         If string(s), must be in registry.BASE_CLASS_REGISTER (first col)
             for instance 'classifier', 'regressor', 'transformer', 'forecaster'
     filter_tags: dict of (str or list of str), default=None
-        subsets the returned objectss as follows:
+        subsets the returned objects as follows:
             each key/value pair is statement in "and"/conjunction
                 key is tag name to sub-set on
                 value str or list of string are tag values
                 condition is "key must be equal to value, or in set(value)"
 
     Returns
     -------
@@ -81,15 +81,15 @@
 def _check_tag_cond(obj, filter_tags=None):
     """Check whether object satisfies filter_tags condition.
 
     Parameters
     ----------
     obj: object inheriting from sktime BaseObject
     filter_tags: dict of (str or list of str), default=None
-        subsets the returned objectss as follows:
+        subsets the returned objects as follows:
             each key/value pair is statement in "and"/conjunction
                 key is tag name to sub-set on
                 value str or list of string are tag values
                 condition is "key must be equal to value, or in set(value)"
 
     Returns
     -------
```

### Comparing `skpro-2.2.2/skpro/tests/scenarios/scenarios_regressor_proba.py` & `skpro-2.3.0/skpro/tests/scenarios/scenarios_regressor_proba.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/tests/test_all_estimators.py` & `skpro-2.3.0/skpro/tests/test_all_estimators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Automated tests based on the skbase test suite template."""
 import numbers
 import types
 from copy import deepcopy
-from inspect import getfullargspec, signature
+from inspect import getfullargspec, isclass, signature
 
 import joblib
 import numpy as np
 import pandas as pd
 from skbase.testing import BaseFixtureGenerator as _BaseFixtureGenerator
 from skbase.testing import QuickTester as _QuickTester
 from skbase.testing import TestAllObjects as _TestAllObjects
@@ -78,21 +78,37 @@
     scenario: instance of TestScenario
         ranges over all scenarios returned by retrieve_scenarios
         applicable for estimator_class or estimator_instance
     """
 
     # overrides object retrieval in scikit-base
     def _all_objects(self):
-        """Retrieve list of all object classes of type self.object_type_filter."""
+        """Retrieve list of all object classes of type self.object_type_filter.
+
+        If self.object_type_filter is None, retrieve all objects.
+        If class, retrieve all classes inheriting from self.object_type_filter.
+        Otherwise (assumed str or list of str), retrieve all classes with tags
+        object_type in self.object_type_filter.
+        """
+        filter = getattr(self, "object_type_filter", None)
+
+        if isclass(filter):
+            object_types = filter.get_class_tag("object_type", None)
+        else:
+            object_types = filter
+
         obj_list = all_objects(
-            object_types=getattr(self, "object_type_filter", None),
+            object_types=object_types,
             return_names=False,
             exclude_objects=self.exclude_objects,
         )
 
+        if isclass(filter):
+            obj_list = [obj for obj in obj_list if issubclass(obj, filter)]
+
         # run_test_for_class selects the estimators to run
         # based on whether they have changed, and whether they have all dependencies
         # internally, uses the ONLY_CHANGED_MODULES flag,
         # and checks the python env against python_dependencies tag
         obj_list = [obj for obj in obj_list if run_test_for_class(obj)]
 
         return obj_list
```

### Comparing `skpro-2.2.2/skpro/tests/test_base.py` & `skpro-2.3.0/skpro/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/tests/test_baselines.py` & `skpro-2.3.0/skpro/tests/test_baselines.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/tests/test_class_register.py` & `skpro-2.3.0/skpro/tests/test_class_register.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/tests/test_density.py` & `skpro-2.3.0/skpro/tests/test_density.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/tests/test_ensemble.py` & `skpro-2.3.0/skpro/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/tests/utils.py` & `skpro-2.3.0/skpro/tests/utils.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/utils/_maint/_show_versions.py` & `skpro-2.3.0/skpro/utils/_maint/_show_versions.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/utils/_maint/tests/test_show_versions.py` & `skpro-2.3.0/skpro/utils/_maint/tests/test_show_versions.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     _get_deps_info,
     show_versions,
 )
 from skpro.utils.validation._dependencies import _check_soft_dependencies
 
 
 def test_show_versions_runs():
-    """Test that show_versions runs without exeptions."""
+    """Test that show_versions runs without exceptions."""
     # only prints, should return None
     assert show_versions() is None
 
 
 def test_deps_info():
     """Test that _get_deps_info returns package/version dict as per contract."""
     deps_info = _get_deps_info()
```

### Comparing `skpro-2.2.2/skpro/utils/deep_equals/_deep_equals.py` & `skpro-2.3.0/skpro/utils/deep_equals/_deep_equals.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/utils/estimator_checks.py` & `skpro-2.3.0/skpro/utils/estimator_checks.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/utils/index.py` & `skpro-2.3.0/skpro/utils/index.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/utils/numpy.py` & `skpro-2.3.0/skpro/utils/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     y : numpy array, 1D or 2D
         Array to flatten
 
     Returns
     -------
     y_flat : numpy array
         1D flattened array if y was 2D column vector, or 1D already
-        otherwise, returne y unchanged
+        otherwise, return y unchanged
     """
     if len(y.shape) == 2 and y.shape[1] == 1:
         y_flat = y.flatten()
     else:
         y_flat = y
 
     return y_flat
```

### Comparing `skpro-2.2.2/skpro/utils/pandas.py` & `skpro-2.3.0/skpro/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/utils/parallel.py` & `skpro-2.3.0/skpro/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/utils/plotting.py` & `skpro-2.3.0/skpro/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/utils/random_state.py` & `skpro-2.3.0/skpro/utils/random_state.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/utils/sklearn.py` & `skpro-2.3.0/skpro/utils/sklearn.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/utils/tests/test_plots.py` & `skpro-2.3.0/skpro/utils/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/utils/utils.py` & `skpro-2.3.0/skpro/utils/utils.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/utils/validation/_dependencies.py` & `skpro-2.3.0/skpro/utils/validation/_dependencies.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/workflow/base.py` & `skpro-2.3.0/skpro/workflow/base.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/workflow/cross_validation.py` & `skpro-2.3.0/skpro/workflow/cross_validation.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/workflow/manager/data.py` & `skpro-2.3.0/skpro/workflow/manager/data.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/workflow/manager/models.py` & `skpro-2.3.0/skpro/workflow/manager/models.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/workflow/table/table.py` & `skpro-2.3.0/skpro/workflow/table/table.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro/workflow/utils.py` & `skpro-2.3.0/skpro/workflow/utils.py`

 * *Files identical despite different names*

### Comparing `skpro-2.2.2/skpro.egg-info/PKG-INFO` & `skpro-2.3.0/skpro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skpro
-Version: 2.2.2
+Version: 2.3.0
 Summary: A unified framework for probability distributions and probabilistic supervised regression
 Author: Franz Király, Frithjof Gressmann, Vitaly Davydov
 Author-email: skpro developers <sktime.toolbox@gmail.com>
 Maintainer: Franz Király, Frithjof Gressmann
 Maintainer-email: skpro developers <sktime.toolbox@gmail.com>
 Project-URL: Homepage, https://github.com/sktime/skpro
 Project-URL: Repository, https://github.com/sktime/skpro
@@ -36,26 +36,26 @@
 Requires-Dist: pandas<2.3.0,>=1.1.0
 Requires-Dist: packaging
 Requires-Dist: scikit-base<0.8.0,>=0.6.1
 Requires-Dist: scikit-learn<1.5.0,>=0.24.0
 Requires-Dist: scipy<2.0.0,>=1.2.0
 Provides-Extra: all-extras
 Requires-Dist: attrs; extra == "all-extras"
+Requires-Dist: cyclic-boosting>=1.4.0; python_version < "3.12" and extra == "all-extras"
 Requires-Dist: distfit; extra == "all-extras"
 Requires-Dist: lifelines<0.29.0; extra == "all-extras"
 Requires-Dist: mapie; extra == "all-extras"
 Requires-Dist: matplotlib>=3.3.2; extra == "all-extras"
-Requires-Dist: ngboost; extra == "all-extras"
+Requires-Dist: ngboost<0.6.0; extra == "all-extras"
 Requires-Dist: polars<0.21.0; extra == "all-extras"
 Requires-Dist: pyarrow<14.0.0; python_version < "3.12" and extra == "all-extras"
 Requires-Dist: scikit-survival<0.23.0; extra == "all-extras"
 Requires-Dist: statsmodels>=0.12.1; extra == "all-extras"
 Requires-Dist: tabulate; extra == "all-extras"
 Requires-Dist: uncertainties; extra == "all-extras"
-Requires-Dist: cyclic-boosting>=1.2.5; python_version < "3.12" and extra == "all-extras"
 Provides-Extra: dev
 Requires-Dist: backoff; extra == "dev"
 Requires-Dist: httpx; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-randomly; extra == "dev"
@@ -69,21 +69,21 @@
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: nbsphinx>=0.8.6; extra == "docs"
 Requires-Dist: numpydoc; extra == "docs"
 Requires-Dist: pydata-sphinx-theme; extra == "docs"
 Requires-Dist: sphinx!=7.2.0,<8.0.0; extra == "docs"
 Requires-Dist: sphinx-design<0.6.0; extra == "docs"
 Requires-Dist: sphinx-issues<5.0.0; extra == "docs"
-Requires-Dist: sphinx-gallery<0.16.0; extra == "docs"
+Requires-Dist: sphinx-gallery<0.17.0; extra == "docs"
 Requires-Dist: sphinx-panels; extra == "docs"
 Requires-Dist: tabulate; extra == "docs"
 
 <a href="https://skpro.readthedocs.io/en/latest"><img src="https://github.com/sktime/skpro/blob/main/docs/source/images/skpro-banner.png" width="500" align="right" /></a>
 
-:rocket: **Version 2.2.2 out now!** [Read the release notes here.](https://skpro.readthedocs.io/en/latest/changelog.html).
+:rocket: **Version 2.3.0 out now!** [Read the release notes here.](https://skpro.readthedocs.io/en/latest/changelog.html).
 
 `skpro` is a library for supervised probabilistic prediction in python.
 It provides `scikit-learn`-like, `scikit-base` compatible interfaces to:
 
 * tabular **supervised regressors for probabilistic prediction** - interval, quantile and distribution predictions
 * tabular **probabilistic time-to-event and survival prediction** - instance-individual survival distributions
 * **metrics to evaluate probabilistic predictions**, e.g., pinball loss, empirical coverage, CRPS, survival losses
@@ -94,15 +94,16 @@
 | Overview | |
 |---|---|
 | **Open Source** |  [![BSD 3-clause](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://github.com/sktime/sktime/blob/main/LICENSE) |
 | **Tutorials** | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sktime/skpro/main?filepath=examples) [![!youtube](https://img.shields.io/static/v1?logo=youtube&label=YouTube&message=tutorials&color=red)](https://www.youtube.com/playlist?list=PLKs3UgGjlWHqNzu0LEOeLKvnjvvest2d0) |
 | **Community** | [![!discord](https://img.shields.io/static/v1?logo=discord&label=discord&message=chat&color=lightgreen)](https://discord.com/invite/54ACzaFsn7) [![!slack](https://img.shields.io/static/v1?logo=linkedin&label=LinkedIn&message=news&color=lightblue)](https://www.linkedin.com/company/scikit-time/) |
 | **CI/CD** | [![github-actions](https://img.shields.io/github/actions/workflow/status/sktime/sktime/wheels.yml?logo=github)](https://github.com/sktime/skpro/actions/workflows/wheels.yml) [![!codecov](https://img.shields.io/codecov/c/github/sktime/skpro?label=codecov&logo=codecov)](https://codecov.io/gh/sktime/skpro) [![readthedocs](https://img.shields.io/readthedocs/skpro?logo=readthedocs)](https://skpro.readthedocs.io/en/latest/) [![platform](https://img.shields.io/conda/pn/conda-forge/skpro)](https://github.com/sktime/skpro) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/skpro?color=orange)](https://pypi.org/project/skpro/) [![!conda](https://img.shields.io/conda/vn/conda-forge/skpro)](https://anaconda.org/conda-forge/skpro) [![!python-versions](https://img.shields.io/pypi/pyversions/skpro)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) |
-| **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/skpro) |
+| **Downloads** | [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/skpro) [![Downloads](https://static.pepy.tech/personalized-badge/skpro?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/skpro) |
+| **Citation** | [![DOI](https://zenodo.org/badge/103107372.svg)](https://zenodo.org/doi/10.5281/zenodo.11002671) |
 
 ## :books: Documentation
 
 | Documentation              |                                                                |
 | -------------------------- | -------------------------------------------------------------- |
 | :star: **[Tutorials]**        | New to skpro? Here's everything you need to know!              |
 | :clipboard: **[Binder Notebooks]** | Example notebooks to play with in your browser.              |
@@ -133,15 +134,15 @@
 | Type                            | Platforms                               |
 | ------------------------------- | --------------------------------------- |
 | :bug: **Bug Reports**              | [GitHub Issue Tracker]                  |
 | :sparkles: **Feature Requests & Ideas** | [GitHub Issue Tracker]                       |
 | :woman_technologist: **Usage Questions**          | [GitHub Discussions] · [Stack Overflow] |
 | :speech_balloon: **General Discussion**        | [GitHub Discussions] |
 | :factory: **Contribution & Development** | `dev-chat` channel · [Discord] |
-| :globe_with_meridians: **Community collaboration session** | [Discord] - Fridays 3 pm UTC, dev/meet-ups channel |
+| :globe_with_meridians: **Community collaboration session** | [Discord] - Fridays 13 UTC, dev/meet-ups channel |
 
 [github issue tracker]: https://github.com/sktime/skpro/issues
 [github discussions]: https://github.com/sktime/skpro/discussions
 [stack overflow]: https://stackoverflow.com/questions/tagged/sktime
 [discord]: https://discord.com/invite/54ACzaFsn7
 
 
@@ -163,15 +164,15 @@
 ``skpro`` curates libraries of components of the following types:
 
 | Module | Status | Links |
 |---|---|---|
 | **[Probabilistic tabular regression]** | maturing | [Tutorial](https://github.com/sktime/skpro/blob/main/examples/01_skpro_intro.ipynb) · [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/regression.html) · [Extension Template](https://github.com/sktime/skpro/blob/main/extension_templates/regression.py) |
 | **[Time-to-event (survival) prediction]** | experimental | [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/survival.html) · [Extension Template](https://github.com/sktime/skpro/blob/main/extension_templates/survival.py) |
 | **[Performance metrics]** | maturing | [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/metrics.html) |
-| **[Probability distributions]** | maturing | [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/distributions.html) |
+| **[Probability distributions]** | maturing | [Tutorial](https://github.com/sktime/skpro/blob/main/examples/03_skpro_distributions.ipynb) · [API Reference](https://skpro.readthedocs.io/en/latest/api_reference/distributions.html) · [Extension Template](https://github.com/sktime/skpro/blob/main/extension_templates/distributions.py) |
 
 [Probabilistic tabular regression]: https://github.com/sktime/skpro/tree/main/skpro/regression
 [Time-to-event (survival) prediction]: https://github.com/sktime/skpro/tree/main/skpro/survival
 [Performance metrics]: https://github.com/sktime/skpro/tree/main/skpro/metrics
 [Probability distributions]: https://github.com/sktime/skpro/tree/main/skpro/distributions
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skpro Version: 2.2.2 Summary: A unified framework
+Metadata-Version: 2.1 Name: skpro Version: 2.3.0 Summary: A unified framework
 for probability distributions and probabilistic supervised regression Author:
 Franz KirÃ¡ly, Frithjof Gressmann, Vitaly Davydov Author-email: skpro
 developers
 gmail.com> Maintainer: Franz KirÃ¡ly, Frithjof Gressmann Maintainer-email:
 skpro developers
 gmail.com> Project-URL: Homepage, https://github.com/sktime/skpro Project-URL:
 Repository, https://github.com/sktime/skpro Project-URL: Documentation, https:/
@@ -20,55 +20,55 @@
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
 Python: <3.13,>=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.txt License-File: AUTHORS.rst Requires-Dist: numpy<1.27,>=1.21.0
 Requires-Dist: pandas<2.3.0,>=1.1.0 Requires-Dist: packaging Requires-Dist:
 scikit-base<0.8.0,>=0.6.1 Requires-Dist: scikit-learn<1.5.0,>=0.24.0 Requires-
 Dist: scipy<2.0.0,>=1.2.0 Provides-Extra: all-extras Requires-Dist: attrs;
-extra == "all-extras" Requires-Dist: distfit; extra == "all-extras" Requires-
-Dist: lifelines<0.29.0; extra == "all-extras" Requires-Dist: mapie; extra ==
-"all-extras" Requires-Dist: matplotlib>=3.3.2; extra == "all-extras" Requires-
-Dist: ngboost; extra == "all-extras" Requires-Dist: polars<0.21.0; extra ==
-"all-extras" Requires-Dist: pyarrow<14.0.0; python_version < "3.12" and extra
-== "all-extras" Requires-Dist: scikit-survival<0.23.0; extra == "all-extras"
-Requires-Dist: statsmodels>=0.12.1; extra == "all-extras" Requires-Dist:
-tabulate; extra == "all-extras" Requires-Dist: uncertainties; extra == "all-
-extras" Requires-Dist: cyclic-boosting>=1.2.5; python_version < "3.12" and
-extra == "all-extras" Provides-Extra: dev Requires-Dist: backoff; extra ==
-"dev" Requires-Dist: httpx; extra == "dev" Requires-Dist: pre-commit; extra ==
-"dev" Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-cov; extra ==
-"dev" Requires-Dist: pytest-randomly; extra == "dev" Requires-Dist: pytest-
-timeout; extra == "dev" Requires-Dist: pytest-xdist; extra == "dev" Requires-
-Dist: wheel; extra == "dev" Provides-Extra: binder Requires-Dist: jupyter;
-extra == "binder" Provides-Extra: docs Requires-Dist: jupyter; extra == "docs"
-Requires-Dist: myst-parser; extra == "docs" Requires-Dist: nbsphinx>=0.8.6;
-extra == "docs" Requires-Dist: numpydoc; extra == "docs" Requires-Dist: pydata-
-sphinx-theme; extra == "docs" Requires-Dist: sphinx!=7.2.0,<8.0.0; extra ==
-"docs" Requires-Dist: sphinx-design<0.6.0; extra == "docs" Requires-Dist:
-sphinx-issues<5.0.0; extra == "docs" Requires-Dist: sphinx-gallery<0.16.0;
-extra == "docs" Requires-Dist: sphinx-panels; extra == "docs" Requires-Dist:
-tabulate; extra == "docs" _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_s_k_t_i_m_e_/_s_k_p_r_o_/_b_l_o_b_/_m_a_i_n_/_d_o_c_s_/
-_s_o_u_r_c_e_/_i_m_a_g_e_s_/_s_k_p_r_o_-_b_a_n_n_e_r_._p_n_g_]:rocket: **Version 2.2.2 out now!** [Read the
-release notes here.](https://skpro.readthedocs.io/en/latest/changelog.html).
-`skpro` is a library for supervised probabilistic prediction in python. It
-provides `scikit-learn`-like, `scikit-base` compatible interfaces to: * tabular
-**supervised regressors for probabilistic prediction** - interval, quantile and
-distribution predictions * tabular **probabilistic time-to-event and survival
-prediction** - instance-individual survival distributions * **metrics to
-evaluate probabilistic predictions**, e.g., pinball loss, empirical coverage,
-CRPS, survival losses * **reductions** to turn `scikit-learn` regressors into
-probabilistic `skpro` regressors, such as bootstrap or conformal * building
-**pipelines and composite models**, including tuning via probabilistic
-performance metrics * symbolic **probability distributions** with value domain
-of `pandas.DataFrame`-s and `pandas`-like interface | Overview | | |---|---| |
-**Open Source** | [![BSD 3-clause](https://img.shields.io/badge/License-
-BSD%203--Clause-blue.svg)](https://github.com/sktime/sktime/blob/main/LICENSE)
-| | **Tutorials** | [![Binder](https://mybinder.org/badge_logo.svg)](https://
-mybinder.org/v2/gh/sktime/skpro/main?filepath=examples) [![!youtube](https://
-img.shields.io/static/
+extra == "all-extras" Requires-Dist: cyclic-boosting>=1.4.0; python_version <
+"3.12" and extra == "all-extras" Requires-Dist: distfit; extra == "all-extras"
+Requires-Dist: lifelines<0.29.0; extra == "all-extras" Requires-Dist: mapie;
+extra == "all-extras" Requires-Dist: matplotlib>=3.3.2; extra == "all-extras"
+Requires-Dist: ngboost<0.6.0; extra == "all-extras" Requires-Dist:
+polars<0.21.0; extra == "all-extras" Requires-Dist: pyarrow<14.0.0;
+python_version < "3.12" and extra == "all-extras" Requires-Dist: scikit-
+survival<0.23.0; extra == "all-extras" Requires-Dist: statsmodels>=0.12.1;
+extra == "all-extras" Requires-Dist: tabulate; extra == "all-extras" Requires-
+Dist: uncertainties; extra == "all-extras" Provides-Extra: dev Requires-Dist:
+backoff; extra == "dev" Requires-Dist: httpx; extra == "dev" Requires-Dist:
+pre-commit; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-Dist:
+pytest-cov; extra == "dev" Requires-Dist: pytest-randomly; extra == "dev"
+Requires-Dist: pytest-timeout; extra == "dev" Requires-Dist: pytest-xdist;
+extra == "dev" Requires-Dist: wheel; extra == "dev" Provides-Extra: binder
+Requires-Dist: jupyter; extra == "binder" Provides-Extra: docs Requires-Dist:
+jupyter; extra == "docs" Requires-Dist: myst-parser; extra == "docs" Requires-
+Dist: nbsphinx>=0.8.6; extra == "docs" Requires-Dist: numpydoc; extra == "docs"
+Requires-Dist: pydata-sphinx-theme; extra == "docs" Requires-Dist:
+sphinx!=7.2.0,<8.0.0; extra == "docs" Requires-Dist: sphinx-design<0.6.0; extra
+== "docs" Requires-Dist: sphinx-issues<5.0.0; extra == "docs" Requires-Dist:
+sphinx-gallery<0.17.0; extra == "docs" Requires-Dist: sphinx-panels; extra ==
+"docs" Requires-Dist: tabulate; extra == "docs" _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_s_k_t_i_m_e_/
+_s_k_p_r_o_/_b_l_o_b_/_m_a_i_n_/_d_o_c_s_/_s_o_u_r_c_e_/_i_m_a_g_e_s_/_s_k_p_r_o_-_b_a_n_n_e_r_._p_n_g_]:rocket: **Version 2.3.0
+out now!** [Read the release notes here.](https://skpro.readthedocs.io/en/
+latest/changelog.html). `skpro` is a library for supervised probabilistic
+prediction in python. It provides `scikit-learn`-like, `scikit-base` compatible
+interfaces to: * tabular **supervised regressors for probabilistic prediction**
+- interval, quantile and distribution predictions * tabular **probabilistic
+time-to-event and survival prediction** - instance-individual survival
+distributions * **metrics to evaluate probabilistic predictions**, e.g.,
+pinball loss, empirical coverage, CRPS, survival losses * **reductions** to
+turn `scikit-learn` regressors into probabilistic `skpro` regressors, such as
+bootstrap or conformal * building **pipelines and composite models**, including
+tuning via probabilistic performance metrics * symbolic **probability
+distributions** with value domain of `pandas.DataFrame`-s and `pandas`-like
+interface | Overview | | |---|---| | **Open Source** | [![BSD 3-clause](https:/
+/img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://github.com/
+sktime/sktime/blob/main/LICENSE) | | **Tutorials** | [![Binder](https://
+mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sktime/skpro/
+main?filepath=examples) [![!youtube](https://img.shields.io/static/
 v1?logo=youtube&label=YouTube&message=tutorials&color=red)](https://
 www.youtube.com/playlist?list=PLKs3UgGjlWHqNzu0LEOeLKvnjvvest2d0) | |
 **Community** | [![!discord](https://img.shields.io/static/
 v1?logo=discord&label=discord&message=chat&color=lightgreen)](https://
 discord.com/invite/54ACzaFsn7) [![!slack](https://img.shields.io/static/
 v1?logo=linkedin&label=LinkedIn&message=news&color=lightblue)](https://
 www.linkedin.com/company/scikit-time/) | | **CI/CD** | [![github-actions]
@@ -80,54 +80,55 @@
 (https://skpro.readthedocs.io/en/latest/) [![platform](https://img.shields.io/
 conda/pn/conda-forge/skpro)](https://github.com/sktime/skpro) | | **Code** | [!
 [!pypi](https://img.shields.io/pypi/v/skpro?color=orange)](https://pypi.org/
 project/skpro/) [![!conda](https://img.shields.io/conda/vn/conda-forge/skpro)]
 (https://anaconda.org/conda-forge/skpro) [![!python-versions](https://
 img.shields.io/pypi/pyversions/skpro)](https://www.python.org/) [![!black]
 (https://img.shields.io/badge/code%20style-black-000000.svg)](https://
-github.com/psf/black) | | **Downloads**| [![Downloads](https://
+github.com/psf/black) | | **Downloads** | [![Downloads](https://
 static.pepy.tech/personalized-badge/
 skpro?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20
 (pypi))](https://pepy.tech/project/skpro) [![Downloads](https://
 static.pepy.tech/personalized-badge/
 skpro?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20
 (pypi))](https://pepy.tech/project/skpro) [![Downloads](https://
 static.pepy.tech/personalized-badge/
 skpro?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20
-(pypi))](https://pepy.tech/project/skpro) | ## :books: Documentation |
-Documentation | | | -------------------------- | ------------------------------
--------------------------------- | | :star: **[Tutorials]** | New to skpro?
-Here's everything you need to know! | | :clipboard: **[Binder Notebooks]** |
-Example notebooks to play with in your browser. | | :woman_technologist: **
-[User Guides]** | How to use skpro and its features. | | :scissors: **
-[Extension Templates]** | How to build your own estimator using skpro's API. |
-| :control_knobs: **[API Reference]** | The detailed reference for skpro's API.
-| | :hammer_and_wrench: **[Changelog]** | Changes and version history. | | :
-deciduous_tree: **[Roadmap]** | skpro's software and community development
-plan. | | :pencil: **[Related Software]** | A list of related software. |
-[tutorials]: https://skpro.readthedocs.io/en/latest/tutorials.html [binder
-notebooks]: https://mybinder.org/v2/gh/sktime/skpro/main?filepath=examples
-[user guides]: https://skpro.readthedocs.io/en/latest/user_guide.html
-[extension templates]: https://github.com/sktime/skpro/tree/main/
-extension_templates [api reference]: https://skpro.readthedocs.io/en/latest/
-api_reference.html [changelog]: https://skpro.readthedocs.io/en/latest/
+(pypi))](https://pepy.tech/project/skpro) | | **Citation** | [![DOI](https://
+zenodo.org/badge/103107372.svg)](https://zenodo.org/doi/10.5281/
+zenodo.11002671) | ## :books: Documentation | Documentation | | | -------------
+------------- | -------------------------------------------------------------
+- | | :star: **[Tutorials]** | New to skpro? Here's everything you need to
+know! | | :clipboard: **[Binder Notebooks]** | Example notebooks to play with
+in your browser. | | :woman_technologist: **[User Guides]** | How to use skpro
+and its features. | | :scissors: **[Extension Templates]** | How to build your
+own estimator using skpro's API. | | :control_knobs: **[API Reference]** | The
+detailed reference for skpro's API. | | :hammer_and_wrench: **[Changelog]** |
+Changes and version history. | | :deciduous_tree: **[Roadmap]** | skpro's
+software and community development plan. | | :pencil: **[Related Software]** |
+A list of related software. | [tutorials]: https://skpro.readthedocs.io/en/
+latest/tutorials.html [binder notebooks]: https://mybinder.org/v2/gh/sktime/
+skpro/main?filepath=examples [user guides]: https://skpro.readthedocs.io/en/
+latest/user_guide.html [extension templates]: https://github.com/sktime/skpro/
+tree/main/extension_templates [api reference]: https://skpro.readthedocs.io/en/
+latest/api_reference.html [changelog]: https://skpro.readthedocs.io/en/latest/
 changelog.html [roadmap]: https://skpro.readthedocs.io/en/latest/roadmap.html
 [related software]: https://skpro.readthedocs.io/en/latest/
 related_software.html ## :speech_balloon: Where to ask questions Questions and
 feedback are extremely welcome! We strongly believe in the value of sharing
 help publicly, as it allows a wider audience to benefit from it. `skpro` is
 maintained by the `sktime` community, we use the same social channels. | Type |
 Platforms | | ------------------------------- | -------------------------------
 -------- | | :bug: **Bug Reports** | [GitHub Issue Tracker] | | :sparkles:
 **Feature Requests & Ideas** | [GitHub Issue Tracker] | | :woman_technologist:
 **Usage Questions** | [GitHub Discussions] Â· [Stack Overflow] | | :
 speech_balloon: **General Discussion** | [GitHub Discussions] | | :factory:
 **Contribution & Development** | `dev-chat` channel Â· [Discord] | | :
 globe_with_meridians: **Community collaboration session** | [Discord] - Fridays
-3 pm UTC, dev/meet-ups channel | [github issue tracker]: https://github.com/
+13 UTC, dev/meet-ups channel | [github issue tracker]: https://github.com/
 sktime/skpro/issues [github discussions]: https://github.com/sktime/skpro/
 discussions [stack overflow]: https://stackoverflow.com/questions/tagged/sktime
 [discord]: https://discord.com/invite/54ACzaFsn7 ## :dizzy: Features Our
 objective is to enhance the interoperability and usability of the AI model
 ecosystem: * ``skpro`` is compatible with [scikit-learn] and [sktime], e.g., an
 ``sktime`` proba forecaster can be built with an ``skpro`` proba regressor
 which in an ``sklearn`` regressor with proba mode added by ``skpro`` *
@@ -144,21 +145,24 @@
 regression.html) Â· [Extension Template](https://github.com/sktime/skpro/blob/
 main/extension_templates/regression.py) | | **[Time-to-event (survival)
 prediction]** | experimental | [API Reference](https://skpro.readthedocs.io/en/
 latest/api_reference/survival.html) Â· [Extension Template](https://github.com/
 sktime/skpro/blob/main/extension_templates/survival.py) | | **[Performance
 metrics]** | maturing | [API Reference](https://skpro.readthedocs.io/en/latest/
 api_reference/metrics.html) | | **[Probability distributions]** | maturing |
-[API Reference](https://skpro.readthedocs.io/en/latest/api_reference/
-distributions.html) | [Probabilistic tabular regression]: https://github.com/
-sktime/skpro/tree/main/skpro/regression [Time-to-event (survival) prediction]:
-https://github.com/sktime/skpro/tree/main/skpro/survival [Performance metrics]:
-https://github.com/sktime/skpro/tree/main/skpro/metrics [Probability
-distributions]: https://github.com/sktime/skpro/tree/main/skpro/distributions
-## :hourglass_flowing_sand: Installing `skpro` To install `skpro`, use `pip`:
+[Tutorial](https://github.com/sktime/skpro/blob/main/examples/
+03_skpro_distributions.ipynb) Â· [API Reference](https://skpro.readthedocs.io/
+en/latest/api_reference/distributions.html) Â· [Extension Template](https://
+github.com/sktime/skpro/blob/main/extension_templates/distributions.py) |
+[Probabilistic tabular regression]: https://github.com/sktime/skpro/tree/main/
+skpro/regression [Time-to-event (survival) prediction]: https://github.com/
+sktime/skpro/tree/main/skpro/survival [Performance metrics]: https://
+github.com/sktime/skpro/tree/main/skpro/metrics [Probability distributions]:
+https://github.com/sktime/skpro/tree/main/skpro/distributions ## :
+hourglass_flowing_sand: Installing `skpro` To install `skpro`, use `pip`:
 ```bash pip install skpro ``` or, with maximum dependencies, ```bash pip
 install skpro[all_extras] ``` Releases are available as source packages and
 binary wheels. You can see all available wheels [here](https://pypi.org/simple/
 skpro/). ## :zap: Quickstart ### Making probabilistic predictions ``` python
 from sklearn.datasets import load_diabetes from sklearn.ensemble import
 RandomForestRegressor from sklearn.linear_model import LinearRegression from
 sklearn.model_selection import train_test_split from skpro.regression.residual
```

### Comparing `skpro-2.2.2/skpro.egg-info/SOURCES.txt` & `skpro-2.3.0/skpro.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,15 @@
 AUTHORS.rst
 LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
 build_tools/changelog.py
 docs/source/conf.py
-examples/custom_model.py
-examples/simple.py
-examples/workflow.py
-examples/parametric/bagging.py
-examples/parametric/hyperparameters.py
-examples/parametric/simple.py
-examples/parametric/workflow.py
-examples/vendors/pymc.py
+extension_templates/distributions.py
 extension_templates/regression.py
 extension_templates/survival.py
 skpro/__init__.py
 skpro.egg-info/PKG-INFO
 skpro.egg-info/SOURCES.txt
 skpro.egg-info/dependency_links.txt
 skpro.egg-info/requires.txt
@@ -52,39 +45,46 @@
 skpro/datatypes/_table/_registry.py
 skpro/datatypes/tests/__init__.py
 skpro/datatypes/tests/test_check.py
 skpro/datatypes/tests/test_convert.py
 skpro/datatypes/tests/test_convert_to.py
 skpro/datatypes/tests/test_lookup.py
 skpro/distributions/__init__.py
+skpro/distributions/beta.py
+skpro/distributions/chi_squared.py
+skpro/distributions/delta.py
 skpro/distributions/empirical.py
+skpro/distributions/exponential.py
 skpro/distributions/fisk.py
 skpro/distributions/laplace.py
 skpro/distributions/logistic.py
 skpro/distributions/lognormal.py
 skpro/distributions/mixture.py
 skpro/distributions/normal.py
 skpro/distributions/poisson.py
 skpro/distributions/qpd.py
 skpro/distributions/qpd_empirical.py
 skpro/distributions/t.py
+skpro/distributions/uniform.py
 skpro/distributions/weibull.py
 skpro/distributions/adapters/__init__.py
 skpro/distributions/adapters/scipy/__init__.py
+skpro/distributions/adapters/scipy/_distribution.py
 skpro/distributions/adapters/scipy/_empirical.py
 skpro/distributions/adapters/scipy/tests/__init__.py
 skpro/distributions/adapters/scipy/tests/test_scipy_adapters.py
 skpro/distributions/adapters/statsmodels/__init__.py
 skpro/distributions/adapters/statsmodels/_empirical.py
 skpro/distributions/base/__init__.py
 skpro/distributions/base/_base.py
 skpro/distributions/base/_delegate.py
 skpro/distributions/tests/__init__.py
 skpro/distributions/tests/test_all_distrs.py
 skpro/distributions/tests/test_base_default_methods.py
+skpro/distributions/tests/test_base_scalar.py
 skpro/distributions/tests/test_proba_basic.py
 skpro/distributions/tests/test_qpd.py
 skpro/metrics/__init__.py
 skpro/metrics/_classes.py
 skpro/metrics/_coerce.py
 skpro/metrics/base.py
 skpro/metrics/survival/__init__.py
@@ -103,36 +103,42 @@
 skpro/registry/_tags.py
 skpro/registry/tests/__init__.py
 skpro/registry/tests/test_scitype.py
 skpro/registry/tests/test_tags.py
 skpro/regression/__init__.py
 skpro/regression/bootstrap.py
 skpro/regression/cyclic_boosting.py
+skpro/regression/delta.py
 skpro/regression/density.py
-skpro/regression/ensemble.py
 skpro/regression/mapie.py
 skpro/regression/multiquantile.py
 skpro/regression/residual.py
 skpro/regression/adapters/__init__.py
+skpro/regression/adapters/ngboost/__init__.py
+skpro/regression/adapters/ngboost/_ngboost_proba.py
 skpro/regression/adapters/sklearn/__init__.py
 skpro/regression/adapters/sklearn/_sklearn_proba.py
 skpro/regression/base/__init__.py
 skpro/regression/base/_base.py
 skpro/regression/base/_delegate.py
 skpro/regression/base/adapters/__init__.py
 skpro/regression/base/adapters/_sklearn.py
 skpro/regression/baselines/__init__.py
 skpro/regression/baselines/density.py
 skpro/regression/compose/__init__.py
 skpro/regression/compose/_pipeline.py
+skpro/regression/ensemble/__init__.py
+skpro/regression/ensemble/_bagging.py
+skpro/regression/ensemble/_ngboost.py
 skpro/regression/gp/__init__.py
 skpro/regression/gp/_sklearn.py
 skpro/regression/linear/__init__.py
 skpro/regression/linear/_glm.py
 skpro/regression/linear/_sklearn.py
+skpro/regression/linear/_sklearn_poisson.py
 skpro/regression/parametric/__init__.py
 skpro/regression/parametric/estimators.py
 skpro/regression/parametric/parametric.py
 skpro/regression/tests/__init__.py
 skpro/regression/tests/test_all_regressors.py
 skpro/regression/tests/test_cyclic_boosting.py
 skpro/regression/vendors/__init__.py
@@ -155,31 +161,36 @@
 skpro/survival/coxph/__init__.py
 skpro/survival/coxph/_coxnet_sksurv.py
 skpro/survival/coxph/_coxph_lifelines.py
 skpro/survival/coxph/_coxph_sksurv.py
 skpro/survival/coxph/_coxph_statsmodels.py
 skpro/survival/ensemble/__init__.py
 skpro/survival/ensemble/_grad_boost_sksurv.py
+skpro/survival/ensemble/_ngboost_surv.py
 skpro/survival/ensemble/_survforest_sksurv.py
 skpro/survival/tree/__init__.py
 skpro/survival/tree/_tree_sksurv.py
 skpro/tests/__init__.py
+skpro/tests/_config.py
+skpro/tests/_config_test_dummy.py
 skpro/tests/test_all_estimators.py
 skpro/tests/test_base.py
 skpro/tests/test_baselines.py
 skpro/tests/test_class_register.py
 skpro/tests/test_density.py
 skpro/tests/test_ensemble.py
 skpro/tests/test_switch.py
 skpro/tests/test_vendors.py
 skpro/tests/utils.py
 skpro/tests/scenarios/__init__.py
 skpro/tests/scenarios/scenarios.py
 skpro/tests/scenarios/scenarios_getter.py
 skpro/tests/scenarios/scenarios_regressor_proba.py
+skpro/tests/tests/__init__.py
+skpro/tests/tests/test_test_utils.py
 skpro/utils/__init__.py
 skpro/utils/estimator_checks.py
 skpro/utils/git_diff.py
 skpro/utils/index.py
 skpro/utils/numpy.py
 skpro/utils/pandas.py
 skpro/utils/parallel.py
```

### Comparing `skpro-2.2.2/skpro.egg-info/requires.txt` & `skpro-2.3.0/skpro.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 
 [all_extras]
 attrs
 distfit
 lifelines<0.29.0
 mapie
 matplotlib>=3.3.2
-ngboost
+ngboost<0.6.0
 polars<0.21.0
 scikit-survival<0.23.0
 statsmodels>=0.12.1
 tabulate
 uncertainties
 
 [all_extras:python_version < "3.12"]
+cyclic-boosting>=1.4.0
 pyarrow<14.0.0
-cyclic-boosting>=1.2.5
 
 [binder]
 jupyter
 
 [dev]
 backoff
 httpx
@@ -41,10 +41,10 @@
 myst-parser
 nbsphinx>=0.8.6
 numpydoc
 pydata-sphinx-theme
 sphinx!=7.2.0,<8.0.0
 sphinx-design<0.6.0
 sphinx-issues<5.0.0
-sphinx-gallery<0.16.0
+sphinx-gallery<0.17.0
 sphinx-panels
 tabulate
```

