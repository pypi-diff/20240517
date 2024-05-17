# Comparing `tmp/nix_gpt_client-0.1.0.tar.gz` & `tmp/nix_gpt_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nix_gpt_client-0.1.0.tar", last modified: Mon May  6 14:36:34 2024, max compression
+gzip compressed data, was "nix_gpt_client-0.1.1.tar", last modified: Fri May 17 12:16:05 2024, max compression
```

## Comparing `nix_gpt_client-0.1.0.tar` & `nix_gpt_client-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-06 14:36:34.460471 nix_gpt_client-0.1.0/
--rw-r--r--   0 nix       (1000) nix       (1000)     1063 2024-05-06 13:36:34.000000 nix_gpt_client-0.1.0/LICENCE
--rw-r--r--   0 nix       (1000) nix       (1000)     4163 2024-05-06 14:36:34.460471 nix_gpt_client-0.1.0/PKG-INFO
--rw-r--r--   0 nix       (1000) nix       (1000)     3470 2024-05-06 14:34:03.000000 nix_gpt_client-0.1.0/README.md
--rw-r--r--   0 nix       (1000) nix       (1000)      832 2024-05-06 14:26:27.000000 nix_gpt_client-0.1.0/pyproject.toml
--rw-r--r--   0 nix       (1000) nix       (1000)       38 2024-05-06 14:36:34.460471 nix_gpt_client-0.1.0/setup.cfg
-drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-06 14:36:34.460471 nix_gpt_client-0.1.0/src/
--rw-r--r--   0 nix       (1000) nix       (1000)        0 2024-05-06 14:33:45.000000 nix_gpt_client-0.1.0/src/__init__.py
-drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-06 14:36:34.460471 nix_gpt_client-0.1.0/src/nix/
--rw-r--r--   0 nix       (1000) nix       (1000)        0 2024-05-06 14:33:10.000000 nix_gpt_client-0.1.0/src/nix/__init__.py
-drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-06 14:36:34.460471 nix_gpt_client-0.1.0/src/nix/gptclient/
--rw-r--r--   0 nix       (1000) nix       (1000)       95 2024-05-06 14:31:38.000000 nix_gpt_client-0.1.0/src/nix/gptclient/__init__.py
--rw-r--r--   0 nix       (1000) nix       (1000)     2026 2024-05-06 14:01:53.000000 nix_gpt_client-0.1.0/src/nix/gptclient/_gpt_client.py
--rw-r--r--   0 nix       (1000) nix       (1000)      239 2024-05-06 12:37:40.000000 nix_gpt_client-0.1.0/src/nix/gptclient/_types.py
--rw-r--r--   0 nix       (1000) nix       (1000)      654 2024-05-06 13:59:31.000000 nix_gpt_client-0.1.0/src/nix/gptclient/_validate.py
-drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-06 14:36:34.460471 nix_gpt_client-0.1.0/src/nix_gpt_client.egg-info/
--rw-r--r--   0 nix       (1000) nix       (1000)     4163 2024-05-06 14:36:34.000000 nix_gpt_client-0.1.0/src/nix_gpt_client.egg-info/PKG-INFO
--rw-r--r--   0 nix       (1000) nix       (1000)      399 2024-05-06 14:36:34.000000 nix_gpt_client-0.1.0/src/nix_gpt_client.egg-info/SOURCES.txt
--rw-r--r--   0 nix       (1000) nix       (1000)        1 2024-05-06 14:36:34.000000 nix_gpt_client-0.1.0/src/nix_gpt_client.egg-info/dependency_links.txt
--rw-r--r--   0 nix       (1000) nix       (1000)        7 2024-05-06 14:36:34.000000 nix_gpt_client-0.1.0/src/nix_gpt_client.egg-info/requires.txt
--rw-r--r--   0 nix       (1000) nix       (1000)       13 2024-05-06 14:36:34.000000 nix_gpt_client-0.1.0/src/nix_gpt_client.egg-info/top_level.txt
+drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-17 12:16:05.263619 nix_gpt_client-0.1.1/
+-rw-r--r--   0 nix       (1000) nix       (1000)     1063 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.1/LICENCE
+-rw-r--r--   0 nix       (1000) nix       (1000)     4163 2024-05-17 12:16:05.263619 nix_gpt_client-0.1.1/PKG-INFO
+-rw-r--r--   0 nix       (1000) nix       (1000)     3470 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.1/README.md
+-rw-r--r--   0 nix       (1000) nix       (1000)      832 2024-05-17 12:10:31.000000 nix_gpt_client-0.1.1/pyproject.toml
+-rw-r--r--   0 nix       (1000) nix       (1000)       38 2024-05-17 12:16:05.263619 nix_gpt_client-0.1.1/setup.cfg
+drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-17 12:16:05.260286 nix_gpt_client-0.1.1/src/
+-rw-r--r--   0 nix       (1000) nix       (1000)        0 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.1/src/__init__.py
+drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-17 12:16:05.260286 nix_gpt_client-0.1.1/src/nix/
+-rw-r--r--   0 nix       (1000) nix       (1000)        0 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.1/src/nix/__init__.py
+drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-17 12:16:05.260286 nix_gpt_client-0.1.1/src/nix/gptclient/
+-rw-r--r--   0 nix       (1000) nix       (1000)       95 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.1/src/nix/gptclient/__init__.py
+-rw-r--r--   0 nix       (1000) nix       (1000)     2026 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.1/src/nix/gptclient/_gpt_client.py
+-rw-r--r--   0 nix       (1000) nix       (1000)      680 2024-05-17 12:09:50.000000 nix_gpt_client-0.1.1/src/nix/gptclient/_types.py
+-rw-r--r--   0 nix       (1000) nix       (1000)      654 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.1/src/nix/gptclient/_validate.py
+drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-17 12:16:05.260286 nix_gpt_client-0.1.1/src/nix_gpt_client.egg-info/
+-rw-r--r--   0 nix       (1000) nix       (1000)     4163 2024-05-17 12:16:05.000000 nix_gpt_client-0.1.1/src/nix_gpt_client.egg-info/PKG-INFO
+-rw-r--r--   0 nix       (1000) nix       (1000)      399 2024-05-17 12:16:05.000000 nix_gpt_client-0.1.1/src/nix_gpt_client.egg-info/SOURCES.txt
+-rw-r--r--   0 nix       (1000) nix       (1000)        1 2024-05-17 12:16:05.000000 nix_gpt_client-0.1.1/src/nix_gpt_client.egg-info/dependency_links.txt
+-rw-r--r--   0 nix       (1000) nix       (1000)        7 2024-05-17 12:16:05.000000 nix_gpt_client-0.1.1/src/nix_gpt_client.egg-info/requires.txt
+-rw-r--r--   0 nix       (1000) nix       (1000)       13 2024-05-17 12:16:05.000000 nix_gpt_client-0.1.1/src/nix_gpt_client.egg-info/top_level.txt
```

### Comparing `nix_gpt_client-0.1.0/LICENCE` & `nix_gpt_client-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `nix_gpt_client-0.1.0/PKG-INFO` & `nix_gpt_client-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nix-gpt-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library for easy interaction with the GPT API, featuring typed requests and responses.
 Author-email: nks_nix <nikusunix@gmail.com>
 Maintainer-email: nks_nix <nikusunix@gmail.com>
 Project-URL: Homepage, https://github.com/nixnks/nix-gpt-client
 Project-URL: Documentation, https://readthedocs.org
 Project-URL: Repository, https://github.com/nixnks/nix-gpt-client.git
 Project-URL: Changelog, https://github.com/nixnks/nix-gpt-client/CHANGELOG.md
```

