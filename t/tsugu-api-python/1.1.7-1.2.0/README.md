# Comparing `tmp/tsugu-api-python-1.1.7.tar.gz` & `tmp/tsugu-api-python-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-api-python-1.1.7.tar", last modified: Thu May 16 04:53:27 2024, max compression
+gzip compressed data, was "tsugu-api-python-1.2.0.tar", last modified: Fri May 17 11:53:53 2024, max compression
```

## Comparing `tsugu-api-python-1.1.7.tar` & `tsugu-api-python-1.2.0.tar`

### file list

```diff
@@ -1,34 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:53:27.536588 tsugu-api-python-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-16 04:53:15.000000 tsugu-api-python-1.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-05-16 04:53:27.532588 tsugu-api-python-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-16 04:53:15.000000 tsugu-api-python-1.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 04:53:27.536588 tsugu-api-python-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-16 04:53:15.000000 tsugu-api-python-1.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:53:27.532588 tsugu-api-python-1.1.7/tsugu_api/
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-16 04:53:15.000000 tsugu-api-python-1.1.7/tsugu_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-16 04:53:15.000000 tsugu-api-python-1.1.7/tsugu_api/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-16 04:53:15.000000 tsugu-api-python-1.1.7/tsugu_api/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-16 04:53:15.000000 tsugu-api-python-1.1.7/tsugu_api/_station.py
--rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-05-16 04:53:15.000000 tsugu-api-python-1.1.7/tsugu_api/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-16 04:53:15.000000 tsugu-api-python-1.1.7/tsugu_api/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-16 04:53:15.000000 tsugu-api-python-1.1.7/tsugu_api/_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-16 04:53:15.000000 tsugu-api-python-1.1.7/tsugu_api/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-16 04:53:15.000000 tsugu-api-python-1.1.7/tsugu_api/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-16 04:53:15.000000 tsugu-api-python-1.1.7/tsugu_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:53:27.532588 tsugu-api-python-1.1.7/tsugu_api_async/
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-16 04:53:15.000000 tsugu-api-python-1.1.7/tsugu_api_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-16 04:53:15.000000 tsugu-api-python-1.1.7/tsugu_api_async/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-16 04:53:15.000000 tsugu-api-python-1.1.7/tsugu_api_async/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-16 04:53:15.000000 tsugu-api-python-1.1.7/tsugu_api_async/_station.py
--rw-r--r--   0 runner    (1001) docker     (127)    11039 2024-05-16 04:53:15.000000 tsugu-api-python-1.1.7/tsugu_api_async/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-16 04:53:15.000000 tsugu-api-python-1.1.7/tsugu_api_async/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-16 04:53:15.000000 tsugu-api-python-1.1.7/tsugu_api_async/_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-16 04:53:15.000000 tsugu-api-python-1.1.7/tsugu_api_async/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-16 04:53:15.000000 tsugu-api-python-1.1.7/tsugu_api_async/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-16 04:53:15.000000 tsugu-api-python-1.1.7/tsugu_api_async/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:53:27.532588 tsugu-api-python-1.1.7/tsugu_api_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-05-16 04:53:27.000000 tsugu-api-python-1.1.7/tsugu_api_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-16 04:53:27.000000 tsugu-api-python-1.1.7/tsugu_api_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 04:53:27.000000 tsugu-api-python-1.1.7/tsugu_api_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 04:53:27.000000 tsugu-api-python-1.1.7/tsugu_api_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-16 04:53:27.000000 tsugu-api-python-1.1.7/tsugu_api_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:53:53.392543 tsugu-api-python-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-17 11:53:44.000000 tsugu-api-python-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-05-17 11:53:53.392543 tsugu-api-python-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-17 11:53:44.000000 tsugu-api-python-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 11:53:53.392543 tsugu-api-python-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-17 11:53:44.000000 tsugu-api-python-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:53:53.388543 tsugu-api-python-1.2.0/tsugu_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-17 11:53:44.000000 tsugu-api-python-1.2.0/tsugu_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-17 11:53:44.000000 tsugu-api-python-1.2.0/tsugu_api/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-17 11:53:44.000000 tsugu-api-python-1.2.0/tsugu_api/_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9448 2024-05-17 11:53:44.000000 tsugu-api-python-1.2.0/tsugu_api/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-17 11:53:44.000000 tsugu-api-python-1.2.0/tsugu_api/_user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:53:53.388543 tsugu-api-python-1.2.0/tsugu_api_async/
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-17 11:53:44.000000 tsugu-api-python-1.2.0/tsugu_api_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-17 11:53:44.000000 tsugu-api-python-1.2.0/tsugu_api_async/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-17 11:53:44.000000 tsugu-api-python-1.2.0/tsugu_api_async/_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11051 2024-05-17 11:53:44.000000 tsugu-api-python-1.2.0/tsugu_api_async/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-17 11:53:44.000000 tsugu-api-python-1.2.0/tsugu_api_async/_user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:53:53.388543 tsugu-api-python-1.2.0/tsugu_api_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-17 11:53:44.000000 tsugu-api-python-1.2.0/tsugu_api_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-05-17 11:53:44.000000 tsugu-api-python-1.2.0/tsugu_api_core/_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-17 11:53:44.000000 tsugu-api-python-1.2.0/tsugu_api_core/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-17 11:53:44.000000 tsugu-api-python-1.2.0/tsugu_api_core/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-17 11:53:44.000000 tsugu-api-python-1.2.0/tsugu_api_core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-17 11:53:44.000000 tsugu-api-python-1.2.0/tsugu_api_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:53:53.388543 tsugu-api-python-1.2.0/tsugu_api_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-05-17 11:53:53.000000 tsugu-api-python-1.2.0/tsugu_api_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-17 11:53:53.000000 tsugu-api-python-1.2.0/tsugu_api_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 11:53:53.000000 tsugu-api-python-1.2.0/tsugu_api_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-17 11:53:53.000000 tsugu-api-python-1.2.0/tsugu_api_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-17 11:53:53.000000 tsugu-api-python-1.2.0/tsugu_api_python.egg-info/top_level.txt
```

### Comparing `tsugu-api-python-1.1.7/LICENSE` & `tsugu-api-python-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.7/PKG-INFO` & `tsugu-api-python-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu-api-python
-Version: 1.1.7
+Version: 1.2.0
 Summary: Tsugu BanGDream Bot 的功能 API 统合包
 Home-page: https://github.com/WindowsSov8forUs/tsugu-api-python
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.1.7 Summary: Tsugu
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.2.0 Summary: Tsugu
 BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
 WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
