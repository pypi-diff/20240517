# Comparing `tmp/f3dasm-1.4.71.tar.gz` & `tmp/f3dasm-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f3dasm-1.4.71.tar", last modified: Mon Apr 22 09:52:32 2024, max compression
+gzip compressed data, was "f3dasm-1.4.8.tar", last modified: Fri May 17 13:49:38 2024, max compression
```

## Comparing `f3dasm-1.4.71.tar` & `f3dasm-1.4.8.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-22 09:52:32.863739 f3dasm-1.4.71/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1531 2023-03-30 12:29:51.000000 f3dasm-1.4.71/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)       74 2023-07-07 13:46:05.000000 f3dasm-1.4.71/MANIFEST.in
--rw-r--r--   0 martin    (1000) martin    (1000)     4480 2024-04-22 09:52:32.863739 f3dasm-1.4.71/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     2900 2023-11-14 18:17:25.000000 f3dasm-1.4.71/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)        6 2024-04-22 08:38:01.000000 f3dasm-1.4.71/VERSION
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-22 09:52:32.855739 f3dasm-1.4.71/docs/
--rw-rw-r--   0 martin    (1000) martin    (1000)       88 2023-12-07 15:18:37.000000 f3dasm-1.4.71/docs/requirements.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      457 2023-07-15 20:12:10.000000 f3dasm-1.4.71/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)       85 2023-09-06 16:39:06.000000 f3dasm-1.4.71/requirements.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)     1401 2024-04-22 09:52:32.863739 f3dasm-1.4.71/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-22 09:52:32.855739 f3dasm-1.4.71/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-22 09:52:32.855739 f3dasm-1.4.71/src/f3dasm/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1776 2024-04-22 07:57:55.000000 f3dasm-1.4.71/src/f3dasm/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)       28 2024-04-22 08:37:43.000000 f3dasm-1.4.71/src/f3dasm/__version__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-22 09:52:32.859739 f3dasm-1.4.71/src/f3dasm/_src/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.71/src/f3dasm/_src/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1241 2023-11-14 18:17:25.000000 f3dasm-1.4.71/src/f3dasm/_src/_argparser.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-22 09:52:32.859739 f3dasm-1.4.71/src/f3dasm/_src/datageneration/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1385 2023-12-07 15:18:37.000000 f3dasm-1.4.71/src/f3dasm/_src/datageneration/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-22 09:52:32.859739 f3dasm-1.4.71/src/f3dasm/_src/datageneration/abaqus/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.71/src/f3dasm/_src/datageneration/abaqus/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5136 2023-11-14 18:17:25.000000 f3dasm-1.4.71/src/f3dasm/_src/datageneration/abaqus/abaqus_functions.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5479 2023-11-14 18:17:25.000000 f3dasm-1.4.71/src/f3dasm/_src/datageneration/abaqus/abaqus_simulator.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1510 2023-11-14 18:17:25.000000 f3dasm-1.4.71/src/f3dasm/_src/datageneration/abaqus/utils.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     8268 2024-04-19 15:20:52.000000 f3dasm-1.4.71/src/f3dasm/_src/datageneration/datagenerator.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-22 09:52:32.859739 f3dasm-1.4.71/src/f3dasm/_src/datageneration/functions/
--rw-rw-r--   0 martin    (1000) martin    (1000)     5229 2023-11-14 18:17:25.000000 f3dasm-1.4.71/src/f3dasm/_src/datageneration/functions/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-22 09:52:32.859739 f3dasm-1.4.71/src/f3dasm/_src/datageneration/functions/adapters/
--rw-rw-r--   0 martin    (1000) martin    (1000)      125 2023-11-14 18:17:25.000000 f3dasm-1.4.71/src/f3dasm/_src/datageneration/functions/adapters/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     8220 2024-04-19 15:20:52.000000 f3dasm-1.4.71/src/f3dasm/_src/datageneration/functions/adapters/augmentor.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4389 2024-04-19 15:20:52.000000 f3dasm-1.4.71/src/f3dasm/_src/datageneration/functions/adapters/pybenchfunction.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     9183 2024-04-19 15:20:52.000000 f3dasm-1.4.71/src/f3dasm/_src/datageneration/functions/function.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1794 2023-11-14 18:17:25.000000 f3dasm-1.4.71/src/f3dasm/_src/datageneration/functions/function_factory.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    80508 2024-04-19 15:20:52.000000 f3dasm-1.4.71/src/f3dasm/_src/datageneration/functions/pybenchfunction.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-22 09:52:32.859739 f3dasm-1.4.71/src/f3dasm/_src/design/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.71/src/f3dasm/_src/design/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    29701 2024-04-19 15:20:52.000000 f3dasm-1.4.71/src/f3dasm/_src/design/domain.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     9767 2024-04-19 15:20:52.000000 f3dasm-1.4.71/src/f3dasm/_src/design/parameter.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10657 2024-04-19 15:20:52.000000 f3dasm-1.4.71/src/f3dasm/_src/design/samplers.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-22 09:52:32.859739 f3dasm-1.4.71/src/f3dasm/_src/experimentdata/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.71/src/f3dasm/_src/experimentdata/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3300 2023-12-07 15:18:37.000000 f3dasm-1.4.71/src/f3dasm/_src/experimentdata/_columns.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    17550 2024-04-19 15:20:52.000000 f3dasm-1.4.71/src/f3dasm/_src/experimentdata/_data.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10047 2024-04-19 15:20:52.000000 f3dasm-1.4.71/src/f3dasm/_src/experimentdata/_io.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10455 2024-04-19 15:20:52.000000 f3dasm-1.4.71/src/f3dasm/_src/experimentdata/_jobqueue.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    23185 2024-04-19 15:20:52.000000 f3dasm-1.4.71/src/f3dasm/_src/experimentdata/_newdata.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    66267 2024-04-19 15:20:52.000000 f3dasm-1.4.71/src/f3dasm/_src/experimentdata/experimentdata.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    12738 2024-04-19 15:20:52.000000 f3dasm-1.4.71/src/f3dasm/_src/experimentdata/experimentsample.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1618 2023-12-07 15:18:37.000000 f3dasm-1.4.71/src/f3dasm/_src/experimentdata/utils.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2125 2024-04-19 15:20:52.000000 f3dasm-1.4.71/src/f3dasm/_src/hydra_utils.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4025 2023-11-14 18:17:25.000000 f3dasm-1.4.71/src/f3dasm/_src/logger.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-22 09:52:32.859739 f3dasm-1.4.71/src/f3dasm/_src/machinelearning/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.71/src/f3dasm/_src/machinelearning/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-22 09:52:32.863739 f3dasm-1.4.71/src/f3dasm/_src/optimization/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1751 2023-12-07 15:18:37.000000 f3dasm-1.4.71/src/f3dasm/_src/optimization/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-22 09:52:32.863739 f3dasm-1.4.71/src/f3dasm/_src/optimization/adapters/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.71/src/f3dasm/_src/optimization/adapters/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2407 2024-04-19 15:20:52.000000 f3dasm-1.4.71/src/f3dasm/_src/optimization/adapters/scipy_implementations.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1157 2024-04-19 15:20:52.000000 f3dasm-1.4.71/src/f3dasm/_src/optimization/cg.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1258 2024-04-19 15:20:52.000000 f3dasm-1.4.71/src/f3dasm/_src/optimization/lbfgsb.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1324 2024-04-19 15:20:52.000000 f3dasm-1.4.71/src/f3dasm/_src/optimization/neldermead.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5903 2024-04-19 15:20:52.000000 f3dasm-1.4.71/src/f3dasm/_src/optimization/optimizer.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2097 2023-12-07 15:18:37.000000 f3dasm-1.4.71/src/f3dasm/_src/optimization/optimizer_factory.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1770 2024-04-19 15:20:52.000000 f3dasm-1.4.71/src/f3dasm/_src/optimization/randomsearch.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     8914 2023-11-14 18:17:25.000000 f3dasm-1.4.71/src/f3dasm/_src/run_optimization.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-22 09:52:32.863739 f3dasm-1.4.71/src/f3dasm/datageneration/
--rw-rw-r--   0 martin    (1000) martin    (1000)      773 2024-04-22 07:46:23.000000 f3dasm-1.4.71/src/f3dasm/datageneration/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      993 2023-10-03 19:08:27.000000 f3dasm-1.4.71/src/f3dasm/datageneration/abaqus.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      906 2023-10-03 19:08:27.000000 f3dasm-1.4.71/src/f3dasm/datageneration/functions.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1442 2024-04-19 15:20:52.000000 f3dasm-1.4.71/src/f3dasm/design.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      791 2024-04-19 15:20:52.000000 f3dasm-1.4.71/src/f3dasm/hydra_tools.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1665 2023-10-03 19:08:27.000000 f3dasm-1.4.71/src/f3dasm/optimization.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-22 09:52:32.863739 f3dasm-1.4.71/src/f3dasm.egg-info/
--rw-r--r--   0 martin    (1000) martin    (1000)     4480 2024-04-22 09:52:32.000000 f3dasm-1.4.71/src/f3dasm.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     2442 2024-04-22 09:52:32.000000 f3dasm-1.4.71/src/f3dasm.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2024-04-22 09:52:32.000000 f3dasm-1.4.71/src/f3dasm.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       86 2024-04-22 09:52:32.000000 f3dasm-1.4.71/src/f3dasm.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        7 2024-04-22 09:52:32.000000 f3dasm-1.4.71/src/f3dasm.egg-info/top_level.txt
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-04-22 09:52:32.863739 f3dasm-1.4.71/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2022-08-17 09:47:40.000000 f3dasm-1.4.71/tests/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      141 2022-08-31 10:13:29.000000 f3dasm-1.4.71/tests/__init__.pyc
--rw-rw-r--   0 martin    (1000) martin    (1000)      855 2023-10-02 00:02:33.000000 f3dasm-1.4.71/tests/conftest.py
--rw-rw-r--   0 martin    (1000) martin    (1000)       29 2023-03-10 12:07:18.000000 f3dasm-1.4.71/tests/requirements.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.406901 f3dasm-1.4.8/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1531 2023-03-30 12:29:51.000000 f3dasm-1.4.8/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)       74 2023-07-07 13:46:05.000000 f3dasm-1.4.8/MANIFEST.in
+-rw-r--r--   0 martin    (1000) martin    (1000)     5938 2024-05-17 13:49:38.406901 f3dasm-1.4.8/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4276 2024-05-17 13:36:49.000000 f3dasm-1.4.8/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)        5 2024-05-17 13:36:49.000000 f3dasm-1.4.8/VERSION
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.394902 f3dasm-1.4.8/docs/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      103 2024-05-17 13:36:49.000000 f3dasm-1.4.8/docs/requirements.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      457 2023-07-15 20:12:10.000000 f3dasm-1.4.8/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)       85 2023-09-06 16:39:06.000000 f3dasm-1.4.8/requirements.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1435 2024-05-17 13:49:38.406901 f3dasm-1.4.8/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.390902 f3dasm-1.4.8/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.394902 f3dasm-1.4.8/src/f3dasm/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1804 2024-05-17 13:36:49.000000 f3dasm-1.4.8/src/f3dasm/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)       27 2024-05-17 13:36:49.000000 f3dasm-1.4.8/src/f3dasm/__version__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.398902 f3dasm-1.4.8/src/f3dasm/_src/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.8/src/f3dasm/_src/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1241 2023-11-14 18:17:25.000000 f3dasm-1.4.8/src/f3dasm/_src/_argparser.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.398902 f3dasm-1.4.8/src/f3dasm/_src/datageneration/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1385 2023-12-07 15:18:37.000000 f3dasm-1.4.8/src/f3dasm/_src/datageneration/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.398902 f3dasm-1.4.8/src/f3dasm/_src/datageneration/abaqus/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.8/src/f3dasm/_src/datageneration/abaqus/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5136 2023-11-14 18:17:25.000000 f3dasm-1.4.8/src/f3dasm/_src/datageneration/abaqus/abaqus_functions.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5479 2023-11-14 18:17:25.000000 f3dasm-1.4.8/src/f3dasm/_src/datageneration/abaqus/abaqus_simulator.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1510 2023-11-14 18:17:25.000000 f3dasm-1.4.8/src/f3dasm/_src/datageneration/abaqus/utils.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8018 2024-05-17 13:36:49.000000 f3dasm-1.4.8/src/f3dasm/_src/datageneration/datagenerator.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.398902 f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5229 2023-11-14 18:17:25.000000 f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.398902 f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/adapters/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      125 2023-11-14 18:17:25.000000 f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/adapters/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8220 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/adapters/augmentor.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4389 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/adapters/pybenchfunction.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9183 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/function.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1794 2023-11-14 18:17:25.000000 f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/function_factory.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    80508 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/pybenchfunction.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.402902 f3dasm-1.4.8/src/f3dasm/_src/design/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.8/src/f3dasm/_src/design/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    21658 2024-05-17 13:36:49.000000 f3dasm-1.4.8/src/f3dasm/_src/design/domain.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10505 2024-05-17 13:36:49.000000 f3dasm-1.4.8/src/f3dasm/_src/design/parameter.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.402902 f3dasm-1.4.8/src/f3dasm/_src/experimentdata/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.8/src/f3dasm/_src/experimentdata/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3673 2024-05-17 13:36:49.000000 f3dasm-1.4.8/src/f3dasm/_src/experimentdata/_columns.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    17943 2024-05-17 13:36:49.000000 f3dasm-1.4.8/src/f3dasm/_src/experimentdata/_data.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10131 2024-05-17 13:36:49.000000 f3dasm-1.4.8/src/f3dasm/_src/experimentdata/_io.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10455 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/_src/experimentdata/_jobqueue.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    23185 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/_src/experimentdata/_newdata.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    68231 2024-05-17 13:36:49.000000 f3dasm-1.4.8/src/f3dasm/_src/experimentdata/experimentdata.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    12764 2024-05-17 13:36:49.000000 f3dasm-1.4.8/src/f3dasm/_src/experimentdata/experimentsample.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    12801 2024-05-17 13:36:49.000000 f3dasm-1.4.8/src/f3dasm/_src/experimentdata/samplers.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1618 2023-12-07 15:18:37.000000 f3dasm-1.4.8/src/f3dasm/_src/experimentdata/utils.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2125 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/_src/hydra_utils.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4025 2023-11-14 18:17:25.000000 f3dasm-1.4.8/src/f3dasm/_src/logger.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.402902 f3dasm-1.4.8/src/f3dasm/_src/machinelearning/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.8/src/f3dasm/_src/machinelearning/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.402902 f3dasm-1.4.8/src/f3dasm/_src/optimization/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1751 2023-12-07 15:18:37.000000 f3dasm-1.4.8/src/f3dasm/_src/optimization/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.402902 f3dasm-1.4.8/src/f3dasm/_src/optimization/adapters/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-10-03 19:08:27.000000 f3dasm-1.4.8/src/f3dasm/_src/optimization/adapters/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2407 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/_src/optimization/adapters/scipy_implementations.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1157 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/_src/optimization/cg.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1258 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/_src/optimization/lbfgsb.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1324 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/_src/optimization/neldermead.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5903 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/_src/optimization/optimizer.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2097 2023-12-07 15:18:37.000000 f3dasm-1.4.8/src/f3dasm/_src/optimization/optimizer_factory.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1770 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/_src/optimization/randomsearch.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8914 2023-11-14 18:17:25.000000 f3dasm-1.4.8/src/f3dasm/_src/run_optimization.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.406901 f3dasm-1.4.8/src/f3dasm/datageneration/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      773 2024-04-22 07:46:23.000000 f3dasm-1.4.8/src/f3dasm/datageneration/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      993 2023-10-03 19:08:27.000000 f3dasm-1.4.8/src/f3dasm/datageneration/abaqus.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      906 2023-10-03 19:08:27.000000 f3dasm-1.4.8/src/f3dasm/datageneration/functions.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1351 2024-05-17 13:36:49.000000 f3dasm-1.4.8/src/f3dasm/design.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      791 2024-04-19 15:20:52.000000 f3dasm-1.4.8/src/f3dasm/hydra_tools.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1665 2023-10-03 19:08:27.000000 f3dasm-1.4.8/src/f3dasm/optimization.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.406901 f3dasm-1.4.8/src/f3dasm.egg-info/
+-rw-r--r--   0 martin    (1000) martin    (1000)     5938 2024-05-17 13:49:38.000000 f3dasm-1.4.8/src/f3dasm.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2450 2024-05-17 13:49:38.000000 f3dasm-1.4.8/src/f3dasm.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2024-05-17 13:49:38.000000 f3dasm-1.4.8/src/f3dasm.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      132 2024-05-17 13:49:38.000000 f3dasm-1.4.8/src/f3dasm.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        7 2024-05-17 13:49:38.000000 f3dasm-1.4.8/src/f3dasm.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-17 13:49:38.406901 f3dasm-1.4.8/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2022-08-17 09:47:40.000000 f3dasm-1.4.8/tests/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      141 2022-08-31 10:13:29.000000 f3dasm-1.4.8/tests/__init__.pyc
+-rw-rw-r--   0 martin    (1000) martin    (1000)      855 2023-10-02 00:02:33.000000 f3dasm-1.4.8/tests/conftest.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)       29 2023-03-10 12:07:18.000000 f3dasm-1.4.8/tests/requirements.txt
```

### Comparing `f3dasm-1.4.71/LICENSE` & `f3dasm-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/PKG-INFO` & `f3dasm-1.4.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f3dasm
-Version: 1.4.71
+Version: 1.4.8
 Summary: f3dasm - Framework for Data-driven development and Analysis of Structures and Materials
 Home-page: https://github.com/bessagroup/f3dasm
 Author: Martin van der Schelling
 Author-email: M.P.vanderSchelling@tudelft.nl
 License: BSD
 Project-URL: Documentation, https://f3dasm.readthedocs.io/
 Project-URL: Wiki, https://github.com/bessagroup/f3dasm/wiki
