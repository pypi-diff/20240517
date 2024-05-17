# Comparing `tmp/planqk-quantum-2.3.0.tar.gz` & `tmp/planqk-quantum-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planqk-quantum-2.3.0.tar", last modified: Fri Apr 26 15:51:03 2024, max compression
+gzip compressed data, was "planqk-quantum-2.3.1.tar", last modified: Fri May 17 17:20:46 2024, max compression
```

## Comparing `planqk-quantum-2.3.0.tar` & `planqk-quantum-2.3.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:51:03.957325 planqk-quantum-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-26 15:51:03.957325 planqk-quantum-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:51:03.949325 planqk-quantum-2.3.0/planqk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:51:03.953325 planqk-quantum-2.3.0/planqk/dwave/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/dwave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/dwave/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:51:03.953325 planqk-quantum-2.3.0/planqk/qiskit/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:51:03.953325 planqk-quantum-2.3.0/planqk/qiskit/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/client/backend_dtos.py
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/client/dto_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/client/job_dtos.py
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/planqk_runtime_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:51:03.953325 planqk-quantum-2.3.0/planqk/qiskit/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:51:03.953325 planqk-quantum-2.3.0/planqk/qiskit/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/aws/aws_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/aws_converters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:51:03.953325 planqk-quantum-2.3.0/planqk/qiskit/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/azure/azure_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/azure/ionq_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:51:03.957325 planqk-quantum-2.3.0/planqk/qiskit/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/ibm/ibm_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/ibm/ibm_provider_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/ibm/ibm_runtime_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:51:03.957325 planqk-quantum-2.3.0/planqk/qiskit/providers/qryd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/qryd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/qryd/pcp_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/qryd/pcz_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/qryd/qryd_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    13352 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/providers/qryd/qryd_converter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/planqk/qiskit/runtime_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:51:03.957325 planqk-quantum-2.3.0/planqk_quantum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-26 15:51:03.000000 planqk-quantum-2.3.0/planqk_quantum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-26 15:51:03.000000 planqk-quantum-2.3.0/planqk_quantum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:51:03.000000 planqk-quantum-2.3.0/planqk_quantum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-26 15:51:03.000000 planqk-quantum-2.3.0/planqk_quantum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-26 15:51:03.000000 planqk-quantum-2.3.0/planqk_quantum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:51:03.957325 planqk-quantum-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-26 15:50:53.000000 planqk-quantum-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:20:46.377042 planqk-quantum-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-05-17 17:20:46.377042 planqk-quantum-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:20:46.369042 planqk-quantum-2.3.1/planqk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:20:46.369042 planqk-quantum-2.3.1/planqk/dwave/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/dwave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/dwave/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:20:46.373041 planqk-quantum-2.3.1/planqk/qiskit/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:20:46.373041 planqk-quantum-2.3.1/planqk/qiskit/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/client/backend_dtos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/client/dto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/client/job_dtos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/planqk_runtime_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:20:46.373041 planqk-quantum-2.3.1/planqk/qiskit/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:20:46.373041 planqk-quantum-2.3.1/planqk/qiskit/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/providers/aws/aws_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/providers/aws_converters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:20:46.373041 planqk-quantum-2.3.1/planqk/qiskit/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/providers/azure/azure_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/providers/azure/ionq_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:20:46.373041 planqk-quantum-2.3.1/planqk/qiskit/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/providers/ibm/ibm_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/providers/ibm/ibm_provider_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/providers/ibm/ibm_runtime_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:20:46.373041 planqk-quantum-2.3.1/planqk/qiskit/providers/qryd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/providers/qryd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/providers/qryd/pcp_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/providers/qryd/pcz_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/providers/qryd/qryd_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13352 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/providers/qryd/qryd_converter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/planqk/qiskit/runtime_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:20:46.377042 planqk-quantum-2.3.1/planqk_quantum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-05-17 17:20:46.000000 planqk-quantum-2.3.1/planqk_quantum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-17 17:20:46.000000 planqk-quantum-2.3.1/planqk_quantum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 17:20:46.000000 planqk-quantum-2.3.1/planqk_quantum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-17 17:20:46.000000 planqk-quantum-2.3.1/planqk_quantum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 17:20:46.000000 planqk-quantum-2.3.1/planqk_quantum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 17:20:46.377042 planqk-quantum-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-17 17:20:37.000000 planqk-quantum-2.3.1/setup.py
```

### Comparing `planqk-quantum-2.3.0/LICENSE` & `planqk-quantum-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.3.0/PKG-INFO` & `planqk-quantum-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planqk-quantum
-Version: 2.3.0
+Version: 2.3.1
 Summary: Python SDK for the PlanQK Platform
 Home-page: https://github.com/planqk/planqk-quantum
 Author: Anaqor AG
 Author-email: info@anaqor.io
 License: apache-2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `planqk-quantum-2.3.0/README.md` & `planqk-quantum-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.3.0/planqk/context.py` & `planqk-quantum-2.3.1/planqk/context.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.3.0/planqk/credentials.py` & `planqk-quantum-2.3.1/planqk/credentials.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.3.0/planqk/dwave/provider.py` & `planqk-quantum-2.3.1/planqk/dwave/provider.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.3.0/planqk/exceptions.py` & `planqk-quantum-2.3.1/planqk/exceptions.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.3.0/planqk/qiskit/backend.py` & `planqk-quantum-2.3.1/planqk/qiskit/backend.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.3.0/planqk/qiskit/client/backend_dtos.py` & `planqk-quantum-2.3.1/planqk/qiskit/client/backend_dtos.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.3.0/planqk/qiskit/client/client.py` & `planqk-quantum-2.3.1/planqk/qiskit/client/client.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.3.0/planqk/qiskit/client/job_dtos.py` & `planqk-quantum-2.3.1/planqk/qiskit/client/job_dtos.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.3.0/planqk/qiskit/job.py` & `planqk-quantum-2.3.1/planqk/qiskit/job.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.3.0/planqk/qiskit/options.py` & `planqk-quantum-2.3.1/planqk/qiskit/options.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.3.0/planqk/qiskit/planqk_runtime_job.py` & `planqk-quantum-2.3.1/planqk/qiskit/planqk_runtime_job.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.3.0/planqk/qiskit/provider.py` & `planqk-quantum-2.3.1/planqk/qiskit/provider.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.3.0/planqk/qiskit/providers/aws/aws_backend.py` & `planqk-quantum-2.3.1/planqk/qiskit/providers/aws/aws_backend.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.3.0/planqk/qiskit/providers/aws_converters.py` & `planqk-quantum-2.3.1/planqk/qiskit/providers/aws_converters.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.3.0/planqk/qiskit/providers/azure/azure_backend.py` & `planqk-quantum-2.3.1/planqk/qiskit/providers/azure/azure_backend.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.3.0/planqk/qiskit/providers/ibm/ibm_backend.py` & `planqk-quantum-2.3.1/planqk/qiskit/providers/ibm/ibm_backend.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.3.0/planqk/qiskit/providers/ibm/ibm_provider_backend.py` & `planqk-quantum-2.3.1/planqk/qiskit/providers/ibm/ibm_provider_backend.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 import json
 from typing import Dict
 from typing import Optional, List
 
-from qiskit import QuantumCircuit
-from qiskit.providers.models import BackendStatus
-from qiskit_ibm_provider import IBMBackend
-from qiskit_ibm_provider.job import IBMCircuitJob
-from qiskit_ibm_provider.utils import RuntimeEncoder
-
 from planqk.qiskit import PlanqkJob
 from planqk.qiskit.client.backend_dtos import STATUS
 from planqk.qiskit.client.client import _PlanqkClient
 from planqk.qiskit.client.job_dtos import JobDto, INPUT_FORMAT, RuntimeJobParamsDto
 from planqk.qiskit.planqk_runtime_job import PlanqkRuntimeJob
 from planqk.qiskit.providers.ibm.ibm_backend import PlanqkIbmBackend
+from qiskit import QuantumCircuit
+from qiskit.providers.models import BackendStatus
+from qiskit_ibm_provider import IBMBackend
+from qiskit_ibm_provider.job import IBMCircuitJob
+from qiskit_ibm_provider.utils import RuntimeEncoder
 
 
 def _encode_circuit_base64(circuit: QuantumCircuit):
     # Transforms circuit to base64 encoded byte stream
     input_json_str = json.dumps(circuit, cls=RuntimeEncoder)
     # Transform back to json but with the base64 encoded byte stream
     return json.loads(input_json_str)
 
 
 class PlanqkIbmProviderBackend(PlanqkIbmBackend):
 
     def __init__(self, **kwargs):
         PlanqkIbmBackend.__init__(self, **kwargs)
-        self.ibm_backend = IBMBackend(configuration=self.configuration(), provider=None, api_client=None)
+        self.ibm_backend = IBMBackend(configuration=self.configuration(),
+                                      provider=kwargs.get('provider'),
+                                      api_client=None)
         self.ibm_backend._runtime_run = self._submit_job
+        self.ibm_backend.properties = self._backend_properties
         self.ibm_backend.status = self.status
 
     def run(self, circuit, **kwargs) -> PlanqkRuntimeJob:
         return IBMBackend.run(self.ibm_backend, circuit, **kwargs)
 
     def status(self):
         operational = self.backend_info.status == STATUS.ONLINE
@@ -66,10 +68,14 @@
                              input_format=INPUT_FORMAT.QISKIT,
                              input=encoded_input,
                              shots=inputs.get('shots'),
                              input_params=runtime_job_params.dict())
 
         return PlanqkRuntimeJob(backend=self, job_details=job_request)
 
+    def _backend_properties(self):
+        # Supported for loading dynamic properties currently not supported
+        return None;
+
     def retrieve_job(self, job_id: str) -> PlanqkJob:
         job_details = _PlanqkClient.get_job(job_id)
         return PlanqkRuntimeJob(backend=self, job_id=job_id, job_details=job_details)
```

