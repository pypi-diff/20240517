# Comparing `tmp/string_comparison-1.0.2.tar.gz` & `tmp/string_comparison-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "string_comparison-1.0.2.tar", last modified: Wed Apr 14 01:15:18 2021, max compression
+gzip compressed data, was "string_comparison-1.1.0.tar", last modified: Fri May 17 16:43:51 2024, max compression
```

## Comparing `string_comparison-1.0.2.tar` & `string_comparison-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0 brad.belyeu   (501) staff       (20)        0 2021-04-14 01:15:18.770701 string_comparison-1.0.2/
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)     1134 2021-04-14 01:15:18.770352 string_comparison-1.0.2/PKG-INFO
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)      318 2021-04-13 17:37:28.000000 string_comparison-1.0.2/README.md
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)       38 2021-04-14 01:15:18.770847 string_comparison-1.0.2/setup.cfg
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)     1045 2021-04-14 01:15:00.000000 string_comparison-1.0.2/setup.py
-drwxrwxrwx   0 brad.belyeu   (501) staff       (20)        0 2021-04-14 01:15:18.769719 string_comparison-1.0.2/string_comparison.egg-info/
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)     1134 2021-04-14 01:15:18.000000 string_comparison-1.0.2/string_comparison.egg-info/PKG-INFO
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)      203 2021-04-14 01:15:18.000000 string_comparison-1.0.2/string_comparison.egg-info/SOURCES.txt
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)        1 2021-04-14 01:15:18.000000 string_comparison-1.0.2/string_comparison.egg-info/dependency_links.txt
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)       18 2021-04-14 01:15:18.000000 string_comparison-1.0.2/string_comparison.egg-info/top_level.txt
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)    19855 2021-04-14 01:14:50.000000 string_comparison-1.0.2/string_comparison.py
+drwxrwxrwx   0 brad.belyeu   (501) staff       (20)        0 2024-05-17 16:43:51.948314 string_comparison-1.1.0/
+-rw-rw-rw-   0 brad.belyeu   (501) staff       (20)     1522 2024-05-17 16:43:51.948163 string_comparison-1.1.0/PKG-INFO
+-rw-rw-rw-   0 brad.belyeu   (501) staff       (20)      658 2024-05-16 20:14:51.000000 string_comparison-1.1.0/README.md
+-rw-rw-rw-   0 brad.belyeu   (501) staff       (20)       38 2024-05-17 16:43:51.948373 string_comparison-1.1.0/setup.cfg
+-rw-rw-rw-   0 brad.belyeu   (501) staff       (20)     1045 2024-05-16 20:14:51.000000 string_comparison-1.1.0/setup.py
+drwxrwxrwx   0 brad.belyeu   (501) staff       (20)        0 2024-05-17 16:43:51.947726 string_comparison-1.1.0/string_comparison.egg-info/
+-rw-rw-rw-   0 brad.belyeu   (501) staff       (20)     1522 2024-05-17 16:43:51.000000 string_comparison-1.1.0/string_comparison.egg-info/PKG-INFO
+-rw-rw-rw-   0 brad.belyeu   (501) staff       (20)      203 2024-05-17 16:43:51.000000 string_comparison-1.1.0/string_comparison.egg-info/SOURCES.txt
+-rw-rw-rw-   0 brad.belyeu   (501) staff       (20)        1 2024-05-17 16:43:51.000000 string_comparison-1.1.0/string_comparison.egg-info/dependency_links.txt
+-rw-rw-rw-   0 brad.belyeu   (501) staff       (20)       18 2024-05-17 16:43:51.000000 string_comparison-1.1.0/string_comparison.egg-info/top_level.txt
+-rw-rw-rw-   0 brad.belyeu   (501) staff       (20)    20480 2024-05-16 20:24:03.000000 string_comparison-1.1.0/string_comparison.py
```

### Comparing `string_comparison-1.0.2/setup.py` & `string_comparison-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 
 from setuptools import setup
 
 if sys.version_info < (3, 7):
     sys.exit("Sorry, Python < 3.7 is not supported")
 
-__version__ = "1.0.2"
+__version__ = "1.1.0"
 
 setup(
     name="string_comparison",
     version=__version__,
     description=__doc__,
     author="Brad Belyeu",
     author_email="bradley.belyeu@life.church",
```

### Comparing `string_comparison-1.0.2/string_comparison.py` & `string_comparison-1.1.0/string_comparison.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """
 String comparison main module.
 
 This maps a Unicode code point key represented as an integer to a corresponding ASCII
 character mapping. In some cases such as Hebrew niqqud & cantillation, we remove the
 character altogether or replace certain punctuation with a space.
+
+In addition, some characters are removed prior to normalization. For example, Unicode control chars.
 """
 
+import unicodedata
+
 UNICODE = {
     0: "",
     171: '"',
     173: "-",
     178: "2",
     179: "3",
     185: "1",
@@ -1294,14 +1298,29 @@
     65370: "z",
     65371: "{",
     65373: "}",
     65374: "~",
 }
 
 
-def normalize(str_):
-    """Normalize a string through possible permutations for comparison."""
-    if not str_:
+def normalize(string):
+    """
+    Normalize a string through possible permutations for comparison.
+
+    View https://www.unicode.org/reports/tr44/#GC_Values_Table for General Category values.
+    """
+    if not string:
         return ""
 
-    translate_table = str_.maketrans(UNICODE)
-    return str_.translate(translate_table).strip().casefold()
+    for char in string:
+        # Remove Unicode control characters.
+        # "C" is returned as the first char for all control chars.
+        if unicodedata.category(char)[0] == "C":
+            string = string.replace(char, "")
+
+        # Normalize space separators into a single normal space
+        if unicodedata.category(char) == "Zs":
+            string = string.replace(char, " ")
+
+    translate_table = string.maketrans(UNICODE)
+
+    return string.translate(translate_table).strip().casefold()
```

