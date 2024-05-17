# Comparing `tmp/twelvelabs-0.1.23.tar.gz` & `tmp/twelvelabs-0.1.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twelvelabs-0.1.23.tar", last modified: Mon May  6 14:49:00 2024, max compression
+gzip compressed data, was "twelvelabs-0.1.24.tar", last modified: Fri May 17 03:30:16 2024, max compression
```

## Comparing `twelvelabs-0.1.23.tar` & `twelvelabs-0.1.24.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:49:00.338317 twelvelabs-0.1.23/
--rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16749 2024-05-06 14:49:00.338317 twelvelabs-0.1.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14147 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 14:49:00.338317 twelvelabs-0.1.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:49:00.334317 twelvelabs-0.1.23/twelvelabs/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:49:00.338317 twelvelabs-0.1.23/twelvelabs/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/models/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/models/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/models/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7099 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/models/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/models/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/models/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/models/video.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:49:00.338317 twelvelabs-0.1.23/twelvelabs/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/resources/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/resources/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/resources/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/resources/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7466 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/resources/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     7783 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/resources/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:49:00.338317 twelvelabs-0.1.23/twelvelabs/types/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/types/index.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:49:00.338317 twelvelabs-0.1.23/twelvelabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16749 2024-05-06 14:49:00.000000 twelvelabs-0.1.23/twelvelabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-06 14:49:00.000000 twelvelabs-0.1.23/twelvelabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 14:49:00.000000 twelvelabs-0.1.23/twelvelabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-06 14:49:00.000000 twelvelabs-0.1.23/twelvelabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 14:49:00.000000 twelvelabs-0.1.23/twelvelabs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:30:16.410175 twelvelabs-0.1.24/
+-rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16859 2024-05-17 03:30:16.410175 twelvelabs-0.1.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 03:30:16.410175 twelvelabs-0.1.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:30:16.406175 twelvelabs-0.1.24/twelvelabs/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:30:16.406175 twelvelabs-0.1.24/twelvelabs/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/models/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/models/classify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/models/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/models/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7099 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/models/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/models/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/models/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:30:16.410175 twelvelabs-0.1.24/twelvelabs/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/resources/classify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/resources/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/resources/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/resources/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/resources/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7463 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/resources/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7783 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/resources/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:30:16.410175 twelvelabs-0.1.24/twelvelabs/types/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/types/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:30:16.406175 twelvelabs-0.1.24/twelvelabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16859 2024-05-17 03:30:16.000000 twelvelabs-0.1.24/twelvelabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-17 03:30:16.000000 twelvelabs-0.1.24/twelvelabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 03:30:16.000000 twelvelabs-0.1.24/twelvelabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-17 03:30:16.000000 twelvelabs-0.1.24/twelvelabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 03:30:16.000000 twelvelabs-0.1.24/twelvelabs.egg-info/top_level.txt
```

### Comparing `twelvelabs-0.1.23/LICENSE` & `twelvelabs-0.1.24/LICENSE`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.23/PKG-INFO` & `twelvelabs-0.1.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: twelvelabs
-Version: 0.1.23
+Version: 0.1.24
 Summary: SDK for Twelve Labs API
 Home-page: https://github.com/twelvelabs-io/twelvelabs-python
 Author: Twelve Labs
 License: UNKNOWN
 Description: # TwelveLabs Python SDK
+        [![PyPI version](https://img.shields.io/pypi/v/twelvelabs.svg)](https://pypi.org/project/twelvelabs/)
         
         This SDK provides a convenient way to interact with the Twelve Labs Video Understanding Platform from an application written in the Python language. The SDK equips you with a set of intuitive classes and methods that streamline the process of interacting with the platform, minimizing the need for boilerplate code.
         
         # Prerequisites
         
         Ensure that the following prerequisites are met before using the SDK:
```

