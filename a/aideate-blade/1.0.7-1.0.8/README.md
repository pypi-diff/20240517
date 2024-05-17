# Comparing `tmp/aideate_blade-1.0.7.tar.gz` & `tmp/aideate_blade-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aideate_blade-1.0.7.tar", last modified: Fri May 17 16:56:10 2024, max compression
+gzip compressed data, was "aideate_blade-1.0.8.tar", last modified: Fri May 17 17:37:27 2024, max compression
```

## Comparing `aideate_blade-1.0.7.tar` & `aideate_blade-1.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 16:56:10.986886 aideate_blade-1.0.7/
--rw-r--r--   0 xiayewang   (501) staff       (20)     1073 2024-05-15 22:37:32.000000 aideate_blade-1.0.7/LICENSE
--rw-r--r--   0 xiayewang   (501) staff       (20)      918 2024-05-17 16:56:10.986708 aideate_blade-1.0.7/PKG-INFO
--rw-r--r--   0 xiayewang   (501) staff       (20)      239 2024-05-16 18:26:11.000000 aideate_blade-1.0.7/README.md
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 16:56:10.986440 aideate_blade-1.0.7/aideate_blade.egg-info/
--rw-r--r--   0 xiayewang   (501) staff       (20)      918 2024-05-17 16:56:10.000000 aideate_blade-1.0.7/aideate_blade.egg-info/PKG-INFO
--rw-r--r--   0 xiayewang   (501) staff       (20)      654 2024-05-17 16:56:10.000000 aideate_blade-1.0.7/aideate_blade.egg-info/SOURCES.txt
--rw-r--r--   0 xiayewang   (501) staff       (20)        1 2024-05-17 16:56:10.000000 aideate_blade-1.0.7/aideate_blade.egg-info/dependency_links.txt
--rw-r--r--   0 xiayewang   (501) staff       (20)      410 2024-05-17 16:56:10.000000 aideate_blade-1.0.7/aideate_blade.egg-info/requires.txt
--rw-r--r--   0 xiayewang   (501) staff       (20)       16 2024-05-17 16:56:10.000000 aideate_blade-1.0.7/aideate_blade.egg-info/top_level.txt
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 16:56:10.984093 aideate_blade-1.0.7/aideate_scraper/
--rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 22:37:32.000000 aideate_blade-1.0.7/aideate_scraper/__init__.py
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 16:56:10.985712 aideate_blade-1.0.7/aideate_scraper/core/
--rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 22:37:32.000000 aideate_blade-1.0.7/aideate_scraper/core/__init__.py
--rw-r--r--   0 xiayewang   (501) staff       (20)     2552 2024-05-16 18:26:11.000000 aideate_blade-1.0.7/aideate_scraper/core/doc_utils.py
--rw-r--r--   0 xiayewang   (501) staff       (20)     7003 2024-05-17 16:42:23.000000 aideate_blade-1.0.7/aideate_scraper/core/eval.py
--rw-r--r--   0 xiayewang   (501) staff       (20)     8106 2024-05-16 18:26:11.000000 aideate_blade-1.0.7/aideate_scraper/core/image_utils.py
--rw-r--r--   0 xiayewang   (501) staff       (20)     8345 2024-05-16 18:26:11.000000 aideate_blade-1.0.7/aideate_scraper/core/s3_utils.py
--rw-r--r--   0 xiayewang   (501) staff       (20)      897 2024-05-17 16:42:14.000000 aideate_blade-1.0.7/aideate_scraper/core/schemas.py
--rw-r--r--   0 xiayewang   (501) staff       (20)    13663 2024-05-17 16:42:14.000000 aideate_blade-1.0.7/aideate_scraper/core/scrape.py
--rw-r--r--   0 xiayewang   (501) staff       (20)     1963 2024-05-17 16:42:14.000000 aideate_blade-1.0.7/aideate_scraper/core/scrape_playwright.py
--rw-r--r--   0 xiayewang   (501) staff       (20)     3892 2024-05-15 22:37:32.000000 aideate_blade-1.0.7/aideate_scraper/core/scrape_utils.py
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 16:56:10.986216 aideate_blade-1.0.7/aideate_scraper/modal/
--rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 22:37:32.000000 aideate_blade-1.0.7/aideate_scraper/modal/__init__.py
--rw-r--r--   0 xiayewang   (501) staff       (20)      520 2024-05-16 18:26:11.000000 aideate_blade-1.0.7/aideate_scraper/modal/modal_client.py
--rw-r--r--   0 xiayewang   (501) staff       (20)      755 2024-05-16 18:26:11.000000 aideate_blade-1.0.7/aideate_scraper/modal/modal_tasks.py
--rw-r--r--   0 xiayewang   (501) staff       (20)       38 2024-05-17 16:56:10.986919 aideate_blade-1.0.7/setup.cfg
--rw-r--r--   0 xiayewang   (501) staff       (20)      996 2024-05-17 16:56:06.000000 aideate_blade-1.0.7/setup.py
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 17:37:27.660273 aideate_blade-1.0.8/
+-rw-r--r--   0 xiayewang   (501) staff       (20)     1073 2024-05-15 22:37:32.000000 aideate_blade-1.0.8/LICENSE
+-rw-r--r--   0 xiayewang   (501) staff       (20)      918 2024-05-17 17:37:27.660052 aideate_blade-1.0.8/PKG-INFO
+-rw-r--r--   0 xiayewang   (501) staff       (20)      239 2024-05-16 18:26:11.000000 aideate_blade-1.0.8/README.md
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 17:37:27.659686 aideate_blade-1.0.8/aideate_blade.egg-info/
+-rw-r--r--   0 xiayewang   (501) staff       (20)      918 2024-05-17 17:37:27.000000 aideate_blade-1.0.8/aideate_blade.egg-info/PKG-INFO
+-rw-r--r--   0 xiayewang   (501) staff       (20)      654 2024-05-17 17:37:27.000000 aideate_blade-1.0.8/aideate_blade.egg-info/SOURCES.txt
+-rw-r--r--   0 xiayewang   (501) staff       (20)        1 2024-05-17 17:37:27.000000 aideate_blade-1.0.8/aideate_blade.egg-info/dependency_links.txt
+-rw-r--r--   0 xiayewang   (501) staff       (20)      410 2024-05-17 17:37:27.000000 aideate_blade-1.0.8/aideate_blade.egg-info/requires.txt
+-rw-r--r--   0 xiayewang   (501) staff       (20)       16 2024-05-17 17:37:27.000000 aideate_blade-1.0.8/aideate_blade.egg-info/top_level.txt
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 17:37:27.656158 aideate_blade-1.0.8/aideate_scraper/
+-rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 22:37:32.000000 aideate_blade-1.0.8/aideate_scraper/__init__.py
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 17:37:27.658608 aideate_blade-1.0.8/aideate_scraper/core/
+-rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 22:37:32.000000 aideate_blade-1.0.8/aideate_scraper/core/__init__.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)     2552 2024-05-16 18:26:11.000000 aideate_blade-1.0.8/aideate_scraper/core/doc_utils.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)     7003 2024-05-17 17:31:01.000000 aideate_blade-1.0.8/aideate_scraper/core/eval.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)     8106 2024-05-16 18:26:11.000000 aideate_blade-1.0.8/aideate_scraper/core/image_utils.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)     8345 2024-05-16 18:26:11.000000 aideate_blade-1.0.8/aideate_scraper/core/s3_utils.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)      897 2024-05-17 16:42:14.000000 aideate_blade-1.0.8/aideate_scraper/core/schemas.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)    14055 2024-05-17 17:31:36.000000 aideate_blade-1.0.8/aideate_scraper/core/scrape.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)     1963 2024-05-17 16:42:14.000000 aideate_blade-1.0.8/aideate_scraper/core/scrape_playwright.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)     3892 2024-05-15 22:37:32.000000 aideate_blade-1.0.8/aideate_scraper/core/scrape_utils.py
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 17:37:27.659209 aideate_blade-1.0.8/aideate_scraper/modal/
+-rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 22:37:32.000000 aideate_blade-1.0.8/aideate_scraper/modal/__init__.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)      486 2024-05-17 17:31:36.000000 aideate_blade-1.0.8/aideate_scraper/modal/modal_client.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)      715 2024-05-17 17:31:36.000000 aideate_blade-1.0.8/aideate_scraper/modal/modal_tasks.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)       38 2024-05-17 17:37:27.660323 aideate_blade-1.0.8/setup.cfg
+-rw-r--r--   0 xiayewang   (501) staff       (20)      996 2024-05-17 17:37:17.000000 aideate_blade-1.0.8/setup.py
```

### Comparing `aideate_blade-1.0.7/LICENSE` & `aideate_blade-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.7/PKG-INFO` & `aideate_blade-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aideate-blade
-Version: 1.0.7
+Version: 1.0.8
 Summary: web content aideate_scraper
 Author: Aideate
 Author-email: xiaye@aideate.ai
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: ipdb==0.13.11
 Requires-Dist: simplejson==3.17.6