```

### Comparing `tsugu-api-python-1.1.7/README.md` & `tsugu-api-python-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.7/setup.py` & `tsugu-api-python-1.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu-api-python',
-    version='1.1.7',
+    version='1.2.0',
     author='WindowsSov8',
     author_email='qwertyuiop2333@hotmail.com',
     description='Tsugu BanGDream Bot 的功能 API 统合包',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/WindowsSov8forUs/tsugu-api-python',
     include_package_data=False,
```

### Comparing `tsugu-api-python-1.1.7/tsugu_api/__init__.py` & `tsugu-api-python-1.2.0/tsugu_api/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 '''
 `tsugu_api` 向 Tsugu 后端 API 请求模块
 '''
 
-from . import settings as settings
-from . import utils as utils
+from tsugu_api_core.utils import *
+
+import tsugu_api_core.settings as settings
 
 from ._user import get_user_data as get_user_data
 from ._user import change_user_data as change_user_data
 from ._user import bind_player_request as bind_player_request
 from ._user import bind_player_verification as bind_player_verification
 
 from ._tsugu import ycx as ycx
```

### Comparing `tsugu-api-python-1.1.7/tsugu_api/_bandoristation.py` & `tsugu-api-python-1.2.0/tsugu_api_async/_bandoristation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from typing import List
 
-from tsugu_api import settings
-from tsugu_api._network import Api
-from tsugu_api._typing import _StationRoom
-from tsugu_api.exception import RoomQueryFailure, RoomSubmitFailure
+from httpx import Response
+
+from tsugu_api_core import settings
+from tsugu_api_core._network import Api
+from tsugu_api_core._typing import _StationRoom
+from tsugu_api_core.exception import RoomQueryFailure, RoomSubmitFailure
 
 BANDORI_STATION_URL = 'https://api.bandoristation.com/index.php'
 
