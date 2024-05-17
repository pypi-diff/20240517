# Comparing `tmp/ru_text_cleaner-1.1.3.tar.gz` & `tmp/ru_text_cleaner-1.1.4.tar.gz`

## Comparing `ru_text_cleaner-1.1.3.tar` & `ru_text_cleaner-1.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/requirements.txt
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/.idea/.gitignore
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/.idea/TextCleaner.iml
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/.idea/misc.xml
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/.idea/vcs.xml
--rw-r--r--   0        0        0     8990 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/.idea/workspace.xml
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/src/ru_text_cleaner/TextCleaner.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/src/ru_text_cleaner/__init__.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/src/ru_text_cleaner/_clean_stopwords.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/src/ru_text_cleaner/_emoji_cleaner.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/src/ru_text_cleaner/_html_cleaner.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/src/ru_text_cleaner/_punctuation_cleaner.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/src/ru_text_cleaner/_spaces_cleaner.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/src/ru_text_cleaner/_to_lower.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/src/ru_text_cleaner/_to_morpheme.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/LICENSE
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/README.md
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.4/requirements.txt
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.4/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.4/.idea/.gitignore
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.4/.idea/TextCleaner.iml
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.4/.idea/misc.xml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.4/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.4/.idea/vcs.xml
+-rw-r--r--   0        0        0     8990 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.4/.idea/workspace.xml
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.4/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.4/src/ru_text_cleaner/TextCleaner.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.4/src/ru_text_cleaner/__init__.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.4/src/ru_text_cleaner/_clean_stopwords.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.4/src/ru_text_cleaner/_emoji_cleaner.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.4/src/ru_text_cleaner/_html_cleaner.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.4/src/ru_text_cleaner/_punctuation_cleaner.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.4/src/ru_text_cleaner/_spaces_cleaner.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.4/src/ru_text_cleaner/_to_lower.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.4/src/ru_text_cleaner/_to_morpheme.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.4/LICENSE
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.4/README.md
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.4/PKG-INFO
```

### Comparing `ru_text_cleaner-1.1.3/.idea/workspace.xml` & `ru_text_cleaner-1.1.4/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-1.1.3/.idea/inspectionProfiles/Project_Default.xml` & `ru_text_cleaner-1.1.4/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-1.1.3/src/ru_text_cleaner/TextCleaner.py` & `ru_text_cleaner-1.1.4/src/ru_text_cleaner/TextCleaner.py`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-1.1.3/src/ru_text_cleaner/_clean_stopwords.py` & `ru_text_cleaner-1.1.4/src/ru_text_cleaner/_clean_stopwords.py`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-1.1.3/src/ru_text_cleaner/_spaces_cleaner.py` & `ru_text_cleaner-1.1.4/src/ru_text_cleaner/_spaces_cleaner.py`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-1.1.3/src/ru_text_cleaner/_to_morpheme.py` & `ru_text_cleaner-1.1.4/src/ru_text_cleaner/_to_morpheme.py`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-1.1.3/LICENSE` & `ru_text_cleaner-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-1.1.3/README.md` & `ru_text_cleaner-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-1.1.3/pyproject.toml` & `ru_text_cleaner-1.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ['pymorphy2>=0.9.1', 'nltk>=3.8.1', 'hatchling', 'emoji>=2.11.1']
 build-backend = "hatchling.build"
 
 [project]
 name = "ru-text-cleaner"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
     { name="Vildan Nasyrov", email="" },
     { name="Artem Gafarov", email="a.m.gafarov@ya.ru" },
 ]
-description = "Prepare russian text for NLP"
+description = "Cleans russian text and preparing for NLP"
 requires-python = ">=3.10.4"
 readme = "README.md"
 classifiers = [
    "Programming Language :: Python :: 3",
    "License :: OSI Approved :: MIT License",
    "Operating System :: OS Independent",
 ]
```

### Comparing `ru_text_cleaner-1.1.3/PKG-INFO` & `ru_text_cleaner-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.3
 Name: ru-text-cleaner
-Version: 1.1.3
-Summary: Prepare russian text for NLP
+Version: 1.1.4
+Summary: Cleans russian text and preparing for NLP
 Project-URL: Homepage, https://github.com/rvneural/TextCleaner
 Project-URL: Issues, https://github.com/rvneural/TextCleaner/issues
 Author: Vildan Nasyrov
 Author-email: Artem Gafarov <a.m.gafarov@ya.ru>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

