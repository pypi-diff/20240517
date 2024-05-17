# Comparing `tmp/cybsi_cloud_sdk-1.1.1.tar.gz` & `tmp/cybsi_cloud_sdk-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybsi_cloud_sdk-1.1.1.tar", max compression
+gzip compressed data, was "cybsi_cloud_sdk-1.1.2.tar", max compression
```

## Comparing `cybsi_cloud_sdk-1.1.1.tar` & `cybsi_cloud_sdk-1.1.2.tar`

### file list

```diff
@@ -1,40 +1,39 @@
--rw-r--r--   0        0        0    10142 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/LICENSE
--rw-r--r--   0        0        0      626 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/README.md
--rw-r--r--   0        0        0      151 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/__init__.py
--rw-r--r--   0        0        0      195 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/__version__.py
--rw-r--r--   0        0        0      405 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/__init__.py
--rw-r--r--   0        0        0     1362 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/api.py
--rw-r--r--   0        0        0      539 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/auth/__init__.py
--rw-r--r--   0        0        0      412 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/auth/api.py
--rw-r--r--   0        0        0     8864 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/auth/api_key.py
--rw-r--r--   0        0        0     1814 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/auth/limits.py
--rw-r--r--   0        0        0     1551 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/auth/permission.py
--rw-r--r--   0        0        0     2159 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/auth/resource.py
--rw-r--r--   0        0        0      821 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/auth/token.py
--rw-r--r--   0        0        0     4393 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/client.py
--rw-r--r--   0        0        0     5631 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/client_config.py
--rw-r--r--   0        0        0      829 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/enum.py
--rw-r--r--   0        0        0     9679 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/error.py
--rw-r--r--   0        0        0      306 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/files/__init__.py
--rw-r--r--   0        0        0    23274 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/files/files.py
--rw-r--r--   0        0        0      541 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/insight/__init__.py
--rw-r--r--   0        0        0     1178 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/insight/api.py
--rw-r--r--   0        0        0     8823 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/insight/schemas.py
--rw-r--r--   0        0        0     7897 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/insight/task_queue.py
--rw-r--r--   0        0        0     7637 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/insight/tasks.py
--rw-r--r--   0        0        0      257 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/internal/__init__.py
--rw-r--r--   0        0        0     2046 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/internal/base.py
--rw-r--r--   0        0        0     8226 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/internal/buffer.py
--rw-r--r--   0        0        0     7192 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/internal/connector.py
--rw-r--r--   0        0        0     1755 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/internal/multipart.py
--rw-r--r--   0        0        0      870 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/internal/time.py
--rw-r--r--   0        0        0      595 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/iocean/__init__.py
--rw-r--r--   0        0        0     1200 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/iocean/api.py
--rw-r--r--   0        0        0     9771 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/iocean/collection.py
--rw-r--r--   0        0        0    15217 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/iocean/objects.py
--rw-r--r--   0        0        0     8513 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/iocean/schemas.py
--rw-r--r--   0        0        0     4302 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/pagination.py
--rw-r--r--   0        0        0      520 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/cloud/view.py
--rw-r--r--   0        0        0        0 2024-05-14 08:45:22.081479 cybsi_cloud_sdk-1.1.1/cybsi/py.typed
--rw-r--r--   0        0        0     1163 2024-05-14 08:45:22.085479 cybsi_cloud_sdk-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1284 1970-01-01 00:00:00.000000 cybsi_cloud_sdk-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    10142 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/LICENSE
+-rw-r--r--   0        0        0      626 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/README.md
+-rw-r--r--   0        0        0      557 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/__init__.py
+-rw-r--r--   0        0        0      195 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/__version__.py
+-rw-r--r--   0        0        0     1362 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/api.py
+-rw-r--r--   0        0        0      539 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/auth/__init__.py
+-rw-r--r--   0        0        0      412 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/auth/api.py
+-rw-r--r--   0        0        0     8864 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/auth/api_key.py
+-rw-r--r--   0        0        0     1814 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/auth/limits.py
+-rw-r--r--   0        0        0     1551 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/auth/permission.py
+-rw-r--r--   0        0        0     2159 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/auth/resource.py
+-rw-r--r--   0        0        0      821 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/auth/token.py
+-rw-r--r--   0        0        0     4393 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/client.py
+-rw-r--r--   0        0        0     5631 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/client_config.py
+-rw-r--r--   0        0        0      829 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/enum.py
+-rw-r--r--   0        0        0     9679 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/error.py
+-rw-r--r--   0        0        0      306 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/files/__init__.py
+-rw-r--r--   0        0        0    23274 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/files/files.py
+-rw-r--r--   0        0        0      541 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/insight/__init__.py
+-rw-r--r--   0        0        0     1178 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/insight/api.py
+-rw-r--r--   0        0        0     8823 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/insight/schemas.py
+-rw-r--r--   0        0        0     7897 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/insight/task_queue.py
+-rw-r--r--   0        0        0     7637 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/insight/tasks.py
+-rw-r--r--   0        0        0      257 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/internal/__init__.py
+-rw-r--r--   0        0        0     2046 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/internal/base.py
+-rw-r--r--   0        0        0     8226 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/internal/buffer.py
+-rw-r--r--   0        0        0     7198 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/internal/connector.py
+-rw-r--r--   0        0        0     1755 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/internal/multipart.py
+-rw-r--r--   0        0        0      870 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/internal/time.py
+-rw-r--r--   0        0        0      595 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/iocean/__init__.py
+-rw-r--r--   0        0        0     1200 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/iocean/api.py
+-rw-r--r--   0        0        0     9771 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/iocean/collection.py
+-rw-r--r--   0        0        0    15217 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/iocean/objects.py
+-rw-r--r--   0        0        0     8513 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/iocean/schemas.py
+-rw-r--r--   0        0        0     4302 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/pagination.py
+-rw-r--r--   0        0        0        0 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/py.typed
+-rw-r--r--   0        0        0      520 2024-05-17 04:56:28.892899 cybsi_cloud_sdk-1.1.2/cybsi/cloud/view.py
+-rw-r--r--   0        0        0     1175 2024-05-17 04:56:28.896899 cybsi_cloud_sdk-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1284 1970-01-01 00:00:00.000000 cybsi_cloud_sdk-1.1.2/PKG-INFO
```

### Comparing `cybsi_cloud_sdk-1.1.1/LICENSE` & `cybsi_cloud_sdk-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/README.md` & `cybsi_cloud_sdk-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/api.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/api.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/auth/__init__.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/auth/api_key.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/auth/api_key.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/auth/limits.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/auth/limits.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/auth/permission.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/auth/permission.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/auth/resource.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/auth/resource.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/auth/token.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/auth/token.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/client.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/client.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/client_config.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/client_config.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/enum.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/enum.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/error.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/error.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/files/files.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/files/files.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/insight/__init__.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/insight/__init__.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/insight/api.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/insight/api.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/insight/schemas.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/insight/schemas.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/insight/task_queue.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/insight/task_queue.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/insight/tasks.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/insight/tasks.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/internal/base.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/internal/base.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/internal/buffer.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/internal/buffer.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/internal/connector.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/internal/connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Optional
 
 import httpx
 
