# Comparing `tmp/openai_priority_loadbalancer-1.0.2.tar.gz` & `tmp/openai_priority_loadbalancer-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_priority_loadbalancer-1.0.2.tar", last modified: Wed May 15 16:31:32 2024, max compression
+gzip compressed data, was "openai_priority_loadbalancer-1.0.3.tar", last modified: Thu May 16 14:33:36 2024, max compression
```

## Comparing `openai_priority_loadbalancer-1.0.2.tar` & `openai_priority_loadbalancer-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 16:31:32.846495 openai_priority_loadbalancer-1.0.2/
--rw-rw-rw-   0        0        0     1068 2024-05-11 18:48:22.000000 openai_priority_loadbalancer-1.0.2/LICENSE
--rw-rw-rw-   0        0        0    12172 2024-05-15 16:29:57.000000 openai_priority_loadbalancer-1.0.2/PACKAGE_README.md
--rw-rw-rw-   0        0        0    12811 2024-05-15 16:31:32.826688 openai_priority_loadbalancer-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    12216 2024-05-15 09:57:38.000000 openai_priority_loadbalancer-1.0.2/README.md
--rw-rw-rw-   0        0        0      711 2024-05-15 16:30:50.000000 openai_priority_loadbalancer-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-15 16:31:32.847207 openai_priority_loadbalancer-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-15 16:31:32.624682 openai_priority_loadbalancer-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-15 16:31:32.696539 openai_priority_loadbalancer-1.0.2/src/openai_priority_loadbalancer/
--rw-rw-rw-   0        0        0       45 2024-05-14 20:10:13.000000 openai_priority_loadbalancer-1.0.2/src/openai_priority_loadbalancer/__init__.py
--rw-rw-rw-   0        0        0    10355 2024-05-15 16:29:57.000000 openai_priority_loadbalancer-1.0.2/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:31:32.820889 openai_priority_loadbalancer-1.0.2/src/openai_priority_loadbalancer.egg-info/
--rw-rw-rw-   0        0        0    12811 2024-05-15 16:31:32.000000 openai_priority_loadbalancer-1.0.2/src/openai_priority_loadbalancer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      439 2024-05-15 16:31:32.000000 openai_priority_loadbalancer-1.0.2/src/openai_priority_loadbalancer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 16:31:32.000000 openai_priority_loadbalancer-1.0.2/src/openai_priority_loadbalancer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-15 16:31:32.000000 openai_priority_loadbalancer-1.0.2/src/openai_priority_loadbalancer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-05-15 16:31:32.000000 openai_priority_loadbalancer-1.0.2/src/openai_priority_loadbalancer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 14:33:36.049955 openai_priority_loadbalancer-1.0.3/
+-rw-rw-rw-   0        0        0     1068 2024-05-11 18:48:22.000000 openai_priority_loadbalancer-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0    12172 2024-05-15 16:29:57.000000 openai_priority_loadbalancer-1.0.3/PACKAGE_README.md
+-rw-rw-rw-   0        0        0    12811 2024-05-16 14:33:36.039540 openai_priority_loadbalancer-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    12397 2024-05-15 19:08:43.000000 openai_priority_loadbalancer-1.0.3/README.md
+-rw-rw-rw-   0        0        0      711 2024-05-16 14:32:56.000000 openai_priority_loadbalancer-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 14:33:36.050725 openai_priority_loadbalancer-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-16 14:33:35.934007 openai_priority_loadbalancer-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-16 14:33:35.961425 openai_priority_loadbalancer-1.0.3/src/openai_priority_loadbalancer/
+-rw-rw-rw-   0        0        0       45 2024-05-14 20:10:13.000000 openai_priority_loadbalancer-1.0.3/src/openai_priority_loadbalancer/__init__.py
+-rw-rw-rw-   0        0        0    13378 2024-05-16 14:20:36.000000 openai_priority_loadbalancer-1.0.3/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:33:36.029121 openai_priority_loadbalancer-1.0.3/src/openai_priority_loadbalancer.egg-info/
+-rw-rw-rw-   0        0        0    12811 2024-05-16 14:33:35.000000 openai_priority_loadbalancer-1.0.3/src/openai_priority_loadbalancer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2024-05-16 14:33:35.000000 openai_priority_loadbalancer-1.0.3/src/openai_priority_loadbalancer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 14:33:35.000000 openai_priority_loadbalancer-1.0.3/src/openai_priority_loadbalancer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-16 14:33:35.000000 openai_priority_loadbalancer-1.0.3/src/openai_priority_loadbalancer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-05-16 14:33:35.000000 openai_priority_loadbalancer-1.0.3/src/openai_priority_loadbalancer.egg-info/top_level.txt
```

### Comparing `openai_priority_loadbalancer-1.0.2/LICENSE` & `openai_priority_loadbalancer-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_priority_loadbalancer-1.0.2/PACKAGE_README.md` & `openai_priority_loadbalancer-1.0.3/PACKAGE_README.md`

 * *Files identical despite different names*

### Comparing `openai_priority_loadbalancer-1.0.2/PKG-INFO` & `openai_priority_loadbalancer-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_priority_loadbalancer
-Version: 1.0.2
+Version: 1.0.3
 Summary: A multi-backend, prioritization load balancer for OpenAI
 Author-email: Simon Kurtz <simonkurtz@gmail.com>
 Project-URL: Homepage, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer
 Project-URL: Issues, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openai_priority_loadbalancer-1.0.2/README.md` & `openai_priority_loadbalancer-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,17 @@
 ### Credentials
 
 Locally, your `AzureDefaultCredential` is used. Each Azure OpenAI instance must be configured with the `Cognitive Services OpenAI` User role for your Azure credential (the identity you use after logging in). This ensures that you can use your credential across all Azure OpenAI instances.
 
 When running in Azure, it's advised to use managed identities.
 
 1. Log in with `az login`.
+1. Set your subscription in which your Azure OpenAI assets reside: `az account set -s <name or id>`
+
+    *Missing this step may result in HTTP 400 errors for a tenant mismatch.*
 
 ## Execution
 
 1. Initially, [python-aoai.ps1](./python-aoai.ps1) once to ensure it executes correctly.
 1. Run [python-aoai.ps1](./python-aoai.ps1) concurrently in multiple terminals to simulate parallel requests from multiple python workers.
 
 ## Distribution of Requests
```

### Comparing `openai_priority_loadbalancer-1.0.2/pyproject.toml` & `openai_priority_loadbalancer-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "openai_priority_loadbalancer"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Simon Kurtz", email="simonkurtz@gmail.com" },
 ]
 description = "A multi-backend, prioritization load balancer for OpenAI"
 readme = "PACKAGE_README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `openai_priority_loadbalancer-1.0.2/src/openai_priority_loadbalancer.egg-info/PKG-INFO` & `openai_priority_loadbalancer-1.0.3/src/openai_priority_loadbalancer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_priority_loadbalancer
-Version: 1.0.2
+Version: 1.0.3
 Summary: A multi-backend, prioritization load balancer for OpenAI
 Author-email: Simon Kurtz <simonkurtz@gmail.com>
 Project-URL: Homepage, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer
 Project-URL: Issues, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

