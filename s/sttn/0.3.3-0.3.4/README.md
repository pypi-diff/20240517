# Comparing `tmp/sttn-0.3.3.tar.gz` & `tmp/sttn-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/user/PycharmProjects/sttn/dist/.tmp-gjw21ore/sttn-0.3.3.tar", last modified: Mon Apr 22 05:18:26 2024, max compression
+gzip compressed data, was "/Users/user/PycharmProjects/sttn/dist/.tmp-v5xhqui3/sttn-0.3.4.tar", last modified: Fri May 17 05:15:04 2024, max compression
```

## Comparing `sttn-0.3.3.tar` & `sttn-0.3.4.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-22 05:18:26.657951 sttn-0.3.3/
--rw-r--r--   0 user       (501) staff       (20)      587 2020-12-07 04:18:16.000000 sttn-0.3.3/.coveragerc
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-22 05:18:26.623424 sttn-0.3.3/.github/
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-22 05:18:26.629388 sttn-0.3.3/.github/workflows/
--rw-r--r--   0 user       (501) staff       (20)      777 2024-02-02 03:00:25.000000 sttn-0.3.3/.github/workflows/python-package-conda.yml
--rw-r--r--   0 user       (501) staff       (20)     1911 2022-02-18 03:29:24.000000 sttn-0.3.3/.gitignore
--rw-r--r--   0 user       (501) staff       (20)      461 2021-08-01 05:26:59.000000 sttn-0.3.3/.readthedocs.yml
--rw-r--r--   0 user       (501) staff       (20)       71 2020-12-07 04:12:52.000000 sttn-0.3.3/AUTHORS.rst
--rw-r--r--   0 user       (501) staff       (20)      128 2020-12-07 04:12:52.000000 sttn-0.3.3/CHANGELOG.rst
--rw-r--r--   0 user       (501) staff       (20)    35149 2020-12-07 04:12:52.000000 sttn-0.3.3/LICENSE.txt
--rw-r--r--   0 user       (501) staff       (20)     3464 2024-04-22 05:18:26.657878 sttn-0.3.3/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      545 2024-02-27 07:09:50.000000 sttn-0.3.3/Pipfile
--rw-r--r--   0 user       (501) staff       (20)   291759 2024-02-27 07:13:45.000000 sttn-0.3.3/Pipfile.lock
--rw-r--r--   0 user       (501) staff       (20)     2505 2024-02-02 06:40:18.000000 sttn-0.3.3/README.rst
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-22 05:18:26.631330 sttn-0.3.3/docs/
--rw-r--r--   0 user       (501) staff       (20)     1153 2021-08-01 05:26:59.000000 sttn-0.3.3/docs/Makefile
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-22 05:18:26.631485 sttn-0.3.3/docs/_static/
--rw-r--r--   0 user       (501) staff       (20)       18 2021-08-01 05:26:59.000000 sttn-0.3.3/docs/_static/.gitignore
--rw-r--r--   0 user       (501) staff       (20)       41 2021-08-01 05:26:59.000000 sttn-0.3.3/docs/authors.rst
--rw-r--r--   0 user       (501) staff       (20)       43 2021-08-01 05:26:59.000000 sttn-0.3.3/docs/changelog.rst
--rw-r--r--   0 user       (501) staff       (20)     9459 2021-08-01 05:26:59.000000 sttn-0.3.3/docs/conf.py
--rw-r--r--   0 user       (501) staff       (20)     2215 2020-12-07 04:18:44.000000 sttn-0.3.3/docs/index.rst
--rw-r--r--   0 user       (501) staff       (20)       67 2021-08-01 05:26:59.000000 sttn-0.3.3/docs/license.rst
--rw-r--r--   0 user       (501) staff       (20)       39 2021-08-01 05:26:59.000000 sttn-0.3.3/docs/readme.rst
--rw-r--r--   0 user       (501) staff       (20)      233 2021-08-01 05:26:59.000000 sttn-0.3.3/docs/requirements.txt
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-22 05:18:26.641408 sttn-0.3.3/notebooks/
--rw-r--r--   0 user       (501) staff       (20)       83 2022-06-12 11:54:34.000000 sttn-0.3.3/notebooks/.gitignore
--rwxr-xr-x   0 user       (501) staff       (20)   414258 2022-02-18 03:29:24.000000 sttn-0.3.3/notebooks/LEHD Origin-Destination employment data.ipynb
--rw-r--r--   0 user       (501) staff       (20)     2827 2023-05-06 17:49:33.000000 sttn-0.3.3/notebooks/LEHD data.ipynb
--rwxr-xr-x   0 user       (501) staff       (20)    20326 2022-02-18 03:29:24.000000 sttn-0.3.3/notebooks/all_gravity_models.ipynb
--rw-r--r--   0 user       (501) staff       (20)    15348 2022-02-18 03:29:24.000000 sttn-0.3.3/notebooks/checkFlow.ipynb
--rwxr-xr-x   0 user       (501) staff       (20)  1402047 2022-02-18 03:29:24.000000 sttn-0.3.3/notebooks/doubly_constrained_general_gravity_linear_DK.ipynb
--rwxr-xr-x   0 user       (501) staff       (20)    26545 2022-02-18 03:29:24.000000 sttn-0.3.3/notebooks/doubly_constrained_gravity_model.ipynb
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-22 05:18:26.643081 sttn-0.3.3/notebooks/img/
--rw-r--r--   0 user       (501) staff       (20)    24266 2021-08-10 04:54:34.000000 sttn-0.3.3/notebooks/img/agg_adjacent_edges.png
--rw-r--r--   0 user       (501) staff       (20)    49043 2021-08-10 04:54:34.000000 sttn-0.3.3/notebooks/img/agg_parallel_edges.png
--rw-r--r--   0 user       (501) staff       (20)    15111 2021-08-10 04:54:34.000000 sttn-0.3.3/notebooks/img/group_nodes.png
--rw-r--r--   0 user       (501) staff       (20)    71234 2021-08-10 04:54:34.000000 sttn-0.3.3/notebooks/img/manhattan_taxi_zones.png
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-22 05:18:26.643317 sttn-0.3.3/notebooks/means of transportation/
--rw-r--r--   0 user       (501) staff       (20)      841 2022-06-12 11:54:34.000000 sttn-0.3.3/notebooks/means of transportation/NYC.csv
--rwxr-xr-x   0 user       (501) staff       (20)   273130 2022-02-18 03:29:24.000000 sttn-0.3.3/notebooks/nyc_311_requests.ipynb
--rwxr-xr-x   0 user       (501) staff       (20)   679766 2022-02-18 03:29:24.000000 sttn-0.3.3/notebooks/nyc_taxi_demo.ipynb
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-22 05:18:26.643473 sttn-0.3.3/notebooks/papers/
--rw-r--r--   0 user       (501) staff       (20)    58560 2021-12-09 05:29:14.000000 sttn-0.3.3/notebooks/papers/YSC 2021.ipynb
--rwxr-xr-x   0 user       (501) staff       (20)   150447 2022-02-18 03:29:24.000000 sttn-0.3.3/notebooks/piecewise_gravity_model.ipynb
--rwxr-xr-x   0 user       (501) staff       (20)    14966 2022-02-18 03:29:24.000000 sttn-0.3.3/notebooks/unconstrained_gravity_models.ipynb
--rw-r--r--   0 user       (501) staff       (20)      197 2021-08-01 05:26:59.000000 sttn-0.3.3/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)     1399 2024-04-22 05:18:26.658567 sttn-0.3.3/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      701 2021-08-01 23:43:48.000000 sttn-0.3.3/setup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-22 05:18:26.643698 sttn-0.3.3/src/
--rw-r--r--   0 user       (501) staff       (20)        0 2022-09-25 21:08:59.000000 sttn-0.3.3/src/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-22 05:18:26.645054 sttn-0.3.3/src/sttn/
--rw-r--r--   0 user       (501) staff       (20)      595 2022-10-21 04:47:07.000000 sttn-0.3.3/src/sttn/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-22 05:18:26.646088 sttn-0.3.3/src/sttn/algorithms/
--rw-r--r--   0 user       (501) staff       (20)       38 2023-02-13 02:11:14.000000 sttn-0.3.3/src/sttn/algorithms/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-22 05:18:26.646398 sttn-0.3.3/src/sttn/algorithms/community/
--rw-r--r--   0 user       (501) staff       (20)      106 2023-02-13 02:15:00.000000 sttn-0.3.3/src/sttn/algorithms/community/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      524 2024-03-21 06:03:57.000000 sttn-0.3.3/src/sttn/algorithms/community/detection.py
--rw-r--r--   0 user       (501) staff       (20)       76 2021-11-21 06:37:38.000000 sttn-0.3.3/src/sttn/constants.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-22 05:18:26.650079 sttn-0.3.3/src/sttn/data/
--rw-r--r--   0 user       (501) staff       (20)        0 2020-12-18 05:49:30.000000 sttn-0.3.3/src/sttn/data/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     5696 2024-04-11 05:53:37.000000 sttn-0.3.3/src/sttn/data/brno.py
--rw-r--r--   0 user       (501) staff       (20)      771 2021-01-17 23:59:47.000000 sttn-0.3.3/src/sttn/data/census.py
--rw-r--r--   0 user       (501) staff       (20)     1074 2020-12-19 21:19:18.000000 sttn-0.3.3/src/sttn/data/data_provider.py
--rw-r--r--   0 user       (501) staff       (20)     5340 2024-04-04 13:04:03.000000 sttn-0.3.3/src/sttn/data/lehd.py
--rw-r--r--   0 user       (501) staff       (20)     7030 2024-04-05 14:29:18.000000 sttn-0.3.3/src/sttn/data/nyc.py
--rw-r--r--   0 user       (501) staff       (20)      430 2024-01-11 12:31:37.000000 sttn-0.3.3/src/sttn/io.py
--rw-r--r--   0 user       (501) staff       (20)     7114 2024-01-11 12:31:17.000000 sttn-0.3.3/src/sttn/network.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-22 05:18:26.652289 sttn-0.3.3/src/sttn/nli/
--rw-r--r--   0 user       (501) staff       (20)       25 2024-01-04 09:05:00.000000 sttn-0.3.3/src/sttn/nli/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3986 2024-04-22 04:53:34.000000 sttn-0.3.3/src/sttn/nli/analyst.py
--rw-r--r--   0 user       (501) staff       (20)     2136 2024-04-22 05:06:11.000000 sttn-0.3.3/src/sttn/nli/data.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-22 05:18:26.652638 sttn-0.3.3/src/sttn/nli/models/
--rw-r--r--   0 user       (501) staff       (20)        0 2024-02-27 06:27:45.000000 sttn-0.3.3/src/sttn/nli/models/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      939 2024-03-04 05:44:58.000000 sttn-0.3.3/src/sttn/nli/models/output.py
--rw-r--r--   0 user       (501) staff       (20)     5731 2024-04-19 05:27:53.000000 sttn-0.3.3/src/sttn/nli/prompts.py
--rw-r--r--   0 user       (501) staff       (20)      147 2024-01-11 12:33:21.000000 sttn-0.3.3/src/sttn/nli/query.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-22 05:18:26.654411 sttn-0.3.3/src/sttn/nli/templates/
--rw-r--r--   0 user       (501) staff       (20)      267 2024-03-29 06:56:07.000000 sttn-0.3.3/src/sttn/nli/templates/code_execution_error.j2
--rw-r--r--   0 user       (501) staff       (20)      903 2024-04-04 05:16:09.000000 sttn-0.3.3/src/sttn/nli/templates/data_analysis.j2
--rw-r--r--   0 user       (501) staff       (20)     2110 2024-04-22 05:07:11.000000 sttn-0.3.3/src/sttn/nli/templates/data_filter.j2
--rw-r--r--   0 user       (501) staff       (20)      540 2024-03-04 05:20:36.000000 sttn-0.3.3/src/sttn/nli/templates/data_provider.j2
--rw-r--r--   0 user       (501) staff       (20)      562 2024-03-04 05:22:59.000000 sttn-0.3.3/src/sttn/nli/templates/data_provider_arguments.j2
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-22 05:18:26.654922 sttn-0.3.3/src/sttn/plot/
--rw-r--r--   0 user       (501) staff       (20)       19 2022-09-25 21:46:22.000000 sttn-0.3.3/src/sttn/plot/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     3930 2024-01-11 12:33:45.000000 sttn-0.3.3/src/sttn/plot/api.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-22 05:18:26.655855 sttn-0.3.3/src/sttn/plot/keplergl/
--rw-r--r--   0 user       (501) staff       (20)        0 2022-09-17 23:00:44.000000 sttn-0.3.3/src/sttn/plot/keplergl/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1639 2024-01-11 12:33:54.000000 sttn-0.3.3/src/sttn/plot/keplergl/filter.py
--rw-r--r--   0 user       (501) staff       (20)     6344 2024-03-21 05:51:59.000000 sttn-0.3.3/src/sttn/plot/keplergl/layer.py
--rw-r--r--   0 user       (501) staff       (20)     2143 2024-01-11 12:34:01.000000 sttn-0.3.3/src/sttn/plot/keplergl/map.py
--rw-r--r--   0 user       (501) staff       (20)     2787 2020-12-07 04:18:24.000000 sttn-0.3.3/src/sttn/skeleton.py
--rw-r--r--   0 user       (501) staff       (20)     1860 2024-01-11 12:33:03.000000 sttn-0.3.3/src/sttn/utils.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-22 05:18:26.657207 sttn-0.3.3/src/sttn.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     3464 2024-04-22 05:18:26.000000 sttn-0.3.3/src/sttn.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     2254 2024-04-22 05:18:26.000000 sttn-0.3.3/src/sttn.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2024-04-22 05:18:26.000000 sttn-0.3.3/src/sttn.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2020-12-07 05:04:43.000000 sttn-0.3.3/src/sttn.egg-info/not-zip-safe
--rw-r--r--   0 user       (501) staff       (20)      150 2024-04-22 05:18:26.000000 sttn-0.3.3/src/sttn.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)        5 2024-04-22 05:18:26.000000 sttn-0.3.3/src/sttn.egg-info/top_level.txt
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-22 05:18:26.656991 sttn-0.3.3/tests/
--rw-r--r--   0 user       (501) staff       (20)      225 2020-12-07 04:16:52.000000 sttn-0.3.3/tests/conftest.py
--rw-r--r--   0 user       (501) staff       (20)     1684 2021-03-28 22:51:50.000000 sttn-0.3.3/tests/test_network_constructor.py
--rw-r--r--   0 user       (501) staff       (20)     2349 2021-03-29 03:32:01.000000 sttn-0.3.3/tests/test_network_operations.py
--rw-r--r--   0 user       (501) staff       (20)      304 2020-12-07 04:18:55.000000 sttn-0.3.3/tests/test_skeleton.py
--rw-r--r--   0 user       (501) staff       (20)     2010 2021-08-01 05:26:59.000000 sttn-0.3.3/tox.ini
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-17 05:15:04.062290 sttn-0.3.4/
+-rw-r--r--   0 user       (501) staff       (20)      587 2020-12-07 04:18:16.000000 sttn-0.3.4/.coveragerc
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-17 05:15:04.025547 sttn-0.3.4/.github/
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-17 05:15:04.032070 sttn-0.3.4/.github/workflows/
+-rw-r--r--   0 user       (501) staff       (20)      777 2024-02-02 03:00:25.000000 sttn-0.3.4/.github/workflows/python-package-conda.yml
+-rw-r--r--   0 user       (501) staff       (20)     1911 2022-02-18 03:29:24.000000 sttn-0.3.4/.gitignore
+-rw-r--r--   0 user       (501) staff       (20)      461 2021-08-01 05:26:59.000000 sttn-0.3.4/.readthedocs.yml
+-rw-r--r--   0 user       (501) staff       (20)       71 2020-12-07 04:12:52.000000 sttn-0.3.4/AUTHORS.rst
+-rw-r--r--   0 user       (501) staff       (20)      128 2020-12-07 04:12:52.000000 sttn-0.3.4/CHANGELOG.rst
+-rw-r--r--   0 user       (501) staff       (20)    35149 2020-12-07 04:12:52.000000 sttn-0.3.4/LICENSE.txt
+-rw-r--r--   0 user       (501) staff       (20)     3464 2024-05-17 05:15:04.062214 sttn-0.3.4/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      545 2024-02-27 07:09:50.000000 sttn-0.3.4/Pipfile
+-rw-r--r--   0 user       (501) staff       (20)   291759 2024-02-27 07:13:45.000000 sttn-0.3.4/Pipfile.lock
+-rw-r--r--   0 user       (501) staff       (20)     2505 2024-02-02 06:40:18.000000 sttn-0.3.4/README.rst
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-17 05:15:04.033858 sttn-0.3.4/docs/
+-rw-r--r--   0 user       (501) staff       (20)     1153 2021-08-01 05:26:59.000000 sttn-0.3.4/docs/Makefile
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-17 05:15:04.034029 sttn-0.3.4/docs/_static/
+-rw-r--r--   0 user       (501) staff       (20)       18 2021-08-01 05:26:59.000000 sttn-0.3.4/docs/_static/.gitignore
+-rw-r--r--   0 user       (501) staff       (20)       41 2021-08-01 05:26:59.000000 sttn-0.3.4/docs/authors.rst
+-rw-r--r--   0 user       (501) staff       (20)       43 2021-08-01 05:26:59.000000 sttn-0.3.4/docs/changelog.rst
+-rw-r--r--   0 user       (501) staff       (20)     9459 2021-08-01 05:26:59.000000 sttn-0.3.4/docs/conf.py
+-rw-r--r--   0 user       (501) staff       (20)     2215 2020-12-07 04:18:44.000000 sttn-0.3.4/docs/index.rst
+-rw-r--r--   0 user       (501) staff       (20)       67 2021-08-01 05:26:59.000000 sttn-0.3.4/docs/license.rst
+-rw-r--r--   0 user       (501) staff       (20)       39 2021-08-01 05:26:59.000000 sttn-0.3.4/docs/readme.rst
+-rw-r--r--   0 user       (501) staff       (20)      233 2021-08-01 05:26:59.000000 sttn-0.3.4/docs/requirements.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-17 05:15:04.048270 sttn-0.3.4/notebooks/
+-rw-r--r--   0 user       (501) staff       (20)       83 2022-06-12 11:54:34.000000 sttn-0.3.4/notebooks/.gitignore
+-rwxr-xr-x   0 user       (501) staff       (20)   414258 2022-02-18 03:29:24.000000 sttn-0.3.4/notebooks/LEHD Origin-Destination employment data.ipynb
+-rw-r--r--   0 user       (501) staff       (20)     2827 2023-05-06 17:49:33.000000 sttn-0.3.4/notebooks/LEHD data.ipynb
+-rwxr-xr-x   0 user       (501) staff       (20)    20326 2022-02-18 03:29:24.000000 sttn-0.3.4/notebooks/all_gravity_models.ipynb
+-rw-r--r--   0 user       (501) staff       (20)    15348 2022-02-18 03:29:24.000000 sttn-0.3.4/notebooks/checkFlow.ipynb
+-rwxr-xr-x   0 user       (501) staff       (20)  1402047 2022-02-18 03:29:24.000000 sttn-0.3.4/notebooks/doubly_constrained_general_gravity_linear_DK.ipynb
+-rwxr-xr-x   0 user       (501) staff       (20)    26545 2022-02-18 03:29:24.000000 sttn-0.3.4/notebooks/doubly_constrained_gravity_model.ipynb
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-17 05:15:04.050814 sttn-0.3.4/notebooks/img/
+-rw-r--r--   0 user       (501) staff       (20)    24266 2021-08-10 04:54:34.000000 sttn-0.3.4/notebooks/img/agg_adjacent_edges.png
+-rw-r--r--   0 user       (501) staff       (20)    49043 2021-08-10 04:54:34.000000 sttn-0.3.4/notebooks/img/agg_parallel_edges.png
+-rw-r--r--   0 user       (501) staff       (20)    15111 2021-08-10 04:54:34.000000 sttn-0.3.4/notebooks/img/group_nodes.png
+-rw-r--r--   0 user       (501) staff       (20)    71234 2021-08-10 04:54:34.000000 sttn-0.3.4/notebooks/img/manhattan_taxi_zones.png
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-17 05:15:04.051076 sttn-0.3.4/notebooks/means of transportation/
+-rw-r--r--   0 user       (501) staff       (20)      841 2022-06-12 11:54:34.000000 sttn-0.3.4/notebooks/means of transportation/NYC.csv
+-rwxr-xr-x   0 user       (501) staff       (20)   273130 2022-02-18 03:29:24.000000 sttn-0.3.4/notebooks/nyc_311_requests.ipynb
+-rwxr-xr-x   0 user       (501) staff       (20)   679766 2022-02-18 03:29:24.000000 sttn-0.3.4/notebooks/nyc_taxi_demo.ipynb
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-17 05:15:04.051236 sttn-0.3.4/notebooks/papers/
+-rw-r--r--   0 user       (501) staff       (20)    58560 2021-12-09 05:29:14.000000 sttn-0.3.4/notebooks/papers/YSC 2021.ipynb
+-rwxr-xr-x   0 user       (501) staff       (20)   150447 2022-02-18 03:29:24.000000 sttn-0.3.4/notebooks/piecewise_gravity_model.ipynb
+-rwxr-xr-x   0 user       (501) staff       (20)    14966 2022-02-18 03:29:24.000000 sttn-0.3.4/notebooks/unconstrained_gravity_models.ipynb
+-rw-r--r--   0 user       (501) staff       (20)      197 2021-08-01 05:26:59.000000 sttn-0.3.4/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)     1399 2024-05-17 05:15:04.062920 sttn-0.3.4/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      701 2021-08-01 23:43:48.000000 sttn-0.3.4/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-17 05:15:04.051493 sttn-0.3.4/src/
+-rw-r--r--   0 user       (501) staff       (20)        0 2022-09-25 21:08:59.000000 sttn-0.3.4/src/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-17 05:15:04.052730 sttn-0.3.4/src/sttn/
+-rw-r--r--   0 user       (501) staff       (20)      595 2022-10-21 04:47:07.000000 sttn-0.3.4/src/sttn/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-17 05:15:04.053750 sttn-0.3.4/src/sttn/algorithms/
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-02-13 02:11:14.000000 sttn-0.3.4/src/sttn/algorithms/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-17 05:15:04.054061 sttn-0.3.4/src/sttn/algorithms/community/
+-rw-r--r--   0 user       (501) staff       (20)      106 2023-02-13 02:15:00.000000 sttn-0.3.4/src/sttn/algorithms/community/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      524 2024-03-21 06:03:57.000000 sttn-0.3.4/src/sttn/algorithms/community/detection.py
+-rw-r--r--   0 user       (501) staff       (20)       76 2021-11-21 06:37:38.000000 sttn-0.3.4/src/sttn/constants.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-17 05:15:04.055328 sttn-0.3.4/src/sttn/data/
+-rw-r--r--   0 user       (501) staff       (20)        0 2020-12-18 05:49:30.000000 sttn-0.3.4/src/sttn/data/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     7628 2024-05-03 05:18:37.000000 sttn-0.3.4/src/sttn/data/brno.py
+-rw-r--r--   0 user       (501) staff       (20)      771 2021-01-17 23:59:47.000000 sttn-0.3.4/src/sttn/data/census.py
+-rw-r--r--   0 user       (501) staff       (20)     1074 2020-12-19 21:19:18.000000 sttn-0.3.4/src/sttn/data/data_provider.py
+-rw-r--r--   0 user       (501) staff       (20)     5366 2024-05-17 05:03:03.000000 sttn-0.3.4/src/sttn/data/lehd.py
+-rw-r--r--   0 user       (501) staff       (20)    15114 2024-05-17 05:02:11.000000 sttn-0.3.4/src/sttn/data/nyc.py
+-rw-r--r--   0 user       (501) staff       (20)      430 2024-01-11 12:31:37.000000 sttn-0.3.4/src/sttn/io.py
+-rw-r--r--   0 user       (501) staff       (20)     7114 2024-01-11 12:31:17.000000 sttn-0.3.4/src/sttn/network.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-17 05:15:04.056854 sttn-0.3.4/src/sttn/nli/
+-rw-r--r--   0 user       (501) staff       (20)       25 2024-01-04 09:05:00.000000 sttn-0.3.4/src/sttn/nli/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     4047 2024-05-17 04:55:04.000000 sttn-0.3.4/src/sttn/nli/analyst.py
+-rw-r--r--   0 user       (501) staff       (20)     2136 2024-04-22 05:06:11.000000 sttn-0.3.4/src/sttn/nli/data.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-17 05:15:04.057220 sttn-0.3.4/src/sttn/nli/models/
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-02-27 06:27:45.000000 sttn-0.3.4/src/sttn/nli/models/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      939 2024-03-04 05:44:58.000000 sttn-0.3.4/src/sttn/nli/models/output.py
+-rw-r--r--   0 user       (501) staff       (20)     6706 2024-05-17 04:53:45.000000 sttn-0.3.4/src/sttn/nli/prompts.py
+-rw-r--r--   0 user       (501) staff       (20)      147 2024-01-11 12:33:21.000000 sttn-0.3.4/src/sttn/nli/query.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-17 05:15:04.058835 sttn-0.3.4/src/sttn/nli/templates/
+-rw-r--r--   0 user       (501) staff       (20)      267 2024-03-29 06:56:07.000000 sttn-0.3.4/src/sttn/nli/templates/code_execution_error.j2
+-rw-r--r--   0 user       (501) staff       (20)      903 2024-04-04 05:16:09.000000 sttn-0.3.4/src/sttn/nli/templates/data_analysis.j2
+-rw-r--r--   0 user       (501) staff       (20)     2110 2024-04-22 05:07:11.000000 sttn-0.3.4/src/sttn/nli/templates/data_filter.j2
+-rw-r--r--   0 user       (501) staff       (20)      540 2024-05-03 05:53:52.000000 sttn-0.3.4/src/sttn/nli/templates/data_provider.j2
+-rw-r--r--   0 user       (501) staff       (20)      561 2024-05-03 05:59:59.000000 sttn-0.3.4/src/sttn/nli/templates/data_provider_arguments.j2
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-17 05:15:04.059275 sttn-0.3.4/src/sttn/plot/
+-rw-r--r--   0 user       (501) staff       (20)       19 2022-09-25 21:46:22.000000 sttn-0.3.4/src/sttn/plot/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3930 2024-01-11 12:33:45.000000 sttn-0.3.4/src/sttn/plot/api.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-17 05:15:04.060203 sttn-0.3.4/src/sttn/plot/keplergl/
+-rw-r--r--   0 user       (501) staff       (20)        0 2022-09-17 23:00:44.000000 sttn-0.3.4/src/sttn/plot/keplergl/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1639 2024-01-11 12:33:54.000000 sttn-0.3.4/src/sttn/plot/keplergl/filter.py
+-rw-r--r--   0 user       (501) staff       (20)     6344 2024-05-03 05:18:24.000000 sttn-0.3.4/src/sttn/plot/keplergl/layer.py
+-rw-r--r--   0 user       (501) staff       (20)     2143 2024-01-11 12:34:01.000000 sttn-0.3.4/src/sttn/plot/keplergl/map.py
+-rw-r--r--   0 user       (501) staff       (20)     2787 2020-12-07 04:18:24.000000 sttn-0.3.4/src/sttn/skeleton.py
+-rw-r--r--   0 user       (501) staff       (20)     1860 2024-01-11 12:33:03.000000 sttn-0.3.4/src/sttn/utils.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-17 05:15:04.061516 sttn-0.3.4/src/sttn.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     3464 2024-05-17 05:15:03.000000 sttn-0.3.4/src/sttn.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     2254 2024-05-17 05:15:04.000000 sttn-0.3.4/src/sttn.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-05-17 05:15:03.000000 sttn-0.3.4/src/sttn.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2020-12-07 05:04:43.000000 sttn-0.3.4/src/sttn.egg-info/not-zip-safe
+-rw-r--r--   0 user       (501) staff       (20)      150 2024-05-17 05:15:03.000000 sttn-0.3.4/src/sttn.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)        5 2024-05-17 05:15:03.000000 sttn-0.3.4/src/sttn.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-17 05:15:04.061315 sttn-0.3.4/tests/
+-rw-r--r--   0 user       (501) staff       (20)      225 2020-12-07 04:16:52.000000 sttn-0.3.4/tests/conftest.py
+-rw-r--r--   0 user       (501) staff       (20)     1684 2021-03-28 22:51:50.000000 sttn-0.3.4/tests/test_network_constructor.py
+-rw-r--r--   0 user       (501) staff       (20)     2349 2021-03-29 03:32:01.000000 sttn-0.3.4/tests/test_network_operations.py
+-rw-r--r--   0 user       (501) staff       (20)      304 2020-12-07 04:18:55.000000 sttn-0.3.4/tests/test_skeleton.py
+-rw-r--r--   0 user       (501) staff       (20)     2010 2021-08-01 05:26:59.000000 sttn-0.3.4/tox.ini
```

### Comparing `sttn-0.3.3/.coveragerc` & `sttn-0.3.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/.github/workflows/python-package-conda.yml` & `sttn-0.3.4/.github/workflows/python-package-conda.yml`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/.gitignore` & `sttn-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/LICENSE.txt` & `sttn-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/PKG-INFO` & `sttn-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sttn
-Version: 0.3.3
+Version: 0.3.4
 Summary: Library for spatio-temporal transactional network analysis
 Home-page: https://github.com/yuribogomolov/sttn
 Author: Yuri Bogomolov
 Author-email: bogomoloviura@gmail.com
 License: GNU GPLv3
 Project-URL: Documentation, https://github.com/yuribogomolov/sttn#readme
 Project-URL: Bug Tracker, https://github.com/yuribogomolov/sttn/issues
```

