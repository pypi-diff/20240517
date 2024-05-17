# Comparing `tmp/saw_client-1.1.0.tar.gz` & `tmp/saw_client-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saw_client-1.1.0.tar", max compression
+gzip compressed data, was "saw_client-1.1.1.tar", max compression
```

## Comparing `saw_client-1.1.0.tar` & `saw_client-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     7375 2023-08-12 12:50:56.261630 saw_client-1.1.0/README.md
--rw-r--r--   0        0        0      353 2023-12-16 12:37:27.785133 saw_client-1.1.0/mypy.ini
--rw-r--r--   0        0        0      640 2024-02-07 21:47:49.833704 saw_client-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    30705 2024-02-02 12:30:22.716057 saw_client-1.1.0/saw_client/__init__.py
--rw-r--r--   0        0        0    12808 2024-02-02 12:30:22.716057 saw_client-1.1.0/saw_client/commands.py
--rw-r--r--   0        0        0    15156 2024-02-02 12:30:22.716057 saw_client-1.1.0/saw_client/connection.py
--rw-r--r--   0        0        0    35276 2024-02-02 12:30:22.716057 saw_client-1.1.0/saw_client/crucible.py
--rw-r--r--   0        0        0    10102 2023-08-12 12:50:56.261630 saw_client-1.1.0/saw_client/dashboard.py
--rw-r--r--   0        0        0     3152 2023-08-12 12:50:56.261630 saw_client-1.1.0/saw_client/exceptions.py
--rw-r--r--   0        0        0      112 2023-08-12 12:50:56.261630 saw_client-1.1.0/saw_client/jvm.py
--rw-r--r--   0        0        0     1955 2023-08-12 12:50:56.261630 saw_client-1.1.0/saw_client/jvm_type.py
--rw-r--r--   0        0        0     1387 2023-08-12 12:50:56.261630 saw_client-1.1.0/saw_client/llvm.py
--rw-r--r--   0        0        0     1736 2023-08-12 12:50:56.261630 saw_client-1.1.0/saw_client/llvm_type.py
--rw-r--r--   0        0        0     2459 2024-02-02 12:30:22.716057 saw_client-1.1.0/saw_client/mir.py
--rw-r--r--   0        0        0     3551 2024-02-02 12:30:22.716057 saw_client-1.1.0/saw_client/mir_type.py
--rw-r--r--   0        0        0      976 2023-08-12 12:50:56.261630 saw_client-1.1.0/saw_client/option.py
--rw-r--r--   0        0        0     3619 2023-12-16 12:37:27.785133 saw_client-1.1.0/saw_client/proofscript.py
--rw-r--r--   0        0        0        0 2023-08-12 12:50:56.261630 saw_client-1.1.0/saw_client/py.typed
--rw-r--r--   0        0        0     5344 2023-12-16 12:37:27.785133 saw_client-1.1.0/saw_client/solver_cache.py
--rw-r--r--   0        0        0      855 2023-08-12 12:50:56.261630 saw_client-1.1.0/saw_client/utils.py
--rw-r--r--   0        0        0     8190 1970-01-01 00:00:00.000000 saw_client-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7467 2024-05-17 02:09:43.078402 saw_client-1.1.1/README.md
+-rw-r--r--   0        0        0      429 2024-05-17 02:09:43.078640 saw_client-1.1.1/mypy.ini
+-rw-r--r--   0        0        0      639 2024-05-17 02:09:57.214833 saw_client-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    30686 2024-05-17 02:09:43.079949 saw_client-1.1.1/saw_client/__init__.py
+-rw-r--r--   0        0        0    12808 2023-09-27 18:17:42.412133 saw_client-1.1.1/saw_client/commands.py
+-rw-r--r--   0        0        0    15117 2024-05-17 02:09:43.080439 saw_client-1.1.1/saw_client/connection.py
+-rw-r--r--   0        0        0    35276 2024-05-14 16:46:22.482703 saw_client-1.1.1/saw_client/crucible.py
+-rw-r--r--   0        0        0    10102 2023-07-19 14:31:39.989063 saw_client-1.1.1/saw_client/dashboard.py
+-rw-r--r--   0        0        0     3152 2023-07-19 14:31:39.989132 saw_client-1.1.1/saw_client/exceptions.py
+-rw-r--r--   0        0        0      112 2023-07-19 14:31:39.989179 saw_client-1.1.1/saw_client/jvm.py
+-rw-r--r--   0        0        0     1955 2023-07-19 14:31:39.989231 saw_client-1.1.1/saw_client/jvm_type.py
+-rw-r--r--   0        0        0     1387 2023-07-19 14:31:39.989278 saw_client-1.1.1/saw_client/llvm.py
+-rw-r--r--   0        0        0     1736 2023-07-19 14:31:39.989374 saw_client-1.1.1/saw_client/llvm_type.py
+-rw-r--r--   0        0        0     2459 2024-05-14 16:46:22.482796 saw_client-1.1.1/saw_client/mir.py
+-rw-r--r--   0        0        0     3551 2024-05-14 16:46:22.482878 saw_client-1.1.1/saw_client/mir_type.py
+-rw-r--r--   0        0        0      976 2023-07-19 14:31:39.989429 saw_client-1.1.1/saw_client/option.py
+-rw-r--r--   0        0        0     3619 2023-07-19 14:31:39.989486 saw_client-1.1.1/saw_client/proofscript.py
+-rw-r--r--   0        0        0        0 2023-07-19 14:31:39.989511 saw_client-1.1.1/saw_client/py.typed
+-rw-r--r--   0        0        0     5329 2024-05-17 02:09:43.080794 saw_client-1.1.1/saw_client/solver_cache.py
+-rw-r--r--   0        0        0      855 2023-07-19 14:31:39.989571 saw_client-1.1.1/saw_client/utils.py
+-rw-r--r--   0        0        0     8333 1970-01-01 00:00:00.000000 saw_client-1.1.1/PKG-INFO
```

### Comparing `saw_client-1.1.0/README.md` & `saw_client-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -195,7 +195,12 @@
 
 ```
 saw_client.connect(url="http://localhost:8080/", reset_server=True)
 ```
 
 will connect to a SAW server running at `http://localhost:8080/` and will
 guarantee any previous state on the server is cleared.
