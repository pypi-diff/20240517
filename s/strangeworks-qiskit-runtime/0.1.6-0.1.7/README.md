# Comparing `tmp/strangeworks_qiskit_runtime-0.1.6.tar.gz` & `tmp/strangeworks_qiskit_runtime-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_qiskit_runtime-0.1.6.tar", max compression
+gzip compressed data, was "strangeworks_qiskit_runtime-0.1.7.tar", max compression
```

## Comparing `strangeworks_qiskit_runtime-0.1.6.tar` & `strangeworks_qiskit_runtime-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      204 2024-02-28 17:08:15.653387 strangeworks_qiskit_runtime-0.1.6/README.md
--rw-r--r--   0        0        0      875 2024-02-28 17:08:41.033546 strangeworks_qiskit_runtime-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      389 2024-02-28 17:08:15.657388 strangeworks_qiskit_runtime-0.1.6/strangeworks_qiskit_runtime/__init__.py
--rw-r--r--   0        0        0     5511 2024-02-28 17:08:15.657388 strangeworks_qiskit_runtime-0.1.6/strangeworks_qiskit_runtime/runtime_client.py
--rw-r--r--   0        0        0    11643 2024-02-28 17:08:15.657388 strangeworks_qiskit_runtime-0.1.6/strangeworks_qiskit_runtime/service.py
--rw-r--r--   0        0        0     6893 2024-02-28 17:08:15.657388 strangeworks_qiskit_runtime-0.1.6/strangeworks_qiskit_runtime/sw_runtime_job.py
--rw-r--r--   0        0        0     5465 2024-02-28 17:08:15.657388 strangeworks_qiskit_runtime-0.1.6/strangeworks_qiskit_runtime/swestimator.py
--rw-r--r--   0        0        0     4549 2024-02-28 17:08:15.657388 strangeworks_qiskit_runtime-0.1.6/strangeworks_qiskit_runtime/swsampler.py
--rw-r--r--   0        0        0      753 1970-01-01 00:00:00.000000 strangeworks_qiskit_runtime-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      204 2024-03-18 18:46:46.318913 strangeworks_qiskit_runtime-0.1.7/README.md
+-rw-r--r--   0        0        0      875 2024-03-18 18:47:01.890787 strangeworks_qiskit_runtime-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      389 2024-03-18 18:46:46.318913 strangeworks_qiskit_runtime-0.1.7/strangeworks_qiskit_runtime/__init__.py
+-rw-r--r--   0        0        0     6228 2024-03-18 18:46:46.322913 strangeworks_qiskit_runtime-0.1.7/strangeworks_qiskit_runtime/runtime_client.py
+-rw-r--r--   0        0        0    11643 2024-03-18 18:46:46.322913 strangeworks_qiskit_runtime-0.1.7/strangeworks_qiskit_runtime/service.py
+-rw-r--r--   0        0        0     6893 2024-03-18 18:46:46.322913 strangeworks_qiskit_runtime-0.1.7/strangeworks_qiskit_runtime/sw_runtime_job.py
+-rw-r--r--   0        0        0     5465 2024-03-18 18:46:46.322913 strangeworks_qiskit_runtime-0.1.7/strangeworks_qiskit_runtime/swestimator.py
+-rw-r--r--   0        0        0     4549 2024-03-18 18:46:46.322913 strangeworks_qiskit_runtime-0.1.7/strangeworks_qiskit_runtime/swsampler.py
+-rw-r--r--   0        0        0      753 1970-01-01 00:00:00.000000 strangeworks_qiskit_runtime-0.1.7/PKG-INFO
```

### Comparing `strangeworks_qiskit_runtime-0.1.6/pyproject.toml` & `strangeworks_qiskit_runtime-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strangeworks-qiskit-runtime"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 packages = [{ include = "strangeworks_qiskit_runtime" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `strangeworks_qiskit_runtime-0.1.6/strangeworks_qiskit_runtime/runtime_client.py` & `strangeworks_qiskit_runtime-0.1.7/strangeworks_qiskit_runtime/runtime_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Strangeworks Runtime Client."""
 
 import json
+from datetime import datetime as python_datetime
 from typing import Any, Dict, List, Optional
 
 import strangeworks
 from qiskit import assemble
 from qiskit_ibm_runtime.api.clients.runtime import RuntimeClient
 from qiskit_ibm_runtime.utils import RuntimeEncoder
 from strangeworks.core.client.resource import Resource
@@ -131,14 +132,35 @@
         return strangeworks.jobs(slug=job_slug)[0]
 
     def jobs_get(self, **kwargs):
         return strangeworks.jobs(
             product_slugs=self._product_slug, resource_slugs=self.rsc.slug
         )
 
+    def backend_properties(
+        self, backend_name: str, datetime: Optional[python_datetime] = None
+    ) -> Dict[str, Any]:
+        """Return the properties of the IBM backend.
+
+        Args:
+            backend_name: The name of the IBM backend.
+            datetime: Date and time for additional filtering of backend properties.
+
+        Returns:
+            Backend properties.
+
+        Raises:
+            NotImplementedError: If `datetime` is specified.
+        """
+        payload = {
+            "backend_name": backend_name,
+            "datetime": datetime,
+        }
+        return strangeworks.execute(self.rsc, payload, "runtime_backend_properties")
+
     def create_session(
         self,
         backend: Optional[str] = None,
         instance: Optional[str] = None,
         max_time: Optional[int] = None,
         channel: Optional[str] = None,
         mode: Optional[str] = None,
```

### Comparing `strangeworks_qiskit_runtime-0.1.6/strangeworks_qiskit_runtime/service.py` & `strangeworks_qiskit_runtime-0.1.7/strangeworks_qiskit_runtime/service.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit_runtime-0.1.6/strangeworks_qiskit_runtime/sw_runtime_job.py` & `strangeworks_qiskit_runtime-0.1.7/strangeworks_qiskit_runtime/sw_runtime_job.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit_runtime-0.1.6/strangeworks_qiskit_runtime/swestimator.py` & `strangeworks_qiskit_runtime-0.1.7/strangeworks_qiskit_runtime/swestimator.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit_runtime-0.1.6/strangeworks_qiskit_runtime/swsampler.py` & `strangeworks_qiskit_runtime-0.1.7/strangeworks_qiskit_runtime/swsampler.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit_runtime-0.1.6/PKG-INFO` & `strangeworks_qiskit_runtime-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strangeworks-qiskit-runtime
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