### Comparing `sttn-0.3.3/Pipfile` & `sttn-0.3.4/Pipfile`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/Pipfile.lock` & `sttn-0.3.4/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/README.rst` & `sttn-0.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/docs/Makefile` & `sttn-0.3.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/docs/conf.py` & `sttn-0.3.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/docs/index.rst` & `sttn-0.3.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/notebooks/LEHD Origin-Destination employment data.ipynb` & `sttn-0.3.4/notebooks/LEHD Origin-Destination employment data.ipynb`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/notebooks/LEHD data.ipynb` & `sttn-0.3.4/notebooks/LEHD data.ipynb`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/notebooks/all_gravity_models.ipynb` & `sttn-0.3.4/notebooks/all_gravity_models.ipynb`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/notebooks/checkFlow.ipynb` & `sttn-0.3.4/notebooks/checkFlow.ipynb`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/notebooks/doubly_constrained_general_gravity_linear_DK.ipynb` & `sttn-0.3.4/notebooks/doubly_constrained_general_gravity_linear_DK.ipynb`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/notebooks/doubly_constrained_gravity_model.ipynb` & `sttn-0.3.4/notebooks/doubly_constrained_gravity_model.ipynb`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/notebooks/img/agg_adjacent_edges.png` & `sttn-0.3.4/notebooks/img/agg_adjacent_edges.png`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/notebooks/img/agg_parallel_edges.png` & `sttn-0.3.4/notebooks/img/agg_parallel_edges.png`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/notebooks/img/group_nodes.png` & `sttn-0.3.4/notebooks/img/group_nodes.png`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/notebooks/img/manhattan_taxi_zones.png` & `sttn-0.3.4/notebooks/img/manhattan_taxi_zones.png`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/notebooks/means of transportation/NYC.csv` & `sttn-0.3.4/notebooks/means of transportation/NYC.csv`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/notebooks/nyc_311_requests.ipynb` & `sttn-0.3.4/notebooks/nyc_311_requests.ipynb`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/notebooks/nyc_taxi_demo.ipynb` & `sttn-0.3.4/notebooks/nyc_taxi_demo.ipynb`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/notebooks/papers/YSC 2021.ipynb` & `sttn-0.3.4/notebooks/papers/YSC 2021.ipynb`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/notebooks/piecewise_gravity_model.ipynb` & `sttn-0.3.4/notebooks/piecewise_gravity_model.ipynb`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/notebooks/unconstrained_gravity_models.ipynb` & `sttn-0.3.4/notebooks/unconstrained_gravity_models.ipynb`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/setup.cfg` & `sttn-0.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/setup.py` & `sttn-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/src/sttn/__init__.py` & `sttn-0.3.4/src/sttn/__init__.py`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/src/sttn/algorithms/community/detection.py` & `sttn-0.3.4/src/sttn/algorithms/community/detection.py`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/src/sttn/data/brno.py` & `sttn-0.3.4/src/sttn/data/brno.py`

 * *Files 19% similar despite different names*

