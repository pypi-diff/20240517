# Comparing `tmp/harken_languages-0.1.2.tar.gz` & `tmp/harken_languages-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harken_languages-0.1.2.tar", max compression
+gzip compressed data, was "harken_languages-0.1.4.tar", max compression
```

## Comparing `harken_languages-0.1.2.tar` & `harken_languages-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       20 2024-02-07 20:02:24.819216 harken_languages-0.1.2/README.md
--rw-r--r--   0        0        0      159 2024-02-11 14:19:13.884600 harken_languages-0.1.2/languages/__init__.py
--rw-r--r--   0        0        0     4704 2023-01-30 19:46:42.900663 harken_languages-0.1.2/languages/data/deepl_languages.json
--rw-r--r--   0        0        0    15319 2023-11-28 20:41:03.930225 harken_languages-0.1.2/languages/data/general_languages.json
--rw-r--r--   0        0        0     9284 2023-11-13 19:30:04.019325 harken_languages-0.1.2/languages/data/google_languages.json
--rw-r--r--   0        0        0     4098 2024-04-22 20:26:06.570089 harken_languages-0.1.2/languages/data/nllb200_languages.json
--rw-r--r--   0        0        0     3536 2024-04-22 20:26:22.329940 harken_languages-0.1.2/languages/languages.py
--rw-r--r--   0        0        0      940 2024-04-22 20:36:31.353490 harken_languages-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      976 1970-01-01 00:00:00.000000 harken_languages-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       20 2024-02-07 20:02:24.819216 harken_languages-0.1.4/README.md
+-rw-r--r--   0        0        0      159 2024-02-11 14:19:13.884600 harken_languages-0.1.4/languages/__init__.py
+-rw-r--r--   0        0        0     4704 2023-01-30 19:46:42.900663 harken_languages-0.1.4/languages/data/deepl_languages.json
+-rw-r--r--   0        0        0    15319 2023-11-28 20:41:03.930225 harken_languages-0.1.4/languages/data/general_languages.json
+-rw-r--r--   0        0        0     9284 2023-11-13 19:30:04.019325 harken_languages-0.1.4/languages/data/google_languages.json
+-rw-r--r--   0        0        0     4098 2024-04-22 20:26:06.570089 harken_languages-0.1.4/languages/data/nllb200_languages.json
+-rw-r--r--   0        0        0     3537 2024-05-17 20:24:29.802650 harken_languages-0.1.4/languages/languages.py
+-rw-r--r--   0        0        0      993 2024-05-17 20:24:35.310594 harken_languages-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1068 1970-01-01 00:00:00.000000 harken_languages-0.1.4/PKG-INFO
```

### Comparing `harken_languages-0.1.2/languages/data/deepl_languages.json` & `harken_languages-0.1.4/languages/data/deepl_languages.json`

 * *Files identical despite different names*

### Comparing `harken_languages-0.1.2/languages/data/general_languages.json` & `harken_languages-0.1.4/languages/data/general_languages.json`

 * *Files identical despite different names*

### Comparing `harken_languages-0.1.2/languages/data/google_languages.json` & `harken_languages-0.1.4/languages/data/google_languages.json`

 * *Files identical despite different names*

### Comparing `harken_languages-0.1.2/languages/data/nllb200_languages.json` & `harken_languages-0.1.4/languages/data/nllb200_languages.json`

 * *Files identical despite different names*

### Comparing `harken_languages-0.1.2/languages/languages.py` & `harken_languages-0.1.4/languages/languages.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         return results[0]
     except:
         return {'name': 'Unknown', 'code': 'unk', 'display': 'Unknown', 'code3': 'unk', 'score': 0}
 
 
 def detect_language_code(text, iso=ISO_639_1, detector="polyglot"):
     language = detect_language(text, detector=detector)
-    return get_language_code(language=language['lang'], iso=iso)
+    return get_language_code(language=language['code3'], iso=iso)
 
 
 def get_language_info(language):
     try:
         obj = Lang(language)
         return {'name': obj.name, 'code': obj.pt1, 'display': obj.name, 'code3': obj.pt3}
     except:
```

### Comparing `harken_languages-0.1.2/pyproject.toml` & `harken_languages-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 [tool.poetry]
 name = "harken-languages"
-version = "0.1.2"
+version = "0.1.4"
 description = "..."
 authors = ["Juan Luis García <juanluis1702@gmail.com>"]
 readme = "README.md"
 packages = [{include = "languages"}]
 
 [tool.poetry.dependencies]
 python = ">=3"
 poetry = "1.7.1"
 funcy = "2.0.0"
+wheel = ">=0.23.0"
 # External dependencies
 structlog = "23.1.0"
 langcodes = "3.3.0"
 polyglot = "16.7.4"
 lingua-language-detector = "2.0.2"
 iso639-lang = "2.2.2"
+PyICU = ">=2.12"
+pycld2 = ">=0.3"
 # Internal dependencies
 
 [tool]
 [tool.black]
 line-length = 100
 target-version = ["py310"]
```

### Comparing `harken_languages-0.1.2/PKG-INFO` & `harken_languages-0.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: harken-languages
-Version: 0.1.2
+Version: 0.1.4
 Summary: ...
 Author: Juan Luis García
 Author-email: juanluis1702@gmail.com
 Requires-Python: >=3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: PyICU (>=2.12)
 Requires-Dist: funcy (==2.0.0)
 Requires-Dist: iso639-lang (==2.2.2)
 Requires-Dist: langcodes (==3.3.0)
 Requires-Dist: lingua-language-detector (==2.0.2)
 Requires-Dist: poetry (==1.7.1)
 Requires-Dist: polyglot (==16.7.4)
+Requires-Dist: pycld2 (>=0.3)
 Requires-Dist: structlog (==23.1.0)
+Requires-Dist: wheel (>=0.23.0)
 Description-Content-Type: text/markdown
 
 # Harken - languages
```

