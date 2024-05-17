# Comparing `tmp/vectorizer-0.1.1.tar.gz` & `tmp/vectorizer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectorizer-0.1.1.tar", last modified: Fri May 17 14:50:00 2024, max compression
+gzip compressed data, was "vectorizer-0.2.0.tar", last modified: Fri May 17 15:01:37 2024, max compression
```

## Comparing `vectorizer-0.1.1.tar` & `vectorizer-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 14:50:00.421731 vectorizer-0.1.1/
--rw-rw-rw-   0        0        0      343 2024-05-17 14:50:00.409211 vectorizer-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-17 12:37:56.000000 vectorizer-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-17 14:50:00.421731 vectorizer-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      889 2024-05-17 14:49:46.000000 vectorizer-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 14:50:00.362337 vectorizer-0.1.1/vectorizer/
--rw-rw-rw-   0        0        0        0 2024-05-17 12:36:42.000000 vectorizer-0.1.1/vectorizer/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-17 14:40:22.000000 vectorizer-0.1.1/vectorizer/text.py
--rw-rw-rw-   0        0        0     2096 2024-05-17 14:49:11.000000 vectorizer-0.1.1/vectorizer/vectorizer.py
-drwxrwxrwx   0        0        0        0 2024-05-17 14:50:00.393589 vectorizer-0.1.1/vectorizer.egg-info/
--rw-rw-rw-   0        0        0      343 2024-05-17 14:49:59.000000 vectorizer-0.1.1/vectorizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2024-05-17 14:50:00.000000 vectorizer-0.1.1/vectorizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 14:49:59.000000 vectorizer-0.1.1/vectorizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-17 14:49:59.000000 vectorizer-0.1.1/vectorizer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 15:01:37.490523 vectorizer-0.2.0/
+-rw-rw-rw-   0        0        0      343 2024-05-17 15:01:37.490523 vectorizer-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-17 12:37:56.000000 vectorizer-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-17 15:01:37.490523 vectorizer-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      889 2024-05-17 15:01:21.000000 vectorizer-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:01:37.459273 vectorizer-0.2.0/vectorizer/
+-rw-rw-rw-   0        0        0        0 2024-05-17 12:36:42.000000 vectorizer-0.2.0/vectorizer/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-17 14:40:22.000000 vectorizer-0.2.0/vectorizer/text.py
+-rw-rw-rw-   0        0        0     2098 2024-05-17 14:56:18.000000 vectorizer-0.2.0/vectorizer/vectorizer.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:01:37.490523 vectorizer-0.2.0/vectorizer.egg-info/
+-rw-rw-rw-   0        0        0      343 2024-05-17 15:01:37.000000 vectorizer-0.2.0/vectorizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2024-05-17 15:01:37.000000 vectorizer-0.2.0/vectorizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 15:01:37.000000 vectorizer-0.2.0/vectorizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-17 15:01:37.000000 vectorizer-0.2.0/vectorizer.egg-info/top_level.txt
```

### Comparing `vectorizer-0.1.1/setup.py` & `vectorizer-0.2.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vectorizer",
-    version="0.1.1",
+    version="0.2.0",
     author="Simean Hamado",
     author_email="fatihamtech@gmail.com",
     description="This package aims to facilitate natural languange processing",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="http://example.com/mypackage",
     packages=find_packages(),
```

### Comparing `vectorizer-0.1.1/vectorizer/vectorizer.py` & `vectorizer-0.2.0/vectorizer/vectorizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         --------------------
         Input: text
         """
 
         if not isinstance(text, str):
             raise ValueError("Input must be a string")
         text = text.lower()
-        return "".join([char for char in text if char not in self.punctuation])
+        return " ".join([char for char in text if char not in self.punctuation])
 
     def tokenize(self, text):
         """Text Tokenizer.
         --------------------
         Input: text
         """
         text = self.standardize(text)
@@ -55,10 +55,10 @@
         return [self.vocabulary.get(token, 1) for token in tokens]
 
     def decode(self, input_sequence):
         """This method turn a  list of numeric into text .
         --------------------
         Input: list of numbers
         """
-        return "".join(
+        return " ".join(
             self.inverse_vocabulary.get(index, "[UNK]") for index in input_sequence
         )
```

