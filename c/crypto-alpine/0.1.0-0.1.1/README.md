# Comparing `tmp/crypto_alpine-0.1.0.tar.gz` & `tmp/crypto_alpine-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto_alpine-0.1.0.tar", max compression
+gzip compressed data, was "crypto_alpine-0.1.1.tar", max compression
```

## Comparing `crypto_alpine-0.1.0.tar` & `crypto_alpine-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2024-05-13 11:50:38.758046 crypto_alpine-0.1.0/LICENSE
--rw-r--r--   0        0        0     1464 2024-05-13 13:21:37.598908 crypto_alpine-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-13 13:04:39.538997 crypto_alpine-0.1.0/alpine/__init__.py
--rw-r--r--   0        0        0       60 2024-05-13 11:45:52.899373 crypto_alpine-0.1.0/alpine/exchanges/__init__.py
--rw-r--r--   0        0        0      904 2024-05-13 11:45:52.895930 crypto_alpine-0.1.0/alpine/exchanges/abstract.py
--rw-r--r--   0        0        0     2061 2024-05-13 11:52:52.024579 crypto_alpine-0.1.0/alpine/exchanges/binance.py
--rw-r--r--   0        0        0     8441 2024-05-13 11:53:00.729945 crypto_alpine-0.1.0/alpine/exchanges/bitget.py
--rw-r--r--   0        0        0     1398 2024-05-13 11:45:52.907314 crypto_alpine-0.1.0/alpine/exchanges/utils.py
--rw-r--r--   0        0        0     4136 2024-05-13 11:45:52.897579 crypto_alpine-0.1.0/alpine/exchanges/wrapper.py
--rw-r--r--   0        0        0      342 2024-05-13 13:15:14.336302 crypto_alpine-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1851 1970-01-01 00:00:00.000000 crypto_alpine-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-13 11:50:38.758046 crypto_alpine-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1464 2024-05-13 13:21:37.598908 crypto_alpine-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-13 13:04:39.538997 crypto_alpine-0.1.1/alpine/__init__.py
+-rw-r--r--   0        0        0       60 2024-05-13 11:45:52.899373 crypto_alpine-0.1.1/alpine/exchanges/__init__.py
+-rw-r--r--   0        0        0     1105 2024-05-17 11:00:34.999485 crypto_alpine-0.1.1/alpine/exchanges/abstract.py
+-rw-r--r--   0        0        0     2061 2024-05-13 11:52:52.024579 crypto_alpine-0.1.1/alpine/exchanges/binance.py
+-rw-r--r--   0        0        0     9475 2024-05-17 11:00:35.044289 crypto_alpine-0.1.1/alpine/exchanges/bitget.py
+-rw-r--r--   0        0        0     1398 2024-05-13 11:45:52.907314 crypto_alpine-0.1.1/alpine/exchanges/utils.py
+-rw-r--r--   0        0        0     4765 2024-05-17 11:00:35.006805 crypto_alpine-0.1.1/alpine/exchanges/wrapper.py
+-rw-r--r--   0        0        0      342 2024-05-17 11:01:09.785579 crypto_alpine-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1851 1970-01-01 00:00:00.000000 crypto_alpine-0.1.1/PKG-INFO
```

### Comparing `crypto_alpine-0.1.0/LICENSE` & `crypto_alpine-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crypto_alpine-0.1.0/README.md` & `crypto_alpine-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `crypto_alpine-0.1.0/alpine/exchanges/abstract.py` & `crypto_alpine-0.1.1/alpine/exchanges/abstract.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,23 @@
         raise NotImplementedError
 
     @abc.abstractmethod
     def get_current_position(self, symbol, margin_coin):
         raise NotImplementedError
 
     @abc.abstractmethod
+    def close_position(self, symbol, position):
+        raise NotImplementedError
+
+    @abc.abstractmethod
     def get_historical_position(self, symbol, margin_coin, limit):
         raise NotImplementedError
 
     @abc.abstractmethod
     def create_order(
         self, position, symbol, price, amount, margin_coin, take_profit, stop_loss
     ):
         raise NotImplementedError
+
+    @abc.abstractmethod
+    def get_account_details(self):
+        raise NotImplementedError
```

### Comparing `crypto_alpine-0.1.0/alpine/exchanges/binance.py` & `crypto_alpine-0.1.1/alpine/exchanges/binance.py`

 * *Files identical despite different names*

### Comparing `crypto_alpine-0.1.0/alpine/exchanges/bitget.py` & `crypto_alpine-0.1.1/alpine/exchanges/bitget.py`

 * *Files 3% similar despite different names*

```diff
@@ -132,16 +132,16 @@
                 "marginCoin": margin_coin,
                 "marginMode": margin_mode,
                 "size": amount,
                 "price": price,
                 "side": side,
                 "tradeSide": trade_side,
                 "orderType": "limit" if price else "market",
-                # "presetStopSurplusPrice": take_profit,
-                # "presetStopLossPrice": stop_loss,
+                "presetStopSurplusPrice": take_profit,
+                "presetStopLossPrice": stop_loss,
             },
         )["data"]["orderId"]
 
     def get_order_detail(self, symbol, order_id):
         """
         Get details about an order.
         :param symbol: symbol to create an order for.
@@ -246,7 +246,43 @@
             "/api/v2/mix/market/symbol-price",
             {
                 "symbol": symbol,
                 "productType": product_type,
             },
         )["data"]
         return float(result[0][index])
+
+    def close_position(self, symbol, position):
+        """
+        Close the current position of the given the symbol.
+        :param symbol: symbol to close the current position.
+        :type symbol: str
+        :param position: Position's direction.
+        :type position: str
+        :returns: None
+        :rtype: None
+        """
+        product_type = "USDT-FUTURES"
+        return self.request(
+            "POST",
+            "/api/v2/mix/order/close-positions",
+            {
+                "symbol": symbol,
+                "holdSide": position,
+                "productType": product_type,
+            },
+        )["data"]
+
+    def get_account_details(self):
+        """
+        Get margin and equity details about the account.
+        :returns: The account details.
+        :rtype: dict
+        """
+        product_type = "USDT-FUTURES"
+        return self.request(
+            "GET",
+            "/api/v2/mix/account/accounts",
+            {
+                "productType": product_type,
+            },
+        )["data"]
```

### Comparing `crypto_alpine-0.1.0/alpine/exchanges/utils.py` & `crypto_alpine-0.1.1/alpine/exchanges/utils.py`

 * *Files identical despite different names*

### Comparing `crypto_alpine-0.1.0/alpine/exchanges/wrapper.py` & `crypto_alpine-0.1.1/alpine/exchanges/wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -106,7 +106,27 @@
         :type margin_coin: str
         :param limit: The limit of historical positions to retrieve for the symbol.
         :type limit: int
         :returns: the position details.
         :rtype: dict
         """
         return self.exchange.get_historical_position(symbol, margin_coin, limit)
+
+    def close_position(self, symbol, position):
+        """
+        Close the current position of the given the symbol.
+        :param symbol: symbol to close the current position.
+        :type symbol: str
+        :param position: Position's direction.
+        :type position: str
+        :returns: None
+        :rtype: None
+        """
+        return self.exchange.close_position(symbol, position)
+
+    def get_account_details(self):
+        """
+        Get margin and equity details about the account.
+        :returns: The account details.
+        :rtype: dict
+        """
+        return self.exchange.get_account_details()
```

### Comparing `crypto_alpine-0.1.0/PKG-INFO` & `crypto_alpine-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-alpine
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python library for cryptocurrency trading
 Author: pydavid
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests (>=2.31.0,<3.0.0)
```

