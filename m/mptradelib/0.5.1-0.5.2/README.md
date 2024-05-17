# Comparing `tmp/mptradelib-0.5.1.tar.gz` & `tmp/mptradelib-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mptradelib-0.5.1.tar", max compression
+gzip compressed data, was "mptradelib-0.5.2.tar", max compression
```

## Comparing `mptradelib-0.5.1.tar` & `mptradelib-0.5.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     3137 2024-05-03 13:20:41.913077 mptradelib-0.5.1/README.md
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.5.1/mptradelib/__init__.py
--rw-r--r--   0        0        0     4475 2024-05-16 13:35:32.766054 mptradelib-0.5.1/mptradelib/backtest.py
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.5.1/mptradelib/broker/__init__.py
--rw-r--r--   0        0        0    11073 2024-05-09 18:27:16.773912 mptradelib-0.5.1/mptradelib/broker/broker.py
--rw-r--r--   0        0        0     5808 2024-05-09 18:04:15.841857 mptradelib-0.5.1/mptradelib/broker/session.py
--rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.5.1/mptradelib/broker/shoonya.py
--rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.5.1/mptradelib/broker/ticker.py
--rw-r--r--   0        0        0        0 2024-05-03 11:19:20.268249 mptradelib-0.5.1/mptradelib/cli/__init__.py
--rw-r--r--   0        0        0     2342 2024-05-09 18:05:58.447254 mptradelib-0.5.1/mptradelib/cli/new.py
--rw-r--r--   0        0        0      953 2024-05-09 18:11:12.323673 mptradelib-0.5.1/mptradelib/cli/templates/strategy/__init__.py.jinja
--rw-r--r--   0        0        0     2984 2024-05-04 12:28:56.516490 mptradelib-0.5.1/mptradelib/cli/templates/strategy/backtest.ipynb.jinja
--rw-r--r--   0        0        0      614 2024-05-03 12:29:43.201283 mptradelib-0.5.1/mptradelib/cli/templates/strategy/livetrade.py.jinja
--rw-r--r--   0        0        0     5394 2024-05-09 18:03:46.504439 mptradelib-0.5.1/mptradelib/feed.py
--rw-r--r--   0        0        0     2007 2024-05-09 18:25:26.040938 mptradelib-0.5.1/mptradelib/livetrade.py
--rw-r--r--   0        0        0       36 2024-05-16 13:40:16.707824 mptradelib-0.5.1/mptradelib/optimizers/__init__.py
--rw-r--r--   0        0        0     3072 2024-05-16 13:38:31.319826 mptradelib-0.5.1/mptradelib/optimizers/walkforward.py
--rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.5.1/mptradelib/test_renko.py
--rw-r--r--   0        0        0       77 2024-05-06 16:16:12.200968 mptradelib-0.5.1/mptradelib/utils/__init__.py
--rw-r--r--   0        0        0      902 2024-05-06 16:14:19.221626 mptradelib-0.5.1/mptradelib/utils/simulated_trades.py
--rw-r--r--   0        0        0     6887 2024-05-12 12:25:21.588670 mptradelib-0.5.1/mptradelib/utils/tearsheet.py
--rw-r--r--   0        0        0      910 2024-05-06 16:15:09.786235 mptradelib-0.5.1/mptradelib/utils/utils.py
--rw-r--r--   0        0        0      846 2024-05-16 13:40:41.159590 mptradelib-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     4041 1970-01-01 00:00:00.000000 mptradelib-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     3137 2024-05-03 13:20:41.913077 mptradelib-0.5.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.5.2/mptradelib/__init__.py
+-rw-r--r--   0        0        0     4562 2024-05-17 20:17:00.043228 mptradelib-0.5.2/mptradelib/backtest.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.5.2/mptradelib/broker/__init__.py
+-rw-r--r--   0        0        0    11073 2024-05-09 18:27:16.773912 mptradelib-0.5.2/mptradelib/broker/broker.py
+-rw-r--r--   0        0        0     5808 2024-05-09 18:04:15.841857 mptradelib-0.5.2/mptradelib/broker/session.py
+-rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.5.2/mptradelib/broker/shoonya.py
+-rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.5.2/mptradelib/broker/ticker.py
+-rw-r--r--   0        0        0        0 2024-05-03 11:19:20.268249 mptradelib-0.5.2/mptradelib/cli/__init__.py
+-rw-r--r--   0        0        0     2342 2024-05-09 18:05:58.447254 mptradelib-0.5.2/mptradelib/cli/new.py
+-rw-r--r--   0        0        0      953 2024-05-09 18:11:12.323673 mptradelib-0.5.2/mptradelib/cli/templates/strategy/__init__.py.jinja
+-rw-r--r--   0        0        0     2984 2024-05-04 12:28:56.516490 mptradelib-0.5.2/mptradelib/cli/templates/strategy/backtest.ipynb.jinja
+-rw-r--r--   0        0        0      614 2024-05-03 12:29:43.201283 mptradelib-0.5.2/mptradelib/cli/templates/strategy/livetrade.py.jinja
+-rw-r--r--   0        0        0     5394 2024-05-09 18:03:46.504439 mptradelib-0.5.2/mptradelib/feed.py
+-rw-r--r--   0        0        0     2007 2024-05-09 18:25:26.040938 mptradelib-0.5.2/mptradelib/livetrade.py
+-rw-r--r--   0        0        0       36 2024-05-16 13:40:16.707824 mptradelib-0.5.2/mptradelib/optimizers/__init__.py
+-rw-r--r--   0        0        0     4949 2024-05-17 20:42:16.487036 mptradelib-0.5.2/mptradelib/optimizers/walkforward.py
+-rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.5.2/mptradelib/test_renko.py
+-rw-r--r--   0        0        0       77 2024-05-06 16:16:12.200968 mptradelib-0.5.2/mptradelib/utils/__init__.py
+-rw-r--r--   0        0        0      902 2024-05-06 16:14:19.221626 mptradelib-0.5.2/mptradelib/utils/simulated_trades.py
+-rw-r--r--   0        0        0     6887 2024-05-12 12:25:21.588670 mptradelib-0.5.2/mptradelib/utils/tearsheet.py
+-rw-r--r--   0        0        0      910 2024-05-06 16:15:09.786235 mptradelib-0.5.2/mptradelib/utils/utils.py
+-rw-r--r--   0        0        0      846 2024-05-17 20:42:27.418984 mptradelib-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4041 1970-01-01 00:00:00.000000 mptradelib-0.5.2/PKG-INFO
```

### Comparing `mptradelib-0.5.1/README.md` & `mptradelib-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.1/mptradelib/backtest.py` & `mptradelib-0.5.2/mptradelib/backtest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime as dt
 import pandas as pd
 from typing import Callable
