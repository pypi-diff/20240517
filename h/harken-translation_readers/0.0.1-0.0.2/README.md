# Comparing `tmp/harken_translation_readers-0.0.1.tar.gz` & `tmp/harken_translation_readers-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harken_translation_readers-0.0.1.tar", max compression
+gzip compressed data, was "harken_translation_readers-0.0.2.tar", max compression
```

## Comparing `harken_translation_readers-0.0.1.tar` & `harken_translation_readers-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       30 2024-05-17 14:47:35.700507 harken_translation_readers-0.0.1/README.md
--rw-r--r--   0        0        0      914 2024-05-17 14:58:34.420997 harken_translation_readers-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        1 2024-05-17 14:47:35.700507 harken_translation_readers-0.0.1/translation_readers/__init__.py
--rw-r--r--   0        0        0      557 2024-05-17 14:57:19.937813 harken_translation_readers-0.0.1/translation_readers/reader.py
--rw-r--r--   0        0        0     1813 2024-05-17 14:57:19.929813 harken_translation_readers-0.0.1/translation_readers/tmx_reader.py
--rw-r--r--   0        0        0      915 1970-01-01 00:00:00.000000 harken_translation_readers-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       30 2024-05-17 14:47:35.700507 harken_translation_readers-0.0.2/README.md
+-rw-r--r--   0        0        0      914 2024-05-17 15:14:28.083353 harken_translation_readers-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      201 2024-05-17 15:14:08.355299 harken_translation_readers-0.0.2/translation_readers/__init__.py
+-rw-r--r--   0        0        0      580 2024-05-17 15:14:21.199335 harken_translation_readers-0.0.2/translation_readers/reader.py
+-rw-r--r--   0        0        0     1813 2024-05-17 14:57:19.929813 harken_translation_readers-0.0.2/translation_readers/tmx_reader.py
+-rw-r--r--   0        0        0      915 1970-01-01 00:00:00.000000 harken_translation_readers-0.0.2/PKG-INFO
```

### Comparing `harken_translation_readers-0.0.1/pyproject.toml` & `harken_translation_readers-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "harken-translation_readers"
-version = "0.0.1"
+version = "0.0.2"
 description = "..."
 authors = ["Juan Luis García <juanluis1702@gmail.com>"]
 readme = "README.md"
 packages = [{include = "translation_readers"}]
 
 [tool.poetry.dependencies]
 python = ">=3"
```

### Comparing `harken_translation_readers-0.0.1/translation_readers/reader.py` & `harken_translation_readers-0.0.2/translation_readers/reader.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,8 +14,10 @@
         if is_a_valid_language(src_lang):
             self.src_lang = get_language_code(src_lang,iso=ISO_639_2)
         if is_a_valid_language(tgt_lang):
             self.tgt_lang = get_language_code(tgt_lang,iso=ISO_639_2)
 
     @abstractmethod
     def get_data(self):
-        pass
+        pass
+
+__all__ = ["Reader"]
```

### Comparing `harken_translation_readers-0.0.1/translation_readers/tmx_reader.py` & `harken_translation_readers-0.0.2/translation_readers/tmx_reader.py`

 * *Files identical despite different names*

### Comparing `harken_translation_readers-0.0.1/PKG-INFO` & `harken_translation_readers-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harken-translation_readers
-Version: 0.0.1
+Version: 0.0.2
 Summary: ...
 Author: Juan Luis García
 Author-email: juanluis1702@gmail.com
 Requires-Python: >=3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

