# Comparing `tmp/trengine-1.1.tar.gz` & `tmp/trengine-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trengine-1.1.tar", last modified: Tue May 14 23:54:43 2024, max compression
+gzip compressed data, was "trengine-1.2.tar", last modified: Thu May 16 23:26:59 2024, max compression
```

## Comparing `trengine-1.1.tar` & `trengine-1.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 23:54:43.255517 trengine-1.1/
--rw-rw-rw-   0        0        0     1080 2024-05-14 23:33:59.000000 trengine-1.1/LICENSE
--rw-rw-rw-   0        0        0     1770 2024-05-14 23:54:43.253523 trengine-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1170 2024-05-14 23:53:46.000000 trengine-1.1/README.md
--rw-rw-rw-   0        0        0      573 2024-05-14 23:53:58.000000 trengine-1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-14 23:54:43.256514 trengine-1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-14 23:54:43.205650 trengine-1.1/trengine/
--rw-rw-rw-   0        0        0     1117 2024-05-14 23:31:04.000000 trengine-1.1/trengine/__init__.py
--rw-rw-rw-   0        0        0     3191 2024-05-14 23:31:17.000000 trengine-1.1/trengine/ajax.py
--rw-rw-rw-   0        0        0       42 2024-05-14 22:39:42.000000 trengine-1.1/trengine/exceptions.py
--rw-rw-rw-   0        0        0     1425 2024-05-14 23:31:17.000000 trengine-1.1/trengine/google.py
--rw-rw-rw-   0        0        0     1783 2024-05-14 23:31:17.000000 trengine-1.1/trengine/hozory.py
--rw-rw-rw-   0        0        0      968 2024-05-14 23:31:17.000000 trengine-1.1/trengine/tdict.py
--rw-rw-rw-   0        0        0     1776 2024-05-14 23:12:07.000000 trengine-1.1/trengine/types.py
-drwxrwxrwx   0        0        0        0 2024-05-14 23:54:43.251528 trengine-1.1/trengine.egg-info/
--rw-rw-rw-   0        0        0     1770 2024-05-14 23:54:43.000000 trengine-1.1/trengine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2024-05-14 23:54:43.000000 trengine-1.1/trengine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 23:54:43.000000 trengine-1.1/trengine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-14 23:54:43.000000 trengine-1.1/trengine.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-14 23:54:43.000000 trengine-1.1/trengine.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 23:26:59.352201 trengine-1.2/
+-rw-rw-rw-   0        0        0     1080 2024-05-16 22:50:59.000000 trengine-1.2/LICENSE
+-rw-rw-rw-   0        0        0     1961 2024-05-16 23:26:59.339235 trengine-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1336 2024-05-16 23:25:50.000000 trengine-1.2/README.md
+-rw-rw-rw-   0        0        0      587 2024-05-16 23:21:24.000000 trengine-1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 23:26:59.352201 trengine-1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-16 23:26:59.144755 trengine-1.2/trengine/
+-rw-rw-rw-   0        0        0     1284 2024-05-16 23:18:11.000000 trengine-1.2/trengine/__init__.py
+-rw-rw-rw-   0        0        0     3191 2024-05-16 22:50:59.000000 trengine-1.2/trengine/ajax.py
+-rw-rw-rw-   0        0        0       42 2024-05-16 22:50:59.000000 trengine-1.2/trengine/exceptions.py
+-rw-rw-rw-   0        0        0     1425 2024-05-16 22:50:59.000000 trengine-1.2/trengine/google.py
+-rw-rw-rw-   0        0        0     1783 2024-05-16 22:50:59.000000 trengine-1.2/trengine/hozory.py
+-rw-rw-rw-   0        0        0     3013 2024-05-16 23:20:58.000000 trengine-1.2/trengine/ocr.py
+-rw-rw-rw-   0        0        0      968 2024-05-16 22:50:59.000000 trengine-1.2/trengine/tdict.py
+-rw-rw-rw-   0        0        0     1776 2024-05-16 22:50:59.000000 trengine-1.2/trengine/types.py
+drwxrwxrwx   0        0        0        0 2024-05-16 23:26:59.338237 trengine-1.2/trengine.egg-info/
+-rw-rw-rw-   0        0        0     1961 2024-05-16 23:26:58.000000 trengine-1.2/trengine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-05-16 23:26:59.000000 trengine-1.2/trengine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 23:26:58.000000 trengine-1.2/trengine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-16 23:26:58.000000 trengine-1.2/trengine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-16 23:26:58.000000 trengine-1.2/trengine.egg-info/top_level.txt
```

### Comparing `trengine-1.1/LICENSE` & `trengine-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trengine-1.1/PKG-INFO` & `trengine-1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: trengine
-Version: 1.1
+Version: 1.2
 Summary: TREngine is python library based on 4 translators engines
 Author-email: ZAID <y8838@hotmail.com>
 Project-URL: Homepage, https://github.com/zaid5o5/trengine
 Project-URL: Issues, https://github.com/zaid5o5/trengine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: asyncio
 Requires-Dist: requests
