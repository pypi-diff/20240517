# Comparing `tmp/fuzzquery-2024.5.16.tar.gz` & `tmp/fuzzquery-2024.5.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuzzquery-2024.5.16.tar", last modified: Thu May 16 17:37:50 2024, max compression
+gzip compressed data, was "fuzzquery-2024.5.17.tar", last modified: Fri May 17 04:00:01 2024, max compression
```

## Comparing `fuzzquery-2024.5.16.tar` & `fuzzquery-2024.5.17.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 17:37:50.707788 fuzzquery-2024.5.16/
--rw-rw-rw-   0        0        0     1090 2024-05-16 01:40:27.000000 fuzzquery-2024.5.16/LICENSE
--rw-rw-rw-   0        0        0     6914 2024-05-16 17:37:50.707788 fuzzquery-2024.5.16/PKG-INFO
--rw-rw-rw-   0        0        0     6311 2024-05-16 17:33:58.000000 fuzzquery-2024.5.16/README.md
--rw-rw-rw-   0        0        0      692 2024-05-16 17:37:04.000000 fuzzquery-2024.5.16/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 17:37:50.707788 fuzzquery-2024.5.16/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-16 17:37:50.645286 fuzzquery-2024.5.16/src/
-drwxrwxrwx   0        0        0        0 2024-05-16 17:37:50.676537 fuzzquery-2024.5.16/src/fuzzquery/
--rw-rw-rw-   0        0        0       21 2024-05-16 01:30:07.000000 fuzzquery-2024.5.16/src/fuzzquery/__init__.py
--rw-rw-rw-   0        0        0     4319 2024-05-16 17:36:21.000000 fuzzquery-2024.5.16/src/fuzzquery/main.py
-drwxrwxrwx   0        0        0        0 2024-05-16 17:37:50.707788 fuzzquery-2024.5.16/src/fuzzquery.egg-info/
--rw-rw-rw-   0        0        0     6914 2024-05-16 17:37:50.000000 fuzzquery-2024.5.16/src/fuzzquery.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2024-05-16 17:37:50.000000 fuzzquery-2024.5.16/src/fuzzquery.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 17:37:50.000000 fuzzquery-2024.5.16/src/fuzzquery.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-16 17:37:50.000000 fuzzquery-2024.5.16/src/fuzzquery.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-16 17:37:50.000000 fuzzquery-2024.5.16/src/fuzzquery.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 04:00:01.934057 fuzzquery-2024.5.17/
+-rw-rw-rw-   0        0        0     1090 2024-05-16 01:40:27.000000 fuzzquery-2024.5.17/LICENSE
+-rw-rw-rw-   0        0        0     6587 2024-05-17 04:00:01.934057 fuzzquery-2024.5.17/PKG-INFO
+-rw-rw-rw-   0        0        0     6017 2024-05-17 03:50:32.000000 fuzzquery-2024.5.17/README.md
+-rw-rw-rw-   0        0        0      659 2024-05-17 03:41:20.000000 fuzzquery-2024.5.17/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 04:00:01.949684 fuzzquery-2024.5.17/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 04:00:01.855924 fuzzquery-2024.5.17/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 04:00:01.902801 fuzzquery-2024.5.17/src/fuzzquery/
+-rw-rw-rw-   0        0        0       22 2024-05-17 01:52:08.000000 fuzzquery-2024.5.17/src/fuzzquery/__init__.py
+-rw-rw-rw-   0        0        0     4385 2024-05-17 02:22:08.000000 fuzzquery-2024.5.17/src/fuzzquery/fuzzy.py
+drwxrwxrwx   0        0        0        0 2024-05-17 04:00:01.934057 fuzzquery-2024.5.17/src/fuzzquery.egg-info/
+-rw-rw-rw-   0        0        0     6587 2024-05-17 04:00:01.000000 fuzzquery-2024.5.17/src/fuzzquery.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-05-17 04:00:01.000000 fuzzquery-2024.5.17/src/fuzzquery.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 04:00:01.000000 fuzzquery-2024.5.17/src/fuzzquery.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-17 04:00:01.000000 fuzzquery-2024.5.17/src/fuzzquery.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-17 04:00:01.000000 fuzzquery-2024.5.17/src/fuzzquery.egg-info/top_level.txt
```

### Comparing `fuzzquery-2024.5.16/LICENSE` & `fuzzquery-2024.5.17/LICENSE`

 * *Files identical despite different names*

### Comparing `fuzzquery-2024.5.16/PKG-INFO` & `fuzzquery-2024.5.17/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,124 +1,126 @@
 Metadata-Version: 2.1
 Name: fuzzquery