```diff
@@ -74,17 +74,50 @@
         nodes = JourneyDataProvider.read_nodes(shapefile_name)
         edges = JourneyDataProvider.read_edges(journey_csv_folder, start_level=start_level, end_level=end_level)
         sttn_network = network.SpatioTemporalNetwork(nodes=nodes, edges=edges)
         return sttn_network
 
 
 class HealthcareDataProvider(DataProvider):
-
+    """
+    Czech Republic healthcare data provider. Builds a network where every node represents a Czech Republic district
+    and every edge contains aggregated patients information where the origin is the residence of patients, and 
+    the destination is a healthcare facility district they commuted to. The provider gives information on how many visits
+    happened from origin to destination districts in a specific month of the year for different specializations and ICD-10
+    disease categories. The dataset covers 13 years of monthly data from 2010-01 to 2022-12. 
+    """
     @staticmethod
     def get_data(data_folder: str) -> network.SpatioTemporalNetwork:
+        """
+        Retrieves Czech Republic Healthcare data. 
+        Args:
+            data_folder (str): path to the data folder
+
+        Returns:
+            SpatioTemporalNetwork: An STTN network where nodes represent the Czech Republic districts 
+                (also called 'okres'), and edges represent the patients' treatment mobility and details.
+
+            The nodes dataframe contains the following columns:
+                'id' (str) - district LAU code
+                'name' (str) - district name
+                'geometry' (shape) - shape object for the district
+
+            The edges dataframe contains the following columns:
+                'origin' (str) - patients' residence district id
+                'destination' (str) - patients' medical facility district id
+                'year_visit' (int) - patients' year of visit
+                'month_visit' (int) - patients' month of visit
+                'specialization' (int) - patients' treatment medical branch specialization number
+                'icd10_category' (int) -patients' disease ICD10 category number
+                'number_of_visits' (int) - total number of patients who visited from a residence district to a healthcare facility,
+                                           grouped by medical specialization and disease category
+
+        
+        """
+      
         nodes = HealthcareDataProvider.read_nodes(f"{data_folder}/lau1.geojson")
         edges = HealthcareDataProvider.read_edges(f"{data_folder}/healthcare.parquet")
 
         ids_to_keep = nodes.index
         edges = edges[
             edges.origin.isin(ids_to_keep) & edges.destination.isin(ids_to_keep)]
```

