# Comparing `tmp/penquins-2.4.0.tar.gz` & `tmp/penquins-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "penquins-2.4.0.tar", last modified: Wed Jan 24 23:41:28 2024, max compression
+gzip compressed data, was "penquins-2.4.1.tar", last modified: Fri May 17 02:22:08 2024, max compression
```

## Comparing `penquins-2.4.0.tar` & `penquins-2.4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2024-01-24 23:41:28.280153 penquins-2.4.0/
--rw-r--r--   0 mcoughlin   (501) staff       (20)     1068 2024-01-24 23:41:21.000000 penquins-2.4.0/LICENSE
--rw-r--r--   0 mcoughlin   (501) staff       (20)      229 2024-01-24 23:41:28.279984 penquins-2.4.0/PKG-INFO
-drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2024-01-24 23:41:28.279027 penquins-2.4.0/penquins/
--rw-r--r--   0 mcoughlin   (501) staff       (20)       24 2024-01-24 23:41:21.000000 penquins-2.4.0/penquins/__init__.py
--rw-r--r--   0 mcoughlin   (501) staff       (20)    29345 2024-01-24 23:41:21.000000 penquins-2.4.0/penquins/penquins.py
-drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2024-01-24 23:41:28.279763 penquins-2.4.0/penquins.egg-info/
--rw-r--r--   0 mcoughlin   (501) staff       (20)      229 2024-01-24 23:41:28.000000 penquins-2.4.0/penquins.egg-info/PKG-INFO
--rw-r--r--   0 mcoughlin   (501) staff       (20)      217 2024-01-24 23:41:28.000000 penquins-2.4.0/penquins.egg-info/SOURCES.txt
--rw-r--r--   0 mcoughlin   (501) staff       (20)        1 2024-01-24 23:41:28.000000 penquins-2.4.0/penquins.egg-info/dependency_links.txt
--rw-r--r--   0 mcoughlin   (501) staff       (20)       60 2024-01-24 23:41:28.000000 penquins-2.4.0/penquins.egg-info/requires.txt
--rw-r--r--   0 mcoughlin   (501) staff       (20)        9 2024-01-24 23:41:28.000000 penquins-2.4.0/penquins.egg-info/top_level.txt
--rw-r--r--   0 mcoughlin   (501) staff       (20)       38 2024-01-24 23:41:28.280211 penquins-2.4.0/setup.cfg
--rw-r--r--   0 mcoughlin   (501) staff       (20)     5088 2024-01-24 23:41:21.000000 penquins-2.4.0/setup.py
+drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2024-05-17 02:22:08.695276 penquins-2.4.1/
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     1068 2024-01-24 23:41:21.000000 penquins-2.4.1/LICENSE
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      229 2024-05-17 02:22:08.695110 penquins-2.4.1/PKG-INFO
+drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2024-05-17 02:22:08.694097 penquins-2.4.1/penquins/
+-rw-r--r--   0 mcoughlin   (501) staff       (20)       24 2024-01-24 23:41:21.000000 penquins-2.4.1/penquins/__init__.py
+-rw-r--r--   0 mcoughlin   (501) staff       (20)    29368 2024-05-17 02:21:47.000000 penquins-2.4.1/penquins/penquins.py
+drwxr-xr-x   0 mcoughlin   (501) staff       (20)        0 2024-05-17 02:22:08.694911 penquins-2.4.1/penquins.egg-info/
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      229 2024-05-17 02:22:08.000000 penquins-2.4.1/penquins.egg-info/PKG-INFO
+-rw-r--r--   0 mcoughlin   (501) staff       (20)      217 2024-05-17 02:22:08.000000 penquins-2.4.1/penquins.egg-info/SOURCES.txt
+-rw-r--r--   0 mcoughlin   (501) staff       (20)        1 2024-05-17 02:22:08.000000 penquins-2.4.1/penquins.egg-info/dependency_links.txt
+-rw-r--r--   0 mcoughlin   (501) staff       (20)       60 2024-05-17 02:22:08.000000 penquins-2.4.1/penquins.egg-info/requires.txt
+-rw-r--r--   0 mcoughlin   (501) staff       (20)        9 2024-05-17 02:22:08.000000 penquins-2.4.1/penquins.egg-info/top_level.txt
+-rw-r--r--   0 mcoughlin   (501) staff       (20)       38 2024-05-17 02:22:08.695330 penquins-2.4.1/setup.cfg
+-rw-r--r--   0 mcoughlin   (501) staff       (20)     5088 2024-05-17 02:21:47.000000 penquins-2.4.1/setup.py
```

### Comparing `penquins-2.4.0/LICENSE` & `penquins-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `penquins-2.4.0/penquins/penquins.py` & `penquins-2.4.1/penquins/penquins.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """ PENQUINS - Processing ENormous Queries of kowalski Users INStantaneously """
 
 __all__ = ["Kowalski", "__version__"]
 
-import os
 import secrets
 import string
 import traceback
 from copy import deepcopy
 from multiprocessing.pool import ThreadPool
 from netrc import netrc
 from typing import Mapping, Optional, Sequence, Union, Tuple
+from urllib.parse import urljoin
 
 import requests
 from bson.json_util import loads
 from requests.adapters import DEFAULT_POOLBLOCK, DEFAULT_POOLSIZE, HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
 from tqdm.auto import tqdm
 
-__version__ = "2.4.0"
+__version__ = "2.4.1"
 
 Num = Union[int, float]
 
 DEFAULT_TIMEOUT: int = 5  # seconds
 DEFAULT_RETRIES: int = 3
 DEFAULT_BACKOFF_FACTOR: int = 1
 
@@ -170,15 +170,15 @@
                 "post": self.instances[name]["session"].post,
                 "put": self.instances[name]["session"].put,
                 "patch": self.instances[name]["session"].patch,
                 "delete": self.instances[name]["session"].delete,
                 "head": self.instances[name]["session"].head,
             }
             # mount session adapters
-            timeout = kwargs.get("timeout", DEFAULT_TIMEOUT)
+            timeout = cfg.get("timeout", kwargs.get("timeout", DEFAULT_TIMEOUT))
             pool_connections = kwargs.get("pool_connections", DEFAULT_POOLSIZE)
             pool_maxsize = kwargs.get("pool_maxsize", DEFAULT_POOLSIZE)
             max_retries = kwargs.get("max_retries", DEFAULT_RETRIES)
             backoff_factor = kwargs.get("backoff_factor", DEFAULT_BACKOFF_FACTOR)
             pool_block = kwargs.get("pool_block", DEFAULT_POOLBLOCK)
 
             retries = Retry(
@@ -335,15 +335,15 @@
                 name = list(self.instances.keys())[0]
             else:
                 raise ValueError(
                     "Please specify instance name when using multiple instances"
                 )
         try:
             resp = self.instances[name]["session"].get(
-                os.path.join(self.instances[name]["base_url"], ""),
+                urljoin(self.instances[name]["base_url"], ""),
                 headers=self.instances[name]["headers"],
             )
 
             if resp.status_code == requests.codes.ok:
                 return True
             return False
 
@@ -373,21 +373,21 @@
         if endpoint is None:
             raise ValueError("Endpoint not specified")
         if method not in ["get", "post", "put", "patch", "delete", "head"]:
             raise ValueError(f"Unsupported method: {method}")
 
         if method != "get":
             resp = self.instances[name]["methods"][method](
-                os.path.join(self.instances[name]["base_url"], endpoint),
+                urljoin(self.instances[name]["base_url"], endpoint),
                 json=data,
                 headers=self.instances[name]["headers"],
             )
         else:
             resp = self.instances[name]["methods"][method](
-                os.path.join(self.instances[name]["base_url"], endpoint),
+                urljoin(self.instances[name]["base_url"], endpoint),
                 params=data,
                 headers=self.instances[name]["headers"],
             )
 
         status_mapper = {
             200: "success",
             400: "error",
@@ -639,15 +639,15 @@
                     secrets.choice(string.ascii_lowercase + string.digits)
                     for _ in range(32)
                 )
 
                 _query["kwargs"]["_id"] = _id
 
         resp = self.instances[name]["session"].post(
-            os.path.join(self.instances[name]["base_url"], "api/queries"),
+            urljoin(self.instances[name]["base_url"], "api/queries"),
             json=_query,
             headers=self.instances[name]["headers"],
         )
         return {name: loads(resp.text)}
 
     def query(
         self,
```

### Comparing `penquins-2.4.0/setup.py` & `penquins-2.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 LONG_DESCRIPTION = ""
 AUTHOR = "Dmitry A. Duev"
 AUTHOR_EMAIL = "duev@caltech.edu"
 LICENSE = "MIT"
 URL = "https://github.com/dmitryduev/penquins"
 
 # VERSION should be PEP386 compatible (http://www.python.org/dev/peps/pep-0386)
-VERSION = "2.4.0"
+VERSION = "2.4.1"
 
 # Indicates if this version is a release version
 RELEASE = "dev" not in VERSION
 
 if not RELEASE:
     VERSION += get_git_devstr(sha=False)
```