+
+
+## Python Version Support
+
+Currently, `saw-remote-api` officially supports python `3.12`.
```

### Comparing `saw_client-1.1.0/pyproject.toml` & `saw_client-1.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "saw-client"
-version = "1.1.0"
+version = "1.1.1"
 readme = "README.md"
 description = "SAW client for the SAW RPC server"
 authors = ["Galois, Inc. <saw@galois.com>"]
 license = "BSD License"
 include = [
     "LICENSE",
     "mypy.ini",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.25.1"
 BitVector = "^3.4.9"
-cryptol = "3.1.0" # { path = "../../deps/cryptol/cryptol-remote-api/python/", develop = true }
-argo-client = "0.0.11"
+cryptol = "3.1.1" # { path = "../../deps/cryptol/cryptol-remote-api/python/", develop = true }
+argo-client = "0.0.12"
 lmdb = "^1.4.1"
 cbor2 = "^5.4.6"
 python-dateutil = "^2.8.2"
 
 [tool.poetry.dev-dependencies]
-mypy = "^0.991"
+mypy = "^1.10"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `saw_client-1.1.0/saw_client/__init__.py` & `saw_client-1.1.1/saw_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass
 from typing import List, Optional, Set, Union, Tuple, Any, IO, TextIO
 import uuid
 import sys
 import time
 import atexit
-from distutils.spawn import find_executable
+from shutil import which
 
 import cryptol
 
 from cryptol import cryptoltypes
 from . import connection
 from argo_client.connection import ServerConnection
 from . import llvm
```

### Comparing `saw_client-1.1.0/saw_client/commands.py` & `saw_client-1.1.1/saw_client/commands.py`

 * *Files identical despite different names*

### Comparing `saw_client-1.1.0/saw_client/connection.py` & `saw_client-1.1.1/saw_client/connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 import os
 import signal
 import sys
-from distutils.spawn import find_executable
+from shutil import which
 from argo_client.connection import ServerConnection, DynamicSocketProcess, HttpProcess, ManagedProcess
 from argo_client.interaction import Interaction, Command
 from .commands import *
 from .option import *
 from typing import Optional, Union, Any, List, TextIO
 
 # FIXME cryptol_path isn't always used...?
@@ -48,19 +48,19 @@
     c = None
     if command is not None:
         if url is not None:
             raise ValueError("A SAW server URL cannot be specified with a command currently.")
         c = SAWConnection(command, log_dest=log_dest)
     elif url is not None:
         c = SAWConnection(ServerConnection(HttpProcess(url, verify=verify)), log_dest=log_dest)
-    elif (command := os.getenv('SAW_SERVER')) is not None and (command := find_executable(command)) is not None:
+    elif (command := os.getenv('SAW_SERVER')) is not None and (command := which(command)) is not None:
         c = SAWConnection(command+" socket", log_dest=log_dest) # SAWConnection(ServerConnection(StdIOProcess(command+" stdio")))
     elif (url := os.getenv('SAW_SERVER_URL')) is not None:
         c = SAWConnection(ServerConnection(HttpProcess(url, verify=verify)), log_dest=log_dest)
-    elif (command := find_executable('saw-remote-api')) is not None:
+    elif (command := which('saw-remote-api')) is not None:
         c = SAWConnection(command+" socket", log_dest=log_dest)
     else:
         raise ValueError(
             """saw.connection.connect requires one of the following:",
             1) a command to launch a SAW server is the first positional argument,
             2) a URL to connect to a running SAW server is provided via the `url` keyword argument,
             3) the environment variable `SAW_SERVER` must refer to a valid server executable, or
```

### Comparing `saw_client-1.1.0/saw_client/crucible.py` & `saw_client-1.1.1/saw_client/crucible.py`

 * *Files identical despite different names*

### Comparing `saw_client-1.1.0/saw_client/dashboard.py` & `saw_client-1.1.1/saw_client/dashboard.py`

 * *Files identical despite different names*

### Comparing `saw_client-1.1.0/saw_client/exceptions.py` & `saw_client-1.1.1/saw_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `saw_client-1.1.0/saw_client/jvm_type.py` & `saw_client-1.1.1/saw_client/jvm_type.py`

 * *Files identical despite different names*

### Comparing `saw_client-1.1.0/saw_client/llvm.py` & `saw_client-1.1.1/saw_client/llvm.py`

 * *Files identical despite different names*

### Comparing `saw_client-1.1.0/saw_client/llvm_type.py` & `saw_client-1.1.1/saw_client/llvm_type.py`

 * *Files identical despite different names*

### Comparing `saw_client-1.1.0/saw_client/mir.py` & `saw_client-1.1.1/saw_client/mir.py`

 * *Files identical despite different names*

### Comparing `saw_client-1.1.0/saw_client/mir_type.py` & `saw_client-1.1.1/saw_client/mir_type.py`

 * *Files identical despite different names*

### Comparing `saw_client-1.1.0/saw_client/option.py` & `saw_client-1.1.1/saw_client/option.py`

 * *Files identical despite different names*

### Comparing `saw_client-1.1.0/saw_client/proofscript.py` & `saw_client-1.1.1/saw_client/proofscript.py`

 * *Files identical despite different names*

### Comparing `saw_client-1.1.0/saw_client/solver_cache.py` & `saw_client-1.1.1/saw_client/solver_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import cbor2 # type: ignore
+import cbor2
 from collections.abc import MutableMapping
 from dataclasses import dataclass
 from datetime import datetime, timezone
 import dateutil.parser
 import lmdb # type: ignore
 import os
 from typing import Dict, List, Optional, Tuple, Union
```

### Comparing `saw_client-1.1.0/saw_client/utils.py` & `saw_client-1.1.1/saw_client/utils.py`

 * *Files identical despite different names*

### Comparing `saw_client-1.1.0/PKG-INFO` & `saw_client-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: saw-client
-Version: 1.1.0
+Version: 1.1.1
 Summary: SAW client for the SAW RPC server
 License: BSD License
 Author: Galois, Inc.
 Author-email: saw@galois.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: BitVector (>=3.4.9,<4.0.0)
-Requires-Dist: argo-client (==0.0.11)
+Requires-Dist: argo-client (==0.0.12)
 Requires-Dist: cbor2 (>=5.4.6,<6.0.0)
-Requires-Dist: cryptol (==3.1.0)
+Requires-Dist: cryptol (==3.1.1)
 Requires-Dist: lmdb (>=1.4.1,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # SAW Python Client
 
@@ -219,7 +220,12 @@
 ```
 saw_client.connect(url="http://localhost:8080/", reset_server=True)
 ```
 
 will connect to a SAW server running at `http://localhost:8080/` and will
 guarantee any previous state on the server is cleared.
 
+
+## Python Version Support
+
+Currently, `saw-remote-api` officially supports python `3.12`.
+
```

