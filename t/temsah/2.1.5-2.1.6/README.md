# Comparing `tmp/temsah-2.1.5.tar.gz` & `tmp/temsah-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temsah-2.1.5.tar", last modified: Wed May 15 19:02:05 2024, max compression
+gzip compressed data, was "temsah-2.1.6.tar", last modified: Fri May 17 16:39:44 2024, max compression
```

## Comparing `temsah-2.1.5.tar` & `temsah-2.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 19:02:05.306172 temsah-2.1.5/
--rw-rw-rw-   0        0        0     1095 2024-02-28 08:08:30.000000 temsah-2.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0      268 2024-05-15 19:02:05.303699 temsah-2.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1746 2024-04-09 22:22:13.000000 temsah-2.1.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-15 19:02:05.306172 temsah-2.1.5/setup.cfg
--rw-rw-rw-   0        0        0      395 2024-05-15 18:57:38.000000 temsah-2.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 19:02:05.273717 temsah-2.1.5/temsah/
--rw-rw-rw-   0        0        0       19 2024-02-22 20:21:12.000000 temsah-2.1.5/temsah/__init__.py
--rw-rw-rw-   0        0        0     3257 2024-05-13 14:37:04.000000 temsah-2.1.5/temsah/currency.py
--rw-rw-rw-   0        0        0    16801 2024-04-18 14:15:12.000000 temsah-2.1.5/temsah/data_extractor.py
--rw-rw-rw-   0        0        0     1695 2024-04-09 18:13:31.000000 temsah-2.1.5/temsah/main.py
-drwxrwxrwx   0        0        0        0 2024-05-15 19:02:05.300540 temsah-2.1.5/temsah.egg-info/
--rw-rw-rw-   0        0        0      268 2024-05-15 19:02:04.000000 temsah-2.1.5/temsah.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2024-05-15 19:02:04.000000 temsah-2.1.5/temsah.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 19:02:04.000000 temsah-2.1.5/temsah.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-15 19:02:04.000000 temsah-2.1.5/temsah.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-15 19:02:04.000000 temsah-2.1.5/temsah.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 16:39:44.101193 temsah-2.1.6/
+-rw-rw-rw-   0        0        0     1095 2024-02-28 08:08:30.000000 temsah-2.1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      268 2024-05-17 16:39:44.100196 temsah-2.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1746 2024-04-09 22:22:13.000000 temsah-2.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-17 16:39:44.102193 temsah-2.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      395 2024-05-17 16:38:18.000000 temsah-2.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 16:39:44.088232 temsah-2.1.6/temsah/
+-rw-rw-rw-   0        0        0       19 2024-02-22 20:21:12.000000 temsah-2.1.6/temsah/__init__.py
+-rw-rw-rw-   0        0        0     3269 2024-05-17 16:35:58.000000 temsah-2.1.6/temsah/currency.py
+-rw-rw-rw-   0        0        0    16801 2024-04-18 14:15:12.000000 temsah-2.1.6/temsah/data_extractor.py
+-rw-rw-rw-   0        0        0     1695 2024-04-09 18:13:31.000000 temsah-2.1.6/temsah/main.py
+drwxrwxrwx   0        0        0        0 2024-05-17 16:39:44.098203 temsah-2.1.6/temsah.egg-info/
+-rw-rw-rw-   0        0        0      268 2024-05-17 16:39:43.000000 temsah-2.1.6/temsah.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2024-05-17 16:39:43.000000 temsah-2.1.6/temsah.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 16:39:43.000000 temsah-2.1.6/temsah.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-17 16:39:43.000000 temsah-2.1.6/temsah.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-17 16:39:43.000000 temsah-2.1.6/temsah.egg-info/top_level.txt
```

### Comparing `temsah-2.1.5/LICENSE.txt` & `temsah-2.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `temsah-2.1.5/README.md` & `temsah-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `temsah-2.1.5/temsah/currency.py` & `temsah-2.1.6/temsah/currency.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from bs4 import BeautifulSoup
 import requests
 import chardet
 
 #-------------------------------------
 class Currency:
     def __init__(self):
-    self.url_aed = 'https://www.tgju.org/profile/price_aed'
-    self.url_dollar = 'https://www.tgju.org/profile/price_dollar_rl'
-    self.currency = {}
+        self.url_aed = 'https://www.tgju.org/profile/price_aed'
+        self.url_dollar = 'https://www.tgju.org/profile/price_dollar_rl'
+        self.currency = {}
 #-------------------------------------
 
     def scrape(self):
         self.currency = {}
         self.scrape_aed()
         self.scrape_dollar()
         return self.currency
```

### Comparing `temsah-2.1.5/temsah/data_extractor.py` & `temsah-2.1.6/temsah/data_extractor.py`

 * *Files identical despite different names*

### Comparing `temsah-2.1.5/temsah/main.py` & `temsah-2.1.6/temsah/main.py`

 * *Files identical despite different names*

