# Comparing `tmp/aideate_blade-1.0.8.tar.gz` & `tmp/aideate_blade-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aideate_blade-1.0.8.tar", last modified: Fri May 17 17:37:27 2024, max compression
+gzip compressed data, was "aideate_blade-1.0.9.tar", last modified: Fri May 17 20:12:06 2024, max compression
```

## Comparing `aideate_blade-1.0.8.tar` & `aideate_blade-1.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 17:37:27.660273 aideate_blade-1.0.8/
--rw-r--r--   0 xiayewang   (501) staff       (20)     1073 2024-05-15 22:37:32.000000 aideate_blade-1.0.8/LICENSE
--rw-r--r--   0 xiayewang   (501) staff       (20)      918 2024-05-17 17:37:27.660052 aideate_blade-1.0.8/PKG-INFO
--rw-r--r--   0 xiayewang   (501) staff       (20)      239 2024-05-16 18:26:11.000000 aideate_blade-1.0.8/README.md
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 17:37:27.659686 aideate_blade-1.0.8/aideate_blade.egg-info/
--rw-r--r--   0 xiayewang   (501) staff       (20)      918 2024-05-17 17:37:27.000000 aideate_blade-1.0.8/aideate_blade.egg-info/PKG-INFO
--rw-r--r--   0 xiayewang   (501) staff       (20)      654 2024-05-17 17:37:27.000000 aideate_blade-1.0.8/aideate_blade.egg-info/SOURCES.txt
--rw-r--r--   0 xiayewang   (501) staff       (20)        1 2024-05-17 17:37:27.000000 aideate_blade-1.0.8/aideate_blade.egg-info/dependency_links.txt
--rw-r--r--   0 xiayewang   (501) staff       (20)      410 2024-05-17 17:37:27.000000 aideate_blade-1.0.8/aideate_blade.egg-info/requires.txt
--rw-r--r--   0 xiayewang   (501) staff       (20)       16 2024-05-17 17:37:27.000000 aideate_blade-1.0.8/aideate_blade.egg-info/top_level.txt
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 17:37:27.656158 aideate_blade-1.0.8/aideate_scraper/
--rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 22:37:32.000000 aideate_blade-1.0.8/aideate_scraper/__init__.py
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 17:37:27.658608 aideate_blade-1.0.8/aideate_scraper/core/
--rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 22:37:32.000000 aideate_blade-1.0.8/aideate_scraper/core/__init__.py
--rw-r--r--   0 xiayewang   (501) staff       (20)     2552 2024-05-16 18:26:11.000000 aideate_blade-1.0.8/aideate_scraper/core/doc_utils.py
--rw-r--r--   0 xiayewang   (501) staff       (20)     7003 2024-05-17 17:31:01.000000 aideate_blade-1.0.8/aideate_scraper/core/eval.py
--rw-r--r--   0 xiayewang   (501) staff       (20)     8106 2024-05-16 18:26:11.000000 aideate_blade-1.0.8/aideate_scraper/core/image_utils.py
--rw-r--r--   0 xiayewang   (501) staff       (20)     8345 2024-05-16 18:26:11.000000 aideate_blade-1.0.8/aideate_scraper/core/s3_utils.py
--rw-r--r--   0 xiayewang   (501) staff       (20)      897 2024-05-17 16:42:14.000000 aideate_blade-1.0.8/aideate_scraper/core/schemas.py
--rw-r--r--   0 xiayewang   (501) staff       (20)    14055 2024-05-17 17:31:36.000000 aideate_blade-1.0.8/aideate_scraper/core/scrape.py
--rw-r--r--   0 xiayewang   (501) staff       (20)     1963 2024-05-17 16:42:14.000000 aideate_blade-1.0.8/aideate_scraper/core/scrape_playwright.py
--rw-r--r--   0 xiayewang   (501) staff       (20)     3892 2024-05-15 22:37:32.000000 aideate_blade-1.0.8/aideate_scraper/core/scrape_utils.py
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 17:37:27.659209 aideate_blade-1.0.8/aideate_scraper/modal/
--rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 22:37:32.000000 aideate_blade-1.0.8/aideate_scraper/modal/__init__.py
--rw-r--r--   0 xiayewang   (501) staff       (20)      486 2024-05-17 17:31:36.000000 aideate_blade-1.0.8/aideate_scraper/modal/modal_client.py
--rw-r--r--   0 xiayewang   (501) staff       (20)      715 2024-05-17 17:31:36.000000 aideate_blade-1.0.8/aideate_scraper/modal/modal_tasks.py
--rw-r--r--   0 xiayewang   (501) staff       (20)       38 2024-05-17 17:37:27.660323 aideate_blade-1.0.8/setup.cfg
--rw-r--r--   0 xiayewang   (501) staff       (20)      996 2024-05-17 17:37:17.000000 aideate_blade-1.0.8/setup.py
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 20:12:06.770680 aideate_blade-1.0.9/
+-rw-r--r--   0 xiayewang   (501) staff       (20)     1073 2024-05-15 22:37:32.000000 aideate_blade-1.0.9/LICENSE
+-rw-r--r--   0 xiayewang   (501) staff       (20)      918 2024-05-17 20:12:06.770477 aideate_blade-1.0.9/PKG-INFO
+-rw-r--r--   0 xiayewang   (501) staff       (20)      239 2024-05-16 18:26:11.000000 aideate_blade-1.0.9/README.md
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 20:12:06.770164 aideate_blade-1.0.9/aideate_blade.egg-info/
+-rw-r--r--   0 xiayewang   (501) staff       (20)      918 2024-05-17 20:12:06.000000 aideate_blade-1.0.9/aideate_blade.egg-info/PKG-INFO
+-rw-r--r--   0 xiayewang   (501) staff       (20)      654 2024-05-17 20:12:06.000000 aideate_blade-1.0.9/aideate_blade.egg-info/SOURCES.txt
+-rw-r--r--   0 xiayewang   (501) staff       (20)        1 2024-05-17 20:12:06.000000 aideate_blade-1.0.9/aideate_blade.egg-info/dependency_links.txt
+-rw-r--r--   0 xiayewang   (501) staff       (20)      410 2024-05-17 20:12:06.000000 aideate_blade-1.0.9/aideate_blade.egg-info/requires.txt
+-rw-r--r--   0 xiayewang   (501) staff       (20)       16 2024-05-17 20:12:06.000000 aideate_blade-1.0.9/aideate_blade.egg-info/top_level.txt
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 20:12:06.767227 aideate_blade-1.0.9/aideate_scraper/
+-rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 22:37:32.000000 aideate_blade-1.0.9/aideate_scraper/__init__.py
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 20:12:06.769385 aideate_blade-1.0.9/aideate_scraper/core/
+-rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 22:37:32.000000 aideate_blade-1.0.9/aideate_scraper/core/__init__.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)     2552 2024-05-16 18:26:11.000000 aideate_blade-1.0.9/aideate_scraper/core/doc_utils.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)     7003 2024-05-17 17:31:01.000000 aideate_blade-1.0.9/aideate_scraper/core/eval.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)     8106 2024-05-16 18:26:11.000000 aideate_blade-1.0.9/aideate_scraper/core/image_utils.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)     8345 2024-05-16 18:26:11.000000 aideate_blade-1.0.9/aideate_scraper/core/s3_utils.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)      897 2024-05-17 16:42:14.000000 aideate_blade-1.0.9/aideate_scraper/core/schemas.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)    14188 2024-05-17 20:10:55.000000 aideate_blade-1.0.9/aideate_scraper/core/scrape.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)     1963 2024-05-17 16:42:14.000000 aideate_blade-1.0.9/aideate_scraper/core/scrape_playwright.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)     3892 2024-05-15 22:37:32.000000 aideate_blade-1.0.9/aideate_scraper/core/scrape_utils.py
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 20:12:06.769888 aideate_blade-1.0.9/aideate_scraper/modal/
+-rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 22:37:32.000000 aideate_blade-1.0.9/aideate_scraper/modal/__init__.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)      486 2024-05-17 17:31:36.000000 aideate_blade-1.0.9/aideate_scraper/modal/modal_client.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)      715 2024-05-17 17:31:36.000000 aideate_blade-1.0.9/aideate_scraper/modal/modal_tasks.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)       38 2024-05-17 20:12:06.770719 aideate_blade-1.0.9/setup.cfg
+-rw-r--r--   0 xiayewang   (501) staff       (20)      996 2024-05-17 20:11:19.000000 aideate_blade-1.0.9/setup.py
```

### Comparing `aideate_blade-1.0.8/LICENSE` & `aideate_blade-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.8/PKG-INFO` & `aideate_blade-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aideate-blade
-Version: 1.0.8
+Version: 1.0.9
 Summary: web content aideate_scraper
 Author: Aideate
 Author-email: xiaye@aideate.ai
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: ipdb==0.13.11
 Requires-Dist: simplejson==3.17.6
