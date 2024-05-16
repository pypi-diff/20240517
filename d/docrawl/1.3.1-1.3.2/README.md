# Comparing `tmp/docrawl-1.3.1.tar.gz` & `tmp/docrawl-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docrawl-1.3.1.tar", last modified: Fri May 10 08:27:04 2024, max compression
+gzip compressed data, was "docrawl-1.3.2.tar", last modified: Thu May 16 23:12:41 2024, max compression
```

## Comparing `docrawl-1.3.1.tar` & `docrawl-1.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 08:27:04.495024 docrawl-1.3.1/
--rw-rw-rw-   0        0        0     1090 2024-03-01 01:29:38.000000 docrawl-1.3.1/LICENSE
--rw-rw-rw-   0        0        0      527 2024-05-10 08:27:04.493512 docrawl-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-03-01 01:29:38.000000 docrawl-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 08:27:04.430213 docrawl-1.3.1/docrawl/
--rw-rw-rw-   0        0        0        0 2024-03-01 01:29:38.000000 docrawl-1.3.1/docrawl/__init__.py
--rw-rw-rw-   0        0        0    13103 2024-05-10 08:26:51.000000 docrawl-1.3.1/docrawl/docrawl_client.py
--rw-rw-rw-   0        0        0    43228 2024-05-10 08:26:51.000000 docrawl-1.3.1/docrawl/docrawl_core.py
--rw-rw-rw-   0        0        0     6847 2024-03-01 01:29:38.000000 docrawl-1.3.1/docrawl/docrawl_launcher.py
--rw-rw-rw-   0        0        0     1108 2024-03-01 01:29:38.000000 docrawl-1.3.1/docrawl/docrawl_logger.py
--rw-rw-rw-   0        0        0     2674 2024-03-01 01:29:38.000000 docrawl-1.3.1/docrawl/elements.py
--rw-rw-rw-   0        0        0       49 2024-05-10 08:26:51.000000 docrawl-1.3.1/docrawl/errors.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:27:04.492520 docrawl-1.3.1/docrawl.egg-info/
--rw-rw-rw-   0        0        0      527 2024-05-10 08:27:04.000000 docrawl-1.3.1/docrawl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-05-10 08:27:04.000000 docrawl-1.3.1/docrawl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 08:27:04.000000 docrawl-1.3.1/docrawl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2024-05-10 08:27:04.000000 docrawl-1.3.1/docrawl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-10 08:27:04.000000 docrawl-1.3.1/docrawl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 08:27:04.495024 docrawl-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      834 2024-05-10 08:26:31.000000 docrawl-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 23:12:41.436941 docrawl-1.3.2/
+-rw-rw-rw-   0        0        0     1090 2024-03-01 01:29:38.000000 docrawl-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0      527 2024-05-16 23:12:41.434938 docrawl-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-03-01 01:29:38.000000 docrawl-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 23:12:41.409381 docrawl-1.3.2/docrawl/
+-rw-rw-rw-   0        0        0        0 2024-03-01 01:29:38.000000 docrawl-1.3.2/docrawl/__init__.py
+-rw-rw-rw-   0        0        0    13161 2024-05-16 23:10:20.000000 docrawl-1.3.2/docrawl/docrawl_client.py
+-rw-rw-rw-   0        0        0    43228 2024-05-10 08:26:51.000000 docrawl-1.3.2/docrawl/docrawl_core.py
+-rw-rw-rw-   0        0        0     6847 2024-03-01 01:29:38.000000 docrawl-1.3.2/docrawl/docrawl_launcher.py
+-rw-rw-rw-   0        0        0     1108 2024-03-01 01:29:38.000000 docrawl-1.3.2/docrawl/docrawl_logger.py
+-rw-rw-rw-   0        0        0     2674 2024-03-01 01:29:38.000000 docrawl-1.3.2/docrawl/elements.py
+-rw-rw-rw-   0        0        0      100 2024-05-16 23:10:20.000000 docrawl-1.3.2/docrawl/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-16 23:12:41.434429 docrawl-1.3.2/docrawl.egg-info/
+-rw-rw-rw-   0        0        0      527 2024-05-16 23:12:41.000000 docrawl-1.3.2/docrawl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-05-16 23:12:41.000000 docrawl-1.3.2/docrawl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 23:12:41.000000 docrawl-1.3.2/docrawl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2024-05-16 23:12:41.000000 docrawl-1.3.2/docrawl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-16 23:12:41.000000 docrawl-1.3.2/docrawl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 23:12:41.436941 docrawl-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      834 2024-05-16 23:10:45.000000 docrawl-1.3.2/setup.py
```

### Comparing `docrawl-1.3.1/LICENSE` & `docrawl-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `docrawl-1.3.1/PKG-INFO` & `docrawl-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrawl
-Version: 1.3.1
+Version: 1.3.2
 Summary: Do automated crawling of pages using scrapy
 Home-page: https://github.com/DovaX/docrawl
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `docrawl-1.3.1/docrawl/docrawl_client.py` & `docrawl-1.3.2/docrawl/docrawl_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import psutil
 from crochet import setup
 from scrapy.crawler import CrawlerRunner
 
 from docrawl.docrawl_core import DocrawlSpider
 from docrawl.docrawl_logger import docrawl_logger