### Comparing `twelvelabs-0.1.23/README.md` & `twelvelabs-0.1.24/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # TwelveLabs Python SDK
+[![PyPI version](https://img.shields.io/pypi/v/twelvelabs.svg)](https://pypi.org/project/twelvelabs/)
 
 This SDK provides a convenient way to interact with the Twelve Labs Video Understanding Platform from an application written in the Python language. The SDK equips you with a set of intuitive classes and methods that streamline the process of interacting with the platform, minimizing the need for boilerplate code.
 
 # Prerequisites
 
 Ensure that the following prerequisites are met before using the SDK:
```

### Comparing `twelvelabs-0.1.23/setup.py` & `twelvelabs-0.1.24/setup.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.23/twelvelabs/__init__.py` & `twelvelabs-0.1.24/twelvelabs/__init__.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.23/twelvelabs/base_client.py` & `twelvelabs-0.1.24/twelvelabs/base_client.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.23/twelvelabs/client.py` & `twelvelabs-0.1.24/twelvelabs/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 class TwelveLabs(APIClient):
     engine: resources.Engine
     index: resources.Index
     task: resources.Task
     search: resources.Search
     generate: resources.Generate
+    classify: resources.Classify
 
     base_url: str
     api_key: str
 
     def __init__(
         self,
         api_key: str,
@@ -38,13 +39,14 @@
         super().__init__(base_url, api_key)
 
         self.engine = resources.Engine(self)
         self.index = resources.Index(self)
         self.task = resources.Task(self)
         self.search = resources.Search(self)
         self.generate = resources.Generate(self)
+        self.classify = resources.Classify(self)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc, tb):
         pass
```

### Comparing `twelvelabs-0.1.23/twelvelabs/exceptions.py` & `twelvelabs-0.1.24/twelvelabs/exceptions.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.23/twelvelabs/models/__init__.py` & `twelvelabs-0.1.24/twelvelabs/models/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,46 @@
-from ._base import Object, ObjectWithTimestamp, PageInfo, RootModelList
+from ._base import Object, ObjectWithTimestamp, PageInfo, TokenPageInfo, RootModelList
 from .engine import Engine
 from .index import Index, IndexListWithPagination
 from .task import Task, TaskStatus, TaskListWithPagination
 from .video import Video, VideoValue, VideoListWithPagination
-from .search import SearchData, SearchPageInfo, SearchResult, CombinedSearchResult, GroupByVideoSearchData
+from .search import (
+    SearchData,
+    SearchResult,
+    CombinedSearchResult,
+)
 from .generate import (
     GenerateOpenEndedTextResult,
     GenerateSummarizeChapterResult,
     GenerateSummarizeHighlightResult,
     GenerateSummarizeResult,
     GenerateGistResult,
 )
+from .classify import ClassifyClassParams, ClassifyResult, ClassifyPageResult
 
 __all__ = [
     "Object",
     "ObjectWithTimestamp",
     "PageInfo",
+    "TokenPageInfo",
     "Engine",
     "Index",
     "IndexListWithPagination",
     "Task",
     "TaskListWithPagination",
     "TaskStatus",
     "Video",
     "VideoValue",
     "VideoListWithPagination",
     "SearchData",
-    "SearchPageInfo",
     "SearchResult",
     "CombinedSearchResult",
+    "ClassifyClassParams",
+    "ClassifyResult",
+    "ClassifyPageResult",
     "GenerateOpenEndedTextResult",
     "GenerateSummarizeChapterResult",
     "GenerateSummarizeHighlightResult",
     "GenerateSummarizeResult",
     "GenerateGistResult",
     "RootModelList",
 ]
```

### Comparing `twelvelabs-0.1.23/twelvelabs/models/_base.py` & `twelvelabs-0.1.24/twelvelabs/models/_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,22 @@
 class PageInfo(BaseModel):
     limit_per_page: int
     page: int
     total_page: int
     total_results: int
 
 
+class TokenPageInfo(BaseModel):
+    limit_per_page: int
+    total_results: int
+    page_expired_at: str
+    next_page_token: Optional[str] = None
+    prev_page_token: Optional[str] = None
+
+
 T = TypeVar("T")
 
 
 class RootModelList(RootModel[List[T]]):
     """
     See https://docs.pydantic.dev/latest/concepts/models/#rootmodel-and-custom-root-types
     """
```

### Comparing `twelvelabs-0.1.23/twelvelabs/models/generate.py` & `twelvelabs-0.1.24/twelvelabs/models/generate.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.23/twelvelabs/models/index.py` & `twelvelabs-0.1.24/twelvelabs/models/index.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.23/twelvelabs/models/search.py` & `twelvelabs-0.1.24/twelvelabs/models/search.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from typing import List, Optional, TYPE_CHECKING, Dict, Any, Union, Literal
 from pydantic import Field, PrivateAttr
 
-from ._base import BaseModel, ModelMixin, RootModelList
+from ._base import BaseModel, ModelMixin, RootModelList, TokenPageInfo
 
 if TYPE_CHECKING:
     from ..resources import Search as SearchResource
 
 
 class SearchPool(BaseModel):
     total_count: int
@@ -33,27 +33,19 @@
 
 
 class GroupByVideoSearchData(BaseModel):
     clips: Optional[RootModelList[SearchData]] = None
     id: str
 
 
-class SearchPageInfo(BaseModel):
-    limit_per_page: int
-    total_results: int
-    page_expired_at: str
-    next_page_token: Optional[str] = None
-    prev_page_token: Optional[str] = None
-
-
 class SearchResult(ModelMixin, BaseModel):
     _resource: SearchResource = PrivateAttr()
     pool: SearchPool = Field(alias="search_pool")
     data: RootModelList[Union[SearchData, GroupByVideoSearchData]]
-    page_info: SearchPageInfo
+    page_info: TokenPageInfo
 
     def __init__(self, resource: SearchResource, **data):
         super().__init__(**data)
         self._resource = resource
 
     def __iter__(self):
         return self
```

### Comparing `twelvelabs-0.1.23/twelvelabs/models/task.py` & `twelvelabs-0.1.24/twelvelabs/models/task.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.23/twelvelabs/models/video.py` & `twelvelabs-0.1.24/twelvelabs/models/video.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.23/twelvelabs/resources/generate.py` & `twelvelabs-0.1.24/twelvelabs/resources/generate.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.23/twelvelabs/resources/index.py` & `twelvelabs-0.1.24/twelvelabs/resources/index.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.23/twelvelabs/resources/search.py` & `twelvelabs-0.1.24/twelvelabs/resources/search.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.23/twelvelabs/resources/task.py` & `twelvelabs-0.1.24/twelvelabs/resources/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             "page_limit": page_limit,
             "sort_by": sort_by,
             "sort_option": sort_option,
         }
         handle_comparison_params(params, "created_at", created_at)
         handle_comparison_params(params, "updated_at", updated_at)
         res = self._get("tasks", params=remove_none_values(params), **kwargs)
-        return RootModelList(   [models.Task(self, **task) for task in res["data"]])
+        return RootModelList([models.Task(self, **task) for task in res["data"]])
 
     def list_pagination(
         self,
         *,
         id: Optional[str] = None,
         index_id: Optional[str] = None,
         filename: Optional[str] = None,
```

### Comparing `twelvelabs-0.1.23/twelvelabs/resources/video.py` & `twelvelabs-0.1.24/twelvelabs/resources/video.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.23/twelvelabs/util.py` & `twelvelabs-0.1.24/twelvelabs/util.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.23/twelvelabs.egg-info/PKG-INFO` & `twelvelabs-0.1.24/twelvelabs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: twelvelabs
-Version: 0.1.23
+Version: 0.1.24
 Summary: SDK for Twelve Labs API
 Home-page: https://github.com/twelvelabs-io/twelvelabs-python
 Author: Twelve Labs
 License: UNKNOWN
 Description: # TwelveLabs Python SDK
+        [![PyPI version](https://img.shields.io/pypi/v/twelvelabs.svg)](https://pypi.org/project/twelvelabs/)
         
         This SDK provides a convenient way to interact with the Twelve Labs Video Understanding Platform from an application written in the Python language. The SDK equips you with a set of intuitive classes and methods that streamline the process of interacting with the platform, minimizing the need for boilerplate code.
         
         # Prerequisites
         
         Ensure that the following prerequisites are met before using the SDK:
```

### Comparing `twelvelabs-0.1.23/twelvelabs.egg-info/SOURCES.txt` & `twelvelabs-0.1.24/twelvelabs.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -11,21 +11,23 @@
 twelvelabs.egg-info/PKG-INFO
 twelvelabs.egg-info/SOURCES.txt
 twelvelabs.egg-info/dependency_links.txt
 twelvelabs.egg-info/requires.txt
 twelvelabs.egg-info/top_level.txt
 twelvelabs/models/__init__.py
 twelvelabs/models/_base.py
+twelvelabs/models/classify.py
 twelvelabs/models/engine.py
 twelvelabs/models/generate.py
 twelvelabs/models/index.py
 twelvelabs/models/search.py
 twelvelabs/models/task.py
 twelvelabs/models/video.py
 twelvelabs/resources/__init__.py
+twelvelabs/resources/classify.py
 twelvelabs/resources/engine.py
 twelvelabs/resources/generate.py
 twelvelabs/resources/index.py
 twelvelabs/resources/search.py
 twelvelabs/resources/task.py
 twelvelabs/resources/video.py
 twelvelabs/types/__init__.py
```

