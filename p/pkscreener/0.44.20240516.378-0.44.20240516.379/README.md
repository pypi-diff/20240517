# Comparing `tmp/pkscreener-0.44.20240516.378.tar.gz` & `tmp/pkscreener-0.44.20240516.379.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240516.378.tar", last modified: Thu May 16 09:19:19 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240516.379.tar", last modified: Thu May 16 10:22:34 2024, max compression
```

## Comparing `pkscreener-0.44.20240516.378.tar` & `pkscreener-0.44.20240516.379.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 09:19:19.849475 pkscreener-0.44.20240516.378/
--rw-rw-rw-   0        0        0     1086 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-16 09:19:19.849475 pkscreener-0.44.20240516.378/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 09:19:19.833866 pkscreener-0.44.20240516.378/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 09:19:19.849475 pkscreener-0.44.20240516.378/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1537 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    34250 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11407 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    42703 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    12534 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    24534 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    22221 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18947 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   155530 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    56135 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4993 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    84725 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3789 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-16 09:19:05.000000 pkscreener-0.44.20240516.378/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   141394 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/globals.py
--rw-rw-rw-   0        0        0     1090 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    53036 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    33750 2024-05-16 09:14:29.000000 pkscreener-0.44.20240516.378/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-16 09:19:19.833866 pkscreener-0.44.20240516.378/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-16 09:19:19.000000 pkscreener-0.44.20240516.378/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-16 09:19:19.000000 pkscreener-0.44.20240516.378/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 09:19:19.000000 pkscreener-0.44.20240516.378/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-16 09:19:19.000000 pkscreener-0.44.20240516.378/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-16 09:19:19.000000 pkscreener-0.44.20240516.378/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-16 09:19:19.000000 pkscreener-0.44.20240516.378/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-16 09:19:19.849475 pkscreener-0.44.20240516.378/setup.cfg
--rw-rw-rw-   0        0        0     4765 2024-05-16 09:14:30.000000 pkscreener-0.44.20240516.378/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 10:22:34.961543 pkscreener-0.44.20240516.379/
+-rw-rw-rw-   0        0        0     1086 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-16 10:22:34.961543 pkscreener-0.44.20240516.379/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 10:22:34.945945 pkscreener-0.44.20240516.379/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 10:22:34.961543 pkscreener-0.44.20240516.379/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1537 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    34250 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11407 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    43311 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    12534 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    24534 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    22221 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18947 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   155530 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    56135 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4993 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    84725 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3789 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-16 10:22:24.000000 pkscreener-0.44.20240516.379/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   141394 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/globals.py
+-rw-rw-rw-   0        0        0     1090 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    53036 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    33750 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-16 10:22:34.945945 pkscreener-0.44.20240516.379/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-16 10:22:34.000000 pkscreener-0.44.20240516.379/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-16 10:22:34.000000 pkscreener-0.44.20240516.379/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 10:22:34.000000 pkscreener-0.44.20240516.379/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-16 10:22:34.000000 pkscreener-0.44.20240516.379/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-16 10:22:34.000000 pkscreener-0.44.20240516.379/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-16 10:22:34.000000 pkscreener-0.44.20240516.379/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-16 10:22:34.961543 pkscreener-0.44.20240516.379/setup.cfg
+-rw-rw-rw-   0        0        0     4765 2024-05-16 10:17:01.000000 pkscreener-0.44.20240516.379/setup.py
```

### Comparing `pkscreener-0.44.20240516.378/LICENSE` & `pkscreener-0.44.20240516.379/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/LICENSE-Others` & `pkscreener-0.44.20240516.379/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/PKG-INFO` & `pkscreener-0.44.20240516.379/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240516.378
+Version: 0.44.20240516.379
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240516.378.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240516.379.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.377/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.378/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.377/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.378/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.377/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.378/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240516.378/README.md` & `pkscreener-0.44.20240516.379/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.377/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.378/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.377/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.378/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.377/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.378/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240516.378/pkscreener/__init__.py` & `pkscreener-0.44.20240516.379/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/classes/ArtTexts.py` & `pkscreener-0.44.20240516.379/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240516.379/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240516.379/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240516.379/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240516.379/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240516.379/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240516.379/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240516.379/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240516.379/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240516.379/pkscreener/classes/MenuOptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,23 +58,23 @@
 level1_P_MenuDict = {
     "1": "Predefined Piped Scanners",
     "2": "Define my custom Piped Scanner",
     "M": "Back to the Top/Main menu",
 }
 PREDEFINED_SCAN_MENU_KEYS = ["1","2","3","4","5","6","7","8","9","10"]
 PREDEFINED_SCAN_MENU_TEXTS = [
-    "Volume Scanners | High Momentum | Breaking Out Now | ATR Cross",
+    "Volume Scanners | High Momentum | Breaking Out Now | ATR Cross     ",
     "Volume Scanners | High Momentum | ATR Cross",
-    "Volume Scanners | High Momentum",
+    "Volume Scanners | High Momentum                                    ",
     "Volume Scanners | ATR Cross",
-    "Volume Scanners | High Bid/Ask Build Up",
+    "Volume Scanners | High Bid/Ask Build Up                            ",
     "High Momentum | ATR Cross",
-    "High Momentum | ATR Trailing Stop",
+    "High Momentum | ATR Trailing Stop                                  ",
     "ATR Cross | ATR Trailing Stop",
-    "TTM Sqeeze Buy | Intraday RSI b/w 0 to 54",
+    "TTM Sqeeze Buy | Intraday RSI b/w 0 to 54                          ",
     "Volume Scanners | ATR Cross | Intraday RSI b/w 0 to 54",
 ]
 level2_P_MenuDict = {}
 for key in PREDEFINED_SCAN_MENU_KEYS:
     level2_P_MenuDict[key] = PREDEFINED_SCAN_MENU_TEXTS[int(key)-1]
 level2_P_MenuDict["M"] = "Back to the Top/Main menu"
 PREDEFINED_SCAN_MENU_VALUES =[
@@ -600,15 +600,15 @@
                 OutputControls().printOutput(
                     colorText.BOLD
                     + menuText
                     + """
 
     Enter your choice > (default is """
                     + colorText.WARN
-                    + self.find("X").keyTextLabel()
+                    + (self.find("X") or menu().create('?','?')).keyTextLabel().strip()
                     + ") "
                     "" + colorText.END
                 )
                 try:
                     OTAUpdater.checkForUpdate(VERSION, skipDownload=True)
                 except:
                     pass
@@ -681,15 +681,15 @@
                 OutputControls().printOutput(
                     colorText.BOLD
                     + menuText
                     + """
 
     Enter your choice > (default is """
                     + colorText.WARN
-                    + self.find(defaultKey).keyTextLabel()
+                    + (self.find(defaultKey) or menu().create('?','?')).keyTextLabel().strip()
                     + ")  "
                     "" + colorText.END
                 )
             return menuText
         
     def renderLevel1_P_Menus(
         self, skip=[], asList=False, renderStyle=None, parent=None
@@ -716,29 +716,29 @@
                 OutputControls().printOutput(
                     colorText.BOLD
                     + menuText
                     + """
 
     Enter your choice > (default is """
                     + colorText.WARN
-                    + self.find('1').keyTextLabel()
+                    + (self.find('1') or menu().create('?','?')).keyTextLabel().strip()
                     + ")  "
                     "" + colorText.END
                 )
             return menuText
 
     def renderLevel2_P_Menus(
         self, skip=[], asList=False, renderStyle=None, parent=None
     ):
         menuText = self.fromDictionary(
             level2_P_MenuDict,
             renderExceptionKeys=["M"],
             renderStyle=renderStyle
             if renderStyle is not None
-            else MenuRenderStyle.STANDALONE,
+            else MenuRenderStyle.TWO_PER_ROW,
             skip=skip,
             parent=parent,
         ).render(asList=asList,coloredValues=["1"])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
@@ -751,15 +751,15 @@
                 OutputControls().printOutput(
                     colorText.BOLD
                     + menuText
                     + """
 
     Enter your choice > (default is """
                     + colorText.WARN
-                    + self.find('1').keyTextLabel()
+                    + (self.find('1') or menu().create('?','?')).keyTextLabel().strip()
                     + ")  "
                     "" + colorText.END
                 )
             return menuText
         
     def renderLevel1_X_Menus(
         self, skip=[], asList=False, renderStyle=None, parent=None
@@ -786,15 +786,15 @@
                 OutputControls().printOutput(
                     colorText.BOLD
                     + menuText
                     + """
 
     Enter your choice > (default is """
                     + colorText.WARN
-                    + self.find(str(configManager.defaultIndex)).keyTextLabel()
+                    + (self.find(str(configManager.defaultIndex)) or menu().create('?','?')).keyTextLabel().strip()
                     + ")  "
                     "" + colorText.END
                 )
             return menuText
 
     def level2_T_MenuDict_L(
         self, skip=[], asList=False, renderStyle=None, parent=None
@@ -821,15 +821,15 @@
                 OutputControls().printOutput(
                     colorText.BOLD
                     + menuText
                     + """
 
     Enter your choice > (default is """
                     + colorText.WARN
-                    + self.find("1").keyTextLabel()
+                    + (self.find("1") or menu().create('?','?')).keyTextLabel().strip()
                     + ")  "
                     "" + colorText.END
                 )
             return menuText
 
     def level2_T_MenuDict_S(
         self, skip=[], asList=False, renderStyle=None, parent=None
@@ -856,15 +856,15 @@
                 OutputControls().printOutput(
                     colorText.BOLD
                     + menuText
                     + """
 
     Enter your choice > (default is """
                     + colorText.WARN
-                    + self.find("1").keyTextLabel()
+                    + (self.find("1") or menu().create('?','?')).keyTextLabel().strip()
                     + ")  "
                     "" + colorText.END
                 )
             return menuText
         
     def renderLevel2_X_Menus(
         self, skip=[], asList=False, renderStyle=None, parent=None
@@ -891,15 +891,15 @@
                 OutputControls().printOutput(
                     colorText.BOLD
                     + menuText
                     + """
 
     Enter your choice > (default is """
                     + colorText.WARN
-                    + self.find("9").keyTextLabel().strip() + ")"
+                    + (self.find("9") or menu().create('?','?')).keyTextLabel().strip() + ")"
                     + colorText.END
                 )
             return menuText
 
     def renderLevel3_X_Reversal_Menus(
         self, skip=[], asList=False, renderStyle=None, parent=None
     ):
@@ -925,15 +925,15 @@
                 OutputControls().printOutput(
                     colorText.BOLD
                     + menuText
                     + """
 
     Enter your choice > (default is """
                     + colorText.WARN
-                    + self.find("3").keyTextLabel().strip() + ")"
+                    + (self.find("3") or menu().create('?','?')).keyTextLabel().strip() + ")"
                     + colorText.END
                 )
             return menuText
 
     def renderLevel3_X_ChartPattern_Menus(
         self, skip=[], asList=False, renderStyle=MenuRenderStyle.STANDALONE, parent=None
     ):
@@ -959,15 +959,15 @@
                 OutputControls().printOutput(
                     colorText.BOLD
                     + menuText
                     + """
 
     Enter your choice > (default is """
                     + colorText.WARN
-                    + self.find("3").keyTextLabel().strip() + ")"
+                    + (self.find("3") or menu().create('?','?')).keyTextLabel().strip() + ")"
                     + colorText.END
                 )
             return menuText
 
     def renderLevel3_X_PopularStocks_Menus(
         self, skip=[], asList=False, renderStyle=MenuRenderStyle.STANDALONE, parent=None
     ):
@@ -993,15 +993,15 @@
                 OutputControls().printOutput(
                     colorText.BOLD
                     + menuText
                     + """
 
     Enter your choice > (default is """
                     + colorText.WARN
-                    + self.find("1").keyTextLabel().strip() + ")"
+                    + ((self.find("1")) or menu().create('?','?')).keyTextLabel().strip() + ")"
                     + colorText.END
                 )
             return menuText
 
     def renderLevel3_X_StockPerformance_Menus(
         self, skip=[], asList=False, renderStyle=MenuRenderStyle.STANDALONE, parent=None
     ):
@@ -1027,15 +1027,15 @@
                 OutputControls().printOutput(
                     colorText.BOLD
                     + menuText
                     + """
 
     Enter your choice > (default is """
                     + colorText.WARN
-                    + self.find("1").keyTextLabel().strip() + ")"
+                    + (self.find("1") or menu().create('?','?')).keyTextLabel().strip() + ")"
                     + colorText.END
                 )
             return menuText
 
     def renderLevel4_X_Lorenzian_Menus(
         self, skip=[], asList=False, renderStyle=MenuRenderStyle.STANDALONE, parent=None
     ):
@@ -1061,15 +1061,15 @@
                 OutputControls().printOutput(
                     colorText.BOLD
                     + menuText
                     + """
 
     Enter your choice > (default is """
                     + colorText.WARN
-                    + self.find("1").keyTextLabel().strip() + ")"
+                    + (self.find("1") or menu().create('?','?')).keyTextLabel().strip() + ")"
                     + colorText.END
                 )
             return menuText
 
 
     def renderLevel4_X_ChartPattern_BBands_SQZ_Menus(
         self, skip=[], asList=False, renderStyle=MenuRenderStyle.STANDALONE, parent=None
@@ -1096,15 +1096,15 @@
                 OutputControls().printOutput(
                     colorText.BOLD
                     + menuText
                     + """
 
     Enter your choice > (default is """
                     + colorText.WARN
-                    + self.find("1").keyTextLabel().strip() + ")"
+                    + (self.find("1") or menu().create('?','?')).keyTextLabel().strip() + ")"
                     + colorText.END
                 )
             return menuText
 
 
     def renderLevel4_X_ChartPattern_Confluence_Menus(
         self, skip=[], asList=False, renderStyle=MenuRenderStyle.STANDALONE, parent=None
@@ -1131,15 +1131,15 @@
                 OutputControls().printOutput(
                     colorText.BOLD
                     + menuText
                     + """
 
     Enter your choice > (default is """
                     + colorText.WARN
-                    + self.find("1").keyTextLabel().strip() + ")"
+                    + (self.find("1") or menu().create('?','?')).keyTextLabel().strip() + ")"
                     + colorText.END
                 )
             return menuText
         
 # Fundamentally good compnaies but nearing 52 week low
 # https://www.tickertape.in/screener/equity/prebuilt/SCR0005
```

### Comparing `pkscreener-0.44.20240516.378/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240516.379/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240516.379/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240516.379/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240516.379/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240516.379/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240516.379/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240516.379/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240516.379/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240516.379/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240516.379/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240516.379/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240516.379/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240516.379/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240516.379/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240516.379/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/classes/keys.py` & `pkscreener-0.44.20240516.379/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/courbd.ttf` & `pkscreener-0.44.20240516.379/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/globals.py` & `pkscreener-0.44.20240516.379/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240516.379/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240516.379/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240516.379/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240516.379/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240516.378
+Version: 0.44.20240516.379
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240516.378.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240516.379.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.377/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.378/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.377/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.378/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240515.377/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240516.378/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240516.378/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240516.379/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240516.378/setup.py` & `pkscreener-0.44.20240516.379/setup.py`

 * *Files identical despite different names*

