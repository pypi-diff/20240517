# Comparing `tmp/pyfancytranslator-1.0.4.tar.gz` & `tmp/pyfancytranslator-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfancytranslator-1.0.4.tar", last modified: Thu May 16 16:14:44 2024, max compression
+gzip compressed data, was "pyfancytranslator-1.0.5.tar", last modified: Fri May 17 14:21:57 2024, max compression
```

## Comparing `pyfancytranslator-1.0.4.tar` & `pyfancytranslator-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 16:14:44.657018 pyfancytranslator-1.0.4/
-drwxrwxrwx   0        0        0        0 2024-05-16 16:14:44.633162 pyfancytranslator-1.0.4/FancyTranslator/
--rw-rw-rw-   0        0        0      175 2024-05-04 12:18:43.000000 pyfancytranslator-1.0.4/FancyTranslator/__init__.py
--rw-rw-rw-   0        0        0     6400 2024-05-16 16:14:14.000000 pyfancytranslator-1.0.4/FancyTranslator/classes.py
--rw-rw-rw-   0        0        0     2596 2024-05-16 16:14:44.657018 pyfancytranslator-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2001 2024-05-03 13:55:21.000000 pyfancytranslator-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 16:14:44.655511 pyfancytranslator-1.0.4/pyfancytranslator.egg-info/
--rw-rw-rw-   0        0        0     2596 2024-05-16 16:14:44.000000 pyfancytranslator-1.0.4/pyfancytranslator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2024-05-16 16:14:44.000000 pyfancytranslator-1.0.4/pyfancytranslator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 16:14:44.000000 pyfancytranslator-1.0.4/pyfancytranslator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-16 16:14:44.000000 pyfancytranslator-1.0.4/pyfancytranslator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      716 2024-05-16 16:14:14.000000 pyfancytranslator-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 16:14:44.657018 pyfancytranslator-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-05-03 13:27:10.000000 pyfancytranslator-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 14:21:57.056972 pyfancytranslator-1.0.5/
+drwxrwxrwx   0        0        0        0 2024-05-17 14:21:57.004223 pyfancytranslator-1.0.5/FancyTranslator/
+-rw-rw-rw-   0        0        0      175 2024-05-04 12:18:43.000000 pyfancytranslator-1.0.5/FancyTranslator/__init__.py
+-rw-rw-rw-   0        0        0     6405 2024-05-17 14:21:43.000000 pyfancytranslator-1.0.5/FancyTranslator/classes.py
+-rw-rw-rw-   0        0        0     2596 2024-05-17 14:21:57.055900 pyfancytranslator-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2001 2024-05-03 13:55:21.000000 pyfancytranslator-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 14:21:57.053432 pyfancytranslator-1.0.5/pyfancytranslator.egg-info/
+-rw-rw-rw-   0        0        0     2596 2024-05-17 14:21:56.000000 pyfancytranslator-1.0.5/pyfancytranslator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2024-05-17 14:21:56.000000 pyfancytranslator-1.0.5/pyfancytranslator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 14:21:56.000000 pyfancytranslator-1.0.5/pyfancytranslator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-17 14:21:56.000000 pyfancytranslator-1.0.5/pyfancytranslator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      716 2024-05-17 14:21:43.000000 pyfancytranslator-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 14:21:57.056972 pyfancytranslator-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-05-03 13:27:10.000000 pyfancytranslator-1.0.5/setup.py
```

### Comparing `pyfancytranslator-1.0.4/FancyTranslator/classes.py` & `pyfancytranslator-1.0.5/FancyTranslator/classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,16 +100,16 @@
         # returns "This is an example with a nested placeholder: Nested"
         ```
         """
         text = self.read(section, key, default)
         if not isinstance(text, str):
             return text
 
-        for placeholder in re.findall('%\\w+(\\.\\w+)*%', text):
-            path = placeholder.split('.')
+        for placeholder in re.findall('%(\\w+(\\.\\w+)*)%', text):
+            path = placeholder[0].split('.')
             obj: None | object = kwargs.get(path.pop(0), None)
             while obj is not None and len(path) > 0:
                 if isinstance(obj, dict):
                     obj = obj.get(path.pop(0), None)
                 else:
                     obj = getattr(obj, path.pop(0), None)
```

### Comparing `pyfancytranslator-1.0.4/PKG-INFO` & `pyfancytranslator-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfancytranslator
-Version: 1.0.4
+Version: 1.0.5
 Summary: A well built translator with placeholders
 Author-email: Ashenguard <ashenguard@agmstudio.xyz>
 Project-URL: Homepage, https://github.com/agm-studio/fancytranslator
 Project-URL: Bug Tracker, https://github.com/agm-studio/fancytranslator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyfancytranslator-1.0.4/README.md` & `pyfancytranslator-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyfancytranslator-1.0.4/pyfancytranslator.egg-info/PKG-INFO` & `pyfancytranslator-1.0.5/pyfancytranslator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfancytranslator
-Version: 1.0.4
+Version: 1.0.5
 Summary: A well built translator with placeholders
 Author-email: Ashenguard <ashenguard@agmstudio.xyz>
 Project-URL: Homepage, https://github.com/agm-studio/fancytranslator
 Project-URL: Bug Tracker, https://github.com/agm-studio/fancytranslator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyfancytranslator-1.0.4/pyproject.toml` & `pyfancytranslator-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyfancytranslator"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
     { name = "Ashenguard", email = "ashenguard@agmstudio.xyz" },
 ]
 description = "A well built translator with placeholders"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