-from tqdm import tqdm
 from retry import retry
 from .broker.broker import Order
 from itertools import product
+import multiprocessing as mp
 
 
 class Backtest:
     params: dict = {
         "sl": None,
         "tp": None
     }
@@ -100,26 +100,30 @@
     def _get_overfitting_score(self, t):
         t['abs_profit'] = t.profit.abs()
         ts = t.sort_values(by=['abs_profit'], ascending=False)
         os = (ts[:int(len(ts)/100)].abs_profit.sum()/ts.abs_profit.sum())*100
         rationalized_df = ts[int(len(ts)/100):]
         return os, rationalized_df
 
+    def _objective(self, params):
+        r, _ = self.run(**params)
+        os, rdf = self._get_overfitting_score(r.copy())
+        if os > 10:
+            r = rdf
+            print("removing event effect - ", params)
+        return {'params': params, 'trades': r}
+
+
     @retry(tries=10)
     def optimize(self, kwargs):
         opt_params, constant_params = self._define_space(kwargs)
         
-        def objective(params):
-            r, _ = self.run(**params)
-            os, rdf = self._get_overfitting_score(r.copy())
-            if os > 10:
-                r = rdf
-                print("removing event effect - ", param)
-            return {'params': params, 'trades': r}
-
         results = []
+        params = []
         for p in product(*opt_params.values()):
             param = dict(zip(opt_params.keys(), p))
             param.update(constant_params)
-            r = objective(param)
-            results.append(r)
+            params.append(param)
+            
+        with mp.Pool(mp.cpu_count()) as p:
+            results = p.map(self._objective, params)
         return results
```

### Comparing `mptradelib-0.5.1/mptradelib/broker/broker.py` & `mptradelib-0.5.2/mptradelib/broker/broker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.1/mptradelib/broker/session.py` & `mptradelib-0.5.2/mptradelib/broker/session.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.1/mptradelib/broker/shoonya.py` & `mptradelib-0.5.2/mptradelib/broker/shoonya.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.1/mptradelib/broker/ticker.py` & `mptradelib-0.5.2/mptradelib/broker/ticker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.1/mptradelib/cli/new.py` & `mptradelib-0.5.2/mptradelib/cli/new.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.1/mptradelib/cli/templates/strategy/__init__.py.jinja` & `mptradelib-0.5.2/mptradelib/cli/templates/strategy/__init__.py.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.1/mptradelib/cli/templates/strategy/backtest.ipynb.jinja` & `mptradelib-0.5.2/mptradelib/cli/templates/strategy/backtest.ipynb.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.1/mptradelib/cli/templates/strategy/livetrade.py.jinja` & `mptradelib-0.5.2/mptradelib/cli/templates/strategy/livetrade.py.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.1/mptradelib/feed.py` & `mptradelib-0.5.2/mptradelib/feed.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.1/mptradelib/livetrade.py` & `mptradelib-0.5.2/mptradelib/livetrade.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.1/mptradelib/test_renko.py` & `mptradelib-0.5.2/mptradelib/test_renko.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.1/mptradelib/utils/simulated_trades.py` & `mptradelib-0.5.2/mptradelib/utils/simulated_trades.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.1/mptradelib/utils/tearsheet.py` & `mptradelib-0.5.2/mptradelib/utils/tearsheet.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.1/mptradelib/utils/utils.py` & `mptradelib-0.5.2/mptradelib/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.1/pyproject.toml` & `mptradelib-0.5.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mptradelib"
-version = "0.5.1"
+version = "0.5.2"
 description = ""
 authors = ["Abhilash Nanda <wishabhilash@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "2.7.1"
```

### Comparing `mptradelib-0.5.1/PKG-INFO` & `mptradelib-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mptradelib
-Version: 0.5.1
+Version: 0.5.2
 Summary: 
 Author: Abhilash Nanda
 Author-email: wishabhilash@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

