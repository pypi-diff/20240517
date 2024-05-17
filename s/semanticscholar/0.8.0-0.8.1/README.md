# Comparing `tmp/semanticscholar-0.8.0.tar.gz` & `tmp/semanticscholar-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semanticscholar-0.8.0.tar", last modified: Sat Mar 16 02:57:43 2024, max compression
+gzip compressed data, was "semanticscholar-0.8.1.tar", last modified: Fri May 17 15:50:33 2024, max compression
```

## Comparing `semanticscholar-0.8.0.tar` & `semanticscholar-0.8.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 02:57:43.487749 semanticscholar-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-16 02:57:35.000000 semanticscholar-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14371 2024-03-16 02:57:43.487749 semanticscholar-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13357 2024-03-16 02:57:35.000000 semanticscholar-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 02:57:43.483749 semanticscholar-0.8.0/semanticscholar/
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-03-16 02:57:35.000000 semanticscholar-0.8.0/semanticscholar/ApiRequester.py
--rw-r--r--   0 runner    (1001) docker     (127)    25263 2024-03-16 02:57:35.000000 semanticscholar-0.8.0/semanticscholar/AsyncSemanticScholar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-03-16 02:57:35.000000 semanticscholar-0.8.0/semanticscholar/Author.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-03-16 02:57:35.000000 semanticscholar-0.8.0/semanticscholar/BaseReference.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-16 02:57:35.000000 semanticscholar-0.8.0/semanticscholar/Citation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-03-16 02:57:35.000000 semanticscholar-0.8.0/semanticscholar/Journal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-03-16 02:57:35.000000 semanticscholar-0.8.0/semanticscholar/PaginatedResults.py
--rw-r--r--   0 runner    (1001) docker     (127)    10827 2024-03-16 02:57:35.000000 semanticscholar-0.8.0/semanticscholar/Paper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-03-16 02:57:35.000000 semanticscholar-0.8.0/semanticscholar/PublicationVenue.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-16 02:57:35.000000 semanticscholar-0.8.0/semanticscholar/Reference.py
--rw-r--r--   0 runner    (1001) docker     (127)    19114 2024-03-16 02:57:35.000000 semanticscholar-0.8.0/semanticscholar/SemanticScholar.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-16 02:57:35.000000 semanticscholar-0.8.0/semanticscholar/SemanticScholarException.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-03-16 02:57:35.000000 semanticscholar-0.8.0/semanticscholar/SemanticScholarObject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-03-16 02:57:35.000000 semanticscholar-0.8.0/semanticscholar/Tldr.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-16 02:57:35.000000 semanticscholar-0.8.0/semanticscholar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 02:57:43.483749 semanticscholar-0.8.0/semanticscholar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14371 2024-03-16 02:57:43.000000 semanticscholar-0.8.0/semanticscholar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-16 02:57:43.000000 semanticscholar-0.8.0/semanticscholar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 02:57:43.000000 semanticscholar-0.8.0/semanticscholar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 02:57:43.000000 semanticscholar-0.8.0/semanticscholar.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-16 02:57:43.000000 semanticscholar-0.8.0/semanticscholar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-16 02:57:43.000000 semanticscholar-0.8.0/semanticscholar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 02:57:43.487749 semanticscholar-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-16 02:57:35.000000 semanticscholar-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 02:57:43.483749 semanticscholar-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    38236 2024-03-16 02:57:35.000000 semanticscholar-0.8.0/tests/test_semanticscholar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:50:33.806467 semanticscholar-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14431 2024-05-17 15:50:33.806467 semanticscholar-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13417 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:50:33.806467 semanticscholar-0.8.1/semanticscholar/
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/ApiRequester.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25987 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/AsyncSemanticScholar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/Author.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/BaseReference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/Citation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/Journal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/PaginatedResults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10827 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/Paper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/PublicationVenue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/Reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/SemanticScholar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/SemanticScholarException.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/SemanticScholarObject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/Tldr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:50:33.806467 semanticscholar-0.8.1/semanticscholar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14431 2024-05-17 15:50:33.000000 semanticscholar-0.8.1/semanticscholar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-17 15:50:33.000000 semanticscholar-0.8.1/semanticscholar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 15:50:33.000000 semanticscholar-0.8.1/semanticscholar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 15:50:33.000000 semanticscholar-0.8.1/semanticscholar.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-17 15:50:33.000000 semanticscholar-0.8.1/semanticscholar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-17 15:50:33.000000 semanticscholar-0.8.1/semanticscholar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 15:50:33.806467 semanticscholar-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:50:33.806467 semanticscholar-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    40321 2024-05-17 15:50:26.000000 semanticscholar-0.8.1/tests/test_semanticscholar.py
```

### Comparing `semanticscholar-0.8.0/LICENSE` & `semanticscholar-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `semanticscholar-0.8.0/PKG-INFO` & `semanticscholar-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semanticscholar
-Version: 0.8.0
+Version: 0.8.1
 Summary: Unofficial Python client library for Semantic Scholar APIs.
 Home-page: http://danielnsilva.com/semanticscholar
 Author: Daniel Silva
 Author-email: danielnsilva@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -31,15 +31,15 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/semanticscholar?style=for-the-badge)
 [![GitHub license](https://img.shields.io/github/license/danielnsilva/semanticscholar?style=for-the-badge)](https://github.com/danielnsilva/semanticscholar/blob/master/LICENSE)
 [![Codacy grade](https://img.shields.io/codacy/grade/1456603c25764b14b441ed509e938154?style=for-the-badge)](https://www.codacy.com/gh/danielnsilva/semanticscholar/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=danielnsilva/semanticscholar&amp;utm_campaign=Badge_Grade)
 [![Codacy coverage](https://img.shields.io/codacy/coverage/1456603c25764b14b441ed509e938154?style=for-the-badge)](https://www.codacy.com/gh/danielnsilva/semanticscholar/dashboard?utm_source=github.com&utm_medium=referral&utm_content=danielnsilva/semanticscholar&utm_campaign=Badge_Coverage)
 
 Unofficial Python client library for [Semantic Scholar APIs](https://api.semanticscholar.org/), currently supporting the Academic Graph API and Recommendations API.
 
-![Usage example](search_paper.gif)
+![Usage example](https://github.com/danielnsilva/semanticscholar/blob/master/search_paper.gif)
 
 ## Table of Contents
 
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
 - [How to install](#how-to-install)
```