-def submit_room_number(number: int, user_id: str, raw_message: str, source: str, token: str) -> None:
+async def submit_room_number(number: int, user_id: str, raw_message: str, source: str, token: str) -> None:
     '''上传房间号
 
     参数:
         number (int): 房间号
         user_id (str): 用户 ID
         raw_message (str): 原始消息，用作房间号注释
         source (str): 房间来源，即令牌名称
@@ -25,34 +27,38 @@
         'user_id': user_id,
         'raw_message': raw_message,
         'source': source,
         'token': token
     }
     
     # 发送请求
-    response = Api(
-        BANDORI_STATION_URL,
-        proxy=settings.backend_proxy
-    ).get(params).json()
+    response = await Api(
+            BANDORI_STATION_URL,
+            proxy=settings.backend_proxy
+    ).aget(params)
+    if isinstance(response, Response): response = response.json()
+    else: response = await response.json()
     if response['status'] == 'failure':
         raise RoomSubmitFailure(response['response'])
 
-def query_room_number() -> List[_StationRoom]:
+async def query_room_number() -> List[_StationRoom]:
     '''获取房间号
 
     返回:
         List[_StationRoom]: 房间信息列表
     '''
     
     # 构建参数
     params = {
         'function': 'query_room_number'
     }
     
     # 发送请求
-    response = Api(
+    response = await Api(
         BANDORI_STATION_URL,
         proxy=settings.backend_proxy
-    ).get(params).json()
+    ).aget(params)
+    if isinstance(response, Response): response = response.json()
+    else: response = await response.json()
     if response['status'] == 'failure':
         raise RoomQueryFailure(response['response'])
     return response['response']
```

### Comparing `tsugu-api-python-1.1.7/tsugu_api/_station.py` & `tsugu-api-python-1.2.0/tsugu_api/_station.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from time import time
 from typing import Optional
 
-from tsugu_api import settings
-from tsugu_api._network import Api
-from tsugu_api._typing import (
+from tsugu_api_core import settings
+from tsugu_api_core._network import Api
+from tsugu_api_core._typing import (
     _QueryResponse,
     _SubmitResponse
 )
 
 def station_submit_room_number(
     number: int,
     raw_message: str,
```

### Comparing `tsugu-api-python-1.1.7/tsugu_api/_tsugu.py` & `tsugu-api-python-1.2.0/tsugu_api/_tsugu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, Optional, Sequence
 
-from tsugu_api import settings
-from tsugu_api._network import Api
-from tsugu_api._typing import (
+from tsugu_api_core import settings
+from tsugu_api_core._network import Api
+from tsugu_api_core._typing import (
     _Room,
     _Server,
     _Response,
     _DifficultyText
 )
 
 def event_stage(server: _Server, event_id: Optional[int] = None, meta: bool = False) -> _Response:
```

### Comparing `tsugu-api-python-1.1.7/tsugu_api/_typing.py` & `tsugu-api-python-1.2.0/tsugu_api_core/_typing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,64 @@
 '''