```

### Comparing `aideate_blade-1.0.8/aideate_blade.egg-info/PKG-INFO` & `aideate_blade-1.0.9/aideate_blade.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aideate-blade
-Version: 1.0.8
+Version: 1.0.9
 Summary: web content aideate_scraper
 Author: Aideate
 Author-email: xiaye@aideate.ai
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: ipdb==0.13.11
 Requires-Dist: simplejson==3.17.6
```

### Comparing `aideate_blade-1.0.8/aideate_blade.egg-info/SOURCES.txt` & `aideate_blade-1.0.9/aideate_blade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.8/aideate_scraper/core/doc_utils.py` & `aideate_blade-1.0.9/aideate_scraper/core/doc_utils.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.8/aideate_scraper/core/eval.py` & `aideate_blade-1.0.9/aideate_scraper/core/eval.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.8/aideate_scraper/core/image_utils.py` & `aideate_blade-1.0.9/aideate_scraper/core/image_utils.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.8/aideate_scraper/core/s3_utils.py` & `aideate_blade-1.0.9/aideate_scraper/core/s3_utils.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.8/aideate_scraper/core/schemas.py` & `aideate_blade-1.0.9/aideate_scraper/core/schemas.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.8/aideate_scraper/core/scrape.py` & `aideate_blade-1.0.9/aideate_scraper/core/scrape.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,35 +250,36 @@
 
 def is_instagram_url(url: str) -> bool:
     return "instagram.com" in url
 
 
 async def ascrape_web(
     url: str,
+    persist_content: bool = True,
     playwright_modal: bool = True,
 ) -> Optional[WebScrapeContent]:
     if not is_instagram_url(url):
         # instagram doesn't work for these options but in general we want them first
 
         content = await aget_scrape_api(url)