-Version: 2024.5.16
-Summary: A lightwieght package for doing fuzzy matches with a simple query language
+Version: 2024.5.17
+Summary: A lightwieght package for fuzzy matching.
 Author-email: OneMadGypsy <onemadgypsy@gmail.com>
 Project-URL: Homepage, https://github.com/OneMadGypsy/fuzzquery
 Project-URL: Issues, https://github.com/OneMadGypsy/fuzzquery/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: regex>=2024.5.15
 
 # fuzzquery
-A lightwieght package for doing fuzzy matches with a simple query language. This works by creating regular expressions for you that utilize the fuzzy matching features of the `regex` package, based on your query tokens. 
+A lightweight package for fuzzy matching.
 
 
 ## Installation:
 To install `fuzzquery` and it's `regex` dependency, open a terminal and input the following command: 
 ### `pip install fuzzquery`
 
+
 ## Theory:
-The regex package has 3 fuzzy matching features:
+The `regex` package has 3 fuzzy matching features:
 
-| type       | dsecription                                       |
+| type       | description                                       |
 | ---------- | ------------------------------------------------- |
 | insert     | 0 or more characters appear **before** your term  |
 | substitute | 0 or more characters are substituted in your term |
 | delete     | 0 or more characters are removed from your term   |
 
-This system completely ignores the native insertion model and creates it's own with substitution and deletion. This is because insertion is wholly uncontrollable. It is the only feature that allows characters where there never were any. My system reformats queries with substitution/deletion characters wherever a token is present. This means if you put a token before your term, it is essentially a controllable insertion. The back-end system will view it as a substitution and/or deletion, but it is a sub/del before your term so, it is functionally an insertion. 
+This system completely ignores the native insertion model and creates it's own with substitution and deletion. This is because insertion is wholly uncontrollable. It is the only feature that allows characters where there never were any. My system reformats queries with substitution/deletion characters wherever a token is present. This means if you put a token before your term, it is functionally an insertion.
 
-Substitutions and deletions can only happen where sub/del characters are present. This is because the sub/del score limit is identical to the amount of sub/del characters. If a non-sub/del character was to be subbed or deleted, it would leave behind an original sub/del character (backtick), and the final sub/del score would be too high to match. Basically, you can reliably search for anything that does **not** have a backtick in it. Technically, you can even reliably search for things that do have a backtick in them, but you are playing with the possibility of hitting an edge case that may yield some incorrect results. However, the `skip` feature could be used to ignore the incorrect results.
 
 ## Documentation:
 
 **notes:**
 
 1) `Iter` is an alias of `list|tuple|set`. It only exists in this documentation as a means to illustrate types in a less complex way.
-2) `skip` (if used) should be an `Iter` of words and/or characters that trigger a skip when found in results to be yielded.
+2) `skip` (if used) should be an `Iter` of words and/or characters that cannot be `in` a result.
 
 --------
 
-#### `finditer`
+### finditer
 > yield all (`span`, `match`) of a single query.
 
 **finditer(`text`:str, `query`:str, `skip`:Iter|None=None, `ci`:bool=False) -> Iterator**
-| arg      | description                                                                   |
-| -------- | ----------------------------------------------------------------------------- |
-| `text`   | the text to search                                                            |
-| `query`  | the query to search for                                                       |
-| `skip`   | iterable of terms and/or characters that trigger a skip when found in results |
-| `ci`     | case-insensitive matching                                                     |
+| arg      | description                                                               |
+| -------- | ------------------------------------------------------------------------- |
+| `text`   | the text to search                                                        |
+| `query`  | the query to search for                                                   |
+| `skip`   | Iter of terms and/or characters that trigger a skip when found in results |
+| `ci`     | case-insensitive matching                                                 |
 
 --------
 
