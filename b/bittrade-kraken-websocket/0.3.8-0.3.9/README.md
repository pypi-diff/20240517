# Comparing `tmp/bittrade_kraken_websocket-0.3.8.tar.gz` & `tmp/bittrade_kraken_websocket-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bittrade_kraken_websocket-0.3.8.tar", max compression
+gzip compressed data, was "bittrade_kraken_websocket-0.3.9.tar", max compression
```

## Comparing `bittrade_kraken_websocket-0.3.8.tar` & `bittrade_kraken_websocket-0.3.9.tar`

### file list

```diff
@@ -1,46 +1,48 @@
--rw-r--r--   0        0        0     3498 2023-01-09 19:54:47.619545 bittrade_kraken_websocket-0.3.8/README.md
--rw-r--r--   0        0        0     1790 2024-03-05 03:52:22.605034 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/__init__.py
--rw-r--r--   0        0        0      315 2024-03-05 03:47:46.867936 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/channels/__init__.py
--rw-r--r--   0        0        0      295 2022-12-29 22:39:59.260864 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/channels/channels.py
--rw-r--r--   0        0        0      103 2022-12-22 19:54:03.647594 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/channels/models/__init__.py
--rw-r--r--   0        0        0      292 2022-12-27 23:52:58.660279 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/channels/models/message.py
--rw-r--r--   0        0        0      175 2022-12-30 09:32:03.640719 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/channels/models/spread.py
--rw-r--r--   0        0        0      645 2022-12-26 10:08:11.875064 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/channels/models/ticker.py
--rw-r--r--   0        0        0      266 2024-03-05 03:43:45.307256 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/channels/models/trade.py
--rw-r--r--   0        0        0     6553 2024-02-16 04:38:44.856902 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/channels/open_orders.py
--rw-r--r--   0        0        0     4187 2023-01-07 09:53:43.396709 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/channels/own_trades.py
--rw-r--r--   0        0        0      369 2022-12-30 09:32:03.642502 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/channels/payload.py
--rw-r--r--   0        0        0      688 2024-02-16 04:38:44.858176 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/channels/spread.py
--rw-r--r--   0        0        0     3249 2023-01-13 21:38:44.629195 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/channels/subscribe.py
--rw-r--r--   0        0        0      867 2023-01-09 01:52:39.957750 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/channels/ticker.py
--rw-r--r--   0        0        0      732 2024-03-05 03:54:03.578673 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/channels/trade.py
--rw-r--r--   0        0        0      126 2023-01-02 09:55:34.234520 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/connection/__init__.py
--rw-r--r--   0        0        0     2301 2022-12-30 09:32:03.645535 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/connection/connection_operators.py
--rw-r--r--   0        0        0      892 2023-01-02 09:55:34.235207 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/connection/enhanced_websocket.py
--rw-r--r--   0        0        0     4290 2023-01-02 09:55:34.235882 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/connection/generic.py
--rw-r--r--   0        0        0      979 2023-01-11 10:23:20.547990 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/connection/private.py
--rw-r--r--   0        0        0      770 2023-01-11 10:23:20.548542 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/connection/public.py
--rw-r--r--   0        0        0     4062 2023-01-09 01:52:39.958583 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/connection/reconnect.py
--rw-r--r--   0        0        0      517 2023-01-02 09:55:34.238792 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/connection/status.py
--rw-r--r--   0        0        0     1811 2023-01-13 21:32:40.838805 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/development/__init__.py
--rw-r--r--   0        0        0      360 2024-02-16 04:38:44.860115 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/events/__init__.py
--rw-r--r--   0        0        0     5910 2024-02-16 04:38:44.860704 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/events/add_order.py
--rw-r--r--   0        0        0     2829 2024-02-16 04:38:44.861334 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/events/cancel_order.py
--rw-r--r--   0        0        0     3053 2024-02-16 04:38:44.861905 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/events/edit_order.py
--rw-r--r--   0        0        0      348 2022-12-27 23:47:27.251422 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/events/events.py
--rw-r--r--   0        0        0      179 2022-12-26 10:08:11.877126 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/events/ids.py
--rw-r--r--   0        0        0      345 2022-12-30 09:32:03.656774 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/events/message.py
--rw-r--r--   0        0        0       21 2022-12-27 23:40:15.935278 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/events/models/__init__.py
--rw-r--r--   0        0        0     1252 2023-01-03 09:00:51.951965 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/events/models/order.py
--rw-r--r--   0        0        0     4557 2022-12-25 10:37:02.309579 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/events/request_response.py
--rw-r--r--   0        0        0        0 2022-12-17 20:41:30.480872 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/messages/__init__.py
--rw-r--r--   0        0        0        0 2022-12-17 22:54:39.222667 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/messages/filters/__init__.py
--rw-r--r--   0        0        0      639 2022-12-29 22:45:19.511699 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/messages/filters/kind.py
--rw-r--r--   0        0        0      197 2022-12-17 21:16:58.319169 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/messages/heartbeat.py
--rw-r--r--   0        0        0      709 2022-12-17 21:40:37.447628 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/messages/json.py
--rw-r--r--   0        0        0     1249 2022-12-22 20:15:47.307161 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/messages/listen.py
--rw-r--r--   0        0        0     1632 2022-12-22 19:50:57.393583 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/messages/sequence.py
--rw-r--r--   0        0        0      364 2022-12-30 09:32:03.657481 bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/operators/__init__.py
--rw-r--r--   0        0        0     1589 2024-03-05 03:55:45.949462 bittrade_kraken_websocket-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     4741 1970-01-01 00:00:00.000000 bittrade_kraken_websocket-0.3.8/setup.py
--rw-r--r--   0        0        0     4495 1970-01-01 00:00:00.000000 bittrade_kraken_websocket-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     3498 2023-01-09 19:54:47.619545 bittrade_kraken_websocket-0.3.9/README.md
+-rw-r--r--   0        0        0     1930 2024-03-05 07:19:24.353452 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/__init__.py
+-rw-r--r--   0        0        0      315 2024-03-05 03:47:46.867936 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/channels/__init__.py
+-rw-r--r--   0        0        0      295 2022-12-29 22:39:59.260864 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/channels/channels.py
+-rw-r--r--   0        0        0      103 2022-12-22 19:54:03.647594 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/channels/models/__init__.py
+-rw-r--r--   0        0        0      292 2022-12-27 23:52:58.660279 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/channels/models/message.py
+-rw-r--r--   0        0        0      220 2024-03-05 07:40:32.164628 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/channels/models/ohlc.py
+-rw-r--r--   0        0        0      175 2022-12-30 09:32:03.640719 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/channels/models/spread.py
+-rw-r--r--   0        0        0      645 2022-12-26 10:08:11.875064 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/channels/models/ticker.py
+-rw-r--r--   0        0        0      209 2024-03-05 07:04:50.305029 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/channels/models/trade.py
+-rw-r--r--   0        0        0      660 2024-03-05 07:16:08.523345 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/channels/ohlc.py
+-rw-r--r--   0        0        0     6553 2024-02-16 04:38:44.856902 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/channels/open_orders.py
+-rw-r--r--   0        0        0     4187 2023-01-07 09:53:43.396709 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/channels/own_trades.py
+-rw-r--r--   0        0        0      369 2022-12-30 09:32:03.642502 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/channels/payload.py
+-rw-r--r--   0        0        0      688 2024-02-16 04:38:44.858176 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/channels/spread.py
+-rw-r--r--   0        0        0     3272 2024-03-05 07:34:54.115717 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/channels/subscribe.py
+-rw-r--r--   0        0        0      867 2023-01-09 01:52:39.957750 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/channels/ticker.py
+-rw-r--r--   0        0        0      732 2024-03-05 03:54:03.578673 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/channels/trade.py
+-rw-r--r--   0        0        0      126 2023-01-02 09:55:34.234520 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/connection/__init__.py
+-rw-r--r--   0        0        0     2301 2022-12-30 09:32:03.645535 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/connection/connection_operators.py
+-rw-r--r--   0        0        0      892 2023-01-02 09:55:34.235207 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/connection/enhanced_websocket.py
+-rw-r--r--   0        0        0     4290 2023-01-02 09:55:34.235882 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/connection/generic.py
+-rw-r--r--   0        0        0      979 2023-01-11 10:23:20.547990 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/connection/private.py
+-rw-r--r--   0        0        0      770 2023-01-11 10:23:20.548542 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/connection/public.py
+-rw-r--r--   0        0        0     4062 2023-01-09 01:52:39.958583 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/connection/reconnect.py
+-rw-r--r--   0        0        0      517 2023-01-02 09:55:34.238792 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/connection/status.py
+-rw-r--r--   0        0        0     1811 2023-01-13 21:32:40.838805 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/development/__init__.py
+-rw-r--r--   0        0        0      360 2024-02-16 04:38:44.860115 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/events/__init__.py
+-rw-r--r--   0        0        0     5910 2024-02-16 04:38:44.860704 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/events/add_order.py
+-rw-r--r--   0        0        0     2829 2024-02-16 04:38:44.861334 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/events/cancel_order.py
+-rw-r--r--   0        0        0     3053 2024-02-16 04:38:44.861905 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/events/edit_order.py
+-rw-r--r--   0        0        0      348 2022-12-27 23:47:27.251422 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/events/events.py
+-rw-r--r--   0        0        0      179 2022-12-26 10:08:11.877126 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/events/ids.py
+-rw-r--r--   0        0        0      345 2022-12-30 09:32:03.656774 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/events/message.py
+-rw-r--r--   0        0        0       21 2022-12-27 23:40:15.935278 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/events/models/__init__.py
+-rw-r--r--   0        0        0     1252 2023-01-03 09:00:51.951965 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/events/models/order.py
+-rw-r--r--   0        0        0     4557 2022-12-25 10:37:02.309579 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/events/request_response.py
+-rw-r--r--   0        0        0        0 2022-12-17 20:41:30.480872 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/messages/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-17 22:54:39.222667 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/messages/filters/__init__.py
+-rw-r--r--   0        0        0      862 2024-03-05 07:36:36.361882 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/messages/filters/kind.py
+-rw-r--r--   0        0        0      197 2022-12-17 21:16:58.319169 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/messages/heartbeat.py
+-rw-r--r--   0        0        0      709 2022-12-17 21:40:37.447628 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/messages/json.py
+-rw-r--r--   0        0        0     1249 2022-12-22 20:15:47.307161 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/messages/listen.py
+-rw-r--r--   0        0        0     1632 2022-12-22 19:50:57.393583 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/messages/sequence.py
+-rw-r--r--   0        0        0      364 2022-12-30 09:32:03.657481 bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/operators/__init__.py
+-rw-r--r--   0        0        0     1589 2024-03-05 07:49:30.159245 bittrade_kraken_websocket-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     4741 1970-01-01 00:00:00.000000 bittrade_kraken_websocket-0.3.9/setup.py
+-rw-r--r--   0        0        0     4495 1970-01-01 00:00:00.000000 bittrade_kraken_websocket-0.3.9/PKG-INFO
```

### Comparing `bittrade_kraken_websocket-0.3.8/README.md` & `bittrade_kraken_websocket-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/__init__.py` & `bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .channels.own_trades import (
     OwnTradesPayload,
     subscribe_own_trades,
     OwnTradesPayloadEntry,
     parse_own_trade,
     OwnTradesPayloadParsed,
 )