### Comparing `semanticscholar-0.8.0/README.md` & `semanticscholar-0.8.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/semanticscholar?style=for-the-badge)
 [![GitHub license](https://img.shields.io/github/license/danielnsilva/semanticscholar?style=for-the-badge)](https://github.com/danielnsilva/semanticscholar/blob/master/LICENSE)
 [![Codacy grade](https://img.shields.io/codacy/grade/1456603c25764b14b441ed509e938154?style=for-the-badge)](https://www.codacy.com/gh/danielnsilva/semanticscholar/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=danielnsilva/semanticscholar&amp;utm_campaign=Badge_Grade)
 [![Codacy coverage](https://img.shields.io/codacy/coverage/1456603c25764b14b441ed509e938154?style=for-the-badge)](https://www.codacy.com/gh/danielnsilva/semanticscholar/dashboard?utm_source=github.com&utm_medium=referral&utm_content=danielnsilva/semanticscholar&utm_campaign=Badge_Coverage)
 
 Unofficial Python client library for [Semantic Scholar APIs](https://api.semanticscholar.org/), currently supporting the Academic Graph API and Recommendations API.
 
-![Usage example](search_paper.gif)
+![Usage example](https://github.com/danielnsilva/semanticscholar/blob/master/search_paper.gif)
 
 ## Table of Contents
 
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
 - [How to install](#how-to-install)
```

### Comparing `semanticscholar-0.8.0/semanticscholar/ApiRequester.py` & `semanticscholar-0.8.1/semanticscholar/ApiRequester.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import List, Union
 
 import httpx
 import asyncio
 import warnings
-import inspect
 import json
-from tenacity import (retry as rerun, retry_if_exception_type, stop_after_attempt,
-                      wait_fixed)
+from tenacity import (retry as rerun, retry_if_exception_type,
+                      stop_after_attempt, wait_fixed)
 
 from semanticscholar.SemanticScholarException import \
     BadQueryParametersException, ObjectNotFoundException
 
 
 class ApiRequester:
```

### Comparing `semanticscholar-0.8.0/semanticscholar/AsyncSemanticScholar.py` & `semanticscholar-0.8.1/semanticscholar/AsyncSemanticScholar.py`

 * *Files 3% similar despite different names*

```diff
@@ -510,43 +510,57 @@
         author = Author(data)
 
         return author
 
     async def get_authors(
                 self,
                 author_ids: List[str],
-                fields: list = None
-            ) -> List[Author]:
+                fields: list = None,
+                return_not_found: bool = False
+            ) -> Union[List[Author], Tuple[List[Author], List[str]]]:
         '''Get details for multiple authors at once
 
         :calls: `POST /author/batch <https://api.semanticscholar.org/api-docs/\
             graph#tag/Author-Data/operation/get_graph_get_author>`_
 
         :param str author_ids: list of S2AuthorId (must be <= 1000).
-        :returns: author data
-        :rtype: :class:`List` of :class:`semanticscholar.Author.Author`
+        :returns: author data, and optionally list of IDs not found.
+        :rtype: :class:`List` of :class:`semanticscholar.Author.Author`\
+            or :class:`Tuple`[:class:`List` of\
+            :class:`semanticscholar.Author.Author`,\
+            :class:`List` of :class:`str`]
         :raises: BadQueryParametersException: if no author was found.
         '''
 
+        if len(author_ids) > 1000 or len(author_ids) == 0:
+            raise ValueError(
+                'The author_ids parameter must be a list of 1 to 1000 IDs.')
+
         if not fields:
             fields = Author.SEARCH_FIELDS
 
         base_url = self.api_url + self.BASE_PATH_GRAPH
         url = f'{base_url}/author/batch'
 
         fields = ','.join(fields)
         parameters = f'&fields={fields}'
 
         payload = { "ids": author_ids }
 
         data = await self._requester.get_data_async(
             url, parameters, self.auth_header, payload)
-        authors = [Author(item) for item in data]
+        authors = [Author(item) for item in data if item is not None]
+
+        found_ids = [author.authorId for author in authors]
+        not_found_ids = list(set(author_ids) - set(found_ids))
+
+        if not_found_ids:
+            warnings.warn(f"IDs not found: {not_found_ids}")
 
-        return authors
+        return authors if not return_not_found else (authors, not_found_ids)
 
     async def get_author_papers(
                 self,
                 author_id: str,
                 fields: list = None,
                 limit: int = 100
             ) -> PaginatedResults:
```

### Comparing `semanticscholar-0.8.0/semanticscholar/Author.py` & `semanticscholar-0.8.1/semanticscholar/Author.py`

 * *Files identical despite different names*

### Comparing `semanticscholar-0.8.0/semanticscholar/BaseReference.py` & `semanticscholar-0.8.1/semanticscholar/BaseReference.py`

 * *Files identical despite different names*

### Comparing `semanticscholar-0.8.0/semanticscholar/PaginatedResults.py` & `semanticscholar-0.8.1/semanticscholar/PaginatedResults.py`

 * *Files identical despite different names*

### Comparing `semanticscholar-0.8.0/semanticscholar/Paper.py` & `semanticscholar-0.8.1/semanticscholar/Paper.py`

 * *Files identical despite different names*

### Comparing `semanticscholar-0.8.0/semanticscholar/PublicationVenue.py` & `semanticscholar-0.8.1/semanticscholar/PublicationVenue.py`

 * *Files identical despite different names*

### Comparing `semanticscholar-0.8.0/semanticscholar/SemanticScholar.py` & `semanticscholar-0.8.1/semanticscholar/SemanticScholar.py`

 * *Files 3% similar despite different names*

```diff
@@ -376,32 +376,37 @@
         )
 
         return author
 
     def get_authors(
                 self,
                 author_ids: List[str],
-                fields: list = None
-            ) -> List[Author]:
+                fields: list = None,
+                return_not_found: bool = False
+            ) -> Union[List[Author], Tuple[List[Author], List[str]]]:
         '''Get details for multiple authors at once
 
         :calls: `POST /author/batch <https://api.semanticscholar.org/api-docs/\
             graph#tag/Author-Data/operation/get_graph_get_author>`_
 
         :param str author_ids: list of S2AuthorId (must be <= 1000).
-        :returns: author data
-        :rtype: :class:`List` of :class:`semanticscholar.Author.Author`
+        :returns: author data, and optionally list of IDs not found.
+        :rtype: :class:`List` of :class:`semanticscholar.Author.Author`\
+            or :class:`Tuple`[:class:`List` of\
+            :class:`semanticscholar.Author.Author`,\
+            :class:`List` of :class:`str`]
         :raises: BadQueryParametersException: if no author was found.
         '''
 
         loop = asyncio.get_event_loop()
         authors = loop.run_until_complete(
             self._AsyncSemanticScholar.get_authors(
                 author_ids=author_ids,
-                fields=fields
+                fields=fields,
+                return_not_found=return_not_found
                 )
         )
 
         return authors
 
     def get_author_papers(
                 self,
```

### Comparing `semanticscholar-0.8.0/semanticscholar/SemanticScholarObject.py` & `semanticscholar-0.8.1/semanticscholar/SemanticScholarObject.py`

 * *Files identical despite different names*

### Comparing `semanticscholar-0.8.0/semanticscholar/Tldr.py` & `semanticscholar-0.8.1/semanticscholar/Tldr.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,53 +1,37 @@
 from typing import Any
 
+from semanticscholar.SemanticScholarObject import SemanticScholarObject
 
-class Tldr:
+
+class Tldr(SemanticScholarObject):
     '''
     This class represents auto-generated short summary of the paper from the
     SciTLDR model.
     '''
 
     def __init__(self, data) -> None:
+        super().__init__()
         self._model = None
         self._text = None
         self._init_attributes(data)
 
-    def __str__(self) -> str:
-        return self._text
-
-    def __repr__(self) -> str:
-        return self.__str__()
-
-    def __getitem__(self, key) -> Any:
-        return self._data.__getitem__(key)
-
-    def keys(self):
-        return self._data.keys()
-
     @property
     def model(self) -> str:
         '''
         :type :class:`str`
         '''
         return self._model
 
     @property
     def text(self) -> str:
         '''
         :type: :class:`str`
         '''
         return self._text
 
-    @property
-    def raw_data(self) -> dict:
-        '''
-        :type: :class:`dict`
-        '''
-        return self._data
-
     def _init_attributes(self, data):
         self._data = data
         if 'model' in data:
             self._model = data['model']
         if 'text' in data:
             self._text = data['text']
```

### Comparing `semanticscholar-0.8.0/semanticscholar.egg-info/PKG-INFO` & `semanticscholar-0.8.1/semanticscholar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semanticscholar
-Version: 0.8.0
+Version: 0.8.1
 Summary: Unofficial Python client library for Semantic Scholar APIs.
 Home-page: http://danielnsilva.com/semanticscholar
 Author: Daniel Silva
 Author-email: danielnsilva@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -31,15 +31,15 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/semanticscholar?style=for-the-badge)
 [![GitHub license](https://img.shields.io/github/license/danielnsilva/semanticscholar?style=for-the-badge)](https://github.com/danielnsilva/semanticscholar/blob/master/LICENSE)
 [![Codacy grade](https://img.shields.io/codacy/grade/1456603c25764b14b441ed509e938154?style=for-the-badge)](https://www.codacy.com/gh/danielnsilva/semanticscholar/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=danielnsilva/semanticscholar&amp;utm_campaign=Badge_Grade)
 [![Codacy coverage](https://img.shields.io/codacy/coverage/1456603c25764b14b441ed509e938154?style=for-the-badge)](https://www.codacy.com/gh/danielnsilva/semanticscholar/dashboard?utm_source=github.com&utm_medium=referral&utm_content=danielnsilva/semanticscholar&utm_campaign=Badge_Coverage)
 
 Unofficial Python client library for [Semantic Scholar APIs](https://api.semanticscholar.org/), currently supporting the Academic Graph API and Recommendations API.
 
-![Usage example](search_paper.gif)
+![Usage example](https://github.com/danielnsilva/semanticscholar/blob/master/search_paper.gif)
 
 ## Table of Contents
 
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
 - [How to install](#how-to-install)
```

### Comparing `semanticscholar-0.8.0/semanticscholar.egg-info/SOURCES.txt` & `semanticscholar-0.8.1/semanticscholar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `semanticscholar-0.8.0/setup.py` & `semanticscholar-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 
 setup(
     name='semanticscholar',
-    version='0.8.0',
+    version='0.8.1',
     description='Unofficial Python client library for Semantic Scholar APIs.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='http://danielnsilva.com/semanticscholar',
     author='Daniel Silva',
     author_email='danielnsilva@gmail.com',
     license='MIT',
```

### Comparing `semanticscholar-0.8.0/tests/test_semanticscholar.py` & `semanticscholar-0.8.1/tests/test_semanticscholar.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         file = open('tests/data/Paper.json', encoding='utf-8')
         data = json.loads(file.read())['journal']
         item = Journal(data)
         self.assertEqual(item.name, data['name'])
         self.assertEqual(item.pages, data['pages'])
         self.assertEqual(item.volume, data['volume'])
         self.assertEqual(item.raw_data, data)
-        self.assertEqual(str(item), data['name'])
+        self.assertEqual(str(item), str(data))
         self.assertEqual(item['name'], data['name'])
         self.assertEqual(item.keys(), data.keys())
         file.close()
 
     def test_paper(self) -> None:
         file = open('tests/data/Paper.json', encoding='utf-8')
         data = json.loads(file.read())
@@ -92,26 +92,26 @@
         self.assertEqual(item.corpusId, data['corpusId'])
         self.assertEqual(item.embedding, data['embedding'])
         self.assertEqual(item.externalIds, data['externalIds'])
         self.assertEqual(item.fieldsOfStudy, data['fieldsOfStudy'])
         self.assertEqual(item.influentialCitationCount,
                          data['influentialCitationCount'])
         self.assertEqual(item.isOpenAccess, data['isOpenAccess'])
-        self.assertEqual(str(item.journal), str(data['journal']['name']))
+        self.assertEqual(str(item.journal), str(data['journal']))
         self.assertEqual(item.openAccessPdf, data['openAccessPdf'])
         self.assertEqual(item.paperId, data['paperId'])
         self.assertEqual(item.publicationDate, datetime.strptime(
             data['publicationDate'], '%Y-%m-%d'))
         self.assertEqual(item.publicationTypes, data['publicationTypes'])
         self.assertEqual(item.publicationVenue, data['publicationVenue'])
         self.assertEqual(item.referenceCount, data['referenceCount'])
         self.assertEqual(str(item.references), str(data['references']))
         self.assertEqual(item.s2FieldsOfStudy, data['s2FieldsOfStudy'])
         self.assertEqual(item.title, data['title'])
-        self.assertEqual(str(item.tldr), data['tldr']['text'])
+        self.assertEqual(str(item.tldr), str(data['tldr']))
         self.assertEqual(item.url, data['url'])
         self.assertEqual(item.venue, data['venue'])
         self.assertEqual(item.year, data['year'])
         self.assertEqual(item.raw_data, data)
         self.assertEqual(str(item), str(data))
         self.assertEqual(item['title'], data['title'])
         self.assertEqual(item.keys(), data.keys())
@@ -152,15 +152,15 @@
     def test_tldr(self) -> None:
         file = open('tests/data/Paper.json', encoding='utf-8')
         data = json.loads(file.read())['tldr']
         item = Tldr(data)
         self.assertEqual(item.model, data['model'])
         self.assertEqual(item.text, data['text'])
         self.assertEqual(item.raw_data, data)
-        self.assertEqual(str(item), data['text'])
+        self.assertEqual(str(item), str(data))
         self.assertEqual(item['model'], data['model'])
         self.assertEqual(item.keys(), data.keys())
         file.close()
 
     @test_vcr.use_cassette
     def test_get_paper(self):
         data = self.sch.get_paper('10.1093/mind/lix.236.433')
@@ -260,14 +260,38 @@
     def test_get_authors(self):
         list_of_author_ids = ['3234559', '1726629', '1711844']
         data = self.sch.get_authors(list_of_author_ids)
         list_of_author_names = ['E. Dijkstra', 'D. Parnas', 'I. Sommerville']
         self.assertCountEqual(
             [item.name for item in data], list_of_author_names)
 
+    def test_get_authors_list_size_exceeded(self):
+        list_of_author_ids = [str(i) for i in range(1001)]
+        self.assertRaises(ValueError, self.sch.get_authors, list_of_author_ids)
+
+    def test_get_authors_list_empty(self):
+        list_of_author_ids = []
+        self.assertRaises(ValueError, self.sch.get_authors, list_of_author_ids)
+
+    @test_vcr.use_cassette
+    def test_get_authors_not_found_warning(self):
+        list_of_author_ids = ['0', '3234559', '1726629', '1711844']
+        with self.assertWarns(UserWarning):
+            self.sch.get_authors(list_of_author_ids)
+
+    @test_vcr.use_cassette
+    def test_get_authors_return_not_found(self):
+        list_of_author_ids = ['0', '3234559', '1726629', '1711844']
+        data = self.sch.get_authors(list_of_author_ids, return_not_found=True)
+        authors = data[0]
+        self.assertEqual(len(authors), 3)
+        not_found = data[1]
+        self.assertEqual(len(not_found), 1)
+        self.assertEqual(not_found[0], '0')
+
     @test_vcr.use_cassette
     def test_get_author_papers(self):
         data = self.sch.get_author_papers(1723755, limit=100)
         self.assertEqual(data.offset, 0)
         self.assertEqual(data.next, 100)
         self.assertEqual(len([item for item in data]), 879)
         self.assertEqual(data[0].title, 'SARS-CoV-2 hijacks p38β/MAPK11 to '
@@ -648,14 +672,40 @@
     async def test_get_authors_async(self):
         list_of_author_ids = ['3234559', '1726629', '1711844']
         data = await self.sch.get_authors(list_of_author_ids)
         list_of_author_names = ['E. Dijkstra', 'D. Parnas', 'I. Sommerville']
         self.assertCountEqual(
             [item.name for item in data], list_of_author_names)
 
+    async def test_get_authors_list_size_exceeded_async(self):
+        list_of_author_ids = [str(i) for i in range(1001)]
+        with self.assertRaises(ValueError):
+            await self.sch.get_authors(list_of_author_ids)
+
+    async def test_get_authors_list_empty_async(self):
+        list_of_author_ids = []
+        with self.assertRaises(ValueError):
+            await self.sch.get_authors(list_of_author_ids)
+
+    @test_vcr.use_cassette
+    async def test_get_authors_not_found_warning_async(self):
+        list_of_author_ids = ['0', '3234559', '1726629', '1711844']
+        with self.assertWarns(UserWarning):
+            await self.sch.get_authors(list_of_author_ids)
+
+    @test_vcr.use_cassette
+    async def test_get_authors_return_not_found_async(self):
+        list_of_author_ids = ['0', '3234559', '1726629', '1711844']
+        data = await self.sch.get_authors(list_of_author_ids, return_not_found=True)
+        authors = data[0]
+        self.assertEqual(len(authors), 3)
+        not_found = data[1]
+        self.assertEqual(len(not_found), 1)
+        self.assertEqual(not_found[0], '0')
+
     @test_vcr.use_cassette
     async def test_not_found_async(self):
         with self.assertRaises(ObjectNotFoundException):
             await self.sch.get_paper(0)
         with self.assertRaises(ObjectNotFoundException):
             await self.sch.get_author(0)
```

