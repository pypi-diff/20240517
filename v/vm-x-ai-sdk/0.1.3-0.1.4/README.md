# Comparing `tmp/vm_x_ai_sdk-0.1.3.tar.gz` & `tmp/vm_x_ai_sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vm_x_ai_sdk-0.1.3.tar", max compression
+gzip compressed data, was "vm_x_ai_sdk-0.1.4.tar", max compression
```

## Comparing `vm_x_ai_sdk-0.1.3.tar` & `vm_x_ai_sdk-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      885 2024-04-22 13:18:57.965987 vm_x_ai_sdk-0.1.3/README.md
--rw-r--r--   0        0        0     1427 2024-04-22 13:18:57.973986 vm_x_ai_sdk-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      714 2024-04-22 13:18:57.965987 vm_x_ai_sdk-0.1.3/vmxai/__init__.py
--rw-r--r--   0        0        0     1668 2024-04-22 13:18:57.965987 vm_x_ai_sdk-0.1.3/vmxai/auth/oauth.py
--rw-r--r--   0        0        0      373 2024-04-22 13:18:57.965987 vm_x_ai_sdk-0.1.3/vmxai/auth/provider.py
--rw-r--r--   0        0        0     1747 2024-04-22 13:18:57.965987 vm_x_ai_sdk-0.1.3/vmxai/client.py
--rw-r--r--   0        0        0       22 2024-04-22 13:18:57.965987 vm_x_ai_sdk-0.1.3/vmxai/protos/__init__.py
--rw-r--r--   0        0        0       33 2024-04-22 13:18:57.969987 vm_x_ai_sdk-0.1.3/vmxai/protos/completion/__init__.py
--rw-r--r--   0        0        0     1705 2024-04-22 13:18:57.969987 vm_x_ai_sdk-0.1.3/vmxai/protos/completion/completion.proto
--rw-r--r--   0        0        0     5194 2024-04-22 13:18:57.969987 vm_x_ai_sdk-0.1.3/vmxai/protos/completion/completion_pb2.py
--rw-r--r--   0        0        0     6034 2024-04-22 13:18:57.969987 vm_x_ai_sdk-0.1.3/vmxai/protos/completion/completion_pb2.pyi
--rw-r--r--   0        0        0     2771 2024-04-22 13:18:57.969987 vm_x_ai_sdk-0.1.3/vmxai/protos/completion/completion_pb2_grpc.py
--rw-r--r--   0        0        0     1862 1970-01-01 00:00:00.000000 vm_x_ai_sdk-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      885 2024-05-17 18:21:45.553249 vm_x_ai_sdk-0.1.4/README.md
+-rw-r--r--   0        0        0     1427 2024-05-17 18:21:45.561249 vm_x_ai_sdk-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      714 2024-05-17 18:21:45.553249 vm_x_ai_sdk-0.1.4/vmxai/__init__.py
+-rw-r--r--   0        0        0     1668 2024-05-17 18:21:45.557249 vm_x_ai_sdk-0.1.4/vmxai/auth/oauth.py
+-rw-r--r--   0        0        0      373 2024-05-17 18:21:45.557249 vm_x_ai_sdk-0.1.4/vmxai/auth/provider.py
+-rw-r--r--   0        0        0     1747 2024-05-17 18:21:45.557249 vm_x_ai_sdk-0.1.4/vmxai/client.py
+-rw-r--r--   0        0        0       22 2024-05-17 18:21:45.557249 vm_x_ai_sdk-0.1.4/vmxai/protos/__init__.py
+-rw-r--r--   0        0        0       33 2024-05-17 18:21:45.557249 vm_x_ai_sdk-0.1.4/vmxai/protos/completion/__init__.py
+-rw-r--r--   0        0        0     1705 2024-05-17 18:21:45.557249 vm_x_ai_sdk-0.1.4/vmxai/protos/completion/completion.proto
+-rw-r--r--   0        0        0     5194 2024-05-17 18:21:45.557249 vm_x_ai_sdk-0.1.4/vmxai/protos/completion/completion_pb2.py
+-rw-r--r--   0        0        0     6034 2024-05-17 18:21:45.557249 vm_x_ai_sdk-0.1.4/vmxai/protos/completion/completion_pb2.pyi
+-rw-r--r--   0        0        0     2771 2024-05-17 18:21:45.557249 vm_x_ai_sdk-0.1.4/vmxai/protos/completion/completion_pb2_grpc.py
+-rw-r--r--   0        0        0     1862 1970-01-01 00:00:00.000000 vm_x_ai_sdk-0.1.4/PKG-INFO
```

### Comparing `vm_x_ai_sdk-0.1.3/README.md` & `vm_x_ai_sdk-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `vm_x_ai_sdk-0.1.3/pyproject.toml` & `vm_x_ai_sdk-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 show_missing = true
 
 [tool.pytest.ini_options]
 addopts = "--cov --cov-report html:'../../coverage/packages/python/html' --cov-report xml:'../../coverage/packages/python/coverage.xml' --html='../../reports/packages/python/unittests/html/index.html' --junitxml='../../reports/packages/python/unittests/junit.xml'"
 
 [tool.poetry]
 name = "vm-x-ai-sdk"
-version = "0.1.3"
+version = "0.1.4"
 description = "VM-X Python SDK"
 authors = [ "VM-X Engineering <eng@vm-x.ai>" ]
 maintainers = [ "VM-X Engineering <eng@vm-x.ai>" ]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/vm-x-ai/vm-x-ai-sdk"
 keywords = [ "VM-X", "AI", "SDK", "Python" ]
```

### Comparing `vm_x_ai_sdk-0.1.3/vmxai/__init__.py` & `vm_x_ai_sdk-0.1.4/vmxai/__init__.py`

 * *Files identical despite different names*

### Comparing `vm_x_ai_sdk-0.1.3/vmxai/auth/oauth.py` & `vm_x_ai_sdk-0.1.4/vmxai/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `vm_x_ai_sdk-0.1.3/vmxai/client.py` & `vm_x_ai_sdk-0.1.4/vmxai/client.py`

 * *Files identical despite different names*

### Comparing `vm_x_ai_sdk-0.1.3/vmxai/protos/completion/completion.proto` & `vm_x_ai_sdk-0.1.4/vmxai/protos/completion/completion.proto`

 * *Files identical despite different names*

### Comparing `vm_x_ai_sdk-0.1.3/vmxai/protos/completion/completion_pb2.py` & `vm_x_ai_sdk-0.1.4/vmxai/protos/completion/completion_pb2.py`

 * *Files identical despite different names*

### Comparing `vm_x_ai_sdk-0.1.3/vmxai/protos/completion/completion_pb2.pyi` & `vm_x_ai_sdk-0.1.4/vmxai/protos/completion/completion_pb2.pyi`

 * *Files identical despite different names*

### Comparing `vm_x_ai_sdk-0.1.3/vmxai/protos/completion/completion_pb2_grpc.py` & `vm_x_ai_sdk-0.1.4/vmxai/protos/completion/completion_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `vm_x_ai_sdk-0.1.3/PKG-INFO` & `vm_x_ai_sdk-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vm-x-ai-sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: VM-X Python SDK
 Home-page: https://github.com/vm-x-ai/vm-x-ai-sdk
 License: MIT
 Keywords: VM-X,AI,SDK,Python
 Author: VM-X Engineering
 Author-email: eng@vm-x.ai
 Maintainer: VM-X Engineering
```