-from cybsi.__version__ import __version__
+from cybsi.cloud.__version__ import __version__
 
 from ..api import Tag
 from ..error import CybsiError, _raise_cybsi_error
 from ..internal.multipart import apply_async_multipart_stream
 
 _BASIC_HEADERS = {
     "User-Agent": f"cybsi-cloud-client/v{__version__}",
```

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/internal/multipart.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/internal/multipart.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/internal/time.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/internal/time.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/iocean/__init__.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/iocean/__init__.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/iocean/api.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/iocean/api.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/iocean/collection.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/iocean/collection.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/iocean/objects.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/iocean/objects.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/iocean/schemas.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/iocean/schemas.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/pagination.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/pagination.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/cybsi/cloud/view.py` & `cybsi_cloud_sdk-1.1.2/cybsi/cloud/view.py`

 * *Files identical despite different names*

### Comparing `cybsi_cloud_sdk-1.1.1/pyproject.toml` & `cybsi_cloud_sdk-1.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "cybsi-cloud-sdk"
-version = "1.1.1"
+version = "1.1.2"
 description = "Cybsi Cloud development kit"
 authors = ["Cybsi Cloud developers"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [
-    { include = "cybsi" },
+    { include = "cybsi/cloud" },
 ]
-include = ["cybsi/py.typed"]
+include = ["cybsi/cloud/py.typed"]
 
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4"
 enum-tools = "0.11.0"
 httpx = "^0.25.1"
 typing-extensions = "^4.8.0"
```

### Comparing `cybsi_cloud_sdk-1.1.1/PKG-INFO` & `cybsi_cloud_sdk-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybsi-cloud-sdk
-Version: 1.1.1
+Version: 1.1.2
 Summary: Cybsi Cloud development kit
 License: Apache-2.0
 Author: Cybsi Cloud developers
 Requires-Python: >=3.8.1,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

