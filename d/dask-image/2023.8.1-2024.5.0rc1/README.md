# Comparing `tmp/dask-image-2023.8.1.tar.gz` & `tmp/dask_image-2024.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-image-2023.8.1.tar", last modified: Fri Aug  4 11:08:20 2023, max compression
+gzip compressed data, was "dask_image-2024.5.0rc1.tar", last modified: Fri May 17 06:25:30 2024, max compression
```

## Comparing `dask-image-2023.8.1.tar` & `dask_image-2024.5.0rc1.tar`

### file list

```diff
@@ -1,106 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:08:20.926084 dask-image-2023.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-04 11:08:10.000000 dask-image-2023.8.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-08-04 11:08:10.000000 dask-image-2023.8.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21206 2023-08-04 11:08:10.000000 dask-image-2023.8.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-04 11:08:10.000000 dask-image-2023.8.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-08-04 11:08:10.000000 dask-image-2023.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    23001 2023-08-04 11:08:20.926084 dask-image-2023.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-04 11:08:10.000000 dask-image-2023.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:08:20.926084 dask-image-2023.8.1/dask_image/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-08-04 11:08:20.926084 dask-image-2023.8.1/dask_image/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:08:20.922084 dask-image-2023.8.1/dask_image/dispatch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/dispatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9369 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/dispatch/_dispatch_ndfilters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/dispatch/_dispatch_ndinterp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/dispatch/_dispatch_ndmorph.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/dispatch/_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/dispatch/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:08:20.922084 dask-image-2023.8.1/dask_image/imread/
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/imread/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:08:20.922084 dask-image-2023.8.1/dask_image/ndfilters/
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/ndfilters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/ndfilters/_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/ndfilters/_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/ndfilters/_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/ndfilters/_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/ndfilters/_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/ndfilters/_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/ndfilters/_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/ndfilters/_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/ndfilters/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:08:20.922084 dask-image-2023.8.1/dask_image/ndfourier/
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/ndfourier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/ndfourier/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:08:20.922084 dask-image-2023.8.1/dask_image/ndinterp/
--rw-r--r--   0 runner    (1001) docker     (123)    13010 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/ndinterp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:08:20.922084 dask-image-2023.8.1/dask_image/ndmeasure/
--rw-r--r--   0 runner    (1001) docker     (123)    23869 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/ndmeasure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:08:20.922084 dask-image-2023.8.1/dask_image/ndmeasure/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/ndmeasure/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/ndmeasure/_utils/_find_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/ndmeasure/_utils/_label.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:08:20.922084 dask-image-2023.8.1/dask_image/ndmorph/
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/ndmorph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/ndmorph/_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-08-04 11:08:10.000000 dask-image-2023.8.1/dask_image/ndmorph/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:08:20.918084 dask-image-2023.8.1/dask_image.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23001 2023-08-04 11:08:20.000000 dask-image-2023.8.1/dask_image.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-08-04 11:08:20.000000 dask-image-2023.8.1/dask_image.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 11:08:20.000000 dask-image-2023.8.1/dask_image.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 11:08:20.000000 dask-image-2023.8.1/dask_image.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-04 11:08:20.000000 dask-image-2023.8.1/dask_image.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-04 11:08:20.000000 dask-image-2023.8.1/dask_image.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:08:20.922084 dask-image-2023.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-08-04 11:08:10.000000 dask-image-2023.8.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-04 11:08:10.000000 dask-image-2023.8.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-04 11:08:10.000000 dask-image-2023.8.1/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9202 2023-08-04 11:08:10.000000 dask-image-2023.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-04 11:08:10.000000 dask-image-2023.8.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-08-04 11:08:10.000000 dask-image-2023.8.1/docs/coverage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-04 11:08:10.000000 dask-image-2023.8.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-08-04 11:08:10.000000 dask-image-2023.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-08-04 11:08:10.000000 dask-image-2023.8.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-08-04 11:08:10.000000 dask-image-2023.8.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-08-04 11:08:10.000000 dask-image-2023.8.1/docs/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:08:20.922084 dask-image-2023.8.1/docs/release/
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-08-04 11:08:10.000000 dask-image-2023.8.1/docs/release/release_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-04 11:08:20.926084 dask-image-2023.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-08-04 11:08:10.000000 dask-image-2023.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:08:20.922084 dask-image-2023.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:08:20.918084 dask-image-2023.8.1/tests/test_dask_image/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:08:20.922084 dask-image-2023.8.1/tests/test_dask_image/test_imread/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/test_dask_image/test_imread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/test_dask_image/test_imread/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/test_dask_image/test_imread/test_cupy_imread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:08:20.926084 dask-image-2023.8.1/tests/test_dask_image/test_ndfilters/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/test_dask_image/test_ndfilters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/test_dask_image/test_ndfilters/test__conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/test_dask_image/test_ndfilters/test__diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/test_dask_image/test_ndfilters/test__edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/test_dask_image/test_ndfilters/test__gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/test_dask_image/test_ndfilters/test__generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/test_dask_image/test_ndfilters/test__order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/test_dask_image/test_ndfilters/test__smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/test_dask_image/test_ndfilters/test__threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/test_dask_image/test_ndfilters/test__utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/test_dask_image/test_ndfilters/test_cupy_ndfilters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/test_dask_image/test_ndfilters/test_cupy_threshold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:08:20.926084 dask-image-2023.8.1/tests/test_dask_image/test_ndfourier/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/test_dask_image/test_ndfourier/test__utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/test_dask_image/test_ndfourier/test_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:08:20.926084 dask-image-2023.8.1/tests/test_dask_image/test_ndinterp/
--rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/test_dask_image/test_ndinterp/test_affine_transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/test_dask_image/test_ndinterp/test_spline_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:08:20.926084 dask-image-2023.8.1/tests/test_dask_image/test_ndmeasure/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/test_dask_image/test_ndmeasure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/test_dask_image/test_ndmeasure/test__utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16764 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/test_dask_image/test_ndmeasure/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/test_dask_image/test_ndmeasure/test_find_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:08:20.926084 dask-image-2023.8.1/tests/test_dask_image/test_ndmorph/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/test_dask_image/test_ndmorph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/test_dask_image/test_ndmorph/test__utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/test_dask_image/test_ndmorph/test_cupy_ndmorph.py
--rw-r--r--   0 runner    (1001) docker     (123)    15796 2023-08-04 11:08:10.000000 dask-image-2023.8.1/tests/test_dask_image/test_ndmorph/test_ndmorph.py
--rw-r--r--   0 runner    (1001) docker     (123)    68567 2023-08-04 11:08:10.000000 dask-image-2023.8.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:25:30.476973 dask_image-2024.5.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/.coveralls.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:25:30.456973 dask_image-2024.5.0rc1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:25:30.456973 dask_image-2024.5.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    24469 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-17 06:25:30.476973 dask_image-2024.5.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:25:30.456973 dask_image-2024.5.0rc1/continuous_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/continuous_integration/environment-3.10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/continuous_integration/environment-3.11.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/continuous_integration/environment-3.12.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/continuous_integration/environment-3.9.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/continuous_integration/environment-doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/continuous_integration/environment-latest.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:25:30.460973 dask_image-2024.5.0rc1/continuous_integration/gpuci/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/continuous_integration/gpuci/axis.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/continuous_integration/gpuci/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:25:30.460973 dask_image-2024.5.0rc1/dask_image/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-17 06:25:30.000000 dask_image-2024.5.0rc1/dask_image/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:25:30.460973 dask_image-2024.5.0rc1/dask_image/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/dispatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9369 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/dispatch/_dispatch_ndfilters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/dispatch/_dispatch_ndinterp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/dispatch/_dispatch_ndmorph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/dispatch/_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/dispatch/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:25:30.460973 dask_image-2024.5.0rc1/dask_image/imread/
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/imread/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:25:30.464973 dask_image-2024.5.0rc1/dask_image/ndfilters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/ndfilters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/ndfilters/_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/ndfilters/_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/ndfilters/_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/ndfilters/_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/ndfilters/_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/ndfilters/_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/ndfilters/_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/ndfilters/_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/ndfilters/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:25:30.464973 dask_image-2024.5.0rc1/dask_image/ndfourier/
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/ndfourier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/ndfourier/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:25:30.464973 dask_image-2024.5.0rc1/dask_image/ndinterp/
+-rw-r--r--   0 runner    (1001) docker     (127)    17746 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/ndinterp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:25:30.464973 dask_image-2024.5.0rc1/dask_image/ndmeasure/
+-rw-r--r--   0 runner    (1001) docker     (127)    24228 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/ndmeasure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:25:30.464973 dask_image-2024.5.0rc1/dask_image/ndmeasure/_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/ndmeasure/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/ndmeasure/_utils/_find_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/ndmeasure/_utils/_label.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:25:30.464973 dask_image-2024.5.0rc1/dask_image/ndmorph/
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/ndmorph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/ndmorph/_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/dask_image/ndmorph/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:25:30.472973 dask_image-2024.5.0rc1/dask_image.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-17 06:25:30.000000 dask_image-2024.5.0rc1/dask_image.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-17 06:25:30.000000 dask_image-2024.5.0rc1/dask_image.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 06:25:30.000000 dask_image-2024.5.0rc1/dask_image.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 06:25:30.000000 dask_image-2024.5.0rc1/dask_image.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-17 06:25:30.000000 dask_image-2024.5.0rc1/dask_image.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-17 06:25:30.000000 dask_image-2024.5.0rc1/dask_image.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:25:30.468973 dask_image-2024.5.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9205 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/docs/coverage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/docs/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:25:30.468973 dask_image-2024.5.0rc1/docs/release/
+-rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/docs/release/generate_release_notes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/docs/release/release_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 06:25:30.476973 dask_image-2024.5.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:25:30.468973 dask_image-2024.5.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:25:30.452973 dask_image-2024.5.0rc1/tests/test_dask_image/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:25:30.468973 dask_image-2024.5.0rc1/tests/test_dask_image/test_imread/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_imread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_imread/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_imread/test_cupy_imread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:25:30.472973 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfilters/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfilters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfilters/test__conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfilters/test__diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfilters/test__edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfilters/test__gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfilters/test__generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfilters/test__order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfilters/test__smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfilters/test__threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfilters/test__utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfilters/test_cupy_ndfilters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfilters/test_cupy_threshold.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:25:30.472973 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfourier/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfourier/test__utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfourier/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:25:30.472973 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndinterp/
+-rw-r--r--   0 runner    (1001) docker     (127)    13191 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndinterp/test_affine_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndinterp/test_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7174 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndinterp/test_spline_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:25:30.472973 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndmeasure/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndmeasure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndmeasure/test__utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26183 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndmeasure/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndmeasure/test_find_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:25:30.472973 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndmorph/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndmorph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndmorph/test__utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndmorph/test_cupy_ndmorph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15796 2024-05-17 06:25:21.000000 dask_image-2024.5.0rc1/tests/test_dask_image/test_ndmorph/test_ndmorph.py
```

### Comparing `dask-image-2023.8.1/CONTRIBUTING.rst` & `dask_image-2024.5.0rc1/CONTRIBUTING.rst`

 * *Files 2% similar despite different names*

```diff
@@ -80,31 +80,32 @@
 
 Ready to contribute? Here's how to set up `dask-image` for local development.
 
 1. Fork the `dask-image` repo on GitHub.
 2. Clone your fork locally::
 
     $ git clone git@github.com:your_name_here/dask-image.git
