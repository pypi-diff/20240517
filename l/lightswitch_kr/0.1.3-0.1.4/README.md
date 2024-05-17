# Comparing `tmp/lightswitch_kr-0.1.3.tar.gz` & `tmp/lightswitch_kr-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightswitch_kr-0.1.3.tar", max compression
+gzip compressed data, was "lightswitch_kr-0.1.4.tar", max compression
```

## Comparing `lightswitch_kr-0.1.3.tar` & `lightswitch_kr-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      261 2024-05-16 05:15:34.401889 lightswitch_kr-0.1.3/lightswitch/__init__.py
--rw-r--r--   0        0        0     3103 2024-05-14 07:02:02.552428 lightswitch_kr-0.1.3/lightswitch/custom_sseclient.py
--rw-r--r--   0        0        0     1587 2024-05-13 01:44:03.193340 lightswitch_kr-0.1.3/lightswitch/exceptions.py
--rw-r--r--   0        0        0     9768 2024-05-16 05:41:52.140479 lightswitch_kr-0.1.3/lightswitch/lightswitch.py
--rw-r--r--   0        0        0     6366 2024-05-16 06:25:46.112204 lightswitch_kr-0.1.3/lightswitch/models.py
--rw-r--r--   0        0        0     1906 2024-05-14 07:02:02.552428 lightswitch_kr-0.1.3/lightswitch/stream_manager.py
--rw-r--r--   0        0        0      617 2024-05-14 07:01:59.092132 lightswitch_kr-0.1.3/lightswitch/utils.py
--rw-r--r--   0        0        0      901 2024-05-16 06:25:53.411646 lightswitch_kr-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-16 05:46:46.226828 lightswitch_kr-0.1.3/README.md
--rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 lightswitch_kr-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      261 2024-05-16 05:15:34.000000 lightswitch_kr-0.1.4/lightswitch/__init__.py
+-rw-r--r--   0        0        0     3103 2024-05-14 07:02:03.000000 lightswitch_kr-0.1.4/lightswitch/custom_sseclient.py
+-rw-r--r--   0        0        0     1587 2024-05-13 01:44:03.000000 lightswitch_kr-0.1.4/lightswitch/exceptions.py
+-rw-r--r--   0        0        0     9789 2024-05-16 15:04:53.472909 lightswitch_kr-0.1.4/lightswitch/lightswitch.py
+-rw-r--r--   0        0        0     6390 2024-05-16 15:21:18.536137 lightswitch_kr-0.1.4/lightswitch/models.py
+-rw-r--r--   0        0        0     1904 2024-05-16 15:03:55.453083 lightswitch_kr-0.1.4/lightswitch/stream_manager.py
+-rw-r--r--   0        0        0      617 2024-05-14 07:01:59.000000 lightswitch_kr-0.1.4/lightswitch/utils.py
+-rw-r--r--   0        0        0      901 2024-05-17 06:37:43.624970 lightswitch_kr-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-16 05:46:46.000000 lightswitch_kr-0.1.4/README.md
+-rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 lightswitch_kr-0.1.4/PKG-INFO
```

### Comparing `lightswitch_kr-0.1.3/lightswitch/custom_sseclient.py` & `lightswitch_kr-0.1.4/lightswitch/custom_sseclient.py`

 * *Files identical despite different names*

### Comparing `lightswitch_kr-0.1.3/lightswitch/exceptions.py` & `lightswitch_kr-0.1.4/lightswitch/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightswitch_kr-0.1.3/lightswitch/lightswitch.py` & `lightswitch_kr-0.1.4/lightswitch/lightswitch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 import typing
 
 
 import requests
 from requests.adapters import HTTPAdapter
 from urllib3 import Retry