-#### `findany`
+### findany
 > `OR` queries together and yield all (`span`, `match`) of whatever matched.
 
 **findany(`text`:str, `queries`:Iter, `skip`:Iter|None=None, `ci`:bool=False) -> Iterator**
-| arg       | description                                                                   |
-| --------- | ----------------------------------------------------------------------------- |
-| `text`    | the text to search                                                            |
-| `queries` | iterable of queries to search for                                             |
-| `skip`    | iterable of terms and/or characters that trigger a skip when found in results |
-| `ci`      | case-insensitive matching                                                     |
+| arg       | description                                                               |
+| --------- | ------------------------------------------------------------------------- |
+| `text`    | the text to search                                                        |
+| `queries` | Iter of queries to search for                                             |
+| `skip`    | Iter of terms and/or characters that trigger a skip when found in results |
+| `ci`      | case-insensitive matching                                                 |
 
 --------
 
-#### `iterall`
+### iterall
 > yield all (`query`, `span`, `match`) of multiple queries.
 
 **iterall(`text`:str, `queries`:Iter, `skip`:Iter|None=None, `ci`:bool=False) -> Iterator**
-| arg       | description                                                                   |
-| --------- | ----------------------------------------------------------------------------- |
-| `text`    | the text to search                                                            |
-| `queries` | iterable of queries to search for                                             |
-| `skip`    | iterable of terms and/or characters that trigger a skip when found in results |
-| `ci`      | case-insensitive matching                                                     |
+| arg       | description                                                               |
+| --------- | ------------------------------------------------------------------------- |
+| `text`    | the text to search                                                        |
+| `queries` | Iter of queries to search for                                             |
+| `skip`    | Iter of terms and/or characters that trigger a skip when found in results |
+| `ci`      | case-insensitive matching                                                 |
 
 
 ## Queries:
 
 A token system is used to represent unknown/fuzzy data. The 3 types of tokens are:
 
 | token  | type    | description                           | example           | result-like                     |
 | ------ | ------- | ------------------------------------- | ----------------- | ------------------------------- |
 | `{x}`  | allowed | 0 to `x` non-whitespace characters    | `"home{5}"`       | `home, homestead, homeward`     |
 | `{!x}` | strict  | exactly `x` non-whitespace characters | `"{1}ward{!2}"`   | `warden, awarded`               |
 | `{?}`  | unknown | 0 or more unknown words               | `"thou {?} kill"` | `thou shalt not kill`           |
 
+
 ## Examples:
 
 ```python3
 import fuzzquery as fq
 
 data = """ 
 I headed homeward to meet with the Wardens. 
 When I arrived, I was greeted by a homely man that told me the homestead was awarded 5 million dollars.
 We intend to use some of the homage to create a homeless ward. 
 The first piece of furniture will be my late-friend Homer's wardrobe.
 """
-queries = ('hom{5} {?} wa{8}', 
+queries = ('hom{5} {?} wa{!1}{5}', 
            'home{5}', 
            '{1}ward{!2}{2}', 
            'home{4} ward{4}')
 
 for query, span, match in fq.iterall(data, queries, ci=True):
     if query: print(f'\n{query.upper()}')
     print(f'  {match}')
 ```
 
 #### output
+
 ```none
-HOM{5} {?} WA{8}
+HOM{5} {?} WA{!1}{5}
   homeward to meet with the Wardens
   homely man that told me the homestead was
   homage to create a homeless ward
   Homer's wardrobe
 
 HOME{5}
   homeward
@@ -129,11 +131,48 @@
 
 {1}WARD{!2}{2}
   Wardens
   awarded
   wardrobe
 
 HOME{4} WARD{4}
-  homeward
   homeless ward
   Homer's wardrobe
 ```
