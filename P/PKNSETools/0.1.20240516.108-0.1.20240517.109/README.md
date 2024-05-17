# Comparing `tmp/PKNSETools-0.1.20240516.108.tar.gz` & `tmp/PKNSETools-0.1.20240517.109.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKNSETools-0.1.20240516.108.tar", last modified: Thu May 16 18:16:50 2024, max compression
+gzip compressed data, was "PKNSETools-0.1.20240517.109.tar", last modified: Fri May 17 03:23:34 2024, max compression
```

## Comparing `PKNSETools-0.1.20240516.108.tar` & `PKNSETools-0.1.20240517.109.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 18:16:50.546068 PKNSETools-0.1.20240516.108/
--rw-rw-rw-   0        0        0     2663 2024-05-16 18:16:50.546068 PKNSETools-0.1.20240516.108/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-16 18:16:50.530445 PKNSETools-0.1.20240516.108/PKNSETools/
-drwxrwxrwx   0        0        0        0 2024-05-16 18:16:50.546068 PKNSETools-0.1.20240516.108/PKNSETools/Benny/
--rw-rw-rw-   0        0        0    34274 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/Benny/NSE.py
--rw-rw-rw-   0        0        0     1198 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/Benny/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 18:16:50.546068 PKNSETools-0.1.20240516.108/PKNSETools/Nasdaq/
--rw-rw-rw-   0        0        0     3386 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/Nasdaq/PKNasdaqIndex.py
--rw-rw-rw-   0        0        0     1225 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/Nasdaq/__init__.py
--rw-rw-rw-   0        0        0     4806 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/PKAllStocks.py
--rw-rw-rw-   0        0        0    10770 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/PKCompanyGeneral.py
--rw-rw-rw-   0        0        0     3303 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/PKCompanyStock.py
--rw-rw-rw-   0        0        0     2635 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/PKConstants.py
--rw-rw-rw-   0        0        0    10388 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/PKIntraDay.py
--rw-rw-rw-   0        0        0    16561 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/PKNSEStockDataFetcher.py
--rw-rw-rw-   0        0        0       31 2024-05-16 18:16:45.000000 PKNSETools-0.1.20240516.108/PKNSETools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 18:16:50.546068 PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/
--rw-rw-rw-   0        0        0     1830 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/NSEStockDB.py
--rw-rw-rw-   0        0        0     1848 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/NSEStockFairValueDB.py
--rw-rw-rw-   0        0        0     1836 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/NSEStockMFIDB.py
--rw-rw-rw-   0        0        0    61961 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
--rw-rw-rw-   0        0        0     1378 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/__init__.py
--rw-rw-rw-   0        0        0     2000 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/error.py
--rw-rw-rw-   0        0        0    40060 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/funds.py
--rw-rw-rw-   0        0        0    22038 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/search.py
--rw-rw-rw-   0        0        0    13495 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/security.py
--rw-rw-rw-   0        0        0    29916 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/stock.py
--rw-rw-rw-   0        0        0    23246 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-16 18:16:50.546068 PKNSETools-0.1.20240516.108/PKNSETools.egg-info/
--rw-rw-rw-   0        0        0     2663 2024-05-16 18:16:50.000000 PKNSETools-0.1.20240516.108/PKNSETools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1004 2024-05-16 18:16:50.000000 PKNSETools-0.1.20240516.108/PKNSETools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 18:16:50.000000 PKNSETools-0.1.20240516.108/PKNSETools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-16 18:16:43.000000 PKNSETools-0.1.20240516.108/PKNSETools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       79 2024-05-16 18:16:50.000000 PKNSETools-0.1.20240516.108/PKNSETools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-16 18:16:50.000000 PKNSETools-0.1.20240516.108/PKNSETools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1884 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/README.md
--rw-rw-rw-   0        0        0       86 2024-05-16 18:16:50.546068 PKNSETools-0.1.20240516.108/setup.cfg
--rw-rw-rw-   0        0        0     3832 2024-05-16 18:15:04.000000 PKNSETools-0.1.20240516.108/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 03:23:34.425099 PKNSETools-0.1.20240517.109/
+-rw-rw-rw-   0        0        0     2663 2024-05-17 03:23:34.425099 PKNSETools-0.1.20240517.109/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-17 03:23:34.425099 PKNSETools-0.1.20240517.109/PKNSETools/
+drwxrwxrwx   0        0        0        0 2024-05-17 03:23:34.425099 PKNSETools-0.1.20240517.109/PKNSETools/Benny/
+-rw-rw-rw-   0        0        0    34274 2024-05-17 03:21:36.000000 PKNSETools-0.1.20240517.109/PKNSETools/Benny/NSE.py
+-rw-rw-rw-   0        0        0     1198 2024-05-17 03:21:36.000000 PKNSETools-0.1.20240517.109/PKNSETools/Benny/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 03:23:34.425099 PKNSETools-0.1.20240517.109/PKNSETools/Nasdaq/
+-rw-rw-rw-   0        0        0     3386 2024-05-17 03:21:36.000000 PKNSETools-0.1.20240517.109/PKNSETools/Nasdaq/PKNasdaqIndex.py
+-rw-rw-rw-   0        0        0     1225 2024-05-17 03:21:36.000000 PKNSETools-0.1.20240517.109/PKNSETools/Nasdaq/__init__.py
+-rw-rw-rw-   0        0        0     4806 2024-05-17 03:21:36.000000 PKNSETools-0.1.20240517.109/PKNSETools/PKAllStocks.py
+-rw-rw-rw-   0        0        0    10770 2024-05-17 03:21:36.000000 PKNSETools-0.1.20240517.109/PKNSETools/PKCompanyGeneral.py
+-rw-rw-rw-   0        0        0     3303 2024-05-17 03:21:36.000000 PKNSETools-0.1.20240517.109/PKNSETools/PKCompanyStock.py
+-rw-rw-rw-   0        0        0     2635 2024-05-17 03:21:36.000000 PKNSETools-0.1.20240517.109/PKNSETools/PKConstants.py
+-rw-rw-rw-   0        0        0    10388 2024-05-17 03:21:36.000000 PKNSETools-0.1.20240517.109/PKNSETools/PKIntraDay.py
+-rw-rw-rw-   0        0        0    16561 2024-05-17 03:21:36.000000 PKNSETools-0.1.20240517.109/PKNSETools/PKNSEStockDataFetcher.py
+-rw-rw-rw-   0        0        0       31 2024-05-17 03:23:30.000000 PKNSETools-0.1.20240517.109/PKNSETools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 03:23:34.425099 PKNSETools-0.1.20240517.109/PKNSETools/morningstartools/
+-rw-rw-rw-   0        0        0     1830 2024-05-17 03:21:36.000000 PKNSETools-0.1.20240517.109/PKNSETools/morningstartools/NSEStockDB.py
+-rw-rw-rw-   0        0        0     1848 2024-05-17 03:21:36.000000 PKNSETools-0.1.20240517.109/PKNSETools/morningstartools/NSEStockFairValueDB.py
+-rw-rw-rw-   0        0        0     1836 2024-05-17 03:21:36.000000 PKNSETools-0.1.20240517.109/PKNSETools/morningstartools/NSEStockMFIDB.py
+-rw-rw-rw-   0        0        0    61961 2024-05-17 03:21:36.000000 PKNSETools-0.1.20240517.109/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
+-rw-rw-rw-   0        0        0     1378 2024-05-17 03:21:36.000000 PKNSETools-0.1.20240517.109/PKNSETools/morningstartools/__init__.py
+-rw-rw-rw-   0        0        0     2000 2024-05-17 03:21:36.000000 PKNSETools-0.1.20240517.109/PKNSETools/morningstartools/error.py
+-rw-rw-rw-   0        0        0    40060 2024-05-17 03:21:36.000000 PKNSETools-0.1.20240517.109/PKNSETools/morningstartools/funds.py
+-rw-rw-rw-   0        0        0    22038 2024-05-17 03:21:36.000000 PKNSETools-0.1.20240517.109/PKNSETools/morningstartools/search.py
+-rw-rw-rw-   0        0        0    13495 2024-05-17 03:21:36.000000 PKNSETools-0.1.20240517.109/PKNSETools/morningstartools/security.py
+-rw-rw-rw-   0        0        0    29916 2024-05-17 03:21:36.000000 PKNSETools-0.1.20240517.109/PKNSETools/morningstartools/stock.py
+-rw-rw-rw-   0        0        0    23246 2024-05-17 03:21:36.000000 PKNSETools-0.1.20240517.109/PKNSETools/morningstartools/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-17 03:23:34.425099 PKNSETools-0.1.20240517.109/PKNSETools.egg-info/
+-rw-rw-rw-   0        0        0     2663 2024-05-17 03:23:34.000000 PKNSETools-0.1.20240517.109/PKNSETools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1004 2024-05-17 03:23:34.000000 PKNSETools-0.1.20240517.109/PKNSETools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 03:23:34.000000 PKNSETools-0.1.20240517.109/PKNSETools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-17 03:23:28.000000 PKNSETools-0.1.20240517.109/PKNSETools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       79 2024-05-17 03:23:34.000000 PKNSETools-0.1.20240517.109/PKNSETools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-17 03:23:34.000000 PKNSETools-0.1.20240517.109/PKNSETools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1884 2024-05-17 03:21:36.000000 PKNSETools-0.1.20240517.109/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-17 03:23:34.425099 PKNSETools-0.1.20240517.109/setup.cfg
+-rw-rw-rw-   0        0        0     3832 2024-05-17 03:21:36.000000 PKNSETools-0.1.20240517.109/setup.py
```

### Comparing `PKNSETools-0.1.20240516.108/PKG-INFO` & `PKNSETools-0.1.20240517.109/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240516.108
+Version: 0.1.20240517.109
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240516.108.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240517.109.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240516.108/PKNSETools/Benny/NSE.py` & `PKNSETools-0.1.20240517.109/PKNSETools/Benny/NSE.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240516.108/PKNSETools/Benny/__init__.py` & `PKNSETools-0.1.20240517.109/PKNSETools/Benny/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240516.108/PKNSETools/Nasdaq/PKNasdaqIndex.py` & `PKNSETools-0.1.20240517.109/PKNSETools/Nasdaq/PKNasdaqIndex.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240516.108/PKNSETools/Nasdaq/__init__.py` & `PKNSETools-0.1.20240517.109/PKNSETools/Nasdaq/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240516.108/PKNSETools/PKAllStocks.py` & `PKNSETools-0.1.20240517.109/PKNSETools/PKAllStocks.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240516.108/PKNSETools/PKCompanyGeneral.py` & `PKNSETools-0.1.20240517.109/PKNSETools/PKCompanyGeneral.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240516.108/PKNSETools/PKCompanyStock.py` & `PKNSETools-0.1.20240517.109/PKNSETools/PKCompanyStock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240516.108/PKNSETools/PKConstants.py` & `PKNSETools-0.1.20240517.109/PKNSETools/PKConstants.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240516.108/PKNSETools/PKIntraDay.py` & `PKNSETools-0.1.20240517.109/PKNSETools/PKIntraDay.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240516.108/PKNSETools/PKNSEStockDataFetcher.py` & `PKNSETools-0.1.20240517.109/PKNSETools/PKNSEStockDataFetcher.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/NSEStockDB.py` & `PKNSETools-0.1.20240517.109/PKNSETools/morningstartools/NSEStockDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/NSEStockFairValueDB.py` & `PKNSETools-0.1.20240517.109/PKNSETools/morningstartools/NSEStockFairValueDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/NSEStockMFIDB.py` & `PKNSETools-0.1.20240517.109/PKNSETools/morningstartools/NSEStockMFIDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/PKMorningstarDataFetcher.py` & `PKNSETools-0.1.20240517.109/PKNSETools/morningstartools/PKMorningstarDataFetcher.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/__init__.py` & `PKNSETools-0.1.20240517.109/PKNSETools/morningstartools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/error.py` & `PKNSETools-0.1.20240517.109/PKNSETools/morningstartools/error.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/funds.py` & `PKNSETools-0.1.20240517.109/PKNSETools/morningstartools/funds.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/search.py` & `PKNSETools-0.1.20240517.109/PKNSETools/morningstartools/search.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/security.py` & `PKNSETools-0.1.20240517.109/PKNSETools/morningstartools/security.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/stock.py` & `PKNSETools-0.1.20240517.109/PKNSETools/morningstartools/stock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240516.108/PKNSETools/morningstartools/utils.py` & `PKNSETools-0.1.20240517.109/PKNSETools/morningstartools/utils.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240516.108/PKNSETools.egg-info/PKG-INFO` & `PKNSETools-0.1.20240517.109/PKNSETools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240516.108
+Version: 0.1.20240517.109
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240516.108.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240517.109.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240516.108/PKNSETools.egg-info/SOURCES.txt` & `PKNSETools-0.1.20240517.109/PKNSETools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240516.108/README.md` & `PKNSETools-0.1.20240517.109/README.md`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240516.108/setup.py` & `PKNSETools-0.1.20240517.109/setup.py`

 * *Files identical despite different names*