### Comparing `sttn-0.3.3/src/sttn/data/census.py` & `sttn-0.3.4/src/sttn/data/census.py`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/src/sttn/data/data_provider.py` & `sttn-0.3.4/src/sttn/data/data_provider.py`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/src/sttn/data/lehd.py` & `sttn-0.3.4/src/sttn/data/lehd.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             year (str): Year of job data, starting from 2002
 
         Returns:
             SpatioTemporalNetwork: An STTN network where node represent census tracts and edges represent employment
                 statistics for people who live in the origin tract and work in the destination tract area.
 
             The nodes dataframe contains the following columns:
-                'id' (int64) - Census tract id
+                'id' (int64) - index column, represents census tract ids
                 'county' (str) - county of the tract (e.g. "Queens County, NY")
                 'zip' (int) - zip code of the tract
                 'geometry' (shape) - shape object for the tract
 
             The edges dataframe contains the following columns:
                 'origin' (int64) - origin Census tract id
                 'destination' (int64) - destination Census tract id
```

### Comparing `sttn-0.3.3/src/sttn/network.py` & `sttn-0.3.4/src/sttn/network.py`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/src/sttn/nli/analyst.py` & `sttn-0.3.4/src/sttn/nli/analyst.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 from sttn.nli import Query
 from sttn.nli.data import NetworkBuilder
 from sttn.nli.prompts import Context
 
 
 class STTNAnalyst:
-    def __init__(self, verbose: bool = False):
+    def __init__(self, verbose: bool = False, model_name: str = "gpt-4o"):
         self._verbose = verbose
-        self._model = ChatOpenAI(temperature=0, model_name="gpt-3.5-turbo-0125")
+        self._model = ChatOpenAI(temperature=0, model_name=model_name)
         prompt = ChatPromptTemplate.from_messages(
             [
                 SystemMessage(
                     content="You are a chatbot having a conversation with a human."
                 ),  # The persistent system prompt
                 MessagesPlaceholder(
                     variable_name="chat_history"
@@ -38,14 +38,15 @@
             llm=self._model,
             prompt=prompt,
             verbose=verbose,
             memory=memory,
         )
         self._network_builder = NetworkBuilder(model=self._chain)
         self._context: Optional[Context] = None
+        self._model_name: str = model_name
 
     def clarify(self, human_input: str) -> str:
         return self._chain.predict(human_input=human_input)
 
     def chat(self, user_query: Optional[str] = None) -> Context:
         if user_query is None:
             print("Enter your question please:")
```