+
+--------
+
+```python3
+import fuzzquery as fq
+
+data = """ 
+I would classify music as one of my favorite hobbies. 
+I love classical music played by classy musicians for a classic musical. 
+Beethoven can not be out-classed, music-wise - a man of class, musically gifted.
+"""
+query = 'class{4} music{4}'
+
+print(f'\n{query.upper()} with skip')
+for span, match in fq.finditer(data, query, skip=('classify', ','), ci=True):
+    print(f'  {match}')
+    
+print(f'\n{query.upper()} no skip')
+for span, match in fq.finditer(data, query, ci=True):
+    print(f'  {match}')
+```
+
+#### output
+
+```none
+CLASS{4} MUSIC{4} with skip
+  classical music
+  classy musicians
+  classic musical
+
+CLASS{4} MUSIC{4} no skip
+  classify music
+  classical music
+  classy musicians
+  classic musical
+  classed, music
+  class, musically
+```
```

### Comparing `fuzzquery-2024.5.16/README.md` & `fuzzquery-2024.5.17/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,109 +1,111 @@
 # fuzzquery
-A lightwieght package for doing fuzzy matches with a simple query language. This works by creating regular expressions for you that utilize the fuzzy matching features of the `regex` package, based on your query tokens. 
+A lightweight package for fuzzy matching.
 
 
 ## Installation:
 To install `fuzzquery` and it's `regex` dependency, open a terminal and input the following command: 
 ### `pip install fuzzquery`
 
+
 ## Theory:
-The regex package has 3 fuzzy matching features:
+The `regex` package has 3 fuzzy matching features:
 
-| type       | dsecription                                       |
+| type       | description                                       |
 | ---------- | ------------------------------------------------- |
 | insert     | 0 or more characters appear **before** your term  |
 | substitute | 0 or more characters are substituted in your term |
 | delete     | 0 or more characters are removed from your term   |
 
-This system completely ignores the native insertion model and creates it's own with substitution and deletion. This is because insertion is wholly uncontrollable. It is the only feature that allows characters where there never were any. My system reformats queries with substitution/deletion characters wherever a token is present. This means if you put a token before your term, it is essentially a controllable insertion. The back-end system will view it as a substitution and/or deletion, but it is a sub/del before your term so, it is functionally an insertion. 
+This system completely ignores the native insertion model and creates it's own with substitution and deletion. This is because insertion is wholly uncontrollable. It is the only feature that allows characters where there never were any. My system reformats queries with substitution/deletion characters wherever a token is present. This means if you put a token before your term, it is functionally an insertion.
 
-Substitutions and deletions can only happen where sub/del characters are present. This is because the sub/del score limit is identical to the amount of sub/del characters. If a non-sub/del character was to be subbed or deleted, it would leave behind an original sub/del character (backtick), and the final sub/del score would be too high to match. Basically, you can reliably search for anything that does **not** have a backtick in it. Technically, you can even reliably search for things that do have a backtick in them, but you are playing with the possibility of hitting an edge case that may yield some incorrect results. However, the `skip` feature could be used to ignore the incorrect results.
 
 ## Documentation:
 
 **notes:**
 
 1) `Iter` is an alias of `list|tuple|set`. It only exists in this documentation as a means to illustrate types in a less complex way.
-2) `skip` (if used) should be an `Iter` of words and/or characters that trigger a skip when found in results to be yielded.
+2) `skip` (if used) should be an `Iter` of words and/or characters that cannot be `in` a result.
 
 --------
 
-#### `finditer`
+### finditer
 > yield all (`span`, `match`) of a single query.
 
 **finditer(`text`:str, `query`:str, `skip`:Iter|None=None, `ci`:bool=False) -> Iterator**
-| arg      | description                                                                   |
-| -------- | ----------------------------------------------------------------------------- |
-| `text`   | the text to search                                                            |
-| `query`  | the query to search for                                                       |
-| `skip`   | iterable of terms and/or characters that trigger a skip when found in results |
-| `ci`     | case-insensitive matching                                                     |
+| arg      | description                                                               |
+| -------- | ------------------------------------------------------------------------- |
+| `text`   | the text to search                                                        |
+| `query`  | the query to search for                                                   |
+| `skip`   | Iter of terms and/or characters that trigger a skip when found in results |
+| `ci`     | case-insensitive matching                                                 |
 
 --------
 