-from .models import Flags, Flag, LSUser
-from .stream_manager import StreamManager, StreamEvent
-from .exceptions import StreamDataError, LSServerError, LSTypeCastError, LSFlagNotFoundError
+from models import Flags, Flag, LSUser
+from stream_manager import StreamManager, StreamEvent
+from exceptions import StreamDataError, LSServerError, LSTypeCastError, LSFlagNotFoundError
 
 
 DEFAULT_API_URL = 'http://localhost:8000/api/v1/'
 DEFAULT_REALTIME_API_URL = 'http://localhost:8000/api/v1/sse/subscribe'
 JsonType = typing.Union[
     None,
     int,
@@ -131,17 +131,18 @@
             elif event_type == "SWITCH":
                 self.toggle_flag(new_flag_data)
 
             else:
                 self.delete_flag(new_flag_data['title'])
 
         except json.JSONDecodeError as e:
-            raise StreamDataError(
-                "new_stream_event로부터 유효한 json 데이터를 가져오는데 실패하였습니다."
-            ) from e
+            pass
+            # raise StreamDataError(
+            #     "new_stream_event로부터 유효한 json 데이터를 가져오는데 실패하였습니다."
+            # ) from e
 
     def add_flag(self, new_flag: Flag):
         if self.flags is None:
             self.flags = Flags()
         self.flags.add_flag(new_flag)
 
     def update_flag(self, title, new_data):
```

### Comparing `lightswitch_kr-0.1.3/lightswitch/models.py` & `lightswitch_kr-0.1.4/lightswitch/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import json
 import typing
 from dataclasses import dataclass, field
 
-from .exceptions import LSFlagNotFoundError
-from .utils import get_hashed_percentage_for_object_ids
+from exceptions import LSFlagNotFoundError
+from utils import get_hashed_percentage_for_object_ids
 
 
 # 데이터 모델 정의
 @dataclass
 class LSUser:
     user_id: str
     property: typing.Dict[str, str] = field(default_factory=dict)
@@ -91,31 +91,31 @@
             limit = start_percentage + portion
             if start_percentage <= user_percentile < limit:
                 value = self.convert_value(context['value'])
                 return value
 
             start_percentage = limit
 
-        return self.default_value
+        return self.convert_value(self.default_value)
 
     def convert_value(self, value: str) -> typing.Any:
         """
         value를 flag 타입에 따라 적절한 데이터 타입으로 변환하여 반환합니다.
         """
         if self.type == "BOOLEAN":
-            return bool(value)
+            return value.upper() == "TRUE"
         if self.type == "INTEGER":
             return int(value)
         if self.type == "JSON":
             try:
                 return json.loads(value)
             except json.JSONDecodeError:
                 return value
         if self.type == "STRING":
-            return str(value)
+            return self
         return value
 
     @classmethod
     def flag_from_api(
             cls,
             flag_data: typing.Mapping[str, typing.Any]
     ) -> Flag:
```

### Comparing `lightswitch_kr-0.1.3/lightswitch/stream_manager.py` & `lightswitch_kr-0.1.4/lightswitch/stream_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 import threading
 import typing
 from typing import Callable, Optional, Protocol
 
 import requests
 
-from .custom_sseclient import CustomSSEClient
-from .exceptions import StreamDataError
+from custom_sseclient import CustomSSEClient
+from exceptions import StreamDataError
 
 logger = logging.getLogger(__name__)
 
 
 class StreamEvent(Protocol):
     data: str
```

### Comparing `lightswitch_kr-0.1.3/lightswitch/utils.py` & `lightswitch_kr-0.1.4/lightswitch/utils.py`

 * *Files identical despite different names*

### Comparing `lightswitch_kr-0.1.3/pyproject.toml` & `lightswitch_kr-0.1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lightswitch_kr"
-version = "0.1.3"
+version = "0.1.4"
 description = "A simple SDK for your API"
 authors = ["sumtuckyi <sumin510@naver.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [
   {include = "lightswitch"},
 ]
```

### Comparing `lightswitch_kr-0.1.3/PKG-INFO` & `lightswitch_kr-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightswitch_kr
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple SDK for your API
 License: MIT
 Author: sumtuckyi
 Author-email: sumin510@naver.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