+Requires-Dist: aiofiles
 
 # Install:
 ```commandline
 pip install trengine
 ```
 
 # About this project:
-- TREngine is python library based on 4 translators engines:
+- TREngine is python library based on 4 translators engines with OCR:
 - Ajax ( [translate.com](https://www.translate.com/translator) )
 - Google ( [translate.google.com](https://translate.google.com/) )
 - Hozory ( [hozory.com](https://hozory.com/FA) )
 - Translatedict ( [translatedict.com](https://www.translatedict.com/) )
+- OCR ( [ocr.space](https://ocr.space/) )
 
 - Supporting Sync & Async.
 
 # How to use?
 - Here an example to use it:
 ```python
 from trengine import Engine
@@ -39,14 +41,17 @@
 
 print(
     eng.google.translate(text, "en"), "\n",
     eng.ajax.translate(text, "en"), "\n",
     eng.hozory.translate(text, "en"), "\n",
     eng.tdict.translate(text, "en"), "\n",
 )
+
+# OCR
+print(eng.ocr.from_image("./test.png"))
 ```
 - Here an async example:
 ```python
 import asyncio
 from trengine import AsyncEngine
 
 eng = AsyncEngine()
@@ -56,9 +61,12 @@
     print(
         await eng.google.translate(text, "en"), "\n",
         await eng.ajax.translate(text, "en"), "\n",
         await eng.hozory.translate(text, "en"), "\n",
         await eng.tdict.translate(text, "en"), "\n",
     )
 
+    # OCR
+    print(await eng.ocr.from_image("./test.png"))
+
 asyncio.run(main())
 ```
```

### Comparing `trengine-1.1/README.md` & `trengine-1.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Install:
 ```commandline
 pip install trengine
 ```
 
 # About this project:
-- TREngine is python library based on 4 translators engines:
+- TREngine is python library based on 4 translators engines with OCR:
 - Ajax ( [translate.com](https://www.translate.com/translator) )
 - Google ( [translate.google.com](https://translate.google.com/) )
 - Hozory ( [hozory.com](https://hozory.com/FA) )
 - Translatedict ( [translatedict.com](https://www.translatedict.com/) )
+- OCR ( [ocr.space](https://ocr.space/) )
 
 - Supporting Sync & Async.
 
 # How to use?
 - Here an example to use it:
 ```python
 from trengine import Engine
@@ -22,14 +23,17 @@
 
 print(
     eng.google.translate(text, "en"), "\n",
     eng.ajax.translate(text, "en"), "\n",
     eng.hozory.translate(text, "en"), "\n",
     eng.tdict.translate(text, "en"), "\n",
 )
+
+# OCR
+print(eng.ocr.from_image("./test.png"))
 ```
 - Here an async example:
 ```python
 import asyncio
 from trengine import AsyncEngine
 
 eng = AsyncEngine()
@@ -39,9 +43,12 @@
     print(
         await eng.google.translate(text, "en"), "\n",
         await eng.ajax.translate(text, "en"), "\n",
         await eng.hozory.translate(text, "en"), "\n",
         await eng.tdict.translate(text, "en"), "\n",
     )
 
+    # OCR
+    print(await eng.ocr.from_image("./test.png"))
+
 asyncio.run(main())
 ```
```

### Comparing `trengine-1.1/pyproject.toml` & `trengine-1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "trengine"
-version = "1.1"
+version = "1.2"
 authors = [
   { name="ZAID", email="y8838@hotmail.com" },
 ]
 description = "TREngine is python library based on 4 translators engines"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -12,12 +12,13 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "aiohttp",
   "asyncio",
   "requests",
+  "aiofiles"
 ]
 
 [project.urls]
 Homepage = "https://github.com/zaid5o5/trengine"
 Issues = "https://github.com/zaid5o5/trengine/issues"
```

### Comparing `trengine-1.1/trengine/__init__.py` & `trengine-1.2/trengine/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from . import ajax, google, hozory, tdict
+from . import ajax, google, hozory, tdict, ocr
 
 __all__ = ["AsyncEngine", "Engine"]
 
 
 class Engine:
     def __init__(self) -> None:
         pass
@@ -19,14 +19,18 @@
     def hozory(self) -> "hozory.HozoryTranslator":
         return hozory.HozoryTranslator()
 
     @property
     def tdict(self) -> "tdict.TdictTranslator":
         return tdict.TdictTranslator()
 
+    @property
+    def ocr(self) -> "ocr.OCR":
+        return ocr.OCR()
+
 
 class AsyncEngine:
     def __init__(self) -> None:
         pass
 
     @property
     def ajax(self) -> "ajax.AsyncAjaxTranslator":
@@ -39,7 +43,11 @@
     @property
     def hozory(self) -> "hozory.AsyncHozoryTranslator":
         return hozory.AsyncHozoryTranslator()
 
     @property
     def tdict(self) -> "tdict.AsyncTdictTranslator":
         return tdict.AsyncTdictTranslator()
+
+    @property
+    def ocr(self) -> "ocr.AsyncOCR":
+        return ocr.AsyncOCR()
```

### Comparing `trengine-1.1/trengine/ajax.py` & `trengine-1.2/trengine/ajax.py`

 * *Files identical despite different names*

### Comparing `trengine-1.1/trengine/google.py` & `trengine-1.2/trengine/google.py`

 * *Files identical despite different names*

### Comparing `trengine-1.1/trengine/hozory.py` & `trengine-1.2/trengine/hozory.py`

 * *Files identical despite different names*

### Comparing `trengine-1.1/trengine/tdict.py` & `trengine-1.2/trengine/tdict.py`

 * *Files identical despite different names*

### Comparing `trengine-1.1/trengine/types.py` & `trengine-1.2/trengine/types.py`

 * *Files identical despite different names*

### Comparing `trengine-1.1/trengine.egg-info/PKG-INFO` & `trengine-1.2/trengine.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: trengine
-Version: 1.1
+Version: 1.2
 Summary: TREngine is python library based on 4 translators engines
 Author-email: ZAID <y8838@hotmail.com>
 Project-URL: Homepage, https://github.com/zaid5o5/trengine
 Project-URL: Issues, https://github.com/zaid5o5/trengine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: asyncio
 Requires-Dist: requests
+Requires-Dist: aiofiles
 
 # Install:
 ```commandline
 pip install trengine
 ```
 
 # About this project:
-- TREngine is python library based on 4 translators engines:
+- TREngine is python library based on 4 translators engines with OCR:
 - Ajax ( [translate.com](https://www.translate.com/translator) )
 - Google ( [translate.google.com](https://translate.google.com/) )
 - Hozory ( [hozory.com](https://hozory.com/FA) )
 - Translatedict ( [translatedict.com](https://www.translatedict.com/) )
+- OCR ( [ocr.space](https://ocr.space/) )
 
 - Supporting Sync & Async.
 
 # How to use?
 - Here an example to use it:
 ```python
 from trengine import Engine
@@ -39,14 +41,17 @@
 
 print(
     eng.google.translate(text, "en"), "\n",
     eng.ajax.translate(text, "en"), "\n",
     eng.hozory.translate(text, "en"), "\n",
     eng.tdict.translate(text, "en"), "\n",
 )
+
+# OCR
+print(eng.ocr.from_image("./test.png"))
 ```
 - Here an async example:
 ```python
 import asyncio
 from trengine import AsyncEngine
 
 eng = AsyncEngine()
@@ -56,9 +61,12 @@
     print(
         await eng.google.translate(text, "en"), "\n",
         await eng.ajax.translate(text, "en"), "\n",
         await eng.hozory.translate(text, "en"), "\n",
         await eng.tdict.translate(text, "en"), "\n",
     )
 
+    # OCR
+    print(await eng.ocr.from_image("./test.png"))
+
 asyncio.run(main())
 ```
```