-#### `findany`
+### findany
 > `OR` queries together and yield all (`span`, `match`) of whatever matched.
 
 **findany(`text`:str, `queries`:Iter, `skip`:Iter|None=None, `ci`:bool=False) -> Iterator**
-| arg       | description                                                                   |
-| --------- | ----------------------------------------------------------------------------- |
-| `text`    | the text to search                                                            |
-| `queries` | iterable of queries to search for                                             |
-| `skip`    | iterable of terms and/or characters that trigger a skip when found in results |
-| `ci`      | case-insensitive matching                                                     |
+| arg       | description                                                               |
+| --------- | ------------------------------------------------------------------------- |
+| `text`    | the text to search                                                        |
+| `queries` | Iter of queries to search for                                             |
+| `skip`    | Iter of terms and/or characters that trigger a skip when found in results |
+| `ci`      | case-insensitive matching                                                 |
 
 --------
 
-#### `iterall`
+### iterall
 > yield all (`query`, `span`, `match`) of multiple queries.
 
 **iterall(`text`:str, `queries`:Iter, `skip`:Iter|None=None, `ci`:bool=False) -> Iterator**
-| arg       | description                                                                   |
-| --------- | ----------------------------------------------------------------------------- |
-| `text`    | the text to search                                                            |
-| `queries` | iterable of queries to search for                                             |
-| `skip`    | iterable of terms and/or characters that trigger a skip when found in results |
-| `ci`      | case-insensitive matching                                                     |
+| arg       | description                                                               |
+| --------- | ------------------------------------------------------------------------- |
+| `text`    | the text to search                                                        |
+| `queries` | Iter of queries to search for                                             |
+| `skip`    | Iter of terms and/or characters that trigger a skip when found in results |
+| `ci`      | case-insensitive matching                                                 |
 
 
 ## Queries:
 
 A token system is used to represent unknown/fuzzy data. The 3 types of tokens are:
 
 | token  | type    | description                           | example           | result-like                     |
 | ------ | ------- | ------------------------------------- | ----------------- | ------------------------------- |
 | `{x}`  | allowed | 0 to `x` non-whitespace characters    | `"home{5}"`       | `home, homestead, homeward`     |
 | `{!x}` | strict  | exactly `x` non-whitespace characters | `"{1}ward{!2}"`   | `warden, awarded`               |
 | `{?}`  | unknown | 0 or more unknown words               | `"thou {?} kill"` | `thou shalt not kill`           |
 
+
 ## Examples:
 
 ```python3
 import fuzzquery as fq
 
 data = """ 
 I headed homeward to meet with the Wardens. 
 When I arrived, I was greeted by a homely man that told me the homestead was awarded 5 million dollars.
 We intend to use some of the homage to create a homeless ward. 
 The first piece of furniture will be my late-friend Homer's wardrobe.
 """
-queries = ('hom{5} {?} wa{8}', 
+queries = ('hom{5} {?} wa{!1}{5}', 
            'home{5}', 
            '{1}ward{!2}{2}', 
            'home{4} ward{4}')
 
 for query, span, match in fq.iterall(data, queries, ci=True):
     if query: print(f'\n{query.upper()}')
     print(f'  {match}')
 ```
 
 #### output
+
 ```none
-HOM{5} {?} WA{8}
+HOM{5} {?} WA{!1}{5}
   homeward to meet with the Wardens
   homely man that told me the homestead was
   homage to create a homeless ward
   Homer's wardrobe
 
 HOME{5}
   homeward
@@ -114,11 +116,48 @@
 
 {1}WARD{!2}{2}
   Wardens
   awarded
   wardrobe
 
 HOME{4} WARD{4}
-  homeward
   homeless ward
   Homer's wardrobe
 ```