### Comparing `planqk-quantum-2.3.0/planqk/qiskit/providers/qryd/pcp_gate.py` & `planqk-quantum-2.3.1/planqk/qiskit/providers/qryd/pcp_gate.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.3.0/planqk/qiskit/providers/qryd/pcz_gate.py` & `planqk-quantum-2.3.1/planqk/qiskit/providers/qryd/pcz_gate.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.3.0/planqk/qiskit/providers/qryd/qryd_backend.py` & `planqk-quantum-2.3.1/planqk/qiskit/providers/qryd/qryd_backend.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.3.0/planqk/qiskit/providers/qryd/qryd_converter_utils.py` & `planqk-quantum-2.3.1/planqk/qiskit/providers/qryd/qryd_converter_utils.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.3.0/planqk/qiskit/runtime_provider.py` & `planqk-quantum-2.3.1/planqk/qiskit/runtime_provider.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.3.0/planqk_quantum.egg-info/PKG-INFO` & `planqk-quantum-2.3.1/planqk_quantum.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planqk-quantum
-Version: 2.3.0
+Version: 2.3.1
 Summary: Python SDK for the PlanQK Platform
 Home-page: https://github.com/planqk/planqk-quantum
 Author: Anaqor AG
 Author-email: info@anaqor.io
 License: apache-2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `planqk-quantum-2.3.0/planqk_quantum.egg-info/SOURCES.txt` & `planqk-quantum-2.3.1/planqk_quantum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.3.0/setup.py` & `planqk-quantum-2.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('./requirements.txt', 'r') as fh:
     requirements = fh.readlines()
 
 setup(
     name='planqk-quantum',
-    version="2.3.0",
+    version="2.3.1",
     author='Anaqor AG',
     author_email='info@anaqor.io',
     url='https://github.com/planqk/planqk-quantum',
     description='Python SDK for the PlanQK Platform',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_namespace_packages(include=['planqk', 'planqk.*']),
```

