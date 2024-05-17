# Comparing `tmp/pyqqq-0.9.7.tar.gz` & `tmp/pyqqq-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq-0.9.7.tar", max compression
+gzip compressed data, was "pyqqq-0.9.8.tar", max compression
```

## Comparing `pyqqq-0.9.7.tar` & `pyqqq-0.9.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.9.7/README.md
--rw-r--r--   0        0        0      791 2024-05-16 01:07:06.025646 pyqqq-0.9.7/pyproject.toml
--rw-r--r--   0        0        0     1606 2024-04-30 07:51:35.706752 pyqqq-0.9.7/pyqqq/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.9.7/pyqqq/brokerage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.9.7/pyqqq/brokerage/ebest/__init__.py
--rw-r--r--   0        0        0    43409 2024-05-07 06:54:47.220204 pyqqq-0.9.7/pyqqq/brokerage/ebest/domestic_stock.py
--rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.9.7/pyqqq/brokerage/ebest/oauth.py
--rw-r--r--   0        0        0    24448 2024-04-25 01:42:27.858549 pyqqq-0.9.7/pyqqq/brokerage/ebest/simple.py
--rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.9.7/pyqqq/brokerage/ebest/tr_client.py
--rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.9.7/pyqqq/brokerage/kis/__init__.py
--rw-r--r--   0        0        0   187522 2024-05-07 09:02:33.261786 pyqqq-0.9.7/pyqqq/brokerage/kis/domestic_stock.py
--rw-r--r--   0        0        0     5356 2024-04-23 09:05:13.260008 pyqqq-0.9.7/pyqqq/brokerage/kis/oauth.py
--rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.9.7/pyqqq/brokerage/kis/overseas_stock.py
--rw-r--r--   0        0        0    24390 2024-04-22 04:52:35.372119 pyqqq-0.9.7/pyqqq/brokerage/kis/simple.py
--rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.9.7/pyqqq/brokerage/kis/tr_client.py
--rw-r--r--   0        0        0      448 2024-04-12 04:14:38.633056 pyqqq-0.9.7/pyqqq/config.py
--rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.9.7/pyqqq/data/__init__.py
--rw-r--r--   0        0        0     5484 2024-05-16 01:05:45.085685 pyqqq-0.9.7/pyqqq/data/daily.py
--rw-r--r--   0        0        0     9684 2024-05-03 09:30:10.903300 pyqqq-0.9.7/pyqqq/data/domestic.py
--rw-r--r--   0        0        0     9628 2024-05-03 08:51:32.698077 pyqqq-0.9.7/pyqqq/data/minutes.py
--rw-r--r--   0        0        0     1521 2024-05-03 08:51:15.982807 pyqqq-0.9.7/pyqqq/data/realtime.py
--rw-r--r--   0        0        0     4136 2024-05-03 08:53:53.080239 pyqqq-0.9.7/pyqqq/data/ticks.py
--rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.9.7/pyqqq/datatypes.py
--rw-r--r--   0        0        0        0 2024-04-12 06:24:35.199779 pyqqq-0.9.7/pyqqq/executors/__init__.py
--rw-r--r--   0        0        0    38035 2024-04-16 05:04:16.530450 pyqqq-0.9.7/pyqqq/executors/hook.py
--rw-r--r--   0        0        0        0 2024-04-15 09:10:29.432687 pyqqq-0.9.7/pyqqq/utils/__init__.py
--rw-r--r--   0        0        0      519 2024-05-03 08:48:33.699191 pyqqq-0.9.7/pyqqq/utils/api_client.py
--rw-r--r--   0        0        0      941 2024-04-30 08:35:54.600146 pyqqq-0.9.7/pyqqq/utils/array.py
--rw-r--r--   0        0        0     3229 2024-04-30 08:36:37.055899 pyqqq-0.9.7/pyqqq/utils/compute.py
--rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.9.7/pyqqq/utils/display.py
--rw-r--r--   0        0        0     3962 2024-04-23 09:09:34.322415 pyqqq-0.9.7/pyqqq/utils/kvstore.py
--rw-r--r--   0        0        0     2641 2024-04-30 08:36:57.232261 pyqqq-0.9.7/pyqqq/utils/limiter.py
--rw-r--r--   0        0        0     2233 2024-04-30 07:41:29.806969 pyqqq-0.9.7/pyqqq/utils/logger.py
--rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.9.7/pyqqq/utils/market_schedule.py
--rw-r--r--   0        0        0    10571 2024-04-16 02:24:46.823810 pyqqq-0.9.7/pyqqq/utils/mock_api.py
--rw-r--r--   0        0        0     2065 2024-04-30 07:36:13.157361 pyqqq-0.9.7/pyqqq/utils/retry.py
--rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 pyqqq-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.9.8/README.md
+-rw-r--r--   0        0        0      773 2024-05-17 04:47:12.953268 pyqqq-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0     1606 2024-04-30 07:51:35.706752 pyqqq-0.9.8/pyqqq/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.9.8/pyqqq/brokerage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.9.8/pyqqq/brokerage/ebest/__init__.py
+-rw-r--r--   0        0        0    43409 2024-05-07 06:54:47.220204 pyqqq-0.9.8/pyqqq/brokerage/ebest/domestic_stock.py
+-rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.9.8/pyqqq/brokerage/ebest/oauth.py
+-rw-r--r--   0        0        0    24876 2024-05-17 02:28:30.291139 pyqqq-0.9.8/pyqqq/brokerage/ebest/simple.py
+-rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.9.8/pyqqq/brokerage/ebest/tr_client.py
+-rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.9.8/pyqqq/brokerage/kis/__init__.py
+-rw-r--r--   0        0        0   187522 2024-05-07 09:02:33.261786 pyqqq-0.9.8/pyqqq/brokerage/kis/domestic_stock.py
+-rw-r--r--   0        0        0     5356 2024-04-23 09:05:13.260008 pyqqq-0.9.8/pyqqq/brokerage/kis/oauth.py
+-rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.9.8/pyqqq/brokerage/kis/overseas_stock.py
+-rw-r--r--   0        0        0    24832 2024-05-17 02:31:00.627918 pyqqq-0.9.8/pyqqq/brokerage/kis/simple.py
+-rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.9.8/pyqqq/brokerage/kis/tr_client.py
+-rw-r--r--   0        0        0      448 2024-04-12 04:14:38.633056 pyqqq-0.9.8/pyqqq/config.py
+-rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.9.8/pyqqq/data/__init__.py
+-rw-r--r--   0        0        0     5484 2024-05-16 01:05:45.085685 pyqqq-0.9.8/pyqqq/data/daily.py
+-rw-r--r--   0        0        0     9684 2024-05-03 09:30:10.903300 pyqqq-0.9.8/pyqqq/data/domestic.py
+-rw-r--r--   0        0        0     9628 2024-05-03 08:51:32.698077 pyqqq-0.9.8/pyqqq/data/minutes.py
+-rw-r--r--   0        0        0     1521 2024-05-03 08:51:15.982807 pyqqq-0.9.8/pyqqq/data/realtime.py
+-rw-r--r--   0        0        0     4136 2024-05-03 08:53:53.080239 pyqqq-0.9.8/pyqqq/data/ticks.py
+-rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.9.8/pyqqq/datatypes.py
+-rw-r--r--   0        0        0        0 2024-04-12 06:24:35.199779 pyqqq-0.9.8/pyqqq/executors/__init__.py
+-rw-r--r--   0        0        0    38035 2024-04-16 05:04:16.530450 pyqqq-0.9.8/pyqqq/executors/hook.py
+-rw-r--r--   0        0        0        0 2024-04-15 09:10:29.432687 pyqqq-0.9.8/pyqqq/utils/__init__.py
+-rw-r--r--   0        0        0      519 2024-05-03 08:48:33.699191 pyqqq-0.9.8/pyqqq/utils/api_client.py
+-rw-r--r--   0        0        0      941 2024-04-30 08:35:54.600146 pyqqq-0.9.8/pyqqq/utils/array.py
+-rw-r--r--   0        0        0     3229 2024-04-30 08:36:37.055899 pyqqq-0.9.8/pyqqq/utils/compute.py
+-rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.9.8/pyqqq/utils/display.py
+-rw-r--r--   0        0        0     3962 2024-04-23 09:09:34.322415 pyqqq-0.9.8/pyqqq/utils/kvstore.py
+-rw-r--r--   0        0        0     2641 2024-04-30 08:36:57.232261 pyqqq-0.9.8/pyqqq/utils/limiter.py
+-rw-r--r--   0        0        0     2233 2024-04-30 07:41:29.806969 pyqqq-0.9.8/pyqqq/utils/logger.py
+-rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.9.8/pyqqq/utils/market_schedule.py
+-rw-r--r--   0        0        0    10571 2024-04-16 02:24:46.823810 pyqqq-0.9.8/pyqqq/utils/mock_api.py
+-rw-r--r--   0        0        0     2065 2024-04-30 07:36:13.157361 pyqqq-0.9.8/pyqqq/utils/retry.py
+-rw-r--r--   0        0        0     1553 1970-01-01 00:00:00.000000 pyqqq-0.9.8/PKG-INFO
```

### Comparing `pyqqq-0.9.7/README.md` & `pyqqq-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.7/pyproject.toml` & `pyqqq-0.9.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyqqq"
-version = "0.9.7"
+version = "0.9.8"
 description = "Package for quantitative strategy development on the PyQQQ platform"
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pyqqq"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
 