+from .channels.ohlc import OHLCPayload, to_ohlc_payload, subscribe_ohlc
 from .channels.open_orders import (
     subscribe_open_orders, 
     OpenOrdersPayload, 
     OpenOrdersPayloadEntry, 
     OpenOrdersPayloadEntryDescr, 
     initial_details_to_order, 
     is_cancel_message, 
@@ -35,14 +36,17 @@
     "initial_details_to_order", 
     "is_cancel_message", 
     "is_close_message", 
     "is_final_message",
     "is_initial_details",
     "is_open_message",
     "is_partial_fill_update", 
+    "OHLCPayload",
+    "subscribe_ohlc",
+    "to_ohlc_payload",
     "OpenOrdersPayload", 
     "OpenOrdersPayloadEntry", 
     "OpenOrdersPayloadEntryDescr", 
     "OwnTradesPayload",
     "OwnTradesPayloadEntry",
     "OwnTradesPayloadParsed",
     "parse_own_trade",
```

### Comparing `bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/channels/models/ticker.py` & `bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/channels/models/ticker.py`

 * *Files identical despite different names*

### Comparing `bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/channels/open_orders.py` & `bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/channels/open_orders.py`

 * *Files identical despite different names*

### Comparing `bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/channels/own_trades.py` & `bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/channels/own_trades.py`

 * *Files identical despite different names*

### Comparing `bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/channels/spread.py` & `bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/channels/spread.py`

 * *Files identical despite different names*

### Comparing `bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/channels/subscribe.py` & `bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/channels/subscribe.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     if is_private:
         messages_operators += [in_sequence(), retry_on_invalid_sequence()]
 
     def socket_to_channel_messages(
         socket: EnhancedWebsocket,
     ) -> Observable[PublicMessage | PrivateMessage]:
         return messages.pipe(
-            keep_channel_messages(channel, pair),
+            keep_channel_messages(channel, pair, subscription_keywords),
             channel_subscription(socket, channel, pair, subscription_keywords),
             *messages_operators,
         )
 
     return compose(
         operators.map(socket_to_channel_messages),
         operators.switch_latest(),
```

### Comparing `bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/channels/ticker.py` & `bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/channels/ticker.py`

 * *Files identical despite different names*

### Comparing `bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/channels/trade.py` & `bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/channels/trade.py`

 * *Files identical despite different names*

### Comparing `bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/connection/connection_operators.py` & `bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/connection/connection_operators.py`

 * *Files identical despite different names*

### Comparing `bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/connection/enhanced_websocket.py` & `bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/connection/enhanced_websocket.py`

 * *Files identical despite different names*

### Comparing `bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/connection/generic.py` & `bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/connection/generic.py`

 * *Files identical despite different names*

### Comparing `bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/connection/private.py` & `bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/connection/private.py`

 * *Files identical despite different names*

### Comparing `bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/connection/public.py` & `bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/connection/public.py`

 * *Files identical despite different names*

### Comparing `bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/connection/reconnect.py` & `bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/connection/reconnect.py`

 * *Files identical despite different names*

### Comparing `bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/connection/status.py` & `bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/connection/status.py`

 * *Files identical despite different names*

### Comparing `bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/development/__init__.py` & `bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/development/__init__.py`

 * *Files identical despite different names*

### Comparing `bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/events/add_order.py` & `bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/events/add_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/events/cancel_order.py` & `bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/events/cancel_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/events/edit_order.py` & `bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/events/edit_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/events/models/order.py` & `bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/events/models/order.py`

 * *Files identical despite different names*

### Comparing `bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/events/request_response.py` & `bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/events/request_response.py`

 * *Files identical despite different names*

### Comparing `bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/messages/json.py` & `bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/messages/json.py`

 * *Files identical despite different names*

### Comparing `bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/messages/listen.py` & `bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/messages/listen.py`

 * *Files identical despite different names*

### Comparing `bittrade_kraken_websocket-0.3.8/bittrade_kraken_websocket/messages/sequence.py` & `bittrade_kraken_websocket-0.3.9/bittrade_kraken_websocket/messages/sequence.py`

 * *Files identical despite different names*

### Comparing `bittrade_kraken_websocket-0.3.8/pyproject.toml` & `bittrade_kraken_websocket-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bittrade-kraken-websocket"
-version = "0.3.8"
+version = "0.3.9"
 description = "Reactive Websocket for Kraken"
 authors = ["mat <matt@techspace.asia>"]
 readme = "README.md"
 repository = "https://github.com/TechSpaceAsia/bittrade-kraken-websocket"
 homepage = "https://github.com/TechSpaceAsia/bittrade-kraken-websocket"
 license = "MIT"
 classifiers = [
```

### Comparing `bittrade_kraken_websocket-0.3.8/setup.py` & `bittrade_kraken_websocket-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  'orjson>=3.8.3,<4.0.0',
  'pydantic>=1.10.4,<2.0.0',
  'reactivex>=4.0.4,<5.0.0',
  'websocket-client>=1.4.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'bittrade-kraken-websocket',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': 'Reactive Websocket for Kraken',
     'long_description': '# Kraken Websocket\n\n[NOT RELEASED] This is very much a work in progress, despite being on pypi.\nMost things might be wrongly documented; API **will** change\n\n## Features\n\n- Reconnect with incremental backoff (per Kraken\'s recommendation)\n- Automatically reset subscription for private feeds when sequence is out of whack\n- request/response factories e.g. `add_order_factory` make websocket events feel like calling an API\n- ... but provides more info than a simple request/response; \n  for instance, `add_order` goes through each stage submitted->pending->open or canceled, \n  emitting a notification at each stage\n\n## Installing\n\n`pip install bittrade-kraken-websocket` or `poetry add bittrade-kraken-websocket`\n\n## General considerations\n\n### Observables/Reactivex\n\nThe whole library is build with [Reactivex](https://rxpy.readthedocs.io/en/latest/).\n\nThough Observables seem complicated at first, they are the best way to handle - and (synchronously) test - complex situations that arise over time, like an invalid sequence of messages or socket disconnection and backoff reconnects.\n\nFor simple use cases, they are also rather easy to use as shown in the [examples](./examples) folder or in the Getting Started below\n\n### Concurrency\n\nInternally the library uses threads.\nFor your main program you don\'t have to worry about threads; you can block the main thread.\n\n## Getting started\n\n### Connect to the public feeds\n\n```python\nfrom bittrade_kraken_websocket import public_websocket_connection, subscribe_ticker\nfrom bittrade_kraken_websocket.operators import keep_messages_only, filter_new_socket_only\n\n# Prepare connection - note, this is a ConnectableObservable, so it will only trigger connection when we call its ``connect`` method\nsocket_connection = public_websocket_connection()\n# Prepare a feed with only "real" messages, dropping things like status update, heartbeat, etc…\nmessages = socket_connection.pipe(\n    keep_messages_only(),\n)\nsocket_connection.pipe(\n    filter_new_socket_only(),\n    subscribe_ticker(\'USDT/USD\', messages)\n).subscribe(\n    print, print, print  # you can do anything with the messages; here we simply print them out\n)\nsocket_connection.connect()\n```\n\n_(This script is complete, it should run "as is")_\n\n\n## Logging\n\nWe use Python\'s standard logging.\nYou can modify what logs you see as follows:\n\n```\nlogging.getLogger(\'bittrade_kraken_websocket\').addHandler(logging.StreamHandler())\n```\n\n## Private feeds\n\nSimilar to [bittrade-kraken-rest](https://github.com/TechSpaceAsia/bittrade-kraken-rest), this library attempts to get as little access to sensitive information as possible.\n\nCurrently, you need to set the token onto the `EnhancedWebsocket`; this means we have no access to your Api key and secret.\nSince the token is connection based and can\'t be reused, this protects you as much as Kraken\'s current authentication method allows.\n\nIn the future we might even let you code your own `send_json` method instead.\n\nSee `examples/private_subscription.py` for an example of implementation\n\n```python\nnew_sockets = connection.pipe(\n    filter_new_socket_only(),\n    operators.map(add_token),\n    operators.share(),\n)\n```\n\n## Examples\n\nMost examples in the `examples` folder make use of the `development` module helpers and the rich logging. You will need to install the dependencies from the `rich` group to use them:\n\n`poetry add bittrade_kraken_websocket -E rich`',
     'author': 'mat',
     'author_email': 'matt@techspace.asia',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/TechSpaceAsia/bittrade-kraken-websocket',
```

### Comparing `bittrade_kraken_websocket-0.3.8/PKG-INFO` & `bittrade_kraken_websocket-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bittrade-kraken-websocket
-Version: 0.3.8
+Version: 0.3.9
 Summary: Reactive Websocket for Kraken
 Home-page: https://github.com/TechSpaceAsia/bittrade-kraken-websocket
 License: MIT
 Author: mat
 Author-email: matt@techspace.asia
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