### Comparing `sttn-0.3.3/src/sttn/nli/data.py` & `sttn-0.3.4/src/sttn/nli/data.py`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/src/sttn/nli/models/output.py` & `sttn-0.3.4/src/sttn/nli/models/output.py`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/src/sttn/nli/prompts.py` & `sttn-0.3.4/src/sttn/nli/prompts.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,15 +42,23 @@
     @property
     def sttn(self):
         return self._sttn
 
     @sttn.setter
     def sttn(self, sttn: SpatioTemporalNetwork):
         self._sttn = sttn
-
+    
+    @property
+    def data_provider_id(self):
+        return self._data_provider_id
+    
+    @data_provider_id.setter
+    def data_provider_id(self, data_provider_id: str):
+        self._data_provider_id = data_provider_id
+        
     @property
     def data_provider_args(self):
         return self._data_provider_args
 
     @data_provider_args.setter
     def data_provider_args(self, _data_provider_args: Dict[str, str]):
         self._data_provider_args = _data_provider_args
@@ -73,15 +81,28 @@
 
 
 class PromptGenerator:
 
     @staticmethod
     def get_df_description(df: pd.DataFrame) -> str:
         schema_str = ""
-        schema_str += "\n".join([f"{col:20}: {dtype}" for col, dtype in df.dtypes.items()])
+        for col, dtype in df.dtypes.items():
+            if dtype.name == 'geometry':
+                schema_str += f"{col}: geometry\n"
+            elif pd.api.types.is_numeric_dtype(dtype):
+                # Calculate min, max, and mean for numeric columns
+                min_val = df[col].min()
+                max_val = df[col].max()
+                mean_val = df[col].mean()
+                schema_str += f"{col:20}: {dtype} - Min: {min_val}, Max: {max_val}, Avg: {mean_val:.2f}\n"
+            else:
+                # Find the 5 most common values for string columns
+                common_vals = df[col].value_counts().head(5)
+                common_vals_str = ", ".join([f"{val} ({count})" for val, count in common_vals.items()])
+                schema_str += f"{col:20}: {dtype} - Most common values: {common_vals_str}\n"
         return schema_str
 
     @staticmethod
     def get_template(template_fname: str) -> Template:
         environment = Environment(loader=PackageLoader("sttn", package_path="nli/templates"))
         return environment.get_template(template_fname)