@@ -13,19 +13,18 @@
 tinydb = "^4.8.0"
 requests = "^2.31.0"
 python-dotenv = "^1.0.1"
 websockets = "^12.0"
 pandas = "^2.0.3"
 cssutils = "^2.10.2"
 cachetools = "^5.3.3"
-sphinx = "^7.3.7"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.2"
-sphinx = "^7.2.6"
+sphinx = "^7.2.7"
 myst-parser = "^2.0.0"
 ipykernel = "^6.29.4"
 pydata-sphinx-theme = "^0.15.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyqqq-0.9.7/pyqqq/__init__.py` & `pyqqq-0.9.8/pyqqq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.7/pyqqq/brokerage/ebest/domestic_stock.py` & `pyqqq-0.9.8/pyqqq/brokerage/ebest/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.7/pyqqq/brokerage/ebest/oauth.py` & `pyqqq-0.9.8/pyqqq/brokerage/ebest/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.7/pyqqq/brokerage/ebest/simple.py` & `pyqqq-0.9.8/pyqqq/brokerage/ebest/simple.py`

 * *Files 0% similar despite different names*

```diff
@@ -371,27 +371,31 @@
             - current_price (int): 현재 가격
             - volume (int): 거래량
             - open_price (int): 시가
             - high_price (int): 고가
             - low_price (int): 저가
             - max_price (int): 상한가
             - min_price (int): 하한가
+            - diff (int): 전일 대비 가격 변화
+            - diff_rate (float): 전일 대비 가격 변화율
         """
         r = self.stock_api.get_price(asset_code)
 
         data = r["output"]
         result = {
             "code": asset_code,
             "current_price": data["price"],
             "volume": data["volume"],
             "open_price": data["open"],
             "high_price": data["high"],
             "low_price": data["low"],
             "max_price": data["uplmtprice"],
             "min_price": data["dnlmtprice"],
+            "diff": data["change"],
+            "diff_rate": float(data["diff"]),
         }
 
         return result
 
     def get_price_for_multiple_stock(self, asset_codes: Set[str]) -> pd.DataFrame:
         """
         여러 종목의 현재 가격 조회
@@ -404,28 +408,32 @@
 
             - code (str): 종목 코드
             - current_price (int): 현재 가격
             - volume (int): 거래량
             - open_price (int): 시가
             - high_price (int): 고가
             - low_price (int): 저가
+            - diff (int): 전일 대비 가격 변화
+            - diff_rate (float): 전일 대비 가격 변화율
         """
         r = get_all_last_trades()
         result = []
 
         for item in r:
             if item["shcode"] in asset_codes:
                 result.append(
                     {
                         "code": item["shcode"],
                         "current_price": item["price"],
                         "volume": item["volume"],
                         "open_price": item["open"],
                         "high_price": item["high"],
                         "low_price": item["low"],
+                        "diff": item["change"],
+                        "diff_rate": round(item["drate"], 2),
                     }
                 )
 
         df = pd.DataFrame(result)
         df.set_index("code", inplace=True)
         return df
```