+    $ cd dask-image
 
 3. Install your local copy into an environment. Assuming you have conda installed, this is how you set up your fork for local development (on Windows drop `source`). Replace `"<some version>"` with the Python version used for testing.::
 
     $ conda create -n dask-image-env python="<some version>"
     $ source activate dask-image-env
-    $ python setup.py develop
+    $ python -m pip install -e .
 
 4. Create a branch for local development::
 
     $ git checkout -b name-of-your-bugfix-or-feature
 
    Now you can make your changes locally.
 
 5. When you're done making changes, check that your changes pass flake8 and the tests, including testing other Python versions::
 
     $ flake8 dask_image tests
-    $ python setup.py test or py.test
+    $ pytest
 
    To get flake8, just conda install it into your environment.
 
 6. Commit your changes and push your branch to GitHub::
 
     $ git add .
     $ git commit -m "Your detailed description of your changes."
@@ -160,15 +161,15 @@
 
     $ conda activate dask-image-testenv
 
 Finally, install the development version of dask-image::
 
 .. code-block:: console
 
-    $ pip install -e .
+    $ pip install -e ".[test]""
 
 For local testing, please run ``pytest`` in the test environment::
 
 .. code-block:: console
 
     $ pytest
```

### Comparing `dask-image-2023.8.1/HISTORY.rst` & `dask_image-2024.5.0rc1/HISTORY.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,78 @@
 =======
 History
 =======
 