-`tsugu_api._typing`
+`tsugu_api_core._typing`
 
 定义了一些类型别名
 '''
 
 from typing import (
     Any,
     List,
     Union,
     Literal,
     TypeAlias,
     TypedDict
 )
 from typing_extensions import NotRequired
 
+from httpx import Response
+from aiohttp import ClientResponse
+
+_ApiResponse: TypeAlias = Union[Response, ClientResponse]
+
 _ServerId: TypeAlias = Literal[0, 1, 2, 3, 4]
 '''
 服务器 ID
 
 值:
     0: 日服
     1: 国际服
     2: 台服
     3: 国服
     4: 韩服
 '''
+SERVER_ID = (0, 1, 2, 3, 4)
 _ServerName: TypeAlias = Literal['jp', 'en', 'tw', 'cn', 'kr']
 '''
 服务器名
 
 值:
     'jp': 日服
     'en': 国际服
     'tw': 台服
     'cn': 国服
     'kr': 韩服
 '''
+SERVER_NAME = ('jp', 'en', 'tw', 'cn', 'kr')
 _Server: TypeAlias = Union[_ServerId, _ServerName]
 '''服务器'''
+SERVER = (0, 1, 2, 3, 4, 'jp', 'en', 'tw', 'cn', 'kr')
+
+def is_server(server: Any) -> bool:
+    return server in SERVER
+
+def is_server_list(server_list: List[Any]) -> bool:
+    for server in server_list:
+        if not is_server(server):
+            return False
+    return True
 
 class _Data(TypedDict):
     '''API 单个响应数据'''
     type: Literal['string', 'base64']
     string: str
 
 _Response: TypeAlias = List[_Data]
@@ -64,15 +81,15 @@
 class _Room(TypedDict):
     '''房间数据'''
     number: int
     rawMessage: str
     source: str
     userId: str
     time: int
-    player: _Player
+    player: NotRequired[_Player]
     avanter: NotRequired[str]
     userName: NotRequired[str]
 
 class _QueryResponse(TypedDict):
     '''`/station/queryAllRoom` 响应结果'''
     status: _Status
     data: Union[str, List[_Room]]
```

### Comparing `tsugu-api-python-1.1.7/tsugu_api/_user.py` & `tsugu-api-python-1.2.0/tsugu_api/_user.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-from typing import Union
-
-from tsugu_api import settings
-from tsugu_api._network import Api
-from tsugu_api._typing import (
+from tsugu_api_core import settings
+from tsugu_api_core._network import Api
+from tsugu_api_core._typing import (
     _Update,
     _ServerId,
     _GetUserDataResponse,
     _ChangeUserDataResponse,
     _BindPlayerRequestResponse,
     _BindPlayerVerificationResponse
 )
```

### Comparing `tsugu-api-python-1.1.7/tsugu_api/settings.py` & `tsugu-api-python-1.2.0/tsugu_api_core/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 '''对 tsugu_api 进行配置'''
 
+from enum import Enum
 from typing import Optional
 
+class Client(str, Enum):
+    HTTPX = 'httpx'
+    '''使用 `httpx`'''
+    AIO_HTTP = 'aiohttp'
+    '''使用 `aiohttp`'''
+
+client: Client = Client.HTTPX
+'''使用的 HTTP 客户端'''
+
 timeout: int = 10
 '''请求超时时间'''
 
 proxy: str = ''
 '''代理地址'''
 
 backend_url: str = 'http://tsugubot.com:8080'
@@ -50,15 +60,15 @@
 compress: bool = True
 '''
 是否压缩返回数据，压缩可减少返回数据大小。
 
 默认为 True，即压缩返回数据。若不压缩返回数据，可将此项设置为 False。
 '''
 
-def _get_proxy() -> Optional[dict[str, str]]:
+def _get_proxies() -> Optional[dict[str, str]]:
     global proxy
     
     if proxy == '':
         return None
     return {
         'http://': proxy,
         'https://': proxy
```

### Comparing `tsugu-api-python-1.1.7/tsugu_api_async/__init__.py` & `tsugu-api-python-1.2.0/tsugu_api_async/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 '''
 `tsugu_api` 向 Tsugu 后端 API 请求模块
 '''
 
-from . import settings as settings
-from . import utils as utils
+from tsugu_api_core.utils import *
+
+import tsugu_api_core.settings as settings
 
 from ._user import get_user_data as get_user_data
 from ._user import change_user_data as change_user_data
 from ._user import bind_player_request as bind_player_request
 from ._user import bind_player_verification as bind_player_verification
 
 from ._tsugu import ycx as ycx
```

### Comparing `tsugu-api-python-1.1.7/tsugu_api_async/_bandoristation.py` & `tsugu-api-python-1.2.0/tsugu_api/_bandoristation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from typing import List
 
-from httpx import Response
-
-from tsugu_api_async import settings
-from tsugu_api_async._network import Api
-from tsugu_api_async._typing import _StationRoom
-from tsugu_api_async.exception import RoomQueryFailure, RoomSubmitFailure
+from tsugu_api_core import settings
+from tsugu_api_core._network import Api
+from tsugu_api_core._typing import _StationRoom
+from tsugu_api_core.exception import RoomQueryFailure, RoomSubmitFailure
 
 BANDORI_STATION_URL = 'https://api.bandoristation.com/index.php'
 
-async def submit_room_number(number: int, user_id: str, raw_message: str, source: str, token: str) -> None:
+def submit_room_number(number: int, user_id: str, raw_message: str, source: str, token: str) -> None:
     '''上传房间号
 
     参数:
         number (int): 房间号
         user_id (str): 用户 ID
         raw_message (str): 原始消息，用作房间号注释
         source (str): 房间来源，即令牌名称
@@ -27,38 +25,34 @@
         'user_id': user_id,
         'raw_message': raw_message,
         'source': source,
         'token': token
     }
     
     # 发送请求
