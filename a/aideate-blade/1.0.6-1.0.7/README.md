# Comparing `tmp/aideate_blade-1.0.6.tar.gz` & `tmp/aideate_blade-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aideate_blade-1.0.6.tar", last modified: Fri May 17 16:53:35 2024, max compression
+gzip compressed data, was "aideate_blade-1.0.7.tar", last modified: Fri May 17 16:56:10 2024, max compression
```

## Comparing `aideate_blade-1.0.6.tar` & `aideate_blade-1.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 16:53:35.056295 aideate_blade-1.0.6/
--rw-r--r--   0 xiayewang   (501) staff       (20)     1073 2024-05-15 22:37:32.000000 aideate_blade-1.0.6/LICENSE
--rw-r--r--   0 xiayewang   (501) staff       (20)      791 2024-05-17 16:53:35.056114 aideate_blade-1.0.6/PKG-INFO
--rw-r--r--   0 xiayewang   (501) staff       (20)      239 2024-05-16 18:26:11.000000 aideate_blade-1.0.6/README.md
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 16:53:35.055840 aideate_blade-1.0.6/aideate_blade.egg-info/
--rw-r--r--   0 xiayewang   (501) staff       (20)      791 2024-05-17 16:53:35.000000 aideate_blade-1.0.6/aideate_blade.egg-info/PKG-INFO
--rw-r--r--   0 xiayewang   (501) staff       (20)      654 2024-05-17 16:53:35.000000 aideate_blade-1.0.6/aideate_blade.egg-info/SOURCES.txt
--rw-r--r--   0 xiayewang   (501) staff       (20)        1 2024-05-17 16:53:35.000000 aideate_blade-1.0.6/aideate_blade.egg-info/dependency_links.txt
--rw-r--r--   0 xiayewang   (501) staff       (20)      343 2024-05-17 16:53:35.000000 aideate_blade-1.0.6/aideate_blade.egg-info/requires.txt
--rw-r--r--   0 xiayewang   (501) staff       (20)       16 2024-05-17 16:53:35.000000 aideate_blade-1.0.6/aideate_blade.egg-info/top_level.txt
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 16:53:35.053038 aideate_blade-1.0.6/aideate_scraper/
--rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 22:37:32.000000 aideate_blade-1.0.6/aideate_scraper/__init__.py
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 16:53:35.055118 aideate_blade-1.0.6/aideate_scraper/core/
--rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 22:37:32.000000 aideate_blade-1.0.6/aideate_scraper/core/__init__.py
--rw-r--r--   0 xiayewang   (501) staff       (20)     2552 2024-05-16 18:26:11.000000 aideate_blade-1.0.6/aideate_scraper/core/doc_utils.py
--rw-r--r--   0 xiayewang   (501) staff       (20)     7003 2024-05-17 16:42:23.000000 aideate_blade-1.0.6/aideate_scraper/core/eval.py
--rw-r--r--   0 xiayewang   (501) staff       (20)     8106 2024-05-16 18:26:11.000000 aideate_blade-1.0.6/aideate_scraper/core/image_utils.py
--rw-r--r--   0 xiayewang   (501) staff       (20)     8345 2024-05-16 18:26:11.000000 aideate_blade-1.0.6/aideate_scraper/core/s3_utils.py
--rw-r--r--   0 xiayewang   (501) staff       (20)      897 2024-05-17 16:42:14.000000 aideate_blade-1.0.6/aideate_scraper/core/schemas.py
--rw-r--r--   0 xiayewang   (501) staff       (20)    13663 2024-05-17 16:42:14.000000 aideate_blade-1.0.6/aideate_scraper/core/scrape.py
--rw-r--r--   0 xiayewang   (501) staff       (20)     1963 2024-05-17 16:42:14.000000 aideate_blade-1.0.6/aideate_scraper/core/scrape_playwright.py
--rw-r--r--   0 xiayewang   (501) staff       (20)     3892 2024-05-15 22:37:32.000000 aideate_blade-1.0.6/aideate_scraper/core/scrape_utils.py
-drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 16:53:35.055609 aideate_blade-1.0.6/aideate_scraper/modal/
--rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 22:37:32.000000 aideate_blade-1.0.6/aideate_scraper/modal/__init__.py
--rw-r--r--   0 xiayewang   (501) staff       (20)      520 2024-05-16 18:26:11.000000 aideate_blade-1.0.6/aideate_scraper/modal/modal_client.py
--rw-r--r--   0 xiayewang   (501) staff       (20)      755 2024-05-16 18:26:11.000000 aideate_blade-1.0.6/aideate_scraper/modal/modal_tasks.py
--rw-r--r--   0 xiayewang   (501) staff       (20)       38 2024-05-17 16:53:35.056330 aideate_blade-1.0.6/setup.cfg
--rw-r--r--   0 xiayewang   (501) staff       (20)      885 2024-05-17 16:53:28.000000 aideate_blade-1.0.6/setup.py
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 16:56:10.986886 aideate_blade-1.0.7/
+-rw-r--r--   0 xiayewang   (501) staff       (20)     1073 2024-05-15 22:37:32.000000 aideate_blade-1.0.7/LICENSE
+-rw-r--r--   0 xiayewang   (501) staff       (20)      918 2024-05-17 16:56:10.986708 aideate_blade-1.0.7/PKG-INFO
+-rw-r--r--   0 xiayewang   (501) staff       (20)      239 2024-05-16 18:26:11.000000 aideate_blade-1.0.7/README.md
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 16:56:10.986440 aideate_blade-1.0.7/aideate_blade.egg-info/
+-rw-r--r--   0 xiayewang   (501) staff       (20)      918 2024-05-17 16:56:10.000000 aideate_blade-1.0.7/aideate_blade.egg-info/PKG-INFO
+-rw-r--r--   0 xiayewang   (501) staff       (20)      654 2024-05-17 16:56:10.000000 aideate_blade-1.0.7/aideate_blade.egg-info/SOURCES.txt
+-rw-r--r--   0 xiayewang   (501) staff       (20)        1 2024-05-17 16:56:10.000000 aideate_blade-1.0.7/aideate_blade.egg-info/dependency_links.txt
+-rw-r--r--   0 xiayewang   (501) staff       (20)      410 2024-05-17 16:56:10.000000 aideate_blade-1.0.7/aideate_blade.egg-info/requires.txt
+-rw-r--r--   0 xiayewang   (501) staff       (20)       16 2024-05-17 16:56:10.000000 aideate_blade-1.0.7/aideate_blade.egg-info/top_level.txt
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 16:56:10.984093 aideate_blade-1.0.7/aideate_scraper/
+-rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 22:37:32.000000 aideate_blade-1.0.7/aideate_scraper/__init__.py
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 16:56:10.985712 aideate_blade-1.0.7/aideate_scraper/core/
+-rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 22:37:32.000000 aideate_blade-1.0.7/aideate_scraper/core/__init__.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)     2552 2024-05-16 18:26:11.000000 aideate_blade-1.0.7/aideate_scraper/core/doc_utils.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)     7003 2024-05-17 16:42:23.000000 aideate_blade-1.0.7/aideate_scraper/core/eval.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)     8106 2024-05-16 18:26:11.000000 aideate_blade-1.0.7/aideate_scraper/core/image_utils.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)     8345 2024-05-16 18:26:11.000000 aideate_blade-1.0.7/aideate_scraper/core/s3_utils.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)      897 2024-05-17 16:42:14.000000 aideate_blade-1.0.7/aideate_scraper/core/schemas.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)    13663 2024-05-17 16:42:14.000000 aideate_blade-1.0.7/aideate_scraper/core/scrape.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)     1963 2024-05-17 16:42:14.000000 aideate_blade-1.0.7/aideate_scraper/core/scrape_playwright.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)     3892 2024-05-15 22:37:32.000000 aideate_blade-1.0.7/aideate_scraper/core/scrape_utils.py
+drwxr-xr-x   0 xiayewang   (501) staff       (20)        0 2024-05-17 16:56:10.986216 aideate_blade-1.0.7/aideate_scraper/modal/
+-rw-r--r--   0 xiayewang   (501) staff       (20)        0 2024-05-15 22:37:32.000000 aideate_blade-1.0.7/aideate_scraper/modal/__init__.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)      520 2024-05-16 18:26:11.000000 aideate_blade-1.0.7/aideate_scraper/modal/modal_client.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)      755 2024-05-16 18:26:11.000000 aideate_blade-1.0.7/aideate_scraper/modal/modal_tasks.py
+-rw-r--r--   0 xiayewang   (501) staff       (20)       38 2024-05-17 16:56:10.986919 aideate_blade-1.0.7/setup.cfg
+-rw-r--r--   0 xiayewang   (501) staff       (20)      996 2024-05-17 16:56:06.000000 aideate_blade-1.0.7/setup.py
```

### Comparing `aideate_blade-1.0.6/LICENSE` & `aideate_blade-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.6/aideate_blade.egg-info/SOURCES.txt` & `aideate_blade-1.0.7/aideate_blade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.6/aideate_scraper/core/doc_utils.py` & `aideate_blade-1.0.7/aideate_scraper/core/doc_utils.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.6/aideate_scraper/core/eval.py` & `aideate_blade-1.0.7/aideate_scraper/core/eval.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.6/aideate_scraper/core/image_utils.py` & `aideate_blade-1.0.7/aideate_scraper/core/image_utils.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.6/aideate_scraper/core/s3_utils.py` & `aideate_blade-1.0.7/aideate_scraper/core/s3_utils.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.6/aideate_scraper/core/schemas.py` & `aideate_blade-1.0.7/aideate_scraper/core/schemas.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.6/aideate_scraper/core/scrape.py` & `aideate_blade-1.0.7/aideate_scraper/core/scrape.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.6/aideate_scraper/core/scrape_playwright.py` & `aideate_blade-1.0.7/aideate_scraper/core/scrape_playwright.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.6/aideate_scraper/core/scrape_utils.py` & `aideate_blade-1.0.7/aideate_scraper/core/scrape_utils.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.6/aideate_scraper/modal/modal_client.py` & `aideate_blade-1.0.7/aideate_scraper/modal/modal_client.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.6/aideate_scraper/modal/modal_tasks.py` & `aideate_blade-1.0.7/aideate_scraper/modal/modal_tasks.py`

 * *Files identical despite different names*

### Comparing `aideate_blade-1.0.6/setup.py` & `aideate_blade-1.0.7/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='aideate-blade',
-    version='1.0.6',
+    version='1.0.7',
     description='web content aideate_scraper',
     author='Aideate',
     author_email='xiaye@aideate.ai',
     packages=find_packages(),
     install_requires=[
         # List your dependencies here
         "pydantic==2.6.1",
@@ -26,9 +26,13 @@
         "extraction==0.3",
         "pdfplumber==0.11.0",
         "stripe==5.5.0",
         "python-magic==0.4.27",
         "StrEnum==0.4.15",
         "modal==0.61.105",
         "setuptools==69.5.1",
+        "tenacity==8.0.1",
+        "httpx==0.21.0",
+        "wandb==0.17.0",
+        "docstring_parser==0.16",
     ],
 )
```

