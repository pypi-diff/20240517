# Comparing `tmp/gocept.pytestlayer-8.1.tar.gz` & `tmp/gocept.pytestlayer-8.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gocept.pytestlayer-8.1.tar", last modified: Mon Sep  5 09:17:18 2022, max compression
+gzip compressed data, was "gocept.pytestlayer-8.1.1.tar", last modified: Fri May 17 06:37:51 2024, max compression
```

## Comparing `gocept.pytestlayer-8.1.tar` & `gocept.pytestlayer-8.1.1.tar`

### file list

```diff
@@ -1,124 +1,28 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-05 09:17:18.421800 gocept.pytestlayer-8.1/
--rw-r--r--   0 mac        (513) staff       (20)      124 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/.coveragerc
--rw-r--r--   0 mac        (513) staff       (20)     1704 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/.pre-commit-config.yaml
--rw-r--r--   0 mac        (513) staff       (20)     2796 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      454 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)      499 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/HACKING.rst
--rw-r--r--   0 mac        (513) staff       (20)     2070 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      230 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)     8251 2022-09-05 09:17:18.421933 gocept.pytestlayer-8.1/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     3341 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      825 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/buildout.cfg
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-05 09:17:18.395632 gocept.pytestlayer-8.1/doc/
--rw-r--r--   0 mac        (513) staff       (20)      100 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/doc/about.rst
--rw-r--r--   0 mac        (513) staff       (20)      110 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/doc/api.rst
--rw-r--r--   0 mac        (513) staff       (20)       28 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/doc/changes.rst
--rw-r--r--   0 mac        (513) staff       (20)      222 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/doc/conf.py
--rw-r--r--   0 mac        (513) staff       (20)      109 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/doc/index.rst
--rw-r--r--   0 mac        (513) staff       (20)      514 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/pytest.ini
--rw-r--r--   0 mac        (513) staff       (20)      213 2022-09-05 09:17:18.422656 gocept.pytestlayer-8.1/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     2145 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-05 09:17:18.385033 gocept.pytestlayer-8.1/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-05 09:17:18.395934 gocept.pytestlayer-8.1/src/gocept/
--rw-r--r--   0 mac        (513) staff       (20)       56 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-05 09:17:18.400997 gocept.pytestlayer-8.1/src/gocept/pytestlayer/
--rw-r--r--   0 mac        (513) staff       (20)        0 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      509 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/_compat.py
--rw-r--r--   0 mac        (513) staff       (20)      624 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/doctest.py
--rw-r--r--   0 mac        (513) staff       (20)     6573 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/fixture.py
--rw-r--r--   0 mac        (513) staff       (20)     3190 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/layered.py
--rw-r--r--   0 mac        (513) staff       (20)     3579 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/plugin.py
--rw-r--r--   0 mac        (513) staff       (20)      244 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/testing.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-05 09:17:18.403065 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/
--rw-r--r--   0 mac        (513) staff       (20)        0 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      102 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/conftest.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-05 09:17:18.389668 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-05 09:17:18.404008 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/bad_layer/
--rw-r--r--   0 mac        (513) staff       (20)        0 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/bad_layer/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)       33 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/bad_layer/conftest.py
--rw-r--r--   0 mac        (513) staff       (20)      186 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/bad_layer/test_core.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-05 09:17:18.404977 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/custom_fixture_name/
--rw-r--r--   0 mac        (513) staff       (20)        0 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/custom_fixture_name/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      270 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/custom_fixture_name/conftest.py
--rw-r--r--   0 mac        (513) staff       (20)      895 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/custom_fixture_name/test_core.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-05 09:17:18.405871 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/keep_layer_across_test_classes/
--rw-r--r--   0 mac        (513) staff       (20)        0 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/keep_layer_across_test_classes/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)       33 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/keep_layer_across_test_classes/conftest.py
--rw-r--r--   0 mac        (513) staff       (20)     2521 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/keep_layer_across_test_classes/test_core.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-05 09:17:18.406930 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/layers_with_same_name/
--rw-r--r--   0 mac        (513) staff       (20)        0 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/layers_with_same_name/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)       33 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/layers_with_same_name/conftest.py
--rw-r--r--   0 mac        (513) staff       (20)      741 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/layers_with_same_name/test_core.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-05 09:17:18.407969 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/no_setup_or_teardown/
--rw-r--r--   0 mac        (513) staff       (20)        0 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/no_setup_or_teardown/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)       33 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/no_setup_or_teardown/conftest.py
--rw-r--r--   0 mac        (513) staff       (20)      253 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/no_setup_or_teardown/test_core.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-05 09:17:18.408904 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/order_by_layer/
--rw-r--r--   0 mac        (513) staff       (20)        0 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/order_by_layer/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)       33 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/order_by_layer/conftest.py
--rw-r--r--   0 mac        (513) staff       (20)     2842 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/order_by_layer/test_core.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-05 09:17:18.410509 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/order_with_layered_suite/
--rw-r--r--   0 mac        (513) staff       (20)        0 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/order_with_layered_suite/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)       33 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/order_with_layered_suite/conftest.py
--rw-r--r--   0 mac        (513) staff       (20)      281 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/order_with_layered_suite/foo.txt
--rw-r--r--   0 mac        (513) staff       (20)      271 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/order_with_layered_suite/foobar.txt
--rw-r--r--   0 mac        (513) staff       (20)     3411 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/order_with_layered_suite/test_core.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-05 09:17:18.411470 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/session_fixture/
--rw-r--r--   0 mac        (513) staff       (20)        0 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/session_fixture/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      312 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/session_fixture/conftest.py
--rw-r--r--   0 mac        (513) staff       (20)      867 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/session_fixture/test_core.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-05 09:17:18.412724 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/shared_with_layered_suite/
--rw-r--r--   0 mac        (513) staff       (20)        0 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/shared_with_layered_suite/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)       32 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/shared_with_layered_suite/conftest.py
--rw-r--r--   0 mac        (513) staff       (20)      191 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/shared_with_layered_suite/mydoctest.txt
--rw-r--r--   0 mac        (513) staff       (20)     1108 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/shared_with_layered_suite/test_core.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-05 09:17:18.413727 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/single_layer/
--rw-r--r--   0 mac        (513) staff       (20)        0 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/single_layer/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)       33 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/single_layer/conftest.py
--rw-r--r--   0 mac        (513) staff       (20)      712 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/single_layer/test_core.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-05 09:17:18.415094 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/single_layer_in_two_modules/
--rw-r--r--   0 mac        (513) staff       (20)        0 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/single_layer_in_two_modules/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)       33 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/single_layer_in_two_modules/conftest.py
--rw-r--r--   0 mac        (513) staff       (20)      712 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/single_layer_in_two_modules/test_core.py
--rw-r--r--   0 mac        (513) staff       (20)      251 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/single_layer_in_two_modules/test_second_module.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-05 09:17:18.416049 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/single_layer_with_unattached_base_layer/
--rw-r--r--   0 mac        (513) staff       (20)        0 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/single_layer_with_unattached_base_layer/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)       33 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/single_layer_with_unattached_base_layer/conftest.py
--rw-r--r--   0 mac        (513) staff       (20)     1152 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/single_layer_with_unattached_base_layer/test_core.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-05 09:17:18.417350 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/single_layered_suite/
--rw-r--r--   0 mac        (513) staff       (20)        0 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/single_layered_suite/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)       33 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/single_layered_suite/conftest.py
--rw-r--r--   0 mac        (513) staff       (20)      186 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/single_layered_suite/doctest.txt
--rw-r--r--   0 mac        (513) staff       (20)      903 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/single_layered_suite/test_core.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-05 09:17:18.419032 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/two_dependent_layered_suites/
--rw-r--r--   0 mac        (513) staff       (20)        0 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/two_dependent_layered_suites/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      272 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/two_dependent_layered_suites/bar.txt
--rw-r--r--   0 mac        (513) staff       (20)       33 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/two_dependent_layered_suites/conftest.py
--rw-r--r--   0 mac        (513) staff       (20)      285 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/two_dependent_layered_suites/foo.txt
--rw-r--r--   0 mac        (513) staff       (20)     1512 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/two_dependent_layered_suites/test_core.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-05 09:17:18.419909 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/two_dependent_layers/
--rw-r--r--   0 mac        (513) staff       (20)        0 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/two_dependent_layers/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)       33 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/two_dependent_layers/conftest.py
--rw-r--r--   0 mac        (513) staff       (20)     1590 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/two_dependent_layers/test_core.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-05 09:17:18.420748 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/two_independent_layers/
--rw-r--r--   0 mac        (513) staff       (20)        0 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/two_independent_layers/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)       33 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/two_independent_layers/conftest.py
--rw-r--r--   0 mac        (513) staff       (20)     1587 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/two_independent_layers/test_core.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-05 09:17:18.421590 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/with_and_without_layer/
--rw-r--r--   0 mac        (513) staff       (20)        0 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/with_and_without_layer/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)       33 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/with_and_without_layer/conftest.py
--rw-r--r--   0 mac        (513) staff       (20)      825 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/fixture/with_and_without_layer/test_core.py
--rw-r--r--   0 mac        (513) staff       (20)      322 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/test_doctest.py
--rw-r--r--   0 mac        (513) staff       (20)      567 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/test_fixture.py
--rw-r--r--   0 mac        (513) staff       (20)    25532 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/test_integration.py
--rw-r--r--   0 mac        (513) staff       (20)      274 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/src/gocept/pytestlayer/tests/test_layer.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-05 09:17:18.398690 gocept.pytestlayer-8.1/src/gocept.pytestlayer.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)     8251 2022-09-05 09:17:17.000000 gocept.pytestlayer-8.1/src/gocept.pytestlayer.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     5323 2022-09-05 09:17:18.000000 gocept.pytestlayer-8.1/src/gocept.pytestlayer.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-09-05 09:17:17.000000 gocept.pytestlayer-8.1/src/gocept.pytestlayer.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)       49 2022-09-05 09:17:18.000000 gocept.pytestlayer-8.1/src/gocept.pytestlayer.egg-info/entry_points.txt
--rw-r--r--   0 mac        (513) staff       (20)        7 2022-09-05 09:17:18.000000 gocept.pytestlayer-8.1/src/gocept.pytestlayer.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-09-05 09:17:17.000000 gocept.pytestlayer-8.1/src/gocept.pytestlayer.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)       61 2022-09-05 09:17:18.000000 gocept.pytestlayer-8.1/src/gocept.pytestlayer.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        7 2022-09-05 09:17:18.000000 gocept.pytestlayer-8.1/src/gocept.pytestlayer.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)      391 2022-09-05 09:17:16.000000 gocept.pytestlayer-8.1/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-17 06:37:51.146222 gocept.pytestlayer-8.1.1/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      131 2024-05-17 06:37:50.000000 gocept.pytestlayer-8.1.1/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      454 2024-05-17 06:37:50.000000 gocept.pytestlayer-8.1.1/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2024-05-17 06:37:50.000000 gocept.pytestlayer-8.1.1/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      230 2024-05-17 06:37:50.000000 gocept.pytestlayer-8.1.1/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1932 2024-05-17 06:37:51.146015 gocept.pytestlayer-8.1.1/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      188 2024-05-17 06:37:50.000000 gocept.pytestlayer-8.1.1/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       38 2024-05-17 06:37:51.146271 gocept.pytestlayer-8.1.1/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1932 2024-05-17 06:37:50.000000 gocept.pytestlayer-8.1.1/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-17 06:37:51.142413 gocept.pytestlayer-8.1.1/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-17 06:37:51.143505 gocept.pytestlayer-8.1.1/src/gocept/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       56 2024-05-17 06:37:50.000000 gocept.pytestlayer-8.1.1/src/gocept/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-17 06:37:51.145560 gocept.pytestlayer-8.1.1/src/gocept/pytestlayer/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      179 2024-05-17 06:37:50.000000 gocept.pytestlayer-8.1.1/src/gocept/pytestlayer/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      179 2024-05-17 06:37:50.000000 gocept.pytestlayer-8.1.1/src/gocept/pytestlayer/doctest.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      179 2024-05-17 06:37:50.000000 gocept.pytestlayer-8.1.1/src/gocept/pytestlayer/fixture.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      179 2024-05-17 06:37:50.000000 gocept.pytestlayer-8.1.1/src/gocept/pytestlayer/layered.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      179 2024-05-17 06:37:50.000000 gocept.pytestlayer-8.1.1/src/gocept/pytestlayer/plugin.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      179 2024-05-17 06:37:50.000000 gocept.pytestlayer-8.1.1/src/gocept/pytestlayer/testing.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-17 06:37:51.145783 gocept.pytestlayer-8.1.1/src/gocept.pytestlayer.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1932 2024-05-17 06:37:51.000000 gocept.pytestlayer-8.1.1/src/gocept.pytestlayer.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      674 2024-05-17 06:37:51.000000 gocept.pytestlayer-8.1.1/src/gocept.pytestlayer.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-05-17 06:37:51.000000 gocept.pytestlayer-8.1.1/src/gocept.pytestlayer.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       49 2024-05-17 06:37:51.000000 gocept.pytestlayer-8.1.1/src/gocept.pytestlayer.egg-info/entry_points.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        7 2024-05-17 06:37:51.000000 gocept.pytestlayer-8.1.1/src/gocept.pytestlayer.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-05-17 06:37:51.000000 gocept.pytestlayer-8.1.1/src/gocept.pytestlayer.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)       11 2024-05-17 06:37:51.000000 gocept.pytestlayer-8.1.1/src/gocept.pytestlayer.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        7 2024-05-17 06:37:51.000000 gocept.pytestlayer-8.1.1/src/gocept.pytestlayer.egg-info/top_level.txt
```

### Comparing `gocept.pytestlayer-8.1/LICENSE.txt` & `gocept.pytestlayer-8.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gocept.pytestlayer-8.1/setup.py` & `gocept.pytestlayer-8.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,79 +1,64 @@
 """Integration of zope.testrunner-style test layers into pytest framework"""
 
 from setuptools import find_packages
 from setuptools import setup
 