### Comparing `pyqqq-0.9.7/pyqqq/brokerage/ebest/tr_client.py` & `pyqqq-0.9.8/pyqqq/brokerage/ebest/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.7/pyqqq/brokerage/kis/domestic_stock.py` & `pyqqq-0.9.8/pyqqq/brokerage/kis/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.7/pyqqq/brokerage/kis/oauth.py` & `pyqqq-0.9.8/pyqqq/brokerage/kis/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.7/pyqqq/brokerage/kis/overseas_stock.py` & `pyqqq-0.9.8/pyqqq/brokerage/kis/overseas_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.7/pyqqq/brokerage/kis/simple.py` & `pyqqq-0.9.8/pyqqq/brokerage/kis/simple.py`

 * *Files 4% similar despite different names*

```diff
@@ -349,27 +349,31 @@
             - current_price (int): 현재 가격
             - volume (int): 거래량
             - open_price (int): 시가
             - high_price (int): 고가
             - low_price (int): 저가
             - max_price (int): 상한가
             - min_price (int): 하한가
+            - diff (int): 전일대비
+            - diff_rate (float): 전일대비율
         """
         r = self.stock_api.get_price(asset_code)
 
         data = r['output']
         result = {
-            'code': asset_code,
-            'current_price': data['stck_prpr'],
-            'volume': data['acml_vol'],
-            'open_price': data['stck_oprc'],
-            'high_price': data['stck_hgpr'],
-            'low_price': data['stck_lwpr'],
-            'max_price': data['stck_mxpr'],
-            'min_price': data['stck_llam'],
+            "code": asset_code,
+            "current_price": data["stck_prpr"],
+            "volume": data["acml_vol"],
+            "open_price": data["stck_oprc"],
+            "high_price": data["stck_hgpr"],
+            "low_price": data["stck_lwpr"],
+            "max_price": data["stck_mxpr"],
+            "min_price": data["stck_llam"],
+            "diff": data["prdy_vrss"],
+            "diff_rate": float(data["prdy_ctrt"]),
         }
 
         return result
 
     def get_price_for_multiple_stock(self, asset_codes: List[str]) -> pd.DataFrame:
         """
         여러 종목의 현재 가격 조회
@@ -382,28 +386,34 @@
 
             - code (str): 종목 코드
             - current_price (int): 현재 가격
             - volume (int): 거래량
             - open_price (int): 시가
             - high_price (int): 고가
             - low_price (int): 저가
+            - diff (int): 전일대비
+            - diff_rate (float): 전일대비율
         """
         r = get_all_last_trades()
         result = []
 
         for item in r:
             if item['shcode'] in asset_codes:
-                result.append({
-                    'code': item['shcode'],
-                    'current_price': item['price'],
-                    'volume': item['volume'],
-                    'open_price': item['open'],
-                    'high_price': item['high'],
-                    'low_price': item['low'],
-                })
+                result.append(
+                    {
+                        "code": item["shcode"],
+                        "current_price": item["price"],
+                        "volume": item["volume"],
+                        "open_price": item["open"],
+                        "high_price": item["high"],
+                        "low_price": item["low"],
+                        "diff": item["change"],
+                        "diff_rate": round(item["drate"], 2),
+                    }
+                )
 
         df = pd.DataFrame(result)
         df.set_index('code', inplace=True)
         return df
 
     @with_mock()
     def create_order(self,
```

