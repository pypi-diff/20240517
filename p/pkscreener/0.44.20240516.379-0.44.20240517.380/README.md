# Comparing `tmp/pkscreener-0.44.20240516.379.tar.gz` & `tmp/pkscreener-0.44.20240517.380.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240516.379.tar", last modified: Thu May 16 10:22:34 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240517.380.tar", last modified: Fri May 17 03:37:14 2024, max compression
```

## Comparing `pkscreener-0.44.20240516.379.tar` & `pkscreener-0.44.20240517.380.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 10:22:34.961543 pkscreener-0.44.20240516.379/
--rw-rw-rw-   0        0        0     1086 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-16 10:22:34.961543 pkscreener-0.44.20240516.379/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 10:22:34.945945 pkscreener-0.44.20240516.379/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 10:22:34.961543 pkscreener-0.44.20240516.379/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1537 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    34250 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11407 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    43311 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    12534 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    24534 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    22221 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18947 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   155530 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    56135 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4993 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    84725 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3789 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-16 10:22:24.000000 pkscreener-0.44.20240516.379/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   141394 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/globals.py
--rw-rw-rw-   0        0        0     1090 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    53036 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    33750 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-16 10:22:34.945945 pkscreener-0.44.20240516.379/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-16 10:22:34.000000 pkscreener-0.44.20240516.379/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-16 10:22:34.000000 pkscreener-0.44.20240516.379/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 10:22:34.000000 pkscreener-0.44.20240516.379/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-16 10:22:34.000000 pkscreener-0.44.20240516.379/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-16 10:22:34.000000 pkscreener-0.44.20240516.379/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-16 10:22:34.000000 pkscreener-0.44.20240516.379/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-16 10:22:34.961543 pkscreener-0.44.20240516.379/setup.cfg
--rw-rw-rw-   0        0        0     4765 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 03:37:14.339276 pkscreener-0.44.20240517.380/
+-rw-rw-rw-   0        0        0     1086 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-17 03:37:14.339276 pkscreener-0.44.20240517.380/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 03:37:14.323648 pkscreener-0.44.20240517.380/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 03:37:14.339276 pkscreener-0.44.20240517.380/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1537 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    34250 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11407 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    43311 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    12534 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    24598 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    22369 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18947 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   156140 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    56357 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4993 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    84725 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3789 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-17 03:37:04.000000 pkscreener-0.44.20240517.380/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   141484 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/globals.py
+-rw-rw-rw-   0        0        0     1090 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    53036 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    33946 2024-05-17 03:32:25.000000 pkscreener-0.44.20240517.380/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-17 03:37:14.339276 pkscreener-0.44.20240517.380/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-17 03:37:14.000000 pkscreener-0.44.20240517.380/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-17 03:37:14.000000 pkscreener-0.44.20240517.380/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 03:37:14.000000 pkscreener-0.44.20240517.380/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-17 03:37:14.000000 pkscreener-0.44.20240517.380/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-17 03:37:14.000000 pkscreener-0.44.20240517.380/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-17 03:37:14.000000 pkscreener-0.44.20240517.380/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-17 03:37:14.339276 pkscreener-0.44.20240517.380/setup.cfg
+-rw-rw-rw-   0        0        0     4765 2024-05-17 03:32:26.000000 pkscreener-0.44.20240517.380/setup.py
```

### Comparing `pkscreener-0.44.20240516.379/LICENSE` & `pkscreener-0.44.20240517.380/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/LICENSE-Others` & `pkscreener-0.44.20240517.380/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/PKG-INFO` & `pkscreener-0.44.20240517.380/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240516.379
+Version: 0.44.20240517.380
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240516.379.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240517.380.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.378/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.379/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.378/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.379/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.378/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.379/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240516.379/README.md` & `pkscreener-0.44.20240517.380/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.378/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.379/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.378/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.379/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.378/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.379/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240516.379/pkscreener/__init__.py` & `pkscreener-0.44.20240517.380/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/pkscreener/classes/ArtTexts.py` & `pkscreener-0.44.20240517.380/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240517.380/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240517.380/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240517.380/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240517.380/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240517.380/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240517.380/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240517.380/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240517.380/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240517.380/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240517.380/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240517.380/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         Utility.tools.saveStockData(allDailyCandles,PKMarketOpenCloseAnalyser.configManager,1,False,False, True)
 
     def ensureIntradayStockDataExists():
         # Ensure that the intraday_stock_data_<date>.pkl file exists
         exists, cache_file = Utility.tools.afterMarketStockDataExists(intraday=True)
         copyFilePath = os.path.join(Archiver.get_user_outputs_dir(), f"copy_{cache_file}")
         srcFilePath = os.path.join(Archiver.get_user_outputs_dir(), cache_file)
-        srcFileSize = os.stat(srcFilePath).st_size
+        srcFileSize = os.stat(srcFilePath).st_size if os.path.exists(srcFilePath) else 0
         if exists and srcFileSize < 1024*1024*50:
              # File less than 30MB ? Must have been corrupted
             try:
                 os.remove(srcFilePath)
                 exists = False
             except:
                 pass
@@ -133,15 +133,15 @@
         return exists, cache_file
 
     def ensureDailyStockDataExists():
         # Ensure that the stock_data_<date>.pkl file exists
         exists, cache_file = Utility.tools.afterMarketStockDataExists(intraday=False)
         copyFilePath = os.path.join(Archiver.get_user_outputs_dir(), f"copy_{cache_file}")
         srcFilePath = os.path.join(Archiver.get_user_outputs_dir(), cache_file)
-        srcFileSize = os.stat(srcFilePath).st_size
+        srcFileSize = os.stat(srcFilePath).st_size if os.path.exists(srcFilePath) else 0
         if exists and srcFileSize < 1024*1024*50:
              # File less than 30MB ? Must have been corrupted
             try:
                 os.remove(srcFilePath)
                 exists = False
             except:
                 pass
@@ -362,15 +362,15 @@
             screen_df.loc[:, col] = save_df.loc[:, col].apply(
                 lambda x: x if col in ["LTP@Alert","AlertTime", "SqrOff", "SqrOffLTP", "EoDLTP","DayHigh","DayHighTime"] else ((colorText.GREEN if x >= 0 else colorText.FAIL) + str(x) + colorText.END)
             )
 
         columns = save_df.columns
         lastIndex = len(save_df)
         for col in columns:
-            if col in ["Stock", "Pattern", "LTP", "SqrOffLTP","SqrOffDiff","DayHigh","DayHighDiff","AlertTime", "EoDLTP", "EoDDiff", "%Chng"]:
+            if col in ["Stock", "Pattern", "LTP", "SqrOffLTP","SqrOffDiff","DayHigh","DayHighDiff", "EoDLTP", "EoDDiff", "%Chng"]:
                 if col == "Stock":
                     save_df.loc[lastIndex,col] = "PORTFOLIO"
                 elif col == "Pattern":
                     save_df.loc[lastIndex,col] = runOptionName if runOptionName is not None else ""
                 elif col in ["LTP", "SqrOffLTP","SqrOffDiff", "EoDLTP", "EoDDiff","DayHigh","DayHighDiff"]:
                     save_df.loc[lastIndex,col] = round(sum(save_df[col].dropna(inplace=False).astype(float)),2)
                 elif col == "%Chng":
```

### Comparing `pkscreener-0.44.20240516.379/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240517.380/pkscreener/classes/PKScanRunner.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,20 +93,20 @@
                 "Trend",
                 "Pattern",
                 "CCI",
             ]
         )
         return screenResults, saveResults
 
-    def initQueues(minimumCount=0):
+    def initQueues(minimumCount=0,userPassedArgs=None):
         tasks_queue = multiprocessing.JoinableQueue()
         results_queue = multiprocessing.Queue()
         logging_queue = multiprocessing.Queue()
 
-        totalConsumers = min(minimumCount, multiprocessing.cpu_count())
+        totalConsumers = 1 if (userPassedArgs is not None and userPassedArgs.singlethread is not None) else min(minimumCount, multiprocessing.cpu_count())
         if totalConsumers == 1:
             totalConsumers = 2  # This is required for single core machine
         if PKScanRunner.configManager.cacheEnabled is True and multiprocessing.cpu_count() > 2:
             totalConsumers -= 1
         return tasks_queue, results_queue, totalConsumers, logging_queue
 
     def populateQueues(items, tasks_queue, exit=False,userPassedArgs=None):
@@ -249,15 +249,15 @@
         for worker in consumers:
             worker.objectDictionaryPrimary = stockDictPrimary
             worker.objectDictionarySecondary = stockDictSecondary
             worker.refreshDatabase = True
             
     def runScanWithParams(userPassedArgs,keyboardInterruptEvent,screenCounter,screenResultsCounter,stockDictPrimary,stockDictSecondary,testing, backtestPeriod, menuOption, executeOption, samplingDuration, items,screenResults, saveResults, backtest_df,scanningCb,tasks_queue, results_queue, consumers,logging_queue):
         if tasks_queue is None or results_queue is None or consumers is None:
-            tasks_queue, results_queue, consumers,logging_queue = PKScanRunner.prepareToRunScan(menuOption,keyboardInterruptEvent,screenCounter, screenResultsCounter, stockDictPrimary,stockDictSecondary, items,executeOption)
+            tasks_queue, results_queue, consumers,logging_queue = PKScanRunner.prepareToRunScan(menuOption,keyboardInterruptEvent,screenCounter, screenResultsCounter, stockDictPrimary,stockDictSecondary, items,executeOption,userPassedArgs)
             try:
                 if logging_queue is not None:
                     log_queue_reader = LogQueueReader(logging_queue)
                     log_queue_reader.start()
             except:
                 pass
         # if executeOption == 29: # Intraday Bid/Ask, for which we need to fetch data from NSE instead of yahoo
@@ -290,53 +290,53 @@
             # Don't terminate the multiprocessing clients if we're 
             # going to pipe the results from an earlier run
             # or we're running in monitoring mode
             PKScanRunner.terminateAllWorkers(userPassedArgs,consumers, tasks_queue, testing)
         return screenResults, saveResults,backtest_df,tasks_queue, results_queue, consumers, logging_queue
 
     @exit_after(180) # Should not remain stuck starting the multiprocessing clients beyond this time
-    def prepareToRunScan(menuOption,keyboardInterruptEvent, screenCounter, screenResultsCounter, stockDictPrimary,stockDictSecondary, items, executeOption):
-        tasks_queue, results_queue, totalConsumers, logging_queue = PKScanRunner.initQueues(len(items))
+    def prepareToRunScan(menuOption,keyboardInterruptEvent, screenCounter, screenResultsCounter, stockDictPrimary,stockDictSecondary, items, executeOption,userPassedArgs):
+        tasks_queue, results_queue, totalConsumers, logging_queue = PKScanRunner.initQueues(len(items),userPassedArgs)
         scr = ScreeningStatistics.ScreeningStatistics(PKScanRunner.configManager, default_logger())
         exists, cache_file = Utility.tools.afterMarketStockDataExists(intraday=PKScanRunner.configManager.isIntradayConfig())
         sec_cache_file = cache_file if "intraday_" in cache_file else f"intraday_{cache_file}"
         consumers = [
                     PKMultiProcessorClient(
                         StockScreener().screenStocks,
                         tasks_queue,
                         results_queue,
                         logging_queue,
                         screenCounter,
                         screenResultsCounter,
-                        stockDictPrimary,
-                        stockDictSecondary,
-                        # (stockDictPrimary if menuOption not in ["C"] else None),
-                        # (stockDictSecondary if menuOption not in ["C"] else None),
+                        # stockDictPrimary,
+                        # stockDictSecondary,
+                        (stockDictPrimary if menuOption not in ["C"] else None),
+                        (stockDictSecondary if menuOption not in ["C"] else None),
                         PKScanRunner.fetcher.proxyServer,
                         keyboardInterruptEvent,
                         default_logger(),
                         PKScanRunner.fetcher,
                         PKScanRunner.configManager,
                         PKScanRunner.candlePatterns,
                         scr,
-                        None,
-                        None
-                        # (cache_file if (exists and menuOption in ["C"]) else None),
-                        # (sec_cache_file if (exists and menuOption in ["C"]) else None),
+                        # None,
+                        # None
+                        (cache_file if (exists and menuOption in ["C"]) else None),
+                        (sec_cache_file if (exists and menuOption in ["C"]) else None),
                     )
                     for _ in range(totalConsumers)
                 ]
         # if executeOption == 29: # Intraday Bid/Ask, for which we need to fetch data from NSE instead of yahoo
         intradayFetcher = Intra_Day("SBINEQN") # This will initialise the cookies etc.
         for consumer in consumers:
             consumer.intradayNSEFetcher = intradayFetcher
         PKScanRunner.startWorkers(consumers)
         return tasks_queue,results_queue,consumers,logging_queue
 
-    @exit_after(180) # Should not remain stuck starting the multiprocessing clients beyond this time
+    @exit_after(120) # Should not remain stuck starting the multiprocessing clients beyond this time
     def startWorkers(consumers):
         try:
             from pytest_cov.embed import cleanup_on_signal, cleanup_on_sigterm
         except ImportError:
             pass
         else:
             if sys.platform.startswith("win"):
```

### Comparing `pkscreener-0.44.20240516.379/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240517.380/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240517.380/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240517.380/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240517.380/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240517.380/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240517.380/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240517.380/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240517.380/pkscreener/classes/ScreeningStatistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -5190,4532 +5190,4570 @@
 00014450: 7572 655f 7469 6d65 0d0a 2020 2020 6465  ure_time..    de
 00014460: 6620 6669 6e64 5570 7472 656e 6428 7365  f findUptrend(se
 00014470: 6c66 2c20 6466 2c20 7363 7265 656e 4469  lf, df, screenDi
 00014480: 6374 2c20 7361 7665 4469 6374 2c20 7465  ct, saveDict, te
 00014490: 7374 696e 672c 2073 746f 636b 2c6f 6e6c  sting, stock,onl
 000144a0: 794d 463d 4661 6c73 652c 686f 7374 4461  yMF=False,hostDa
 000144b0: 7461 3d4e 6f6e 652c 6578 6368 616e 6765  ta=None,exchange
-000144c0: 4e61 6d65 3d22 494e 4449 4122 293a 0d0a  Name="INDIA"):..
-000144d0: 2020 2020 2020 2020 2320 7368 6f75 6c64          # should
-000144e0: 5072 6f63 6565 6420 3d20 5472 7565 0d0a  Proceed = True..
-000144f0: 2020 2020 2020 2020 6973 5570 7472 656e          isUptren
-00014500: 6420 3d20 4661 6c73 650d 0a20 2020 2020  d = False..     
-00014510: 2020 2069 7344 6f77 6e74 7265 6e64 203d     isDowntrend =
-00014520: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-00014530: 6973 3530 444d 4155 7074 7265 6e64 203d  is50DMAUptrend =
-00014540: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-00014550: 6973 3530 444d 4144 6f77 6e74 7265 6e64  is50DMADowntrend
-00014560: 203d 2046 616c 7365 0d0a 2020 2020 2020   = False..      
-00014570: 2020 6465 6369 7369 6f6e 203d 2022 220d    decision = "".
-00014580: 0a20 2020 2020 2020 2064 6d61 3530 6465  .        dma50de
-00014590: 6369 7369 6f6e 203d 2022 220d 0a20 2020  cision = ""..   
-000145a0: 2020 2020 2066 6169 7256 616c 7565 203d       fairValue =
-000145b0: 2030 0d0a 2020 2020 2020 2020 6661 6972   0..        fair
-000145c0: 5661 6c75 6544 6966 6620 3d20 300d 0a20  ValueDiff = 0.. 
-000145d0: 2020 2020 2020 2023 2069 6620 6466 2069         # if df i
-000145e0: 7320 4e6f 6e65 206f 7220 6c65 6e28 6466  s None or len(df
-000145f0: 2920 3c20 3232 3020 6f72 2074 6573 7469  ) < 220 or testi
-00014600: 6e67 3a0d 0a20 2020 2020 2020 2023 2020  ng:..        #  
-00014610: 2020 2073 686f 756c 6450 726f 6365 6564     shouldProceed
-00014620: 203d 2046 616c 7365 0d0a 2020 2020 2020   = False..      
-00014630: 2020 6966 2064 6620 6973 206e 6f74 204e    if df is not N
-00014640: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00014650: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-00014660: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-00014670: 662e 636f 7079 2829 0d0a 2020 2020 2020  f.copy()..      
-00014680: 2020 2020 2020 2020 2020 6461 7461 203d            data =
-00014690: 2064 6174 615b 3a3a 2d31 5d0d 0a20 2020   data[::-1]..   
-000146a0: 2020 2020 2020 2020 2020 2020 2074 6f64               tod
-000146b0: 6179 5f73 6d61 203d 2070 6b74 616c 6962  ay_sma = pktalib
-000146c0: 2e53 4d41 2864 6174 615b 2243 6c6f 7365  .SMA(data["Close
-000146d0: 225d 2c20 7469 6d65 7065 7269 6f64 3d35  "], timeperiod=5
-000146e0: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
-000146f0: 2020 2020 736d 615f 6d69 6e75 7339 203d      sma_minus9 =
-00014700: 2070 6b74 616c 6962 2e53 4d41 2864 6174   pktalib.SMA(dat
-00014710: 612e 6865 6164 286c 656e 2864 6174 6129  a.head(len(data)
-00014720: 2d39 295b 2243 6c6f 7365 225d 2c20 7469  -9)["Close"], ti
-00014730: 6d65 7065 7269 6f64 3d35 3029 0d0a 2020  meperiod=50)..  
-00014740: 2020 2020 2020 2020 2020 2020 2020 736d                sm
-00014750: 615f 6d69 6e75 7331 3420 3d20 706b 7461  a_minus14 = pkta
-00014760: 6c69 622e 534d 4128 6461 7461 2e68 6561  lib.SMA(data.hea
-00014770: 6428 6c65 6e28 6461 7461 292d 3134 295b  d(len(data)-14)[
-00014780: 2243 6c6f 7365 225d 2c20 7469 6d65 7065  "Close"], timepe
-00014790: 7269 6f64 3d35 3029 0d0a 2020 2020 2020  riod=50)..      
-000147a0: 2020 2020 2020 2020 2020 736d 615f 6d69            sma_mi
-000147b0: 6e75 7332 3020 3d20 706b 7461 6c69 622e  nus20 = pktalib.
-000147c0: 534d 4128 6461 7461 2e68 6561 6428 6c65  SMA(data.head(le
-000147d0: 6e28 6461 7461 292d 3230 295b 2243 6c6f  n(data)-20)["Clo
-000147e0: 7365 225d 2c20 7469 6d65 7065 7269 6f64  se"], timeperiod
-000147f0: 3d35 3029 0d0a 2020 2020 2020 2020 2020  =50)..          
-00014800: 2020 2020 2020 746f 6461 795f 6c6d 6120        today_lma 
-00014810: 3d20 706b 7461 6c69 622e 534d 4128 6461  = pktalib.SMA(da
-00014820: 7461 5b22 436c 6f73 6522 5d2c 2074 696d  ta["Close"], tim
-00014830: 6570 6572 696f 643d 3230 3029 0d0a 2020  eperiod=200)..  
-00014840: 2020 2020 2020 2020 2020 2020 2020 6c6d                lm
-00014850: 615f 6d69 6e75 7332 3020 3d20 706b 7461  a_minus20 = pkta
-00014860: 6c69 622e 534d 4128 6461 7461 2e68 6561  lib.SMA(data.hea
-00014870: 6428 6c65 6e28 6461 7461 292d 3230 295b  d(len(data)-20)[
-00014880: 2243 6c6f 7365 225d 2c20 7469 6d65 7065  "Close"], timepe
-00014890: 7269 6f64 3d32 3030 290d 0a20 2020 2020  riod=200)..     
-000148a0: 2020 2020 2020 2020 2020 206c 6d61 5f6d             lma_m
-000148b0: 696e 7573 3830 203d 2070 6b74 616c 6962  inus80 = pktalib
-000148c0: 2e53 4d41 2864 6174 612e 6865 6164 286c  .SMA(data.head(l
-000148d0: 656e 2864 6174 6129 2d38 3029 5b22 436c  en(data)-80)["Cl
-000148e0: 6f73 6522 5d2c 2074 696d 6570 6572 696f  ose"], timeperio
-000148f0: 643d 3230 3029 0d0a 2020 2020 2020 2020  d=200)..        
-00014900: 2020 2020 2020 2020 6c6d 615f 6d69 6e75          lma_minu
-00014910: 7331 3030 203d 2070 6b74 616c 6962 2e53  s100 = pktalib.S
-00014920: 4d41 2864 6174 612e 6865 6164 286c 656e  MA(data.head(len
-00014930: 2864 6174 6129 2d31 3030 295b 2243 6c6f  (data)-100)["Clo
-00014940: 7365 225d 2c20 7469 6d65 7065 7269 6f64  se"], timeperiod
-00014950: 3d32 3030 290d 0a20 2020 2020 2020 2020  =200)..         
-00014960: 2020 2020 2020 2074 6f64 6179 5f6c 6d61         today_lma
-00014970: 203d 2074 6f64 6179 5f6c 6d61 2e69 6c6f   = today_lma.ilo
-00014980: 635b 6c65 6e28 746f 6461 795f 6c6d 6129  c[len(today_lma)
-00014990: 2d31 5d20 6966 2074 6f64 6179 5f6c 6d61  -1] if today_lma
-000149a0: 2069 7320 6e6f 7420 4e6f 6e65 2065 6c73   is not None els
-000149b0: 6520 300d 0a20 2020 2020 2020 2020 2020  e 0..           
-000149c0: 2020 2020 206c 6d61 5f6d 696e 7573 3230       lma_minus20
-000149d0: 203d 206c 6d61 5f6d 696e 7573 3230 2e69   = lma_minus20.i
-000149e0: 6c6f 635b 6c65 6e28 6c6d 615f 6d69 6e75  loc[len(lma_minu
-000149f0: 7332 3029 2d31 5d20 6966 206c 6d61 5f6d  s20)-1] if lma_m
-00014a00: 696e 7573 3230 2069 7320 6e6f 7420 4e6f  inus20 is not No
-00014a10: 6e65 2065 6c73 6520 300d 0a20 2020 2020  ne else 0..     
-00014a20: 2020 2020 2020 2020 2020 206c 6d61 5f6d             lma_m
-00014a30: 696e 7573 3830 203d 206c 6d61 5f6d 696e  inus80 = lma_min
-00014a40: 7573 3830 2e69 6c6f 635b 6c65 6e28 6c6d  us80.iloc[len(lm
-00014a50: 615f 6d69 6e75 7338 3029 2d31 5d20 6966  a_minus80)-1] if
-00014a60: 206c 6d61 5f6d 696e 7573 3830 2069 7320   lma_minus80 is 
-00014a70: 6e6f 7420 4e6f 6e65 2065 6c73 6520 300d  not None else 0.
-00014a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014a90: 206c 6d61 5f6d 696e 7573 3130 3020 3d20   lma_minus100 = 
-00014aa0: 6c6d 615f 6d69 6e75 7331 3030 2e69 6c6f  lma_minus100.ilo
-00014ab0: 635b 6c65 6e28 6c6d 615f 6d69 6e75 7331  c[len(lma_minus1
-00014ac0: 3030 292d 315d 2069 6620 6c6d 615f 6d69  00)-1] if lma_mi
-00014ad0: 6e75 7331 3030 2069 7320 6e6f 7420 4e6f  nus100 is not No
-00014ae0: 6e65 2065 6c73 6520 300d 0a20 2020 2020  ne else 0..     
-00014af0: 2020 2020 2020 2020 2020 2074 6f64 6179             today
-00014b00: 5f73 6d61 203d 2074 6f64 6179 5f73 6d61  _sma = today_sma
-00014b10: 2e69 6c6f 635b 6c65 6e28 746f 6461 795f  .iloc[len(today_
-00014b20: 736d 6129 2d31 5d20 6966 2074 6f64 6179  sma)-1] if today
-00014b30: 5f73 6d61 2069 7320 6e6f 7420 4e6f 6e65  _sma is not None
-00014b40: 2065 6c73 6520 300d 0a20 2020 2020 2020   else 0..       
-00014b50: 2020 2020 2020 2020 2073 6d61 5f6d 696e           sma_min
-00014b60: 7573 3920 3d20 736d 615f 6d69 6e75 7339  us9 = sma_minus9
-00014b70: 2e69 6c6f 635b 6c65 6e28 736d 615f 6d69  .iloc[len(sma_mi
-00014b80: 6e75 7339 292d 315d 2069 6620 736d 615f  nus9)-1] if sma_
-00014b90: 6d69 6e75 7339 2069 7320 6e6f 7420 4e6f  minus9 is not No
-00014ba0: 6e65 2065 6c73 6520 300d 0a20 2020 2020  ne else 0..     
-00014bb0: 2020 2020 2020 2020 2020 2073 6d61 5f6d             sma_m
-00014bc0: 696e 7573 3134 203d 2073 6d61 5f6d 696e  inus14 = sma_min
-00014bd0: 7573 3134 2e69 6c6f 635b 6c65 6e28 736d  us14.iloc[len(sm
-00014be0: 615f 6d69 6e75 7331 3429 2d31 5d20 6966  a_minus14)-1] if
-00014bf0: 2073 6d61 5f6d 696e 7573 3134 2069 7320   sma_minus14 is 
-00014c00: 6e6f 7420 4e6f 6e65 2065 6c73 6520 300d  not None else 0.
-00014c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014c20: 2073 6d61 5f6d 696e 7573 3230 203d 2073   sma_minus20 = s
-00014c30: 6d61 5f6d 696e 7573 3230 2e69 6c6f 635b  ma_minus20.iloc[
-00014c40: 6c65 6e28 736d 615f 6d69 6e75 7332 3029  len(sma_minus20)
-00014c50: 2d31 5d20 6966 2073 6d61 5f6d 696e 7573  -1] if sma_minus
-00014c60: 3230 2069 7320 6e6f 7420 4e6f 6e65 2065  20 is not None e
-00014c70: 6c73 6520 300d 0a20 2020 2020 2020 2020  lse 0..         
-00014c80: 2020 2020 2020 2069 7355 7074 7265 6e64         isUptrend
-00014c90: 203d 2028 746f 6461 795f 6c6d 6120 3e20   = (today_lma > 
-00014ca0: 6c6d 615f 6d69 6e75 7332 3029 206f 7220  lma_minus20) or 
-00014cb0: 2874 6f64 6179 5f6c 6d61 203e 206c 6d61  (today_lma > lma
-00014cc0: 5f6d 696e 7573 3830 2920 6f72 2028 746f  _minus80) or (to
-00014cd0: 6461 795f 6c6d 6120 3e20 6c6d 615f 6d69  day_lma > lma_mi
-00014ce0: 6e75 7331 3030 290d 0a20 2020 2020 2020  nus100)..       
-00014cf0: 2020 2020 2020 2020 2069 7344 6f77 6e74           isDownt
-00014d00: 7265 6e64 203d 2028 746f 6461 795f 6c6d  rend = (today_lm
-00014d10: 6120 3c20 6c6d 615f 6d69 6e75 7332 3029  a < lma_minus20)
-00014d20: 2061 6e64 2028 746f 6461 795f 6c6d 6120   and (today_lma 
-00014d30: 3c20 6c6d 615f 6d69 6e75 7338 3029 2061  < lma_minus80) a
-00014d40: 6e64 2028 746f 6461 795f 6c6d 6120 3c20  nd (today_lma < 
-00014d50: 6c6d 615f 6d69 6e75 7331 3030 290d 0a20  lma_minus100).. 
-00014d60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00014d70: 7335 3044 4d41 5570 7472 656e 6420 3d20  s50DMAUptrend = 
-00014d80: 2874 6f64 6179 5f73 6d61 203e 2073 6d61  (today_sma > sma
-00014d90: 5f6d 696e 7573 3929 206f 7220 2874 6f64  _minus9) or (tod
-00014da0: 6179 5f73 6d61 203e 2073 6d61 5f6d 696e  ay_sma > sma_min
-00014db0: 7573 3134 2920 6f72 2028 746f 6461 795f  us14) or (today_
-00014dc0: 736d 6120 3e20 736d 615f 6d69 6e75 7332  sma > sma_minus2
-00014dd0: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
-00014de0: 2020 2020 6973 3530 444d 4144 6f77 6e74      is50DMADownt
-00014df0: 7265 6e64 203d 2028 746f 6461 795f 736d  rend = (today_sm
-00014e00: 6120 3c20 736d 615f 6d69 6e75 7339 2920  a < sma_minus9) 
-00014e10: 616e 6420 2874 6f64 6179 5f73 6d61 203c  and (today_sma <
-00014e20: 2073 6d61 5f6d 696e 7573 3134 2920 616e   sma_minus14) an
-00014e30: 6420 2874 6f64 6179 5f73 6d61 203c 2073  d (today_sma < s
-00014e40: 6d61 5f6d 696e 7573 3230 290d 0a20 2020  ma_minus20)..   
-00014e50: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-00014e60: 4578 6365 7074 696f 6e3a 2020 2320 7072  Exception:  # pr
-00014e70: 6167 6d61 3a20 6e6f 2063 6f76 6572 0d0a  agma: no cover..
-00014e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e90: 2320 7365 6c66 2e64 6566 6175 6c74 5f6c  # self.default_l
-00014ea0: 6f67 6765 722e 6465 6275 6728 652c 2065  ogger.debug(e, e
-00014eb0: 7863 5f69 6e66 6f3d 5472 7565 290d 0a20  xc_info=True).. 
-00014ec0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00014ed0: 6173 730d 0a20 2020 2020 2020 2064 6563  ass..        dec
-00014ee0: 6973 696f 6e20 3d20 2754 3ae2 96b2 2720  ision = 'T:...' 
-00014ef0: 6966 2069 7355 7074 7265 6e64 2065 6c73  if isUptrend els
-00014f00: 6520 2827 543a e296 bc27 2069 6620 6973  e ('T:...' if is
-00014f10: 446f 776e 7472 656e 6420 656c 7365 2027  Downtrend else '
-00014f20: 2729 0d0a 2020 2020 2020 2020 646d 6135  ')..        dma5
-00014f30: 3064 6563 6973 696f 6e20 3d20 2774 3ae2  0decision = 't:.
-00014f40: 96b2 2720 6966 2069 7335 3044 4d41 5570  ..' if is50DMAUp
-00014f50: 7472 656e 6420 656c 7365 2028 2774 3ae2  trend else ('t:.
-00014f60: 96bc 2720 6966 2069 7335 3044 4d41 446f  ..' if is50DMADo
-00014f70: 776e 7472 656e 6420 656c 7365 2027 2729  wntrend else '')
-00014f80: 0d0a 2020 2020 2020 2020 6d66 5f69 6e73  ..        mf_ins
-00014f90: 745f 6f77 6e65 7273 6869 7043 6861 6e67  t_ownershipChang
-00014fa0: 6520 3d20 300d 0a20 2020 2020 2020 2063  e = 0..        c
-00014fb0: 6861 6e67 655f 6d69 6c6c 696f 6e73 203d  hange_millions =
-00014fc0: 2222 0d0a 2020 2020 2020 2020 7472 793a  ""..        try:
-00014fd0: 0d0a 2020 2020 2020 2020 2020 2020 6d66  ..            mf
-00014fe0: 5f69 6e73 745f 6f77 6e65 7273 6869 7043  _inst_ownershipC
-00014ff0: 6861 6e67 6520 3d20 7365 6c66 2e67 6574  hange = self.get
-00015000: 4d75 7475 616c 4675 6e64 5374 6174 7573  MutualFundStatus
-00015010: 2873 746f 636b 2c6f 6e6c 794d 463d 6f6e  (stock,onlyMF=on
-00015020: 6c79 4d46 2c68 6f73 7444 6174 613d 686f  lyMF,hostData=ho
-00015030: 7374 4461 7461 2c66 6f72 6365 3d28 686f  stData,force=(ho
-00015040: 7374 4461 7461 2069 7320 4e6f 6e65 206f  stData is None o
-00015050: 7220 686f 7374 4461 7461 2e65 6d70 7479  r hostData.empty
-00015060: 206f 7220 6e6f 7420 2822 4d46 2220 696e   or not ("MF" in
-00015070: 2068 6f73 7444 6174 612e 636f 6c75 6d6e   hostData.column
-00015080: 7320 6f72 2022 4649 4922 2069 6e20 686f  s or "FII" in ho
-00015090: 7374 4461 7461 2e63 6f6c 756d 6e73 2929  stData.columns))
-000150a0: 2c65 7863 6861 6e67 654e 616d 653d 6578  ,exchangeName=ex
-000150b0: 6368 616e 6765 4e61 6d65 290d 0a20 2020  changeName)..   
-000150c0: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
-000150d0: 7374 616e 6365 286d 665f 696e 7374 5f6f  stance(mf_inst_o
-000150e0: 776e 6572 7368 6970 4368 616e 6765 2c20  wnershipChange, 
-000150f0: 7064 2e53 6572 6965 7329 3a0d 0a20 2020  pd.Series):..   
-00015100: 2020 2020 2020 2020 2020 2020 206d 665f               mf_
-00015110: 696e 7374 5f6f 776e 6572 7368 6970 4368  inst_ownershipCh
-00015120: 616e 6765 203d 2030 0d0a 2020 2020 2020  ange = 0..      
-00015130: 2020 2020 2020 726f 756e 644f 6666 203d        roundOff =
-00015140: 2032 0d0a 2020 2020 2020 2020 2020 2020   2..            
-00015150: 6d69 6c6c 696f 6e73 203d 2072 6f75 6e64  millions = round
-00015160: 286d 665f 696e 7374 5f6f 776e 6572 7368  (mf_inst_ownersh
-00015170: 6970 4368 616e 6765 2f31 3030 3030 3030  ipChange/1000000
-00015180: 2c72 6f75 6e64 4f66 6629 0d0a 2020 2020  ,roundOff)..    
-00015190: 2020 2020 2020 2020 7768 696c 6520 666c          while fl
-000151a0: 6f61 7428 6d69 6c6c 696f 6e73 2920 3d3d  oat(millions) ==
-000151b0: 2030 2061 6e64 2072 6f75 6e64 4f66 6620   0 and roundOff 
-000151c0: 3c3d 353a 0d0a 2020 2020 2020 2020 2020  <=5:..          
-000151d0: 2020 2020 2020 726f 756e 644f 6666 202b        roundOff +
-000151e0: 3d31 0d0a 2020 2020 2020 2020 2020 2020  =1..            
-000151f0: 2020 2020 6d69 6c6c 696f 6e73 203d 2072      millions = r
-00015200: 6f75 6e64 286d 665f 696e 7374 5f6f 776e  ound(mf_inst_own
-00015210: 6572 7368 6970 4368 616e 6765 2f31 3030  ershipChange/100
-00015220: 3030 3030 2c72 6f75 6e64 4f66 6629 0d0a  0000,roundOff)..
-00015230: 2020 2020 2020 2020 2020 2020 6368 616e              chan
-00015240: 6765 5f6d 696c 6c69 6f6e 7320 3d20 6622  ge_millions = f"
-00015250: 287b 6d69 6c6c 696f 6e73 7d4d 2922 0d0a  ({millions}M)"..
-00015260: 2020 2020 2020 2020 6578 6365 7074 2045          except E
-00015270: 7863 6570 7469 6f6e 2061 7320 653a 2020  xception as e:  
-00015280: 2320 7072 6167 6d61 3a20 6e6f 2063 6f76  # pragma: no cov
-00015290: 6572 0d0a 2020 2020 2020 2020 2020 2020  er..            
-000152a0: 7365 6c66 2e64 6566 6175 6c74 5f6c 6f67  self.default_log
-000152b0: 6765 722e 6465 6275 6728 652c 2065 7863  ger.debug(e, exc
-000152c0: 5f69 6e66 6f3d 5472 7565 290d 0a20 2020  _info=True)..   
-000152d0: 2020 2020 2020 2020 2070 6173 730d 0a20           pass.. 
-000152e0: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
-000152f0: 2020 2020 2020 2020 2023 4c65 7427 7320           #Let's 
-00015300: 6765 7420 7468 6520 6661 6972 2076 616c  get the fair val
-00015310: 7565 2c20 6569 7468 6572 2073 6176 6564  ue, either saved
-00015320: 206f 7220 6672 6573 6820 6672 6f6d 2073   or fresh from s
-00015330: 6572 7669 6365 0d0a 2020 2020 2020 2020  ervice..        
-00015340: 2020 2020 6661 6972 5661 6c75 6520 3d20      fairValue = 
-00015350: 7365 6c66 2e67 6574 4661 6972 5661 6c75  self.getFairValu
-00015360: 6528 7374 6f63 6b2c 686f 7374 4461 7461  e(stock,hostData
-00015370: 2c66 6f72 6365 3d28 686f 7374 4461 7461  ,force=(hostData
-00015380: 2069 7320 4e6f 6e65 206f 7220 686f 7374   is None or host
-00015390: 4461 7461 2e65 6d70 7479 206f 7220 2246  Data.empty or "F
-000153a0: 6169 7256 616c 7565 2220 6e6f 7420 696e  airValue" not in
-000153b0: 2068 6f73 7444 6174 612e 636f 6c75 6d6e   hostData.column
-000153c0: 7329 2c65 7863 6861 6e67 654e 616d 653d  s),exchangeName=
-000153d0: 6578 6368 616e 6765 4e61 6d65 290d 0a20  exchangeName).. 
-000153e0: 2020 2020 2020 2020 2020 2069 6620 6661             if fa
-000153f0: 6972 5661 6c75 6520 6973 206e 6f74 204e  irValue is not N
-00015400: 6f6e 6520 616e 6420 6661 6972 5661 6c75  one and fairValu
-00015410: 6520 213d 2030 3a0d 0a20 2020 2020 2020  e != 0:..       
-00015420: 2020 2020 2020 2020 206c 7470 203d 2073           ltp = s
-00015430: 6176 6544 6963 745b 224c 5450 225d 0d0a  aveDict["LTP"]..
-00015440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015450: 6661 6972 5661 6c75 6544 6966 6620 3d20  fairValueDiff = 
-00015460: 726f 756e 6428 6661 6972 5661 6c75 6520  round(fairValue 
-00015470: 2d20 6c74 702c 3029 0d0a 2020 2020 2020  - ltp,0)..      
-00015480: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
-00015490: 6374 5b22 4661 6972 5661 6c75 6522 5d20  ct["FairValue"] 
-000154a0: 3d20 7374 7228 6661 6972 5661 6c75 6529  = str(fairValue)
-000154b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000154c0: 2020 7361 7665 4469 6374 5b22 4656 4469    saveDict["FVDi
-000154d0: 6666 225d 203d 2066 6169 7256 616c 7565  ff"] = fairValue
-000154e0: 4469 6666 0d0a 2020 2020 2020 2020 2020  Diff..          
-000154f0: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
-00015500: 5b22 4656 4469 6666 225d 203d 2066 6169  ["FVDiff"] = fai
-00015510: 7256 616c 7565 4469 6666 0d0a 2020 2020  rValueDiff..    
-00015520: 2020 2020 2020 2020 2020 2020 7363 7265              scre
-00015530: 656e 4469 6374 5b22 4661 6972 5661 6c75  enDict["FairValu
-00015540: 6522 5d20 3d20 2863 6f6c 6f72 5465 7874  e"] = (colorText
-00015550: 2e47 5245 454e 2069 6620 6661 6972 5661  .GREEN if fairVa
-00015560: 6c75 6520 3e3d 206c 7470 2065 6c73 6520  lue >= ltp else 
-00015570: 636f 6c6f 7254 6578 742e 4641 494c 2920  colorText.FAIL) 
-00015580: 2b20 7361 7665 4469 6374 5b22 4661 6972  + saveDict["Fair
-00015590: 5661 6c75 6522 5d20 2b20 636f 6c6f 7254  Value"] + colorT
-000155a0: 6578 742e 454e 440d 0a20 2020 2020 2020  ext.END..       
-000155b0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-000155c0: 6e20 6173 2065 3a20 2023 2070 7261 676d  n as e:  # pragm
-000155d0: 613a 206e 6f20 636f 7665 720d 0a20 2020  a: no cover..   
-000155e0: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
-000155f0: 6661 756c 745f 6c6f 6767 6572 2e64 6562  fault_logger.deb
-00015600: 7567 2865 2c20 6578 635f 696e 666f 3d54  ug(e, exc_info=T
-00015610: 7275 6529 0d0a 2020 2020 2020 2020 2020  rue)..          
-00015620: 2020 7061 7373 0d0a 2020 2020 2020 2020    pass..        
-00015630: 6d66 203d 2022 220d 0a20 2020 2020 2020  mf = ""..       
-00015640: 206d 6673 203d 2022 220d 0a20 2020 2020   mfs = ""..     
-00015650: 2020 2069 6620 6d66 5f69 6e73 745f 6f77     if mf_inst_ow
-00015660: 6e65 7273 6869 7043 6861 6e67 6520 3e20  nershipChange > 
-00015670: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-00015680: 6d66 203d 2066 224d 4649 3ae2 96b2 207b  mf = f"MFI:... {
-00015690: 6368 616e 6765 5f6d 696c 6c69 6f6e 737d  change_millions}
-000156a0: 220d 0a20 2020 2020 2020 2020 2020 206d  "..            m
-000156b0: 6673 203d 2063 6f6c 6f72 5465 7874 2e47  fs = colorText.G
-000156c0: 5245 454e 202b 206d 6620 2b20 636f 6c6f  REEN + mf + colo
-000156d0: 7254 6578 742e 454e 440d 0a20 2020 2020  rText.END..     
-000156e0: 2020 2065 6c69 6620 6d66 5f69 6e73 745f     elif mf_inst_
-000156f0: 6f77 6e65 7273 6869 7043 6861 6e67 6520  ownershipChange 
-00015700: 3c20 303a 0d0a 2020 2020 2020 2020 2020  < 0:..          
-00015710: 2020 6d66 203d 2066 224d 4649 3ae2 96bc    mf = f"MFI:...
-00015720: 207b 6368 616e 6765 5f6d 696c 6c69 6f6e   {change_million
-00015730: 737d 220d 0a20 2020 2020 2020 2020 2020  s}"..           
-00015740: 206d 6673 203d 2063 6f6c 6f72 5465 7874   mfs = colorText
-00015750: 2e46 4149 4c20 2b20 6d66 202b 2063 6f6c  .FAIL + mf + col
-00015760: 6f72 5465 7874 2e45 4e44 0d0a 0d0a 2020  orText.END....  
-00015770: 2020 2020 2020 7361 7665 6420 3d20 7365        saved = se
-00015780: 6c66 2e66 696e 6443 7572 7265 6e74 5361  lf.findCurrentSa
-00015790: 7665 6456 616c 7565 2873 6372 6565 6e44  vedValue(screenD
-000157a0: 6963 742c 7361 7665 4469 6374 2c22 5472  ict,saveDict,"Tr
-000157b0: 656e 6422 290d 0a20 2020 2020 2020 2064  end")..        d
-000157c0: 6563 6973 696f 6e5f 7363 7220 3d20 2863  ecision_scr = (c
-000157d0: 6f6c 6f72 5465 7874 2e47 5245 454e 2069  olorText.GREEN i
-000157e0: 6620 6973 5570 7472 656e 6420 656c 7365  f isUptrend else
-000157f0: 2028 636f 6c6f 7254 6578 742e 4641 494c   (colorText.FAIL
-00015800: 2069 6620 6973 446f 776e 7472 656e 6420   if isDowntrend 
-00015810: 656c 7365 2063 6f6c 6f72 5465 7874 2e57  else colorText.W
-00015820: 4152 4e29 2920 2b20 6622 7b64 6563 6973  ARN)) + f"{decis
-00015830: 696f 6e7d 2220 2b20 636f 6c6f 7254 6578  ion}" + colorTex
-00015840: 742e 454e 440d 0a20 2020 2020 2020 2064  t.END..        d
-00015850: 6d61 3530 6465 6369 7369 6f6e 5f73 6372  ma50decision_scr
-00015860: 203d 2028 636f 6c6f 7254 6578 742e 4752   = (colorText.GR
-00015870: 4545 4e20 6966 2069 7335 3044 4d41 5570  EEN if is50DMAUp
-00015880: 7472 656e 6420 656c 7365 2028 636f 6c6f  trend else (colo
-00015890: 7254 6578 742e 4641 494c 2069 6620 6973  rText.FAIL if is
-000158a0: 3530 444d 4144 6f77 6e74 7265 6e64 2065  50DMADowntrend e
-000158b0: 6c73 6520 636f 6c6f 7254 6578 742e 5741  lse colorText.WA
-000158c0: 524e 2929 202b 2066 227b 646d 6135 3064  RN)) + f"{dma50d
-000158d0: 6563 6973 696f 6e7d 2220 2b20 636f 6c6f  ecision}" + colo
-000158e0: 7254 6578 742e 454e 440d 0a20 2020 2020  rText.END..     
-000158f0: 2020 2073 6176 6544 6963 745b 2254 7265     saveDict["Tre
-00015900: 6e64 225d 203d 2066 227b 7361 7665 645b  nd"] = f"{saved[
-00015910: 315d 7d20 7b64 6563 6973 696f 6e7d 207b  1]} {decision} {
-00015920: 646d 6135 3064 6563 6973 696f 6e7d 207b  dma50decision} {
-00015930: 6d66 7d22 0d0a 2020 2020 2020 2020 7363  mf}"..        sc
-00015940: 7265 656e 4469 6374 5b22 5472 656e 6422  reenDict["Trend"
-00015950: 5d20 3d20 6622 7b73 6176 6564 5b30 5d7d  ] = f"{saved[0]}
-00015960: 207b 6465 6369 7369 6f6e 5f73 6372 7d20   {decision_scr} 
-00015970: 7b64 6d61 3530 6465 6369 7369 6f6e 5f73  {dma50decision_s
-00015980: 6372 7d20 7b6d 6673 7d22 0d0a 2020 2020  cr} {mfs}"..    
-00015990: 2020 2020 7361 7665 4469 6374 5b22 4d46      saveDict["MF
-000159a0: 4922 5d20 3d20 6d66 5f69 6e73 745f 6f77  I"] = mf_inst_ow
-000159b0: 6e65 7273 6869 7043 6861 6e67 650d 0a20  nershipChange.. 
-000159c0: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
-000159d0: 745b 224d 4649 225d 203d 206d 665f 696e  t["MFI"] = mf_in
-000159e0: 7374 5f6f 776e 6572 7368 6970 4368 616e  st_ownershipChan
-000159f0: 6765 0d0a 2020 2020 2020 2020 7265 7475  ge..        retu
-00015a00: 726e 2069 7355 7074 7265 6e64 2c20 6d66  rn isUptrend, mf
-00015a10: 5f69 6e73 745f 6f77 6e65 7273 6869 7043  _inst_ownershipC
-00015a20: 6861 6e67 652c 2066 6169 7256 616c 7565  hange, fairValue
-00015a30: 4469 6666 0d0a 2020 2020 0d0a 2020 2020  Diff..    ..    
-00015a40: 2320 5072 6976 6174 6520 6d65 7468 6f64  # Private method
-00015a50: 2074 6f20 6669 6e64 2063 616e 646c 6520   to find candle 
-00015a60: 7479 7065 0d0a 2020 2020 2320 5472 7565  type..    # True
-00015a70: 203d 2042 756c 6c69 7368 2c20 4661 6c73   = Bullish, Fals
-00015a80: 6520 3d20 4265 6172 6973 680d 0a20 2020  e = Bearish..   
-00015a90: 2064 6566 2067 6574 4361 6e64 6c65 5479   def getCandleTy
-00015aa0: 7065 2873 656c 662c 2064 6169 6c79 4461  pe(self, dailyDa
-00015ab0: 7461 293a 0d0a 2020 2020 2020 2020 7265  ta):..        re
-00015ac0: 7475 726e 2062 6f6f 6c28 6461 696c 7944  turn bool(dailyD
-00015ad0: 6174 615b 2243 6c6f 7365 225d 2e69 6c6f  ata["Close"].ilo
-00015ae0: 635b 305d 203e 3d20 6461 696c 7944 6174  c[0] >= dailyDat
-00015af0: 615b 224f 7065 6e22 5d2e 696c 6f63 5b30  a["Open"].iloc[0
-00015b00: 5d29 0d0a 0d0a 2020 2020 6465 6620 6765  ])....    def ge
-00015b10: 7443 616e 646c 6542 6f64 7948 6569 6768  tCandleBodyHeigh
-00015b20: 7428 7365 6c66 2c20 6461 696c 7944 6174  t(self, dailyDat
-00015b30: 6129 3a0d 0a20 2020 2020 2020 2062 6f64  a):..        bod
-00015b40: 7948 6569 6768 7420 3d20 6461 696c 7944  yHeight = dailyD
-00015b50: 6174 615b 2243 6c6f 7365 225d 2e69 6c6f  ata["Close"].ilo
-00015b60: 635b 305d 202d 2064 6169 6c79 4461 7461  c[0] - dailyData
-00015b70: 5b22 4f70 656e 225d 2e69 6c6f 635b 305d  ["Open"].iloc[0]
-00015b80: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00015b90: 2062 6f64 7948 6569 6768 740d 0a0d 0a20   bodyHeight.... 
-00015ba0: 2020 2064 6566 2067 6574 4661 6972 5661     def getFairVa
-00015bb0: 6c75 6528 7365 6c66 2c20 7374 6f63 6b2c  lue(self, stock,
-00015bc0: 2068 6f73 7444 6174 613d 4e6f 6e65 2c20   hostData=None, 
-00015bd0: 666f 7263 653d 4661 6c73 652c 6578 6368  force=False,exch
-00015be0: 616e 6765 4e61 6d65 3d22 494e 4449 4122  angeName="INDIA"
-00015bf0: 293a 0d0a 2020 2020 2020 2020 6966 2068  ):..        if h
-00015c00: 6f73 7444 6174 6120 6973 204e 6f6e 6520  ostData is None 
-00015c10: 6f72 206c 656e 2868 6f73 7444 6174 6129  or len(hostData)
-00015c20: 203c 2031 3a0d 0a20 2020 2020 2020 2020   < 1:..         
-00015c30: 2020 2068 6f73 7444 6174 6120 3d20 7064     hostData = pd
-00015c40: 2e44 6174 6146 7261 6d65 2829 0d0a 2020  .DataFrame()..  
-00015c50: 2020 2020 2020 2320 4c65 7427 7320 6c6f        # Let's lo
-00015c60: 6f6b 2066 6f72 2066 6169 7220 7661 6c75  ok for fair valu
-00015c70: 6573 0d0a 2020 2020 2020 2020 6661 6972  es..        fair
-00015c80: 5661 6c75 6520 3d20 300d 0a20 2020 2020  Value = 0..     
-00015c90: 2020 2069 6620 2246 6169 7256 616c 7565     if "FairValue
-00015ca0: 2220 696e 2068 6f73 7444 6174 612e 636f  " in hostData.co
-00015cb0: 6c75 6d6e 7320 616e 6420 504b 4461 7465  lumns and PKDate
-00015cc0: 5574 696c 6974 6965 732e 6375 7272 656e  Utilities.curren
-00015cd0: 7444 6174 6554 696d 6528 292e 7765 656b  tDateTime().week
-00015ce0: 6461 7928 2920 3c3d 2034 3a0d 0a20 2020  day() <= 4:..   
-00015cf0: 2020 2020 2020 2020 2074 7279 3a0d 0a20           try:.. 
-00015d00: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00015d10: 6169 7256 616c 7565 203d 2068 6f73 7444  airValue = hostD
-00015d20: 6174 612e 6c6f 635b 686f 7374 4461 7461  ata.loc[hostData
-00015d30: 2e69 6e64 6578 5b2d 315d 2c22 4661 6972  .index[-1],"Fair
-00015d40: 5661 6c75 6522 5d0d 0a20 2020 2020 2020  Value"]..       
-00015d50: 2020 2020 2065 7863 6570 7420 284b 6579       except (Key
-00015d60: 4572 726f 722c 496e 6465 7845 7272 6f72  Error,IndexError
-00015d70: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00015d80: 2020 2020 2020 2020 7061 7373 0d0a 2020          pass..  
-00015d90: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00015da0: 2020 2020 2020 2020 2069 6620 504b 4461           if PKDa
-00015db0: 7465 5574 696c 6974 6965 732e 6375 7272  teUtilities.curr
-00015dc0: 656e 7444 6174 6554 696d 6528 292e 7765  entDateTime().we
-00015dd0: 656b 6461 7928 2920 3e3d 2035 206f 7220  ekday() >= 5 or 
-00015de0: 666f 7263 653a 0d0a 2020 2020 2020 2020  force:..        
-00015df0: 2020 2020 2020 2020 7365 6375 7269 7479          security
-00015e00: 203d 204e 6f6e 650d 0a20 2020 2020 2020   = None..       
-00015e10: 2020 2020 2020 2020 2023 2052 6566 7265           # Refre
-00015e20: 7368 2065 6163 6820 7361 7475 7264 6179  sh each saturday
-00015e30: 206f 7220 7375 6e64 6179 206f 7220 7768   or sunday or wh
-00015e40: 656e 206e 6f74 2066 6f75 6e64 2069 6e20  en not found in 
-00015e50: 7361 7665 6420 6461 7461 0d0a 2020 2020  saved data..    
-00015e60: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00015e70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015e80: 2020 2020 2020 7769 7468 2053 7570 7072        with Suppr
-00015e90: 6573 734f 7574 7075 7428 7375 7070 7265  essOutput(suppre
-00015ea0: 7373 5f73 7464 6572 723d 5472 7565 2c20  ss_stderr=True, 
-00015eb0: 7375 7070 7265 7373 5f73 7464 6f75 743d  suppress_stdout=
-00015ec0: 5472 7565 293a 0d0a 2020 2020 2020 2020  True):..        
-00015ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ee0: 7365 6375 7269 7479 203d 2053 746f 636b  security = Stock
-00015ef0: 2873 746f 636b 2c65 7863 6861 6e67 653d  (stock,exchange=
-00015f00: 6578 6368 616e 6765 4e61 6d65 290d 0a20  exchangeName).. 
-00015f10: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00015f20: 7863 6570 7420 5661 6c75 6545 7272 6f72  xcept ValueError
-00015f30: 3a20 2320 7072 6167 6d61 3a20 6e6f 2063  : # pragma: no c
-00015f40: 6f76 6572 0d0a 2020 2020 2020 2020 2020  over..          
-00015f50: 2020 2020 2020 2020 2020 2320 5765 2064            # We d
-00015f60: 6964 206e 6f74 2066 696e 6420 7468 6520  id not find the 
-00015f70: 7374 6f63 6b3f 2049 7427 7320 6f6b 6179  stock? It's okay
-00015f80: 2e20 4d6f 7665 206f 6e20 746f 2074 6865  . Move on to the
-00015f90: 206e 6578 7420 6f6e 652e 0d0a 2020 2020   next one...    
-00015fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015fb0: 7061 7373 0d0a 2020 2020 2020 2020 2020  pass..          
-00015fc0: 2020 2020 2020 6966 2073 6563 7572 6974        if securit
-00015fd0: 7920 6973 206e 6f74 204e 6f6e 653a 0d0a  y is not None:..
-00015fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ff0: 2020 2020 7769 7468 2053 7570 7072 6573      with Suppres
-00016000: 734f 7574 7075 7428 7375 7070 7265 7373  sOutput(suppress
-00016010: 5f73 7464 6572 723d 5472 7565 2c20 7375  _stderr=True, su
-00016020: 7070 7265 7373 5f73 7464 6f75 743d 5472  ppress_stdout=Tr
-00016030: 7565 293a 0d0a 2020 2020 2020 2020 2020  ue):..          
-00016040: 2020 2020 2020 2020 2020 2020 2020 6676                fv
-00016050: 203d 2073 6563 7572 6974 792e 6661 6972   = security.fair
-00016060: 5661 6c75 6528 290d 0a20 2020 2020 2020  Value()..       
-00016070: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00016080: 6676 2069 7320 6e6f 7420 4e6f 6e65 3a0d  fv is not None:.
-00016090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000160a0: 2020 2020 2020 2020 2074 7279 3a0d 0a20           try:.. 
-000160b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000160c0: 2020 2020 2020 2020 2020 2066 7652 6573             fvRes
-000160d0: 706f 6e73 6556 616c 7565 203d 2066 765b  ponseValue = fv[
-000160e0: 226c 6174 6573 7446 6169 7256 616c 7565  "latestFairValue
-000160f0: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
-00016100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016110: 6966 2066 7652 6573 706f 6e73 6556 616c  if fvResponseVal
-00016120: 7565 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ue is not None:.
-00016130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016150: 2066 6169 7256 616c 7565 203d 2066 6c6f   fairValue = flo
-00016160: 6174 2866 7652 6573 706f 6e73 6556 616c  at(fvResponseVal
-00016170: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
-00016180: 2020 2020 2020 2020 2020 2020 2065 7863               exc
-00016190: 6570 743a 2023 2070 7261 676d 613a 206e  ept: # pragma: n
-000161a0: 6f20 636f 7665 720d 0a20 2020 2020 2020  o cover..       
-000161b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000161c0: 2020 2020 2070 6173 730d 0a20 2020 2020       pass..     
-000161d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000161e0: 2020 2020 2020 2023 2073 656c 662e 6465         # self.de
-000161f0: 6661 756c 745f 6c6f 6767 6572 2e64 6562  fault_logger.deb
-00016200: 7567 2866 227b 657d 5c6e 5265 7370 6f6e  ug(f"{e}\nRespon
-00016210: 7365 3a66 763a 5c6e 7b66 767d 222c 2065  se:fv:\n{fv}", e
-00016220: 7863 5f69 6e66 6f3d 5472 7565 290d 0a20  xc_info=True).. 
-00016230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016240: 2020 2066 6169 7256 616c 7565 203d 2072     fairValue = r
-00016250: 6f75 6e64 2866 6c6f 6174 2866 6169 7256  ound(float(fairV
-00016260: 616c 7565 292c 3129 0d0a 2020 2020 2020  alue),1)..      
-00016270: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-00016280: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
-00016290: 2020 2020 2020 2020 2020 2020 686f 7374              host
-000162a0: 4461 7461 2e6c 6f63 5b68 6f73 7444 6174  Data.loc[hostDat
-000162b0: 612e 696e 6465 785b 2d31 5d2c 2246 6169  a.index[-1],"Fai
-000162c0: 7256 616c 7565 225d 203d 2066 6169 7256  rValue"] = fairV
-000162d0: 616c 7565 0d0a 2020 2020 2020 2020 2020  alue..          
-000162e0: 2020 2020 2020 2020 2020 6578 6365 7074            except
-000162f0: 2028 4b65 7945 7272 6f72 2c49 6e64 6578   (KeyError,Index
-00016300: 4572 726f 7229 3a0d 0a20 2020 2020 2020  Error):..       
-00016310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016320: 2070 6173 730d 0a20 2020 2020 2020 2072   pass..        r
-00016330: 6574 7572 6e20 6661 6972 5661 6c75 650d  eturn fairValue.
-00016340: 0a0d 0a20 2020 2064 6566 2067 6574 4d75  ...    def getMu
-00016350: 7475 616c 4675 6e64 5374 6174 7573 2873  tualFundStatus(s
-00016360: 656c 662c 2073 746f 636b 2c6f 6e6c 794d  elf, stock,onlyM
-00016370: 463d 4661 6c73 652c 2068 6f73 7444 6174  F=False, hostDat
-00016380: 613d 4e6f 6e65 2c20 666f 7263 653d 4661  a=None, force=Fa
-00016390: 6c73 652c 6578 6368 616e 6765 4e61 6d65  lse,exchangeName
-000163a0: 3d22 494e 4449 4122 293a 0d0a 2020 2020  ="INDIA"):..    
-000163b0: 2020 2020 6966 2068 6f73 7444 6174 6120      if hostData 
-000163c0: 6973 204e 6f6e 6520 6f72 206c 656e 2868  is None or len(h
-000163d0: 6f73 7444 6174 6129 203c 2031 3a0d 0a20  ostData) < 1:.. 
-000163e0: 2020 2020 2020 2020 2020 2068 6f73 7444             hostD
-000163f0: 6174 6120 3d20 7064 2e44 6174 6146 7261  ata = pd.DataFra
-00016400: 6d65 2829 0d0a 2020 2020 2020 2020 0d0a  me()..        ..
-00016410: 2020 2020 2020 2020 6e65 7443 6861 6e67          netChang
-00016420: 654d 4620 3d20 300d 0a20 2020 2020 2020  eMF = 0..       
-00016430: 206e 6574 4368 616e 6765 496e 7374 203d   netChangeInst =
-00016440: 2030 0d0a 2020 2020 2020 2020 6c61 7465   0..        late
-00016450: 7374 5f6d 6664 6174 6520 3d20 4e6f 6e65  st_mfdate = None
-00016460: 0d0a 2020 2020 2020 2020 6c61 7465 7374  ..        latest
-00016470: 5f69 6e73 7464 6174 6520 3d20 4e6f 6e65  _instdate = None
-00016480: 0d0a 2020 2020 2020 2020 6e65 6564 7346  ..        needsF
-00016490: 7265 7368 5570 6461 7465 203d 2054 7275  reshUpdate = Tru
-000164a0: 650d 0a20 2020 2020 2020 206c 6173 7444  e..        lastD
-000164b0: 6179 4c61 7374 4d6f 6e74 6820 3d20 504b  ayLastMonth = PK
-000164c0: 4461 7465 5574 696c 6974 6965 732e 6c61  DateUtilities.la
-000164d0: 7374 5f64 6179 5f6f 665f 7072 6576 696f  st_day_of_previo
-000164e0: 7573 5f6d 6f6e 7468 2850 4b44 6174 6555  us_month(PKDateU
-000164f0: 7469 6c69 7469 6573 2e63 7572 7265 6e74  tilities.current
-00016500: 4461 7465 5469 6d65 2829 290d 0a20 2020  DateTime())..   
-00016510: 2020 2020 2069 6620 686f 7374 4461 7461       if hostData
-00016520: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-00016530: 206c 656e 2868 6f73 7444 6174 6129 203e   len(hostData) >
-00016540: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
-00016550: 2069 6620 224d 4622 2069 6e20 686f 7374   if "MF" in host
-00016560: 4461 7461 2e63 6f6c 756d 6e73 206f 7220  Data.columns or 
-00016570: 2246 4949 2220 696e 2068 6f73 7444 6174  "FII" in hostDat
-00016580: 612e 636f 6c75 6d6e 733a 0d0a 2020 2020  a.columns:..    
-00016590: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-000165a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000165b0: 2020 2020 2020 6e65 7443 6861 6e67 654d        netChangeM
-000165c0: 4620 3d20 686f 7374 4461 7461 2e6c 6f63  F = hostData.loc
-000165d0: 5b68 6f73 7444 6174 612e 696e 6465 785b  [hostData.index[
-000165e0: 2d31 5d2c 224d 4622 5d0d 0a20 2020 2020  -1],"MF"]..     
-000165f0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-00016600: 7420 284b 6579 4572 726f 722c 496e 6465  t (KeyError,Inde
-00016610: 7845 7272 6f72 293a 0d0a 2020 2020 2020  xError):..      
-00016620: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00016630: 7373 0d0a 2020 2020 2020 2020 2020 2020  ss..            
-00016640: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-00016650: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-00016660: 7443 6861 6e67 6549 6e73 7420 3d20 686f  tChangeInst = ho
-00016670: 7374 4461 7461 2e6c 6f63 5b68 6f73 7444  stData.loc[hostD
-00016680: 6174 612e 696e 6465 785b 2d31 5d2c 2246  ata.index[-1],"F
-00016690: 4949 225d 0d0a 2020 2020 2020 2020 2020  II"]..          
-000166a0: 2020 2020 2020 6578 6365 7074 2028 4b65        except (Ke
-000166b0: 7945 7272 6f72 2c49 6e64 6578 4572 726f  yError,IndexErro
-000166c0: 7229 3a0d 0a20 2020 2020 2020 2020 2020  r):..           
-000166d0: 2020 2020 2020 2020 2070 6173 730d 0a20           pass.. 
-000166e0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000166f0: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
-00016700: 2020 2020 2020 2020 206c 6174 6573 745f           latest_
-00016710: 6d66 6461 7465 203d 2068 6f73 7444 6174  mfdate = hostDat
-00016720: 612e 6c6f 635b 686f 7374 4461 7461 2e69  a.loc[hostData.i
-00016730: 6e64 6578 5b2d 315d 2c22 4d46 5f44 6174  ndex[-1],"MF_Dat
-00016740: 6522 5d0d 0a20 2020 2020 2020 2020 2020  e"]..           
-00016750: 2020 2020 2065 7863 6570 7420 284b 6579       except (Key
-00016760: 4572 726f 722c 496e 6465 7845 7272 6f72  Error,IndexError
-00016770: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00016780: 2020 2020 2020 2020 7061 7373 0d0a 2020          pass..  
-00016790: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-000167a0: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
-000167b0: 2020 2020 2020 2020 6c61 7465 7374 5f69          latest_i
-000167c0: 6e73 7464 6174 6520 3d20 686f 7374 4461  nstdate = hostDa
-000167d0: 7461 2e6c 6f63 5b68 6f73 7444 6174 612e  ta.loc[hostData.
-000167e0: 696e 6465 785b 2d31 5d2c 2246 4949 5f44  index[-1],"FII_D
-000167f0: 6174 6522 5d0d 0a20 2020 2020 2020 2020  ate"]..         
-00016800: 2020 2020 2020 2065 7863 6570 7420 284b         except (K
-00016810: 6579 4572 726f 722c 496e 6465 7845 7272  eyError,IndexErr
-00016820: 6f72 293a 0d0a 2020 2020 2020 2020 2020  or):..          
-00016830: 2020 2020 2020 2020 2020 7061 7373 0d0a            pass..
+000144c0: 4e61 6d65 3d22 494e 4449 4122 2c72 6566  Name="INDIA",ref
+000144d0: 7265 7368 4d46 416e 6446 563d 5472 7565  reshMFAndFV=True
+000144e0: 293a 0d0a 2020 2020 2020 2020 2320 7368  ):..        # sh
+000144f0: 6f75 6c64 5072 6f63 6565 6420 3d20 5472  ouldProceed = Tr
+00014500: 7565 0d0a 2020 2020 2020 2020 6973 5570  ue..        isUp
+00014510: 7472 656e 6420 3d20 4661 6c73 650d 0a20  trend = False.. 
+00014520: 2020 2020 2020 2069 7344 6f77 6e74 7265         isDowntre
+00014530: 6e64 203d 2046 616c 7365 0d0a 2020 2020  nd = False..    
+00014540: 2020 2020 6973 3530 444d 4155 7074 7265      is50DMAUptre
+00014550: 6e64 203d 2046 616c 7365 0d0a 2020 2020  nd = False..    
+00014560: 2020 2020 6973 3530 444d 4144 6f77 6e74      is50DMADownt
+00014570: 7265 6e64 203d 2046 616c 7365 0d0a 2020  rend = False..  
+00014580: 2020 2020 2020 6465 6369 7369 6f6e 203d        decision =
+00014590: 2022 220d 0a20 2020 2020 2020 2064 6d61   ""..        dma
+000145a0: 3530 6465 6369 7369 6f6e 203d 2022 220d  50decision = "".
+000145b0: 0a20 2020 2020 2020 2066 6169 7256 616c  .        fairVal
+000145c0: 7565 203d 2030 0d0a 2020 2020 2020 2020  ue = 0..        
+000145d0: 6661 6972 5661 6c75 6544 6966 6620 3d20  fairValueDiff = 
+000145e0: 300d 0a20 2020 2020 2020 2023 2069 6620  0..        # if 
+000145f0: 6466 2069 7320 4e6f 6e65 206f 7220 6c65  df is None or le
+00014600: 6e28 6466 2920 3c20 3232 3020 6f72 2074  n(df) < 220 or t
+00014610: 6573 7469 6e67 3a0d 0a20 2020 2020 2020  esting:..       
+00014620: 2023 2020 2020 2073 686f 756c 6450 726f   #     shouldPro
+00014630: 6365 6564 203d 2046 616c 7365 0d0a 2020  ceed = False..  
+00014640: 2020 2020 2020 6966 2064 6620 6973 206e        if df is n
+00014650: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+00014660: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
+00014670: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00014680: 203d 2064 662e 636f 7079 2829 0d0a 2020   = df.copy()..  
+00014690: 2020 2020 2020 2020 2020 2020 2020 6461                da
+000146a0: 7461 203d 2064 6174 615b 3a3a 2d31 5d0d  ta = data[::-1].
+000146b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000146c0: 2074 6f64 6179 5f73 6d61 203d 2070 6b74   today_sma = pkt
+000146d0: 616c 6962 2e53 4d41 2864 6174 615b 2243  alib.SMA(data["C
+000146e0: 6c6f 7365 225d 2c20 7469 6d65 7065 7269  lose"], timeperi
+000146f0: 6f64 3d35 3029 0d0a 2020 2020 2020 2020  od=50)..        
+00014700: 2020 2020 2020 2020 736d 615f 6d69 6e75          sma_minu
+00014710: 7339 203d 2070 6b74 616c 6962 2e53 4d41  s9 = pktalib.SMA
+00014720: 2864 6174 612e 6865 6164 286c 656e 2864  (data.head(len(d
+00014730: 6174 6129 2d39 295b 2243 6c6f 7365 225d  ata)-9)["Close"]
+00014740: 2c20 7469 6d65 7065 7269 6f64 3d35 3029  , timeperiod=50)
+00014750: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014760: 2020 736d 615f 6d69 6e75 7331 3420 3d20    sma_minus14 = 
+00014770: 706b 7461 6c69 622e 534d 4128 6461 7461  pktalib.SMA(data
+00014780: 2e68 6561 6428 6c65 6e28 6461 7461 292d  .head(len(data)-
+00014790: 3134 295b 2243 6c6f 7365 225d 2c20 7469  14)["Close"], ti
+000147a0: 6d65 7065 7269 6f64 3d35 3029 0d0a 2020  meperiod=50)..  
+000147b0: 2020 2020 2020 2020 2020 2020 2020 736d                sm
+000147c0: 615f 6d69 6e75 7332 3020 3d20 706b 7461  a_minus20 = pkta
+000147d0: 6c69 622e 534d 4128 6461 7461 2e68 6561  lib.SMA(data.hea
+000147e0: 6428 6c65 6e28 6461 7461 292d 3230 295b  d(len(data)-20)[
+000147f0: 2243 6c6f 7365 225d 2c20 7469 6d65 7065  "Close"], timepe
+00014800: 7269 6f64 3d35 3029 0d0a 2020 2020 2020  riod=50)..      
+00014810: 2020 2020 2020 2020 2020 746f 6461 795f            today_
+00014820: 6c6d 6120 3d20 706b 7461 6c69 622e 534d  lma = pktalib.SM
+00014830: 4128 6461 7461 5b22 436c 6f73 6522 5d2c  A(data["Close"],
+00014840: 2074 696d 6570 6572 696f 643d 3230 3029   timeperiod=200)
+00014850: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014860: 2020 6c6d 615f 6d69 6e75 7332 3020 3d20    lma_minus20 = 
+00014870: 706b 7461 6c69 622e 534d 4128 6461 7461  pktalib.SMA(data
+00014880: 2e68 6561 6428 6c65 6e28 6461 7461 292d  .head(len(data)-
+00014890: 3230 295b 2243 6c6f 7365 225d 2c20 7469  20)["Close"], ti
+000148a0: 6d65 7065 7269 6f64 3d32 3030 290d 0a20  meperiod=200).. 
+000148b0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+000148c0: 6d61 5f6d 696e 7573 3830 203d 2070 6b74  ma_minus80 = pkt
+000148d0: 616c 6962 2e53 4d41 2864 6174 612e 6865  alib.SMA(data.he
+000148e0: 6164 286c 656e 2864 6174 6129 2d38 3029  ad(len(data)-80)
+000148f0: 5b22 436c 6f73 6522 5d2c 2074 696d 6570  ["Close"], timep
+00014900: 6572 696f 643d 3230 3029 0d0a 2020 2020  eriod=200)..    
+00014910: 2020 2020 2020 2020 2020 2020 6c6d 615f              lma_
+00014920: 6d69 6e75 7331 3030 203d 2070 6b74 616c  minus100 = pktal
+00014930: 6962 2e53 4d41 2864 6174 612e 6865 6164  ib.SMA(data.head
+00014940: 286c 656e 2864 6174 6129 2d31 3030 295b  (len(data)-100)[
+00014950: 2243 6c6f 7365 225d 2c20 7469 6d65 7065  "Close"], timepe
+00014960: 7269 6f64 3d32 3030 290d 0a20 2020 2020  riod=200)..     
+00014970: 2020 2020 2020 2020 2020 2074 6f64 6179             today
+00014980: 5f6c 6d61 203d 2074 6f64 6179 5f6c 6d61  _lma = today_lma
+00014990: 2e69 6c6f 635b 6c65 6e28 746f 6461 795f  .iloc[len(today_
+000149a0: 6c6d 6129 2d31 5d20 6966 2074 6f64 6179  lma)-1] if today
+000149b0: 5f6c 6d61 2069 7320 6e6f 7420 4e6f 6e65  _lma is not None
+000149c0: 2065 6c73 6520 300d 0a20 2020 2020 2020   else 0..       
+000149d0: 2020 2020 2020 2020 206c 6d61 5f6d 696e           lma_min
+000149e0: 7573 3230 203d 206c 6d61 5f6d 696e 7573  us20 = lma_minus
+000149f0: 3230 2e69 6c6f 635b 6c65 6e28 6c6d 615f  20.iloc[len(lma_
+00014a00: 6d69 6e75 7332 3029 2d31 5d20 6966 206c  minus20)-1] if l
+00014a10: 6d61 5f6d 696e 7573 3230 2069 7320 6e6f  ma_minus20 is no
+00014a20: 7420 4e6f 6e65 2065 6c73 6520 300d 0a20  t None else 0.. 
+00014a30: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00014a40: 6d61 5f6d 696e 7573 3830 203d 206c 6d61  ma_minus80 = lma
+00014a50: 5f6d 696e 7573 3830 2e69 6c6f 635b 6c65  _minus80.iloc[le
+00014a60: 6e28 6c6d 615f 6d69 6e75 7338 3029 2d31  n(lma_minus80)-1
+00014a70: 5d20 6966 206c 6d61 5f6d 696e 7573 3830  ] if lma_minus80
+00014a80: 2069 7320 6e6f 7420 4e6f 6e65 2065 6c73   is not None els
+00014a90: 6520 300d 0a20 2020 2020 2020 2020 2020  e 0..           
+00014aa0: 2020 2020 206c 6d61 5f6d 696e 7573 3130       lma_minus10
+00014ab0: 3020 3d20 6c6d 615f 6d69 6e75 7331 3030  0 = lma_minus100
+00014ac0: 2e69 6c6f 635b 6c65 6e28 6c6d 615f 6d69  .iloc[len(lma_mi
+00014ad0: 6e75 7331 3030 292d 315d 2069 6620 6c6d  nus100)-1] if lm
+00014ae0: 615f 6d69 6e75 7331 3030 2069 7320 6e6f  a_minus100 is no
+00014af0: 7420 4e6f 6e65 2065 6c73 6520 300d 0a20  t None else 0.. 
+00014b00: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00014b10: 6f64 6179 5f73 6d61 203d 2074 6f64 6179  oday_sma = today
+00014b20: 5f73 6d61 2e69 6c6f 635b 6c65 6e28 746f  _sma.iloc[len(to
+00014b30: 6461 795f 736d 6129 2d31 5d20 6966 2074  day_sma)-1] if t
+00014b40: 6f64 6179 5f73 6d61 2069 7320 6e6f 7420  oday_sma is not 
+00014b50: 4e6f 6e65 2065 6c73 6520 300d 0a20 2020  None else 0..   
+00014b60: 2020 2020 2020 2020 2020 2020 2073 6d61               sma
+00014b70: 5f6d 696e 7573 3920 3d20 736d 615f 6d69  _minus9 = sma_mi
+00014b80: 6e75 7339 2e69 6c6f 635b 6c65 6e28 736d  nus9.iloc[len(sm
+00014b90: 615f 6d69 6e75 7339 292d 315d 2069 6620  a_minus9)-1] if 
+00014ba0: 736d 615f 6d69 6e75 7339 2069 7320 6e6f  sma_minus9 is no
+00014bb0: 7420 4e6f 6e65 2065 6c73 6520 300d 0a20  t None else 0.. 
+00014bc0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00014bd0: 6d61 5f6d 696e 7573 3134 203d 2073 6d61  ma_minus14 = sma
+00014be0: 5f6d 696e 7573 3134 2e69 6c6f 635b 6c65  _minus14.iloc[le
+00014bf0: 6e28 736d 615f 6d69 6e75 7331 3429 2d31  n(sma_minus14)-1
+00014c00: 5d20 6966 2073 6d61 5f6d 696e 7573 3134  ] if sma_minus14
+00014c10: 2069 7320 6e6f 7420 4e6f 6e65 2065 6c73   is not None els
+00014c20: 6520 300d 0a20 2020 2020 2020 2020 2020  e 0..           
+00014c30: 2020 2020 2073 6d61 5f6d 696e 7573 3230       sma_minus20
+00014c40: 203d 2073 6d61 5f6d 696e 7573 3230 2e69   = sma_minus20.i
+00014c50: 6c6f 635b 6c65 6e28 736d 615f 6d69 6e75  loc[len(sma_minu
+00014c60: 7332 3029 2d31 5d20 6966 2073 6d61 5f6d  s20)-1] if sma_m
+00014c70: 696e 7573 3230 2069 7320 6e6f 7420 4e6f  inus20 is not No
+00014c80: 6e65 2065 6c73 6520 300d 0a20 2020 2020  ne else 0..     
+00014c90: 2020 2020 2020 2020 2020 2069 7355 7074             isUpt
+00014ca0: 7265 6e64 203d 2028 746f 6461 795f 6c6d  rend = (today_lm
+00014cb0: 6120 3e20 6c6d 615f 6d69 6e75 7332 3029  a > lma_minus20)
+00014cc0: 206f 7220 2874 6f64 6179 5f6c 6d61 203e   or (today_lma >
+00014cd0: 206c 6d61 5f6d 696e 7573 3830 2920 6f72   lma_minus80) or
+00014ce0: 2028 746f 6461 795f 6c6d 6120 3e20 6c6d   (today_lma > lm
+00014cf0: 615f 6d69 6e75 7331 3030 290d 0a20 2020  a_minus100)..   
+00014d00: 2020 2020 2020 2020 2020 2020 2069 7344               isD
+00014d10: 6f77 6e74 7265 6e64 203d 2028 746f 6461  owntrend = (toda
+00014d20: 795f 6c6d 6120 3c20 6c6d 615f 6d69 6e75  y_lma < lma_minu
+00014d30: 7332 3029 2061 6e64 2028 746f 6461 795f  s20) and (today_
+00014d40: 6c6d 6120 3c20 6c6d 615f 6d69 6e75 7338  lma < lma_minus8
+00014d50: 3029 2061 6e64 2028 746f 6461 795f 6c6d  0) and (today_lm
+00014d60: 6120 3c20 6c6d 615f 6d69 6e75 7331 3030  a < lma_minus100
+00014d70: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00014d80: 2020 2069 7335 3044 4d41 5570 7472 656e     is50DMAUptren
+00014d90: 6420 3d20 2874 6f64 6179 5f73 6d61 203e  d = (today_sma >
+00014da0: 2073 6d61 5f6d 696e 7573 3929 206f 7220   sma_minus9) or 
+00014db0: 2874 6f64 6179 5f73 6d61 203e 2073 6d61  (today_sma > sma
+00014dc0: 5f6d 696e 7573 3134 2920 6f72 2028 746f  _minus14) or (to
+00014dd0: 6461 795f 736d 6120 3e20 736d 615f 6d69  day_sma > sma_mi
+00014de0: 6e75 7332 3029 0d0a 2020 2020 2020 2020  nus20)..        
+00014df0: 2020 2020 2020 2020 6973 3530 444d 4144          is50DMAD
+00014e00: 6f77 6e74 7265 6e64 203d 2028 746f 6461  owntrend = (toda
+00014e10: 795f 736d 6120 3c20 736d 615f 6d69 6e75  y_sma < sma_minu
+00014e20: 7339 2920 616e 6420 2874 6f64 6179 5f73  s9) and (today_s
+00014e30: 6d61 203c 2073 6d61 5f6d 696e 7573 3134  ma < sma_minus14
+00014e40: 2920 616e 6420 2874 6f64 6179 5f73 6d61  ) and (today_sma
+00014e50: 203c 2073 6d61 5f6d 696e 7573 3230 290d   < sma_minus20).
+00014e60: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+00014e70: 6570 7420 4578 6365 7074 696f 6e3a 2020  ept Exception:  
+00014e80: 2320 7072 6167 6d61 3a20 6e6f 2063 6f76  # pragma: no cov
+00014e90: 6572 0d0a 2020 2020 2020 2020 2020 2020  er..            
+00014ea0: 2020 2020 2320 7365 6c66 2e64 6566 6175      # self.defau
+00014eb0: 6c74 5f6c 6f67 6765 722e 6465 6275 6728  lt_logger.debug(
+00014ec0: 652c 2065 7863 5f69 6e66 6f3d 5472 7565  e, exc_info=True
+00014ed0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00014ee0: 2020 2070 6173 730d 0a20 2020 2020 2020     pass..       
+00014ef0: 2064 6563 6973 696f 6e20 3d20 2754 3ae2   decision = 'T:.
+00014f00: 96b2 2720 6966 2069 7355 7074 7265 6e64  ..' if isUptrend
+00014f10: 2065 6c73 6520 2827 543a e296 bc27 2069   else ('T:...' i
+00014f20: 6620 6973 446f 776e 7472 656e 6420 656c  f isDowntrend el
+00014f30: 7365 2027 2729 0d0a 2020 2020 2020 2020  se '')..        
+00014f40: 646d 6135 3064 6563 6973 696f 6e20 3d20  dma50decision = 
+00014f50: 2774 3ae2 96b2 2720 6966 2069 7335 3044  't:...' if is50D
+00014f60: 4d41 5570 7472 656e 6420 656c 7365 2028  MAUptrend else (
+00014f70: 2774 3ae2 96bc 2720 6966 2069 7335 3044  't:...' if is50D
+00014f80: 4d41 446f 776e 7472 656e 6420 656c 7365  MADowntrend else
+00014f90: 2027 2729 0d0a 2020 2020 2020 2020 6d66   '')..        mf
+00014fa0: 5f69 6e73 745f 6f77 6e65 7273 6869 7043  _inst_ownershipC
+00014fb0: 6861 6e67 6520 3d20 300d 0a20 2020 2020  hange = 0..     
+00014fc0: 2020 2063 6861 6e67 655f 6d69 6c6c 696f     change_millio
+00014fd0: 6e73 203d 2222 0d0a 2020 2020 2020 2020  ns =""..        
+00014fe0: 6d66 203d 2022 220d 0a20 2020 2020 2020  mf = ""..       
+00014ff0: 206d 6673 203d 2022 220d 0a20 2020 2020   mfs = ""..     
+00015000: 2020 2069 6620 7265 6672 6573 684d 4641     if refreshMFA
+00015010: 6e64 4656 3a0d 0a20 2020 2020 2020 2020  ndFV:..         
+00015020: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
+00015030: 2020 2020 2020 2020 206d 665f 696e 7374           mf_inst
+00015040: 5f6f 776e 6572 7368 6970 4368 616e 6765  _ownershipChange
+00015050: 203d 2073 656c 662e 6765 744d 7574 7561   = self.getMutua
+00015060: 6c46 756e 6453 7461 7475 7328 7374 6f63  lFundStatus(stoc
+00015070: 6b2c 6f6e 6c79 4d46 3d6f 6e6c 794d 462c  k,onlyMF=onlyMF,
+00015080: 686f 7374 4461 7461 3d68 6f73 7444 6174  hostData=hostDat
+00015090: 612c 666f 7263 653d 2868 6f73 7444 6174  a,force=(hostDat
+000150a0: 6120 6973 204e 6f6e 6520 6f72 2068 6f73  a is None or hos
+000150b0: 7444 6174 612e 656d 7074 7920 6f72 206e  tData.empty or n
+000150c0: 6f74 2028 224d 4622 2069 6e20 686f 7374  ot ("MF" in host
+000150d0: 4461 7461 2e63 6f6c 756d 6e73 206f 7220  Data.columns or 
+000150e0: 2246 4949 2220 696e 2068 6f73 7444 6174  "FII" in hostDat
+000150f0: 612e 636f 6c75 6d6e 7329 292c 6578 6368  a.columns)),exch
+00015100: 616e 6765 4e61 6d65 3d65 7863 6861 6e67  angeName=exchang
+00015110: 654e 616d 6529 0d0a 2020 2020 2020 2020  eName)..        
+00015120: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00015130: 7461 6e63 6528 6d66 5f69 6e73 745f 6f77  tance(mf_inst_ow
+00015140: 6e65 7273 6869 7043 6861 6e67 652c 2070  nershipChange, p
+00015150: 642e 5365 7269 6573 293a 0d0a 2020 2020  d.Series):..    
+00015160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015170: 6d66 5f69 6e73 745f 6f77 6e65 7273 6869  mf_inst_ownershi
+00015180: 7043 6861 6e67 6520 3d20 300d 0a20 2020  pChange = 0..   
+00015190: 2020 2020 2020 2020 2020 2020 2072 6f75               rou
+000151a0: 6e64 4f66 6620 3d20 320d 0a20 2020 2020  ndOff = 2..     
+000151b0: 2020 2020 2020 2020 2020 206d 696c 6c69             milli
+000151c0: 6f6e 7320 3d20 726f 756e 6428 6d66 5f69  ons = round(mf_i
+000151d0: 6e73 745f 6f77 6e65 7273 6869 7043 6861  nst_ownershipCha
+000151e0: 6e67 652f 3130 3030 3030 302c 726f 756e  nge/1000000,roun
+000151f0: 644f 6666 290d 0a20 2020 2020 2020 2020  dOff)..         
+00015200: 2020 2020 2020 2077 6869 6c65 2066 6c6f         while flo
+00015210: 6174 286d 696c 6c69 6f6e 7329 203d 3d20  at(millions) == 
+00015220: 3020 616e 6420 726f 756e 644f 6666 203c  0 and roundOff <
+00015230: 3d35 3a0d 0a20 2020 2020 2020 2020 2020  =5:..           
+00015240: 2020 2020 2020 2020 2072 6f75 6e64 4f66           roundOf
+00015250: 6620 2b3d 310d 0a20 2020 2020 2020 2020  f +=1..         
+00015260: 2020 2020 2020 2020 2020 206d 696c 6c69             milli
+00015270: 6f6e 7320 3d20 726f 756e 6428 6d66 5f69  ons = round(mf_i
+00015280: 6e73 745f 6f77 6e65 7273 6869 7043 6861  nst_ownershipCha
+00015290: 6e67 652f 3130 3030 3030 302c 726f 756e  nge/1000000,roun
+000152a0: 644f 6666 290d 0a20 2020 2020 2020 2020  dOff)..         
+000152b0: 2020 2020 2020 2063 6861 6e67 655f 6d69         change_mi
+000152c0: 6c6c 696f 6e73 203d 2066 2228 7b6d 696c  llions = f"({mil
+000152d0: 6c69 6f6e 737d 4d29 220d 0a20 2020 2020  lions}M)"..     
+000152e0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+000152f0: 6365 7074 696f 6e20 6173 2065 3a20 2023  ception as e:  #
+00015300: 2070 7261 676d 613a 206e 6f20 636f 7665   pragma: no cove
+00015310: 720d 0a20 2020 2020 2020 2020 2020 2020  r..             
+00015320: 2020 2073 656c 662e 6465 6661 756c 745f     self.default_
+00015330: 6c6f 6767 6572 2e64 6562 7567 2865 2c20  logger.debug(e, 
+00015340: 6578 635f 696e 666f 3d54 7275 6529 0d0a  exc_info=True)..
+00015350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015360: 7061 7373 0d0a 2020 2020 2020 2020 2020  pass..          
+00015370: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
+00015380: 2020 2020 2020 2020 234c 6574 2773 2067          #Let's g
+00015390: 6574 2074 6865 2066 6169 7220 7661 6c75  et the fair valu
+000153a0: 652c 2065 6974 6865 7220 7361 7665 6420  e, either saved 
+000153b0: 6f72 2066 7265 7368 2066 726f 6d20 7365  or fresh from se
+000153c0: 7276 6963 650d 0a20 2020 2020 2020 2020  rvice..         
+000153d0: 2020 2020 2020 2066 6169 7256 616c 7565         fairValue
+000153e0: 203d 2073 656c 662e 6765 7446 6169 7256   = self.getFairV
+000153f0: 616c 7565 2873 746f 636b 2c68 6f73 7444  alue(stock,hostD
+00015400: 6174 612c 666f 7263 653d 2868 6f73 7444  ata,force=(hostD
+00015410: 6174 6120 6973 204e 6f6e 6520 6f72 2068  ata is None or h
+00015420: 6f73 7444 6174 612e 656d 7074 7920 6f72  ostData.empty or
+00015430: 2022 4661 6972 5661 6c75 6522 206e 6f74   "FairValue" not
+00015440: 2069 6e20 686f 7374 4461 7461 2e63 6f6c   in hostData.col
+00015450: 756d 6e73 292c 6578 6368 616e 6765 4e61  umns),exchangeNa
+00015460: 6d65 3d65 7863 6861 6e67 654e 616d 6529  me=exchangeName)
+00015470: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015480: 2020 6966 2066 6169 7256 616c 7565 2069    if fairValue i
+00015490: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2066  s not None and f
+000154a0: 6169 7256 616c 7565 2021 3d20 303a 0d0a  airValue != 0:..
+000154b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000154c0: 2020 2020 6c74 7020 3d20 7361 7665 4469      ltp = saveDi
+000154d0: 6374 5b22 4c54 5022 5d0d 0a20 2020 2020  ct["LTP"]..     
+000154e0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000154f0: 6169 7256 616c 7565 4469 6666 203d 2072  airValueDiff = r
+00015500: 6f75 6e64 2866 6169 7256 616c 7565 202d  ound(fairValue -
+00015510: 206c 7470 2c30 290d 0a20 2020 2020 2020   ltp,0)..       
+00015520: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+00015530: 6544 6963 745b 2246 6169 7256 616c 7565  eDict["FairValue
+00015540: 225d 203d 2073 7472 2866 6169 7256 616c  "] = str(fairVal
+00015550: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
+00015560: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
+00015570: 745b 2246 5644 6966 6622 5d20 3d20 6661  t["FVDiff"] = fa
+00015580: 6972 5661 6c75 6544 6966 660d 0a20 2020  irValueDiff..   
+00015590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000155a0: 2073 6372 6565 6e44 6963 745b 2246 5644   screenDict["FVD
+000155b0: 6966 6622 5d20 3d20 6661 6972 5661 6c75  iff"] = fairValu
+000155c0: 6544 6966 660d 0a20 2020 2020 2020 2020  eDiff..         
+000155d0: 2020 2020 2020 2020 2020 2073 6372 6565             scree
+000155e0: 6e44 6963 745b 2246 6169 7256 616c 7565  nDict["FairValue
+000155f0: 225d 203d 2028 636f 6c6f 7254 6578 742e  "] = (colorText.
+00015600: 4752 4545 4e20 6966 2066 6169 7256 616c  GREEN if fairVal
+00015610: 7565 203e 3d20 6c74 7020 656c 7365 2063  ue >= ltp else c
+00015620: 6f6c 6f72 5465 7874 2e46 4149 4c29 202b  olorText.FAIL) +
+00015630: 2073 6176 6544 6963 745b 2246 6169 7256   saveDict["FairV
+00015640: 616c 7565 225d 202b 2063 6f6c 6f72 5465  alue"] + colorTe
+00015650: 7874 2e45 4e44 0d0a 2020 2020 2020 2020  xt.END..        
+00015660: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
+00015670: 7469 6f6e 2061 7320 653a 2020 2320 7072  tion as e:  # pr
+00015680: 6167 6d61 3a20 6e6f 2063 6f76 6572 0d0a  agma: no cover..
+00015690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000156a0: 7365 6c66 2e64 6566 6175 6c74 5f6c 6f67  self.default_log
+000156b0: 6765 722e 6465 6275 6728 652c 2065 7863  ger.debug(e, exc
+000156c0: 5f69 6e66 6f3d 5472 7565 290d 0a20 2020  _info=True)..   
+000156d0: 2020 2020 2020 2020 2020 2020 2070 6173               pas
+000156e0: 730d 0a20 2020 2020 2020 2020 2020 200d  s..            .
+000156f0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00015700: 6d66 5f69 6e73 745f 6f77 6e65 7273 6869  mf_inst_ownershi
+00015710: 7043 6861 6e67 6520 3e20 303a 0d0a 2020  pChange > 0:..  
+00015720: 2020 2020 2020 2020 2020 2020 2020 6d66                mf
+00015730: 203d 2066 224d 4649 3ae2 96b2 207b 6368   = f"MFI:... {ch
+00015740: 616e 6765 5f6d 696c 6c69 6f6e 737d 220d  ange_millions}".
+00015750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015760: 206d 6673 203d 2063 6f6c 6f72 5465 7874   mfs = colorText
+00015770: 2e47 5245 454e 202b 206d 6620 2b20 636f  .GREEN + mf + co
+00015780: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
+00015790: 2020 2020 2020 2020 2065 6c69 6620 6d66           elif mf
+000157a0: 5f69 6e73 745f 6f77 6e65 7273 6869 7043  _inst_ownershipC
+000157b0: 6861 6e67 6520 3c20 303a 0d0a 2020 2020  hange < 0:..    
+000157c0: 2020 2020 2020 2020 2020 2020 6d66 203d              mf =
+000157d0: 2066 224d 4649 3ae2 96bc 207b 6368 616e   f"MFI:... {chan
+000157e0: 6765 5f6d 696c 6c69 6f6e 737d 220d 0a20  ge_millions}".. 
+000157f0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00015800: 6673 203d 2063 6f6c 6f72 5465 7874 2e46  fs = colorText.F
+00015810: 4149 4c20 2b20 6d66 202b 2063 6f6c 6f72  AIL + mf + color
+00015820: 5465 7874 2e45 4e44 0d0a 0d0a 2020 2020  Text.END....    
+00015830: 2020 2020 7361 7665 6420 3d20 7365 6c66      saved = self
+00015840: 2e66 696e 6443 7572 7265 6e74 5361 7665  .findCurrentSave
+00015850: 6456 616c 7565 2873 6372 6565 6e44 6963  dValue(screenDic
+00015860: 742c 7361 7665 4469 6374 2c22 5472 656e  t,saveDict,"Tren
+00015870: 6422 290d 0a20 2020 2020 2020 2064 6563  d")..        dec
+00015880: 6973 696f 6e5f 7363 7220 3d20 2863 6f6c  ision_scr = (col
+00015890: 6f72 5465 7874 2e47 5245 454e 2069 6620  orText.GREEN if 
+000158a0: 6973 5570 7472 656e 6420 656c 7365 2028  isUptrend else (
+000158b0: 636f 6c6f 7254 6578 742e 4641 494c 2069  colorText.FAIL i
+000158c0: 6620 6973 446f 776e 7472 656e 6420 656c  f isDowntrend el
+000158d0: 7365 2063 6f6c 6f72 5465 7874 2e57 4152  se colorText.WAR
+000158e0: 4e29 2920 2b20 6622 7b64 6563 6973 696f  N)) + f"{decisio
+000158f0: 6e7d 2220 2b20 636f 6c6f 7254 6578 742e  n}" + colorText.
+00015900: 454e 440d 0a20 2020 2020 2020 2064 6d61  END..        dma
+00015910: 3530 6465 6369 7369 6f6e 5f73 6372 203d  50decision_scr =
+00015920: 2028 636f 6c6f 7254 6578 742e 4752 4545   (colorText.GREE
+00015930: 4e20 6966 2069 7335 3044 4d41 5570 7472  N if is50DMAUptr
+00015940: 656e 6420 656c 7365 2028 636f 6c6f 7254  end else (colorT
+00015950: 6578 742e 4641 494c 2069 6620 6973 3530  ext.FAIL if is50
+00015960: 444d 4144 6f77 6e74 7265 6e64 2065 6c73  DMADowntrend els
+00015970: 6520 636f 6c6f 7254 6578 742e 5741 524e  e colorText.WARN
+00015980: 2929 202b 2066 227b 646d 6135 3064 6563  )) + f"{dma50dec
+00015990: 6973 696f 6e7d 2220 2b20 636f 6c6f 7254  ision}" + colorT
+000159a0: 6578 742e 454e 440d 0a20 2020 2020 2020  ext.END..       
+000159b0: 2073 6176 6544 6963 745b 2254 7265 6e64   saveDict["Trend
+000159c0: 225d 203d 2066 227b 7361 7665 645b 315d  "] = f"{saved[1]
+000159d0: 7d20 7b64 6563 6973 696f 6e7d 207b 646d  } {decision} {dm
+000159e0: 6135 3064 6563 6973 696f 6e7d 207b 6d66  a50decision} {mf
+000159f0: 7d22 0d0a 2020 2020 2020 2020 7363 7265  }"..        scre
+00015a00: 656e 4469 6374 5b22 5472 656e 6422 5d20  enDict["Trend"] 
+00015a10: 3d20 6622 7b73 6176 6564 5b30 5d7d 207b  = f"{saved[0]} {
+00015a20: 6465 6369 7369 6f6e 5f73 6372 7d20 7b64  decision_scr} {d
+00015a30: 6d61 3530 6465 6369 7369 6f6e 5f73 6372  ma50decision_scr
+00015a40: 7d20 7b6d 6673 7d22 0d0a 2020 2020 2020  } {mfs}"..      
+00015a50: 2020 7361 7665 4469 6374 5b22 4d46 4922    saveDict["MFI"
+00015a60: 5d20 3d20 6d66 5f69 6e73 745f 6f77 6e65  ] = mf_inst_owne
+00015a70: 7273 6869 7043 6861 6e67 650d 0a20 2020  rshipChange..   
+00015a80: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+00015a90: 224d 4649 225d 203d 206d 665f 696e 7374  "MFI"] = mf_inst
+00015aa0: 5f6f 776e 6572 7368 6970 4368 616e 6765  _ownershipChange
+00015ab0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00015ac0: 2069 7355 7074 7265 6e64 2c20 6d66 5f69   isUptrend, mf_i
+00015ad0: 6e73 745f 6f77 6e65 7273 6869 7043 6861  nst_ownershipCha
+00015ae0: 6e67 652c 2066 6169 7256 616c 7565 4469  nge, fairValueDi
+00015af0: 6666 0d0a 2020 2020 0d0a 2020 2020 2320  ff..    ..    # 
+00015b00: 5072 6976 6174 6520 6d65 7468 6f64 2074  Private method t
+00015b10: 6f20 6669 6e64 2063 616e 646c 6520 7479  o find candle ty
+00015b20: 7065 0d0a 2020 2020 2320 5472 7565 203d  pe..    # True =
+00015b30: 2042 756c 6c69 7368 2c20 4661 6c73 6520   Bullish, False 
+00015b40: 3d20 4265 6172 6973 680d 0a20 2020 2064  = Bearish..    d
+00015b50: 6566 2067 6574 4361 6e64 6c65 5479 7065  ef getCandleType
+00015b60: 2873 656c 662c 2064 6169 6c79 4461 7461  (self, dailyData
+00015b70: 293a 0d0a 2020 2020 2020 2020 7265 7475  ):..        retu
+00015b80: 726e 2062 6f6f 6c28 6461 696c 7944 6174  rn bool(dailyDat
+00015b90: 615b 2243 6c6f 7365 225d 2e69 6c6f 635b  a["Close"].iloc[
+00015ba0: 305d 203e 3d20 6461 696c 7944 6174 615b  0] >= dailyData[
+00015bb0: 224f 7065 6e22 5d2e 696c 6f63 5b30 5d29  "Open"].iloc[0])
+00015bc0: 0d0a 0d0a 2020 2020 6465 6620 6765 7443  ....    def getC
+00015bd0: 616e 646c 6542 6f64 7948 6569 6768 7428  andleBodyHeight(
+00015be0: 7365 6c66 2c20 6461 696c 7944 6174 6129  self, dailyData)
+00015bf0: 3a0d 0a20 2020 2020 2020 2062 6f64 7948  :..        bodyH
+00015c00: 6569 6768 7420 3d20 6461 696c 7944 6174  eight = dailyDat
+00015c10: 615b 2243 6c6f 7365 225d 2e69 6c6f 635b  a["Close"].iloc[
+00015c20: 305d 202d 2064 6169 6c79 4461 7461 5b22  0] - dailyData["
+00015c30: 4f70 656e 225d 2e69 6c6f 635b 305d 0d0a  Open"].iloc[0]..
+00015c40: 2020 2020 2020 2020 7265 7475 726e 2062          return b
+00015c50: 6f64 7948 6569 6768 740d 0a0d 0a20 2020  odyHeight....   
+00015c60: 2064 6566 2067 6574 4661 6972 5661 6c75   def getFairValu
+00015c70: 6528 7365 6c66 2c20 7374 6f63 6b2c 2068  e(self, stock, h
+00015c80: 6f73 7444 6174 613d 4e6f 6e65 2c20 666f  ostData=None, fo
+00015c90: 7263 653d 4661 6c73 652c 6578 6368 616e  rce=False,exchan
+00015ca0: 6765 4e61 6d65 3d22 494e 4449 4122 293a  geName="INDIA"):
+00015cb0: 0d0a 2020 2020 2020 2020 6966 2068 6f73  ..        if hos
+00015cc0: 7444 6174 6120 6973 204e 6f6e 6520 6f72  tData is None or
+00015cd0: 206c 656e 2868 6f73 7444 6174 6129 203c   len(hostData) <
+00015ce0: 2031 3a0d 0a20 2020 2020 2020 2020 2020   1:..           
+00015cf0: 2068 6f73 7444 6174 6120 3d20 7064 2e44   hostData = pd.D
+00015d00: 6174 6146 7261 6d65 2829 0d0a 2020 2020  ataFrame()..    
+00015d10: 2020 2020 2320 4c65 7427 7320 6c6f 6f6b      # Let's look
+00015d20: 2066 6f72 2066 6169 7220 7661 6c75 6573   for fair values
+00015d30: 0d0a 2020 2020 2020 2020 6661 6972 5661  ..        fairVa
+00015d40: 6c75 6520 3d20 300d 0a20 2020 2020 2020  lue = 0..       
+00015d50: 2069 6620 2246 6169 7256 616c 7565 2220   if "FairValue" 
+00015d60: 696e 2068 6f73 7444 6174 612e 636f 6c75  in hostData.colu
+00015d70: 6d6e 7320 616e 6420 504b 4461 7465 5574  mns and PKDateUt
+00015d80: 696c 6974 6965 732e 6375 7272 656e 7444  ilities.currentD
+00015d90: 6174 6554 696d 6528 292e 7765 656b 6461  ateTime().weekda
+00015da0: 7928 2920 3c3d 2034 3a0d 0a20 2020 2020  y() <= 4:..     
+00015db0: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
+00015dc0: 2020 2020 2020 2020 2020 2020 2066 6169               fai
+00015dd0: 7256 616c 7565 203d 2068 6f73 7444 6174  rValue = hostDat
+00015de0: 612e 6c6f 635b 686f 7374 4461 7461 2e69  a.loc[hostData.i
+00015df0: 6e64 6578 5b2d 315d 2c22 4661 6972 5661  ndex[-1],"FairVa
+00015e00: 6c75 6522 5d0d 0a20 2020 2020 2020 2020  lue"]..         
+00015e10: 2020 2065 7863 6570 7420 284b 6579 4572     except (KeyEr
+00015e20: 726f 722c 496e 6465 7845 7272 6f72 293a  ror,IndexError):
+00015e30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015e40: 2020 2020 2020 7061 7373 0d0a 2020 2020        pass..    
+00015e50: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00015e60: 2020 2020 2020 2069 6620 504b 4461 7465         if PKDate
+00015e70: 5574 696c 6974 6965 732e 6375 7272 656e  Utilities.curren
+00015e80: 7444 6174 6554 696d 6528 292e 7765 656b  tDateTime().week
+00015e90: 6461 7928 2920 3e3d 2035 206f 7220 666f  day() >= 5 or fo
+00015ea0: 7263 653a 0d0a 2020 2020 2020 2020 2020  rce:..          
+00015eb0: 2020 2020 2020 7365 6375 7269 7479 203d        security =
+00015ec0: 204e 6f6e 650d 0a20 2020 2020 2020 2020   None..         
+00015ed0: 2020 2020 2020 2023 2052 6566 7265 7368         # Refresh
+00015ee0: 2065 6163 6820 7361 7475 7264 6179 206f   each saturday o
+00015ef0: 7220 7375 6e64 6179 206f 7220 7768 656e  r sunday or when
+00015f00: 206e 6f74 2066 6f75 6e64 2069 6e20 7361   not found in sa
+00015f10: 7665 6420 6461 7461 0d0a 2020 2020 2020  ved data..      
+00015f20: 2020 2020 2020 2020 2020 7472 793a 0d0a            try:..
+00015f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f40: 2020 2020 7769 7468 2053 7570 7072 6573      with Suppres
+00015f50: 734f 7574 7075 7428 7375 7070 7265 7373  sOutput(suppress
+00015f60: 5f73 7464 6572 723d 5472 7565 2c20 7375  _stderr=True, su
+00015f70: 7070 7265 7373 5f73 7464 6f75 743d 5472  ppress_stdout=Tr
+00015f80: 7565 293a 0d0a 2020 2020 2020 2020 2020  ue):..          
+00015f90: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00015fa0: 6375 7269 7479 203d 2053 746f 636b 2873  curity = Stock(s
+00015fb0: 746f 636b 2c65 7863 6861 6e67 653d 6578  tock,exchange=ex
+00015fc0: 6368 616e 6765 4e61 6d65 290d 0a20 2020  changeName)..   
+00015fd0: 2020 2020 2020 2020 2020 2020 2065 7863               exc
+00015fe0: 6570 7420 5661 6c75 6545 7272 6f72 3a20  ept ValueError: 
+00015ff0: 2320 7072 6167 6d61 3a20 6e6f 2063 6f76  # pragma: no cov
+00016000: 6572 0d0a 2020 2020 2020 2020 2020 2020  er..            
+00016010: 2020 2020 2020 2020 2320 5765 2064 6964          # We did
+00016020: 206e 6f74 2066 696e 6420 7468 6520 7374   not find the st
+00016030: 6f63 6b3f 2049 7427 7320 6f6b 6179 2e20  ock? It's okay. 
+00016040: 4d6f 7665 206f 6e20 746f 2074 6865 206e  Move on to the n
+00016050: 6578 7420 6f6e 652e 0d0a 2020 2020 2020  ext one...      
+00016060: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00016070: 7373 0d0a 2020 2020 2020 2020 2020 2020  ss..            
+00016080: 2020 2020 6966 2073 6563 7572 6974 7920      if security 
+00016090: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+000160a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000160b0: 2020 7769 7468 2053 7570 7072 6573 734f    with SuppressO
+000160c0: 7574 7075 7428 7375 7070 7265 7373 5f73  utput(suppress_s
+000160d0: 7464 6572 723d 5472 7565 2c20 7375 7070  tderr=True, supp
+000160e0: 7265 7373 5f73 7464 6f75 743d 5472 7565  ress_stdout=True
+000160f0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00016100: 2020 2020 2020 2020 2020 2020 6676 203d              fv =
+00016110: 2073 6563 7572 6974 792e 6661 6972 5661   security.fairVa
+00016120: 6c75 6528 290d 0a20 2020 2020 2020 2020  lue()..         
+00016130: 2020 2020 2020 2020 2020 2069 6620 6676             if fv
+00016140: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+00016150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016160: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
+00016170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016180: 2020 2020 2020 2020 2066 7652 6573 706f           fvRespo
+00016190: 6e73 6556 616c 7565 203d 2066 765b 226c  nseValue = fv["l
+000161a0: 6174 6573 7446 6169 7256 616c 7565 225d  atestFairValue"]
+000161b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000161c0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000161d0: 2066 7652 6573 706f 6e73 6556 616c 7565   fvResponseValue
+000161e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+000161f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016200: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00016210: 6169 7256 616c 7565 203d 2066 6c6f 6174  airValue = float
+00016220: 2866 7652 6573 706f 6e73 6556 616c 7565  (fvResponseValue
+00016230: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00016240: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00016250: 743a 2023 2070 7261 676d 613a 206e 6f20  t: # pragma: no 
+00016260: 636f 7665 720d 0a20 2020 2020 2020 2020  cover..         
+00016270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016280: 2020 2070 6173 730d 0a20 2020 2020 2020     pass..       
+00016290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000162a0: 2020 2020 2023 2073 656c 662e 6465 6661       # self.defa
+000162b0: 756c 745f 6c6f 6767 6572 2e64 6562 7567  ult_logger.debug
+000162c0: 2866 227b 657d 5c6e 5265 7370 6f6e 7365  (f"{e}\nResponse
+000162d0: 3a66 763a 5c6e 7b66 767d 222c 2065 7863  :fv:\n{fv}", exc
+000162e0: 5f69 6e66 6f3d 5472 7565 290d 0a20 2020  _info=True)..   
+000162f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016300: 2066 6169 7256 616c 7565 203d 2072 6f75   fairValue = rou
+00016310: 6e64 2866 6c6f 6174 2866 6169 7256 616c  nd(float(fairVal
+00016320: 7565 292c 3129 0d0a 2020 2020 2020 2020  ue),1)..        
+00016330: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+00016340: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016350: 2020 2020 2020 2020 2020 686f 7374 4461            hostDa
+00016360: 7461 2e6c 6f63 5b68 6f73 7444 6174 612e  ta.loc[hostData.
+00016370: 696e 6465 785b 2d31 5d2c 2246 6169 7256  index[-1],"FairV
+00016380: 616c 7565 225d 203d 2066 6169 7256 616c  alue"] = fairVal
+00016390: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
+000163a0: 2020 2020 2020 2020 6578 6365 7074 2028          except (
+000163b0: 4b65 7945 7272 6f72 2c49 6e64 6578 4572  KeyError,IndexEr
+000163c0: 726f 7229 3a0d 0a20 2020 2020 2020 2020  ror):..         
+000163d0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000163e0: 6173 730d 0a20 2020 2020 2020 2072 6574  ass..        ret
+000163f0: 7572 6e20 6661 6972 5661 6c75 650d 0a0d  urn fairValue...
+00016400: 0a20 2020 2064 6566 2067 6574 4d75 7475  .    def getMutu
+00016410: 616c 4675 6e64 5374 6174 7573 2873 656c  alFundStatus(sel
+00016420: 662c 2073 746f 636b 2c6f 6e6c 794d 463d  f, stock,onlyMF=
+00016430: 4661 6c73 652c 2068 6f73 7444 6174 613d  False, hostData=
+00016440: 4e6f 6e65 2c20 666f 7263 653d 4661 6c73  None, force=Fals
+00016450: 652c 6578 6368 616e 6765 4e61 6d65 3d22  e,exchangeName="
+00016460: 494e 4449 4122 293a 0d0a 2020 2020 2020  INDIA"):..      
+00016470: 2020 6966 2068 6f73 7444 6174 6120 6973    if hostData is
+00016480: 204e 6f6e 6520 6f72 206c 656e 2868 6f73   None or len(hos
+00016490: 7444 6174 6129 203c 2031 3a0d 0a20 2020  tData) < 1:..   
+000164a0: 2020 2020 2020 2020 2068 6f73 7444 6174           hostDat
+000164b0: 6120 3d20 7064 2e44 6174 6146 7261 6d65  a = pd.DataFrame
+000164c0: 2829 0d0a 2020 2020 2020 2020 0d0a 2020  ()..        ..  
+000164d0: 2020 2020 2020 6e65 7443 6861 6e67 654d        netChangeM
+000164e0: 4620 3d20 300d 0a20 2020 2020 2020 206e  F = 0..        n
+000164f0: 6574 4368 616e 6765 496e 7374 203d 2030  etChangeInst = 0
+00016500: 0d0a 2020 2020 2020 2020 6c61 7465 7374  ..        latest
+00016510: 5f6d 6664 6174 6520 3d20 4e6f 6e65 0d0a  _mfdate = None..
+00016520: 2020 2020 2020 2020 6c61 7465 7374 5f69          latest_i
+00016530: 6e73 7464 6174 6520 3d20 4e6f 6e65 0d0a  nstdate = None..
+00016540: 2020 2020 2020 2020 6e65 6564 7346 7265          needsFre
+00016550: 7368 5570 6461 7465 203d 2054 7275 650d  shUpdate = True.
+00016560: 0a20 2020 2020 2020 206c 6173 7444 6179  .        lastDay
+00016570: 4c61 7374 4d6f 6e74 6820 3d20 504b 4461  LastMonth = PKDa
+00016580: 7465 5574 696c 6974 6965 732e 6c61 7374  teUtilities.last
+00016590: 5f64 6179 5f6f 665f 7072 6576 696f 7573  _day_of_previous
+000165a0: 5f6d 6f6e 7468 2850 4b44 6174 6555 7469  _month(PKDateUti
+000165b0: 6c69 7469 6573 2e63 7572 7265 6e74 4461  lities.currentDa
+000165c0: 7465 5469 6d65 2829 290d 0a20 2020 2020  teTime())..     
+000165d0: 2020 2069 6620 686f 7374 4461 7461 2069     if hostData i
+000165e0: 7320 6e6f 7420 4e6f 6e65 2061 6e64 206c  s not None and l
+000165f0: 656e 2868 6f73 7444 6174 6129 203e 2030  en(hostData) > 0
+00016600: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
+00016610: 6620 224d 4622 2069 6e20 686f 7374 4461  f "MF" in hostDa
+00016620: 7461 2e63 6f6c 756d 6e73 206f 7220 2246  ta.columns or "F
+00016630: 4949 2220 696e 2068 6f73 7444 6174 612e  II" in hostData.
+00016640: 636f 6c75 6d6e 733a 0d0a 2020 2020 2020  columns:..      
+00016650: 2020 2020 2020 2020 2020 7472 793a 0d0a            try:..
+00016660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016670: 2020 2020 6e65 7443 6861 6e67 654d 4620      netChangeMF 
+00016680: 3d20 686f 7374 4461 7461 2e6c 6f63 5b68  = hostData.loc[h
+00016690: 6f73 7444 6174 612e 696e 6465 785b 2d31  ostData.index[-1
+000166a0: 5d2c 224d 4622 5d0d 0a20 2020 2020 2020  ],"MF"]..       
+000166b0: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+000166c0: 284b 6579 4572 726f 722c 496e 6465 7845  (KeyError,IndexE
+000166d0: 7272 6f72 293a 0d0a 2020 2020 2020 2020  rror):..        
+000166e0: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+000166f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016700: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
+00016710: 2020 2020 2020 2020 2020 2020 6e65 7443              netC
+00016720: 6861 6e67 6549 6e73 7420 3d20 686f 7374  hangeInst = host
+00016730: 4461 7461 2e6c 6f63 5b68 6f73 7444 6174  Data.loc[hostDat
+00016740: 612e 696e 6465 785b 2d31 5d2c 2246 4949  a.index[-1],"FII
+00016750: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
+00016760: 2020 2020 6578 6365 7074 2028 4b65 7945      except (KeyE
+00016770: 7272 6f72 2c49 6e64 6578 4572 726f 7229  rror,IndexError)
+00016780: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00016790: 2020 2020 2020 2070 6173 730d 0a20 2020         pass..   
+000167a0: 2020 2020 2020 2020 2020 2020 2074 7279               try
+000167b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000167c0: 2020 2020 2020 206c 6174 6573 745f 6d66         latest_mf
+000167d0: 6461 7465 203d 2068 6f73 7444 6174 612e  date = hostData.
+000167e0: 6c6f 635b 686f 7374 4461 7461 2e69 6e64  loc[hostData.ind
+000167f0: 6578 5b2d 315d 2c22 4d46 5f44 6174 6522  ex[-1],"MF_Date"
+00016800: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00016810: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00016820: 616e 6365 286c 6174 6573 745f 6d66 6461  ance(latest_mfda
+00016830: 7465 2c20 666c 6f61 7429 3a0d 0a20 2020  te, float):..   
 00016840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016850: 6966 206c 6174 6573 745f 6d66 6461 7465  if latest_mfdate
-00016860: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
-00016870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016880: 2020 2073 6176 6564 5f6d 6664 6174 6520     saved_mfdate 
-00016890: 3d20 504b 4461 7465 5574 696c 6974 6965  = PKDateUtilitie
-000168a0: 732e 6461 7465 4672 6f6d 596d 6453 7472  s.dateFromYmdStr
-000168b0: 696e 6728 6c61 7465 7374 5f6d 6664 6174  ing(latest_mfdat
-000168c0: 652e 7370 6c69 7428 2254 2229 5b30 5d29  e.split("T")[0])
-000168d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000168e0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-000168f0: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-00016900: 6564 5f6d 6664 6174 6520 3d20 6c61 7374  ed_mfdate = last
-00016910: 4461 794c 6173 744d 6f6e 7468 202d 2064  DayLastMonth - d
-00016920: 6174 6574 696d 652e 7469 6d65 6465 6c74  atetime.timedelt
-00016930: 6128 3129 0d0a 2020 2020 2020 2020 2020  a(1)..          
-00016940: 2020 2020 2020 6966 206c 6174 6573 745f        if latest_
-00016950: 696e 7374 6461 7465 2069 7320 6e6f 7420  instdate is not 
-00016960: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00016970: 2020 2020 2020 2020 2020 2073 6176 6564             saved
-00016980: 5f69 6e73 7464 6174 6520 3d20 504b 4461  _instdate = PKDa
-00016990: 7465 5574 696c 6974 6965 732e 6461 7465  teUtilities.date
-000169a0: 4672 6f6d 596d 6453 7472 696e 6728 6c61  FromYmdString(la
-000169b0: 7465 7374 5f69 6e73 7464 6174 652e 7370  test_instdate.sp
-000169c0: 6c69 7428 2254 2229 5b30 5d29 0d0a 2020  lit("T")[0])..  
-000169d0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-000169e0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-000169f0: 2020 2020 2020 2020 2073 6176 6564 5f69           saved_i
-00016a00: 6e73 7464 6174 6520 3d20 6c61 7374 4461  nstdate = lastDa
-00016a10: 794c 6173 744d 6f6e 7468 202d 2064 6174  yLastMonth - dat
-00016a20: 6574 696d 652e 7469 6d65 6465 6c74 6128  etime.timedelta(
-00016a30: 3129 0d0a 2020 2020 2020 2020 2020 2020  1)..            
-00016a40: 2020 2020 746f 6461 7920 3d20 504b 4461      today = PKDa
-00016a50: 7465 5574 696c 6974 6965 732e 6375 7272  teUtilities.curr
-00016a60: 656e 7444 6174 6554 696d 6528 290d 0a20  entDateTime().. 
-00016a70: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00016a80: 6565 6473 4672 6573 6855 7064 6174 6520  eedsFreshUpdate 
-00016a90: 3d20 2873 6176 6564 5f6d 6664 6174 652e  = (saved_mfdate.
-00016aa0: 6461 7465 2829 203c 206c 6173 7444 6179  date() < lastDay
-00016ab0: 4c61 7374 4d6f 6e74 682e 6461 7465 2829  LastMonth.date()
-00016ac0: 2920 616e 6420 2873 6176 6564 5f69 6e73  ) and (saved_ins
-00016ad0: 7464 6174 652e 6461 7465 2829 203c 206c  tdate.date() < l
-00016ae0: 6173 7444 6179 4c61 7374 4d6f 6e74 682e  astDayLastMonth.
-00016af0: 6461 7465 2829 290d 0a20 2020 2020 2020  date())..       
-00016b00: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00016b10: 2020 2020 2020 2020 2020 2020 6e65 6564              need
-00016b20: 7346 7265 7368 5570 6461 7465 203d 2054  sFreshUpdate = T
-00016b30: 7275 650d 0a0d 0a20 2020 2020 2020 2069  rue....        i
-00016b40: 6620 6e65 6564 7346 7265 7368 5570 6461  f needsFreshUpda
-00016b50: 7465 2061 6e64 2066 6f72 6365 3a0d 0a20  te and force:.. 
-00016b60: 2020 2020 2020 2020 2020 206e 6574 4368             netCh
-00016b70: 616e 6765 4d46 2c20 6e65 7443 6861 6e67  angeMF, netChang
-00016b80: 6549 6e73 742c 206c 6174 6573 745f 6d66  eInst, latest_mf
-00016b90: 6461 7465 2c20 6c61 7465 7374 5f69 6e73  date, latest_ins
-00016ba0: 7464 6174 6520 3d20 7365 6c66 2e67 6574  tdate = self.get
-00016bb0: 4672 6573 684d 4649 5374 6174 7573 2873  FreshMFIStatus(s
-00016bc0: 746f 636b 2c65 7863 6861 6e67 654e 616d  tock,exchangeNam
-00016bd0: 653d 6578 6368 616e 6765 4e61 6d65 290d  e=exchangeName).
-00016be0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00016bf0: 6e65 7443 6861 6e67 654d 4620 6973 206e  netChangeMF is n
-00016c00: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-00016c10: 2020 2020 2020 2020 2020 7472 793a 0d0a            try:..
-00016c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c30: 2020 2020 686f 7374 4461 7461 2e6c 6f63      hostData.loc
-00016c40: 5b68 6f73 7444 6174 612e 696e 6465 785b  [hostData.index[
-00016c50: 2d31 5d2c 224d 4622 5d20 3d20 6e65 7443  -1],"MF"] = netC
-00016c60: 6861 6e67 654d 460d 0a20 2020 2020 2020  hangeMF..       
-00016c70: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-00016c80: 284b 6579 4572 726f 722c 496e 6465 7845  (KeyError,IndexE
-00016c90: 7272 6f72 293a 0d0a 2020 2020 2020 2020  rror):..        
-00016ca0: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-00016cb0: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-00016cc0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00016cd0: 2020 2020 206e 6574 4368 616e 6765 4d46       netChangeMF
-00016ce0: 203d 2030 0d0a 2020 2020 2020 2020 2020   = 0..          
-00016cf0: 2020 6966 206c 6174 6573 745f 6d66 6461    if latest_mfda
-00016d00: 7465 2069 7320 6e6f 7420 4e6f 6e65 3a0d  te is not None:.
-00016d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016d20: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
-00016d30: 2020 2020 2020 2020 2020 2068 6f73 7444             hostD
-00016d40: 6174 612e 6c6f 635b 686f 7374 4461 7461  ata.loc[hostData
-00016d50: 2e69 6e64 6578 5b2d 315d 2c22 4d46 5f44  .index[-1],"MF_D
-00016d60: 6174 6522 5d20 3d20 6c61 7465 7374 5f6d  ate"] = latest_m
-00016d70: 6664 6174 650d 0a20 2020 2020 2020 2020  fdate..         
-00016d80: 2020 2020 2020 2065 7863 6570 7420 284b         except (K
-00016d90: 6579 4572 726f 722c 496e 6465 7845 7272  eyError,IndexErr
-00016da0: 6f72 293a 0d0a 2020 2020 2020 2020 2020  or):..          
-00016db0: 2020 2020 2020 2020 2020 7061 7373 0d0a            pass..
-00016dc0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00016dd0: 6574 4368 616e 6765 496e 7374 2069 7320  etChangeInst is 
-00016de0: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-00016df0: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
-00016e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016e10: 2020 2020 2068 6f73 7444 6174 612e 6c6f       hostData.lo
-00016e20: 635b 686f 7374 4461 7461 2e69 6e64 6578  c[hostData.index
-00016e30: 5b2d 315d 2c22 4649 4922 5d20 3d20 6e65  [-1],"FII"] = ne
-00016e40: 7443 6861 6e67 6549 6e73 740d 0a20 2020  tChangeInst..   
-00016e50: 2020 2020 2020 2020 2020 2020 2065 7863               exc
-00016e60: 6570 7420 284b 6579 4572 726f 722c 496e  ept (KeyError,In
-00016e70: 6465 7845 7272 6f72 293a 0d0a 2020 2020  dexError):..    
-00016e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e90: 7061 7373 0d0a 2020 2020 2020 2020 2020  pass..          
-00016ea0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00016eb0: 2020 2020 2020 2020 206e 6574 4368 616e           netChan
-00016ec0: 6765 496e 7374 203d 2030 0d0a 2020 2020  geInst = 0..    
-00016ed0: 2020 2020 2020 2020 6966 206c 6174 6573          if lates
-00016ee0: 745f 696e 7374 6461 7465 2069 7320 6e6f  t_instdate is no
-00016ef0: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-00016f00: 2020 2020 2020 2020 2074 7279 3a0d 0a20           try:.. 
-00016f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f20: 2020 2068 6f73 7444 6174 612e 6c6f 635b     hostData.loc[
-00016f30: 686f 7374 4461 7461 2e69 6e64 6578 5b2d  hostData.index[-
-00016f40: 315d 2c22 4649 495f 4461 7465 225d 203d  1],"FII_Date"] =
-00016f50: 206c 6174 6573 745f 696e 7374 6461 7465   latest_instdate
-00016f60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016f70: 2020 6578 6365 7074 2028 4b65 7945 7272    except (KeyErr
-00016f80: 6f72 2c49 6e64 6578 4572 726f 7229 3a0d  or,IndexError):.
-00016f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016fa0: 2020 2020 2070 6173 730d 0a20 2020 2020       pass..     
-00016fb0: 2020 206c 6173 7444 6179 4c61 7374 4d6f     lastDayLastMo
-00016fc0: 6e74 6820 3d20 6c61 7374 4461 794c 6173  nth = lastDayLas
-00016fd0: 744d 6f6e 7468 2e73 7472 6674 696d 6528  tMonth.strftime(
-00016fe0: 2225 592d 256d 2d25 6454 3030 3a30 303a  "%Y-%m-%dT00:00:
-00016ff0: 3030 2e30 3030 2229 0d0a 2020 2020 2020  00.000")..      
-00017000: 2020 6966 206f 6e6c 794d 463a 0d0a 2020    if onlyMF:..  
-00017010: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00017020: 206e 6574 4368 616e 6765 4d46 0d0a 2020   netChangeMF..  
-00017030: 2020 2020 2020 6966 206c 6174 6573 745f        if latest_
-00017040: 696e 7374 6461 7465 203d 3d20 6c61 7465  instdate == late
-00017050: 7374 5f6d 6664 6174 653a 0d0a 2020 2020  st_mfdate:..    
-00017060: 2020 2020 2020 2020 7265 7475 726e 2028          return (
-00017070: 6e65 7443 6861 6e67 654d 4620 2b20 6e65  netChangeMF + ne
-00017080: 7443 6861 6e67 6549 6e73 7429 0d0a 2020  tChangeInst)..  
-00017090: 2020 2020 2020 656c 6966 206c 6174 6573        elif lates
-000170a0: 745f 6d66 6461 7465 203d 3d20 6c61 7374  t_mfdate == last
-000170b0: 4461 794c 6173 744d 6f6e 7468 3a0d 0a20  DayLastMonth:.. 
-000170c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000170d0: 6e20 6e65 7443 6861 6e67 654d 460d 0a20  n netChangeMF.. 
-000170e0: 2020 2020 2020 2065 6c69 6620 6c61 7465         elif late
-000170f0: 7374 5f69 6e73 7464 6174 6520 3d3d 206c  st_instdate == l
-00017100: 6173 7444 6179 4c61 7374 4d6f 6e74 683a  astDayLastMonth:
-00017110: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00017120: 7475 726e 206e 6574 4368 616e 6765 496e  turn netChangeIn
-00017130: 7374 0d0a 2020 2020 2020 2020 656c 7365  st..        else
-00017140: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
-00017150: 2066 696e 6420 7468 6520 6c61 7465 7374   find the latest
-00017160: 2064 6174 650d 0a20 2020 2020 2020 2020   date..         
-00017170: 2020 2069 6620 6c61 7465 7374 5f6d 6664     if latest_mfd
-00017180: 6174 6520 6973 206e 6f74 204e 6f6e 653a  ate is not None:
-00017190: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000171a0: 2020 6c61 7465 7374 5f6d 6664 6174 6520    latest_mfdate 
-000171b0: 3d20 504b 4461 7465 5574 696c 6974 6965  = PKDateUtilitie
-000171c0: 732e 6461 7465 4672 6f6d 596d 6453 7472  s.dateFromYmdStr
-000171d0: 696e 6728 6c61 7465 7374 5f6d 6664 6174  ing(latest_mfdat
-000171e0: 652e 7370 6c69 7428 2254 2229 5b30 5d29  e.split("T")[0])
-000171f0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00017200: 206c 6174 6573 745f 696e 7374 6461 7465   latest_instdate
-00017210: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
-00017220: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00017230: 6174 6573 745f 696e 7374 6461 7465 203d  atest_instdate =
-00017240: 2050 4b44 6174 6555 7469 6c69 7469 6573   PKDateUtilities
-00017250: 2e64 6174 6546 726f 6d59 6d64 5374 7269  .dateFromYmdStri
-00017260: 6e67 286c 6174 6573 745f 696e 7374 6461  ng(latest_instda
-00017270: 7465 2e73 706c 6974 2822 5422 295b 305d  te.split("T")[0]
-00017280: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
-00017290: 6574 7572 6e20 6e65 7443 6861 6e67 654d  eturn netChangeM
-000172a0: 4620 6966 2028 286c 6174 6573 745f 6d66  F if ((latest_mf
-000172b0: 6461 7465 2069 7320 6e6f 7420 4e6f 6e65  date is not None
-000172c0: 2920 616e 6420 6c61 7465 7374 5f6d 6664  ) and latest_mfd
-000172d0: 6174 6520 3e20 286c 6174 6573 745f 696e  ate > (latest_in
-000172e0: 7374 6461 7465 2069 6620 6c61 7465 7374  stdate if latest
-000172f0: 5f69 6e73 7464 6174 6520 6973 206e 6f74  _instdate is not
-00017300: 204e 6f6e 6520 656c 7365 2028 6c61 7465   None else (late
-00017310: 7374 5f6d 6664 6174 6520 2d20 6461 7465  st_mfdate - date
-00017320: 7469 6d65 2e74 696d 6564 656c 7461 2831  time.timedelta(1
-00017330: 2929 2929 2065 6c73 6520 6e65 7443 6861  )))) else netCha
-00017340: 6e67 6549 6e73 740d 0a0d 0a20 2020 2064  ngeInst....    d
-00017350: 6566 2067 6574 4672 6573 684d 4649 5374  ef getFreshMFISt
-00017360: 6174 7573 2873 656c 662c 2073 746f 636b  atus(self, stock
-00017370: 2c65 7863 6861 6e67 654e 616d 653d 2249  ,exchangeName="I
-00017380: 4e44 4941 2229 3a0d 0a20 2020 2020 2020  NDIA"):..       
-00017390: 2063 6861 6e67 6553 7461 7475 7344 6174   changeStatusDat
-000173a0: 614d 4620 3d20 4e6f 6e65 0d0a 2020 2020  aMF = None..    
-000173b0: 2020 2020 6368 616e 6765 5374 6174 7573      changeStatus
-000173c0: 4461 7461 496e 7374 203d 204e 6f6e 650d  DataInst = None.
-000173d0: 0a20 2020 2020 2020 206e 6574 4368 616e  .        netChan
-000173e0: 6765 4d46 203d 2030 0d0a 2020 2020 2020  geMF = 0..      
-000173f0: 2020 6e65 7443 6861 6e67 6549 6e73 7420    netChangeInst 
-00017400: 3d20 300d 0a20 2020 2020 2020 206c 6174  = 0..        lat
-00017410: 6573 745f 6d66 6461 7465 203d 204e 6f6e  est_mfdate = Non
-00017420: 650d 0a20 2020 2020 2020 206c 6174 6573  e..        lates
-00017430: 745f 696e 7374 6461 7465 203d 204e 6f6e  t_instdate = Non
-00017440: 650d 0a20 2020 2020 2020 2073 6563 7572  e..        secur
-00017450: 6974 7920 3d20 4e6f 6e65 0d0a 2020 2020  ity = None..    
-00017460: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-00017470: 2020 2020 2020 7769 7468 2053 7570 7072        with Suppr
-00017480: 6573 734f 7574 7075 7428 7375 7070 7265  essOutput(suppre
-00017490: 7373 5f73 7464 6572 723d 5472 7565 2c20  ss_stderr=True, 
-000174a0: 7375 7070 7265 7373 5f73 7464 6f75 743d  suppress_stdout=
-000174b0: 5472 7565 293a 0d0a 2020 2020 2020 2020  True):..        
-000174c0: 2020 2020 2020 2020 7365 6375 7269 7479          security
-000174d0: 203d 2053 746f 636b 2873 746f 636b 2c65   = Stock(stock,e
-000174e0: 7863 6861 6e67 653d 6578 6368 616e 6765  xchange=exchange
-000174f0: 4e61 6d65 290d 0a20 2020 2020 2020 2065  Name)..        e
-00017500: 7863 6570 7420 5661 6c75 6545 7272 6f72  xcept ValueError
-00017510: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
-00017520: 2057 6520 6469 6420 6e6f 7420 6669 6e64   We did not find
-00017530: 2074 6865 2073 746f 636b 3f20 4974 2773   the stock? It's
-00017540: 206f 6b61 792e 204d 6f76 6520 6f6e 2074   okay. Move on t
-00017550: 6f20 7468 6520 6e65 7874 206f 6e65 2e0d  o the next one..
-00017560: 0a20 2020 2020 2020 2020 2020 2070 6173  .            pas
-00017570: 730d 0a20 2020 2020 2020 2069 6620 7365  s..        if se
-00017580: 6375 7269 7479 2069 7320 6e6f 7420 4e6f  curity is not No
-00017590: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-000175a0: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
-000175b0: 2020 2020 2020 2077 6974 6820 5375 7070         with Supp
-000175c0: 7265 7373 4f75 7470 7574 2873 7570 7072  ressOutput(suppr
-000175d0: 6573 735f 7374 6465 7272 3d54 7275 652c  ess_stderr=True,
-000175e0: 2073 7570 7072 6573 735f 7374 646f 7574   suppress_stdout
-000175f0: 3d54 7275 6529 3a0d 0a20 2020 2020 2020  =True):..       
-00017600: 2020 2020 2020 2020 2020 2020 2063 6861               cha
-00017610: 6e67 6553 7461 7475 7352 6f77 734d 4620  ngeStatusRowsMF 
-00017620: 3d20 7365 6375 7269 7479 2e6d 7574 7561  = security.mutua
-00017630: 6c46 756e 644f 776e 6572 7368 6970 2874  lFundOwnership(t
-00017640: 6f70 3d35 290d 0a20 2020 2020 2020 2020  op=5)..         
-00017650: 2020 2020 2020 2020 2020 2063 6861 6e67             chang
-00017660: 6553 7461 7475 7352 6f77 7349 6e73 7420  eStatusRowsInst 
-00017670: 3d20 7365 6375 7269 7479 2e69 6e73 7469  = security.insti
-00017680: 7475 7469 6f6e 4f77 6e65 7273 6869 7028  tutionOwnership(
-00017690: 746f 703d 3529 0d0a 2020 2020 2020 2020  top=5)..        
-000176a0: 2020 2020 2020 2020 2020 2020 6368 616e              chan
-000176b0: 6765 5374 6174 7573 4461 7461 4d46 203d  geStatusDataMF =
-000176c0: 2073 6563 7572 6974 792e 6d75 7475 616c   security.mutual
-000176d0: 4675 6e64 4649 4943 6861 6e67 6544 6174  FundFIIChangeDat
-000176e0: 6128 6368 616e 6765 5374 6174 7573 526f  a(changeStatusRo
-000176f0: 7773 4d46 290d 0a20 2020 2020 2020 2020  wsMF)..         
-00017700: 2020 2020 2020 2020 2020 2063 6861 6e67             chang
-00017710: 6553 7461 7475 7344 6174 6149 6e73 7420  eStatusDataInst 
-00017720: 3d20 7365 6375 7269 7479 2e6d 7574 7561  = security.mutua
-00017730: 6c46 756e 6446 4949 4368 616e 6765 4461  lFundFIIChangeDa
-00017740: 7461 2863 6861 6e67 6553 7461 7475 7352  ta(changeStatusR
-00017750: 6f77 7349 6e73 7429 0d0a 2020 2020 2020  owsInst)..      
-00017760: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-00017770: 6570 7469 6f6e 2061 7320 653a 0d0a 2020  eption as e:..  
-00017780: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00017790: 6c66 2e64 6566 6175 6c74 5f6c 6f67 6765  lf.default_logge
-000177a0: 722e 6465 6275 6728 652c 2065 7863 5f69  r.debug(e, exc_i
-000177b0: 6e66 6f3d 5472 7565 290d 0a20 2020 2020  nfo=True)..     
-000177c0: 2020 2020 2020 2020 2020 2023 2054 7970             # Typ
-000177d0: 6545 7272 6f72 206f 7220 436f 6e6e 6563  eError or Connec
-000177e0: 7469 6f6e 4572 726f 7220 6265 6361 7573  tionError becaus
-000177f0: 6520 7765 2063 6f75 6c64 206e 6f74 2066  e we could not f
-00017800: 696e 6420 7468 6520 7374 6f63 6b20 6f72  ind the stock or
-00017810: 204d 4649 2064 6174 6120 6973 6e27 7420   MFI data isn't 
-00017820: 6176 6169 6c61 626c 653f 0d0a 2020 2020  available?..    
-00017830: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-00017840: 0d0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
-00017850: 7374 4461 794c 6173 744d 6f6e 7468 203d  stDayLastMonth =
-00017860: 2050 4b44 6174 6555 7469 6c69 7469 6573   PKDateUtilities
-00017870: 2e6c 6173 745f 6461 795f 6f66 5f70 7265  .last_day_of_pre
-00017880: 7669 6f75 735f 6d6f 6e74 6828 504b 4461  vious_month(PKDa
-00017890: 7465 5574 696c 6974 6965 732e 6375 7272  teUtilities.curr
-000178a0: 656e 7444 6174 6554 696d 6528 2929 0d0a  entDateTime())..
-000178b0: 2020 2020 2020 2020 2020 2020 6c61 7374              last
-000178c0: 4461 794c 6173 744d 6f6e 7468 203d 206c  DayLastMonth = l
-000178d0: 6173 7444 6179 4c61 7374 4d6f 6e74 682e  astDayLastMonth.
-000178e0: 7374 7266 7469 6d65 2822 2559 2d25 6d2d  strftime("%Y-%m-
-000178f0: 2564 5430 303a 3030 3a30 302e 3030 3022  %dT00:00:00.000"
-00017900: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
-00017910: 6620 6368 616e 6765 5374 6174 7573 4461  f changeStatusDa
-00017920: 7461 4d46 2069 7320 6e6f 7420 4e6f 6e65  taMF is not None
-00017930: 2061 6e64 206c 656e 2863 6861 6e67 6553   and len(changeS
-00017940: 7461 7475 7344 6174 614d 4629 203e 2030  tatusDataMF) > 0
-00017950: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00017960: 2020 2064 665f 6772 6f75 7065 644d 4620     df_groupedMF 
-00017970: 3d20 6368 616e 6765 5374 6174 7573 4461  = changeStatusDa
-00017980: 7461 4d46 2e67 726f 7570 6279 2822 6461  taMF.groupby("da
-00017990: 7465 222c 2073 6f72 743d 4661 6c73 6529  te", sort=False)
-000179a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000179b0: 2020 666f 7220 6d66 6461 7465 2c20 6466    for mfdate, df
-000179c0: 5f67 726f 7570 4d46 2069 6e20 6466 5f67  _groupMF in df_g
-000179d0: 726f 7570 6564 4d46 3a0d 0a20 2020 2020  roupedMF:..     
-000179e0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-000179f0: 6574 4368 616e 6765 4d46 203d 2064 665f  etChangeMF = df_
-00017a00: 6772 6f75 704d 465b 2263 6861 6e67 6541  groupMF["changeA
-00017a10: 6d6f 756e 7422 5d2e 7375 6d28 290d 0a20  mount"].sum().. 
-00017a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a30: 2020 206c 6174 6573 745f 6d66 6461 7465     latest_mfdate
-00017a40: 203d 206d 6664 6174 650d 0a20 2020 2020   = mfdate..     
-00017a50: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00017a60: 7265 616b 0d0a 2020 2020 2020 2020 2020  reak..          
-00017a70: 2020 6966 2063 6861 6e67 6553 7461 7475    if changeStatu
-00017a80: 7344 6174 6149 6e73 7420 6973 206e 6f74  sDataInst is not
-00017a90: 204e 6f6e 6520 616e 6420 6c65 6e28 6368   None and len(ch
-00017aa0: 616e 6765 5374 6174 7573 4461 7461 496e  angeStatusDataIn
-00017ab0: 7374 2920 3e20 303a 0d0a 2020 2020 2020  st) > 0:..      
-00017ac0: 2020 2020 2020 2020 2020 6466 5f67 726f            df_gro
-00017ad0: 7570 6564 496e 7374 203d 2063 6861 6e67  upedInst = chang
-00017ae0: 6553 7461 7475 7344 6174 6149 6e73 742e  eStatusDataInst.
-00017af0: 6772 6f75 7062 7928 2264 6174 6522 2c20  groupby("date", 
-00017b00: 736f 7274 3d46 616c 7365 290d 0a20 2020  sort=False)..   
-00017b10: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00017b20: 2069 6e73 7464 6174 652c 2064 665f 6772   instdate, df_gr
-00017b30: 6f75 7049 6e73 7420 696e 2064 665f 6772  oupInst in df_gr
-00017b40: 6f75 7065 6449 6e73 743a 0d0a 2020 2020  oupedInst:..    
-00017b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b60: 6966 2028 6c61 7465 7374 5f6d 6664 6174  if (latest_mfdat
-00017b70: 6520 6973 206e 6f74 204e 6f6e 6520 616e  e is not None an
-00017b80: 6420 6c61 7465 7374 5f6d 6664 6174 6520  d latest_mfdate 
-00017b90: 3d3d 2069 6e73 7464 6174 6529 206f 7220  == instdate) or 
-00017ba0: 286c 6174 6573 745f 6d66 6461 7465 2069  (latest_mfdate i
-00017bb0: 7320 4e6f 6e65 2920 6f72 2028 696e 7374  s None) or (inst
-00017bc0: 6461 7465 203d 3d20 6c61 7374 4461 794c  date == lastDayL
-00017bd0: 6173 744d 6f6e 7468 293a 0d0a 2020 2020  astMonth):..    
-00017be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017bf0: 2020 2020 6e65 7443 6861 6e67 6549 6e73      netChangeIns
-00017c00: 7420 3d20 6466 5f67 726f 7570 496e 7374  t = df_groupInst
-00017c10: 5b22 6368 616e 6765 416d 6f75 6e74 225d  ["changeAmount"]
-00017c20: 2e73 756d 2829 0d0a 2020 2020 2020 2020  .sum()..        
-00017c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c40: 6c61 7465 7374 5f69 6e73 7464 6174 6520  latest_instdate 
-00017c50: 3d20 696e 7374 6461 7465 0d0a 2020 2020  = instdate..    
+00016850: 2020 2020 206c 6174 6573 745f 6d66 6461       latest_mfda
+00016860: 7465 203d 2064 6174 6574 696d 652e 6461  te = datetime.da
+00016870: 7465 7469 6d65 2e66 726f 6d74 696d 6573  tetime.fromtimes
+00016880: 7461 6d70 286c 6174 6573 745f 6d66 6461  tamp(latest_mfda
+00016890: 7465 292e 7374 7266 7469 6d65 2827 2559  te).strftime('%Y
+000168a0: 2d25 6d2d 2564 2729 0d0a 2020 2020 2020  -%m-%d')..      
+000168b0: 2020 2020 2020 2020 2020 6578 6365 7074            except
+000168c0: 2028 4b65 7945 7272 6f72 2c49 6e64 6578   (KeyError,Index
+000168d0: 4572 726f 7229 3a0d 0a20 2020 2020 2020  Error):..       
+000168e0: 2020 2020 2020 2020 2020 2020 2070 6173               pas
+000168f0: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+00016900: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
+00016910: 2020 2020 2020 2020 2020 2020 206c 6174               lat
+00016920: 6573 745f 696e 7374 6461 7465 203d 2068  est_instdate = h
+00016930: 6f73 7444 6174 612e 6c6f 635b 686f 7374  ostData.loc[host
+00016940: 4461 7461 2e69 6e64 6578 5b2d 315d 2c22  Data.index[-1],"
+00016950: 4649 495f 4461 7465 225d 0d0a 2020 2020  FII_Date"]..    
+00016960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016970: 6966 2069 7369 6e73 7461 6e63 6528 6c61  if isinstance(la
+00016980: 7465 7374 5f69 6e73 7464 6174 652c 2066  test_instdate, f
+00016990: 6c6f 6174 293a 0d0a 2020 2020 2020 2020  loat):..        
+000169a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000169b0: 6c61 7465 7374 5f69 6e73 7464 6174 6520  latest_instdate 
+000169c0: 3d20 6461 7465 7469 6d65 2e64 6174 6574  = datetime.datet
+000169d0: 696d 652e 6672 6f6d 7469 6d65 7374 616d  ime.fromtimestam
+000169e0: 7028 6c61 7465 7374 5f69 6e73 7464 6174  p(latest_instdat
+000169f0: 6529 2e73 7472 6674 696d 6528 2725 592d  e).strftime('%Y-
+00016a00: 256d 2d25 6427 290d 0a20 2020 2020 2020  %m-%d')..       
+00016a10: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+00016a20: 284b 6579 4572 726f 722c 496e 6465 7845  (KeyError,IndexE
+00016a30: 7272 6f72 293a 0d0a 2020 2020 2020 2020  rror):..        
+00016a40: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+00016a50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016a60: 2020 6966 206c 6174 6573 745f 6d66 6461    if latest_mfda
+00016a70: 7465 2069 7320 6e6f 7420 4e6f 6e65 3a0d  te is not None:.
+00016a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016a90: 2020 2020 2073 6176 6564 5f6d 6664 6174       saved_mfdat
+00016aa0: 6520 3d20 504b 4461 7465 5574 696c 6974  e = PKDateUtilit
+00016ab0: 6965 732e 6461 7465 4672 6f6d 596d 6453  ies.dateFromYmdS
+00016ac0: 7472 696e 6728 6c61 7465 7374 5f6d 6664  tring(latest_mfd
+00016ad0: 6174 652e 7370 6c69 7428 2254 2229 5b30  ate.split("T")[0
+00016ae0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00016af0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00016b00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016b10: 6176 6564 5f6d 6664 6174 6520 3d20 6c61  aved_mfdate = la
+00016b20: 7374 4461 794c 6173 744d 6f6e 7468 202d  stDayLastMonth -
+00016b30: 2064 6174 6574 696d 652e 7469 6d65 6465   datetime.timede
+00016b40: 6c74 6128 3129 0d0a 2020 2020 2020 2020  lta(1)..        
+00016b50: 2020 2020 2020 2020 6966 206c 6174 6573          if lates
+00016b60: 745f 696e 7374 6461 7465 2069 7320 6e6f  t_instdate is no
+00016b70: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+00016b80: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+00016b90: 6564 5f69 6e73 7464 6174 6520 3d20 504b  ed_instdate = PK
+00016ba0: 4461 7465 5574 696c 6974 6965 732e 6461  DateUtilities.da
+00016bb0: 7465 4672 6f6d 596d 6453 7472 696e 6728  teFromYmdString(
+00016bc0: 6c61 7465 7374 5f69 6e73 7464 6174 652e  latest_instdate.
+00016bd0: 7370 6c69 7428 2254 2229 5b30 5d29 0d0a  split("T")[0])..
+00016be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016bf0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00016c00: 2020 2020 2020 2020 2020 2073 6176 6564             saved
+00016c10: 5f69 6e73 7464 6174 6520 3d20 6c61 7374  _instdate = last
+00016c20: 4461 794c 6173 744d 6f6e 7468 202d 2064  DayLastMonth - d
+00016c30: 6174 6574 696d 652e 7469 6d65 6465 6c74  atetime.timedelt
+00016c40: 6128 3129 0d0a 2020 2020 2020 2020 2020  a(1)..          
+00016c50: 2020 2020 2020 746f 6461 7920 3d20 504b        today = PK
+00016c60: 4461 7465 5574 696c 6974 6965 732e 6375  DateUtilities.cu
+00016c70: 7272 656e 7444 6174 6554 696d 6528 290d  rrentDateTime().
+00016c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016c90: 206e 6565 6473 4672 6573 6855 7064 6174   needsFreshUpdat
+00016ca0: 6520 3d20 2873 6176 6564 5f6d 6664 6174  e = (saved_mfdat
+00016cb0: 652e 6461 7465 2829 203c 206c 6173 7444  e.date() < lastD
+00016cc0: 6179 4c61 7374 4d6f 6e74 682e 6461 7465  ayLastMonth.date
+00016cd0: 2829 2920 616e 6420 2873 6176 6564 5f69  ()) and (saved_i
+00016ce0: 6e73 7464 6174 652e 6461 7465 2829 203c  nstdate.date() <
+00016cf0: 206c 6173 7444 6179 4c61 7374 4d6f 6e74   lastDayLastMont
+00016d00: 682e 6461 7465 2829 290d 0a20 2020 2020  h.date())..     
+00016d10: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00016d20: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+00016d30: 6564 7346 7265 7368 5570 6461 7465 203d  edsFreshUpdate =
+00016d40: 2054 7275 650d 0a0d 0a20 2020 2020 2020   True....       
+00016d50: 2069 6620 6e65 6564 7346 7265 7368 5570   if needsFreshUp
+00016d60: 6461 7465 2061 6e64 2066 6f72 6365 3a0d  date and force:.
+00016d70: 0a20 2020 2020 2020 2020 2020 206e 6574  .            net
+00016d80: 4368 616e 6765 4d46 2c20 6e65 7443 6861  ChangeMF, netCha
+00016d90: 6e67 6549 6e73 742c 206c 6174 6573 745f  ngeInst, latest_
+00016da0: 6d66 6461 7465 2c20 6c61 7465 7374 5f69  mfdate, latest_i
+00016db0: 6e73 7464 6174 6520 3d20 7365 6c66 2e67  nstdate = self.g
+00016dc0: 6574 4672 6573 684d 4649 5374 6174 7573  etFreshMFIStatus
+00016dd0: 2873 746f 636b 2c65 7863 6861 6e67 654e  (stock,exchangeN
+00016de0: 616d 653d 6578 6368 616e 6765 4e61 6d65  ame=exchangeName
+00016df0: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
+00016e00: 6620 6e65 7443 6861 6e67 654d 4620 6973  f netChangeMF is
+00016e10: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+00016e20: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+00016e30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016e40: 2020 2020 2020 686f 7374 4461 7461 2e6c        hostData.l
+00016e50: 6f63 5b68 6f73 7444 6174 612e 696e 6465  oc[hostData.inde
+00016e60: 785b 2d31 5d2c 224d 4622 5d20 3d20 6e65  x[-1],"MF"] = ne
+00016e70: 7443 6861 6e67 654d 460d 0a20 2020 2020  tChangeMF..     
+00016e80: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00016e90: 7420 284b 6579 4572 726f 722c 496e 6465  t (KeyError,Inde
+00016ea0: 7845 7272 6f72 293a 0d0a 2020 2020 2020  xError):..      
+00016eb0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00016ec0: 7373 0d0a 2020 2020 2020 2020 2020 2020  ss..            
+00016ed0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00016ee0: 2020 2020 2020 206e 6574 4368 616e 6765         netChange
+00016ef0: 4d46 203d 2030 0d0a 2020 2020 2020 2020  MF = 0..        
+00016f00: 2020 2020 6966 206c 6174 6573 745f 6d66      if latest_mf
+00016f10: 6461 7465 2069 7320 6e6f 7420 4e6f 6e65  date is not None
+00016f20: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00016f30: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
+00016f40: 2020 2020 2020 2020 2020 2020 2068 6f73               hos
+00016f50: 7444 6174 612e 6c6f 635b 686f 7374 4461  tData.loc[hostDa
+00016f60: 7461 2e69 6e64 6578 5b2d 315d 2c22 4d46  ta.index[-1],"MF
+00016f70: 5f44 6174 6522 5d20 3d20 6c61 7465 7374  _Date"] = latest
+00016f80: 5f6d 6664 6174 650d 0a20 2020 2020 2020  _mfdate..       
+00016f90: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+00016fa0: 284b 6579 4572 726f 722c 496e 6465 7845  (KeyError,IndexE
+00016fb0: 7272 6f72 293a 0d0a 2020 2020 2020 2020  rror):..        
+00016fc0: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+00016fd0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00016fe0: 206e 6574 4368 616e 6765 496e 7374 2069   netChangeInst i
+00016ff0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+00017000: 2020 2020 2020 2020 2020 2020 2074 7279               try
+00017010: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00017020: 2020 2020 2020 2068 6f73 7444 6174 612e         hostData.
+00017030: 6c6f 635b 686f 7374 4461 7461 2e69 6e64  loc[hostData.ind
+00017040: 6578 5b2d 315d 2c22 4649 4922 5d20 3d20  ex[-1],"FII"] = 
+00017050: 6e65 7443 6861 6e67 6549 6e73 740d 0a20  netChangeInst.. 
+00017060: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00017070: 7863 6570 7420 284b 6579 4572 726f 722c  xcept (KeyError,
+00017080: 496e 6465 7845 7272 6f72 293a 0d0a 2020  IndexError):..  
+00017090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000170a0: 2020 7061 7373 0d0a 2020 2020 2020 2020    pass..        
+000170b0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+000170c0: 2020 2020 2020 2020 2020 206e 6574 4368             netCh
+000170d0: 616e 6765 496e 7374 203d 2030 0d0a 2020  angeInst = 0..  
+000170e0: 2020 2020 2020 2020 2020 6966 206c 6174            if lat
+000170f0: 6573 745f 696e 7374 6461 7465 2069 7320  est_instdate is 
+00017100: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+00017110: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
+00017120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017130: 2020 2020 2068 6f73 7444 6174 612e 6c6f       hostData.lo
+00017140: 635b 686f 7374 4461 7461 2e69 6e64 6578  c[hostData.index
+00017150: 5b2d 315d 2c22 4649 495f 4461 7465 225d  [-1],"FII_Date"]
+00017160: 203d 206c 6174 6573 745f 696e 7374 6461   = latest_instda
+00017170: 7465 0d0a 2020 2020 2020 2020 2020 2020  te..            
+00017180: 2020 2020 6578 6365 7074 2028 4b65 7945      except (KeyE
+00017190: 7272 6f72 2c49 6e64 6578 4572 726f 7229  rror,IndexError)
+000171a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000171b0: 2020 2020 2020 2070 6173 730d 0a20 2020         pass..   
+000171c0: 2020 2020 206c 6173 7444 6179 4c61 7374       lastDayLast
+000171d0: 4d6f 6e74 6820 3d20 6c61 7374 4461 794c  Month = lastDayL
+000171e0: 6173 744d 6f6e 7468 2e73 7472 6674 696d  astMonth.strftim
+000171f0: 6528 2225 592d 256d 2d25 6454 3030 3a30  e("%Y-%m-%dT00:0
+00017200: 303a 3030 2e30 3030 2229 0d0a 2020 2020  0:00.000")..    
+00017210: 2020 2020 6966 206f 6e6c 794d 463a 0d0a      if onlyMF:..
+00017220: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00017230: 726e 206e 6574 4368 616e 6765 4d46 0d0a  rn netChangeMF..
+00017240: 2020 2020 2020 2020 6966 206c 6174 6573          if lates
+00017250: 745f 696e 7374 6461 7465 203d 3d20 6c61  t_instdate == la
+00017260: 7465 7374 5f6d 6664 6174 653a 0d0a 2020  test_mfdate:..  
+00017270: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00017280: 2028 6e65 7443 6861 6e67 654d 4620 2b20   (netChangeMF + 
+00017290: 6e65 7443 6861 6e67 6549 6e73 7429 0d0a  netChangeInst)..
+000172a0: 2020 2020 2020 2020 656c 6966 206c 6174          elif lat
+000172b0: 6573 745f 6d66 6461 7465 203d 3d20 6c61  est_mfdate == la
+000172c0: 7374 4461 794c 6173 744d 6f6e 7468 3a0d  stDayLastMonth:.
+000172d0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000172e0: 7572 6e20 6e65 7443 6861 6e67 654d 460d  urn netChangeMF.
+000172f0: 0a20 2020 2020 2020 2065 6c69 6620 6c61  .        elif la
+00017300: 7465 7374 5f69 6e73 7464 6174 6520 3d3d  test_instdate ==
+00017310: 206c 6173 7444 6179 4c61 7374 4d6f 6e74   lastDayLastMont
+00017320: 683a 0d0a 2020 2020 2020 2020 2020 2020  h:..            
+00017330: 7265 7475 726e 206e 6574 4368 616e 6765  return netChange
+00017340: 496e 7374 0d0a 2020 2020 2020 2020 656c  Inst..        el
+00017350: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00017360: 2023 2066 696e 6420 7468 6520 6c61 7465   # find the late
+00017370: 7374 2064 6174 650d 0a20 2020 2020 2020  st date..       
+00017380: 2020 2020 2069 6620 6c61 7465 7374 5f6d       if latest_m
+00017390: 6664 6174 6520 6973 206e 6f74 204e 6f6e  fdate is not Non
+000173a0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000173b0: 2020 2020 6c61 7465 7374 5f6d 6664 6174      latest_mfdat
+000173c0: 6520 3d20 504b 4461 7465 5574 696c 6974  e = PKDateUtilit
+000173d0: 6965 732e 6461 7465 4672 6f6d 596d 6453  ies.dateFromYmdS
+000173e0: 7472 696e 6728 6c61 7465 7374 5f6d 6664  tring(latest_mfd
+000173f0: 6174 652e 7370 6c69 7428 2254 2229 5b30  ate.split("T")[0
+00017400: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00017410: 6966 206c 6174 6573 745f 696e 7374 6461  if latest_instda
+00017420: 7465 2069 7320 6e6f 7420 4e6f 6e65 3a0d  te is not None:.
+00017430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017440: 206c 6174 6573 745f 696e 7374 6461 7465   latest_instdate
+00017450: 203d 2050 4b44 6174 6555 7469 6c69 7469   = PKDateUtiliti
+00017460: 6573 2e64 6174 6546 726f 6d59 6d64 5374  es.dateFromYmdSt
+00017470: 7269 6e67 286c 6174 6573 745f 696e 7374  ring(latest_inst
+00017480: 6461 7465 2e73 706c 6974 2822 5422 295b  date.split("T")[
+00017490: 305d 290d 0a20 2020 2020 2020 2020 2020  0])..           
+000174a0: 2072 6574 7572 6e20 6e65 7443 6861 6e67   return netChang
+000174b0: 654d 4620 6966 2028 286c 6174 6573 745f  eMF if ((latest_
+000174c0: 6d66 6461 7465 2069 7320 6e6f 7420 4e6f  mfdate is not No
+000174d0: 6e65 2920 616e 6420 6c61 7465 7374 5f6d  ne) and latest_m
+000174e0: 6664 6174 6520 3e20 286c 6174 6573 745f  fdate > (latest_
+000174f0: 696e 7374 6461 7465 2069 6620 6c61 7465  instdate if late
+00017500: 7374 5f69 6e73 7464 6174 6520 6973 206e  st_instdate is n
+00017510: 6f74 204e 6f6e 6520 656c 7365 2028 6c61  ot None else (la
+00017520: 7465 7374 5f6d 6664 6174 6520 2d20 6461  test_mfdate - da
+00017530: 7465 7469 6d65 2e74 696d 6564 656c 7461  tetime.timedelta
+00017540: 2831 2929 2929 2065 6c73 6520 6e65 7443  (1)))) else netC
+00017550: 6861 6e67 6549 6e73 740d 0a0d 0a20 2020  hangeInst....   
+00017560: 2064 6566 2067 6574 4672 6573 684d 4649   def getFreshMFI
+00017570: 5374 6174 7573 2873 656c 662c 2073 746f  Status(self, sto
+00017580: 636b 2c65 7863 6861 6e67 654e 616d 653d  ck,exchangeName=
+00017590: 2249 4e44 4941 2229 3a0d 0a20 2020 2020  "INDIA"):..     
+000175a0: 2020 2063 6861 6e67 6553 7461 7475 7344     changeStatusD
+000175b0: 6174 614d 4620 3d20 4e6f 6e65 0d0a 2020  ataMF = None..  
+000175c0: 2020 2020 2020 6368 616e 6765 5374 6174        changeStat
+000175d0: 7573 4461 7461 496e 7374 203d 204e 6f6e  usDataInst = Non
+000175e0: 650d 0a20 2020 2020 2020 206e 6574 4368  e..        netCh
+000175f0: 616e 6765 4d46 203d 2030 0d0a 2020 2020  angeMF = 0..    
+00017600: 2020 2020 6e65 7443 6861 6e67 6549 6e73      netChangeIns
+00017610: 7420 3d20 300d 0a20 2020 2020 2020 206c  t = 0..        l
+00017620: 6174 6573 745f 6d66 6461 7465 203d 204e  atest_mfdate = N
+00017630: 6f6e 650d 0a20 2020 2020 2020 206c 6174  one..        lat
+00017640: 6573 745f 696e 7374 6461 7465 203d 204e  est_instdate = N
+00017650: 6f6e 650d 0a20 2020 2020 2020 2073 6563  one..        sec
+00017660: 7572 6974 7920 3d20 4e6f 6e65 0d0a 2020  urity = None..  
+00017670: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
+00017680: 2020 2020 2020 2020 7769 7468 2053 7570          with Sup
+00017690: 7072 6573 734f 7574 7075 7428 7375 7070  pressOutput(supp
+000176a0: 7265 7373 5f73 7464 6572 723d 5472 7565  ress_stderr=True
+000176b0: 2c20 7375 7070 7265 7373 5f73 7464 6f75  , suppress_stdou
+000176c0: 743d 5472 7565 293a 0d0a 2020 2020 2020  t=True):..      
+000176d0: 2020 2020 2020 2020 2020 7365 6375 7269            securi
+000176e0: 7479 203d 2053 746f 636b 2873 746f 636b  ty = Stock(stock
+000176f0: 2c65 7863 6861 6e67 653d 6578 6368 616e  ,exchange=exchan
+00017700: 6765 4e61 6d65 290d 0a20 2020 2020 2020  geName)..       
+00017710: 2065 7863 6570 7420 5661 6c75 6545 7272   except ValueErr
+00017720: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
+00017730: 2023 2057 6520 6469 6420 6e6f 7420 6669   # We did not fi
+00017740: 6e64 2074 6865 2073 746f 636b 3f20 4974  nd the stock? It
+00017750: 2773 206f 6b61 792e 204d 6f76 6520 6f6e  's okay. Move on
+00017760: 2074 6f20 7468 6520 6e65 7874 206f 6e65   to the next one
+00017770: 2e0d 0a20 2020 2020 2020 2020 2020 2070  ...            p
+00017780: 6173 730d 0a20 2020 2020 2020 2069 6620  ass..        if 
+00017790: 7365 6375 7269 7479 2069 7320 6e6f 7420  security is not 
+000177a0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+000177b0: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
+000177c0: 2020 2020 2020 2020 2077 6974 6820 5375           with Su
+000177d0: 7070 7265 7373 4f75 7470 7574 2873 7570  ppressOutput(sup
+000177e0: 7072 6573 735f 7374 6465 7272 3d54 7275  press_stderr=Tru
+000177f0: 652c 2073 7570 7072 6573 735f 7374 646f  e, suppress_stdo
+00017800: 7574 3d54 7275 6529 3a0d 0a20 2020 2020  ut=True):..     
+00017810: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00017820: 6861 6e67 6553 7461 7475 7352 6f77 734d  hangeStatusRowsM
+00017830: 4620 3d20 7365 6375 7269 7479 2e6d 7574  F = security.mut
+00017840: 7561 6c46 756e 644f 776e 6572 7368 6970  ualFundOwnership
+00017850: 2874 6f70 3d35 290d 0a20 2020 2020 2020  (top=5)..       
+00017860: 2020 2020 2020 2020 2020 2020 2063 6861               cha
+00017870: 6e67 6553 7461 7475 7352 6f77 7349 6e73  ngeStatusRowsIns
+00017880: 7420 3d20 7365 6375 7269 7479 2e69 6e73  t = security.ins
+00017890: 7469 7475 7469 6f6e 4f77 6e65 7273 6869  titutionOwnershi
+000178a0: 7028 746f 703d 3529 0d0a 2020 2020 2020  p(top=5)..      
+000178b0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
+000178c0: 616e 6765 5374 6174 7573 4461 7461 4d46  angeStatusDataMF
+000178d0: 203d 2073 6563 7572 6974 792e 6d75 7475   = security.mutu
+000178e0: 616c 4675 6e64 4649 4943 6861 6e67 6544  alFundFIIChangeD
+000178f0: 6174 6128 6368 616e 6765 5374 6174 7573  ata(changeStatus
+00017900: 526f 7773 4d46 290d 0a20 2020 2020 2020  RowsMF)..       
+00017910: 2020 2020 2020 2020 2020 2020 2063 6861               cha
+00017920: 6e67 6553 7461 7475 7344 6174 6149 6e73  ngeStatusDataIns
+00017930: 7420 3d20 7365 6375 7269 7479 2e6d 7574  t = security.mut
+00017940: 7561 6c46 756e 6446 4949 4368 616e 6765  ualFundFIIChange
+00017950: 4461 7461 2863 6861 6e67 6553 7461 7475  Data(changeStatu
+00017960: 7352 6f77 7349 6e73 7429 0d0a 2020 2020  sRowsInst)..    
+00017970: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+00017980: 7863 6570 7469 6f6e 2061 7320 653a 0d0a  xception as e:..
+00017990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000179a0: 7365 6c66 2e64 6566 6175 6c74 5f6c 6f67  self.default_log
+000179b0: 6765 722e 6465 6275 6728 652c 2065 7863  ger.debug(e, exc
+000179c0: 5f69 6e66 6f3d 5472 7565 290d 0a20 2020  _info=True)..   
+000179d0: 2020 2020 2020 2020 2020 2020 2023 2054               # T
+000179e0: 7970 6545 7272 6f72 206f 7220 436f 6e6e  ypeError or Conn
+000179f0: 6563 7469 6f6e 4572 726f 7220 6265 6361  ectionError beca
+00017a00: 7573 6520 7765 2063 6f75 6c64 206e 6f74  use we could not
+00017a10: 2066 696e 6420 7468 6520 7374 6f63 6b20   find the stock 
+00017a20: 6f72 204d 4649 2064 6174 6120 6973 6e27  or MFI data isn'
+00017a30: 7420 6176 6169 6c61 626c 653f 0d0a 2020  t available?..  
+00017a40: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00017a50: 7373 0d0a 2020 2020 2020 2020 2020 2020  ss..            
+00017a60: 6c61 7374 4461 794c 6173 744d 6f6e 7468  lastDayLastMonth
+00017a70: 203d 2050 4b44 6174 6555 7469 6c69 7469   = PKDateUtiliti
+00017a80: 6573 2e6c 6173 745f 6461 795f 6f66 5f70  es.last_day_of_p
+00017a90: 7265 7669 6f75 735f 6d6f 6e74 6828 504b  revious_month(PK
+00017aa0: 4461 7465 5574 696c 6974 6965 732e 6375  DateUtilities.cu
+00017ab0: 7272 656e 7444 6174 6554 696d 6528 2929  rrentDateTime())
+00017ac0: 0d0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
+00017ad0: 7374 4461 794c 6173 744d 6f6e 7468 203d  stDayLastMonth =
+00017ae0: 206c 6173 7444 6179 4c61 7374 4d6f 6e74   lastDayLastMont
+00017af0: 682e 7374 7266 7469 6d65 2822 2559 2d25  h.strftime("%Y-%
+00017b00: 6d2d 2564 5430 303a 3030 3a30 302e 3030  m-%dT00:00:00.00
+00017b10: 3022 290d 0a20 2020 2020 2020 2020 2020  0")..           
+00017b20: 2069 6620 6368 616e 6765 5374 6174 7573   if changeStatus
+00017b30: 4461 7461 4d46 2069 7320 6e6f 7420 4e6f  DataMF is not No
+00017b40: 6e65 2061 6e64 206c 656e 2863 6861 6e67  ne and len(chang
+00017b50: 6553 7461 7475 7344 6174 614d 4629 203e  eStatusDataMF) >
+00017b60: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
+00017b70: 2020 2020 2064 665f 6772 6f75 7065 644d       df_groupedM
+00017b80: 4620 3d20 6368 616e 6765 5374 6174 7573  F = changeStatus
+00017b90: 4461 7461 4d46 2e67 726f 7570 6279 2822  DataMF.groupby("
+00017ba0: 6461 7465 222c 2073 6f72 743d 4661 6c73  date", sort=Fals
+00017bb0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00017bc0: 2020 2020 666f 7220 6d66 6461 7465 2c20      for mfdate, 
+00017bd0: 6466 5f67 726f 7570 4d46 2069 6e20 6466  df_groupMF in df
+00017be0: 5f67 726f 7570 6564 4d46 3a0d 0a20 2020  _groupedMF:..   
+00017bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c00: 206e 6574 4368 616e 6765 4d46 203d 2064   netChangeMF = d
+00017c10: 665f 6772 6f75 704d 465b 2263 6861 6e67  f_groupMF["chang
+00017c20: 6541 6d6f 756e 7422 5d2e 7375 6d28 290d  eAmount"].sum().
+00017c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017c40: 2020 2020 206c 6174 6573 745f 6d66 6461       latest_mfda
+00017c50: 7465 203d 206d 6664 6174 650d 0a20 2020  te = mfdate..   
 00017c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c70: 6272 6561 6b0d 0a20 2020 2020 2020 2072  break..        r
-00017c80: 6574 7572 6e20 6e65 7443 6861 6e67 654d  eturn netChangeM
-00017c90: 462c 6e65 7443 6861 6e67 6549 6e73 742c  F,netChangeInst,
-00017ca0: 6c61 7465 7374 5f6d 6664 6174 652c 6c61  latest_mfdate,la
-00017cb0: 7465 7374 5f69 6e73 7464 6174 650d 0a0d  test_instdate...
-00017cc0: 0a0d 0a20 2020 2064 6566 2067 6574 4e69  ...    def getNi
-00017cd0: 6674 7950 7265 6469 6374 696f 6e28 7365  ftyPrediction(se
-00017ce0: 6c66 2c20 6466 293a 0d0a 2020 2020 2020  lf, df):..      
-00017cf0: 2020 696d 706f 7274 2077 6172 6e69 6e67    import warning
-00017d00: 730d 0a0d 0a20 2020 2020 2020 2077 6172  s....        war
-00017d10: 6e69 6e67 732e 6669 6c74 6572 7761 726e  nings.filterwarn
-00017d20: 696e 6773 2822 6967 6e6f 7265 2229 0d0a  ings("ignore")..
-00017d30: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-00017d40: 662e 636f 7079 2829 0d0a 2020 2020 2020  f.copy()..      
-00017d50: 2020 6d6f 6465 6c2c 2070 6b6c 203d 2055    model, pkl = U
-00017d60: 7469 6c69 7479 2e74 6f6f 6c73 2e67 6574  tility.tools.get
-00017d70: 4e69 6674 794d 6f64 656c 2829 0d0a 2020  NiftyModel()..  
-00017d80: 2020 2020 2020 6966 206d 6f64 656c 2069        if model i
-00017d90: 7320 4e6f 6e65 206f 7220 706b 6c20 6973  s None or pkl is
-00017da0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00017db0: 2020 2020 7265 7475 726e 2030 2c20 2255      return 0, "U
-00017dc0: 6e6b 6e6f 776e 222c 2022 556e 6b6e 6f77  nknown", "Unknow
-00017dd0: 6e22 0d0a 2020 2020 2020 2020 7769 7468  n"..        with
-00017de0: 2053 7570 7072 6573 734f 7574 7075 7428   SuppressOutput(
-00017df0: 7375 7070 7265 7373 5f73 7464 6572 723d  suppress_stderr=
-00017e00: 5472 7565 2c20 7375 7070 7265 7373 5f73  True, suppress_s
-00017e10: 7464 6f75 743d 5472 7565 293a 0d0a 2020  tdout=True):..  
-00017e20: 2020 2020 2020 2020 2020 6461 7461 203d            data =
-00017e30: 2064 6174 615b 706b 6c5b 2263 6f6c 756d   data[pkl["colum
-00017e40: 6e73 225d 5d0d 0a20 2020 2020 2020 2020  ns"]]..         
-00017e50: 2020 2023 2323 2076 3220 5072 6570 726f     ### v2 Prepro
-00017e60: 6365 7373 696e 670d 0a20 2020 2020 2020  cessing..       
-00017e70: 2020 2020 2064 6174 615b 2248 6967 6822       data["High"
-00017e80: 5d20 3d20 6461 7461 5b22 4869 6768 225d  ] = data["High"]
-00017e90: 2e70 6374 5f63 6861 6e67 6528 2920 2a20  .pct_change() * 
-00017ea0: 3130 300d 0a20 2020 2020 2020 2020 2020  100..           
-00017eb0: 2064 6174 615b 224c 6f77 225d 203d 2064   data["Low"] = d
-00017ec0: 6174 615b 224c 6f77 225d 2e70 6374 5f63  ata["Low"].pct_c
-00017ed0: 6861 6e67 6528 2920 2a20 3130 300d 0a20  hange() * 100.. 
-00017ee0: 2020 2020 2020 2020 2020 2064 6174 615b             data[
-00017ef0: 224f 7065 6e22 5d20 3d20 6461 7461 5b22  "Open"] = data["
-00017f00: 4f70 656e 225d 2e70 6374 5f63 6861 6e67  Open"].pct_chang
-00017f10: 6528 2920 2a20 3130 300d 0a20 2020 2020  e() * 100..     
-00017f20: 2020 2020 2020 2064 6174 615b 2243 6c6f         data["Clo
-00017f30: 7365 225d 203d 2064 6174 615b 2243 6c6f  se"] = data["Clo
-00017f40: 7365 225d 2e70 6374 5f63 6861 6e67 6528  se"].pct_change(
-00017f50: 2920 2a20 3130 300d 0a20 2020 2020 2020  ) * 100..       
-00017f60: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
-00017f70: 2e69 6c6f 635b 2d31 5d0d 0a20 2020 2020  .iloc[-1]..     
-00017f80: 2020 2020 2020 2023 2323 0d0a 2020 2020         ###..    
-00017f90: 2020 2020 2020 2020 6461 7461 203d 2070          data = p
-00017fa0: 6b6c 5b22 7363 616c 6572 225d 2e74 7261  kl["scaler"].tra
-00017fb0: 6e73 666f 726d 285b 6461 7461 5d29 0d0a  nsform([data])..
-00017fc0: 2020 2020 2020 2020 2020 2020 7769 7468              with
-00017fd0: 2053 7570 7072 6573 734f 7574 7075 7428   SuppressOutput(
-00017fe0: 7375 7070 7265 7373 5f73 7464 6f75 743d  suppress_stdout=
-00017ff0: 5472 7565 2c20 7375 7070 7265 7373 5f73  True, suppress_s
-00018000: 7464 6572 723d 5472 7565 293a 0d0a 2020  tderr=True):..  
-00018010: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00018020: 6564 203d 206d 6f64 656c 2e70 7265 6469  ed = model.predi
-00018030: 6374 2864 6174 6129 5b30 5d0d 0a20 2020  ct(data)[0]..   
-00018040: 2020 2020 2069 6620 7072 6564 203e 2030       if pred > 0
-00018050: 2e35 3a0d 0a20 2020 2020 2020 2020 2020  .5:..           
-00018060: 206f 7574 5465 7874 203d 2022 4245 4152   outText = "BEAR
-00018070: 4953 4822 0d0a 2020 2020 2020 2020 2020  ISH"..          
-00018080: 2020 6f75 7420 3d20 280d 0a20 2020 2020    out = (..     
-00018090: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
-000180a0: 5465 7874 2e42 4f4c 440d 0a20 2020 2020  Text.BOLD..     
-000180b0: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-000180c0: 6f72 5465 7874 2e46 4149 4c0d 0a20 2020  orText.FAIL..   
-000180d0: 2020 2020 2020 2020 2020 2020 202b 206f               + o
-000180e0: 7574 5465 7874 0d0a 2020 2020 2020 2020  utText..        
-000180f0: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
-00018100: 6578 742e 454e 440d 0a20 2020 2020 2020  ext.END..       
-00018110: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
-00018120: 5465 7874 2e42 4f4c 440d 0a20 2020 2020  Text.BOLD..     
-00018130: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00018140: 2020 2020 2020 7375 6720 3d20 2248 6f6c        sug = "Hol
-00018150: 6420 796f 7572 2053 686f 7274 2070 6f73  d your Short pos
-00018160: 6974 696f 6e21 220d 0a20 2020 2020 2020  ition!"..       
-00018170: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00018180: 2020 2020 6f75 7454 6578 7420 3d20 2242      outText = "B
-00018190: 554c 4c49 5348 220d 0a20 2020 2020 2020  ULLISH"..       
-000181a0: 2020 2020 206f 7574 203d 2028 0d0a 2020       out = (..  
-000181b0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-000181c0: 6c6f 7254 6578 742e 424f 4c44 0d0a 2020  lorText.BOLD..  
-000181d0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-000181e0: 636f 6c6f 7254 6578 742e 4752 4545 4e0d  colorText.GREEN.
-000181f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018200: 202b 206f 7574 5465 7874 0d0a 2020 2020   + outText..    
-00018210: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
-00018220: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
-00018230: 2020 2020 2020 2020 2020 2020 202b 2063               + c
-00018240: 6f6c 6f72 5465 7874 2e42 4f4c 440d 0a20  olorText.BOLD.. 
-00018250: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
-00018260: 2020 2020 2020 2020 2020 7375 6720 3d20            sug = 
-00018270: 2253 7461 7920 4275 6c6c 6973 6821 220d  "Stay Bullish!".
-00018280: 0a20 2020 2020 2020 2069 6620 504b 4461  .        if PKDa
-00018290: 7465 5574 696c 6974 6965 732e 6973 436c  teUtilities.isCl
-000182a0: 6f73 696e 6748 6f75 7228 293a 0d0a 2020  osingHour():..  
-000182b0: 2020 2020 2020 2020 2020 4f75 7470 7574            Output
-000182c0: 436f 6e74 726f 6c73 2829 2e70 7269 6e74  Controls().print
-000182d0: 4f75 7470 7574 280d 0a20 2020 2020 2020  Output(..       
-000182e0: 2020 2020 2020 2020 2063 6f6c 6f72 5465           colorTe
-000182f0: 7874 2e42 4f4c 440d 0a20 2020 2020 2020  xt.BOLD..       
-00018300: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
-00018310: 5465 7874 2e57 4152 4e0d 0a20 2020 2020  Text.WARN..     
-00018320: 2020 2020 2020 2020 2020 202b 2022 4e6f             + "No
-00018330: 7465 3a20 5468 6520 4149 2070 7265 6469  te: The AI predi
-00018340: 6374 696f 6e20 7368 6f75 6c64 2062 6520  ction should be 
-00018350: 6578 6563 7574 6564 2041 6674 6572 2033  executed After 3
-00018360: 2050 4d20 6f72 204e 6561 7220 746f 2043   PM or Near to C
-00018370: 6c6f 7369 6e67 2074 696d 6520 6173 2074  losing time as t
-00018380: 6865 2050 7265 6469 6374 696f 6e20 4163  he Prediction Ac
-00018390: 6375 7261 6379 2069 7320 6261 7365 6420  curacy is based 
-000183a0: 6f6e 2074 6865 2043 6c6f 7369 6e67 2070  on the Closing p
-000183b0: 7269 6365 2122 0d0a 2020 2020 2020 2020  rice!"..        
-000183c0: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
-000183d0: 6578 742e 454e 440d 0a20 2020 2020 2020  ext.END..       
-000183e0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-000183f0: 7072 6564 6963 7469 6f6e 5465 7874 203d  predictionText =
-00018400: 2022 4d61 726b 6574 206d 6179 204f 7065   "Market may Ope
-00018410: 6e20 7b7d 206e 6578 7420 6461 7921 207b  n {} next day! {
-00018420: 7d22 2e66 6f72 6d61 7428 6f75 742c 2073  }".format(out, s
-00018430: 7567 290d 0a20 2020 2020 2020 2073 7472  ug)..        str
-00018440: 656e 6774 6854 6578 7420 3d20 2250 726f  engthText = "Pro
-00018450: 6261 6269 6c69 7479 2f53 7472 656e 6774  bability/Strengt
-00018460: 6820 6f66 2050 7265 6469 6374 696f 6e20  h of Prediction 
-00018470: 3d20 7b7d 2522 2e66 6f72 6d61 7428 0d0a  = {}%".format(..
-00018480: 2020 2020 2020 2020 2020 2020 5574 696c              Util
-00018490: 6974 792e 746f 6f6c 732e 6765 7453 6967  ity.tools.getSig
-000184a0: 6d6f 6964 436f 6e66 6964 656e 6365 2870  moidConfidence(p
-000184b0: 7265 645b 305d 290d 0a20 2020 2020 2020  red[0])..       
-000184c0: 2029 0d0a 2020 2020 2020 2020 4f75 7470   )..        Outp
+00017c70: 2062 7265 616b 0d0a 2020 2020 2020 2020   break..        
+00017c80: 2020 2020 6966 2063 6861 6e67 6553 7461      if changeSta
+00017c90: 7475 7344 6174 6149 6e73 7420 6973 206e  tusDataInst is n
+00017ca0: 6f74 204e 6f6e 6520 616e 6420 6c65 6e28  ot None and len(
+00017cb0: 6368 616e 6765 5374 6174 7573 4461 7461  changeStatusData
+00017cc0: 496e 7374 2920 3e20 303a 0d0a 2020 2020  Inst) > 0:..    
+00017cd0: 2020 2020 2020 2020 2020 2020 6466 5f67              df_g
+00017ce0: 726f 7570 6564 496e 7374 203d 2063 6861  roupedInst = cha
+00017cf0: 6e67 6553 7461 7475 7344 6174 6149 6e73  ngeStatusDataIns
+00017d00: 742e 6772 6f75 7062 7928 2264 6174 6522  t.groupby("date"
+00017d10: 2c20 736f 7274 3d46 616c 7365 290d 0a20  , sort=False).. 
+00017d20: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00017d30: 6f72 2069 6e73 7464 6174 652c 2064 665f  or instdate, df_
+00017d40: 6772 6f75 7049 6e73 7420 696e 2064 665f  groupInst in df_
+00017d50: 6772 6f75 7065 6449 6e73 743a 0d0a 2020  groupedInst:..  
+00017d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d70: 2020 6966 2028 6c61 7465 7374 5f6d 6664    if (latest_mfd
+00017d80: 6174 6520 6973 206e 6f74 204e 6f6e 6520  ate is not None 
+00017d90: 616e 6420 6c61 7465 7374 5f6d 6664 6174  and latest_mfdat
+00017da0: 6520 3d3d 2069 6e73 7464 6174 6529 206f  e == instdate) o
+00017db0: 7220 286c 6174 6573 745f 6d66 6461 7465  r (latest_mfdate
+00017dc0: 2069 7320 4e6f 6e65 2920 6f72 2028 696e   is None) or (in
+00017dd0: 7374 6461 7465 203d 3d20 6c61 7374 4461  stdate == lastDa
+00017de0: 794c 6173 744d 6f6e 7468 293a 0d0a 2020  yLastMonth):..  
+00017df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e00: 2020 2020 2020 6e65 7443 6861 6e67 6549        netChangeI
+00017e10: 6e73 7420 3d20 6466 5f67 726f 7570 496e  nst = df_groupIn
+00017e20: 7374 5b22 6368 616e 6765 416d 6f75 6e74  st["changeAmount
+00017e30: 225d 2e73 756d 2829 0d0a 2020 2020 2020  "].sum()..      
+00017e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e50: 2020 6c61 7465 7374 5f69 6e73 7464 6174    latest_instdat
+00017e60: 6520 3d20 696e 7374 6461 7465 0d0a 2020  e = instdate..  
+00017e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e80: 2020 6272 6561 6b0d 0a20 2020 2020 2020    break..       
+00017e90: 2072 6574 7572 6e20 6e65 7443 6861 6e67   return netChang
+00017ea0: 654d 462c 6e65 7443 6861 6e67 6549 6e73  eMF,netChangeIns
+00017eb0: 742c 6c61 7465 7374 5f6d 6664 6174 652c  t,latest_mfdate,
+00017ec0: 6c61 7465 7374 5f69 6e73 7464 6174 650d  latest_instdate.
+00017ed0: 0a0d 0a0d 0a20 2020 2064 6566 2067 6574  .....    def get
+00017ee0: 4e69 6674 7950 7265 6469 6374 696f 6e28  NiftyPrediction(
+00017ef0: 7365 6c66 2c20 6466 293a 0d0a 2020 2020  self, df):..    
+00017f00: 2020 2020 696d 706f 7274 2077 6172 6e69      import warni
+00017f10: 6e67 730d 0a0d 0a20 2020 2020 2020 2077  ngs....        w
+00017f20: 6172 6e69 6e67 732e 6669 6c74 6572 7761  arnings.filterwa
+00017f30: 726e 696e 6773 2822 6967 6e6f 7265 2229  rnings("ignore")
+00017f40: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
+00017f50: 2064 662e 636f 7079 2829 0d0a 2020 2020   df.copy()..    
+00017f60: 2020 2020 6d6f 6465 6c2c 2070 6b6c 203d      model, pkl =
+00017f70: 2055 7469 6c69 7479 2e74 6f6f 6c73 2e67   Utility.tools.g
+00017f80: 6574 4e69 6674 794d 6f64 656c 2829 0d0a  etNiftyModel()..
+00017f90: 2020 2020 2020 2020 6966 206d 6f64 656c          if model
+00017fa0: 2069 7320 4e6f 6e65 206f 7220 706b 6c20   is None or pkl 
+00017fb0: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
+00017fc0: 2020 2020 2020 7265 7475 726e 2030 2c20        return 0, 
+00017fd0: 2255 6e6b 6e6f 776e 222c 2022 556e 6b6e  "Unknown", "Unkn
+00017fe0: 6f77 6e22 0d0a 2020 2020 2020 2020 7769  own"..        wi
+00017ff0: 7468 2053 7570 7072 6573 734f 7574 7075  th SuppressOutpu
+00018000: 7428 7375 7070 7265 7373 5f73 7464 6572  t(suppress_stder
+00018010: 723d 5472 7565 2c20 7375 7070 7265 7373  r=True, suppress
+00018020: 5f73 7464 6f75 743d 5472 7565 293a 0d0a  _stdout=True):..
+00018030: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00018040: 203d 2064 6174 615b 706b 6c5b 2263 6f6c   = data[pkl["col
+00018050: 756d 6e73 225d 5d0d 0a20 2020 2020 2020  umns"]]..       
+00018060: 2020 2020 2023 2323 2076 3220 5072 6570       ### v2 Prep
+00018070: 726f 6365 7373 696e 670d 0a20 2020 2020  rocessing..     
+00018080: 2020 2020 2020 2064 6174 615b 2248 6967         data["Hig
+00018090: 6822 5d20 3d20 6461 7461 5b22 4869 6768  h"] = data["High
+000180a0: 225d 2e70 6374 5f63 6861 6e67 6528 2920  "].pct_change() 
+000180b0: 2a20 3130 300d 0a20 2020 2020 2020 2020  * 100..         
+000180c0: 2020 2064 6174 615b 224c 6f77 225d 203d     data["Low"] =
+000180d0: 2064 6174 615b 224c 6f77 225d 2e70 6374   data["Low"].pct
+000180e0: 5f63 6861 6e67 6528 2920 2a20 3130 300d  _change() * 100.
+000180f0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+00018100: 615b 224f 7065 6e22 5d20 3d20 6461 7461  a["Open"] = data
+00018110: 5b22 4f70 656e 225d 2e70 6374 5f63 6861  ["Open"].pct_cha
+00018120: 6e67 6528 2920 2a20 3130 300d 0a20 2020  nge() * 100..   
+00018130: 2020 2020 2020 2020 2064 6174 615b 2243           data["C
+00018140: 6c6f 7365 225d 203d 2064 6174 615b 2243  lose"] = data["C
+00018150: 6c6f 7365 225d 2e70 6374 5f63 6861 6e67  lose"].pct_chang
+00018160: 6528 2920 2a20 3130 300d 0a20 2020 2020  e() * 100..     
+00018170: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
+00018180: 7461 2e69 6c6f 635b 2d31 5d0d 0a20 2020  ta.iloc[-1]..   
+00018190: 2020 2020 2020 2020 2023 2323 0d0a 2020           ###..  
+000181a0: 2020 2020 2020 2020 2020 6461 7461 203d            data =
+000181b0: 2070 6b6c 5b22 7363 616c 6572 225d 2e74   pkl["scaler"].t
+000181c0: 7261 6e73 666f 726d 285b 6461 7461 5d29  ransform([data])
+000181d0: 0d0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
+000181e0: 7468 2053 7570 7072 6573 734f 7574 7075  th SuppressOutpu
+000181f0: 7428 7375 7070 7265 7373 5f73 7464 6f75  t(suppress_stdou
+00018200: 743d 5472 7565 2c20 7375 7070 7265 7373  t=True, suppress
+00018210: 5f73 7464 6572 723d 5472 7565 293a 0d0a  _stderr=True):..
+00018220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018230: 7072 6564 203d 206d 6f64 656c 2e70 7265  pred = model.pre
+00018240: 6469 6374 2864 6174 6129 5b30 5d0d 0a20  dict(data)[0].. 
+00018250: 2020 2020 2020 2069 6620 7072 6564 203e         if pred >
+00018260: 2030 2e35 3a0d 0a20 2020 2020 2020 2020   0.5:..         
+00018270: 2020 206f 7574 5465 7874 203d 2022 4245     outText = "BE
+00018280: 4152 4953 4822 0d0a 2020 2020 2020 2020  ARISH"..        
+00018290: 2020 2020 6f75 7420 3d20 280d 0a20 2020      out = (..   
+000182a0: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
+000182b0: 6f72 5465 7874 2e42 4f4c 440d 0a20 2020  orText.BOLD..   
+000182c0: 2020 2020 2020 2020 2020 2020 202b 2063               + c
+000182d0: 6f6c 6f72 5465 7874 2e46 4149 4c0d 0a20  olorText.FAIL.. 
+000182e0: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+000182f0: 206f 7574 5465 7874 0d0a 2020 2020 2020   outText..      
+00018300: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
+00018310: 7254 6578 742e 454e 440d 0a20 2020 2020  rText.END..     
+00018320: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
+00018330: 6f72 5465 7874 2e42 4f4c 440d 0a20 2020  orText.BOLD..   
+00018340: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
+00018350: 2020 2020 2020 2020 7375 6720 3d20 2248          sug = "H
+00018360: 6f6c 6420 796f 7572 2053 686f 7274 2070  old your Short p
+00018370: 6f73 6974 696f 6e21 220d 0a20 2020 2020  osition!"..     
+00018380: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00018390: 2020 2020 2020 6f75 7454 6578 7420 3d20        outText = 
+000183a0: 2242 554c 4c49 5348 220d 0a20 2020 2020  "BULLISH"..     
+000183b0: 2020 2020 2020 206f 7574 203d 2028 0d0a         out = (..
+000183c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000183d0: 636f 6c6f 7254 6578 742e 424f 4c44 0d0a  colorText.BOLD..
+000183e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000183f0: 2b20 636f 6c6f 7254 6578 742e 4752 4545  + colorText.GREE
+00018400: 4e0d 0a20 2020 2020 2020 2020 2020 2020  N..             
+00018410: 2020 202b 206f 7574 5465 7874 0d0a 2020     + outText..  
+00018420: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+00018430: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
+00018440: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+00018450: 2063 6f6c 6f72 5465 7874 2e42 4f4c 440d   colorText.BOLD.
+00018460: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
+00018470: 2020 2020 2020 2020 2020 2020 7375 6720              sug 
+00018480: 3d20 2253 7461 7920 4275 6c6c 6973 6821  = "Stay Bullish!
+00018490: 220d 0a20 2020 2020 2020 2069 6620 504b  "..        if PK
+000184a0: 4461 7465 5574 696c 6974 6965 732e 6973  DateUtilities.is
+000184b0: 436c 6f73 696e 6748 6f75 7228 293a 0d0a  ClosingHour():..
+000184c0: 2020 2020 2020 2020 2020 2020 4f75 7470              Outp
 000184d0: 7574 436f 6e74 726f 6c73 2829 2e70 7269  utControls().pri
 000184e0: 6e74 4f75 7470 7574 280d 0a20 2020 2020  ntOutput(..     
-000184f0: 2020 2020 2020 2063 6f6c 6f72 5465 7874         colorText
-00018500: 2e42 4f4c 440d 0a20 2020 2020 2020 2020  .BOLD..         
-00018510: 2020 202b 2063 6f6c 6f72 5465 7874 2e42     + colorText.B
-00018520: 4c55 450d 0a20 2020 2020 2020 2020 2020  LUE..           
-00018530: 202b 2022 5c6e 220d 0a20 2020 2020 2020   + "\n"..       
-00018540: 2020 2020 202b 2022 5b2b 5d20 4e69 6674       + "[+] Nift
-00018550: 7920 4149 2050 7265 6469 6374 696f 6e20  y AI Prediction 
-00018560: 2d3e 2022 0d0a 2020 2020 2020 2020 2020  -> "..          
-00018570: 2020 2b20 636f 6c6f 7254 6578 742e 454e    + colorText.EN
-00018580: 440d 0a20 2020 2020 2020 2020 2020 202b  D..            +
-00018590: 2063 6f6c 6f72 5465 7874 2e42 4f4c 440d   colorText.BOLD.
-000185a0: 0a20 2020 2020 2020 2020 2020 202b 2070  .            + p
-000185b0: 7265 6469 6374 696f 6e54 6578 740d 0a20  redictionText.. 
-000185c0: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-000185d0: 6f72 5465 7874 2e45 4e44 0d0a 2020 2020  orText.END..    
-000185e0: 2020 2020 290d 0a20 2020 2020 2020 204f      )..        O
-000185f0: 7574 7075 7443 6f6e 7472 6f6c 7328 292e  utputControls().
-00018600: 7072 696e 744f 7574 7075 7428 0d0a 2020  printOutput(..  
-00018610: 2020 2020 2020 2020 2020 636f 6c6f 7254            colorT
-00018620: 6578 742e 424f 4c44 0d0a 2020 2020 2020  ext.BOLD..      
-00018630: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
-00018640: 742e 424c 5545 0d0a 2020 2020 2020 2020  t.BLUE..        
-00018650: 2020 2020 2b20 225c 6e22 0d0a 2020 2020      + "\n"..    
-00018660: 2020 2020 2020 2020 2b20 225b 2b5d 204e          + "[+] N
-00018670: 6966 7479 2041 4920 5072 6564 6963 7469  ifty AI Predicti
-00018680: 6f6e 202d 3e20 220d 0a20 2020 2020 2020  on -> "..       
-00018690: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-000186a0: 2e45 4e44 0d0a 2020 2020 2020 2020 2020  .END..          
-000186b0: 2020 2b20 7374 7265 6e67 7468 5465 7874    + strengthText
-000186c0: 0d0a 2020 2020 2020 2020 290d 0a0d 0a20  ..        ).... 
-000186d0: 2020 2020 2020 2072 6574 7572 6e20 7072         return pr
-000186e0: 6564 2c20 7072 6564 6963 7469 6f6e 5465  ed, predictionTe
-000186f0: 7874 2e72 6570 6c61 6365 286f 7574 2c20  xt.replace(out, 
-00018700: 6f75 7454 6578 7429 2c20 7374 7265 6e67  outText), streng
-00018710: 7468 5465 7874 0d0a 0d0a 2020 2020 6465  thText....    de
-00018720: 6620 6d6f 6e69 746f 7246 6976 6545 6d61  f monitorFiveEma
-00018730: 2873 656c 662c 2066 6574 6368 6572 2c20  (self, fetcher, 
-00018740: 7265 7375 6c74 5f64 662c 206c 6173 745f  result_df, last_
-00018750: 7369 676e 616c 2c20 7269 736b 5f72 6577  signal, risk_rew
-00018760: 6172 643d 3329 3a0d 0a20 2020 2020 2020  ard=3):..       
-00018770: 2063 6f6c 5f6e 616d 6573 203d 205b 2248   col_names = ["H
-00018780: 6967 6822 2c20 224c 6f77 222c 2022 436c  igh", "Low", "Cl
-00018790: 6f73 6522 2c20 2235 454d 4122 5d0d 0a20  ose", "5EMA"].. 
-000187a0: 2020 2020 2020 2064 6174 615f 6c69 7374         data_list
-000187b0: 203d 205b 226e 6966 7479 5f62 7579 222c   = ["nifty_buy",
-000187c0: 2022 6261 6e6b 6e69 6674 795f 6275 7922   "banknifty_buy"
-000187d0: 2c20 226e 6966 7479 5f73 656c 6c22 2c20  , "nifty_sell", 
-000187e0: 2262 616e 6b6e 6966 7479 5f73 656c 6c22  "banknifty_sell"
-000187f0: 5d0d 0a0d 0a20 2020 2020 2020 2064 6174  ]....        dat
-00018800: 615f 7475 706c 6520 3d20 6665 7463 6865  a_tuple = fetche
-00018810: 722e 6665 7463 6846 6976 6545 6d61 4461  r.fetchFiveEmaDa
-00018820: 7461 2829 0d0a 2020 2020 2020 2020 666f  ta()..        fo
-00018830: 7220 636e 7420 696e 2072 616e 6765 286c  r cnt in range(l
-00018840: 656e 2864 6174 615f 7475 706c 6529 293a  en(data_tuple)):
-00018850: 0d0a 2020 2020 2020 2020 2020 2020 6420  ..            d 
-00018860: 3d20 6461 7461 5f74 7570 6c65 5b63 6e74  = data_tuple[cnt
-00018870: 5d0d 0a20 2020 2020 2020 2020 2020 2064  ]..            d
-00018880: 5b22 3545 4d41 225d 203d 2070 6b74 616c  ["5EMA"] = pktal
-00018890: 6962 2e45 4d41 2864 5b22 436c 6f73 6522  ib.EMA(d["Close"
-000188a0: 5d2c 2074 696d 6570 6572 696f 643d 3529  ], timeperiod=5)
-000188b0: 0d0a 2020 2020 2020 2020 2020 2020 6420  ..            d 
-000188c0: 3d20 645b 636f 6c5f 6e61 6d65 735d 0d0a  = d[col_names]..
-000188d0: 2020 2020 2020 2020 2020 2020 6420 3d20              d = 
-000188e0: 642e 6472 6f70 6e61 2829 2e72 6f75 6e64  d.dropna().round
-000188f0: 2832 290d 0a0d 0a20 2020 2020 2020 2020  (2)....         
-00018900: 2020 2077 6974 6820 5375 7070 7265 7373     with Suppress
-00018910: 4f75 7470 7574 2873 7570 7072 6573 735f  Output(suppress_
-00018920: 7374 6465 7272 3d54 7275 652c 2073 7570  stderr=True, sup
-00018930: 7072 6573 735f 7374 646f 7574 3d54 7275  press_stdout=Tru
-00018940: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
-00018950: 2020 2020 2069 6620 2273 656c 6c22 2069       if "sell" i
-00018960: 6e20 6461 7461 5f6c 6973 745b 636e 745d  n data_list[cnt]
-00018970: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00018980: 2020 2020 2020 2073 7472 6563 6865 6420         streched 
-00018990: 3d20 645b 2864 2e4c 6f77 203e 2064 5b22  = d[(d.Low > d["
-000189a0: 3545 4d41 225d 2920 2620 2864 2e4c 6f77  5EMA"]) & (d.Low
-000189b0: 202d 2064 5b22 3545 4d41 225d 203e 2030   - d["5EMA"] > 0
-000189c0: 2e35 295d 0d0a 2020 2020 2020 2020 2020  .5)]..          
-000189d0: 2020 2020 2020 2020 2020 7374 7265 6368            strech
-000189e0: 6564 5b22 534c 225d 203d 2073 7472 6563  ed["SL"] = strec
-000189f0: 6865 642e 4869 6768 0d0a 2020 2020 2020  hed.High..      
-00018a00: 2020 2020 2020 2020 2020 2020 2020 7661                va
-00018a10: 6c69 6461 7465 203d 2064 5b0d 0a20 2020  lidate = d[..   
-00018a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a30: 2020 2020 2028 642e 4c6f 772e 7368 6966       (d.Low.shif
-00018a40: 7428 3129 203e 2064 5b22 3545 4d41 225d  t(1) > d["5EMA"]
-00018a50: 2e73 6869 6674 2831 2929 0d0a 2020 2020  .shift(1))..    
-00018a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a70: 2020 2020 2620 2864 2e4c 6f77 2e73 6869      & (d.Low.shi
-00018a80: 6674 2831 2920 2d20 645b 2235 454d 4122  ft(1) - d["5EMA"
-00018a90: 5d2e 7368 6966 7428 3129 203e 2030 2e35  ].shift(1) > 0.5
-00018aa0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00018ab0: 2020 2020 2020 205d 0d0a 2020 2020 2020         ]..      
-00018ac0: 2020 2020 2020 2020 2020 2020 2020 6f6c                ol
-00018ad0: 645f 696e 6465 7820 3d20 7661 6c69 6461  d_index = valida
-00018ae0: 7465 2e69 6e64 6578 0d0a 2020 2020 2020  te.index..      
-00018af0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-00018b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018b10: 2020 2020 206d 6173 6b20 3d20 2864 2e48       mask = (d.H
-00018b20: 6967 6820 3c20 645b 2235 454d 4122 5d29  igh < d["5EMA"])
-00018b30: 2026 2028 645b 2235 454d 4122 5d20 2d20   & (d["5EMA"] - 
-00018b40: 642e 4869 6768 203e 2030 2e35 2920 2023  d.High > 0.5)  #
-00018b50: 2042 7579 0d0a 2020 2020 2020 2020 2020   Buy..          
-00018b60: 2020 2020 2020 2020 2020 7374 7265 6368            strech
-00018b70: 6564 203d 2064 5b6d 6173 6b5d 0d0a 2020  ed = d[mask]..  
-00018b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b90: 2020 7374 7265 6368 6564 5b22 534c 225d    streched["SL"]
-00018ba0: 203d 2073 7472 6563 6865 642e 4c6f 770d   = streched.Low.
-00018bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018bc0: 2020 2020 2076 616c 6964 6174 6520 3d20       validate = 
-00018bd0: 642e 6c6f 635b 6d61 736b 2e73 6869 6674  d.loc[mask.shift
-00018be0: 2831 292e 6669 6c6c 6e61 2846 616c 7365  (1).fillna(False
-00018bf0: 295d 0d0a 2020 2020 2020 2020 2020 2020  )]..            
-00018c00: 2020 2020 2020 2020 6f6c 645f 696e 6465          old_inde
-00018c10: 7820 3d20 7661 6c69 6461 7465 2e69 6e64  x = validate.ind
-00018c20: 6578 0d0a 2020 2020 2020 2020 2020 2020  ex..            
-00018c30: 7467 7420 3d20 7064 2e44 6174 6146 7261  tgt = pd.DataFra
-00018c40: 6d65 280d 0a20 2020 2020 2020 2020 2020  me(..           
-00018c50: 2020 2020 2028 0d0a 2020 2020 2020 2020       (..        
-00018c60: 2020 2020 2020 2020 2020 2020 7661 6c69              vali
-00018c70: 6461 7465 2e43 6c6f 7365 2e72 6573 6574  date.Close.reset
-00018c80: 5f69 6e64 6578 2864 726f 703d 5472 7565  _index(drop=True
-00018c90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00018ca0: 2020 2020 2020 202d 2028 0d0a 2020 2020         - (..    
-00018cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018cc0: 2020 2020 280d 0a20 2020 2020 2020 2020      (..         
+000184f0: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
+00018500: 5465 7874 2e42 4f4c 440d 0a20 2020 2020  Text.BOLD..     
+00018510: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
+00018520: 6f72 5465 7874 2e57 4152 4e0d 0a20 2020  orText.WARN..   
+00018530: 2020 2020 2020 2020 2020 2020 202b 2022               + "
+00018540: 4e6f 7465 3a20 5468 6520 4149 2070 7265  Note: The AI pre
+00018550: 6469 6374 696f 6e20 7368 6f75 6c64 2062  diction should b
+00018560: 6520 6578 6563 7574 6564 2041 6674 6572  e executed After
+00018570: 2033 2050 4d20 6f72 204e 6561 7220 746f   3 PM or Near to
+00018580: 2043 6c6f 7369 6e67 2074 696d 6520 6173   Closing time as
+00018590: 2074 6865 2050 7265 6469 6374 696f 6e20   the Prediction 
+000185a0: 4163 6375 7261 6379 2069 7320 6261 7365  Accuracy is base
+000185b0: 6420 6f6e 2074 6865 2043 6c6f 7369 6e67  d on the Closing
+000185c0: 2070 7269 6365 2122 0d0a 2020 2020 2020   price!"..      
+000185d0: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
+000185e0: 7254 6578 742e 454e 440d 0a20 2020 2020  rText.END..     
+000185f0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+00018600: 2020 7072 6564 6963 7469 6f6e 5465 7874    predictionText
+00018610: 203d 2022 4d61 726b 6574 206d 6179 204f   = "Market may O
+00018620: 7065 6e20 7b7d 206e 6578 7420 6461 7921  pen {} next day!
+00018630: 207b 7d22 2e66 6f72 6d61 7428 6f75 742c   {}".format(out,
+00018640: 2073 7567 290d 0a20 2020 2020 2020 2073   sug)..        s
+00018650: 7472 656e 6774 6854 6578 7420 3d20 2250  trengthText = "P
+00018660: 726f 6261 6269 6c69 7479 2f53 7472 656e  robability/Stren
+00018670: 6774 6820 6f66 2050 7265 6469 6374 696f  gth of Predictio
+00018680: 6e20 3d20 7b7d 2522 2e66 6f72 6d61 7428  n = {}%".format(
+00018690: 0d0a 2020 2020 2020 2020 2020 2020 5574  ..            Ut
+000186a0: 696c 6974 792e 746f 6f6c 732e 6765 7453  ility.tools.getS
+000186b0: 6967 6d6f 6964 436f 6e66 6964 656e 6365  igmoidConfidence
+000186c0: 2870 7265 645b 305d 290d 0a20 2020 2020  (pred[0])..     
+000186d0: 2020 2029 0d0a 2020 2020 2020 2020 4f75     )..        Ou
+000186e0: 7470 7574 436f 6e74 726f 6c73 2829 2e70  tputControls().p
+000186f0: 7269 6e74 4f75 7470 7574 280d 0a20 2020  rintOutput(..   
+00018700: 2020 2020 2020 2020 2063 6f6c 6f72 5465           colorTe
+00018710: 7874 2e42 4f4c 440d 0a20 2020 2020 2020  xt.BOLD..       
+00018720: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
+00018730: 2e42 4c55 450d 0a20 2020 2020 2020 2020  .BLUE..         
+00018740: 2020 202b 2022 5c6e 220d 0a20 2020 2020     + "\n"..     
+00018750: 2020 2020 2020 202b 2022 5b2b 5d20 4e69         + "[+] Ni
+00018760: 6674 7920 4149 2050 7265 6469 6374 696f  fty AI Predictio
+00018770: 6e20 2d3e 2022 0d0a 2020 2020 2020 2020  n -> "..        
+00018780: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
+00018790: 454e 440d 0a20 2020 2020 2020 2020 2020  END..           
+000187a0: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
+000187b0: 440d 0a20 2020 2020 2020 2020 2020 202b  D..            +
+000187c0: 2070 7265 6469 6374 696f 6e54 6578 740d   predictionText.
+000187d0: 0a20 2020 2020 2020 2020 2020 202b 2063  .            + c
+000187e0: 6f6c 6f72 5465 7874 2e45 4e44 0d0a 2020  olorText.END..  
+000187f0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+00018800: 204f 7574 7075 7443 6f6e 7472 6f6c 7328   OutputControls(
+00018810: 292e 7072 696e 744f 7574 7075 7428 0d0a  ).printOutput(..
+00018820: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
+00018830: 7254 6578 742e 424f 4c44 0d0a 2020 2020  rText.BOLD..    
+00018840: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
+00018850: 6578 742e 424c 5545 0d0a 2020 2020 2020  ext.BLUE..      
+00018860: 2020 2020 2020 2b20 225c 6e22 0d0a 2020        + "\n"..  
+00018870: 2020 2020 2020 2020 2020 2b20 225b 2b5d            + "[+]
+00018880: 204e 6966 7479 2041 4920 5072 6564 6963   Nifty AI Predic
+00018890: 7469 6f6e 202d 3e20 220d 0a20 2020 2020  tion -> "..     
+000188a0: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
+000188b0: 7874 2e45 4e44 0d0a 2020 2020 2020 2020  xt.END..        
+000188c0: 2020 2020 2b20 7374 7265 6e67 7468 5465      + strengthTe
+000188d0: 7874 0d0a 2020 2020 2020 2020 290d 0a0d  xt..        )...
+000188e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000188f0: 7072 6564 2c20 7072 6564 6963 7469 6f6e  pred, prediction
+00018900: 5465 7874 2e72 6570 6c61 6365 286f 7574  Text.replace(out
+00018910: 2c20 6f75 7454 6578 7429 2c20 7374 7265  , outText), stre
+00018920: 6e67 7468 5465 7874 0d0a 0d0a 2020 2020  ngthText....    
+00018930: 6465 6620 6d6f 6e69 746f 7246 6976 6545  def monitorFiveE
+00018940: 6d61 2873 656c 662c 2066 6574 6368 6572  ma(self, fetcher
+00018950: 2c20 7265 7375 6c74 5f64 662c 206c 6173  , result_df, las
+00018960: 745f 7369 676e 616c 2c20 7269 736b 5f72  t_signal, risk_r
+00018970: 6577 6172 643d 3329 3a0d 0a20 2020 2020  eward=3):..     
+00018980: 2020 2063 6f6c 5f6e 616d 6573 203d 205b     col_names = [
+00018990: 2248 6967 6822 2c20 224c 6f77 222c 2022  "High", "Low", "
+000189a0: 436c 6f73 6522 2c20 2235 454d 4122 5d0d  Close", "5EMA"].
+000189b0: 0a20 2020 2020 2020 2064 6174 615f 6c69  .        data_li
+000189c0: 7374 203d 205b 226e 6966 7479 5f62 7579  st = ["nifty_buy
+000189d0: 222c 2022 6261 6e6b 6e69 6674 795f 6275  ", "banknifty_bu
+000189e0: 7922 2c20 226e 6966 7479 5f73 656c 6c22  y", "nifty_sell"
+000189f0: 2c20 2262 616e 6b6e 6966 7479 5f73 656c  , "banknifty_sel
+00018a00: 6c22 5d0d 0a0d 0a20 2020 2020 2020 2064  l"]....        d
+00018a10: 6174 615f 7475 706c 6520 3d20 6665 7463  ata_tuple = fetc
+00018a20: 6865 722e 6665 7463 6846 6976 6545 6d61  her.fetchFiveEma
+00018a30: 4461 7461 2829 0d0a 2020 2020 2020 2020  Data()..        
+00018a40: 666f 7220 636e 7420 696e 2072 616e 6765  for cnt in range
+00018a50: 286c 656e 2864 6174 615f 7475 706c 6529  (len(data_tuple)
+00018a60: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00018a70: 6420 3d20 6461 7461 5f74 7570 6c65 5b63  d = data_tuple[c
+00018a80: 6e74 5d0d 0a20 2020 2020 2020 2020 2020  nt]..           
+00018a90: 2064 5b22 3545 4d41 225d 203d 2070 6b74   d["5EMA"] = pkt
+00018aa0: 616c 6962 2e45 4d41 2864 5b22 436c 6f73  alib.EMA(d["Clos
+00018ab0: 6522 5d2c 2074 696d 6570 6572 696f 643d  e"], timeperiod=
+00018ac0: 3529 0d0a 2020 2020 2020 2020 2020 2020  5)..            
+00018ad0: 6420 3d20 645b 636f 6c5f 6e61 6d65 735d  d = d[col_names]
+00018ae0: 0d0a 2020 2020 2020 2020 2020 2020 6420  ..            d 
+00018af0: 3d20 642e 6472 6f70 6e61 2829 2e72 6f75  = d.dropna().rou
+00018b00: 6e64 2832 290d 0a0d 0a20 2020 2020 2020  nd(2)....       
+00018b10: 2020 2020 2077 6974 6820 5375 7070 7265       with Suppre
+00018b20: 7373 4f75 7470 7574 2873 7570 7072 6573  ssOutput(suppres
+00018b30: 735f 7374 6465 7272 3d54 7275 652c 2073  s_stderr=True, s
+00018b40: 7570 7072 6573 735f 7374 646f 7574 3d54  uppress_stdout=T
+00018b50: 7275 6529 3a0d 0a20 2020 2020 2020 2020  rue):..         
+00018b60: 2020 2020 2020 2069 6620 2273 656c 6c22         if "sell"
+00018b70: 2069 6e20 6461 7461 5f6c 6973 745b 636e   in data_list[cn
+00018b80: 745d 3a0d 0a20 2020 2020 2020 2020 2020  t]:..           
+00018b90: 2020 2020 2020 2020 2073 7472 6563 6865           streche
+00018ba0: 6420 3d20 645b 2864 2e4c 6f77 203e 2064  d = d[(d.Low > d
+00018bb0: 5b22 3545 4d41 225d 2920 2620 2864 2e4c  ["5EMA"]) & (d.L
+00018bc0: 6f77 202d 2064 5b22 3545 4d41 225d 203e  ow - d["5EMA"] >
+00018bd0: 2030 2e35 295d 0d0a 2020 2020 2020 2020   0.5)]..        
+00018be0: 2020 2020 2020 2020 2020 2020 7374 7265              stre
+00018bf0: 6368 6564 5b22 534c 225d 203d 2073 7472  ched["SL"] = str
+00018c00: 6563 6865 642e 4869 6768 0d0a 2020 2020  eched.High..    
+00018c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018c20: 7661 6c69 6461 7465 203d 2064 5b0d 0a20  validate = d[.. 
+00018c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018c40: 2020 2020 2020 2028 642e 4c6f 772e 7368         (d.Low.sh
+00018c50: 6966 7428 3129 203e 2064 5b22 3545 4d41  ift(1) > d["5EMA
+00018c60: 225d 2e73 6869 6674 2831 2929 0d0a 2020  "].shift(1))..  
+00018c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018c80: 2020 2020 2020 2620 2864 2e4c 6f77 2e73        & (d.Low.s
+00018c90: 6869 6674 2831 2920 2d20 645b 2235 454d  hift(1) - d["5EM
+00018ca0: 4122 5d2e 7368 6966 7428 3129 203e 2030  A"].shift(1) > 0
+00018cb0: 2e35 290d 0a20 2020 2020 2020 2020 2020  .5)..           
+00018cc0: 2020 2020 2020 2020 205d 0d0a 2020 2020           ]..    
 00018cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ce0: 2020 2073 7472 6563 6865 642e 534c 2e72     streched.SL.r
-00018cf0: 6573 6574 5f69 6e64 6578 2864 726f 703d  eset_index(drop=
-00018d00: 5472 7565 290d 0a20 2020 2020 2020 2020  True)..         
-00018d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d20: 2020 202d 2076 616c 6964 6174 652e 436c     - validate.Cl
-00018d30: 6f73 652e 7265 7365 745f 696e 6465 7828  ose.reset_index(
-00018d40: 6472 6f70 3d54 7275 6529 0d0a 2020 2020  drop=True)..    
-00018d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d60: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-00018d70: 2020 2020 2020 2020 2020 2020 2020 202a                 *
-00018d80: 2072 6973 6b5f 7265 7761 7264 0d0a 2020   risk_reward..  
+00018ce0: 6f6c 645f 696e 6465 7820 3d20 7661 6c69  old_index = vali
+00018cf0: 6461 7465 2e69 6e64 6578 0d0a 2020 2020  date.index..    
+00018d00: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00018d10: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00018d20: 2020 2020 2020 206d 6173 6b20 3d20 2864         mask = (d
+00018d30: 2e48 6967 6820 3c20 645b 2235 454d 4122  .High < d["5EMA"
+00018d40: 5d29 2026 2028 645b 2235 454d 4122 5d20  ]) & (d["5EMA"] 
+00018d50: 2d20 642e 4869 6768 203e 2030 2e35 2920  - d.High > 0.5) 
+00018d60: 2023 2042 7579 0d0a 2020 2020 2020 2020   # Buy..        
+00018d70: 2020 2020 2020 2020 2020 2020 7374 7265              stre
+00018d80: 6368 6564 203d 2064 5b6d 6173 6b5d 0d0a  ched = d[mask]..
 00018d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018da0: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-00018db0: 2020 2020 2029 2c0d 0a20 2020 2020 2020       ),..       
-00018dc0: 2020 2020 2020 2020 2063 6f6c 756d 6e73           columns
-00018dd0: 3d5b 2254 6172 6765 7422 5d2c 0d0a 2020  =["Target"],..  
-00018de0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
-00018df0: 2020 2020 2020 2020 2076 616c 6964 6174           validat
-00018e00: 6520 3d20 7064 2e63 6f6e 6361 7428 0d0a  e = pd.concat(..
-00018e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e20: 5b0d 0a20 2020 2020 2020 2020 2020 2020  [..             
-00018e30: 2020 2020 2020 2076 616c 6964 6174 652e         validate.
-00018e40: 7265 7365 745f 696e 6465 7828 6472 6f70  reset_index(drop
-00018e50: 3d54 7275 6529 2c0d 0a20 2020 2020 2020  =True),..       
-00018e60: 2020 2020 2020 2020 2020 2020 2073 7472               str
-00018e70: 6563 6865 645b 2253 4c22 5d2e 7265 7365  eched["SL"].rese
-00018e80: 745f 696e 6465 7828 6472 6f70 3d54 7275  t_index(drop=Tru
-00018e90: 6529 2c0d 0a20 2020 2020 2020 2020 2020  e),..           
-00018ea0: 2020 2020 2020 2020 2074 6774 2c0d 0a20           tgt,.. 
-00018eb0: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00018ec0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00018ed0: 2020 2061 7869 733d 312c 0d0a 2020 2020     axis=1,..    
-00018ee0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-00018ef0: 2020 2020 2020 2076 616c 6964 6174 6520         validate 
-00018f00: 3d20 7661 6c69 6461 7465 2e74 6169 6c28  = validate.tail(
-00018f10: 6c65 6e28 6f6c 645f 696e 6465 7829 290d  len(old_index)).
-00018f20: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
-00018f30: 6964 6174 6520 3d20 7661 6c69 6461 7465  idate = validate
-00018f40: 2e73 6574 5f69 6e64 6578 286f 6c64 5f69  .set_index(old_i
-00018f50: 6e64 6578 290d 0a20 2020 2020 2020 2020  ndex)..         
-00018f60: 2020 2069 6620 2273 656c 6c22 2069 6e20     if "sell" in 
-00018f70: 6461 7461 5f6c 6973 745b 636e 745d 3a0d  data_list[cnt]:.
-00018f80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018f90: 2066 696e 616c 203d 2076 616c 6964 6174   final = validat
-00018fa0: 655b 7661 6c69 6461 7465 2e43 6c6f 7365  e[validate.Close
-00018fb0: 203c 2076 616c 6964 6174 655b 2235 454d   < validate["5EM
-00018fc0: 4122 5d5d 2e74 6169 6c28 3129 0d0a 2020  A"]].tail(1)..  
-00018fd0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-00018fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018ff0: 2066 696e 616c 203d 2076 616c 6964 6174   final = validat
-00019000: 655b 7661 6c69 6461 7465 2e43 6c6f 7365  e[validate.Close
-00019010: 203e 2076 616c 6964 6174 655b 2235 454d   > validate["5EM
-00019020: 4122 5d5d 2e74 6169 6c28 3129 0d0a 0d0a  A"]].tail(1)....
-00019030: 2020 2020 2020 2020 2020 2020 6966 2064              if d
-00019040: 6174 615f 6c69 7374 5b63 6e74 5d20 6e6f  ata_list[cnt] no
-00019050: 7420 696e 206c 6173 745f 7369 676e 616c  t in last_signal
-00019060: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00019070: 2020 206c 6173 745f 7369 676e 616c 5b64     last_signal[d
-00019080: 6174 615f 6c69 7374 5b63 6e74 5d5d 203d  ata_list[cnt]] =
-00019090: 2066 696e 616c 0d0a 2020 2020 2020 2020   final..        
-000190a0: 2020 2020 656c 6966 2064 6174 615f 6c69      elif data_li
-000190b0: 7374 5b63 6e74 5d20 696e 206c 6173 745f  st[cnt] in last_
-000190c0: 7369 676e 616c 3a0d 0a20 2020 2020 2020  signal:..       
-000190d0: 2020 2020 2020 2020 2074 7279 3a0d 0a20           try:.. 
-000190e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000190f0: 2020 2063 6f6e 6469 7469 6f6e 203d 206c     condition = l
-00019100: 6173 745f 7369 676e 616c 5b64 6174 615f  ast_signal[data_
-00019110: 6c69 7374 5b63 6e74 5d5d 5b30 5d5b 2253  list[cnt]][0]["S
-00019120: 4c22 5d5b 305d 0d0a 2020 2020 2020 2020  L"][0]..        
-00019130: 2020 2020 2020 2020 6578 6365 7074 204b          except K
-00019140: 6579 4572 726f 7220 6173 2065 3a20 2320  eyError as e: # 
-00019150: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
-00019160: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019170: 2020 2020 2020 7365 6c66 2e64 6566 6175        self.defau
-00019180: 6c74 5f6c 6f67 6765 722e 6465 6275 6728  lt_logger.debug(
-00019190: 652c 2065 7863 5f69 6e66 6f3d 5472 7565  e, exc_info=True
-000191a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000191b0: 2020 2020 2020 2063 6f6e 6469 7469 6f6e         condition
-000191c0: 203d 206c 6173 745f 7369 676e 616c 5b64   = last_signal[d
-000191d0: 6174 615f 6c69 7374 5b63 6e74 5d5d 5b22  ata_list[cnt]]["
-000191e0: 534c 225d 5b30 5d0d 0a20 2020 2020 2020  SL"][0]..       
-000191f0: 2020 2020 2020 2020 2023 2069 6620 6c61           # if la
-00019200: 7374 5f73 6967 6e61 6c5b 6461 7461 5f6c  st_signal[data_l
-00019210: 6973 745b 636e 745d 5d20 6973 206e 6f74  ist[cnt]] is not
-00019220: 2066 696e 616c 3a20 2020 2020 2020 2020   final:         
-00019230: 2023 2044 6562 7567 202d 2053 686f 7773   # Debug - Shows
-00019240: 2061 6c6c 2063 6f6e 6469 7469 6f6e 730d   all conditions.
-00019250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019260: 2069 6620 6c65 6e28 6669 6e61 6c5b 2253   if len(final["S
-00019270: 4c22 5d29 203e 2030 2061 6e64 2063 6f6e  L"]) > 0 and con
-00019280: 6469 7469 6f6e 2021 3d20 6669 6e61 6c5b  dition != final[
-00019290: 2253 4c22 5d2e 696c 6f63 5b30 5d3a 0d0a  "SL"].iloc[0]:..
-000192a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000192b0: 2020 2020 2320 446f 2073 6f6d 6574 6869      # Do somethi
-000192c0: 6e67 2077 6974 6820 7265 7375 6c74 730d  ng with results.
-000192d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000192e0: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-000192f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019300: 2020 2072 6573 756c 745f 6466 203d 2070     result_df = p
-00019310: 642e 636f 6e63 6174 280d 0a20 2020 2020  d.concat(..     
-00019320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019330: 2020 2020 2020 205b 0d0a 2020 2020 2020         [..      
-00019340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019350: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00019360: 5f64 662c 0d0a 2020 2020 2020 2020 2020  _df,..          
-00019370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019380: 2020 2020 2020 7064 2e44 6174 6146 7261        pd.DataFra
-00019390: 6d65 280d 0a20 2020 2020 2020 2020 2020  me(..           
-000193a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000193b0: 2020 2020 2020 2020 205b 0d0a 2020 2020           [..    
-000193c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000193d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000193e0: 2020 2020 5b0d 0a20 2020 2020 2020 2020      [..         
-000193f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019410: 2020 2063 6f6c 6f72 5465 7874 2e42 4c55     colorText.BLU
-00019420: 450d 0a20 2020 2020 2020 2020 2020 2020  E..             
-00019430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019440: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-00019450: 2073 7472 2866 696e 616c 2e69 6e64 6578   str(final.index
-00019460: 5b30 5d29 0d0a 2020 2020 2020 2020 2020  [0])..          
-00019470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019490: 2020 2b20 636f 6c6f 7254 6578 742e 454e    + colorText.EN
-000194a0: 442c 0d0a 2020 2020 2020 2020 2020 2020  D,..            
-000194b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000194c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000194d0: 636f 6c6f 7254 6578 742e 424f 4c44 0d0a  colorText.BOLD..
-000194e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000194f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019500: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
-00019510: 6c6f 7254 6578 742e 5741 524e 0d0a 2020  lorText.WARN..  
-00019520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018da0: 2020 2020 7374 7265 6368 6564 5b22 534c      streched["SL
+00018db0: 225d 203d 2073 7472 6563 6865 642e 4c6f  "] = streched.Lo
+00018dc0: 770d 0a20 2020 2020 2020 2020 2020 2020  w..             
+00018dd0: 2020 2020 2020 2076 616c 6964 6174 6520         validate 
+00018de0: 3d20 642e 6c6f 635b 6d61 736b 2e73 6869  = d.loc[mask.shi
+00018df0: 6674 2831 292e 6669 6c6c 6e61 2846 616c  ft(1).fillna(Fal
+00018e00: 7365 295d 0d0a 2020 2020 2020 2020 2020  se)]..          
+00018e10: 2020 2020 2020 2020 2020 6f6c 645f 696e            old_in
+00018e20: 6465 7820 3d20 7661 6c69 6461 7465 2e69  dex = validate.i
+00018e30: 6e64 6578 0d0a 2020 2020 2020 2020 2020  ndex..          
+00018e40: 2020 7467 7420 3d20 7064 2e44 6174 6146    tgt = pd.DataF
+00018e50: 7261 6d65 280d 0a20 2020 2020 2020 2020  rame(..         
+00018e60: 2020 2020 2020 2028 0d0a 2020 2020 2020         (..      
+00018e70: 2020 2020 2020 2020 2020 2020 2020 7661                va
+00018e80: 6c69 6461 7465 2e43 6c6f 7365 2e72 6573  lidate.Close.res
+00018e90: 6574 5f69 6e64 6578 2864 726f 703d 5472  et_index(drop=Tr
+00018ea0: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
+00018eb0: 2020 2020 2020 2020 202d 2028 0d0a 2020           - (..  
+00018ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ed0: 2020 2020 2020 280d 0a20 2020 2020 2020        (..       
+00018ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ef0: 2020 2020 2073 7472 6563 6865 642e 534c       streched.SL
+00018f00: 2e72 6573 6574 5f69 6e64 6578 2864 726f  .reset_index(dro
+00018f10: 703d 5472 7565 290d 0a20 2020 2020 2020  p=True)..       
+00018f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f30: 2020 2020 202d 2076 616c 6964 6174 652e       - validate.
+00018f40: 436c 6f73 652e 7265 7365 745f 696e 6465  Close.reset_inde
+00018f50: 7828 6472 6f70 3d54 7275 6529 0d0a 2020  x(drop=True)..  
+00018f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f70: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+00018f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f90: 202a 2072 6973 6b5f 7265 7761 7264 0d0a   * risk_reward..
+00018fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018fb0: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+00018fc0: 2020 2020 2020 2029 2c0d 0a20 2020 2020         ),..     
+00018fd0: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
+00018fe0: 6e73 3d5b 2254 6172 6765 7422 5d2c 0d0a  ns=["Target"],..
+00018ff0: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+00019000: 2020 2020 2020 2020 2020 2076 616c 6964             valid
+00019010: 6174 6520 3d20 7064 2e63 6f6e 6361 7428  ate = pd.concat(
+00019020: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019030: 2020 5b0d 0a20 2020 2020 2020 2020 2020    [..           
+00019040: 2020 2020 2020 2020 2076 616c 6964 6174           validat
+00019050: 652e 7265 7365 745f 696e 6465 7828 6472  e.reset_index(dr
+00019060: 6f70 3d54 7275 6529 2c0d 0a20 2020 2020  op=True),..     
+00019070: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00019080: 7472 6563 6865 645b 2253 4c22 5d2e 7265  treched["SL"].re
+00019090: 7365 745f 696e 6465 7828 6472 6f70 3d54  set_index(drop=T
+000190a0: 7275 6529 2c0d 0a20 2020 2020 2020 2020  rue),..         
+000190b0: 2020 2020 2020 2020 2020 2074 6774 2c0d             tgt,.
+000190c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000190d0: 205d 2c0d 0a20 2020 2020 2020 2020 2020   ],..           
+000190e0: 2020 2020 2061 7869 733d 312c 0d0a 2020       axis=1,..  
+000190f0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+00019100: 2020 2020 2020 2020 2076 616c 6964 6174           validat
+00019110: 6520 3d20 7661 6c69 6461 7465 2e74 6169  e = validate.tai
+00019120: 6c28 6c65 6e28 6f6c 645f 696e 6465 7829  l(len(old_index)
+00019130: 290d 0a20 2020 2020 2020 2020 2020 2076  )..            v
+00019140: 616c 6964 6174 6520 3d20 7661 6c69 6461  alidate = valida
+00019150: 7465 2e73 6574 5f69 6e64 6578 286f 6c64  te.set_index(old
+00019160: 5f69 6e64 6578 290d 0a20 2020 2020 2020  _index)..       
+00019170: 2020 2020 2069 6620 2273 656c 6c22 2069       if "sell" i
+00019180: 6e20 6461 7461 5f6c 6973 745b 636e 745d  n data_list[cnt]
+00019190: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000191a0: 2020 2066 696e 616c 203d 2076 616c 6964     final = valid
+000191b0: 6174 655b 7661 6c69 6461 7465 2e43 6c6f  ate[validate.Clo
+000191c0: 7365 203c 2076 616c 6964 6174 655b 2235  se < validate["5
+000191d0: 454d 4122 5d5d 2e74 6169 6c28 3129 0d0a  EMA"]].tail(1)..
+000191e0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000191f0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00019200: 2020 2066 696e 616c 203d 2076 616c 6964     final = valid
+00019210: 6174 655b 7661 6c69 6461 7465 2e43 6c6f  ate[validate.Clo
+00019220: 7365 203e 2076 616c 6964 6174 655b 2235  se > validate["5
+00019230: 454d 4122 5d5d 2e74 6169 6c28 3129 0d0a  EMA"]].tail(1)..
+00019240: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00019250: 2064 6174 615f 6c69 7374 5b63 6e74 5d20   data_list[cnt] 
+00019260: 6e6f 7420 696e 206c 6173 745f 7369 676e  not in last_sign
+00019270: 616c 3a0d 0a20 2020 2020 2020 2020 2020  al:..           
+00019280: 2020 2020 206c 6173 745f 7369 676e 616c       last_signal
+00019290: 5b64 6174 615f 6c69 7374 5b63 6e74 5d5d  [data_list[cnt]]
+000192a0: 203d 2066 696e 616c 0d0a 2020 2020 2020   = final..      
+000192b0: 2020 2020 2020 656c 6966 2064 6174 615f        elif data_
+000192c0: 6c69 7374 5b63 6e74 5d20 696e 206c 6173  list[cnt] in las
+000192d0: 745f 7369 676e 616c 3a0d 0a20 2020 2020  t_signal:..     
+000192e0: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
+000192f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019300: 2020 2020 2063 6f6e 6469 7469 6f6e 203d       condition =
+00019310: 206c 6173 745f 7369 676e 616c 5b64 6174   last_signal[dat
+00019320: 615f 6c69 7374 5b63 6e74 5d5d 5b30 5d5b  a_list[cnt]][0][
+00019330: 2253 4c22 5d5b 305d 0d0a 2020 2020 2020  "SL"][0]..      
+00019340: 2020 2020 2020 2020 2020 6578 6365 7074            except
+00019350: 204b 6579 4572 726f 7220 6173 2065 3a20   KeyError as e: 
+00019360: 2320 7072 6167 6d61 3a20 6e6f 2063 6f76  # pragma: no cov
+00019370: 6572 0d0a 2020 2020 2020 2020 2020 2020  er..            
+00019380: 2020 2020 2020 2020 7365 6c66 2e64 6566          self.def
+00019390: 6175 6c74 5f6c 6f67 6765 722e 6465 6275  ault_logger.debu
+000193a0: 6728 652c 2065 7863 5f69 6e66 6f3d 5472  g(e, exc_info=Tr
+000193b0: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
+000193c0: 2020 2020 2020 2020 2063 6f6e 6469 7469           conditi
+000193d0: 6f6e 203d 206c 6173 745f 7369 676e 616c  on = last_signal
+000193e0: 5b64 6174 615f 6c69 7374 5b63 6e74 5d5d  [data_list[cnt]]
+000193f0: 5b22 534c 225d 5b30 5d0d 0a20 2020 2020  ["SL"][0]..     
+00019400: 2020 2020 2020 2020 2020 2023 2069 6620             # if 
+00019410: 6c61 7374 5f73 6967 6e61 6c5b 6461 7461  last_signal[data
+00019420: 5f6c 6973 745b 636e 745d 5d20 6973 206e  _list[cnt]] is n
+00019430: 6f74 2066 696e 616c 3a20 2020 2020 2020  ot final:       
+00019440: 2020 2023 2044 6562 7567 202d 2053 686f     # Debug - Sho
+00019450: 7773 2061 6c6c 2063 6f6e 6469 7469 6f6e  ws all condition
+00019460: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+00019470: 2020 2069 6620 6c65 6e28 6669 6e61 6c5b     if len(final[
+00019480: 2253 4c22 5d29 203e 2030 2061 6e64 2063  "SL"]) > 0 and c
+00019490: 6f6e 6469 7469 6f6e 2021 3d20 6669 6e61  ondition != fina
+000194a0: 6c5b 2253 4c22 5d2e 696c 6f63 5b30 5d3a  l["SL"].iloc[0]:
+000194b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000194c0: 2020 2020 2020 2320 446f 2073 6f6d 6574        # Do somet
+000194d0: 6869 6e67 2077 6974 6820 7265 7375 6c74  hing with result
+000194e0: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+000194f0: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
+00019500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019510: 2020 2020 2072 6573 756c 745f 6466 203d       result_df =
+00019520: 2070 642e 636f 6e63 6174 280d 0a20 2020   pd.concat(..   
 00019530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019540: 2020 2020 2020 2020 2020 2b20 6461 7461            + data
-00019550: 5f6c 6973 745b 636e 745d 2e73 706c 6974  _list[cnt].split
-00019560: 2822 5f22 295b 305d 2e75 7070 6572 2829  ("_")[0].upper()
-00019570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019540: 2020 2020 2020 2020 205b 0d0a 2020 2020           [..    
+00019550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019560: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00019570: 6c74 5f64 662c 0d0a 2020 2020 2020 2020  lt_df,..        
 00019580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019590: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-000195a0: 636f 6c6f 7254 6578 742e 454e 442c 0d0a  colorText.END,..
+00019590: 2020 2020 2020 2020 7064 2e44 6174 6146          pd.DataF
+000195a0: 7261 6d65 280d 0a20 2020 2020 2020 2020  rame(..         
 000195b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000195c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000195d0: 2020 2020 2020 2020 2020 2020 280d 0a20              (.. 
+000195c0: 2020 2020 2020 2020 2020 205b 0d0a 2020             [..  
+000195d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000195e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000195f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019600: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00019610: 6f6c 6f72 5465 7874 2e42 4f4c 440d 0a20  olorText.BOLD.. 
-00019620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019640: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-00019650: 2063 6f6c 6f72 5465 7874 2e46 4149 4c0d   colorText.FAIL.
-00019660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000195f0: 2020 2020 2020 5b0d 0a20 2020 2020 2020        [..       
+00019600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019620: 2020 2020 2063 6f6c 6f72 5465 7874 2e42       colorText.B
+00019630: 4c55 450d 0a20 2020 2020 2020 2020 2020  LUE..           
+00019640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019660: 202b 2073 7472 2866 696e 616c 2e69 6e64   + str(final.ind
+00019670: 6578 5b30 5d29 0d0a 2020 2020 2020 2020  ex[0])..        
 00019680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019690: 202b 2064 6174 615f 6c69 7374 5b63 6e74   + data_list[cnt
-000196a0: 5d2e 7370 6c69 7428 225f 2229 5b31 5d2e  ].split("_")[1].
-000196b0: 7570 7065 7228 290d 0a20 2020 2020 2020  upper()..       
+00019690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000196a0: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
+000196b0: 454e 442c 0d0a 2020 2020 2020 2020 2020  END,..          
 000196c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000196d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000196e0: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
-000196f0: 5465 7874 2e45 4e44 0d0a 2020 2020 2020  Text.END..      
+000196e0: 2020 636f 6c6f 7254 6578 742e 424f 4c44    colorText.BOLD
+000196f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00019700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019720: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+00019710: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+00019720: 636f 6c6f 7254 6578 742e 5741 524e 0d0a  colorText.WARN..
 00019730: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019750: 2020 2020 2069 6620 2273 656c 6c22 2069       if "sell" i
-00019760: 6e20 6461 7461 5f6c 6973 745b 636e 745d  n data_list[cnt]
-00019770: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019790: 2020 2020 2020 2020 2020 2020 2020 656c                el
-000197a0: 7365 2028 0d0a 2020 2020 2020 2020 2020  se (..          
-000197b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000197c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000197d0: 2020 2020 2020 636f 6c6f 7254 6578 742e        colorText.
-000197e0: 424f 4c44 0d0a 2020 2020 2020 2020 2020  BOLD..          
-000197f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019750: 2020 2020 2020 2020 2020 2020 2b20 6461              + da
+00019760: 7461 5f6c 6973 745b 636e 745d 2e73 706c  ta_list[cnt].spl
+00019770: 6974 2822 5f22 295b 305d 2e75 7070 6572  it("_")[0].upper
+00019780: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+00019790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197b0: 2b20 636f 6c6f 7254 6578 742e 454e 442c  + colorText.END,
+000197c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000197d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197e0: 2020 2020 2020 2020 2020 2020 2020 280d                (.
+000197f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00019800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019810: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
-00019820: 742e 4752 4545 4e0d 0a20 2020 2020 2020  t.GREEN..       
-00019830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019820: 2063 6f6c 6f72 5465 7874 2e42 4f4c 440d   colorText.BOLD.
+00019830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00019840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019850: 2020 2020 2020 2020 202b 2064 6174 615f           + data_
-00019860: 6c69 7374 5b63 6e74 5d2e 7370 6c69 7428  list[cnt].split(
-00019870: 225f 2229 5b31 5d2e 7570 7065 7228 290d  "_")[1].upper().
-00019880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019860: 202b 2063 6f6c 6f72 5465 7874 2e46 4149   + colorText.FAI
+00019870: 4c0d 0a20 2020 2020 2020 2020 2020 2020  L..             
+00019880: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000198a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000198b0: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
-000198c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000198a0: 2020 202b 2064 6174 615f 6c69 7374 5b63     + data_list[c
+000198b0: 6e74 5d2e 7370 6c69 7428 225f 2229 5b31  nt].split("_")[1
+000198c0: 5d2e 7570 7065 7228 290d 0a20 2020 2020  ].upper()..     
 000198d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000198e0: 2020 2020 2020 2020 2020 2020 2020 292c                ),
-000198f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019910: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00019920: 6c6f 7254 6578 742e 4641 494c 0d0a 2020  lorText.FAIL..  
-00019930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000198e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000198f0: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
+00019900: 6f72 5465 7874 2e45 4e44 0d0a 2020 2020  orText.END..    
+00019910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019930: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
 00019940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019950: 2020 2020 2020 2020 2020 2b20 7374 7228            + str(
-00019960: 6669 6e61 6c2e 534c 5b30 5d29 0d0a 2020  final.SL[0])..  
-00019970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019990: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
-000199a0: 7254 6578 742e 454e 442c 0d0a 2020 2020  rText.END,..    
-000199b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019960: 2020 2020 2020 2069 6620 2273 656c 6c22         if "sell"
+00019970: 2069 6e20 6461 7461 5f6c 6973 745b 636e   in data_list[cn
+00019980: 745d 0d0a 2020 2020 2020 2020 2020 2020  t]..            
+00019990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000199a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000199b0: 656c 7365 2028 0d0a 2020 2020 2020 2020  else (..        
 000199c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000199d0: 2020 2020 2020 2020 636f 6c6f 7254 6578          colorTex
-000199e0: 742e 4752 4545 4e0d 0a20 2020 2020 2020  t.GREEN..       
-000199f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000199d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000199e0: 2020 2020 2020 2020 636f 6c6f 7254 6578          colorTex
+000199f0: 742e 424f 4c44 0d0a 2020 2020 2020 2020  t.BOLD..        
 00019a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019a10: 2020 2020 202b 2073 7472 2866 696e 616c       + str(final
-00019a20: 2e54 6172 6765 745b 305d 290d 0a20 2020  .Target[0])..   
-00019a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a20: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
+00019a30: 6578 742e 4752 4545 4e0d 0a20 2020 2020  ext.GREEN..     
 00019a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019a50: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
-00019a60: 5465 7874 2e45 4e44 2c0d 0a20 2020 2020  Text.END,..     
-00019a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019a90: 2020 2020 2020 2066 2231 3a7b 7269 736b         f"1:{risk
-00019aa0: 5f72 6577 6172 647d 222c 0d0a 2020 2020  _reward}",..    
+00019a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a60: 2020 2020 2020 2020 2020 202b 2064 6174             + dat
+00019a70: 615f 6c69 7374 5b63 6e74 5d2e 7370 6c69  a_list[cnt].spli
+00019a80: 7428 225f 2229 5b31 5d2e 7570 7065 7228  t("_")[1].upper(
+00019a90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00019aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ad0: 2020 2020 5d0d 0a20 2020 2020 2020 2020      ]..         
+00019ac0: 2020 202b 2063 6f6c 6f72 5465 7874 2e45     + colorText.E
+00019ad0: 4e44 0d0a 2020 2020 2020 2020 2020 2020  ND..            
 00019ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019af0: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
-00019b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b00: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
 00019b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019b20: 2020 2063 6f6c 756d 6e73 3d72 6573 756c     columns=resul
-00019b30: 745f 6466 2e63 6f6c 756d 6e73 2c0d 0a20  t_df.columns,.. 
+00019b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b30: 636f 6c6f 7254 6578 742e 4641 494c 0d0a  colorText.FAIL..
 00019b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019b50: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00019b60: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00019b70: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00019b80: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00019b90: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00019ba0: 7869 733d 302c 0d0a 2020 2020 2020 2020  xis=0,..        
-00019bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019bc0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00019bd0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00019be0: 745f 6466 2e72 6573 6574 5f69 6e64 6578  t_df.reset_index
-00019bf0: 2864 726f 703d 5472 7565 2c20 696e 706c  (drop=True, inpl
-00019c00: 6163 653d 5472 7565 290d 0a20 2020 2020  ace=True)..     
-00019c10: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00019c20: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-00019c30: 6173 2065 3a20 2023 2070 7261 676d 613a  as e:  # pragma:
-00019c40: 206e 6f20 636f 7665 720d 0a20 2020 2020   no cover..     
+00019b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b60: 2020 2020 2020 2020 2020 2020 2b20 7374              + st
+00019b70: 7228 6669 6e61 6c2e 534c 5b30 5d29 0d0a  r(final.SL[0])..
+00019b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ba0: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
+00019bb0: 6c6f 7254 6578 742e 454e 442c 0d0a 2020  lorText.END,..  
+00019bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019be0: 2020 2020 2020 2020 2020 636f 6c6f 7254            colorT
+00019bf0: 6578 742e 4752 4545 4e0d 0a20 2020 2020  ext.GREEN..     
+00019c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019c20: 2020 2020 2020 202b 2073 7472 2866 696e         + str(fin
+00019c30: 616c 2e54 6172 6765 745b 305d 290d 0a20  al.Target[0]).. 
+00019c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c60: 2020 2073 656c 662e 6465 6661 756c 745f     self.default_
-00019c70: 6c6f 6767 6572 2e64 6562 7567 2865 2c20  logger.debug(e, 
-00019c80: 6578 635f 696e 666f 3d54 7275 6529 0d0a  exc_info=True)..
+00019c60: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
+00019c70: 6f72 5465 7874 2e45 4e44 2c0d 0a20 2020  orText.END,..   
+00019c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ca0: 2020 2020 2020 2020 7061 7373 0d0a 2020          pass..  
-00019cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019cc0: 2020 2320 5468 656e 2075 7064 6174 650d    # Then update.
-00019cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019ce0: 2020 2020 206c 6173 745f 7369 676e 616c       last_signal
-00019cf0: 5b64 6174 615f 6c69 7374 5b63 6e74 5d5d  [data_list[cnt]]
-00019d00: 203d 205b 6669 6e61 6c5d 0d0a 2020 2020   = [final]..    
-00019d10: 2020 2020 6966 2072 6573 756c 745f 6466      if result_df
-00019d20: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
-00019d30: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00019d40: 745f 6466 2e64 726f 705f 6475 706c 6963  t_df.drop_duplic
-00019d50: 6174 6573 286b 6565 703d 226c 6173 7422  ates(keep="last"
-00019d60: 2c20 696e 706c 6163 653d 5472 7565 290d  , inplace=True).
-00019d70: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00019d80: 756c 745f 6466 2e73 6f72 745f 7661 6c75  ult_df.sort_valu
-00019d90: 6573 2862 793d 2254 696d 6522 2c20 696e  es(by="Time", in
-00019da0: 706c 6163 653d 5472 7565 290d 0a20 2020  place=True)..   
-00019db0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-00019dc0: 6c74 5f64 665b 3a3a 2d31 5d0d 0a0d 0a20  lt_df[::-1].... 
-00019dd0: 2020 2023 2050 7265 7072 6f63 6573 7320     # Preprocess 
-00019de0: 7468 6520 6163 7175 6972 6564 2064 6174  the acquired dat
-00019df0: 610d 0a20 2020 2064 6566 2070 7265 7072  a..    def prepr
-00019e00: 6f63 6573 7344 6174 6128 7365 6c66 2c20  ocessData(self, 
-00019e10: 6466 2c20 6461 7973 546f 4c6f 6f6b 6261  df, daysToLookba
-00019e20: 636b 3d4e 6f6e 6529 3a0d 0a20 2020 2020  ck=None):..     
-00019e30: 2020 2061 7373 6572 7420 6973 696e 7374     assert isinst
-00019e40: 616e 6365 2864 662c 2070 642e 4461 7461  ance(df, pd.Data
-00019e50: 4672 616d 6529 0d0a 2020 2020 2020 2020  Frame)..        
-00019e60: 6461 7461 203d 2064 662e 636f 7079 2829  data = df.copy()
-00019e70: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
-00019e80: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00019e90: 203d 2064 6174 612e 7265 706c 6163 6528   = data.replace(
-00019ea0: 6e70 2e69 6e66 2c20 6e70 2e6e 616e 292e  np.inf, np.nan).
-00019eb0: 7265 706c 6163 6528 2d6e 702e 696e 662c  replace(-np.inf,
-00019ec0: 206e 702e 6e61 6e29 2e64 726f 706e 6128   np.nan).dropna(
-00019ed0: 686f 773d 2261 6c6c 2229 0d0a 2020 2020  how="all")..    
-00019ee0: 2020 2020 2020 2020 2320 7365 6c66 2e64          # self.d
-00019ef0: 6566 6175 6c74 5f6c 6f67 6765 722e 696e  efault_logger.in
-00019f00: 666f 2866 2250 7265 7072 6f63 6573 7369  fo(f"Preprocessi
-00019f10: 6e67 2064 6174 613a 5c6e 7b64 6174 612e  ng data:\n{data.
-00019f20: 6865 6164 2831 297d 5c6e 2229 0d0a 2020  head(1)}\n")..  
-00019f30: 2020 2020 2020 2020 2020 6966 2064 6179            if day
-00019f40: 7354 6f4c 6f6f 6b62 6163 6b20 6973 204e  sToLookback is N
-00019f50: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00019f60: 2020 2020 2020 6461 7973 546f 4c6f 6f6b        daysToLook
-00019f70: 6261 636b 203d 2073 656c 662e 636f 6e66  back = self.conf
-00019f80: 6967 4d61 6e61 6765 722e 6461 7973 546f  igManager.daysTo
-00019f90: 4c6f 6f6b 6261 636b 0d0a 2020 2020 2020  Lookback..      
-00019fa0: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
-00019fb0: 6e66 6967 4d61 6e61 6765 722e 7573 6545  nfigManager.useE
-00019fc0: 4d41 3a0d 0a20 2020 2020 2020 2020 2020  MA:..           
-00019fd0: 2020 2020 2073 6d61 203d 2070 6b74 616c       sma = pktal
-00019fe0: 6962 2e45 4d41 2864 6174 615b 2243 6c6f  ib.EMA(data["Clo
-00019ff0: 7365 225d 2c20 7469 6d65 7065 7269 6f64  se"], timeperiod
-0001a000: 3d35 3029 0d0a 2020 2020 2020 2020 2020  =50)..          
-0001a010: 2020 2020 2020 6c6d 6120 3d20 706b 7461        lma = pkta
-0001a020: 6c69 622e 454d 4128 6461 7461 5b22 436c  lib.EMA(data["Cl
-0001a030: 6f73 6522 5d2c 2074 696d 6570 6572 696f  ose"], timeperio
-0001a040: 643d 3230 3029 0d0a 2020 2020 2020 2020  d=200)..        
-0001a050: 2020 2020 2020 2020 7373 6d61 203d 2070          ssma = p
-0001a060: 6b74 616c 6962 2e45 4d41 2864 6174 615b  ktalib.EMA(data[
-0001a070: 2243 6c6f 7365 225d 2c20 7469 6d65 7065  "Close"], timepe
-0001a080: 7269 6f64 3d39 290d 0a20 2020 2020 2020  riod=9)..       
-0001a090: 2020 2020 2020 2020 2064 6174 612e 696e           data.in
-0001a0a0: 7365 7274 286c 656e 2864 6174 612e 636f  sert(len(data.co
-0001a0b0: 6c75 6d6e 7329 2c20 2253 4d41 222c 2073  lumns), "SMA", s
-0001a0c0: 6d61 290d 0a20 2020 2020 2020 2020 2020  ma)..           
-0001a0d0: 2020 2020 2064 6174 612e 696e 7365 7274       data.insert
-0001a0e0: 286c 656e 2864 6174 612e 636f 6c75 6d6e  (len(data.column
-0001a0f0: 7329 2c20 224c 4d41 222c 206c 6d61 290d  s), "LMA", lma).
-0001a100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a110: 2064 6174 612e 696e 7365 7274 286c 656e   data.insert(len
-0001a120: 2864 6174 612e 636f 6c75 6d6e 7329 2c20  (data.columns), 
-0001a130: 2253 534d 4122 2c20 7373 6d61 290d 0a20  "SSMA", ssma).. 
-0001a140: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0001a150: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a160: 2020 736d 6120 3d20 706b 7461 6c69 622e    sma = pktalib.
-0001a170: 534d 4128 6461 7461 5b22 436c 6f73 6522  SMA(data["Close"
-0001a180: 5d2c 2074 696d 6570 6572 696f 643d 3530  ], timeperiod=50
-0001a190: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0001a1a0: 2020 206c 6d61 203d 2070 6b74 616c 6962     lma = pktalib
-0001a1b0: 2e53 4d41 2864 6174 615b 2243 6c6f 7365  .SMA(data["Close
-0001a1c0: 225d 2c20 7469 6d65 7065 7269 6f64 3d32  "], timeperiod=2
-0001a1d0: 3030 290d 0a20 2020 2020 2020 2020 2020  00)..           
-0001a1e0: 2020 2020 2073 736d 6120 3d20 706b 7461       ssma = pkta
-0001a1f0: 6c69 622e 534d 4128 6461 7461 5b22 436c  lib.SMA(data["Cl
-0001a200: 6f73 6522 5d2c 2074 696d 6570 6572 696f  ose"], timeperio
-0001a210: 643d 3929 0d0a 2020 2020 2020 2020 2020  d=9)..          
-0001a220: 2020 2020 2020 6461 7461 2e69 6e73 6572        data.inser
-0001a230: 7428 6c65 6e28 6461 7461 2e63 6f6c 756d  t(len(data.colum
-0001a240: 6e73 292c 2022 534d 4122 2c20 736d 6129  ns), "SMA", sma)
-0001a250: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a260: 2020 6461 7461 2e69 6e73 6572 7428 6c65    data.insert(le
-0001a270: 6e28 6461 7461 2e63 6f6c 756d 6e73 292c  n(data.columns),
-0001a280: 2022 4c4d 4122 2c20 6c6d 6129 0d0a 2020   "LMA", lma)..  
-0001a290: 2020 2020 2020 2020 2020 2020 2020 6461                da
-0001a2a0: 7461 2e69 6e73 6572 7428 6c65 6e28 6461  ta.insert(len(da
-0001a2b0: 7461 2e63 6f6c 756d 6e73 292c 2022 5353  ta.columns), "SS
-0001a2c0: 4d41 222c 2073 736d 6129 0d0a 2020 2020  MA", ssma)..    
-0001a2d0: 2020 2020 2020 2020 766f 6c20 3d20 706b          vol = pk
-0001a2e0: 7461 6c69 622e 534d 4128 6461 7461 5b22  talib.SMA(data["
-0001a2f0: 566f 6c75 6d65 225d 2c20 7469 6d65 7065  Volume"], timepe
-0001a300: 7269 6f64 3d32 3029 0d0a 2020 2020 2020  riod=20)..      
-0001a310: 2020 2020 2020 7273 6920 3d20 706b 7461        rsi = pkta
-0001a320: 6c69 622e 5253 4928 6461 7461 5b22 436c  lib.RSI(data["Cl
-0001a330: 6f73 6522 5d2c 2074 696d 6570 6572 696f  ose"], timeperio
-0001a340: 643d 3134 290d 0a20 2020 2020 2020 2020  d=14)..         
-0001a350: 2020 2064 6174 612e 696e 7365 7274 286c     data.insert(l
-0001a360: 656e 2864 6174 612e 636f 6c75 6d6e 7329  en(data.columns)
-0001a370: 2c20 2256 6f6c 4d41 222c 2076 6f6c 290d  , "VolMA", vol).
-0001a380: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-0001a390: 612e 696e 7365 7274 286c 656e 2864 6174  a.insert(len(dat
-0001a3a0: 612e 636f 6c75 6d6e 7329 2c20 2252 5349  a.columns), "RSI
-0001a3b0: 222c 2072 7369 290d 0a20 2020 2020 2020  ", rsi)..       
-0001a3c0: 2020 2020 2063 6369 203d 2070 6b74 616c       cci = pktal
-0001a3d0: 6962 2e43 4349 2864 6174 615b 2248 6967  ib.CCI(data["Hig
-0001a3e0: 6822 5d2c 2064 6174 615b 224c 6f77 225d  h"], data["Low"]
-0001a3f0: 2c20 6461 7461 5b22 436c 6f73 6522 5d2c  , data["Close"],
-0001a400: 2074 696d 6570 6572 696f 643d 3134 290d   timeperiod=14).
-0001a410: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-0001a420: 612e 696e 7365 7274 286c 656e 2864 6174  a.insert(len(dat
-0001a430: 612e 636f 6c75 6d6e 7329 2c20 2243 4349  a.columns), "CCI
-0001a440: 222c 2063 6369 290d 0a20 2020 2020 2020  ", cci)..       
-0001a450: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-0001a460: 2020 2020 2020 2020 2020 2066 6173 746b             fastk
-0001a470: 2c20 6661 7374 6420 3d20 706b 7461 6c69  , fastd = pktali
-0001a480: 622e 5354 4f43 4852 5349 280d 0a20 2020  b.STOCHRSI(..   
-0001a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a4a0: 2064 6174 615b 2243 6c6f 7365 225d 2c20   data["Close"], 
-0001a4b0: 7469 6d65 7065 7269 6f64 3d31 342c 2066  timeperiod=14, f
-0001a4c0: 6173 746b 5f70 6572 696f 643d 352c 2066  astk_period=5, f
-0001a4d0: 6173 7464 5f70 6572 696f 643d 332c 2066  astd_period=3, f
-0001a4e0: 6173 7464 5f6d 6174 7970 653d 300d 0a20  astd_matype=0.. 
-0001a4f0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0001a500: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a510: 2020 6461 7461 2e69 6e73 6572 7428 6c65    data.insert(le
-0001a520: 6e28 6461 7461 2e63 6f6c 756d 6e73 292c  n(data.columns),
-0001a530: 2022 4641 5354 4b22 2c20 6661 7374 6b29   "FASTK", fastk)
-0001a540: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a550: 2020 6461 7461 2e69 6e73 6572 7428 6c65    data.insert(le
-0001a560: 6e28 6461 7461 2e63 6f6c 756d 6e73 292c  n(data.columns),
-0001a570: 2022 4641 5354 4422 2c20 6661 7374 6429   "FASTD", fastd)
-0001a580: 0d0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
-0001a590: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
-0001a5a0: 7320 653a 0d0a 2020 2020 2020 2020 2020  s e:..          
-0001a5b0: 2020 2020 2020 7365 6c66 2e64 6566 6175        self.defau
-0001a5c0: 6c74 5f6c 6f67 6765 722e 6465 6275 6728  lt_logger.debug(
-0001a5d0: 652c 2065 7863 5f69 6e66 6f3d 5472 7565  e, exc_info=True
-0001a5e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0001a5f0: 2020 2070 6173 730d 0a20 2020 2020 2020     pass..       
-0001a600: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-0001a610: 6e20 6173 2065 3a0d 0a20 2020 2020 2020  n as e:..       
-0001a620: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
-0001a630: 6661 756c 745f 6c6f 6767 6572 2e64 6562  fault_logger.deb
-0001a640: 7567 2865 2c20 6578 635f 696e 666f 3d54  ug(e, exc_info=T
-0001a650: 7275 6529 0d0a 2020 2020 2020 2020 2020  rue)..          
-0001a660: 2020 2020 2020 7061 7373 0d0a 2020 2020        pass..    
-0001a670: 2020 2020 6461 7461 203d 2064 6174 615b      data = data[
-0001a680: 3a3a 2d31 5d20 2023 2052 6576 6572 7365  ::-1]  # Reverse
-0001a690: 2074 6865 2064 6174 6166 7261 6d65 0d0a   the dataframe..
-0001a6a0: 2020 2020 2020 2020 2320 6461 7461 203d          # data =
-0001a6b0: 2064 6174 612e 6669 6c6c 6e61 2830 290d   data.fillna(0).
-0001a6c0: 0a20 2020 2020 2020 2023 2064 6174 6120  .        # data 
-0001a6d0: 3d20 6461 7461 2e72 6570 6c61 6365 285b  = data.replace([
-0001a6e0: 6e70 2e69 6e66 2c20 2d6e 702e 696e 665d  np.inf, -np.inf]
-0001a6f0: 2c20 3029 0d0a 2020 2020 2020 2020 6675  , 0)..        fu
-0001a700: 6c6c 4461 7461 203d 2064 6174 610d 0a20  llData = data.. 
-0001a710: 2020 2020 2020 2074 7269 6d6d 6564 4461         trimmedDa
-0001a720: 7461 203d 2064 6174 612e 6865 6164 2864  ta = data.head(d
-0001a730: 6179 7354 6f4c 6f6f 6b62 6163 6b29 0d0a  aysToLookback)..
-0001a740: 2020 2020 2020 2020 7265 7475 726e 2028          return (
-0001a750: 6675 6c6c 4461 7461 2c20 7472 696d 6d65  fullData, trimme
-0001a760: 6444 6174 6129 0d0a 0d0a 2020 2020 2320  dData)....    # 
-0001a770: 5661 6c69 6461 7465 2069 6620 7468 6520  Validate if the 
-0001a780: 7374 6f63 6b20 6973 2062 756c 6c69 7368  stock is bullish
-0001a790: 2069 6e20 7468 6520 7368 6f72 7420 7465   in the short te
-0001a7a0: 726d 0d0a 2020 2020 6465 6620 7661 6c69  rm..    def vali
-0001a7b0: 6461 7465 3135 4d69 6e75 7465 5072 6963  date15MinutePric
-0001a7c0: 6556 6f6c 756d 6542 7265 616b 6f75 7428  eVolumeBreakout(
-0001a7d0: 7365 6c66 2c20 6466 293a 0d0a 2020 2020  self, df):..    
-0001a7e0: 2020 2020 6966 2064 6620 6973 204e 6f6e      if df is Non
-0001a7f0: 6520 6f72 206c 656e 2864 6629 203d 3d20  e or len(df) == 
-0001a800: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-0001a810: 7265 7475 726e 2046 616c 7365 0d0a 2020  return False..  
-0001a820: 2020 2020 2020 2320 6874 7470 733a 2f2f        # https://
-0001a830: 6368 6172 7469 6e6b 2e63 6f6d 2f73 6372  chartink.com/scr
-0001a840: 6565 6e65 722f 3135 2d6d 696e 2d70 7269  eener/15-min-pri
-0001a850: 6365 2d76 6f6c 756d 652d 6272 6561 6b6f  ce-volume-breako
-0001a860: 7574 0d0a 2020 2020 2020 2020 6461 7461  ut..        data
-0001a870: 203d 2064 662e 636f 7079 2829 0d0a 2020   = df.copy()..  
+00019ca0: 2020 2020 2020 2020 2066 2231 3a7b 7269           f"1:{ri
+00019cb0: 736b 5f72 6577 6172 647d 222c 0d0a 2020  sk_reward}",..  
+00019cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ce0: 2020 2020 2020 5d0d 0a20 2020 2020 2020        ]..       
+00019cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019d00: 2020 2020 2020 2020 2020 2020 205d 2c0d               ],.
+00019d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019d30: 2020 2020 2063 6f6c 756d 6e73 3d72 6573       columns=res
+00019d40: 756c 745f 6466 2e63 6f6c 756d 6e73 2c0d  ult_df.columns,.
+00019d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019d70: 2029 2c0d 0a20 2020 2020 2020 2020 2020   ),..           
+00019d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019d90: 205d 2c0d 0a20 2020 2020 2020 2020 2020   ],..           
+00019da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019db0: 2061 7869 733d 302c 0d0a 2020 2020 2020   axis=0,..      
+00019dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019dd0: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
+00019de0: 2020 2020 2020 2020 2020 2020 2072 6573               res
+00019df0: 756c 745f 6466 2e72 6573 6574 5f69 6e64  ult_df.reset_ind
+00019e00: 6578 2864 726f 703d 5472 7565 2c20 696e  ex(drop=True, in
+00019e10: 706c 6163 653d 5472 7565 290d 0a20 2020  place=True)..   
+00019e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019e30: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00019e40: 6e20 6173 2065 3a20 2023 2070 7261 676d  n as e:  # pragm
+00019e50: 613a 206e 6f20 636f 7665 720d 0a20 2020  a: no cover..   
+00019e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019e70: 2020 2020 2073 656c 662e 6465 6661 756c       self.defaul
+00019e80: 745f 6c6f 6767 6572 2e64 6562 7567 2865  t_logger.debug(e
+00019e90: 2c20 6578 635f 696e 666f 3d54 7275 6529  , exc_info=True)
+00019ea0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019eb0: 2020 2020 2020 2020 2020 7061 7373 0d0a            pass..
+00019ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ed0: 2020 2020 2320 5468 656e 2075 7064 6174      # Then updat
+00019ee0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+00019ef0: 2020 2020 2020 206c 6173 745f 7369 676e         last_sign
+00019f00: 616c 5b64 6174 615f 6c69 7374 5b63 6e74  al[data_list[cnt
+00019f10: 5d5d 203d 205b 6669 6e61 6c5d 0d0a 2020  ]] = [final]..  
+00019f20: 2020 2020 2020 6966 2072 6573 756c 745f        if result_
+00019f30: 6466 2069 7320 6e6f 7420 4e6f 6e65 3a0d  df is not None:.
+00019f40: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00019f50: 756c 745f 6466 2e64 726f 705f 6475 706c  ult_df.drop_dupl
+00019f60: 6963 6174 6573 286b 6565 703d 226c 6173  icates(keep="las
+00019f70: 7422 2c20 696e 706c 6163 653d 5472 7565  t", inplace=True
+00019f80: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
+00019f90: 6573 756c 745f 6466 2e73 6f72 745f 7661  esult_df.sort_va
+00019fa0: 6c75 6573 2862 793d 2254 696d 6522 2c20  lues(by="Time", 
+00019fb0: 696e 706c 6163 653d 5472 7565 290d 0a20  inplace=True).. 
+00019fc0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00019fd0: 7375 6c74 5f64 665b 3a3a 2d31 5d0d 0a0d  sult_df[::-1]...
+00019fe0: 0a20 2020 2023 2050 7265 7072 6f63 6573  .    # Preproces
+00019ff0: 7320 7468 6520 6163 7175 6972 6564 2064  s the acquired d
+0001a000: 6174 610d 0a20 2020 2064 6566 2070 7265  ata..    def pre
+0001a010: 7072 6f63 6573 7344 6174 6128 7365 6c66  processData(self
+0001a020: 2c20 6466 2c20 6461 7973 546f 4c6f 6f6b  , df, daysToLook
+0001a030: 6261 636b 3d4e 6f6e 6529 3a0d 0a20 2020  back=None):..   
+0001a040: 2020 2020 2061 7373 6572 7420 6973 696e       assert isin
+0001a050: 7374 616e 6365 2864 662c 2070 642e 4461  stance(df, pd.Da
+0001a060: 7461 4672 616d 6529 0d0a 2020 2020 2020  taFrame)..      
+0001a070: 2020 6461 7461 203d 2064 662e 636f 7079    data = df.copy
+0001a080: 2829 0d0a 2020 2020 2020 2020 7472 793a  ()..        try:
+0001a090: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
+0001a0a0: 7461 203d 2064 6174 612e 7265 706c 6163  ta = data.replac
+0001a0b0: 6528 6e70 2e69 6e66 2c20 6e70 2e6e 616e  e(np.inf, np.nan
+0001a0c0: 292e 7265 706c 6163 6528 2d6e 702e 696e  ).replace(-np.in
+0001a0d0: 662c 206e 702e 6e61 6e29 2e64 726f 706e  f, np.nan).dropn
+0001a0e0: 6128 686f 773d 2261 6c6c 2229 0d0a 2020  a(how="all")..  
+0001a0f0: 2020 2020 2020 2020 2020 2320 7365 6c66            # self
+0001a100: 2e64 6566 6175 6c74 5f6c 6f67 6765 722e  .default_logger.
+0001a110: 696e 666f 2866 2250 7265 7072 6f63 6573  info(f"Preproces
+0001a120: 7369 6e67 2064 6174 613a 5c6e 7b64 6174  sing data:\n{dat
+0001a130: 612e 6865 6164 2831 297d 5c6e 2229 0d0a  a.head(1)}\n")..
+0001a140: 2020 2020 2020 2020 2020 2020 6966 2064              if d
+0001a150: 6179 7354 6f4c 6f6f 6b62 6163 6b20 6973  aysToLookback is
+0001a160: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+0001a170: 2020 2020 2020 2020 6461 7973 546f 4c6f          daysToLo
+0001a180: 6f6b 6261 636b 203d 2073 656c 662e 636f  okback = self.co
+0001a190: 6e66 6967 4d61 6e61 6765 722e 6461 7973  nfigManager.days
+0001a1a0: 546f 4c6f 6f6b 6261 636b 0d0a 2020 2020  ToLookback..    
+0001a1b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0001a1c0: 636f 6e66 6967 4d61 6e61 6765 722e 7573  configManager.us
+0001a1d0: 6545 4d41 3a0d 0a20 2020 2020 2020 2020  eEMA:..         
+0001a1e0: 2020 2020 2020 2073 6d61 203d 2070 6b74         sma = pkt
+0001a1f0: 616c 6962 2e45 4d41 2864 6174 615b 2243  alib.EMA(data["C
+0001a200: 6c6f 7365 225d 2c20 7469 6d65 7065 7269  lose"], timeperi
+0001a210: 6f64 3d35 3029 0d0a 2020 2020 2020 2020  od=50)..        
+0001a220: 2020 2020 2020 2020 6c6d 6120 3d20 706b          lma = pk
+0001a230: 7461 6c69 622e 454d 4128 6461 7461 5b22  talib.EMA(data["
+0001a240: 436c 6f73 6522 5d2c 2074 696d 6570 6572  Close"], timeper
+0001a250: 696f 643d 3230 3029 0d0a 2020 2020 2020  iod=200)..      
+0001a260: 2020 2020 2020 2020 2020 7373 6d61 203d            ssma =
+0001a270: 2070 6b74 616c 6962 2e45 4d41 2864 6174   pktalib.EMA(dat
+0001a280: 615b 2243 6c6f 7365 225d 2c20 7469 6d65  a["Close"], time
+0001a290: 7065 7269 6f64 3d39 290d 0a20 2020 2020  period=9)..     
+0001a2a0: 2020 2020 2020 2020 2020 2064 6174 612e             data.
+0001a2b0: 696e 7365 7274 286c 656e 2864 6174 612e  insert(len(data.
+0001a2c0: 636f 6c75 6d6e 7329 2c20 2253 4d41 222c  columns), "SMA",
+0001a2d0: 2073 6d61 290d 0a20 2020 2020 2020 2020   sma)..         
+0001a2e0: 2020 2020 2020 2064 6174 612e 696e 7365         data.inse
+0001a2f0: 7274 286c 656e 2864 6174 612e 636f 6c75  rt(len(data.colu
+0001a300: 6d6e 7329 2c20 224c 4d41 222c 206c 6d61  mns), "LMA", lma
+0001a310: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001a320: 2020 2064 6174 612e 696e 7365 7274 286c     data.insert(l
+0001a330: 656e 2864 6174 612e 636f 6c75 6d6e 7329  en(data.columns)
+0001a340: 2c20 2253 534d 4122 2c20 7373 6d61 290d  , "SSMA", ssma).
+0001a350: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+0001a360: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0001a370: 2020 2020 736d 6120 3d20 706b 7461 6c69      sma = pktali
+0001a380: 622e 534d 4128 6461 7461 5b22 436c 6f73  b.SMA(data["Clos
+0001a390: 6522 5d2c 2074 696d 6570 6572 696f 643d  e"], timeperiod=
+0001a3a0: 3530 290d 0a20 2020 2020 2020 2020 2020  50)..           
+0001a3b0: 2020 2020 206c 6d61 203d 2070 6b74 616c       lma = pktal
+0001a3c0: 6962 2e53 4d41 2864 6174 615b 2243 6c6f  ib.SMA(data["Clo
+0001a3d0: 7365 225d 2c20 7469 6d65 7065 7269 6f64  se"], timeperiod
+0001a3e0: 3d32 3030 290d 0a20 2020 2020 2020 2020  =200)..         
+0001a3f0: 2020 2020 2020 2073 736d 6120 3d20 706b         ssma = pk
+0001a400: 7461 6c69 622e 534d 4128 6461 7461 5b22  talib.SMA(data["
+0001a410: 436c 6f73 6522 5d2c 2074 696d 6570 6572  Close"], timeper
+0001a420: 696f 643d 3929 0d0a 2020 2020 2020 2020  iod=9)..        
+0001a430: 2020 2020 2020 2020 6461 7461 2e69 6e73          data.ins
+0001a440: 6572 7428 6c65 6e28 6461 7461 2e63 6f6c  ert(len(data.col
+0001a450: 756d 6e73 292c 2022 534d 4122 2c20 736d  umns), "SMA", sm
+0001a460: 6129 0d0a 2020 2020 2020 2020 2020 2020  a)..            
+0001a470: 2020 2020 6461 7461 2e69 6e73 6572 7428      data.insert(
+0001a480: 6c65 6e28 6461 7461 2e63 6f6c 756d 6e73  len(data.columns
+0001a490: 292c 2022 4c4d 4122 2c20 6c6d 6129 0d0a  ), "LMA", lma)..
+0001a4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a4b0: 6461 7461 2e69 6e73 6572 7428 6c65 6e28  data.insert(len(
+0001a4c0: 6461 7461 2e63 6f6c 756d 6e73 292c 2022  data.columns), "
+0001a4d0: 5353 4d41 222c 2073 736d 6129 0d0a 2020  SSMA", ssma)..  
+0001a4e0: 2020 2020 2020 2020 2020 766f 6c20 3d20            vol = 
+0001a4f0: 706b 7461 6c69 622e 534d 4128 6461 7461  pktalib.SMA(data
+0001a500: 5b22 566f 6c75 6d65 225d 2c20 7469 6d65  ["Volume"], time
+0001a510: 7065 7269 6f64 3d32 3029 0d0a 2020 2020  period=20)..    
+0001a520: 2020 2020 2020 2020 7273 6920 3d20 706b          rsi = pk
+0001a530: 7461 6c69 622e 5253 4928 6461 7461 5b22  talib.RSI(data["
+0001a540: 436c 6f73 6522 5d2c 2074 696d 6570 6572  Close"], timeper
+0001a550: 696f 643d 3134 290d 0a20 2020 2020 2020  iod=14)..       
+0001a560: 2020 2020 2064 6174 612e 696e 7365 7274       data.insert
+0001a570: 286c 656e 2864 6174 612e 636f 6c75 6d6e  (len(data.column
+0001a580: 7329 2c20 2256 6f6c 4d41 222c 2076 6f6c  s), "VolMA", vol
+0001a590: 290d 0a20 2020 2020 2020 2020 2020 2064  )..            d
+0001a5a0: 6174 612e 696e 7365 7274 286c 656e 2864  ata.insert(len(d
+0001a5b0: 6174 612e 636f 6c75 6d6e 7329 2c20 2252  ata.columns), "R
+0001a5c0: 5349 222c 2072 7369 290d 0a20 2020 2020  SI", rsi)..     
+0001a5d0: 2020 2020 2020 2063 6369 203d 2070 6b74         cci = pkt
+0001a5e0: 616c 6962 2e43 4349 2864 6174 615b 2248  alib.CCI(data["H
+0001a5f0: 6967 6822 5d2c 2064 6174 615b 224c 6f77  igh"], data["Low
+0001a600: 225d 2c20 6461 7461 5b22 436c 6f73 6522  "], data["Close"
+0001a610: 5d2c 2074 696d 6570 6572 696f 643d 3134  ], timeperiod=14
+0001a620: 290d 0a20 2020 2020 2020 2020 2020 2064  )..            d
+0001a630: 6174 612e 696e 7365 7274 286c 656e 2864  ata.insert(len(d
+0001a640: 6174 612e 636f 6c75 6d6e 7329 2c20 2243  ata.columns), "C
+0001a650: 4349 222c 2063 6369 290d 0a20 2020 2020  CI", cci)..     
+0001a660: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
+0001a670: 2020 2020 2020 2020 2020 2020 2066 6173               fas
+0001a680: 746b 2c20 6661 7374 6420 3d20 706b 7461  tk, fastd = pkta
+0001a690: 6c69 622e 5354 4f43 4852 5349 280d 0a20  lib.STOCHRSI(.. 
+0001a6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a6b0: 2020 2064 6174 615b 2243 6c6f 7365 225d     data["Close"]
+0001a6c0: 2c20 7469 6d65 7065 7269 6f64 3d31 342c  , timeperiod=14,
+0001a6d0: 2066 6173 746b 5f70 6572 696f 643d 352c   fastk_period=5,
+0001a6e0: 2066 6173 7464 5f70 6572 696f 643d 332c   fastd_period=3,
+0001a6f0: 2066 6173 7464 5f6d 6174 7970 653d 300d   fastd_matype=0.
+0001a700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a710: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+0001a720: 2020 2020 6461 7461 2e69 6e73 6572 7428      data.insert(
+0001a730: 6c65 6e28 6461 7461 2e63 6f6c 756d 6e73  len(data.columns
+0001a740: 292c 2022 4641 5354 4b22 2c20 6661 7374  ), "FASTK", fast
+0001a750: 6b29 0d0a 2020 2020 2020 2020 2020 2020  k)..            
+0001a760: 2020 2020 6461 7461 2e69 6e73 6572 7428      data.insert(
+0001a770: 6c65 6e28 6461 7461 2e63 6f6c 756d 6e73  len(data.columns
+0001a780: 292c 2022 4641 5354 4422 2c20 6661 7374  ), "FASTD", fast
+0001a790: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
+0001a7a0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+0001a7b0: 2061 7320 653a 0d0a 2020 2020 2020 2020   as e:..        
+0001a7c0: 2020 2020 2020 2020 7365 6c66 2e64 6566          self.def
+0001a7d0: 6175 6c74 5f6c 6f67 6765 722e 6465 6275  ault_logger.debu
+0001a7e0: 6728 652c 2065 7863 5f69 6e66 6f3d 5472  g(e, exc_info=Tr
+0001a7f0: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
+0001a800: 2020 2020 2070 6173 730d 0a20 2020 2020       pass..     
+0001a810: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+0001a820: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
+0001a830: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001a840: 6465 6661 756c 745f 6c6f 6767 6572 2e64  default_logger.d
+0001a850: 6562 7567 2865 2c20 6578 635f 696e 666f  ebug(e, exc_info
+0001a860: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
+0001a870: 2020 2020 2020 2020 7061 7373 0d0a 2020          pass..  
 0001a880: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-0001a890: 612e 6669 6c6c 6e61 2830 290d 0a20 2020  a.fillna(0)..   
-0001a8a0: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
-0001a8b0: 2e72 6570 6c61 6365 285b 6e70 2e69 6e66  .replace([np.inf
-0001a8c0: 2c20 2d6e 702e 696e 665d 2c20 3029 0d0a  , -np.inf], 0)..
-0001a8d0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-0001a8e0: 6174 615b 3a3a 2d31 5d20 2023 2052 6576  ata[::-1]  # Rev
-0001a8f0: 6572 7365 2074 6865 2064 6174 6166 7261  erse the datafra
-0001a900: 6d65 2073 6f20 7468 6174 2069 7473 2074  me so that its t
-0001a910: 6865 206f 6c64 6573 7420 6461 7465 2066  he oldest date f
-0001a920: 6972 7374 0d0a 2020 2020 2020 2020 6461  irst..        da
-0001a930: 7461 5b22 534d 4132 3022 5d20 3d20 706b  ta["SMA20"] = pk
-0001a940: 7461 6c69 622e 534d 4128 6461 7461 5b22  talib.SMA(data["
-0001a950: 436c 6f73 6522 5d2c 2032 3029 0d0a 2020  Close"], 20)..  
-0001a960: 2020 2020 2020 6461 7461 5b22 534d 4132        data["SMA2
-0001a970: 3056 225d 203d 2070 6b74 616c 6962 2e53  0V"] = pktalib.S
-0001a980: 4d41 2864 6174 615b 2256 6f6c 756d 6522  MA(data["Volume"
-0001a990: 5d2c 2032 3029 0d0a 2020 2020 2020 2020  ], 20)..        
-0001a9a0: 6461 7461 203d 2064 6174 615b 0d0a 2020  data = data[..  
-0001a9b0: 2020 2020 2020 2020 2020 3a3a 2d31 0d0a            ::-1..
-0001a9c0: 2020 2020 2020 2020 5d20 2023 2052 6576          ]  # Rev
-0001a9d0: 6572 7365 2074 6865 2064 6174 6166 7261  erse the datafra
-0001a9e0: 6d65 2073 6f20 7468 6174 2069 7427 7320  me so that it's 
-0001a9f0: 7468 6520 6d6f 7374 2072 6563 656e 7420  the most recent 
-0001aa00: 6461 7465 2066 6972 7374 0d0a 2020 2020  date first..    
-0001aa10: 2020 2020 7265 6365 6e74 203d 2064 6174      recent = dat
-0001aa20: 612e 6865 6164 2833 290d 0a20 2020 2020  a.head(3)..     
-0001aa30: 2020 2069 6620 6c65 6e28 7265 6365 6e74     if len(recent
-0001aa40: 2920 3c20 333a 0d0a 2020 2020 2020 2020  ) < 3:..        
-0001aa50: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-0001aa60: 0d0a 2020 2020 2020 2020 636f 6e64 3120  ..        cond1 
-0001aa70: 3d20 7265 6365 6e74 5b22 436c 6f73 6522  = recent["Close"
-0001aa80: 5d2e 696c 6f63 5b30 5d20 3e20 7265 6365  ].iloc[0] > rece
-0001aa90: 6e74 5b22 436c 6f73 6522 5d2e 696c 6f63  nt["Close"].iloc
-0001aaa0: 5b31 5d0d 0a20 2020 2020 2020 2063 6f6e  [1]..        con
-0001aab0: 6432 203d 2063 6f6e 6431 2061 6e64 2028  d2 = cond1 and (
-0001aac0: 7265 6365 6e74 5b22 436c 6f73 6522 5d2e  recent["Close"].
-0001aad0: 696c 6f63 5b30 5d20 3e20 7265 6365 6e74  iloc[0] > recent
-0001aae0: 5b22 534d 4132 3022 5d2e 696c 6f63 5b30  ["SMA20"].iloc[0
-0001aaf0: 5d29 0d0a 2020 2020 2020 2020 636f 6e64  ])..        cond
-0001ab00: 3320 3d20 636f 6e64 3220 616e 6420 2872  3 = cond2 and (r
-0001ab10: 6563 656e 745b 2243 6c6f 7365 225d 2e69  ecent["Close"].i
-0001ab20: 6c6f 635b 315d 203e 2072 6563 656e 745b  loc[1] > recent[
-0001ab30: 2248 6967 6822 5d2e 696c 6f63 5b32 5d29  "High"].iloc[2])
-0001ab40: 0d0a 2020 2020 2020 2020 636f 6e64 3420  ..        cond4 
-0001ab50: 3d20 636f 6e64 3320 616e 6420 2872 6563  = cond3 and (rec
-0001ab60: 656e 745b 2256 6f6c 756d 6522 5d2e 696c  ent["Volume"].il
-0001ab70: 6f63 5b30 5d20 3e20 7265 6365 6e74 5b22  oc[0] > recent["
-0001ab80: 534d 4132 3056 225d 2e69 6c6f 635b 305d  SMA20V"].iloc[0]
-0001ab90: 290d 0a20 2020 2020 2020 2063 6f6e 6435  )..        cond5
-0001aba0: 203d 2063 6f6e 6434 2061 6e64 2028 7265   = cond4 and (re
-0001abb0: 6365 6e74 5b22 566f 6c75 6d65 225d 2e69  cent["Volume"].i
-0001abc0: 6c6f 635b 315d 203e 2072 6563 656e 745b  loc[1] > recent[
-0001abd0: 2253 4d41 3230 5622 5d2e 696c 6f63 5b30  "SMA20V"].iloc[0
-0001abe0: 5d29 0d0a 2020 2020 2020 2020 7265 7475  ])..        retu
-0001abf0: 726e 2063 6f6e 6435 0d0a 0d0a 2020 2020  rn cond5....    
-0001ac00: 6465 6620 7661 6c69 6461 7465 4275 6c6c  def validateBull
-0001ac10: 6973 6846 6f72 546f 6d6f 7272 6f77 2873  ishForTomorrow(s
-0001ac20: 656c 662c 2064 6629 3a0d 0a20 2020 2020  elf, df):..     
-0001ac30: 2020 2069 6620 6466 2069 7320 4e6f 6e65     if df is None
-0001ac40: 206f 7220 6c65 6e28 6466 2920 3d3d 2030   or len(df) == 0
-0001ac50: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-0001ac60: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
-0001ac70: 2020 2020 2064 6174 6120 3d20 6466 2e63       data = df.c
-0001ac80: 6f70 7928 290d 0a20 2020 2020 2020 2023  opy()..        #
-0001ac90: 2068 7474 7073 3a2f 2f63 6861 7274 696e   https://chartin
-0001aca0: 6b2e 636f 6d2f 7363 7265 656e 6572 2f62  k.com/screener/b
-0001acb0: 756c 6c69 7368 2d66 6f72 2d74 6f6d 6f72  ullish-for-tomor
-0001acc0: 726f 770d 0a20 2020 2020 2020 2064 6174  row..        dat
-0001acd0: 6120 3d20 6461 7461 2e66 696c 6c6e 6128  a = data.fillna(
-0001ace0: 3029 0d0a 2020 2020 2020 2020 6461 7461  0)..        data
-0001acf0: 203d 2064 6174 612e 7265 706c 6163 6528   = data.replace(
-0001ad00: 5b6e 702e 696e 662c 202d 6e70 2e69 6e66  [np.inf, -np.inf
-0001ad10: 5d2c 2030 290d 0a20 2020 2020 2020 2064  ], 0)..        d
-0001ad20: 6174 6120 3d20 6461 7461 5b3a 3a2d 315d  ata = data[::-1]
-0001ad30: 2020 2320 5265 7665 7273 6520 7468 6520    # Reverse the 
-0001ad40: 6461 7461 6672 616d 6520 736f 2074 6861  dataframe so tha
-0001ad50: 7420 6974 7320 7468 6520 6f6c 6465 7374  t its the oldest
-0001ad60: 2064 6174 6520 6669 7273 740d 0a20 2020   date first..   
-0001ad70: 2020 2020 206d 6163 644c 696e 6520 3d20       macdLine = 
-0001ad80: 706b 7461 6c69 622e 4d41 4344 2864 6174  pktalib.MACD(dat
-0001ad90: 615b 2243 6c6f 7365 225d 2c20 3132 2c20  a["Close"], 12, 
-0001ada0: 3236 2c20 3929 5b30 5d2e 7461 696c 2833  26, 9)[0].tail(3
-0001adb0: 290d 0a20 2020 2020 2020 206d 6163 6453  )..        macdS
-0001adc0: 6967 6e61 6c20 3d20 706b 7461 6c69 622e  ignal = pktalib.
-0001add0: 4d41 4344 2864 6174 615b 2243 6c6f 7365  MACD(data["Close
-0001ade0: 225d 2c20 3132 2c20 3236 2c20 3929 5b31  "], 12, 26, 9)[1
-0001adf0: 5d2e 7461 696c 2833 290d 0a20 2020 2020  ].tail(3)..     
-0001ae00: 2020 206d 6163 6448 6973 7420 3d20 706b     macdHist = pk
-0001ae10: 7461 6c69 622e 4d41 4344 2864 6174 615b  talib.MACD(data[
-0001ae20: 2243 6c6f 7365 225d 2c20 3132 2c20 3236  "Close"], 12, 26
-0001ae30: 2c20 3929 5b32 5d2e 7461 696c 2833 290d  , 9)[2].tail(3).
-0001ae40: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
-0001ae50: 6e20 280d 0a20 2020 2020 2020 2020 2020  n (..           
-0001ae60: 2028 6d61 6364 4869 7374 2e69 6c6f 635b   (macdHist.iloc[
-0001ae70: 3a31 5d2e 696c 6f63 5b30 5d20 3c20 6d61  :1].iloc[0] < ma
-0001ae80: 6364 4869 7374 2e69 6c6f 635b 3a32 5d2e  cdHist.iloc[:2].
-0001ae90: 696c 6f63 5b31 5d29 0d0a 2020 2020 2020  iloc[1])..      
-0001aea0: 2020 2020 2020 616e 6420 286d 6163 6448        and (macdH
-0001aeb0: 6973 742e 696c 6f63 5b3a 335d 2e69 6c6f  ist.iloc[:3].ilo
-0001aec0: 635b 325d 203e 206d 6163 6448 6973 742e  c[2] > macdHist.
-0001aed0: 696c 6f63 5b3a 325d 2e69 6c6f 635b 315d  iloc[:2].iloc[1]
-0001aee0: 290d 0a20 2020 2020 2020 2020 2020 2061  )..            a
-0001aef0: 6e64 2028 0d0a 2020 2020 2020 2020 2020  nd (..          
-0001af00: 2020 2020 2020 286d 6163 644c 696e 652e        (macdLine.
-0001af10: 696c 6f63 5b3a 335d 2e69 6c6f 635b 325d  iloc[:3].iloc[2]
-0001af20: 202d 206d 6163 6453 6967 6e61 6c2e 696c   - macdSignal.il
-0001af30: 6f63 5b3a 335d 2e69 6c6f 635b 325d 290d  oc[:3].iloc[2]).
-0001af40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001af50: 202d 2028 6d61 6364 4c69 6e65 2e69 6c6f   - (macdLine.ilo
-0001af60: 635b 3a32 5d2e 696c 6f63 5b31 5d20 2d20  c[:2].iloc[1] - 
-0001af70: 6d61 6364 5369 676e 616c 2e69 6c6f 635b  macdSignal.iloc[
-0001af80: 3a32 5d2e 696c 6f63 5b31 5d29 0d0a 2020  :2].iloc[1])..  
-0001af90: 2020 2020 2020 2020 2020 2020 2020 3e3d                >=
-0001afa0: 2030 2e34 0d0a 2020 2020 2020 2020 2020   0.4..          
-0001afb0: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-0001afc0: 2061 6e64 2028 0d0a 2020 2020 2020 2020   and (..        
-0001afd0: 2020 2020 2020 2020 286d 6163 644c 696e          (macdLin
-0001afe0: 652e 696c 6f63 5b3a 325d 2e69 6c6f 635b  e.iloc[:2].iloc[
-0001aff0: 315d 202d 206d 6163 6453 6967 6e61 6c2e  1] - macdSignal.
-0001b000: 696c 6f63 5b3a 325d 2e69 6c6f 635b 315d  iloc[:2].iloc[1]
-0001b010: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0001b020: 2020 202d 2028 6d61 6364 4c69 6e65 2e69     - (macdLine.i
-0001b030: 6c6f 635b 3a31 5d2e 696c 6f63 5b30 5d20  loc[:1].iloc[0] 
-0001b040: 2d20 6d61 6364 5369 676e 616c 2e69 6c6f  - macdSignal.ilo
-0001b050: 635b 3a31 5d2e 696c 6f63 5b30 5d29 0d0a  c[:1].iloc[0])..
-0001b060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b070: 3c3d 2030 2e32 0d0a 2020 2020 2020 2020  <= 0.2..        
-0001b080: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-0001b090: 2020 2061 6e64 2028 6d61 6364 4c69 6e65     and (macdLine
-0001b0a0: 2e69 6c6f 635b 3a33 5d2e 696c 6f63 5b32  .iloc[:3].iloc[2
-0001b0b0: 5d20 3e20 6d61 6364 5369 676e 616c 2e69  ] > macdSignal.i
-0001b0c0: 6c6f 635b 3a33 5d2e 696c 6f63 5b32 5d29  loc[:3].iloc[2])
-0001b0d0: 0d0a 2020 2020 2020 2020 2020 2020 616e  ..            an
-0001b0e0: 6420 280d 0a20 2020 2020 2020 2020 2020  d (..           
-0001b0f0: 2020 2020 2028 6d61 6364 4c69 6e65 2e69       (macdLine.i
-0001b100: 6c6f 635b 3a33 5d2e 696c 6f63 5b32 5d20  loc[:3].iloc[2] 
-0001b110: 2d20 6d61 6364 5369 676e 616c 2e69 6c6f  - macdSignal.ilo
-0001b120: 635b 3a33 5d2e 696c 6f63 5b32 5d29 0d0a  c[:3].iloc[2])..
-0001b130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b140: 2d20 286d 6163 644c 696e 652e 696c 6f63  - (macdLine.iloc
-0001b150: 5b3a 325d 2e69 6c6f 635b 315d 202d 206d  [:2].iloc[1] - m
-0001b160: 6163 6453 6967 6e61 6c2e 696c 6f63 5b3a  acdSignal.iloc[:
-0001b170: 325d 2e69 6c6f 635b 315d 290d 0a20 2020  2].iloc[1])..   
-0001b180: 2020 2020 2020 2020 2020 2020 203c 2031               < 1
-0001b190: 0d0a 2020 2020 2020 2020 2020 2020 290d  ..            ).
-0001b1a0: 0a20 2020 2020 2020 2029 0d0a 0d0a 2020  .        )....  
-0001b1b0: 2020 2340 6d65 6173 7572 655f 7469 6d65    #@measure_time
-0001b1c0: 0d0a 2020 2020 2320 7661 6c69 6461 7465  ..    # validate
-0001b1d0: 2069 6620 4343 4920 6973 2077 6974 6869   if CCI is withi
-0001b1e0: 6e20 6769 7665 6e20 7261 6e67 650d 0a20  n given range.. 
-0001b1f0: 2020 2064 6566 2076 616c 6964 6174 6543     def validateC
-0001b200: 4349 2873 656c 662c 2064 662c 2073 6372  CI(self, df, scr
-0001b210: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
-0001b220: 742c 206d 696e 4343 492c 206d 6178 4343  t, minCCI, maxCC
-0001b230: 4929 3a0d 0a20 2020 2020 2020 2069 6620  I):..        if 
-0001b240: 6466 2069 7320 4e6f 6e65 206f 7220 6c65  df is None or le
-0001b250: 6e28 6466 2920 3d3d 2030 3a0d 0a20 2020  n(df) == 0:..   
-0001b260: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0001b270: 4661 6c73 650d 0a20 2020 2020 2020 2064  False..        d
-0001b280: 6174 6120 3d20 6466 2e63 6f70 7928 290d  ata = df.copy().
-0001b290: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-0001b2a0: 6461 7461 2e66 696c 6c6e 6128 3029 0d0a  data.fillna(0)..
-0001b2b0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-0001b2c0: 6174 612e 7265 706c 6163 6528 5b6e 702e  ata.replace([np.
-0001b2d0: 696e 662c 202d 6e70 2e69 6e66 5d2c 2030  inf, -np.inf], 0
-0001b2e0: 290d 0a20 2020 2020 2020 2063 6369 203d  )..        cci =
-0001b2f0: 2069 6e74 2864 6174 612e 6865 6164 2831   int(data.head(1
-0001b300: 295b 2243 4349 225d 2e69 6c6f 635b 305d  )["CCI"].iloc[0]
-0001b310: 290d 0a20 2020 2020 2020 2073 6176 6544  )..        saveD
-0001b320: 6963 745b 2243 4349 225d 203d 2063 6369  ict["CCI"] = cci
-0001b330: 0d0a 2020 2020 2020 2020 6966 2028 6363  ..        if (cc
-0001b340: 6920 3e3d 206d 696e 4343 4920 616e 6420  i >= minCCI and 
-0001b350: 6363 6920 3c3d 206d 6178 4343 4929 3a0d  cci <= maxCCI):.
-0001b360: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0001b370: 2822 5570 2220 696e 2073 6176 6544 6963  ("Up" in saveDic
-0001b380: 745b 2254 7265 6e64 225d 293a 0d0a 2020  t["Trend"]):..  
-0001b390: 2020 2020 2020 2020 2020 2020 2020 7363                sc
-0001b3a0: 7265 656e 4469 6374 5b22 4343 4922 5d20  reenDict["CCI"] 
-0001b3b0: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
-0001b3c0: 2020 2020 2020 2020 2028 636f 6c6f 7254           (colorT
-0001b3d0: 6578 742e 424f 4c44 2069 6620 2822 5374  ext.BOLD if ("St
-0001b3e0: 726f 6e67 2220 696e 2073 6176 6544 6963  rong" in saveDic
-0001b3f0: 745b 2254 7265 6e64 225d 2920 656c 7365  t["Trend"]) else
-0001b400: 2022 2229 202b 2063 6f6c 6f72 5465 7874   "") + colorText
-0001b410: 2e47 5245 454e 202b 2073 7472 2863 6369  .GREEN + str(cci
-0001b420: 2920 2b20 636f 6c6f 7254 6578 742e 454e  ) + colorText.EN
-0001b430: 440d 0a20 2020 2020 2020 2020 2020 2020  D..             
-0001b440: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
-0001b450: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-0001b460: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-0001b470: 6963 745b 2243 4349 225d 203d 2028 0d0a  ict["CCI"] = (..
-0001b480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b490: 2020 2020 2863 6f6c 6f72 5465 7874 2e42      (colorText.B
-0001b4a0: 4f4c 4420 6966 2028 2253 7472 6f6e 6722  OLD if ("Strong"
-0001b4b0: 2069 6e20 7361 7665 4469 6374 5b22 5472   in saveDict["Tr
-0001b4c0: 656e 6422 5d29 2065 6c73 6520 2222 2920  end"]) else "") 
-0001b4d0: 2b20 636f 6c6f 7254 6578 742e 4641 494c  + colorText.FAIL
-0001b4e0: 202b 2073 7472 2863 6369 2920 2b20 636f   + str(cci) + co
-0001b4f0: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
-0001b500: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
-0001b510: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0001b520: 726e 2054 7275 650d 0a20 2020 2020 2020  rn True..       
-0001b530: 2073 6372 6565 6e44 6963 745b 2243 4349   screenDict["CCI
-0001b540: 225d 203d 2063 6f6c 6f72 5465 7874 2e42  "] = colorText.B
-0001b550: 4f4c 4420 2b20 636f 6c6f 7254 6578 742e  OLD + colorText.
-0001b560: 4641 494c 202b 2073 7472 2863 6369 2920  FAIL + str(cci) 
-0001b570: 2b20 636f 6c6f 7254 6578 742e 454e 440d  + colorText.END.
-0001b580: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001b590: 4661 6c73 650d 0a0d 0a20 2020 2023 2046  False....    # F
-0001b5a0: 696e 6420 436f 6e66 6c75 6365 6e63 650d  ind Conflucence.
-0001b5b0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-0001b5c0: 6543 6f6e 666c 7565 6e63 6528 7365 6c66  eConfluence(self
-0001b5d0: 2c20 7374 6f63 6b2c 2064 662c 2073 6372  , stock, df, scr
-0001b5e0: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
-0001b5f0: 742c 2070 6572 6365 6e74 6167 653d 302e  t, percentage=0.
-0001b600: 312c 636f 6e66 4669 6c74 6572 3d33 293a  1,confFilter=3):
-0001b610: 0d0a 2020 2020 2020 2020 6966 2064 6620  ..        if df 
-0001b620: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
-0001b630: 6629 203d 3d20 303a 0d0a 2020 2020 2020  f) == 0:..      
-0001b640: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-0001b650: 7365 0d0a 2020 2020 2020 2020 6461 7461  se..        data
-0001b660: 203d 2064 662e 636f 7079 2829 0d0a 2020   = df.copy()..  
-0001b670: 2020 2020 2020 7265 6365 6e74 203d 2064        recent = d
-0001b680: 6174 612e 6865 6164 2832 290d 0a20 2020  ata.head(2)..   
-0001b690: 2020 2020 2069 6620 6c65 6e28 7265 6365       if len(rece
-0001b6a0: 6e74 2920 3c20 323a 0d0a 2020 2020 2020  nt) < 2:..      
-0001b6b0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-0001b6c0: 7365 0d0a 2020 2020 2020 2020 6973 3530  se..        is50
-0001b6d0: 444d 4155 7054 7265 6e64 203d 2028 7265  DMAUpTrend = (re
-0001b6e0: 6365 6e74 5b22 534d 4122 5d2e 696c 6f63  cent["SMA"].iloc
-0001b6f0: 5b30 5d20 3e20 7265 6365 6e74 5b22 534d  [0] > recent["SM
-0001b700: 4122 5d2e 696c 6f63 5b31 5d29 0d0a 2020  A"].iloc[1])..  
-0001b710: 2020 2020 2020 6973 3530 444d 4144 6f77        is50DMADow
-0001b720: 6e54 7265 6e64 203d 2028 7265 6365 6e74  nTrend = (recent
-0001b730: 5b22 534d 4122 5d2e 696c 6f63 5b30 5d20  ["SMA"].iloc[0] 
-0001b740: 3c20 7265 6365 6e74 5b22 534d 4122 5d2e  < recent["SMA"].
-0001b750: 696c 6f63 5b31 5d29 0d0a 2020 2020 2020  iloc[1])..      
-0001b760: 2020 6973 476f 6c64 656e 4372 6f73 734f    isGoldenCrossO
-0001b770: 7665 7220 3d20 2872 6563 656e 745b 2253  ver = (recent["S
-0001b780: 4d41 225d 2e69 6c6f 635b 305d 203e 3d20  MA"].iloc[0] >= 
-0001b790: 7265 6365 6e74 5b22 4c4d 4122 5d2e 696c  recent["LMA"].il
-0001b7a0: 6f63 5b30 5d29 2061 6e64 205c 0d0a 2020  oc[0]) and \..  
-0001b7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b7c0: 2020 2020 2020 2020 2020 2872 6563 656e            (recen
-0001b7d0: 745b 2253 4d41 225d 2e69 6c6f 635b 315d  t["SMA"].iloc[1]
-0001b7e0: 203c 3d20 7265 6365 6e74 5b22 4c4d 4122   <= recent["LMA"
-0001b7f0: 5d2e 696c 6f63 5b31 5d29 0d0a 2020 2020  ].iloc[1])..    
-0001b800: 2020 2020 6973 4465 6164 4372 6f73 734f      isDeadCrossO
-0001b810: 7665 7220 3d20 2872 6563 656e 745b 2253  ver = (recent["S
-0001b820: 4d41 225d 2e69 6c6f 635b 305d 203c 3d20  MA"].iloc[0] <= 
-0001b830: 7265 6365 6e74 5b22 4c4d 4122 5d2e 696c  recent["LMA"].il
-0001b840: 6f63 5b30 5d29 2061 6e64 205c 0d0a 2020  oc[0]) and \..  
-0001b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b860: 2020 2020 2020 2020 2020 2872 6563 656e            (recen
-0001b870: 745b 2253 4d41 225d 2e69 6c6f 635b 315d  t["SMA"].iloc[1]
-0001b880: 203e 3d20 7265 6365 6e74 5b22 4c4d 4122   >= recent["LMA"
-0001b890: 5d2e 696c 6f63 5b31 5d29 0d0a 2020 2020  ].iloc[1])..    
-0001b8a0: 2020 2020 6973 3530 444d 4120 3d20 2872      is50DMA = (r
-0001b8b0: 6563 656e 745b 2253 4d41 225d 2e69 6c6f  ecent["SMA"].ilo
-0001b8c0: 635b 305d 203c 3d20 7265 6365 6e74 5b22  c[0] <= recent["
-0001b8d0: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d29  Close"].iloc[0])
-0001b8e0: 0d0a 2020 2020 2020 2020 6973 3230 3044  ..        is200D
-0001b8f0: 4d41 203d 2028 7265 6365 6e74 5b22 4c4d  MA = (recent["LM
-0001b900: 4122 5d2e 696c 6f63 5b30 5d20 3c3d 2072  A"].iloc[0] <= r
-0001b910: 6563 656e 745b 2243 6c6f 7365 225d 2e69  ecent["Close"].i
-0001b920: 6c6f 635b 305d 290d 0a20 2020 2020 2020  loc[0])..       
-0001b930: 2064 6966 6665 7265 6e63 6520 3d20 726f   difference = ro
-0001b940: 756e 6428 2872 6563 656e 745b 2253 4d41  und((recent["SMA
-0001b950: 225d 2e69 6c6f 635b 305d 202d 2072 6563  "].iloc[0] - rec
-0001b960: 656e 745b 224c 4d41 225d 2e69 6c6f 635b  ent["LMA"].iloc[
-0001b970: 305d 290d 0a20 2020 2020 2020 2020 2020  0])..           
-0001b980: 2020 2020 202f 2072 6563 656e 745b 2243       / recent["C
-0001b990: 6c6f 7365 225d 2e69 6c6f 635b 305d 0d0a  lose"].iloc[0]..
-0001b9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b9b0: 2a20 3130 302c 0d0a 2020 2020 2020 2020  * 100,..        
-0001b9c0: 2020 2020 2020 2020 322c 0d0a 2020 2020          2,..    
-0001b9d0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-0001b9e0: 2020 2073 6176 6544 6963 745b 2243 6f6e     saveDict["Con
-0001b9f0: 6644 4d41 4469 6666 6572 656e 6365 225d  fDMADifference"]
-0001ba00: 203d 2064 6966 6665 7265 6e63 650d 0a20   = difference.. 
-0001ba10: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
-0001ba20: 745b 2243 6f6e 6644 4d41 4469 6666 6572  t["ConfDMADiffer
-0001ba30: 656e 6365 225d 203d 2064 6966 6665 7265  ence"] = differe
-0001ba40: 6e63 650d 0a20 2020 2020 2020 2073 6176  nce..        sav
-0001ba50: 6564 203d 2073 656c 662e 6669 6e64 4375  ed = self.findCu
-0001ba60: 7272 656e 7453 6176 6564 5661 6c75 6528  rrentSavedValue(
-0001ba70: 7363 7265 656e 4469 6374 2c73 6176 6544  screenDict,saveD
-0001ba80: 6963 742c 224d 412d 5369 676e 616c 2229  ict,"MA-Signal")
-0001ba90: 0d0a 2020 2020 2020 2020 2320 6469 6666  ..        # diff
-0001baa0: 6572 656e 6365 203d 2061 6273 2864 6966  erence = abs(dif
-0001bab0: 6665 7265 6e63 6529 0d0a 2020 2020 2020  ference)..      
-0001bac0: 2020 636f 6e66 5465 7874 203d 2066 227b    confText = f"{
-0001bad0: 2747 6f6c 6465 6e43 726f 7373 6f76 6572  'GoldenCrossover
-0001bae0: 2720 6966 2069 7347 6f6c 6465 6e43 726f  ' if isGoldenCro
-0001baf0: 7373 4f76 6572 2065 6c73 6520 2827 4465  ssOver else ('De
-0001bb00: 6164 4372 6f73 736f 7665 7227 2069 6620  adCrossover' if 
-0001bb10: 6973 4465 6164 4372 6f73 734f 7665 7220  isDeadCrossOver 
-0001bb20: 656c 7365 2028 2743 6f6e 662e 5570 2720  else ('Conf.Up' 
-0001bb30: 6966 2069 7335 3044 4d41 5570 5472 656e  if is50DMAUpTren
-0001bb40: 6420 656c 7365 2028 2743 6f6e 662e 446f  d else ('Conf.Do
-0001bb50: 776e 2720 6966 2069 7335 3044 4d41 446f  wn' if is50DMADo
-0001bb60: 776e 5472 656e 6420 656c 7365 2028 2735  wnTrend else ('5
-0001bb70: 3044 4d41 2720 6966 2069 7335 3044 4d41  0DMA' if is50DMA
-0001bb80: 2065 6c73 6520 2827 3230 3044 4d41 2720   else ('200DMA' 
-0001bb90: 6966 2069 7332 3030 444d 4120 656c 7365  if is200DMA else
-0001bba0: 2027 556e 6b6e 6f77 6e27 2929 2929 297d   'Unknown')))))}
-0001bbb0: 220d 0a20 2020 2020 2020 2069 6620 6162  "..        if ab
-0001bbc0: 7328 7265 6365 6e74 5b22 534d 4122 5d2e  s(recent["SMA"].
-0001bbd0: 696c 6f63 5b30 5d20 2d20 7265 6365 6e74  iloc[0] - recent
-0001bbe0: 5b22 4c4d 4122 5d2e 696c 6f63 5b30 5d29  ["LMA"].iloc[0])
-0001bbf0: 203c 3d20 280d 0a20 2020 2020 2020 2020   <= (..         
-0001bc00: 2020 2072 6563 656e 745b 2253 4d41 225d     recent["SMA"]
-0001bc10: 2e69 6c6f 635b 305d 202a 2070 6572 6365  .iloc[0] * perce
-0001bc20: 6e74 6167 650d 0a20 2020 2020 2020 2029  ntage..        )
-0001bc30: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-0001bc40: 6620 7265 6365 6e74 5b22 534d 4122 5d2e  f recent["SMA"].
-0001bc50: 696c 6f63 5b30 5d20 3e3d 2072 6563 656e  iloc[0] >= recen
-0001bc60: 745b 224c 4d41 225d 2e69 6c6f 635b 305d  t["LMA"].iloc[0]
-0001bc70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001bc80: 2020 2073 6372 6565 6e44 6963 745b 224d     screenDict["M
-0001bc90: 412d 5369 676e 616c 225d 203d 2028 0d0a  A-Signal"] = (..
-0001bca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bcb0: 2020 2020 7361 7665 645b 305d 200d 0a20      saved[0] .. 
-0001bcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bcd0: 2020 202b 2063 6f6c 6f72 5465 7874 2e42     + colorText.B
-0001bce0: 4f4c 440d 0a20 2020 2020 2020 2020 2020  OLD..           
-0001bcf0: 2020 2020 2020 2020 202b 2028 636f 6c6f           + (colo
-0001bd00: 7254 6578 742e 4752 4545 4e20 6966 2069  rText.GREEN if i
-0001bd10: 7335 3044 4d41 5570 5472 656e 6420 656c  s50DMAUpTrend el
-0001bd20: 7365 2028 636f 6c6f 7254 6578 742e 4641  se (colorText.FA
-0001bd30: 494c 2069 6620 6973 3530 444d 4144 6f77  IL if is50DMADow
-0001bd40: 6e54 7265 6e64 2065 6c73 6520 636f 6c6f  nTrend else colo
-0001bd50: 7254 6578 742e 5741 524e 2929 0d0a 2020  rText.WARN))..  
-0001bd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bd70: 2020 2b20 6622 7b63 6f6e 6654 6578 747d    + f"{confText}
-0001bd80: 2028 7b64 6966 6665 7265 6e63 657d 2529   ({difference}%)
-0001bd90: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-0001bda0: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
-0001bdb0: 7874 2e45 4e44 0d0a 2020 2020 2020 2020  xt.END..        
-0001bdc0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-0001bdd0: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
-0001bde0: 6963 745b 224d 412d 5369 676e 616c 225d  ict["MA-Signal"]
-0001bdf0: 203d 2073 6176 6564 5b31 5d20 2b20 6622   = saved[1] + f"
-0001be00: 7b63 6f6e 6654 6578 747d 2028 7b64 6966  {confText} ({dif
-0001be10: 6665 7265 6e63 657d 2529 220d 0a20 2020  ference}%)"..   
-0001be20: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-0001be30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001be40: 7363 7265 656e 4469 6374 5b22 4d41 2d53  screenDict["MA-S
-0001be50: 6967 6e61 6c22 5d20 3d20 280d 0a20 2020  ignal"] = (..   
-0001be60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001be70: 2073 6176 6564 5b30 5d20 0d0a 2020 2020   saved[0] ..    
-0001be80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001be90: 2b20 636f 6c6f 7254 6578 742e 424f 4c44  + colorText.BOLD
-0001bea0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001beb0: 2020 2020 2020 2b20 2863 6f6c 6f72 5465        + (colorTe
-0001bec0: 7874 2e47 5245 454e 2069 6620 6973 3530  xt.GREEN if is50
-0001bed0: 444d 4155 7054 7265 6e64 2065 6c73 6520  DMAUpTrend else 
-0001bee0: 2863 6f6c 6f72 5465 7874 2e46 4149 4c20  (colorText.FAIL 
-0001bef0: 6966 2069 7335 3044 4d41 446f 776e 5472  if is50DMADownTr
-0001bf00: 656e 6420 656c 7365 2063 6f6c 6f72 5465  end else colorTe
-0001bf10: 7874 2e57 4152 4e29 290d 0a20 2020 2020  xt.WARN))..     
-0001bf20: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-0001bf30: 2066 227b 636f 6e66 5465 7874 7d20 287b   f"{confText} ({
-0001bf40: 6469 6666 6572 656e 6365 7d25 2922 0d0a  difference}%)"..
-0001bf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bf60: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
-0001bf70: 454e 440d 0a20 2020 2020 2020 2020 2020  END..           
-0001bf80: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-0001bf90: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
-0001bfa0: 5b22 4d41 2d53 6967 6e61 6c22 5d20 3d20  ["MA-Signal"] = 
-0001bfb0: 7361 7665 645b 315d 202b 2066 227b 636f  saved[1] + f"{co
-0001bfc0: 6e66 5465 7874 7d20 287b 6469 6666 6572  nfText} ({differ
-0001bfd0: 656e 6365 7d25 2922 0d0a 2020 2020 2020  ence}%)"..      
-0001bfe0: 2020 2020 2020 7265 7475 726e 2063 6f6e        return con
-0001bff0: 6646 696c 7465 7220 3d3d 2033 206f 7220  fFilter == 3 or 
-0001c000: 5c0d 0a20 2020 2020 2020 2020 2020 2020  \..             
-0001c010: 2020 2028 636f 6e66 4669 6c74 6572 203d     (confFilter =
-0001c020: 3d20 3120 616e 6420 2869 7335 3044 4d41  = 1 and (is50DMA
-0001c030: 5570 5472 656e 6420 6f72 2028 6973 476f  UpTrend or (isGo
-0001c040: 6c64 656e 4372 6f73 734f 7665 7220 6f72  ldenCrossOver or
-0001c050: 2027 5570 2720 696e 2063 6f6e 6654 6578   'Up' in confTex
-0001c060: 7429 2929 206f 7220 5c0d 0a20 2020 2020  t))) or \..     
-0001c070: 2020 2020 2020 2020 2020 2028 636f 6e66             (conf
-0001c080: 4669 6c74 6572 203d 3d20 3220 616e 6420  Filter == 2 and 
-0001c090: 2869 7335 3044 4d41 446f 776e 5472 656e  (is50DMADownTren
-0001c0a0: 6420 6f72 2069 7344 6561 6443 726f 7373  d or isDeadCross
-0001c0b0: 4f76 6572 206f 7220 2744 6f77 6e27 2069  Over or 'Down' i
-0001c0c0: 6e20 636f 6e66 5465 7874 2929 0d0a 2020  n confText))..  
-0001c0d0: 2020 2020 2020 2320 4d61 7962 6520 7468        # Maybe th
-0001c0e0: 6520 6469 6666 6572 656e 6365 2069 7320  e difference is 
-0001c0f0: 6e6f 7420 7769 7468 696e 2074 6865 2072  not within the r
-0001c100: 616e 6765 2c20 6275 7420 7765 2764 2073  ange, but we'd s
-0001c110: 7469 6c6c 206c 696b 6520 746f 206b 6565  till like to kee
-0001c120: 7020 7468 6520 7374 6f63 6b20 696e 0d0a  p the stock in..
-0001c130: 2020 2020 2020 2020 2320 7468 6520 6c69          # the li
-0001c140: 7374 2069 6620 6974 2773 2061 2067 6f6c  st if it's a gol
-0001c150: 6465 6e20 6372 6f73 736f 7665 7220 6f72  den crossover or
-0001c160: 2064 6561 6420 6372 6f73 736f 7665 720d   dead crossover.
-0001c170: 0a20 2020 2020 2020 2069 6620 6973 476f  .        if isGo
-0001c180: 6c64 656e 4372 6f73 734f 7665 7220 6f72  ldenCrossOver or
-0001c190: 2069 7344 6561 6443 726f 7373 4f76 6572   isDeadCrossOver
-0001c1a0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-0001c1b0: 6372 6565 6e44 6963 745b 224d 412d 5369  creenDict["MA-Si
-0001c1c0: 676e 616c 225d 203d 2028 0d0a 2020 2020  gnal"] = (..    
-0001c1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c1e0: 7361 7665 645b 305d 200d 0a20 2020 2020  saved[0] ..     
-0001c1f0: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-0001c200: 2063 6f6c 6f72 5465 7874 2e42 4f4c 440d   colorText.BOLD.
-0001c210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c220: 2020 2020 202b 2028 636f 6c6f 7254 6578       + (colorTex
-0001c230: 742e 4752 4545 4e20 6966 2069 7335 3044  t.GREEN if is50D
-0001c240: 4d41 5570 5472 656e 6420 656c 7365 2028  MAUpTrend else (
-0001c250: 636f 6c6f 7254 6578 742e 4641 494c 2069  colorText.FAIL i
-0001c260: 6620 6973 3530 444d 4144 6f77 6e54 7265  f is50DMADownTre
-0001c270: 6e64 2065 6c73 6520 636f 6c6f 7254 6578  nd else colorTex
-0001c280: 742e 5741 524e 2929 0d0a 2020 2020 2020  t.WARN))..      
-0001c290: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-0001c2a0: 6622 7b63 6f6e 6654 6578 747d 2028 7b64  f"{confText} ({d
-0001c2b0: 6966 6665 7265 6e63 657d 2529 220d 0a20  ifference}%)".. 
-0001c2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c2d0: 2020 202b 2063 6f6c 6f72 5465 7874 2e45     + colorText.E
-0001c2e0: 4e44 0d0a 2020 2020 2020 2020 2020 2020  ND..            
-0001c2f0: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-0001c300: 2020 2073 6176 6544 6963 745b 224d 412d     saveDict["MA-
-0001c310: 5369 676e 616c 225d 203d 2073 6176 6564  Signal"] = saved
-0001c320: 5b31 5d20 2b20 6622 7b63 6f6e 6654 6578  [1] + f"{confTex
-0001c330: 747d 2028 7b64 6966 6665 7265 6e63 657d  t} ({difference}
-0001c340: 2529 220d 0a20 2020 2020 2020 2020 2020  %)"..           
-0001c350: 2072 6574 7572 6e20 636f 6e66 4669 6c74   return confFilt
-0001c360: 6572 203d 3d20 3320 6f72 205c 0d0a 2020  er == 3 or \..  
-0001c370: 2020 2020 2020 2020 2020 2020 2020 2863                (c
-0001c380: 6f6e 6646 696c 7465 7220 3d3d 2031 2061  onfFilter == 1 a
-0001c390: 6e64 2069 7347 6f6c 6465 6e43 726f 7373  nd isGoldenCross
-0001c3a0: 4f76 6572 2920 6f72 205c 0d0a 2020 2020  Over) or \..    
-0001c3b0: 2020 2020 2020 2020 2020 2020 2863 6f6e              (con
-0001c3c0: 6646 696c 7465 7220 3d3d 2032 2061 6e64  fFilter == 2 and
-0001c3d0: 2069 7344 6561 6443 726f 7373 4f76 6572   isDeadCrossOver
-0001c3e0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-0001c3f0: 6e20 4661 6c73 650d 0a0d 0a20 2020 2023  n False....    #
-0001c400: 406d 6561 7375 7265 5f74 696d 650d 0a20  @measure_time.. 
-0001c410: 2020 2023 2056 616c 6964 6174 6520 6966     # Validate if
-0001c420: 2073 6861 7265 2070 7269 6365 7320 6172   share prices ar
-0001c430: 6520 636f 6e73 6f6c 6964 6174 696e 670d  e consolidating.
-0001c440: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-0001c450: 6543 6f6e 736f 6c69 6461 7469 6f6e 2873  eConsolidation(s
-0001c460: 656c 662c 2064 662c 2073 6372 6565 6e44  elf, df, screenD
-0001c470: 6963 742c 2073 6176 6544 6963 742c 2070  ict, saveDict, p
-0001c480: 6572 6365 6e74 6167 653d 3130 293a 0d0a  ercentage=10):..
-0001c490: 2020 2020 2020 2020 6966 2064 6620 6973          if df is
-0001c4a0: 204e 6f6e 6520 6f72 206c 656e 2864 6629   None or len(df)
-0001c4b0: 203d 3d20 303a 0d0a 2020 2020 2020 2020   == 0:..        
-0001c4c0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-0001c4d0: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
-0001c4e0: 2064 662e 636f 7079 2829 0d0a 2020 2020   df.copy()..    
-0001c4f0: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
-0001c500: 6669 6c6c 6e61 2830 290d 0a20 2020 2020  fillna(0)..     
-0001c510: 2020 2064 6174 6120 3d20 6461 7461 2e72     data = data.r
-0001c520: 6570 6c61 6365 285b 6e70 2e69 6e66 2c20  eplace([np.inf, 
-0001c530: 2d6e 702e 696e 665d 2c20 3029 0d0a 2020  -np.inf], 0)..  
-0001c540: 2020 2020 2020 6863 203d 2064 6174 612e        hc = data.
-0001c550: 6465 7363 7269 6265 2829 5b22 436c 6f73  describe()["Clos
-0001c560: 6522 5d5b 226d 6178 225d 0d0a 2020 2020  e"]["max"]..    
-0001c570: 2020 2020 6c63 203d 2064 6174 612e 6465      lc = data.de
-0001c580: 7363 7269 6265 2829 5b22 436c 6f73 6522  scribe()["Close"
-0001c590: 5d5b 226d 696e 225d 0d0a 2020 2020 2020  ]["min"]..      
-0001c5a0: 2020 6966 2028 6863 202d 206c 6329 203c    if (hc - lc) <
-0001c5b0: 3d20 2868 6320 2a20 7065 7263 656e 7461  = (hc * percenta
-0001c5c0: 6765 202f 2031 3030 2920 616e 6420 2868  ge / 100) and (h
-0001c5d0: 6320 2d20 6c63 2021 3d20 3029 3a0d 0a20  c - lc != 0):.. 
-0001c5e0: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-0001c5f0: 6e44 6963 745b 2243 6f6e 736f 6c2e 225d  nDict["Consol."]
-0001c600: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-0001c610: 2020 2020 2020 636f 6c6f 7254 6578 742e        colorText.
-0001c620: 424f 4c44 0d0a 2020 2020 2020 2020 2020  BOLD..          
-0001c630: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
-0001c640: 742e 4752 4545 4e0d 0a20 2020 2020 2020  t.GREEN..       
-0001c650: 2020 2020 2020 2020 202b 2022 5261 6e67           + "Rang
-0001c660: 653a 220d 0a20 2020 2020 2020 2020 2020  e:"..           
-0001c670: 2020 2020 202b 2073 7472 2872 6f75 6e64       + str(round
-0001c680: 2828 6162 7328 2868 6320 2d20 6c63 2920  ((abs((hc - lc) 
-0001c690: 2f20 6863 2920 2a20 3130 3029 2c20 3129  / hc) * 100), 1)
-0001c6a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0001c6b0: 2020 202b 2022 2522 0d0a 2020 2020 2020     + "%"..      
-0001c6c0: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
-0001c6d0: 7254 6578 742e 454e 440d 0a20 2020 2020  rText.END..     
-0001c6e0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-0001c6f0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-0001c700: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-0001c710: 2243 6f6e 736f 6c2e 225d 203d 2028 0d0a  "Consol."] = (..
-0001c720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c730: 636f 6c6f 7254 6578 742e 424f 4c44 0d0a  colorText.BOLD..
-0001c740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c750: 2b20 636f 6c6f 7254 6578 742e 4641 494c  + colorText.FAIL
-0001c760: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001c770: 2020 2b20 2252 616e 6765 3a22 0d0a 2020    + "Range:"..  
-0001c780: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-0001c790: 7374 7228 726f 756e 6428 2861 6273 2828  str(round((abs((
-0001c7a0: 6863 202d 206c 6329 202f 2068 6329 202a  hc - lc) / hc) *
-0001c7b0: 2031 3030 292c 2031 2929 0d0a 2020 2020   100), 1))..    
-0001c7c0: 2020 2020 2020 2020 2020 2020 2b20 2225              + "%
-0001c7d0: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-0001c7e0: 2020 202b 2063 6f6c 6f72 5465 7874 2e45     + colorText.E
-0001c7f0: 4e44 0d0a 2020 2020 2020 2020 2020 2020  ND..            
-0001c800: 290d 0a20 2020 2020 2020 2073 6176 6544  )..        saveD
-0001c810: 6963 745b 2243 6f6e 736f 6c2e 225d 203d  ict["Consol."] =
-0001c820: 2066 2752 616e 6765 3a7b 7374 7228 726f   f'Range:{str(ro
-0001c830: 756e 6428 2861 6273 2828 6863 2d6c 6329  und((abs((hc-lc)
-0001c840: 2f68 6329 2a31 3030 292c 3129 292b 2225  /hc)*100),1))+"%
-0001c850: 227d 270d 0a20 2020 2020 2020 2072 6574  "}'..        ret
-0001c860: 7572 6e20 726f 756e 6428 2861 6273 2828  urn round((abs((
-0001c870: 6863 202d 206c 6329 202f 2068 6329 202a  hc - lc) / hc) *
-0001c880: 2031 3030 292c 2031 290d 0a0d 0a20 2020   100), 1)....   
-0001c890: 2023 2076 616c 6964 6174 6520 6966 2074   # validate if t
-0001c8a0: 6865 2073 746f 636b 2068 6173 2062 6565  he stock has bee
-0001c8b0: 6e20 6861 7669 6e67 2068 6967 6865 7220  n having higher 
-0001c8c0: 6869 6768 732c 2068 6967 6865 7220 6c6f  highs, higher lo
-0001c8d0: 7773 0d0a 2020 2020 2320 616e 6420 6869  ws..    # and hi
-0001c8e0: 6768 6572 2063 6c6f 7365 2077 6974 6820  gher close with 
-0001c8f0: 6c61 7465 7374 2063 6c6f 7365 203e 2073  latest close > s
-0001c900: 7570 6572 7472 656e 6420 616e 6420 382d  upertrend and 8-
-0001c910: 454d 412e 0d0a 2020 2020 6465 6620 7661  EMA...    def va
-0001c920: 6c69 6461 7465 4869 6768 6572 4869 6768  lidateHigherHigh
-0001c930: 7348 6967 6865 724c 6f77 7348 6967 6865  sHigherLowsHighe
-0001c940: 7243 6c6f 7365 2873 656c 662c 2064 6629  rClose(self, df)
-0001c950: 3a0d 0a20 2020 2020 2020 2069 6620 6466  :..        if df
-0001c960: 2069 7320 4e6f 6e65 206f 7220 6c65 6e28   is None or len(
-0001c970: 6466 2920 3d3d 2030 3a0d 0a20 2020 2020  df) == 0:..     
-0001c980: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-0001c990: 6c73 650d 0a20 2020 2020 2020 2064 6174  lse..        dat
-0001c9a0: 6120 3d20 6466 2e63 6f70 7928 290d 0a20  a = df.copy().. 
-0001c9b0: 2020 2020 2020 2064 6179 3020 3d20 6461         day0 = da
-0001c9c0: 7461 0d0a 2020 2020 2020 2020 6461 7931  ta..        day1
-0001c9d0: 203d 2064 6174 615b 313a 5d0d 0a20 2020   = data[1:]..   
-0001c9e0: 2020 2020 2064 6179 3220 3d20 6461 7461       day2 = data
-0001c9f0: 5b32 3a5d 0d0a 2020 2020 2020 2020 6461  [2:]..        da
-0001ca00: 7933 203d 2064 6174 615b 333a 5d0d 0a20  y3 = data[3:].. 
-0001ca10: 2020 2020 2020 2069 6620 6c65 6e28 6461         if len(da
-0001ca20: 7931 2920 3c20 3120 6f72 206c 656e 2864  y1) < 1 or len(d
-0001ca30: 6179 3229 203c 2031 206f 7220 6c65 6e28  ay2) < 1 or len(
-0001ca40: 6461 7933 2920 3c20 313a 0d0a 2020 2020  day3) < 1:..    
-0001ca50: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-0001ca60: 616c 7365 0d0a 2020 2020 2020 2020 6869  alse..        hi
-0001ca70: 6768 6572 4869 6768 7320 3d20 280d 0a20  gherHighs = (.. 
-0001ca80: 2020 2020 2020 2020 2020 2028 6461 7930             (day0
-0001ca90: 5b22 4869 6768 225d 2e69 6c6f 635b 305d  ["High"].iloc[0]
-0001caa0: 203e 2064 6179 315b 2248 6967 6822 5d2e   > day1["High"].
-0001cab0: 696c 6f63 5b30 5d29 0d0a 2020 2020 2020  iloc[0])..      
-0001cac0: 2020 2020 2020 616e 6420 2864 6179 315b        and (day1[
-0001cad0: 2248 6967 6822 5d2e 696c 6f63 5b30 5d20  "High"].iloc[0] 
-0001cae0: 3e20 6461 7932 5b22 4869 6768 225d 2e69  > day2["High"].i
-0001caf0: 6c6f 635b 305d 290d 0a20 2020 2020 2020  loc[0])..       
-0001cb00: 2020 2020 2061 6e64 2028 6461 7932 5b22       and (day2["
-0001cb10: 4869 6768 225d 2e69 6c6f 635b 305d 203e  High"].iloc[0] >
-0001cb20: 2064 6179 335b 2248 6967 6822 5d2e 696c   day3["High"].il
-0001cb30: 6f63 5b30 5d29 0d0a 2020 2020 2020 2020  oc[0])..        
-0001cb40: 290d 0a20 2020 2020 2020 2068 6967 6865  )..        highe
-0001cb50: 724c 6f77 7320 3d20 280d 0a20 2020 2020  rLows = (..     
-0001cb60: 2020 2020 2020 2028 6461 7930 5b22 4c6f         (day0["Lo
-0001cb70: 7722 5d2e 696c 6f63 5b30 5d20 3e20 6461  w"].iloc[0] > da
-0001cb80: 7931 5b22 4c6f 7722 5d2e 696c 6f63 5b30  y1["Low"].iloc[0
-0001cb90: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-0001cba0: 616e 6420 2864 6179 315b 224c 6f77 225d  and (day1["Low"]
-0001cbb0: 2e69 6c6f 635b 305d 203e 2064 6179 325b  .iloc[0] > day2[
-0001cbc0: 224c 6f77 225d 2e69 6c6f 635b 305d 290d  "Low"].iloc[0]).
-0001cbd0: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
-0001cbe0: 2028 6461 7932 5b22 4c6f 7722 5d2e 696c   (day2["Low"].il
-0001cbf0: 6f63 5b30 5d20 3e20 6461 7933 5b22 4c6f  oc[0] > day3["Lo
-0001cc00: 7722 5d2e 696c 6f63 5b30 5d29 0d0a 2020  w"].iloc[0])..  
-0001cc10: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-0001cc20: 2068 6967 6865 7243 6c6f 7365 203d 2028   higherClose = (
-0001cc30: 0d0a 2020 2020 2020 2020 2020 2020 2864  ..            (d
-0001cc40: 6179 305b 2243 6c6f 7365 225d 2e69 6c6f  ay0["Close"].ilo
-0001cc50: 635b 305d 203e 2064 6179 315b 2243 6c6f  c[0] > day1["Clo
-0001cc60: 7365 225d 2e69 6c6f 635b 305d 290d 0a20  se"].iloc[0]).. 
-0001cc70: 2020 2020 2020 2020 2020 2061 6e64 2028             and (
-0001cc80: 6461 7931 5b22 436c 6f73 6522 5d2e 696c  day1["Close"].il
-0001cc90: 6f63 5b30 5d20 3e20 6461 7932 5b22 436c  oc[0] > day2["Cl
-0001cca0: 6f73 6522 5d2e 696c 6f63 5b30 5d29 0d0a  ose"].iloc[0])..
-0001ccb0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-0001ccc0: 2864 6179 325b 2243 6c6f 7365 225d 2e69  (day2["Close"].i
-0001ccd0: 6c6f 635b 305d 203e 2064 6179 335b 2243  loc[0] > day3["C
-0001cce0: 6c6f 7365 225d 2e69 6c6f 635b 305d 290d  lose"].iloc[0]).
-0001ccf0: 0a20 2020 2020 2020 2029 0d0a 2020 2020  .        )..    
-0001cd00: 2020 2020 2320 6869 6768 6572 5253 4920      # higherRSI 
-0001cd10: 3d20 2864 6179 305b 2252 5349 225d 2e69  = (day0["RSI"].i
-0001cd20: 6c6f 635b 305d 203e 2064 6179 315b 2252  loc[0] > day1["R
-0001cd30: 5349 225d 2e69 6c6f 635b 305d 2920 616e  SI"].iloc[0]) an
-0001cd40: 6420 5c0d 0a20 2020 2020 2020 2023 2020  d \..        #  
-0001cd50: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-0001cd60: 6461 7931 5b22 5253 4922 5d2e 696c 6f63  day1["RSI"].iloc
-0001cd70: 5b30 5d20 3e20 6461 7932 5b22 5253 4922  [0] > day2["RSI"
-0001cd80: 5d2e 696c 6f63 5b30 5d29 2061 6e64 205c  ].iloc[0]) and \
-0001cd90: 0d0a 2020 2020 2020 2020 2320 2020 2020  ..        #     
-0001cda0: 2020 2020 2020 2020 2020 2020 2864 6179              (day
-0001cdb0: 325b 2252 5349 225d 2e69 6c6f 635b 305d  2["RSI"].iloc[0]
-0001cdc0: 203e 2064 6179 335b 2252 5349 225d 2e69   > day3["RSI"].i
-0001cdd0: 6c6f 635b 305d 2920 616e 6420 5c0d 0a20  loc[0]) and \.. 
-0001cde0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0001cdf0: 2020 2020 2020 2020 2064 6179 335b 2252           day3["R
-0001ce00: 5349 225d 2e69 6c6f 635b 305d 203e 3d20  SI"].iloc[0] >= 
-0001ce10: 3530 2061 6e64 2064 6179 305b 2252 5349  50 and day0["RSI
-0001ce20: 225d 2e69 6c6f 635b 305d 203e 3d20 3635  "].iloc[0] >= 65
-0001ce30: 0d0a 2020 2020 2020 2020 7265 7665 7273  ..        revers
-0001ce40: 6564 4461 7461 203d 2064 6174 615b 3a3a  edData = data[::
-0001ce50: 2d31 5d2e 636f 7079 2829 0d0a 2020 2020  -1].copy()..    
-0001ce60: 2020 2020 7265 7665 7273 6564 4461 7461      reversedData
-0001ce70: 5b22 5355 5045 5254 225d 203d 2070 6b74  ["SUPERT"] = pkt
-0001ce80: 616c 6962 2e73 7570 6572 7472 656e 6428  alib.supertrend(
-0001ce90: 7265 7665 7273 6564 4461 7461 2c20 372c  reversedData, 7,
-0001cea0: 2033 295b 2253 5550 4552 545f 375f 332e   3)["SUPERT_7_3.
-0001ceb0: 3022 5d0d 0a20 2020 2020 2020 2072 6576  0"]..        rev
-0001cec0: 6572 7365 6444 6174 615b 2245 4d41 3822  ersedData["EMA8"
-0001ced0: 5d20 3d20 706b 7461 6c69 622e 454d 4128  ] = pktalib.EMA(
-0001cee0: 7265 7665 7273 6564 4461 7461 5b22 436c  reversedData["Cl
-0001cef0: 6f73 6522 5d2c 2074 696d 6570 6572 696f  ose"], timeperio
-0001cf00: 643d 3929 0d0a 2020 2020 2020 2020 6869  d=9)..        hi
-0001cf10: 6768 6572 436c 6f73 6520 3d20 280d 0a20  gherClose = (.. 
-0001cf20: 2020 2020 2020 2020 2020 2068 6967 6865             highe
-0001cf30: 7243 6c6f 7365 0d0a 2020 2020 2020 2020  rClose..        
-0001cf40: 2020 2020 616e 6420 6461 7930 5b22 436c      and day0["Cl
-0001cf50: 6f73 6522 5d2e 696c 6f63 5b30 5d20 3e20  ose"].iloc[0] > 
-0001cf60: 7265 7665 7273 6564 4461 7461 2e74 6169  reversedData.tai
-0001cf70: 6c28 3129 5b22 5355 5045 5254 225d 2e69  l(1)["SUPERT"].i
-0001cf80: 6c6f 635b 305d 0d0a 2020 2020 2020 2020  loc[0]..        
-0001cf90: 2020 2020 616e 6420 6461 7930 5b22 436c      and day0["Cl
-0001cfa0: 6f73 6522 5d2e 696c 6f63 5b30 5d20 3e20  ose"].iloc[0] > 
-0001cfb0: 7265 7665 7273 6564 4461 7461 2e74 6169  reversedData.tai
-0001cfc0: 6c28 3129 5b22 454d 4138 225d 2e69 6c6f  l(1)["EMA8"].ilo
-0001cfd0: 635b 305d 0d0a 2020 2020 2020 2020 290d  c[0]..        ).
-0001cfe0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001cff0: 6869 6768 6572 4869 6768 7320 616e 6420  higherHighs and 
-0001d000: 6869 6768 6572 4c6f 7773 2061 6e64 2068  higherLows and h
-0001d010: 6967 6865 7243 6c6f 7365 0d0a 0d0a 2020  igherClose....  
-0001d020: 2020 2340 6d65 6173 7572 655f 7469 6d65    #@measure_time
-0001d030: 0d0a 2020 2020 2320 5661 6c69 6461 7465  ..    # Validate
-0001d040: 2027 496e 7369 6465 2042 6172 2720 7374   'Inside Bar' st
-0001d050: 7275 6374 7572 6520 666f 7220 7265 6365  ructure for rece
-0001d060: 6e74 2064 6179 730d 0a20 2020 2064 6566  nt days..    def
-0001d070: 2076 616c 6964 6174 6549 6e73 6964 6542   validateInsideB
-0001d080: 6172 280d 0a20 2020 2020 2020 2073 656c  ar(..        sel
-0001d090: 662c 2064 662c 2073 6372 6565 6e44 6963  f, df, screenDic
-0001d0a0: 742c 2073 6176 6544 6963 742c 2063 6861  t, saveDict, cha
-0001d0b0: 7274 5061 7474 6572 6e3d 312c 2064 6179  rtPattern=1, day
-0001d0c0: 7354 6f4c 6f6f 6b62 6163 6b3d 350d 0a20  sToLookback=5.. 
-0001d0d0: 2020 2029 3a0d 0a20 2020 2020 2020 2069     ):..        i
-0001d0e0: 6620 6466 2069 7320 4e6f 6e65 206f 7220  f df is None or 
-0001d0f0: 6c65 6e28 6466 2920 3d3d 2030 3a0d 0a20  len(df) == 0:.. 
-0001d100: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0001d110: 6e20 4661 6c73 650d 0a20 2020 2020 2020  n False..       
-0001d120: 2064 6174 6120 3d20 6466 2e63 6f70 7928   data = df.copy(
-0001d130: 290d 0a20 2020 2020 2020 206f 7267 4461  )..        orgDa
-0001d140: 7461 203d 2064 6174 610d 0a20 2020 2020  ta = data..     
-0001d150: 2020 2073 6176 6564 203d 2073 656c 662e     saved = self.
-0001d160: 6669 6e64 4375 7272 656e 7453 6176 6564  findCurrentSaved
-0001d170: 5661 6c75 6528 7363 7265 656e 4469 6374  Value(screenDict
-0001d180: 2c20 7361 7665 4469 6374 2c20 2250 6174  , saveDict, "Pat
-0001d190: 7465 726e 2229 0d0a 2020 2020 2020 2020  tern")..        
-0001d1a0: 666f 7220 6920 696e 2072 616e 6765 2869  for i in range(i
-0001d1b0: 6e74 2864 6179 7354 6f4c 6f6f 6b62 6163  nt(daysToLookbac
-0001d1c0: 6b29 2c20 696e 7428 726f 756e 6428 6461  k), int(round(da
-0001d1d0: 7973 546f 4c6f 6f6b 6261 636b 202a 2030  ysToLookback * 0
-0001d1e0: 2e35 2929 202d 2031 2c20 2d31 293a 0d0a  .5)) - 1, -1):..
-0001d1f0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-0001d200: 203d 3d20 323a 0d0a 2020 2020 2020 2020   == 2:..        
-0001d210: 2020 2020 2020 2020 7265 7475 726e 2030          return 0
-0001d220: 2020 2320 4578 6974 2069 6620 6f6e 6c79    # Exit if only
-0001d230: 206c 6173 7420 3220 6361 6e64 6c65 7320   last 2 candles 
-0001d240: 6172 6520 6c65 6674 0d0a 2020 2020 2020  are left..      
-0001d250: 2020 2020 2020 6966 2063 6861 7274 5061        if chartPa
-0001d260: 7474 6572 6e20 3d3d 2031 3a0d 0a20 2020  ttern == 1:..   
-0001d270: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0001d280: 2255 7022 2069 6e20 7361 7665 4469 6374  "Up" in saveDict
-0001d290: 5b22 5472 656e 6422 5d20 616e 6420 280d  ["Trend"] and (.
-0001d2a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d2b0: 2020 2020 2022 4275 6c6c 2220 696e 2073       "Bull" in s
-0001d2c0: 6176 6544 6963 745b 224d 412d 5369 676e  aveDict["MA-Sign
-0001d2d0: 616c 225d 0d0a 2020 2020 2020 2020 2020  al"]..          
-0001d2e0: 2020 2020 2020 2020 2020 6f72 2022 5375            or "Su
-0001d2f0: 7070 6f72 7422 2069 6e20 7361 7665 4469  pport" in saveDi
-0001d300: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d0d  ct["MA-Signal"].
-0001d310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d320: 2029 3a0d 0a20 2020 2020 2020 2020 2020   ):..           
-0001d330: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
-0001d340: 6f72 6744 6174 612e 6865 6164 2869 290d  orgData.head(i).
-0001d350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d360: 2020 2020 2072 6566 4361 6e64 6c65 203d       refCandle =
-0001d370: 2064 6174 612e 7461 696c 2831 290d 0a20   data.tail(1).. 
-0001d380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d390: 2020 2069 6620 280d 0a20 2020 2020 2020     if (..       
-0001d3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d3b0: 2028 6c65 6e28 6461 7461 2e48 6967 685b   (len(data.High[
-0001d3c0: 6461 7461 2e48 6967 6820 3e20 7265 6643  data.High > refC
-0001d3d0: 616e 646c 652e 4869 6768 2e69 7465 6d28  andle.High.item(
-0001d3e0: 295d 2920 3d3d 2030 290d 0a20 2020 2020  )]) == 0)..     
-0001d3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d400: 2020 2061 6e64 2028 6c65 6e28 6461 7461     and (len(data
-0001d410: 2e4c 6f77 5b64 6174 612e 4c6f 7720 3c20  .Low[data.Low < 
-0001d420: 7265 6643 616e 646c 652e 4c6f 772e 6974  refCandle.Low.it
-0001d430: 656d 2829 5d29 203d 3d20 3029 0d0a 2020  em()]) == 0)..  
-0001d440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d450: 2020 2020 2020 616e 6420 286c 656e 2864        and (len(d
-0001d460: 6174 612e 4f70 656e 5b64 6174 612e 4f70  ata.Open[data.Op
-0001d470: 656e 203e 2072 6566 4361 6e64 6c65 2e48  en > refCandle.H
-0001d480: 6967 682e 6974 656d 2829 5d29 203d 3d20  igh.item()]) == 
-0001d490: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
-0001d4a0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-0001d4b0: 286c 656e 2864 6174 612e 436c 6f73 655b  (len(data.Close[
-0001d4c0: 6461 7461 2e43 6c6f 7365 203c 2072 6566  data.Close < ref
-0001d4d0: 4361 6e64 6c65 2e4c 6f77 2e69 7465 6d28  Candle.Low.item(
-0001d4e0: 295d 2920 3d3d 2030 290d 0a20 2020 2020  )]) == 0)..     
-0001d4f0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0001d500: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001d510: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-0001d520: 6e44 6963 745b 2250 6174 7465 726e 225d  nDict["Pattern"]
-0001d530: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-0001d540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d550: 2020 7361 7665 645b 305d 0d0a 2020 2020    saved[0]..    
-0001d560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d570: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
-0001d580: 6578 742e 424f 4c44 0d0a 2020 2020 2020  ext.BOLD..      
-0001d590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d5a0: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
-0001d5b0: 742e 5741 524e 0d0a 2020 2020 2020 2020  t.WARN..        
-0001d5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d5d0: 2020 2020 2b20 2822 496e 7369 6465 2042      + ("Inside B
-0001d5e0: 6172 2028 2564 2922 2025 2069 290d 0a20  ar (%d)" % i).. 
-0001d5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d600: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-0001d610: 6f72 5465 7874 2e45 4e44 0d0a 2020 2020  orText.END..    
-0001d620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d630: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-0001d640: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001d650: 6176 6544 6963 745b 2250 6174 7465 726e  aveDict["Pattern
-0001d660: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
-0001d670: 2249 6e73 6964 6520 4261 7220 2825 6429  "Inside Bar (%d)
-0001d680: 2220 2520 690d 0a20 2020 2020 2020 2020  " % i..         
-0001d690: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0001d6a0: 6574 7572 6e20 690d 0a20 2020 2020 2020  eturn i..       
-0001d6b0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-0001d6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d6d0: 2020 2020 7265 7475 726e 2030 0d0a 2020      return 0..  
-0001d6e0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-0001d6f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d700: 2069 6620 2244 6f77 6e22 2069 6e20 7361   if "Down" in sa
-0001d710: 7665 4469 6374 5b22 5472 656e 6422 5d20  veDict["Trend"] 
-0001d720: 616e 6420 280d 0a20 2020 2020 2020 2020  and (..         
-0001d730: 2020 2020 2020 2020 2020 2022 4265 6172             "Bear
-0001d740: 2220 696e 2073 6176 6544 6963 745b 224d  " in saveDict["M
-0001d750: 412d 5369 676e 616c 225d 206f 7220 2252  A-Signal"] or "R
-0001d760: 6573 6973 7422 2069 6e20 7361 7665 4469  esist" in saveDi
-0001d770: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d0d  ct["MA-Signal"].
-0001d780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d790: 2029 3a0d 0a20 2020 2020 2020 2020 2020   ):..           
-0001d7a0: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
-0001d7b0: 6f72 6744 6174 612e 6865 6164 2869 290d  orgData.head(i).
-0001d7c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d7d0: 2020 2020 2072 6566 4361 6e64 6c65 203d       refCandle =
-0001d7e0: 2064 6174 612e 7461 696c 2831 290d 0a20   data.tail(1).. 
-0001d7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d800: 2020 2069 6620 280d 0a20 2020 2020 2020     if (..       
-0001d810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d820: 2028 6c65 6e28 6461 7461 2e48 6967 685b   (len(data.High[
-0001d830: 6461 7461 2e48 6967 6820 3e20 7265 6643  data.High > refC
-0001d840: 616e 646c 652e 4869 6768 2e69 7465 6d28  andle.High.item(
-0001d850: 295d 2920 3d3d 2030 290d 0a20 2020 2020  )]) == 0)..     
-0001d860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d870: 2020 2061 6e64 2028 6c65 6e28 6461 7461     and (len(data
-0001d880: 2e4c 6f77 5b64 6174 612e 4c6f 7720 3c20  .Low[data.Low < 
-0001d890: 7265 6643 616e 646c 652e 4c6f 772e 6974  refCandle.Low.it
-0001d8a0: 656d 2829 5d29 203d 3d20 3029 0d0a 2020  em()]) == 0)..  
-0001d8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d8c0: 2020 2020 2020 616e 6420 286c 656e 2864        and (len(d
-0001d8d0: 6174 612e 4f70 656e 5b64 6174 612e 4f70  ata.Open[data.Op
-0001d8e0: 656e 203e 2072 6566 4361 6e64 6c65 2e48  en > refCandle.H
-0001d8f0: 6967 682e 6974 656d 2829 5d29 203d 3d20  igh.item()]) == 
-0001d900: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
-0001d910: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-0001d920: 286c 656e 2864 6174 612e 436c 6f73 655b  (len(data.Close[
-0001d930: 6461 7461 2e43 6c6f 7365 203c 2072 6566  data.Close < ref
-0001d940: 4361 6e64 6c65 2e4c 6f77 2e69 7465 6d28  Candle.Low.item(
-0001d950: 295d 2920 3d3d 2030 290d 0a20 2020 2020  )]) == 0)..     
-0001d960: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0001d970: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001d980: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-0001d990: 6e44 6963 745b 2250 6174 7465 726e 225d  nDict["Pattern"]
-0001d9a0: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-0001d9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d9c0: 2020 7361 7665 645b 305d 0d0a 2020 2020    saved[0]..    
-0001d9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d9e0: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
-0001d9f0: 6578 742e 424f 4c44 0d0a 2020 2020 2020  ext.BOLD..      
-0001da00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001da10: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
-0001da20: 742e 5741 524e 0d0a 2020 2020 2020 2020  t.WARN..        
-0001da30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001da40: 2020 2020 2b20 2822 496e 7369 6465 2042      + ("Inside B
-0001da50: 6172 2028 2564 2922 2025 2069 290d 0a20  ar (%d)" % i).. 
-0001da60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001da70: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-0001da80: 6f72 5465 7874 2e45 4e44 0d0a 2020 2020  orText.END..    
-0001da90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001daa0: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-0001dab0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001dac0: 6176 6544 6963 745b 2250 6174 7465 726e  aveDict["Pattern
-0001dad0: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
-0001dae0: 2249 6e73 6964 6520 4261 7220 2825 6429  "Inside Bar (%d)
-0001daf0: 2220 2520 690d 0a20 2020 2020 2020 2020  " % i..         
-0001db00: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0001db10: 6574 7572 6e20 690d 0a20 2020 2020 2020  eturn i..       
-0001db20: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-0001db30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001db40: 2020 2020 7265 7475 726e 2030 0d0a 2020      return 0..  
-0001db50: 2020 2020 2020 7265 7475 726e 2030 0d0a        return 0..
-0001db60: 0d0a 2020 2020 2320 4669 6e64 2049 504f  ..    # Find IPO
-0001db70: 2062 6173 650d 0a20 2020 2064 6566 2076   base..    def v
-0001db80: 616c 6964 6174 6549 706f 4261 7365 2873  alidateIpoBase(s
-0001db90: 656c 662c 2073 746f 636b 2c20 6466 2c20  elf, stock, df, 
-0001dba0: 7363 7265 656e 4469 6374 2c20 7361 7665  screenDict, save
-0001dbb0: 4469 6374 2c20 7065 7263 656e 7461 6765  Dict, percentage
-0001dbc0: 3d30 2e33 293a 0d0a 2020 2020 2020 2020  =0.3):..        
-0001dbd0: 6966 2064 6620 6973 204e 6f6e 6520 6f72  if df is None or
-0001dbe0: 206c 656e 2864 6629 203d 3d20 303a 0d0a   len(df) == 0:..
-0001dbf0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0001dc00: 726e 2046 616c 7365 0d0a 2020 2020 2020  rn False..      
-0001dc10: 2020 6461 7461 203d 2064 662e 636f 7079    data = df.copy
-0001dc20: 2829 0d0a 2020 2020 2020 2020 6c69 7374  ()..        list
-0001dc30: 696e 6750 7269 6365 203d 2064 6174 615b  ingPrice = data[
-0001dc40: 3a3a 2d31 5d2e 6865 6164 2831 295b 224f  ::-1].head(1)["O
-0001dc50: 7065 6e22 5d2e 696c 6f63 5b30 5d0d 0a20  pen"].iloc[0].. 
-0001dc60: 2020 2020 2020 2063 7572 7265 6e74 5072         currentPr
-0001dc70: 6963 6520 3d20 6461 7461 2e68 6561 6428  ice = data.head(
-0001dc80: 3129 5b22 436c 6f73 6522 5d2e 696c 6f63  1)["Close"].iloc
-0001dc90: 5b30 5d0d 0a20 2020 2020 2020 2041 5448  [0]..        ATH
-0001dca0: 203d 2064 6174 612e 6465 7363 7269 6265   = data.describe
-0001dcb0: 2829 5b22 4869 6768 225d 5b22 6d61 7822  ()["High"]["max"
-0001dcc0: 5d0d 0a20 2020 2020 2020 2069 6620 4154  ]..        if AT
-0001dcd0: 4820 3e20 286c 6973 7469 6e67 5072 6963  H > (listingPric
-0001dce0: 6520 2b20 286c 6973 7469 6e67 5072 6963  e + (listingPric
-0001dcf0: 6520 2a20 7065 7263 656e 7461 6765 2929  e * percentage))
-0001dd00: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-0001dd10: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
-0001dd20: 2020 2020 2061 7761 7920 3d20 726f 756e       away = roun
-0001dd30: 6428 2828 6375 7272 656e 7450 7269 6365  d(((currentPrice
-0001dd40: 202d 206c 6973 7469 6e67 5072 6963 6529   - listingPrice)
-0001dd50: 202f 206c 6973 7469 6e67 5072 6963 6529   / listingPrice)
-0001dd60: 202a 2031 3030 2c20 3129 0d0a 2020 2020   * 100, 1)..    
-0001dd70: 2020 2020 6966 2028 0d0a 2020 2020 2020      if (..      
-0001dd80: 2020 2020 2020 286c 6973 7469 6e67 5072        (listingPr
-0001dd90: 6963 6520 2d20 286c 6973 7469 6e67 5072  ice - (listingPr
-0001dda0: 6963 6520 2a20 7065 7263 656e 7461 6765  ice * percentage
-0001ddb0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0001ddc0: 3c3d 2063 7572 7265 6e74 5072 6963 650d  <= currentPrice.
-0001ddd0: 0a20 2020 2020 2020 2020 2020 203c 3d20  .            <= 
-0001dde0: 286c 6973 7469 6e67 5072 6963 6520 2b20  (listingPrice + 
-0001ddf0: 286c 6973 7469 6e67 5072 6963 6520 2a20  (listingPrice * 
-0001de00: 7065 7263 656e 7461 6765 2929 0d0a 2020  percentage))..  
-0001de10: 2020 2020 2020 293a 0d0a 2020 2020 2020        ):..      
-0001de20: 2020 2020 2020 7361 7665 6420 3d20 7365        saved = se
-0001de30: 6c66 2e66 696e 6443 7572 7265 6e74 5361  lf.findCurrentSa
-0001de40: 7665 6456 616c 7565 2873 6372 6565 6e44  vedValue(screenD
-0001de50: 6963 742c 2073 6176 6544 6963 742c 2022  ict, saveDict, "
-0001de60: 5061 7474 6572 6e22 290d 0a20 2020 2020  Pattern")..     
-0001de70: 2020 2020 2020 2069 6620 6177 6179 203e         if away >
-0001de80: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
-0001de90: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-0001dea0: 2250 6174 7465 726e 225d 203d 2028 0d0a  "Pattern"] = (..
-0001deb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dec0: 2020 2020 7361 7665 645b 305d 200d 0a20      saved[0] .. 
-0001ded0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dee0: 2020 202b 2063 6f6c 6f72 5465 7874 2e42     + colorText.B
-0001def0: 4f4c 440d 0a20 2020 2020 2020 2020 2020  OLD..           
-0001df00: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
-0001df10: 5465 7874 2e47 5245 454e 0d0a 2020 2020  Text.GREEN..    
-0001df20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001df30: 2b20 6622 4950 4f20 4261 7365 2028 7b61  + f"IPO Base ({a
-0001df40: 7761 797d 2025 2922 0d0a 2020 2020 2020  way} %)"..      
-0001df50: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-0001df60: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
-0001df70: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0001df80: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-0001df90: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-0001dfa0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-0001dfb0: 2250 6174 7465 726e 225d 203d 2028 0d0a  "Pattern"] = (..
-0001dfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dfd0: 2020 2020 7361 7665 645b 305d 0d0a 2020      saved[0]..  
-0001dfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dff0: 2020 2b20 636f 6c6f 7254 6578 742e 424f    + colorText.BO
-0001e000: 4c44 0d0a 2020 2020 2020 2020 2020 2020  LD..            
-0001e010: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
-0001e020: 6578 742e 4752 4545 4e0d 0a20 2020 2020  ext.GREEN..     
-0001e030: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-0001e040: 2022 4950 4f20 4261 7365 2022 0d0a 2020   "IPO Base "..  
-0001e050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e060: 2020 2b20 636f 6c6f 7254 6578 742e 4641    + colorText.FA
-0001e070: 494c 0d0a 2020 2020 2020 2020 2020 2020  IL..            
-0001e080: 2020 2020 2020 2020 2b20 6622 287b 6177          + f"({aw
-0001e090: 6179 7d20 2529 220d 0a20 2020 2020 2020  ay} %)"..       
-0001e0a0: 2020 2020 2020 2020 2020 2020 202b 2063               + c
-0001e0b0: 6f6c 6f72 5465 7874 2e45 4e44 0d0a 2020  olorText.END..  
-0001e0c0: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-0001e0d0: 0a20 2020 2020 2020 2020 2020 2073 6176  .            sav
-0001e0e0: 6544 6963 745b 2250 6174 7465 726e 225d  eDict["Pattern"]
-0001e0f0: 203d 2073 6176 6564 5b31 5d20 2b20 6622   = saved[1] + f"
-0001e100: 4950 4f20 4261 7365 2028 7b61 7761 797d  IPO Base ({away}
-0001e110: 2025 2922 0d0a 2020 2020 2020 2020 2020   %)"..          
-0001e120: 2020 7265 7475 726e 2054 7275 650d 0a20    return True.. 
-0001e130: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-0001e140: 6c73 650d 0a0d 0a20 2020 2023 406d 6561  lse....    #@mea
-0001e150: 7375 7265 5f74 696d 650d 0a20 2020 2023  sure_time..    #
-0001e160: 2056 616c 6964 6174 6520 4c6f 7265 6e74   Validate Lorent
-0001e170: 7a69 616e 2043 6c61 7373 6966 6963 6174  zian Classificat
-0001e180: 696f 6e20 7369 676e 616c 0d0a 2020 2020  ion signal..    
-0001e190: 6465 6620 7661 6c69 6461 7465 4c6f 7265  def validateLore
-0001e1a0: 6e74 7a69 616e 2873 656c 662c 2064 662c  ntzian(self, df,
-0001e1b0: 2073 6372 6565 6e44 6963 742c 2073 6176   screenDict, sav
-0001e1c0: 6544 6963 742c 206c 6f6f 6b46 6f72 3d33  eDict, lookFor=3
-0001e1d0: 293a 0d0a 2020 2020 2020 2020 6966 2064  ):..        if d
-0001e1e0: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
-0001e1f0: 2864 6629 203d 3d20 303a 0d0a 2020 2020  (df) == 0:..    
-0001e200: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-0001e210: 616c 7365 0d0a 2020 2020 2020 2020 6461  alse..        da
-0001e220: 7461 203d 2064 662e 636f 7079 2829 0d0a  ta = df.copy()..
-0001e230: 2020 2020 2020 2020 2320 6c6f 6f6b 466f          # lookFo
-0001e240: 723a 2031 2d42 7579 2c20 322d 5365 6c6c  r: 1-Buy, 2-Sell
-0001e250: 2c20 332d 416e 790d 0a20 2020 2020 2020  , 3-Any..       
-0001e260: 2064 6174 6120 3d20 6461 7461 5b3a 3a2d   data = data[::-
-0001e270: 315d 2020 2320 5265 7665 7273 6520 7468  1]  # Reverse th
-0001e280: 6520 6461 7461 6672 616d 650d 0a20 2020  e dataframe..   
-0001e290: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
-0001e2a0: 2e72 656e 616d 6528 0d0a 2020 2020 2020  .rename(..      
-0001e2b0: 2020 2020 2020 636f 6c75 6d6e 733d 7b0d        columns={.
-0001e2c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e2d0: 2022 4f70 656e 223a 2022 6f70 656e 222c   "Open": "open",
-0001e2e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001e2f0: 2020 2243 6c6f 7365 223a 2022 636c 6f73    "Close": "clos
-0001e300: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
-0001e310: 2020 2020 2022 4869 6768 223a 2022 6869       "High": "hi
-0001e320: 6768 222c 0d0a 2020 2020 2020 2020 2020  gh",..          
-0001e330: 2020 2020 2020 224c 6f77 223a 2022 6c6f        "Low": "lo
-0001e340: 7722 2c0d 0a20 2020 2020 2020 2020 2020  w",..           
-0001e350: 2020 2020 2022 566f 6c75 6d65 223a 2022       "Volume": "
-0001e360: 766f 6c75 6d65 222c 0d0a 2020 2020 2020  volume",..      
-0001e370: 2020 2020 2020 7d0d 0a20 2020 2020 2020        }..       
-0001e380: 2029 0d0a 2020 2020 2020 2020 7472 793a   )..        try:
-0001e390: 0d0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
-0001e3a0: 7468 2053 7570 7072 6573 734f 7574 7075  th SuppressOutpu
-0001e3b0: 7428 7375 7070 7265 7373 5f73 7464 6f75  t(suppress_stdou
-0001e3c0: 743d 5472 7565 2c20 7375 7070 7265 7373  t=True, suppress
-0001e3d0: 5f73 7464 6572 723d 5472 7565 293a 0d0a  _stderr=True):..
-0001e3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e3f0: 6c63 203d 2061 7461 2e4c 6f72 656e 747a  lc = ata.Lorentz
-0001e400: 6961 6e43 6c61 7373 6966 6963 6174 696f  ianClassificatio
-0001e410: 6e28 6461 7461 3d64 6174 6129 0d0a 2020  n(data=data)..  
-0001e420: 2020 2020 2020 2020 2020 7361 7665 6420            saved 
-0001e430: 3d20 7365 6c66 2e66 696e 6443 7572 7265  = self.findCurre
-0001e440: 6e74 5361 7665 6456 616c 7565 2873 6372  ntSavedValue(scr
-0001e450: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
-0001e460: 742c 2022 5061 7474 6572 6e22 290d 0a20  t, "Pattern").. 
-0001e470: 2020 2020 2020 2020 2020 2069 6620 6c63             if lc
-0001e480: 2e64 662e 696c 6f63 5b2d 315d 5b22 6973  .df.iloc[-1]["is
-0001e490: 4e65 7742 7579 5369 676e 616c 225d 3a0d  NewBuySignal"]:.
-0001e4a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e4b0: 2073 6372 6565 6e44 6963 745b 2250 6174   screenDict["Pat
-0001e4c0: 7465 726e 225d 203d 2028 0d0a 2020 2020  tern"] = (..    
-0001e4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e4e0: 7361 7665 645b 305d 202b 2063 6f6c 6f72  saved[0] + color
-0001e4f0: 5465 7874 2e42 4f4c 4420 2b20 636f 6c6f  Text.BOLD + colo
-0001e500: 7254 6578 742e 4752 4545 4e20 2b20 224c  rText.GREEN + "L
-0001e510: 6f72 656e 747a 6961 6e2d 4275 7922 202b  orentzian-Buy" +
-0001e520: 2063 6f6c 6f72 5465 7874 2e45 4e44 0d0a   colorText.END..
-0001e530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e540: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0001e550: 2020 2073 6176 6544 6963 745b 2250 6174     saveDict["Pat
-0001e560: 7465 726e 225d 203d 2073 6176 6564 5b31  tern"] = saved[1
-0001e570: 5d20 2b20 224c 6f72 656e 747a 6961 6e2d  ] + "Lorentzian-
-0001e580: 4275 7922 0d0a 2020 2020 2020 2020 2020  Buy"..          
-0001e590: 2020 2020 2020 6966 206c 6f6f 6b46 6f72        if lookFor
-0001e5a0: 2021 3d20 323a 2023 204e 6f74 2053 656c   != 2: # Not Sel
-0001e5b0: 6c0d 0a20 2020 2020 2020 2020 2020 2020  l..             
-0001e5c0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-0001e5d0: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
-0001e5e0: 656c 6966 206c 632e 6466 2e69 6c6f 635b  elif lc.df.iloc[
-0001e5f0: 2d31 5d5b 2269 734e 6577 5365 6c6c 5369  -1]["isNewSellSi
-0001e600: 676e 616c 225d 3a0d 0a20 2020 2020 2020  gnal"]:..       
-0001e610: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-0001e620: 6963 745b 2250 6174 7465 726e 225d 203d  ict["Pattern"] =
-0001e630: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-0001e640: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
-0001e650: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-0001e660: 4420 2b20 636f 6c6f 7254 6578 742e 4641  D + colorText.FA
-0001e670: 494c 202b 2022 4c6f 7265 6e74 7a69 616e  IL + "Lorentzian
-0001e680: 2d53 656c 6c22 202b 2063 6f6c 6f72 5465  -Sell" + colorTe
-0001e690: 7874 2e45 4e44 0d0a 2020 2020 2020 2020  xt.END..        
-0001e6a0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-0001e6b0: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
-0001e6c0: 6963 745b 2250 6174 7465 726e 225d 203d  ict["Pattern"] =
-0001e6d0: 2073 6176 6564 5b31 5d20 2b20 224c 6f72   saved[1] + "Lor
-0001e6e0: 656e 747a 6961 6e2d 5365 6c6c 220d 0a20  entzian-Sell".. 
-0001e6f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001e700: 6620 6c6f 6f6b 466f 7220 213d 2031 3a20  f lookFor != 1: 
-0001e710: 2320 4e6f 7420 4275 790d 0a20 2020 2020  # Not Buy..     
-0001e720: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0001e730: 6574 7572 6e20 5472 7565 0d0a 2020 2020  eturn True..    
-0001e740: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-0001e750: 7469 6f6e 3a20 2023 2070 7261 676d 613a  tion:  # pragma:
-0001e760: 206e 6f20 636f 7665 720d 0a20 2020 2020   no cover..     
-0001e770: 2020 2020 2020 2023 2056 616c 7565 4572         # ValueEr
-0001e780: 726f 723a 206f 7065 7261 6e64 7320 636f  ror: operands co
-0001e790: 756c 6420 6e6f 7420 6265 2062 726f 6164  uld not be broad
-0001e7a0: 6361 7374 2074 6f67 6574 6865 7220 7769  cast together wi
-0001e7b0: 7468 2073 6861 7065 7320 2832 302c 2920  th shapes (20,) 
-0001e7c0: 2832 362c 290d 0a20 2020 2020 2020 2020  (26,)..         
-0001e7d0: 2020 2023 2046 696c 6520 222f 6f70 742f     # File "/opt/
-0001e7e0: 686f 6d65 6272 6577 2f6c 6962 2f70 7974  homebrew/lib/pyt
-0001e7f0: 686f 6e33 2e31 312f 7369 7465 2d70 6163  hon3.11/site-pac
-0001e800: 6b61 6765 732f 6164 7661 6e63 6564 5f74  kages/advanced_t
-0001e810: 612f 4c6f 7265 6e74 7a69 616e 436c 6173  a/LorentzianClas
-0001e820: 7369 6669 6361 7469 6f6e 2f43 6c61 7373  sification/Class
-0001e830: 6966 6965 722e 7079 222c 206c 696e 6520  ifier.py", line 
-0001e840: 3138 362c 2069 6e20 5f5f 696e 6974 5f5f  186, in __init__
-0001e850: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0001e860: 4669 6c65 2022 2f6f 7074 2f68 6f6d 6562  File "/opt/homeb
-0001e870: 7265 772f 6c69 622f 7079 7468 6f6e 332e  rew/lib/python3.
-0001e880: 3131 2f73 6974 652d 7061 636b 6167 6573  11/site-packages
-0001e890: 2f61 6476 616e 6365 645f 7461 2f4c 6f72  /advanced_ta/Lor
-0001e8a0: 656e 747a 6961 6e43 6c61 7373 6966 6963  entzianClassific
-0001e8b0: 6174 696f 6e2f 436c 6173 7369 6669 6572  ation/Classifier
-0001e8c0: 2e70 7922 2c20 6c69 6e65 2033 3935 2c20  .py", line 395, 
-0001e8d0: 696e 205f 5f63 6c61 7373 6966 790d 0a20  in __classify.. 
-0001e8e0: 2020 2020 2020 2020 2020 2023 2046 696c             # Fil
-0001e8f0: 6520 222f 6f70 742f 686f 6d65 6272 6577  e "/opt/homebrew
-0001e900: 2f6c 6962 2f70 7974 686f 6e33 2e31 312f  /lib/python3.11/
-0001e910: 7369 7465 2d70 6163 6b61 6765 732f 7061  site-packages/pa
-0001e920: 6e64 6173 2f63 6f72 652f 6f70 732f 636f  ndas/core/ops/co
-0001e930: 6d6d 6f6e 2e70 7922 2c20 6c69 6e65 2037  mmon.py", line 7
-0001e940: 362c 2069 6e20 6e65 775f 6d65 7468 6f64  6, in new_method
-0001e950: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0001e960: 4669 6c65 2022 2f6f 7074 2f68 6f6d 6562  File "/opt/homeb
-0001e970: 7265 772f 6c69 622f 7079 7468 6f6e 332e  rew/lib/python3.
-0001e980: 3131 2f73 6974 652d 7061 636b 6167 6573  11/site-packages
-0001e990: 2f70 616e 6461 732f 636f 7265 2f61 7272  /pandas/core/arr
-0001e9a0: 6179 6c69 6b65 2e70 7922 2c20 6c69 6e65  aylike.py", line
-0001e9b0: 2037 302c 2069 6e20 5f5f 616e 645f 5f0d   70, in __and__.
-0001e9c0: 0a20 2020 2020 2020 2020 2020 2023 2046  .            # F
-0001e9d0: 696c 6520 222f 6f70 742f 686f 6d65 6272  ile "/opt/homebr
-0001e9e0: 6577 2f6c 6962 2f70 7974 686f 6e33 2e31  ew/lib/python3.1
-0001e9f0: 312f 7369 7465 2d70 6163 6b61 6765 732f  1/site-packages/
-0001ea00: 7061 6e64 6173 2f63 6f72 652f 7365 7269  pandas/core/seri
-0001ea10: 6573 2e70 7922 2c20 6c69 6e65 2035 3831  es.py", line 581
-0001ea20: 302c 2069 6e20 5f6c 6f67 6963 616c 5f6d  0, in _logical_m
-0001ea30: 6574 686f 640d 0a20 2020 2020 2020 2020  ethod..         
-0001ea40: 2020 2023 2046 696c 6520 222f 6f70 742f     # File "/opt/
-0001ea50: 686f 6d65 6272 6577 2f6c 6962 2f70 7974  homebrew/lib/pyt
-0001ea60: 686f 6e33 2e31 312f 7369 7465 2d70 6163  hon3.11/site-pac
-0001ea70: 6b61 6765 732f 7061 6e64 6173 2f63 6f72  kages/pandas/cor
-0001ea80: 652f 6f70 732f 6172 7261 795f 6f70 732e  e/ops/array_ops.
-0001ea90: 7079 222c 206c 696e 6520 3435 362c 2069  py", line 456, i
-0001eaa0: 6e20 6c6f 6769 6361 6c5f 6f70 0d0a 2020  n logical_op..  
-0001eab0: 2020 2020 2020 2020 2020 2320 4669 6c65            # File
-0001eac0: 2022 2f6f 7074 2f68 6f6d 6562 7265 772f   "/opt/homebrew/
-0001ead0: 6c69 622f 7079 7468 6f6e 332e 3131 2f73  lib/python3.11/s
-0001eae0: 6974 652d 7061 636b 6167 6573 2f70 616e  ite-packages/pan
-0001eaf0: 6461 732f 636f 7265 2f6f 7073 2f61 7272  das/core/ops/arr
-0001eb00: 6179 5f6f 7073 2e70 7922 2c20 6c69 6e65  ay_ops.py", line
-0001eb10: 2033 3634 2c20 696e 206e 615f 6c6f 6769   364, in na_logi
-0001eb20: 6361 6c5f 6f70 0d0a 2020 2020 2020 2020  cal_op..        
-0001eb30: 2020 2020 2320 7365 6c66 2e64 6566 6175      # self.defau
-0001eb40: 6c74 5f6c 6f67 6765 722e 6465 6275 6728  lt_logger.debug(
-0001eb50: 652c 2065 7863 5f69 6e66 6f3d 5472 7565  e, exc_info=True
-0001eb60: 290d 0a20 2020 2020 2020 2020 2020 2070  )..            p
-0001eb70: 6173 730d 0a20 2020 2020 2020 2072 6574  ass..        ret
-0001eb80: 7572 6e20 4661 6c73 650d 0a0d 0a20 2020  urn False....   
-0001eb90: 2023 2076 616c 6964 6174 6520 6966 2074   # validate if t
-0001eba0: 6865 2073 746f 636b 2068 6173 2062 6565  he stock has bee
-0001ebb0: 6e20 6861 7669 6e67 206c 6f77 6572 206c  n having lower l
-0001ebc0: 6f77 732c 206c 6f77 6572 2068 6967 6873  ows, lower highs
-0001ebd0: 0d0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-0001ebe0: 7465 4c6f 7765 7248 6967 6873 4c6f 7765  teLowerHighsLowe
-0001ebf0: 724c 6f77 7328 7365 6c66 2c20 6466 293a  rLows(self, df):
-0001ec00: 0d0a 2020 2020 2020 2020 6966 2064 6620  ..        if df 
-0001ec10: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
-0001ec20: 6629 203d 3d20 303a 0d0a 2020 2020 2020  f) == 0:..      
-0001ec30: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-0001ec40: 7365 0d0a 2020 2020 2020 2020 6461 7461  se..        data
-0001ec50: 203d 2064 662e 636f 7079 2829 0d0a 2020   = df.copy()..  
-0001ec60: 2020 2020 2020 6461 7930 203d 2064 6174        day0 = dat
-0001ec70: 610d 0a20 2020 2020 2020 2064 6179 3120  a..        day1 
-0001ec80: 3d20 6461 7461 5b31 3a5d 0d0a 2020 2020  = data[1:]..    
-0001ec90: 2020 2020 6461 7932 203d 2064 6174 615b      day2 = data[
-0001eca0: 323a 5d0d 0a20 2020 2020 2020 2064 6179  2:]..        day
-0001ecb0: 3320 3d20 6461 7461 5b33 3a5d 0d0a 2020  3 = data[3:]..  
-0001ecc0: 2020 2020 2020 6c6f 7765 7248 6967 6873        lowerHighs
-0001ecd0: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-0001ece0: 2020 2864 6179 305b 2248 6967 6822 5d2e    (day0["High"].
-0001ecf0: 696c 6f63 5b30 5d20 3c20 6461 7931 5b22  iloc[0] < day1["
-0001ed00: 4869 6768 225d 2e69 6c6f 635b 305d 290d  High"].iloc[0]).
-0001ed10: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
-0001ed20: 2028 6461 7931 5b22 4869 6768 225d 2e69   (day1["High"].i
-0001ed30: 6c6f 635b 305d 203c 2064 6179 325b 2248  loc[0] < day2["H
-0001ed40: 6967 6822 5d2e 696c 6f63 5b30 5d29 0d0a  igh"].iloc[0])..
-0001ed50: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-0001ed60: 2864 6179 325b 2248 6967 6822 5d2e 696c  (day2["High"].il
-0001ed70: 6f63 5b30 5d20 3c20 6461 7933 5b22 4869  oc[0] < day3["Hi
-0001ed80: 6768 225d 2e69 6c6f 635b 305d 290d 0a20  gh"].iloc[0]).. 
-0001ed90: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-0001eda0: 2020 6c6f 7765 724c 6f77 7320 3d20 280d    lowerLows = (.
-0001edb0: 0a20 2020 2020 2020 2020 2020 2028 6461  .            (da
-0001edc0: 7930 5b22 4c6f 7722 5d2e 696c 6f63 5b30  y0["Low"].iloc[0
-0001edd0: 5d20 3c20 6461 7931 5b22 4c6f 7722 5d2e  ] < day1["Low"].
-0001ede0: 696c 6f63 5b30 5d29 0d0a 2020 2020 2020  iloc[0])..      
-0001edf0: 2020 2020 2020 616e 6420 2864 6179 315b        and (day1[
-0001ee00: 224c 6f77 225d 2e69 6c6f 635b 305d 203c  "Low"].iloc[0] <
-0001ee10: 2064 6179 325b 224c 6f77 225d 2e69 6c6f   day2["Low"].ilo
-0001ee20: 635b 305d 290d 0a20 2020 2020 2020 2020  c[0])..         
-0001ee30: 2020 2061 6e64 2028 6461 7932 5b22 4c6f     and (day2["Lo
-0001ee40: 7722 5d2e 696c 6f63 5b30 5d20 3c20 6461  w"].iloc[0] < da
-0001ee50: 7933 5b22 4c6f 7722 5d2e 696c 6f63 5b30  y3["Low"].iloc[0
-0001ee60: 5d29 0d0a 2020 2020 2020 2020 290d 0a20  ])..        ).. 
-0001ee70: 2020 2020 2020 2068 6967 6865 7252 5349         higherRSI
-0001ee80: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-0001ee90: 2020 2864 6179 305b 2252 5349 225d 2e69    (day0["RSI"].i
-0001eea0: 6c6f 635b 305d 203c 2064 6179 315b 2252  loc[0] < day1["R
-0001eeb0: 5349 225d 2e69 6c6f 635b 305d 290d 0a20  SI"].iloc[0]).. 
-0001eec0: 2020 2020 2020 2020 2020 2061 6e64 2028             and (
-0001eed0: 6461 7931 5b22 5253 4922 5d2e 696c 6f63  day1["RSI"].iloc
-0001eee0: 5b30 5d20 3c20 6461 7932 5b22 5253 4922  [0] < day2["RSI"
-0001eef0: 5d2e 696c 6f63 5b30 5d29 0d0a 2020 2020  ].iloc[0])..    
-0001ef00: 2020 2020 2020 2020 616e 6420 2864 6179          and (day
-0001ef10: 325b 2252 5349 225d 2e69 6c6f 635b 305d  2["RSI"].iloc[0]
-0001ef20: 203c 2064 6179 335b 2252 5349 225d 2e69   < day3["RSI"].i
-0001ef30: 6c6f 635b 305d 290d 0a20 2020 2020 2020  loc[0])..       
-0001ef40: 2020 2020 2061 6e64 2064 6179 305b 2252       and day0["R
-0001ef50: 5349 225d 2e69 6c6f 635b 305d 203e 3d20  SI"].iloc[0] >= 
-0001ef60: 3530 0d0a 2020 2020 2020 2020 290d 0a20  50..        ).. 
-0001ef70: 2020 2020 2020 2072 6574 7572 6e20 6c6f         return lo
-0001ef80: 7765 7248 6967 6873 2061 6e64 206c 6f77  werHighs and low
-0001ef90: 6572 4c6f 7773 2061 6e64 2068 6967 6865  erLows and highe
-0001efa0: 7252 5349 0d0a 0d0a 2020 2020 2320 5661  rRSI....    # Va
-0001efb0: 6c69 6461 7465 2069 6620 7265 6365 6e74  lidate if recent
-0001efc0: 2076 6f6c 756d 6520 6973 206c 6f77 6573   volume is lowes
-0001efd0: 7420 6f66 206c 6173 7420 274e 2720 4461  t of last 'N' Da
-0001efe0: 7973 0d0a 2020 2020 6465 6620 7661 6c69  ys..    def vali
-0001eff0: 6461 7465 4c6f 7765 7374 566f 6c75 6d65  dateLowestVolume
-0001f000: 2873 656c 662c 2064 662c 2064 6179 7346  (self, df, daysF
-0001f010: 6f72 4c6f 7765 7374 566f 6c75 6d65 293a  orLowestVolume):
-0001f020: 0d0a 2020 2020 2020 2020 6966 2064 6620  ..        if df 
-0001f030: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
-0001f040: 6629 203d 3d20 303a 0d0a 2020 2020 2020  f) == 0:..      
-0001f050: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-0001f060: 7365 0d0a 2020 2020 2020 2020 6461 7461  se..        data
-0001f070: 203d 2064 662e 636f 7079 2829 0d0a 2020   = df.copy()..  
-0001f080: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-0001f090: 612e 6669 6c6c 6e61 2830 290d 0a20 2020  a.fillna(0)..   
-0001f0a0: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
-0001f0b0: 2e72 6570 6c61 6365 285b 6e70 2e69 6e66  .replace([np.inf
-0001f0c0: 2c20 2d6e 702e 696e 665d 2c20 3029 0d0a  , -np.inf], 0)..
-0001f0d0: 2020 2020 2020 2020 6966 2064 6179 7346          if daysF
-0001f0e0: 6f72 4c6f 7765 7374 566f 6c75 6d65 2069  orLowestVolume i
-0001f0f0: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
-0001f100: 2020 2020 2064 6179 7346 6f72 4c6f 7765       daysForLowe
-0001f110: 7374 566f 6c75 6d65 203d 2033 300d 0a20  stVolume = 30.. 
-0001f120: 2020 2020 2020 2069 6620 6c65 6e28 6461         if len(da
-0001f130: 7461 2920 3c20 6461 7973 466f 724c 6f77  ta) < daysForLow
-0001f140: 6573 7456 6f6c 756d 653a 0d0a 2020 2020  estVolume:..    
-0001f150: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-0001f160: 616c 7365 0d0a 2020 2020 2020 2020 6461  alse..        da
-0001f170: 7461 203d 2064 6174 612e 6865 6164 2864  ta = data.head(d
-0001f180: 6179 7346 6f72 4c6f 7765 7374 566f 6c75  aysForLowestVolu
-0001f190: 6d65 290d 0a20 2020 2020 2020 2072 6563  me)..        rec
-0001f1a0: 656e 7420 3d20 6461 7461 2e68 6561 6428  ent = data.head(
-0001f1b0: 3129 0d0a 2020 2020 2020 2020 6966 206c  1)..        if l
-0001f1c0: 656e 2872 6563 656e 7429 203c 2031 3a0d  en(recent) < 1:.
-0001f1d0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0001f1e0: 7572 6e20 4661 6c73 650d 0a20 2020 2020  urn False..     
-0001f1f0: 2020 2069 6620 2872 6563 656e 745b 2256     if (recent["V
-0001f200: 6f6c 756d 6522 5d2e 696c 6f63 5b30 5d20  olume"].iloc[0] 
-0001f210: 3c3d 2064 6174 612e 6465 7363 7269 6265  <= data.describe
-0001f220: 2829 5b22 566f 6c75 6d65 225d 5b22 6d69  ()["Volume"]["mi
-0001f230: 6e22 5d29 2061 6e64 2072 6563 656e 745b  n"]) and recent[
-0001f240: 0d0a 2020 2020 2020 2020 2020 2020 2256  ..            "V
-0001f250: 6f6c 756d 6522 0d0a 2020 2020 2020 2020  olume"..        
-0001f260: 5d5b 305d 2021 3d20 6e70 2e6e 616e 3a0d  ][0] != np.nan:.
-0001f270: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0001f280: 7572 6e20 5472 7565 0d0a 2020 2020 2020  urn True..      
-0001f290: 2020 7265 7475 726e 2046 616c 7365 0d0a    return False..
-0001f2a0: 0d0a 2020 2020 2320 5661 6c69 6461 7465  ..    # Validate
-0001f2b0: 204c 5450 2077 6974 6869 6e20 6c69 6d69   LTP within limi
-0001f2c0: 7473 0d0a 2020 2020 6465 6620 7661 6c69  ts..    def vali
-0001f2d0: 6461 7465 4c54 5028 7365 6c66 2c20 6466  dateLTP(self, df
-0001f2e0: 2c20 7363 7265 656e 4469 6374 2c20 7361  , screenDict, sa
-0001f2f0: 7665 4469 6374 2c20 6d69 6e4c 5450 3d4e  veDict, minLTP=N
-0001f300: 6f6e 652c 206d 6178 4c54 503d 4e6f 6e65  one, maxLTP=None
-0001f310: 2c6d 696e 4368 616e 6765 3d30 293a 0d0a  ,minChange=0):..
-0001f320: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-0001f330: 662e 636f 7079 2829 0d0a 2020 2020 2020  f.copy()..      
-0001f340: 2020 6c74 7056 616c 6964 203d 2046 616c    ltpValid = Fal
-0001f350: 7365 0d0a 2020 2020 2020 2020 6966 206d  se..        if m
-0001f360: 696e 4c54 5020 6973 204e 6f6e 653a 0d0a  inLTP is None:..
-0001f370: 2020 2020 2020 2020 2020 2020 6d69 6e4c              minL
-0001f380: 5450 203d 2073 656c 662e 636f 6e66 6967  TP = self.config
-0001f390: 4d61 6e61 6765 722e 6d69 6e4c 5450 0d0a  Manager.minLTP..
-0001f3a0: 2020 2020 2020 2020 6966 206d 6178 4c54          if maxLT
-0001f3b0: 5020 6973 204e 6f6e 653a 0d0a 2020 2020  P is None:..    
-0001f3c0: 2020 2020 2020 2020 6d61 784c 5450 203d          maxLTP =
-0001f3d0: 2073 656c 662e 636f 6e66 6967 4d61 6e61   self.configMana
-0001f3e0: 6765 722e 6d61 784c 5450 0d0a 2020 2020  ger.maxLTP..    
-0001f3f0: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
-0001f400: 6669 6c6c 6e61 2830 290d 0a20 2020 2020  fillna(0)..     
-0001f410: 2020 2064 6174 6120 3d20 6461 7461 2e72     data = data.r
-0001f420: 6570 6c61 6365 285b 6e70 2e69 6e66 2c20  eplace([np.inf, 
-0001f430: 2d6e 702e 696e 665d 2c20 3029 0d0a 2020  -np.inf], 0)..  
-0001f440: 2020 2020 2020 7265 6365 6e74 203d 2064        recent = d
-0001f450: 6174 612e 6865 6164 2831 290d 0a0d 0a20  ata.head(1).... 
-0001f460: 2020 2020 2020 2070 6374 5f63 6861 6e67         pct_chang
-0001f470: 6520 3d20 2864 6174 615b 3a3a 2d31 5d5b  e = (data[::-1][
-0001f480: 2243 6c6f 7365 225d 2e70 6374 5f63 6861  "Close"].pct_cha
-0001f490: 6e67 6528 2920 2a20 3130 3029 2e69 6c6f  nge() * 100).ilo
-0001f4a0: 635b 2d31 5d0d 0a20 2020 2020 2020 2069  c[-1]..        i
-0001f4b0: 6620 7063 745f 6368 616e 6765 203d 3d20  f pct_change == 
-0001f4c0: 6e70 2e69 6e66 206f 7220 7063 745f 6368  np.inf or pct_ch
-0001f4d0: 616e 6765 203d 3d20 2d6e 702e 696e 663a  ange == -np.inf:
-0001f4e0: 0d0a 2020 2020 2020 2020 2020 2020 7063  ..            pc
-0001f4f0: 745f 6368 616e 6765 203d 2030 0d0a 2020  t_change = 0..  
-0001f500: 2020 2020 2020 7063 745f 7361 7665 203d        pct_save =
-0001f510: 2022 252e 3166 2525 2220 2520 7063 745f   "%.1f%%" % pct_
-0001f520: 6368 616e 6765 0d0a 2020 2020 2020 2020  change..        
-0001f530: 6966 2070 6374 5f63 6861 6e67 6520 3e20  if pct_change > 
-0001f540: 302e 323a 0d0a 2020 2020 2020 2020 2020  0.2:..          
-0001f550: 2020 7063 745f 6368 616e 6765 203d 2063    pct_change = c
-0001f560: 6f6c 6f72 5465 7874 2e47 5245 454e 202b  olorText.GREEN +
-0001f570: 2028 2225 2e31 6625 2522 2025 2070 6374   ("%.1f%%" % pct
-0001f580: 5f63 6861 6e67 6529 202b 2063 6f6c 6f72  _change) + color
-0001f590: 5465 7874 2e45 4e44 0d0a 2020 2020 2020  Text.END..      
-0001f5a0: 2020 656c 6966 2070 6374 5f63 6861 6e67    elif pct_chang
-0001f5b0: 6520 3c20 2d30 2e32 3a0d 0a20 2020 2020  e < -0.2:..     
-0001f5c0: 2020 2020 2020 2070 6374 5f63 6861 6e67         pct_chang
-0001f5d0: 6520 3d20 636f 6c6f 7254 6578 742e 4641  e = colorText.FA
-0001f5e0: 494c 202b 2028 2225 2e31 6625 2522 2025  IL + ("%.1f%%" %
-0001f5f0: 2070 6374 5f63 6861 6e67 6529 202b 2063   pct_change) + c
-0001f600: 6f6c 6f72 5465 7874 2e45 4e44 0d0a 2020  olorText.END..  
-0001f610: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-0001f620: 2020 2020 2020 2020 2070 6374 5f63 6861           pct_cha
-0001f630: 6e67 6520 3d20 636f 6c6f 7254 6578 742e  nge = colorText.
-0001f640: 5741 524e 202b 2028 2225 2e31 6625 2522  WARN + ("%.1f%%"
-0001f650: 2025 2070 6374 5f63 6861 6e67 6529 202b   % pct_change) +
-0001f660: 2063 6f6c 6f72 5465 7874 2e45 4e44 0d0a   colorText.END..
-0001f670: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
-0001f680: 5b22 2543 686e 6722 5d20 3d20 7063 745f  ["%Chng"] = pct_
-0001f690: 7361 7665 0d0a 2020 2020 2020 2020 7363  save..        sc
-0001f6a0: 7265 656e 4469 6374 5b22 2543 686e 6722  reenDict["%Chng"
-0001f6b0: 5d20 3d20 7063 745f 6368 616e 6765 0d0a  ] = pct_change..
-0001f6c0: 2020 2020 2020 2020 6c74 7020 3d20 726f          ltp = ro
-0001f6d0: 756e 6428 7265 6365 6e74 5b22 436c 6f73  und(recent["Clos
-0001f6e0: 6522 5d2e 696c 6f63 5b30 5d2c 2032 290d  e"].iloc[0], 2).
-0001f6f0: 0a20 2020 2020 2020 2076 6572 6966 7953  .        verifyS
-0001f700: 7461 6765 5477 6f20 3d20 5472 7565 0d0a  tageTwo = True..
-0001f710: 2020 2020 2020 2020 6966 206c 656e 2864          if len(d
-0001f720: 6174 6129 203e 2032 3530 3a0d 0a20 2020  ata) > 250:..   
-0001f730: 2020 2020 2020 2020 2079 6561 726c 794c           yearlyL
-0001f740: 6f77 203d 2064 6174 612e 6865 6164 2832  ow = data.head(2
-0001f750: 3530 295b 2243 6c6f 7365 225d 2e6d 696e  50)["Close"].min
-0001f760: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-0001f770: 7965 6172 6c79 4869 6768 203d 2064 6174  yearlyHigh = dat
-0001f780: 612e 6865 6164 2832 3530 295b 2243 6c6f  a.head(250)["Clo
-0001f790: 7365 225d 2e6d 6178 2829 0d0a 2020 2020  se"].max()..    
-0001f7a0: 2020 2020 2020 2020 6966 206c 7470 203c          if ltp <
-0001f7b0: 2028 3220 2a20 7965 6172 6c79 4c6f 7729   (2 * yearlyLow)
-0001f7c0: 2061 6e64 206c 7470 203c 2028 302e 3735   and ltp < (0.75
-0001f7d0: 202a 2079 6561 726c 7948 6967 6829 3a0d   * yearlyHigh):.
-0001f7e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001f7f0: 2076 6572 6966 7953 7461 6765 5477 6f20   verifyStageTwo 
-0001f800: 3d20 4661 6c73 650d 0a20 2020 2020 2020  = False..       
-0001f810: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-0001f820: 6963 745b 2253 746f 636b 225d 203d 2063  ict["Stock"] = c
-0001f830: 6f6c 6f72 5465 7874 2e46 4149 4c20 2b20  olorText.FAIL + 
-0001f840: 7361 7665 4469 6374 5b22 5374 6f63 6b22  saveDict["Stock"
-0001f850: 5d20 2b20 636f 6c6f 7254 6578 742e 454e  ] + colorText.EN
-0001f860: 440d 0a20 2020 2020 2020 2069 6620 6c74  D..        if lt
-0001f870: 7020 3e3d 206d 696e 4c54 5020 616e 6420  p >= minLTP and 
-0001f880: 6c74 7020 3c3d 206d 6178 4c54 503a 0d0a  ltp <= maxLTP:..
-0001f890: 2020 2020 2020 2020 2020 2020 6c74 7056              ltpV
-0001f8a0: 616c 6964 203d 2054 7275 650d 0a20 2020  alid = True..   
-0001f8b0: 2020 2020 2020 2020 2069 6620 6d69 6e43           if minC
-0001f8c0: 6861 6e67 6520 213d 2030 3a0d 0a20 2020  hange != 0:..   
-0001f8d0: 2020 2020 2020 2020 2020 2020 2023 2055               # U
-0001f8e0: 7365 7220 6861 7320 7375 7070 6c69 6564  ser has supplied
-0001f8f0: 2073 6f6d 6520 6669 6c74 6572 2066 6f72   some filter for
-0001f900: 2070 6572 6365 6e74 6167 6520 6368 616e   percentage chan
-0001f910: 6765 0d0a 2020 2020 2020 2020 2020 2020  ge..            
-0001f920: 2020 2020 6c74 7056 616c 6964 203d 2066      ltpValid = f
-0001f930: 6c6f 6174 2873 7472 2870 6374 5f73 6176  loat(str(pct_sav
-0001f940: 6529 2e72 6570 6c61 6365 2822 2522 2c22  e).replace("%","
-0001f950: 2229 2920 3e3d 206d 696e 4368 616e 6765  ")) >= minChange
-0001f960: 0d0a 2020 2020 2020 2020 2020 2020 7361  ..            sa
-0001f970: 7665 4469 6374 5b22 4c54 5022 5d20 3d20  veDict["LTP"] = 
-0001f980: 726f 756e 6428 6c74 702c 2032 290d 0a20  round(ltp, 2).. 
-0001f990: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-0001f9a0: 6e44 6963 745b 224c 5450 225d 203d 2028  nDict["LTP"] = (
-0001f9b0: 636f 6c6f 7254 6578 742e 4752 4545 4e20  colorText.GREEN 
-0001f9c0: 6966 206c 7470 5661 6c69 6420 656c 7365  if ltpValid else
-0001f9d0: 2063 6f6c 6f72 5465 7874 2e46 4149 4c29   colorText.FAIL)
-0001f9e0: 202b 2028 2225 2e32 6622 2025 206c 7470   + ("%.2f" % ltp
-0001f9f0: 2920 2b20 636f 6c6f 7254 6578 742e 454e  ) + colorText.EN
-0001fa00: 440d 0a20 2020 2020 2020 2020 2020 2072  D..            r
-0001fa10: 6574 7572 6e20 6c74 7056 616c 6964 2c20  eturn ltpValid, 
-0001fa20: 7665 7269 6679 5374 6167 6554 776f 0d0a  verifyStageTwo..
-0001fa30: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
-0001fa40: 6374 5b22 4c54 5022 5d20 3d20 636f 6c6f  ct["LTP"] = colo
-0001fa50: 7254 6578 742e 4641 494c 202b 2028 2225  rText.FAIL + ("%
-0001fa60: 2e32 6622 2025 206c 7470 2920 2b20 636f  .2f" % ltp) + co
-0001fa70: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
-0001fa80: 2020 2020 2073 6176 6544 6963 745b 224c       saveDict["L
-0001fa90: 5450 225d 203d 2072 6f75 6e64 286c 7470  TP"] = round(ltp
-0001faa0: 2c20 3229 0d0a 2020 2020 2020 2020 7265  , 2)..        re
-0001fab0: 7475 726e 206c 7470 5661 6c69 642c 2076  turn ltpValid, v
-0001fac0: 6572 6966 7953 7461 6765 5477 6f0d 0a0d  erifyStageTwo...
-0001fad0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-0001fae0: 654c 5450 466f 7250 6f72 7466 6f6c 696f  eLTPForPortfolio
-0001faf0: 4361 6c63 2873 656c 662c 2064 662c 2073  Calc(self, df, s
-0001fb00: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
-0001fb10: 6963 742c 7265 7175 6573 7465 6450 6572  ict,requestedPer
-0001fb20: 696f 643d 3029 3a0d 0a20 2020 2020 2020  iod=0):..       
-0001fb30: 2064 6174 6120 3d20 6466 2e63 6f70 7928   data = df.copy(
-0001fb40: 290d 0a20 2020 2020 2020 2070 6572 696f  )..        perio
-0001fb50: 6473 203d 2073 656c 662e 636f 6e66 6967  ds = self.config
-0001fb60: 4d61 6e61 6765 722e 7065 7269 6f64 7352  Manager.periodsR
-0001fb70: 616e 6765 0d0a 2020 2020 2020 2020 6966  ange..        if
-0001fb80: 2072 6571 7565 7374 6564 5065 7269 6f64   requestedPeriod
-0001fb90: 203e 2030 2061 6e64 2072 6571 7565 7374   > 0 and request
-0001fba0: 6564 5065 7269 6f64 206e 6f74 2069 6e20  edPeriod not in 
-0001fbb0: 7065 7269 6f64 733a 0d0a 2020 2020 2020  periods:..      
-0001fbc0: 2020 2020 2020 7065 7269 6f64 732e 6170        periods.ap
-0001fbd0: 7065 6e64 2872 6571 7565 7374 6564 5065  pend(requestedPe
-0001fbe0: 7269 6f64 290d 0a20 2020 2020 2020 2070  riod)..        p
-0001fbf0: 7265 7669 6f75 735f 7265 6365 6e74 203d  revious_recent =
-0001fc00: 2064 6174 612e 6865 6164 2831 290d 0a20   data.head(1).. 
-0001fc10: 2020 2020 2020 2070 7265 7669 6f75 735f         previous_
-0001fc20: 7265 6365 6e74 2e72 6573 6574 5f69 6e64  recent.reset_ind
-0001fc30: 6578 2869 6e70 6c61 6365 3d54 7275 6529  ex(inplace=True)
-0001fc40: 0d0a 2020 2020 2020 2020 6361 6c63 5f64  ..        calc_d
-0001fc50: 6174 6520 3d20 7374 7228 7072 6576 696f  ate = str(previo
-0001fc60: 7573 5f72 6563 656e 742e 696c 6f63 5b3a  us_recent.iloc[:
-0001fc70: 2c20 305d 5b30 5d29 2e73 706c 6974 2822  , 0][0]).split("
-0001fc80: 2022 295b 305d 0d0a 2020 2020 2020 2020   ")[0]..        
-0001fc90: 666f 7220 7072 6420 696e 2070 6572 696f  for prd in perio
-0001fca0: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
-0001fcb0: 2069 6620 6c65 6e28 6461 7461 2920 3e3d   if len(data) >=
-0001fcc0: 2070 7264 202b 2031 3a0d 0a20 2020 2020   prd + 1:..     
-0001fcd0: 2020 2020 2020 2020 2020 2070 7265 764c             prevL
-0001fce0: 7470 203d 2064 6174 615b 2243 6c6f 7365  tp = data["Close
-0001fcf0: 225d 2e69 6c6f 635b 305d 0d0a 2020 2020  "].iloc[0]..    
-0001fd00: 2020 2020 2020 2020 2020 2020 6c74 7054              ltpT
-0001fd10: 6479 203d 2064 6174 615b 2243 6c6f 7365  dy = data["Close
-0001fd20: 225d 2e69 6c6f 635b 7072 645d 0d0a 2020  "].iloc[prd]..  
-0001fd30: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0001fd40: 2069 7369 6e73 7461 6e63 6528 7072 6576   isinstance(prev
-0001fd50: 4c74 702c 7064 2e53 6572 6965 7329 3a0d  Ltp,pd.Series):.
-0001fd60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001fd70: 2020 2020 2070 7265 764c 7470 203d 2070       prevLtp = p
-0001fd80: 7265 764c 7470 5b30 5d0d 0a20 2020 2020  revLtp[0]..     
-0001fd90: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0001fda0: 7470 5464 7920 3d20 6c74 7054 6479 5b30  tpTdy = ltpTdy[0
-0001fdb0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-0001fdc0: 2020 2073 6372 6565 6e44 6963 745b 6622     screenDict[f"
-0001fdd0: 4c54 507b 7072 647d 225d 203d 2028 0d0a  LTP{prd}"] = (..
-0001fde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fdf0: 2020 2020 2863 6f6c 6f72 5465 7874 2e47      (colorText.G
-0001fe00: 5245 454e 2069 6620 286c 7470 5464 7920  REEN if (ltpTdy 
-0001fe10: 3e3d 2070 7265 764c 7470 2920 656c 7365  >= prevLtp) else
-0001fe20: 2028 636f 6c6f 7254 6578 742e 4641 494c   (colorText.FAIL
-0001fe30: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0001fe40: 2020 2020 2020 2020 2b20 7374 7228 227b          + str("{
-0001fe50: 3a2e 3266 7d22 2e66 6f72 6d61 7428 6c74  :.2f}".format(lt
-0001fe60: 7054 6479 2929 0d0a 2020 2020 2020 2020  pTdy))..        
-0001fe70: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
-0001fe80: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
-0001fe90: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
-0001fea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001feb0: 7363 7265 656e 4469 6374 5b66 2247 726f  screenDict[f"Gro
-0001fec0: 7774 687b 7072 647d 225d 203d 2028 0d0a  wth{prd}"] = (..
-0001fed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fee0: 2020 2020 2863 6f6c 6f72 5465 7874 2e47      (colorText.G
-0001fef0: 5245 454e 2069 6620 286c 7470 5464 7920  REEN if (ltpTdy 
-0001ff00: 3e3d 2070 7265 764c 7470 2920 656c 7365  >= prevLtp) else
-0001ff10: 2028 636f 6c6f 7254 6578 742e 4641 494c   (colorText.FAIL
-0001ff20: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0001ff30: 2020 2020 2020 2020 2b20 7374 7228 227b          + str("{
-0001ff40: 3a2e 3266 7d22 2e66 6f72 6d61 7428 6c74  :.2f}".format(lt
-0001ff50: 7054 6479 202d 2070 7265 764c 7470 2929  pTdy - prevLtp))
-0001ff60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001ff70: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
-0001ff80: 742e 454e 440d 0a20 2020 2020 2020 2020  t.END..         
-0001ff90: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-0001ffa0: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
-0001ffb0: 6374 5b66 224c 5450 7b70 7264 7d22 5d20  ct[f"LTP{prd}"] 
-0001ffc0: 3d20 726f 756e 6428 6c74 7054 6479 2c20  = round(ltpTdy, 
-0001ffd0: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
-0001ffe0: 2020 2020 7361 7665 4469 6374 5b66 2247      saveDict[f"G
-0001fff0: 726f 7774 687b 7072 647d 225d 203d 2072  rowth{prd}"] = r
-00020000: 6f75 6e64 286c 7470 5464 7920 2d20 7072  ound(ltpTdy - pr
-00020010: 6576 4c74 702c 2032 290d 0a20 2020 2020  evLtp, 2)..     
-00020020: 2020 2020 2020 2020 2020 2069 6620 7072             if pr
-00020030: 6420 3d3d 2032 3220 6f72 2028 7072 6420  d == 22 or (prd 
-00020040: 3d3d 2072 6571 7565 7374 6564 5065 7269  == requestedPeri
-00020050: 6f64 293a 0d0a 2020 2020 2020 2020 2020  od):..          
-00020060: 2020 2020 2020 2020 2020 6368 616e 6765            change
-00020070: 5065 7263 656e 7420 3d20 726f 756e 6428  Percent = round(
-00020080: 2828 7072 6576 4c74 702d 6c74 7054 6479  ((prevLtp-ltpTdy
-00020090: 2920 6966 2072 6571 7565 7374 6564 5065  ) if requestedPe
-000200a0: 7269 6f64 203d 3d30 2065 6c73 6520 286c  riod ==0 else (l
-000200b0: 7470 5464 7920 2d20 7072 6576 4c74 7029  tpTdy - prevLtp)
-000200c0: 292a 3130 302f 6c74 7054 6479 2c20 3229  )*100/ltpTdy, 2)
-000200d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000200e0: 2020 2020 2020 7361 7665 4469 6374 5b66        saveDict[f
-000200f0: 227b 7072 647d 2d50 6420 2522 5d20 3d20  "{prd}-Pd %"] = 
-00020100: 6622 7b63 6861 6e67 6550 6572 6365 6e74  f"{changePercent
-00020110: 7d25 220d 0a20 2020 2020 2020 2020 2020  }%"..           
-00020120: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-00020130: 6963 745b 6622 7b70 7264 7d2d 5064 2025  ict[f"{prd}-Pd %
-00020140: 225d 203d 2028 636f 6c6f 7254 6578 742e  "] = (colorText.
-00020150: 4752 4545 4e20 6966 2063 6861 6e67 6550  GREEN if changeP
-00020160: 6572 6365 6e74 203e 3d30 2065 6c73 6520  ercent >=0 else 
-00020170: 636f 6c6f 7254 6578 742e 4641 494c 2920  colorText.FAIL) 
-00020180: 2b20 6622 7b63 6861 6e67 6550 6572 6365  + f"{changePerce
-00020190: 6e74 7d25 2220 2b20 636f 6c6f 7254 6578  nt}%" + colorTex
-000201a0: 742e 454e 440d 0a20 2020 2020 2020 2020  t.END..         
-000201b0: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
-000201c0: 745b 2244 6174 6522 5d20 3d20 6361 6c63  t["Date"] = calc
-000201d0: 5f64 6174 650d 0a20 2020 2020 2020 2020  _date..         
-000201e0: 2020 2020 2020 2073 6176 6544 6963 745b         saveDict[
-000201f0: 2244 6174 6522 5d20 3d20 6361 6c63 5f64  "Date"] = calc_d
-00020200: 6174 650d 0a20 2020 2020 2020 2020 2020  ate..           
-00020210: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00020220: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
-00020230: 5b66 224c 5450 7b70 7264 7d22 5d20 3d20  [f"LTP{prd}"] = 
-00020240: 6e70 2e6e 616e 0d0a 2020 2020 2020 2020  np.nan..        
-00020250: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
-00020260: 5b66 2247 726f 7774 687b 7072 647d 225d  [f"Growth{prd}"]
-00020270: 203d 206e 702e 6e61 6e0d 0a20 2020 2020   = np.nan..     
-00020280: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-00020290: 6e44 6963 745b 2244 6174 6522 5d20 3d20  nDict["Date"] = 
-000202a0: 6361 6c63 5f64 6174 650d 0a20 2020 2020  calc_date..     
-000202b0: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
-000202c0: 6963 745b 2244 6174 6522 5d20 3d20 6361  ict["Date"] = ca
-000202d0: 6c63 5f64 6174 650d 0a0d 0a20 2020 2023  lc_date....    #
-000202e0: 2046 696e 6420 7374 6f63 6b73 2074 6861   Find stocks tha
-000202f0: 7420 6172 6520 6265 6172 6973 6820 696e  t are bearish in
-00020300: 7472 6164 6179 3a20 4d61 6364 2048 6973  traday: Macd His
-00020310: 746f 6772 616d 206e 6567 6174 6976 650d  togram negative.
-00020320: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-00020330: 654d 4143 4448 6973 746f 6772 616d 4265  eMACDHistogramBe
-00020340: 6c6f 7730 2873 656c 662c 2064 6629 3a0d  low0(self, df):.
-00020350: 0a20 2020 2020 2020 2069 6620 6466 2069  .        if df i
-00020360: 7320 4e6f 6e65 206f 7220 6c65 6e28 6466  s None or len(df
-00020370: 2920 3d3d 2030 3a0d 0a20 2020 2020 2020  ) == 0:..       
-00020380: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-00020390: 650d 0a20 2020 2020 2020 2064 6174 6120  e..        data 
-000203a0: 3d20 6466 2e63 6f70 7928 290d 0a20 2020  = df.copy()..   
-000203b0: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
-000203c0: 2e66 696c 6c6e 6128 3029 0d0a 2020 2020  .fillna(0)..    
-000203d0: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
-000203e0: 7265 706c 6163 6528 5b6e 702e 696e 662c  replace([np.inf,
-000203f0: 202d 6e70 2e69 6e66 5d2c 2030 290d 0a20   -np.inf], 0).. 
-00020400: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-00020410: 7461 5b3a 3a2d 315d 2020 2320 5265 7665  ta[::-1]  # Reve
-00020420: 7273 6520 7468 6520 6461 7461 6672 616d  rse the datafram
-00020430: 6520 736f 2074 6861 7420 6974 7320 7468  e so that its th
-00020440: 6520 6f6c 6465 7374 2064 6174 6520 6669  e oldest date fi
-00020450: 7273 740d 0a20 2020 2020 2020 206d 6163  rst..        mac
-00020460: 6420 3d20 706b 7461 6c69 622e 4d41 4344  d = pktalib.MACD
-00020470: 2864 6174 615b 2243 6c6f 7365 225d 2c20  (data["Close"], 
-00020480: 3132 2c20 3236 2c20 3929 5b32 5d2e 7461  12, 26, 9)[2].ta
-00020490: 696c 2831 290d 0a20 2020 2020 2020 2072  il(1)..        r
-000204a0: 6574 7572 6e20 6d61 6364 2e69 6c6f 635b  eturn macd.iloc[
-000204b0: 3a31 5d5b 305d 203c 2030 0d0a 0d0a 2020  :1][0] < 0....  
-000204c0: 2020 2340 6d65 6173 7572 655f 7469 6d65    #@measure_time
-000204d0: 0d0a 2020 2020 2320 4669 6e64 2069 6620  ..    # Find if 
-000204e0: 7374 6f63 6b20 6761 696e 696e 6720 6275  stock gaining bu
-000204f0: 6c6c 6973 6820 6d6f 6d65 6e74 756d 0d0a  llish momentum..
-00020500: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-00020510: 4d6f 6d65 6e74 756d 2873 656c 662c 2064  Momentum(self, d
-00020520: 662c 2073 6372 6565 6e44 6963 742c 2073  f, screenDict, s
-00020530: 6176 6544 6963 7429 3a0d 0a20 2020 2020  aveDict):..     
-00020540: 2020 2069 6620 6466 2069 7320 4e6f 6e65     if df is None
-00020550: 206f 7220 6c65 6e28 6466 2920 3d3d 2030   or len(df) == 0
-00020560: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00020570: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
-00020580: 2020 2020 2064 6174 6120 3d20 6466 2e63       data = df.c
-00020590: 6f70 7928 290d 0a20 2020 2020 2020 2074  opy()..        t
-000205a0: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
-000205b0: 2064 6174 6120 3d20 6461 7461 2e68 6561   data = data.hea
-000205c0: 6428 3329 0d0a 2020 2020 2020 2020 2020  d(3)..          
-000205d0: 2020 6966 206c 656e 2864 6174 6129 203c    if len(data) <
-000205e0: 2033 3a0d 0a20 2020 2020 2020 2020 2020   3:..           
-000205f0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-00020600: 650d 0a20 2020 2020 2020 2020 2020 2066  e..            f
-00020610: 6f72 2072 6f77 2069 6e20 6461 7461 2e69  or row in data.i
-00020620: 7465 7272 6f77 7328 293a 0d0a 2020 2020  terrows():..    
-00020630: 2020 2020 2020 2020 2020 2020 2320 416c              # Al
-00020640: 6c20 3320 6361 6e64 6c65 7320 7368 6f75  l 3 candles shou
-00020650: 6c64 2062 6520 4772 6565 6e20 616e 6420  ld be Green and 
-00020660: 4e4f 5420 4369 7263 7569 7473 0d0a 2020  NOT Circuits..  
-00020670: 2020 2020 2020 2020 2020 2020 2020 7963                yc
-00020680: 203d 2072 6f77 5b31 5d5b 2243 6c6f 7365   = row[1]["Close
-00020690: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
-000206a0: 2020 2020 796f 203d 2072 6f77 5b31 5d5b      yo = row[1][
-000206b0: 224f 7065 6e22 5d0d 0a20 2020 2020 2020  "Open"]..       
-000206c0: 2020 2020 2020 2020 2069 6620 7963 203c           if yc <
-000206d0: 3d20 796f 3a0d 0a20 2020 2020 2020 2020  = yo:..         
-000206e0: 2020 2020 2020 2020 2020 2023 2073 656c             # sel
-000206f0: 662e 6465 6661 756c 745f 6c6f 6767 6572  f.default_logger
-00020700: 2e69 6e66 6f28 0d0a 2020 2020 2020 2020  .info(..        
-00020710: 2020 2020 2020 2020 2020 2020 2320 2020              #   
-00020720: 2020 6627 5374 6f63 6b3a 7b73 6176 6544    f'Stock:{saveD
-00020730: 6963 745b 2253 746f 636b 225d 7d2c 2069  ict["Stock"]}, i
-00020740: 7320 6e6f 7420 6120 6d6f 6d65 6e74 756d  s not a momentum
-00020750: 2d67 6169 6e65 7220 6265 6361 7573 6520  -gainer because 
-00020760: 7965 7374 6572 6461 792d 636c 6f73 6520  yesterday-close 
-00020770: 287b 7963 7d29 203c 3d20 7965 7374 6572  ({yc}) <= yester
-00020780: 6461 792d 6f70 656e 2028 7b79 6f7d 2927  day-open ({yo})'
-00020790: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000207a0: 2020 2020 2020 2320 290d 0a20 2020 2020        # )..     
-000207b0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000207c0: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
-000207d0: 2020 2020 2020 2020 206f 7065 6e44 6573           openDes
-000207e0: 6320 3d20 6461 7461 2e73 6f72 745f 7661  c = data.sort_va
-000207f0: 6c75 6573 2862 793d 5b22 4f70 656e 225d  lues(by=["Open"]
-00020800: 2c20 6173 6365 6e64 696e 673d 4661 6c73  , ascending=Fals
-00020810: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-00020820: 636c 6f73 6544 6573 6320 3d20 6461 7461  closeDesc = data
-00020830: 2e73 6f72 745f 7661 6c75 6573 2862 793d  .sort_values(by=
-00020840: 5b22 436c 6f73 6522 5d2c 2061 7363 656e  ["Close"], ascen
-00020850: 6469 6e67 3d46 616c 7365 290d 0a20 2020  ding=False)..   
-00020860: 2020 2020 2020 2020 2076 6f6c 4465 7363           volDesc
-00020870: 203d 2064 6174 612e 736f 7274 5f76 616c   = data.sort_val
-00020880: 7565 7328 6279 3d5b 2256 6f6c 756d 6522  ues(by=["Volume"
-00020890: 5d2c 2061 7363 656e 6469 6e67 3d46 616c  ], ascending=Fal
-000208a0: 7365 290d 0a20 2020 2020 2020 2020 2020  se)..           
-000208b0: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
-000208c0: 2020 2020 2020 2069 6620 280d 0a20 2020         if (..   
+0001a890: 615b 3a3a 2d31 5d20 2023 2052 6576 6572  a[::-1]  # Rever
+0001a8a0: 7365 2074 6865 2064 6174 6166 7261 6d65  se the dataframe
+0001a8b0: 0d0a 2020 2020 2020 2020 2320 6461 7461  ..        # data
+0001a8c0: 203d 2064 6174 612e 6669 6c6c 6e61 2830   = data.fillna(0
+0001a8d0: 290d 0a20 2020 2020 2020 2023 2064 6174  )..        # dat
+0001a8e0: 6120 3d20 6461 7461 2e72 6570 6c61 6365  a = data.replace
+0001a8f0: 285b 6e70 2e69 6e66 2c20 2d6e 702e 696e  ([np.inf, -np.in
+0001a900: 665d 2c20 3029 0d0a 2020 2020 2020 2020  f], 0)..        
+0001a910: 6675 6c6c 4461 7461 203d 2064 6174 610d  fullData = data.
+0001a920: 0a20 2020 2020 2020 2074 7269 6d6d 6564  .        trimmed
+0001a930: 4461 7461 203d 2064 6174 612e 6865 6164  Data = data.head
+0001a940: 2864 6179 7354 6f4c 6f6f 6b62 6163 6b29  (daysToLookback)
+0001a950: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0001a960: 2028 6675 6c6c 4461 7461 2c20 7472 696d   (fullData, trim
+0001a970: 6d65 6444 6174 6129 0d0a 0d0a 2020 2020  medData)....    
+0001a980: 2320 5661 6c69 6461 7465 2069 6620 7468  # Validate if th
+0001a990: 6520 7374 6f63 6b20 6973 2062 756c 6c69  e stock is bulli
+0001a9a0: 7368 2069 6e20 7468 6520 7368 6f72 7420  sh in the short 
+0001a9b0: 7465 726d 0d0a 2020 2020 6465 6620 7661  term..    def va
+0001a9c0: 6c69 6461 7465 3135 4d69 6e75 7465 5072  lidate15MinutePr
+0001a9d0: 6963 6556 6f6c 756d 6542 7265 616b 6f75  iceVolumeBreakou
+0001a9e0: 7428 7365 6c66 2c20 6466 293a 0d0a 2020  t(self, df):..  
+0001a9f0: 2020 2020 2020 6966 2064 6620 6973 204e        if df is N
+0001aa00: 6f6e 6520 6f72 206c 656e 2864 6629 203d  one or len(df) =
+0001aa10: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
+0001aa20: 2020 7265 7475 726e 2046 616c 7365 0d0a    return False..
+0001aa30: 2020 2020 2020 2020 2320 6874 7470 733a          # https:
+0001aa40: 2f2f 6368 6172 7469 6e6b 2e63 6f6d 2f73  //chartink.com/s
+0001aa50: 6372 6565 6e65 722f 3135 2d6d 696e 2d70  creener/15-min-p
+0001aa60: 7269 6365 2d76 6f6c 756d 652d 6272 6561  rice-volume-brea
+0001aa70: 6b6f 7574 0d0a 2020 2020 2020 2020 6461  kout..        da
+0001aa80: 7461 203d 2064 662e 636f 7079 2829 0d0a  ta = df.copy()..
+0001aa90: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+0001aaa0: 6174 612e 6669 6c6c 6e61 2830 290d 0a20  ata.fillna(0).. 
+0001aab0: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
+0001aac0: 7461 2e72 6570 6c61 6365 285b 6e70 2e69  ta.replace([np.i
+0001aad0: 6e66 2c20 2d6e 702e 696e 665d 2c20 3029  nf, -np.inf], 0)
+0001aae0: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
+0001aaf0: 2064 6174 615b 3a3a 2d31 5d20 2023 2052   data[::-1]  # R
+0001ab00: 6576 6572 7365 2074 6865 2064 6174 6166  everse the dataf
+0001ab10: 7261 6d65 2073 6f20 7468 6174 2069 7473  rame so that its
+0001ab20: 2074 6865 206f 6c64 6573 7420 6461 7465   the oldest date
+0001ab30: 2066 6972 7374 0d0a 2020 2020 2020 2020   first..        
+0001ab40: 6461 7461 5b22 534d 4132 3022 5d20 3d20  data["SMA20"] = 
+0001ab50: 706b 7461 6c69 622e 534d 4128 6461 7461  pktalib.SMA(data
+0001ab60: 5b22 436c 6f73 6522 5d2c 2032 3029 0d0a  ["Close"], 20)..
+0001ab70: 2020 2020 2020 2020 6461 7461 5b22 534d          data["SM
+0001ab80: 4132 3056 225d 203d 2070 6b74 616c 6962  A20V"] = pktalib
+0001ab90: 2e53 4d41 2864 6174 615b 2256 6f6c 756d  .SMA(data["Volum
+0001aba0: 6522 5d2c 2032 3029 0d0a 2020 2020 2020  e"], 20)..      
+0001abb0: 2020 6461 7461 203d 2064 6174 615b 0d0a    data = data[..
+0001abc0: 2020 2020 2020 2020 2020 2020 3a3a 2d31              ::-1
+0001abd0: 0d0a 2020 2020 2020 2020 5d20 2023 2052  ..        ]  # R
+0001abe0: 6576 6572 7365 2074 6865 2064 6174 6166  everse the dataf
+0001abf0: 7261 6d65 2073 6f20 7468 6174 2069 7427  rame so that it'
+0001ac00: 7320 7468 6520 6d6f 7374 2072 6563 656e  s the most recen
+0001ac10: 7420 6461 7465 2066 6972 7374 0d0a 2020  t date first..  
+0001ac20: 2020 2020 2020 7265 6365 6e74 203d 2064        recent = d
+0001ac30: 6174 612e 6865 6164 2833 290d 0a20 2020  ata.head(3)..   
+0001ac40: 2020 2020 2069 6620 6c65 6e28 7265 6365       if len(rece
+0001ac50: 6e74 2920 3c20 333a 0d0a 2020 2020 2020  nt) < 3:..      
+0001ac60: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+0001ac70: 7365 0d0a 2020 2020 2020 2020 636f 6e64  se..        cond
+0001ac80: 3120 3d20 7265 6365 6e74 5b22 436c 6f73  1 = recent["Clos
+0001ac90: 6522 5d2e 696c 6f63 5b30 5d20 3e20 7265  e"].iloc[0] > re
+0001aca0: 6365 6e74 5b22 436c 6f73 6522 5d2e 696c  cent["Close"].il
+0001acb0: 6f63 5b31 5d0d 0a20 2020 2020 2020 2063  oc[1]..        c
+0001acc0: 6f6e 6432 203d 2063 6f6e 6431 2061 6e64  ond2 = cond1 and
+0001acd0: 2028 7265 6365 6e74 5b22 436c 6f73 6522   (recent["Close"
+0001ace0: 5d2e 696c 6f63 5b30 5d20 3e20 7265 6365  ].iloc[0] > rece
+0001acf0: 6e74 5b22 534d 4132 3022 5d2e 696c 6f63  nt["SMA20"].iloc
+0001ad00: 5b30 5d29 0d0a 2020 2020 2020 2020 636f  [0])..        co
+0001ad10: 6e64 3320 3d20 636f 6e64 3220 616e 6420  nd3 = cond2 and 
+0001ad20: 2872 6563 656e 745b 2243 6c6f 7365 225d  (recent["Close"]
+0001ad30: 2e69 6c6f 635b 315d 203e 2072 6563 656e  .iloc[1] > recen
+0001ad40: 745b 2248 6967 6822 5d2e 696c 6f63 5b32  t["High"].iloc[2
+0001ad50: 5d29 0d0a 2020 2020 2020 2020 636f 6e64  ])..        cond
+0001ad60: 3420 3d20 636f 6e64 3320 616e 6420 2872  4 = cond3 and (r
+0001ad70: 6563 656e 745b 2256 6f6c 756d 6522 5d2e  ecent["Volume"].
+0001ad80: 696c 6f63 5b30 5d20 3e20 7265 6365 6e74  iloc[0] > recent
+0001ad90: 5b22 534d 4132 3056 225d 2e69 6c6f 635b  ["SMA20V"].iloc[
+0001ada0: 305d 290d 0a20 2020 2020 2020 2063 6f6e  0])..        con
+0001adb0: 6435 203d 2063 6f6e 6434 2061 6e64 2028  d5 = cond4 and (
+0001adc0: 7265 6365 6e74 5b22 566f 6c75 6d65 225d  recent["Volume"]
+0001add0: 2e69 6c6f 635b 315d 203e 2072 6563 656e  .iloc[1] > recen
+0001ade0: 745b 2253 4d41 3230 5622 5d2e 696c 6f63  t["SMA20V"].iloc
+0001adf0: 5b30 5d29 0d0a 2020 2020 2020 2020 7265  [0])..        re
+0001ae00: 7475 726e 2063 6f6e 6435 0d0a 0d0a 2020  turn cond5....  
+0001ae10: 2020 6465 6620 7661 6c69 6461 7465 4275    def validateBu
+0001ae20: 6c6c 6973 6846 6f72 546f 6d6f 7272 6f77  llishForTomorrow
+0001ae30: 2873 656c 662c 2064 6629 3a0d 0a20 2020  (self, df):..   
+0001ae40: 2020 2020 2069 6620 6466 2069 7320 4e6f       if df is No
+0001ae50: 6e65 206f 7220 6c65 6e28 6466 2920 3d3d  ne or len(df) ==
+0001ae60: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
+0001ae70: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
+0001ae80: 2020 2020 2020 2064 6174 6120 3d20 6466         data = df
+0001ae90: 2e63 6f70 7928 290d 0a20 2020 2020 2020  .copy()..       
+0001aea0: 2023 2068 7474 7073 3a2f 2f63 6861 7274   # https://chart
+0001aeb0: 696e 6b2e 636f 6d2f 7363 7265 656e 6572  ink.com/screener
+0001aec0: 2f62 756c 6c69 7368 2d66 6f72 2d74 6f6d  /bullish-for-tom
+0001aed0: 6f72 726f 770d 0a20 2020 2020 2020 2064  orrow..        d
+0001aee0: 6174 6120 3d20 6461 7461 2e66 696c 6c6e  ata = data.filln
+0001aef0: 6128 3029 0d0a 2020 2020 2020 2020 6461  a(0)..        da
+0001af00: 7461 203d 2064 6174 612e 7265 706c 6163  ta = data.replac
+0001af10: 6528 5b6e 702e 696e 662c 202d 6e70 2e69  e([np.inf, -np.i
+0001af20: 6e66 5d2c 2030 290d 0a20 2020 2020 2020  nf], 0)..       
+0001af30: 2064 6174 6120 3d20 6461 7461 5b3a 3a2d   data = data[::-
+0001af40: 315d 2020 2320 5265 7665 7273 6520 7468  1]  # Reverse th
+0001af50: 6520 6461 7461 6672 616d 6520 736f 2074  e dataframe so t
+0001af60: 6861 7420 6974 7320 7468 6520 6f6c 6465  hat its the olde
+0001af70: 7374 2064 6174 6520 6669 7273 740d 0a20  st date first.. 
+0001af80: 2020 2020 2020 206d 6163 644c 696e 6520         macdLine 
+0001af90: 3d20 706b 7461 6c69 622e 4d41 4344 2864  = pktalib.MACD(d
+0001afa0: 6174 615b 2243 6c6f 7365 225d 2c20 3132  ata["Close"], 12
+0001afb0: 2c20 3236 2c20 3929 5b30 5d2e 7461 696c  , 26, 9)[0].tail
+0001afc0: 2833 290d 0a20 2020 2020 2020 206d 6163  (3)..        mac
+0001afd0: 6453 6967 6e61 6c20 3d20 706b 7461 6c69  dSignal = pktali
+0001afe0: 622e 4d41 4344 2864 6174 615b 2243 6c6f  b.MACD(data["Clo
+0001aff0: 7365 225d 2c20 3132 2c20 3236 2c20 3929  se"], 12, 26, 9)
+0001b000: 5b31 5d2e 7461 696c 2833 290d 0a20 2020  [1].tail(3)..   
+0001b010: 2020 2020 206d 6163 6448 6973 7420 3d20       macdHist = 
+0001b020: 706b 7461 6c69 622e 4d41 4344 2864 6174  pktalib.MACD(dat
+0001b030: 615b 2243 6c6f 7365 225d 2c20 3132 2c20  a["Close"], 12, 
+0001b040: 3236 2c20 3929 5b32 5d2e 7461 696c 2833  26, 9)[2].tail(3
+0001b050: 290d 0a0d 0a20 2020 2020 2020 2072 6574  )....        ret
+0001b060: 7572 6e20 280d 0a20 2020 2020 2020 2020  urn (..         
+0001b070: 2020 2028 6d61 6364 4869 7374 2e69 6c6f     (macdHist.ilo
+0001b080: 635b 3a31 5d2e 696c 6f63 5b30 5d20 3c20  c[:1].iloc[0] < 
+0001b090: 6d61 6364 4869 7374 2e69 6c6f 635b 3a32  macdHist.iloc[:2
+0001b0a0: 5d2e 696c 6f63 5b31 5d29 0d0a 2020 2020  ].iloc[1])..    
+0001b0b0: 2020 2020 2020 2020 616e 6420 286d 6163          and (mac
+0001b0c0: 6448 6973 742e 696c 6f63 5b3a 335d 2e69  dHist.iloc[:3].i
+0001b0d0: 6c6f 635b 325d 203e 206d 6163 6448 6973  loc[2] > macdHis
+0001b0e0: 742e 696c 6f63 5b3a 325d 2e69 6c6f 635b  t.iloc[:2].iloc[
+0001b0f0: 315d 290d 0a20 2020 2020 2020 2020 2020  1])..           
+0001b100: 2061 6e64 2028 0d0a 2020 2020 2020 2020   and (..        
+0001b110: 2020 2020 2020 2020 286d 6163 644c 696e          (macdLin
+0001b120: 652e 696c 6f63 5b3a 335d 2e69 6c6f 635b  e.iloc[:3].iloc[
+0001b130: 325d 202d 206d 6163 6453 6967 6e61 6c2e  2] - macdSignal.
+0001b140: 696c 6f63 5b3a 335d 2e69 6c6f 635b 325d  iloc[:3].iloc[2]
+0001b150: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001b160: 2020 202d 2028 6d61 6364 4c69 6e65 2e69     - (macdLine.i
+0001b170: 6c6f 635b 3a32 5d2e 696c 6f63 5b31 5d20  loc[:2].iloc[1] 
+0001b180: 2d20 6d61 6364 5369 676e 616c 2e69 6c6f  - macdSignal.ilo
+0001b190: 635b 3a32 5d2e 696c 6f63 5b31 5d29 0d0a  c[:2].iloc[1])..
+0001b1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b1b0: 3e3d 2030 2e34 0d0a 2020 2020 2020 2020  >= 0.4..        
+0001b1c0: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+0001b1d0: 2020 2061 6e64 2028 0d0a 2020 2020 2020     and (..      
+0001b1e0: 2020 2020 2020 2020 2020 286d 6163 644c            (macdL
+0001b1f0: 696e 652e 696c 6f63 5b3a 325d 2e69 6c6f  ine.iloc[:2].ilo
+0001b200: 635b 315d 202d 206d 6163 6453 6967 6e61  c[1] - macdSigna
+0001b210: 6c2e 696c 6f63 5b3a 325d 2e69 6c6f 635b  l.iloc[:2].iloc[
+0001b220: 315d 290d 0a20 2020 2020 2020 2020 2020  1])..           
+0001b230: 2020 2020 202d 2028 6d61 6364 4c69 6e65       - (macdLine
+0001b240: 2e69 6c6f 635b 3a31 5d2e 696c 6f63 5b30  .iloc[:1].iloc[0
+0001b250: 5d20 2d20 6d61 6364 5369 676e 616c 2e69  ] - macdSignal.i
+0001b260: 6c6f 635b 3a31 5d2e 696c 6f63 5b30 5d29  loc[:1].iloc[0])
+0001b270: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001b280: 2020 3c3d 2030 2e32 0d0a 2020 2020 2020    <= 0.2..      
+0001b290: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+0001b2a0: 2020 2020 2061 6e64 2028 6d61 6364 4c69       and (macdLi
+0001b2b0: 6e65 2e69 6c6f 635b 3a33 5d2e 696c 6f63  ne.iloc[:3].iloc
+0001b2c0: 5b32 5d20 3e20 6d61 6364 5369 676e 616c  [2] > macdSignal
+0001b2d0: 2e69 6c6f 635b 3a33 5d2e 696c 6f63 5b32  .iloc[:3].iloc[2
+0001b2e0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+0001b2f0: 616e 6420 280d 0a20 2020 2020 2020 2020  and (..         
+0001b300: 2020 2020 2020 2028 6d61 6364 4c69 6e65         (macdLine
+0001b310: 2e69 6c6f 635b 3a33 5d2e 696c 6f63 5b32  .iloc[:3].iloc[2
+0001b320: 5d20 2d20 6d61 6364 5369 676e 616c 2e69  ] - macdSignal.i
+0001b330: 6c6f 635b 3a33 5d2e 696c 6f63 5b32 5d29  loc[:3].iloc[2])
+0001b340: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001b350: 2020 2d20 286d 6163 644c 696e 652e 696c    - (macdLine.il
+0001b360: 6f63 5b3a 325d 2e69 6c6f 635b 315d 202d  oc[:2].iloc[1] -
+0001b370: 206d 6163 6453 6967 6e61 6c2e 696c 6f63   macdSignal.iloc
+0001b380: 5b3a 325d 2e69 6c6f 635b 315d 290d 0a20  [:2].iloc[1]).. 
+0001b390: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0001b3a0: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
+0001b3b0: 290d 0a20 2020 2020 2020 2029 0d0a 0d0a  )..        )....
+0001b3c0: 2020 2020 2340 6d65 6173 7572 655f 7469      #@measure_ti
+0001b3d0: 6d65 0d0a 2020 2020 2320 7661 6c69 6461  me..    # valida
+0001b3e0: 7465 2069 6620 4343 4920 6973 2077 6974  te if CCI is wit
+0001b3f0: 6869 6e20 6769 7665 6e20 7261 6e67 650d  hin given range.
+0001b400: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+0001b410: 6543 4349 2873 656c 662c 2064 662c 2073  eCCI(self, df, s
+0001b420: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
+0001b430: 6963 742c 206d 696e 4343 492c 206d 6178  ict, minCCI, max
+0001b440: 4343 4929 3a0d 0a20 2020 2020 2020 2069  CCI):..        i
+0001b450: 6620 6466 2069 7320 4e6f 6e65 206f 7220  f df is None or 
+0001b460: 6c65 6e28 6466 2920 3d3d 2030 3a0d 0a20  len(df) == 0:.. 
+0001b470: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0001b480: 6e20 4661 6c73 650d 0a20 2020 2020 2020  n False..       
+0001b490: 2064 6174 6120 3d20 6466 2e63 6f70 7928   data = df.copy(
+0001b4a0: 290d 0a20 2020 2020 2020 2064 6174 6120  )..        data 
+0001b4b0: 3d20 6461 7461 2e66 696c 6c6e 6128 3029  = data.fillna(0)
+0001b4c0: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
+0001b4d0: 2064 6174 612e 7265 706c 6163 6528 5b6e   data.replace([n
+0001b4e0: 702e 696e 662c 202d 6e70 2e69 6e66 5d2c  p.inf, -np.inf],
+0001b4f0: 2030 290d 0a20 2020 2020 2020 2063 6369   0)..        cci
+0001b500: 203d 2069 6e74 2864 6174 612e 6865 6164   = int(data.head
+0001b510: 2831 295b 2243 4349 225d 2e69 6c6f 635b  (1)["CCI"].iloc[
+0001b520: 305d 290d 0a20 2020 2020 2020 2073 6176  0])..        sav
+0001b530: 6544 6963 745b 2243 4349 225d 203d 2063  eDict["CCI"] = c
+0001b540: 6369 0d0a 2020 2020 2020 2020 6966 2028  ci..        if (
+0001b550: 6363 6920 3e3d 206d 696e 4343 4920 616e  cci >= minCCI an
+0001b560: 6420 6363 6920 3c3d 206d 6178 4343 4929  d cci <= maxCCI)
+0001b570: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
+0001b580: 6620 2822 5570 2220 696e 2073 6176 6544  f ("Up" in saveD
+0001b590: 6963 745b 2254 7265 6e64 225d 293a 0d0a  ict["Trend"]):..
+0001b5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b5b0: 7363 7265 656e 4469 6374 5b22 4343 4922  screenDict["CCI"
+0001b5c0: 5d20 3d20 280d 0a20 2020 2020 2020 2020  ] = (..         
+0001b5d0: 2020 2020 2020 2020 2020 2028 636f 6c6f             (colo
+0001b5e0: 7254 6578 742e 424f 4c44 2069 6620 2822  rText.BOLD if ("
+0001b5f0: 5374 726f 6e67 2220 696e 2073 6176 6544  Strong" in saveD
+0001b600: 6963 745b 2254 7265 6e64 225d 2920 656c  ict["Trend"]) el
+0001b610: 7365 2022 2229 202b 2063 6f6c 6f72 5465  se "") + colorTe
+0001b620: 7874 2e47 5245 454e 202b 2073 7472 2863  xt.GREEN + str(c
+0001b630: 6369 2920 2b20 636f 6c6f 7254 6578 742e  ci) + colorText.
+0001b640: 454e 440d 0a20 2020 2020 2020 2020 2020  END..           
+0001b650: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+0001b660: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+0001b670: 2020 2020 2020 2020 2020 2073 6372 6565             scree
+0001b680: 6e44 6963 745b 2243 4349 225d 203d 2028  nDict["CCI"] = (
+0001b690: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001b6a0: 2020 2020 2020 2863 6f6c 6f72 5465 7874        (colorText
+0001b6b0: 2e42 4f4c 4420 6966 2028 2253 7472 6f6e  .BOLD if ("Stron
+0001b6c0: 6722 2069 6e20 7361 7665 4469 6374 5b22  g" in saveDict["
+0001b6d0: 5472 656e 6422 5d29 2065 6c73 6520 2222  Trend"]) else ""
+0001b6e0: 2920 2b20 636f 6c6f 7254 6578 742e 4641  ) + colorText.FA
+0001b6f0: 494c 202b 2073 7472 2863 6369 2920 2b20  IL + str(cci) + 
+0001b700: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
+0001b710: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0001b720: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+0001b730: 7475 726e 2054 7275 650d 0a20 2020 2020  turn True..     
+0001b740: 2020 2073 6372 6565 6e44 6963 745b 2243     screenDict["C
+0001b750: 4349 225d 203d 2063 6f6c 6f72 5465 7874  CI"] = colorText
+0001b760: 2e42 4f4c 4420 2b20 636f 6c6f 7254 6578  .BOLD + colorTex
+0001b770: 742e 4641 494c 202b 2073 7472 2863 6369  t.FAIL + str(cci
+0001b780: 2920 2b20 636f 6c6f 7254 6578 742e 454e  ) + colorText.EN
+0001b790: 440d 0a20 2020 2020 2020 2072 6574 7572  D..        retur
+0001b7a0: 6e20 4661 6c73 650d 0a0d 0a20 2020 2023  n False....    #
+0001b7b0: 2046 696e 6420 436f 6e66 6c75 6365 6e63   Find Conflucenc
+0001b7c0: 650d 0a20 2020 2064 6566 2076 616c 6964  e..    def valid
+0001b7d0: 6174 6543 6f6e 666c 7565 6e63 6528 7365  ateConfluence(se
+0001b7e0: 6c66 2c20 7374 6f63 6b2c 2064 662c 2073  lf, stock, df, s
+0001b7f0: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
+0001b800: 6963 742c 2070 6572 6365 6e74 6167 653d  ict, percentage=
+0001b810: 302e 312c 636f 6e66 4669 6c74 6572 3d33  0.1,confFilter=3
+0001b820: 293a 0d0a 2020 2020 2020 2020 6966 2064  ):..        if d
+0001b830: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
+0001b840: 2864 6629 203d 3d20 303a 0d0a 2020 2020  (df) == 0:..    
+0001b850: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+0001b860: 616c 7365 0d0a 2020 2020 2020 2020 6461  alse..        da
+0001b870: 7461 203d 2064 662e 636f 7079 2829 0d0a  ta = df.copy()..
+0001b880: 2020 2020 2020 2020 7265 6365 6e74 203d          recent =
+0001b890: 2064 6174 612e 6865 6164 2832 290d 0a20   data.head(2).. 
+0001b8a0: 2020 2020 2020 2069 6620 6c65 6e28 7265         if len(re
+0001b8b0: 6365 6e74 2920 3c20 323a 0d0a 2020 2020  cent) < 2:..    
+0001b8c0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+0001b8d0: 616c 7365 0d0a 2020 2020 2020 2020 6973  alse..        is
+0001b8e0: 3530 444d 4155 7054 7265 6e64 203d 2028  50DMAUpTrend = (
+0001b8f0: 7265 6365 6e74 5b22 534d 4122 5d2e 696c  recent["SMA"].il
+0001b900: 6f63 5b30 5d20 3e20 7265 6365 6e74 5b22  oc[0] > recent["
+0001b910: 534d 4122 5d2e 696c 6f63 5b31 5d29 0d0a  SMA"].iloc[1])..
+0001b920: 2020 2020 2020 2020 6973 3530 444d 4144          is50DMAD
+0001b930: 6f77 6e54 7265 6e64 203d 2028 7265 6365  ownTrend = (rece
+0001b940: 6e74 5b22 534d 4122 5d2e 696c 6f63 5b30  nt["SMA"].iloc[0
+0001b950: 5d20 3c20 7265 6365 6e74 5b22 534d 4122  ] < recent["SMA"
+0001b960: 5d2e 696c 6f63 5b31 5d29 0d0a 2020 2020  ].iloc[1])..    
+0001b970: 2020 2020 6973 476f 6c64 656e 4372 6f73      isGoldenCros
+0001b980: 734f 7665 7220 3d20 2872 6563 656e 745b  sOver = (recent[
+0001b990: 2253 4d41 225d 2e69 6c6f 635b 305d 203e  "SMA"].iloc[0] >
+0001b9a0: 3d20 7265 6365 6e74 5b22 4c4d 4122 5d2e  = recent["LMA"].
+0001b9b0: 696c 6f63 5b30 5d29 2061 6e64 205c 0d0a  iloc[0]) and \..
+0001b9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b9d0: 2020 2020 2020 2020 2020 2020 2872 6563              (rec
+0001b9e0: 656e 745b 2253 4d41 225d 2e69 6c6f 635b  ent["SMA"].iloc[
+0001b9f0: 315d 203c 3d20 7265 6365 6e74 5b22 4c4d  1] <= recent["LM
+0001ba00: 4122 5d2e 696c 6f63 5b31 5d29 0d0a 2020  A"].iloc[1])..  
+0001ba10: 2020 2020 2020 6973 4465 6164 4372 6f73        isDeadCros
+0001ba20: 734f 7665 7220 3d20 2872 6563 656e 745b  sOver = (recent[
+0001ba30: 2253 4d41 225d 2e69 6c6f 635b 305d 203c  "SMA"].iloc[0] <
+0001ba40: 3d20 7265 6365 6e74 5b22 4c4d 4122 5d2e  = recent["LMA"].
+0001ba50: 696c 6f63 5b30 5d29 2061 6e64 205c 0d0a  iloc[0]) and \..
+0001ba60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ba70: 2020 2020 2020 2020 2020 2020 2872 6563              (rec
+0001ba80: 656e 745b 2253 4d41 225d 2e69 6c6f 635b  ent["SMA"].iloc[
+0001ba90: 315d 203e 3d20 7265 6365 6e74 5b22 4c4d  1] >= recent["LM
+0001baa0: 4122 5d2e 696c 6f63 5b31 5d29 0d0a 2020  A"].iloc[1])..  
+0001bab0: 2020 2020 2020 6973 3530 444d 4120 3d20        is50DMA = 
+0001bac0: 2872 6563 656e 745b 2253 4d41 225d 2e69  (recent["SMA"].i
+0001bad0: 6c6f 635b 305d 203c 3d20 7265 6365 6e74  loc[0] <= recent
+0001bae0: 5b22 436c 6f73 6522 5d2e 696c 6f63 5b30  ["Close"].iloc[0
+0001baf0: 5d29 0d0a 2020 2020 2020 2020 6973 3230  ])..        is20
+0001bb00: 3044 4d41 203d 2028 7265 6365 6e74 5b22  0DMA = (recent["
+0001bb10: 4c4d 4122 5d2e 696c 6f63 5b30 5d20 3c3d  LMA"].iloc[0] <=
+0001bb20: 2072 6563 656e 745b 2243 6c6f 7365 225d   recent["Close"]
+0001bb30: 2e69 6c6f 635b 305d 290d 0a20 2020 2020  .iloc[0])..     
+0001bb40: 2020 2064 6966 6665 7265 6e63 6520 3d20     difference = 
+0001bb50: 726f 756e 6428 2872 6563 656e 745b 2253  round((recent["S
+0001bb60: 4d41 225d 2e69 6c6f 635b 305d 202d 2072  MA"].iloc[0] - r
+0001bb70: 6563 656e 745b 224c 4d41 225d 2e69 6c6f  ecent["LMA"].ilo
+0001bb80: 635b 305d 290d 0a20 2020 2020 2020 2020  c[0])..         
+0001bb90: 2020 2020 2020 202f 2072 6563 656e 745b         / recent[
+0001bba0: 2243 6c6f 7365 225d 2e69 6c6f 635b 305d  "Close"].iloc[0]
+0001bbb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001bbc0: 2020 2a20 3130 302c 0d0a 2020 2020 2020    * 100,..      
+0001bbd0: 2020 2020 2020 2020 2020 322c 0d0a 2020            2,..  
+0001bbe0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+0001bbf0: 2020 2020 2073 6176 6544 6963 745b 2243       saveDict["C
+0001bc00: 6f6e 6644 4d41 4469 6666 6572 656e 6365  onfDMADifference
+0001bc10: 225d 203d 2064 6966 6665 7265 6e63 650d  "] = difference.
+0001bc20: 0a20 2020 2020 2020 2073 6372 6565 6e44  .        screenD
+0001bc30: 6963 745b 2243 6f6e 6644 4d41 4469 6666  ict["ConfDMADiff
+0001bc40: 6572 656e 6365 225d 203d 2064 6966 6665  erence"] = diffe
+0001bc50: 7265 6e63 650d 0a20 2020 2020 2020 2073  rence..        s
+0001bc60: 6176 6564 203d 2073 656c 662e 6669 6e64  aved = self.find
+0001bc70: 4375 7272 656e 7453 6176 6564 5661 6c75  CurrentSavedValu
+0001bc80: 6528 7363 7265 656e 4469 6374 2c73 6176  e(screenDict,sav
+0001bc90: 6544 6963 742c 224d 412d 5369 676e 616c  eDict,"MA-Signal
+0001bca0: 2229 0d0a 2020 2020 2020 2020 2320 6469  ")..        # di
+0001bcb0: 6666 6572 656e 6365 203d 2061 6273 2864  fference = abs(d
+0001bcc0: 6966 6665 7265 6e63 6529 0d0a 2020 2020  ifference)..    
+0001bcd0: 2020 2020 636f 6e66 5465 7874 203d 2066      confText = f
+0001bce0: 227b 2747 6f6c 6465 6e43 726f 7373 6f76  "{'GoldenCrossov
+0001bcf0: 6572 2720 6966 2069 7347 6f6c 6465 6e43  er' if isGoldenC
+0001bd00: 726f 7373 4f76 6572 2065 6c73 6520 2827  rossOver else ('
+0001bd10: 4465 6164 4372 6f73 736f 7665 7227 2069  DeadCrossover' i
+0001bd20: 6620 6973 4465 6164 4372 6f73 734f 7665  f isDeadCrossOve
+0001bd30: 7220 656c 7365 2028 2743 6f6e 662e 5570  r else ('Conf.Up
+0001bd40: 2720 6966 2069 7335 3044 4d41 5570 5472  ' if is50DMAUpTr
+0001bd50: 656e 6420 656c 7365 2028 2743 6f6e 662e  end else ('Conf.
+0001bd60: 446f 776e 2720 6966 2069 7335 3044 4d41  Down' if is50DMA
+0001bd70: 446f 776e 5472 656e 6420 656c 7365 2028  DownTrend else (
+0001bd80: 2735 3044 4d41 2720 6966 2069 7335 3044  '50DMA' if is50D
+0001bd90: 4d41 2065 6c73 6520 2827 3230 3044 4d41  MA else ('200DMA
+0001bda0: 2720 6966 2069 7332 3030 444d 4120 656c  ' if is200DMA el
+0001bdb0: 7365 2027 556e 6b6e 6f77 6e27 2929 2929  se 'Unknown'))))
+0001bdc0: 297d 220d 0a20 2020 2020 2020 2069 6620  )}"..        if 
+0001bdd0: 6162 7328 7265 6365 6e74 5b22 534d 4122  abs(recent["SMA"
+0001bde0: 5d2e 696c 6f63 5b30 5d20 2d20 7265 6365  ].iloc[0] - rece
+0001bdf0: 6e74 5b22 4c4d 4122 5d2e 696c 6f63 5b30  nt["LMA"].iloc[0
+0001be00: 5d29 203c 3d20 280d 0a20 2020 2020 2020  ]) <= (..       
+0001be10: 2020 2020 2072 6563 656e 745b 2253 4d41       recent["SMA
+0001be20: 225d 2e69 6c6f 635b 305d 202a 2070 6572  "].iloc[0] * per
+0001be30: 6365 6e74 6167 650d 0a20 2020 2020 2020  centage..       
+0001be40: 2029 3a0d 0a20 2020 2020 2020 2020 2020   ):..           
+0001be50: 2069 6620 7265 6365 6e74 5b22 534d 4122   if recent["SMA"
+0001be60: 5d2e 696c 6f63 5b30 5d20 3e3d 2072 6563  ].iloc[0] >= rec
+0001be70: 656e 745b 224c 4d41 225d 2e69 6c6f 635b  ent["LMA"].iloc[
+0001be80: 305d 3a0d 0a20 2020 2020 2020 2020 2020  0]:..           
+0001be90: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+0001bea0: 224d 412d 5369 676e 616c 225d 203d 2028  "MA-Signal"] = (
+0001beb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001bec0: 2020 2020 2020 7361 7665 645b 305d 200d        saved[0] .
+0001bed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001bee0: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
+0001bef0: 2e42 4f4c 440d 0a20 2020 2020 2020 2020  .BOLD..         
+0001bf00: 2020 2020 2020 2020 2020 202b 2028 636f             + (co
+0001bf10: 6c6f 7254 6578 742e 4752 4545 4e20 6966  lorText.GREEN if
+0001bf20: 2069 7335 3044 4d41 5570 5472 656e 6420   is50DMAUpTrend 
+0001bf30: 656c 7365 2028 636f 6c6f 7254 6578 742e  else (colorText.
+0001bf40: 4641 494c 2069 6620 6973 3530 444d 4144  FAIL if is50DMAD
+0001bf50: 6f77 6e54 7265 6e64 2065 6c73 6520 636f  ownTrend else co
+0001bf60: 6c6f 7254 6578 742e 5741 524e 2929 0d0a  lorText.WARN))..
+0001bf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bf80: 2020 2020 2b20 6622 7b63 6f6e 6654 6578      + f"{confTex
+0001bf90: 747d 2028 7b64 6966 6665 7265 6e63 657d  t} ({difference}
+0001bfa0: 2529 220d 0a20 2020 2020 2020 2020 2020  %)"..           
+0001bfb0: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
+0001bfc0: 5465 7874 2e45 4e44 0d0a 2020 2020 2020  Text.END..      
+0001bfd0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+0001bfe0: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+0001bff0: 6544 6963 745b 224d 412d 5369 676e 616c  eDict["MA-Signal
+0001c000: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
+0001c010: 6622 7b63 6f6e 6654 6578 747d 2028 7b64  f"{confText} ({d
+0001c020: 6966 6665 7265 6e63 657d 2529 220d 0a20  ifference}%)".. 
+0001c030: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0001c040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001c050: 2020 7363 7265 656e 4469 6374 5b22 4d41    screenDict["MA
+0001c060: 2d53 6967 6e61 6c22 5d20 3d20 280d 0a20  -Signal"] = (.. 
+0001c070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c080: 2020 2073 6176 6564 5b30 5d20 0d0a 2020     saved[0] ..  
+0001c090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c0a0: 2020 2b20 636f 6c6f 7254 6578 742e 424f    + colorText.BO
+0001c0b0: 4c44 0d0a 2020 2020 2020 2020 2020 2020  LD..            
+0001c0c0: 2020 2020 2020 2020 2b20 2863 6f6c 6f72          + (color
+0001c0d0: 5465 7874 2e47 5245 454e 2069 6620 6973  Text.GREEN if is
+0001c0e0: 3530 444d 4155 7054 7265 6e64 2065 6c73  50DMAUpTrend els
+0001c0f0: 6520 2863 6f6c 6f72 5465 7874 2e46 4149  e (colorText.FAI
+0001c100: 4c20 6966 2069 7335 3044 4d41 446f 776e  L if is50DMADown
+0001c110: 5472 656e 6420 656c 7365 2063 6f6c 6f72  Trend else color
+0001c120: 5465 7874 2e57 4152 4e29 290d 0a20 2020  Text.WARN))..   
+0001c130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c140: 202b 2066 227b 636f 6e66 5465 7874 7d20   + f"{confText} 
+0001c150: 287b 6469 6666 6572 656e 6365 7d25 2922  ({difference}%)"
+0001c160: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001c170: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
+0001c180: 742e 454e 440d 0a20 2020 2020 2020 2020  t.END..         
+0001c190: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+0001c1a0: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
+0001c1b0: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
+0001c1c0: 3d20 7361 7665 645b 315d 202b 2066 227b  = saved[1] + f"{
+0001c1d0: 636f 6e66 5465 7874 7d20 287b 6469 6666  confText} ({diff
+0001c1e0: 6572 656e 6365 7d25 2922 0d0a 2020 2020  erence}%)"..    
+0001c1f0: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+0001c200: 6f6e 6646 696c 7465 7220 3d3d 2033 206f  onfFilter == 3 o
+0001c210: 7220 5c0d 0a20 2020 2020 2020 2020 2020  r \..           
+0001c220: 2020 2020 2028 636f 6e66 4669 6c74 6572       (confFilter
+0001c230: 203d 3d20 3120 616e 6420 2869 7335 3044   == 1 and (is50D
+0001c240: 4d41 5570 5472 656e 6420 6f72 2028 6973  MAUpTrend or (is
+0001c250: 476f 6c64 656e 4372 6f73 734f 7665 7220  GoldenCrossOver 
+0001c260: 6f72 2027 5570 2720 696e 2063 6f6e 6654  or 'Up' in confT
+0001c270: 6578 7429 2929 206f 7220 5c0d 0a20 2020  ext))) or \..   
+0001c280: 2020 2020 2020 2020 2020 2020 2028 636f               (co
+0001c290: 6e66 4669 6c74 6572 203d 3d20 3220 616e  nfFilter == 2 an
+0001c2a0: 6420 2869 7335 3044 4d41 446f 776e 5472  d (is50DMADownTr
+0001c2b0: 656e 6420 6f72 2069 7344 6561 6443 726f  end or isDeadCro
+0001c2c0: 7373 4f76 6572 206f 7220 2744 6f77 6e27  ssOver or 'Down'
+0001c2d0: 2069 6e20 636f 6e66 5465 7874 2929 0d0a   in confText))..
+0001c2e0: 2020 2020 2020 2020 2320 4d61 7962 6520          # Maybe 
+0001c2f0: 7468 6520 6469 6666 6572 656e 6365 2069  the difference i
+0001c300: 7320 6e6f 7420 7769 7468 696e 2074 6865  s not within the
+0001c310: 2072 616e 6765 2c20 6275 7420 7765 2764   range, but we'd
+0001c320: 2073 7469 6c6c 206c 696b 6520 746f 206b   still like to k
+0001c330: 6565 7020 7468 6520 7374 6f63 6b20 696e  eep the stock in
+0001c340: 0d0a 2020 2020 2020 2020 2320 7468 6520  ..        # the 
+0001c350: 6c69 7374 2069 6620 6974 2773 2061 2067  list if it's a g
+0001c360: 6f6c 6465 6e20 6372 6f73 736f 7665 7220  olden crossover 
+0001c370: 6f72 2064 6561 6420 6372 6f73 736f 7665  or dead crossove
+0001c380: 720d 0a20 2020 2020 2020 2069 6620 6973  r..        if is
+0001c390: 476f 6c64 656e 4372 6f73 734f 7665 7220  GoldenCrossOver 
+0001c3a0: 6f72 2069 7344 6561 6443 726f 7373 4f76  or isDeadCrossOv
+0001c3b0: 6572 3a0d 0a20 2020 2020 2020 2020 2020  er:..           
+0001c3c0: 2073 6372 6565 6e44 6963 745b 224d 412d   screenDict["MA-
+0001c3d0: 5369 676e 616c 225d 203d 2028 0d0a 2020  Signal"] = (..  
+0001c3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c3f0: 2020 7361 7665 645b 305d 200d 0a20 2020    saved[0] ..   
+0001c400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c410: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
+0001c420: 440d 0a20 2020 2020 2020 2020 2020 2020  D..             
+0001c430: 2020 2020 2020 202b 2028 636f 6c6f 7254         + (colorT
+0001c440: 6578 742e 4752 4545 4e20 6966 2069 7335  ext.GREEN if is5
+0001c450: 3044 4d41 5570 5472 656e 6420 656c 7365  0DMAUpTrend else
+0001c460: 2028 636f 6c6f 7254 6578 742e 4641 494c   (colorText.FAIL
+0001c470: 2069 6620 6973 3530 444d 4144 6f77 6e54   if is50DMADownT
+0001c480: 7265 6e64 2065 6c73 6520 636f 6c6f 7254  rend else colorT
+0001c490: 6578 742e 5741 524e 2929 0d0a 2020 2020  ext.WARN))..    
+0001c4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c4b0: 2b20 6622 7b63 6f6e 6654 6578 747d 2028  + f"{confText} (
+0001c4c0: 7b64 6966 6665 7265 6e63 657d 2529 220d  {difference}%)".
+0001c4d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c4e0: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
+0001c4f0: 2e45 4e44 0d0a 2020 2020 2020 2020 2020  .END..          
+0001c500: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+0001c510: 2020 2020 2073 6176 6544 6963 745b 224d       saveDict["M
+0001c520: 412d 5369 676e 616c 225d 203d 2073 6176  A-Signal"] = sav
+0001c530: 6564 5b31 5d20 2b20 6622 7b63 6f6e 6654  ed[1] + f"{confT
+0001c540: 6578 747d 2028 7b64 6966 6665 7265 6e63  ext} ({differenc
+0001c550: 657d 2529 220d 0a20 2020 2020 2020 2020  e}%)"..         
+0001c560: 2020 2072 6574 7572 6e20 636f 6e66 4669     return confFi
+0001c570: 6c74 6572 203d 3d20 3320 6f72 205c 0d0a  lter == 3 or \..
+0001c580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c590: 2863 6f6e 6646 696c 7465 7220 3d3d 2031  (confFilter == 1
+0001c5a0: 2061 6e64 2069 7347 6f6c 6465 6e43 726f   and isGoldenCro
+0001c5b0: 7373 4f76 6572 2920 6f72 205c 0d0a 2020  ssOver) or \..  
+0001c5c0: 2020 2020 2020 2020 2020 2020 2020 2863                (c
+0001c5d0: 6f6e 6646 696c 7465 7220 3d3d 2032 2061  onfFilter == 2 a
+0001c5e0: 6e64 2069 7344 6561 6443 726f 7373 4f76  nd isDeadCrossOv
+0001c5f0: 6572 290d 0a20 2020 2020 2020 2072 6574  er)..        ret
+0001c600: 7572 6e20 4661 6c73 650d 0a0d 0a20 2020  urn False....   
+0001c610: 2023 406d 6561 7375 7265 5f74 696d 650d   #@measure_time.
+0001c620: 0a20 2020 2023 2056 616c 6964 6174 6520  .    # Validate 
+0001c630: 6966 2073 6861 7265 2070 7269 6365 7320  if share prices 
+0001c640: 6172 6520 636f 6e73 6f6c 6964 6174 696e  are consolidatin
+0001c650: 670d 0a20 2020 2064 6566 2076 616c 6964  g..    def valid
+0001c660: 6174 6543 6f6e 736f 6c69 6461 7469 6f6e  ateConsolidation
+0001c670: 2873 656c 662c 2064 662c 2073 6372 6565  (self, df, scree
+0001c680: 6e44 6963 742c 2073 6176 6544 6963 742c  nDict, saveDict,
+0001c690: 2070 6572 6365 6e74 6167 653d 3130 293a   percentage=10):
+0001c6a0: 0d0a 2020 2020 2020 2020 6966 2064 6620  ..        if df 
+0001c6b0: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
+0001c6c0: 6629 203d 3d20 303a 0d0a 2020 2020 2020  f) == 0:..      
+0001c6d0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+0001c6e0: 7365 0d0a 2020 2020 2020 2020 6461 7461  se..        data
+0001c6f0: 203d 2064 662e 636f 7079 2829 0d0a 2020   = df.copy()..  
+0001c700: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
+0001c710: 612e 6669 6c6c 6e61 2830 290d 0a20 2020  a.fillna(0)..   
+0001c720: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+0001c730: 2e72 6570 6c61 6365 285b 6e70 2e69 6e66  .replace([np.inf
+0001c740: 2c20 2d6e 702e 696e 665d 2c20 3029 0d0a  , -np.inf], 0)..
+0001c750: 2020 2020 2020 2020 6863 203d 2064 6174          hc = dat
+0001c760: 612e 6465 7363 7269 6265 2829 5b22 436c  a.describe()["Cl
+0001c770: 6f73 6522 5d5b 226d 6178 225d 0d0a 2020  ose"]["max"]..  
+0001c780: 2020 2020 2020 6c63 203d 2064 6174 612e        lc = data.
+0001c790: 6465 7363 7269 6265 2829 5b22 436c 6f73  describe()["Clos
+0001c7a0: 6522 5d5b 226d 696e 225d 0d0a 2020 2020  e"]["min"]..    
+0001c7b0: 2020 2020 6966 2028 6863 202d 206c 6329      if (hc - lc)
+0001c7c0: 203c 3d20 2868 6320 2a20 7065 7263 656e   <= (hc * percen
+0001c7d0: 7461 6765 202f 2031 3030 2920 616e 6420  tage / 100) and 
+0001c7e0: 2868 6320 2d20 6c63 2021 3d20 3029 3a0d  (hc - lc != 0):.
+0001c7f0: 0a20 2020 2020 2020 2020 2020 2073 6372  .            scr
+0001c800: 6565 6e44 6963 745b 2243 6f6e 736f 6c2e  eenDict["Consol.
+0001c810: 225d 203d 2028 0d0a 2020 2020 2020 2020  "] = (..        
+0001c820: 2020 2020 2020 2020 636f 6c6f 7254 6578          colorTex
+0001c830: 742e 424f 4c44 0d0a 2020 2020 2020 2020  t.BOLD..        
+0001c840: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
+0001c850: 6578 742e 4752 4545 4e0d 0a20 2020 2020  ext.GREEN..     
+0001c860: 2020 2020 2020 2020 2020 202b 2022 5261             + "Ra
+0001c870: 6e67 653a 220d 0a20 2020 2020 2020 2020  nge:"..         
+0001c880: 2020 2020 2020 202b 2073 7472 2872 6f75         + str(rou
+0001c890: 6e64 2828 6162 7328 2868 6320 2d20 6c63  nd((abs((hc - lc
+0001c8a0: 2920 2f20 6863 2920 2a20 3130 3029 2c20  ) / hc) * 100), 
+0001c8b0: 3129 290d 0a20 2020 2020 2020 2020 2020  1))..           
+0001c8c0: 2020 2020 202b 2022 2522 0d0a 2020 2020       + "%"..    
+0001c8d0: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
+0001c8e0: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
+0001c8f0: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
+0001c900: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+0001c910: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+0001c920: 745b 2243 6f6e 736f 6c2e 225d 203d 2028  t["Consol."] = (
+0001c930: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001c940: 2020 636f 6c6f 7254 6578 742e 424f 4c44    colorText.BOLD
+0001c950: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001c960: 2020 2b20 636f 6c6f 7254 6578 742e 4641    + colorText.FA
+0001c970: 494c 0d0a 2020 2020 2020 2020 2020 2020  IL..            
+0001c980: 2020 2020 2b20 2252 616e 6765 3a22 0d0a      + "Range:"..
+0001c990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c9a0: 2b20 7374 7228 726f 756e 6428 2861 6273  + str(round((abs
+0001c9b0: 2828 6863 202d 206c 6329 202f 2068 6329  ((hc - lc) / hc)
+0001c9c0: 202a 2031 3030 292c 2031 2929 0d0a 2020   * 100), 1))..  
+0001c9d0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+0001c9e0: 2225 220d 0a20 2020 2020 2020 2020 2020  "%"..           
+0001c9f0: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
+0001ca00: 2e45 4e44 0d0a 2020 2020 2020 2020 2020  .END..          
+0001ca10: 2020 290d 0a20 2020 2020 2020 2073 6176    )..        sav
+0001ca20: 6544 6963 745b 2243 6f6e 736f 6c2e 225d  eDict["Consol."]
+0001ca30: 203d 2066 2752 616e 6765 3a7b 7374 7228   = f'Range:{str(
+0001ca40: 726f 756e 6428 2861 6273 2828 6863 2d6c  round((abs((hc-l
+0001ca50: 6329 2f68 6329 2a31 3030 292c 3129 292b  c)/hc)*100),1))+
+0001ca60: 2225 227d 270d 0a20 2020 2020 2020 2072  "%"}'..        r
+0001ca70: 6574 7572 6e20 726f 756e 6428 2861 6273  eturn round((abs
+0001ca80: 2828 6863 202d 206c 6329 202f 2068 6329  ((hc - lc) / hc)
+0001ca90: 202a 2031 3030 292c 2031 290d 0a0d 0a20   * 100), 1).... 
+0001caa0: 2020 2023 2076 616c 6964 6174 6520 6966     # validate if
+0001cab0: 2074 6865 2073 746f 636b 2068 6173 2062   the stock has b
+0001cac0: 6565 6e20 6861 7669 6e67 2068 6967 6865  een having highe
+0001cad0: 7220 6869 6768 732c 2068 6967 6865 7220  r highs, higher 
+0001cae0: 6c6f 7773 0d0a 2020 2020 2320 616e 6420  lows..    # and 
+0001caf0: 6869 6768 6572 2063 6c6f 7365 2077 6974  higher close wit
+0001cb00: 6820 6c61 7465 7374 2063 6c6f 7365 203e  h latest close >
+0001cb10: 2073 7570 6572 7472 656e 6420 616e 6420   supertrend and 
+0001cb20: 382d 454d 412e 0d0a 2020 2020 6465 6620  8-EMA...    def 
+0001cb30: 7661 6c69 6461 7465 4869 6768 6572 4869  validateHigherHi
+0001cb40: 6768 7348 6967 6865 724c 6f77 7348 6967  ghsHigherLowsHig
+0001cb50: 6865 7243 6c6f 7365 2873 656c 662c 2064  herClose(self, d
+0001cb60: 6629 3a0d 0a20 2020 2020 2020 2069 6620  f):..        if 
+0001cb70: 6466 2069 7320 4e6f 6e65 206f 7220 6c65  df is None or le
+0001cb80: 6e28 6466 2920 3d3d 2030 3a0d 0a20 2020  n(df) == 0:..   
+0001cb90: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0001cba0: 4661 6c73 650d 0a20 2020 2020 2020 2064  False..        d
+0001cbb0: 6174 6120 3d20 6466 2e63 6f70 7928 290d  ata = df.copy().
+0001cbc0: 0a20 2020 2020 2020 2064 6179 3020 3d20  .        day0 = 
+0001cbd0: 6461 7461 0d0a 2020 2020 2020 2020 6461  data..        da
+0001cbe0: 7931 203d 2064 6174 615b 313a 5d0d 0a20  y1 = data[1:].. 
+0001cbf0: 2020 2020 2020 2064 6179 3220 3d20 6461         day2 = da
+0001cc00: 7461 5b32 3a5d 0d0a 2020 2020 2020 2020  ta[2:]..        
+0001cc10: 6461 7933 203d 2064 6174 615b 333a 5d0d  day3 = data[3:].
+0001cc20: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+0001cc30: 6461 7931 2920 3c20 3120 6f72 206c 656e  day1) < 1 or len
+0001cc40: 2864 6179 3229 203c 2031 206f 7220 6c65  (day2) < 1 or le
+0001cc50: 6e28 6461 7933 2920 3c20 313a 0d0a 2020  n(day3) < 1:..  
+0001cc60: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0001cc70: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+0001cc80: 6869 6768 6572 4869 6768 7320 3d20 280d  higherHighs = (.
+0001cc90: 0a20 2020 2020 2020 2020 2020 2028 6461  .            (da
+0001cca0: 7930 5b22 4869 6768 225d 2e69 6c6f 635b  y0["High"].iloc[
+0001ccb0: 305d 203e 2064 6179 315b 2248 6967 6822  0] > day1["High"
+0001ccc0: 5d2e 696c 6f63 5b30 5d29 0d0a 2020 2020  ].iloc[0])..    
+0001ccd0: 2020 2020 2020 2020 616e 6420 2864 6179          and (day
+0001cce0: 315b 2248 6967 6822 5d2e 696c 6f63 5b30  1["High"].iloc[0
+0001ccf0: 5d20 3e20 6461 7932 5b22 4869 6768 225d  ] > day2["High"]
+0001cd00: 2e69 6c6f 635b 305d 290d 0a20 2020 2020  .iloc[0])..     
+0001cd10: 2020 2020 2020 2061 6e64 2028 6461 7932         and (day2
+0001cd20: 5b22 4869 6768 225d 2e69 6c6f 635b 305d  ["High"].iloc[0]
+0001cd30: 203e 2064 6179 335b 2248 6967 6822 5d2e   > day3["High"].
+0001cd40: 696c 6f63 5b30 5d29 0d0a 2020 2020 2020  iloc[0])..      
+0001cd50: 2020 290d 0a20 2020 2020 2020 2068 6967    )..        hig
+0001cd60: 6865 724c 6f77 7320 3d20 280d 0a20 2020  herLows = (..   
+0001cd70: 2020 2020 2020 2020 2028 6461 7930 5b22           (day0["
+0001cd80: 4c6f 7722 5d2e 696c 6f63 5b30 5d20 3e20  Low"].iloc[0] > 
+0001cd90: 6461 7931 5b22 4c6f 7722 5d2e 696c 6f63  day1["Low"].iloc
+0001cda0: 5b30 5d29 0d0a 2020 2020 2020 2020 2020  [0])..          
+0001cdb0: 2020 616e 6420 2864 6179 315b 224c 6f77    and (day1["Low
+0001cdc0: 225d 2e69 6c6f 635b 305d 203e 2064 6179  "].iloc[0] > day
+0001cdd0: 325b 224c 6f77 225d 2e69 6c6f 635b 305d  2["Low"].iloc[0]
+0001cde0: 290d 0a20 2020 2020 2020 2020 2020 2061  )..            a
+0001cdf0: 6e64 2028 6461 7932 5b22 4c6f 7722 5d2e  nd (day2["Low"].
+0001ce00: 696c 6f63 5b30 5d20 3e20 6461 7933 5b22  iloc[0] > day3["
+0001ce10: 4c6f 7722 5d2e 696c 6f63 5b30 5d29 0d0a  Low"].iloc[0])..
+0001ce20: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+0001ce30: 2020 2068 6967 6865 7243 6c6f 7365 203d     higherClose =
+0001ce40: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+0001ce50: 2864 6179 305b 2243 6c6f 7365 225d 2e69  (day0["Close"].i
+0001ce60: 6c6f 635b 305d 203e 2064 6179 315b 2243  loc[0] > day1["C
+0001ce70: 6c6f 7365 225d 2e69 6c6f 635b 305d 290d  lose"].iloc[0]).
+0001ce80: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
+0001ce90: 2028 6461 7931 5b22 436c 6f73 6522 5d2e   (day1["Close"].
+0001cea0: 696c 6f63 5b30 5d20 3e20 6461 7932 5b22  iloc[0] > day2["
+0001ceb0: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d29  Close"].iloc[0])
+0001cec0: 0d0a 2020 2020 2020 2020 2020 2020 616e  ..            an
+0001ced0: 6420 2864 6179 325b 2243 6c6f 7365 225d  d (day2["Close"]
+0001cee0: 2e69 6c6f 635b 305d 203e 2064 6179 335b  .iloc[0] > day3[
+0001cef0: 2243 6c6f 7365 225d 2e69 6c6f 635b 305d  "Close"].iloc[0]
+0001cf00: 290d 0a20 2020 2020 2020 2029 0d0a 2020  )..        )..  
+0001cf10: 2020 2020 2020 2320 6869 6768 6572 5253        # higherRS
+0001cf20: 4920 3d20 2864 6179 305b 2252 5349 225d  I = (day0["RSI"]
+0001cf30: 2e69 6c6f 635b 305d 203e 2064 6179 315b  .iloc[0] > day1[
+0001cf40: 2252 5349 225d 2e69 6c6f 635b 305d 2920  "RSI"].iloc[0]) 
+0001cf50: 616e 6420 5c0d 0a20 2020 2020 2020 2023  and \..        #
+0001cf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cf70: 2028 6461 7931 5b22 5253 4922 5d2e 696c   (day1["RSI"].il
+0001cf80: 6f63 5b30 5d20 3e20 6461 7932 5b22 5253  oc[0] > day2["RS
+0001cf90: 4922 5d2e 696c 6f63 5b30 5d29 2061 6e64  I"].iloc[0]) and
+0001cfa0: 205c 0d0a 2020 2020 2020 2020 2320 2020   \..        #   
+0001cfb0: 2020 2020 2020 2020 2020 2020 2020 2864                (d
+0001cfc0: 6179 325b 2252 5349 225d 2e69 6c6f 635b  ay2["RSI"].iloc[
+0001cfd0: 305d 203e 2064 6179 335b 2252 5349 225d  0] > day3["RSI"]
+0001cfe0: 2e69 6c6f 635b 305d 2920 616e 6420 5c0d  .iloc[0]) and \.
+0001cff0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0001d000: 2020 2020 2020 2020 2020 2064 6179 335b             day3[
+0001d010: 2252 5349 225d 2e69 6c6f 635b 305d 203e  "RSI"].iloc[0] >
+0001d020: 3d20 3530 2061 6e64 2064 6179 305b 2252  = 50 and day0["R
+0001d030: 5349 225d 2e69 6c6f 635b 305d 203e 3d20  SI"].iloc[0] >= 
+0001d040: 3635 0d0a 2020 2020 2020 2020 7265 7665  65..        reve
+0001d050: 7273 6564 4461 7461 203d 2064 6174 615b  rsedData = data[
+0001d060: 3a3a 2d31 5d2e 636f 7079 2829 0d0a 2020  ::-1].copy()..  
+0001d070: 2020 2020 2020 7265 7665 7273 6564 4461        reversedDa
+0001d080: 7461 5b22 5355 5045 5254 225d 203d 2070  ta["SUPERT"] = p
+0001d090: 6b74 616c 6962 2e73 7570 6572 7472 656e  ktalib.supertren
+0001d0a0: 6428 7265 7665 7273 6564 4461 7461 2c20  d(reversedData, 
+0001d0b0: 372c 2033 295b 2253 5550 4552 545f 375f  7, 3)["SUPERT_7_
+0001d0c0: 332e 3022 5d0d 0a20 2020 2020 2020 2072  3.0"]..        r
+0001d0d0: 6576 6572 7365 6444 6174 615b 2245 4d41  eversedData["EMA
+0001d0e0: 3822 5d20 3d20 706b 7461 6c69 622e 454d  8"] = pktalib.EM
+0001d0f0: 4128 7265 7665 7273 6564 4461 7461 5b22  A(reversedData["
+0001d100: 436c 6f73 6522 5d2c 2074 696d 6570 6572  Close"], timeper
+0001d110: 696f 643d 3929 0d0a 2020 2020 2020 2020  iod=9)..        
+0001d120: 6869 6768 6572 436c 6f73 6520 3d20 280d  higherClose = (.
+0001d130: 0a20 2020 2020 2020 2020 2020 2068 6967  .            hig
+0001d140: 6865 7243 6c6f 7365 0d0a 2020 2020 2020  herClose..      
+0001d150: 2020 2020 2020 616e 6420 6461 7930 5b22        and day0["
+0001d160: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d20  Close"].iloc[0] 
+0001d170: 3e20 7265 7665 7273 6564 4461 7461 2e74  > reversedData.t
+0001d180: 6169 6c28 3129 5b22 5355 5045 5254 225d  ail(1)["SUPERT"]
+0001d190: 2e69 6c6f 635b 305d 0d0a 2020 2020 2020  .iloc[0]..      
+0001d1a0: 2020 2020 2020 616e 6420 6461 7930 5b22        and day0["
+0001d1b0: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d20  Close"].iloc[0] 
+0001d1c0: 3e20 7265 7665 7273 6564 4461 7461 2e74  > reversedData.t
+0001d1d0: 6169 6c28 3129 5b22 454d 4138 225d 2e69  ail(1)["EMA8"].i
+0001d1e0: 6c6f 635b 305d 0d0a 2020 2020 2020 2020  loc[0]..        
+0001d1f0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+0001d200: 6e20 6869 6768 6572 4869 6768 7320 616e  n higherHighs an
+0001d210: 6420 6869 6768 6572 4c6f 7773 2061 6e64  d higherLows and
+0001d220: 2068 6967 6865 7243 6c6f 7365 0d0a 0d0a   higherClose....
+0001d230: 2020 2020 2340 6d65 6173 7572 655f 7469      #@measure_ti
+0001d240: 6d65 0d0a 2020 2020 2320 5661 6c69 6461  me..    # Valida
+0001d250: 7465 2027 496e 7369 6465 2042 6172 2720  te 'Inside Bar' 
+0001d260: 7374 7275 6374 7572 6520 666f 7220 7265  structure for re
+0001d270: 6365 6e74 2064 6179 730d 0a20 2020 2064  cent days..    d
+0001d280: 6566 2076 616c 6964 6174 6549 6e73 6964  ef validateInsid
+0001d290: 6542 6172 280d 0a20 2020 2020 2020 2073  eBar(..        s
+0001d2a0: 656c 662c 2064 662c 2073 6372 6565 6e44  elf, df, screenD
+0001d2b0: 6963 742c 2073 6176 6544 6963 742c 2063  ict, saveDict, c
+0001d2c0: 6861 7274 5061 7474 6572 6e3d 312c 2064  hartPattern=1, d
+0001d2d0: 6179 7354 6f4c 6f6f 6b62 6163 6b3d 350d  aysToLookback=5.
+0001d2e0: 0a20 2020 2029 3a0d 0a20 2020 2020 2020  .    ):..       
+0001d2f0: 2069 6620 6466 2069 7320 4e6f 6e65 206f   if df is None o
+0001d300: 7220 6c65 6e28 6466 2920 3d3d 2030 3a0d  r len(df) == 0:.
+0001d310: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0001d320: 7572 6e20 4661 6c73 650d 0a20 2020 2020  urn False..     
+0001d330: 2020 2064 6174 6120 3d20 6466 2e63 6f70     data = df.cop
+0001d340: 7928 290d 0a20 2020 2020 2020 206f 7267  y()..        org
+0001d350: 4461 7461 203d 2064 6174 610d 0a20 2020  Data = data..   
+0001d360: 2020 2020 2073 6176 6564 203d 2073 656c       saved = sel
+0001d370: 662e 6669 6e64 4375 7272 656e 7453 6176  f.findCurrentSav
+0001d380: 6564 5661 6c75 6528 7363 7265 656e 4469  edValue(screenDi
+0001d390: 6374 2c20 7361 7665 4469 6374 2c20 2250  ct, saveDict, "P
+0001d3a0: 6174 7465 726e 2229 0d0a 2020 2020 2020  attern")..      
+0001d3b0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+0001d3c0: 2869 6e74 2864 6179 7354 6f4c 6f6f 6b62  (int(daysToLookb
+0001d3d0: 6163 6b29 2c20 696e 7428 726f 756e 6428  ack), int(round(
+0001d3e0: 6461 7973 546f 4c6f 6f6b 6261 636b 202a  daysToLookback *
+0001d3f0: 2030 2e35 2929 202d 2031 2c20 2d31 293a   0.5)) - 1, -1):
+0001d400: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0001d410: 2069 203d 3d20 323a 0d0a 2020 2020 2020   i == 2:..      
+0001d420: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0001d430: 2030 2020 2320 4578 6974 2069 6620 6f6e   0  # Exit if on
+0001d440: 6c79 206c 6173 7420 3220 6361 6e64 6c65  ly last 2 candle
+0001d450: 7320 6172 6520 6c65 6674 0d0a 2020 2020  s are left..    
+0001d460: 2020 2020 2020 2020 6966 2063 6861 7274          if chart
+0001d470: 5061 7474 6572 6e20 3d3d 2031 3a0d 0a20  Pattern == 1:.. 
+0001d480: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001d490: 6620 2255 7022 2069 6e20 7361 7665 4469  f "Up" in saveDi
+0001d4a0: 6374 5b22 5472 656e 6422 5d20 616e 6420  ct["Trend"] and 
+0001d4b0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+0001d4c0: 2020 2020 2020 2022 4275 6c6c 2220 696e         "Bull" in
+0001d4d0: 2073 6176 6544 6963 745b 224d 412d 5369   saveDict["MA-Si
+0001d4e0: 676e 616c 225d 0d0a 2020 2020 2020 2020  gnal"]..        
+0001d4f0: 2020 2020 2020 2020 2020 2020 6f72 2022              or "
+0001d500: 5375 7070 6f72 7422 2069 6e20 7361 7665  Support" in save
+0001d510: 4469 6374 5b22 4d41 2d53 6967 6e61 6c22  Dict["MA-Signal"
+0001d520: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+0001d530: 2020 2029 3a0d 0a20 2020 2020 2020 2020     ):..         
+0001d540: 2020 2020 2020 2020 2020 2064 6174 6120             data 
+0001d550: 3d20 6f72 6744 6174 612e 6865 6164 2869  = orgData.head(i
+0001d560: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001d570: 2020 2020 2020 2072 6566 4361 6e64 6c65         refCandle
+0001d580: 203d 2064 6174 612e 7461 696c 2831 290d   = data.tail(1).
+0001d590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d5a0: 2020 2020 2069 6620 280d 0a20 2020 2020       if (..     
+0001d5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d5c0: 2020 2028 6c65 6e28 6461 7461 2e48 6967     (len(data.Hig
+0001d5d0: 685b 6461 7461 2e48 6967 6820 3e20 7265  h[data.High > re
+0001d5e0: 6643 616e 646c 652e 4869 6768 2e69 7465  fCandle.High.ite
+0001d5f0: 6d28 295d 2920 3d3d 2030 290d 0a20 2020  m()]) == 0)..   
+0001d600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d610: 2020 2020 2061 6e64 2028 6c65 6e28 6461       and (len(da
+0001d620: 7461 2e4c 6f77 5b64 6174 612e 4c6f 7720  ta.Low[data.Low 
+0001d630: 3c20 7265 6643 616e 646c 652e 4c6f 772e  < refCandle.Low.
+0001d640: 6974 656d 2829 5d29 203d 3d20 3029 0d0a  item()]) == 0)..
+0001d650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d660: 2020 2020 2020 2020 616e 6420 286c 656e          and (len
+0001d670: 2864 6174 612e 4f70 656e 5b64 6174 612e  (data.Open[data.
+0001d680: 4f70 656e 203e 2072 6566 4361 6e64 6c65  Open > refCandle
+0001d690: 2e48 6967 682e 6974 656d 2829 5d29 203d  .High.item()]) =
+0001d6a0: 3d20 3029 0d0a 2020 2020 2020 2020 2020  = 0)..          
+0001d6b0: 2020 2020 2020 2020 2020 2020 2020 616e                an
+0001d6c0: 6420 286c 656e 2864 6174 612e 436c 6f73  d (len(data.Clos
+0001d6d0: 655b 6461 7461 2e43 6c6f 7365 203c 2072  e[data.Close < r
+0001d6e0: 6566 4361 6e64 6c65 2e4c 6f77 2e69 7465  efCandle.Low.ite
+0001d6f0: 6d28 295d 2920 3d3d 2030 290d 0a20 2020  m()]) == 0)..   
+0001d700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d710: 2029 3a0d 0a20 2020 2020 2020 2020 2020   ):..           
+0001d720: 2020 2020 2020 2020 2020 2020 2073 6372               scr
+0001d730: 6565 6e44 6963 745b 2250 6174 7465 726e  eenDict["Pattern
+0001d740: 225d 203d 2028 0d0a 2020 2020 2020 2020  "] = (..        
+0001d750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d760: 2020 2020 7361 7665 645b 305d 0d0a 2020      saved[0]..  
+0001d770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d780: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
+0001d790: 7254 6578 742e 424f 4c44 0d0a 2020 2020  rText.BOLD..    
+0001d7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d7b0: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
+0001d7c0: 6578 742e 5741 524e 0d0a 2020 2020 2020  ext.WARN..      
+0001d7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d7e0: 2020 2020 2020 2b20 2822 496e 7369 6465        + ("Inside
+0001d7f0: 2042 6172 2028 2564 2922 2025 2069 290d   Bar (%d)" % i).
+0001d800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d810: 2020 2020 2020 2020 2020 2020 202b 2063               + c
+0001d820: 6f6c 6f72 5465 7874 2e45 4e44 0d0a 2020  olorText.END..  
+0001d830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d840: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+0001d850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d860: 2073 6176 6544 6963 745b 2250 6174 7465   saveDict["Patte
+0001d870: 726e 225d 203d 2073 6176 6564 5b31 5d20  rn"] = saved[1] 
+0001d880: 2b20 2249 6e73 6964 6520 4261 7220 2825  + "Inside Bar (%
+0001d890: 6429 2220 2520 690d 0a20 2020 2020 2020  d)" % i..       
+0001d8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d8b0: 2072 6574 7572 6e20 690d 0a20 2020 2020   return i..     
+0001d8c0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0001d8d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001d8e0: 2020 2020 2020 7265 7475 726e 2030 0d0a        return 0..
+0001d8f0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0001d900: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001d910: 2020 2069 6620 2244 6f77 6e22 2069 6e20     if "Down" in 
+0001d920: 7361 7665 4469 6374 5b22 5472 656e 6422  saveDict["Trend"
+0001d930: 5d20 616e 6420 280d 0a20 2020 2020 2020  ] and (..       
+0001d940: 2020 2020 2020 2020 2020 2020 2022 4265               "Be
+0001d950: 6172 2220 696e 2073 6176 6544 6963 745b  ar" in saveDict[
+0001d960: 224d 412d 5369 676e 616c 225d 206f 7220  "MA-Signal"] or 
+0001d970: 2252 6573 6973 7422 2069 6e20 7361 7665  "Resist" in save
+0001d980: 4469 6374 5b22 4d41 2d53 6967 6e61 6c22  Dict["MA-Signal"
+0001d990: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+0001d9a0: 2020 2029 3a0d 0a20 2020 2020 2020 2020     ):..         
+0001d9b0: 2020 2020 2020 2020 2020 2064 6174 6120             data 
+0001d9c0: 3d20 6f72 6744 6174 612e 6865 6164 2869  = orgData.head(i
+0001d9d0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001d9e0: 2020 2020 2020 2072 6566 4361 6e64 6c65         refCandle
+0001d9f0: 203d 2064 6174 612e 7461 696c 2831 290d   = data.tail(1).
+0001da00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001da10: 2020 2020 2069 6620 280d 0a20 2020 2020       if (..     
+0001da20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001da30: 2020 2028 6c65 6e28 6461 7461 2e48 6967     (len(data.Hig
+0001da40: 685b 6461 7461 2e48 6967 6820 3e20 7265  h[data.High > re
+0001da50: 6643 616e 646c 652e 4869 6768 2e69 7465  fCandle.High.ite
+0001da60: 6d28 295d 2920 3d3d 2030 290d 0a20 2020  m()]) == 0)..   
+0001da70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001da80: 2020 2020 2061 6e64 2028 6c65 6e28 6461       and (len(da
+0001da90: 7461 2e4c 6f77 5b64 6174 612e 4c6f 7720  ta.Low[data.Low 
+0001daa0: 3c20 7265 6643 616e 646c 652e 4c6f 772e  < refCandle.Low.
+0001dab0: 6974 656d 2829 5d29 203d 3d20 3029 0d0a  item()]) == 0)..
+0001dac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dad0: 2020 2020 2020 2020 616e 6420 286c 656e          and (len
+0001dae0: 2864 6174 612e 4f70 656e 5b64 6174 612e  (data.Open[data.
+0001daf0: 4f70 656e 203e 2072 6566 4361 6e64 6c65  Open > refCandle
+0001db00: 2e48 6967 682e 6974 656d 2829 5d29 203d  .High.item()]) =
+0001db10: 3d20 3029 0d0a 2020 2020 2020 2020 2020  = 0)..          
+0001db20: 2020 2020 2020 2020 2020 2020 2020 616e                an
+0001db30: 6420 286c 656e 2864 6174 612e 436c 6f73  d (len(data.Clos
+0001db40: 655b 6461 7461 2e43 6c6f 7365 203c 2072  e[data.Close < r
+0001db50: 6566 4361 6e64 6c65 2e4c 6f77 2e69 7465  efCandle.Low.ite
+0001db60: 6d28 295d 2920 3d3d 2030 290d 0a20 2020  m()]) == 0)..   
+0001db70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db80: 2029 3a0d 0a20 2020 2020 2020 2020 2020   ):..           
+0001db90: 2020 2020 2020 2020 2020 2020 2073 6372               scr
+0001dba0: 6565 6e44 6963 745b 2250 6174 7465 726e  eenDict["Pattern
+0001dbb0: 225d 203d 2028 0d0a 2020 2020 2020 2020  "] = (..        
+0001dbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dbd0: 2020 2020 7361 7665 645b 305d 0d0a 2020      saved[0]..  
+0001dbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dbf0: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
+0001dc00: 7254 6578 742e 424f 4c44 0d0a 2020 2020  rText.BOLD..    
+0001dc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dc20: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
+0001dc30: 6578 742e 5741 524e 0d0a 2020 2020 2020  ext.WARN..      
+0001dc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dc50: 2020 2020 2020 2b20 2822 496e 7369 6465        + ("Inside
+0001dc60: 2042 6172 2028 2564 2922 2025 2069 290d   Bar (%d)" % i).
+0001dc70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001dc80: 2020 2020 2020 2020 2020 2020 202b 2063               + c
+0001dc90: 6f6c 6f72 5465 7874 2e45 4e44 0d0a 2020  olorText.END..  
+0001dca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dcb0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+0001dcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dcd0: 2073 6176 6544 6963 745b 2250 6174 7465   saveDict["Patte
+0001dce0: 726e 225d 203d 2073 6176 6564 5b31 5d20  rn"] = saved[1] 
+0001dcf0: 2b20 2249 6e73 6964 6520 4261 7220 2825  + "Inside Bar (%
+0001dd00: 6429 2220 2520 690d 0a20 2020 2020 2020  d)" % i..       
+0001dd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dd20: 2072 6574 7572 6e20 690d 0a20 2020 2020   return i..     
+0001dd30: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0001dd40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001dd50: 2020 2020 2020 7265 7475 726e 2030 0d0a        return 0..
+0001dd60: 2020 2020 2020 2020 7265 7475 726e 2030          return 0
+0001dd70: 0d0a 0d0a 2020 2020 2320 4669 6e64 2049  ....    # Find I
+0001dd80: 504f 2062 6173 650d 0a20 2020 2064 6566  PO base..    def
+0001dd90: 2076 616c 6964 6174 6549 706f 4261 7365   validateIpoBase
+0001dda0: 2873 656c 662c 2073 746f 636b 2c20 6466  (self, stock, df
+0001ddb0: 2c20 7363 7265 656e 4469 6374 2c20 7361  , screenDict, sa
+0001ddc0: 7665 4469 6374 2c20 7065 7263 656e 7461  veDict, percenta
+0001ddd0: 6765 3d30 2e33 293a 0d0a 2020 2020 2020  ge=0.3):..      
+0001dde0: 2020 6966 2064 6620 6973 204e 6f6e 6520    if df is None 
+0001ddf0: 6f72 206c 656e 2864 6629 203d 3d20 303a  or len(df) == 0:
+0001de00: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+0001de10: 7475 726e 2046 616c 7365 0d0a 2020 2020  turn False..    
+0001de20: 2020 2020 6461 7461 203d 2064 662e 636f      data = df.co
+0001de30: 7079 2829 0d0a 2020 2020 2020 2020 6c69  py()..        li
+0001de40: 7374 696e 6750 7269 6365 203d 2064 6174  stingPrice = dat
+0001de50: 615b 3a3a 2d31 5d2e 6865 6164 2831 295b  a[::-1].head(1)[
+0001de60: 224f 7065 6e22 5d2e 696c 6f63 5b30 5d0d  "Open"].iloc[0].
+0001de70: 0a20 2020 2020 2020 2063 7572 7265 6e74  .        current
+0001de80: 5072 6963 6520 3d20 6461 7461 2e68 6561  Price = data.hea
+0001de90: 6428 3129 5b22 436c 6f73 6522 5d2e 696c  d(1)["Close"].il
+0001dea0: 6f63 5b30 5d0d 0a20 2020 2020 2020 2041  oc[0]..        A
+0001deb0: 5448 203d 2064 6174 612e 6465 7363 7269  TH = data.descri
+0001dec0: 6265 2829 5b22 4869 6768 225d 5b22 6d61  be()["High"]["ma
+0001ded0: 7822 5d0d 0a20 2020 2020 2020 2069 6620  x"]..        if 
+0001dee0: 4154 4820 3e20 286c 6973 7469 6e67 5072  ATH > (listingPr
+0001def0: 6963 6520 2b20 286c 6973 7469 6e67 5072  ice + (listingPr
+0001df00: 6963 6520 2a20 7065 7263 656e 7461 6765  ice * percentage
+0001df10: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
+0001df20: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
+0001df30: 2020 2020 2020 2061 7761 7920 3d20 726f         away = ro
+0001df40: 756e 6428 2828 6375 7272 656e 7450 7269  und(((currentPri
+0001df50: 6365 202d 206c 6973 7469 6e67 5072 6963  ce - listingPric
+0001df60: 6529 202f 206c 6973 7469 6e67 5072 6963  e) / listingPric
+0001df70: 6529 202a 2031 3030 2c20 3129 0d0a 2020  e) * 100, 1)..  
+0001df80: 2020 2020 2020 6966 2028 0d0a 2020 2020        if (..    
+0001df90: 2020 2020 2020 2020 286c 6973 7469 6e67          (listing
+0001dfa0: 5072 6963 6520 2d20 286c 6973 7469 6e67  Price - (listing
+0001dfb0: 5072 6963 6520 2a20 7065 7263 656e 7461  Price * percenta
+0001dfc0: 6765 2929 0d0a 2020 2020 2020 2020 2020  ge))..          
+0001dfd0: 2020 3c3d 2063 7572 7265 6e74 5072 6963    <= currentPric
+0001dfe0: 650d 0a20 2020 2020 2020 2020 2020 203c  e..            <
+0001dff0: 3d20 286c 6973 7469 6e67 5072 6963 6520  = (listingPrice 
+0001e000: 2b20 286c 6973 7469 6e67 5072 6963 6520  + (listingPrice 
+0001e010: 2a20 7065 7263 656e 7461 6765 2929 0d0a  * percentage))..
+0001e020: 2020 2020 2020 2020 293a 0d0a 2020 2020          ):..    
+0001e030: 2020 2020 2020 2020 7361 7665 6420 3d20          saved = 
+0001e040: 7365 6c66 2e66 696e 6443 7572 7265 6e74  self.findCurrent
+0001e050: 5361 7665 6456 616c 7565 2873 6372 6565  SavedValue(scree
+0001e060: 6e44 6963 742c 2073 6176 6544 6963 742c  nDict, saveDict,
+0001e070: 2022 5061 7474 6572 6e22 290d 0a20 2020   "Pattern")..   
+0001e080: 2020 2020 2020 2020 2069 6620 6177 6179           if away
+0001e090: 203e 2030 3a0d 0a20 2020 2020 2020 2020   > 0:..         
+0001e0a0: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+0001e0b0: 745b 2250 6174 7465 726e 225d 203d 2028  t["Pattern"] = (
+0001e0c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001e0d0: 2020 2020 2020 7361 7665 645b 305d 200d        saved[0] .
+0001e0e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e0f0: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
+0001e100: 2e42 4f4c 440d 0a20 2020 2020 2020 2020  .BOLD..         
+0001e110: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
+0001e120: 6f72 5465 7874 2e47 5245 454e 0d0a 2020  orText.GREEN..  
+0001e130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e140: 2020 2b20 6622 4950 4f20 4261 7365 2028    + f"IPO Base (
+0001e150: 7b61 7761 797d 2025 2922 0d0a 2020 2020  {away} %)"..    
+0001e160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e170: 2b20 636f 6c6f 7254 6578 742e 454e 440d  + colorText.END.
+0001e180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e190: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+0001e1a0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+0001e1b0: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+0001e1c0: 745b 2250 6174 7465 726e 225d 203d 2028  t["Pattern"] = (
+0001e1d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001e1e0: 2020 2020 2020 7361 7665 645b 305d 0d0a        saved[0]..
+0001e1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e200: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
+0001e210: 424f 4c44 0d0a 2020 2020 2020 2020 2020  BOLD..          
+0001e220: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
+0001e230: 7254 6578 742e 4752 4545 4e0d 0a20 2020  rText.GREEN..   
+0001e240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e250: 202b 2022 4950 4f20 4261 7365 2022 0d0a   + "IPO Base "..
+0001e260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e270: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
+0001e280: 4641 494c 0d0a 2020 2020 2020 2020 2020  FAIL..          
+0001e290: 2020 2020 2020 2020 2020 2b20 6622 287b            + f"({
+0001e2a0: 6177 6179 7d20 2529 220d 0a20 2020 2020  away} %)"..     
+0001e2b0: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+0001e2c0: 2063 6f6c 6f72 5465 7874 2e45 4e44 0d0a   colorText.END..
+0001e2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e2e0: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+0001e2f0: 6176 6544 6963 745b 2250 6174 7465 726e  aveDict["Pattern
+0001e300: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
+0001e310: 6622 4950 4f20 4261 7365 2028 7b61 7761  f"IPO Base ({awa
+0001e320: 797d 2025 2922 0d0a 2020 2020 2020 2020  y} %)"..        
+0001e330: 2020 2020 7265 7475 726e 2054 7275 650d      return True.
+0001e340: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001e350: 4661 6c73 650d 0a0d 0a20 2020 2023 406d  False....    #@m
+0001e360: 6561 7375 7265 5f74 696d 650d 0a20 2020  easure_time..   
+0001e370: 2023 2056 616c 6964 6174 6520 4c6f 7265   # Validate Lore
+0001e380: 6e74 7a69 616e 2043 6c61 7373 6966 6963  ntzian Classific
+0001e390: 6174 696f 6e20 7369 676e 616c 0d0a 2020  ation signal..  
+0001e3a0: 2020 6465 6620 7661 6c69 6461 7465 4c6f    def validateLo
+0001e3b0: 7265 6e74 7a69 616e 2873 656c 662c 2064  rentzian(self, d
+0001e3c0: 662c 2073 6372 6565 6e44 6963 742c 2073  f, screenDict, s
+0001e3d0: 6176 6544 6963 742c 206c 6f6f 6b46 6f72  aveDict, lookFor
+0001e3e0: 3d33 293a 0d0a 2020 2020 2020 2020 6966  =3):..        if
+0001e3f0: 2064 6620 6973 204e 6f6e 6520 6f72 206c   df is None or l
+0001e400: 656e 2864 6629 203d 3d20 303a 0d0a 2020  en(df) == 0:..  
+0001e410: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0001e420: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+0001e430: 6461 7461 203d 2064 662e 636f 7079 2829  data = df.copy()
+0001e440: 0d0a 2020 2020 2020 2020 2320 6c6f 6f6b  ..        # look
+0001e450: 466f 723a 2031 2d42 7579 2c20 322d 5365  For: 1-Buy, 2-Se
+0001e460: 6c6c 2c20 332d 416e 790d 0a20 2020 2020  ll, 3-Any..     
+0001e470: 2020 2064 6174 6120 3d20 6461 7461 5b3a     data = data[:
+0001e480: 3a2d 315d 2020 2320 5265 7665 7273 6520  :-1]  # Reverse 
+0001e490: 7468 6520 6461 7461 6672 616d 650d 0a20  the dataframe.. 
+0001e4a0: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
+0001e4b0: 7461 2e72 656e 616d 6528 0d0a 2020 2020  ta.rename(..    
+0001e4c0: 2020 2020 2020 2020 636f 6c75 6d6e 733d          columns=
+0001e4d0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
+0001e4e0: 2020 2022 4f70 656e 223a 2022 6f70 656e     "Open": "open
+0001e4f0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+0001e500: 2020 2020 2243 6c6f 7365 223a 2022 636c      "Close": "cl
+0001e510: 6f73 6522 2c0d 0a20 2020 2020 2020 2020  ose",..         
+0001e520: 2020 2020 2020 2022 4869 6768 223a 2022         "High": "
+0001e530: 6869 6768 222c 0d0a 2020 2020 2020 2020  high",..        
+0001e540: 2020 2020 2020 2020 224c 6f77 223a 2022          "Low": "
+0001e550: 6c6f 7722 2c0d 0a20 2020 2020 2020 2020  low",..         
+0001e560: 2020 2020 2020 2022 566f 6c75 6d65 223a         "Volume":
+0001e570: 2022 766f 6c75 6d65 222c 0d0a 2020 2020   "volume",..    
+0001e580: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
+0001e590: 2020 2029 0d0a 2020 2020 2020 2020 7472     )..        tr
+0001e5a0: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+0001e5b0: 7769 7468 2053 7570 7072 6573 734f 7574  with SuppressOut
+0001e5c0: 7075 7428 7375 7070 7265 7373 5f73 7464  put(suppress_std
+0001e5d0: 6f75 743d 5472 7565 2c20 7375 7070 7265  out=True, suppre
+0001e5e0: 7373 5f73 7464 6572 723d 5472 7565 293a  ss_stderr=True):
+0001e5f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001e600: 2020 6c63 203d 2061 7461 2e4c 6f72 656e    lc = ata.Loren
+0001e610: 747a 6961 6e43 6c61 7373 6966 6963 6174  tzianClassificat
+0001e620: 696f 6e28 6461 7461 3d64 6174 6129 0d0a  ion(data=data)..
+0001e630: 2020 2020 2020 2020 2020 2020 7361 7665              save
+0001e640: 6420 3d20 7365 6c66 2e66 696e 6443 7572  d = self.findCur
+0001e650: 7265 6e74 5361 7665 6456 616c 7565 2873  rentSavedValue(s
+0001e660: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
+0001e670: 6963 742c 2022 5061 7474 6572 6e22 290d  ict, "Pattern").
+0001e680: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001e690: 6c63 2e64 662e 696c 6f63 5b2d 315d 5b22  lc.df.iloc[-1]["
+0001e6a0: 6973 4e65 7742 7579 5369 676e 616c 225d  isNewBuySignal"]
+0001e6b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001e6c0: 2020 2073 6372 6565 6e44 6963 745b 2250     screenDict["P
+0001e6d0: 6174 7465 726e 225d 203d 2028 0d0a 2020  attern"] = (..  
+0001e6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e6f0: 2020 7361 7665 645b 305d 202b 2063 6f6c    saved[0] + col
+0001e700: 6f72 5465 7874 2e42 4f4c 4420 2b20 636f  orText.BOLD + co
+0001e710: 6c6f 7254 6578 742e 4752 4545 4e20 2b20  lorText.GREEN + 
+0001e720: 224c 6f72 656e 747a 6961 6e2d 4275 7922  "Lorentzian-Buy"
+0001e730: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
+0001e740: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001e750: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
+0001e760: 2020 2020 2073 6176 6544 6963 745b 2250       saveDict["P
+0001e770: 6174 7465 726e 225d 203d 2073 6176 6564  attern"] = saved
+0001e780: 5b31 5d20 2b20 224c 6f72 656e 747a 6961  [1] + "Lorentzia
+0001e790: 6e2d 4275 7922 0d0a 2020 2020 2020 2020  n-Buy"..        
+0001e7a0: 2020 2020 2020 2020 6966 206c 6f6f 6b46          if lookF
+0001e7b0: 6f72 2021 3d20 323a 2023 204e 6f74 2053  or != 2: # Not S
+0001e7c0: 656c 6c0d 0a20 2020 2020 2020 2020 2020  ell..           
+0001e7d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0001e7e0: 5472 7565 0d0a 2020 2020 2020 2020 2020  True..          
+0001e7f0: 2020 656c 6966 206c 632e 6466 2e69 6c6f    elif lc.df.ilo
+0001e800: 635b 2d31 5d5b 2269 734e 6577 5365 6c6c  c[-1]["isNewSell
+0001e810: 5369 676e 616c 225d 3a0d 0a20 2020 2020  Signal"]:..     
+0001e820: 2020 2020 2020 2020 2020 2073 6372 6565             scree
+0001e830: 6e44 6963 745b 2250 6174 7465 726e 225d  nDict["Pattern"]
+0001e840: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
+0001e850: 2020 2020 2020 2020 2020 7361 7665 645b            saved[
+0001e860: 305d 202b 2063 6f6c 6f72 5465 7874 2e42  0] + colorText.B
+0001e870: 4f4c 4420 2b20 636f 6c6f 7254 6578 742e  OLD + colorText.
+0001e880: 4641 494c 202b 2022 4c6f 7265 6e74 7a69  FAIL + "Lorentzi
+0001e890: 616e 2d53 656c 6c22 202b 2063 6f6c 6f72  an-Sell" + color
+0001e8a0: 5465 7874 2e45 4e44 0d0a 2020 2020 2020  Text.END..      
+0001e8b0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+0001e8c0: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+0001e8d0: 6544 6963 745b 2250 6174 7465 726e 225d  eDict["Pattern"]
+0001e8e0: 203d 2073 6176 6564 5b31 5d20 2b20 224c   = saved[1] + "L
+0001e8f0: 6f72 656e 747a 6961 6e2d 5365 6c6c 220d  orentzian-Sell".
+0001e900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e910: 2069 6620 6c6f 6f6b 466f 7220 213d 2031   if lookFor != 1
+0001e920: 3a20 2320 4e6f 7420 4275 790d 0a20 2020  : # Not Buy..   
+0001e930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e940: 2072 6574 7572 6e20 5472 7565 0d0a 2020   return True..  
+0001e950: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+0001e960: 6570 7469 6f6e 3a20 2023 2070 7261 676d  eption:  # pragm
+0001e970: 613a 206e 6f20 636f 7665 720d 0a20 2020  a: no cover..   
+0001e980: 2020 2020 2020 2020 2023 2056 616c 7565           # Value
+0001e990: 4572 726f 723a 206f 7065 7261 6e64 7320  Error: operands 
+0001e9a0: 636f 756c 6420 6e6f 7420 6265 2062 726f  could not be bro
+0001e9b0: 6164 6361 7374 2074 6f67 6574 6865 7220  adcast together 
+0001e9c0: 7769 7468 2073 6861 7065 7320 2832 302c  with shapes (20,
+0001e9d0: 2920 2832 362c 290d 0a20 2020 2020 2020  ) (26,)..       
+0001e9e0: 2020 2020 2023 2046 696c 6520 222f 6f70       # File "/op
+0001e9f0: 742f 686f 6d65 6272 6577 2f6c 6962 2f70  t/homebrew/lib/p
+0001ea00: 7974 686f 6e33 2e31 312f 7369 7465 2d70  ython3.11/site-p
+0001ea10: 6163 6b61 6765 732f 6164 7661 6e63 6564  ackages/advanced
+0001ea20: 5f74 612f 4c6f 7265 6e74 7a69 616e 436c  _ta/LorentzianCl
+0001ea30: 6173 7369 6669 6361 7469 6f6e 2f43 6c61  assification/Cla
+0001ea40: 7373 6966 6965 722e 7079 222c 206c 696e  ssifier.py", lin
+0001ea50: 6520 3138 362c 2069 6e20 5f5f 696e 6974  e 186, in __init
+0001ea60: 5f5f 0d0a 2020 2020 2020 2020 2020 2020  __..            
+0001ea70: 2320 4669 6c65 2022 2f6f 7074 2f68 6f6d  # File "/opt/hom
+0001ea80: 6562 7265 772f 6c69 622f 7079 7468 6f6e  ebrew/lib/python
+0001ea90: 332e 3131 2f73 6974 652d 7061 636b 6167  3.11/site-packag
+0001eaa0: 6573 2f61 6476 616e 6365 645f 7461 2f4c  es/advanced_ta/L
+0001eab0: 6f72 656e 747a 6961 6e43 6c61 7373 6966  orentzianClassif
+0001eac0: 6963 6174 696f 6e2f 436c 6173 7369 6669  ication/Classifi
+0001ead0: 6572 2e70 7922 2c20 6c69 6e65 2033 3935  er.py", line 395
+0001eae0: 2c20 696e 205f 5f63 6c61 7373 6966 790d  , in __classify.
+0001eaf0: 0a20 2020 2020 2020 2020 2020 2023 2046  .            # F
+0001eb00: 696c 6520 222f 6f70 742f 686f 6d65 6272  ile "/opt/homebr
+0001eb10: 6577 2f6c 6962 2f70 7974 686f 6e33 2e31  ew/lib/python3.1
+0001eb20: 312f 7369 7465 2d70 6163 6b61 6765 732f  1/site-packages/
+0001eb30: 7061 6e64 6173 2f63 6f72 652f 6f70 732f  pandas/core/ops/
+0001eb40: 636f 6d6d 6f6e 2e70 7922 2c20 6c69 6e65  common.py", line
+0001eb50: 2037 362c 2069 6e20 6e65 775f 6d65 7468   76, in new_meth
+0001eb60: 6f64 0d0a 2020 2020 2020 2020 2020 2020  od..            
+0001eb70: 2320 4669 6c65 2022 2f6f 7074 2f68 6f6d  # File "/opt/hom
+0001eb80: 6562 7265 772f 6c69 622f 7079 7468 6f6e  ebrew/lib/python
+0001eb90: 332e 3131 2f73 6974 652d 7061 636b 6167  3.11/site-packag
+0001eba0: 6573 2f70 616e 6461 732f 636f 7265 2f61  es/pandas/core/a
+0001ebb0: 7272 6179 6c69 6b65 2e70 7922 2c20 6c69  rraylike.py", li
+0001ebc0: 6e65 2037 302c 2069 6e20 5f5f 616e 645f  ne 70, in __and_
+0001ebd0: 5f0d 0a20 2020 2020 2020 2020 2020 2023  _..            #
+0001ebe0: 2046 696c 6520 222f 6f70 742f 686f 6d65   File "/opt/home
+0001ebf0: 6272 6577 2f6c 6962 2f70 7974 686f 6e33  brew/lib/python3
+0001ec00: 2e31 312f 7369 7465 2d70 6163 6b61 6765  .11/site-package
+0001ec10: 732f 7061 6e64 6173 2f63 6f72 652f 7365  s/pandas/core/se
+0001ec20: 7269 6573 2e70 7922 2c20 6c69 6e65 2035  ries.py", line 5
+0001ec30: 3831 302c 2069 6e20 5f6c 6f67 6963 616c  810, in _logical
+0001ec40: 5f6d 6574 686f 640d 0a20 2020 2020 2020  _method..       
+0001ec50: 2020 2020 2023 2046 696c 6520 222f 6f70       # File "/op
+0001ec60: 742f 686f 6d65 6272 6577 2f6c 6962 2f70  t/homebrew/lib/p
+0001ec70: 7974 686f 6e33 2e31 312f 7369 7465 2d70  ython3.11/site-p
+0001ec80: 6163 6b61 6765 732f 7061 6e64 6173 2f63  ackages/pandas/c
+0001ec90: 6f72 652f 6f70 732f 6172 7261 795f 6f70  ore/ops/array_op
+0001eca0: 732e 7079 222c 206c 696e 6520 3435 362c  s.py", line 456,
+0001ecb0: 2069 6e20 6c6f 6769 6361 6c5f 6f70 0d0a   in logical_op..
+0001ecc0: 2020 2020 2020 2020 2020 2020 2320 4669              # Fi
+0001ecd0: 6c65 2022 2f6f 7074 2f68 6f6d 6562 7265  le "/opt/homebre
+0001ece0: 772f 6c69 622f 7079 7468 6f6e 332e 3131  w/lib/python3.11
+0001ecf0: 2f73 6974 652d 7061 636b 6167 6573 2f70  /site-packages/p
+0001ed00: 616e 6461 732f 636f 7265 2f6f 7073 2f61  andas/core/ops/a
+0001ed10: 7272 6179 5f6f 7073 2e70 7922 2c20 6c69  rray_ops.py", li
+0001ed20: 6e65 2033 3634 2c20 696e 206e 615f 6c6f  ne 364, in na_lo
+0001ed30: 6769 6361 6c5f 6f70 0d0a 2020 2020 2020  gical_op..      
+0001ed40: 2020 2020 2020 2320 7365 6c66 2e64 6566        # self.def
+0001ed50: 6175 6c74 5f6c 6f67 6765 722e 6465 6275  ault_logger.debu
+0001ed60: 6728 652c 2065 7863 5f69 6e66 6f3d 5472  g(e, exc_info=Tr
+0001ed70: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
+0001ed80: 2070 6173 730d 0a20 2020 2020 2020 2072   pass..        r
+0001ed90: 6574 7572 6e20 4661 6c73 650d 0a0d 0a20  eturn False.... 
+0001eda0: 2020 2023 2076 616c 6964 6174 6520 6966     # validate if
+0001edb0: 2074 6865 2073 746f 636b 2068 6173 2062   the stock has b
+0001edc0: 6565 6e20 6861 7669 6e67 206c 6f77 6572  een having lower
+0001edd0: 206c 6f77 732c 206c 6f77 6572 2068 6967   lows, lower hig
+0001ede0: 6873 0d0a 2020 2020 6465 6620 7661 6c69  hs..    def vali
+0001edf0: 6461 7465 4c6f 7765 7248 6967 6873 4c6f  dateLowerHighsLo
+0001ee00: 7765 724c 6f77 7328 7365 6c66 2c20 6466  werLows(self, df
+0001ee10: 293a 0d0a 2020 2020 2020 2020 6966 2064  ):..        if d
+0001ee20: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
+0001ee30: 2864 6629 203d 3d20 303a 0d0a 2020 2020  (df) == 0:..    
+0001ee40: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+0001ee50: 616c 7365 0d0a 2020 2020 2020 2020 6461  alse..        da
+0001ee60: 7461 203d 2064 662e 636f 7079 2829 0d0a  ta = df.copy()..
+0001ee70: 2020 2020 2020 2020 6461 7930 203d 2064          day0 = d
+0001ee80: 6174 610d 0a20 2020 2020 2020 2064 6179  ata..        day
+0001ee90: 3120 3d20 6461 7461 5b31 3a5d 0d0a 2020  1 = data[1:]..  
+0001eea0: 2020 2020 2020 6461 7932 203d 2064 6174        day2 = dat
+0001eeb0: 615b 323a 5d0d 0a20 2020 2020 2020 2064  a[2:]..        d
+0001eec0: 6179 3320 3d20 6461 7461 5b33 3a5d 0d0a  ay3 = data[3:]..
+0001eed0: 2020 2020 2020 2020 6c6f 7765 7248 6967          lowerHig
+0001eee0: 6873 203d 2028 0d0a 2020 2020 2020 2020  hs = (..        
+0001eef0: 2020 2020 2864 6179 305b 2248 6967 6822      (day0["High"
+0001ef00: 5d2e 696c 6f63 5b30 5d20 3c20 6461 7931  ].iloc[0] < day1
+0001ef10: 5b22 4869 6768 225d 2e69 6c6f 635b 305d  ["High"].iloc[0]
+0001ef20: 290d 0a20 2020 2020 2020 2020 2020 2061  )..            a
+0001ef30: 6e64 2028 6461 7931 5b22 4869 6768 225d  nd (day1["High"]
+0001ef40: 2e69 6c6f 635b 305d 203c 2064 6179 325b  .iloc[0] < day2[
+0001ef50: 2248 6967 6822 5d2e 696c 6f63 5b30 5d29  "High"].iloc[0])
+0001ef60: 0d0a 2020 2020 2020 2020 2020 2020 616e  ..            an
+0001ef70: 6420 2864 6179 325b 2248 6967 6822 5d2e  d (day2["High"].
+0001ef80: 696c 6f63 5b30 5d20 3c20 6461 7933 5b22  iloc[0] < day3["
+0001ef90: 4869 6768 225d 2e69 6c6f 635b 305d 290d  High"].iloc[0]).
+0001efa0: 0a20 2020 2020 2020 2029 0d0a 2020 2020  .        )..    
+0001efb0: 2020 2020 6c6f 7765 724c 6f77 7320 3d20      lowerLows = 
+0001efc0: 280d 0a20 2020 2020 2020 2020 2020 2028  (..            (
+0001efd0: 6461 7930 5b22 4c6f 7722 5d2e 696c 6f63  day0["Low"].iloc
+0001efe0: 5b30 5d20 3c20 6461 7931 5b22 4c6f 7722  [0] < day1["Low"
+0001eff0: 5d2e 696c 6f63 5b30 5d29 0d0a 2020 2020  ].iloc[0])..    
+0001f000: 2020 2020 2020 2020 616e 6420 2864 6179          and (day
+0001f010: 315b 224c 6f77 225d 2e69 6c6f 635b 305d  1["Low"].iloc[0]
+0001f020: 203c 2064 6179 325b 224c 6f77 225d 2e69   < day2["Low"].i
+0001f030: 6c6f 635b 305d 290d 0a20 2020 2020 2020  loc[0])..       
+0001f040: 2020 2020 2061 6e64 2028 6461 7932 5b22       and (day2["
+0001f050: 4c6f 7722 5d2e 696c 6f63 5b30 5d20 3c20  Low"].iloc[0] < 
+0001f060: 6461 7933 5b22 4c6f 7722 5d2e 696c 6f63  day3["Low"].iloc
+0001f070: 5b30 5d29 0d0a 2020 2020 2020 2020 290d  [0])..        ).
+0001f080: 0a20 2020 2020 2020 2068 6967 6865 7252  .        higherR
+0001f090: 5349 203d 2028 0d0a 2020 2020 2020 2020  SI = (..        
+0001f0a0: 2020 2020 2864 6179 305b 2252 5349 225d      (day0["RSI"]
+0001f0b0: 2e69 6c6f 635b 305d 203c 2064 6179 315b  .iloc[0] < day1[
+0001f0c0: 2252 5349 225d 2e69 6c6f 635b 305d 290d  "RSI"].iloc[0]).
+0001f0d0: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
+0001f0e0: 2028 6461 7931 5b22 5253 4922 5d2e 696c   (day1["RSI"].il
+0001f0f0: 6f63 5b30 5d20 3c20 6461 7932 5b22 5253  oc[0] < day2["RS
+0001f100: 4922 5d2e 696c 6f63 5b30 5d29 0d0a 2020  I"].iloc[0])..  
+0001f110: 2020 2020 2020 2020 2020 616e 6420 2864            and (d
+0001f120: 6179 325b 2252 5349 225d 2e69 6c6f 635b  ay2["RSI"].iloc[
+0001f130: 305d 203c 2064 6179 335b 2252 5349 225d  0] < day3["RSI"]
+0001f140: 2e69 6c6f 635b 305d 290d 0a20 2020 2020  .iloc[0])..     
+0001f150: 2020 2020 2020 2061 6e64 2064 6179 305b         and day0[
+0001f160: 2252 5349 225d 2e69 6c6f 635b 305d 203e  "RSI"].iloc[0] >
+0001f170: 3d20 3530 0d0a 2020 2020 2020 2020 290d  = 50..        ).
+0001f180: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001f190: 6c6f 7765 7248 6967 6873 2061 6e64 206c  lowerHighs and l
+0001f1a0: 6f77 6572 4c6f 7773 2061 6e64 2068 6967  owerLows and hig
+0001f1b0: 6865 7252 5349 0d0a 0d0a 2020 2020 2320  herRSI....    # 
+0001f1c0: 5661 6c69 6461 7465 2069 6620 7265 6365  Validate if rece
+0001f1d0: 6e74 2076 6f6c 756d 6520 6973 206c 6f77  nt volume is low
+0001f1e0: 6573 7420 6f66 206c 6173 7420 274e 2720  est of last 'N' 
+0001f1f0: 4461 7973 0d0a 2020 2020 6465 6620 7661  Days..    def va
+0001f200: 6c69 6461 7465 4c6f 7765 7374 566f 6c75  lidateLowestVolu
+0001f210: 6d65 2873 656c 662c 2064 662c 2064 6179  me(self, df, day
+0001f220: 7346 6f72 4c6f 7765 7374 566f 6c75 6d65  sForLowestVolume
+0001f230: 293a 0d0a 2020 2020 2020 2020 6966 2064  ):..        if d
+0001f240: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
+0001f250: 2864 6629 203d 3d20 303a 0d0a 2020 2020  (df) == 0:..    
+0001f260: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+0001f270: 616c 7365 0d0a 2020 2020 2020 2020 6461  alse..        da
+0001f280: 7461 203d 2064 662e 636f 7079 2829 0d0a  ta = df.copy()..
+0001f290: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+0001f2a0: 6174 612e 6669 6c6c 6e61 2830 290d 0a20  ata.fillna(0).. 
+0001f2b0: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
+0001f2c0: 7461 2e72 6570 6c61 6365 285b 6e70 2e69  ta.replace([np.i
+0001f2d0: 6e66 2c20 2d6e 702e 696e 665d 2c20 3029  nf, -np.inf], 0)
+0001f2e0: 0d0a 2020 2020 2020 2020 6966 2064 6179  ..        if day
+0001f2f0: 7346 6f72 4c6f 7765 7374 566f 6c75 6d65  sForLowestVolume
+0001f300: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
+0001f310: 2020 2020 2020 2064 6179 7346 6f72 4c6f         daysForLo
+0001f320: 7765 7374 566f 6c75 6d65 203d 2033 300d  westVolume = 30.
+0001f330: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+0001f340: 6461 7461 2920 3c20 6461 7973 466f 724c  data) < daysForL
+0001f350: 6f77 6573 7456 6f6c 756d 653a 0d0a 2020  owestVolume:..  
+0001f360: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0001f370: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+0001f380: 6461 7461 203d 2064 6174 612e 6865 6164  data = data.head
+0001f390: 2864 6179 7346 6f72 4c6f 7765 7374 566f  (daysForLowestVo
+0001f3a0: 6c75 6d65 290d 0a20 2020 2020 2020 2072  lume)..        r
+0001f3b0: 6563 656e 7420 3d20 6461 7461 2e68 6561  ecent = data.hea
+0001f3c0: 6428 3129 0d0a 2020 2020 2020 2020 6966  d(1)..        if
+0001f3d0: 206c 656e 2872 6563 656e 7429 203c 2031   len(recent) < 1
+0001f3e0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+0001f3f0: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
+0001f400: 2020 2020 2069 6620 2872 6563 656e 745b       if (recent[
+0001f410: 2256 6f6c 756d 6522 5d2e 696c 6f63 5b30  "Volume"].iloc[0
+0001f420: 5d20 3c3d 2064 6174 612e 6465 7363 7269  ] <= data.descri
+0001f430: 6265 2829 5b22 566f 6c75 6d65 225d 5b22  be()["Volume"]["
+0001f440: 6d69 6e22 5d29 2061 6e64 2072 6563 656e  min"]) and recen
+0001f450: 745b 0d0a 2020 2020 2020 2020 2020 2020  t[..            
+0001f460: 2256 6f6c 756d 6522 0d0a 2020 2020 2020  "Volume"..      
+0001f470: 2020 5d5b 305d 2021 3d20 6e70 2e6e 616e    ][0] != np.nan
+0001f480: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+0001f490: 6574 7572 6e20 5472 7565 0d0a 2020 2020  eturn True..    
+0001f4a0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+0001f4b0: 0d0a 0d0a 2020 2020 2320 5661 6c69 6461  ....    # Valida
+0001f4c0: 7465 204c 5450 2077 6974 6869 6e20 6c69  te LTP within li
+0001f4d0: 6d69 7473 0d0a 2020 2020 6465 6620 7661  mits..    def va
+0001f4e0: 6c69 6461 7465 4c54 5028 7365 6c66 2c20  lidateLTP(self, 
+0001f4f0: 6466 2c20 7363 7265 656e 4469 6374 2c20  df, screenDict, 
+0001f500: 7361 7665 4469 6374 2c20 6d69 6e4c 5450  saveDict, minLTP
+0001f510: 3d4e 6f6e 652c 206d 6178 4c54 503d 4e6f  =None, maxLTP=No
+0001f520: 6e65 2c6d 696e 4368 616e 6765 3d30 293a  ne,minChange=0):
+0001f530: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
+0001f540: 2064 662e 636f 7079 2829 0d0a 2020 2020   df.copy()..    
+0001f550: 2020 2020 6c74 7056 616c 6964 203d 2046      ltpValid = F
+0001f560: 616c 7365 0d0a 2020 2020 2020 2020 6966  alse..        if
+0001f570: 206d 696e 4c54 5020 6973 204e 6f6e 653a   minLTP is None:
+0001f580: 0d0a 2020 2020 2020 2020 2020 2020 6d69  ..            mi
+0001f590: 6e4c 5450 203d 2073 656c 662e 636f 6e66  nLTP = self.conf
+0001f5a0: 6967 4d61 6e61 6765 722e 6d69 6e4c 5450  igManager.minLTP
+0001f5b0: 0d0a 2020 2020 2020 2020 6966 206d 6178  ..        if max
+0001f5c0: 4c54 5020 6973 204e 6f6e 653a 0d0a 2020  LTP is None:..  
+0001f5d0: 2020 2020 2020 2020 2020 6d61 784c 5450            maxLTP
+0001f5e0: 203d 2073 656c 662e 636f 6e66 6967 4d61   = self.configMa
+0001f5f0: 6e61 6765 722e 6d61 784c 5450 0d0a 2020  nager.maxLTP..  
+0001f600: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
+0001f610: 612e 6669 6c6c 6e61 2830 290d 0a20 2020  a.fillna(0)..   
+0001f620: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+0001f630: 2e72 6570 6c61 6365 285b 6e70 2e69 6e66  .replace([np.inf
+0001f640: 2c20 2d6e 702e 696e 665d 2c20 3029 0d0a  , -np.inf], 0)..
+0001f650: 2020 2020 2020 2020 7265 6365 6e74 203d          recent =
+0001f660: 2064 6174 612e 6865 6164 2831 290d 0a0d   data.head(1)...
+0001f670: 0a20 2020 2020 2020 2070 6374 5f63 6861  .        pct_cha
+0001f680: 6e67 6520 3d20 2864 6174 615b 3a3a 2d31  nge = (data[::-1
+0001f690: 5d5b 2243 6c6f 7365 225d 2e70 6374 5f63  ]["Close"].pct_c
+0001f6a0: 6861 6e67 6528 2920 2a20 3130 3029 2e69  hange() * 100).i
+0001f6b0: 6c6f 635b 2d31 5d0d 0a20 2020 2020 2020  loc[-1]..       
+0001f6c0: 2069 6620 7063 745f 6368 616e 6765 203d   if pct_change =
+0001f6d0: 3d20 6e70 2e69 6e66 206f 7220 7063 745f  = np.inf or pct_
+0001f6e0: 6368 616e 6765 203d 3d20 2d6e 702e 696e  change == -np.in
+0001f6f0: 663a 0d0a 2020 2020 2020 2020 2020 2020  f:..            
+0001f700: 7063 745f 6368 616e 6765 203d 2030 0d0a  pct_change = 0..
+0001f710: 2020 2020 2020 2020 7063 745f 7361 7665          pct_save
+0001f720: 203d 2022 252e 3166 2525 2220 2520 7063   = "%.1f%%" % pc
+0001f730: 745f 6368 616e 6765 0d0a 2020 2020 2020  t_change..      
+0001f740: 2020 6966 2070 6374 5f63 6861 6e67 6520    if pct_change 
+0001f750: 3e20 302e 323a 0d0a 2020 2020 2020 2020  > 0.2:..        
+0001f760: 2020 2020 7063 745f 6368 616e 6765 203d      pct_change =
+0001f770: 2063 6f6c 6f72 5465 7874 2e47 5245 454e   colorText.GREEN
+0001f780: 202b 2028 2225 2e31 6625 2522 2025 2070   + ("%.1f%%" % p
+0001f790: 6374 5f63 6861 6e67 6529 202b 2063 6f6c  ct_change) + col
+0001f7a0: 6f72 5465 7874 2e45 4e44 0d0a 2020 2020  orText.END..    
+0001f7b0: 2020 2020 656c 6966 2070 6374 5f63 6861      elif pct_cha
+0001f7c0: 6e67 6520 3c20 2d30 2e32 3a0d 0a20 2020  nge < -0.2:..   
+0001f7d0: 2020 2020 2020 2020 2070 6374 5f63 6861           pct_cha
+0001f7e0: 6e67 6520 3d20 636f 6c6f 7254 6578 742e  nge = colorText.
+0001f7f0: 4641 494c 202b 2028 2225 2e31 6625 2522  FAIL + ("%.1f%%"
+0001f800: 2025 2070 6374 5f63 6861 6e67 6529 202b   % pct_change) +
+0001f810: 2063 6f6c 6f72 5465 7874 2e45 4e44 0d0a   colorText.END..
+0001f820: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+0001f830: 2020 2020 2020 2020 2020 2070 6374 5f63             pct_c
+0001f840: 6861 6e67 6520 3d20 636f 6c6f 7254 6578  hange = colorTex
+0001f850: 742e 5741 524e 202b 2028 2225 2e31 6625  t.WARN + ("%.1f%
+0001f860: 2522 2025 2070 6374 5f63 6861 6e67 6529  %" % pct_change)
+0001f870: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
+0001f880: 0d0a 2020 2020 2020 2020 7361 7665 4469  ..        saveDi
+0001f890: 6374 5b22 2543 686e 6722 5d20 3d20 7063  ct["%Chng"] = pc
+0001f8a0: 745f 7361 7665 0d0a 2020 2020 2020 2020  t_save..        
+0001f8b0: 7363 7265 656e 4469 6374 5b22 2543 686e  screenDict["%Chn
+0001f8c0: 6722 5d20 3d20 7063 745f 6368 616e 6765  g"] = pct_change
+0001f8d0: 0d0a 2020 2020 2020 2020 6c74 7020 3d20  ..        ltp = 
+0001f8e0: 726f 756e 6428 7265 6365 6e74 5b22 436c  round(recent["Cl
+0001f8f0: 6f73 6522 5d2e 696c 6f63 5b30 5d2c 2032  ose"].iloc[0], 2
+0001f900: 290d 0a20 2020 2020 2020 2076 6572 6966  )..        verif
+0001f910: 7953 7461 6765 5477 6f20 3d20 5472 7565  yStageTwo = True
+0001f920: 0d0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
+0001f930: 2864 6174 6129 203e 2032 3530 3a0d 0a20  (data) > 250:.. 
+0001f940: 2020 2020 2020 2020 2020 2079 6561 726c             yearl
+0001f950: 794c 6f77 203d 2064 6174 612e 6865 6164  yLow = data.head
+0001f960: 2832 3530 295b 2243 6c6f 7365 225d 2e6d  (250)["Close"].m
+0001f970: 696e 2829 0d0a 2020 2020 2020 2020 2020  in()..          
+0001f980: 2020 7965 6172 6c79 4869 6768 203d 2064    yearlyHigh = d
+0001f990: 6174 612e 6865 6164 2832 3530 295b 2243  ata.head(250)["C
+0001f9a0: 6c6f 7365 225d 2e6d 6178 2829 0d0a 2020  lose"].max()..  
+0001f9b0: 2020 2020 2020 2020 2020 6966 206c 7470            if ltp
+0001f9c0: 203c 2028 3220 2a20 7965 6172 6c79 4c6f   < (2 * yearlyLo
+0001f9d0: 7729 2061 6e64 206c 7470 203c 2028 302e  w) and ltp < (0.
+0001f9e0: 3735 202a 2079 6561 726c 7948 6967 6829  75 * yearlyHigh)
+0001f9f0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001fa00: 2020 2076 6572 6966 7953 7461 6765 5477     verifyStageTw
+0001fa10: 6f20 3d20 4661 6c73 650d 0a20 2020 2020  o = False..     
+0001fa20: 2020 2020 2020 2020 2020 2073 6372 6565             scree
+0001fa30: 6e44 6963 745b 2253 746f 636b 225d 203d  nDict["Stock"] =
+0001fa40: 2063 6f6c 6f72 5465 7874 2e46 4149 4c20   colorText.FAIL 
+0001fa50: 2b20 7361 7665 4469 6374 5b22 5374 6f63  + saveDict["Stoc
+0001fa60: 6b22 5d20 2b20 636f 6c6f 7254 6578 742e  k"] + colorText.
+0001fa70: 454e 440d 0a20 2020 2020 2020 2069 6620  END..        if 
+0001fa80: 6c74 7020 3e3d 206d 696e 4c54 5020 616e  ltp >= minLTP an
+0001fa90: 6420 6c74 7020 3c3d 206d 6178 4c54 503a  d ltp <= maxLTP:
+0001faa0: 0d0a 2020 2020 2020 2020 2020 2020 6c74  ..            lt
+0001fab0: 7056 616c 6964 203d 2054 7275 650d 0a20  pValid = True.. 
+0001fac0: 2020 2020 2020 2020 2020 2069 6620 6d69             if mi
+0001fad0: 6e43 6861 6e67 6520 213d 2030 3a0d 0a20  nChange != 0:.. 
+0001fae0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0001faf0: 2055 7365 7220 6861 7320 7375 7070 6c69   User has suppli
+0001fb00: 6564 2073 6f6d 6520 6669 6c74 6572 2066  ed some filter f
+0001fb10: 6f72 2070 6572 6365 6e74 6167 6520 6368  or percentage ch
+0001fb20: 616e 6765 0d0a 2020 2020 2020 2020 2020  ange..          
+0001fb30: 2020 2020 2020 6c74 7056 616c 6964 203d        ltpValid =
+0001fb40: 2066 6c6f 6174 2873 7472 2870 6374 5f73   float(str(pct_s
+0001fb50: 6176 6529 2e72 6570 6c61 6365 2822 2522  ave).replace("%"
+0001fb60: 2c22 2229 2920 3e3d 206d 696e 4368 616e  ,"")) >= minChan
+0001fb70: 6765 0d0a 2020 2020 2020 2020 2020 2020  ge..            
+0001fb80: 7361 7665 4469 6374 5b22 4c54 5022 5d20  saveDict["LTP"] 
+0001fb90: 3d20 726f 756e 6428 6c74 702c 2032 290d  = round(ltp, 2).
+0001fba0: 0a20 2020 2020 2020 2020 2020 2073 6372  .            scr
+0001fbb0: 6565 6e44 6963 745b 224c 5450 225d 203d  eenDict["LTP"] =
+0001fbc0: 2028 636f 6c6f 7254 6578 742e 4752 4545   (colorText.GREE
+0001fbd0: 4e20 6966 206c 7470 5661 6c69 6420 656c  N if ltpValid el
+0001fbe0: 7365 2063 6f6c 6f72 5465 7874 2e46 4149  se colorText.FAI
+0001fbf0: 4c29 202b 2028 2225 2e32 6622 2025 206c  L) + ("%.2f" % l
+0001fc00: 7470 2920 2b20 636f 6c6f 7254 6578 742e  tp) + colorText.
+0001fc10: 454e 440d 0a20 2020 2020 2020 2020 2020  END..           
+0001fc20: 2072 6574 7572 6e20 6c74 7056 616c 6964   return ltpValid
+0001fc30: 2c20 7665 7269 6679 5374 6167 6554 776f  , verifyStageTwo
+0001fc40: 0d0a 2020 2020 2020 2020 7363 7265 656e  ..        screen
+0001fc50: 4469 6374 5b22 4c54 5022 5d20 3d20 636f  Dict["LTP"] = co
+0001fc60: 6c6f 7254 6578 742e 4641 494c 202b 2028  lorText.FAIL + (
+0001fc70: 2225 2e32 6622 2025 206c 7470 2920 2b20  "%.2f" % ltp) + 
+0001fc80: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
+0001fc90: 2020 2020 2020 2073 6176 6544 6963 745b         saveDict[
+0001fca0: 224c 5450 225d 203d 2072 6f75 6e64 286c  "LTP"] = round(l
+0001fcb0: 7470 2c20 3229 0d0a 2020 2020 2020 2020  tp, 2)..        
+0001fcc0: 7265 7475 726e 206c 7470 5661 6c69 642c  return ltpValid,
+0001fcd0: 2076 6572 6966 7953 7461 6765 5477 6f0d   verifyStageTwo.
+0001fce0: 0a0d 0a20 2020 2064 6566 2076 616c 6964  ...    def valid
+0001fcf0: 6174 654c 5450 466f 7250 6f72 7466 6f6c  ateLTPForPortfol
+0001fd00: 696f 4361 6c63 2873 656c 662c 2064 662c  ioCalc(self, df,
+0001fd10: 2073 6372 6565 6e44 6963 742c 2073 6176   screenDict, sav
+0001fd20: 6544 6963 742c 7265 7175 6573 7465 6450  eDict,requestedP
+0001fd30: 6572 696f 643d 3029 3a0d 0a20 2020 2020  eriod=0):..     
+0001fd40: 2020 2064 6174 6120 3d20 6466 2e63 6f70     data = df.cop
+0001fd50: 7928 290d 0a20 2020 2020 2020 2070 6572  y()..        per
+0001fd60: 696f 6473 203d 2073 656c 662e 636f 6e66  iods = self.conf
+0001fd70: 6967 4d61 6e61 6765 722e 7065 7269 6f64  igManager.period
+0001fd80: 7352 616e 6765 0d0a 2020 2020 2020 2020  sRange..        
+0001fd90: 6966 2072 6571 7565 7374 6564 5065 7269  if requestedPeri
+0001fda0: 6f64 203e 2030 2061 6e64 2072 6571 7565  od > 0 and reque
+0001fdb0: 7374 6564 5065 7269 6f64 206e 6f74 2069  stedPeriod not i
+0001fdc0: 6e20 7065 7269 6f64 733a 0d0a 2020 2020  n periods:..    
+0001fdd0: 2020 2020 2020 2020 7065 7269 6f64 732e          periods.
+0001fde0: 6170 7065 6e64 2872 6571 7565 7374 6564  append(requested
+0001fdf0: 5065 7269 6f64 290d 0a20 2020 2020 2020  Period)..       
+0001fe00: 2070 7265 7669 6f75 735f 7265 6365 6e74   previous_recent
+0001fe10: 203d 2064 6174 612e 6865 6164 2831 290d   = data.head(1).
+0001fe20: 0a20 2020 2020 2020 2070 7265 7669 6f75  .        previou
+0001fe30: 735f 7265 6365 6e74 2e72 6573 6574 5f69  s_recent.reset_i
+0001fe40: 6e64 6578 2869 6e70 6c61 6365 3d54 7275  ndex(inplace=Tru
+0001fe50: 6529 0d0a 2020 2020 2020 2020 6361 6c63  e)..        calc
+0001fe60: 5f64 6174 6520 3d20 7374 7228 7072 6576  _date = str(prev
+0001fe70: 696f 7573 5f72 6563 656e 742e 696c 6f63  ious_recent.iloc
+0001fe80: 5b3a 2c20 305d 5b30 5d29 2e73 706c 6974  [:, 0][0]).split
+0001fe90: 2822 2022 295b 305d 0d0a 2020 2020 2020  (" ")[0]..      
+0001fea0: 2020 666f 7220 7072 6420 696e 2070 6572    for prd in per
+0001feb0: 696f 6473 3a0d 0a20 2020 2020 2020 2020  iods:..         
+0001fec0: 2020 2069 6620 6c65 6e28 6461 7461 2920     if len(data) 
+0001fed0: 3e3d 2070 7264 202b 2031 3a0d 0a20 2020  >= prd + 1:..   
+0001fee0: 2020 2020 2020 2020 2020 2020 2070 7265               pre
+0001fef0: 764c 7470 203d 2064 6174 615b 2243 6c6f  vLtp = data["Clo
+0001ff00: 7365 225d 2e69 6c6f 635b 305d 0d0a 2020  se"].iloc[0]..  
+0001ff10: 2020 2020 2020 2020 2020 2020 2020 6c74                lt
+0001ff20: 7054 6479 203d 2064 6174 615b 2243 6c6f  pTdy = data["Clo
+0001ff30: 7365 225d 2e69 6c6f 635b 7072 645d 0d0a  se"].iloc[prd]..
+0001ff40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ff50: 6966 2069 7369 6e73 7461 6e63 6528 7072  if isinstance(pr
+0001ff60: 6576 4c74 702c 7064 2e53 6572 6965 7329  evLtp,pd.Series)
+0001ff70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001ff80: 2020 2020 2020 2070 7265 764c 7470 203d         prevLtp =
+0001ff90: 2070 7265 764c 7470 5b30 5d0d 0a20 2020   prevLtp[0]..   
+0001ffa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ffb0: 206c 7470 5464 7920 3d20 6c74 7054 6479   ltpTdy = ltpTdy
+0001ffc0: 5b30 5d0d 0a20 2020 2020 2020 2020 2020  [0]..           
+0001ffd0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+0001ffe0: 6622 4c54 507b 7072 647d 225d 203d 2028  f"LTP{prd}"] = (
+0001fff0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00020000: 2020 2020 2020 2863 6f6c 6f72 5465 7874        (colorText
+00020010: 2e47 5245 454e 2069 6620 286c 7470 5464  .GREEN if (ltpTd
+00020020: 7920 3e3d 2070 7265 764c 7470 2920 656c  y >= prevLtp) el
+00020030: 7365 2028 636f 6c6f 7254 6578 742e 4641  se (colorText.FA
+00020040: 494c 2929 0d0a 2020 2020 2020 2020 2020  IL))..          
+00020050: 2020 2020 2020 2020 2020 2b20 7374 7228            + str(
+00020060: 227b 3a2e 3266 7d22 2e66 6f72 6d61 7428  "{:.2f}".format(
+00020070: 6c74 7054 6479 2929 0d0a 2020 2020 2020  ltpTdy))..      
+00020080: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+00020090: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
+000200a0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+000200b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000200c0: 2020 7363 7265 656e 4469 6374 5b66 2247    screenDict[f"G
+000200d0: 726f 7774 687b 7072 647d 225d 203d 2028  rowth{prd}"] = (
+000200e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000200f0: 2020 2020 2020 2863 6f6c 6f72 5465 7874        (colorText
+00020100: 2e47 5245 454e 2069 6620 286c 7470 5464  .GREEN if (ltpTd
+00020110: 7920 3e3d 2070 7265 764c 7470 2920 656c  y >= prevLtp) el
+00020120: 7365 2028 636f 6c6f 7254 6578 742e 4641  se (colorText.FA
+00020130: 494c 2929 0d0a 2020 2020 2020 2020 2020  IL))..          
+00020140: 2020 2020 2020 2020 2020 2b20 7374 7228            + str(
+00020150: 227b 3a2e 3266 7d22 2e66 6f72 6d61 7428  "{:.2f}".format(
+00020160: 6c74 7054 6479 202d 2070 7265 764c 7470  ltpTdy - prevLtp
+00020170: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00020180: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
+00020190: 6578 742e 454e 440d 0a20 2020 2020 2020  ext.END..       
+000201a0: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
+000201b0: 2020 2020 2020 2020 2020 2020 7361 7665              save
+000201c0: 4469 6374 5b66 224c 5450 7b70 7264 7d22  Dict[f"LTP{prd}"
+000201d0: 5d20 3d20 726f 756e 6428 6c74 7054 6479  ] = round(ltpTdy
+000201e0: 2c20 3229 0d0a 2020 2020 2020 2020 2020  , 2)..          
+000201f0: 2020 2020 2020 7361 7665 4469 6374 5b66        saveDict[f
+00020200: 2247 726f 7774 687b 7072 647d 225d 203d  "Growth{prd}"] =
+00020210: 2072 6f75 6e64 286c 7470 5464 7920 2d20   round(ltpTdy - 
+00020220: 7072 6576 4c74 702c 2032 290d 0a20 2020  prevLtp, 2)..   
+00020230: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00020240: 7072 6420 3d3d 2032 3220 6f72 2028 7072  prd == 22 or (pr
+00020250: 6420 3d3d 2072 6571 7565 7374 6564 5065  d == requestedPe
+00020260: 7269 6f64 293a 0d0a 2020 2020 2020 2020  riod):..        
+00020270: 2020 2020 2020 2020 2020 2020 6368 616e              chan
+00020280: 6765 5065 7263 656e 7420 3d20 726f 756e  gePercent = roun
+00020290: 6428 2828 7072 6576 4c74 702d 6c74 7054  d(((prevLtp-ltpT
+000202a0: 6479 2920 6966 2072 6571 7565 7374 6564  dy) if requested
+000202b0: 5065 7269 6f64 203d 3d30 2065 6c73 6520  Period ==0 else 
+000202c0: 286c 7470 5464 7920 2d20 7072 6576 4c74  (ltpTdy - prevLt
+000202d0: 7029 292a 3130 302f 6c74 7054 6479 2c20  p))*100/ltpTdy, 
+000202e0: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
+000202f0: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
+00020300: 5b66 227b 7072 647d 2d50 6420 2522 5d20  [f"{prd}-Pd %"] 
+00020310: 3d20 6622 7b63 6861 6e67 6550 6572 6365  = f"{changePerce
+00020320: 6e74 7d25 2220 6966 206e 6f74 2070 642e  nt}%" if not pd.
+00020330: 6973 6e61 2863 6861 6e67 6550 6572 6365  isna(changePerce
+00020340: 6e74 2920 656c 7365 2027 2d27 0d0a 2020  nt) else '-'..  
+00020350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020360: 2020 7363 7265 656e 4469 6374 5b66 227b    screenDict[f"{
+00020370: 7072 647d 2d50 6420 2522 5d20 3d20 2828  prd}-Pd %"] = ((
+00020380: 636f 6c6f 7254 6578 742e 4752 4545 4e20  colorText.GREEN 
+00020390: 6966 2063 6861 6e67 6550 6572 6365 6e74  if changePercent
+000203a0: 203e 3d30 2065 6c73 6520 636f 6c6f 7254   >=0 else colorT
+000203b0: 6578 742e 4641 494c 2920 2b20 6622 7b63  ext.FAIL) + f"{c
+000203c0: 6861 6e67 6550 6572 6365 6e74 7d25 2220  hangePercent}%" 
+000203d0: 2b20 636f 6c6f 7254 6578 742e 454e 4429  + colorText.END)
+000203e0: 2069 6620 6e6f 7420 7064 2e69 736e 6128   if not pd.isna(
+000203f0: 6368 616e 6765 5065 7263 656e 7429 2065  changePercent) e
+00020400: 6c73 6520 272d 270d 0a20 2020 2020 2020  lse '-'..       
+00020410: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
+00020420: 6963 745b 2244 6174 6522 5d20 3d20 6361  ict["Date"] = ca
+00020430: 6c63 5f64 6174 650d 0a20 2020 2020 2020  lc_date..       
+00020440: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
+00020450: 745b 2244 6174 6522 5d20 3d20 6361 6c63  t["Date"] = calc
+00020460: 5f64 6174 650d 0a20 2020 2020 2020 2020  _date..         
+00020470: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00020480: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
+00020490: 6374 5b66 224c 5450 7b70 7264 7d22 5d20  ct[f"LTP{prd}"] 
+000204a0: 3d20 6e70 2e6e 616e 0d0a 2020 2020 2020  = np.nan..      
+000204b0: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
+000204c0: 6374 5b66 2247 726f 7774 687b 7072 647d  ct[f"Growth{prd}
+000204d0: 225d 203d 206e 702e 6e61 6e0d 0a20 2020  "] = np.nan..   
+000204e0: 2020 2020 2020 2020 2020 2020 2073 6372               scr
+000204f0: 6565 6e44 6963 745b 2244 6174 6522 5d20  eenDict["Date"] 
+00020500: 3d20 6361 6c63 5f64 6174 650d 0a20 2020  = calc_date..   
+00020510: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+00020520: 6544 6963 745b 2244 6174 6522 5d20 3d20  eDict["Date"] = 
+00020530: 6361 6c63 5f64 6174 650d 0a0d 0a20 2020  calc_date....   
+00020540: 2023 2046 696e 6420 7374 6f63 6b73 2074   # Find stocks t
+00020550: 6861 7420 6172 6520 6265 6172 6973 6820  hat are bearish 
+00020560: 696e 7472 6164 6179 3a20 4d61 6364 2048  intraday: Macd H
+00020570: 6973 746f 6772 616d 206e 6567 6174 6976  istogram negativ
+00020580: 650d 0a20 2020 2064 6566 2076 616c 6964  e..    def valid
+00020590: 6174 654d 4143 4448 6973 746f 6772 616d  ateMACDHistogram
+000205a0: 4265 6c6f 7730 2873 656c 662c 2064 6629  Below0(self, df)
+000205b0: 3a0d 0a20 2020 2020 2020 2069 6620 6466  :..        if df
+000205c0: 2069 7320 4e6f 6e65 206f 7220 6c65 6e28   is None or len(
+000205d0: 6466 2920 3d3d 2030 3a0d 0a20 2020 2020  df) == 0:..     
+000205e0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+000205f0: 6c73 650d 0a20 2020 2020 2020 2064 6174  lse..        dat
+00020600: 6120 3d20 6466 2e63 6f70 7928 290d 0a20  a = df.copy().. 
+00020610: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
+00020620: 7461 2e66 696c 6c6e 6128 3029 0d0a 2020  ta.fillna(0)..  
+00020630: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
+00020640: 612e 7265 706c 6163 6528 5b6e 702e 696e  a.replace([np.in
+00020650: 662c 202d 6e70 2e69 6e66 5d2c 2030 290d  f, -np.inf], 0).
+00020660: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+00020670: 6461 7461 5b3a 3a2d 315d 2020 2320 5265  data[::-1]  # Re
+00020680: 7665 7273 6520 7468 6520 6461 7461 6672  verse the datafr
+00020690: 616d 6520 736f 2074 6861 7420 6974 7320  ame so that its 
+000206a0: 7468 6520 6f6c 6465 7374 2064 6174 6520  the oldest date 
+000206b0: 6669 7273 740d 0a20 2020 2020 2020 206d  first..        m
+000206c0: 6163 6420 3d20 706b 7461 6c69 622e 4d41  acd = pktalib.MA
+000206d0: 4344 2864 6174 615b 2243 6c6f 7365 225d  CD(data["Close"]
+000206e0: 2c20 3132 2c20 3236 2c20 3929 5b32 5d2e  , 12, 26, 9)[2].
+000206f0: 7461 696c 2831 290d 0a20 2020 2020 2020  tail(1)..       
+00020700: 2072 6574 7572 6e20 6d61 6364 2e69 6c6f   return macd.ilo
+00020710: 635b 3a31 5d5b 305d 203c 2030 0d0a 0d0a  c[:1][0] < 0....
+00020720: 2020 2020 2340 6d65 6173 7572 655f 7469      #@measure_ti
+00020730: 6d65 0d0a 2020 2020 2320 4669 6e64 2069  me..    # Find i
+00020740: 6620 7374 6f63 6b20 6761 696e 696e 6720  f stock gaining 
+00020750: 6275 6c6c 6973 6820 6d6f 6d65 6e74 756d  bullish momentum
+00020760: 0d0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+00020770: 7465 4d6f 6d65 6e74 756d 2873 656c 662c  teMomentum(self,
+00020780: 2064 662c 2073 6372 6565 6e44 6963 742c   df, screenDict,
+00020790: 2073 6176 6544 6963 7429 3a0d 0a20 2020   saveDict):..   
+000207a0: 2020 2020 2069 6620 6466 2069 7320 4e6f       if df is No
+000207b0: 6e65 206f 7220 6c65 6e28 6466 2920 3d3d  ne or len(df) ==
+000207c0: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
+000207d0: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
+000207e0: 2020 2020 2020 2064 6174 6120 3d20 6466         data = df
+000207f0: 2e63 6f70 7928 290d 0a20 2020 2020 2020  .copy()..       
+00020800: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
+00020810: 2020 2064 6174 6120 3d20 6461 7461 2e68     data = data.h
+00020820: 6561 6428 3329 0d0a 2020 2020 2020 2020  ead(3)..        
+00020830: 2020 2020 6966 206c 656e 2864 6174 6129      if len(data)
+00020840: 203c 2033 3a0d 0a20 2020 2020 2020 2020   < 3:..         
+00020850: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00020860: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
+00020870: 2066 6f72 2072 6f77 2069 6e20 6461 7461   for row in data
+00020880: 2e69 7465 7272 6f77 7328 293a 0d0a 2020  .iterrows():..  
+00020890: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+000208a0: 416c 6c20 3320 6361 6e64 6c65 7320 7368  All 3 candles sh
+000208b0: 6f75 6c64 2062 6520 4772 6565 6e20 616e  ould be Green an
+000208c0: 6420 4e4f 5420 4369 7263 7569 7473 0d0a  d NOT Circuits..
 000208d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000208e0: 2064 6174 612e 6571 7561 6c73 286f 7065   data.equals(ope
-000208f0: 6e44 6573 6329 0d0a 2020 2020 2020 2020  nDesc)..        
-00020900: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-00020910: 6461 7461 2e65 7175 616c 7328 636c 6f73  data.equals(clos
-00020920: 6544 6573 6329 0d0a 2020 2020 2020 2020  eDesc)..        
-00020930: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-00020940: 6461 7461 2e65 7175 616c 7328 766f 6c44  data.equals(volD
-00020950: 6573 6329 0d0a 2020 2020 2020 2020 2020  esc)..          
-00020960: 2020 2020 2020 293a 0d0a 2020 2020 2020        ):..      
+000208e0: 7963 203d 2072 6f77 5b31 5d5b 2243 6c6f  yc = row[1]["Clo
+000208f0: 7365 225d 0d0a 2020 2020 2020 2020 2020  se"]..          
+00020900: 2020 2020 2020 796f 203d 2072 6f77 5b31        yo = row[1
+00020910: 5d5b 224f 7065 6e22 5d0d 0a20 2020 2020  ]["Open"]..     
+00020920: 2020 2020 2020 2020 2020 2069 6620 7963             if yc
+00020930: 203c 3d20 796f 3a0d 0a20 2020 2020 2020   <= yo:..       
+00020940: 2020 2020 2020 2020 2020 2020 2023 2073               # s
+00020950: 656c 662e 6465 6661 756c 745f 6c6f 6767  elf.default_logg
+00020960: 6572 2e69 6e66 6f28 0d0a 2020 2020 2020  er.info(..      
 00020970: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00020980: 7365 6c66 2e64 6566 6175 6c74 5f6c 6f67  self.default_log
-00020990: 6765 722e 696e 666f 280d 0a20 2020 2020  ger.info(..     
-000209a0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-000209b0: 2020 2020 2066 2753 746f 636b 3a7b 7361       f'Stock:{sa
-000209c0: 7665 4469 6374 5b22 5374 6f63 6b22 5d7d  veDict["Stock"]}
-000209d0: 2c20 6f70 656e 2c63 6c6f 7365 2061 6e64  , open,close and
-000209e0: 2076 6f6c 756d 6520 6571 7561 6c20 6672   volume equal fr
-000209f0: 6f6d 2064 6179 2062 6566 6f72 6520 7965  om day before ye
-00020a00: 7374 6572 6461 792e 2041 2070 6f74 656e  sterday. A poten
-00020a10: 7469 616c 206d 6f6d 656e 7475 6d2d 6761  tial momentum-ga
-00020a20: 696e 6572 2127 0d0a 2020 2020 2020 2020  iner!'..        
-00020a30: 2020 2020 2020 2020 2020 2020 2320 290d              # ).
-00020a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020a50: 2020 2020 2074 6f20 3d20 6461 7461 5b22       to = data["
-00020a60: 4f70 656e 225d 2e69 6c6f 635b 305d 0d0a  Open"].iloc[0]..
-00020a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020a80: 2020 2020 7963 203d 2064 6174 615b 2243      yc = data["C
-00020a90: 6c6f 7365 225d 2e69 6c6f 635b 315d 0d0a  lose"].iloc[1]..
-00020aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020ab0: 2020 2020 796f 203d 2064 6174 615b 224f      yo = data["O
-00020ac0: 7065 6e22 5d2e 696c 6f63 5b31 5d0d 0a20  pen"].iloc[1].. 
-00020ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020ae0: 2020 2064 7963 203d 2064 6174 615b 2243     dyc = data["C
-00020af0: 6c6f 7365 225d 2e69 6c6f 635b 325d 0d0a  lose"].iloc[2]..
-00020b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020b10: 2020 2020 6966 2028 746f 203e 3d20 7963      if (to >= yc
-00020b20: 2920 616e 6420 2879 6f20 3e3d 2064 7963  ) and (yo >= dyc
-00020b30: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00020b40: 2020 2020 2020 2020 2020 2020 2320 7365              # se
-00020b50: 6c66 2e64 6566 6175 6c74 5f6c 6f67 6765  lf.default_logge
-00020b60: 722e 696e 666f 280d 0a20 2020 2020 2020  r.info(..       
-00020b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020b80: 2023 2020 2020 2066 2753 746f 636b 3a7b   #     f'Stock:{
-00020b90: 7361 7665 4469 6374 5b22 5374 6f63 6b22  saveDict["Stock"
-00020ba0: 5d7d 2c20 6973 2061 206d 6f6d 656e 7475  ]}, is a momentu
-00020bb0: 6d2d 6761 696e 6572 2062 6563 6175 7365  m-gainer because
-00020bc0: 2074 6f64 6179 2d6f 7065 6e20 287b 746f   today-open ({to
-00020bd0: 7d29 203e 3d20 7965 7374 6572 6461 792d  }) >= yesterday-
-00020be0: 636c 6f73 6520 287b 7963 7d29 2061 6e64  close ({yc}) and
-00020bf0: 2079 6573 7465 7264 6179 2d6f 7065 6e28   yesterday-open(
-00020c00: 7b79 6f7d 2920 3e3d 2064 6179 2d62 6566  {yo}) >= day-bef
-00020c10: 6f72 652d 636c 6f73 6528 7b64 7963 7d29  ore-close({dyc})
-00020c20: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
-00020c30: 2020 2020 2020 2020 2020 2023 2029 0d0a             # )..
-00020c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020c50: 2020 2020 2020 2020 7361 7665 6420 3d20          saved = 
-00020c60: 7365 6c66 2e66 696e 6443 7572 7265 6e74  self.findCurrent
-00020c70: 5361 7665 6456 616c 7565 2873 6372 6565  SavedValue(scree
-00020c80: 6e44 6963 742c 2073 6176 6544 6963 742c  nDict, saveDict,
-00020c90: 2022 5061 7474 6572 6e22 290d 0a20 2020   "Pattern")..   
-00020ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020cb0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-00020cc0: 2250 6174 7465 726e 225d 203d 2028 0d0a  "Pattern"] = (..
-00020cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020ce0: 2020 2020 2020 2020 2020 2020 7361 7665              save
-00020cf0: 645b 305d 0d0a 2020 2020 2020 2020 2020  d[0]..          
-00020d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020d10: 2020 2b20 636f 6c6f 7254 6578 742e 424f    + colorText.BO
-00020d20: 4c44 0d0a 2020 2020 2020 2020 2020 2020  LD..            
-00020d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020d40: 2b20 636f 6c6f 7254 6578 742e 4752 4545  + colorText.GREE
-00020d50: 4e0d 0a20 2020 2020 2020 2020 2020 2020  N..             
-00020d60: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-00020d70: 2022 4d6f 6d65 6e74 756d 2047 6169 6e65   "Momentum Gaine
-00020d80: 7222 0d0a 2020 2020 2020 2020 2020 2020  r"..            
-00020d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020da0: 2b20 636f 6c6f 7254 6578 742e 454e 440d  + colorText.END.
-00020db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020dc0: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
+00020980: 2020 2020 6627 5374 6f63 6b3a 7b73 6176      f'Stock:{sav
+00020990: 6544 6963 745b 2253 746f 636b 225d 7d2c  eDict["Stock"]},
+000209a0: 2069 7320 6e6f 7420 6120 6d6f 6d65 6e74   is not a moment
+000209b0: 756d 2d67 6169 6e65 7220 6265 6361 7573  um-gainer becaus
+000209c0: 6520 7965 7374 6572 6461 792d 636c 6f73  e yesterday-clos
+000209d0: 6520 287b 7963 7d29 203c 3d20 7965 7374  e ({yc}) <= yest
+000209e0: 6572 6461 792d 6f70 656e 2028 7b79 6f7d  erday-open ({yo}
+000209f0: 2927 0d0a 2020 2020 2020 2020 2020 2020  )'..            
+00020a00: 2020 2020 2020 2020 2320 290d 0a20 2020          # )..   
+00020a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020a20: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
+00020a30: 2020 2020 2020 2020 2020 206f 7065 6e44             openD
+00020a40: 6573 6320 3d20 6461 7461 2e73 6f72 745f  esc = data.sort_
+00020a50: 7661 6c75 6573 2862 793d 5b22 4f70 656e  values(by=["Open
+00020a60: 225d 2c20 6173 6365 6e64 696e 673d 4661  "], ascending=Fa
+00020a70: 6c73 6529 0d0a 2020 2020 2020 2020 2020  lse)..          
+00020a80: 2020 636c 6f73 6544 6573 6320 3d20 6461    closeDesc = da
+00020a90: 7461 2e73 6f72 745f 7661 6c75 6573 2862  ta.sort_values(b
+00020aa0: 793d 5b22 436c 6f73 6522 5d2c 2061 7363  y=["Close"], asc
+00020ab0: 656e 6469 6e67 3d46 616c 7365 290d 0a20  ending=False).. 
+00020ac0: 2020 2020 2020 2020 2020 2076 6f6c 4465             volDe
+00020ad0: 7363 203d 2064 6174 612e 736f 7274 5f76  sc = data.sort_v
+00020ae0: 616c 7565 7328 6279 3d5b 2256 6f6c 756d  alues(by=["Volum
+00020af0: 6522 5d2c 2061 7363 656e 6469 6e67 3d46  e"], ascending=F
+00020b00: 616c 7365 290d 0a20 2020 2020 2020 2020  alse)..         
+00020b10: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
+00020b20: 2020 2020 2020 2020 2069 6620 280d 0a20           if (.. 
+00020b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020b40: 2020 2064 6174 612e 6571 7561 6c73 286f     data.equals(o
+00020b50: 7065 6e44 6573 6329 0d0a 2020 2020 2020  penDesc)..      
+00020b60: 2020 2020 2020 2020 2020 2020 2020 616e                an
+00020b70: 6420 6461 7461 2e65 7175 616c 7328 636c  d data.equals(cl
+00020b80: 6f73 6544 6573 6329 0d0a 2020 2020 2020  oseDesc)..      
+00020b90: 2020 2020 2020 2020 2020 2020 2020 616e                an
+00020ba0: 6420 6461 7461 2e65 7175 616c 7328 766f  d data.equals(vo
+00020bb0: 6c44 6573 6329 0d0a 2020 2020 2020 2020  lDesc)..        
+00020bc0: 2020 2020 2020 2020 293a 0d0a 2020 2020          ):..    
+00020bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020be0: 2320 7365 6c66 2e64 6566 6175 6c74 5f6c  # self.default_l
+00020bf0: 6f67 6765 722e 696e 666f 280d 0a20 2020  ogger.info(..   
+00020c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020c10: 2023 2020 2020 2066 2753 746f 636b 3a7b   #     f'Stock:{
+00020c20: 7361 7665 4469 6374 5b22 5374 6f63 6b22  saveDict["Stock"
+00020c30: 5d7d 2c20 6f70 656e 2c63 6c6f 7365 2061  ]}, open,close a
+00020c40: 6e64 2076 6f6c 756d 6520 6571 7561 6c20  nd volume equal 
+00020c50: 6672 6f6d 2064 6179 2062 6566 6f72 6520  from day before 
+00020c60: 7965 7374 6572 6461 792e 2041 2070 6f74  yesterday. A pot
+00020c70: 656e 7469 616c 206d 6f6d 656e 7475 6d2d  ential momentum-
+00020c80: 6761 696e 6572 2127 0d0a 2020 2020 2020  gainer!'..      
+00020c90: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00020ca0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00020cb0: 2020 2020 2020 2074 6f20 3d20 6461 7461         to = data
+00020cc0: 5b22 4f70 656e 225d 2e69 6c6f 635b 305d  ["Open"].iloc[0]
+00020cd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00020ce0: 2020 2020 2020 7963 203d 2064 6174 615b        yc = data[
+00020cf0: 2243 6c6f 7365 225d 2e69 6c6f 635b 315d  "Close"].iloc[1]
+00020d00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00020d10: 2020 2020 2020 796f 203d 2064 6174 615b        yo = data[
+00020d20: 224f 7065 6e22 5d2e 696c 6f63 5b31 5d0d  "Open"].iloc[1].
+00020d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020d40: 2020 2020 2064 7963 203d 2064 6174 615b       dyc = data[
+00020d50: 2243 6c6f 7365 225d 2e69 6c6f 635b 325d  "Close"].iloc[2]
+00020d60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00020d70: 2020 2020 2020 6966 2028 746f 203e 3d20        if (to >= 
+00020d80: 7963 2920 616e 6420 2879 6f20 3e3d 2064  yc) and (yo >= d
+00020d90: 7963 293a 0d0a 2020 2020 2020 2020 2020  yc):..          
+00020da0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00020db0: 7365 6c66 2e64 6566 6175 6c74 5f6c 6f67  self.default_log
+00020dc0: 6765 722e 696e 666f 280d 0a20 2020 2020  ger.info(..     
 00020dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020de0: 2020 2020 7361 7665 4469 6374 5b22 5061      saveDict["Pa
-00020df0: 7474 6572 6e22 5d20 3d20 7361 7665 645b  ttern"] = saved[
-00020e00: 315d 202b 2022 4d6f 6d65 6e74 756d 2047  1] + "Momentum G
-00020e10: 6169 6e65 7222 0d0a 2020 2020 2020 2020  ainer"..        
-00020e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020e30: 7265 7475 726e 2054 7275 650d 0a20 2020  return True..   
-00020e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020e50: 2023 2073 656c 662e 6465 6661 756c 745f   # self.default_
-00020e60: 6c6f 6767 6572 2e69 6e66 6f28 0d0a 2020  logger.info(..  
-00020e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020e80: 2020 2320 2020 2020 6627 5374 6f63 6b3a    #     f'Stock:
-00020e90: 7b73 6176 6544 6963 745b 2253 746f 636b  {saveDict["Stock
-00020ea0: 225d 7d2c 2069 7320 6e6f 7420 6120 6d6f  "]}, is not a mo
-00020eb0: 6d65 6e74 756d 2d67 6169 6e65 7220 6265  mentum-gainer be
-00020ec0: 6361 7573 6520 6569 7468 6572 2074 6f64  cause either tod
-00020ed0: 6179 2d6f 7065 6e20 287b 746f 7d29 203c  ay-open ({to}) <
-00020ee0: 2079 6573 7465 7264 6179 2d63 6c6f 7365   yesterday-close
-00020ef0: 2028 7b79 637d 2920 6f72 2079 6573 7465   ({yc}) or yeste
-00020f00: 7264 6179 2d6f 7065 6e28 7b79 6f7d 2920  rday-open({yo}) 
-00020f10: 3c20 6461 792d 6265 666f 7265 2d63 6c6f  < day-before-clo
-00020f20: 7365 287b 6479 637d 2927 0d0a 2020 2020  se({dyc})'..    
-00020f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020f40: 2320 290d 0a20 2020 2020 2020 2020 2020  # )..           
-00020f50: 2065 7863 6570 7420 496e 6465 7845 7272   except IndexErr
-00020f60: 6f72 2061 7320 653a 2023 2070 7261 676d  or as e: # pragm
-00020f70: 613a 206e 6f20 636f 7665 720d 0a20 2020  a: no cover..   
-00020f80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00020f90: 662e 6465 6661 756c 745f 6c6f 6767 6572  f.default_logger
-00020fa0: 2e64 6562 7567 2865 2c20 6578 635f 696e  .debug(e, exc_in
-00020fb0: 666f 3d54 7275 6529 0d0a 2020 2020 2020  fo=True)..      
-00020fc0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-00020fd0: 6566 6175 6c74 5f6c 6f67 6765 722e 6465  efault_logger.de
-00020fe0: 6275 6728 6461 7461 290d 0a20 2020 2020  bug(data)..     
-00020ff0: 2020 2020 2020 2020 2020 2070 6173 730d             pass.
-00021000: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00021010: 7572 6e20 4661 6c73 650d 0a20 2020 2020  urn False..     
-00021020: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-00021030: 696f 6e20 6173 2065 3a20 2023 2070 7261  ion as e:  # pra
-00021040: 676d 613a 206e 6f20 636f 7665 720d 0a20  gma: no cover.. 
-00021050: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00021060: 6465 6661 756c 745f 6c6f 6767 6572 2e64  default_logger.d
-00021070: 6562 7567 2865 2c20 6578 635f 696e 666f  ebug(e, exc_info
-00021080: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
-00021090: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-000210a0: 0d0a 0d0a 2020 2020 2340 6d65 6173 7572  ....    #@measur
-000210b0: 655f 7469 6d65 0d0a 2020 2020 2320 5661  e_time..    # Va
-000210c0: 6c69 6461 7465 204d 6f76 696e 6720 6176  lidate Moving av
-000210d0: 6572 6167 6573 2061 6e64 206c 6f6f 6b20  erages and look 
-000210e0: 666f 7220 6275 792f 7365 6c6c 2073 6967  for buy/sell sig
-000210f0: 6e61 6c73 0d0a 2020 2020 6465 6620 7661  nals..    def va
-00021100: 6c69 6461 7465 4d6f 7669 6e67 4176 6572  lidateMovingAver
-00021110: 6167 6573 2873 656c 662c 2064 662c 2073  ages(self, df, s
-00021120: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
-00021130: 6963 742c 206d 6152 616e 6765 3d32 2e35  ict, maRange=2.5
-00021140: 293a 0d0a 2020 2020 2020 2020 6461 7461  ):..        data
-00021150: 203d 2064 662e 636f 7079 2829 0d0a 2020   = df.copy()..  
-00021160: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-00021170: 612e 6669 6c6c 6e61 2830 290d 0a20 2020  a.fillna(0)..   
-00021180: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
-00021190: 2e72 6570 6c61 6365 285b 6e70 2e69 6e66  .replace([np.inf
-000211a0: 2c20 2d6e 702e 696e 665d 2c20 3029 0d0a  , -np.inf], 0)..
-000211b0: 2020 2020 2020 2020 7265 6365 6e74 203d          recent =
-000211c0: 2064 6174 612e 6865 6164 2831 290d 0a20   data.head(1).. 
-000211d0: 2020 2020 2020 2073 6176 6564 203d 2073         saved = s
-000211e0: 656c 662e 6669 6e64 4375 7272 656e 7453  elf.findCurrentS
-000211f0: 6176 6564 5661 6c75 6528 7363 7265 656e  avedValue(screen
-00021200: 4469 6374 2c73 6176 6544 6963 742c 224d  Dict,saveDict,"M
-00021210: 412d 5369 676e 616c 2229 0d0a 2020 2020  A-Signal")..    
-00021220: 2020 2020 6966 2028 0d0a 2020 2020 2020      if (..      
-00021230: 2020 2020 2020 7265 6365 6e74 5b22 534d        recent["SM
-00021240: 4122 5d2e 696c 6f63 5b30 5d20 3e20 7265  A"].iloc[0] > re
-00021250: 6365 6e74 5b22 4c4d 4122 5d2e 696c 6f63  cent["LMA"].iloc
-00021260: 5b30 5d0d 0a20 2020 2020 2020 2020 2020  [0]..           
-00021270: 2061 6e64 2072 6563 656e 745b 2243 6c6f   and recent["Clo
-00021280: 7365 225d 2e69 6c6f 635b 305d 203e 2072  se"].iloc[0] > r
-00021290: 6563 656e 745b 2253 4d41 225d 2e69 6c6f  ecent["SMA"].ilo
-000212a0: 635b 305d 0d0a 2020 2020 2020 2020 293a  c[0]..        ):
-000212b0: 0d0a 2020 2020 2020 2020 2020 2020 7363  ..            sc
-000212c0: 7265 656e 4469 6374 5b22 4d41 2d53 6967  reenDict["MA-Sig
-000212d0: 6e61 6c22 5d20 3d20 280d 0a20 2020 2020  nal"] = (..     
-000212e0: 2020 2020 2020 2020 2020 2073 6176 6564             saved
-000212f0: 5b30 5d20 2b20 636f 6c6f 7254 6578 742e  [0] + colorText.
-00021300: 424f 4c44 202b 2063 6f6c 6f72 5465 7874  BOLD + colorText
-00021310: 2e47 5245 454e 202b 2022 4275 6c6c 6973  .GREEN + "Bullis
-00021320: 6822 202b 2063 6f6c 6f72 5465 7874 2e45  h" + colorText.E
-00021330: 4e44 0d0a 2020 2020 2020 2020 2020 2020  ND..            
-00021340: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-00021350: 6176 6544 6963 745b 224d 412d 5369 676e  aveDict["MA-Sign
-00021360: 616c 225d 203d 2073 6176 6564 5b31 5d20  al"] = saved[1] 
-00021370: 2b20 2242 756c 6c69 7368 220d 0a20 2020  + "Bullish"..   
-00021380: 2020 2020 2065 6c69 6620 7265 6365 6e74       elif recent
-00021390: 5b22 534d 4122 5d2e 696c 6f63 5b30 5d20  ["SMA"].iloc[0] 
-000213a0: 3c20 7265 6365 6e74 5b22 4c4d 4122 5d2e  < recent["LMA"].
-000213b0: 696c 6f63 5b30 5d3a 0d0a 2020 2020 2020  iloc[0]:..      
-000213c0: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
-000213d0: 5b22 4d41 2d53 6967 6e61 6c22 5d20 3d20  ["MA-Signal"] = 
-000213e0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-000213f0: 2020 2073 6176 6564 5b30 5d20 2b20 636f     saved[0] + co
-00021400: 6c6f 7254 6578 742e 424f 4c44 202b 2063  lorText.BOLD + c
-00021410: 6f6c 6f72 5465 7874 2e46 4149 4c20 2b20  olorText.FAIL + 
-00021420: 2242 6561 7269 7368 2220 2b20 636f 6c6f  "Bearish" + colo
-00021430: 7254 6578 742e 454e 440d 0a20 2020 2020  rText.END..     
-00021440: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00021450: 2020 2020 2020 7361 7665 4469 6374 5b22        saveDict["
-00021460: 4d41 2d53 6967 6e61 6c22 5d20 3d20 7361  MA-Signal"] = sa
-00021470: 7665 645b 315d 202b 2022 4265 6172 6973  ved[1] + "Bearis
-00021480: 6822 0d0a 2020 2020 2020 2020 656c 6966  h"..        elif
-00021490: 2072 6563 656e 745b 2253 4d41 225d 2e69   recent["SMA"].i
-000214a0: 6c6f 635b 305d 203d 3d20 303a 0d0a 2020  loc[0] == 0:..  
-000214b0: 2020 2020 2020 2020 2020 7363 7265 656e            screen
-000214c0: 4469 6374 5b22 4d41 2d53 6967 6e61 6c22  Dict["MA-Signal"
-000214d0: 5d20 3d20 280d 0a20 2020 2020 2020 2020  ] = (..         
-000214e0: 2020 2020 2020 2073 6176 6564 5b30 5d20         saved[0] 
-000214f0: 2b20 636f 6c6f 7254 6578 742e 424f 4c44  + colorText.BOLD
-00021500: 202b 2063 6f6c 6f72 5465 7874 2e57 4152   + colorText.WAR
-00021510: 4e20 2b20 2255 6e6b 6e6f 776e 2220 2b20  N + "Unknown" + 
-00021520: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
-00021530: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
-00021540: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
-00021550: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
-00021560: 3d20 7361 7665 645b 315d 202b 2022 556e  = saved[1] + "Un
-00021570: 6b6e 6f77 6e22 0d0a 2020 2020 2020 2020  known"..        
-00021580: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00021590: 2020 2073 6372 6565 6e44 6963 745b 224d     screenDict["M
-000215a0: 412d 5369 676e 616c 225d 203d 2028 0d0a  A-Signal"] = (..
-000215b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000215c0: 7361 7665 645b 305d 202b 2063 6f6c 6f72  saved[0] + color
-000215d0: 5465 7874 2e42 4f4c 4420 2b20 636f 6c6f  Text.BOLD + colo
-000215e0: 7254 6578 742e 5741 524e 202b 2022 4e65  rText.WARN + "Ne
-000215f0: 7574 7261 6c22 202b 2063 6f6c 6f72 5465  utral" + colorTe
-00021600: 7874 2e45 4e44 0d0a 2020 2020 2020 2020  xt.END..        
-00021610: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-00021620: 2020 2073 6176 6544 6963 745b 224d 412d     saveDict["MA-
-00021630: 5369 676e 616c 225d 203d 2073 6176 6564  Signal"] = saved
-00021640: 5b31 5d20 2b20 224e 6575 7472 616c 220d  [1] + "Neutral".
-00021650: 0a0d 0a20 2020 2020 2020 2073 6d61 4465  ...        smaDe
-00021660: 7620 3d20 6461 7461 5b22 534d 4122 5d2e  v = data["SMA"].
-00021670: 696c 6f63 5b30 5d20 2a20 6d61 5261 6e67  iloc[0] * maRang
-00021680: 6520 2f20 3130 300d 0a20 2020 2020 2020  e / 100..       
-00021690: 206c 6d61 4465 7620 3d20 6461 7461 5b22   lmaDev = data["
-000216a0: 4c4d 4122 5d2e 696c 6f63 5b30 5d20 2a20  LMA"].iloc[0] * 
-000216b0: 6d61 5261 6e67 6520 2f20 3130 300d 0a20  maRange / 100.. 
-000216c0: 2020 2020 2020 206f 7065 6e2c 2068 6967         open, hig
-000216d0: 682c 206c 6f77 2c20 636c 6f73 652c 2073  h, low, close, s
-000216e0: 6d61 2c20 6c6d 6120 3d20 280d 0a20 2020  ma, lma = (..   
-000216f0: 2020 2020 2020 2020 2064 6174 615b 224f           data["O
-00021700: 7065 6e22 5d2e 696c 6f63 5b30 5d2c 0d0a  pen"].iloc[0],..
-00021710: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00021720: 5b22 4869 6768 225d 2e69 6c6f 635b 305d  ["High"].iloc[0]
-00021730: 2c0d 0a20 2020 2020 2020 2020 2020 2064  ,..            d
-00021740: 6174 615b 224c 6f77 225d 2e69 6c6f 635b  ata["Low"].iloc[
-00021750: 305d 2c0d 0a20 2020 2020 2020 2020 2020  0],..           
-00021760: 2064 6174 615b 2243 6c6f 7365 225d 2e69   data["Close"].i
-00021770: 6c6f 635b 305d 2c0d 0a20 2020 2020 2020  loc[0],..       
-00021780: 2020 2020 2064 6174 615b 2253 4d41 225d       data["SMA"]
-00021790: 2e69 6c6f 635b 305d 2c0d 0a20 2020 2020  .iloc[0],..     
-000217a0: 2020 2020 2020 2064 6174 615b 224c 4d41         data["LMA
-000217b0: 225d 2e69 6c6f 635b 305d 2c0d 0a20 2020  "].iloc[0],..   
-000217c0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-000217d0: 6d61 5265 7665 7273 616c 203d 2030 0d0a  maReversal = 0..
-000217e0: 2020 2020 2020 2020 2320 5461 6b69 6e67          # Taking
-000217f0: 2053 7570 706f 7274 2035 300d 0a20 2020   Support 50..   
-00021800: 2020 2020 2069 6620 636c 6f73 6520 3e20       if close > 
-00021810: 736d 6120 616e 6420 6c6f 7720 3c3d 2028  sma and low <= (
-00021820: 736d 6120 2b20 736d 6144 6576 293a 0d0a  sma + smaDev):..
-00021830: 2020 2020 2020 2020 2020 2020 7363 7265              scre
-00021840: 656e 4469 6374 5b22 4d41 2d53 6967 6e61  enDict["MA-Signa
-00021850: 6c22 5d20 3d20 280d 0a20 2020 2020 2020  l"] = (..       
-00021860: 2020 2020 2020 2020 2073 6176 6564 5b30           saved[0
-00021870: 5d20 2b20 636f 6c6f 7254 6578 742e 424f  ] + colorText.BO
-00021880: 4c44 202b 2063 6f6c 6f72 5465 7874 2e47  LD + colorText.G
-00021890: 5245 454e 202b 2022 3530 4d41 2d53 7570  REEN + "50MA-Sup
-000218a0: 706f 7274 2220 2b20 636f 6c6f 7254 6578  port" + colorTex
-000218b0: 742e 454e 440d 0a20 2020 2020 2020 2020  t.END..         
-000218c0: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
-000218d0: 2020 7361 7665 4469 6374 5b22 4d41 2d53    saveDict["MA-S
-000218e0: 6967 6e61 6c22 5d20 3d20 7361 7665 645b  ignal"] = saved[
-000218f0: 315d 202b 2022 3530 4d41 2d53 7570 706f  1] + "50MA-Suppo
-00021900: 7274 220d 0a20 2020 2020 2020 2020 2020  rt"..           
-00021910: 206d 6152 6576 6572 7361 6c20 3d20 310d   maReversal = 1.
-00021920: 0a20 2020 2020 2020 2023 2056 616c 6964  .        # Valid
-00021930: 6174 696e 6720 5265 7369 7374 616e 6365  ating Resistance
-00021940: 2035 300d 0a20 2020 2020 2020 2065 6c69   50..        eli
-00021950: 6620 636c 6f73 6520 3c20 736d 6120 616e  f close < sma an
-00021960: 6420 6869 6768 203e 3d20 2873 6d61 202d  d high >= (sma -
-00021970: 2073 6d61 4465 7629 3a0d 0a20 2020 2020   smaDev):..     
-00021980: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
-00021990: 745b 224d 412d 5369 676e 616c 225d 203d  t["MA-Signal"] =
-000219a0: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-000219b0: 2020 2020 7361 7665 645b 305d 202b 2063      saved[0] + c
-000219c0: 6f6c 6f72 5465 7874 2e42 4f4c 4420 2b20  olorText.BOLD + 
-000219d0: 636f 6c6f 7254 6578 742e 4641 494c 202b  colorText.FAIL +
-000219e0: 2022 3530 4d41 2d52 6573 6973 7422 202b   "50MA-Resist" +
-000219f0: 2063 6f6c 6f72 5465 7874 2e45 4e44 0d0a   colorText.END..
-00021a00: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
-00021a10: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
-00021a20: 6963 745b 224d 412d 5369 676e 616c 225d  ict["MA-Signal"]
-00021a30: 203d 2073 6176 6564 5b31 5d20 2b20 2235   = saved[1] + "5
-00021a40: 304d 412d 5265 7369 7374 220d 0a20 2020  0MA-Resist"..   
-00021a50: 2020 2020 2020 2020 206d 6152 6576 6572           maRever
-00021a60: 7361 6c20 3d20 2d31 0d0a 2020 2020 2020  sal = -1..      
-00021a70: 2020 2320 5461 6b69 6e67 2053 7570 706f    # Taking Suppo
-00021a80: 7274 2032 3030 0d0a 2020 2020 2020 2020  rt 200..        
-00021a90: 656c 6966 2063 6c6f 7365 203e 206c 6d61  elif close > lma
-00021aa0: 2061 6e64 206c 6f77 203c 3d20 286c 6d61   and low <= (lma
-00021ab0: 202b 206c 6d61 4465 7629 3a0d 0a20 2020   + lmaDev):..   
-00021ac0: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-00021ad0: 6963 745b 224d 412d 5369 676e 616c 225d  ict["MA-Signal"]
-00021ae0: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-00021af0: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
-00021b00: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
-00021b10: 2b20 636f 6c6f 7254 6578 742e 4752 4545  + colorText.GREE
-00021b20: 4e20 2b20 2232 3030 4d41 2d53 7570 706f  N + "200MA-Suppo
-00021b30: 7274 2220 2b20 636f 6c6f 7254 6578 742e  rt" + colorText.
-00021b40: 454e 440d 0a20 2020 2020 2020 2020 2020  END..           
-00021b50: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
-00021b60: 7361 7665 4469 6374 5b22 4d41 2d53 6967  saveDict["MA-Sig
-00021b70: 6e61 6c22 5d20 3d20 7361 7665 645b 315d  nal"] = saved[1]
-00021b80: 202b 2022 3230 304d 412d 5375 7070 6f72   + "200MA-Suppor
-00021b90: 7422 0d0a 2020 2020 2020 2020 2020 2020  t"..            
-00021ba0: 6d61 5265 7665 7273 616c 203d 2031 0d0a  maReversal = 1..
-00021bb0: 2020 2020 2020 2020 2320 5661 6c69 6461          # Valida
-00021bc0: 7469 6e67 2052 6573 6973 7461 6e63 6520  ting Resistance 
-00021bd0: 3230 300d 0a20 2020 2020 2020 2065 6c69  200..        eli
-00021be0: 6620 636c 6f73 6520 3c20 6c6d 6120 616e  f close < lma an
-00021bf0: 6420 6869 6768 203e 3d20 286c 6d61 202d  d high >= (lma -
-00021c00: 206c 6d61 4465 7629 3a0d 0a20 2020 2020   lmaDev):..     
-00021c10: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
-00021c20: 745b 224d 412d 5369 676e 616c 225d 203d  t["MA-Signal"] =
-00021c30: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-00021c40: 2020 2020 7361 7665 645b 305d 202b 2063      saved[0] + c
-00021c50: 6f6c 6f72 5465 7874 2e42 4f4c 4420 2b20  olorText.BOLD + 
-00021c60: 636f 6c6f 7254 6578 742e 4641 494c 202b  colorText.FAIL +
-00021c70: 2022 3230 304d 412d 5265 7369 7374 2220   "200MA-Resist" 
-00021c80: 2b20 636f 6c6f 7254 6578 742e 454e 440d  + colorText.END.
-00021c90: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
-00021ca0: 2020 2020 2020 2020 2020 2020 7361 7665              save
-00021cb0: 4469 6374 5b22 4d41 2d53 6967 6e61 6c22  Dict["MA-Signal"
-00021cc0: 5d20 3d20 7361 7665 645b 315d 202b 2022  ] = saved[1] + "
-00021cd0: 3230 304d 412d 5265 7369 7374 220d 0a20  200MA-Resist".. 
-00021ce0: 2020 2020 2020 2020 2020 206d 6152 6576             maRev
-00021cf0: 6572 7361 6c20 3d20 2d31 0d0a 2020 2020  ersal = -1..    
-00021d00: 2020 2020 2320 466f 7220 6120 4275 6c6c      # For a Bull
-00021d10: 6973 6820 4361 6e64 6c65 0d0a 2020 2020  ish Candle..    
-00021d20: 2020 2020 6966 2073 656c 662e 6765 7443      if self.getC
-00021d30: 616e 646c 6554 7970 6528 6461 7461 293a  andleType(data):
-00021d40: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00021d50: 4372 6f73 7369 6e67 2075 7020 3530 0d0a  Crossing up 50..
-00021d60: 2020 2020 2020 2020 2020 2020 6966 206f              if o
-00021d70: 7065 6e20 3c20 736d 6120 616e 6420 636c  pen < sma and cl
-00021d80: 6f73 6520 3e20 736d 613a 0d0a 2020 2020  ose > sma:..    
-00021d90: 2020 2020 2020 2020 2020 2020 7363 7265              scre
-00021da0: 656e 4469 6374 5b22 4d41 2d53 6967 6e61  enDict["MA-Signa
-00021db0: 6c22 5d20 3d20 280d 0a20 2020 2020 2020  l"] = (..       
-00021dc0: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-00021dd0: 6564 5b30 5d20 2b20 636f 6c6f 7254 6578  ed[0] + colorTex
-00021de0: 742e 424f 4c44 202b 2063 6f6c 6f72 5465  t.BOLD + colorTe
-00021df0: 7874 2e47 5245 454e 202b 2022 4275 6c6c  xt.GREEN + "Bull
-00021e00: 4372 6f73 732d 3530 4d41 2220 2b20 636f  Cross-50MA" + co
-00021e10: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
-00021e20: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
-00021e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021e40: 7361 7665 4469 6374 5b22 4d41 2d53 6967  saveDict["MA-Sig
-00021e50: 6e61 6c22 5d20 3d20 7361 7665 645b 315d  nal"] = saved[1]
-00021e60: 202b 2022 4275 6c6c 4372 6f73 732d 3530   + "BullCross-50
-00021e70: 4d41 220d 0a20 2020 2020 2020 2020 2020  MA"..           
-00021e80: 2020 2020 206d 6152 6576 6572 7361 6c20       maReversal 
-00021e90: 3d20 310d 0a20 2020 2020 2020 2020 2020  = 1..           
-00021ea0: 2023 2043 726f 7373 696e 6720 7570 2032   # Crossing up 2
-00021eb0: 3030 0d0a 2020 2020 2020 2020 2020 2020  00..            
-00021ec0: 656c 6966 206f 7065 6e20 3c20 6c6d 6120  elif open < lma 
-00021ed0: 616e 6420 636c 6f73 6520 3e20 6c6d 613a  and close > lma:
-00021ee0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00021ef0: 2020 7363 7265 656e 4469 6374 5b22 4d41    screenDict["MA
-00021f00: 2d53 6967 6e61 6c22 5d20 3d20 280d 0a20  -Signal"] = (.. 
-00021f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021f20: 2020 2073 6176 6564 5b30 5d20 2b20 636f     saved[0] + co
-00021f30: 6c6f 7254 6578 742e 424f 4c44 202b 2063  lorText.BOLD + c
-00021f40: 6f6c 6f72 5465 7874 2e47 5245 454e 202b  olorText.GREEN +
-00021f50: 2022 4275 6c6c 4372 6f73 732d 3230 304d   "BullCross-200M
-00021f60: 4122 202b 2063 6f6c 6f72 5465 7874 2e45  A" + colorText.E
-00021f70: 4e44 0d0a 2020 2020 2020 2020 2020 2020  ND..            
-00021f80: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-00021f90: 2020 2020 2020 2073 6176 6544 6963 745b         saveDict[
-00021fa0: 224d 412d 5369 676e 616c 225d 203d 2073  "MA-Signal"] = s
-00021fb0: 6176 6564 5b31 5d20 2b20 2242 756c 6c43  aved[1] + "BullC
-00021fc0: 726f 7373 2d32 3030 4d41 220d 0a20 2020  ross-200MA"..   
-00021fd0: 2020 2020 2020 2020 2020 2020 206d 6152               maR
-00021fe0: 6576 6572 7361 6c20 3d20 310d 0a20 2020  eversal = 1..   
-00021ff0: 2020 2020 2023 2046 6f72 2061 2042 6561       # For a Bea
-00022000: 7269 7368 2043 616e 646c 650d 0a20 2020  rish Candle..   
-00022010: 2020 2020 2065 6c69 6620 6e6f 7420 7365       elif not se
-00022020: 6c66 2e67 6574 4361 6e64 6c65 5479 7065  lf.getCandleType
-00022030: 2864 6174 6129 3a0d 0a20 2020 2020 2020  (data):..       
-00022040: 2020 2020 2023 2043 726f 7373 696e 6720       # Crossing 
-00022050: 646f 776e 2035 300d 0a20 2020 2020 2020  down 50..       
-00022060: 2020 2020 2069 6620 6f70 656e 203e 2073       if open > s
-00022070: 6d61 2061 6e64 2063 6c6f 7365 203c 2073  ma and close < s
-00022080: 6d61 3a0d 0a20 2020 2020 2020 2020 2020  ma:..           
-00022090: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-000220a0: 224d 412d 5369 676e 616c 225d 203d 2028  "MA-Signal"] = (
-000220b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000220c0: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
-000220d0: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
-000220e0: 2b20 636f 6c6f 7254 6578 742e 4641 494c  + colorText.FAIL
-000220f0: 202b 2022 4265 6172 4372 6f73 732d 3530   + "BearCross-50
-00022100: 4d41 2220 2b20 636f 6c6f 7254 6578 742e  MA" + colorText.
-00022110: 454e 440d 0a20 2020 2020 2020 2020 2020  END..           
-00022120: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-00022130: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
-00022140: 5b22 4d41 2d53 6967 6e61 6c22 5d20 3d20  ["MA-Signal"] = 
-00022150: 7361 7665 645b 315d 202b 2022 4265 6172  saved[1] + "Bear
-00022160: 4372 6f73 732d 3530 4d41 220d 0a20 2020  Cross-50MA"..   
-00022170: 2020 2020 2020 2020 2020 2020 206d 6152               maR
-00022180: 6576 6572 7361 6c20 3d20 2d31 0d0a 2020  eversal = -1..  
-00022190: 2020 2020 2020 2020 2020 2320 4372 6f73            # Cros
-000221a0: 7369 6e67 2075 7020 3230 300d 0a20 2020  sing up 200..   
-000221b0: 2020 2020 2020 2020 2065 6c69 6620 6f70           elif op
-000221c0: 656e 203e 206c 6d61 2061 6e64 2063 6c6f  en > lma and clo
-000221d0: 7365 203c 206c 6d61 3a0d 0a20 2020 2020  se < lma:..     
-000221e0: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-000221f0: 6e44 6963 745b 224d 412d 5369 676e 616c  nDict["MA-Signal
-00022200: 225d 203d 2028 0d0a 2020 2020 2020 2020  "] = (..        
-00022210: 2020 2020 2020 2020 2020 2020 7361 7665              save
-00022220: 645b 305d 202b 2063 6f6c 6f72 5465 7874  d[0] + colorText
-00022230: 2e42 4f4c 4420 2b20 636f 6c6f 7254 6578  .BOLD + colorTex
-00022240: 742e 4641 494c 202b 2022 4265 6172 4372  t.FAIL + "BearCr
-00022250: 6f73 732d 3230 304d 4122 202b 2063 6f6c  oss-200MA" + col
-00022260: 6f72 5465 7874 2e45 4e44 0d0a 2020 2020  orText.END..    
-00022270: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
-00022280: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00022290: 6176 6544 6963 745b 224d 412d 5369 676e  aveDict["MA-Sign
-000222a0: 616c 225d 203d 2073 6176 6564 5b31 5d20  al"] = saved[1] 
-000222b0: 2b20 2242 6561 7243 726f 7373 2d32 3030  + "BearCross-200
-000222c0: 4d41 220d 0a20 2020 2020 2020 2020 2020  MA"..           
-000222d0: 2020 2020 206d 6152 6576 6572 7361 6c20       maReversal 
-000222e0: 3d20 2d31 0d0a 2020 2020 2020 2020 7265  = -1..        re
-000222f0: 7475 726e 206d 6152 6576 6572 7361 6c0d  turn maReversal.
-00022300: 0a0d 0a20 2020 2023 2046 696e 6420 4e52  ...    # Find NR
-00022310: 7820 7261 6e67 6520 666f 7220 5265 7665  x range for Reve
-00022320: 7273 616c 0d0a 2020 2020 6465 6620 7661  rsal..    def va
-00022330: 6c69 6461 7465 4e61 7272 6f77 5261 6e67  lidateNarrowRang
-00022340: 6528 7365 6c66 2c20 6466 2c20 7363 7265  e(self, df, scre
-00022350: 656e 4469 6374 2c20 7361 7665 4469 6374  enDict, saveDict
-00022360: 2c20 6e72 3d34 293a 0d0a 2020 2020 2020  , nr=4):..      
-00022370: 2020 6966 2064 6620 6973 204e 6f6e 6520    if df is None 
-00022380: 6f72 206c 656e 2864 6629 203d 3d20 303a  or len(df) == 0:
-00022390: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-000223a0: 7475 726e 2046 616c 7365 0d0a 2020 2020  turn False..    
-000223b0: 2020 2020 6461 7461 203d 2064 662e 636f      data = df.co
-000223c0: 7079 2829 0d0a 2020 2020 2020 2020 7361  py()..        sa
-000223d0: 7665 6420 3d20 7365 6c66 2e66 696e 6443  ved = self.findC
-000223e0: 7572 7265 6e74 5361 7665 6456 616c 7565  urrentSavedValue
-000223f0: 2873 6372 6565 6e44 6963 742c 2073 6176  (screenDict, sav
-00022400: 6544 6963 742c 2022 5061 7474 6572 6e22  eDict, "Pattern"
-00022410: 290d 0a20 2020 2020 2020 2069 6620 504b  )..        if PK
-00022420: 4461 7465 5574 696c 6974 6965 732e 6973  DateUtilities.is
-00022430: 5472 6164 696e 6754 696d 6528 293a 0d0a  TradingTime():..
-00022440: 2020 2020 2020 2020 2020 2020 7261 6e67              rang
-00022450: 6544 6174 6120 3d20 6461 7461 2e68 6561  eData = data.hea
-00022460: 6428 6e72 202b 2031 295b 313a 5d0d 0a20  d(nr + 1)[1:].. 
-00022470: 2020 2020 2020 2020 2020 206e 6f77 5f63             now_c
-00022480: 616e 646c 6520 3d20 6461 7461 2e68 6561  andle = data.hea
-00022490: 6428 3129 0d0a 2020 2020 2020 2020 2020  d(1)..          
-000224a0: 2020 7261 6e67 6544 6174 615b 2252 616e    rangeData["Ran
-000224b0: 6765 225d 203d 2061 6273 2872 616e 6765  ge"] = abs(range
-000224c0: 4461 7461 5b22 436c 6f73 6522 5d20 2d20  Data["Close"] - 
-000224d0: 7261 6e67 6544 6174 615b 224f 7065 6e22  rangeData["Open"
-000224e0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-000224f0: 7265 6365 6e74 203d 2072 616e 6765 4461  recent = rangeDa
-00022500: 7461 2e68 6561 6428 3129 0d0a 2020 2020  ta.head(1)..    
-00022510: 2020 2020 2020 2020 6966 2028 0d0a 2020          if (..  
-00022520: 2020 2020 2020 2020 2020 2020 2020 6c65                le
-00022530: 6e28 7265 6365 6e74 2920 3d3d 2031 0d0a  n(recent) == 1..
-00022540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022550: 616e 6420 7265 6365 6e74 5b22 5261 6e67  and recent["Rang
-00022560: 6522 5d2e 696c 6f63 5b30 5d20 3d3d 2072  e"].iloc[0] == r
-00022570: 616e 6765 4461 7461 2e64 6573 6372 6962  angeData.describ
-00022580: 6528 295b 2252 616e 6765 225d 5b22 6d69  e()["Range"]["mi
-00022590: 6e22 5d0d 0a20 2020 2020 2020 2020 2020  n"]..           
-000225a0: 2029 3a0d 0a20 2020 2020 2020 2020 2020   ):..           
-000225b0: 2020 2020 2069 6620 280d 0a20 2020 2020       if (..     
-000225c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000225d0: 656c 662e 6765 7443 616e 646c 6554 7970  elf.getCandleTyp
-000225e0: 6528 7265 6365 6e74 290d 0a20 2020 2020  e(recent)..     
-000225f0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00022600: 6e64 206e 6f77 5f63 616e 646c 655b 2243  nd now_candle["C
-00022610: 6c6f 7365 225d 2e69 6c6f 635b 305d 203e  lose"].iloc[0] >
-00022620: 3d20 7265 6365 6e74 5b22 436c 6f73 6522  = recent["Close"
-00022630: 5d2e 696c 6f63 5b30 5d0d 0a20 2020 2020  ].iloc[0]..     
-00022640: 2020 2020 2020 2020 2020 2029 3a0d 0a20             ):.. 
-00022650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022660: 2020 2073 6372 6565 6e44 6963 745b 2250     screenDict["P
-00022670: 6174 7465 726e 225d 203d 2028 0d0a 2020  attern"] = (..  
-00022680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022690: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
-000226a0: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
-000226b0: 2b20 636f 6c6f 7254 6578 742e 4752 4545  + colorText.GREE
-000226c0: 4e20 2b20 6622 4275 792d 4e52 7b6e 727d  N + f"Buy-NR{nr}
-000226d0: 2220 2b20 636f 6c6f 7254 6578 742e 454e  " + colorText.EN
-000226e0: 440d 0a20 2020 2020 2020 2020 2020 2020  D..             
-000226f0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00022700: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-00022710: 7665 4469 6374 5b22 5061 7474 6572 6e22  veDict["Pattern"
-00022720: 5d20 3d20 7361 7665 645b 315d 202b 2066  ] = saved[1] + f
-00022730: 2242 7579 2d4e 527b 6e72 7d22 0d0a 2020  "Buy-NR{nr}"..  
-00022740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022750: 2020 7265 7475 726e 2054 7275 650d 0a20    return True.. 
-00022760: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00022770: 6c69 6620 280d 0a20 2020 2020 2020 2020  lif (..         
-00022780: 2020 2020 2020 2020 2020 206e 6f74 2073             not s
-00022790: 656c 662e 6765 7443 616e 646c 6554 7970  elf.getCandleTyp
-000227a0: 6528 7265 6365 6e74 290d 0a20 2020 2020  e(recent)..     
-000227b0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000227c0: 6e64 206e 6f77 5f63 616e 646c 655b 2243  nd now_candle["C
-000227d0: 6c6f 7365 225d 2e69 6c6f 635b 305d 203c  lose"].iloc[0] <
-000227e0: 3d20 7265 6365 6e74 5b22 436c 6f73 6522  = recent["Close"
-000227f0: 5d2e 696c 6f63 5b30 5d0d 0a20 2020 2020  ].iloc[0]..     
-00022800: 2020 2020 2020 2020 2020 2029 3a0d 0a20             ):.. 
-00022810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022820: 2020 2073 6372 6565 6e44 6963 745b 2250     screenDict["P
-00022830: 6174 7465 726e 225d 203d 2028 0d0a 2020  attern"] = (..  
-00022840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022850: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
-00022860: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
-00022870: 2b20 636f 6c6f 7254 6578 742e 4641 494c  + colorText.FAIL
-00022880: 202b 2066 2253 656c 6c2d 4e52 7b6e 727d   + f"Sell-NR{nr}
-00022890: 2220 2b20 636f 6c6f 7254 6578 742e 454e  " + colorText.EN
-000228a0: 440d 0a20 2020 2020 2020 2020 2020 2020  D..             
-000228b0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-000228c0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-000228d0: 7665 4469 6374 5b22 5061 7474 6572 6e22  veDict["Pattern"
-000228e0: 5d20 3d20 7361 7665 645b 315d 202b 2066  ] = saved[1] + f
-000228f0: 2253 656c 6c2d 4e52 7b6e 727d 220d 0a20  "Sell-NR{nr}".. 
-00022900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022910: 2020 2072 6574 7572 6e20 5472 7565 0d0a     return True..
-00022920: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00022930: 726e 2046 616c 7365 0d0a 2020 2020 2020  rn False..      
-00022940: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00022950: 2020 2020 2072 616e 6765 4461 7461 203d       rangeData =
-00022960: 2064 6174 612e 6865 6164 286e 7229 0d0a   data.head(nr)..
-00022970: 2020 2020 2020 2020 2020 2020 7261 6e67              rang
-00022980: 6544 6174 612e 6c6f 635b 3a2c 2752 616e  eData.loc[:,'Ran
-00022990: 6765 275d 203d 2061 6273 2872 616e 6765  ge'] = abs(range
-000229a0: 4461 7461 5b22 436c 6f73 6522 5d20 2d20  Data["Close"] - 
-000229b0: 7261 6e67 6544 6174 615b 224f 7065 6e22  rangeData["Open"
-000229c0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-000229d0: 7265 6365 6e74 203d 2072 616e 6765 4461  recent = rangeDa
-000229e0: 7461 2e68 6561 6428 3129 0d0a 2020 2020  ta.head(1)..    
-000229f0: 2020 2020 2020 2020 6966 2072 6563 656e          if recen
-00022a00: 745b 2252 616e 6765 225d 2e69 6c6f 635b  t["Range"].iloc[
-00022a10: 305d 203d 3d20 7261 6e67 6544 6174 612e  0] == rangeData.
-00022a20: 6465 7363 7269 6265 2829 5b22 5261 6e67  describe()["Rang
-00022a30: 6522 5d5b 226d 696e 225d 3a0d 0a20 2020  e"]["min"]:..   
-00022a40: 2020 2020 2020 2020 2020 2020 2073 6372               scr
-00022a50: 6565 6e44 6963 745b 2250 6174 7465 726e  eenDict["Pattern
-00022a60: 225d 203d 2028 0d0a 2020 2020 2020 2020  "] = (..        
-00022a70: 2020 2020 2020 2020 2020 2020 7361 7665              save
-00022a80: 645b 305d 202b 2063 6f6c 6f72 5465 7874  d[0] + colorText
-00022a90: 2e42 4f4c 4420 2b20 636f 6c6f 7254 6578  .BOLD + colorTex
-00022aa0: 742e 4752 4545 4e20 2b20 6622 4e52 7b6e  t.GREEN + f"NR{n
-00022ab0: 727d 2220 2b20 636f 6c6f 7254 6578 742e  r}" + colorText.
-00022ac0: 454e 440d 0a20 2020 2020 2020 2020 2020  END..           
-00022ad0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-00022ae0: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
-00022af0: 5b22 5061 7474 6572 6e22 5d20 3d20 7361  ["Pattern"] = sa
-00022b00: 7665 645b 315d 202b 2066 224e 527b 6e72  ved[1] + f"NR{nr
-00022b10: 7d22 0d0a 2020 2020 2020 2020 2020 2020  }"..            
-00022b20: 2020 2020 7265 7475 726e 2054 7275 650d      return True.
-00022b30: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00022b40: 7572 6e20 4661 6c73 650d 0a0d 0a20 2020  urn False....   
-00022b50: 2023 2046 696e 6420 6966 2073 746f 636b   # Find if stock
-00022b60: 2069 7320 6e65 776c 7920 6c69 7374 6564   is newly listed
-00022b70: 0d0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-00022b80: 7465 4e65 776c 794c 6973 7465 6428 7365  teNewlyListed(se
-00022b90: 6c66 2c20 6466 2c20 6461 7973 546f 4c6f  lf, df, daysToLo
-00022ba0: 6f6b 6261 636b 293a 0d0a 2020 2020 2020  okback):..      
-00022bb0: 2020 6966 2064 6620 6973 204e 6f6e 6520    if df is None 
-00022bc0: 6f72 206c 656e 2864 6629 203d 3d20 303a  or len(df) == 0:
-00022bd0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00022be0: 7475 726e 2046 616c 7365 0d0a 2020 2020  turn False..    
-00022bf0: 2020 2020 6461 7461 203d 2064 662e 636f      data = df.co
-00022c00: 7079 2829 0d0a 2020 2020 2020 2020 6461  py()..        da
-00022c10: 7973 546f 4c6f 6f6b 6261 636b 203d 2069  ysToLookback = i
-00022c20: 6e74 2864 6179 7354 6f4c 6f6f 6b62 6163  nt(daysToLookbac
-00022c30: 6b5b 3a2d 315d 290d 0a20 2020 2020 2020  k[:-1])..       
-00022c40: 2072 6563 656e 7420 3d20 6461 7461 2e68   recent = data.h
-00022c50: 6561 6428 3129 0d0a 2020 2020 2020 2020  ead(1)..        
-00022c60: 6966 206c 656e 2872 6563 656e 7429 203c  if len(recent) <
-00022c70: 2031 3a0d 0a20 2020 2020 2020 2020 2020   1:..           
-00022c80: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
-00022c90: 2020 2020 2020 2069 6620 6c65 6e28 6461         if len(da
-00022ca0: 7461 2920 3c20 6461 7973 546f 4c6f 6f6b  ta) < daysToLook
-00022cb0: 6261 636b 2061 6e64 2028 0d0a 2020 2020  back and (..    
-00022cc0: 2020 2020 2020 2020 7265 6365 6e74 5b22          recent["
-00022cd0: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d20  Close"].iloc[0] 
-00022ce0: 213d 206e 702e 6e61 6e20 616e 6420 7265  != np.nan and re
-00022cf0: 6365 6e74 5b22 436c 6f73 6522 5d2e 696c  cent["Close"].il
-00022d00: 6f63 5b30 5d20 3e20 300d 0a20 2020 2020  oc[0] > 0..     
-00022d10: 2020 2029 3a0d 0a20 2020 2020 2020 2020     ):..         
-00022d20: 2020 2072 6574 7572 6e20 5472 7565 0d0a     return True..
-00022d30: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00022d40: 616c 7365 0d0a 0d0a 2020 2020 2320 5661  alse....    # Va
-00022d50: 6c69 6461 7465 2069 6620 7468 6520 7374  lidate if the st
-00022d60: 6f63 6b20 7072 6963 6573 2061 7265 2061  ock prices are a
-00022d70: 7420 6c65 6173 7420 7269 7369 6e67 2062  t least rising b
-00022d80: 7920 3225 2066 6f72 2074 6865 206c 6173  y 2% for the las
-00022d90: 7420 3320 7365 7373 696f 6e73 0d0a 2020  t 3 sessions..  
-00022da0: 2020 6465 6620 7661 6c69 6461 7465 5072    def validatePr
-00022db0: 6963 6552 6973 696e 6742 7941 744c 6561  iceRisingByAtLea
-00022dc0: 7374 3250 6572 6365 6e74 2873 656c 662c  st2Percent(self,
-00022dd0: 2064 662c 2073 6372 6565 6e44 6963 742c   df, screenDict,
-00022de0: 2073 6176 6544 6963 7429 3a0d 0a20 2020   saveDict):..   
-00022df0: 2020 2020 2069 6620 6466 2069 7320 4e6f       if df is No
-00022e00: 6e65 206f 7220 6c65 6e28 6466 2920 3d3d  ne or len(df) ==
-00022e10: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
-00022e20: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
-00022e30: 2020 2020 2020 2064 6174 6120 3d20 6466         data = df
-00022e40: 2e63 6f70 7928 290d 0a20 2020 2020 2020  .copy()..       
-00022e50: 2064 6174 6120 3d20 6461 7461 2e66 696c   data = data.fil
-00022e60: 6c6e 6128 3029 0d0a 2020 2020 2020 2020  lna(0)..        
-00022e70: 6461 7461 203d 2064 6174 612e 7265 706c  data = data.repl
-00022e80: 6163 6528 5b6e 702e 696e 662c 202d 6e70  ace([np.inf, -np
-00022e90: 2e69 6e66 5d2c 2030 290d 0a20 2020 2020  .inf], 0)..     
-00022ea0: 2020 2064 6174 6120 3d20 6461 7461 2e68     data = data.h
-00022eb0: 6561 6428 3429 0d0a 2020 2020 2020 2020  ead(4)..        
-00022ec0: 6966 206c 656e 2864 6174 6129 203c 2034  if len(data) < 4
-00022ed0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00022ee0: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
-00022ef0: 2020 2020 2064 6179 3020 3d20 6461 7461       day0 = data
-00022f00: 2e69 6c6f 635b 305d 5b22 436c 6f73 6522  .iloc[0]["Close"
-00022f10: 5d2e 6974 656d 2829 0d0a 2020 2020 2020  ].item()..      
-00022f20: 2020 6461 794d 696e 7573 3120 3d20 6461    dayMinus1 = da
-00022f30: 7461 2e69 6c6f 635b 315d 5b22 436c 6f73  ta.iloc[1]["Clos
-00022f40: 6522 5d2e 6974 656d 2829 0d0a 2020 2020  e"].item()..    
-00022f50: 2020 2020 6461 794d 696e 7573 3220 3d20      dayMinus2 = 
-00022f60: 6461 7461 2e69 6c6f 635b 325d 5b22 436c  data.iloc[2]["Cl
-00022f70: 6f73 6522 5d2e 6974 656d 2829 0d0a 2020  ose"].item()..  
-00022f80: 2020 2020 2020 6461 794d 696e 7573 3320        dayMinus3 
-00022f90: 3d20 6461 7461 2e69 6c6f 635b 335d 5b22  = data.iloc[3]["
-00022fa0: 436c 6f73 6522 5d2e 6974 656d 2829 0d0a  Close"].item()..
-00022fb0: 2020 2020 2020 2020 7065 7263 656e 7433          percent3
-00022fc0: 203d 2072 6f75 6e64 2828 6461 794d 696e   = round((dayMin
-00022fd0: 7573 3220 2d20 6461 794d 696e 7573 3329  us2 - dayMinus3)
-00022fe0: 202a 2031 3030 202f 2064 6179 4d69 6e75   * 100 / dayMinu
-00022ff0: 7333 2c20 3229 0d0a 2020 2020 2020 2020  s3, 2)..        
-00023000: 7065 7263 656e 7432 203d 2072 6f75 6e64  percent2 = round
-00023010: 2828 6461 794d 696e 7573 3120 2d20 6461  ((dayMinus1 - da
-00023020: 794d 696e 7573 3229 202a 2031 3030 202f  yMinus2) * 100 /
-00023030: 2064 6179 4d69 6e75 7332 2c20 3229 0d0a   dayMinus2, 2)..
-00023040: 2020 2020 2020 2020 7065 7263 656e 7431          percent1
-00023050: 203d 2072 6f75 6e64 2828 6461 7930 202d   = round((day0 -
-00023060: 2064 6179 4d69 6e75 7331 2920 2a20 3130   dayMinus1) * 10
-00023070: 3020 2f20 6461 794d 696e 7573 312c 2032  0 / dayMinus1, 2
-00023080: 290d 0a0d 0a20 2020 2020 2020 2069 6620  )....        if 
-00023090: 7065 7263 656e 7431 203e 3d20 3220 616e  percent1 >= 2 an
-000230a0: 6420 7065 7263 656e 7432 203e 3d20 3220  d percent2 >= 2 
-000230b0: 616e 6420 7065 7263 656e 7433 203e 3d20  and percent3 >= 
-000230c0: 323a 0d0a 2020 2020 2020 2020 2020 2020  2:..            
-000230d0: 7063 745f 6368 616e 6765 5f74 6578 7420  pct_change_text 
-000230e0: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
-000230f0: 2020 2020 2028 2225 2e31 6625 2522 2025       ("%.1f%%" %
-00023100: 2070 6572 6365 6e74 3129 0d0a 2020 2020   percent1)..    
-00023110: 2020 2020 2020 2020 2020 2020 2b20 2822              + ("
-00023120: 2028 252e 3166 2525 2c22 2025 2070 6572   (%.1f%%," % per
-00023130: 6365 6e74 3229 0d0a 2020 2020 2020 2020  cent2)..        
-00023140: 2020 2020 2020 2020 2b20 2822 2025 2e31          + (" %.1
-00023150: 6625 2529 2220 2520 7065 7263 656e 7433  f%%)" % percent3
-00023160: 290d 0a20 2020 2020 2020 2020 2020 2029  )..            )
-00023170: 0d0a 2020 2020 2020 2020 2020 2020 7361  ..            sa
-00023180: 7665 4469 6374 5b22 2543 686e 6722 5d20  veDict["%Chng"] 
-00023190: 3d20 7063 745f 6368 616e 6765 5f74 6578  = pct_change_tex
-000231a0: 740d 0a20 2020 2020 2020 2020 2020 2073  t..            s
-000231b0: 6372 6565 6e44 6963 745b 2225 4368 6e67  creenDict["%Chng
-000231c0: 225d 203d 2063 6f6c 6f72 5465 7874 2e47  "] = colorText.G
-000231d0: 5245 454e 202b 2070 6374 5f63 6861 6e67  REEN + pct_chang
-000231e0: 655f 7465 7874 202b 2063 6f6c 6f72 5465  e_text + colorTe
-000231f0: 7874 2e45 4e44 0d0a 2020 2020 2020 2020  xt.END..        
-00023200: 2020 2020 7265 7475 726e 2054 7275 6520      return True 
-00023210: 616e 6420 7365 6c66 2e67 6574 4361 6e64  and self.getCand
-00023220: 6c65 5479 7065 2864 6174 612e 6865 6164  leType(data.head
-00023230: 2831 2929 0d0a 2020 2020 2020 2020 7265  (1))..        re
-00023240: 7475 726e 2046 616c 7365 0d0a 0d0a 2020  turn False....  
-00023250: 2020 2340 6d65 6173 7572 655f 7469 6d65    #@measure_time
-00023260: 0d0a 2020 2020 2320 7661 6c69 6461 7465  ..    # validate
-00023270: 2069 6620 5253 4920 6973 2077 6974 6869   if RSI is withi
-00023280: 6e20 6769 7665 6e20 7261 6e67 650d 0a20  n given range.. 
-00023290: 2020 2064 6566 2076 616c 6964 6174 6552     def validateR
-000232a0: 5349 2873 656c 662c 2064 662c 2073 6372  SI(self, df, scr
-000232b0: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
-000232c0: 742c 206d 696e 5253 492c 206d 6178 5253  t, minRSI, maxRS
-000232d0: 492c 7273 694b 6579 3d22 5253 4922 293a  I,rsiKey="RSI"):
-000232e0: 0d0a 2020 2020 2020 2020 6966 2064 6620  ..        if df 
-000232f0: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
-00023300: 6629 203d 3d20 303a 0d0a 2020 2020 2020  f) == 0:..      
-00023310: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00023320: 7365 0d0a 2020 2020 2020 2020 6966 2072  se..        if r
-00023330: 7369 4b65 7920 6e6f 7420 696e 2064 662e  siKey not in df.
-00023340: 636f 6c75 6d6e 733a 0d0a 2020 2020 2020  columns:..      
-00023350: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00023360: 7365 0d0a 2020 2020 2020 2020 6461 7461  se..        data
-00023370: 203d 2064 662e 636f 7079 2829 0d0a 2020   = df.copy()..  
-00023380: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-00023390: 612e 6669 6c6c 6e61 2830 290d 0a20 2020  a.fillna(0)..   
-000233a0: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
-000233b0: 2e72 6570 6c61 6365 285b 6e70 2e69 6e66  .replace([np.inf
-000233c0: 2c20 2d6e 702e 696e 665d 2c20 3029 0d0a  , -np.inf], 0)..
-000233d0: 2020 2020 2020 2020 7273 6920 3d20 696e          rsi = in
-000233e0: 7428 6461 7461 2e68 6561 6428 3129 5b72  t(data.head(1)[r
-000233f0: 7369 4b65 795d 2e69 6c6f 635b 305d 290d  siKey].iloc[0]).
-00023400: 0a20 2020 2020 2020 2073 6176 6544 6963  .        saveDic
-00023410: 745b 7273 694b 6579 5d20 3d20 7273 690d  t[rsiKey] = rsi.
-00023420: 0a20 2020 2020 2020 2023 2068 7474 7073  .        # https
-00023430: 3a2f 2f63 6861 7274 696e 6b2e 636f 6d2f  ://chartink.com/
-00023440: 7363 7265 656e 6572 2f72 7369 2d73 6372  screener/rsi-scr
-00023450: 6565 6e69 6e67 0d0a 2020 2020 2020 2020  eening..        
-00023460: 6966 2072 7369 3e20 3020 616e 6420 7273  if rsi> 0 and rs
-00023470: 6920 3e3d 206d 696e 5253 4920 616e 6420  i >= minRSI and 
-00023480: 7273 6920 3c3d 206d 6178 5253 493a 2020  rsi <= maxRSI:  
-00023490: 2320 6f72 2028 7273 6920 3c3d 2037 3120  # or (rsi <= 71 
-000234a0: 616e 6420 7273 6920 3e3d 2036 3729 3a0d  and rsi >= 67):.
-000234b0: 0a20 2020 2020 2020 2020 2020 2073 6372  .            scr
-000234c0: 6565 6e44 6963 745b 7273 694b 6579 5d20  eenDict[rsiKey] 
-000234d0: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
-000234e0: 2020 2020 2063 6f6c 6f72 5465 7874 2e42       colorText.B
-000234f0: 4f4c 4420 2b20 636f 6c6f 7254 6578 742e  OLD + colorText.
-00023500: 4752 4545 4e20 2b20 7374 7228 7273 6929  GREEN + str(rsi)
-00023510: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
-00023520: 0d0a 2020 2020 2020 2020 2020 2020 290d  ..            ).
-00023530: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00023540: 7572 6e20 5472 7565 2069 6620 2872 7369  urn True if (rsi
-00023550: 4b65 7920 3d3d 2022 5253 4969 2229 2065  Key == "RSIi") e
-00023560: 6c73 6520 2873 656c 662e 7661 6c69 6461  lse (self.valida
-00023570: 7465 5253 4928 6466 2c20 7363 7265 656e  teRSI(df, screen
-00023580: 4469 6374 2c20 7361 7665 4469 6374 2c20  Dict, saveDict, 
-00023590: 6d69 6e52 5349 2c20 6d61 7852 5349 2c72  minRSI, maxRSI,r
-000235a0: 7369 4b65 793d 2252 5349 6922 2920 6f72  siKey="RSIi") or
-000235b0: 2054 7275 6529 0d0a 2020 2020 2020 2020   True)..        
-000235c0: 7363 7265 656e 4469 6374 5b72 7369 4b65  screenDict[rsiKe
-000235d0: 795d 203d 2063 6f6c 6f72 5465 7874 2e42  y] = colorText.B
-000235e0: 4f4c 4420 2b20 636f 6c6f 7254 6578 742e  OLD + colorText.
-000235f0: 4641 494c 202b 2073 7472 2872 7369 2920  FAIL + str(rsi) 
-00023600: 2b20 636f 6c6f 7254 6578 742e 454e 440d  + colorText.END.
-00023610: 0a20 2020 2020 2020 2023 2049 6620 6569  .        # If ei
-00023620: 7468 6572 2064 6169 6c79 206f 7220 696e  ther daily or in
-00023630: 7472 6164 6179 2052 5349 2063 6f6d 6573  traday RSI comes
-00023640: 2077 6974 6869 6e20 7261 6e67 653f 0d0a   within range?..
-00023650: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00023660: 616c 7365 2069 6620 2872 7369 4b65 7920  alse if (rsiKey 
-00023670: 3d3d 2022 5253 4969 2229 2065 6c73 6520  == "RSIi") else 
-00023680: 2873 656c 662e 7661 6c69 6461 7465 5253  (self.validateRS
-00023690: 4928 6466 2c20 7363 7265 656e 4469 6374  I(df, screenDict
-000236a0: 2c20 7361 7665 4469 6374 2c20 6d69 6e52  , saveDict, minR
-000236b0: 5349 2c20 6d61 7852 5349 2c72 7369 4b65  SI, maxRSI,rsiKe
-000236c0: 793d 2252 5349 6922 2929 0d0a 0d0a 2020  y="RSIi"))....  
-000236d0: 2020 2320 5661 6c69 6461 7465 2069 6620    # Validate if 
-000236e0: 7468 6520 7374 6f63 6b20 6973 2062 756c  the stock is bul
-000236f0: 6c69 7368 2069 6e20 7468 6520 7368 6f72  lish in the shor
-00023700: 7420 7465 726d 0d0a 2020 2020 6465 6620  t term..    def 
-00023710: 7661 6c69 6461 7465 5368 6f72 7454 6572  validateShortTer
-00023720: 6d42 756c 6c69 7368 2873 656c 662c 2064  mBullish(self, d
-00023730: 662c 2073 6372 6565 6e44 6963 742c 2073  f, screenDict, s
-00023740: 6176 6544 6963 7429 3a0d 0a20 2020 2020  aveDict):..     
-00023750: 2020 2069 6620 6466 2069 7320 4e6f 6e65     if df is None
-00023760: 206f 7220 6c65 6e28 6466 2920 3d3d 2030   or len(df) == 0
-00023770: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00023780: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
-00023790: 2020 2020 2064 6174 6120 3d20 6466 2e63       data = df.c
-000237a0: 6f70 7928 290d 0a20 2020 2020 2020 2023  opy()..        #
-000237b0: 2068 7474 7073 3a2f 2f63 6861 7274 696e   https://chartin
-000237c0: 6b2e 636f 6d2f 7363 7265 656e 6572 2f73  k.com/screener/s
-000237d0: 686f 7274 2d74 6572 6d2d 6275 6c6c 6973  hort-term-bullis
-000237e0: 680d 0a20 2020 2020 2020 2064 6174 6120  h..        data 
-000237f0: 3d20 6461 7461 2e66 696c 6c6e 6128 3029  = data.fillna(0)
-00023800: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
-00023810: 2064 6174 612e 7265 706c 6163 6528 5b6e   data.replace([n
-00023820: 702e 696e 662c 202d 6e70 2e69 6e66 5d2c  p.inf, -np.inf],
-00023830: 2030 290d 0a20 2020 2020 2020 2072 6563   0)..        rec
-00023840: 656e 7420 3d20 6461 7461 2e68 6561 6428  ent = data.head(
-00023850: 3129 0d0a 2020 2020 2020 2020 666b 203d  1)..        fk =
-00023860: 2030 2069 6620 6c65 6e28 6461 7461 2920   0 if len(data) 
-00023870: 3c20 3320 656c 7365 206e 702e 726f 756e  < 3 else np.roun
-00023880: 6428 6461 7461 5b22 4641 5354 4b22 5d2e  d(data["FASTK"].
-00023890: 696c 6f63 5b32 5d2c 2035 290d 0a20 2020  iloc[2], 5)..   
-000238a0: 2020 2020 2023 2052 6576 6572 7365 2074       # Reverse t
-000238b0: 6865 2064 6174 6166 7261 6d65 2066 6f72  he dataframe for
-000238c0: 2069 6368 696d 6f6b 7520 6361 6c63 756c   ichimoku calcul
-000238d0: 6174 696f 6e73 2077 6974 6820 6461 7465  ations with date
-000238e0: 2069 6e20 6173 6365 6e64 696e 6720 6f72   in ascending or
-000238f0: 6465 720d 0a20 2020 2020 2020 2064 665f  der..        df_
-00023900: 6e65 7720 3d20 6461 7461 5b3a 3a2d 315d  new = data[::-1]
-00023910: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
-00023920: 2020 2020 2020 2020 2020 2020 6466 5f69              df_i
-00023930: 6368 6920 3d20 6466 5f6e 6577 2e72 656e  chi = df_new.ren
-00023940: 616d 6528 0d0a 2020 2020 2020 2020 2020  ame(..          
-00023950: 2020 2020 2020 636f 6c75 6d6e 733d 7b0d        columns={.
-00023960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00023970: 2020 2020 2022 4f70 656e 223a 2022 6f70       "Open": "op
-00023980: 656e 222c 0d0a 2020 2020 2020 2020 2020  en",..          
-00023990: 2020 2020 2020 2020 2020 2248 6967 6822            "High"
-000239a0: 3a20 2268 6967 6822 2c0d 0a20 2020 2020  : "high",..     
-000239b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000239c0: 4c6f 7722 3a20 226c 6f77 222c 0d0a 2020  Low": "low",..  
-000239d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000239e0: 2020 2243 6c6f 7365 223a 2022 636c 6f73    "Close": "clos
-000239f0: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
-00023a00: 2020 2020 2020 2020 2022 566f 6c75 6d65           "Volume
-00023a10: 223a 2022 766f 6c75 6d65 222c 0d0a 2020  ": "volume",..  
-00023a20: 2020 2020 2020 2020 2020 2020 2020 7d0d                }.
-00023a30: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
-00023a40: 2020 2020 2020 2020 2020 2020 6963 6869              ichi
-00023a50: 203d 2070 6b74 616c 6962 2e69 6368 696d   = pktalib.ichim
-00023a60: 6f6b 7528 6466 5f69 6368 692c 2039 2c20  oku(df_ichi, 9, 
-00023a70: 3236 2c20 3532 2c20 3236 290d 0a20 2020  26, 52, 26)..   
-00023a80: 2020 2020 2020 2020 2069 6620 6963 6869           if ichi
-00023a90: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
-00023aa0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00023ab0: 6e20 4661 6c73 650d 0a20 2020 2020 2020  n False..       
-00023ac0: 2020 2020 2064 665f 6e65 7720 3d20 7064       df_new = pd
-00023ad0: 2e63 6f6e 6361 7428 5b64 665f 6e65 772c  .concat([df_new,
-00023ae0: 2069 6368 695d 2c20 6178 6973 3d31 290d   ichi], axis=1).
-00023af0: 0a20 2020 2020 2020 2020 2020 2023 2052  .            # R
-00023b00: 6576 6572 7365 2061 6761 696e 2074 6f20  everse again to 
-00023b10: 6765 7420 7468 6520 6d6f 7374 2072 6563  get the most rec
-00023b20: 656e 7420 6461 7465 206f 6e20 746f 700d  ent date on top.
-00023b30: 0a20 2020 2020 2020 2020 2020 2064 665f  .            df_
-00023b40: 6e65 7720 3d20 6466 5f6e 6577 5b3a 3a2d  new = df_new[::-
-00023b50: 315d 0d0a 2020 2020 2020 2020 2020 2020  1]..            
-00023b60: 6466 5f6e 6577 203d 2064 665f 6e65 772e  df_new = df_new.
-00023b70: 6865 6164 2831 290d 0a20 2020 2020 2020  head(1)..       
-00023b80: 2020 2020 2064 665f 6e65 775b 2263 6c6f       df_new["clo
-00023b90: 7564 5f67 7265 656e 225d 203d 2064 665f  ud_green"] = df_
-00023ba0: 6e65 775b 2249 5341 5f39 225d 2e69 6c6f  new["ISA_9"].ilo
-00023bb0: 635b 305d 203e 2064 665f 6e65 775b 2249  c[0] > df_new["I
-00023bc0: 5342 5f32 3622 5d2e 696c 6f63 5b30 5d0d  SB_26"].iloc[0].
-00023bd0: 0a20 2020 2020 2020 2020 2020 2064 665f  .            df_
-00023be0: 6e65 775b 2263 6c6f 7564 5f72 6564 225d  new["cloud_red"]
-00023bf0: 203d 2064 665f 6e65 775b 2249 5342 5f32   = df_new["ISB_2
-00023c00: 3622 5d2e 696c 6f63 5b30 5d20 3e20 6466  6"].iloc[0] > df
-00023c10: 5f6e 6577 5b22 4953 415f 3922 5d2e 696c  _new["ISA_9"].il
-00023c20: 6f63 5b30 5d0d 0a20 2020 2020 2020 2065  oc[0]..        e
-00023c30: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-00023c40: 6173 2065 3a20 2023 2070 7261 676d 613a  as e:  # pragma:
-00023c50: 206e 6f20 636f 7665 720d 0a20 2020 2020   no cover..     
-00023c60: 2020 2020 2020 2073 656c 662e 6465 6661         self.defa
-00023c70: 756c 745f 6c6f 6767 6572 2e64 6562 7567  ult_logger.debug
-00023c80: 2865 2c20 6578 635f 696e 666f 3d54 7275  (e, exc_info=Tru
-00023c90: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-00023ca0: 7061 7373 0d0a 2020 2020 2020 2020 6162  pass..        ab
-00023cb0: 6f76 6543 6c6f 7564 546f 7020 3d20 4661  oveCloudTop = Fa
-00023cc0: 6c73 650d 0a20 2020 2020 2020 2023 2062  lse..        # b
-00023cd0: 6173 656c 696e 6520 3e20 636c 6f75 6420  aseline > cloud 
-00023ce0: 746f 7020 2863 6c6f 7564 2069 7320 626f  top (cloud is bo
-00023cf0: 756e 6420 6279 2073 7061 6e20 6120 616e  und by span a an
-00023d00: 6420 7370 616e 2062 2920 616e 6420 636c  d span b) and cl
-00023d10: 6f73 6520 6973 203e 2063 6c6f 7564 2074  ose is > cloud t
-00023d20: 6f70 0d0a 2020 2020 2020 2020 6966 2064  op..        if d
-00023d30: 665f 6e65 775b 2263 6c6f 7564 5f67 7265  f_new["cloud_gre
-00023d40: 656e 225d 2e69 6c6f 635b 305d 3a0d 0a20  en"].iloc[0]:.. 
-00023d50: 2020 2020 2020 2020 2020 2061 626f 7665             above
-00023d60: 436c 6f75 6454 6f70 203d 2028 0d0a 2020  CloudTop = (..  
-00023d70: 2020 2020 2020 2020 2020 2020 2020 6466                df
-00023d80: 5f6e 6577 5b22 494b 535f 3236 225d 2e69  _new["IKS_26"].i
-00023d90: 6c6f 635b 305d 203e 2064 665f 6e65 775b  loc[0] > df_new[
-00023da0: 2249 5341 5f39 225d 2e69 6c6f 635b 305d  "ISA_9"].iloc[0]
-00023db0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00023dc0: 2020 616e 6420 7265 6365 6e74 5b22 436c    and recent["Cl
-00023dd0: 6f73 6522 5d2e 696c 6f63 5b30 5d20 3e20  ose"].iloc[0] > 
-00023de0: 6466 5f6e 6577 5b22 4953 415f 3922 5d2e  df_new["ISA_9"].
-00023df0: 696c 6f63 5b30 5d0d 0a20 2020 2020 2020  iloc[0]..       
-00023e00: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-00023e10: 656c 6966 2064 665f 6e65 775b 2263 6c6f  elif df_new["clo
-00023e20: 7564 5f72 6564 225d 2e69 6c6f 635b 305d  ud_red"].iloc[0]
-00023e30: 3a0d 0a20 2020 2020 2020 2020 2020 2061  :..            a
-00023e40: 626f 7665 436c 6f75 6454 6f70 203d 2028  boveCloudTop = (
-00023e50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00023e60: 2020 6466 5f6e 6577 5b22 494b 535f 3236    df_new["IKS_26
-00023e70: 225d 2e69 6c6f 635b 305d 203e 2064 665f  "].iloc[0] > df_
-00023e80: 6e65 775b 2249 5342 5f32 3622 5d2e 696c  new["ISB_26"].il
-00023e90: 6f63 5b30 5d0d 0a20 2020 2020 2020 2020  oc[0]..         
-00023ea0: 2020 2020 2020 2061 6e64 2072 6563 656e         and recen
-00023eb0: 745b 2243 6c6f 7365 225d 2e69 6c6f 635b  t["Close"].iloc[
-00023ec0: 305d 203e 2064 665f 6e65 775b 2249 5342  0] > df_new["ISB
-00023ed0: 5f32 3622 5d2e 696c 6f63 5b30 5d0d 0a20  _26"].iloc[0].. 
-00023ee0: 2020 2020 2020 2020 2020 2029 0d0a 0d0a             )....
-00023ef0: 2020 2020 2020 2020 2320 4c61 7465 7374          # Latest
-00023f00: 2049 6368 696d 6f6b 7520 6261 7365 6c69   Ichimoku baseli
-00023f10: 6e65 2069 7320 3c20 6c61 7465 7374 2049  ne is < latest I
-00023f20: 6368 696d 6f6b 7520 636f 6e76 6572 7369  chimoku conversi
-00023f30: 6f6e 206c 696e 650d 0a20 2020 2020 2020  on line..       
-00023f40: 2069 6620 6162 6f76 6543 6c6f 7564 546f   if aboveCloudTo
-00023f50: 7020 616e 6420 6466 5f6e 6577 5b22 494b  p and df_new["IK
-00023f60: 535f 3236 225d 2e69 6c6f 635b 305d 203c  S_26"].iloc[0] <
-00023f70: 2064 665f 6e65 775b 2249 5453 5f39 225d   df_new["ITS_9"]
-00023f80: 2e69 6c6f 635b 305d 3a0d 0a20 2020 2020  .iloc[0]:..     
-00023f90: 2020 2020 2020 2023 2053 746f 6368 5253         # StochRS
-00023fa0: 4920 6372 6f73 7365 6420 3230 2061 6e64  I crossed 20 and
-00023fb0: 2052 5349 203e 2035 300d 0a20 2020 2020   RSI > 50..     
-00023fc0: 2020 2020 2020 2069 6620 666b 203e 2032         if fk > 2
-00023fd0: 3020 616e 6420 7265 6365 6e74 5b22 5253  0 and recent["RS
-00023fe0: 4922 5d2e 696c 6f63 5b30 5d20 3e20 3530  I"].iloc[0] > 50
-00023ff0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00024000: 2020 2023 2063 6f6e 6469 7469 6f6e 206f     # condition o
-00024010: 6620 6372 6f73 7369 6e67 2074 6865 2053  f crossing the S
-00024020: 746f 6368 5253 4920 6d61 696e 2073 6967  tochRSI main sig
-00024030: 6e61 6c20 6c69 6e65 2066 726f 6d20 626f  nal line from bo
-00024040: 7474 6f6d 2074 6f20 746f 700d 0a20 2020  ttom to top..   
-00024050: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00024060: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-00024070: 2020 2020 2020 2064 6174 615b 2246 4153         data["FAS
-00024080: 5444 225d 2e69 6c6f 635b 3130 305d 203c  TD"].iloc[100] <
-00024090: 2064 6174 615b 2246 4153 544b 225d 2e69   data["FASTK"].i
-000240a0: 6c6f 635b 3130 305d 0d0a 2020 2020 2020  loc[100]..      
-000240b0: 2020 2020 2020 2020 2020 2020 2020 616e                an
-000240c0: 6420 6461 7461 5b22 4641 5354 4422 5d2e  d data["FASTD"].
-000240d0: 696c 6f63 5b31 3031 5d20 3e20 6461 7461  iloc[101] > data
-000240e0: 5b22 4641 5354 4b22 5d2e 696c 6f63 5b31  ["FASTK"].iloc[1
-000240f0: 3031 5d0d 0a20 2020 2020 2020 2020 2020  01]..           
-00024100: 2020 2020 2029 3a0d 0a20 2020 2020 2020       ):..       
-00024110: 2020 2020 2020 2020 2020 2020 2023 2063               # c
-00024120: 6c6f 7365 203e 2035 3020 7065 7269 6f64  lose > 50 period
-00024130: 2053 4d41 2f45 4d41 2061 6e64 2032 3030   SMA/EMA and 200
-00024140: 2070 6572 696f 6420 534d 412f 454d 410d   period SMA/EMA.
-00024150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024160: 2020 2020 2069 6620 280d 0a20 2020 2020       if (..     
-00024170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024180: 2020 2072 6563 656e 745b 2253 534d 4122     recent["SSMA"
-00024190: 5d2e 696c 6f63 5b30 5d20 3e20 7265 6365  ].iloc[0] > rece
-000241a0: 6e74 5b22 534d 4122 5d2e 696c 6f63 5b30  nt["SMA"].iloc[0
-000241b0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000241c0: 2020 2020 2020 2020 2020 2061 6e64 2072             and r
-000241d0: 6563 656e 745b 2243 6c6f 7365 225d 2e69  ecent["Close"].i
-000241e0: 6c6f 635b 305d 203e 2072 6563 656e 745b  loc[0] > recent[
-000241f0: 2253 534d 4122 5d2e 696c 6f63 5b30 5d0d  "SSMA"].iloc[0].
-00024200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024210: 2020 2020 2020 2020 2061 6e64 2072 6563           and rec
-00024220: 656e 745b 2243 6c6f 7365 225d 2e69 6c6f  ent["Close"].ilo
-00024230: 635b 305d 203e 2072 6563 656e 745b 224c  c[0] > recent["L
-00024240: 4d41 225d 2e69 6c6f 635b 305d 0d0a 2020  MA"].iloc[0]..  
-00024250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024260: 2020 293a 0d0a 2020 2020 2020 2020 2020    ):..          
-00024270: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-00024280: 7665 6420 3d20 7365 6c66 2e66 696e 6443  ved = self.findC
-00024290: 7572 7265 6e74 5361 7665 6456 616c 7565  urrentSavedValue
-000242a0: 2873 6372 6565 6e44 6963 742c 7361 7665  (screenDict,save
-000242b0: 4469 6374 2c22 4d41 2d53 6967 6e61 6c22  Dict,"MA-Signal"
-000242c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000242d0: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-000242e0: 6e44 6963 745b 224d 412d 5369 676e 616c  nDict["MA-Signal
-000242f0: 225d 203d 2028 0d0a 2020 2020 2020 2020  "] = (..        
-00024300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024310: 2020 2020 7361 7665 645b 305d 202b 2063      saved[0] + c
-00024320: 6f6c 6f72 5465 7874 2e42 4f4c 4420 2b20  olorText.BOLD + 
-00024330: 636f 6c6f 7254 6578 742e 4752 4545 4e20  colorText.GREEN 
-00024340: 2b20 2242 756c 6c69 7368 2220 2b20 636f  + "Bullish" + co
-00024350: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
-00024360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024370: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-00024380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024390: 7361 7665 4469 6374 5b22 4d41 2d53 6967  saveDict["MA-Sig
-000243a0: 6e61 6c22 5d20 3d20 7361 7665 645b 315d  nal"] = saved[1]
-000243b0: 202b 2022 4275 6c6c 6973 6822 0d0a 2020   + "Bullish"..  
-000243c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000243d0: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-000243e0: 650d 0a20 2020 2020 2020 2072 6574 7572  e..        retur
-000243f0: 6e20 4661 6c73 650d 0a0d 0a20 2020 2023  n False....    #
-00024400: 2056 616c 6964 6174 6520 5650 430d 0a20   Validate VPC.. 
-00024410: 2020 2064 6566 2076 616c 6964 6174 6556     def validateV
-00024420: 4350 280d 0a20 2020 2020 2020 2073 656c  CP(..        sel
-00024430: 662c 2064 662c 2073 6372 6565 6e44 6963  f, df, screenDic
-00024440: 742c 2073 6176 6544 6963 742c 2073 746f  t, saveDict, sto
-00024450: 636b 4e61 6d65 3d4e 6f6e 652c 2077 696e  ckName=None, win
-00024460: 646f 773d 332c 2070 6572 6365 6e74 6167  dow=3, percentag
-00024470: 6546 726f 6d54 6f70 3d33 0d0a 2020 2020  eFromTop=3..    
-00024480: 293a 0d0a 2020 2020 2020 2020 6966 2064  ):..        if d
-00024490: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
-000244a0: 2864 6629 203d 3d20 303a 0d0a 2020 2020  (df) == 0:..    
-000244b0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-000244c0: 616c 7365 0d0a 2020 2020 2020 2020 6461  alse..        da
-000244d0: 7461 203d 2064 662e 636f 7079 2829 0d0a  ta = df.copy()..
-000244e0: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
-000244f0: 2020 2020 2020 2020 2020 7065 7263 656e            percen
-00024500: 7461 6765 4672 6f6d 546f 7020 2f3d 2031  tageFromTop /= 1
-00024510: 3030 0d0a 2020 2020 2020 2020 2020 2020  00..            
-00024520: 6461 7461 2e72 6573 6574 5f69 6e64 6578  data.reset_index
-00024530: 2869 6e70 6c61 6365 3d54 7275 6529 0d0a  (inplace=True)..
-00024540: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00024550: 2e72 656e 616d 6528 636f 6c75 6d6e 733d  .rename(columns=
-00024560: 7b22 696e 6465 7822 3a20 2244 6174 6522  {"index": "Date"
-00024570: 7d2c 2069 6e70 6c61 6365 3d54 7275 6529  }, inplace=True)
-00024580: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
-00024590: 7461 5b22 746f 7073 225d 203d 2028 0d0a  ta["tops"] = (..
-000245a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000245b0: 6461 7461 5b22 4869 6768 225d 0d0a 2020  data["High"]..  
-000245c0: 2020 2020 2020 2020 2020 2020 2020 2e69                .i
-000245d0: 6c6f 635b 0d0a 2020 2020 2020 2020 2020  loc[..          
-000245e0: 2020 2020 2020 2020 2020 6c69 7374 280d            list(.
-000245f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024600: 2020 2020 2020 2020 2070 6b74 616c 6962           pktalib
-00024610: 2e61 7267 7265 6c65 7874 7265 6d61 280d  .argrelextrema(.
-00024620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024630: 2020 2020 2020 2020 2020 2020 206e 702e               np.
-00024640: 6172 7261 7928 6461 7461 5b22 4869 6768  array(data["High
-00024650: 225d 292c 206e 702e 6772 6561 7465 725f  "]), np.greater_
-00024660: 6571 7561 6c2c 206f 7264 6572 3d77 696e  equal, order=win
-00024670: 646f 770d 0a20 2020 2020 2020 2020 2020  dow..           
-00024680: 2020 2020 2020 2020 2020 2020 2029 5b30               )[0
-00024690: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000246a0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-000246b0: 2020 2020 2020 2020 2020 5d0d 0a20 2020            ]..   
-000246c0: 2020 2020 2020 2020 2020 2020 202e 6865               .he
-000246d0: 6164 2834 290d 0a20 2020 2020 2020 2020  ad(4)..         
-000246e0: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
-000246f0: 2020 6461 7461 5b22 626f 7473 225d 203d    data["bots"] =
-00024700: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-00024710: 2020 2020 6461 7461 5b22 4c6f 7722 5d0d      data["Low"].
-00024720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024730: 202e 696c 6f63 5b0d 0a20 2020 2020 2020   .iloc[..       
-00024740: 2020 2020 2020 2020 2020 2020 206c 6973               lis
-00024750: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
-00024760: 2020 2020 2020 2020 2020 2020 706b 7461              pkta
-00024770: 6c69 622e 6172 6772 656c 6578 7472 656d  lib.argrelextrem
-00024780: 6128 0d0a 2020 2020 2020 2020 2020 2020  a(..            
-00024790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000247a0: 6e70 2e61 7272 6179 2864 6174 615b 224c  np.array(data["L
-000247b0: 6f77 225d 292c 206e 702e 6c65 7373 5f65  ow"]), np.less_e
-000247c0: 7175 616c 2c20 6f72 6465 723d 7769 6e64  qual, order=wind
-000247d0: 6f77 0d0a 2020 2020 2020 2020 2020 2020  ow..            
-000247e0: 2020 2020 2020 2020 2020 2020 295b 305d              )[0]
-000247f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00024800: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00024810: 2020 2020 2020 2020 205d 0d0a 2020 2020           ]..    
-00024820: 2020 2020 2020 2020 2020 2020 2e68 6561              .hea
-00024830: 6428 3429 0d0a 2020 2020 2020 2020 2020  d(4)..          
-00024840: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-00024850: 2064 6174 6120 3d20 6461 7461 2e66 696c   data = data.fil
-00024860: 6c6e 6128 3029 0d0a 2020 2020 2020 2020  lna(0)..        
-00024870: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
-00024880: 7265 706c 6163 6528 5b6e 702e 696e 662c  replace([np.inf,
-00024890: 202d 6e70 2e69 6e66 5d2c 2030 290d 0a20   -np.inf], 0).. 
-000248a0: 2020 2020 2020 2020 2020 2074 6f70 7320             tops 
-000248b0: 3d20 6461 7461 5b64 6174 612e 746f 7073  = data[data.tops
-000248c0: 203e 2030 5d0d 0a20 2020 2020 2020 2020   > 0]..         
-000248d0: 2020 2023 2062 6f74 7320 3d20 6461 7461     # bots = data
-000248e0: 5b64 6174 612e 626f 7473 203e 2030 5d0d  [data.bots > 0].
-000248f0: 0a20 2020 2020 2020 2020 2020 2068 6967  .            hig
-00024900: 6865 7374 546f 7020 3d20 726f 756e 6428  hestTop = round(
-00024910: 746f 7073 2e64 6573 6372 6962 6528 295b  tops.describe()[
-00024920: 2248 6967 6822 5d5b 226d 6178 225d 2c20  "High"]["max"], 
-00024930: 3129 0d0a 2020 2020 2020 2020 2020 2020  1)..            
-00024940: 6669 6c74 6572 6564 546f 7073 203d 2074  filteredTops = t
-00024950: 6f70 735b 0d0a 2020 2020 2020 2020 2020  ops[..          
-00024960: 2020 2020 2020 746f 7073 2e74 6f70 7320        tops.tops 
-00024970: 3e20 2868 6967 6865 7374 546f 7020 2d20  > (highestTop - 
-00024980: 2868 6967 6865 7374 546f 7020 2a20 7065  (highestTop * pe
-00024990: 7263 656e 7461 6765 4672 6f6d 546f 7029  rcentageFromTop)
-000249a0: 290d 0a20 2020 2020 2020 2020 2020 205d  )..            ]
-000249b0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-000249c0: 2066 696c 7465 7265 6454 6f70 732e 6571   filteredTops.eq
-000249d0: 7561 6c73 2874 6f70 7329 3a20 2023 2054  uals(tops):  # T
-000249e0: 6f70 7320 6172 6520 696e 2074 6865 2072  ops are in the r
-000249f0: 616e 6765 0d0a 2020 2020 2020 2020 2020  ange..          
-00024a00: 2020 2020 2020 6c6f 7750 6f69 6e74 7320        lowPoints 
-00024a10: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00024a20: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-00024a30: 616e 6765 286c 656e 2874 6f70 7329 202d  ange(len(tops) -
-00024a40: 2031 293a 0d0a 2020 2020 2020 2020 2020   1):..          
-00024a50: 2020 2020 2020 2020 2020 656e 6444 6174            endDat
-00024a60: 6520 3d20 746f 7073 2e69 6c6f 635b 695d  e = tops.iloc[i]
-00024a70: 5b22 4461 7465 225d 0d0a 2020 2020 2020  ["Date"]..      
-00024a80: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00024a90: 6172 7444 6174 6520 3d20 746f 7073 2e69  artDate = tops.i
-00024aa0: 6c6f 635b 6920 2b20 315d 5b22 4461 7465  loc[i + 1]["Date
-00024ab0: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
-00024ac0: 2020 2020 2020 2020 6c6f 7750 6f69 6e74          lowPoint
-00024ad0: 732e 6170 7065 6e64 280d 0a20 2020 2020  s.append(..     
-00024ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024af0: 2020 2064 6174 615b 0d0a 2020 2020 2020     data[..      
-00024b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024b10: 2020 2020 2020 2864 6174 612e 4461 7465        (data.Date
-00024b20: 203e 3d20 7374 6172 7444 6174 6529 2026   >= startDate) &
-00024b30: 2028 6461 7461 2e44 6174 6520 3c3d 2065   (data.Date <= e
-00024b40: 6e64 4461 7465 290d 0a20 2020 2020 2020  ndDate)..       
-00024b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024b60: 205d 2e64 6573 6372 6962 6528 295b 224c   ].describe()["L
-00024b70: 6f77 225d 5b22 6d69 6e22 5d0d 0a20 2020  ow"]["min"]..   
-00024b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024b90: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
-00024ba0: 2020 2020 6c6f 7750 6f69 6e74 734f 7267      lowPointsOrg
-00024bb0: 203d 206c 6f77 506f 696e 7473 0d0a 2020   = lowPoints..  
-00024bc0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00024bd0: 7750 6f69 6e74 732e 736f 7274 2872 6576  wPoints.sort(rev
-00024be0: 6572 7365 3d54 7275 6529 0d0a 2020 2020  erse=True)..    
-00024bf0: 2020 2020 2020 2020 2020 2020 6c6f 7750              lowP
-00024c00: 6f69 6e74 7353 6f72 7465 6420 3d20 6c6f  ointsSorted = lo
-00024c10: 7750 6f69 6e74 730d 0a20 2020 2020 2020  wPoints..       
-00024c20: 2020 2020 2020 2020 206c 7470 203d 2064           ltp = d
-00024c30: 6174 612e 6865 6164 2831 295b 2243 6c6f  ata.head(1)["Clo
-00024c40: 7365 225d 2e69 6c6f 635b 305d 0d0a 2020  se"].iloc[0]..  
-00024c50: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00024c60: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-00024c70: 2020 2020 2020 2020 6c6f 7750 6f69 6e74          lowPoint
-00024c80: 734f 7267 203d 3d20 6c6f 7750 6f69 6e74  sOrg == lowPoint
-00024c90: 7353 6f72 7465 640d 0a20 2020 2020 2020  sSorted..       
-00024ca0: 2020 2020 2020 2020 2020 2020 2061 6e64               and
-00024cb0: 206c 7470 203c 2068 6967 6865 7374 546f   ltp < highestTo
-00024cc0: 700d 0a20 2020 2020 2020 2020 2020 2020  p..             
-00024cd0: 2020 2020 2020 2061 6e64 206c 7470 203e         and ltp >
-00024ce0: 206c 6f77 506f 696e 7473 5b30 5d0d 0a20   lowPoints[0].. 
-00024cf0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00024d00: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00024d10: 2020 2020 2020 2073 6176 6564 203d 2073         saved = s
-00024d20: 656c 662e 6669 6e64 4375 7272 656e 7453  elf.findCurrentS
-00024d30: 6176 6564 5661 6c75 6528 7363 7265 656e  avedValue(screen
-00024d40: 4469 6374 2c20 7361 7665 4469 6374 2c20  Dict, saveDict, 
-00024d50: 2250 6174 7465 726e 2229 0d0a 2020 2020  "Pattern")..    
+00020de0: 2020 2023 2020 2020 2066 2753 746f 636b     #     f'Stock
+00020df0: 3a7b 7361 7665 4469 6374 5b22 5374 6f63  :{saveDict["Stoc
+00020e00: 6b22 5d7d 2c20 6973 2061 206d 6f6d 656e  k"]}, is a momen
+00020e10: 7475 6d2d 6761 696e 6572 2062 6563 6175  tum-gainer becau
+00020e20: 7365 2074 6f64 6179 2d6f 7065 6e20 287b  se today-open ({
+00020e30: 746f 7d29 203e 3d20 7965 7374 6572 6461  to}) >= yesterda
+00020e40: 792d 636c 6f73 6520 287b 7963 7d29 2061  y-close ({yc}) a
+00020e50: 6e64 2079 6573 7465 7264 6179 2d6f 7065  nd yesterday-ope
+00020e60: 6e28 7b79 6f7d 2920 3e3d 2064 6179 2d62  n({yo}) >= day-b
+00020e70: 6566 6f72 652d 636c 6f73 6528 7b64 7963  efore-close({dyc
+00020e80: 7d29 270d 0a20 2020 2020 2020 2020 2020  })'..           
+00020e90: 2020 2020 2020 2020 2020 2020 2023 2029               # )
+00020ea0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00020eb0: 2020 2020 2020 2020 2020 7361 7665 6420            saved 
+00020ec0: 3d20 7365 6c66 2e66 696e 6443 7572 7265  = self.findCurre
+00020ed0: 6e74 5361 7665 6456 616c 7565 2873 6372  ntSavedValue(scr
+00020ee0: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
+00020ef0: 742c 2022 5061 7474 6572 6e22 290d 0a20  t, "Pattern").. 
+00020f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020f10: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+00020f20: 745b 2250 6174 7465 726e 225d 203d 2028  t["Pattern"] = (
+00020f30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00020f40: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+00020f50: 7665 645b 305d 0d0a 2020 2020 2020 2020  ved[0]..        
+00020f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020f70: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
+00020f80: 424f 4c44 0d0a 2020 2020 2020 2020 2020  BOLD..          
+00020f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020fa0: 2020 2b20 636f 6c6f 7254 6578 742e 4752    + colorText.GR
+00020fb0: 4545 4e0d 0a20 2020 2020 2020 2020 2020  EEN..           
+00020fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020fd0: 202b 2022 4d6f 6d65 6e74 756d 2047 6169   + "Momentum Gai
+00020fe0: 6e65 7222 0d0a 2020 2020 2020 2020 2020  ner"..          
+00020ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021000: 2020 2b20 636f 6c6f 7254 6578 742e 454e    + colorText.EN
+00021010: 440d 0a20 2020 2020 2020 2020 2020 2020  D..             
+00021020: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+00021030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021040: 2020 2020 2020 7361 7665 4469 6374 5b22        saveDict["
+00021050: 5061 7474 6572 6e22 5d20 3d20 7361 7665  Pattern"] = save
+00021060: 645b 315d 202b 2022 4d6f 6d65 6e74 756d  d[1] + "Momentum
+00021070: 2047 6169 6e65 7222 0d0a 2020 2020 2020   Gainer"..      
+00021080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021090: 2020 7265 7475 726e 2054 7275 650d 0a20    return True.. 
+000210a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000210b0: 2020 2023 2073 656c 662e 6465 6661 756c     # self.defaul
+000210c0: 745f 6c6f 6767 6572 2e69 6e66 6f28 0d0a  t_logger.info(..
+000210d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000210e0: 2020 2020 2320 2020 2020 6627 5374 6f63      #     f'Stoc
+000210f0: 6b3a 7b73 6176 6544 6963 745b 2253 746f  k:{saveDict["Sto
+00021100: 636b 225d 7d2c 2069 7320 6e6f 7420 6120  ck"]}, is not a 
+00021110: 6d6f 6d65 6e74 756d 2d67 6169 6e65 7220  momentum-gainer 
+00021120: 6265 6361 7573 6520 6569 7468 6572 2074  because either t
+00021130: 6f64 6179 2d6f 7065 6e20 287b 746f 7d29  oday-open ({to})
+00021140: 203c 2079 6573 7465 7264 6179 2d63 6c6f   < yesterday-clo
+00021150: 7365 2028 7b79 637d 2920 6f72 2079 6573  se ({yc}) or yes
+00021160: 7465 7264 6179 2d6f 7065 6e28 7b79 6f7d  terday-open({yo}
+00021170: 2920 3c20 6461 792d 6265 666f 7265 2d63  ) < day-before-c
+00021180: 6c6f 7365 287b 6479 637d 2927 0d0a 2020  lose({dyc})'..  
+00021190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000211a0: 2020 2320 290d 0a20 2020 2020 2020 2020    # )..         
+000211b0: 2020 2065 7863 6570 7420 496e 6465 7845     except IndexE
+000211c0: 7272 6f72 2061 7320 653a 2023 2070 7261  rror as e: # pra
+000211d0: 676d 613a 206e 6f20 636f 7665 720d 0a20  gma: no cover.. 
+000211e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000211f0: 656c 662e 6465 6661 756c 745f 6c6f 6767  elf.default_logg
+00021200: 6572 2e64 6562 7567 2865 2c20 6578 635f  er.debug(e, exc_
+00021210: 696e 666f 3d54 7275 6529 0d0a 2020 2020  info=True)..    
+00021220: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00021230: 2e64 6566 6175 6c74 5f6c 6f67 6765 722e  .default_logger.
+00021240: 6465 6275 6728 6461 7461 290d 0a20 2020  debug(data)..   
+00021250: 2020 2020 2020 2020 2020 2020 2070 6173               pas
+00021260: 730d 0a20 2020 2020 2020 2020 2020 2072  s..            r
+00021270: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
+00021280: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
+00021290: 7074 696f 6e20 6173 2065 3a20 2023 2070  ption as e:  # p
+000212a0: 7261 676d 613a 206e 6f20 636f 7665 720d  ragma: no cover.
+000212b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000212c0: 662e 6465 6661 756c 745f 6c6f 6767 6572  f.default_logger
+000212d0: 2e64 6562 7567 2865 2c20 6578 635f 696e  .debug(e, exc_in
+000212e0: 666f 3d54 7275 6529 0d0a 2020 2020 2020  fo=True)..      
+000212f0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+00021300: 7365 0d0a 0d0a 2020 2020 2340 6d65 6173  se....    #@meas
+00021310: 7572 655f 7469 6d65 0d0a 2020 2020 2320  ure_time..    # 
+00021320: 5661 6c69 6461 7465 204d 6f76 696e 6720  Validate Moving 
+00021330: 6176 6572 6167 6573 2061 6e64 206c 6f6f  averages and loo
+00021340: 6b20 666f 7220 6275 792f 7365 6c6c 2073  k for buy/sell s
+00021350: 6967 6e61 6c73 0d0a 2020 2020 6465 6620  ignals..    def 
+00021360: 7661 6c69 6461 7465 4d6f 7669 6e67 4176  validateMovingAv
+00021370: 6572 6167 6573 2873 656c 662c 2064 662c  erages(self, df,
+00021380: 2073 6372 6565 6e44 6963 742c 2073 6176   screenDict, sav
+00021390: 6544 6963 742c 206d 6152 616e 6765 3d32  eDict, maRange=2
+000213a0: 2e35 293a 0d0a 2020 2020 2020 2020 6461  .5):..        da
+000213b0: 7461 203d 2064 662e 636f 7079 2829 0d0a  ta = df.copy()..
+000213c0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+000213d0: 6174 612e 6669 6c6c 6e61 2830 290d 0a20  ata.fillna(0).. 
+000213e0: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
+000213f0: 7461 2e72 6570 6c61 6365 285b 6e70 2e69  ta.replace([np.i
+00021400: 6e66 2c20 2d6e 702e 696e 665d 2c20 3029  nf, -np.inf], 0)
+00021410: 0d0a 2020 2020 2020 2020 7265 6365 6e74  ..        recent
+00021420: 203d 2064 6174 612e 6865 6164 2831 290d   = data.head(1).
+00021430: 0a20 2020 2020 2020 2073 6176 6564 203d  .        saved =
+00021440: 2073 656c 662e 6669 6e64 4375 7272 656e   self.findCurren
+00021450: 7453 6176 6564 5661 6c75 6528 7363 7265  tSavedValue(scre
+00021460: 656e 4469 6374 2c73 6176 6544 6963 742c  enDict,saveDict,
+00021470: 224d 412d 5369 676e 616c 2229 0d0a 2020  "MA-Signal")..  
+00021480: 2020 2020 2020 6966 2028 0d0a 2020 2020        if (..    
+00021490: 2020 2020 2020 2020 7265 6365 6e74 5b22          recent["
+000214a0: 534d 4122 5d2e 696c 6f63 5b30 5d20 3e20  SMA"].iloc[0] > 
+000214b0: 7265 6365 6e74 5b22 4c4d 4122 5d2e 696c  recent["LMA"].il
+000214c0: 6f63 5b30 5d0d 0a20 2020 2020 2020 2020  oc[0]..         
+000214d0: 2020 2061 6e64 2072 6563 656e 745b 2243     and recent["C
+000214e0: 6c6f 7365 225d 2e69 6c6f 635b 305d 203e  lose"].iloc[0] >
+000214f0: 2072 6563 656e 745b 2253 4d41 225d 2e69   recent["SMA"].i
+00021500: 6c6f 635b 305d 0d0a 2020 2020 2020 2020  loc[0]..        
+00021510: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00021520: 7363 7265 656e 4469 6374 5b22 4d41 2d53  screenDict["MA-S
+00021530: 6967 6e61 6c22 5d20 3d20 280d 0a20 2020  ignal"] = (..   
+00021540: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+00021550: 6564 5b30 5d20 2b20 636f 6c6f 7254 6578  ed[0] + colorTex
+00021560: 742e 424f 4c44 202b 2063 6f6c 6f72 5465  t.BOLD + colorTe
+00021570: 7874 2e47 5245 454e 202b 2022 4275 6c6c  xt.GREEN + "Bull
+00021580: 6973 6822 202b 2063 6f6c 6f72 5465 7874  ish" + colorText
+00021590: 2e45 4e44 0d0a 2020 2020 2020 2020 2020  .END..          
+000215a0: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
+000215b0: 2073 6176 6544 6963 745b 224d 412d 5369   saveDict["MA-Si
+000215c0: 676e 616c 225d 203d 2073 6176 6564 5b31  gnal"] = saved[1
+000215d0: 5d20 2b20 2242 756c 6c69 7368 220d 0a20  ] + "Bullish".. 
+000215e0: 2020 2020 2020 2065 6c69 6620 7265 6365         elif rece
+000215f0: 6e74 5b22 534d 4122 5d2e 696c 6f63 5b30  nt["SMA"].iloc[0
+00021600: 5d20 3c20 7265 6365 6e74 5b22 4c4d 4122  ] < recent["LMA"
+00021610: 5d2e 696c 6f63 5b30 5d3a 0d0a 2020 2020  ].iloc[0]:..    
+00021620: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
+00021630: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
+00021640: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
+00021650: 2020 2020 2073 6176 6564 5b30 5d20 2b20       saved[0] + 
+00021660: 636f 6c6f 7254 6578 742e 424f 4c44 202b  colorText.BOLD +
+00021670: 2063 6f6c 6f72 5465 7874 2e46 4149 4c20   colorText.FAIL 
+00021680: 2b20 2242 6561 7269 7368 2220 2b20 636f  + "Bearish" + co
+00021690: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
+000216a0: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
+000216b0: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
+000216c0: 5b22 4d41 2d53 6967 6e61 6c22 5d20 3d20  ["MA-Signal"] = 
+000216d0: 7361 7665 645b 315d 202b 2022 4265 6172  saved[1] + "Bear
+000216e0: 6973 6822 0d0a 2020 2020 2020 2020 656c  ish"..        el
+000216f0: 6966 2072 6563 656e 745b 2253 4d41 225d  if recent["SMA"]
+00021700: 2e69 6c6f 635b 305d 203d 3d20 303a 0d0a  .iloc[0] == 0:..
+00021710: 2020 2020 2020 2020 2020 2020 7363 7265              scre
+00021720: 656e 4469 6374 5b22 4d41 2d53 6967 6e61  enDict["MA-Signa
+00021730: 6c22 5d20 3d20 280d 0a20 2020 2020 2020  l"] = (..       
+00021740: 2020 2020 2020 2020 2073 6176 6564 5b30           saved[0
+00021750: 5d20 2b20 636f 6c6f 7254 6578 742e 424f  ] + colorText.BO
+00021760: 4c44 202b 2063 6f6c 6f72 5465 7874 2e57  LD + colorText.W
+00021770: 4152 4e20 2b20 2255 6e6b 6e6f 776e 2220  ARN + "Unknown" 
+00021780: 2b20 636f 6c6f 7254 6578 742e 454e 440d  + colorText.END.
+00021790: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
+000217a0: 2020 2020 2020 2020 2020 2020 7361 7665              save
+000217b0: 4469 6374 5b22 4d41 2d53 6967 6e61 6c22  Dict["MA-Signal"
+000217c0: 5d20 3d20 7361 7665 645b 315d 202b 2022  ] = saved[1] + "
+000217d0: 556e 6b6e 6f77 6e22 0d0a 2020 2020 2020  Unknown"..      
+000217e0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+000217f0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+00021800: 224d 412d 5369 676e 616c 225d 203d 2028  "MA-Signal"] = (
+00021810: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00021820: 2020 7361 7665 645b 305d 202b 2063 6f6c    saved[0] + col
+00021830: 6f72 5465 7874 2e42 4f4c 4420 2b20 636f  orText.BOLD + co
+00021840: 6c6f 7254 6578 742e 5741 524e 202b 2022  lorText.WARN + "
+00021850: 4e65 7574 7261 6c22 202b 2063 6f6c 6f72  Neutral" + color
+00021860: 5465 7874 2e45 4e44 0d0a 2020 2020 2020  Text.END..      
+00021870: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+00021880: 2020 2020 2073 6176 6544 6963 745b 224d       saveDict["M
+00021890: 412d 5369 676e 616c 225d 203d 2073 6176  A-Signal"] = sav
+000218a0: 6564 5b31 5d20 2b20 224e 6575 7472 616c  ed[1] + "Neutral
+000218b0: 220d 0a0d 0a20 2020 2020 2020 2073 6d61  "....        sma
+000218c0: 4465 7620 3d20 6461 7461 5b22 534d 4122  Dev = data["SMA"
+000218d0: 5d2e 696c 6f63 5b30 5d20 2a20 6d61 5261  ].iloc[0] * maRa
+000218e0: 6e67 6520 2f20 3130 300d 0a20 2020 2020  nge / 100..     
+000218f0: 2020 206c 6d61 4465 7620 3d20 6461 7461     lmaDev = data
+00021900: 5b22 4c4d 4122 5d2e 696c 6f63 5b30 5d20  ["LMA"].iloc[0] 
+00021910: 2a20 6d61 5261 6e67 6520 2f20 3130 300d  * maRange / 100.
+00021920: 0a20 2020 2020 2020 206f 7065 6e2c 2068  .        open, h
+00021930: 6967 682c 206c 6f77 2c20 636c 6f73 652c  igh, low, close,
+00021940: 2073 6d61 2c20 6c6d 6120 3d20 280d 0a20   sma, lma = (.. 
+00021950: 2020 2020 2020 2020 2020 2064 6174 615b             data[
+00021960: 224f 7065 6e22 5d2e 696c 6f63 5b30 5d2c  "Open"].iloc[0],
+00021970: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
+00021980: 7461 5b22 4869 6768 225d 2e69 6c6f 635b  ta["High"].iloc[
+00021990: 305d 2c0d 0a20 2020 2020 2020 2020 2020  0],..           
+000219a0: 2064 6174 615b 224c 6f77 225d 2e69 6c6f   data["Low"].ilo
+000219b0: 635b 305d 2c0d 0a20 2020 2020 2020 2020  c[0],..         
+000219c0: 2020 2064 6174 615b 2243 6c6f 7365 225d     data["Close"]
+000219d0: 2e69 6c6f 635b 305d 2c0d 0a20 2020 2020  .iloc[0],..     
+000219e0: 2020 2020 2020 2064 6174 615b 2253 4d41         data["SMA
+000219f0: 225d 2e69 6c6f 635b 305d 2c0d 0a20 2020  "].iloc[0],..   
+00021a00: 2020 2020 2020 2020 2064 6174 615b 224c           data["L
+00021a10: 4d41 225d 2e69 6c6f 635b 305d 2c0d 0a20  MA"].iloc[0],.. 
+00021a20: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+00021a30: 2020 6d61 5265 7665 7273 616c 203d 2030    maReversal = 0
+00021a40: 0d0a 2020 2020 2020 2020 2320 5461 6b69  ..        # Taki
+00021a50: 6e67 2053 7570 706f 7274 2035 300d 0a20  ng Support 50.. 
+00021a60: 2020 2020 2020 2069 6620 636c 6f73 6520         if close 
+00021a70: 3e20 736d 6120 616e 6420 6c6f 7720 3c3d  > sma and low <=
+00021a80: 2028 736d 6120 2b20 736d 6144 6576 293a   (sma + smaDev):
+00021a90: 0d0a 2020 2020 2020 2020 2020 2020 7363  ..            sc
+00021aa0: 7265 656e 4469 6374 5b22 4d41 2d53 6967  reenDict["MA-Sig
+00021ab0: 6e61 6c22 5d20 3d20 280d 0a20 2020 2020  nal"] = (..     
+00021ac0: 2020 2020 2020 2020 2020 2073 6176 6564             saved
+00021ad0: 5b30 5d20 2b20 636f 6c6f 7254 6578 742e  [0] + colorText.
+00021ae0: 424f 4c44 202b 2063 6f6c 6f72 5465 7874  BOLD + colorText
+00021af0: 2e47 5245 454e 202b 2022 3530 4d41 2d53  .GREEN + "50MA-S
+00021b00: 7570 706f 7274 2220 2b20 636f 6c6f 7254  upport" + colorT
+00021b10: 6578 742e 454e 440d 0a20 2020 2020 2020  ext.END..       
+00021b20: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00021b30: 2020 2020 7361 7665 4469 6374 5b22 4d41      saveDict["MA
+00021b40: 2d53 6967 6e61 6c22 5d20 3d20 7361 7665  -Signal"] = save
+00021b50: 645b 315d 202b 2022 3530 4d41 2d53 7570  d[1] + "50MA-Sup
+00021b60: 706f 7274 220d 0a20 2020 2020 2020 2020  port"..         
+00021b70: 2020 206d 6152 6576 6572 7361 6c20 3d20     maReversal = 
+00021b80: 310d 0a20 2020 2020 2020 2023 2056 616c  1..        # Val
+00021b90: 6964 6174 696e 6720 5265 7369 7374 616e  idating Resistan
+00021ba0: 6365 2035 300d 0a20 2020 2020 2020 2065  ce 50..        e
+00021bb0: 6c69 6620 636c 6f73 6520 3c20 736d 6120  lif close < sma 
+00021bc0: 616e 6420 6869 6768 203e 3d20 2873 6d61  and high >= (sma
+00021bd0: 202d 2073 6d61 4465 7629 3a0d 0a20 2020   - smaDev):..   
+00021be0: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
+00021bf0: 6963 745b 224d 412d 5369 676e 616c 225d  ict["MA-Signal"]
+00021c00: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
+00021c10: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
+00021c20: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
+00021c30: 2b20 636f 6c6f 7254 6578 742e 4641 494c  + colorText.FAIL
+00021c40: 202b 2022 3530 4d41 2d52 6573 6973 7422   + "50MA-Resist"
+00021c50: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
+00021c60: 0d0a 2020 2020 2020 2020 2020 2020 290d  ..            ).
+00021c70: 0a20 2020 2020 2020 2020 2020 2073 6176  .            sav
+00021c80: 6544 6963 745b 224d 412d 5369 676e 616c  eDict["MA-Signal
+00021c90: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
+00021ca0: 2235 304d 412d 5265 7369 7374 220d 0a20  "50MA-Resist".. 
+00021cb0: 2020 2020 2020 2020 2020 206d 6152 6576             maRev
+00021cc0: 6572 7361 6c20 3d20 2d31 0d0a 2020 2020  ersal = -1..    
+00021cd0: 2020 2020 2320 5461 6b69 6e67 2053 7570      # Taking Sup
+00021ce0: 706f 7274 2032 3030 0d0a 2020 2020 2020  port 200..      
+00021cf0: 2020 656c 6966 2063 6c6f 7365 203e 206c    elif close > l
+00021d00: 6d61 2061 6e64 206c 6f77 203c 3d20 286c  ma and low <= (l
+00021d10: 6d61 202b 206c 6d61 4465 7629 3a0d 0a20  ma + lmaDev):.. 
+00021d20: 2020 2020 2020 2020 2020 2073 6372 6565             scree
+00021d30: 6e44 6963 745b 224d 412d 5369 676e 616c  nDict["MA-Signal
+00021d40: 225d 203d 2028 0d0a 2020 2020 2020 2020  "] = (..        
+00021d50: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
+00021d60: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
+00021d70: 4420 2b20 636f 6c6f 7254 6578 742e 4752  D + colorText.GR
+00021d80: 4545 4e20 2b20 2232 3030 4d41 2d53 7570  EEN + "200MA-Sup
+00021d90: 706f 7274 2220 2b20 636f 6c6f 7254 6578  port" + colorTex
+00021da0: 742e 454e 440d 0a20 2020 2020 2020 2020  t.END..         
+00021db0: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
+00021dc0: 2020 7361 7665 4469 6374 5b22 4d41 2d53    saveDict["MA-S
+00021dd0: 6967 6e61 6c22 5d20 3d20 7361 7665 645b  ignal"] = saved[
+00021de0: 315d 202b 2022 3230 304d 412d 5375 7070  1] + "200MA-Supp
+00021df0: 6f72 7422 0d0a 2020 2020 2020 2020 2020  ort"..          
+00021e00: 2020 6d61 5265 7665 7273 616c 203d 2031    maReversal = 1
+00021e10: 0d0a 2020 2020 2020 2020 2320 5661 6c69  ..        # Vali
+00021e20: 6461 7469 6e67 2052 6573 6973 7461 6e63  dating Resistanc
+00021e30: 6520 3230 300d 0a20 2020 2020 2020 2065  e 200..        e
+00021e40: 6c69 6620 636c 6f73 6520 3c20 6c6d 6120  lif close < lma 
+00021e50: 616e 6420 6869 6768 203e 3d20 286c 6d61  and high >= (lma
+00021e60: 202d 206c 6d61 4465 7629 3a0d 0a20 2020   - lmaDev):..   
+00021e70: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
+00021e80: 6963 745b 224d 412d 5369 676e 616c 225d  ict["MA-Signal"]
+00021e90: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
+00021ea0: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
+00021eb0: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
+00021ec0: 2b20 636f 6c6f 7254 6578 742e 4641 494c  + colorText.FAIL
+00021ed0: 202b 2022 3230 304d 412d 5265 7369 7374   + "200MA-Resist
+00021ee0: 2220 2b20 636f 6c6f 7254 6578 742e 454e  " + colorText.EN
+00021ef0: 440d 0a20 2020 2020 2020 2020 2020 2029  D..            )
+00021f00: 0d0a 2020 2020 2020 2020 2020 2020 7361  ..            sa
+00021f10: 7665 4469 6374 5b22 4d41 2d53 6967 6e61  veDict["MA-Signa
+00021f20: 6c22 5d20 3d20 7361 7665 645b 315d 202b  l"] = saved[1] +
+00021f30: 2022 3230 304d 412d 5265 7369 7374 220d   "200MA-Resist".
+00021f40: 0a20 2020 2020 2020 2020 2020 206d 6152  .            maR
+00021f50: 6576 6572 7361 6c20 3d20 2d31 0d0a 2020  eversal = -1..  
+00021f60: 2020 2020 2020 2320 466f 7220 6120 4275        # For a Bu
+00021f70: 6c6c 6973 6820 4361 6e64 6c65 0d0a 2020  llish Candle..  
+00021f80: 2020 2020 2020 6966 2073 656c 662e 6765        if self.ge
+00021f90: 7443 616e 646c 6554 7970 6528 6461 7461  tCandleType(data
+00021fa0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00021fb0: 2320 4372 6f73 7369 6e67 2075 7020 3530  # Crossing up 50
+00021fc0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00021fd0: 206f 7065 6e20 3c20 736d 6120 616e 6420   open < sma and 
+00021fe0: 636c 6f73 6520 3e20 736d 613a 0d0a 2020  close > sma:..  
+00021ff0: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+00022000: 7265 656e 4469 6374 5b22 4d41 2d53 6967  reenDict["MA-Sig
+00022010: 6e61 6c22 5d20 3d20 280d 0a20 2020 2020  nal"] = (..     
+00022020: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00022030: 6176 6564 5b30 5d20 2b20 636f 6c6f 7254  aved[0] + colorT
+00022040: 6578 742e 424f 4c44 202b 2063 6f6c 6f72  ext.BOLD + color
+00022050: 5465 7874 2e47 5245 454e 202b 2022 4275  Text.GREEN + "Bu
+00022060: 6c6c 4372 6f73 732d 3530 4d41 2220 2b20  llCross-50MA" + 
+00022070: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
+00022080: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00022090: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000220a0: 2020 7361 7665 4469 6374 5b22 4d41 2d53    saveDict["MA-S
+000220b0: 6967 6e61 6c22 5d20 3d20 7361 7665 645b  ignal"] = saved[
+000220c0: 315d 202b 2022 4275 6c6c 4372 6f73 732d  1] + "BullCross-
+000220d0: 3530 4d41 220d 0a20 2020 2020 2020 2020  50MA"..         
+000220e0: 2020 2020 2020 206d 6152 6576 6572 7361         maReversa
+000220f0: 6c20 3d20 310d 0a20 2020 2020 2020 2020  l = 1..         
+00022100: 2020 2023 2043 726f 7373 696e 6720 7570     # Crossing up
+00022110: 2032 3030 0d0a 2020 2020 2020 2020 2020   200..          
+00022120: 2020 656c 6966 206f 7065 6e20 3c20 6c6d    elif open < lm
+00022130: 6120 616e 6420 636c 6f73 6520 3e20 6c6d  a and close > lm
+00022140: 613a 0d0a 2020 2020 2020 2020 2020 2020  a:..            
+00022150: 2020 2020 7363 7265 656e 4469 6374 5b22      screenDict["
+00022160: 4d41 2d53 6967 6e61 6c22 5d20 3d20 280d  MA-Signal"] = (.
+00022170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022180: 2020 2020 2073 6176 6564 5b30 5d20 2b20       saved[0] + 
+00022190: 636f 6c6f 7254 6578 742e 424f 4c44 202b  colorText.BOLD +
+000221a0: 2063 6f6c 6f72 5465 7874 2e47 5245 454e   colorText.GREEN
+000221b0: 202b 2022 4275 6c6c 4372 6f73 732d 3230   + "BullCross-20
+000221c0: 304d 4122 202b 2063 6f6c 6f72 5465 7874  0MA" + colorText
+000221d0: 2e45 4e44 0d0a 2020 2020 2020 2020 2020  .END..          
+000221e0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+000221f0: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
+00022200: 745b 224d 412d 5369 676e 616c 225d 203d  t["MA-Signal"] =
+00022210: 2073 6176 6564 5b31 5d20 2b20 2242 756c   saved[1] + "Bul
+00022220: 6c43 726f 7373 2d32 3030 4d41 220d 0a20  lCross-200MA".. 
+00022230: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00022240: 6152 6576 6572 7361 6c20 3d20 310d 0a20  aReversal = 1.. 
+00022250: 2020 2020 2020 2023 2046 6f72 2061 2042         # For a B
+00022260: 6561 7269 7368 2043 616e 646c 650d 0a20  earish Candle.. 
+00022270: 2020 2020 2020 2065 6c69 6620 6e6f 7420         elif not 
+00022280: 7365 6c66 2e67 6574 4361 6e64 6c65 5479  self.getCandleTy
+00022290: 7065 2864 6174 6129 3a0d 0a20 2020 2020  pe(data):..     
+000222a0: 2020 2020 2020 2023 2043 726f 7373 696e         # Crossin
+000222b0: 6720 646f 776e 2035 300d 0a20 2020 2020  g down 50..     
+000222c0: 2020 2020 2020 2069 6620 6f70 656e 203e         if open >
+000222d0: 2073 6d61 2061 6e64 2063 6c6f 7365 203c   sma and close <
+000222e0: 2073 6d61 3a0d 0a20 2020 2020 2020 2020   sma:..         
+000222f0: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+00022300: 745b 224d 412d 5369 676e 616c 225d 203d  t["MA-Signal"] =
+00022310: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+00022320: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
+00022330: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
+00022340: 4420 2b20 636f 6c6f 7254 6578 742e 4641  D + colorText.FA
+00022350: 494c 202b 2022 4265 6172 4372 6f73 732d  IL + "BearCross-
+00022360: 3530 4d41 2220 2b20 636f 6c6f 7254 6578  50MA" + colorTex
+00022370: 742e 454e 440d 0a20 2020 2020 2020 2020  t.END..         
+00022380: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+00022390: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
+000223a0: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
+000223b0: 3d20 7361 7665 645b 315d 202b 2022 4265  = saved[1] + "Be
+000223c0: 6172 4372 6f73 732d 3530 4d41 220d 0a20  arCross-50MA".. 
+000223d0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000223e0: 6152 6576 6572 7361 6c20 3d20 2d31 0d0a  aReversal = -1..
+000223f0: 2020 2020 2020 2020 2020 2020 2320 4372              # Cr
+00022400: 6f73 7369 6e67 2075 7020 3230 300d 0a20  ossing up 200.. 
+00022410: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00022420: 6f70 656e 203e 206c 6d61 2061 6e64 2063  open > lma and c
+00022430: 6c6f 7365 203c 206c 6d61 3a0d 0a20 2020  lose < lma:..   
+00022440: 2020 2020 2020 2020 2020 2020 2073 6372               scr
+00022450: 6565 6e44 6963 745b 224d 412d 5369 676e  eenDict["MA-Sign
+00022460: 616c 225d 203d 2028 0d0a 2020 2020 2020  al"] = (..      
+00022470: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+00022480: 7665 645b 305d 202b 2063 6f6c 6f72 5465  ved[0] + colorTe
+00022490: 7874 2e42 4f4c 4420 2b20 636f 6c6f 7254  xt.BOLD + colorT
+000224a0: 6578 742e 4641 494c 202b 2022 4265 6172  ext.FAIL + "Bear
+000224b0: 4372 6f73 732d 3230 304d 4122 202b 2063  Cross-200MA" + c
+000224c0: 6f6c 6f72 5465 7874 2e45 4e44 0d0a 2020  olorText.END..  
+000224d0: 2020 2020 2020 2020 2020 2020 2020 290d                ).
+000224e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000224f0: 2073 6176 6544 6963 745b 224d 412d 5369   saveDict["MA-Si
+00022500: 676e 616c 225d 203d 2073 6176 6564 5b31  gnal"] = saved[1
+00022510: 5d20 2b20 2242 6561 7243 726f 7373 2d32  ] + "BearCross-2
+00022520: 3030 4d41 220d 0a20 2020 2020 2020 2020  00MA"..         
+00022530: 2020 2020 2020 206d 6152 6576 6572 7361         maReversa
+00022540: 6c20 3d20 2d31 0d0a 2020 2020 2020 2020  l = -1..        
+00022550: 7265 7475 726e 206d 6152 6576 6572 7361  return maReversa
+00022560: 6c0d 0a0d 0a20 2020 2023 2046 696e 6420  l....    # Find 
+00022570: 4e52 7820 7261 6e67 6520 666f 7220 5265  NRx range for Re
+00022580: 7665 7273 616c 0d0a 2020 2020 6465 6620  versal..    def 
+00022590: 7661 6c69 6461 7465 4e61 7272 6f77 5261  validateNarrowRa
+000225a0: 6e67 6528 7365 6c66 2c20 6466 2c20 7363  nge(self, df, sc
+000225b0: 7265 656e 4469 6374 2c20 7361 7665 4469  reenDict, saveDi
+000225c0: 6374 2c20 6e72 3d34 293a 0d0a 2020 2020  ct, nr=4):..    
+000225d0: 2020 2020 6966 2064 6620 6973 204e 6f6e      if df is Non
+000225e0: 6520 6f72 206c 656e 2864 6629 203d 3d20  e or len(df) == 
+000225f0: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+00022600: 7265 7475 726e 2046 616c 7365 0d0a 2020  return False..  
+00022610: 2020 2020 2020 6461 7461 203d 2064 662e        data = df.
+00022620: 636f 7079 2829 0d0a 2020 2020 2020 2020  copy()..        
+00022630: 7361 7665 6420 3d20 7365 6c66 2e66 696e  saved = self.fin
+00022640: 6443 7572 7265 6e74 5361 7665 6456 616c  dCurrentSavedVal
+00022650: 7565 2873 6372 6565 6e44 6963 742c 2073  ue(screenDict, s
+00022660: 6176 6544 6963 742c 2022 5061 7474 6572  aveDict, "Patter
+00022670: 6e22 290d 0a20 2020 2020 2020 2069 6620  n")..        if 
+00022680: 504b 4461 7465 5574 696c 6974 6965 732e  PKDateUtilities.
+00022690: 6973 5472 6164 696e 6754 696d 6528 293a  isTradingTime():
+000226a0: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
+000226b0: 6e67 6544 6174 6120 3d20 6461 7461 2e68  ngeData = data.h
+000226c0: 6561 6428 6e72 202b 2031 295b 313a 5d0d  ead(nr + 1)[1:].
+000226d0: 0a20 2020 2020 2020 2020 2020 206e 6f77  .            now
+000226e0: 5f63 616e 646c 6520 3d20 6461 7461 2e68  _candle = data.h
+000226f0: 6561 6428 3129 0d0a 2020 2020 2020 2020  ead(1)..        
+00022700: 2020 2020 7261 6e67 6544 6174 615b 2252      rangeData["R
+00022710: 616e 6765 225d 203d 2061 6273 2872 616e  ange"] = abs(ran
+00022720: 6765 4461 7461 5b22 436c 6f73 6522 5d20  geData["Close"] 
+00022730: 2d20 7261 6e67 6544 6174 615b 224f 7065  - rangeData["Ope
+00022740: 6e22 5d29 0d0a 2020 2020 2020 2020 2020  n"])..          
+00022750: 2020 7265 6365 6e74 203d 2072 616e 6765    recent = range
+00022760: 4461 7461 2e68 6561 6428 3129 0d0a 2020  Data.head(1)..  
+00022770: 2020 2020 2020 2020 2020 6966 2028 0d0a            if (..
+00022780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022790: 6c65 6e28 7265 6365 6e74 2920 3d3d 2031  len(recent) == 1
+000227a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000227b0: 2020 616e 6420 7265 6365 6e74 5b22 5261    and recent["Ra
+000227c0: 6e67 6522 5d2e 696c 6f63 5b30 5d20 3d3d  nge"].iloc[0] ==
+000227d0: 2072 616e 6765 4461 7461 2e64 6573 6372   rangeData.descr
+000227e0: 6962 6528 295b 2252 616e 6765 225d 5b22  ibe()["Range"]["
+000227f0: 6d69 6e22 5d0d 0a20 2020 2020 2020 2020  min"]..         
+00022800: 2020 2029 3a0d 0a20 2020 2020 2020 2020     ):..         
+00022810: 2020 2020 2020 2069 6620 280d 0a20 2020         if (..   
+00022820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022830: 2073 656c 662e 6765 7443 616e 646c 6554   self.getCandleT
+00022840: 7970 6528 7265 6365 6e74 290d 0a20 2020  ype(recent)..   
+00022850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022860: 2061 6e64 206e 6f77 5f63 616e 646c 655b   and now_candle[
+00022870: 2243 6c6f 7365 225d 2e69 6c6f 635b 305d  "Close"].iloc[0]
+00022880: 203e 3d20 7265 6365 6e74 5b22 436c 6f73   >= recent["Clos
+00022890: 6522 5d2e 696c 6f63 5b30 5d0d 0a20 2020  e"].iloc[0]..   
+000228a0: 2020 2020 2020 2020 2020 2020 2029 3a0d               ):.
+000228b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000228c0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+000228d0: 2250 6174 7465 726e 225d 203d 2028 0d0a  "Pattern"] = (..
+000228e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000228f0: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
+00022900: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
+00022910: 4420 2b20 636f 6c6f 7254 6578 742e 4752  D + colorText.GR
+00022920: 4545 4e20 2b20 6622 4275 792d 4e52 7b6e  EEN + f"Buy-NR{n
+00022930: 727d 2220 2b20 636f 6c6f 7254 6578 742e  r}" + colorText.
+00022940: 454e 440d 0a20 2020 2020 2020 2020 2020  END..           
+00022950: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
+00022960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022970: 7361 7665 4469 6374 5b22 5061 7474 6572  saveDict["Patter
+00022980: 6e22 5d20 3d20 7361 7665 645b 315d 202b  n"] = saved[1] +
+00022990: 2066 2242 7579 2d4e 527b 6e72 7d22 0d0a   f"Buy-NR{nr}"..
+000229a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000229b0: 2020 2020 7265 7475 726e 2054 7275 650d      return True.
+000229c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000229d0: 2065 6c69 6620 280d 0a20 2020 2020 2020   elif (..       
+000229e0: 2020 2020 2020 2020 2020 2020 206e 6f74               not
+000229f0: 2073 656c 662e 6765 7443 616e 646c 6554   self.getCandleT
+00022a00: 7970 6528 7265 6365 6e74 290d 0a20 2020  ype(recent)..   
+00022a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022a20: 2061 6e64 206e 6f77 5f63 616e 646c 655b   and now_candle[
+00022a30: 2243 6c6f 7365 225d 2e69 6c6f 635b 305d  "Close"].iloc[0]
+00022a40: 203c 3d20 7265 6365 6e74 5b22 436c 6f73   <= recent["Clos
+00022a50: 6522 5d2e 696c 6f63 5b30 5d0d 0a20 2020  e"].iloc[0]..   
+00022a60: 2020 2020 2020 2020 2020 2020 2029 3a0d               ):.
+00022a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022a80: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+00022a90: 2250 6174 7465 726e 225d 203d 2028 0d0a  "Pattern"] = (..
+00022aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022ab0: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
+00022ac0: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
+00022ad0: 4420 2b20 636f 6c6f 7254 6578 742e 4641  D + colorText.FA
+00022ae0: 494c 202b 2066 2253 656c 6c2d 4e52 7b6e  IL + f"Sell-NR{n
+00022af0: 727d 2220 2b20 636f 6c6f 7254 6578 742e  r}" + colorText.
+00022b00: 454e 440d 0a20 2020 2020 2020 2020 2020  END..           
+00022b10: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
+00022b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022b30: 7361 7665 4469 6374 5b22 5061 7474 6572  saveDict["Patter
+00022b40: 6e22 5d20 3d20 7361 7665 645b 315d 202b  n"] = saved[1] +
+00022b50: 2066 2253 656c 6c2d 4e52 7b6e 727d 220d   f"Sell-NR{nr}".
+00022b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022b70: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00022b80: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00022b90: 7475 726e 2046 616c 7365 0d0a 2020 2020  turn False..    
+00022ba0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00022bb0: 2020 2020 2020 2072 616e 6765 4461 7461         rangeData
+00022bc0: 203d 2064 6174 612e 6865 6164 286e 7229   = data.head(nr)
+00022bd0: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
+00022be0: 6e67 6544 6174 612e 6c6f 635b 3a2c 2752  ngeData.loc[:,'R
+00022bf0: 616e 6765 275d 203d 2061 6273 2872 616e  ange'] = abs(ran
+00022c00: 6765 4461 7461 5b22 436c 6f73 6522 5d20  geData["Close"] 
+00022c10: 2d20 7261 6e67 6544 6174 615b 224f 7065  - rangeData["Ope
+00022c20: 6e22 5d29 0d0a 2020 2020 2020 2020 2020  n"])..          
+00022c30: 2020 7265 6365 6e74 203d 2072 616e 6765    recent = range
+00022c40: 4461 7461 2e68 6561 6428 3129 0d0a 2020  Data.head(1)..  
+00022c50: 2020 2020 2020 2020 2020 6966 2072 6563            if rec
+00022c60: 656e 745b 2252 616e 6765 225d 2e69 6c6f  ent["Range"].ilo
+00022c70: 635b 305d 203d 3d20 7261 6e67 6544 6174  c[0] == rangeDat
+00022c80: 612e 6465 7363 7269 6265 2829 5b22 5261  a.describe()["Ra
+00022c90: 6e67 6522 5d5b 226d 696e 225d 3a0d 0a20  nge"]["min"]:.. 
+00022ca0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00022cb0: 6372 6565 6e44 6963 745b 2250 6174 7465  creenDict["Patte
+00022cc0: 726e 225d 203d 2028 0d0a 2020 2020 2020  rn"] = (..      
+00022cd0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+00022ce0: 7665 645b 305d 202b 2063 6f6c 6f72 5465  ved[0] + colorTe
+00022cf0: 7874 2e42 4f4c 4420 2b20 636f 6c6f 7254  xt.BOLD + colorT
+00022d00: 6578 742e 4752 4545 4e20 2b20 6622 4e52  ext.GREEN + f"NR
+00022d10: 7b6e 727d 2220 2b20 636f 6c6f 7254 6578  {nr}" + colorTex
+00022d20: 742e 454e 440d 0a20 2020 2020 2020 2020  t.END..         
+00022d30: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+00022d40: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
+00022d50: 6374 5b22 5061 7474 6572 6e22 5d20 3d20  ct["Pattern"] = 
+00022d60: 7361 7665 645b 315d 202b 2066 224e 527b  saved[1] + f"NR{
+00022d70: 6e72 7d22 0d0a 2020 2020 2020 2020 2020  nr}"..          
+00022d80: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+00022d90: 650d 0a20 2020 2020 2020 2020 2020 2072  e..            r
+00022da0: 6574 7572 6e20 4661 6c73 650d 0a0d 0a20  eturn False.... 
+00022db0: 2020 2023 2046 696e 6420 6966 2073 746f     # Find if sto
+00022dc0: 636b 2069 7320 6e65 776c 7920 6c69 7374  ck is newly list
+00022dd0: 6564 0d0a 2020 2020 6465 6620 7661 6c69  ed..    def vali
+00022de0: 6461 7465 4e65 776c 794c 6973 7465 6428  dateNewlyListed(
+00022df0: 7365 6c66 2c20 6466 2c20 6461 7973 546f  self, df, daysTo
+00022e00: 4c6f 6f6b 6261 636b 293a 0d0a 2020 2020  Lookback):..    
+00022e10: 2020 2020 6966 2064 6620 6973 204e 6f6e      if df is Non
+00022e20: 6520 6f72 206c 656e 2864 6629 203d 3d20  e or len(df) == 
+00022e30: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+00022e40: 7265 7475 726e 2046 616c 7365 0d0a 2020  return False..  
+00022e50: 2020 2020 2020 6461 7461 203d 2064 662e        data = df.
+00022e60: 636f 7079 2829 0d0a 2020 2020 2020 2020  copy()..        
+00022e70: 6461 7973 546f 4c6f 6f6b 6261 636b 203d  daysToLookback =
+00022e80: 2069 6e74 2864 6179 7354 6f4c 6f6f 6b62   int(daysToLookb
+00022e90: 6163 6b5b 3a2d 315d 290d 0a20 2020 2020  ack[:-1])..     
+00022ea0: 2020 2072 6563 656e 7420 3d20 6461 7461     recent = data
+00022eb0: 2e68 6561 6428 3129 0d0a 2020 2020 2020  .head(1)..      
+00022ec0: 2020 6966 206c 656e 2872 6563 656e 7429    if len(recent)
+00022ed0: 203c 2031 3a0d 0a20 2020 2020 2020 2020   < 1:..         
+00022ee0: 2020 2072 6574 7572 6e20 4661 6c73 650d     return False.
+00022ef0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+00022f00: 6461 7461 2920 3c20 6461 7973 546f 4c6f  data) < daysToLo
+00022f10: 6f6b 6261 636b 2061 6e64 2028 0d0a 2020  okback and (..  
+00022f20: 2020 2020 2020 2020 2020 7265 6365 6e74            recent
+00022f30: 5b22 436c 6f73 6522 5d2e 696c 6f63 5b30  ["Close"].iloc[0
+00022f40: 5d20 213d 206e 702e 6e61 6e20 616e 6420  ] != np.nan and 
+00022f50: 7265 6365 6e74 5b22 436c 6f73 6522 5d2e  recent["Close"].
+00022f60: 696c 6f63 5b30 5d20 3e20 300d 0a20 2020  iloc[0] > 0..   
+00022f70: 2020 2020 2029 3a0d 0a20 2020 2020 2020       ):..       
+00022f80: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00022f90: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00022fa0: 2046 616c 7365 0d0a 0d0a 2020 2020 2320   False....    # 
+00022fb0: 5661 6c69 6461 7465 2069 6620 7468 6520  Validate if the 
+00022fc0: 7374 6f63 6b20 7072 6963 6573 2061 7265  stock prices are
+00022fd0: 2061 7420 6c65 6173 7420 7269 7369 6e67   at least rising
+00022fe0: 2062 7920 3225 2066 6f72 2074 6865 206c   by 2% for the l
+00022ff0: 6173 7420 3320 7365 7373 696f 6e73 0d0a  ast 3 sessions..
+00023000: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+00023010: 5072 6963 6552 6973 696e 6742 7941 744c  PriceRisingByAtL
+00023020: 6561 7374 3250 6572 6365 6e74 2873 656c  east2Percent(sel
+00023030: 662c 2064 662c 2073 6372 6565 6e44 6963  f, df, screenDic
+00023040: 742c 2073 6176 6544 6963 7429 3a0d 0a20  t, saveDict):.. 
+00023050: 2020 2020 2020 2069 6620 6466 2069 7320         if df is 
+00023060: 4e6f 6e65 206f 7220 6c65 6e28 6466 2920  None or len(df) 
+00023070: 3d3d 2030 3a0d 0a20 2020 2020 2020 2020  == 0:..         
+00023080: 2020 2072 6574 7572 6e20 4661 6c73 650d     return False.
+00023090: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+000230a0: 6466 2e63 6f70 7928 290d 0a20 2020 2020  df.copy()..     
+000230b0: 2020 2064 6174 6120 3d20 6461 7461 2e66     data = data.f
+000230c0: 696c 6c6e 6128 3029 0d0a 2020 2020 2020  illna(0)..      
+000230d0: 2020 6461 7461 203d 2064 6174 612e 7265    data = data.re
+000230e0: 706c 6163 6528 5b6e 702e 696e 662c 202d  place([np.inf, -
+000230f0: 6e70 2e69 6e66 5d2c 2030 290d 0a20 2020  np.inf], 0)..   
+00023100: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+00023110: 2e68 6561 6428 3429 0d0a 2020 2020 2020  .head(4)..      
+00023120: 2020 6966 206c 656e 2864 6174 6129 203c    if len(data) <
+00023130: 2034 3a0d 0a20 2020 2020 2020 2020 2020   4:..           
+00023140: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
+00023150: 2020 2020 2020 2064 6179 3020 3d20 6461         day0 = da
+00023160: 7461 2e69 6c6f 635b 305d 5b22 436c 6f73  ta.iloc[0]["Clos
+00023170: 6522 5d2e 6974 656d 2829 0d0a 2020 2020  e"].item()..    
+00023180: 2020 2020 6461 794d 696e 7573 3120 3d20      dayMinus1 = 
+00023190: 6461 7461 2e69 6c6f 635b 315d 5b22 436c  data.iloc[1]["Cl
+000231a0: 6f73 6522 5d2e 6974 656d 2829 0d0a 2020  ose"].item()..  
+000231b0: 2020 2020 2020 6461 794d 696e 7573 3220        dayMinus2 
+000231c0: 3d20 6461 7461 2e69 6c6f 635b 325d 5b22  = data.iloc[2]["
+000231d0: 436c 6f73 6522 5d2e 6974 656d 2829 0d0a  Close"].item()..
+000231e0: 2020 2020 2020 2020 6461 794d 696e 7573          dayMinus
+000231f0: 3320 3d20 6461 7461 2e69 6c6f 635b 335d  3 = data.iloc[3]
+00023200: 5b22 436c 6f73 6522 5d2e 6974 656d 2829  ["Close"].item()
+00023210: 0d0a 2020 2020 2020 2020 7065 7263 656e  ..        percen
+00023220: 7433 203d 2072 6f75 6e64 2828 6461 794d  t3 = round((dayM
+00023230: 696e 7573 3220 2d20 6461 794d 696e 7573  inus2 - dayMinus
+00023240: 3329 202a 2031 3030 202f 2064 6179 4d69  3) * 100 / dayMi
+00023250: 6e75 7333 2c20 3229 0d0a 2020 2020 2020  nus3, 2)..      
+00023260: 2020 7065 7263 656e 7432 203d 2072 6f75    percent2 = rou
+00023270: 6e64 2828 6461 794d 696e 7573 3120 2d20  nd((dayMinus1 - 
+00023280: 6461 794d 696e 7573 3229 202a 2031 3030  dayMinus2) * 100
+00023290: 202f 2064 6179 4d69 6e75 7332 2c20 3229   / dayMinus2, 2)
+000232a0: 0d0a 2020 2020 2020 2020 7065 7263 656e  ..        percen
+000232b0: 7431 203d 2072 6f75 6e64 2828 6461 7930  t1 = round((day0
+000232c0: 202d 2064 6179 4d69 6e75 7331 2920 2a20   - dayMinus1) * 
+000232d0: 3130 3020 2f20 6461 794d 696e 7573 312c  100 / dayMinus1,
+000232e0: 2032 290d 0a0d 0a20 2020 2020 2020 2069   2)....        i
+000232f0: 6620 7065 7263 656e 7431 203e 3d20 3220  f percent1 >= 2 
+00023300: 616e 6420 7065 7263 656e 7432 203e 3d20  and percent2 >= 
+00023310: 3220 616e 6420 7065 7263 656e 7433 203e  2 and percent3 >
+00023320: 3d20 323a 0d0a 2020 2020 2020 2020 2020  = 2:..          
+00023330: 2020 7063 745f 6368 616e 6765 5f74 6578    pct_change_tex
+00023340: 7420 3d20 280d 0a20 2020 2020 2020 2020  t = (..         
+00023350: 2020 2020 2020 2028 2225 2e31 6625 2522         ("%.1f%%"
+00023360: 2025 2070 6572 6365 6e74 3129 0d0a 2020   % percent1)..  
+00023370: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+00023380: 2822 2028 252e 3166 2525 2c22 2025 2070  (" (%.1f%%," % p
+00023390: 6572 6365 6e74 3229 0d0a 2020 2020 2020  ercent2)..      
+000233a0: 2020 2020 2020 2020 2020 2b20 2822 2025            + (" %
+000233b0: 2e31 6625 2529 2220 2520 7065 7263 656e  .1f%%)" % percen
+000233c0: 7433 290d 0a20 2020 2020 2020 2020 2020  t3)..           
+000233d0: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+000233e0: 7361 7665 4469 6374 5b22 2543 686e 6722  saveDict["%Chng"
+000233f0: 5d20 3d20 7063 745f 6368 616e 6765 5f74  ] = pct_change_t
+00023400: 6578 740d 0a20 2020 2020 2020 2020 2020  ext..           
+00023410: 2073 6372 6565 6e44 6963 745b 2225 4368   screenDict["%Ch
+00023420: 6e67 225d 203d 2063 6f6c 6f72 5465 7874  ng"] = colorText
+00023430: 2e47 5245 454e 202b 2070 6374 5f63 6861  .GREEN + pct_cha
+00023440: 6e67 655f 7465 7874 202b 2063 6f6c 6f72  nge_text + color
+00023450: 5465 7874 2e45 4e44 0d0a 2020 2020 2020  Text.END..      
+00023460: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+00023470: 6520 616e 6420 7365 6c66 2e67 6574 4361  e and self.getCa
+00023480: 6e64 6c65 5479 7065 2864 6174 612e 6865  ndleType(data.he
+00023490: 6164 2831 2929 0d0a 2020 2020 2020 2020  ad(1))..        
+000234a0: 7265 7475 726e 2046 616c 7365 0d0a 0d0a  return False....
+000234b0: 2020 2020 2340 6d65 6173 7572 655f 7469      #@measure_ti
+000234c0: 6d65 0d0a 2020 2020 2320 7661 6c69 6461  me..    # valida
+000234d0: 7465 2069 6620 5253 4920 6973 2077 6974  te if RSI is wit
+000234e0: 6869 6e20 6769 7665 6e20 7261 6e67 650d  hin given range.
+000234f0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+00023500: 6552 5349 2873 656c 662c 2064 662c 2073  eRSI(self, df, s
+00023510: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
+00023520: 6963 742c 206d 696e 5253 492c 206d 6178  ict, minRSI, max
+00023530: 5253 492c 7273 694b 6579 3d22 5253 4922  RSI,rsiKey="RSI"
+00023540: 293a 0d0a 2020 2020 2020 2020 6966 2064  ):..        if d
+00023550: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
+00023560: 2864 6629 203d 3d20 303a 0d0a 2020 2020  (df) == 0:..    
+00023570: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+00023580: 616c 7365 0d0a 2020 2020 2020 2020 6966  alse..        if
+00023590: 2072 7369 4b65 7920 6e6f 7420 696e 2064   rsiKey not in d
+000235a0: 662e 636f 6c75 6d6e 733a 0d0a 2020 2020  f.columns:..    
+000235b0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+000235c0: 616c 7365 0d0a 2020 2020 2020 2020 6461  alse..        da
+000235d0: 7461 203d 2064 662e 636f 7079 2829 0d0a  ta = df.copy()..
+000235e0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+000235f0: 6174 612e 6669 6c6c 6e61 2830 290d 0a20  ata.fillna(0).. 
+00023600: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
+00023610: 7461 2e72 6570 6c61 6365 285b 6e70 2e69  ta.replace([np.i
+00023620: 6e66 2c20 2d6e 702e 696e 665d 2c20 3029  nf, -np.inf], 0)
+00023630: 0d0a 2020 2020 2020 2020 7273 6920 3d20  ..        rsi = 
+00023640: 696e 7428 6461 7461 2e68 6561 6428 3129  int(data.head(1)
+00023650: 5b72 7369 4b65 795d 2e69 6c6f 635b 305d  [rsiKey].iloc[0]
+00023660: 290d 0a20 2020 2020 2020 2073 6176 6544  )..        saveD
+00023670: 6963 745b 7273 694b 6579 5d20 3d20 7273  ict[rsiKey] = rs
+00023680: 690d 0a20 2020 2020 2020 2023 2068 7474  i..        # htt
+00023690: 7073 3a2f 2f63 6861 7274 696e 6b2e 636f  ps://chartink.co
+000236a0: 6d2f 7363 7265 656e 6572 2f72 7369 2d73  m/screener/rsi-s
+000236b0: 6372 6565 6e69 6e67 0d0a 2020 2020 2020  creening..      
+000236c0: 2020 6966 2072 7369 3e20 3020 616e 6420    if rsi> 0 and 
+000236d0: 7273 6920 3e3d 206d 696e 5253 4920 616e  rsi >= minRSI an
+000236e0: 6420 7273 6920 3c3d 206d 6178 5253 493a  d rsi <= maxRSI:
+000236f0: 2020 2320 6f72 2028 7273 6920 3c3d 2037    # or (rsi <= 7
+00023700: 3120 616e 6420 7273 6920 3e3d 2036 3729  1 and rsi >= 67)
+00023710: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00023720: 6372 6565 6e44 6963 745b 7273 694b 6579  creenDict[rsiKey
+00023730: 5d20 3d20 280d 0a20 2020 2020 2020 2020  ] = (..         
+00023740: 2020 2020 2020 2063 6f6c 6f72 5465 7874         colorText
+00023750: 2e42 4f4c 4420 2b20 636f 6c6f 7254 6578  .BOLD + colorTex
+00023760: 742e 4752 4545 4e20 2b20 7374 7228 7273  t.GREEN + str(rs
+00023770: 6929 202b 2063 6f6c 6f72 5465 7874 2e45  i) + colorText.E
+00023780: 4e44 0d0a 2020 2020 2020 2020 2020 2020  ND..            
+00023790: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
+000237a0: 6574 7572 6e20 5472 7565 2069 6620 2872  eturn True if (r
+000237b0: 7369 4b65 7920 3d3d 2022 5253 4969 2229  siKey == "RSIi")
+000237c0: 2065 6c73 6520 2873 656c 662e 7661 6c69   else (self.vali
+000237d0: 6461 7465 5253 4928 6466 2c20 7363 7265  dateRSI(df, scre
+000237e0: 656e 4469 6374 2c20 7361 7665 4469 6374  enDict, saveDict
+000237f0: 2c20 6d69 6e52 5349 2c20 6d61 7852 5349  , minRSI, maxRSI
+00023800: 2c72 7369 4b65 793d 2252 5349 6922 2920  ,rsiKey="RSIi") 
+00023810: 6f72 2054 7275 6529 0d0a 2020 2020 2020  or True)..      
+00023820: 2020 7363 7265 656e 4469 6374 5b72 7369    screenDict[rsi
+00023830: 4b65 795d 203d 2063 6f6c 6f72 5465 7874  Key] = colorText
+00023840: 2e42 4f4c 4420 2b20 636f 6c6f 7254 6578  .BOLD + colorTex
+00023850: 742e 4641 494c 202b 2073 7472 2872 7369  t.FAIL + str(rsi
+00023860: 2920 2b20 636f 6c6f 7254 6578 742e 454e  ) + colorText.EN
+00023870: 440d 0a20 2020 2020 2020 2023 2049 6620  D..        # If 
+00023880: 6569 7468 6572 2064 6169 6c79 206f 7220  either daily or 
+00023890: 696e 7472 6164 6179 2052 5349 2063 6f6d  intraday RSI com
+000238a0: 6573 2077 6974 6869 6e20 7261 6e67 653f  es within range?
+000238b0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000238c0: 2046 616c 7365 2069 6620 2872 7369 4b65   False if (rsiKe
+000238d0: 7920 3d3d 2022 5253 4969 2229 2065 6c73  y == "RSIi") els
+000238e0: 6520 2873 656c 662e 7661 6c69 6461 7465  e (self.validate
+000238f0: 5253 4928 6466 2c20 7363 7265 656e 4469  RSI(df, screenDi
+00023900: 6374 2c20 7361 7665 4469 6374 2c20 6d69  ct, saveDict, mi
+00023910: 6e52 5349 2c20 6d61 7852 5349 2c72 7369  nRSI, maxRSI,rsi
+00023920: 4b65 793d 2252 5349 6922 2929 0d0a 0d0a  Key="RSIi"))....
+00023930: 2020 2020 2320 5661 6c69 6461 7465 2069      # Validate i
+00023940: 6620 7468 6520 7374 6f63 6b20 6973 2062  f the stock is b
+00023950: 756c 6c69 7368 2069 6e20 7468 6520 7368  ullish in the sh
+00023960: 6f72 7420 7465 726d 0d0a 2020 2020 6465  ort term..    de
+00023970: 6620 7661 6c69 6461 7465 5368 6f72 7454  f validateShortT
+00023980: 6572 6d42 756c 6c69 7368 2873 656c 662c  ermBullish(self,
+00023990: 2064 662c 2073 6372 6565 6e44 6963 742c   df, screenDict,
+000239a0: 2073 6176 6544 6963 7429 3a0d 0a20 2020   saveDict):..   
+000239b0: 2020 2020 2069 6620 6466 2069 7320 4e6f       if df is No
+000239c0: 6e65 206f 7220 6c65 6e28 6466 2920 3d3d  ne or len(df) ==
+000239d0: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
+000239e0: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
+000239f0: 2020 2020 2020 2064 6174 6120 3d20 6466         data = df
+00023a00: 2e63 6f70 7928 290d 0a20 2020 2020 2020  .copy()..       
+00023a10: 2023 2068 7474 7073 3a2f 2f63 6861 7274   # https://chart
+00023a20: 696e 6b2e 636f 6d2f 7363 7265 656e 6572  ink.com/screener
+00023a30: 2f73 686f 7274 2d74 6572 6d2d 6275 6c6c  /short-term-bull
+00023a40: 6973 680d 0a20 2020 2020 2020 2064 6174  ish..        dat
+00023a50: 6120 3d20 6461 7461 2e66 696c 6c6e 6128  a = data.fillna(
+00023a60: 3029 0d0a 2020 2020 2020 2020 6461 7461  0)..        data
+00023a70: 203d 2064 6174 612e 7265 706c 6163 6528   = data.replace(
+00023a80: 5b6e 702e 696e 662c 202d 6e70 2e69 6e66  [np.inf, -np.inf
+00023a90: 5d2c 2030 290d 0a20 2020 2020 2020 2072  ], 0)..        r
+00023aa0: 6563 656e 7420 3d20 6461 7461 2e68 6561  ecent = data.hea
+00023ab0: 6428 3129 0d0a 2020 2020 2020 2020 666b  d(1)..        fk
+00023ac0: 203d 2030 2069 6620 6c65 6e28 6461 7461   = 0 if len(data
+00023ad0: 2920 3c20 3320 656c 7365 206e 702e 726f  ) < 3 else np.ro
+00023ae0: 756e 6428 6461 7461 5b22 4641 5354 4b22  und(data["FASTK"
+00023af0: 5d2e 696c 6f63 5b32 5d2c 2035 290d 0a20  ].iloc[2], 5).. 
+00023b00: 2020 2020 2020 2023 2052 6576 6572 7365         # Reverse
+00023b10: 2074 6865 2064 6174 6166 7261 6d65 2066   the dataframe f
+00023b20: 6f72 2069 6368 696d 6f6b 7520 6361 6c63  or ichimoku calc
+00023b30: 756c 6174 696f 6e73 2077 6974 6820 6461  ulations with da
+00023b40: 7465 2069 6e20 6173 6365 6e64 696e 6720  te in ascending 
+00023b50: 6f72 6465 720d 0a20 2020 2020 2020 2064  order..        d
+00023b60: 665f 6e65 7720 3d20 6461 7461 5b3a 3a2d  f_new = data[::-
+00023b70: 315d 0d0a 2020 2020 2020 2020 7472 793a  1]..        try:
+00023b80: 0d0a 2020 2020 2020 2020 2020 2020 6466  ..            df
+00023b90: 5f69 6368 6920 3d20 6466 5f6e 6577 2e72  _ichi = df_new.r
+00023ba0: 656e 616d 6528 0d0a 2020 2020 2020 2020  ename(..        
+00023bb0: 2020 2020 2020 2020 636f 6c75 6d6e 733d          columns=
+00023bc0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
+00023bd0: 2020 2020 2020 2022 4f70 656e 223a 2022         "Open": "
+00023be0: 6f70 656e 222c 0d0a 2020 2020 2020 2020  open",..        
+00023bf0: 2020 2020 2020 2020 2020 2020 2248 6967              "Hig
+00023c00: 6822 3a20 2268 6967 6822 2c0d 0a20 2020  h": "high",..   
+00023c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023c20: 2022 4c6f 7722 3a20 226c 6f77 222c 0d0a   "Low": "low",..
+00023c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023c40: 2020 2020 2243 6c6f 7365 223a 2022 636c      "Close": "cl
+00023c50: 6f73 6522 2c0d 0a20 2020 2020 2020 2020  ose",..         
+00023c60: 2020 2020 2020 2020 2020 2022 566f 6c75             "Volu
+00023c70: 6d65 223a 2022 766f 6c75 6d65 222c 0d0a  me": "volume",..
+00023c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023c90: 7d0d 0a20 2020 2020 2020 2020 2020 2029  }..            )
+00023ca0: 0d0a 2020 2020 2020 2020 2020 2020 6963  ..            ic
+00023cb0: 6869 203d 2070 6b74 616c 6962 2e69 6368  hi = pktalib.ich
+00023cc0: 696d 6f6b 7528 6466 5f69 6368 692c 2039  imoku(df_ichi, 9
+00023cd0: 2c20 3236 2c20 3532 2c20 3236 290d 0a20  , 26, 52, 26).. 
+00023ce0: 2020 2020 2020 2020 2020 2069 6620 6963             if ic
+00023cf0: 6869 2069 7320 4e6f 6e65 3a0d 0a20 2020  hi is None:..   
+00023d00: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00023d10: 7572 6e20 4661 6c73 650d 0a20 2020 2020  urn False..     
+00023d20: 2020 2020 2020 2064 665f 6e65 7720 3d20         df_new = 
+00023d30: 7064 2e63 6f6e 6361 7428 5b64 665f 6e65  pd.concat([df_ne
+00023d40: 772c 2069 6368 695d 2c20 6178 6973 3d31  w, ichi], axis=1
+00023d50: 290d 0a20 2020 2020 2020 2020 2020 2023  )..            #
+00023d60: 2052 6576 6572 7365 2061 6761 696e 2074   Reverse again t
+00023d70: 6f20 6765 7420 7468 6520 6d6f 7374 2072  o get the most r
+00023d80: 6563 656e 7420 6461 7465 206f 6e20 746f  ecent date on to
+00023d90: 700d 0a20 2020 2020 2020 2020 2020 2064  p..            d
+00023da0: 665f 6e65 7720 3d20 6466 5f6e 6577 5b3a  f_new = df_new[:
+00023db0: 3a2d 315d 0d0a 2020 2020 2020 2020 2020  :-1]..          
+00023dc0: 2020 6466 5f6e 6577 203d 2064 665f 6e65    df_new = df_ne
+00023dd0: 772e 6865 6164 2831 290d 0a20 2020 2020  w.head(1)..     
+00023de0: 2020 2020 2020 2064 665f 6e65 775b 2263         df_new["c
+00023df0: 6c6f 7564 5f67 7265 656e 225d 203d 2064  loud_green"] = d
+00023e00: 665f 6e65 775b 2249 5341 5f39 225d 2e69  f_new["ISA_9"].i
+00023e10: 6c6f 635b 305d 203e 2064 665f 6e65 775b  loc[0] > df_new[
+00023e20: 2249 5342 5f32 3622 5d2e 696c 6f63 5b30  "ISB_26"].iloc[0
+00023e30: 5d0d 0a20 2020 2020 2020 2020 2020 2064  ]..            d
+00023e40: 665f 6e65 775b 2263 6c6f 7564 5f72 6564  f_new["cloud_red
+00023e50: 225d 203d 2064 665f 6e65 775b 2249 5342  "] = df_new["ISB
+00023e60: 5f32 3622 5d2e 696c 6f63 5b30 5d20 3e20  _26"].iloc[0] > 
+00023e70: 6466 5f6e 6577 5b22 4953 415f 3922 5d2e  df_new["ISA_9"].
+00023e80: 696c 6f63 5b30 5d0d 0a20 2020 2020 2020  iloc[0]..       
+00023e90: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00023ea0: 6e20 6173 2065 3a20 2023 2070 7261 676d  n as e:  # pragm
+00023eb0: 613a 206e 6f20 636f 7665 720d 0a20 2020  a: no cover..   
+00023ec0: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
+00023ed0: 6661 756c 745f 6c6f 6767 6572 2e64 6562  fault_logger.deb
+00023ee0: 7567 2865 2c20 6578 635f 696e 666f 3d54  ug(e, exc_info=T
+00023ef0: 7275 6529 0d0a 2020 2020 2020 2020 2020  rue)..          
+00023f00: 2020 7061 7373 0d0a 2020 2020 2020 2020    pass..        
+00023f10: 6162 6f76 6543 6c6f 7564 546f 7020 3d20  aboveCloudTop = 
+00023f20: 4661 6c73 650d 0a20 2020 2020 2020 2023  False..        #
+00023f30: 2062 6173 656c 696e 6520 3e20 636c 6f75   baseline > clou
+00023f40: 6420 746f 7020 2863 6c6f 7564 2069 7320  d top (cloud is 
+00023f50: 626f 756e 6420 6279 2073 7061 6e20 6120  bound by span a 
+00023f60: 616e 6420 7370 616e 2062 2920 616e 6420  and span b) and 
+00023f70: 636c 6f73 6520 6973 203e 2063 6c6f 7564  close is > cloud
+00023f80: 2074 6f70 0d0a 2020 2020 2020 2020 6966   top..        if
+00023f90: 2064 665f 6e65 775b 2263 6c6f 7564 5f67   df_new["cloud_g
+00023fa0: 7265 656e 225d 2e69 6c6f 635b 305d 3a0d  reen"].iloc[0]:.
+00023fb0: 0a20 2020 2020 2020 2020 2020 2061 626f  .            abo
+00023fc0: 7665 436c 6f75 6454 6f70 203d 2028 0d0a  veCloudTop = (..
+00023fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023fe0: 6466 5f6e 6577 5b22 494b 535f 3236 225d  df_new["IKS_26"]
+00023ff0: 2e69 6c6f 635b 305d 203e 2064 665f 6e65  .iloc[0] > df_ne
+00024000: 775b 2249 5341 5f39 225d 2e69 6c6f 635b  w["ISA_9"].iloc[
+00024010: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
+00024020: 2020 2020 616e 6420 7265 6365 6e74 5b22      and recent["
+00024030: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d20  Close"].iloc[0] 
+00024040: 3e20 6466 5f6e 6577 5b22 4953 415f 3922  > df_new["ISA_9"
+00024050: 5d2e 696c 6f63 5b30 5d0d 0a20 2020 2020  ].iloc[0]..     
+00024060: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+00024070: 2020 656c 6966 2064 665f 6e65 775b 2263    elif df_new["c
+00024080: 6c6f 7564 5f72 6564 225d 2e69 6c6f 635b  loud_red"].iloc[
+00024090: 305d 3a0d 0a20 2020 2020 2020 2020 2020  0]:..           
+000240a0: 2061 626f 7665 436c 6f75 6454 6f70 203d   aboveCloudTop =
+000240b0: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+000240c0: 2020 2020 6466 5f6e 6577 5b22 494b 535f      df_new["IKS_
+000240d0: 3236 225d 2e69 6c6f 635b 305d 203e 2064  26"].iloc[0] > d
+000240e0: 665f 6e65 775b 2249 5342 5f32 3622 5d2e  f_new["ISB_26"].
+000240f0: 696c 6f63 5b30 5d0d 0a20 2020 2020 2020  iloc[0]..       
+00024100: 2020 2020 2020 2020 2061 6e64 2072 6563           and rec
+00024110: 656e 745b 2243 6c6f 7365 225d 2e69 6c6f  ent["Close"].ilo
+00024120: 635b 305d 203e 2064 665f 6e65 775b 2249  c[0] > df_new["I
+00024130: 5342 5f32 3622 5d2e 696c 6f63 5b30 5d0d  SB_26"].iloc[0].
+00024140: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
+00024150: 0d0a 2020 2020 2020 2020 2320 4c61 7465  ..        # Late
+00024160: 7374 2049 6368 696d 6f6b 7520 6261 7365  st Ichimoku base
+00024170: 6c69 6e65 2069 7320 3c20 6c61 7465 7374  line is < latest
+00024180: 2049 6368 696d 6f6b 7520 636f 6e76 6572   Ichimoku conver
+00024190: 7369 6f6e 206c 696e 650d 0a20 2020 2020  sion line..     
+000241a0: 2020 2069 6620 6162 6f76 6543 6c6f 7564     if aboveCloud
+000241b0: 546f 7020 616e 6420 6466 5f6e 6577 5b22  Top and df_new["
+000241c0: 494b 535f 3236 225d 2e69 6c6f 635b 305d  IKS_26"].iloc[0]
+000241d0: 203c 2064 665f 6e65 775b 2249 5453 5f39   < df_new["ITS_9
+000241e0: 225d 2e69 6c6f 635b 305d 3a0d 0a20 2020  "].iloc[0]:..   
+000241f0: 2020 2020 2020 2020 2023 2053 746f 6368           # Stoch
+00024200: 5253 4920 6372 6f73 7365 6420 3230 2061  RSI crossed 20 a
+00024210: 6e64 2052 5349 203e 2035 300d 0a20 2020  nd RSI > 50..   
+00024220: 2020 2020 2020 2020 2069 6620 666b 203e           if fk >
+00024230: 2032 3020 616e 6420 7265 6365 6e74 5b22   20 and recent["
+00024240: 5253 4922 5d2e 696c 6f63 5b30 5d20 3e20  RSI"].iloc[0] > 
+00024250: 3530 3a0d 0a20 2020 2020 2020 2020 2020  50:..           
+00024260: 2020 2020 2023 2063 6f6e 6469 7469 6f6e       # condition
+00024270: 206f 6620 6372 6f73 7369 6e67 2074 6865   of crossing the
+00024280: 2053 746f 6368 5253 4920 6d61 696e 2073   StochRSI main s
+00024290: 6967 6e61 6c20 6c69 6e65 2066 726f 6d20  ignal line from 
+000242a0: 626f 7474 6f6d 2074 6f20 746f 700d 0a20  bottom to top.. 
+000242b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000242c0: 6620 280d 0a20 2020 2020 2020 2020 2020  f (..           
+000242d0: 2020 2020 2020 2020 2064 6174 615b 2246           data["F
+000242e0: 4153 5444 225d 2e69 6c6f 635b 3130 305d  ASTD"].iloc[100]
+000242f0: 203c 2064 6174 615b 2246 4153 544b 225d   < data["FASTK"]
+00024300: 2e69 6c6f 635b 3130 305d 0d0a 2020 2020  .iloc[100]..    
+00024310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024320: 616e 6420 6461 7461 5b22 4641 5354 4422  and data["FASTD"
+00024330: 5d2e 696c 6f63 5b31 3031 5d20 3e20 6461  ].iloc[101] > da
+00024340: 7461 5b22 4641 5354 4b22 5d2e 696c 6f63  ta["FASTK"].iloc
+00024350: 5b31 3031 5d0d 0a20 2020 2020 2020 2020  [101]..         
+00024360: 2020 2020 2020 2029 3a0d 0a20 2020 2020         ):..     
+00024370: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00024380: 2063 6c6f 7365 203e 2035 3020 7065 7269   close > 50 peri
+00024390: 6f64 2053 4d41 2f45 4d41 2061 6e64 2032  od SMA/EMA and 2
+000243a0: 3030 2070 6572 696f 6420 534d 412f 454d  00 period SMA/EM
+000243b0: 410d 0a20 2020 2020 2020 2020 2020 2020  A..             
+000243c0: 2020 2020 2020 2069 6620 280d 0a20 2020         if (..   
+000243d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000243e0: 2020 2020 2072 6563 656e 745b 2253 534d       recent["SSM
+000243f0: 4122 5d2e 696c 6f63 5b30 5d20 3e20 7265  A"].iloc[0] > re
+00024400: 6365 6e74 5b22 534d 4122 5d2e 696c 6f63  cent["SMA"].iloc
+00024410: 5b30 5d0d 0a20 2020 2020 2020 2020 2020  [0]..           
+00024420: 2020 2020 2020 2020 2020 2020 2061 6e64               and
+00024430: 2072 6563 656e 745b 2243 6c6f 7365 225d   recent["Close"]
+00024440: 2e69 6c6f 635b 305d 203e 2072 6563 656e  .iloc[0] > recen
+00024450: 745b 2253 534d 4122 5d2e 696c 6f63 5b30  t["SSMA"].iloc[0
+00024460: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00024470: 2020 2020 2020 2020 2020 2061 6e64 2072             and r
+00024480: 6563 656e 745b 2243 6c6f 7365 225d 2e69  ecent["Close"].i
+00024490: 6c6f 635b 305d 203e 2072 6563 656e 745b  loc[0] > recent[
+000244a0: 224c 4d41 225d 2e69 6c6f 635b 305d 0d0a  "LMA"].iloc[0]..
+000244b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000244c0: 2020 2020 293a 0d0a 2020 2020 2020 2020      ):..        
+000244d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000244e0: 7361 7665 6420 3d20 7365 6c66 2e66 696e  saved = self.fin
+000244f0: 6443 7572 7265 6e74 5361 7665 6456 616c  dCurrentSavedVal
+00024500: 7565 2873 6372 6565 6e44 6963 742c 7361  ue(screenDict,sa
+00024510: 7665 4469 6374 2c22 4d41 2d53 6967 6e61  veDict,"MA-Signa
+00024520: 6c22 290d 0a20 2020 2020 2020 2020 2020  l")..           
+00024530: 2020 2020 2020 2020 2020 2020 2073 6372               scr
+00024540: 6565 6e44 6963 745b 224d 412d 5369 676e  eenDict["MA-Sign
+00024550: 616c 225d 203d 2028 0d0a 2020 2020 2020  al"] = (..      
+00024560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024570: 2020 2020 2020 7361 7665 645b 305d 202b        saved[0] +
+00024580: 2063 6f6c 6f72 5465 7874 2e42 4f4c 4420   colorText.BOLD 
+00024590: 2b20 636f 6c6f 7254 6578 742e 4752 4545  + colorText.GREE
+000245a0: 4e20 2b20 2242 756c 6c69 7368 2220 2b20  N + "Bullish" + 
+000245b0: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
+000245c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000245d0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+000245e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000245f0: 2020 7361 7665 4469 6374 5b22 4d41 2d53    saveDict["MA-S
+00024600: 6967 6e61 6c22 5d20 3d20 7361 7665 645b  ignal"] = saved[
+00024610: 315d 202b 2022 4275 6c6c 6973 6822 0d0a  1] + "Bullish"..
+00024620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024630: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+00024640: 7275 650d 0a20 2020 2020 2020 2072 6574  rue..        ret
+00024650: 7572 6e20 4661 6c73 650d 0a0d 0a20 2020  urn False....   
+00024660: 2023 2056 616c 6964 6174 6520 5650 430d   # Validate VPC.
+00024670: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+00024680: 6556 4350 280d 0a20 2020 2020 2020 2073  eVCP(..        s
+00024690: 656c 662c 2064 662c 2073 6372 6565 6e44  elf, df, screenD
+000246a0: 6963 742c 2073 6176 6544 6963 742c 2073  ict, saveDict, s
+000246b0: 746f 636b 4e61 6d65 3d4e 6f6e 652c 2077  tockName=None, w
+000246c0: 696e 646f 773d 332c 2070 6572 6365 6e74  indow=3, percent
+000246d0: 6167 6546 726f 6d54 6f70 3d33 0d0a 2020  ageFromTop=3..  
+000246e0: 2020 293a 0d0a 2020 2020 2020 2020 6966    ):..        if
+000246f0: 2064 6620 6973 204e 6f6e 6520 6f72 206c   df is None or l
+00024700: 656e 2864 6629 203d 3d20 303a 0d0a 2020  en(df) == 0:..  
+00024710: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00024720: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+00024730: 6461 7461 203d 2064 662e 636f 7079 2829  data = df.copy()
+00024740: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
+00024750: 2020 2020 2020 2020 2020 2020 7065 7263              perc
+00024760: 656e 7461 6765 4672 6f6d 546f 7020 2f3d  entageFromTop /=
+00024770: 2031 3030 0d0a 2020 2020 2020 2020 2020   100..          
+00024780: 2020 6461 7461 2e72 6573 6574 5f69 6e64    data.reset_ind
+00024790: 6578 2869 6e70 6c61 6365 3d54 7275 6529  ex(inplace=True)
+000247a0: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
+000247b0: 7461 2e72 656e 616d 6528 636f 6c75 6d6e  ta.rename(column
+000247c0: 733d 7b22 696e 6465 7822 3a20 2244 6174  s={"index": "Dat
+000247d0: 6522 7d2c 2069 6e70 6c61 6365 3d54 7275  e"}, inplace=Tru
+000247e0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+000247f0: 6461 7461 5b22 746f 7073 225d 203d 2028  data["tops"] = (
+00024800: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00024810: 2020 6461 7461 5b22 4869 6768 225d 0d0a    data["High"]..
+00024820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024830: 2e69 6c6f 635b 0d0a 2020 2020 2020 2020  .iloc[..        
+00024840: 2020 2020 2020 2020 2020 2020 6c69 7374              list
+00024850: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00024860: 2020 2020 2020 2020 2020 2070 6b74 616c             pktal
+00024870: 6962 2e61 7267 7265 6c65 7874 7265 6d61  ib.argrelextrema
+00024880: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00024890: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000248a0: 702e 6172 7261 7928 6461 7461 5b22 4869  p.array(data["Hi
+000248b0: 6768 225d 292c 206e 702e 6772 6561 7465  gh"]), np.greate
+000248c0: 725f 6571 7561 6c2c 206f 7264 6572 3d77  r_equal, order=w
+000248d0: 696e 646f 770d 0a20 2020 2020 2020 2020  indow..         
+000248e0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+000248f0: 5b30 5d0d 0a20 2020 2020 2020 2020 2020  [0]..           
+00024900: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
+00024910: 2020 2020 2020 2020 2020 2020 5d0d 0a20              ].. 
+00024920: 2020 2020 2020 2020 2020 2020 2020 202e                 .
+00024930: 6865 6164 2834 290d 0a20 2020 2020 2020  head(4)..       
+00024940: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00024950: 2020 2020 6461 7461 5b22 626f 7473 225d      data["bots"]
+00024960: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
+00024970: 2020 2020 2020 6461 7461 5b22 4c6f 7722        data["Low"
+00024980: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00024990: 2020 202e 696c 6f63 5b0d 0a20 2020 2020     .iloc[..     
+000249a0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+000249b0: 6973 7428 0d0a 2020 2020 2020 2020 2020  ist(..          
+000249c0: 2020 2020 2020 2020 2020 2020 2020 706b                pk
+000249d0: 7461 6c69 622e 6172 6772 656c 6578 7472  talib.argrelextr
+000249e0: 656d 6128 0d0a 2020 2020 2020 2020 2020  ema(..          
+000249f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024a00: 2020 6e70 2e61 7272 6179 2864 6174 615b    np.array(data[
+00024a10: 224c 6f77 225d 292c 206e 702e 6c65 7373  "Low"]), np.less
+00024a20: 5f65 7175 616c 2c20 6f72 6465 723d 7769  _equal, order=wi
+00024a30: 6e64 6f77 0d0a 2020 2020 2020 2020 2020  ndow..          
+00024a40: 2020 2020 2020 2020 2020 2020 2020 295b                )[
+00024a50: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
+00024a60: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+00024a70: 2020 2020 2020 2020 2020 205d 0d0a 2020             ]..  
+00024a80: 2020 2020 2020 2020 2020 2020 2020 2e68                .h
+00024a90: 6561 6428 3429 0d0a 2020 2020 2020 2020  ead(4)..        
+00024aa0: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+00024ab0: 2020 2064 6174 6120 3d20 6461 7461 2e66     data = data.f
+00024ac0: 696c 6c6e 6128 3029 0d0a 2020 2020 2020  illna(0)..      
+00024ad0: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
+00024ae0: 612e 7265 706c 6163 6528 5b6e 702e 696e  a.replace([np.in
+00024af0: 662c 202d 6e70 2e69 6e66 5d2c 2030 290d  f, -np.inf], 0).
+00024b00: 0a20 2020 2020 2020 2020 2020 2074 6f70  .            top
+00024b10: 7320 3d20 6461 7461 5b64 6174 612e 746f  s = data[data.to
+00024b20: 7073 203e 2030 5d0d 0a20 2020 2020 2020  ps > 0]..       
+00024b30: 2020 2020 2023 2062 6f74 7320 3d20 6461       # bots = da
+00024b40: 7461 5b64 6174 612e 626f 7473 203e 2030  ta[data.bots > 0
+00024b50: 5d0d 0a20 2020 2020 2020 2020 2020 2068  ]..            h
+00024b60: 6967 6865 7374 546f 7020 3d20 726f 756e  ighestTop = roun
+00024b70: 6428 746f 7073 2e64 6573 6372 6962 6528  d(tops.describe(
+00024b80: 295b 2248 6967 6822 5d5b 226d 6178 225d  )["High"]["max"]
+00024b90: 2c20 3129 0d0a 2020 2020 2020 2020 2020  , 1)..          
+00024ba0: 2020 6669 6c74 6572 6564 546f 7073 203d    filteredTops =
+00024bb0: 2074 6f70 735b 0d0a 2020 2020 2020 2020   tops[..        
+00024bc0: 2020 2020 2020 2020 746f 7073 2e74 6f70          tops.top
+00024bd0: 7320 3e20 2868 6967 6865 7374 546f 7020  s > (highestTop 
+00024be0: 2d20 2868 6967 6865 7374 546f 7020 2a20  - (highestTop * 
+00024bf0: 7065 7263 656e 7461 6765 4672 6f6d 546f  percentageFromTo
+00024c00: 7029 290d 0a20 2020 2020 2020 2020 2020  p))..           
+00024c10: 205d 0d0a 2020 2020 2020 2020 2020 2020   ]..            
+00024c20: 6966 2066 696c 7465 7265 6454 6f70 732e  if filteredTops.
+00024c30: 6571 7561 6c73 2874 6f70 7329 3a20 2023  equals(tops):  #
+00024c40: 2054 6f70 7320 6172 6520 696e 2074 6865   Tops are in the
+00024c50: 2072 616e 6765 0d0a 2020 2020 2020 2020   range..        
+00024c60: 2020 2020 2020 2020 6c6f 7750 6f69 6e74          lowPoint
+00024c70: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+00024c80: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00024c90: 2072 616e 6765 286c 656e 2874 6f70 7329   range(len(tops)
+00024ca0: 202d 2031 293a 0d0a 2020 2020 2020 2020   - 1):..        
+00024cb0: 2020 2020 2020 2020 2020 2020 656e 6444              endD
+00024cc0: 6174 6520 3d20 746f 7073 2e69 6c6f 635b  ate = tops.iloc[
+00024cd0: 695d 5b22 4461 7465 225d 0d0a 2020 2020  i]["Date"]..    
+00024ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024cf0: 7374 6172 7444 6174 6520 3d20 746f 7073  startDate = tops
+00024d00: 2e69 6c6f 635b 6920 2b20 315d 5b22 4461  .iloc[i + 1]["Da
+00024d10: 7465 225d 0d0a 2020 2020 2020 2020 2020  te"]..          
+00024d20: 2020 2020 2020 2020 2020 6c6f 7750 6f69            lowPoi
+00024d30: 6e74 732e 6170 7065 6e64 280d 0a20 2020  nts.append(..   
+00024d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024d50: 2020 2020 2064 6174 615b 0d0a 2020 2020       data[..    
 00024d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024d70: 7363 7265 656e 4469 6374 5b22 5061 7474  screenDict["Patt
-00024d80: 6572 6e22 5d20 3d20 280d 0a20 2020 2020  ern"] = (..     
-00024d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024da0: 2020 2073 6176 6564 5b30 5d20 0d0a 2020     saved[0] ..  
+00024d70: 2020 2020 2020 2020 2864 6174 612e 4461          (data.Da
+00024d80: 7465 203e 3d20 7374 6172 7444 6174 6529  te >= startDate)
+00024d90: 2026 2028 6461 7461 2e44 6174 6520 3c3d   & (data.Date <=
+00024da0: 2065 6e64 4461 7465 290d 0a20 2020 2020   endDate)..     
 00024db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024dc0: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
-00024dd0: 742e 424f 4c44 0d0a 2020 2020 2020 2020  t.BOLD..        
+00024dc0: 2020 205d 2e64 6573 6372 6962 6528 295b     ].describe()[
+00024dd0: 224c 6f77 225d 5b22 6d69 6e22 5d0d 0a20  "Low"]["min"].. 
 00024de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024df0: 2b20 636f 6c6f 7254 6578 742e 4752 4545  + colorText.GREE
-00024e00: 4e0d 0a20 2020 2020 2020 2020 2020 2020  N..             
-00024e10: 2020 2020 2020 2020 2020 202b 2066 2256             + f"V
-00024e20: 4350 2028 424f 3a20 7b68 6967 6865 7374  CP (BO: {highest
-00024e30: 546f 707d 2922 0d0a 2020 2020 2020 2020  Top})"..        
-00024e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024e50: 2b20 636f 6c6f 7254 6578 742e 454e 440d  + colorText.END.
-00024e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024e70: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-00024e80: 2020 2020 2020 2020 2020 2020 7361 7665              save
-00024e90: 4469 6374 5b22 5061 7474 6572 6e22 5d20  Dict["Pattern"] 
-00024ea0: 3d20 7361 7665 645b 315d 202b 2066 2256  = saved[1] + f"V
-00024eb0: 4350 2028 424f 3a20 7b68 6967 6865 7374  CP (BO: {highest
-00024ec0: 546f 707d 2922 0d0a 2020 2020 2020 2020  Top})"..        
-00024ed0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00024ee0: 726e 2054 7275 650d 0a20 2020 2020 2020  rn True..       
-00024ef0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-00024f00: 6e20 6173 2065 3a20 2023 2070 7261 676d  n as e:  # pragm
-00024f10: 613a 206e 6f20 636f 7665 720d 0a20 2020  a: no cover..   
-00024f20: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
-00024f30: 6661 756c 745f 6c6f 6767 6572 2e64 6562  fault_logger.deb
-00024f40: 7567 2865 2c20 6578 635f 696e 666f 3d54  ug(e, exc_info=T
-00024f50: 7275 6529 0d0a 2020 2020 2020 2020 7265  rue)..        re
-00024f60: 7475 726e 2046 616c 7365 0d0a 0d0a 2020  turn False....  
-00024f70: 2020 2320 5661 6c69 6461 7465 2069 6620    # Validate if 
-00024f80: 766f 6c75 6d65 206f 6620 6c61 7374 2064  volume of last d
-00024f90: 6179 2069 7320 6869 6768 6572 2074 6861  ay is higher tha
-00024fa0: 6e20 6176 670d 0a20 2020 2064 6566 2076  n avg..    def v
-00024fb0: 616c 6964 6174 6556 6f6c 756d 6528 0d0a  alidateVolume(..
-00024fc0: 2020 2020 2020 2020 7365 6c66 2c20 6466          self, df
-00024fd0: 2c20 7363 7265 656e 4469 6374 2c20 7361  , screenDict, sa
-00024fe0: 7665 4469 6374 2c20 766f 6c75 6d65 5261  veDict, volumeRa
-00024ff0: 7469 6f3d 322e 352c 206d 696e 566f 6c75  tio=2.5, minVolu
-00025000: 6d65 3d31 3030 0d0a 2020 2020 293a 0d0a  me=100..    ):..
-00025010: 2020 2020 2020 2020 6966 2064 6620 6973          if df is
-00025020: 204e 6f6e 6520 6f72 206c 656e 2864 6629   None or len(df)
-00025030: 203d 3d20 303a 0d0a 2020 2020 2020 2020   == 0:..        
-00025040: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-00025050: 2c20 4661 6c73 650d 0a20 2020 2020 2020  , False..       
-00025060: 2064 6174 6120 3d20 6466 2e63 6f70 7928   data = df.copy(
-00025070: 290d 0a20 2020 2020 2020 2064 6174 6120  )..        data 
-00025080: 3d20 6461 7461 2e66 696c 6c6e 6128 3029  = data.fillna(0)
-00025090: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
-000250a0: 2064 6174 612e 7265 706c 6163 6528 5b6e   data.replace([n
-000250b0: 702e 696e 662c 202d 6e70 2e69 6e66 5d2c  p.inf, -np.inf],
-000250c0: 2030 290d 0a20 2020 2020 2020 2072 6563   0)..        rec
-000250d0: 656e 7420 3d20 6461 7461 2e68 6561 6428  ent = data.head(
-000250e0: 3129 0d0a 2020 2020 2020 2020 2320 4569  1)..        # Ei
-000250f0: 7468 6572 2074 6865 2072 6f6c 6c69 6e67  ther the rolling
-00025100: 2076 6f6c 756d 6520 6f66 2070 6173 7420   volume of past 
-00025110: 3230 2073 6573 7369 6f6e 7320 6f72 2074  20 sessions or t
-00025120: 6f64 6179 2773 2076 6f6c 756d 6520 7368  oday's volume sh
-00025130: 6f75 6c64 2062 6520 3e20 6d69 6e20 766f  ould be > min vo
-00025140: 6c75 6d65 0d0a 2020 2020 2020 2020 6861  lume..        ha
-00025150: 734d 696e 696d 756d 566f 6c75 6d65 203d  sMinimumVolume =
-00025160: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-00025170: 7265 6365 6e74 5b22 566f 6c4d 4122 5d2e  recent["VolMA"].
-00025180: 696c 6f63 5b30 5d20 3e3d 206d 696e 566f  iloc[0] >= minVo
-00025190: 6c75 6d65 0d0a 2020 2020 2020 2020 2020  lume..          
-000251a0: 2020 6f72 2072 6563 656e 745b 2256 6f6c    or recent["Vol
-000251b0: 756d 6522 5d2e 696c 6f63 5b30 5d20 3e3d  ume"].iloc[0] >=
-000251c0: 206d 696e 566f 6c75 6d65 0d0a 2020 2020   minVolume..    
-000251d0: 2020 2020 290d 0a20 2020 2020 2020 2069      )..        i
-000251e0: 6620 7265 6365 6e74 5b22 566f 6c4d 4122  f recent["VolMA"
-000251f0: 5d2e 696c 6f63 5b30 5d20 3d3d 2030 3a20  ].iloc[0] == 0: 
-00025200: 2023 2048 616e 646c 6573 2044 6976 6964   # Handles Divid
-00025210: 6520 6279 2030 2077 6172 6e69 6e67 0d0a  e by 0 warning..
-00025220: 2020 2020 2020 2020 2020 2020 7361 7665              save
-00025230: 4469 6374 5b22 566f 6c75 6d65 225d 203d  Dict["Volume"] =
-00025240: 2030 2020 2320 2255 6e6b 6e6f 776e 220d   0  # "Unknown".
-00025250: 0a20 2020 2020 2020 2020 2020 2073 6372  .            scr
-00025260: 6565 6e44 6963 745b 2256 6f6c 756d 6522  eenDict["Volume"
-00025270: 5d20 3d20 300d 0a20 2020 2020 2020 2020  ] = 0..         
-00025280: 2020 2072 6574 7572 6e20 4661 6c73 652c     return False,
-00025290: 2068 6173 4d69 6e69 6d75 6d56 6f6c 756d   hasMinimumVolum
-000252a0: 650d 0a20 2020 2020 2020 2072 6174 696f  e..        ratio
-000252b0: 203d 2072 6f75 6e64 2872 6563 656e 745b   = round(recent[
-000252c0: 2256 6f6c 756d 6522 5d2e 696c 6f63 5b30  "Volume"].iloc[0
-000252d0: 5d20 2f20 7265 6365 6e74 5b22 566f 6c4d  ] / recent["VolM
-000252e0: 4122 5d2e 696c 6f63 5b30 5d2c 2032 290d  A"].iloc[0], 2).
-000252f0: 0a20 2020 2020 2020 2073 6176 6544 6963  .        saveDic
-00025300: 745b 2256 6f6c 756d 6522 5d20 3d20 7261  t["Volume"] = ra
-00025310: 7469 6f0d 0a20 2020 2020 2020 2069 6620  tio..        if 
-00025320: 7261 7469 6f20 3e3d 2076 6f6c 756d 6552  ratio >= volumeR
-00025330: 6174 696f 2061 6e64 2072 6174 696f 2021  atio and ratio !
-00025340: 3d20 6e70 2e6e 616e 2061 6e64 2028 6e6f  = np.nan and (no
-00025350: 7420 6d61 7468 2e69 7369 6e66 2872 6174  t math.isinf(rat
-00025360: 696f 2929 3a0d 0a20 2020 2020 2020 2020  io)):..         
-00025370: 2020 2073 6372 6565 6e44 6963 745b 2256     screenDict["V
-00025380: 6f6c 756d 6522 5d20 3d20 7261 7469 6f0d  olume"] = ratio.
-00025390: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000253a0: 7572 6e20 5472 7565 2c20 6861 734d 696e  urn True, hasMin
-000253b0: 696d 756d 566f 6c75 6d65 0d0a 2020 2020  imumVolume..    
-000253c0: 2020 2020 7363 7265 656e 4469 6374 5b22      screenDict["
-000253d0: 566f 6c75 6d65 225d 203d 2072 6174 696f  Volume"] = ratio
-000253e0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000253f0: 2046 616c 7365 2c20 6861 734d 696e 696d   False, hasMinim
-00025400: 756d 566f 6c75 6d65 0d0a 0d0a 2020 2020  umVolume....    
-00025410: 2320 4669 6e64 2069 6620 7374 6f63 6b20  # Find if stock 
-00025420: 6973 2076 616c 6964 6174 696e 6720 766f  is validating vo
-00025430: 6c75 6d65 2073 7072 6561 6420 616e 616c  lume spread anal
-00025440: 7973 6973 0d0a 2020 2020 6465 6620 7661  ysis..    def va
-00025450: 6c69 6461 7465 566f 6c75 6d65 5370 7265  lidateVolumeSpre
-00025460: 6164 416e 616c 7973 6973 2873 656c 662c  adAnalysis(self,
-00025470: 2064 662c 2073 6372 6565 6e44 6963 742c   df, screenDict,
-00025480: 2073 6176 6544 6963 7429 3a0d 0a20 2020   saveDict):..   
-00025490: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-000254a0: 2020 2020 2020 2069 6620 6466 2069 7320         if df is 
-000254b0: 4e6f 6e65 206f 7220 6c65 6e28 6466 2920  None or len(df) 
-000254c0: 3d3d 2030 3a0d 0a20 2020 2020 2020 2020  == 0:..         
-000254d0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-000254e0: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
-000254f0: 2064 6174 6120 3d20 6466 2e63 6f70 7928   data = df.copy(
-00025500: 290d 0a20 2020 2020 2020 2020 2020 2064  )..            d
-00025510: 6174 6120 3d20 6461 7461 2e68 6561 6428  ata = data.head(
-00025520: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
-00025530: 6966 206c 656e 2864 6174 6129 203c 2032  if len(data) < 2
-00025540: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00025550: 2020 2072 6574 7572 6e20 4661 6c73 650d     return False.
-00025560: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
-00025570: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00025580: 2020 2023 2043 6865 636b 2066 6f72 2070     # Check for p
-00025590: 7265 7669 6f75 7320 5245 4420 6361 6e64  revious RED cand
-000255a0: 6c65 730d 0a20 2020 2020 2020 2020 2020  les..           
-000255b0: 2020 2020 2023 2043 7572 7265 6e74 2063       # Current c
-000255c0: 616e 646c 6520 3d20 3074 682c 2050 7265  andle = 0th, Pre
-000255d0: 7669 6f75 7320 4361 6e64 6c65 203d 2031  vious Candle = 1
-000255e0: 7374 2066 6f72 2066 6f6c 6c6f 7769 6e67  st for following
-000255f0: 206c 6f67 6963 0d0a 2020 2020 2020 2020   logic..        
-00025600: 2020 2020 2020 2020 6966 2064 6174 612e          if data.
-00025610: 696c 6f63 5b31 5d5b 224f 7065 6e22 5d20  iloc[1]["Open"] 
-00025620: 3e3d 2064 6174 612e 696c 6f63 5b31 5d5b  >= data.iloc[1][
-00025630: 2243 6c6f 7365 225d 3a0d 0a20 2020 2020  "Close"]:..     
-00025640: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00025650: 7072 6561 6431 203d 2061 6273 2864 6174  pread1 = abs(dat
-00025660: 612e 696c 6f63 5b31 5d5b 224f 7065 6e22  a.iloc[1]["Open"
-00025670: 5d20 2d20 6461 7461 2e69 6c6f 635b 315d  ] - data.iloc[1]
-00025680: 5b22 436c 6f73 6522 5d29 0d0a 2020 2020  ["Close"])..    
-00025690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000256a0: 7370 7265 6164 3020 3d20 6162 7328 6461  spread0 = abs(da
-000256b0: 7461 2e69 6c6f 635b 305d 5b22 4f70 656e  ta.iloc[0]["Open
-000256c0: 225d 202d 2064 6174 612e 696c 6f63 5b30  "] - data.iloc[0
-000256d0: 5d5b 2243 6c6f 7365 225d 290d 0a20 2020  ]["Close"])..   
-000256e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000256f0: 206c 6f77 6572 5f77 6963 6b5f 7370 7265   lower_wick_spre
-00025700: 6164 3020 3d20 280d 0a20 2020 2020 2020  ad0 = (..       
-00025710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025720: 206d 6178 2864 6174 612e 696c 6f63 5b30   max(data.iloc[0
-00025730: 5d5b 224f 7065 6e22 5d2c 2064 6174 612e  ]["Open"], data.
-00025740: 696c 6f63 5b30 5d5b 2243 6c6f 7365 225d  iloc[0]["Close"]
-00025750: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00025760: 2020 2020 2020 2020 2020 202d 2064 6174             - dat
-00025770: 612e 696c 6f63 5b30 5d5b 224c 6f77 225d  a.iloc[0]["Low"]
-00025780: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00025790: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-000257a0: 2020 2020 2020 2020 2020 2020 2076 6f6c               vol
-000257b0: 3120 3d20 6461 7461 2e69 6c6f 635b 315d  1 = data.iloc[1]
-000257c0: 5b22 566f 6c75 6d65 225d 0d0a 2020 2020  ["Volume"]..    
-000257d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000257e0: 766f 6c30 203d 2064 6174 612e 696c 6f63  vol0 = data.iloc
-000257f0: 5b30 5d5b 2256 6f6c 756d 6522 5d0d 0a20  [0]["Volume"].. 
-00025800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025810: 2020 2073 6176 6564 203d 2073 656c 662e     saved = self.
-00025820: 6669 6e64 4375 7272 656e 7453 6176 6564  findCurrentSaved
-00025830: 5661 6c75 6528 7363 7265 656e 4469 6374  Value(screenDict
-00025840: 2c20 7361 7665 4469 6374 2c20 2250 6174  , saveDict, "Pat
-00025850: 7465 726e 2229 0d0a 2020 2020 2020 2020  tern")..        
-00025860: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-00025870: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00025880: 2020 2020 2020 2020 2020 7370 7265 6164            spread
-00025890: 3020 3e20 7370 7265 6164 310d 0a20 2020  0 > spread1..   
+00024df0: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
+00024e00: 2020 2020 2020 6c6f 7750 6f69 6e74 734f        lowPointsO
+00024e10: 7267 203d 206c 6f77 506f 696e 7473 0d0a  rg = lowPoints..
+00024e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024e30: 6c6f 7750 6f69 6e74 732e 736f 7274 2872  lowPoints.sort(r
+00024e40: 6576 6572 7365 3d54 7275 6529 0d0a 2020  everse=True)..  
+00024e50: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00024e60: 7750 6f69 6e74 7353 6f72 7465 6420 3d20  wPointsSorted = 
+00024e70: 6c6f 7750 6f69 6e74 730d 0a20 2020 2020  lowPoints..     
+00024e80: 2020 2020 2020 2020 2020 206c 7470 203d             ltp =
+00024e90: 2064 6174 612e 6865 6164 2831 295b 2243   data.head(1)["C
+00024ea0: 6c6f 7365 225d 2e69 6c6f 635b 305d 0d0a  lose"].iloc[0]..
+00024eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024ec0: 6966 2028 0d0a 2020 2020 2020 2020 2020  if (..          
+00024ed0: 2020 2020 2020 2020 2020 6c6f 7750 6f69            lowPoi
+00024ee0: 6e74 734f 7267 203d 3d20 6c6f 7750 6f69  ntsOrg == lowPoi
+00024ef0: 6e74 7353 6f72 7465 640d 0a20 2020 2020  ntsSorted..     
+00024f00: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00024f10: 6e64 206c 7470 203c 2068 6967 6865 7374  nd ltp < highest
+00024f20: 546f 700d 0a20 2020 2020 2020 2020 2020  Top..           
+00024f30: 2020 2020 2020 2020 2061 6e64 206c 7470           and ltp
+00024f40: 203e 206c 6f77 506f 696e 7473 5b30 5d0d   > lowPoints[0].
+00024f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024f60: 2029 3a0d 0a20 2020 2020 2020 2020 2020   ):..           
+00024f70: 2020 2020 2020 2020 2073 6176 6564 203d           saved =
+00024f80: 2073 656c 662e 6669 6e64 4375 7272 656e   self.findCurren
+00024f90: 7453 6176 6564 5661 6c75 6528 7363 7265  tSavedValue(scre
+00024fa0: 656e 4469 6374 2c20 7361 7665 4469 6374  enDict, saveDict
+00024fb0: 2c20 2250 6174 7465 726e 2229 0d0a 2020  , "Pattern")..  
+00024fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024fd0: 2020 7363 7265 656e 4469 6374 5b22 5061    screenDict["Pa
+00024fe0: 7474 6572 6e22 5d20 3d20 280d 0a20 2020  ttern"] = (..   
+00024ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025000: 2020 2020 2073 6176 6564 5b30 5d20 0d0a       saved[0] ..
+00025010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025020: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
+00025030: 6578 742e 424f 4c44 0d0a 2020 2020 2020  ext.BOLD..      
+00025040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025050: 2020 2b20 636f 6c6f 7254 6578 742e 4752    + colorText.GR
+00025060: 4545 4e0d 0a20 2020 2020 2020 2020 2020  EEN..           
+00025070: 2020 2020 2020 2020 2020 2020 202b 2066               + f
+00025080: 2256 4350 2028 424f 3a20 7b68 6967 6865  "VCP (BO: {highe
+00025090: 7374 546f 707d 2922 0d0a 2020 2020 2020  stTop})"..      
+000250a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000250b0: 2020 2b20 636f 6c6f 7254 6578 742e 454e    + colorText.EN
+000250c0: 440d 0a20 2020 2020 2020 2020 2020 2020  D..             
+000250d0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+000250e0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+000250f0: 7665 4469 6374 5b22 5061 7474 6572 6e22  veDict["Pattern"
+00025100: 5d20 3d20 7361 7665 645b 315d 202b 2066  ] = saved[1] + f
+00025110: 2256 4350 2028 424f 3a20 7b68 6967 6865  "VCP (BO: {highe
+00025120: 7374 546f 707d 2922 0d0a 2020 2020 2020  stTop})"..      
+00025130: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00025140: 7475 726e 2054 7275 650d 0a20 2020 2020  turn True..     
+00025150: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+00025160: 696f 6e20 6173 2065 3a20 2023 2070 7261  ion as e:  # pra
+00025170: 676d 613a 206e 6f20 636f 7665 720d 0a20  gma: no cover.. 
+00025180: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00025190: 6465 6661 756c 745f 6c6f 6767 6572 2e64  default_logger.d
+000251a0: 6562 7567 2865 2c20 6578 635f 696e 666f  ebug(e, exc_info
+000251b0: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
+000251c0: 7265 7475 726e 2046 616c 7365 0d0a 0d0a  return False....
+000251d0: 2020 2020 2320 5661 6c69 6461 7465 2069      # Validate i
+000251e0: 6620 766f 6c75 6d65 206f 6620 6c61 7374  f volume of last
+000251f0: 2064 6179 2069 7320 6869 6768 6572 2074   day is higher t
+00025200: 6861 6e20 6176 670d 0a20 2020 2064 6566  han avg..    def
+00025210: 2076 616c 6964 6174 6556 6f6c 756d 6528   validateVolume(
+00025220: 0d0a 2020 2020 2020 2020 7365 6c66 2c20  ..        self, 
+00025230: 6466 2c20 7363 7265 656e 4469 6374 2c20  df, screenDict, 
+00025240: 7361 7665 4469 6374 2c20 766f 6c75 6d65  saveDict, volume
+00025250: 5261 7469 6f3d 322e 352c 206d 696e 566f  Ratio=2.5, minVo
+00025260: 6c75 6d65 3d31 3030 0d0a 2020 2020 293a  lume=100..    ):
+00025270: 0d0a 2020 2020 2020 2020 6966 2064 6620  ..        if df 
+00025280: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
+00025290: 6629 203d 3d20 303a 0d0a 2020 2020 2020  f) == 0:..      
+000252a0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+000252b0: 7365 2c20 4661 6c73 650d 0a20 2020 2020  se, False..     
+000252c0: 2020 2064 6174 6120 3d20 6466 2e63 6f70     data = df.cop
+000252d0: 7928 290d 0a20 2020 2020 2020 2064 6174  y()..        dat
+000252e0: 6120 3d20 6461 7461 2e66 696c 6c6e 6128  a = data.fillna(
+000252f0: 3029 0d0a 2020 2020 2020 2020 6461 7461  0)..        data
+00025300: 203d 2064 6174 612e 7265 706c 6163 6528   = data.replace(
+00025310: 5b6e 702e 696e 662c 202d 6e70 2e69 6e66  [np.inf, -np.inf
+00025320: 5d2c 2030 290d 0a20 2020 2020 2020 2072  ], 0)..        r
+00025330: 6563 656e 7420 3d20 6461 7461 2e68 6561  ecent = data.hea
+00025340: 6428 3129 0d0a 2020 2020 2020 2020 2320  d(1)..        # 
+00025350: 4569 7468 6572 2074 6865 2072 6f6c 6c69  Either the rolli
+00025360: 6e67 2076 6f6c 756d 6520 6f66 2070 6173  ng volume of pas
+00025370: 7420 3230 2073 6573 7369 6f6e 7320 6f72  t 20 sessions or
+00025380: 2074 6f64 6179 2773 2076 6f6c 756d 6520   today's volume 
+00025390: 7368 6f75 6c64 2062 6520 3e20 6d69 6e20  should be > min 
+000253a0: 766f 6c75 6d65 0d0a 2020 2020 2020 2020  volume..        
+000253b0: 6861 734d 696e 696d 756d 566f 6c75 6d65  hasMinimumVolume
+000253c0: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
+000253d0: 2020 7265 6365 6e74 5b22 566f 6c4d 4122    recent["VolMA"
+000253e0: 5d2e 696c 6f63 5b30 5d20 3e3d 206d 696e  ].iloc[0] >= min
+000253f0: 566f 6c75 6d65 0d0a 2020 2020 2020 2020  Volume..        
+00025400: 2020 2020 6f72 2072 6563 656e 745b 2256      or recent["V
+00025410: 6f6c 756d 6522 5d2e 696c 6f63 5b30 5d20  olume"].iloc[0] 
+00025420: 3e3d 206d 696e 566f 6c75 6d65 0d0a 2020  >= minVolume..  
+00025430: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+00025440: 2069 6620 7265 6365 6e74 5b22 566f 6c4d   if recent["VolM
+00025450: 4122 5d2e 696c 6f63 5b30 5d20 3d3d 2030  A"].iloc[0] == 0
+00025460: 3a20 2023 2048 616e 646c 6573 2044 6976  :  # Handles Div
+00025470: 6964 6520 6279 2030 2077 6172 6e69 6e67  ide by 0 warning
+00025480: 0d0a 2020 2020 2020 2020 2020 2020 7361  ..            sa
+00025490: 7665 4469 6374 5b22 566f 6c75 6d65 225d  veDict["Volume"]
+000254a0: 203d 2030 2020 2320 2255 6e6b 6e6f 776e   = 0  # "Unknown
+000254b0: 220d 0a20 2020 2020 2020 2020 2020 2073  "..            s
+000254c0: 6372 6565 6e44 6963 745b 2256 6f6c 756d  creenDict["Volum
+000254d0: 6522 5d20 3d20 300d 0a20 2020 2020 2020  e"] = 0..       
+000254e0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+000254f0: 652c 2068 6173 4d69 6e69 6d75 6d56 6f6c  e, hasMinimumVol
+00025500: 756d 650d 0a20 2020 2020 2020 2072 6174  ume..        rat
+00025510: 696f 203d 2072 6f75 6e64 2872 6563 656e  io = round(recen
+00025520: 745b 2256 6f6c 756d 6522 5d2e 696c 6f63  t["Volume"].iloc
+00025530: 5b30 5d20 2f20 7265 6365 6e74 5b22 566f  [0] / recent["Vo
+00025540: 6c4d 4122 5d2e 696c 6f63 5b30 5d2c 2032  lMA"].iloc[0], 2
+00025550: 290d 0a20 2020 2020 2020 2073 6176 6544  )..        saveD
+00025560: 6963 745b 2256 6f6c 756d 6522 5d20 3d20  ict["Volume"] = 
+00025570: 7261 7469 6f0d 0a20 2020 2020 2020 2069  ratio..        i
+00025580: 6620 7261 7469 6f20 3e3d 2076 6f6c 756d  f ratio >= volum
+00025590: 6552 6174 696f 2061 6e64 2072 6174 696f  eRatio and ratio
+000255a0: 2021 3d20 6e70 2e6e 616e 2061 6e64 2028   != np.nan and (
+000255b0: 6e6f 7420 6d61 7468 2e69 7369 6e66 2872  not math.isinf(r
+000255c0: 6174 696f 2929 3a0d 0a20 2020 2020 2020  atio)):..       
+000255d0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+000255e0: 2256 6f6c 756d 6522 5d20 3d20 7261 7469  "Volume"] = rati
+000255f0: 6f0d 0a20 2020 2020 2020 2020 2020 2072  o..            r
+00025600: 6574 7572 6e20 5472 7565 2c20 6861 734d  eturn True, hasM
+00025610: 696e 696d 756d 566f 6c75 6d65 0d0a 2020  inimumVolume..  
+00025620: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
+00025630: 5b22 566f 6c75 6d65 225d 203d 2072 6174  ["Volume"] = rat
+00025640: 696f 0d0a 2020 2020 2020 2020 7265 7475  io..        retu
+00025650: 726e 2046 616c 7365 2c20 6861 734d 696e  rn False, hasMin
+00025660: 696d 756d 566f 6c75 6d65 0d0a 0d0a 2020  imumVolume....  
+00025670: 2020 2320 4669 6e64 2069 6620 7374 6f63    # Find if stoc
+00025680: 6b20 6973 2076 616c 6964 6174 696e 6720  k is validating 
+00025690: 766f 6c75 6d65 2073 7072 6561 6420 616e  volume spread an
+000256a0: 616c 7973 6973 0d0a 2020 2020 6465 6620  alysis..    def 
+000256b0: 7661 6c69 6461 7465 566f 6c75 6d65 5370  validateVolumeSp
+000256c0: 7265 6164 416e 616c 7973 6973 2873 656c  readAnalysis(sel
+000256d0: 662c 2064 662c 2073 6372 6565 6e44 6963  f, df, screenDic
+000256e0: 742c 2073 6176 6544 6963 7429 3a0d 0a20  t, saveDict):.. 
+000256f0: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
+00025700: 2020 2020 2020 2020 2069 6620 6466 2069           if df i
+00025710: 7320 4e6f 6e65 206f 7220 6c65 6e28 6466  s None or len(df
+00025720: 2920 3d3d 2030 3a0d 0a20 2020 2020 2020  ) == 0:..       
+00025730: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00025740: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
+00025750: 2020 2064 6174 6120 3d20 6466 2e63 6f70     data = df.cop
+00025760: 7928 290d 0a20 2020 2020 2020 2020 2020  y()..           
+00025770: 2064 6174 6120 3d20 6461 7461 2e68 6561   data = data.hea
+00025780: 6428 3229 0d0a 2020 2020 2020 2020 2020  d(2)..          
+00025790: 2020 6966 206c 656e 2864 6174 6129 203c    if len(data) <
+000257a0: 2032 3a0d 0a20 2020 2020 2020 2020 2020   2:..           
+000257b0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+000257c0: 650d 0a20 2020 2020 2020 2020 2020 2074  e..            t
+000257d0: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+000257e0: 2020 2020 2023 2043 6865 636b 2066 6f72       # Check for
+000257f0: 2070 7265 7669 6f75 7320 5245 4420 6361   previous RED ca
+00025800: 6e64 6c65 730d 0a20 2020 2020 2020 2020  ndles..         
+00025810: 2020 2020 2020 2023 2043 7572 7265 6e74         # Current
+00025820: 2063 616e 646c 6520 3d20 3074 682c 2050   candle = 0th, P
+00025830: 7265 7669 6f75 7320 4361 6e64 6c65 203d  revious Candle =
+00025840: 2031 7374 2066 6f72 2066 6f6c 6c6f 7769   1st for followi
+00025850: 6e67 206c 6f67 6963 0d0a 2020 2020 2020  ng logic..      
+00025860: 2020 2020 2020 2020 2020 6966 2064 6174            if dat
+00025870: 612e 696c 6f63 5b31 5d5b 224f 7065 6e22  a.iloc[1]["Open"
+00025880: 5d20 3e3d 2064 6174 612e 696c 6f63 5b31  ] >= data.iloc[1
+00025890: 5d5b 2243 6c6f 7365 225d 3a0d 0a20 2020  ]["Close"]:..   
 000258a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000258b0: 2020 2020 2061 6e64 2076 6f6c 3020 3c20       and vol0 < 
-000258c0: 766f 6c31 0d0a 2020 2020 2020 2020 2020  vol1..          
-000258d0: 2020 2020 2020 2020 2020 2020 2020 616e                an
-000258e0: 6420 6461 7461 2e69 6c6f 635b 305d 5b22  d data.iloc[0]["
-000258f0: 566f 6c75 6d65 225d 203c 2064 6174 612e  Volume"] < data.
-00025900: 696c 6f63 5b30 5d5b 2256 6f6c 4d41 225d  iloc[0]["VolMA"]
-00025910: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00025920: 2020 2020 2020 2020 2020 616e 6420 6461            and da
-00025930: 7461 2e69 6c6f 635b 305d 5b22 436c 6f73  ta.iloc[0]["Clos
-00025940: 6522 5d20 3c3d 2064 6174 612e 696c 6f63  e"] <= data.iloc
-00025950: 5b31 5d5b 224f 7065 6e22 5d0d 0a20 2020  [1]["Open"]..   
-00025960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025970: 2020 2020 2061 6e64 2073 7072 6561 6430       and spread0
-00025980: 203c 206c 6f77 6572 5f77 6963 6b5f 7370   < lower_wick_sp
-00025990: 7265 6164 300d 0a20 2020 2020 2020 2020  read0..         
-000259a0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000259b0: 6e64 2064 6174 612e 696c 6f63 5b30 5d5b  nd data.iloc[0][
-000259c0: 2256 6f6c 756d 6522 5d20 3c3d 2069 6e74  "Volume"] <= int
-000259d0: 2864 6174 612e 696c 6f63 5b31 5d5b 2256  (data.iloc[1]["V
-000259e0: 6f6c 756d 6522 5d20 2a20 302e 3735 290d  olume"] * 0.75).
-000259f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00025a00: 2020 2020 2029 3a0d 0a20 2020 2020 2020       ):..       
-00025a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025a20: 2073 6372 6565 6e44 6963 745b 2250 6174   screenDict["Pat
-00025a30: 7465 726e 225d 203d 2028 0d0a 2020 2020  tern"] = (..    
-00025a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025a50: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
-00025a60: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00025a70: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-00025a80: 2063 6f6c 6f72 5465 7874 2e42 4f4c 440d   colorText.BOLD.
-00025a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00025aa0: 2020 2020 2020 2020 2020 2020 202b 2063               + c
-00025ab0: 6f6c 6f72 5465 7874 2e47 5245 454e 0d0a  olorText.GREEN..
-00025ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025ad0: 2020 2020 2020 2020 2020 2020 2b20 2253              + "S
-00025ae0: 7570 706c 7920 4472 6f75 6768 7422 0d0a  upply Drought"..
-00025af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025b00: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
-00025b10: 6c6f 7254 6578 742e 454e 440d 0a20 2020  lorText.END..   
-00025b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025b30: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-00025b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025b50: 7361 7665 4469 6374 5b22 5061 7474 6572  saveDict["Patter
-00025b60: 6e22 5d20 3d20 7361 7665 645b 315d 202b  n"] = saved[1] +
-00025b70: 2022 5375 7070 6c79 2044 726f 7567 6874   "Supply Drought
-00025b80: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-00025b90: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00025ba0: 6e20 5472 7565 0d0a 2020 2020 2020 2020  n True..        
-00025bb0: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-00025bc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00025bd0: 2020 2020 2020 2020 2020 7370 7265 6164            spread
-00025be0: 3020 3c20 7370 7265 6164 310d 0a20 2020  0 < spread1..   
-00025bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025c00: 2020 2020 2061 6e64 2076 6f6c 3020 3e20       and vol0 > 
-00025c10: 766f 6c31 0d0a 2020 2020 2020 2020 2020  vol1..          
-00025c20: 2020 2020 2020 2020 2020 2020 2020 616e                an
-00025c30: 6420 6461 7461 2e69 6c6f 635b 305d 5b22  d data.iloc[0]["
-00025c40: 566f 6c75 6d65 225d 203e 2064 6174 612e  Volume"] > data.
-00025c50: 696c 6f63 5b30 5d5b 2256 6f6c 4d41 225d  iloc[0]["VolMA"]
-00025c60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00025c70: 2020 2020 2020 2020 2020 616e 6420 6461            and da
-00025c80: 7461 2e69 6c6f 635b 305d 5b22 436c 6f73  ta.iloc[0]["Clos
-00025c90: 6522 5d20 3c3d 2064 6174 612e 696c 6f63  e"] <= data.iloc
-00025ca0: 5b31 5d5b 224f 7065 6e22 5d0d 0a20 2020  [1]["Open"]..   
-00025cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025cc0: 2029 3a0d 0a20 2020 2020 2020 2020 2020   ):..           
-00025cd0: 2020 2020 2020 2020 2020 2020 2073 6372               scr
-00025ce0: 6565 6e44 6963 745b 2250 6174 7465 726e  eenDict["Pattern
-00025cf0: 225d 203d 2028 0d0a 2020 2020 2020 2020  "] = (..        
-00025d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025d10: 2020 2020 7361 7665 645b 305d 200d 0a20      saved[0] .. 
-00025d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025d30: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-00025d40: 6f72 5465 7874 2e42 4f4c 440d 0a20 2020  orText.BOLD..   
-00025d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025d60: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
-00025d70: 5465 7874 2e47 5245 454e 0d0a 2020 2020  Text.GREEN..    
+000258b0: 2073 7072 6561 6431 203d 2061 6273 2864   spread1 = abs(d
+000258c0: 6174 612e 696c 6f63 5b31 5d5b 224f 7065  ata.iloc[1]["Ope
+000258d0: 6e22 5d20 2d20 6461 7461 2e69 6c6f 635b  n"] - data.iloc[
+000258e0: 315d 5b22 436c 6f73 6522 5d29 0d0a 2020  1]["Close"])..  
+000258f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025900: 2020 7370 7265 6164 3020 3d20 6162 7328    spread0 = abs(
+00025910: 6461 7461 2e69 6c6f 635b 305d 5b22 4f70  data.iloc[0]["Op
+00025920: 656e 225d 202d 2064 6174 612e 696c 6f63  en"] - data.iloc
+00025930: 5b30 5d5b 2243 6c6f 7365 225d 290d 0a20  [0]["Close"]).. 
+00025940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025950: 2020 206c 6f77 6572 5f77 6963 6b5f 7370     lower_wick_sp
+00025960: 7265 6164 3020 3d20 280d 0a20 2020 2020  read0 = (..     
+00025970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025980: 2020 206d 6178 2864 6174 612e 696c 6f63     max(data.iloc
+00025990: 5b30 5d5b 224f 7065 6e22 5d2c 2064 6174  [0]["Open"], dat
+000259a0: 612e 696c 6f63 5b30 5d5b 2243 6c6f 7365  a.iloc[0]["Close
+000259b0: 225d 290d 0a20 2020 2020 2020 2020 2020  "])..           
+000259c0: 2020 2020 2020 2020 2020 2020 202d 2064               - d
+000259d0: 6174 612e 696c 6f63 5b30 5d5b 224c 6f77  ata.iloc[0]["Low
+000259e0: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
+000259f0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+00025a00: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00025a10: 6f6c 3120 3d20 6461 7461 2e69 6c6f 635b  ol1 = data.iloc[
+00025a20: 315d 5b22 566f 6c75 6d65 225d 0d0a 2020  1]["Volume"]..  
+00025a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025a40: 2020 766f 6c30 203d 2064 6174 612e 696c    vol0 = data.il
+00025a50: 6f63 5b30 5d5b 2256 6f6c 756d 6522 5d0d  oc[0]["Volume"].
+00025a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025a70: 2020 2020 2073 6176 6564 203d 2073 656c       saved = sel
+00025a80: 662e 6669 6e64 4375 7272 656e 7453 6176  f.findCurrentSav
+00025a90: 6564 5661 6c75 6528 7363 7265 656e 4469  edValue(screenDi
+00025aa0: 6374 2c20 7361 7665 4469 6374 2c20 2250  ct, saveDict, "P
+00025ab0: 6174 7465 726e 2229 0d0a 2020 2020 2020  attern")..      
+00025ac0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00025ad0: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+00025ae0: 2020 2020 2020 2020 2020 2020 7370 7265              spre
+00025af0: 6164 3020 3e20 7370 7265 6164 310d 0a20  ad0 > spread1.. 
+00025b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025b10: 2020 2020 2020 2061 6e64 2076 6f6c 3020         and vol0 
+00025b20: 3c20 766f 6c31 0d0a 2020 2020 2020 2020  < vol1..        
+00025b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025b40: 616e 6420 6461 7461 2e69 6c6f 635b 305d  and data.iloc[0]
+00025b50: 5b22 566f 6c75 6d65 225d 203c 2064 6174  ["Volume"] < dat
+00025b60: 612e 696c 6f63 5b30 5d5b 2256 6f6c 4d41  a.iloc[0]["VolMA
+00025b70: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
+00025b80: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+00025b90: 6461 7461 2e69 6c6f 635b 305d 5b22 436c  data.iloc[0]["Cl
+00025ba0: 6f73 6522 5d20 3c3d 2064 6174 612e 696c  ose"] <= data.il
+00025bb0: 6f63 5b31 5d5b 224f 7065 6e22 5d0d 0a20  oc[1]["Open"].. 
+00025bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025bd0: 2020 2020 2020 2061 6e64 2073 7072 6561         and sprea
+00025be0: 6430 203c 206c 6f77 6572 5f77 6963 6b5f  d0 < lower_wick_
+00025bf0: 7370 7265 6164 300d 0a20 2020 2020 2020  spread0..       
+00025c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025c10: 2061 6e64 2064 6174 612e 696c 6f63 5b30   and data.iloc[0
+00025c20: 5d5b 2256 6f6c 756d 6522 5d20 3c3d 2069  ]["Volume"] <= i
+00025c30: 6e74 2864 6174 612e 696c 6f63 5b31 5d5b  nt(data.iloc[1][
+00025c40: 2256 6f6c 756d 6522 5d20 2a20 302e 3735  "Volume"] * 0.75
+00025c50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00025c60: 2020 2020 2020 2029 3a0d 0a20 2020 2020         ):..     
+00025c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025c80: 2020 2073 6372 6565 6e44 6963 745b 2250     screenDict["P
+00025c90: 6174 7465 726e 225d 203d 2028 0d0a 2020  attern"] = (..  
+00025ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025cb0: 2020 2020 2020 2020 2020 7361 7665 645b            saved[
+00025cc0: 305d 200d 0a20 2020 2020 2020 2020 2020  0] ..           
+00025cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025ce0: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
+00025cf0: 440d 0a20 2020 2020 2020 2020 2020 2020  D..             
+00025d00: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+00025d10: 2063 6f6c 6f72 5465 7874 2e47 5245 454e   colorText.GREEN
+00025d20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00025d30: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+00025d40: 2253 7570 706c 7920 4472 6f75 6768 7422  "Supply Drought"
+00025d50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00025d60: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+00025d70: 636f 6c6f 7254 6578 742e 454e 440d 0a20  colorText.END.. 
 00025d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025d90: 2020 2020 2020 2020 2b20 2244 656d 616e          + "Deman
-00025da0: 6420 5269 7365 220d 0a20 2020 2020 2020  d Rise"..       
-00025db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025dc0: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-00025dd0: 2e45 4e44 0d0a 2020 2020 2020 2020 2020  .END..          
-00025de0: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-00025df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00025e00: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
-00025e10: 745b 2250 6174 7465 726e 225d 203d 2073  t["Pattern"] = s
-00025e20: 6176 6564 5b31 5d20 2b20 2244 656d 616e  aved[1] + "Deman
-00025e30: 6420 5269 7365 220d 0a20 2020 2020 2020  d Rise"..       
-00025e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025e50: 2072 6574 7572 6e20 5472 7565 0d0a 2020   return True..  
-00025e60: 2020 2020 2020 2020 2020 6578 6365 7074            except
-00025e70: 2049 6e64 6578 4572 726f 7220 6173 2065   IndexError as e
-00025e80: 3a20 2320 7072 6167 6d61 3a20 6e6f 2063  : # pragma: no c
-00025e90: 6f76 6572 0d0a 2020 2020 2020 2020 2020  over..          
-00025ea0: 2020 2020 2020 7365 6c66 2e64 6566 6175        self.defau
-00025eb0: 6c74 5f6c 6f67 6765 722e 6465 6275 6728  lt_logger.debug(
-00025ec0: 652c 2065 7863 5f69 6e66 6f3d 5472 7565  e, exc_info=True
-00025ed0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00025ee0: 2020 2070 6173 730d 0a20 2020 2020 2020     pass..       
-00025ef0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-00025f00: 650d 0a20 2020 2020 2020 2065 7863 6570  e..        excep
-00025f10: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-00025f20: 3a20 2023 2070 7261 676d 613a 206e 6f20  :  # pragma: no 
-00025f30: 636f 7665 720d 0a20 2020 2020 2020 2020  cover..         
-00025f40: 2020 2073 656c 662e 6465 6661 756c 745f     self.default_
-00025f50: 6c6f 6767 6572 2e64 6562 7567 2865 2c20  logger.debug(e, 
-00025f60: 6578 635f 696e 666f 3d54 7275 6529 0d0a  exc_info=True)..
-00025f70: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00025f80: 726e 2046 616c 7365 0d0a                 rn False..
+00025d90: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+00025da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025db0: 2020 7361 7665 4469 6374 5b22 5061 7474    saveDict["Patt
+00025dc0: 6572 6e22 5d20 3d20 7361 7665 645b 315d  ern"] = saved[1]
+00025dd0: 202b 2022 5375 7070 6c79 2044 726f 7567   + "Supply Droug
+00025de0: 6874 220d 0a20 2020 2020 2020 2020 2020  ht"..           
+00025df0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00025e00: 7572 6e20 5472 7565 0d0a 2020 2020 2020  urn True..      
+00025e10: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00025e20: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+00025e30: 2020 2020 2020 2020 2020 2020 7370 7265              spre
+00025e40: 6164 3020 3c20 7370 7265 6164 310d 0a20  ad0 < spread1.. 
+00025e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025e60: 2020 2020 2020 2061 6e64 2076 6f6c 3020         and vol0 
+00025e70: 3e20 766f 6c31 0d0a 2020 2020 2020 2020  > vol1..        
+00025e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025e90: 616e 6420 6461 7461 2e69 6c6f 635b 305d  and data.iloc[0]
+00025ea0: 5b22 566f 6c75 6d65 225d 203e 2064 6174  ["Volume"] > dat
+00025eb0: 612e 696c 6f63 5b30 5d5b 2256 6f6c 4d41  a.iloc[0]["VolMA
+00025ec0: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
+00025ed0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+00025ee0: 6461 7461 2e69 6c6f 635b 305d 5b22 436c  data.iloc[0]["Cl
+00025ef0: 6f73 6522 5d20 3c3d 2064 6174 612e 696c  ose"] <= data.il
+00025f00: 6f63 5b31 5d5b 224f 7065 6e22 5d0d 0a20  oc[1]["Open"].. 
+00025f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025f20: 2020 2029 3a0d 0a20 2020 2020 2020 2020     ):..         
+00025f30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00025f40: 6372 6565 6e44 6963 745b 2250 6174 7465  creenDict["Patte
+00025f50: 726e 225d 203d 2028 0d0a 2020 2020 2020  rn"] = (..      
+00025f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025f70: 2020 2020 2020 7361 7665 645b 305d 200d        saved[0] .
+00025f80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025f90: 2020 2020 2020 2020 2020 2020 202b 2063               + c
+00025fa0: 6f6c 6f72 5465 7874 2e42 4f4c 440d 0a20  olorText.BOLD.. 
+00025fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025fc0: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
+00025fd0: 6f72 5465 7874 2e47 5245 454e 0d0a 2020  orText.GREEN..  
+00025fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025ff0: 2020 2020 2020 2020 2020 2b20 2244 656d            + "Dem
+00026000: 616e 6420 5269 7365 220d 0a20 2020 2020  and Rise"..     
+00026010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026020: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
+00026030: 7874 2e45 4e44 0d0a 2020 2020 2020 2020  xt.END..        
+00026040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026050: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00026060: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
+00026070: 6963 745b 2250 6174 7465 726e 225d 203d  ict["Pattern"] =
+00026080: 2073 6176 6564 5b31 5d20 2b20 2244 656d   saved[1] + "Dem
+00026090: 616e 6420 5269 7365 220d 0a20 2020 2020  and Rise"..     
+000260a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000260b0: 2020 2072 6574 7572 6e20 5472 7565 0d0a     return True..
+000260c0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+000260d0: 7074 2049 6e64 6578 4572 726f 7220 6173  pt IndexError as
+000260e0: 2065 3a20 2320 7072 6167 6d61 3a20 6e6f   e: # pragma: no
+000260f0: 2063 6f76 6572 0d0a 2020 2020 2020 2020   cover..        
+00026100: 2020 2020 2020 2020 7365 6c66 2e64 6566          self.def
+00026110: 6175 6c74 5f6c 6f67 6765 722e 6465 6275  ault_logger.debu
+00026120: 6728 652c 2065 7863 5f69 6e66 6f3d 5472  g(e, exc_info=Tr
+00026130: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
+00026140: 2020 2020 2070 6173 730d 0a20 2020 2020       pass..     
+00026150: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00026160: 6c73 650d 0a20 2020 2020 2020 2065 7863  lse..        exc
+00026170: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
+00026180: 2065 3a20 2023 2070 7261 676d 613a 206e   e:  # pragma: n
+00026190: 6f20 636f 7665 720d 0a20 2020 2020 2020  o cover..       
+000261a0: 2020 2020 2073 656c 662e 6465 6661 756c       self.defaul
+000261b0: 745f 6c6f 6767 6572 2e64 6562 7567 2865  t_logger.debug(e
+000261c0: 2c20 6578 635f 696e 666f 3d54 7275 6529  , exc_info=True)
+000261d0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+000261e0: 7475 726e 2046 616c 7365 0d0a            turn False..
```

### Comparing `pkscreener-0.44.20240516.379/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240517.380/pkscreener/classes/StockScreener.py`

 * *Files 0% similar despite different names*

```diff
@@ -438,15 +438,16 @@
                                 fullData,
                                 screeningDictionary,
                                 saveDictionary,
                                 testbuild,
                                 stock,
                                 onlyMF=(executeOption == 21 and reversalOption in [5,6]),
                                 hostData=data,
-                                exchangeName=exchangeName
+                                exchangeName=exchangeName,
+                                refreshMFAndFV=(menuOption in ["X"])
                             )
                             hostRef.objectDictionaryPrimary[stock] = data.to_dict("split")
                 except np.RankWarning as e: # pragma: no cover 
                     hostRef.default_logger.debug(e, exc_info=True)
                     screeningDictionary["Trend"] = "Unknown"
                     saveDictionary["Trend"] = "Unknown"
                 # CCI also uses "Trend" value from findTrend above.
@@ -861,23 +862,26 @@
                 columns = hostData["columns"]
                 data = pd.DataFrame(
                         hostData["data"], columns=columns, index=hostData["index"]
                     )
             except (ValueError, AssertionError) as e:
                 # 9 columns passed, passed data had 11 columns
                 # 10 columns passed, passed data had 11 columns
-                hostRef.default_logger.debug(e, exc_info=True)
-                e_diff = str(e).replace(" columns passed, passed data had ",",").replace(" columns","").split(",")
-                num_diff = int(e_diff[1]) - int(e_diff[0])
-                while (num_diff > 0):
-                    columns.append(f"temp{num_diff}")
-                    num_diff -= 1
-                data = pd.DataFrame(
-                        hostData["data"], columns=columns, index=hostData["index"]
-                    )
+                excLookingFor = " columns passed, passed data had "
+                if excLookingFor in str(e):
+                    e_diff = str(e).replace(excLookingFor,",").replace(" columns","").split(",")
+                    num_diff = int(e_diff[1]) - int(e_diff[0])
+                    while (num_diff > 0):
+                        columns.append(f"temp{num_diff}")
+                        num_diff -= 1
+                    data = pd.DataFrame(
+                            hostData["data"], columns=columns, index=hostData["index"]
+                        )
+                else:
+                    hostRef.default_logger.debug(e, exc_info=True)
                 pass
 
         if ((shouldCache and not self.isTradingTime and (hostData is None  or hostDataLength == 0)) or downloadOnly) \
             or (shouldCache and hostData is None):  # and backtestDuration == 0 # save only if we're NOT backtesting
                 if start is None and data is not None:
                     objectDictionary[stock] = data.to_dict("split")
                 if downloadOnly:
```

### Comparing `pkscreener-0.44.20240516.379/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240517.380/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240517.380/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240517.380/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/pkscreener/classes/keys.py` & `pkscreener-0.44.20240517.380/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/pkscreener/courbd.ttf` & `pkscreener-0.44.20240517.380/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/pkscreener/globals.py` & `pkscreener-0.44.20240517.380/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -2057,15 +2057,15 @@
                     caption_df.loc[:, "LTP"] = caption_df.loc[:, "LTP"].apply(
                         lambda x: str(int(round(float(x),0)))
                     )
                     caption_df.loc[:, "%Chng"] = caption_df.loc[:, "%Chng"].apply(
                         lambda x: f'{int(round(float(x.replace("%","")),0))}%'
                     )
                     caption_df.loc[:, "Volume"] = caption_df.loc[:, "Volume"].apply(
-                        lambda x: f'{int(round(float(x.replace("x","")),0))}x'
+                        lambda x: f'{int(round(float(x.replace("x","")),0))}x' if (len(x.replace("x","").strip()) > 0 and not pd.isna(float(x.replace("x","")))) else ''
                     )
                     caption_df.rename(columns={"%Chng": "Ch%","Volume":"Vol"}, inplace=True)
                     for col in caption_df.columns:
                         caption_df[col] = caption_df[col].astype(str)
                     caption_results = colorText.miniTabulator().tabulate(
                         caption_df,
                         headers="keys",
```

### Comparing `pkscreener-0.44.20240516.379/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240517.380/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240517.380/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240517.380/pkscreener/pkscreenercli.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,14 +204,20 @@
 argParser.add_argument(
     "--simulate",
     type=json.loads, # '{"isTrading":true,"currentDateTime":"2024-04-29 09:35:38"}'
     help="Simulate various conditions",
     required=False,
 )
 argParser.add_argument(
+    "--singlethread",
+    action="store_true",
+    help="Run analysis for debugging purposes in a single process, single threaded environment",
+    required=False,
+)
+argParser.add_argument(
     "-t",
     "--testbuild",
     action="store_true",
     help="Run in test-build mode",
     required=False,
 )
 argParser.add_argument(
```

### Comparing `pkscreener-0.44.20240516.379/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240517.380/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240516.379
+Version: 0.44.20240517.380
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240516.379.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240517.380.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.378/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.379/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.378/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.379/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.378/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.379/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240516.379/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240517.380/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.379/setup.py` & `pkscreener-0.44.20240517.380/setup.py`

 * *Files identical despite different names*