-from docrawl.errors import SpiderFunctionError
+from docrawl.errors import PageDidNotLoadError, SpiderFunctionError
 from keepvariable.keepvariable_core import KeepVariableDummyRedisServer
 
 
 @dataclass
 class DocrawlSettings:
     pid: int
     driver: str
@@ -92,14 +92,15 @@
             time.sleep(0.5)
             # docrawl_logger.info('Page is still loading, waiting 0.5 sec ...')
 
         if is_page_loaded:
             docrawl_logger.success('Page loaded')
         else:
             docrawl_logger.error('Page was not loaded')
+            raise PageDidNotLoadError()
 
     def _wait_until_function_is_done(self, timeout):
         # Load spider_requests and spider_functions
         try:
             spider_function = self.get_browser_meta_data()['function']
             is_function_done = spider_function['done']
             function_error_message = spider_function['error']
@@ -248,47 +249,44 @@
             'filename': filename
         }
 
         self._execute_function('get_current_url', inp, timeout)
 
     def close_browser(self, timeout=10):
         """Launch close_browser function from core."""
-
         self._execute_function('close_browser', None, timeout)
 
         pid = self.get_browser_meta_data()['browser']['pid']
 
         with suppress(Exception):
             psutil.Process(pid).terminate()
 
         docrawl_logger.warning(f'Is browser closed: {self.is_browser_active()}')
 
     def scroll_web_page(self, scroll_to, scroll_by, scroll_max, timeout=20):
         """
         Launches scroll_web_page function from core.
             :param scroll_to: string, scroll direction (Up/Down)
             :param scroll_by: int, scroll distance
-            :param scroll_max: bool, scroll to maximum
+            :param scroll_max: bool, scroll to maximum.
         """
-
         inp = {
             'scroll_to': scroll_to,
             'scroll_by': scroll_by,
             'scroll_max': scroll_max
         }
 
         self._execute_function('scroll_web_page', inp, timeout)
 
     def download_images(self, image_xpath, filename, timeout=20):
         """
         Launches download_image function from core.
             :param image_xpath: string, url of image
-            :param filename: string, output filename
+            :param filename: string, output filename.
         """
-
         inp = {
             'image_xpath': image_xpath,
             'filename': filename,
         }
 
         self._execute_function('download_images', inp, timeout)
```

### Comparing `docrawl-1.3.1/docrawl/docrawl_core.py` & `docrawl-1.3.2/docrawl/docrawl_core.py`

 * *Files identical despite different names*

### Comparing `docrawl-1.3.1/docrawl/docrawl_launcher.py` & `docrawl-1.3.2/docrawl/docrawl_launcher.py`

 * *Files identical despite different names*

### Comparing `docrawl-1.3.1/docrawl/docrawl_logger.py` & `docrawl-1.3.2/docrawl/docrawl_logger.py`

 * *Files identical despite different names*

### Comparing `docrawl-1.3.1/docrawl/elements.py` & `docrawl-1.3.2/docrawl/elements.py`

 * *Files identical despite different names*

### Comparing `docrawl-1.3.1/docrawl.egg-info/PKG-INFO` & `docrawl-1.3.2/docrawl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrawl
-Version: 1.3.1
+Version: 1.3.2
 Summary: Do automated crawling of pages using scrapy
 Home-page: https://github.com/DovaX/docrawl
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `docrawl-1.3.1/setup.py` & `docrawl-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='docrawl',
-    version='1.3.1',
+    version='1.3.2',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='Do automated crawling of pages using scrapy',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/docrawl',
     packages=setuptools.find_packages(),
```