```

### Comparing `aideate_blade-1.0.7/aideate_blade.egg-info/PKG-INFO` & `aideate_blade-1.0.8/aideate_blade.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aideate-blade
-Version: 1.0.7
+Version: 1.0.8
 Summary: web content aideate_scraper
 Author: Aideate
 Author-email: xiaye@aideate.ai
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: ipdb==0.13.11
 Requires-Dist: simplejson==3.17.6
```

### Comparing `aideate_blade-1.0.7/aideate_blade.egg-info/SOURCES.txt` & `aideate_blade-1.0.8/aideate_blade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.7/aideate_scraper/core/doc_utils.py` & `aideate_blade-1.0.8/aideate_scraper/core/doc_utils.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.7/aideate_scraper/core/eval.py` & `aideate_blade-1.0.8/aideate_scraper/core/eval.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.7/aideate_scraper/core/image_utils.py` & `aideate_blade-1.0.8/aideate_scraper/core/image_utils.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.7/aideate_scraper/core/s3_utils.py` & `aideate_blade-1.0.8/aideate_scraper/core/s3_utils.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.7/aideate_scraper/core/schemas.py` & `aideate_blade-1.0.8/aideate_scraper/core/schemas.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.7/aideate_scraper/core/scrape.py` & `aideate_blade-1.0.8/aideate_scraper/core/scrape.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from snakemd import Document as mdDocument
 from tenacity import retry, retry_if_exception_type, stop_after_attempt, wait_fixed
 
 from aideate_scraper.core.doc_utils import doc_manager
 from aideate_scraper.core.image_utils import image_manager
 from aideate_scraper.core.schemas import WebScrapeContent, WebContentType
 from aideate_scraper.core.scrape_playwright import aget_playwright