### Comparing `nix_gpt_client-0.1.0/README.md` & `nix_gpt_client-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nix_gpt_client-0.1.0/pyproject.toml` & `nix_gpt_client-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nix-gpt-client"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
     "openai"
 ]
 requires-python = ">=3.11"
 authors = [
     { name = "nks_nix", email = "nikusunix@gmail.com" },
 ]
```

### Comparing `nix_gpt_client-0.1.0/src/nix/gptclient/_gpt_client.py` & `nix_gpt_client-0.1.1/src/nix/gptclient/_gpt_client.py`

 * *Files identical despite different names*

### Comparing `nix_gpt_client-0.1.0/src/nix/gptclient/_validate.py` & `nix_gpt_client-0.1.1/src/nix/gptclient/_validate.py`

 * *Files identical despite different names*

### Comparing `nix_gpt_client-0.1.0/src/nix_gpt_client.egg-info/PKG-INFO` & `nix_gpt_client-0.1.1/src/nix_gpt_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nix-gpt-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library for easy interaction with the GPT API, featuring typed requests and responses.
 Author-email: nks_nix <nikusunix@gmail.com>
 Maintainer-email: nks_nix <nikusunix@gmail.com>
 Project-URL: Homepage, https://github.com/nixnks/nix-gpt-client
 Project-URL: Documentation, https://readthedocs.org
 Project-URL: Repository, https://github.com/nixnks/nix-gpt-client.git
 Project-URL: Changelog, https://github.com/nixnks/nix-gpt-client/CHANGELOG.md
```