-    response = await Api(
-            BANDORI_STATION_URL,
-            proxy=settings.backend_proxy
-    ).get(params)
-    if isinstance(response, Response): response = response.json()
-    else: response = await response.json()
+    response = Api(
+        BANDORI_STATION_URL,
+        proxy=settings.backend_proxy
+    ).get(params).json()
     if response['status'] == 'failure':
         raise RoomSubmitFailure(response['response'])
 
-async def query_room_number() -> List[_StationRoom]:
+def query_room_number() -> List[_StationRoom]:
     '''获取房间号
 
     返回:
         List[_StationRoom]: 房间信息列表
     '''
     
     # 构建参数
     params = {
         'function': 'query_room_number'
     }
     
     # 发送请求
-    response = await Api(
+    response = Api(
         BANDORI_STATION_URL,
         proxy=settings.backend_proxy
-    ).get(params)
-    if isinstance(response, Response): response = response.json()
-    else: response = await response.json()
+    ).get(params).json()
     if response['status'] == 'failure':
         raise RoomQueryFailure(response['response'])
     return response['response']
```

### Comparing `tsugu-api-python-1.1.7/tsugu_api_async/_network.py` & `tsugu-api-python-1.2.0/tsugu_api_core/_network.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''`tsugu_api_async._network`
 
 向 Tsugu 后端发送请求相关模块'''
 from json import dumps
 from typing import Any, Literal, Optional, cast
 
 from aiohttp import ClientSession
-from httpx import Request, Response, AsyncClient, HTTPStatusError
+from httpx import Client, Request, Response, AsyncClient, HTTPStatusError
 
 from . import settings
 from ._typing import _ApiResponse
 
 # 向后端发送 API 请求类
 class Api:
     '''向后端发送 API 请求类
@@ -29,22 +29,22 @@
     ) -> None:
         '''初始化'''
         self.url = url
         self.proxy = proxy
         return
     
     # 请求发送