+from aideate_scraper.modal.modal_client import playwright_web_scrape as modal_playwright_web_scrape
 from aideate_scraper.core.scrape_utils import TIMEOUT_SEC, get_user_agent
 from settings import ZENROWS_API_KEY
 
 logger = logging.getLogger(__name__)
 
 
 GET_COUNTER = Counter("blade_scrape_get_request", "Number of get requests")
@@ -248,15 +249,16 @@
 
 
 def is_instagram_url(url: str) -> bool:
     return "instagram.com" in url
 
 
 async def ascrape_web(
-    url: str
+    url: str,
+    playwright_modal: bool = True,
 ) -> Optional[WebScrapeContent]:
     if not is_instagram_url(url):
         # instagram doesn't work for these options but in general we want them first
 
         content = await aget_scrape_api(url)
         response = await process_web_content(content, url)
         if response:
@@ -264,37 +266,47 @@
 
         # fallback to requests
         content = await aget(url)
         response = await process_web_content(content, url)
         if response:
             return response
 
-    content = await aget_playwright(url)
+    if playwright_modal:
+        content = await modal_playwright_web_scrape(url)
+    else:
+        content = await aget_playwright(url)
     response = await process_web_content(content, url)
     if response:
         return response
 
     return None
 
 
-async def async_scrape_web_content(url: str) -> Optional[Union[str, bytes]]:
+async def async_scrape_web_content(
+    url: str,
+    playwright_modal: bool = True,
+) -> Optional[Union[str, bytes]]:
     # scrape without parsing
     if not is_instagram_url(url):
         # instagram doesn't work for these options but in general we want them first
 
         content = await aget_scrape_api(url)
         if content:
             return content
 
         # fallback to requests
         content = await aget(url)
         if content:
             return content
 
