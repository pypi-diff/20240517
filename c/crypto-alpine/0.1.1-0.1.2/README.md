# Comparing `tmp/crypto_alpine-0.1.1.tar.gz` & `tmp/crypto_alpine-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto_alpine-0.1.1.tar", max compression
+gzip compressed data, was "crypto_alpine-0.1.2.tar", max compression
```

## Comparing `crypto_alpine-0.1.1.tar` & `crypto_alpine-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2024-05-13 11:50:38.758046 crypto_alpine-0.1.1/LICENSE
--rw-r--r--   0        0        0     1464 2024-05-13 13:21:37.598908 crypto_alpine-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-05-13 13:04:39.538997 crypto_alpine-0.1.1/alpine/__init__.py
--rw-r--r--   0        0        0       60 2024-05-13 11:45:52.899373 crypto_alpine-0.1.1/alpine/exchanges/__init__.py
--rw-r--r--   0        0        0     1105 2024-05-17 11:00:34.999485 crypto_alpine-0.1.1/alpine/exchanges/abstract.py
--rw-r--r--   0        0        0     2061 2024-05-13 11:52:52.024579 crypto_alpine-0.1.1/alpine/exchanges/binance.py
--rw-r--r--   0        0        0     9475 2024-05-17 11:00:35.044289 crypto_alpine-0.1.1/alpine/exchanges/bitget.py
--rw-r--r--   0        0        0     1398 2024-05-13 11:45:52.907314 crypto_alpine-0.1.1/alpine/exchanges/utils.py
--rw-r--r--   0        0        0     4765 2024-05-17 11:00:35.006805 crypto_alpine-0.1.1/alpine/exchanges/wrapper.py
--rw-r--r--   0        0        0      342 2024-05-17 11:01:09.785579 crypto_alpine-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1851 1970-01-01 00:00:00.000000 crypto_alpine-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-13 11:50:38.758046 crypto_alpine-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1741 2024-05-17 11:17:12.556373 crypto_alpine-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-13 13:04:39.538997 crypto_alpine-0.1.2/alpine/__init__.py
+-rw-r--r--   0        0        0       60 2024-05-13 11:45:52.899373 crypto_alpine-0.1.2/alpine/exchanges/__init__.py
+-rw-r--r--   0        0        0     1105 2024-05-17 11:15:36.947709 crypto_alpine-0.1.2/alpine/exchanges/abstract.py
+-rw-r--r--   0        0        0     2027 2024-05-17 11:15:38.697801 crypto_alpine-0.1.2/alpine/exchanges/binance.py
+-rw-r--r--   0        0        0     9424 2024-05-17 11:15:39.270381 crypto_alpine-0.1.2/alpine/exchanges/bitget.py
+-rw-r--r--   0        0        0     1398 2024-05-13 11:45:52.907314 crypto_alpine-0.1.2/alpine/exchanges/utils.py
+-rw-r--r--   0        0        0     5350 2024-05-17 11:17:19.491187 crypto_alpine-0.1.2/alpine/exchanges/wrapper.py
+-rw-r--r--   0        0        0      342 2024-05-17 11:15:45.690424 crypto_alpine-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2128 1970-01-01 00:00:00.000000 crypto_alpine-0.1.2/PKG-INFO
```

### Comparing `crypto_alpine-0.1.1/LICENSE` & `crypto_alpine-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `crypto_alpine-0.1.1/README.md` & `crypto_alpine-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 ```
 pip install -U crypto-alpine
 ```
 
 ## Documentation
 
-1. Set environment variables
+1. Set environment variables (optional)
 
 ```
 export API_SECRET_KEY=xxx
 export API_ACCESS_KEY=yyy
 export API_PASSPHRASE=zzz
 ```
 
@@ -22,14 +22,22 @@
 
 ```
 from alpine.exchanges import Wrapper
 
 w = Wrapper('bitget')
 ```
 
+Note that if you don't want to use enviroment variables (if you wish to use the library within your code), you can define them during the initialization:
+
+```
+from alpine.exchanges import Wrapper
+
+w = Wrapper('bitget', <access_key>, <secret_key>, <passphrase>)
+```
+
 3. Set a leverage
 
 ```
 w.set_leverage(leverage, position, symbol, margin_coin)
 # Example: w.set_leverage(10, "long", "FETUSDT", "usdt")
 ```
```

### Comparing `crypto_alpine-0.1.1/alpine/exchanges/abstract.py` & `crypto_alpine-0.1.2/alpine/exchanges/abstract.py`

 * *Files identical despite different names*

