# Comparing `tmp/pyfancytranslator-1.0.3.tar.gz` & `tmp/pyfancytranslator-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfancytranslator-1.0.3.tar", last modified: Sat May  4 11:59:46 2024, max compression
+gzip compressed data, was "pyfancytranslator-1.0.4.tar", last modified: Thu May 16 16:14:44 2024, max compression
```

## Comparing `pyfancytranslator-1.0.3.tar` & `pyfancytranslator-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 11:59:46.216307 pyfancytranslator-1.0.3/
-drwxrwxrwx   0        0        0        0 2024-05-04 11:59:46.203167 pyfancytranslator-1.0.3/FancyTranslator/
--rw-rw-rw-   0        0        0      175 2024-05-04 11:59:22.000000 pyfancytranslator-1.0.3/FancyTranslator/__init__.py
--rw-rw-rw-   0        0        0     6363 2024-05-04 11:59:22.000000 pyfancytranslator-1.0.3/FancyTranslator/classes.py
--rw-rw-rw-   0        0        0     2596 2024-05-04 11:59:46.215345 pyfancytranslator-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2001 2024-05-03 13:55:21.000000 pyfancytranslator-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 11:59:46.214312 pyfancytranslator-1.0.3/pyfancytranslator.egg-info/
--rw-rw-rw-   0        0        0     2596 2024-05-04 11:59:46.000000 pyfancytranslator-1.0.3/pyfancytranslator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2024-05-04 11:59:46.000000 pyfancytranslator-1.0.3/pyfancytranslator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 11:59:46.000000 pyfancytranslator-1.0.3/pyfancytranslator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-04 11:59:46.000000 pyfancytranslator-1.0.3/pyfancytranslator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      716 2024-05-04 11:59:22.000000 pyfancytranslator-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-04 11:59:46.216307 pyfancytranslator-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-05-03 13:27:10.000000 pyfancytranslator-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 16:14:44.657018 pyfancytranslator-1.0.4/
+drwxrwxrwx   0        0        0        0 2024-05-16 16:14:44.633162 pyfancytranslator-1.0.4/FancyTranslator/
+-rw-rw-rw-   0        0        0      175 2024-05-04 12:18:43.000000 pyfancytranslator-1.0.4/FancyTranslator/__init__.py
+-rw-rw-rw-   0        0        0     6400 2024-05-16 16:14:14.000000 pyfancytranslator-1.0.4/FancyTranslator/classes.py
+-rw-rw-rw-   0        0        0     2596 2024-05-16 16:14:44.657018 pyfancytranslator-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2001 2024-05-03 13:55:21.000000 pyfancytranslator-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 16:14:44.655511 pyfancytranslator-1.0.4/pyfancytranslator.egg-info/
+-rw-rw-rw-   0        0        0     2596 2024-05-16 16:14:44.000000 pyfancytranslator-1.0.4/pyfancytranslator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2024-05-16 16:14:44.000000 pyfancytranslator-1.0.4/pyfancytranslator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 16:14:44.000000 pyfancytranslator-1.0.4/pyfancytranslator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-16 16:14:44.000000 pyfancytranslator-1.0.4/pyfancytranslator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      716 2024-05-16 16:14:14.000000 pyfancytranslator-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 16:14:44.657018 pyfancytranslator-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-05-03 13:27:10.000000 pyfancytranslator-1.0.4/setup.py
```

### Comparing `pyfancytranslator-1.0.3/FancyTranslator/classes.py` & `pyfancytranslator-1.0.4/FancyTranslator/classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,19 +28,19 @@
     Parameters:
         :param parser (Parser): Parser instance, aka the data holder
         :param code (str): Language code, aka the language file name
         :param name (str): Language name, read from the langauge file, section "Translation", key "name"
         :param logger (logging.Logger): The child logger of translator logger for this language
     """
 
-    def __init__(self, translator: 'Translator', code: str):
+    def __init__(self, translator: 'Translator', code: str, encoding="utf-8"):
         self.code = code
 
         cf = ConfigParser()
-        cf.read(f"{translator.path}/{code}.ini")
+        cf.read(f"{translator.path}/{code}.ini", encoding=encoding)
 
         count = 0
         self.parser = Parser()
         for section in cf.sections():
             for option in cf.options(section):
                 self.parser.set(section, option, cf.get(section, option))
                 count += 1
```

### Comparing `pyfancytranslator-1.0.3/PKG-INFO` & `pyfancytranslator-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfancytranslator
-Version: 1.0.3
+Version: 1.0.4
 Summary: A well built translator with placeholders
 Author-email: Ashenguard <ashenguard@agmstudio.xyz>
 Project-URL: Homepage, https://github.com/agm-studio/fancytranslator
 Project-URL: Bug Tracker, https://github.com/agm-studio/fancytranslator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyfancytranslator-1.0.3/README.md` & `pyfancytranslator-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyfancytranslator-1.0.3/pyfancytranslator.egg-info/PKG-INFO` & `pyfancytranslator-1.0.4/pyfancytranslator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfancytranslator
-Version: 1.0.3
+Version: 1.0.4
 Summary: A well built translator with placeholders
 Author-email: Ashenguard <ashenguard@agmstudio.xyz>
 Project-URL: Homepage, https://github.com/agm-studio/fancytranslator
 Project-URL: Bug Tracker, https://github.com/agm-studio/fancytranslator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyfancytranslator-1.0.3/pyproject.toml` & `pyfancytranslator-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyfancytranslator"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
     { name = "Ashenguard", email = "ashenguard@agmstudio.xyz" },
 ]
 description = "A well built translator with placeholders"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

