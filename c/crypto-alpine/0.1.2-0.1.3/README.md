# Comparing `tmp/crypto_alpine-0.1.2.tar.gz` & `tmp/crypto_alpine-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto_alpine-0.1.2.tar", max compression
+gzip compressed data, was "crypto_alpine-0.1.3.tar", max compression
```

## Comparing `crypto_alpine-0.1.2.tar` & `crypto_alpine-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2024-05-13 11:50:38.758046 crypto_alpine-0.1.2/LICENSE
--rw-r--r--   0        0        0     1741 2024-05-17 11:17:12.556373 crypto_alpine-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-05-13 13:04:39.538997 crypto_alpine-0.1.2/alpine/__init__.py
--rw-r--r--   0        0        0       60 2024-05-13 11:45:52.899373 crypto_alpine-0.1.2/alpine/exchanges/__init__.py
--rw-r--r--   0        0        0     1105 2024-05-17 11:15:36.947709 crypto_alpine-0.1.2/alpine/exchanges/abstract.py
--rw-r--r--   0        0        0     2027 2024-05-17 11:15:38.697801 crypto_alpine-0.1.2/alpine/exchanges/binance.py
--rw-r--r--   0        0        0     9424 2024-05-17 11:15:39.270381 crypto_alpine-0.1.2/alpine/exchanges/bitget.py
--rw-r--r--   0        0        0     1398 2024-05-13 11:45:52.907314 crypto_alpine-0.1.2/alpine/exchanges/utils.py
--rw-r--r--   0        0        0     5350 2024-05-17 11:17:19.491187 crypto_alpine-0.1.2/alpine/exchanges/wrapper.py
--rw-r--r--   0        0        0      342 2024-05-17 11:15:45.690424 crypto_alpine-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2128 1970-01-01 00:00:00.000000 crypto_alpine-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-13 11:50:38.758046 crypto_alpine-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1741 2024-05-17 11:17:12.556373 crypto_alpine-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-13 13:04:39.538997 crypto_alpine-0.1.3/alpine/__init__.py
+-rw-r--r--   0        0        0       60 2024-05-13 11:45:52.899373 crypto_alpine-0.1.3/alpine/exchanges/__init__.py
+-rw-r--r--   0        0        0     1105 2024-05-17 11:15:36.947709 crypto_alpine-0.1.3/alpine/exchanges/abstract.py
+-rw-r--r--   0        0        0     2027 2024-05-17 11:15:38.697801 crypto_alpine-0.1.3/alpine/exchanges/binance.py
+-rw-r--r--   0        0        0     9424 2024-05-17 11:15:39.270381 crypto_alpine-0.1.3/alpine/exchanges/bitget.py
+-rw-r--r--   0        0        0     1398 2024-05-13 11:45:52.907314 crypto_alpine-0.1.3/alpine/exchanges/utils.py
+-rw-r--r--   0        0        0     5386 2024-05-17 11:29:48.149712 crypto_alpine-0.1.3/alpine/exchanges/wrapper.py
+-rw-r--r--   0        0        0      342 2024-05-17 11:29:47.364769 crypto_alpine-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2128 1970-01-01 00:00:00.000000 crypto_alpine-0.1.3/PKG-INFO
```

### Comparing `crypto_alpine-0.1.2/LICENSE` & `crypto_alpine-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `crypto_alpine-0.1.2/README.md` & `crypto_alpine-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `crypto_alpine-0.1.2/alpine/exchanges/abstract.py` & `crypto_alpine-0.1.3/alpine/exchanges/abstract.py`

 * *Files identical despite different names*

### Comparing `crypto_alpine-0.1.2/alpine/exchanges/binance.py` & `crypto_alpine-0.1.3/alpine/exchanges/binance.py`

 * *Files identical despite different names*

### Comparing `crypto_alpine-0.1.2/alpine/exchanges/bitget.py` & `crypto_alpine-0.1.3/alpine/exchanges/bitget.py`

 * *Files identical despite different names*

### Comparing `crypto_alpine-0.1.2/alpine/exchanges/utils.py` & `crypto_alpine-0.1.3/alpine/exchanges/utils.py`

 * *Files identical despite different names*

### Comparing `crypto_alpine-0.1.2/alpine/exchanges/wrapper.py` & `crypto_alpine-0.1.3/alpine/exchanges/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,20 @@
         :type access_key: None, str
         :param secret_key: Secret key to connect to the API.
         :type secret_key: None, str
         :param passphrase: Passphrase to connect to the API.
         :type passphrase: None, str
         """
         self.exchange_name = exchange_name
-        self.access_key = access_key or os.environ.get("API_ACCESS_KEY")
-        self.secret_key = secret_key or os.environ.get("API_SECRET_KEY")
-        self.passphrase = passphrase or os.environ.get("API_PASSPHRASE")
         module = importlib.import_module(f"alpine.exchanges.{exchange_name}")
         self.exchange = getattr(module, exchange_name.capitalize())()
+        self.exchange.access_key = access_key or os.environ.get("API_ACCESS_KEY")
+        self.exchange.secret_key = secret_key or os.environ.get("API_SECRET_KEY")
+        self.exchange.passphrase = passphrase or os.environ.get("API_PASSPHRASE")
+        
 
     def set_leverage(self, value, position, symbol, margin_coin):
         """
         Set the leverage to value.
         :param value: the leverage's value.
         :type value: int
         :param position: Position's direction.
```

### Comparing `crypto_alpine-0.1.2/PKG-INFO` & `crypto_alpine-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-alpine
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python library for cryptocurrency trading
 Author: pydavid
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests (>=2.31.0,<3.0.0)
```