-    return await aget_playwright(url)
+    if playwright_modal:
+        content = await modal_playwright_web_scrape(url)
+    else:
+        content = await aget_playwright(url)
+    return content
 
 
 class ContentExceedMaxLimit(Exception):
     pass
 
 
 def make_default_headers(user_agent: str) -> dict:
```

### Comparing `aideate_blade-1.0.7/aideate_scraper/core/scrape_playwright.py` & `aideate_blade-1.0.8/aideate_scraper/core/scrape_playwright.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.7/aideate_scraper/core/scrape_utils.py` & `aideate_blade-1.0.8/aideate_scraper/core/scrape_utils.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.7/aideate_scraper/modal/modal_tasks.py` & `aideate_blade-1.0.8/aideate_scraper/modal/modal_tasks.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# from typing import List, Optional
-#
-# from modal import Function, Image, Mount, Secret, Stub, asgi_app, gpu, method
-#
-# import proto.gen.message_pb2 as message_pb2
-# from modal_functions.tasks.base import image
-#
-# workers_stub = Stub("web-scraper", image=image)
-#
-#
-# @workers_stub.function(secrets=[Secret.from_name("my-aws-secret")])
-# async def playwright_web_scrape(url) -> Optional[message_pb2.DocumentMessage]:
-#     from aideate_scraper.core.scrape_playwright import aget_playwright
-#
-#     result = await aget_playwright(url)
-#     return result
-#
-#
-# # Test each method
-# @workers_stub.local_entrypoint()
-# async def test_methods():
-#     print(
-#         playwright_web_scrape.remote(url="https://www.youtube.com/shorts/o0Q6mK-hSIw")
-#     )
+from typing import List, Optional
+
+from modal import Function, Image, Mount, Secret, Stub, asgi_app, gpu, method
+
+import proto.gen.message_pb2 as message_pb2
+from modal_functions.tasks.base import image
+
+workers_stub = Stub("web-scraper", image=image)
+
+
+@workers_stub.function(secrets=[Secret.from_name("my-aws-secret")])
+async def playwright_web_scrape(url) -> Optional[message_pb2.DocumentMessage]:
+    from aideate_scraper.core.scrape_playwright import aget_playwright
+
+    result = await aget_playwright(url)
+    return result
+
+
+# Test each method
+@workers_stub.local_entrypoint()
+async def test_methods():
+    print(
+        playwright_web_scrape.remote(url="https://www.youtube.com/shorts/o0Q6mK-hSIw")
+    )
```

### Comparing `aideate_blade-1.0.7/setup.py` & `aideate_blade-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='aideate-blade',
-    version='1.0.7',
+    version='1.0.8',
     description='web content aideate_scraper',
     author='Aideate',
     author_email='xiaye@aideate.ai',
     packages=find_packages(),
     install_requires=[
         # List your dependencies here
         "pydantic==2.6.1",
```

