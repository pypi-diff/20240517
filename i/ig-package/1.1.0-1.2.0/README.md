# Comparing `tmp/ig_package-1.1.0.tar.gz` & `tmp/ig_package-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ig_package-1.1.0.tar", max compression
+gzip compressed data, was "ig_package-1.2.0.tar", max compression
```

## Comparing `ig_package-1.1.0.tar` & `ig_package-1.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1089 2024-04-03 23:27:00.840175 ig_package-1.1.0/LICENSE
--rw-r--r--   0        0        0      583 2024-05-02 15:14:26.376283 ig_package-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1971 2024-04-08 19:00:44.044419 ig_package-1.1.0/README.md
--rw-r--r--   0        0        0      158 2024-04-01 22:15:12.186529 ig_package-1.1.0/src/ig_package/__init__.py
--rw-r--r--   0        0        0    22166 2024-05-02 14:51:17.205879 ig_package-1.1.0/src/ig_package/main.py
--rw-r--r--   0        0        0     2471 1970-01-01 00:00:00.000000 ig_package-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-03 23:27:00.840175 ig_package-1.2.0/LICENSE
+-rw-r--r--   0        0        0      607 2024-05-05 16:14:18.381072 ig_package-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1971 2024-04-08 19:00:44.044419 ig_package-1.2.0/README.md
+-rw-r--r--   0        0        0      158 2024-04-01 22:15:12.186529 ig_package-1.2.0/src/ig_package/__init__.py
+-rw-r--r--   0        0        0    22246 2024-05-05 13:57:10.860163 ig_package-1.2.0/src/ig_package/main.py
+-rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 ig_package-1.2.0/PKG-INFO
```

### Comparing `ig_package-1.1.0/LICENSE` & `ig_package-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ig_package-1.1.0/pyproject.toml` & `ig_package-1.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "ig-package"
-version = "1.1.0"
+version = "1.2.0"
 description = "A package allowing easy interaction with IG Group's REST API."
 authors = ["hnewey7 <hnewey7@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 requests = "^2.31.0"
 pandas = "^2.2.1"
+trading-ig = "^0.0.22"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
 myst-nb = {version = "^1.0.0", python = "^3.9"}
 sphinx-autoapi = "^3.0.0"
```

### Comparing `ig_package-1.1.0/README.md` & `ig_package-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ig_package-1.1.0/src/ig_package/main.py` & `ig_package-1.2.0/src/ig_package/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import os
 from pathlib import Path
 import time
 from datetime import datetime
 import pandas as pd
 
 from trading_ig import IGService, IGStreamService
-from IG_API_Details import config
 from trading_ig.streamer.manager import StreamingManager
 
 # - - - - - - - - - - - - - - - - - - - - -
 
 global logger
 logger = logging.getLogger()
 
@@ -78,16 +77,18 @@
   """ Object to interact with IG Group's API.
         - Open trading sessions.
         - Get historical data.
         - Close trading sessions.
 
       **NOTE: API key, username and password should be entered when initialising the IG object."""
 
-  def __init__(self,API_key:str,username:str,password:str,watchlist_enable:bool=False) -> None:
+  def __init__(self,API_key:str,username:str,password:str,acc_type:str,acc_number:str,watchlist_enable:bool=False) -> None:
     self.watchlist_enable = watchlist_enable
+    self.acc_type = acc_type
+    self.acc_number = acc_number
     # Defining header.
     self.header = {
       "Content-Type":"application/json; charset=UTF-8",
       "Accept":"application/json; charset=UTF-8",
       "VERSION":"2",
       "X-IG-API-KEY":API_key
     }
@@ -121,15 +122,15 @@
       return True
     else:
       return False
 
   def open_streaming_session(self) -> None:
     """ Opening a streaming session through IG, allowing data to be collected in real time."""
     # Opening IG service.
-    self.ig_service = IGService(config.username,config.password,config.api_key,config.acc_type,config.acc_number)
+    self.ig_service = IGService(self.body["identifier"],self.body["password"],self.header["X-IG-API-KEY"],self.acc_type,self.acc_number)
     # Opening streaming service.
     self.ig_streaming_service = IGStreamService(self.ig_service)
     self.ig_streaming_service.create_session(version="3")
     self.streaming_manager = StreamingManager(self.ig_streaming_service)
 
   def check_trading_session(self) -> bool:
     """ Checking if trading session active.
```

### Comparing `ig_package-1.1.0/PKG-INFO` & `ig_package-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: ig-package
-Version: 1.1.0
+Version: 1.2.0
 Summary: A package allowing easy interaction with IG Group's REST API.
 License: MIT
 Author: hnewey7
 Author-email: hnewey7@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: trading-ig (>=0.0.22,<0.0.23)
 Description-Content-Type: text/markdown
 
 # Python Package for IG Group's API.
 
 ## A package allowing easy interaction with IG Group's REST API.
 
 This project is a fully functional package that allows easy interaction with IG Group's REST API. The main function being to retrieve historical data for later use in backtesting. To do this, key functions were defined for:
```

