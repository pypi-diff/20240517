# Comparing `tmp/9gag_scraper-0.0.5.tar.gz` & `tmp/9gag_scraper-0.0.6.tar.gz`

## Comparing `9gag_scraper-0.0.5.tar` & `9gag_scraper-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 9gag_scraper-0.0.5/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 9gag_scraper-0.0.5/LICENCE.md
--rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 9gag_scraper-0.0.5/README.md
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 9gag_scraper-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 9gag_scraper-0.0.5/requirements.txt
--rw-r--r--   0        0        0     9256 2020-02-02 00:00:00.000000 9gag_scraper-0.0.5/dist/9gag_scraper-0.0.2--none-any.whl
--rw-r--r--   0        0        0     7846 2020-02-02 00:00:00.000000 9gag_scraper-0.0.5/dist/9gag_scraper-0.0.2.tar.gz
--rw-r--r--   0        0        0     9263 2020-02-02 00:00:00.000000 9gag_scraper-0.0.5/dist/9gag_scraper-0.0.3-py2.py3-none-any.whl
--rw-r--r--   0        0        0    27208 2020-02-02 00:00:00.000000 9gag_scraper-0.0.5/dist/9gag_scraper-0.0.3.tar.gz
--rw-r--r--   0        0        0     9271 2020-02-02 00:00:00.000000 9gag_scraper-0.0.5/dist/9gag_scraper-0.0.4-py2.py3-none-any.whl
--rw-r--r--   0        0        0    57006 2020-02-02 00:00:00.000000 9gag_scraper-0.0.5/dist/9gag_scraper-0.0.4.tar.gz
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 9gag_scraper-0.0.5/src/9gag_scraper/__init__.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 9gag_scraper-0.0.5/src/9gag_scraper/__main__.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 9gag_scraper-0.0.5/src/9gag_scraper/controller.py
--rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 9gag_scraper-0.0.5/src/9gag_scraper/gui.py
--rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 9gag_scraper-0.0.5/src/9gag_scraper/scraper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 9gag_scraper-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 9gag_scraper-0.0.5/tests/test_scraper.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 9gag_scraper-0.0.5/.gitignore
--rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 9gag_scraper-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 9gag_scraper-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 9gag_scraper-0.0.6/LICENCE.md
+-rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 9gag_scraper-0.0.6/README.md
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 9gag_scraper-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 9gag_scraper-0.0.6/requirements.txt
+-rw-r--r--   0        0        0     9256 2020-02-02 00:00:00.000000 9gag_scraper-0.0.6/dist/9gag_scraper-0.0.2--none-any.whl
+-rw-r--r--   0        0        0     7846 2020-02-02 00:00:00.000000 9gag_scraper-0.0.6/dist/9gag_scraper-0.0.2.tar.gz
+-rw-r--r--   0        0        0     9263 2020-02-02 00:00:00.000000 9gag_scraper-0.0.6/dist/9gag_scraper-0.0.3-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    27208 2020-02-02 00:00:00.000000 9gag_scraper-0.0.6/dist/9gag_scraper-0.0.3.tar.gz
+-rw-r--r--   0        0        0     9271 2020-02-02 00:00:00.000000 9gag_scraper-0.0.6/dist/9gag_scraper-0.0.4-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    57006 2020-02-02 00:00:00.000000 9gag_scraper-0.0.6/dist/9gag_scraper-0.0.4.tar.gz
+-rw-r--r--   0        0        0     9306 2020-02-02 00:00:00.000000 9gag_scraper-0.0.6/dist/9gag_scraper-0.0.5-py2.py3-none-any.whl
+-rw-r--r--   0        0        0   122648 2020-02-02 00:00:00.000000 9gag_scraper-0.0.6/dist/9gag_scraper-0.0.5.tar.gz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 9gag_scraper-0.0.6/src/9gag_scraper/__init__.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 9gag_scraper-0.0.6/src/9gag_scraper/__main__.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 9gag_scraper-0.0.6/src/9gag_scraper/controller.py
+-rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 9gag_scraper-0.0.6/src/9gag_scraper/gui.py
+-rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 9gag_scraper-0.0.6/src/9gag_scraper/scraper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 9gag_scraper-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 9gag_scraper-0.0.6/tests/test_scraper.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 9gag_scraper-0.0.6/.gitignore
+-rw-r--r--   0        0        0     5149 2020-02-02 00:00:00.000000 9gag_scraper-0.0.6/PKG-INFO
```

### Comparing `9gag_scraper-0.0.5/LICENCE.md` & `9gag_scraper-0.0.6/LICENCE.md`

 * *Files identical despite different names*

### Comparing `9gag_scraper-0.0.5/README.md` & `9gag_scraper-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `9gag_scraper-0.0.5/pyproject.toml` & `9gag_scraper-0.0.6/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "9gag_scraper"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Federlizer", email="federlizer@protonmail.com" },
 ]
 description = "A simple 9GAG scraper"
 readme = "README.md"
 requires-python = ">=2.7"
 classifiers = [
     "Programming Language :: Python :: 2",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "selenium==3.141.0",
+    "backports.functools-lru-cache==1.6.6",
+    "beautifulsoup4==4.9.3",
+    "bs4==0.0.2",
+    "certifi==2021.10.8",
+    "chardet==4.0.0",
+    "idna==2.10",
+    "Pillow==6.2.2",
     "requests==2.27.1",
+    "selenium==3.141.0",
+    "soupsieve==1.9.6",
+    "urllib3==1.26.18",
 ]
 
 [project.urls]
 Homepage = "https://github.com/federlizer-strypes/9gag-scraper"
 Issues = "https://github.com/federlizer-strypes/9gag-scraper/issues"
```