-
 setup(
     name='gocept.pytestlayer',
-    version='8.1',
-
+    version='8.1.1',
     python_requires=', '.join([
         '>=3.7',
     ]),
     install_requires=[
-        'pytest >= 6.0',
         'setuptools',
-        'zope.dottedname',
     ],
-
-    extras_require={
-        'test': [
-            'plone.testing',
-        ],
-    },
-
+    extras_require={},
     entry_points={
-        'console_scripts': [
-            # 'binary-name = gocept.pytestlayer.module:function'
-        ],
         'pytest11': [
             'zopelayer = gocept.pytestlayer.plugin',
         ],
     },
-
     author='gocept <mail@gocept.com>',
     author_email='mail@gocept.com',
     license='ZPL 2.1',
     url='https://github.com/gocept/gocept.pytestlayer/',
-
     keywords='pytest zope.testrunner layer fixture',
     classifiers="""\
-Development Status :: 4 - Beta
+Development Status :: 7 - Inactive
 Environment :: Console
 Framework :: Pytest
 Framework :: Plone
-Framework :: Zope2
-Framework :: Zope3
+Framework :: Zope :: 3
+Framework :: Zope :: 5
 Intended Audience :: Developers
 License :: OSI Approved
 License :: OSI Approved :: Zope Public License
 Natural Language :: English
 Operating System :: OS Independent
 Programming Language :: Python
 Programming Language :: Python :: 3
-Programming Language :: Python :: 3.6
 Programming Language :: Python :: 3.7
 Programming Language :: Python :: 3.8
 Programming Language :: Python :: 3.9
 Programming Language :: Python :: 3.10
+Programming Language :: Python :: 3.11
 Programming Language :: Python :: Implementation
 Programming Language :: Python :: Implementation :: CPython
 Programming Language :: Python :: Implementation :: PyPy
 Topic :: Software Development
 Topic :: Software Development :: Libraries
 Topic :: Software Development :: Libraries :: Python Modules
 Topic :: Software Development :: Testing
 """[:-1].split('\n'),
     description=__doc__.strip(),
-    long_description='\n\n'.join(open(name).read() for name in (
-        'README.rst',
-        'HACKING.rst',
-        'CHANGES.rst',
-    )),
+    long_description='\n\n'.join(
+        open(name).read() for name in (
+            'README.rst',
+            'CHANGES.rst',
+        )),
     namespace_packages=['gocept'],
     packages=find_packages('src'),
     package_dir={'': 'src'},
     include_package_data=True,
     zip_safe=False,
 )
```