+2024.5.0 (2024-05-17)
+----------------------
+
+We're pleased to announce the release of dask-image 2024.5.0!
+
+Highlights
+
+Highlights of this release include:
+
+* Martin Schorb adding 'rotate', 'spline_filter' and 'spline_filter1d' functions (#213)
+* Erik Holmgren adding functionality to allow wrapping labels over array boundaries (#344), and 
+* Christoph Sommer's work allowing aicsimageio and other da.core.Array sub-classes as input arrays (#361)
+
+New Features
+
+* Add the rotate, spline_filter, and spline_filter1d functions to ndimage (#213)
+* Wrapping labels over array boundaries (#344)
+* Add python 3.12 support (#370)
+
+Improvements
+
+* Relaxed type check of input array, to allow da.core.Array sub-classes… (#361)
+* Update slice index comment to reflect code change (#353)
+
+Maintenance
+
+* Switch to pyproject.toml package setup, replace versioneer with setuptools-scm (#306)
+* Fix cupy pytest errors (#368)
+* Switch to newer GPU CI images (#345)
+* Bump GPU CI to CUDA 11.8 (#348)
+* Maintenance: fix CI test errors (#366)
+* Update CI test environments (#367)
+* Additions to release guide and change to release note generation script (#339)
+* Fix typo in pull request template (#347)
+* Workaround for the sphinx version problem in the readthedocs build environment (#354)
+* Pin dask to 2024.4.1 to avoid error during dask.dataframe import with python 3.11.9 (#363)
+* Get rid of distutils dependency -- Depend on newer scipy (#346)
+* Bump actions/checkout from 3 to 4 (#342)
+* Bump actions/setup-python from 4 to 5 (#350)
+* Bump coverallsapp/github-action from 2.2.1 to 2.2.3 (#343)
+* Bump conda-incubator/setup-miniconda from 2 to 3 (#349)
+* Bump coverallsapp/github-action from 2.2.3 to 2.3.0 (#365)
+* Update versioneer to version 0.29 for compatibility with python 3.12 (#357)
+
+
+9 authors added to this release (alphabetical)
+
+* `Charles Blackmon-Luca <https://github.com/dask/dask-image/commits?author=charlesbluca>`_ - @charlesbluca
+* `Christoph Sommer <https://github.com/dask/dask-image/commits?author=sommerc>`_ - @sommerc
+* `dependabot[bot] <https://github.com/dask/dask-image/commits?author=dependabot[bot]>`_ - @dependabot[bot]
+* `Erik Holmgren <https://github.com/dask/dask-image/commits?author=Holmgren825>`_ - @Holmgren825
+* `Genevieve Buckley <https://github.com/dask/dask-image/commits?author=GenevieveBuckley>`_ - @GenevieveBuckley
+* `jakirkham <https://github.com/dask/dask-image/commits?author=jakirkham>`_ - @jakirkham
+* `Mark Harfouche <https://github.com/dask/dask-image/commits?author=hmaarrfk>`_ - @hmaarrfk
+* `Martin Schorb <https://github.com/dask/dask-image/commits?author=martinschorb>`_ - @martinschorb
+* `Marvin Albert <https://github.com/dask/dask-image/commits?author=m-albert>`_ - @m-albert
+
+
+5 reviewers added to this release (alphabetical)
+
+* `Erik Holmgren <https://github.com/dask/dask-image/commits?author=Holmgren825>`_ - @Holmgren825
+* `Genevieve Buckley <https://github.com/dask/dask-image/commits?author=GenevieveBuckley>`_ - @GenevieveBuckley
+* `jakirkham <https://github.com/dask/dask-image/commits?author=jakirkham>`_ - @jakirkham
+* `Juan Nunez-Iglesias <https://github.com/dask/dask-image/commits?author=jni>`_ - @jni
+* `Marvin Albert <https://github.com/dask/dask-image/commits?author=m-albert>`_ - @m-albert
+
+
 2023.08.1 (2023-08-04)
 ----------------------
 
 We're pleased to announce the release of dask-image 2023.08.1!
 
 This is a patch release to complete the dropping of python 3.8
 in the previous release.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dask-image-2023.8.1/LICENSE.txt` & `dask_image-2024.5.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/README.rst` & `dask_image-2024.5.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/dask_image/dispatch/_dispatch_ndfilters.py` & `dask_image-2024.5.0rc1/dask_image/dispatch/_dispatch_ndfilters.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/dask_image/dispatch/_dispatch_ndinterp.py` & `dask_image-2024.5.0rc1/dask_image/dispatch/_dispatch_ndinterp.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/dask_image/dispatch/_dispatch_ndmorph.py` & `dask_image-2024.5.0rc1/dask_image/dispatch/_dispatch_ndmorph.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/dask_image/dispatch/_dispatcher.py` & `dask_image-2024.5.0rc1/dask_image/dispatch/_dispatcher.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/dask_image/dispatch/_utils.py` & `dask_image-2024.5.0rc1/dask_image/dispatch/_utils.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/dask_image/imread/__init__.py` & `dask_image-2024.5.0rc1/dask_image/imread/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/dask_image/ndfilters/__init__.py` & `dask_image-2024.5.0rc1/dask_image/ndfilters/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/dask_image/ndfilters/_conv.py` & `dask_image-2024.5.0rc1/dask_image/ndfilters/_conv.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/dask_image/ndfilters/_edge.py` & `dask_image-2024.5.0rc1/dask_image/ndfilters/_edge.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/dask_image/ndfilters/_gaussian.py` & `dask_image-2024.5.0rc1/dask_image/ndfilters/_gaussian.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/dask_image/ndfilters/_generic.py` & `dask_image-2024.5.0rc1/dask_image/ndfilters/_generic.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/dask_image/ndfilters/_order.py` & `dask_image-2024.5.0rc1/dask_image/ndfilters/_order.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/dask_image/ndfilters/_smooth.py` & `dask_image-2024.5.0rc1/dask_image/ndfilters/_smooth.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/dask_image/ndfilters/_threshold.py` & `dask_image-2024.5.0rc1/dask_image/ndfilters/_threshold.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/dask_image/ndfilters/_utils.py` & `dask_image-2024.5.0rc1/dask_image/ndfilters/_utils.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/dask_image/ndfourier/__init__.py` & `dask_image-2024.5.0rc1/dask_image/ndfourier/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/dask_image/ndfourier/_utils.py` & `dask_image-2024.5.0rc1/dask_image/ndfourier/_utils.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/dask_image/ndinterp/__init__.py` & `dask_image-2024.5.0rc1/dask_image/ndinterp/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 # -*- coding: utf-8 -*-
 
 import functools
 import math
 from itertools import product
-import warnings
 
 import dask.array as da
 import numpy as np
 from dask.base import tokenize
 from dask.highlevelgraph import HighLevelGraph
 import scipy
 from scipy.ndimage import affine_transform as ndimage_affine_transform
+from scipy.special import sindg, cosdg
 
 from ..dispatch._dispatch_ndinterp import (
     dispatch_affine_transform,
     dispatch_asarray,
     dispatch_spline_filter,
     dispatch_spline_filter1d,
 )
 from ..ndfilters._utils import _get_depth_boundary
 
 from ..dispatch._dispatch_ndinterp import (dispatch_affine_transform,
                                            dispatch_asarray)
 
 __all__ = [
     "affine_transform",
+    "rotate",
+    "spline_filter",
+    "spline_filter1d",
 ]
 
 
 def affine_transform(
         image,
         matrix,
         offset=0.0,
@@ -76,15 +79,15 @@
     Returns
     -------
     affine_transform : Dask Array
         A dask array representing the transformed output
 
     """
 
-    if not type(image) == da.core.Array:
+    if not isinstance(image, da.core.Array):
         image = da.from_array(image)
 
     if output_shape is None:
         output_shape = image.shape
 
     if output_chunks is None:
         output_chunks = image.shape
@@ -243,14 +246,168 @@
                            # chunks=output_chunks,
                            chunks=normalized_chunks,
                            meta=meta)
 
     return transformed
 
 
+def rotate(
+        input_arr,
+        angle,
+        axes=(1, 0),
+        reshape=True,
+        output_chunks=None,
+        **kwargs,
+        ):
+    """Rotate an array using Dask.
+
+    The array is rotated in the plane defined by the two axes given by the
+    `axes` parameter using spline interpolation of the requested order.
+
+    Chunkwise processing is performed using `dask_image.ndinterp.affine_transform`,
+    for which further parameters supported by the ndimage functions can be
+    passed as keyword arguments.
+
+    Notes
+    -----
+        Differences to `ndimage.rotate`:
+        - currently, prefiltering is not supported
+          (affecting the output in case of interpolation `order > 1`)
+        - default order is 1
+        - modes 'reflect', 'mirror' and 'wrap' are not supported
+
+        Arguments are equal to `ndimage.rotate` except for
+        - `output` (not present here)
+        - `output_chunks` (relevant in the dask array context)
+
+    Parameters
+    ----------
+    input_arr : array_like (Numpy Array, Cupy Array, Dask Array...)
+        The image array.
+    angle : float
+        The rotation angle in degrees.
+    axes : tuple of 2 ints, optional
+        The two axes that define the plane of rotation. Default is the first
+        two axes.
+    reshape : bool, optional
+        If `reshape` is true, the output shape is adapted so that the input
+        array is contained completely in the output. Default is True.
+    output_chunks : tuple of ints, optional
+        The shape of the chunks of the output Dask Array.
+    **kwargs : dict, optional
+        Additional keyword arguments are passed to
+        `dask_image.ndinterp.affine_transform`.
+
+    Returns
+    -------
+    rotate : Dask Array
+        A dask array representing the rotated input.
+
+    Examples
+    --------
+    >>> from scipy import ndimage, misc
+    >>> import matplotlib.pyplot as plt
+    >>> import dask.array as da
+    >>> fig = plt.figure(figsize=(10, 3))
+    >>> ax1, ax2, ax3 = fig.subplots(1, 3)
+    >>> img = da.from_array(misc.ascent(),chunks=(64,64))
+    >>> img_45 = dask_image.ndinterp.rotate(img, 45, reshape=False)
+    >>> full_img_45 = dask_image.ndinterp.rotate(img, 45, reshape=True)
+    >>> ax1.imshow(img, cmap='gray')
+    >>> ax1.set_axis_off()
+    >>> ax2.imshow(img_45, cmap='gray')
+    >>> ax2.set_axis_off()
+    >>> ax3.imshow(full_img_45, cmap='gray')
+    >>> ax3.set_axis_off()
+    >>> fig.set_tight_layout(True)
+    >>> plt.show()
+    >>> print(img.shape)
+    (512, 512)
+    >>> print(img_45.shape)
+    (512, 512)
+    >>> print(full_img_45.shape)
+    (724, 724)
+
+    """
+    if not isinstance(input_arr, da.core.Array):
+        input_arr = da.from_array(input_arr)
+
+    if output_chunks is None:
+        output_chunks = input_arr.chunksize
+
+    ndim = input_arr.ndim
+
+    if ndim < 2:
+        raise ValueError('input array should be at least 2D')
+
+    axes = list(axes)
+
+    if len(axes) != 2:
+        raise ValueError('axes should contain exactly two values')
+
+    if not all([float(ax).is_integer() for ax in axes]):
+        raise ValueError('axes should contain only integer values')
+
+    if axes[0] < 0:
+        axes[0] += ndim
+    if axes[1] < 0:
+        axes[1] += ndim
+    if axes[0] < 0 or axes[1] < 0 or axes[0] >= ndim or axes[1] >= ndim:
+        raise ValueError('invalid rotation plane specified')
+
+    axes.sort()
+
+    c, s = cosdg(angle), sindg(angle)
+
+    rot_matrix = np.array([[c, s],
+                           [-s, c]])
+
+    img_shape = np.asarray(input_arr.shape)
+    in_plane_shape = img_shape[axes]
+
+    if reshape:
+        # Compute transformed input bounds
+        iy, ix = in_plane_shape
+        out_bounds = rot_matrix @ [[0, 0, iy, iy],
+                                   [0, ix, 0, ix]]
+        # Compute the shape of the transformed input plane
+        out_plane_shape = (out_bounds.ptp(axis=1) + 0.5).astype(int)
+    else:
+        out_plane_shape = img_shape[axes]
+
+    output_shape = np.array(img_shape)
+    output_shape[axes] = out_plane_shape
+    output_shape = tuple(output_shape)
+
+    out_center = rot_matrix @ ((out_plane_shape - 1) / 2)
+    in_center = (in_plane_shape - 1) / 2
+    offset = in_center - out_center
+
+    matrix_nd = np.eye(ndim)
+    offset_nd = np.zeros(ndim)
+
+    for o_x,idx in enumerate(axes):
+
+        matrix_nd[idx,axes[0]] = rot_matrix[o_x,0]
+        matrix_nd[idx,axes[1]] = rot_matrix[o_x,1]
+
+        offset_nd[idx] = offset[o_x]
+
+    output = affine_transform(
+        input_arr,
+        matrix=matrix_nd,
+        offset=offset_nd,
+        output_shape=output_shape,
+        output_chunks=output_chunks,
+        **kwargs,
+        )
+
+    return output
+
+
 # magnitude of the maximum filter pole for each order
 # (obtained from scipy/ndimage/src/ni_splines.c)
 _maximum_pole = {
     2: 0.171572875253809902396622551580603843,
     3: 0.267949192431122706472553658494127633,
     4: 0.361341225900220177092212841325675255,
     5: 0.430575347099973791851434783493520110,
@@ -273,15 +430,15 @@
         mode='mirror',
         output_chunks=None,
         *,
         depth=None,
         **kwargs
 ):
 
-    if not type(image) == da.core.Array:
+    if not isinstance(image, da.core.Array):
         image = da.from_array(image)
 
     # use dispatching mechanism to determine backend
     spline_filter_method = dispatch_spline_filter(image)
 
     try:
         dtype = np.dtype(output)
@@ -331,15 +488,15 @@
         mode='mirror',
         output_chunks=None,
         *,
         depth=None,
         **kwargs
 ):
 
-    if not type(image) == da.core.Array:
+    if not isinstance(image, da.core.Array):
         image = da.from_array(image)
 
     # use dispatching mechanism to determine backend
     spline_filter1d_method = dispatch_spline_filter1d(image)
 
     try:
         dtype = np.dtype(output)
```

### Comparing `dask-image-2023.8.1/dask_image/ndmeasure/__init__.py` & `dask_image-2024.5.0rc1/dask_image/ndmeasure/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,15 +299,15 @@
     result = labeled_comprehension(
         image, label_image, index, func, object, None
     )
 
     return result
 
 
-def label(image, structure=None):
+def label(image, structure=None, wrap_axes=None):
     """
     Label features in an array.
 
     Parameters
     ----------
     image : ndarray
         An array-like object to be labeled.  Any non-zero values in ``image``
@@ -319,14 +319,22 @@
         equal to one.  That is, for a 2-D ``image`` array, the default
         structuring element is::
 
             [[0,1,0],
              [1,1,1],
              [0,1,0]]
 
+    wrap_axes : tuple of int, optional
+        Whether labels should be wrapped across array boundaries, and if so which axes.
+        This feature is not present in `ndimage.label`.
+        Examples:
+        - (0,) only wrap across the 0th axis.
+        - (0, 1) wrap across the 0th and 1st axis.
+        - (0, 1, 3)  wrap across 0th, 1st and 3rd axis.
+
     Returns
     -------
     label : ndarray or int
         An integer ndarray where each unique feature in ``image`` has a unique
         label in the returned array.
     num_features : int
         How many objects were found.
@@ -359,20 +367,22 @@
 
     # Put all the blocks together
     block_labeled = da.block(labeled_blocks.tolist())
 
     # Now, build a label connectivity graph that groups labels across blocks.
     # We use this graph to find connected components and then relabel each
     # block according to those.
-    label_groups = _label.label_adjacency_graph(block_labeled, structure,
-                                                total)
+    label_groups = _label.label_adjacency_graph(
+        block_labeled, structure, total, wrap_axes=wrap_axes
+    )
     new_labeling = _label.connected_components_delayed(label_groups)
     relabeled = _label.relabel_blocks(block_labeled, new_labeling)
     n = da.max(relabeled)
 
+
     return (relabeled, n)
 
 
 def labeled_comprehension(image,
                           label_image,
                           index,
                           func,
```

### Comparing `dask-image-2023.8.1/dask_image/ndmeasure/_utils/__init__.py` & `dask_image-2024.5.0rc1/dask_image/ndmeasure/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/dask_image/ndmeasure/_utils/_find_objects.py` & `dask_image-2024.5.0rc1/dask_image/ndmeasure/_utils/_find_objects.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/dask_image/ndmeasure/_utils/_label.py` & `dask_image-2024.5.0rc1/dask_image/ndmeasure/_utils/_label.py`

 * *Files 11% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 def _to_csr_matrix(i, j, n):
     """Using i and j as coo-format coordinates, return csr matrix."""
     v = np.ones_like(i)
     mat = scipy.sparse.coo_matrix((v, (i, j)), shape=(n, n))
     return mat.tocsr()
 
 
-def label_adjacency_graph(labels, structure, nlabels):
+def label_adjacency_graph(labels, structure, nlabels, wrap_axes=None):
     """
     Adjacency graph of labels between chunks of ``labels``.
 
     Each chunk in ``labels`` has been labeled independently, and the labels
     in different chunks are guaranteed to be unique.
 
     Here we construct a graph connecting labels in different chunks that
@@ -140,110 +140,140 @@
     labels : dask array of int
         The input labeled array, where each chunk is independently labeled.
     structure : array of bool
         Structuring element, shape (3,) * labels.ndim.
     nlabels : delayed int
         The total number of labels in ``labels`` *before* correcting for
         global consistency.
+    wrap_axes : tuple of int, optional
+        Should labels be wrapped across array boundaries, and if so which axes.
+        - (0,) only wrap over the 0th axis.
+        - (0, 1) wrap over the 0th and 1st axis.
+        - (0, 1, 3)  wrap over 0th, 1st and 3rd axis.
 
     Returns
     -------
     mat : delayed scipy.sparse.csr_matrix
         This matrix has value 1 at (i, j) if label i is connected to
         label j in the global volume, 0 everywhere else.
     """
 
     if structure is None:
         structure = scipy.ndimage.generate_binary_structure(labels.ndim, 1)
 
-    faces = _chunk_faces(labels.chunks, labels.shape, structure)
+    face_slices = _chunk_faces(
+        labels.chunks, labels.shape, structure, wrap_axes=wrap_axes
+    )
     all_mappings = [da.empty((2, 0), dtype=LABEL_DTYPE, chunks=1)]
-    for face_slice in faces:
+
+    for face_slice in face_slices:
         face = labels[face_slice]
         mapped = _across_block_label_grouping_delayed(face, structure)
         all_mappings.append(mapped)
+
     all_mappings = da.concatenate(all_mappings, axis=1)
     i, j = all_mappings
     mat = _to_csr_matrix(i, j, nlabels + 1)
+
     return mat
 
 
-def _chunk_faces(chunks, shape, structure):
+def _chunk_faces(chunks, shape, structure, wrap_axes=None):
     """
     Return slices for two-pixel-wide boundaries between chunks.
 
     Parameters
     ----------
     chunks : tuple of tuple of int
         The chunk specification of the array.
     shape : tuple of int
         The shape of the array.
     structure: array of bool
         Structuring element, shape (3,) * ndim.
+    wrap_axes : tuple of int, optional
+        Should labels be wrapped across array boundaries, and if so which axes.
+        - (0,) only wrap over the 0th axis.
+        - (0, 1) wrap over the 0th and 1st axis.
+        - (0, 1, 3)  wrap over 0th, 1st and 3rd axis.
 
-    Returns
+    Yields
     -------
-    faces : list of tuple of slices
-        Each element in this list indexes a face between two chunks.
+    tuple of slices
+        Each element indexes a face between two chunks.
 
     Examples
     --------
     >>> import dask.array as da
     >>> import scipy.ndimage as ndi
     >>> a = da.arange(110, chunks=110).reshape((10, 11)).rechunk(5)
     >>> structure = ndi.generate_binary_structure(2, 1)
-    >>> chunk_faces(a.chunks, a.shape, structure)
+    >>> list(chunk_faces(a.chunks, a.shape, structure))
     [(slice(4, 6, None), slice(0, 5, None)),
      (slice(4, 6, None), slice(5, 10, None)),
      (slice(4, 6, None), slice(10, 11, None)),
      (slice(0, 5, None), slice(4, 6, None)),
      (slice(0, 5, None), slice(9, 11, None)),
      (slice(5, 10, None), slice(4, 6, None)),
      (slice(5, 10, None), slice(9, 11, None))]
     """
 
     ndim = len(shape)
-    numblocks = tuple(list(len(c) for c in chunks))
-    
+
     slices = da.core.slices_from_chunks(chunks)
-    
+
     # arrange block/chunk indices on grid
-    block_summary = np.arange(len(slices)).reshape(numblocks)
-    
-    faces = []
-    for ind_curr_block, curr_block in enumerate(np.ndindex(numblocks)):
-        
+    block_summary = np.arange(len(slices)).reshape(
+        [len(c) for c in chunks])
+
+    # Iterate over all blocks and use the structuring element
+    # to determine which blocks should be connected.
+    # For wrappped axes, we need to consider the block
+    # before the current block with index -1 as well.
+    numblocks = [len(c) if wrap_axes is None or ax not in wrap_axes
+                 else len(c) + 1 for ax, c in enumerate(chunks)]
+    for curr_block in np.ndindex(tuple(numblocks)):
+
+        curr_block = list(curr_block)
+
+        if wrap_axes is not None:
+            # start at -1 indices for wrapped axes
+            for wrap_axis in wrap_axes:
+                curr_block[wrap_axis] = curr_block[wrap_axis] - 1
+
+        # iterate over neighbors of the current block
         for pos_structure_coord in np.array(np.where(structure)).T:
-                        
+
             # only consider forward neighbors
             if min(pos_structure_coord) < 1 or \
                max(pos_structure_coord) < 2: continue
 
             neigh_block = [curr_block[dim] + pos_structure_coord[dim] - 1
                            for dim in range(ndim)]
 
-            if max([neigh_block[dim] >= numblocks[dim] for dim in range(ndim)]): continue
+            if max([neigh_block[dim] >= block_summary.shape[dim]
+                    for dim in range(ndim)]): continue
 
-            # get neighbor slice index
-            ind_neigh_block = block_summary[tuple(neigh_block)]
+            # get current slice index
+            ind_curr_block = block_summary[tuple(curr_block)]
 
             curr_slice = []
             for dim in range(ndim):
                 # keep slice if not on boundary
-                if slices[ind_curr_block][dim] == slices[ind_neigh_block][dim]:
+                if neigh_block[dim] == curr_block[dim]:
                     curr_slice.append(slices[ind_curr_block][dim])
                 # otherwise, add two-pixel-wide boundary
                 else:
-                    curr_slice.append(slice(
-                        slices[ind_curr_block][dim].stop - 1,
-                        slices[ind_curr_block][dim].stop + 1))
-                    
-            faces.append(tuple(curr_slice))
-            
-    return faces
+                    if slices[ind_curr_block][dim].stop == shape[dim]:
+                        curr_slice.append(slice(None, None, shape[dim] - 1))
+                    else:
+                        curr_slice.append(slice(
+                            slices[ind_curr_block][dim].stop - 1,
+                            slices[ind_curr_block][dim].stop + 1))
+
+            yield tuple(curr_slice)
 
 
 def block_ndi_label_delayed(block, structure):
     """
     Delayed version of ``scipy.ndimage.label``.
 
     Parameters
```

### Comparing `dask-image-2023.8.1/dask_image/ndmorph/__init__.py` & `dask_image-2024.5.0rc1/dask_image/ndmorph/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/dask_image/ndmorph/_ops.py` & `dask_image-2024.5.0rc1/dask_image/ndmorph/_ops.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/dask_image/ndmorph/_utils.py` & `dask_image-2024.5.0rc1/dask_image/ndmorph/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         generate_binary_structure = dispatch_binary_structure(image)
         structure = generate_binary_structure(image.ndim, 1)
     elif hasattr(structure, 'ndim'):
         if structure.ndim != image.ndim:
             raise RuntimeError(
                 "`structure` must have the same rank as `image`."
             )
-        if not issubclass(structure.dtype.type, np.bool8):
+        if not issubclass(structure.dtype.type, np.bool_):
             structure = (structure != 0)
     else:
         raise TypeError("`structure` must be an array.")
 
     return structure
 
 
@@ -55,17 +55,17 @@
     if mask is None:
         mask = True
 
     mask_type = _get_dtype(mask).type
     if isinstance(mask, (np.ndarray, da.Array)):
         if mask.shape != image.shape:
             raise RuntimeError("`mask` must have the same shape as `image`.")
-        if not issubclass(mask_type, np.bool8):
+        if not issubclass(mask_type, np.bool_):
             mask = (mask != 0)
-    elif issubclass(mask_type, np.bool8):
+    elif issubclass(mask_type, np.bool_):
         mask = bool(mask)
     else:
         raise TypeError("`mask` must be a Boolean or an array.")
 
     return mask
```

### Comparing `dask-image-2023.8.1/docs/Makefile` & `dask_image-2024.5.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/docs/conf.py` & `dask_image-2024.5.0rc1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
 import sys
 import os
 
+import dask_image._version
+
 # If extensions (or modules to document with autodoc) are in another
 # directory, add these directories to sys.path here. If the directory is
 # relative to the documentation root, use os.path.abspath to make it
 # absolute, like shown here.
 #sys.path.insert(0, os.path.abspath('.'))
 
 # Get the project root dir, which is the parent dir of this
@@ -27,16 +29,14 @@
 project_root = os.path.dirname(cwd)
 
 # Insert the project root dir as the first element in the PYTHONPATH.
 # This lets us ensure that the source package is imported, and that its
 # version is used.
 sys.path.insert(0, project_root)
 
-import dask_image
-
 # -- General configuration ---------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
@@ -63,18 +63,18 @@
 project = u'dask-image'
 copyright = u"2018, John Kirkham"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
-# The short X.Y version.
-version = dask_image.__version__
 # The full version, including alpha/beta/rc tags.
-release = dask_image.__version__
+release = dask_image._version.__version__
+# The short X.Y.Z version.
+version = '.'.join(release.split('.')[:3])
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to
 # some non-false value, then it is used:
@@ -284,15 +284,14 @@
 
 # Run sphinx-apidoc before building docs.
 def run_apidoc(_):
     ignore_paths = [
         "../setup.py",
         "../tests",
         "../travis_pypi_setup.py",
-        "../versioneer.py"
     ]
 
     argv = [
         "-f",
         "-T",
         "-e",
         "-M",
```

### Comparing `dask-image-2023.8.1/docs/coverage.rst` & `dask_image-2024.5.0rc1/docs/coverage.rst`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,15 @@
      - ✓
    * - ``rank_filter``
      - ✓
      - ✓
      - ✓
    * - ``rotate``
      - ✓
-     -
+     - ✓
      -
    * - ``shift``
      - ✓
      -
      -
    * - ``sobel``
      - ✓
@@ -307,8 +307,7 @@
      - ✓
      -
      -
    * - ``zoom``
      - ✓
      -
      -
-
```

### Comparing `dask-image-2023.8.1/docs/index.rst` & `dask_image-2024.5.0rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/docs/installation.rst` & `dask_image-2024.5.0rc1/docs/installation.rst`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 If you don't have `conda`_ installed, you can download and install it with the
 `Anaconda distribution here`_.
 
 Alternatively, you can install dask-image with pip:
 
 .. code-block:: console
 
-    $ pip install dask-image
+    $ python -m pip install dask-image
 
 If you don't have `pip`_ installed, this `Python installation guide`_
 can guide you through the process.
 
 .. _conda: https://conda.io/en/latest/
 .. _Anaconda distribution here: https://www.anaconda.com/distribution/
 .. _pip: https://pip.pypa.io
@@ -53,12 +53,13 @@
 
     $ curl  -OL https://github.com/dask/dask-image/tarball/main
 
 Once you have a copy of the source, you can install it with:
 
 .. code-block:: console
 
-    $ python setup.py install
+    $ cd dask-image
+    $ python -m pip install .
 
 
 .. _Github repo: https://github.com/dask/dask-image
 .. _tarball: https://github.com/dask/dask-image/tarball/main
```

### Comparing `dask-image-2023.8.1/docs/make.bat` & `dask_image-2024.5.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/docs/quickstart.rst` & `dask_image-2024.5.0rc1/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/docs/release/release_guide.rst` & `dask_image-2024.5.0rc1/docs/release/release_guide.rst`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 You will also need these additional release dependencies
 to complete the release process:
 
 
 .. code-block:: bash
 
-   pip install PyGithub>=1.44.1 twine>=3.1.1 tqdm
+   pip install "PyGithub>=1.44.1" "twine>=3.1.1" tqdm
 
 
 
 Set PyPI password as GitHub secret
 ----------------------------------
 
 The `dask/dask-image` repository must have a PyPI API token as a GitHub secret.
@@ -38,28 +38,28 @@
 
 We use `calendar versioning (CalVer) <https://calver.org/>`_
 for `dask-image`. This means version numbers have the format
 `YYYY.MM.X`. Here, YYYY indicates the year, MM indicates the month,
 and X is an integer counter beginning at zero (to distinguish
 between cases where multiple releases were made in the same month).
 
-`Versioneer <https://github.com/warner/python-versioneer>`_
+`setuptools-scm <https://setuptools-scm.readthedocs.io/en/stable/>`_
 then determines the exact version from the latest
 `git tag <https://git-scm.com/book/en/v2/Git-Basics-Tagging>`_
 beginning with `v`. So our git tags will have the format `vYYYY.MM.X`.
 
 So for example, a git tag "v2030.01.0" will be the first release
 made in the month of January, in the year 2030.
 
 Generate the release notes
 --------------------------
 
 The release notes contain a list of merges, contributors, and reviewers.
 
-1. Crate a GH_TOKEN environment variable on your computer.
+1. Create a GH_TOKEN environment variable on your computer.
 
     On Linux/Mac:
 
     .. code-block:: bash
 
        export GH_TOKEN=<your-gh-api-token>
 
@@ -116,17 +116,18 @@
 Create the release candidate
 -----------------------------
 
 Go to the dask-image releases page: https://github.com/dask/dask-image/releases
 
 Click the "Draft Release" button to create a new release candidate.
 
-- Both the tag version and release title should have the format ``vYYYY.MM.DDrc1``.
+- Both the tag version and release title should have the format ``vYYYY.MM.Xrc1``.
 - Copy-paste the release notes from ``HISTORY.rst`` for this release into the
   description text box.
+- Tick "Set as a pre-release"
 
 Note here how we are using ``rc`` for release candidate to create a version
 of our release we can test before making the real release.
 
 Creating the release will trigger a GitHub actions script,
 which automatically uploads the release to PyPI.
 
@@ -142,24 +143,26 @@
 
 
 It is recommended that the release candidate is tested in a virtual environment
 in order to isolate dependencies.
 
 If the release candidate is not what you want, make your changes and
 repeat the process from the beginning but
-incrementing the number after ``rc`` (e.g. ``vYYYY.MM.DDrc1``).
+incrementing the number after ``rc`` (e.g. ``vYYYY.MM.Xrc1``).
 
 Once you are satisfied with the release candidate it is time to generate
 the actual release.
 
 Generating the actual release
 -----------------------------
 
 To generate the actual release you will now repeat the processes above
-but now dropping the ``rc`` suffix from the version number.
+but now
+- dropping the ``rc`` suffix from the version number.
+- ticking "Set as the latest release"
 
 This will automatically upload the release to PyPI, and will also
 automatically begin the process to release the new version on conda-forge.
 
 Releasing on conda-forge
 ------------------------
 
@@ -167,16 +170,23 @@
 ``regro-cf-autotick-bot`` to see that there is a new release
 available on PyPI, and open a pull request in the ``dask-image``
 conda-forge feedstock here: https://github.com/conda-forge/dask-image-feedstock
 
 Note: the conda-forge bot will not open a PR for any of the release candidates,
 only for the final release. Only one PR is opened for
 
+As an alternative to waiting for the conda-forge bot to notice the new release,
+you can submit a new dask-image feedstock issue indicating
+``@conda-forge-admin, please update version`` in the issue title. This will
+`trigger <https://conda-forge.org/docs/maintainer/infrastructure.html#conda-forge-admin-please-update-version>`_`
+the bot to check for new versions.
+
 Before merging the pull request, first you should check:
 
 * That all the tests have passed on CI for this pull request
-* If any dependencies were changed, and should be updated in the pull request
+* If any dependencies were changed, and should be updated by
+  commiting changes to ``recipe/meta.yaml`` to the pull request
 
 Once that all looks good you can merge the pull request,
 and the newest version of ``dask-image`` will automatically be made
 available on conda-forge. We're finished!
```

### Comparing `dask-image-2023.8.1/tests/test_dask_image/test_imread/test_cupy_imread.py` & `dask_image-2024.5.0rc1/tests/test_dask_image/test_imread/test_cupy_imread.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/tests/test_dask_image/test_ndfilters/test__conv.py` & `dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfilters/test__conv.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/tests/test_dask_image/test_ndfilters/test__diff.py` & `dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfilters/test__diff.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/tests/test_dask_image/test_ndfilters/test__edge.py` & `dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfilters/test__edge.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/tests/test_dask_image/test_ndfilters/test__gaussian.py` & `dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfilters/test__gaussian.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/tests/test_dask_image/test_ndfilters/test__generic.py` & `dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfilters/test__generic.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/tests/test_dask_image/test_ndfilters/test__order.py` & `dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfilters/test__order.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/tests/test_dask_image/test_ndfilters/test__smooth.py` & `dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfilters/test__smooth.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/tests/test_dask_image/test_ndfilters/test__threshold.py` & `dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfilters/test__threshold.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,111 +1,124 @@
 import dask.array as da
 import numpy as np
 from numpy.testing import assert_equal
 import pytest
 
 from dask_image.ndfilters import threshold_local
 
+@pytest.fixture
+def simple_test_image():
+    image = da.from_array(np.array(
+        [[0, 0, 1, 3, 5],
+         [0, 1, 4, 3, 4],
+         [1, 2, 5, 4, 1],
+         [2, 4, 5, 2, 1],
+         [4, 5, 1, 0, 0]], dtype=int), chunks=(5, 5))
+    return image
+
+
+# ==================================================
+# Test Threshold Filters
+# ==================================================
+
+@pytest.mark.parametrize('block_size', [
+    3,
+    [3, 3],
+    np.array([3, 3]),
+    da.from_array(np.array([3, 3]), chunks=1),
+    da.from_array(np.array([3, 3]), chunks=2),
+])
+def test_threshold_local_gaussian(simple_test_image, block_size):
+    ref = np.array(
+        [[False, False, False, False,  True],
+            [False, False,  True, False,  True],
+            [False, False,  True,  True, False],
+            [False,  True,  True, False, False],
+            [True,  True, False, False, False]]
+    )
+    out = threshold_local(simple_test_image, block_size, method='gaussian')
+    assert_equal(ref, (simple_test_image > out).compute())
+
+    out = threshold_local(simple_test_image, block_size, method='gaussian',
+                            param=1./3.)
+    assert_equal(ref, (simple_test_image > out).compute())
+
+
+@pytest.mark.parametrize('block_size', [
+    3,
+    [3, 3],
+    np.array([3, 3]),
+    da.from_array(np.array([3, 3]), chunks=1),
+    da.from_array(np.array([3, 3]), chunks=2),
+])
+def test_threshold_local_mean(simple_test_image, block_size):
+    ref = np.array(
+        [[False, False, False, False,  True],
+            [False, False,  True, False,  True],
+            [False, False,  True,  True, False],
+            [False,  True,  True, False, False],
+            [True,  True, False, False, False]]
+    )
+    out = threshold_local(simple_test_image, block_size, method='mean')
+    assert_equal(ref, (simple_test_image > out).compute())
+
 
 @pytest.mark.parametrize('block_size', [
     3,
     [3, 3],
     np.array([3, 3]),
     da.from_array(np.array([3, 3]), chunks=1),
     da.from_array(np.array([3, 3]), chunks=2),
 ])
-class TestSimpleImage:
-    def setup(self):
-        self.image = da.from_array(np.array(
-            [[0, 0, 1, 3, 5],
-             [0, 1, 4, 3, 4],
-             [1, 2, 5, 4, 1],
-             [2, 4, 5, 2, 1],
-             [4, 5, 1, 0, 0]], dtype=int), chunks=(5, 5))
-
-    def test_threshold_local_gaussian(self, block_size):
-        ref = np.array(
-            [[False, False, False, False,  True],
-             [False, False,  True, False,  True],
-             [False, False,  True,  True, False],
-             [False,  True,  True, False, False],
-             [True,  True, False, False, False]]
-        )
-        out = threshold_local(self.image, block_size, method='gaussian')
-        assert_equal(ref, (self.image > out).compute())
-
-        out = threshold_local(self.image, block_size, method='gaussian',
-                              param=1./3.)
-        assert_equal(ref, (self.image > out).compute())
-
-    def test_threshold_local_mean(self, block_size):
-        ref = np.array(
-            [[False, False, False, False,  True],
-             [False, False,  True, False,  True],
-             [False, False,  True,  True, False],
-             [False,  True,  True, False, False],
-             [True,  True, False, False, False]]
-        )
-        out = threshold_local(self.image, block_size, method='mean')
-        assert_equal(ref, (self.image > out).compute())
-
-    def test_threshold_local_median(self, block_size):
-        ref = np.array(
-            [[False, False, False, False,  True],
-             [False, False,  True, False, False],
-             [False, False,  True, False, False],
-             [False, False,  True,  True, False],
-             [False,  True, False, False, False]]
-        )
-        out = threshold_local(self.image, block_size, method='median')
-        assert_equal(ref, (self.image > out).compute())
-
-
-class TestGenericFilter:
-    def setup(self):
-        self.image = da.from_array(np.array(
-            [[0, 0, 1, 3, 5],
-             [0, 1, 4, 3, 4],
-             [1, 2, 5, 4, 1],
-             [2, 4, 5, 2, 1],
-             [4, 5, 1, 0, 0]], dtype=int), chunks=(5, 5))
-
-    def test_threshold_local_generic(self):
-        ref = np.array(
-            [[1.,  7., 16., 29., 37.],
-             [5., 14., 23., 30., 30.],
-             [13., 24., 30., 29., 21.],
-             [25., 29., 28., 19., 10.],
-             [34., 31., 23., 10.,  4.]]
-        )
-        unchanged = threshold_local(self.image, 1, method='generic', param=sum)
-        out = threshold_local(self.image, 3, method='generic', param=sum)
-        assert np.allclose(unchanged.compute(), self.image.compute())
-        assert np.allclose(out.compute(), ref)
-
-    def test_threshold_local_generic_invalid(self):
-        expected_error_message = "Must include a valid function to use as "
-        "the 'param' keyword argument."
-        with pytest.raises(ValueError) as e:
-            threshold_local(self.image, 3, method='generic', param='sum')
-            assert e == expected_error_message
-
-
-class TestInvalidArguments:
-    def setup(self):
-        self.image = da.from_array(np.array(
-            [[0, 0, 1, 3, 5],
-             [0, 1, 4, 3, 4],
-             [1, 2, 5, 4, 1],
-             [2, 4, 5, 2, 1],
-             [4, 5, 1, 0, 0]], dtype=int), chunks=(5, 5))
-
-    @pytest.mark.parametrize("method, block_size, error_type", [
-        ('median', np.nan, TypeError),
-    ])
-    def test_nan_blocksize(self, method, block_size, error_type):
-        with pytest.raises(error_type):
-            threshold_local(self.image, block_size, method=method)
-
-    def test_invalid_threshold_method(self):
-        with pytest.raises(ValueError):
-            threshold_local(self.image, 3, method='invalid')
+def test_threshold_local_median(simple_test_image, block_size):
+    ref = np.array(
+        [[False, False, False, False,  True],
+            [False, False,  True, False, False],
+            [False, False,  True, False, False],
+            [False, False,  True,  True, False],
+            [False,  True, False, False, False]]
+    )
+    out = threshold_local(simple_test_image, block_size, method='median')
+    assert_equal(ref, (simple_test_image > out).compute())
+
+
+# ==================================================
+# Test Generic Filters
+# ==================================================
+
+def test_threshold_local_generic(simple_test_image):
+    ref = np.array(
+        [[1.,  7., 16., 29., 37.],
+         [5., 14., 23., 30., 30.],
+         [13., 24., 30., 29., 21.],
+         [25., 29., 28., 19., 10.],
+         [34., 31., 23., 10.,  4.]]
+    )
+    unchanged = threshold_local(simple_test_image, 1, method='generic', param=sum)
+    out = threshold_local(simple_test_image, 3, method='generic', param=sum)
+    assert np.allclose(unchanged.compute(), simple_test_image.compute())
+    assert np.allclose(out.compute(), ref)
+
+
+def test_threshold_local_generic_invalid(simple_test_image):
+    expected_error_message = "Must include a valid function to use as "
+    "the 'param' keyword argument."
+    with pytest.raises(ValueError) as e:
+        threshold_local(simple_test_image, 3, method='generic', param='sum')
+        assert e == expected_error_message
+
+
+# ==================================================
+# Test Invalid Arguments
+# ==================================================
+
+@pytest.mark.parametrize("method, block_size, error_type", [
+    ('median', np.nan, TypeError),
+])
+def test_nan_blocksize(simple_test_image, method, block_size, error_type):
+    with pytest.raises(error_type):
+        threshold_local(simple_test_image, block_size, method=method)
+
+
+def test_invalid_threshold_method(simple_test_image):
+    with pytest.raises(ValueError):
+        threshold_local(simple_test_image, 3, method='invalid')
```

### Comparing `dask-image-2023.8.1/tests/test_dask_image/test_ndfilters/test__utils.py` & `dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfilters/test__utils.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/tests/test_dask_image/test_ndfilters/test_cupy_ndfilters.py` & `dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfilters/test_cupy_ndfilters.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/tests/test_dask_image/test_ndfilters/test_cupy_threshold.py` & `dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfilters/test_cupy_threshold.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,114 +5,129 @@
 import numpy as np
 import pytest
 
 from dask_image.ndfilters import threshold_local
 
 cupy = pytest.importorskip("cupy", minversion="5.0.0")
 
+@pytest.fixture
+def simple_test_image():
+    image = da.from_array(cupy.array(
+        [[0, 0, 1, 3, 5],
+         [0, 1, 4, 3, 4],
+         [1, 2, 5, 4, 1],
+         [2, 4, 5, 2, 1],
+         [4, 5, 1, 0, 0]], dtype=int), chunks=(5, 5))
+    return image
+
+
+# ==================================================
+# Test Threshold Filters
+# ==================================================
+
+@pytest.mark.cupy
+@pytest.mark.parametrize('block_size', [
+    3,
+    [3, 3],
+    np.array([3, 3]),
+    da.from_array(np.array([3, 3]), chunks=1),
+    da.from_array(np.array([3, 3]), chunks=2),
+])
+def test_threshold_local_gaussian(simple_test_image, block_size):
+    ref = np.array(
+        [[False, False, False, False,  True],
+            [False, False,  True, False,  True],
+            [False, False,  True,  True, False],
+            [False,  True,  True, False, False],
+            [True,  True, False, False, False]]
+    )
+    out = threshold_local(simple_test_image, block_size, method='gaussian')
+    cupy.testing.assert_array_equal(ref, (simple_test_image > out).compute())
+
+    out = threshold_local(simple_test_image, block_size, method='gaussian',
+                            param=1./3.)
+    cupy.testing.assert_array_equal(ref, (simple_test_image > out).compute())
+
+
+@pytest.mark.cupy
+@pytest.mark.parametrize('block_size', [
+    3,
+    [3, 3],
+    np.array([3, 3]),
+    da.from_array(np.array([3, 3]), chunks=1),
+    da.from_array(np.array([3, 3]), chunks=2),
+])
+def test_threshold_local_mean(simple_test_image, block_size):
+    ref = cupy.array(
+        [[False, False, False, False,  True],
+            [False, False,  True, False,  True],
+            [False, False,  True,  True, False],
+            [False,  True,  True, False, False],
+            [True,  True, False, False, False]]
+    )
+    out = threshold_local(simple_test_image, block_size, method='mean')
+    cupy.testing.assert_array_equal(ref, (simple_test_image > out).compute())
+
 
 @pytest.mark.cupy
 @pytest.mark.parametrize('block_size', [
     3,
     [3, 3],
     np.array([3, 3]),
     da.from_array(np.array([3, 3]), chunks=1),
     da.from_array(np.array([3, 3]), chunks=2),
 ])
-class TestSimpleImage:
-    def setup(self):
-        self.image = da.from_array(cupy.array(
-            [[0, 0, 1, 3, 5],
-             [0, 1, 4, 3, 4],
-             [1, 2, 5, 4, 1],
-             [2, 4, 5, 2, 1],
-             [4, 5, 1, 0, 0]], dtype=int), chunks=(5, 5))
-
-    def test_threshold_local_gaussian(self, block_size):
-        ref = np.array(
-            [[False, False, False, False,  True],
-             [False, False,  True, False,  True],
-             [False, False,  True,  True, False],
-             [False,  True,  True, False, False],
-             [True,  True, False, False, False]]
-        )
-        out = threshold_local(self.image, block_size, method='gaussian')
-        cupy.testing.assert_array_equal(ref, (self.image > out).compute())
-
-        out = threshold_local(self.image, block_size, method='gaussian',
-                              param=1./3.)
-        cupy.testing.assert_array_equal(ref, (self.image > out).compute())
-
-    def test_threshold_local_mean(self, block_size):
-        ref = cupy.array(
-            [[False, False, False, False,  True],
-             [False, False,  True, False,  True],
-             [False, False,  True,  True, False],
-             [False,  True,  True, False, False],
-             [True,  True, False, False, False]]
-        )
-        out = threshold_local(self.image, block_size, method='mean')
-        cupy.testing.assert_array_equal(ref, (self.image > out).compute())
-
-    def test_threshold_local_median(self, block_size):
-        ref = cupy.array(
-            [[False, False, False, False,  True],
-             [False, False,  True, False, False],
-             [False, False,  True, False, False],
-             [False, False,  True,  True, False],
-             [False,  True, False, False, False]]
-        )
-        out = threshold_local(self.image, block_size, method='median')
-        cupy.testing.assert_array_equal(ref, (self.image > out).compute())
-
-
-class TestGenericFilter:
-    def setup(self):
-        self.image = da.from_array(cupy.array(
-            [[0, 0, 1, 3, 5],
-             [0, 1, 4, 3, 4],
-             [1, 2, 5, 4, 1],
-             [2, 4, 5, 2, 1],
-             [4, 5, 1, 0, 0]], dtype=int), chunks=(5, 5))
-
-    def test_threshold_local_generic(self):
-        ref = cupy.array(
-            [[1.,  7., 16., 29., 37.],
-             [5., 14., 23., 30., 30.],
-             [13., 24., 30., 29., 21.],
-             [25., 29., 28., 19., 10.],
-             [34., 31., 23., 10.,  4.]]
-        )
-        my_sum = cupy.ReductionKernel(
-            'T x', 'T out', 'x', 'a + b', 'out = a', '0', 'my_sum')
-        unchanged = threshold_local(self.image, 1, method='generic', param=my_sum)  # noqa: E501
-        out = threshold_local(self.image, 3, method='generic', param=my_sum)
-        assert cupy.allclose(unchanged.compute(), self.image.compute())
-        assert cupy.allclose(out.compute(), ref)
-
-    def test_threshold_local_generic_invalid(self):
-        expected_error_message = "Must include a valid function to use as "
-        "the 'param' keyword argument."
-        with pytest.raises(ValueError) as e:
-            threshold_local(self.image, 3, method='generic', param='sum')
-            assert e == expected_error_message
-
-
-class TestInvalidArguments:
-    def setup(self):
-        self.image = da.from_array(cupy.array(
-            [[0, 0, 1, 3, 5],
-             [0, 1, 4, 3, 4],
-             [1, 2, 5, 4, 1],
-             [2, 4, 5, 2, 1],
-             [4, 5, 1, 0, 0]], dtype=int), chunks=(5, 5))
-
-    @pytest.mark.parametrize("method, block_size, error_type", [
-        ('median', cupy.nan, TypeError),
-    ])
-    def test_nan_blocksize(self, method, block_size, error_type):
-        with pytest.raises(error_type):
-            threshold_local(self.image, block_size, method=method)
-
-    def test_invalid_threshold_method(self):
-        with pytest.raises(ValueError):
-            threshold_local(self.image, 3, method='invalid')
+def test_threshold_local_median(simple_test_image, block_size):
+    ref = cupy.array(
+        [[False, False, False, False,  True],
+            [False, False,  True, False, False],
+            [False, False,  True, False, False],
+            [False, False,  True,  True, False],
+            [False,  True, False, False, False]]
+    )
+    out = threshold_local(simple_test_image, block_size, method='median')
+    cupy.testing.assert_array_equal(ref, (simple_test_image > out).compute())
+
+
+# ==================================================
+# Test Generic Filters
+# ==================================================
+
+def test_threshold_local_generic(simple_test_image):
+    ref = cupy.array(
+        [[1.,  7., 16., 29., 37.],
+            [5., 14., 23., 30., 30.],
+            [13., 24., 30., 29., 21.],
+            [25., 29., 28., 19., 10.],
+            [34., 31., 23., 10.,  4.]]
+    )
+    my_sum = cupy.ReductionKernel(
+        'T x', 'T out', 'x', 'a + b', 'out = a', '0', 'my_sum')
+    unchanged = threshold_local(simple_test_image, 1, method='generic', param=my_sum)  # noqa: E501
+    out = threshold_local(simple_test_image, 3, method='generic', param=my_sum)
+    assert cupy.allclose(unchanged.compute(), simple_test_image.compute())
+    assert cupy.allclose(out.compute(), ref)
+
+
+def test_threshold_local_generic_invalid(simple_test_image):
+    expected_error_message = "Must include a valid function to use as "
+    "the 'param' keyword argument."
+    with pytest.raises(ValueError) as e:
+        threshold_local(simple_test_image, 3, method='generic', param='sum')
+        assert e == expected_error_message
+
+
+# ==================================================
+# Test Invalid Arguments
+# ==================================================
+
+@pytest.mark.parametrize("method, block_size, error_type", [
+    ('median', cupy.nan, TypeError),
+])
+def test_nan_blocksize(simple_test_image, method, block_size, error_type):
+    with pytest.raises(error_type):
+        threshold_local(simple_test_image, block_size, method=method)
+
+
+def test_invalid_threshold_method(simple_test_image):
+    with pytest.raises(ValueError):
+        threshold_local(simple_test_image, 3, method='invalid')
```

### Comparing `dask-image-2023.8.1/tests/test_dask_image/test_ndfourier/test__utils.py` & `dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfourier/test__utils.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/tests/test_dask_image/test_ndfourier/test_core.py` & `dask_image-2024.5.0rc1/tests/test_dask_image/test_ndfourier/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import numbers
-from distutils.version import LooseVersion
 
 import pytest
 import numpy as np
 import scipy as sp
 import scipy.ndimage
 
 import dask.array as da
@@ -88,15 +87,14 @@
         ("fourier_shift", numbers.Real),
         ("fourier_gaussian", numbers.Integral),
         ("fourier_uniform", numbers.Integral),
     ]
 )
 def test_fourier_filter_type(funcname, upcast_type, dtype):
     if (
-            LooseVersion(sp.__version__) >= "1.0.0" and
             dtype in [np.int64, np.float64] and
             funcname in ["fourier_gaussian", "fourier_uniform"]
        ):
         pytest.skip(
             "SciPy 1.0.0+ doesn't handle double precision values correctly."
         )
```

### Comparing `dask-image-2023.8.1/tests/test_dask_image/test_ndinterp/test_affine_transformation.py` & `dask_image-2024.5.0rc1/tests/test_dask_image/test_ndinterp/test_affine_transformation.py`

 * *Files 5% similar despite different names*

```diff
@@ -280,21 +280,14 @@
     image = da.ones((3, 3))
     image_t = dask_image.ndinterp.affine_transform(image, np.eye(2), [0, 0])
 
     assert image_t.shape == image.shape
     assert image_t.chunks == tuple([(s,) for s in image.shape])
 
 
-def test_affine_transform_prefilter_warning():
-
-    with pytest.warns(UserWarning):
-        dask_image.ndinterp.affine_transform(da.ones(20), [1], [0],
-                                             order=3, prefilter=True)
-
-
 @pytest.mark.timeout(15)
 def test_affine_transform_large_input_small_output_cpu():
     """
     Make sure input array does not need to be computed entirely
     """
 
     # fully computed, this array would occupy 8TB
```

### Comparing `dask-image-2023.8.1/tests/test_dask_image/test_ndinterp/test_spline_filter.py` & `dask_image-2024.5.0rc1/tests/test_dask_image/test_ndinterp/test_spline_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
     axis_size,
     interp_order,
     interp_mode,
     chunksize,
     axis,
 ):
     if axis == 1 and n < 2:
-        pytest.skip(msg="skip axis=1 for 1d signals")
+        pytest.skip("skip axis=1 for 1d signals")
 
     validate_spline_filter(
         n=n,
         axis_size=axis_size,
         interp_order=interp_order,
         interp_mode=interp_mode,
         chunksize=chunksize,
```

### Comparing `dask-image-2023.8.1/tests/test_dask_image/test_ndmeasure/test__utils.py` & `dask_image-2024.5.0rc1/tests/test_dask_image/test_ndmeasure/test__utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,16 +51,14 @@
     da.utils.assert_eq(d_n, d)
     da.utils.assert_eq(d_lbls_n, d_lbls)
     da.utils.assert_eq(ind_n, np.array(1, dtype=int))
 
 
 @pytest.mark.parametrize(
     "shape, chunks, ind", [
-        ((15, 16), (4, 5), 1),
-        ((15, 16), (4, 5), [1]),
         ((15, 16), (4, 5), [[1, 2, 3, 4]]),
         ((15, 16), (4, 5), [[1, 2], [3, 4]]),
         ((15, 16), (4, 5), [[[1], [2], [3], [4]]]),
     ]
 )
 def test__norm_input_labels_index_warn(shape, chunks, ind):
     a = np.random.random(shape)
@@ -74,15 +72,15 @@
         (a < 0.0625).astype(lbls.dtype)
     )
     d_lbls = da.from_array(lbls, chunks=d.chunks)
 
     ind = np.array(ind)
     d_ind = da.from_array(ind, chunks=1)
 
-    with pytest.warns(None) as w:
+    with pytest.warns(FutureWarning) as w:
         dask_image.ndmeasure._utils._norm_input_labels_index(
             d, d_lbls, d_ind
         )
 
     if ind.ndim > 1:
         assert len(w) == 1
         w.pop(FutureWarning)
```

### Comparing `dask-image-2023.8.1/tests/test_dask_image/test_ndmeasure/test_find_objects.py` & `dask_image-2024.5.0rc1/tests/test_dask_image/test_ndmeasure/test_find_objects.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/tests/test_dask_image/test_ndmorph/test__utils.py` & `dask_image-2024.5.0rc1/tests/test_dask_image/test_ndmorph/test__utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 def test__get_iterations(expected, iterations):
     assert expected == _utils._get_iterations(iterations)
 
 
 @pytest.mark.parametrize(
     "expected, a",
     [
-        (np.bool8, False),
+        (np.bool_, False),
         (np.int_, 2),
         (np.float64, 3.1),
         (np.complex128, 1 + 2j),
         (np.int16, np.int16(6)),
         (np.uint32, np.arange(3, dtype=np.uint32)),
     ]
 )
@@ -146,20 +146,20 @@
     [
         (True, da.arange(2, dtype=bool, chunks=(2,)), None),
         (True, da.arange(2, dtype=bool, chunks=(2,)), True),
         (False, da.arange(2, dtype=bool, chunks=(2,)), False),
         (
             True,
             da.arange(2, dtype=bool, chunks=(2,)),
-            np.bool8(True)
+            np.bool_(True)
         ),
         (
             False,
             da.arange(2, dtype=bool, chunks=(2,)),
-            np.bool8(False)
+            np.bool_(False)
         ),
         (
             np.arange(2, dtype=bool),
             da.arange(2, dtype=bool, chunks=(2,)),
             np.arange(2, dtype=bool)
         ),
         (
```

### Comparing `dask-image-2023.8.1/tests/test_dask_image/test_ndmorph/test_cupy_ndmorph.py` & `dask_image-2024.5.0rc1/tests/test_dask_image/test_ndmorph/test_cupy_ndmorph.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.8.1/tests/test_dask_image/test_ndmorph/test_ndmorph.py` & `dask_image-2024.5.0rc1/tests/test_dask_image/test_ndmorph/test_ndmorph.py`

 * *Files identical despite different names*