```

### Comparing `sttn-0.3.3/src/sttn/nli/templates/data_analysis.j2` & `sttn-0.3.4/src/sttn/nli/templates/data_analysis.j2`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/src/sttn/nli/templates/data_filter.j2` & `sttn-0.3.4/src/sttn/nli/templates/data_filter.j2`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/src/sttn/nli/templates/data_provider.j2` & `sttn-0.3.4/src/sttn/nli/templates/data_provider.j2`

 * *Files 2% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 provider_id: {{ data_provider.__name__ }}
 provider_documentation: {{ data_provider.__doc__ }}
 -----
 {% endfor %}
 
 === Task ===
 Output a json message with two fields:
-`provider_id` - the provider id that can be used to answer the question above, or an empty string if none of the providers from the list can be used.
-`justification` - reasoning for the provider selection
+"provider_id" - the provider id that can be used to answer the question above, or an empty string if none of the providers from the list can be used.
+"justification" - reasoning for the provider selection
```

### Comparing `sttn-0.3.3/src/sttn/nli/templates/data_provider_arguments.j2` & `sttn-0.3.4/src/sttn/nli/templates/data_provider_arguments.j2`

 * *Files 6% similar despite different names*

```diff
@@ -7,11 +7,10 @@
 {{ data_provider_documentation }}
 
 === Data Description ===
 {{ data_description }}
 
 === Task ===
 Print a valid json message with the following fields:
-`feasible` - boolean `True` if the data provider can retrieve data for the user query and `False` otherwise
-`justification` - string with feasibility justification
-`arguments` - a json string with one field for each data provider argument with the right value
-
+"feasible" - boolean "True" if the data provider can retrieve data for the user query and "False" otherwise
+"justification" - string with feasibility justification
+"arguments" - a json object with one field for each data provider argument with the right value
```