### Comparing `pyqqq-0.9.7/pyqqq/brokerage/kis/tr_client.py` & `pyqqq-0.9.8/pyqqq/brokerage/kis/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.7/pyqqq/data/daily.py` & `pyqqq-0.9.8/pyqqq/data/daily.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.7/pyqqq/data/domestic.py` & `pyqqq-0.9.8/pyqqq/data/domestic.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.7/pyqqq/data/minutes.py` & `pyqqq-0.9.8/pyqqq/data/minutes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.7/pyqqq/data/realtime.py` & `pyqqq-0.9.8/pyqqq/data/realtime.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.7/pyqqq/data/ticks.py` & `pyqqq-0.9.8/pyqqq/data/ticks.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.7/pyqqq/datatypes.py` & `pyqqq-0.9.8/pyqqq/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.7/pyqqq/executors/hook.py` & `pyqqq-0.9.8/pyqqq/executors/hook.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.7/pyqqq/utils/api_client.py` & `pyqqq-0.9.8/pyqqq/utils/api_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.7/pyqqq/utils/array.py` & `pyqqq-0.9.8/pyqqq/utils/array.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.7/pyqqq/utils/compute.py` & `pyqqq-0.9.8/pyqqq/utils/compute.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.7/pyqqq/utils/display.py` & `pyqqq-0.9.8/pyqqq/utils/display.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.7/pyqqq/utils/kvstore.py` & `pyqqq-0.9.8/pyqqq/utils/kvstore.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.7/pyqqq/utils/limiter.py` & `pyqqq-0.9.8/pyqqq/utils/limiter.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.7/pyqqq/utils/logger.py` & `pyqqq-0.9.8/pyqqq/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.7/pyqqq/utils/market_schedule.py` & `pyqqq-0.9.8/pyqqq/utils/market_schedule.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.7/pyqqq/utils/mock_api.py` & `pyqqq-0.9.8/pyqqq/utils/mock_api.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.7/pyqqq/utils/retry.py` & `pyqqq-0.9.8/pyqqq/utils/retry.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.7/PKG-INFO` & `pyqqq-0.9.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqqq
-Version: 0.9.7
+Version: 0.9.8
 Summary: Package for quantitative strategy development on the PyQQQ platform
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cachetools (>=5.3.3,<6.0.0)
 Requires-Dist: cssutils (>=2.10.2,<3.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: sphinx (>=7.3.7,<8.0.0)
 Requires-Dist: tinydb (>=4.8.0,<5.0.0)
 Requires-Dist: websockets (>=12.0,<13.0)
 Project-URL: Documentation, https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io
 Description-Content-Type: text/markdown
 
 # PyQQQ SDK
```

