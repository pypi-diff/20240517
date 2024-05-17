# Comparing `tmp/prionet-0.0.1.tar.gz` & `tmp/prionet-0.0.2.tar.gz`

## Comparing `prionet-0.0.1.tar` & `prionet-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 prionet-0.0.1/src/PrioNet/__init__.py
--rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 prionet-0.0.1/src/PrioNet/bybit.py
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 prionet-0.0.1/src/PrioNet/log.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 prionet-0.0.1/src/PrioNet/telegram.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 prionet-0.0.1/tests/log.ipynb
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 prionet-0.0.1/.gitignore
--rw-r--r--   0        0        0    34502 2020-02-02 00:00:00.000000 prionet-0.0.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 prionet-0.0.1/README.md
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 prionet-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 prionet-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 prionet-0.0.2/PrioNet/__init__.py
+-rwxr-xr-x   0        0        0     5047 2020-02-02 00:00:00.000000 prionet-0.0.2/PrioNet/bybit.py
+-rwxr-xr-x   0        0        0     6921 2020-02-02 00:00:00.000000 prionet-0.0.2/PrioNet/framework.py
+-rwxr-xr-x   0        0        0     8272 2020-02-02 00:00:00.000000 prionet-0.0.2/PrioNet/log.py
+-rwxr-xr-x   0        0        0      668 2020-02-02 00:00:00.000000 prionet-0.0.2/PrioNet/telegram.py
+-rwxr-xr-x   0        0        0     2769 2020-02-02 00:00:00.000000 prionet-0.0.2/tests/log.ipynb
+-rwxr-xr-x   0        0        0      160 2020-02-02 00:00:00.000000 prionet-0.0.2/.gitignore
+-rwxr-xr-x   0        0        0    34502 2020-02-02 00:00:00.000000 prionet-0.0.2/LICENSE
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 prionet-0.0.2/README.md
+-rwxr-xr-x   0        0        0      512 2020-02-02 00:00:00.000000 prionet-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 prionet-0.0.2/PKG-INFO
```

### Comparing `prionet-0.0.1/src/PrioNet/bybit.py` & `prionet-0.0.2/PrioNet/bybit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from pybit.unified_trading import HTTP
 
-class ByBit:
-    def __init__(self, api_key, api_secret):
+class ByBitManager:
+    def __init__(self, api_key, api_secret, testnet=False, demo=False):
         ''' Initialize the ByBit API
 
         Parameters:
             - api_key (str): API key
             - api_secret (str): API secret
+            - testnet (bool): Testnet or not
         '''
-        self.session = HTTP(api_key, api_secret)
+        self.session = HTTP(api_key=api_key, api_secret=api_secret, testnet=testnet, demo=demo)
 
     def set_info(self, symbol, qty, tp, sl):
         ''' Set information for the order
 
         Parameters:
             - symbol (str): Symbol
             - qty (float): Quantity
@@ -36,19 +37,19 @@
         Returns:
             - bid_price (float): Bid price
             - bid_qty (float): Bid quantity
             - ask_price (float): Ask price
             - ask_qty (float): Ask quantity
         '''
         # Bid price -> Sell price
-        self.bid_price = self.session.get_orderbook(category="linear", symbol=self.symbol).get('result')['b'][0][0]
-        self.bid_qty = self.session.get_orderbook(category="linear", symbol=self.symbol).get('result')['b'][0][1]
+        self.bid_price = float(self.session.get_orderbook(category="linear", symbol=self.symbol).get('result')['b'][0][0])
+        self.bid_qty = float(self.session.get_orderbook(category="linear", symbol=self.symbol).get('result')['b'][0][1])
         # Ask price -> Buy price
-        self.ask_price = self.session.get_orderbook(category="linear", symbol=self.symbol).get('result')['a'][0][0]
-        self.ask_qty = self.session.get_orderbook(category="linear", symbol=self.symbol).get('result')['a'][0][1]
+        self.ask_price = float(self.session.get_orderbook(category="linear", symbol=self.symbol).get('result')['a'][0][0])
+        self.ask_qty = float(self.session.get_orderbook(category="linear", symbol=self.symbol).get('result')['a'][0][1])
         # Return prices
         return {
             'bid_price': self.bid_price,
             'bid_qty': self.bid_qty,
             'ask_price': self.ask_price,
             'ask_qty': self.ask_qty
         }