+
+--------
+
+```python3
+import fuzzquery as fq
+
+data = """ 
+I would classify music as one of my favorite hobbies. 
+I love classical music played by classy musicians for a classic musical. 
+Beethoven can not be out-classed, music-wise - a man of class, musically gifted.
+"""
+query = 'class{4} music{4}'
+
+print(f'\n{query.upper()} with skip')
+for span, match in fq.finditer(data, query, skip=('classify', ','), ci=True):
+    print(f'  {match}')
+    
+print(f'\n{query.upper()} no skip')
+for span, match in fq.finditer(data, query, ci=True):
+    print(f'  {match}')
+```
+
+#### output
+
+```none
+CLASS{4} MUSIC{4} with skip
+  classical music
+  classy musicians
+  classic musical
+
+CLASS{4} MUSIC{4} no skip
+  classify music
+  classical music
+  classy musicians
+  classic musical
+  classed, music
+  class, musically
+```
```

### Comparing `fuzzquery-2024.5.16/pyproject.toml` & `fuzzquery-2024.5.17/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fuzzquery"
-version = "2024.5.16"
+version = "2024.5.17"
 authors = [
   { name="OneMadGypsy", email="onemadgypsy@gmail.com" },
 ]
-description = "A lightwieght package for doing fuzzy matches with a simple query language"
+description = "A lightwieght package for fuzzy matching."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `fuzzquery-2024.5.16/src/fuzzquery/main.py` & `fuzzquery-2024.5.17/src/fuzzquery/fuzzy.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 __all__ = 'finditer', 'findany', 'iterall'
 
 REPL  = '`'                                  # character to represent substitution and deletion points
 TOKEN = regex.compile(r'\{(!{0,1}\d+|\?)\}') # for splitting on token guts
 FLAGS = regex.V1, regex.V1|regex.I           # case-sensitive, case-insensitive
 
 FORMAT = {# https://github.com/mrabarnett/mrab-regex?tab=readme-ov-file#approximate-fuzzy-matching-hg-issue-12-hg-issue-41-hg-issue-109
-    '.':r'{{{over}i+1d+1s<={limit}:\S}}',    # suggestive range
-    '!':r'{{{limit}<=s<={limit}:\S}}'   ,    # strict range
-    '?':r'(\w+\W+)*?'                   ,}   # 0 or more unknown words 
+    '.':r'{{{over}i+1d+1s<={limit}:\S}}',    # allowed range of mixed substitutions and deletions
+    '!':r'{{{limit}<=s<={limit}:\S}}'   ,    # strict amount of substitutions only
+    '?':r'([\w\W]+?(?=\s))*?'           ,}   # 0 or more unknown words 
     
 
 # convert query to expression
 def __expr(query:str, group:bool=True) -> str:
 
     # convert term segment to expression
     def subexpr(segment:str) -> str:
@@ -33,15 +33,15 @@
         return expr
     
     # map[list] of term segments
     segmap = map(TOKEN.split, query.split(' '))
     
     # generator of terms from processed term segments
     terms = (r''.join(map(subexpr, filter(None, segments))) for segments in segmap)