@@ -12,35 +12,37 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: xarray
 Requires-Dist: matplotlib
 Requires-Dist: hydra-core
 Requires-Dist: pathos>=0.3.0
 Requires-Dist: autograd
 Requires-Dist: SALib
 Requires-Dist: filelock
+Provides-Extra: benchmark
+Requires-Dist: abaqus2py==1.0.0; extra == "benchmark"
+Requires-Dist: f3dasm_optimize; extra == "benchmark"
 
 f3dasm
 ------
 *Framework for data-driven design \& analysis of structures and materials*
 
 ***
 
@@ -49,30 +51,54 @@
 [![GitHub license](https://img.shields.io/badge/license-BSD-blue)](https://github.com/bessagroup/f3dasm)
 [![Documentation Status](https://readthedocs.org/projects/f3dasm/badge/?version=latest)](https://f3dasm.readthedocs.io/en/latest/?badge=latest)
 
 [**Docs**](https://f3dasm.readthedocs.io/)
 | [**Installation**](https://f3dasm.readthedocs.io/en/latest/rst_doc_files/general/gettingstarted.html)
 | [**GitHub**](https://github.com/bessagroup/f3dasm)
 | [**PyPI**](https://pypi.org/project/f3dasm/)
-| [**Practical sessions**](https://github.com/mpvanderschelling/f3dasm_teach)
 
 ## Summary
 
-Welcome to `f3dasm`, a Python package for data-driven design and analysis of structures and materials.
+Welcome to `f3dasm`, a **f**ramework for **d**ata-**d**riven **d**esign and **a**nalysis of **s**tructures and **m**aterials.
 
+`f3dasm` introduces a general and user-friendly data-driven Python package for researchers and practitioners working on design and analysis of materials and structures. Some of the key features include:
+
+-  **Modular design** 
+    - The framework introduces flexible interfaces, allowing users to easily integrate their own models and algorithms.
+
+- **Automatic data management**
+    -  The framework automatically manages I/O processes, saving you time and effort implementing these common procedures.
+
+- **Easy parallelization**
+    - The framework manages parallelization of experiments, and is compatible with both local and high-performance cluster computing.
+
+- **Built-in defaults**
+    - The framework includes a collection of benchmark functions, optimization algorithms and sampling strategies to get you started right away!
+
+- **Hydra integration**
+    - The framework is supports the [hydra](https://hydra.cc/) configuration manager, to easily manage and run experiments.
+
+## Getting started
+
+The best way to get started is to follow the [installation instructions](https://f3dasm.readthedocs.io/en/latest/rst_doc_files/general/gettingstarted.html).
+
+## Illustrative benchmarks
+
+This package includes a collection of illustrative benchmark studies that demonstrate the capabilities of the framework. These studies are available in the `/studies` folder, and include the following studies:
+
+- Benchmarking optimization algorithms against well-known benchmark functions
+- 'Fragile Becomes Supercompressible' ([Bessa et al. (2019)](https://onlinelibrary.wiley.com/doi/full/10.1002/adma.201904845))
 
 ## Authorship
 
 * Current created and developer: [M.P. van der Schelling](https://github.com/mpvanderschelling/) (M.P.vanderSchelling@tudelft.nl)
 
 The Bessa research group at TU Delft is small... At the moment, we have limited availability to help future users/developers adapting the code to new problems, but we will do our best to help!
 
-## Getting started
 
-The best way to get started is to follow the [installation instructions](https://f3dasm.readthedocs.io/en/latest/rst_doc_files/general/gettingstarted.html).
 
 ## Referencing
 
 If you use or edit our work, please cite at least one of the appropriate references:
 
 [1] Bessa, M. A., Bostanabad, R., Liu, Z., Hu, A., Apley, D. W., Brinson, C., Chen, W., & Liu, W. K. (2017). A framework for data-driven analysis of materials under uncertainty: Countering the curse of dimensionality. Computer Methods in Applied Mechanics and Engineering, 320, 633-667.
 
@@ -84,12 +110,12 @@
 
 ## Community Support
 
 If you find any **issues, bugs or problems** with this template, please use the [GitHub issue tracker](https://github.com/bessagroup/f3dasm/issues) to report them.
 
 ## License
 
-Copyright 2023, Martin van der Schelling
+Copyright 2024, Martin van der Schelling
 
 All rights reserved.
 
 This project is licensed under the BSD 3-Clause License. See [LICENSE](https://github.com/bessagroup/f3dasm/blob/main/LICENSE) for the full license text.
```

### Comparing `f3dasm-1.4.71/setup.cfg` & `f3dasm-1.4.8/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -16,30 +16,32 @@
 	License :: OSI Approved :: BSD License
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	Intended Audience :: Information Technology
 	Intended Audience :: Science/Research
 	Topic :: Scientific/Engineering :: Artificial Intelligence
 	Topic :: Software Development :: Libraries :: Python Modules
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Operating System :: Microsoft :: Windows
 	Operating System :: POSIX :: Linux
 	Operating System :: MacOS
 
 [options]
-python_requires = >=3.7
+python_requires = >=3.8
 package_dir = 
 	= src
 packages = find:
 install_requires = file: requirements.txt
 
+[options.extras_require]
+benchmark = abaqus2py ==1.0.0; f3dasm_optimize
+
 [options.packages.find]
 where = src
 exclude = 
 	docs
 	tests
 
 [egg_info]
```

### Comparing `f3dasm-1.4.71/src/f3dasm/__init__.py` & `f3dasm-1.4.8/src/f3dasm/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,32 +2,24 @@
 f3dasm - A package for data-driven design and analysis of structures
 and materials
 
 This package provides tools for designing and optimizing materials, including
 functions for data analysis, design of experiments, machine learning,
 optimization, sampling, and simulation.
 
-Usage
------
-
->>> import f3dasm
-
-Links
------
-
 - Documentation: https://f3dasm.readthedocs.io
-
-Author: Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)
+- Author: Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)
 """
 
 #                                                                       Modules
 # =============================================================================
 
 from .__version__ import __version__
 from ._src._argparser import HPC_JOBID
+from ._src.experimentdata._io import StoreProtocol
 from ._src.experimentdata.experimentdata import ExperimentData
 from ._src.experimentdata.experimentsample import ExperimentSample
 from ._src.logger import DistributedFileHandler, logger
 from ._src.run_optimization import (OptimizationResult, calculate_mean_std,
                                     run_multiple_realizations,
                                     run_optimization)
 
@@ -49,8 +41,9 @@
     'DistributedFileHandler',
     'logger',
     'OptimizationResult',
     'run_multiple_realizations',
     'run_optimization',
     'HPC_JOBID',
     'calculate_mean_std',
+    'StoreProtocol',
 ]
```

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/_argparser.py` & `f3dasm-1.4.8/src/f3dasm/_src/_argparser.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/datageneration/__init__.py` & `f3dasm-1.4.8/src/f3dasm/_src/datageneration/__init__.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/datageneration/abaqus/abaqus_functions.py` & `f3dasm-1.4.8/src/f3dasm/_src/datageneration/abaqus/abaqus_functions.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/datageneration/abaqus/abaqus_simulator.py` & `f3dasm-1.4.8/src/f3dasm/_src/datageneration/abaqus/abaqus_simulator.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/datageneration/abaqus/utils.py` & `f3dasm-1.4.8/src/f3dasm/_src/datageneration/abaqus/utils.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/datageneration/datagenerator.py` & `f3dasm-1.4.8/src/f3dasm/_src/datageneration/datagenerator.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,54 +5,39 @@
 #                                                                       Modules
 # =============================================================================
 
 
 from __future__ import annotations
 
 # Standard
-import sys
+import inspect
 from abc import abstractmethod
 from functools import partial
 from typing import Any, Callable, Dict, List, Optional
 
-if sys.version_info < (3, 8):  # NOQA
-    from typing_extensions import Protocol  # NOQA
-else:
-    from typing import Protocol
-
 # Third-party
 import numpy as np
 
 # Local
 from ..design.domain import Domain
-from ..experimentdata.experimentsample import _experimentsample_factory
+# from ..experimentdata._io import StoreProtocol
+from ..experimentdata.experimentsample import (ExperimentSample,
+                                               _experimentsample_factory)
 from ..logger import time_and_log
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = "Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)"
 __credits__ = ["Martin van der Schelling"]
 __status__ = "Alpha"
 # =============================================================================
 #
 # =============================================================================
 
 
-class ExperimentSample(Protocol):
-    def get(self, key: str) -> Any:
-        ...
-
-    def store(self, object: Any, name: str, to_disk: bool) -> None:
-        ...
-
-    @property
-    def job_number(self) -> int:
-        ...
-
-
 class DataGenerator:
     """Base class for a data generator"""
 
     def pre_process(
             self, experiment_sample: ExperimentSample, **kwargs) -> None:
         """Interface function that handles the pre-processing of
          the data generator
@@ -186,27 +171,24 @@
         kwargs : dict
             The keyword arguments to pass to the post-processing function
         """
         self.post_process = partial(func, **kwargs)
 
 
 def convert_function(f: Callable,
-                     input: List[str],
                      output: Optional[List[str]] = None,
                      kwargs: Optional[Dict[str, Any]] = None,
                      to_disk: Optional[List[str]] = None) -> DataGenerator:
     """
     Converts a given function `f` into a `DataGenerator` object.
 
     Parameters
     ----------
     f : Callable
         The function to be converted.
-    input : List[str]
-        A list of argument names required by the function.
     output : Optional[List[str]], optional
         A list of names for the return values of the function.
         Defaults to None.
     kwargs : Optional[Dict[str, Any]], optional
         Additional keyword arguments passed to the function. Defaults to None.
     to_disk : Optional[List[str]], optional
         The list of output names where the value needs to be stored on disk.
@@ -220,23 +202,24 @@
     Notes
     -----
 
     The function `f` can have any number of arguments and any number of returns
     as long as they are consistent with the `input` and `output` arguments that
     are given to this function.
     """
-
+    signature = inspect.signature(f)
+    input = list(signature.parameters)
     kwargs = kwargs if kwargs is not None else {}
     to_disk = to_disk if to_disk is not None else []
     output = output if output is not None else []
 
     class TempDataGenerator(DataGenerator):
         def execute(self, **_kwargs) -> None:
             _input = {input_name: self.experiment_sample.get(input_name)
-                      for input_name in input}
+                      for input_name in input if input_name not in kwargs}
             _output = f(**_input, **kwargs)
 
             # check if output is empty
             if output is None:
                 return
 
             if len(output) == 1:
```

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/datageneration/functions/__init__.py` & `f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/datageneration/functions/adapters/augmentor.py` & `f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/adapters/augmentor.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/datageneration/functions/adapters/pybenchfunction.py` & `f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/adapters/pybenchfunction.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/datageneration/functions/function.py` & `f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/function.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/datageneration/functions/function_factory.py` & `f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/function_factory.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/datageneration/functions/pybenchfunction.py` & `f3dasm-1.4.8/src/f3dasm/_src/datageneration/functions/pybenchfunction.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/design/domain.py` & `f3dasm-1.4.8/src/f3dasm/_src/design/domain.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 # Standard
 import math
 import pickle
 import sys
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import Any, Dict, Iterable, Iterator, List, Sequence, Type
+from typing import (Any, Dict, Iterable, Iterator, List, Optional, Sequence,
+                    Type)
 
 if sys.version_info < (3, 8):  # NOQA
     from typing_extensions import Literal  # NOQA
 else:
     from typing import Literal
 
 # Third-party core
@@ -258,29 +259,14 @@
             pickle.dump(self, f)
 
     def _cast_types_dataframe(self) -> dict:
         """Make a dictionary that provides the datatype of each parameter"""
         return {name: parameter._type for
                 name, parameter in self.space.items()}
 
-    def _create_empty_dataframe(self) -> pd.DataFrame:
-        """Create an empty DataFrame with input columns.
-
-        Returns
-        -------
-        pd.DataFrame
-            DataFrame containing "input" columns.
-        """
-        # input columns
-        input_columns = [name for name in self.space.keys()]
-
-        return pd.DataFrame(columns=input_columns).astype(
-            self._cast_types_dataframe()
-        )
-
 #                                                  Append and remove parameters
 # =============================================================================
 
     def _add(self, name: str, parameter: _Parameter):
         # Check if parameter is already in the domain
         if name in self.space:
             raise KeyError(
@@ -386,31 +372,14 @@
         >>> domain = Domain()
         >>> domain.add_constant('param1', 0)
         >>> domain.space
         {'param1': ConstantParameter(value=0)}
         """
         self._add(name, _ConstantParameter(value))
 
-    def add_parameter(self, name: str):
-        """Add a new parameter to the domain.
-
-        Parameters
-        ----------
-        name : str
-            Name of the input parameter.
-
-        Example
-        -------
-        >>> domain = Domain()
-        >>> domain.add_parameter('param1')
-        >>> domain.space
-        {'param1': Parameter()}
-        """
-        self._add(name, _Parameter())
-
     def add(self, name: str,
             type: Literal['float', 'int', 'category', 'constant'],
             **kwargs):
         """Add a new input parameter to the domain.
 
         Parameters
         ----------
@@ -472,194 +441,14 @@
                         Choose a different name.")
             return
 
         self.output_space[name] = _OutputParameter(to_disk)
 #                                                                       Getters
 # =============================================================================
 
-    def get_continuous_parameters(self) -> Dict[str, _ContinuousParameter]:
-        """Get all continuous input parameters.
-
-        Returns
-        -------
-        Dict[str, _ContinuousParameter]
-            Space of continuous input parameters.
-
-        Example
-        -------
-        >>> domain = Domain()
-        >>> domain.space = {
-        ...     'param1': _ContinuousParameter(lower_bound=0., upper_bound=1.),
-        ...     'param2': CategoricalParameter(categories=['A', 'B', 'C']),
-        ...     'param3': _ContinuousParameter(lower_bound=2., upper_bound=5.)
-        ... }
-        >>> continuous_input_params = domain.get_continuous_input_parameters()
-        >>> continuous_input_params
-        {'param1': _ContinuousParameter(lower_bound=0., upper_bound=1.),
-         'param3': _ContinuousParameter(lower_bound=2., upper_bound=5.)}
-        """
-        return self._filter(_ContinuousParameter).space
-
-    def get_continuous_names(self) -> List[str]:
-        """Get the names of continuous input parameters in the input space.
-
-        Returns
-        -------
-        List[str]
-            List of names of continuous input parameters.
-
-        Example
-        -------
-        >>> domain = Domain()
-        >>> domain.space = {
-        ...     'param1': _ContinuousParameter(lower_bound=0., upper_bound=1.),
-        ...     'param2': _DiscreteParameter(lower_bound=1, upper_bound=3),
-        ...     'param3': _ContinuousParameter(lower_bound=2., upper_bound=5.)
-        ... }
-        >>> continuous_input_names = domain.get_continuous_input_names()
-        >>> continuous_input_names
-        ['param1', 'param3']
-        """
-        return self._filter(_ContinuousParameter).names
-
-    def get_discrete_parameters(self) -> Dict[str, _DiscreteParameter]:
-        """Retrieve all discrete input parameters.
-
-        Returns
-        -------
-        Dict[str, _DiscreteParameter]
-            Space of discrete input parameters.
-
-        Example
-        -------
-        >>> domain = Domain()
-        >>> domain.space = {
-        ...     'param1': _DiscreteParameter(lower_bound=1, upperBound=4),
-        ...     'param2': CategoricalParameter(categories=['A', 'B', 'C']),
-        ...     'param3': _DiscreteParameter(lower_bound=4, upperBound=6)
-        ... }
-        >>> discrete_input_params = domain.get_discrete_input_parameters()
-        >>> discrete_input_params
-        {'param1': _DiscreteParameter(lower_bound=1, upperBound=4)),
-         'param3': _DiscreteParameter(lower_bound=4, upperBound=6)}
-        """
-        return self._filter(_DiscreteParameter).space
-
-    def get_discrete_names(self) -> List[str]:
-        """Retrieve the names of all discrete input parameters.
-
-        Returns
-        -------
-        List[str]
-            List of names of discrete input parameters.
-
-        Example
-        -------
-        >>> domain = Domain()
-        >>> domain.space = {
-        ...     'param1': _DiscreteParameter(lower_bound=1, upperBound=4),
-        ...     'param2': _ContinuousParameter(lower_bound=0, upper_bound=1),
-        ...     'param3': _DiscreteParameter(lower_bound=4, upperBound=6)
-        ... }
-        >>> discrete_input_names = domain.get_discrete_input_names()
-        >>> discrete_input_names
-        ['param1', 'param3']
-        """
-        return self._filter(_DiscreteParameter).names
-
-    def get_categorical_parameters(self) -> Dict[str, _CategoricalParameter]:
-        """Retrieve all categorical input parameters.
-
-        Returns
-        -------
-        Dict[str, CategoricalParameter]
-            Space of categorical input parameters.
-
-        Example
-        -------
-        >>> domain = Domain()
-        >>> domain.space = {
-        ...     'param1': CategoricalParameter(categories=['A', 'B', 'C']),
-        ...     'param2': _ContinuousParameter(lower_bound=0, upper_bound=1),
-        ...     'param3': CategoricalParameter(categories=['X', 'Y', 'Z'])
-        ... }
-        >>> categorical_input_params =
-         domain.get_categorical_input_parameters()
-        >>> categorical_input_params
-        {'param1': CategoricalParameter(categories=['A', 'B', 'C']),
-         'param3': CategoricalParameter(categories=['X', 'Y', 'Z'])}
-        """
-        return self._filter(_CategoricalParameter).space
-
-    def get_categorical_names(self) -> List[str]:
-        """Retrieve the names of categorical input parameters.
-
-        Returns
-        -------
-        List[str]
-            List of names of categorical input parameters.
-
-        Example
-        -------
-        >>> domain = Domain()
-        >>> domain.space = {
-        ...     'param1': CategoricalParameter(categories=['A', 'B', 'C']),
-        ...     'param2': _ContinuousParameter(lower_bound=0, upper_bound=1),
-        ...     'param3': CategoricalParameter(categories=['X', 'Y', 'Z'])
-        ... }
-        >>> categorical_input_names = domain.get_categorical_input_names()
-        >>> categorical_input_names
-        ['param1', 'param3']
-        """
-        return self._filter(_CategoricalParameter).names
-
-    def get_constant_parameters(self) -> Dict[str, _ConstantParameter]:
-        """Retrieve all constant input parameters.
-
-        Returns
-        -------
-        Dict[str, ConstantParameter]
-            Space of constant input parameters.
-
-        Example
-        -------
-        >>> domain = Domain()
-        >>> domain.space = {
-        ...     'param1': ConstantParameter(value=0),
-        ...     'param2': CategoricalParameter(categories=['A', 'B', 'C']),
-        ...     'param3': ConstantParameter(value=1)
-        ... }
-        >>> constant_input_params = domain.get_constant_input_parameters()
-        >>> constant_input_params
-        {'param1': ConstantParameter(value=0),
-         'param3': ConstantParameter(value=1)}
-        """
-        return self._filter(_ConstantParameter).space
-
-    def get_constant_names(self) -> List[str]:
-        """Receive the names of the constant input parameters
-
-        Returns
-        -------
-            list of names of constant input parameters
-
-        Example
-        -------
-        >>> domain = Domain()
-        >>> domain.space = {
-        ...     'param1': ConstantParameter(value=0),
-        ...     'param2': ConstantParameter(value=1),
-        ...     'param3': _ContinuousParameter(lower_bound=0, upper_bound=1)
-        ... }
-        >>> constant_input_names = domain.get_constant_input_names()
-        >>> constant_input_names
-        ['param1', 'param2']
-        """
-        return self._filter(_ConstantParameter).names
-
     def get_bounds(self) -> np.ndarray:
         """Return the boundary constraints of the continuous input parameters
 
         Returns
         -------
             numpy array with lower and upper bound for each \
             continuous input dimension
@@ -676,15 +465,15 @@
         >>> bounds
         array([[ 0.,  1.],
             [-1.,  1.],
             [ 0., 10.]])
         """
         return np.array(
             [[parameter.lower_bound, parameter.upper_bound]
-                for _, parameter in self.get_continuous_parameters().items()]
+                for _, parameter in self.continuous.space.items()]
         )
 
     def _filter(self, type: Type[_Parameter]) -> Domain:
         """Filter the parameters of the domain by type
 
         Parameters
         ----------
@@ -784,38 +573,14 @@
 #                                                                 Miscellaneous
 # =============================================================================
 
     def _all_input_continuous(self) -> bool:
         """Check if all input parameters are continuous"""
         return len(self) == len(self._filter(_ContinuousParameter))
 
-    def _check_output(self, names: List[str]):
-        """Check if output is in the domain and add it if not
-
-        Parameters
-        ----------
-
-        names : list of str
-            Names of the outputs to be checked
-
-        Example
-        -------
-        >>> domain = Domain()
-        >>> domain.add_output('output1')
-        >>> domain.add_output('output2')
-        >>> domain._check_output(['output1', 'output2', 'output3'])
-        >>> domain.output_space
-        {'output1': _ContinuousParameter(lower_bound=-inf, upper_bound=inf),
-         'output2': _ContinuousParameter(lower_bound=-inf, upper_bound=inf),
-         'output3': _ContinuousParameter(lower_bound=-inf, upper_bound=inf)}
-        """
-        for output_name in names:
-            if not self.is_in_output(output_name):
-                self.add_output(output_name, to_disk=False)
-
     def is_in_output(self, output_name: str) -> bool:
         """Check if output is in the domain
 
         Parameters
         ----------
         output_name : str
             Name of the output
@@ -834,24 +599,26 @@
         >>> domain.is_in_output('output2')
         False
         """
         return output_name in self.output_space
 
 
 def make_nd_continuous_domain(bounds: np.ndarray | List[List[float]],
-                              dimensionality: int) -> Domain:
+                              dimensionality: Optional[int] = None) -> Domain:
     """Create a continuous domain.
 
     Parameters
     ----------
     bounds : numpy.ndarray
-        A 2D numpy array of shape (dimensionality, 2) specifying the lower \
+        A 2D numpy array of shape (dimensionality, 2) specifying the lower
         and upper bounds of every dimension.
     dimensionality : int
-        The number of dimensions.
+        The number of dimensions, optional. If not given, it is inferred
+        from the shape of the bounds. Argument is still present for legacy
+        reasons.
 
     Returns
     -------
     Domain
         A continuous domain with a continuous input.
 
     Note
@@ -871,26 +638,27 @@
     >>> domain = make_nd_continuous_domain(bounds, dimensionality)
     """
     space = {}
 
     # bounds is a list of lists, convert to numpy array:
     bounds = np.array(bounds)
 
+    dimensionality = bounds.shape[0]
+
     for dim in range(dimensionality):
         space[f"x{dim}"] = _ContinuousParameter(
             lower_bound=bounds[dim, 0], upper_bound=bounds[dim, 1])
 
     return Domain(space)
 
 
 def _domain_factory(domain: Domain | DictConfig | None,
                     input_data: pd.DataFrame,
                     output_data: pd.DataFrame) -> Domain:
     if isinstance(domain, Domain):
-        # domain._check_output(output_data.columns)
         return domain
 
     elif isinstance(domain, (Path, str)):
         return Domain.from_file(Path(domain))
 
     elif isinstance(domain, DictConfig):
         return Domain.from_yaml(domain)
```

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/design/parameter.py` & `f3dasm-1.4.8/src/f3dasm/_src/design/parameter.py`

 * *Files 8% similar despite different names*

```diff
@@ -186,14 +186,42 @@
         """Check if the lower boundary is lower than the higher boundary"""
         if self.upper_bound <= self.lower_bound:
             raise ValueError(f"The `upper_bound` value must be larger than \
                              the `lower_bound` value "
                              f"(lower_bound={self.lower_bound}, \
                                  higher_bound={self.upper_bound}")
 
+    def to_discrete(self, step: int = 1) -> _DiscreteParameter:
+        """Convert the continuous parameter to a discrete parameter.
+
+        Parameters
+        ----------
+        step : int
+            The step size of the discrete search space, which defaults to 1.
+
+        Returns
+        -------
+        DiscreteParameter
+            The discrete parameter.
+
+        Raises
+        ------
+        ValueError
+            If the step size is less than or equal to 0.
+
+        """
+        if step <= 0:
+            raise ValueError("The step size must be larger than 0.")
+
+        return _DiscreteParameter(
+            lower_bound=int(self.lower_bound),
+            upper_bound=int(self.upper_bound),
+            step=step
+        )
+
 
 @dataclass
 class _DiscreteParameter(_Parameter):
     """Create a search space parameter that is discrete
 
     Parameters
     ----------
@@ -247,15 +275,15 @@
         if self.upper_bound == self.lower_bound:
             raise ValueError("same lower as upper bound!")
 
         if self.step <= 0:
             raise ValueError("step size must be larger than 0!")
 
 
-@dataclass
+@ dataclass
 class _CategoricalParameter(_Parameter):
     """Create a search space parameter that is categorical
 
     Parameters
     ----------
     categories
         list of strings that represent available categories
```

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/experimentdata/_columns.py` & `f3dasm-1.4.8/src/f3dasm/_src/experimentdata/_columns.py`

 * *Files 17% similar despite different names*

```diff
@@ -51,14 +51,29 @@
 
         self.columns: Dict[str, None] = columns
 
     def __repr__(self) -> str:
         """Representation of the _Columns object."""
         return self.columns.keys().__repr__()
 
+    def __add__(self, __o: _Columns) -> _Columns:
+        """Add two _Columns objects.
+
+        Parameters
+        ----------
+        __o: _Columns
+            _Columns object to add
+
+        Returns
+        -------
+        _Columns
+            _Columns object with the columns of both _Columns objects
+        """
+        return _Columns({**self.columns, **__o.columns})
+
     @property
     def names(self) -> List[str]:
         """List of the names of the columns.
 
         Returns
         -------
         List[str]
```

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/experimentdata/_data.py` & `f3dasm-1.4.8/src/f3dasm/_src/experimentdata/_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         _dtypes = {index: parameter._type for index,
                    (_, parameter) in enumerate(domain.space.items())}
 
         df = pd.DataFrame(columns=range(len(domain))).astype(_dtypes)
 
         # Set the categories tot the categorical parameters
         for index, (name, categorical_input) in enumerate(
-                domain.get_categorical_parameters().items()):
+                domain.categorical.space.items()):
             df[index] = pd.Categorical(
                 df[index], categories=categorical_input.categories)
 
         _columns = {name: None for name in domain.names}
         return cls(df, columns=_Columns(_columns))
 
     @classmethod
@@ -432,14 +432,30 @@
 
         for other_column in other.columns.names:
             if other_column not in self.columns.names:
                 self.add_column(other_column)
 
         self.data.update(other.data.set_index(pd.Index(indices)))
 
+    def join(self, __o: _Data) -> _Data:
+        """Join two Data objects together.
+
+        Parameters
+        ----------
+        __o : Data
+            The Data object to join.
+
+        Returns
+        -------
+            The joined Data object.
+        """
+        return _Data(
+            pd.concat([self.data, __o.data], axis=1, ignore_index=True),
+            columns=self.columns + __o.columns)
+
 #                                                           Getters and setters
 # =============================================================================
 
     def get_data_dict(self, index: int) -> Dict[str, Any]:
         return self.to_dataframe().loc[index].to_dict()
 
     def set_data(self, index: int, value: Any, column: Optional[str] = None):
```

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/experimentdata/_io.py` & `f3dasm-1.4.8/src/f3dasm/_src/experimentdata/_io.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 RESOLUTION_MATPLOTLIB_FIGURE = 300
 MAX_TRIES = 10
 
 #                                                               Storing methods
 # =============================================================================
 
 
-class _Store:
+class StoreProtocol:
     """Base class for storing and loading output data from disk"""
     suffix: int
 
     def __init__(self, object: Any, path: Path):
         """
         Protocol class for storing and loading output data from disk
 
@@ -89,15 +89,15 @@
         ------
         NotImplementedError
             Raises if the method is not implemented
         """
         raise NotImplementedError()
 
 
-class PickleStore(_Store):
+class PickleStore(StoreProtocol):
     """Class to store and load objects using the pickle protocol"""
     suffix: str = '.pkl'
 
     def store(self) -> None:
         """
         Store the object to disk using the pickle protocol
         """
@@ -114,15 +114,15 @@
             The loaded object
 
         """
         with open(self.path.with_suffix(self.suffix), 'rb') as file:
             return pickle.load(file)
 
 
-class NumpyStore(_Store):
+class NumpyStore(StoreProtocol):
     """Class to store and load objects using the numpy protocol"""
     suffix: str = '.npy'
 
     def store(self) -> None:
         """
         Store the object to disk using the numpy protocol
         """
@@ -136,15 +136,15 @@
         -------
         np.ndarray
             The loaded object
         """
         return np.load(file=self.path.with_suffix(self.suffix))
 
 
-class PandasStore(_Store):
+class PandasStore(StoreProtocol):
     """Class to store and load objects using the pandas protocol"""
     suffix: str = '.csv'
 
     def store(self) -> None:
         """
         Store the object to disk using the pandas protocol
         """
@@ -158,15 +158,15 @@
         -------
         pd.DataFrame
             The loaded object
         """
         return pd.read_csv(self.path.with_suffix(self.suffix))
 
 
-class XarrayStore(_Store):
+class XarrayStore(StoreProtocol):
     """Class to store and load objects using the xarray protocol"""
     suffix: str = '.nc'
 
     def store(self) -> None:
         """
         Store the object to disk using the xarray protocol
         """
@@ -180,15 +180,15 @@
         -------
         xr.DataArray | xr.Dataset
             The loaded object
         """
         return xr.open_dataset(self.path.with_suffix(self.suffix))
 
 
-class FigureStore(_Store):
+class FigureStore(StoreProtocol):
     """Class to store and load objects using the matplotlib protocol"""
     suffix: str = '.png'
 
     def store(self) -> None:
         """
         Store the figure to disk as a png file
 
@@ -219,29 +219,29 @@
         - (M, N, 4) for RGBA images.
 
         Images are returned as float arrays (0-1).
         """
         return plt.imread(self.path.with_suffix(self.suffix))
 
 
-STORE_TYPE_MAPPING: Mapping[Type, _Store] = {
+STORE_TYPE_MAPPING: Mapping[Type, StoreProtocol] = {
     np.ndarray: NumpyStore,
     pd.DataFrame: PandasStore,
     pd.Series: PandasStore,
     xr.DataArray: XarrayStore,
     xr.Dataset: XarrayStore,
     plt.Figure: FigureStore,
 }
 
 #                                                  Loading and saving functions
 # =============================================================================
 
 
 def load_object(path: Path, experimentdata_directory: Path,
-                store_method: Type[_Store] = PickleStore) -> Any:
+                store_method: Type[StoreProtocol] = PickleStore) -> Any:
     """
     Load an object from disk from a given path and storing method
 
     Parameters
     ----------
     path : Path
         path of the object to load
@@ -277,28 +277,28 @@
         return None
 
     # Extract the suffix from the item's path
     item_suffix = _path.suffix
 
     # Use a generator expression to find the first matching store type,
     #  or None if no match is found
-    matched_store_type: _Store = next(
+    matched_store_type: StoreProtocol = next(
         (store_type for store_type in STORE_TYPE_MAPPING.values() if
          store_type.suffix == item_suffix), PickleStore)
 
     if matched_store_type:
         return matched_store_type(None, _path).load()
     else:
         # Handle the case when no matching suffix is found
         raise ValueError(
             f"No matching store type for item type: '{item_suffix}'")
 
 
 def save_object(object: Any, path: Path, experimentdata_directory: Path,
-                store_method: Optional[Type[_Store]] = None) -> str:
+                store_method: Optional[Type[StoreProtocol]] = None) -> str:
     """Function to save the object to path,
      with the appropriate storing method.
 
     Parameters
     ----------
     object : Any
         Object to store
@@ -324,20 +324,20 @@
         storage = store_method(object, _path)
         return
 
     # Check if object type is supported
     object_type = type(object)
 
     if object_type not in STORE_TYPE_MAPPING:
-        storage: _Store = PickleStore(object, _path)
+        storage: StoreProtocol = PickleStore(object, _path)
         logger.debug(f"Object type {object_type} is not natively supported. "
                      f"The default pickle storage method will be used.")
 
     else:
-        storage: _Store = STORE_TYPE_MAPPING[object_type](object, _path)
+        storage: StoreProtocol = STORE_TYPE_MAPPING[object_type](object, _path)
     # Store object
     storage.store()
     return storage.suffix
 
 
 def _project_dir_factory(project_dir: Path | str | None) -> Path:
     """Creates a Path object for the project directory from a particular input
```

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/experimentdata/_jobqueue.py` & `f3dasm-1.4.8/src/f3dasm/_src/experimentdata/_jobqueue.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/experimentdata/_newdata.py` & `f3dasm-1.4.8/src/f3dasm/_src/experimentdata/_newdata.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/experimentdata/experimentdata.py` & `f3dasm-1.4.8/src/f3dasm/_src/experimentdata/experimentdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 """
 
 #                                                                       Modules
 # =============================================================================
 
 from __future__ import annotations
 
-import sys
+import inspect
 # Standard
+import sys
 import traceback
 from functools import wraps
 from pathlib import Path
 from time import sleep
 from typing import (Any, Callable, Dict, Iterable, Iterator, List, Optional,
                     Tuple, Type)
 
@@ -29,27 +30,27 @@
 import xarray as xr
 from filelock import FileLock
 from hydra.utils import get_original_cwd
 from omegaconf import DictConfig
 from pathos.helpers import mp
 
 # Local
-from ..datageneration.datagenerator import DataGenerator
+from ..datageneration.datagenerator import DataGenerator, convert_function
 from ..datageneration.functions.function_factory import _datagenerator_factory
 from ..design.domain import Domain, _domain_factory
-from ..design.samplers import Sampler, SamplerNames, _sampler_factory
 from ..logger import logger
 from ..optimization import Optimizer
 from ..optimization.optimizer_factory import _optimizer_factory
 from ._data import DataTypes, _Data, _data_factory
 from ._io import (DOMAIN_FILENAME, EXPERIMENTDATA_SUBFOLDER,
                   INPUT_DATA_FILENAME, JOBS_FILENAME, LOCK_FILENAME, MAX_TRIES,
                   OUTPUT_DATA_FILENAME, _project_dir_factory)
 from ._jobqueue import NoOpenJobsError, Status, _jobs_factory
 from .experimentsample import ExperimentSample
+from .samplers import Sampler, SamplerNames, _sampler_factory
 from .utils import number_of_overiterations, number_of_updates
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
 __status__ = 'Stable'
@@ -289,15 +290,16 @@
                     f"Cannot find the folder {project_dir} !")
 
             return cls._from_file_attempt(filename_with_path)
 
     @classmethod
     def from_sampling(cls, sampler: Sampler | str, domain: Domain | DictConfig,
                       n_samples: int = 1,
-                      seed: Optional[int] = None) -> ExperimentData:
+                      seed: Optional[int] = None,
+                      **kwargs) -> ExperimentData:
         """Create an ExperimentData object from a sampler.
 
         Parameters
         ----------
         sampler : Sampler | str
             Sampler object containing the sampling strategy or one of the
             built-in sampler names.
@@ -320,17 +322,20 @@
         If a string is passed for the sampler argument, it should be one
         of the built-in samplers:
 
         * 'random' : Random sampling
         * 'latin' : Latin Hypercube Sampling
         * 'sobol' : Sobol Sequence Sampling
         * 'grid' : Grid Search Sampling
+
+        Any additional keyword arguments are passed to the sampler.
         """
         experimentdata = cls(domain=domain)
-        experimentdata.sample(sampler=sampler, n_samples=n_samples, seed=seed)
+        experimentdata.sample(
+            sampler=sampler, n_samples=n_samples, seed=seed, **kwargs)
         return experimentdata
 
     @classmethod
     def from_yaml(cls, config: DictConfig) -> ExperimentData:
         """Create an ExperimentData object from a hydra yaml configuration.
 
         Parameters
@@ -864,14 +869,33 @@
 
         if self._input_data.is_empty():
             self._output_data.reset_index()
         else:
             self._output_data.reset_index(self._input_data.indices)
         self._jobs.reset_index()
 
+    def join(self, other: ExperimentData) -> ExperimentData:
+        """Join two ExperimentData objects.
+
+        Parameters
+        ----------
+        other : ExperimentData
+            The other ExperimentData object to join with.
+
+        Returns
+        -------
+        ExperimentData
+            The joined ExperimentData object.
+        """
+        return ExperimentData(
+            input_data=self._input_data.join(other._input_data),
+            output_data=self._output_data.join(other._output_data),
+            jobs=self._jobs,
+            domain=self.domain + other.domain,
+            project_dir=self.project_dir)
 #                                                                  ExperimentSample
     # =============================================================================
 
     def get_experiment_sample(self, index: int) -> ExperimentSample:
         """
         Gets the experiment_sample at the given index.
 
@@ -1087,42 +1111,56 @@
         self.mark(indices=indices, status='open')
     #                                                            Datageneration
     # =========================================================================
 
     def evaluate(self, data_generator: DataGenerator,
                  mode: Literal['sequential', 'parallel',
                                'cluster', 'cluster_parallel'] = 'sequential',
-                 kwargs: Optional[dict] = None) -> None:
+                 kwargs: Optional[dict] = None,
+                 output_names: Optional[List[str]] = None) -> None:
         """Run any function over the entirety of the experiments
 
         Parameters
         ----------
         data_generator : DataGenerator
-            data grenerator to use
+            data generator to use
         mode : str, optional
             operational mode, by default 'sequential'. Choose between:
 
             * 'sequential' : Run the operation sequentially
             * 'parallel' : Run the operation on multiple cores
             * 'cluster' : Run the operation on the cluster
             * 'cluster_parallel' : Run the operation on the cluster in parallel
 
         kwargs, optional
             Any keyword arguments that need to
             be supplied to the function, by default None
+        output_names : List[str], optional
+            If you provide a function as data generator, you have to provide
+            the names of all the output parameters that are in the return
+            statement, in order of appearance.
 
         Raises
         ------
         ValueError
             Raised when invalid parallelization mode is specified
         """
         if kwargs is None:
             kwargs = {}
 
-        if isinstance(data_generator, str):
+        if inspect.isfunction(data_generator):
+            if output_names is None:
+                raise TypeError(
+                    ("If you provide a function as data generator, you have to"
+                     "provide the names of the return arguments with the"
+                     "output_names attribute."))
+            data_generator = convert_function(
+                f=data_generator, output=output_names)
+
+        elif isinstance(data_generator, str):
             data_generator = _datagenerator_factory(
                 data_generator, self.domain, kwargs)
 
         if mode.lower() == "sequential":
             return self._run_sequential(data_generator, kwargs)
         elif mode.lower() == "parallel":
             return self._run_multiprocessing(data_generator, kwargs)
@@ -1704,15 +1742,15 @@
         # Reset the optimizer
         optimizer.reset(ExperimentData(domain=self.domain))
 
     #                                                                  Sampling
     # =========================================================================
 
     def sample(self, sampler: Sampler | SamplerNames, n_samples: int = 1,
-               seed: Optional[int] = None) -> None:
+               seed: Optional[int] = None, **kwargs) -> None:
         """Sample data from the domain providing the sampler strategy
 
         Parameters
         ----------
         sampler: Sampler | str
             Sampler callable or string of built-in sampler
             If a string is passed, it should be one of the built-in samplers:
@@ -1722,25 +1760,36 @@
             * 'sobol' : Sobol Sequence Sampling
             * 'grid' : Grid Search Sampling
         n_samples : int, optional
             Number of samples to generate, by default 1
         seed : Optional[int], optional
             Seed to use for the sampler, by default None
 
+        Note
+        ----
+        When using the 'grid' sampler, an optional argument
+        'stepsize_continuous_parameters' can be passed to specify the stepsize
+        to cast continuous parameters to discrete parameters.
+
+        - The stepsize should be a dictionary with the parameter names as keys\
+        and the stepsize as values.
+        - Alternatively, a single stepsize can be passed for all continuous\
+        parameters.
+
         Raises
         ------
         ValueError
             Raised when invalid sampler type is specified
         """
 
         if isinstance(sampler, str):
             sampler = _sampler_factory(sampler, self.domain)
 
         sample_data: DataTypes = sampler(
-            domain=self.domain, n_samples=n_samples, seed=seed)
+            domain=self.domain, n_samples=n_samples, seed=seed, **kwargs)
         self.add(input_data=sample_data, domain=self.domain)
 
     #                                                         Project directory
     # =========================================================================
 
     def set_project_dir(self, project_dir: Path | str):
         """Set the directory of the f3dasm project folder.
```

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/experimentdata/experimentsample.py` & `f3dasm-1.4.8/src/f3dasm/_src/experimentdata/experimentsample.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # Third-party
 import autograd.numpy as np
 
 # Local
 from ..design.domain import Domain
 from ..logger import logger
-from ._io import _Store, load_object, save_object
+from ._io import StoreProtocol, load_object, save_object
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
 __status__ = 'Stable'
 # =============================================================================
@@ -144,15 +144,15 @@
                            for name in default_output_name}
         else:
             dict_output = {default_output_name: (output_value, False)}
 
         return dict_input, dict_output
 
     def get(self, item: str,
-            load_method: Optional[Type[_Store]] = None) -> Any:
+            load_method: Optional[Type[StoreProtocol]] = None) -> Any:
         """Retrieve a sample parameter by its name.
 
         Parameters
         ----------
         item : str
             name of the parameter
         load_method : Optional[Type[_Store]], optional
@@ -308,15 +308,15 @@
         Dict[str, Any]
             A dictionary containing the input and output data.
         """
         return {**self.input_data, **self.output_data,
                 'job_number': self.job_number}
 
     def store(self, name: str, object: Any, to_disk: bool = False,
-              store_method: Optional[Type[_Store]] = None) -> None:
+              store_method: Optional[Type[StoreProtocol]] = None) -> None:
         """Store an object to disk.
 
         Parameters
         ----------
 
         name : str
             The name of the file to store the object in.
@@ -336,16 +336,17 @@
         """
         if to_disk:
             self._store_to_disk(object=object, name=name,
                                 store_method=store_method)
         else:
             self._store_to_experimentdata(object=object, name=name)
 
-    def _store_to_disk(self, object: Any, name: str,
-                       store_method: Optional[Type[_Store]] = None) -> None:
+    def _store_to_disk(
+        self, object: Any, name: str,
+            store_method: Optional[Type[StoreProtocol]] = None) -> None:
         file_path = Path(name) / str(self.job_number)
 
         # Check if the file_dir exists
         (self._experimentdata_directory / Path(name)
          ).mkdir(parents=True, exist_ok=True)
 
         # Save the object to disk
```

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/experimentdata/utils.py` & `f3dasm-1.4.8/src/f3dasm/_src/experimentdata/utils.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/hydra_utils.py` & `f3dasm-1.4.8/src/f3dasm/_src/hydra_utils.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/logger.py` & `f3dasm-1.4.8/src/f3dasm/_src/logger.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/optimization/__init__.py` & `f3dasm-1.4.8/src/f3dasm/_src/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/optimization/adapters/scipy_implementations.py` & `f3dasm-1.4.8/src/f3dasm/_src/optimization/adapters/scipy_implementations.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/optimization/cg.py` & `f3dasm-1.4.8/src/f3dasm/_src/optimization/cg.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/optimization/lbfgsb.py` & `f3dasm-1.4.8/src/f3dasm/_src/optimization/lbfgsb.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/optimization/neldermead.py` & `f3dasm-1.4.8/src/f3dasm/_src/optimization/neldermead.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/optimization/optimizer.py` & `f3dasm-1.4.8/src/f3dasm/_src/optimization/optimizer.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/optimization/optimizer_factory.py` & `f3dasm-1.4.8/src/f3dasm/_src/optimization/optimizer_factory.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/optimization/randomsearch.py` & `f3dasm-1.4.8/src/f3dasm/_src/optimization/randomsearch.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/_src/run_optimization.py` & `f3dasm-1.4.8/src/f3dasm/_src/run_optimization.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/datageneration/__init__.py` & `f3dasm-1.4.8/src/f3dasm/datageneration/__init__.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/datageneration/abaqus.py` & `f3dasm-1.4.8/src/f3dasm/datageneration/abaqus.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/datageneration/functions.py` & `f3dasm-1.4.8/src/f3dasm/datageneration/functions.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/hydra_tools.py` & `f3dasm-1.4.8/src/f3dasm/hydra_tools.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm/optimization.py` & `f3dasm-1.4.8/src/f3dasm/optimization.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.4.71/src/f3dasm.egg-info/PKG-INFO` & `f3dasm-1.4.8/src/f3dasm.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f3dasm
-Version: 1.4.71
+Version: 1.4.8
 Summary: f3dasm - Framework for Data-driven development and Analysis of Structures and Materials
 Home-page: https://github.com/bessagroup/f3dasm
 Author: Martin van der Schelling
 Author-email: M.P.vanderSchelling@tudelft.nl
 License: BSD
 Project-URL: Documentation, https://f3dasm.readthedocs.io/
 Project-URL: Wiki, https://github.com/bessagroup/f3dasm/wiki
@@ -12,35 +12,37 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: xarray
 Requires-Dist: matplotlib
 Requires-Dist: hydra-core
 Requires-Dist: pathos>=0.3.0
 Requires-Dist: autograd
 Requires-Dist: SALib
 Requires-Dist: filelock
+Provides-Extra: benchmark
+Requires-Dist: abaqus2py==1.0.0; extra == "benchmark"
+Requires-Dist: f3dasm_optimize; extra == "benchmark"
 
 f3dasm
 ------
 *Framework for data-driven design \& analysis of structures and materials*
 
 ***
 
@@ -49,30 +51,54 @@
 [![GitHub license](https://img.shields.io/badge/license-BSD-blue)](https://github.com/bessagroup/f3dasm)
 [![Documentation Status](https://readthedocs.org/projects/f3dasm/badge/?version=latest)](https://f3dasm.readthedocs.io/en/latest/?badge=latest)
 
 [**Docs**](https://f3dasm.readthedocs.io/)
 | [**Installation**](https://f3dasm.readthedocs.io/en/latest/rst_doc_files/general/gettingstarted.html)
 | [**GitHub**](https://github.com/bessagroup/f3dasm)
 | [**PyPI**](https://pypi.org/project/f3dasm/)
-| [**Practical sessions**](https://github.com/mpvanderschelling/f3dasm_teach)
 
 ## Summary
 
-Welcome to `f3dasm`, a Python package for data-driven design and analysis of structures and materials.
+Welcome to `f3dasm`, a **f**ramework for **d**ata-**d**riven **d**esign and **a**nalysis of **s**tructures and **m**aterials.
 
+`f3dasm` introduces a general and user-friendly data-driven Python package for researchers and practitioners working on design and analysis of materials and structures. Some of the key features include:
+
+-  **Modular design** 
+    - The framework introduces flexible interfaces, allowing users to easily integrate their own models and algorithms.
+
+- **Automatic data management**
+    -  The framework automatically manages I/O processes, saving you time and effort implementing these common procedures.
+
+- **Easy parallelization**
+    - The framework manages parallelization of experiments, and is compatible with both local and high-performance cluster computing.
+
+- **Built-in defaults**
+    - The framework includes a collection of benchmark functions, optimization algorithms and sampling strategies to get you started right away!
+
+- **Hydra integration**
+    - The framework is supports the [hydra](https://hydra.cc/) configuration manager, to easily manage and run experiments.
+
+## Getting started
+
+The best way to get started is to follow the [installation instructions](https://f3dasm.readthedocs.io/en/latest/rst_doc_files/general/gettingstarted.html).
+
+## Illustrative benchmarks
+
+This package includes a collection of illustrative benchmark studies that demonstrate the capabilities of the framework. These studies are available in the `/studies` folder, and include the following studies:
+
+- Benchmarking optimization algorithms against well-known benchmark functions
+- 'Fragile Becomes Supercompressible' ([Bessa et al. (2019)](https://onlinelibrary.wiley.com/doi/full/10.1002/adma.201904845))
 
 ## Authorship
 
 * Current created and developer: [M.P. van der Schelling](https://github.com/mpvanderschelling/) (M.P.vanderSchelling@tudelft.nl)
 
 The Bessa research group at TU Delft is small... At the moment, we have limited availability to help future users/developers adapting the code to new problems, but we will do our best to help!
 
-## Getting started
 
-The best way to get started is to follow the [installation instructions](https://f3dasm.readthedocs.io/en/latest/rst_doc_files/general/gettingstarted.html).
 
 ## Referencing
 
 If you use or edit our work, please cite at least one of the appropriate references:
 
 [1] Bessa, M. A., Bostanabad, R., Liu, Z., Hu, A., Apley, D. W., Brinson, C., Chen, W., & Liu, W. K. (2017). A framework for data-driven analysis of materials under uncertainty: Countering the curse of dimensionality. Computer Methods in Applied Mechanics and Engineering, 320, 633-667.
 
@@ -84,12 +110,12 @@
 
 ## Community Support
 
 If you find any **issues, bugs or problems** with this template, please use the [GitHub issue tracker](https://github.com/bessagroup/f3dasm/issues) to report them.
 
 ## License
 
-Copyright 2023, Martin van der Schelling
+Copyright 2024, Martin van der Schelling
 
 All rights reserved.
 
 This project is licensed under the BSD 3-Clause License. See [LICENSE](https://github.com/bessagroup/f3dasm/blob/main/LICENSE) for the full license text.
```

### Comparing `f3dasm-1.4.71/src/f3dasm.egg-info/SOURCES.txt` & `f3dasm-1.4.8/src/f3dasm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -33,23 +33,23 @@
 src/f3dasm/_src/datageneration/functions/pybenchfunction.py
 src/f3dasm/_src/datageneration/functions/adapters/__init__.py
 src/f3dasm/_src/datageneration/functions/adapters/augmentor.py
 src/f3dasm/_src/datageneration/functions/adapters/pybenchfunction.py
 src/f3dasm/_src/design/__init__.py
 src/f3dasm/_src/design/domain.py
 src/f3dasm/_src/design/parameter.py
-src/f3dasm/_src/design/samplers.py
 src/f3dasm/_src/experimentdata/__init__.py
 src/f3dasm/_src/experimentdata/_columns.py
 src/f3dasm/_src/experimentdata/_data.py
 src/f3dasm/_src/experimentdata/_io.py
 src/f3dasm/_src/experimentdata/_jobqueue.py
 src/f3dasm/_src/experimentdata/_newdata.py
 src/f3dasm/_src/experimentdata/experimentdata.py
 src/f3dasm/_src/experimentdata/experimentsample.py
+src/f3dasm/_src/experimentdata/samplers.py
 src/f3dasm/_src/experimentdata/utils.py
 src/f3dasm/_src/machinelearning/__init__.py
 src/f3dasm/_src/optimization/__init__.py
 src/f3dasm/_src/optimization/cg.py
 src/f3dasm/_src/optimization/lbfgsb.py
 src/f3dasm/_src/optimization/neldermead.py
 src/f3dasm/_src/optimization/optimizer.py
```

### Comparing `f3dasm-1.4.71/tests/conftest.py` & `f3dasm-1.4.8/tests/conftest.py`

 * *Files identical despite different names*