@@ -58,63 +59,63 @@
 
         Parameters:
             - side (str): Buy or Sell 
 
         Returns:
             - bool: Order placed successfully or not       
         '''
-        try:
-            # Register last side
-            self.side = side
+        # Register last side
+        self.side = side
+        # Check if the minimum quantity is respected
+        self.get_precision()
+        if self.qty < self.min_qty:
+            return None
+        else:
             # Get bid and ask prices
             self.bid_ask_prices()
-
             # Based on the side, place the order
             # Set stop loss and take profit
             if side == "Buy":
                 self.price = self.ask_price
-                self.take_profit = self.ask_price + (1 + self.tp)
-                self.stop_loss = self.ask_price - (1 + self.sl)
+                self.take_profit = self.ask_price * (1 + self.tp)
+                self.stop_loss = self.ask_price * (1 - self.sl)
             elif side == "Sell":
                 self.price = self.bid_price
-                self.take_profit = self.bid_price - (1 + self.tp)
-                self.stop_loss = self.bid_price + (1 + self.sl)
-
+                self.take_profit = self.bid_price * (1 - self.tp)
+                self.stop_loss = self.bid_price * (1 + self.sl)
             # Place order
-            order = self.session.place_active_order(
+            order = self.session.place_order(
                 category="linear", 
-                side=self.side, 
+                side=side, 
                 symbol=self.symbol, 
                 order_type="Market", 
-                qty=self.qty)
+                qty=self.qty,
+                takeProfit=self.take_profit,
+                stopLoss=self.stop_loss,)
             # Get order ID
-            self.order_id = order.get('result')['orderId']
-        except:
-            # Return that the order was not placed successfully
-            return False
-        
-        # Return that the order was placed successfully
-        return True
+            self.order_id = order['result']['orderId']
+            
+            # Return that the order was placed successfully
+            return order
 
     def get_position(self):
         ''' Get position informations
 
         Returns:
             - dict: Position informations
         '''
         # Get position
-        position = self.session.get_positions(category='linear', symbol=self.symbol)
-        # Order informations
-        order = position['result']['list'][0]
+        position = self.session.get_positions(category='linear', symbol=self.symbol)['result']['list'][0]
         # Get position informations
-        self.position_side = order['side']
-        self.position_size = order['size']
-        self.position_avgprice = order['avgPrice']
-        self.position_value = order['positionValue']
-        self.position_price = order['markPrice']
+        self.position_side = position['side']
+        self.position_size = position['size']
+        self.position_avgprice = position['avgPrice']
+        self.position_value = position['positionValue']
+        self.pnl = position['unrealisedPnl']
+        self.position_price = position['markPrice']
 
         # Return position informations
         return {
             'side': self.position_side,
             'size': self.position_size,
             'avgprice': self.position_avgprice,
             'value': self.position_value,
@@ -127,15 +128,15 @@
             - dict: Precision informations
         '''
         precision = self.session.get_instruments_info(
             category='linear',
             symbol=self.symbol
         )['result']['list'][0]
         # Get precision informations on quantity and price
-        self.min_qty = precision['lotSizeFilter']['qtyStep']
+        self.min_qty = float(precision['lotSizeFilter']['minOrderQty'])
         # At the moment, we are not using price precision
         # price = precision['priceFilter']['tickSize']
 
         # Return precision informations
         return {
             'min_qty': self.min_qty
         }
```

### Comparing `prionet-0.0.1/tests/log.ipynb` & `prionet-0.0.2/tests/log.ipynb`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9805803571428571%*

 * *Differences: {"'cells'": '{7: {\'execution_count\': 5, \'outputs\': {0: {\'data\': {\'text/plain\': ["\'Hello '*

 * *            'World!\\\\n\'"]}, \'execution_count\': 5}}}, 8: {\'execution_count\': 6, \'outputs\': '*

 * *            '{0: {\'data\': {\'text/plain\': ["\'Hello World!\\\\n\'"]}, \'execution_count\': '*

 * *            "6}}}, insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', "*

 * *            "OrderedDict()), ('source', ['## Log Test Notebook'])]))]}",*

 * * "'metadata'": "{'language_info': {'version': '3.10.13'} […]*

```diff
@@ -1,10 +1,17 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Log Test Notebook"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import sys\n",
                 "sys.path.append('../src')\\\n",
@@ -67,24 +74,24 @@
             "metadata": {},
             "source": [
                 "### Read File"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'NEUTRAL'"
+                            "'Hello World!\\n'"
                         ]
                     },
-                    "execution_count": 6,
+                    "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Create a log file trying to read a non-existing file\n",
                 "read_file(\n",
@@ -92,24 +99,24 @@
                 "    filename='test.log',\n",
                 "    default_content='NEUTRAL'\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'NEUTRAL'"
+                            "'Hello World!\\n'"
                         ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Read the log file content\n",
                 "read_file(\n",
@@ -131,13 +138,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.12.2"
+            "version": "3.10.13"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `prionet-0.0.1/LICENSE` & `prionet-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prionet-0.0.1/pyproject.toml` & `prionet-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PrioNet"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Giuseppe Priolo", email="priopio7@gmail.com" },
 ]
 description = "A package for analyizing financial data"
 readme = "README.md"
 requires-python = ">=3"
 classifiers = [
```

