# Comparing `tmp/9gag_scraper-0.0.2.tar.gz` & `tmp/9gag_scraper-0.0.3.tar.gz`

## Comparing `9gag_scraper-0.0.2.tar` & `9gag_scraper-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 9gag_scraper-0.0.2/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 9gag_scraper-0.0.2/LICENCE.md
--rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 9gag_scraper-0.0.2/README.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 9gag_scraper-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 9gag_scraper-0.0.2/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 9gag_scraper-0.0.2/src/9gag_scraper/__init__.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 9gag_scraper-0.0.2/src/9gag_scraper/controller.py
--rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 9gag_scraper-0.0.2/src/9gag_scraper/gui.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 9gag_scraper-0.0.2/src/9gag_scraper/main.py
--rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 9gag_scraper-0.0.2/src/9gag_scraper/scraper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 9gag_scraper-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 9gag_scraper-0.0.2/tests/test_scraper.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 9gag_scraper-0.0.2/.gitignore
--rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 9gag_scraper-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 9gag_scraper-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 9gag_scraper-0.0.3/LICENCE.md
+-rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 9gag_scraper-0.0.3/README.md
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 9gag_scraper-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 9gag_scraper-0.0.3/requirements.txt
+-rw-r--r--   0        0        0     9256 2020-02-02 00:00:00.000000 9gag_scraper-0.0.3/dist/9gag_scraper-0.0.2--none-any.whl
+-rw-r--r--   0        0        0     7846 2020-02-02 00:00:00.000000 9gag_scraper-0.0.3/dist/9gag_scraper-0.0.2.tar.gz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 9gag_scraper-0.0.3/src/9gag_scraper/__init__.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 9gag_scraper-0.0.3/src/9gag_scraper/controller.py
+-rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 9gag_scraper-0.0.3/src/9gag_scraper/gui.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 9gag_scraper-0.0.3/src/9gag_scraper/main.py
+-rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 9gag_scraper-0.0.3/src/9gag_scraper/scraper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 9gag_scraper-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 9gag_scraper-0.0.3/tests/test_scraper.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 9gag_scraper-0.0.3/.gitignore
+-rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 9gag_scraper-0.0.3/PKG-INFO
```

### Comparing `9gag_scraper-0.0.2/LICENCE.md` & `9gag_scraper-0.0.3/LICENCE.md`

 * *Files identical despite different names*

### Comparing `9gag_scraper-0.0.2/README.md` & `9gag_scraper-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `9gag_scraper-0.0.2/pyproject.toml` & `9gag_scraper-0.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "9gag_scraper"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Federlizer", email="federlizer@protonmail.com" },
 ]
 description = "A simple 9GAG scraper"
 readme = "README.md"
-requires-python = "==2.7.18"
+requires-python = ">=2.7"
 classifiers = [
     "Programming Language :: Python :: 2",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `9gag_scraper-0.0.2/src/9gag_scraper/controller.py` & `9gag_scraper-0.0.3/src/9gag_scraper/controller.py`

 * *Files identical despite different names*

### Comparing `9gag_scraper-0.0.2/src/9gag_scraper/gui.py` & `9gag_scraper-0.0.3/src/9gag_scraper/gui.py`

 * *Files identical despite different names*

### Comparing `9gag_scraper-0.0.2/src/9gag_scraper/main.py` & `9gag_scraper-0.0.3/src/9gag_scraper/main.py`

 * *Files identical despite different names*

### Comparing `9gag_scraper-0.0.2/src/9gag_scraper/scraper.py` & `9gag_scraper-0.0.3/src/9gag_scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `9gag_scraper-0.0.2/tests/test_scraper.py` & `9gag_scraper-0.0.3/tests/test_scraper.py`

 * *Files identical despite different names*

### Comparing `9gag_scraper-0.0.2/PKG-INFO` & `9gag_scraper-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: 9gag-scraper
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple 9GAG scraper
 Project-URL: Homepage, https://github.com/federlizer-strypes/9gag-scraper
 Project-URL: Issues, https://github.com/federlizer-strypes/9gag-scraper/issues
 Author-email: Federlizer <federlizer@protonmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
-Requires-Python: ==2.7.18
+Requires-Python: >=2.7
 Description-Content-Type: text/markdown
 
 # 9GAG Scraper
 
 A simple 9GAG scraper that uses selenium's Chromium webdriver. It allows you to scrape the images given a particular
 search term. The application is written in Python 2.7 with Tkinter 8.6.
```