### Comparing `9gag_scraper-0.0.5/dist/9gag_scraper-0.0.2--none-any.whl` & `9gag_scraper-0.0.6/dist/9gag_scraper-0.0.2--none-any.whl`

 * *Files identical despite different names*

### Comparing `9gag_scraper-0.0.5/dist/9gag_scraper-0.0.2.tar.gz` & `9gag_scraper-0.0.6/dist/9gag_scraper-0.0.2.tar.gz`

 * *Files identical despite different names*

### Comparing `9gag_scraper-0.0.5/dist/9gag_scraper-0.0.3-py2.py3-none-any.whl` & `9gag_scraper-0.0.6/dist/9gag_scraper-0.0.3-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `9gag_scraper-0.0.5/dist/9gag_scraper-0.0.3.tar.gz` & `9gag_scraper-0.0.6/dist/9gag_scraper-0.0.3.tar.gz`

 * *Files identical despite different names*

### Comparing `9gag_scraper-0.0.5/dist/9gag_scraper-0.0.4-py2.py3-none-any.whl` & `9gag_scraper-0.0.6/dist/9gag_scraper-0.0.4-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `9gag_scraper-0.0.5/dist/9gag_scraper-0.0.4.tar.gz` & `9gag_scraper-0.0.6/dist/9gag_scraper-0.0.4.tar.gz`

 * *Files identical despite different names*

### Comparing `9gag_scraper-0.0.5/src/9gag_scraper/__main__.py` & `9gag_scraper-0.0.6/src/9gag_scraper/__main__.py`

 * *Files identical despite different names*

### Comparing `9gag_scraper-0.0.5/src/9gag_scraper/controller.py` & `9gag_scraper-0.0.6/src/9gag_scraper/controller.py`

 * *Files identical despite different names*

### Comparing `9gag_scraper-0.0.5/src/9gag_scraper/gui.py` & `9gag_scraper-0.0.6/src/9gag_scraper/gui.py`

 * *Files identical despite different names*

### Comparing `9gag_scraper-0.0.5/src/9gag_scraper/scraper.py` & `9gag_scraper-0.0.6/src/9gag_scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `9gag_scraper-0.0.5/tests/test_scraper.py` & `9gag_scraper-0.0.6/tests/test_scraper.py`

 * *Files identical despite different names*

### Comparing `9gag_scraper-0.0.5/PKG-INFO` & `9gag_scraper-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 Metadata-Version: 2.1
 Name: 9gag-scraper
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple 9GAG scraper
 Project-URL: Homepage, https://github.com/federlizer-strypes/9gag-scraper
 Project-URL: Issues, https://github.com/federlizer-strypes/9gag-scraper/issues
 Author-email: Federlizer <federlizer@protonmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Requires-Python: >=2.7
+Requires-Dist: backports-functools-lru-cache==1.6.6
+Requires-Dist: beautifulsoup4==4.9.3
+Requires-Dist: bs4==0.0.2
+Requires-Dist: certifi==2021.10.8
+Requires-Dist: chardet==4.0.0
+Requires-Dist: idna==2.10
+Requires-Dist: pillow==6.2.2
 Requires-Dist: requests==2.27.1
 Requires-Dist: selenium==3.141.0
+Requires-Dist: soupsieve==1.9.6
+Requires-Dist: urllib3==1.26.18
 Description-Content-Type: text/markdown
 
 # 9GAG Scraper
 
 A simple 9GAG scraper that uses selenium's Chromium webdriver. It allows you to scrape the images given a particular
 search term. The application is written in Python 2.7 with Tkinter 8.6.
```

