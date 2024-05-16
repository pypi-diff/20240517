# Comparing `tmp/definite_sdk-0.1.0.tar.gz` & `tmp/definite_sdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "definite_sdk-0.1.0.tar", max compression
+gzip compressed data, was "definite_sdk-0.1.3.tar", max compression
```

## Comparing `definite_sdk-0.1.0.tar` & `definite_sdk-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2024-05-16 01:55:23.896740 definite_sdk-0.1.0/LICENSE
--rw-r--r--   0        0        0      136 2024-05-16 01:55:23.896740 definite_sdk-0.1.0/README.md
--rw-r--r--   0        0        0      708 2024-05-16 01:55:23.896740 definite_sdk-0.1.0/definite_sdk/client.py
--rw-r--r--   0        0        0     5060 2024-05-16 01:55:23.896740 definite_sdk-0.1.0/definite_sdk/store.py
--rw-r--r--   0        0        0      503 2024-05-16 01:55:23.896740 definite_sdk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      702 1970-01-01 00:00:00.000000 definite_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-16 23:16:41.775288 definite_sdk-0.1.3/LICENSE
+-rw-r--r--   0        0        0      136 2024-05-16 23:16:41.775288 definite_sdk-0.1.3/README.md
+-rw-r--r--   0        0        0      721 2024-05-16 23:16:41.775288 definite_sdk-0.1.3/definite_sdk/client.py
+-rw-r--r--   0        0        0     5034 2024-05-16 23:16:41.775288 definite_sdk-0.1.3/definite_sdk/store.py
+-rw-r--r--   0        0        0      503 2024-05-16 23:16:41.779288 definite_sdk-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      702 1970-01-01 00:00:00.000000 definite_sdk-0.1.3/PKG-INFO
```

### Comparing `definite_sdk-0.1.0/LICENSE` & `definite_sdk-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `definite_sdk-0.1.0/definite_sdk/client.py` & `definite_sdk-0.1.3/definite_sdk/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from store import DefiniteKVStore
+from definite_sdk.store import DefiniteKVStore
 
 API_URL = "https://api.definite.app"
 
 
 class DefiniteClient:
     """Client for interacting with the Definite API."""
```

### Comparing `definite_sdk-0.1.0/definite_sdk/store.py` & `definite_sdk-0.1.3/definite_sdk/store.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,15 @@
             Exception: If the store fails to load.
         """
 
         self._api_key = api_key
         self._name = name
         self._store_url = api_url + STORE_ENDPOINT
         response = requests.get(
-            self._store_url,
-            json={"name": self._name},
+            self._store_url + f"/{name}",
             headers={"Authorization": "Bearer " + self._api_key},
         )
 
         if response.status_code == 404:
             # Store not found. Create a new one.
             self._data = {}
             self._version_id = None
```

### Comparing `definite_sdk-0.1.0/PKG-INFO` & `definite_sdk-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: definite-sdk
-Version: 0.1.0
+Version: 0.1.3
 Summary: Definite SDK for Python
 License: MIT
 Author: Definite
 Author-email: hello@definite.app
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