-    expr  = r'\s*'.join(terms)
+    expr  = r'((?<=\s)|\s)'.join(terms)
     grp   = (0,1)[group is True]
     
     # create final expression
     return f'{"("*grp}{expr}{")"*grp}'
    
 """ execute expression on text
     `expr` : final regex pattern
```

### Comparing `fuzzquery-2024.5.16/src/fuzzquery.egg-info/PKG-INFO` & `fuzzquery-2024.5.17/src/fuzzquery.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,124 +1,126 @@
 Metadata-Version: 2.1
 Name: fuzzquery
-Version: 2024.5.16
-Summary: A lightwieght package for doing fuzzy matches with a simple query language
+Version: 2024.5.17
+Summary: A lightwieght package for fuzzy matching.
 Author-email: OneMadGypsy <onemadgypsy@gmail.com>
 Project-URL: Homepage, https://github.com/OneMadGypsy/fuzzquery
 Project-URL: Issues, https://github.com/OneMadGypsy/fuzzquery/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: regex>=2024.5.15
 
 # fuzzquery
-A lightwieght package for doing fuzzy matches with a simple query language. This works by creating regular expressions for you that utilize the fuzzy matching features of the `regex` package, based on your query tokens. 
+A lightweight package for fuzzy matching.
 
 
 ## Installation:
 To install `fuzzquery` and it's `regex` dependency, open a terminal and input the following command: 
 ### `pip install fuzzquery`
 
+
 ## Theory:
-The regex package has 3 fuzzy matching features:
+The `regex` package has 3 fuzzy matching features:
 
-| type       | dsecription                                       |
+| type       | description                                       |
 | ---------- | ------------------------------------------------- |
 | insert     | 0 or more characters appear **before** your term  |
 | substitute | 0 or more characters are substituted in your term |
 | delete     | 0 or more characters are removed from your term   |
 
-This system completely ignores the native insertion model and creates it's own with substitution and deletion. This is because insertion is wholly uncontrollable. It is the only feature that allows characters where there never were any. My system reformats queries with substitution/deletion characters wherever a token is present. This means if you put a token before your term, it is essentially a controllable insertion. The back-end system will view it as a substitution and/or deletion, but it is a sub/del before your term so, it is functionally an insertion. 
+This system completely ignores the native insertion model and creates it's own with substitution and deletion. This is because insertion is wholly uncontrollable. It is the only feature that allows characters where there never were any. My system reformats queries with substitution/deletion characters wherever a token is present. This means if you put a token before your term, it is functionally an insertion.
 
-Substitutions and deletions can only happen where sub/del characters are present. This is because the sub/del score limit is identical to the amount of sub/del characters. If a non-sub/del character was to be subbed or deleted, it would leave behind an original sub/del character (backtick), and the final sub/del score would be too high to match. Basically, you can reliably search for anything that does **not** have a backtick in it. Technically, you can even reliably search for things that do have a backtick in them, but you are playing with the possibility of hitting an edge case that may yield some incorrect results. However, the `skip` feature could be used to ignore the incorrect results.
 
 ## Documentation:
 
 **notes:**
 
 1) `Iter` is an alias of `list|tuple|set`. It only exists in this documentation as a means to illustrate types in a less complex way.
-2) `skip` (if used) should be an `Iter` of words and/or characters that trigger a skip when found in results to be yielded.
+2) `skip` (if used) should be an `Iter` of words and/or characters that cannot be `in` a result.
 
 --------
 
-#### `finditer`
+### finditer
 > yield all (`span`, `match`) of a single query.
 
 **finditer(`text`:str, `query`:str, `skip`:Iter|None=None, `ci`:bool=False) -> Iterator**
-| arg      | description                                                                   |
-| -------- | ----------------------------------------------------------------------------- |
-| `text`   | the text to search                                                            |
-| `query`  | the query to search for                                                       |
-| `skip`   | iterable of terms and/or characters that trigger a skip when found in results |
-| `ci`     | case-insensitive matching                                                     |
+| arg      | description                                                               |
+| -------- | ------------------------------------------------------------------------- |
+| `text`   | the text to search                                                        |
+| `query`  | the query to search for                                                   |
+| `skip`   | Iter of terms and/or characters that trigger a skip when found in results |
+| `ci`     | case-insensitive matching                                                 |
 
 --------
 
-#### `findany`
+### findany
 > `OR` queries together and yield all (`span`, `match`) of whatever matched.
 
 **findany(`text`:str, `queries`:Iter, `skip`:Iter|None=None, `ci`:bool=False) -> Iterator**
-| arg       | description                                                                   |
-| --------- | ----------------------------------------------------------------------------- |
-| `text`    | the text to search                                                            |
-| `queries` | iterable of queries to search for                                             |
-| `skip`    | iterable of terms and/or characters that trigger a skip when found in results |
-| `ci`      | case-insensitive matching                                                     |
+| arg       | description                                                               |
+| --------- | ------------------------------------------------------------------------- |
+| `text`    | the text to search                                                        |
+| `queries` | Iter of queries to search for                                             |
+| `skip`    | Iter of terms and/or characters that trigger a skip when found in results |
+| `ci`      | case-insensitive matching                                                 |
 
 --------
 
-#### `iterall`
+### iterall
 > yield all (`query`, `span`, `match`) of multiple queries.
 
 **iterall(`text`:str, `queries`:Iter, `skip`:Iter|None=None, `ci`:bool=False) -> Iterator**
-| arg       | description                                                                   |
-| --------- | ----------------------------------------------------------------------------- |
-| `text`    | the text to search                                                            |
-| `queries` | iterable of queries to search for                                             |
-| `skip`    | iterable of terms and/or characters that trigger a skip when found in results |
-| `ci`      | case-insensitive matching                                                     |
+| arg       | description                                                               |
+| --------- | ------------------------------------------------------------------------- |
+| `text`    | the text to search                                                        |
+| `queries` | Iter of queries to search for                                             |
+| `skip`    | Iter of terms and/or characters that trigger a skip when found in results |
+| `ci`      | case-insensitive matching                                                 |
 
 
 ## Queries:
 
 A token system is used to represent unknown/fuzzy data. The 3 types of tokens are:
 
 | token  | type    | description                           | example           | result-like                     |
 | ------ | ------- | ------------------------------------- | ----------------- | ------------------------------- |
 | `{x}`  | allowed | 0 to `x` non-whitespace characters    | `"home{5}"`       | `home, homestead, homeward`     |
 | `{!x}` | strict  | exactly `x` non-whitespace characters | `"{1}ward{!2}"`   | `warden, awarded`               |
 | `{?}`  | unknown | 0 or more unknown words               | `"thou {?} kill"` | `thou shalt not kill`           |
 
+
 ## Examples:
 
 ```python3
 import fuzzquery as fq
 
 data = """ 
 I headed homeward to meet with the Wardens. 
 When I arrived, I was greeted by a homely man that told me the homestead was awarded 5 million dollars.
 We intend to use some of the homage to create a homeless ward. 
 The first piece of furniture will be my late-friend Homer's wardrobe.
 """
-queries = ('hom{5} {?} wa{8}', 
+queries = ('hom{5} {?} wa{!1}{5}', 
            'home{5}', 
            '{1}ward{!2}{2}', 
            'home{4} ward{4}')
 
 for query, span, match in fq.iterall(data, queries, ci=True):
     if query: print(f'\n{query.upper()}')
     print(f'  {match}')
 ```
 
 #### output
+
 ```none
-HOM{5} {?} WA{8}
+HOM{5} {?} WA{!1}{5}
   homeward to meet with the Wardens
   homely man that told me the homestead was
   homage to create a homeless ward
   Homer's wardrobe
 
 HOME{5}
   homeward
@@ -129,11 +131,48 @@
 
 {1}WARD{!2}{2}
   Wardens
   awarded
   wardrobe
 
 HOME{4} WARD{4}
-  homeward
   homeless ward
   Homer's wardrobe
 ```
+
+--------
+
+```python3
+import fuzzquery as fq
+
+data = """ 
+I would classify music as one of my favorite hobbies. 
+I love classical music played by classy musicians for a classic musical. 
+Beethoven can not be out-classed, music-wise - a man of class, musically gifted.
+"""
+query = 'class{4} music{4}'
+
+print(f'\n{query.upper()} with skip')
+for span, match in fq.finditer(data, query, skip=('classify', ','), ci=True):
+    print(f'  {match}')
+    
+print(f'\n{query.upper()} no skip')
+for span, match in fq.finditer(data, query, ci=True):
+    print(f'  {match}')
+```
+
+#### output
+
+```none
+CLASS{4} MUSIC{4} with skip
+  classical music
+  classy musicians
+  classic musical
+
+CLASS{4} MUSIC{4} no skip
+  classify music
+  classical music
+  classy musicians
+  classic musical
+  classed, music
+  class, musically
+```
```

