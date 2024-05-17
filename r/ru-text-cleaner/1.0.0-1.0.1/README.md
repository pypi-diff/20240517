# Comparing `tmp/ru_text_cleaner-1.0.0.tar.gz` & `tmp/ru_text_cleaner-1.0.1.tar.gz`

## Comparing `ru_text_cleaner-1.0.0.tar` & `ru_text_cleaner-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.0/requirements.txt
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.0/.idea/.gitignore
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.0/.idea/TextCleaner.iml
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.0/.idea/misc.xml
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.0/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.0/.idea/vcs.xml
--rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.0/.idea/workspace.xml
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.0/src/ru_text_cleaner/TextCleaner.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.0/src/ru_text_cleaner/__init__.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.0/src/ru_text_cleaner/_clean_stopwords.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.0/src/ru_text_cleaner/_emoji_cleaner.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.0/src/ru_text_cleaner/_html_cleaner.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.0/src/ru_text_cleaner/_punctuation_cleaner.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.0/src/ru_text_cleaner/_spaces_cleaner.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.0/src/ru_text_cleaner/_to_lower.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.0/src/ru_text_cleaner/_to_morpheme.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.0/LICENSE
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.0/README.md
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.1/requirements.txt
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.1/.idea/.gitignore
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.1/.idea/TextCleaner.iml
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.1/.idea/misc.xml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.1/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.1/.idea/workspace.xml
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.1/src/ru_text_cleaner/TextCleaner.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.1/src/ru_text_cleaner/__init__.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.1/src/ru_text_cleaner/_clean_stopwords.py
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.1/src/ru_text_cleaner/_emoji_cleaner.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.1/src/ru_text_cleaner/_html_cleaner.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.1/src/ru_text_cleaner/_punctuation_cleaner.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.1/src/ru_text_cleaner/_spaces_cleaner.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.1/src/ru_text_cleaner/_to_lower.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.1/src/ru_text_cleaner/_to_morpheme.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.1/README.md
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 ru_text_cleaner-1.0.1/PKG-INFO
```

### Comparing `ru_text_cleaner-1.0.0/.idea/inspectionProfiles/Project_Default.xml` & `ru_text_cleaner-1.0.1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-1.0.0/src/ru_text_cleaner/TextCleaner.py` & `ru_text_cleaner-1.0.1/src/ru_text_cleaner/TextCleaner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-from . import *
+import _clean_stopwords
+import _emoji_cleaner
+import _html_cleaner
+import _punctuation_cleaner
+import _spaces_cleaner
+import _to_lower
+import _to_morpheme
 
 
 class TextCleaner:
     def __init__(self, spaces=True, punctuation=True, html=True, emoji=True, lower=True,
                  stop_words=True, morpheme=True):
 
         """
@@ -22,21 +28,21 @@
         self.punctuation = punctuation
         self.html = html
         self.emoji = emoji
         self.lower = lower
         self.stopwords = stop_words
         self.morpheme = morpheme
 
-        self.to_lower = to_lower_text
-        self.clean_emoji = clean_emoji
-        self.clean_punctuation = clean_punctuation
-        self.clean_html = clean_html
-        self.clean_space = clean_spaces
-        self.clean_stopwords = clean_stopwords
-        self.to_morpheme = text_to_morphems
+        self.to_lower = _to_lower
+        self.clean_emoji = _emoji_cleaner
+        self.clean_punctuation = _punctuation_cleaner
+        self.clean_html = _html_cleaner
+        self.clean_space = _spaces_cleaner
+        self.clean_stopwords = _clean_stopwords
+        self.to_morpheme = _to_morpheme
 
     def clean_text(self, text: str) -> str:
 
         """ Метод clean_text форматирует текст в зависимости от поставленных флагов"""
 
         if self.lower:
             text = self.to_lower(self, text)
```

### Comparing `ru_text_cleaner-1.0.0/src/ru_text_cleaner/_clean_stopwords.py` & `ru_text_cleaner-1.0.1/src/ru_text_cleaner/_clean_stopwords.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from . import *
+import nltk
+
+nltk.download('stopwords')
 
 
 def clean_stopwords(self, text: str) -> str:
 
     """
     Метод clean_stopwords убирает все стоп слова
```

### Comparing `ru_text_cleaner-1.0.0/src/ru_text_cleaner/_emoji_cleaner.py` & `ru_text_cleaner-1.0.1/src/ru_text_cleaner/_emoji_cleaner.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from . import *
+import re
 
 
 def clean_emoji(self, text: str) -> str:
 
     """
         Функция clean_emoji удаляет все emoji из текста
```

### Comparing `ru_text_cleaner-1.0.0/src/ru_text_cleaner/_spaces_cleaner.py` & `ru_text_cleaner-1.0.1/src/ru_text_cleaner/_spaces_cleaner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from . import *
-
+import re
 
 def clean_spaces(self, text: str) -> str:
 
     """
     Метод clean_spaces убирает лишние пробелы из текста
 
         re.sub(r' +', ' ', text) - Ищет в переданном тексте лишние пробелы, заменяет их на один пробел
```

### Comparing `ru_text_cleaner-1.0.0/src/ru_text_cleaner/_to_morpheme.py` & `ru_text_cleaner-1.0.1/src/ru_text_cleaner/_to_morpheme.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from . import *
+import pymorphy2
 
 
 def text_to_morphems(self, text: str) -> str:
 
     """
     Метод text_to_morphems заменяет слова на морфемы
```

### Comparing `ru_text_cleaner-1.0.0/LICENSE` & `ru_text_cleaner-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-1.0.0/README.md` & `ru_text_cleaner-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-1.0.0/pyproject.toml` & `ru_text_cleaner-1.0.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['pymorphy2>=0.9.1', 'nltk>=3.8.1', 'hatchling']
 build-backend = "hatchling.build"
 
 [project]
 name = "ru-text-cleaner"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     { name="Artem Gafarov", email="a.m.gafarov@ya.ru" },
     { name="Vildan Nasyrov", email="" },
 ]
 description = "Prepare russian text for NLTK"
 requires-python = ">=3.10.4"
 readme = "README.md"
```

### Comparing `ru_text_cleaner-1.0.0/PKG-INFO` & `ru_text_cleaner-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ru-text-cleaner
-Version: 1.0.0
+Version: 1.0.1
 Summary: Prepare russian text for NLTK
 Project-URL: Homepage, https://github.com/rvneural/TextCleaner
 Project-URL: Issues, https://github.com/rvneural/TextCleaner/issues
 Author: Vildan Nasyrov
 Author-email: Artem Gafarov <a.m.gafarov@ya.ru>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