### Comparing `sttn-0.3.3/src/sttn/plot/api.py` & `sttn-0.3.4/src/sttn/plot/api.py`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/src/sttn/plot/keplergl/filter.py` & `sttn-0.3.4/src/sttn/plot/keplergl/filter.py`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/src/sttn/plot/keplergl/layer.py` & `sttn-0.3.4/src/sttn/plot/keplergl/layer.py`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/src/sttn/plot/keplergl/map.py` & `sttn-0.3.4/src/sttn/plot/keplergl/map.py`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/src/sttn/skeleton.py` & `sttn-0.3.4/src/sttn/skeleton.py`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/src/sttn/utils.py` & `sttn-0.3.4/src/sttn/utils.py`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/src/sttn.egg-info/PKG-INFO` & `sttn-0.3.4/src/sttn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sttn
-Version: 0.3.3
+Version: 0.3.4
 Summary: Library for spatio-temporal transactional network analysis
 Home-page: https://github.com/yuribogomolov/sttn
 Author: Yuri Bogomolov
 Author-email: bogomoloviura@gmail.com
 License: GNU GPLv3
 Project-URL: Documentation, https://github.com/yuribogomolov/sttn#readme
 Project-URL: Bug Tracker, https://github.com/yuribogomolov/sttn/issues
```

### Comparing `sttn-0.3.3/src/sttn.egg-info/SOURCES.txt` & `sttn-0.3.4/src/sttn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/tests/test_network_constructor.py` & `sttn-0.3.4/tests/test_network_constructor.py`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/tests/test_network_operations.py` & `sttn-0.3.4/tests/test_network_operations.py`

 * *Files identical despite different names*

### Comparing `sttn-0.3.3/tox.ini` & `sttn-0.3.4/tox.ini`

 * *Files identical despite different names*