-    async def _request(
+    async def _arequest(
         self,
         method: Literal['get', 'post'],
         *,
         params: Optional[dict[str, Any]]=None,
         data: Optional[dict[str, Any]]=None
     ) -> _ApiResponse:
-        '''请求发送
+        '''异步请求发送
 
         参数:
             method (Literal[&#39;get&#39;, &#39;post&#39;]): API 调用方法
             params (Optional[dict[str, Any]]): 请求的参数
             data (Optional[dict[str, Any]]): 请求的数据
 
         返回:
@@ -54,15 +54,15 @@
         if method == 'post':
             headers = {'Content-Type': 'application/json'}
         else:
             headers = None
         
         # 构建代理服务器字典
         if self.proxy:
-            proxies = settings._get_proxy()
+            proxies = settings._get_proxies()
         else:
             proxies = None
         
         # 发送请求并获取响应
         if settings.client == settings.Client.HTTPX:
             async with AsyncClient(proxies=cast(dict, proxies), timeout=settings.timeout, trust_env=False) as client:
                 # 构建一个请求体
@@ -98,28 +98,103 @@
         else:
             if response.status == 400:
                 return response
             else:
                 response.raise_for_status()
         return response
     
-    async def post(self, data: Optional[dict[str, Any]]=None) -> _ApiResponse:
-        '''发送 POST 请求
+    async def apost(self, data: Optional[dict[str, Any]]=None) -> _ApiResponse:
+        '''异步发送 POST 请求
 
         参数:
             data (Optional[dict[str, Any]]): 请求的数据
 
         返回:
             _ApiResponse: 收到的响应
         '''
-        return await self._request('post', data=data)
+        return await self._arequest('post', data=data)
     
-    async def get(self, params: Optional[dict[str, Any]]=None) -> _ApiResponse:
-        '''发送 GET 请求
+    async def aget(self, params: Optional[dict[str, Any]]=None) -> _ApiResponse:
+        '''异步发送 GET 请求
 
         参数:
             params (Optional[dict[str, Any]]): 请求的参数
 
         返回:
             _ApiResponse: 收到的响应
         '''
-        return await self._request('get', params=params)
+        return await self._arequest('get', params=params)
+
+    # 请求发送
+    def _request(
+        self,
+        method: Literal['get', 'post'],
+        *,
+        params: Optional[dict[str, Any]]=None,
+        data: Optional[dict[str, Any]]=None
+    ) -> Response:
+        '''请求发送
+
+        参数:
+            method (Literal[&#39;get&#39;, &#39;post&#39;]): API 调用方法
+            params (Optional[dict[str, Any]]): 请求的参数
+            data (Optional[dict[str, Any]]): 请求的数据
+
+        返回:
+            Response: 收到的响应
+        '''
+        # 构建请求头
+        if method == 'post':
+            headers = {'Content-Type': 'application/json'}
+        else:
+            headers = None
+        
+        # 构建一个请求体
+        request = Request(
+            method,
+            self.url,
+            params=params,
+            data=cast(dict, dumps(data)) if data is not None else data,
+            headers=headers
+        )
+        
+        # 构建代理服务器字典
+        if self.proxy:
+            proxies = settings._get_proxies()
+        else:
+            proxies = None
+        
+        # 发送请求并获取响应
+        with Client(proxies=cast(dict, proxies), timeout=settings.timeout, trust_env=False) as client:
+            response = client.send(request)
+        
+        # 处理接收到的响应
+        try:
+            response.raise_for_status()
+        except HTTPStatusError as exception:
+            if exception.response.status_code == 400:
+                return response
+            else:
+                raise exception
+        return response
+    
+    def post(self, data: Optional[dict[str, Any]]=None) -> Response:
+        '''发送 POST 请求
+
+        参数:
+            data (Optional[dict[str, Any]]): 请求的数据
+
+        返回:
+            Response: 收到的响应
+        '''
+        return self._request('post', data=data)
+    
+    def get(self, params: Optional[dict[str, Any]]=None) -> Response:
+        '''发送 GET 请求
+
+        参数:
+            params (Optional[dict[str, Any]]): 请求的参数
+
+        返回:
+            Response: 收到的响应
+        '''
+        return self._request('get', params=params)
```

### Comparing `tsugu-api-python-1.1.7/tsugu_api_async/_station.py` & `tsugu-api-python-1.2.0/tsugu_api_async/_station.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from time import time
 from typing import Optional
 
 from httpx import Response
 
-from tsugu_api_async import settings
-from tsugu_api_async._network import Api
-from tsugu_api_async._typing import (
+from tsugu_api_core import settings
+from tsugu_api_core._network import Api
+from tsugu_api_core._typing import (
     _QueryResponse,
     _SubmitResponse
 )
 
 async def station_submit_room_number(
     number: int,
     raw_message: str,
@@ -47,15 +47,15 @@
     if bandori_station_token:
         data['bandoriStationToken'] = bandori_station_token
     
     # 发送请求
     resonse = await Api(
         url,
         proxy=settings.userdata_backend_proxy
-    ).post(data)
+    ).apost(data)
     if isinstance(resonse, Response): return resonse.json()
     return await resonse.json()
 
 async def station_query_all_room() -> _QueryResponse:
     '''查询最近车站车牌
 
     返回:
@@ -65,10 +65,10 @@
     # 构建 URL
     url = settings.userdata_backend_url + '/station/queryAllRoom'
     
     # 发送请求
     response = await Api(
         url,
         proxy=settings.userdata_backend_proxy
-    ).get()
+    ).aget()
     if isinstance(response, Response): return response.json()
     return await response.json()
```

### Comparing `tsugu-api-python-1.1.7/tsugu_api_async/_tsugu.py` & `tsugu-api-python-1.2.0/tsugu_api_async/_tsugu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List, Optional, Sequence
 
 from httpx import Response
 
-from tsugu_api_async import settings
-from tsugu_api_async._network import Api
-from tsugu_api_async._typing import (
+from tsugu_api_core import settings
+from tsugu_api_core._network import Api
+from tsugu_api_core._typing import (
     _Room,
     _Server,
     _Response,
     _DifficultyText
 )
 
 async def event_stage(server: _Server, event_id: Optional[int] = None, meta: bool = False) -> _Response:
@@ -35,15 +35,15 @@
     if event_id:
         data['eventId'] = event_id
     
     # 发送请求
     response = await Api(
         url,
         proxy=settings.backend_proxy
-    ).post(data)
+    ).apost(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
 async def gacha_simulate(server_mode: _Server, times: Optional[int] = None, gacha_id: Optional[int] = None) -> _Response:
     '''模拟抽卡
 
     参数:
@@ -68,15 +68,15 @@
     if gacha_id:
         data['gachaId'] = gacha_id
     
     # 发送请求
     response = await Api(
         url,
         proxy=settings.backend_proxy
-    ).post(data)
+    ).apost(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
 async def get_card_illustration(card_id: int) -> _Response:
     '''获取卡面
 
     参数:
@@ -94,15 +94,15 @@
         'cardId': str(card_id)
     }
     
     # 发送请求
     response = await Api(
         url,
         proxy=settings.backend_proxy
-    ).post(data)
+    ).apost(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
 async def lsycx(server: _Server, tier: int, event_id: Optional[int] = None) -> _Response:
     '''查询历史排行榜预测线
 
     参数:
@@ -126,15 +126,15 @@
     if event_id:
         data['eventId'] = event_id
     
     # 发送请求
     response = await Api(
         url,
         proxy=settings.backend_proxy
-    ).post(data)
+    ).apost(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
 async def room_list(room_list: List[_Room]) -> _Response:
     '''绘制车牌绘图
 
     参数:
@@ -153,15 +153,15 @@
         'compress': settings.compress
     }
     
     # 发送请求
     response = await Api(
         url,
         proxy=settings.backend_proxy
-    ).post(data)
+    ).apost(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
 async def search_card(default_servers: Sequence[_Server], text: str) -> _Response:
     '''查询卡片
 
     参数:
@@ -183,15 +183,15 @@
         'compress': settings.compress
     }
     
     # 发送请求
     response = await Api(
         url,
         proxy=settings.backend_proxy
-    ).post(data)
+    ).apost(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
 async def search_character(default_servers: Sequence[_Server], text: str) -> _Response:
     '''查询角色
 
     参数:
@@ -212,15 +212,15 @@
         'compress': settings.compress
     }
     
     # 发送请求
     response = await Api(
         url,
         proxy=settings.backend_proxy
-    ).post(data)
+    ).apost(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
 async def search_event(default_servers: Sequence[_Server], text: str) -> _Response:
     '''查询活动
 
     参数:
@@ -242,15 +242,15 @@
         'compress': settings.compress
     }
     
     # 发送请求
     response = await Api(
         url,
         proxy=settings.backend_proxy
-    ).post(data)
+    ).apost(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
 async def search_gacha(default_servers: Sequence[_Server], gacha_id: int) -> _Response:
     '''查询卡池
 
     参数:
@@ -272,15 +272,15 @@
         'compress': settings.compress
     }
     
     # 发送请求
     response = await Api(
         url,
         proxy=settings.backend_proxy
-    ).post(data)
+    ).apost(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
 async def search_player(player_id: int, server: _Server) -> _Response:
     '''查询玩家状态
 
     参数:
@@ -302,15 +302,15 @@
         'compress': settings.compress
     }
     
     # 发送请求
     response = await Api(
         url,
         proxy=settings.backend_proxy
-    ).post(data)
+    ).apost(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
 async def search_song(default_servers: Sequence[_Server], text: str) -> _Response:
     '''查询歌曲
 
     参数:
@@ -331,15 +331,15 @@
         'compress': settings.compress
     }
     
     # 发送请求
     response = await Api(
         url,
         proxy=settings.backend_proxy
-    ).post(data)
+    ).apost(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
 async def song_chart(default_servers: Sequence[_Server], song_id: int, difficulty_text: _DifficultyText) -> _Response:
     '''查询歌曲谱面
 
     参数:
@@ -362,15 +362,15 @@
         'compress': settings.compress
     }
     
     # 发送请求
     response = await Api(
         url,
         proxy=settings.backend_proxy
-    ).post(data)
+    ).apost(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
 async def song_meta(default_servers: Sequence[_Server], server: _Server) -> _Response:
     '''查询歌曲分数表
 
     参数:
@@ -391,15 +391,15 @@
         'compress': settings.compress
     }
     
     # 发送请求
     response = await Api(
         url,
         proxy=settings.backend_proxy
-    ).post(data)
+    ).apost(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
 async def ycx(server: _Server, tier: int, event_id: Optional[int] = None) -> _Response:
     '''查询排行榜预测线
 
     参数:
@@ -423,15 +423,15 @@
     if event_id:
         data['eventId'] = event_id
     
     # 发送请求
     response = await Api(
         url,
         proxy=settings.backend_proxy
-    ).post(data)
+    ).apost(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
 async def ycx_all(server: _Server, event_id: Optional[int] = None) -> _Response:
     '''查询全挡位预测线
 
     参数:
@@ -453,10 +453,10 @@
     if event_id:
         data['eventId'] = event_id
     
     # 发送请求
     response = await Api(
         url,
         proxy=settings.backend_proxy
-    ).post(data)
+    ).apost(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
```

### Comparing `tsugu-api-python-1.1.7/tsugu_api_async/_user.py` & `tsugu-api-python-1.2.0/tsugu_api_async/_user.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-from typing import Union
-
 from httpx import Response
 
-from tsugu_api_async import settings
-from tsugu_api_async._network import Api
-from tsugu_api_async._typing import (
+from tsugu_api_core import settings
+from tsugu_api_core._network import Api
+from tsugu_api_core._typing import (
     _Update,
     _ServerId,
     _GetUserDataResponse,
     _ChangeUserDataResponse,
     _BindPlayerRequestResponse,
     _BindPlayerVerificationResponse
 )
@@ -33,15 +31,15 @@
         'user_id': user_id
     }
     
     # 发送请求
     response = await Api(
         url,
         proxy=settings.userdata_backend_proxy
-    ).post(data)
+    ).apost(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
 async def change_user_data(platform: str, user_id: str, update: _Update) -> _ChangeUserDataResponse:
     '''修改用户数据
 
     参数:
@@ -63,15 +61,15 @@
         'update': update
     }
     
     # 发送请求
     response = await Api(
         url,
         proxy=settings.userdata_backend_proxy
-    ).post(data)
+    ).apost(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
 async def bind_player_request(
     platform: str,
     user_id: str,
     server: _ServerId,
@@ -100,15 +98,15 @@
         'bindType': bind_type
     }
     
     # 发送请求
     response = await Api(
         url,
         proxy=settings.userdata_backend_proxy
-    ).post(data)
+    ).apost(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
 async def bind_player_verification(
     platform: str,
     user_id: str,
     server: _ServerId,
@@ -140,10 +138,10 @@
         'bindType': bind_type
     }
     
     # 发送请求
     response = await Api(
         url,
         proxy=settings.userdata_backend_proxy
-    ).post(data)
+    ).apost(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
```

### Comparing `tsugu-api-python-1.1.7/tsugu_api_python.egg-info/PKG-INFO` & `tsugu-api-python-1.2.0/tsugu_api_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu-api-python
-Version: 1.1.7
+Version: 1.2.0
 Summary: Tsugu BanGDream Bot 的功能 API 统合包
 Home-page: https://github.com/WindowsSov8forUs/tsugu-api-python
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.1.7 Summary: Tsugu
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.2.0 Summary: Tsugu
 BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
 WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
```

### Comparing `tsugu-api-python-1.1.7/tsugu_api_python.egg-info/SOURCES.txt` & `tsugu-api-python-1.2.0/tsugu_api_python.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 LICENSE
 README.md
 setup.py
 tsugu_api/__init__.py
 tsugu_api/_bandoristation.py
-tsugu_api/_network.py
 tsugu_api/_station.py
 tsugu_api/_tsugu.py
-tsugu_api/_typing.py
 tsugu_api/_user.py
-tsugu_api/exception.py
-tsugu_api/settings.py
-tsugu_api/utils.py
 tsugu_api_async/__init__.py
 tsugu_api_async/_bandoristation.py
-tsugu_api_async/_network.py
 tsugu_api_async/_station.py
 tsugu_api_async/_tsugu.py
-tsugu_api_async/_typing.py
 tsugu_api_async/_user.py
-tsugu_api_async/exception.py
-tsugu_api_async/settings.py
-tsugu_api_async/utils.py
+tsugu_api_core/__init__.py
+tsugu_api_core/_network.py
+tsugu_api_core/_typing.py
+tsugu_api_core/exception.py
+tsugu_api_core/settings.py
+tsugu_api_core/utils.py
 tsugu_api_python.egg-info/PKG-INFO
 tsugu_api_python.egg-info/SOURCES.txt
 tsugu_api_python.egg-info/dependency_links.txt
 tsugu_api_python.egg-info/requires.txt
 tsugu_api_python.egg-info/top_level.txt
```

