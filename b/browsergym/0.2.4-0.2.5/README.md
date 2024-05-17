# Comparing `tmp/browsergym-0.2.4-py3-none-any.whl.zip` & `tmp/browsergym-0.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 3645 bytes, number of entries: 5
--rw-r--r--  2.0 unx      579 b- defN 24-May-17 20:08 browsergym-0.2.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     5854 b- defN 24-May-17 20:08 browsergym-0.2.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-17 20:08 browsergym-0.2.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-May-17 20:08 browsergym-0.2.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      399 b- defN 24-May-17 20:08 browsergym-0.2.4.dist-info/RECORD
-5 files, 6925 bytes uncompressed, 2895 bytes compressed:  58.2%
+Zip file size: 3646 bytes, number of entries: 5
+-rw-r--r--  2.0 unx      579 b- defN 24-May-17 20:23 browsergym-0.2.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5854 b- defN 24-May-17 20:23 browsergym-0.2.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-17 20:23 browsergym-0.2.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-May-17 20:23 browsergym-0.2.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      399 b- defN 24-May-17 20:23 browsergym-0.2.5.dist-info/RECORD
+5 files, 6925 bytes uncompressed, 2896 bytes compressed:  58.2%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: browsergym-0.2.4.dist-info/LICENSE
+Filename: browsergym-0.2.5.dist-info/LICENSE
 Comment: 
 
-Filename: browsergym-0.2.4.dist-info/METADATA
+Filename: browsergym-0.2.5.dist-info/METADATA
 Comment: 
 
-Filename: browsergym-0.2.4.dist-info/WHEEL
+Filename: browsergym-0.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: browsergym-0.2.4.dist-info/top_level.txt
+Filename: browsergym-0.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: browsergym-0.2.4.dist-info/RECORD
+Filename: browsergym-0.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `browsergym-0.2.4.dist-info/LICENSE` & `browsergym-0.2.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `browsergym-0.2.4.dist-info/METADATA` & `browsergym-0.2.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: browsergym
-Version: 0.2.4
+Version: 0.2.5
 Summary: BrowserGym: a gym environment for web task automation in the Chromium browser
 Author: Rim Assouel, Léo Boisvert, Massimo Caccia, Alex Drouin, Maxime Gasse, Alex Lacoste, Tom Marty
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: browsergym-core ==0.2.4
-Requires-Dist: browsergym-miniwob ==0.2.4
-Requires-Dist: browsergym-webarena ==0.2.4
-Requires-Dist: browsergym-experiments ==0.2.4
+Requires-Dist: browsergym-core ==0.2.5
+Requires-Dist: browsergym-miniwob ==0.2.5
+Requires-Dist: browsergym-webarena ==0.2.5
+Requires-Dist: browsergym-experiments ==0.2.5
 Requires-Dist: browsergym-workarena
 
 # BrowserGym: a Gym Environment for Web Task Automation
 
 [[Setup]](#setup) ♦ [[Usage]](#usage) ♦ [[Demo]](#demo)
 
 This package provides `browsergym`, a gym environment for web task automation in the Chromium browser.
```