### Comparing `crypto_alpine-0.1.1/alpine/exchanges/binance.py` & `crypto_alpine-0.1.2/alpine/exchanges/binance.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     def _signature(self, params):
         """
          HTTP Calls needs a specific signature.
         :param params: The HTTP parameters.
          :type params: dict
         """
         return hmac.new(
-            os.environ.get("API_SECRET_KEY").encode("utf-8"),
+            self.secret_key.encode("utf-8"),
             params.encode("utf-8"),
             hashlib.sha256,
         ).hexdigest()
 
     def request(self, method, path, params):
         """
         HTTP Call to the API.
@@ -36,15 +36,15 @@
         path_query = urllib.parse.urlencode(params, True).replace("%40", "@")
         payload = {
             "signature": self._signature(path_query),
             "timestamp": int(time.time() * 1000),
             "params": path_query,
         }
         headers = {
-            "X-MBX-APIKEY": os.environ.get("API_ACCESS_KEY"),
+            "X-MBX-APIKEY": self.access_key,
         }
         r = requests.request(
             method, f"{self.API_ENDPOINT}{path}", json=payload, headers=headers
         )
         try:
             r.raise_for_status()
         except requests.exceptions.HTTPError:
```

### Comparing `crypto_alpine-0.1.1/alpine/exchanges/bitget.py` & `crypto_alpine-0.1.2/alpine/exchanges/bitget.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         :type params: dict
         """
         if method == "POST":
             pre_hash = f"{timestamp}{method}{path}{json.dumps(params)}"
         else:
             pre_hash = f"{timestamp}{method}{path}?{urllib.parse.urlencode(params)}"
         mac = hmac.new(
-            bytes(os.environ.get("API_SECRET_KEY"), encoding="utf8"),
+            bytes(self.secret_key, encoding="utf8"),
             bytes(pre_hash, encoding="utf-8"),
             digestmod="sha256",
         )
         return base64.b64encode(mac.digest())
 
     def request(self, method, path, params):
         """
@@ -48,18 +48,18 @@
         :type params: dict
         """
         timestamp = int(time.time() * 1000)
         params = (
             dict(sorted(params.items())) if params else None
         )  # We need to sort the dictionnary ASC
         headers = {
-            "ACCESS-KEY": os.environ.get("API_ACCESS_KEY"),
+            "ACCESS-KEY": self.access_key,
             "ACCESS-SIGN": self._signature(timestamp, method, path, params),
             "ACCESS-TIMESTAMP": str(timestamp),
-            "ACCESS-PASSPHRASE": os.environ.get("API_PASSPHRASE"),
+            "ACCESS-PASSPHRASE": self.passphrase,
             "locale": "en-US",
         }
 
         kwargs = {"params": params} if method == "GET" else {"json": params}
         r = requests.request(
             method, f"{self.API_ENDPOINT}{path}", headers=headers, **kwargs
         )
```

### Comparing `crypto_alpine-0.1.1/alpine/exchanges/utils.py` & `crypto_alpine-0.1.2/alpine/exchanges/utils.py`

 * *Files identical despite different names*

### Comparing `crypto_alpine-0.1.1/alpine/exchanges/wrapper.py` & `crypto_alpine-0.1.2/alpine/exchanges/wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,29 @@
 import importlib
+import os
 
 
 class Wrapper:
-    def __init__(self, exchange_name):
+    def __init__(
+        self, exchange_name, access_key=None, secret_key=None, passphrase=None
+    ):
         """
         :param exchange_name: The exchange name to use.
         :type exchange_name: str
+        :param access_key: Access key to connect to the API.
+        :type access_key: None, str
+        :param secret_key: Secret key to connect to the API.
+        :type secret_key: None, str
+        :param passphrase: Passphrase to connect to the API.
+        :type passphrase: None, str
         """
         self.exchange_name = exchange_name
+        self.access_key = access_key or os.environ.get("API_ACCESS_KEY")
+        self.secret_key = secret_key or os.environ.get("API_SECRET_KEY")
+        self.passphrase = passphrase or os.environ.get("API_PASSPHRASE")
         module = importlib.import_module(f"alpine.exchanges.{exchange_name}")
         self.exchange = getattr(module, exchange_name.capitalize())()
 
     def set_leverage(self, value, position, symbol, margin_coin):
         """
         Set the leverage to value.
         :param value: the leverage's value.
```

### Comparing `crypto_alpine-0.1.1/PKG-INFO` & `crypto_alpine-0.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-alpine
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python library for cryptocurrency trading
 Author: pydavid
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests (>=2.31.0,<3.0.0)
@@ -18,15 +18,15 @@
 
 ```
 pip install -U crypto-alpine
 ```
 
 ## Documentation
 
-1. Set environment variables
+1. Set environment variables (optional)
 
 ```
 export API_SECRET_KEY=xxx
 export API_ACCESS_KEY=yyy
 export API_PASSPHRASE=zzz
 ```
 
@@ -34,14 +34,22 @@
 
 ```
 from alpine.exchanges import Wrapper
 
 w = Wrapper('bitget')
 ```
 
+Note that if you don't want to use enviroment variables (if you wish to use the library within your code), you can define them during the initialization:
+
+```
+from alpine.exchanges import Wrapper
+
+w = Wrapper('bitget', <access_key>, <secret_key>, <passphrase>)
+```
+
 3. Set a leverage
 
 ```
 w.set_leverage(leverage, position, symbol, margin_coin)
 # Example: w.set_leverage(10, "long", "FETUSDT", "usdt")
 ```
```