-        response = await process_web_content(content, url)
+        response = await process_web_content(content, url, persist_content=persist_content)
         if response:
             return response
 
         # fallback to requests
         content = await aget(url)
-        response = await process_web_content(content, url)
+        response = await process_web_content(content, url, persist_content=persist_content)
         if response:
             return response
 
     if playwright_modal:
         content = await modal_playwright_web_scrape(url)
     else:
         content = await aget_playwright(url)
-    response = await process_web_content(content, url)
+    response = await process_web_content(content, url, persist_content=persist_content)
     if response:
         return response
 
     return None
 
 
 async def async_scrape_web_content(
```

### Comparing `aideate_blade-1.0.8/aideate_scraper/core/scrape_playwright.py` & `aideate_blade-1.0.9/aideate_scraper/core/scrape_playwright.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.8/aideate_scraper/core/scrape_utils.py` & `aideate_blade-1.0.9/aideate_scraper/core/scrape_utils.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.8/aideate_scraper/modal/modal_tasks.py` & `aideate_blade-1.0.9/aideate_scraper/modal/modal_tasks.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.8/setup.py` & `aideate_blade-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='aideate-blade',
-    version='1.0.8',
+    version='1.0.9',
     description='web content aideate_scraper',
     author='Aideate',
     author_email='xiaye@aideate.ai',
     packages=find_packages(),
     install_requires=[
         # List your dependencies here
         "pydantic==2.6.1",
```

