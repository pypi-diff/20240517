# Comparing `tmp/bestdori-api-1.1.1.tar.gz` & `tmp/bestdori-api-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bestdori-api-1.1.1.tar", last modified: Mon May 13 02:53:51 2024, max compression
+gzip compressed data, was "bestdori-api-1.1.2.tar", last modified: Fri May 17 16:32:22 2024, max compression
```

## Comparing `bestdori-api-1.1.1.tar` & `bestdori-api-1.1.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:53:51.322723 bestdori-api-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-05-13 02:53:51.322723 bestdori-api-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:53:51.318723 bestdori-api-1.1.1/bestdori/
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:53:51.318723 bestdori-api-1.1.1/bestdori/ayachan/
--rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/ayachan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/ayachan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:53:51.318723 bestdori-api-1.1.1/bestdori/ayachan/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/ayachan/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/ayachan/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/ayachan/utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/ayachan/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/cards.py
--rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/characters.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/charts.py
--rw-r--r--   0 runner    (1001) docker     (127)    12237 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/comics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12181 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/costumes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/eventarchives.py
--rw-r--r--   0 runner    (1001) docker     (127)    22526 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/festival.py
--rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/logincampaigns.py
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/miracleticket.py
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/missions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:53:51.322723 bestdori-api-1.1.1/bestdori/models/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/models/content.py
--rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/models/note.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/player.py
--rw-r--r--   0 runner    (1001) docker     (127)    34492 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/songmeta.py
--rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/songs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)    13044 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:53:51.322723 bestdori-api-1.1.1/bestdori/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22155 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/bestdori/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:53:51.322723 bestdori-api-1.1.1/bestdori_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-05-13 02:53:51.000000 bestdori-api-1.1.1/bestdori_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-13 02:53:51.000000 bestdori-api-1.1.1/bestdori_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 02:53:51.000000 bestdori-api-1.1.1/bestdori_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-13 02:53:51.000000 bestdori-api-1.1.1/bestdori_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-13 02:53:51.000000 bestdori-api-1.1.1/bestdori_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 02:53:51.322723 bestdori-api-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-13 02:53:41.000000 bestdori-api-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:32:22.686246 bestdori-api-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-05-17 16:32:22.686246 bestdori-api-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:32:22.682246 bestdori-api-1.1.2/bestdori/
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:32:22.682246 bestdori-api-1.1.2/bestdori/ayachan/
+-rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/ayachan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/ayachan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:32:22.682246 bestdori-api-1.1.2/bestdori/ayachan/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/ayachan/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/ayachan/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/ayachan/utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/ayachan/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16502 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/cards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/characters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/comics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12187 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/costumes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/eventarchives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22538 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9313 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/festival.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12819 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/logincampaigns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/miracleticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/missions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:32:22.686246 bestdori-api-1.1.2/bestdori/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/models/content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/models/note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34540 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/songmeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11231 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/songs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13050 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:32:22.686246 bestdori-api-1.1.2/bestdori/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22168 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/bestdori/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:32:22.686246 bestdori-api-1.1.2/bestdori_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-05-17 16:32:22.000000 bestdori-api-1.1.2/bestdori_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-17 16:32:22.000000 bestdori-api-1.1.2/bestdori_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 16:32:22.000000 bestdori-api-1.1.2/bestdori_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-17 16:32:22.000000 bestdori-api-1.1.2/bestdori_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 16:32:22.000000 bestdori-api-1.1.2/bestdori_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 16:32:22.686246 bestdori-api-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-17 16:32:13.000000 bestdori-api-1.1.2/setup.py
```

### Comparing `bestdori-api-1.1.1/LICENSE` & `bestdori-api-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.1/PKG-INFO` & `bestdori-api-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bestdori-api
-Version: 1.1.1
+Version: 1.1.2
 Summary: Bestdori 的各种 API 调用整合，另外附带部分功能
 Home-page: https://github.com/WindowsSov8forUs/bestdori-api
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bestdori-api Version: 1.1.1 Summary: Bestdori
+Metadata-Version: 2.1 Name: bestdori-api Version: 1.1.2 Summary: Bestdori
 çåç§ API è°ç¨æ´åï¼å¦å¤éå¸¦é¨ååè½ Home-page: https://
 github.com/WindowsSov8forUs/bestdori-api Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
   ![bestdori-api logo](https://github.com/WindowsSov8forUs/bestdori-api/blob/
 main/logo.png) # Bestdori-api _â¨ [Bestdori](https://bestdori.com/) çåç§
          API è°ç¨æ´åï¼å¦å¤éå¸¦é¨ååè½ â¨_ **:warning:
         è¯¥é¡¹ç®ä»ç¶æ¥éæ´æ°ä¸ Debug ï¼ä½¿ç¨æ¶è¥éå° Bug
```

### Comparing `bestdori-api-1.1.1/README.md` & `bestdori-api-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.1/bestdori/__init__.py` & `bestdori-api-1.1.2/bestdori/__init__.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.1/bestdori/ayachan/__init__.py` & `bestdori-api-1.1.2/bestdori/ayachan/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,105 +1,105 @@
 '''`bestdori.ayachan`
 
 ayachan 的各种 API 调用整合'''
 from pathlib import Path
 from mimetypes import guess_type
-from typing import Any, Union, Literal
+from typing import Any, Dict, Union, Literal
 
 from httpx import Response
 
 from .utils import API, Api
 from bestdori.charts import Chart
 from .exceptions import SonolusException
 
 DIFF_STR = ['easy', 'normal', 'hard', 'expert', 'special']
 
 # 自定义谱面分析
-def chart_metrics_custom(chart: Chart, diff: Literal[0, 1, 2, 3, 4]) -> dict[str, Any]:
+def chart_metrics_custom(chart: Chart, diff: Literal[0, 1, 2, 3, 4]) -> Dict[str, Any]:
     '''自定义谱面分析
 
     参数:
         chart (Chart): 谱面
         diff (Literal[0, 1, 2, 3, 4]): 难度类型
 
     返回:
-        dict[str, Any]: 分析结果
+        Dict[str, Any]: 分析结果
     '''
     return Api(API['chart_metrics']['custom'].format(diff_str=DIFF_STR[diff])).post(data=chart.to_list()).json()
 
 # 异步自定义谱面分析
-async def chart_metrics_custom_async(chart: Chart, diff: Literal[0, 1, 2, 3, 4]) -> dict[str, Any]:
+async def chart_metrics_custom_async(chart: Chart, diff: Literal[0, 1, 2, 3, 4]) -> Dict[str, Any]:
     '''自定义谱面分析
 
     参数:
         chart (Chart): 谱面
         diff (Literal[0, 1, 2, 3, 4]): 难度类型
 
     返回:
-        dict[str, Any]: 分析结果
+        Dict[str, Any]: 分析结果
     '''
     response = await Api(API['chart_metrics']['custom'].format(diff_str=DIFF_STR[diff])).apost(data=chart.to_list())
     if isinstance(response, Response): return response.json()
     return await response.json()
 
 # BanG Dream 谱面分析
 def chart_metrics_bandori(
     id: int,
     diff: Literal[0, 1, 2, 3, 4]
-) -> dict[str, Any]:
+) -> Dict[str, Any]:
     '''BanG Dream 谱面分析
 
     参数:
         id (int): 歌曲 ID
         diff (Literal[0, 1, 2, 3, 4]): 难度类型
 
     返回:
-        dict[str, Any]: 分析结果
+        Dict[str, Any]: 分析结果
     '''
     return Api(API['chart_metrics']['bandori'].format(chart_id=id, diff_str=DIFF_STR[diff])).get().json()
 
 # 异步 BanG Dream 谱面分析
 async def chart_metrics_bandori_async(
     id: int,
     diff: Literal[0, 1, 2, 3, 4]
-) -> dict[str, Any]:
+) -> Dict[str, Any]:
     '''BanG Dream 谱面分析
 
     参数:
         id (int): 歌曲 ID
         diff (Literal[0, 1, 2, 3, 4]): 难度类型
 
     返回:
-        dict[str, Any]: 分析结果
+        Dict[str, Any]: 分析结果
     '''
     response = await Api(API['chart_metrics']['bandori'].format(chart_id=id, diff_str=DIFF_STR[diff])).aget()
     if isinstance(response, Response): return response.json()
     return await response.json()
 
 # Bestdori 谱面分析
-def chart_metrics_bestdori(id: int) -> dict[str, Any]:
+def chart_metrics_bestdori(id: int) -> Dict[str, Any]:
     '''Bestdori 谱面分析
 
     参数:
         id (int): 谱面 ID
 
     返回:
-        dict[str, Any]: 分析结果
+        Dict[str, Any]: 分析结果
     '''
     return Api(API['chart_metrics']['bestdori'].format(chart_id=id)).get().json()
 
 # 异步 Bestdori 谱面分析
-async def chart_metrics_bestdori_async(id: int) -> dict[str, Any]:
+async def chart_metrics_bestdori_async(id: int) -> Dict[str, Any]:
     '''Bestdori 谱面分析
 
     参数:
         id (int): 谱面 ID
 
     返回:
-        dict[str, Any]: 分析结果
+        Dict[str, Any]: 分析结果
     '''
     response = await Api(API['chart_metrics']['bestdori'].format(chart_id=id)).aget()
     if isinstance(response, Response): return response.json()
     return await response.json()
 
 # Sonolus 谱面测试上传
 def post_sonolus_levels(
@@ -125,15 +125,15 @@
     '''
     # 转换文件路径并获取名称
     if isinstance(bgm, str):
         bgm = Path(bgm)
     bgm_name = bgm.name
     
     # 构建数据
-    data: dict[str, Any] = {
+    data: Dict[str, Any] = {
         'title': title,
         'difficulty': str(difficulty),
         'lifetime': str(lifetime),
         'chart': chart.json()
     }
     if hidden:
         data['hidden'] = True
@@ -175,15 +175,15 @@
     '''
     # 转换文件路径并获取名称
     if isinstance(bgm, str):
         bgm = Path(bgm)
     bgm_name = bgm.name
     
     # 构建数据
-    data: dict[str, Any] = {
+    data: Dict[str, Any] = {
         'title': title,
         'difficulty': str(difficulty),
         'lifetime': str(lifetime),
         'chart': chart.json()
     }
     if hidden:
         data['hidden'] = True
@@ -229,33 +229,33 @@
         Chart: 谱面
     '''
     response = await Api(API['levels']['get'].format(uid=uid)).aget()
     if isinstance(response, Response): return Chart.normalize(response.json())
     return Chart.normalize(await response.json())
 
 # Sonolus 测试服谱面信息获取
-def sonolus_levels(uid: int) -> dict[str, Any]:
+def sonolus_levels(uid: int) -> Dict[str, Any]:
     '''Sonolus 测试服谱面信息获取
 
     参数:
         uid (int): 测试服 ID
 
     返回:
-        dict[str, Any]: 谱面信息
+        Dict[str, Any]: 谱面信息
     '''
     return Api(API['levels']['info'].format(uid=uid)).get().json()
 
 # 异步 Sonolus 测试服谱面信息获取
-async def sonolus_levels_async(uid: int) -> dict[str, Any]:
+async def sonolus_levels_async(uid: int) -> Dict[str, Any]:
     '''Sonolus 测试服谱面信息获取
 
     参数:
         uid (int): 测试服 ID
 
     返回:
-        dict[str, Any]: 谱面信息
+        Dict[str, Any]: 谱面信息
     '''
     response = await Api(API['levels']['info'].format(uid=uid)).aget()
     if isinstance(response, Response): return response.json()
     return await response.json()
 
 from .utils import settings as settings
```

### Comparing `bestdori-api-1.1.1/bestdori/ayachan/utils/network.py` & `bestdori-api-1.1.2/bestdori/ayachan/utils/network.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''`bestdori.ayachan.utils.network`
 
 向 ayachan 发送请求相关模块'''
 from json import dumps
 from io import BufferedReader
-from typing import Any, Union, Literal, Optional, cast
+from typing import Any, Dict, Tuple, Union, Literal, Optional, cast
 
 from httpx import HTTPStatusError
 from aiohttp import ClientResponseError
 from aiohttp import ClientSession, ClientResponse
 from httpx import Client, Request, Response, AsyncClient
 
 from . import settings
@@ -19,15 +19,15 @@
     '''向 ayachan 发送 API 请求类
 
     参数:
         api (str): 请求的 API 地址
     '''
     api: str
     '''请求的 API 地址'''
-    _proxies: Optional[Union[dict[str, str], str]]=None
+    _proxies: Optional[Union[Dict[str, str], str]]=None
     '''代理服务器'''
     # 初始化
     def __init__(
         self,
         api: str
     ) -> None:
         '''初始化'''
@@ -50,26 +50,26 @@
             return _url
     
     # 请求发送
     def _request(
         self,
         method: Literal['get', 'post'],
         *,
-        params: Optional[dict[str, Any]]=None,
+        params: Optional[Dict[str, Any]]=None,
         data: Optional[Any]=None,
-        files: Optional[dict[str, tuple[str, BufferedReader, Optional[str]]]]=None,
+        files: Optional[Dict[str, Tuple[str, BufferedReader, Optional[str]]]]=None,
         json: Optional[Any]=None
     ) -> Response:
         '''请求发送
 
         参数:
             method (Literal[&#39;get&#39;, &#39;post&#39;]): API 调用方法
-            params (Optional[dict[str, Any]], optional): 调用参数
+            params (Optional[Dict[str, Any]], optional): 调用参数
             data (Optional[Any], optional): 调用参数，将以 `json` 字符串形式发送
-            files (Optional[dict[str, tuple[str, BufferedReader, Optional[str]]]], optional): 发送文件参数
+            files (Optional[Dict[str, Tuple[str, BufferedReader, Optional[str]]]], optional): 发送文件参数
             json (Optional[Any], optional): 调用参数，将以 `json` 字符串形式发送
 
         返回:
             Response: 收到的响应
         '''
         # 构建一个请求体
         request = Request(
@@ -98,26 +98,26 @@
         return response
     
     # 异步请求发送
     async def _request_async(
         self,
         method: Literal['get', 'post'],
         *,
-        params: Optional[dict[str, Any]]=None,
+        params: Optional[Dict[str, Any]]=None,
         data: Optional[Any]=None,
-        files: Optional[dict[str, tuple[str, BufferedReader, Optional[str]]]]=None,
+        files: Optional[Dict[str, Tuple[str, BufferedReader, Optional[str]]]]=None,
         json: Optional[Any]=None
     ) -> Union[Response, ClientResponse]:
         '''请求发送
 
         参数:
             method (Literal[&#39;get&#39;, &#39;post&#39;]): API 调用方法
-            params (Optional[dict[str, Any]], optional): 调用参数
+            params (Optional[Dict[str, Any]], optional): 调用参数
             data (Optional[Any], optional): 调用参数，将以 `json` 字符串形式发送
-            files (Optional[dict[str, tuple[str, BufferedReader, Optional[str]]]], optional): 发送文件参数
+            files (Optional[Dict[str, Tuple[str, BufferedReader, Optional[str]]]], optional): 发送文件参数
             json (Optional[Any], optional): 调用参数，将以 `json` 字符串形式发送
 
         返回:
             Response: 收到的响应
         '''
         if settings.async_client == ClientSetting.HTTPX:
             # 构建一个请求体
@@ -164,98 +164,98 @@
                 ) as response:
                     response.raise_for_status()
         
         return response
 
     def get(
         self,
-        params: Optional[dict[str, Any]]=None
+        params: Optional[Dict[str, Any]]=None
     ) -> Response:
         '''发送 GET 请求
 
         参数:
-            params (Optional[dict[str, Any]], optional): 调用参数
+            params (Optional[Dict[str, Any]], optional): 调用参数
 
         返回:
             Response: 收到的响应
         '''
         return self._request('get', params=params)
     
     async def aget(
         self,
-        params: Optional[dict[str, Any]]=None
+        params: Optional[Dict[str, Any]]=None
     ) -> Union[Response, ClientResponse]:
         '''发送 GET 请求
 
         参数:
-            params (Optional[dict[str, Any]], optional): 调用参数
+            params (Optional[Dict[str, Any]], optional): 调用参数
 
         返回:
             Response: 收到的响应
         '''
         return await self._request_async('get', params=params)
     
     def post(
         self,
         data: Optional[Any]=None,
-        files: Optional[dict[str, tuple[str, BufferedReader, Optional[str]]]]=None,
+        files: Optional[Dict[str, Tuple[str, BufferedReader, Optional[str]]]]=None,
         json: Optional[Any]=None
     ) -> Response:
         '''发送 POST 请求
 
         参数:
             data (Optional[Any], optional): 调用参数，将以 `json` 字符串形式发送
-            files (Optional[dict[str, tuple[str, BufferedReader, Optional[str]]]], optional): 发送文件参数
+            files (Optional[Dict[str, Tuple[str, BufferedReader, Optional[str]]]], optional): 发送文件参数
             json (Optional[Any], optional): 调用参数，将以 `json` 字符串形式发送
 
         返回:
             Response: 收到的响应
         '''
         return self._request('post', data=data, files=files, json=json)
     
     async def apost(
         self,
         data: Optional[Any]=None,
-        files: Optional[dict[str, tuple[str, BufferedReader, Optional[str]]]]=None,
+        files: Optional[Dict[str, Tuple[str, BufferedReader, Optional[str]]]]=None,
         json: Optional[Any]=None
     ) -> Union[Response, ClientResponse]:
         '''发送 POST 请求
 
         参数:
             data (Optional[Any], optional): 调用参数，将以 `json` 字符串形式发送
-            files (Optional[dict[str, tuple[str, BufferedReader, Optional[str]]]], optional): 发送文件参数
+            files (Optional[Dict[str, Tuple[str, BufferedReader, Optional[str]]]], optional): 发送文件参数
             json (Optional[Any], optional): 调用参数，将以 `json` 字符串形式发送
 
         返回:
             Response: 收到的响应
         '''
         return await self._request_async('post', data=data, files=files, json=json)
 
 # 获取 ayachan 资源数据
 class Assets:
     '''获取 Bestdori 资源数据
 
     参数:
         url (str): 请求的资源地址
-        proxy (Optional[Union[dict[str, str], str]]): 代理服务器
+        proxy (Optional[Union[Dict[str, str], str]]): 代理服务器
     '''
     url: str
     '''请求的资源地址'''
-    _proxies: Optional[Union[dict[str, str], str]]=None
+    _proxies: Optional[Union[Dict[str, str], str]]=None
     '''代理服务器'''
     # 初始化
     def __init__(
         self,
         url: str
     ) -> None:
         '''获取 Bestdori 资源数据
 
         参数:
             url (str): 请求的资源地址
-            proxy (Optional[Union[dict[str, str], str]]): 代理服务器
+            proxy (Optional[Union[Dict[str, str], str]]): 代理服务器
         '''
         self.url = url
         if isinstance(settings.proxy, str):
             self._proxies = {'http://': settings.proxy, 'https://': settings.proxy}
         elif isinstance(settings.proxy, dict):
             self._proxies = settings.proxy
         return
```

### Comparing `bestdori-api-1.1.1/bestdori/ayachan/utils/utils.py` & `bestdori-api-1.1.2/bestdori/ayachan/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.1/bestdori/cards.py` & `bestdori-api-1.1.2/bestdori/cards.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 '''`bestdori.cards`
 
 BanG Dream! 卡牌相关操作'''
-from typing import Any, Literal
+from typing import Any, Dict, Literal
 
 from aiohttp import ClientResponseError
 from httpx import Response, HTTPStatusError
 
 from .utils.utils import API, RES, ASSETS
 from .post import get_list, get_list_async
 from .utils.network import Api, Res, Assets
 from .exceptions import (
     NoDataException,
     CardNotExistError
 )
 
 # 获取总卡牌信息
-def get_all(index: Literal[0, 5]=5) -> dict[str, dict[str, Any]]:
+def get_all(index: Literal[0, 5]=5) -> Dict[str, Dict[str, Any]]:
     '''获取总卡牌信息
 
     参数:
         index (Literal[0, 5], optional): 指定获取哪种 `all.json`
             `0`: 仅获取所有已有卡牌 ID `all.0.json`
             `5`: 获取所有已有卡牌的简洁信息 `all.5.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总卡牌信息
+        Dict[str, Dict[str, Any]]: 获取到的总卡牌信息
     '''
     return Api(API['cards']['all'].format(index=index)).get().json()
 
 # 异步获取总卡牌信息
-async def get_all_async(index: Literal[0, 5]=5) -> dict[str, dict[str, Any]]:
+async def get_all_async(index: Literal[0, 5]=5) -> Dict[str, Dict[str, Any]]:
     '''获取总卡牌信息
 
     参数:
         index (Literal[0, 5], optional): 指定获取哪种 `all.json`
             `0`: 仅获取所有已有卡牌 ID `all.0.json`
             `5`: 获取所有已有卡牌的简洁信息 `all.5.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总卡牌信息
+        Dict[str, Dict[str, Any]]: 获取到的总卡牌信息
     '''
     response = await Api(API['cards']['all'].format(index=index)).aget()
     
     if isinstance(response, Response):
         return response.json()
     else:
         return await response.json()
@@ -167,15 +167,15 @@
         '''卡牌类
 
         参数:
             id (int): 卡牌 ID
         '''
         self.id: int = id
         '''卡牌 ID'''
-        self.__info: dict[str, Any] = {}
+        self.__info: Dict[str, Any] = {}
         '''卡牌信息存储'''
         return
     
     # 卡牌标题
     @property
     def prefix(self) -> str:
         '''卡牌标题'''
@@ -203,19 +203,19 @@
         elif released_at[2] is not None: return 'tw'
         elif released_at[3] is not None: return 'cn'
         elif released_at[4] is not None: return 'kr'
         else:
             raise NoDataException('卡牌所在服务器')
     
     # 获取卡牌信息
-    def get_info(self) -> dict[str, Any]:
+    def get_info(self) -> Dict[str, Any]:
         '''获取卡牌信息
 
         返回:
-            dict[str, Any]: 卡牌详细信息
+            Dict[str, Any]: 卡牌详细信息
         '''
         try:
             response = Api(
                 API['cards']['info'].format(id=self.id)
             ).get()
         except HTTPStatusError as exception:
             if exception.response.status_code == 404:
@@ -223,19 +223,19 @@
             else:
                 raise exception
         
         self.__info = dict(response.json())
         return self.__info
     
     # 异步获取卡牌信息
-    async def get_info_async(self) -> dict[str, Any]:
+    async def get_info_async(self) -> Dict[str, Any]:
         '''获取卡牌信息
 
         返回:
-            dict[str, Any]: 卡牌详细信息
+            Dict[str, Any]: 卡牌详细信息
         '''
         try:
             response = await Api(
                 API['cards']['info'].format(id=self.id)
             ).aget()
         except HTTPStatusError as exception:
             if exception.response.status_code == 404:
@@ -251,56 +251,56 @@
         if isinstance(response, Response):
             self.__info = dict(response.json())
         else:
             self.__info = dict(await response.json())
         return self.__info
     
     # 获取缓存信息
-    def __get_info_cache(self) -> dict[str, Any]:
+    def __get_info_cache(self) -> Dict[str, Any]:
         '''获取缓存信息
 
         返回:
-            dict[str, Any]: 缓存信息
+            Dict[str, Any]: 缓存信息
         '''
         if not self.__info:
             return self.get_info()
         return self.__info
     
     # 异步获取缓存信息
-    async def __get_info_cache_async(self) -> dict[str, Any]:
+    async def __get_info_cache_async(self) -> Dict[str, Any]:
         '''获取缓存信息
 
         返回:
-            dict[str, Any]: 缓存信息
+            Dict[str, Any]: 缓存信息
         '''
         if not self.__info:
             return await self.get_info_async()
         return self.__info
     
     # 获取卡牌评论
     def get_comment(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取卡牌评论
 
         参数:
             limit (int, optional): 展示出的评论数，默认为 20
             offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
 
         返回:
-            dict[str, Any]: 搜索结果
+            Dict[str, Any]: 搜索结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的评论总数
-                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                    "posts": ... # List[Dict[str, Any]] 列举出的评论
                 }
                 ```
         '''
         return get_list(
             category_name='CARD_COMMENT',
             category_id=str(self.id),
             order=order,
@@ -310,29 +310,29 @@
     
     # 异步获取卡牌评论
     async def get_comment_async(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取卡牌评论
 
         参数:
             limit (int, optional): 展示出的评论数，默认为 20
             offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
 
         返回:
-            dict[str, Any]: 搜索结果
+            Dict[str, Any]: 搜索结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的评论总数
-                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                    "posts": ... # List[Dict[str, Any]] 列举出的评论
                 }
                 ```
         '''
         return await get_list_async(
             category_name='CARD_COMMENT',
             category_id=str(self.id),
             order=order,
```

### Comparing `bestdori-api-1.1.1/bestdori/characters.py` & `bestdori-api-1.1.2/bestdori/characters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 '''`bestdori.characters`
 
 BanG Dream! 角色相关操作'''
-from typing import Any, Literal
+from typing import Any, Dict, Tuple, Literal
 
 from aiohttp import ClientResponseError
 from httpx import Response, HTTPStatusError
 
 from .utils import hexto_rgb
 from .utils.utils import API, RES, ASSETS
 from .post import get_list, get_list_async
 from .utils.network import Api, Res, Assets
 from .exceptions import (
     NoDataException,
     CharacterNotExistError
 )
 
 # 获取总角色信息
-def get_all(index: Literal[2]=2) -> dict[str, dict[str, Any]]:
+def get_all(index: Literal[2]=2) -> Dict[str, Dict[str, Any]]:
     '''获取总角色信息
 
     参数:
         index (Literal[2], optional): 指定获取哪种 `all.json`
             `2`: 获取所有已有角色信息 `all.2.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总角色信息
+        Dict[str, Dict[str, Any]]: 获取到的总角色信息
     '''
     return Api(API['characters']['all'].format(index=index)).get().json()
 
 # 异步获取总角色信息
-async def get_all_async(index: Literal[2]=2) -> dict[str, dict[str, Any]]:
+async def get_all_async(index: Literal[2]=2) -> Dict[str, Dict[str, Any]]:
     '''获取总角色信息
 
     参数:
         index (Literal[2], optional): 指定获取哪种 `all.json`
             `2`: 获取所有已有角色信息 `all.2.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总角色信息
+        Dict[str, Dict[str, Any]]: 获取到的总角色信息
     '''
     response = await Api(API['characters']['all'].format(index=index)).aget()
     if isinstance(response, Response):
         return response.json()
     else:
         return await response.json()
     
 
 # 获取主要角色信息
-def get_main(index: Literal[3]=3) -> dict[str, dict[str, Any]]:
+def get_main(index: Literal[3]=3) -> Dict[str, Dict[str, Any]]:
     '''获取主要角色信息
 
     参数:
         index (Literal[3], optional): 指定获取哪种 `all.json`
             `3`: 获取所有已有主要角色信息 `all.3.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的主要角色信息
+        Dict[str, Dict[str, Any]]: 获取到的主要角色信息
     '''
     return Api(API['characters']['main'].format(index=index)).get().json()
 
 # 异步获取主要角色信息
-async def get_main_async(index: Literal[3]=3) -> dict[str, dict[str, Any]]:
+async def get_main_async(index: Literal[3]=3) -> Dict[str, Dict[str, Any]]:
     '''获取主要角色信息
 
     参数:
         index (Literal[3], optional): 指定获取哪种 `all.json`
             `3`: 获取所有已有主要角色信息 `all.3.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的主要角色信息
+        Dict[str, Dict[str, Any]]: 获取到的主要角色信息
     '''
     response = await Api(API['characters']['main'].format(index=index)).aget()
     if isinstance(response, Response):
         return response.json()
     else:
         return await response.json()
 
@@ -88,15 +88,15 @@
         '''角色类
 
         参数:
             id (int): 角色 ID
         '''
         self.id: int = id
         '''角色 ID'''
-        self.__info: dict[str, Any] = {}
+        self.__info: Dict[str, Any] = {}
         '''角色信息'''
         return
     
     # 角色名称
     @property
     def name(self) -> str:
         '''角色名称'''
@@ -108,32 +108,32 @@
         try:
             return next(filter(lambda x: x is not None, character_name))
         except StopIteration:
             raise NoDataException('角色名称')
     
     # 角色代表色
     @property
-    def color(self) -> tuple[int, int, int]:
+    def color(self) -> Tuple[int, int, int]:
         '''角色代表色'''
         info = self.__info
         # 获取 colorCode 数据
         if (color_code := info.get('colorCode', None)) is None:
             raise NoDataException('角色颜色')
         # 将 colorCode 转换为颜色元组
         try:
             return hexto_rgb(color_code)
         except ValueError:
             raise NoDataException('角色颜色')
     
     # 获取角色信息
-    def get_info(self) -> dict[str, Any]:
+    def get_info(self) -> Dict[str, Any]:
         '''获取角色信息
 
         返回:
-            dict[str, Any]: 角色详细信息
+            Dict[str, Any]: 角色详细信息
         '''
         try:
             response = Api(
                 API['characters']['info'].format(id=self.id)
             ).get()
         except HTTPStatusError as exception:
             if exception.response.status_code == 404:
@@ -141,19 +141,19 @@
             else:
                 raise exception
         
         self.__info = dict(response.json())
         return self.__info
     
     # 异步获取角色信息
-    async def get_info_async(self) -> dict[str, Any]:
+    async def get_info_async(self) -> Dict[str, Any]:
         '''获取角色信息
 
         返回:
-            dict[str, Any]: 角色详细信息
+            Dict[str, Any]: 角色详细信息
         '''
         try:
             response = await Api(
                 API['characters']['info'].format(id=self.id)
             ).aget()
         except HTTPStatusError as exception:
             if exception.response.status_code == 404:
@@ -174,29 +174,29 @@
     
     # 获取角色评论
     def get_comment(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取角色评论
 
         参数:
             limit (int, optional): 展示出的评论数，默认为 20
             offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
 
         返回:
-            dict[str, Any]: 搜索结果
+            Dict[str, Any]: 搜索结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的评论总数
-                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                    "posts": ... # List[Dict[str, Any]] 列举出的评论
                 }
                 ```
         '''
         return get_list(
             category_name='CHARACTER_COMMENT',
             category_id=str(self.id),
             order=order,
@@ -206,29 +206,29 @@
     
     # 异步获取角色评论
     async def get_comment_async(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取角色评论
 
         参数:
             limit (int, optional): 展示出的评论数，默认为 20
             offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
 
         返回:
-            dict[str, Any]: 搜索结果
+            Dict[str, Any]: 搜索结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的评论总数
-                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                    "posts": ... # List[Dict[str, Any]] 列举出的评论
                 }
                 ```
         '''
         return await get_list_async(
             category_name='CHARACTER_COMMENT',
             category_id=str(self.id),
             order=order,
```

### Comparing `bestdori-api-1.1.1/bestdori/charts.py` & `bestdori-api-1.1.2/bestdori/charts.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 '''`bestdori.charts`
 
 谱面相关操作'''
 from json import dumps, loads
-from typing import Any, Literal
+from typing import Any, Dict, List, Literal
 
 from httpx import Response
 
 from .models.note import *
 from .utils.utils import API
 from .utils.network import Api
 
 # 谱面数据类
 class Statistics:
     '''谱面数据类
 
     参数:
         time (float): 谱面时长
         notes (int): 谱面音符总数
-        bpm (list[float]): 谱面 BPM 范围
+        bpm (List[float]): 谱面 BPM 范围
         main_bpm (float): 谱面主 BPM
     '''
     # 初始化
-    def __init__(self, time: float, notes: int, bpm: list[float], main_bpm: float) -> None:
+    def __init__(self, time: float, notes: int, bpm: List[float], main_bpm: float) -> None:
         '''谱面数据类
 
         参数:
             time (float): 谱面时长
             notes (int): 谱面音符总数
-            bpm (list[float]): 谱面 BPM 范围
+            bpm (List[float]): 谱面 BPM 范围
             main_bpm (float): 谱面主 BPM
         '''
         self.time: float = time
         '''谱面时长'''
         self.notes: int = notes
         '''谱面音符总数'''
-        self.bpm: list[float] = bpm
+        self.bpm: List[float] = bpm
         '''谱面 BPM 范围'''
         self.main_bpm: float = main_bpm
         '''谱面主 BPM'''
         return
 
 # 谱面类
-class Chart(list[NoteType]):
+class Chart(List[NoteType]):
     '''谱面类，统合针对谱面的一层操作
 
     参数:
-        chart (list[dict[str, Any]]): 原始谱面代码'''
+        chart (List[Dict[str, Any]]): 原始谱面代码'''
     # 初始化
-    def __init__(self, chart: list[dict[str, Any]]) -> None:
+    def __init__(self, chart: List[Dict[str, Any]]) -> None:
         '''谱面类，统合针对谱面的一层操作
 
         参数:
-            chart (list[dict[str, Any]]): 原始谱面代码'''
+            chart (List[Dict[str, Any]]): 原始谱面代码'''
         super().__init__()
         for note in chart:
             # 遍历分类添加
             if note['type'] in ['Long', 'Slide']:
                 self.append(Slide(**note))
             elif note['type'] == 'BPM':
                 self.append(BPM(**note))
@@ -79,19 +79,19 @@
                         return True
             elif isinstance(note, Directional):
                 return True
         return False
     
     # 谱面规范化处理
     @classmethod
-    def normalize(cls, chart: list[dict[str, Any]]) -> 'Chart':
+    def normalize(cls, chart: List[Dict[str, Any]]) -> 'Chart':
         '''谱面规范化处理
 
         参数:
-            chart (list[dict[str, Any]]): 待处理谱面
+            chart (List[Dict[str, Any]]): 待处理谱面
 
         返回:
             Chart: 处理后谱面
         '''
         normalized_chart: cls = cls(chart)
         # 对谱面进行排序
         normalized_chart.sort(key=lambda x: x.beat)
@@ -150,15 +150,15 @@
         '''
         # 初始化统计数据
         start_beat = 0.0 # 谱面开始 beat 值
         end_beat = 0.0 # 谱面结束 beat 值
         prev_bpm = 120.0 # 上一个 BPM 线的 BPM 值
         prev_bpm_beat = 0.0 # 上一个 BPM 线的 beat 值
         total_notes = 0 # 总物量
-        bpm_list: list[dict[str, float]] = [] # BPM 统计列表，统计所有出现的 BPM 及其有效时间
+        bpm_list: List[Dict[str, float]] = [] # BPM 统计列表，统计所有出现的 BPM 及其有效时间
         
         # 遍历谱面数据
         for note in self:
             # 谱面为一个字典列表，每一个 note 都是一个字典
             if isinstance(note, BPM): # 如果当前是 BPM
                 if note.bpm >= 0: # 如果当前 BPM 大于等于 0
                     # 如果不是谱面一开始的 BPM 线且已有 note 被记录（即已出现过有效 bpm ）
@@ -241,17 +241,17 @@
             duration,
             total_notes,
             [bpm_min, bpm_max] if bpm_min != bpm_max else [bpm_min],
             bpm_main
         )
 
     # 转换为字典列表对象
-    def to_list(self) -> list[dict[str, Any]]:
-        '''将 `Chart` 谱面转换为 `list[dict[str, Any]]` 对象'''
-        chart_data: list[dict[str, Any]] = []
+    def to_list(self) -> List[Dict[str, Any]]:
+        '''将 `Chart` 谱面转换为 `List[Dict[str, Any]]` 对象'''
+        chart_data: List[Dict[str, Any]] = []
         for note in self:
             chart_data.append(note.__dict__)
         return chart_data
     
     # 转换为 json 字符串
     def json(self) -> str:
         '''将 `Chart` 谱面转换为 `json` 字符串'''
```

### Comparing `bestdori-api-1.1.1/bestdori/comics.py` & `bestdori-api-1.1.2/bestdori/comics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 '''`bestdori.comics`
 
 BanG Dream! 漫画相关操作'''
-from typing import Any, Literal
+from typing import Any, Dict, Literal
 
 from httpx import Response
 
 from .utils.utils import API, ASSETS
 from .utils.network import Api, Assets
 from .post import get_list, get_list_async
 from .exceptions import (
     NoDataException,
     ComicNotExistError,
     ServerNotAvailableError
 )
 
 # 获取总漫画信息
-def get_all(index: Literal[5]=5) -> dict[str, dict[str, Any]]:
+def get_all(index: Literal[5]=5) -> Dict[str, Dict[str, Any]]:
     '''获取总漫画信息
 
     参数:
         index (Literal[5], optional): 指定获取哪种 `all.json`
             `5`: 获取所有已有漫画信息 `all.5.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总漫画信息
+        Dict[str, Dict[str, Any]]: 获取到的总漫画信息
     '''
     return Api(API['all']['comics'].format(index=index)).get().json()
 
 # 异步获取总漫画信息
-async def get_all_async(index: Literal[5]=5) -> dict[str, dict[str, Any]]:
+async def get_all_async(index: Literal[5]=5) -> Dict[str, Dict[str, Any]]:
     '''获取总漫画信息
 
     参数:
         index (Literal[5], optional): 指定获取哪种 `all.json`
             `5`: 获取所有已有漫画信息 `all.5.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总漫画信息
+        Dict[str, Dict[str, Any]]: 获取到的总漫画信息
     '''
     response = await Api(API['all']['comics'].format(index=index)).aget()
     if isinstance(response, Response):
         return response.json()
     else:
         return await response.json()
 
@@ -56,15 +56,15 @@
         '''漫画类
 
         参数:
             id (int): 漫画 ID
         '''
         self.id: int = id
         '''漫画 ID'''
-        self.__info: dict[str, Any] = {}
+        self.__info: Dict[str, Any] = {}
         '''漫画信息'''
         return
     
     # 漫画标题
     @property
     def title(self) -> str:
         '''漫画标题'''
@@ -128,84 +128,84 @@
         # 判断漫画类型
         if 'fourframe' in asset_bundle_name:
             return 'fourframe'
         else:
             return 'singleframe'
     
     # 获取漫画信息
-    def get_info(self) -> dict[str, Any]:
+    def get_info(self) -> Dict[str, Any]:
         '''获取漫画信息
 
         返回:
-            dict[str, Any]: 漫画详细信息
+            Dict[str, Any]: 漫画详细信息
         '''
         if not self.__info:
             _all = get_all()
             if str(self.id) not in _all:
                 raise ComicNotExistError(self.id)
             self.__info = _all[str(self.id)]
         return self.__info
     
     # 异步获取漫画信息
-    async def get_info_async(self) -> dict[str, Any]:
+    async def get_info_async(self) -> Dict[str, Any]:
         '''获取漫画信息
 
         返回:
-            dict[str, Any]: 漫画详细信息
+            Dict[str, Any]: 漫画详细信息
         '''
         if not self.__info:
             _all = await get_all_async()
             if str(self.id) not in _all:
                 raise ComicNotExistError(self.id)
             self.__info = _all[str(self.id)]
         return self.__info
     
     # 获取缓存信息
-    def __get_info_cache(self) -> dict[str, Any]:
+    def __get_info_cache(self) -> Dict[str, Any]:
         '''获取缓存信息
 
         返回:
-            dict[str, Any]: 缓存信息
+            Dict[str, Any]: 缓存信息
         '''
         if not self.__info:
             return self.get_info()
         return self.__info
     
     # 异步获取缓存信息
-    async def __get_info_cache_async(self) -> dict[str, Any]:
+    async def __get_info_cache_async(self) -> Dict[str, Any]:
         '''获取缓存信息
 
         返回:
-            dict[str, Any]: 缓存信息
+            Dict[str, Any]: 缓存信息
         '''
         if not self.__info:
             return await self.get_info_async()
         return self.__info
     
     # 获取漫画评论
     def get_comment(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取漫画评论
 
         参数:
             limit (int, optional): 展示出的评论数，默认为 20
             offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
 
         返回:
-            dict[str, Any]: 搜索结果
+            Dict[str, Any]: 搜索结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的评论总数
-                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                    "posts": ... # List[Dict[str, Any]] 列举出的评论
                 }
                 ```
         '''
         return get_list(
             category_name='COMIC_COMMENT',
             category_id=str(self.id),
             order=order,
@@ -215,29 +215,29 @@
     
     # 异步获取漫画评论
     async def get_comment_async(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取漫画评论
 
         参数:
             limit (int, optional): 展示出的评论数，默认为 20
             offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
 
         返回:
-            dict[str, Any]: 搜索结果
+            Dict[str, Any]: 搜索结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的评论总数
-                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                    "posts": ... # List[Dict[str, Any]] 列举出的评论
                 }
                 ```
         '''
         return await get_list_async(
             category_name='COMIC_COMMENT',
             category_id=str(self.id),
             order=order,
```

### Comparing `bestdori-api-1.1.1/bestdori/costumes.py` & `bestdori-api-1.1.2/bestdori/costumes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 '''`bestdori.costumes`
 
 BanG Dream! 服装相关操作'''
-from typing import Any, Literal
+from typing import Any, Dict, Literal
 
 from aiohttp import ClientResponseError
 from httpx import Response, HTTPStatusError
 
 from .utils.utils import API, ASSETS
 from .utils.network import Api, Assets
 from .post import get_list, get_list_async
 from .exceptions import (
     NoDataException,
     AssetsNotExistError,
     CostumeNotExistError
 )
 
 # 获取总服装信息
-def get_all(index: Literal[0, 5]=5) -> dict[str, dict[str, Any]]:
+def get_all(index: Literal[0, 5]=5) -> Dict[str, Dict[str, Any]]:
     '''获取总服装信息
 
     参数:
         index (Literal[0, 5], optional): 指定获取哪种 `all.json`
             `0`: 仅获取所有已有服装 ID `all.0.json`
             `5`: 获取所有已有服装的简洁信息 `all.5.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总服装信息
+        Dict[str, Dict[str, Any]]: 获取到的总服装信息
     '''
     return Api(API['costumes']['all'].format(index=index)).get().json()
 
 # 异步获取总服装信息
-async def get_all_async(index: Literal[0, 5]=5) -> dict[str, dict[str, Any]]:
+async def get_all_async(index: Literal[0, 5]=5) -> Dict[str, Dict[str, Any]]:
     '''获取总服装信息
 
     参数:
         index (Literal[0, 5], optional): 指定获取哪种 `all.json`
             `0`: 仅获取所有已有服装 ID `all.0.json`
             `5`: 获取所有已有服装的简洁信息 `all.5.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总服装信息
+        Dict[str, Dict[str, Any]]: 获取到的总服装信息
     '''
     response = await Api(API['costumes']['all'].format(index=index)).aget()
     if isinstance(response, Response):
         return response.json()
     else:
         return await response.json()
 
@@ -59,15 +59,15 @@
         '''服装类
 
         参数:
             id (int): 服装 ID
         '''
         self.id: int = id
         '''服装 ID'''
-        self.__info: dict[str, Any] = {}
+        self.__info: Dict[str, Any] = {}
         '''服装信息'''
         return
     
     # 角色 ID
     @property
     def character_id(self) -> int:
         '''角色 ID'''
@@ -117,19 +117,19 @@
         elif published_at[2] is not None: return 'tw'
         elif published_at[3] is not None: return 'cn'
         elif published_at[4] is not None: return 'kr'
         else:
             raise NoDataException('服装所在服务器')
     
     # 获取服装信息
-    def get_info(self) -> dict[str, Any]:
+    def get_info(self) -> Dict[str, Any]:
         '''获取服装信息
 
         返回:
-            dict[str, Any]: 服装详细信息
+            Dict[str, Any]: 服装详细信息
         '''
         try:
             response = Api(
                 API['costumes']['info'].format(id=self.id)
             ).get()
         except HTTPStatusError as exception:
             if exception.response.status_code == 404:
@@ -137,19 +137,19 @@
             else:
                 raise exception
         
         self.__info = dict(response.json())
         return self.__info
     
     # 异步获取服装信息
-    async def get_info_async(self) -> dict[str, Any]:
+    async def get_info_async(self) -> Dict[str, Any]:
         '''获取服装信息
 
         返回:
-            dict[str, Any]: 服装详细信息
+            Dict[str, Any]: 服装详细信息
         '''
         try:
             response = await Api(
                 API['costumes']['info'].format(id=self.id)
             ).aget()
         except HTTPStatusError as exception:
             if exception.response.status_code == 404:
@@ -165,56 +165,56 @@
         if isinstance(response, Response):
             self.__info = dict(response.json())
         else:
             self.__info = dict(await response.json())
         return self.__info
     
     # 获取缓存信息
-    def __get_info_cache(self) -> dict[str, Any]:
+    def __get_info_cache(self) -> Dict[str, Any]:
         '''获取缓存信息
 
         返回:
-            dict[str, Any]: 服装详细信息
+            Dict[str, Any]: 服装详细信息
         '''
         if not self.__info:
             return self.get_info()
         return self.__info
     
     # 异步获取缓存信息
-    async def __get_info_cache_async(self) -> dict[str, Any]:
+    async def __get_info_cache_async(self) -> Dict[str, Any]:
         '''获取缓存信息
 
         返回:
-            dict[str, Any]: 服装详细信息
+            Dict[str, Any]: 服装详细信息
         '''
         if not self.__info:
             return await self.get_info_async()
         return self.__info
     
     # 获取服装评论
     def get_comment(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取服装评论
 
         参数:
             limit (int, optional): 展示出的评论数，默认为 20
             offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
 
         返回:
-            dict[str, Any]: 搜索结果
+            Dict[str, Any]: 搜索结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的评论总数
-                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                    "posts": ... # List[Dict[str, Any]] 列举出的评论
                 }
                 ```
         '''
         return get_list(
             category_name='COSTUME_COMMENT',
             category_id=str(self.id),
             order=order,
@@ -224,29 +224,29 @@
     
     # 异步获取服装评论
     async def get_comment_async(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取服装评论
 
         参数:
             limit (int, optional): 展示出的评论数，默认为 20
             offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
 
         返回:
-            dict[str, Any]: 搜索结果
+            Dict[str, Any]: 搜索结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的评论总数
-                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                    "posts": ... # List[Dict[str, Any]] 列举出的评论
                 }
                 ```
         '''
         return await get_list_async(
             category_name='COSTUME_COMMENT',
             category_id=str(self.id),
             order=order,
```

### Comparing `bestdori-api-1.1.1/bestdori/eventarchives.py` & `bestdori-api-1.1.2/bestdori/eventarchives.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 '''`bestdori.eventarchives`
 
 BanG Dream! 活动数据相关操作'''
-from typing import Any, Literal
+from typing import Any, Dict, List, Literal
 
 from httpx import Response
 
 from .utils.utils import API
 from .utils.network import Api
 from .post import get_list, get_list_async
 from .exceptions import (
     EventNotExistError
 )
 
 # 获取总活动数据信息
-def get_all(index: Literal[5]=5) -> dict[str, dict[str, Any]]:
+def get_all(index: Literal[5]=5) -> Dict[str, Dict[str, Any]]:
     '''获取总活动信息
 
     参数:
         index (Literal[5], optional): 指定获取哪种 `all.json`
             `5`: 获取所有已有活动数据的简洁信息 `all.5.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总活动信息
+        Dict[str, Dict[str, Any]]: 获取到的总活动信息
     '''
     return Api(API['all']['archives'].format(index=index)).get().json()
 
 # 异步获取总活动数据信息
-async def get_all_async(index: Literal[5]=5) -> dict[str, dict[str, Any]]:
+async def get_all_async(index: Literal[5]=5) -> Dict[str, Dict[str, Any]]:
     '''获取总活动信息
 
     参数:
         index (Literal[5], optional): 指定获取哪种 `all.json`
             `5`: 获取所有已有活动数据的简洁信息 `all.5.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总活动信息
+        Dict[str, Dict[str, Any]]: 获取到的总活动信息
     '''
     response = await Api(API['all']['archives'].format(index=index)).aget()
     if isinstance(response, Response):
         return response.json()
     else:
         return await response.json()
 
@@ -54,67 +54,67 @@
         '''活动数据类
 
         参数:
             id (int): 活动 ID
         '''
         self.id: int = id
         '''活动 ID'''
-        self.__info: dict[str, Any] = {}
+        self.__info: Dict[str, Any] = {}
         '''活动信息'''
         return
     
     # 获取活动数据信息
-    def get_info(self) -> dict[str, Any]:
+    def get_info(self) -> Dict[str, Any]:
         '''获取活动数据信息
 
         返回:
-            dict[str, Any]: 活动数据信息
+            Dict[str, Any]: 活动数据信息
         '''
         _all = get_all()
         if str(self.id) not in _all:
             raise EventNotExistError(self.id)
         self.__info = _all[str(self.id)]
         
         return self.__info
     
     # 异步获取活动数据信息
-    async def get_info_async(self) -> dict[str, Any]:
+    async def get_info_async(self) -> Dict[str, Any]:
         '''获取活动数据信息
 
         返回:
-            dict[str, Any]: 活动数据信息
+            Dict[str, Any]: 活动数据信息
         '''
         _all = await get_all_async()
         if str(self.id) not in _all:
             raise EventNotExistError(self.id)
         self.__info = _all[str(self.id)]
         
         return self.__info
     
     # 获取排名分数线
     def get_top(
         self,
         server: Literal[0, 1, 2, 3, 4],
         mid: Literal['0']='0',
         latest: Literal['1']='1'
-    ) -> dict[str, list[dict[str, Any]]]:
+    ) -> Dict[str, List[Dict[str, Any]]]:
         '''获取排名分数线
 
         参数:
             server (Literal[0, 1, 2, 3, 4]): 指定服务器
                 `0`: 日服
                 `1`: 英服
                 `2`: 台服
                 `3`: 国服
                 `4`: 韩服
             mid (Literal[&#39;0&#39;], optional): 指定是否为中间分数线，默认为 `0`
             latest (Literal[&#39;1&#39;], optional): 指定是否为最终分数线，默认为 `1`
 
         返回:
-            dict[str, list[dict[str, Any]]]: 排名分数线数据
+            Dict[str, List[Dict[str, Any]]]: 排名分数线数据
         '''
         return Api(API['events']['top']).get(
             params={
                 'server': server,
                 'event': self.id,
                 'mid': mid,
                 'latest': latest
@@ -123,29 +123,29 @@
     
     # 异步获取排名分数线
     async def get_top_async(
         self,
         server: Literal[0, 1, 2, 3, 4],
         mid: Literal['0']='0',
         latest: Literal['1']='1'
-    ) -> dict[str, list[dict[str, Any]]]:
+    ) -> Dict[str, List[Dict[str, Any]]]:
         '''获取排名分数线
 
         参数:
             server (Literal[0, 1, 2, 3, 4]): 指定服务器
                 `0`: 日服
                 `1`: 英服
                 `2`: 台服
                 `3`: 国服
                 `4`: 韩服
             mid (Literal[&#39;0&#39;], optional): 指定是否为中间分数线，默认为 `0`
             latest (Literal[&#39;1&#39;], optional): 指定是否为最终分数线，默认为 `1`
 
         返回:
-            dict[str, list[dict[str, Any]]]: 排名分数线数据
+            Dict[str, List[Dict[str, Any]]]: 排名分数线数据
         '''
         response = await Api(API['events']['top']).aget(
             params={
                 'server': server,
                 'event': self.id,
                 'mid': mid,
                 'latest': latest
@@ -158,29 +158,29 @@
 
     # 获取活动数据评论
     def get_comment(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取动数据评论
 
         参数:
             limit (int, optional): 展示出的评论数，默认为 20
             offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
 
         返回:
-            dict[str, Any]: 搜索结果
+            Dict[str, Any]: 搜索结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的评论总数
-                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                    "posts": ... # List[Dict[str, Any]] 列举出的评论
                 }
                 ```
         '''
         return get_list(
             category_id=str(self.id),
             category_name='EVENTARCHIVE_COMMENT',
             limit=limit,
@@ -190,29 +190,29 @@
     
     # 异步获取活动数据评论
     async def get_comment_async(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取动数据评论
 
         参数:
             limit (int, optional): 展示出的评论数，默认为 20
             offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
 
         返回:
-            dict[str, Any]: 搜索结果
+            Dict[str, Any]: 搜索结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的评论总数
-                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                    "posts": ... # List[Dict[str, Any]] 列举出的评论
                 }
                 ```
         '''
         return await get_list_async(
             category_id=str(self.id),
             category_name='EVENTARCHIVE_COMMENT',
             limit=limit,
```

### Comparing `bestdori-api-1.1.1/bestdori/events.py` & `bestdori-api-1.1.2/bestdori/events.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''`bestdori.events`
 
 BanG Dream! 活动相关操作'''
-from typing import Any, Literal, Optional
+from typing import Any, Dict, List, Literal, Optional
 
 from aiohttp import ClientResponseError
 from httpx import Response, HTTPStatusError
 
 from .utils.utils import API, ASSETS
 from .utils.network import Api, Assets
 from .eventarchives import EventArchive
@@ -23,40 +23,40 @@
     EventNotExistError,
     AssetsNotExistError,
     EventHasNoStampError,
     ServerNotAvailableError
 )
 
 # 获取总活动信息
-def get_all(index: Literal[0, 5, 6]=5) -> dict[str, dict[str, Any]]:
+def get_all(index: Literal[0, 5, 6]=5) -> Dict[str, Dict[str, Any]]:
     '''获取总活动信息
 
     参数:
         index (Literal[0, 5, 6], optional): 指定获取哪种 `all.json`
             `0`: 仅获取所有已有活动 ID `all.0.json`
             `5`: 获取所有已有活动的简洁信息 `all.5.json`
             `6`: 获取所有已有活动的简洁信息 `all.6.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总活动信息
+        Dict[str, Dict[str, Any]]: 获取到的总活动信息
     '''
     return Api(API['events']['all'].format(index=index)).get().json()
 
 # 异步获取总活动信息
-async def get_all_async(index: Literal[0, 5, 6]=5) -> dict[str, dict[str, Any]]:
+async def get_all_async(index: Literal[0, 5, 6]=5) -> Dict[str, Dict[str, Any]]:
     '''获取总活动信息
 
     参数:
         index (Literal[0, 5, 6], optional): 指定获取哪种 `all.json`
             `0`: 仅获取所有已有活动 ID `all.0.json`
             `5`: 获取所有已有活动的简洁信息 `all.5.json`
             `6`: 获取所有已有活动的简洁信息 `all.6.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总活动信息
+        Dict[str, Dict[str, Any]]: 获取到的总活动信息
     '''
     response = await Api(API['events']['all'].format(index=index)).aget()
     if isinstance(response, Response):
         return response.json()
     else:
         return await response.json()
 
@@ -74,15 +74,15 @@
         参数:
             id (int): 活动 ID
         '''
         self.id: int = id
         '''活动 ID'''
         self.archive: EventArchive = EventArchive(self.id)
         '''活动数据'''
-        self.__info: dict[str, Any] = {}
+        self.__info: Dict[str, Any] = {}
         '''活动信息'''
         return
     
     # 活动标题
     @property
     def name(self) -> str:
         '''活动标题'''
@@ -114,19 +114,19 @@
         elif start_at[2] is not None: return 'tw'
         elif start_at[3] is not None: return 'cn'
         elif start_at[4] is not None: return 'kr'
         else:
             raise NoDataException('活动所在服务器')
     
     # 获取活动信息
-    def get_info(self) -> dict[str, Any]:
+    def get_info(self) -> Dict[str, Any]:
         '''获取活动信息
 
         返回:
-            dict[str, Any]: 活动详细信息
+            Dict[str, Any]: 活动详细信息
         '''
         try:
             response = Api(
                 API['events']['info'].format(id=self.id)
             ).get()
         except HTTPStatusError as exception:
             if exception.response.status_code == 404:
@@ -134,19 +134,19 @@
             else:
                 raise exception
         
         self._info = dict(response.json())
         return self._info
     
     # 异步获取活动信息
-    async def get_info_async(self) -> dict[str, Any]:
+    async def get_info_async(self) -> Dict[str, Any]:
         '''获取活动信息
 
         返回:
-            dict[str, Any]: 活动详细信息
+            Dict[str, Any]: 活动详细信息
         '''
         try:
             response = await Api(
                 API['events']['info'].format(id=self.id)
             ).aget()
         except HTTPStatusError as exception:
             if exception.response.status_code == 404:
@@ -162,56 +162,56 @@
         if isinstance(response, Response):
             self._info = dict(response.json())
         else:
             self._info = dict(await response.json())
         return self._info
     
     # 获取缓存信息
-    def __get_info_cache(self) -> dict[str, Any]:
+    def __get_info_cache(self) -> Dict[str, Any]:
         '''获取缓存信息
 
         返回:
-            dict[str, Any]: 活动详细信息
+            Dict[str, Any]: 活动详细信息
         '''
         if not self._info:
             return self.get_info()
         return self._info
     
     # 异步获取缓存信息
-    async def __get_info_cache_async(self) -> dict[str, Any]:
+    async def __get_info_cache_async(self) -> Dict[str, Any]:
         '''获取缓存信息
 
         返回:
-            dict[str, Any]: 活动详细信息
+            Dict[str, Any]: 活动详细信息
         '''
         if not self._info:
             return await self.get_info_async()
         return self._info
     
     # 获取活动评论
     def get_comment(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取活动评论
 
         参数:
             limit (int, optional): 展示出的评论数，默认为 20
             offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
 
         返回:
-            dict[str, Any]: 搜索结果
+            Dict[str, Any]: 搜索结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的评论总数
-                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                    "posts": ... # List[Dict[str, Any]] 列举出的评论
                 }
                 ```
         '''
         return get_list(
             category_name='EVENT_COMMENT',
             category_id=str(self.id),
             order=order,
@@ -221,29 +221,29 @@
     
     # 异步获取活动评论
     async def get_comment_async(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取活动评论
 
         参数:
             limit (int, optional): 展示出的评论数，默认为 20
             offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
 
         返回:
-            dict[str, Any]: 搜索结果
+            Dict[str, Any]: 搜索结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的评论总数
-                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                    "posts": ... # List[Dict[str, Any]] 列举出的评论
                 }
                 ```
         '''
         return await get_list_async(
             category_name='EVENT_COMMENT',
             category_id=str(self.id),
             order=order,
@@ -503,29 +503,29 @@
 
     # 获取排名分数线
     def get_top(
         self,
         server: Optional[Literal[0, 1, 2, 3, 4]]=None,
         mid: Literal['0']='0',
         latest: Literal['1']='1'
-    ) -> dict[str, list[dict[str, Any]]]:
+    ) -> Dict[str, List[Dict[str, Any]]]:
         '''获取排名分数线
 
         参数:
             server (Optional[Literal[0, 1, 2, 3, 4]], optional): 指定服务器
                 `0`: 日服
                 `1`: 英服
                 `2`: 台服
                 `3`: 国服
                 `4`: 韩服
             mid (Literal[&#39;0&#39;], optional): 指定是否为中间分数线，默认为 `0`
             latest (Literal[&#39;1&#39;], optional): 指定是否为最终分数线，默认为 `1`
 
         返回:
-            dict[str, list[dict[str, Any]]]: 排名分数线数据
+            Dict[str, List[Dict[str, Any]]]: 排名分数线数据
         '''
         if server is None:
             self.__get_info_cache()
             if self.server == 'jp': server = 0
             elif self.server == 'en': server = 1
             elif self.server == 'tw': server = 2
             elif self.server == 'cn': server = 3
@@ -535,80 +535,80 @@
     
     # 异步获取排名分数线
     async def get_top_async(
         self,
         server: Optional[Literal[0, 1, 2, 3, 4]]=None,
         mid: Literal['0']='0',
         latest: Literal['1']='1'
-    ) -> dict[str, list[dict[str, Any]]]:
+    ) -> Dict[str, List[Dict[str, Any]]]:
         '''获取排名分数线
 
         参数:
             server (Optional[Literal[0, 1, 2, 3, 4]], optional): 指定服务器
                 `0`: 日服
                 `1`: 英服
                 `2`: 台服
                 `3`: 国服
                 `4`: 韩服
             mid (Literal[&#39;0&#39;], optional): 指定是否为中间分数线，默认为 `0`
             latest (Literal[&#39;1&#39;], optional): 指定是否为最终分数线，默认为 `1`
 
         返回:
-            dict[str, list[dict[str, Any]]]: 排名分数线数据
+            Dict[str, List[Dict[str, Any]]]: 排名分数线数据
         '''
         if server is None:
             await self.__get_info_cache_async()
             if self.server == 'jp': server = 0
             elif self.server == 'en': server = 1
             elif self.server == 'tw': server = 2
             elif self.server == 'cn': server = 3
             elif self.server == 'kr': server = 4
             else: raise NoDataException('活动服务器')
         return await self.archive.get_top_async(server, mid, latest)
 
     # 获取团队 LIVE 佳节活动歌曲循环数据
-    def get_rotation_musics(self) -> list[RotationMusic]:
+    def get_rotation_musics(self) -> List[RotationMusic]:
         '''获取团队 LIVE 佳节活动歌曲循环数据
 
         返回:
-            list[dict[str, Any]]: 团队 LIVE 佳节活动歌曲循环数据
+            List[Dict[str, Any]]: 团队 LIVE 佳节活动歌曲循环数据
         '''
         info = self.__get_info_cache()
         if (_event_type := info.get('eventTyppe', '')) != 'festival':
             raise ValueError(f'Rotation musics are only available for festival events, not {_event_type}.')
         return get_rotation_musics(self.id)
     
     # 异步获取团队 LIVE 佳节活动歌曲循环数据
-    async def get_rotation_musics_async(self) -> list[RotationMusic]:
+    async def get_rotation_musics_async(self) -> List[RotationMusic]:
         '''获取团队 LIVE 佳节活动歌曲循环数据
 
         返回:
-            list[dict[str, Any]]: 团队 LIVE 佳节活动歌曲循环数据
+            List[Dict[str, Any]]: 团队 LIVE 佳节活动歌曲循环数据
         '''
         info = await self.__get_info_cache_async()
         if (_event_type := info.get('eventTyppe', '')) != 'festival':
             raise ValueError(f'Rotation musics are only available for festival events, not {_event_type}.')
         return await get_rotation_musics_async(self.id)
     
     # 获取团队 LIVE 佳节活动舞台数据
-    def get_stages(self) -> list[Stage]:
+    def get_stages(self) -> List[Stage]:
         '''获取团队 LIVE 佳节活动舞台数据
 
         返回:
-            list[dict[str, Any]]: 团队 LIVE 佳节活动舞台数据
+            List[Dict[str, Any]]: 团队 LIVE 佳节活动舞台数据
         '''
         info = self.__get_info_cache()
         if (_event_type := info.get('eventTyppe', '')) != 'festival':
             raise ValueError(f'Stages are only available for festival events, not {_event_type}.')
         return get_stages(self.id)
     
     # 异步获取团队 LIVE 佳节活动舞台数据
-    async def get_stages_async(self) -> list[Stage]:
+    async def get_stages_async(self) -> List[Stage]:
         '''获取团队 LIVE 佳节活动舞台数据
 
         返回:
-            list[dict[str, Any]]: 团队 LIVE 佳节活动舞台数据
+            List[Dict[str, Any]]: 团队 LIVE 佳节活动舞台数据
         '''
         info = await self.__get_info_cache_async()
         if (_event_type := info.get('eventTyppe', '')) != 'festival':
             raise ValueError(f'Stages are only available for festival events, not {_event_type}.')
         return await get_stages_async(self.id)
```

### Comparing `bestdori-api-1.1.1/bestdori/exceptions.py` & `bestdori-api-1.1.2/bestdori/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 '''`bestdori.exceptions`
 
 API 错误信息相关操作'''
-from typing import Any
+from typing import Any, Dict
 
-from httpx._models import Response
 from httpx._exceptions import RequestError
 
 # 错误基类
-class BaseException(Exception):
+class BestdoriException(Exception):
     '''错误基类'''
     # 初始化
     def __init__(self, msg: str) -> None:
         self.message = msg
         '''错误信息'''
     
     # 字符串化
     def __str__(self) -> str:
         '''输出字符串'''
         return self.message
 
 # 请求发送错误
-class RequestException(BaseException):
+class RequestException(BestdoriException):
     '''请求发送错误'''
     # 初始化
     def __init__(self, api: str, msg: str='无错误代码获取', **kwargs: Any) -> None:
         if len(kwargs) > 0:
             msg += f': {kwargs}'
         else:
             msg += '。'
@@ -34,15 +33,15 @@
     
     # 字符串化
     def __str__(self) -> str:
         '''输出字符串'''
         return f'向 Bestdori {self.api} 发送请求时出错。{self.message}'
 
 # 资源错误
-class AssetsException(BaseException):
+class AssetsException(BestdoriException):
     '''资源错误'''
     # 初始化
     def __init__(self, msg: str, **kwargs: Any) -> None:
         if len(kwargs) > 0:
             msg += f': {kwargs}'
         else:
             msg += '。'
@@ -50,45 +49,45 @@
     
     # 字符串化
     def __str__(self) -> str:
         '''输出字符串'''
         return f'获取资源时出错。{self.message}'
 
 # 帖子错误
-class PostException(BaseException):
+class PostException(BestdoriException):
     '''帖子错误'''
     # 初始化
     def __init__(self, msg: str) -> None:
         super().__init__(msg)
         self.message = msg
         '''错误信息'''
         return
 
 # 帖子不是社区谱面
 class PostHasNoChartError(PostException):
     '''帖子不是社区谱面'''
     # 初始化
-    def __init__(self, post: dict[str, Any]) -> None:
+    def __init__(self, post: Dict[str, Any]) -> None:
         name = post.get('categoryName', 'DEFAULT_POST')
         msg = f'该帖子类型 {name} 不是社区谱面。'
         super().__init__(msg)
         return
 
 # 帖子没有音乐字段
 class PostHasNoSongError(PostException):
     '''帖子没有音乐字段'''
     # 初始化
-    def __init__(self, post: dict[str, Any]) -> None:
+    def __init__(self, post: Dict[str, Any]) -> None:
         name = post.get('categoryName', 'DEFAULT_POST')
         msg = f'该帖子类型 {name} 不存在歌曲资源。'
         super().__init__(msg)
         return
 
 # 某 id 指定的资源不存在
-class NotExistException(BaseException):
+class NotExistException(BestdoriException):
     '''资源不存在'''
     # 初始化
     def __init__(self, src: str) -> None:
         msg = f'{src} 不存在。'
         super().__init__(msg)
         self.message = msg
         '''错误信息'''
@@ -260,48 +259,48 @@
     # 初始化
     def __init__(self, server: str, id: int) -> None:
         msg = f'服务器 {server} 上的玩家 ID {id} 不存在。'
         super().__init__(msg)
         return
 
 # 服务器指定错误
-class ServerNotAvailableError(BaseException):
+class ServerNotAvailableError(BestdoriException):
     '''服务器指定错误'''
     # 初始化
     def __init__(self, name: str, server: str) -> None:
         msg = f'{name} 在服务器 {server} 不可用。'
         super().__init__(msg)
         self.message = msg
         '''错误信息'''
         return
 
 # 活动没有奖励贴纸错误
-class EventHasNoStampError(BaseException):
+class EventHasNoStampError(BestdoriException):
     '''活动没有奖励贴纸错误'''
     # 初始化
     def __init__(self, id: int) -> None:
         msg = f'活动 ID {id} 没有奖励贴纸。'
         super().__init__(msg)
         self.message = msg
         '''错误信息'''
         return
 
 # 无法获取到信息错误
-class NoDataException(BaseException):
+class NoDataException(BestdoriException):
     '''无法获取到信息错误'''
     # 初始化
     def __init__(self, src: str) -> None:
         msg = f'无法获取 {src} 。'
         super().__init__(msg)
         self.message = msg
         '''错误信息'''
         return
 
 # 设置出错
-class SettingsException(BaseException):
+class SettingsException(BestdoriException):
     '''设置出错'''
     # 初始化
     def __init__(self, msg: str) -> None:
         super().__init__(msg)
         self.message = msg
         '''错误信息'''
         return
@@ -321,15 +320,15 @@
     # 初始化
     def __init__(self, url: str) -> None:
         msg = f'没有获取到 {url} 的 ContentType'
         super().__init__(msg)
         return
 
 # 请求错误集合
-REQUEST_EXCEPTION: dict[str, type[RequestException]] = {
+REQUEST_EXCEPTION: Dict[str, type[RequestException]] = {
     'REQUEST_INVALID': RequestInvalidError,
     'LOGIN_REQUIRED': LoginRequiredError,
     'CREDENTIALS_INVALID': CredentialsInvalidError,
     'USER_INVALID': UserInvalidError,
     'ALREADY_UPLOADED': AlreadyUploadedError,
     'POST_INVALID': PostInvalidError
 }
```

### Comparing `bestdori-api-1.1.1/bestdori/festival.py` & `bestdori-api-1.1.2/bestdori/festival.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''`bestdori.festival` 团队佳节活动专属数据获取 API
 
 包括舞台数据、活动歌曲数据'''
 
-from typing import TypedDict
+from typing import Dict, List, TypedDict
 
 from httpx import Response
 
 from .utils.utils import API
 from .utils.network import Api
 
 # 歌曲循环数据类型
@@ -18,59 +18,59 @@
 # 舞台数据类型
 class Stage(TypedDict):
     type: str
     startAt: str
     endAt: str
 
 # 获取歌曲循环数据
-def get_rotation_musics(id: int) -> list[RotationMusic]:
+def get_rotation_musics(id: int) -> List[RotationMusic]:
     '''获取歌曲循环数据
 
     参数:
         id (int): 活动 ID
 
     返回:
-        list[dict[str, Any]]: 歌曲循环数据
+        List[Dict[str, Any]]: 歌曲循环数据
     '''
     return Api(API['festival']['rotation_musics'].format(id=id)).get().json()
 
 # 异步获取歌曲循环数据
-async def get_rotation_musics_async(id: int) -> list[RotationMusic]:
+async def get_rotation_musics_async(id: int) -> List[RotationMusic]:
     '''获取歌曲循环数据
 
     参数:
         id (int): 活动 ID
 
     返回:
-        list[dict[str, Any]]: 歌曲循环数据
+        List[Dict[str, Any]]: 歌曲循环数据
     '''
     response = await Api(API['festival']['rotation_musics'].format(id=id)).aget()
     if isinstance(response, Response):
         return response.json()
     return await response.json()
 
 # 获取舞台数据
-def get_stages(id: int) -> list[Stage]:
+def get_stages(id: int) -> List[Stage]:
     '''获取舞台数据
 
     参数:
         id (int): 活动 ID
 
     返回:
-        list[dict[str, Any]]: 舞台数据
+        List[Dict[str, Any]]: 舞台数据
     '''
     return Api(API['festival']['stages'].format(id=id)).get().json()
 
 # 异步获取舞台数据
-async def get_stages_async(id: int) -> list[Stage]:
+async def get_stages_async(id: int) -> List[Stage]:
     '''获取舞台数据
 
     参数:
         id (int): 活动 ID
 
     返回:
-        list[dict[str, Any]]: 舞台数据
+        List[Dict[str, Any]]: 舞台数据
     '''
     response = await Api(API['festival']['stages'].format(id=id)).aget()
     if isinstance(response, Response):
         return response.json()
     return await response.json()
```

### Comparing `bestdori-api-1.1.1/bestdori/gacha.py` & `bestdori-api-1.1.2/bestdori/gacha.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''`bestdori.gacha`
 
 BanG Dream! 招募相关操作'''
 import asyncio
-from typing import Any, Literal
+from typing import Any, Dict, List, Literal
 
 from aiohttp import ClientResponseError
 from httpx import Response, HTTPStatusError
 
 from .utils.utils import API, ASSETS
 from .utils.network import Api, Assets
 from .post import get_list, get_list_async
@@ -14,38 +14,38 @@
     NoDataException,
     GachaNotExistError,
     AssetsNotExistError,
     ServerNotAvailableError
 )
 
 # 获取总招募信息
-def get_all(index: Literal[0, 5]=5) -> dict[str, dict[str, Any]]:
+def get_all(index: Literal[0, 5]=5) -> Dict[str, Dict[str, Any]]:
     '''获取总招募信息
 
     参数:
         index (Literal[0, 5], optional): 指定获取哪种 `all.json`
             `0`: 仅获取所有已有招募 ID `all.0.json`
             `5`: 获取所有已有招募的简洁信息 `all.5.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总招募信息
+        Dict[str, Dict[str, Any]]: 获取到的总招募信息
     '''
     return Api(API['gacha']['all'].format(index=index)).get().json()
 
 # 异步获取总招募信息
-async def get_all_async(index: Literal[0, 5]=5) -> dict[str, dict[str, Any]]:
+async def get_all_async(index: Literal[0, 5]=5) -> Dict[str, Dict[str, Any]]:
     '''获取总招募信息
 
     参数:
         index (Literal[0, 5], optional): 指定获取哪种 `all.json`
             `0`: 仅获取所有已有招募 ID `all.0.json`
             `5`: 获取所有已有招募的简洁信息 `all.5.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总招募信息
+        Dict[str, Dict[str, Any]]: 获取到的总招募信息
     '''
     response = await Api(API['gacha']['all'].format(index=index)).aget()
     if isinstance(response, Response):
         return response.json()
     else:
         return await response.json()
 
@@ -61,15 +61,15 @@
         '''招募类
 
         参数:
             id (int): 招募 ID
         '''
         self.id: int = id
         '''招募 ID'''
-        self.__info: dict[str, Any] = {}
+        self.__info: Dict[str, Any] = {}
         '''招募信息'''
         return
     
     # 获取招募标题
     @property
     def name(self) -> str:
         '''获取招募标题
@@ -105,19 +105,19 @@
         elif published_at[2] is not None: return 'tw'
         elif published_at[3] is not None: return 'cn'
         elif published_at[4] is not None: return 'kr'
         else:
             raise NoDataException('招募所在服务器')
     
     # 获取招募信息
-    def get_info(self) -> dict[str, Any]:
+    def get_info(self) -> Dict[str, Any]:
         '''获取招募信息
 
         返回:
-            dict[str, Any]: 招募详细信息
+            Dict[str, Any]: 招募详细信息
         '''
         try:
             response = Api(
                 API['gacha']['info'].format(id=self.id)
             ).get()
         except HTTPStatusError as exception:
             if exception.response.status_code == 404:
@@ -125,19 +125,19 @@
             else:
                 raise exception
         
         self.__info = dict(response.json())
         return self.__info
     
     # 异步获取招募信息
-    async def get_info_async(self) -> dict[str, Any]:
+    async def get_info_async(self) -> Dict[str, Any]:
         '''获取招募信息
 
         返回:
-            dict[str, Any]: 招募详细信息
+            Dict[str, Any]: 招募详细信息
         '''
         try:
             response = await Api(
                 API['gacha']['info'].format(id=self.id)
             ).aget()
         except ClientResponseError as exception:
             if exception.status == 404:
@@ -145,56 +145,56 @@
             else:
                 raise exception
         
         self.__info = dict(await response.json())
         return self.__info
     
     # 获取缓存信息
-    def __get_info_cache(self) -> dict[str, Any]:
+    def __get_info_cache(self) -> Dict[str, Any]:
         '''获取缓存信息
 
         返回:
-            dict[str, Any]: 缓存信息
+            Dict[str, Any]: 缓存信息
         '''
         if not self.__info:
             return self.get_info()
         return self.__info
     
     # 异步获取缓存信息
-    async def __get_info_cache_async(self) -> dict[str, Any]:
+    async def __get_info_cache_async(self) -> Dict[str, Any]:
         '''获取缓存信息
 
         返回:
-            dict[str, Any]: 缓存信息
+            Dict[str, Any]: 缓存信息
         '''
         if not self.__info:
             return await self.get_info_async()
         return self.__info
     
     # 获取招募评论
     def get_comment(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取招募评论
 
         参数:
             limit (int, optional): 展示出的评论数，默认为 20
             offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
 
         返回:
-            dict[str, Any]: 搜索结果
+            Dict[str, Any]: 搜索结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的评论总数
-                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                    "posts": ... # List[Dict[str, Any]] 列举出的评论
                 }
                 ```
         '''
         return get_list(
             category_name='GACHA_COMMENT',
             category_id=str(self.id),
             order=order,
@@ -204,29 +204,29 @@
     
     # 异步获取招募评论
     async def get_comment_async(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取招募评论
 
         参数:
             limit (int, optional): 展示出的评论数，默认为 20
             offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
 
         返回:
-            dict[str, Any]: 搜索结果
+            Dict[str, Any]: 搜索结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的评论总数
-                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                    "posts": ... # List[Dict[str, Any]] 列举出的评论
                 }
                 ```
         '''
         return await get_list_async(
             category_name='GACHA_COMMENT',
             category_id=str(self.id),
             order=order,
@@ -285,26 +285,26 @@
         return await Assets(
             ASSETS['homebanner']['get'].format(
                 banner_asset_bundle_name=banner_asset_bundle_name
             ), server
         ).aget()
     
     # 获取招募 pickup 图像
-    def get_pickups(self, server: Literal['jp', 'en', 'tw', 'cn', 'kr']) -> list[bytes]:
+    def get_pickups(self, server: Literal['jp', 'en', 'tw', 'cn', 'kr']) -> List[bytes]:
         '''获取招募 pickup 图像
 
         参数:
             server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]): 服务器
 
         返回:
-            list[bytes]: pickup 图像字节数据 `bytes` 列表
+            List[bytes]: pickup 图像字节数据 `bytes` 列表
         '''
         PICKUPS = ['pickup1', 'pickup2', 'pickup']
         # 遍历尝试获取
-        pickup_list: list[bytes] = []
+        pickup_list: List[bytes] = []
         for pickup in PICKUPS:
             try:
                 pickup_list.append(
                     Assets(
                         ASSETS['gacha']['screen'].format(
                             id=self.id, asset_name=pickup
                         ), server
@@ -314,26 +314,26 @@
                 continue
         if len(pickup_list) <= 0:
             # 没有获取到任何 pickup 图像
             raise AssetsNotExistError('招募 pickup 图像')
         return pickup_list
     
     # 异步获取招募 pickup 图像
-    async def get_pickups_async(self, server: Literal['jp', 'en', 'tw', 'cn', 'kr']) -> list[bytes]:
+    async def get_pickups_async(self, server: Literal['jp', 'en', 'tw', 'cn', 'kr']) -> List[bytes]:
         '''获取招募 pickup 图像
 
         参数:
             server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]): 服务器
 
         返回:
-            list[bytes]: pickup 图像字节数据 `bytes` 列表
+            List[bytes]: pickup 图像字节数据 `bytes` 列表
         '''
         PICKUPS = ['pickup1', 'pickup2', 'pickup']
         # 遍历尝试获取
-        pickup_list: list[bytes] = []
+        pickup_list: List[bytes] = []
         tasks = [Assets(ASSETS['gacha']['screen'].format(id=self.id, asset_name=pickup), server).aget() for pickup in PICKUPS]
         for task in asyncio.as_completed(tasks):
             try:
                 pickup_list.append(await task)
             except:
                 continue
         if len(pickup_list) <= 0:
```

### Comparing `bestdori-api-1.1.1/bestdori/logincampaigns.py` & `bestdori-api-1.1.2/bestdori/logincampaigns.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 '''`bestdori.logincampaigns`
 
 BanG Dream! 登录奖励相关操作'''
-from typing import Any, Literal
+from typing import Any, Dict, List, Literal
 
 from aiohttp import ClientResponseError
 from httpx import Response, HTTPStatusError
 
 from .utils.utils import API, ASSETS
 from .utils.network import Api, Assets
 from .post import get_list, get_list_async
 from .exceptions import (
     NoDataException,
     ServerNotAvailableError,
     LoginCampaignNotExistError
 )
 
 # 获取总登录奖励信息
-def get_all(index: Literal[0, 5]=5) -> dict[str, dict[str, Any]]:
+def get_all(index: Literal[0, 5]=5) -> Dict[str, Dict[str, Any]]:
     '''获取总登录奖励信息
 
     参数:
         index (Literal[0, 5], optional): 指定获取哪种 `all.json`
             `0`: 仅获取所有已有登录奖励 ID `all.0.json`
             `5`: 获取所有已有登录奖励的简洁信息 `all.5.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总登录奖励信息
+        Dict[str, Dict[str, Any]]: 获取到的总登录奖励信息
     '''
     return Api(API['loginCampaigns']['all'].format(index=index)).get().json()
 
 # 异步获取总登录奖励信息
-async def get_all_async(index: Literal[0, 5]=5) -> dict[str, dict[str, Any]]:
+async def get_all_async(index: Literal[0, 5]=5) -> Dict[str, Dict[str, Any]]:
     '''获取总登录奖励信息
 
     参数:
         index (Literal[0, 5], optional): 指定获取哪种 `all.json`
             `0`: 仅获取所有已有登录奖励 ID `all.0.json`
             `5`: 获取所有已有登录奖励的简洁信息 `all.5.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总登录奖励信息
+        Dict[str, Dict[str, Any]]: 获取到的总登录奖励信息
     '''
     response = await Api(API['loginCampaigns']['all'].format(index=index)).aget()
     if isinstance(response, Response): return response.json()
     return await response.json()
 
 # 登录奖励类
 class LoginCampaign:
@@ -57,15 +57,15 @@
         '''登录奖励类
 
         参数:
             id (int): 登录奖励 ID
         '''
         self.id: int = id
         '''登录奖励 ID'''
-        self.__info: dict[str, Any] = {}
+        self.__info: Dict[str, Any] = {}
         '''登录奖励信息'''
         return
     
     # 登录奖励标题
     @property
     def name(self) -> str:
         '''登录奖励标题'''
@@ -93,38 +93,38 @@
         elif published_at[2] is not None: return 'tw'
         elif published_at[3] is not None: return 'cn'
         elif published_at[4] is not None: return 'kr'
         else:
             raise NoDataException('登录奖励所在服务器')
     
     # 获取登录奖励信息
-    def get_info(self) -> dict[str, Any]:
+    def get_info(self) -> Dict[str, Any]:
         '''获取登录奖励信息
 
         返回:
-            dict[str, Any]: 登录奖励详细信息
+            Dict[str, Any]: 登录奖励详细信息
         '''
         try:
             response = Api(
                 API['loginCampaigns']['info'].format(id=self.id)
             ).get()
         except HTTPStatusError as exception:
             if exception.response.status_code == 404:
                 raise LoginCampaignNotExistError(self.id)
             raise exception
         
         self.__info = dict(response.json())
         return self.__info
     
     # 异步获取登录奖励信息
-    async def get_info_async(self) -> dict[str, Any]:
+    async def get_info_async(self) -> Dict[str, Any]:
         '''获取登录奖励信息
 
         返回:
-            dict[str, Any]: 登录奖励详细信息
+            Dict[str, Any]: 登录奖励详细信息
         '''
         try:
             response = await Api(
                 API['loginCampaigns']['info'].format(id=self.id)
             ).aget()
         except HTTPStatusError as exception:
             if exception.response.status_code == 404:
@@ -138,56 +138,56 @@
         if isinstance(response, Response):
             self.__info = dict(response.json())
         else:
             self.__info = dict(await response.json())
         return self.__info
     
     # 获取缓存信息
-    def __get_info_cache(self) -> dict[str, Any]:
+    def __get_info_cache(self) -> Dict[str, Any]:
         '''获取缓存信息
 
         返回:
-            dict[str, Any]: 缓存信息
+            Dict[str, Any]: 缓存信息
         '''
         if not self.__info:
             return self.get_info()
         return self.__info
     
     # 异步获取缓存信息
-    async def __get_info_cache_async(self) -> dict[str, Any]:
+    async def __get_info_cache_async(self) -> Dict[str, Any]:
         '''获取缓存信息
 
         返回:
-            dict[str, Any]: 缓存信息
+            Dict[str, Any]: 缓存信息
         '''
         if not self.__info:
             return await self.get_info_async()
         return self.__info
     
     # 获取登录奖励评论
     def get_comment(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取登录奖励评论
 
         参数:
             limit (int, optional): 展示出的评论数，默认为 20
             offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
 
         返回:
-            dict[str, Any]: 搜索结果
+            Dict[str, Any]: 搜索结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的评论总数
-                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                    "posts": ... # List[Dict[str, Any]] 列举出的评论
                 }
                 ```
         '''
         return get_list(
             category_name='LOGINCAMPAIGN_COMMENT',
             category_id=str(self.id),
             order=order,
@@ -197,29 +197,29 @@
     
     # 异步获取登录奖励评论
     async def get_comment_async(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取登录奖励评论
 
         参数:
             limit (int, optional): 展示出的评论数，默认为 20
             offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
 
         返回:
-            dict[str, Any]: 搜索结果
+            Dict[str, Any]: 搜索结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的评论总数
-                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                    "posts": ... # List[Dict[str, Any]] 列举出的评论
                 }
                 ```
         '''
         return await get_list_async(
             category_name='LOGINCAMPAIGN_COMMENT',
             category_id=str(self.id),
             order=order,
```

### Comparing `bestdori-api-1.1.1/bestdori/miracleticket.py` & `bestdori-api-1.1.2/bestdori/miracleticket.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 '''`bestdori.miracleticket`
 
 BanG Dream! 自选券相关操作'''
-from typing import Any, Literal
+from typing import Any, Dict, List, Literal
 
 from httpx import Response
 
 from .utils.utils import API
 from .utils.network import Api
 from .exceptions import (
     NoDataException,
     ServerNotAvailableError,
     MiracleTicketExchangeNotExistError
 )
 
 # 获取总自选券信息
-def get_all(index: Literal[5]=5) -> dict[str, dict[str, Any]]:
+def get_all(index: Literal[5]=5) -> Dict[str, Dict[str, Any]]:
     '''获取总自选券信息
 
     参数:
         index (Literal[5], optional): 指定获取哪种 `all.json`
             `5`: 获取所有已有自选券信息 `all.5.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总自选券信息
+        Dict[str, Dict[str, Any]]: 获取到的总自选券信息
     '''
     return Api(
         API['all']['miracleTicketExchanges'].format(index=index)
     ).get().json()
 
 # 异步获取总自选券信息
-async def get_all_async(index: Literal[5]=5) -> dict[str, dict[str, Any]]:
+async def get_all_async(index: Literal[5]=5) -> Dict[str, Dict[str, Any]]:
     '''获取总自选券信息
 
     参数:
         index (Literal[5], optional): 指定获取哪种 `all.json`
             `5`: 获取所有已有自选券信息 `all.5.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总自选券信息
+        Dict[str, Dict[str, Any]]: 获取到的总自选券信息
     '''
     response = await Api(
         API['all']['miracleTicketExchanges'].format(index=index)
     ).aget()
     if isinstance(response, Response): return response.json()
     return await response.json()
 
@@ -57,15 +57,15 @@
         '''自选券类
 
         参数:
             id (int): 自选券 ID
         '''
         self.id: int = id
         '''自选券 ID'''
-        self.__info: dict[str, Any] = {}
+        self.__info: Dict[str, Any] = {}
         '''自选券信息'''
         return
     
     # 自选券标题
     @property
     def name(self) -> str:
         '''自选券标题'''
@@ -93,91 +93,91 @@
         elif ids[2] is not None: return 'tw'
         elif ids[3] is not None: return 'cn'
         elif ids[4] is not None: return 'kr'
         else:
             raise NoDataException('自选券所在服务器')
     
     # 获取自选券信息
-    def get_info(self) -> dict[str, Any]:
+    def get_info(self) -> Dict[str, Any]:
         '''获取自选券信息
 
         返回:
-            dict[str, Any]: 自选券详细信息
+            Dict[str, Any]: 自选券详细信息
         '''
         _all = get_all(5)
         if not self.id in _all.keys():
             raise MiracleTicketExchangeNotExistError(self.id)
         self.__info = _all[str(self.id)]
         return self.__info
     
     # 异步获取自选券信息
-    async def get_info_async(self) -> dict[str, Any]:
+    async def get_info_async(self) -> Dict[str, Any]:
         '''获取自选券信息
 
         返回:
-            dict[str, Any]: 自选券详细信息
+            Dict[str, Any]: 自选券详细信息
         '''
         _all = await get_all_async(5)
         if not self.id in _all.keys():
             raise MiracleTicketExchangeNotExistError(self.id)
         self.__info = _all[str(self.id)]
         return self.__info
     
     # 获取缓存信息
-    def __get_info_cache(self) -> dict[str, Any]:
+    def __get_info_cache(self) -> Dict[str, Any]:
         '''获取缓存信息
 
         返回:
-            dict[str, Any]: 缓存信息
+            Dict[str, Any]: 缓存信息
         '''
         if not self.__info:
             return self.get_info()
         return self.__info
     
     # 异步获取缓存信息
-    async def __get_info_cache_async(self) -> dict[str, Any]:
+    async def __get_info_cache_async(self) -> Dict[str, Any]:
         '''获取缓存信息
 
         返回:
-            dict[str, Any]: 缓存信息
+            Dict[str, Any]: 缓存信息
         '''
         if not self.__info:
             return await self.get_info_async()
         return self.__info
     
     # 获取自选券 ID 列表
-    def get_ids(self, server: Literal['jp', 'en', 'tw', 'cn', 'kr']) -> list[int]:
+    def get_ids(self, server: Literal['jp', 'en', 'tw', 'cn', 'kr']) -> List[int]:
         '''获取自选券 ID 列表
 
         参数:
             server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]): 指定服务器
 
         返回:
-            list[int]: 自选券 ID 列表
+            List[int]: 自选券 ID 列表
         '''
         info = self.__get_info_cache()
         # 获取 ids 数据
         if (ids := info.get('ids', None)) is None:
             raise NoDataException('自选券 ID 列表')
         # 判断服务器
         SERVERS = ['jp', 'en', 'tw', 'cn', 'kr']
         index = SERVERS.index(server)
         if ids[index] is None:
             raise ServerNotAvailableError(f'活动 {self.name}', server)
         return ids[index]
     
     # 异步获取自选券 ID 列表
-    async def get_ids_async(self, server: Literal['jp', 'en', 'tw', 'cn', 'kr']) -> list[int]:
+    async def get_ids_async(self, server: Literal['jp', 'en', 'tw', 'cn', 'kr']) -> List[int]:
         '''获取自选券 ID 列表
 
         参数:
             server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]): 指定服务器
 
         返回:
-            list[int]: 自选券 ID 列表
+            List[int]: 自选券 ID 列表
         '''
         info = await self.__get_info_cache_async()
         # 获取 ids 数据
         if (ids := info.get('ids', None)) is None:
             raise NoDataException('自选券 ID 列表')
         # 判断服务器
         SERVERS = ['jp', 'en', 'tw', 'cn', 'kr']
```

### Comparing `bestdori-api-1.1.1/bestdori/missions.py` & `bestdori-api-1.1.2/bestdori/missions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 '''`bestdori.missions`
 
 BanG Dream! 任务相关操作'''
-from typing import Any, Literal
+from typing import Any, Dict, List, Literal
 
 from aiohttp import ClientResponseError
 from httpx import Response, HTTPStatusError
 
 from .utils.utils import API
 from .utils.network import Api
 from .post import get_list, get_list_async
 from .exceptions import (
     NoDataException,
     MissionNotExistError
 )
 
 # 获取总任务信息
-def get_all(index: Literal[0, 5]=5) -> dict[str, dict[str, Any]]:
+def get_all(index: Literal[0, 5]=5) -> Dict[str, Dict[str, Any]]:
     '''获取总任务信息
 
     参数:
         index (Literal[0, 5], optional): 指定获取哪种 `all.json`
             `0`: 仅获取所有已有任务 ID `all.0.json`
             `5`: 获取所有已有任务的简洁信息 `all.5.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总任务信息
+        Dict[str, Dict[str, Any]]: 获取到的总任务信息
     '''
     return Api(API['missions']['all'].format(index=index)).get().json()
 
 # 异步获取总任务信息
-async def get_all_async(index: Literal[0, 5]=5) -> dict[str, dict[str, Any]]:
+async def get_all_async(index: Literal[0, 5]=5) -> Dict[str, Dict[str, Any]]:
     '''获取总任务信息
 
     参数:
         index (Literal[0, 5], optional): 指定获取哪种 `all.json`
             `0`: 仅获取所有已有任务 ID `all.0.json`
             `5`: 获取所有已有任务的简洁信息 `all.5.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总任务信息
+        Dict[str, Dict[str, Any]]: 获取到的总任务信息
     '''
     response = await Api(API['missions']['all'].format(index=index)).aget()
     if isinstance(response, Response): return response.json()
     return await response.json()
 
 # 任务类
 class Mission:
@@ -56,15 +56,15 @@
         '''任务类
 
         参数:
             id (int): 任务 ID
         '''
         self.id: int = id
         '''任务 ID'''
-        self.__info: dict[str, Any] = {}
+        self.__info: Dict[str, Any] = {}
         '''任务信息'''
         return
     
     # 任务标题
     @property
     def title(self) -> str:
         '''任务标题'''
@@ -92,38 +92,38 @@
         elif start_at[2] is not None: return 'tw'
         elif start_at[3] is not None: return 'cn'
         elif start_at[4] is not None: return 'kr'
         else:
             raise NoDataException('任务所在服务器')
     
     # 获取任务信息
-    def get_info(self) -> dict[str, Any]:
+    def get_info(self) -> Dict[str, Any]:
         '''获取任务信息
 
         返回:
-            dict[str, Any]: 任务详细信息
+            Dict[str, Any]: 任务详细信息
         '''
         try:
             response = Api(
                 API['missions']['info'].format(id=self.id)
             ).get()
         except HTTPStatusError as exception:
             if exception.response.status_code == 404:
                 raise MissionNotExistError(self.id)
             raise exception
         
         self.__info = dict(response.json())
         return self.__info
     
     # 异步获取任务信息
-    async def get_info_async(self) -> dict[str, Any]:
+    async def get_info_async(self) -> Dict[str, Any]:
         '''获取任务信息
 
         返回:
-            dict[str, Any]: 任务详细信息
+            Dict[str, Any]: 任务详细信息
         '''
         try:
             response = await Api(
                 API['missions']['info'].format(id=self.id)
             ).aget()
         except HTTPStatusError as exception:
             if exception.response.status_code == 404:
@@ -142,29 +142,29 @@
     
     # 获取任务评论
     def get_comment(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取任务评论
 
         参数:
             limit (int, optional): 展示出的评论数，默认为 20
             offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
 
         返回:
-            dict[str, Any]: 搜索结果
+            Dict[str, Any]: 搜索结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的评论总数
-                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                    "posts": ... # List[Dict[str, Any]] 列举出的评论
                 }
                 ```
         '''
         return get_list(
             category_name='MISSION_COMMENT',
             category_id=str(self.id),
             order=order,
@@ -174,29 +174,29 @@
     
     # 异步获取任务评论
     async def get_comment_async(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取任务评论
 
         参数:
             limit (int, optional): 展示出的评论数，默认为 20
             offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
 
         返回:
-            dict[str, Any]: 搜索结果
+            Dict[str, Any]: 搜索结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的评论总数
-                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                    "posts": ... # List[Dict[str, Any]] 列举出的评论
                 }
                 ```
         '''
         return await get_list_async(
             category_name='MISSION_COMMENT',
             category_id=str(self.id),
             order=order,
```

### Comparing `bestdori-api-1.1.1/bestdori/models/__init__.py` & `bestdori-api-1.1.2/bestdori/models/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 '''`bestdori.models` 对象定义模块'''
 
 from .content import Br as Br
 from .content import Link as Link
-from .content import List as List
 from .content import Text as Text
 from .content import Emoji as Emoji
 from .content import Image as Image
 from .content import Content as Content
 from .content import Heading as Heading
 from .content import Mention as Mention
+from .content import ContentList as ContentList
 
 from .note import BPM as BPM
 from .note import Slide as Slide
 from .note import Single as Single
 from .note import NoteType as NoteType
 from .note import Connection as Connection
 from .note import Directional as Directional
```

### Comparing `bestdori-api-1.1.1/bestdori/models/content.py` & `bestdori-api-1.1.2/bestdori/models/content.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 '''`bestdori.utils.content`
 
 Bestdori 帖子内容模块'''
-from typing import Literal, Any
+from typing import Literal, Any, Dict, List
 
 # 内容类
 class Content:
     '''内容类'''
     type: str
     '''内容类型'''
     # 初始化
-    def __init__(self, values: dict[str, Any]) -> None:
+    def __init__(self, values: Dict[str, Any]) -> None:
         '''初始化'''
         for key, value in values.items():
             setattr(self, key, value)
         return
     
     # 纯文本
     @staticmethod
@@ -77,19 +77,19 @@
         返回:
             Heading: 标题对象 `bestdori.utils.Heading`
         '''
         return Heading({'type': 'heading', 'data': data, 'margin': margin})
     
     # 图片
     @staticmethod
-    def image(objects: list[str], display: Literal[0, 1, 2]=0) -> 'Image':
+    def image(objects: List[str], display: Literal[0, 1, 2]=0) -> 'Image':
         '''图片
 
         参数:
-            objects (list[str]): 图片对象网址列表
+            objects (List[str]): 图片对象网址列表
             
             display (Literal[&#39;0&#39;, &#39;1&#39;, &#39;2&#39;], optional): 显示类型 `0`: 大图 `1`: 缩略图 `2`: 图标
 
         返回:
             Image: 图片对象 `bestdori.utils.Image`
         '''
         return Image({'type': 'image', 'objects': objects, 'display': display})
@@ -138,29 +138,29 @@
             'gacha-info',
             'song-info',
             'logincampaign-info',
             'comic-info',
             'mission-info'
         ],
         display: Literal[0, 1, 2],
-        objects: list[str]
-    ) -> 'List':
+        objects: List[str]
+    ) -> 'ContentList':
         '''列表
 
         参数:
             target (str): 列表对象
             
             display (Literal[&#39;0&#39;, &#39;1&#39;, &#39;2&#39;]): 显示类型
             
             objects (list[str]): 列表对象 ID 列表
 
         返回:
             List: 列表对象 `bestdori.utils.List`
         '''
-        return List({'type': 'list', 'target': target, 'display': display, 'objects': objects})
+        return ContentList({'type': 'list', 'target': target, 'display': display, 'objects': objects})
 
 # 文本类
 class Text(Content):
     '''文本类'''
     type: str = 'text'
     '''内容类型'''
     data: str
@@ -200,31 +200,31 @@
 # 图片类
 class Image(Content):
     '''图片类'''
     type: str = 'image'
     '''内容类型'''
     display: Literal[0, 1, 2]
     '''显示类型 `0`: 大图 `1`: 缩略图 `2`: 图标'''
-    objects: list[str]
+    objects: List[str]
     '''图片对象网址列表'''
 
 # 链接类
 class Link(Content):
     '''链接类'''
     type: str = 'link'
     '''内容类型'''
     target: str
     '''链接对象'''
     data: str
     '''链接信息'''
 
 # 列表类
-class List(Content):
+class ContentList(Content):
     '''列表类'''
     type: str = 'list'
     '''内容类型'''
     target: str
     '''列表对象'''
     display: Literal[0, 1, 2]
     '''显示类型'''
-    objects: list[str]
+    objects: List[str]
     '''列表对象 ID 列表'''
```

### Comparing `bestdori-api-1.1.1/bestdori/models/note.py` & `bestdori-api-1.1.2/bestdori/models/note.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''`bestdori.utils.note`
 
 谱面音符相关模块'''
-from typing import Literal, Any
+from typing import Literal, Any, Dict, List
 from typing_extensions import override
 
 # 谱面音符类
 class NoteType:
     '''谱面音符类'''
     type: str
     '''音符类型'''
@@ -58,15 +58,15 @@
         '''初始化'''
         for key, value in values.items():
             setattr(self, key, value)
         return
     
     # 字典化
     @property
-    def __dict__(self) -> dict[str, Any]:
+    def __dict__(self) -> Dict[str, Any]:
         '''字典化'''
         note = {'beat': self.beat, 'lane': self.lane}
         if self.hidden:
             note['hidden'] = self.hidden
         if self.flick:
             note['flick'] = self.flick
         if self.skill:
@@ -83,15 +83,15 @@
         beat (float): 节拍数'''
     type: str = 'BPM'
     '''音符类型'''
     bpm: float
     '''BPM 值'''
     # 字典化
     @property
-    def __dict__(self) -> dict:
+    def __dict__(self) -> Dict[str, Any]:
         '''字典化'''
         return {
             'bpm': self.bpm,
             'beat': self.beat,
             'type': self.type
         }
 
@@ -113,15 +113,15 @@
     '''轨道数'''
     flick: bool = False
     '''是否为滑键'''
     skill: bool = False
     '''是否为技能键'''
     # 字典化
     @property
-    def __dict__(self) -> dict:
+    def __dict__(self) -> Dict[str, Any]:
         '''字典化'''
         note = {
             'beat': self.beat,
             'lane': self.lane,
             'type': self.type
         }
         if self.flick:
@@ -148,15 +148,15 @@
     '''轨道数'''
     width: int
     '''滑键宽度'''
     direction: Literal['Left', 'Right']
     '''滑键方向'''
     # 字典化
     @property
-    def __dict__(self) -> dict:
+    def __dict__(self) -> Dict[str, Any]:
         '''字典化'''
         note = {
             'beat': self.beat,
             'lane': self.lane,
             'type': self.type,
             'width': self.width,
             'direction': self.direction
@@ -164,41 +164,41 @@
         return note
 
 # 滑条
 class Slide(NoteType):
     '''滑条
 
     参数:
-        connections (list[Connection]): 滑键节点'''
+        connections (List[Connection]): 滑键节点'''
     type: str = 'Slide'
     '''音符类型'''
-    connections: list[Connection]
+    connections: List[Connection]
     '''滑键节点'''
     # 初始化
     def __init__(self, **values) -> None:
         '''初始化'''
         for key, value in values.items():
             if key == 'type':
                 continue
             if key == 'connections':
-                connections: list[Connection] = []
+                connections: List[Connection] = []
                 # 提取起始节拍数
                 self.beat = value[0]['beat']
                 
                 for connection in value:
                     connections.append(Connection(**connection))
                 value = connections
             setattr(self, key, value)
         return
     
     # 字典化
     @property
-    def __dict__(self) -> dict:
+    def __dict__(self) -> Dict[str, Any]:
         '''字典化'''
-        note: dict[str, Any] = {
+        note: Dict[str, Any] = {
             'type': self.type
         }
         if self.connections:
             note['connections'] = [connection.__dict__ for connection in self.connections]
         return note
     
     # 节拍数增减
```

### Comparing `bestdori-api-1.1.1/bestdori/player.py` & `bestdori-api-1.1.2/bestdori/player.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''`bestdori.player`
 
 BanG Dream! 玩家信息相关操作'''
 
-from typing import Any, Optional
+from typing import Any, Dict, Optional
 
 from httpx import Response
 
 from .utils.utils import API
 from .utils.network import Api
 from .exceptions import PlayerNotExistError
 
@@ -16,43 +16,43 @@
     参数:
         id (int): 玩家 ID
         server (str): 服务器
     '''
     def __init__(self, id: int, server: str) -> None:
         self.id: int = id
         self.server: str = server
-        self.__info: Optional[dict[str, Any]] = None
+        self.__info: Optional[Dict[str, Any]] = None
     
-    def get_info(self) -> dict[str, Any]:
+    def get_info(self) -> Dict[str, Any]:
         '''获取玩家信息
 
         返回:
-            dict[str, Any]: 玩家信息
+            Dict[str, Any]: 玩家信息
         '''
         params = {
             'mode': 2
         }
         _info = Api(
             API['player']['info'].format(server=self.server, id=self.id)
         ).get(params=params).json()
         if not _info.get('result', False):
             raise ValueError(f'Invalid Server: {self.server}')
-        _data: dict[str, Any] = _info.get('data', {})
-        _profile: Optional[dict[str, Any]] = _data.get('profile', None)
+        _data: Dict[str, Any] = _info.get('data', {})
+        _profile: Optional[Dict[str, Any]] = _data.get('profile', None)
         if _profile is None:
             raise PlayerNotExistError(self.server, self.id)
         self.__info = _profile
         
         return self.__info
     
-    async def get_info_async(self) -> dict[str, Any]:
+    async def get_info_async(self) -> Dict[str, Any]:
         '''获取玩家信息
 
         返回:
-            dict[str, Any]: 玩家信息
+            Dict[str, Any]: 玩家信息
         '''
         params = {
             'mode': 2
         }
         response = await Api(
             API['player']['info'].format(server=self.server, id=self.id)
         ).aget(params=params)
@@ -60,14 +60,14 @@
         if isinstance(response, Response):
             _info = response.json()
         else:
             _info = await response.json()
         
         if not _info.get('result', False):
             raise ValueError(f'Invalid Server: {self.server}')
-        _data: dict[str, Any] = _info.get('data', {})
-        _profile: Optional[dict[str, Any]] = _data.get('profile', None)
+        _data: Dict[str, Any] = _info.get('data', {})
+        _profile: Optional[Dict[str, Any]] = _data.get('profile', None)
         if _profile is None:
             raise PlayerNotExistError(self.server, self.id)
         self.__info = _profile
         
         return self.__info
```

### Comparing `bestdori-api-1.1.1/bestdori/post.py` & `bestdori-api-1.1.2/bestdori/post.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 '''`bestdori.post`
 
 社区帖子相关操作'''
 from typing_extensions import overload
-from typing import TYPE_CHECKING, Any, Union, Literal, Optional, TypedDict
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Dict,
+    List,
+    Union,
+    Literal,
+    Optional,
+    TypedDict
+)
 
 from httpx import Response
 
 from .charts import Chart
 from .models.content import Content
 from .utils.utils import API, ASSETS
 from .utils.network import Api, Assets
@@ -58,105 +67,105 @@
 # 搜索社区谱面
 @overload
 def get_list(
     *,
     search: str='',
     category_name: Literal['SELF_POST']='SELF_POST',
     category_id: Literal['chart']='chart',
-    tags: list[Tag]=[],
+    tags: List[Tag]=[],
     order: Literal['TIME_DESC', 'TIME_ASC']='TIME_DESC',
     limit: int=20,
     offset: int=0
-) -> dict[str, Any]:
+) -> Dict[str, Any]:
     '''搜索社区谱面
         ```python
         # 以 'Arghena' 为关键词，搜索社区谱面
         Post.search(search='Arghena', caregory_name='SELF_POST', category_id='chart')
         ```
 
     参数:
         search (str, optional): 搜索关键词，默认为空
         category_name (Literal[&#39;SELF_POST&#39;], optional): 搜索的帖子类型 `SELF_POST`
         category_id (Literal[&#39;chart&#39;, &#39;text&#39;], optional): 搜索的画廊种类 `chart`
-        tags (list[Tag], optional): 搜索的标签，默认为空
+        tags (List[Tag], optional): 搜索的标签，默认为空
         order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 帖子排序，默认时间倒序
         limit (int, optional): 展示出的帖子数，默认 20
         offset (int, optional): 忽略前面的 `offset` 个帖子，默认 0
 
     返回:
-        dict[str, Any]: 搜索结果
+        Dict[str, Any]: 搜索结果
             ```python
             result: bool # 是否有响应
             count: int # 搜索到的谱面总数
-            posts: list[dict[str, Any]] # 列举出的谱面
+            posts: List[Dict[str, Any]] # 列举出的谱面
             ```
     '''
     ...
 
 # 搜索用户帖子
 @overload
 def get_list(
     *,
     username: str,
     limit: int=20,
     offset: int=0,
     order: Literal['TIME_DESC', 'TIME_ASC']='TIME_DESC'
-) -> dict[str, Any]:
+) -> Dict[str, Any]:
     '''搜索用户帖子
 
     参数:        
         username (str): 用户名
         limit (int, optional): 展示出的帖子数，默认 20
         offset (int, optional): 忽略前面的 `offset` 个帖子，默认 0
         order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 帖子排序，默认时间倒序
 
     返回:
-        dict[str, Any]: 搜索结果
+        Dict[str, Any]: 搜索结果
             ```python
             result: bool # 是否有响应
             count: int # 搜索到的帖子总数
-            posts: list[dict[str, Any]] # 列举出的帖子
+            posts: List[Dict[str, Any]] # 列举出的帖子
             ```
     '''
     ...
 
 # 搜索帖子
 @overload
 def get_list(
     *,
     search: Optional[str]=None,
     following: Optional[bool]=None,
     category_name: Optional[str]=None,
     category_id: Optional[str]=None,
-    tags: Optional[list[Tag]]=None,
+    tags: Optional[List[Tag]]=None,
     username: Optional[str]=None,
     order: Literal['TIME_DESC', 'TIME_ASC'],
     limit: int=20,
     offset: int=0
-) -> dict[str, Any]:
+) -> Dict[str, Any]:
     '''搜索帖子
 
     参数:        
         order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;]): 帖子排序
         search (Optional[str], optional): 搜索关键词
         following (Optional[bool], optional): 是否关注
         category_name (Optional[str], optional): 画廊名称
         category_id (Optional[str], optional): 画廊 ID
         tags (Optional[List[Tag]], optional): 帖子标签
         username (Optional[str], optional): 用户名
         limit (int, optional): 展示出的帖子数，默认 20
         offset (int, optional): 忽略前面的 `offset` 个帖子，默认 0
 
     返回:
-        dict[str, Any]: 搜索结果
+        Dict[str, Any]: 搜索结果
     '''
     ...
 
 # 搜索帖子
-def get_list(**kwargs: Any) -> dict[str, Any]:
+def get_list(**kwargs: Any) -> Dict[str, Any]:
     # 去除 None 值字段
     kwargs = {key: value for key, value in kwargs.items() if value is not None}
     # 将下划线字段名转换为小驼峰字段名
     kwargs = {
         (
             "".join(x.capitalize() if i > 0 else x for i, x in enumerate(key.split("_")))
         ): value for key, value in kwargs.items() if value is not None
@@ -167,105 +176,105 @@
 # 异步搜索社区谱面
 @overload
 async def get_list_async(
     *,
     search: str='',
     category_name: Literal['SELF_POST']='SELF_POST',
     category_id: Literal['chart']='chart',
-    tags: list[Tag]=[],
+    tags: List[Tag]=[],
     order: Literal['TIME_DESC', 'TIME_ASC']='TIME_DESC',
     limit: int=20,
     offset: int=0
-) -> dict[str, Any]:
+) -> Dict[str, Any]:
     '''搜索社区谱面
         ```python
         # 以 'Arghena' 为关键词，搜索社区谱面
         Post.search(search='Arghena', caregory_name='SELF_POST', category_id='chart')
         ```
 
     参数:
         search (str, optional): 搜索关键词，默认为空
         category_name (Literal[&#39;SELF_POST&#39;], optional): 搜索的帖子类型 `SELF_POST`
         category_id (Literal[&#39;chart&#39;, &#39;text&#39;], optional): 搜索的画廊种类 `chart`
-        tags (list[Tag], optional): 搜索的标签，默认为空
+        tags (List[Tag], optional): 搜索的标签，默认为空
         order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 帖子排序，默认时间倒序
         limit (int, optional): 展示出的帖子数，默认 20
         offset (int, optional): 忽略前面的 `offset` 个帖子，默认 0
 
     返回:
-        dict[str, Any]: 搜索结果
+        Dict[str, Any]: 搜索结果
             ```python
             result: bool # 是否有响应
             count: int # 搜索到的谱面总数
-            posts: list[dict[str, Any]] # 列举出的谱面
+            posts: List[Dict[str, Any]] # 列举出的谱面
             ```
     '''
     ...
 
 # 异步搜索用户帖子
 @overload
 async def get_list_async(
     *,
     username: str,
     limit: int=20,
     offset: int=0,
     order: Literal['TIME_DESC', 'TIME_ASC']='TIME_DESC'
-) -> dict[str, Any]:
+) -> Dict[str, Any]:
     '''搜索用户帖子
 
     参数:        
         username (str): 用户名
         limit (int, optional): 展示出的帖子数，默认 20
         offset (int, optional): 忽略前面的 `offset` 个帖子，默认 0
         order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 帖子排序，默认时间倒序
 
     返回:
-        dict[str, Any]: 搜索结果
+        Dict[str, Any]: 搜索结果
             ```python
             result: bool # 是否有响应
             count: int # 搜索到的帖子总数
-            posts: list[dict[str, Any]] # 列举出的帖子
+            posts: List[Dict[str, Any]] # 列举出的帖子
             ```
     '''
     ...
 
 # 异步搜索帖子
 @overload
 async def get_list_async(
     *,
     search: Optional[str]=None,
     following: Optional[bool]=None,
     category_name: Optional[str]=None,
     category_id: Optional[str]=None,
-    tags: Optional[list[Tag]]=None,
+    tags: Optional[List[Tag]]=None,
     username: Optional[str]=None,
     order: Literal['TIME_DESC', 'TIME_ASC'],
     limit: int=20,
     offset: int=0
-) -> dict[str, Any]:
+) -> Dict[str, Any]:
     '''搜索帖子
 
     参数:        
         order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;]): 帖子排序
         search (Optional[str], optional): 搜索关键词
         following (Optional[bool], optional): 是否关注
         category_name (Optional[str], optional): 画廊名称
         category_id (Optional[str], optional): 画廊 ID
         tags (Optional[List[Tag]], optional): 帖子标签
         username (Optional[str], optional): 用户名
         limit (int, optional): 展示出的帖子数，默认 20
         offset (int, optional): 忽略前面的 `offset` 个帖子，默认 0
 
     返回:
-        dict[str, Any]: 搜索结果
+        Dict[str, Any]: 搜索结果
     '''
     ...
 
 # 异步搜索帖子
-async def get_list_async(**kwargs: Any) -> dict[str, Any]:
+async def get_list_async(**kwargs: Any) -> Dict[str, Any]:
     # 去除 None 值字段
     kwargs = {key: value for key, value in kwargs.items() if value is not None}
     # 将下划线字段名转换为小驼峰字段名
     kwargs = {
         (
             "".join(x.capitalize() if i > 0 else x for i, x in enumerate(key.split("_")))
         ): value for key, value in kwargs.items() if value is not None
@@ -277,24 +286,24 @@
         return await response.json()
 
 # 搜索标签
 def search_tags(
     type: str,
     data: str='',
     fuzzy: bool=True
-) -> list[Tag]:
+) -> List[Tag]:
     '''搜索已有标签
 
     参数:
         type (str): 标签类型
         data (str, optional): 搜索标签数据关键词
         fuzzy (bool, optional): 是否使用模糊搜索
 
     返回:
-        list[Tag]: 标签类 `Tag` 列表
+        List[Tag]: 标签类 `Tag` 列表
     '''
     response = Api(API['post']['tag']).get(
         params={
             'type': type,
             'data': data,
             'fuzzy': fuzzy
         }
@@ -305,24 +314,24 @@
         raise RequestException(API['post']['tag'], '搜索标签时出现未知错误')
 
 # 异步搜索标签
 async def search_tags_async(
     type: str,
     data: str='',
     fuzzy: bool=True
-) -> list[Tag]:
+) -> List[Tag]:
     '''搜索已有标签
 
     参数:
         type (str): 标签类型
         data (str, optional): 搜索标签数据关键词
         fuzzy (bool, optional): 是否使用模糊搜索
 
     返回:
-        list[Tag]: 标签类 `Tag` 列表
+        List[Tag]: 标签类 `Tag` 列表
     '''
     response = await Api(API['post']['tag']).aget(
         params={
             'type': type,
             'data': data,
             'fuzzy': fuzzy
         }
@@ -343,60 +352,60 @@
 def post(
     me: 'Me',
     *,
     artists: str,
     category_id: Literal['chart']='chart',
     category_name: Literal['SELF_POST']='SELF_POST',
     chart: Chart,
-    content: list[Content],
+    content: List[Content],
     diff: Literal[0, 1, 2, 3, 4],
     level: int,
     song: Union[CustomSong, ProvidedSong],
-    tags: list[Tag]=[],
+    tags: List[Tag]=[],
     title: str
 ) -> int:
     '''发表谱面
 
     参数:
         me (Me): 自身用户对象
         artists (str): 歌手
         category_id (Literal[&#39;chart&#39;], optional): 谱面画廊 ID `chart`
         category_name (Literal[&#39;SELF_POST&#39;], optional): 谱面画廊名称 `SELF_POST`
         chart (Chart): 谱面
-        content (list[Content]): 帖子内容
+        content (List[Content]): 帖子内容
         diff (Literal[0, 1, 2, 3, 4]): 难度
         level (int): 等级
         song (Union[CustomSong, ProvidedSong]): 歌曲
-        tags (list[Tag], optional): 谱面标签
+        tags (List[Tag], optional): 谱面标签
         title (str): 谱面标题
 
     返回:
         int: 谱面 ID
     '''
     ...
 
 # 发表文本帖子
 @overload
 def post(
     me: 'Me',
     *,
     category_id: Literal['text']='text',
     category_name: Literal['SELF_POST']='SELF_POST',
-    content: list[Content],
-    tags: list[Tag]=[],
+    content: List[Content],
+    tags: List[Tag]=[],
     title: str
 ) -> int:
     '''发表文本帖子
 
     参数:
         me (Me): 自身用户对象
         category_id (Literal[&#39;text&#39;], optional): 帖子画廊 ID `text`
         category_name (Literal[&#39;SELF_POST&#39;], optional): 帖子画廊名称 `SELF_POST`
-        content (list[Content]): 帖子内容
-        tags (list[Tag], optional): 帖子标签
+        content (List[Content]): 帖子内容
+        tags (List[Tag], optional): 帖子标签
         title (str): 帖子标题
 
     返回:
         int: 帖子 ID
     '''
     ...
 
@@ -405,34 +414,34 @@
 def post(
     me: 'Me',
     *,
     artists: Optional[str]=None,
     category_id: str,
     category_name: str,
     chart: Optional[Chart]=None,
-    content: list[Content],
+    content: List[Content],
     diff: Optional[Literal[0, 1, 2, 3, 4]]=None,
     level: Optional[int]=None,
     song: Optional[Union[CustomSong, ProvidedSong]]=None,
-    tags: Optional[list[Tag]]=None,
+    tags: Optional[List[Tag]]=None,
     title: Optional[str]=None
 ) -> int:
     '''发表帖子
 
     参数:
         me (Me): 自身用户对象
         artists (Optional[str], optional): 歌手
         category_id (str): 帖子画廊 ID
         category_name (str): 帖子画廊名称
         chart (Optional[Chart], optional): 谱面
-        content (list[Content]): 帖子内容
+        content (List[Content]): 帖子内容
         diff (Optional[Literal[0, 1, 2, 3, 4]], optional): 难度
         level (Optional[int], optional): 等级
         song (Optional[Union[CustomSong, ProvidedSong]], optional): 歌曲
-        tags (Optional[list[Tag]], optional): 帖子标签
+        tags (Optional[List[Tag]], optional): 帖子标签
         title (Optional[str], optional): 帖子标题
 
     返回:
         int: 帖子 ID
     '''
     ...
 
@@ -469,60 +478,60 @@
 async def apost(
     me: 'Me',
     *,
     artists: str,
     category_id: Literal['chart']='chart',
     category_name: Literal['SELF_POST']='SELF_POST',
     chart: Chart,
-    content: list[Content],
+    content: List[Content],
     diff: Literal[0, 1, 2, 3, 4],
     level: int,
     song: Union[CustomSong, ProvidedSong],
-    tags: list[Tag]=[],
+    tags: List[Tag]=[],
     title: str
 ) -> int:
     '''发表谱面
 
     参数:
         me (Me): 自身用户对象
         artists (str): 歌手
         category_id (Literal[&#39;chart&#39;], optional): 谱面画廊 ID `chart`
         category_name (Literal[&#39;SELF_POST&#39;], optional): 谱面画廊名称 `SELF_POST`
         chart (Chart): 谱面
-        content (list[Content]): 帖子内容
+        content (List[Content]): 帖子内容
         diff (Literal[0, 1, 2, 3, 4]): 难度
         level (int): 等级
         song (Union[CustomSong, ProvidedSong]): 歌曲
-        tags (list[Tag], optional): 谱面标签
+        tags (List[Tag], optional): 谱面标签
         title (str): 谱面标题
 
     返回:
         int: 谱面 ID
     '''
     ...
 
 # 异步发表文本帖子
 @overload
 async def apost(
     me: 'Me',
     *,
     category_id: Literal['text']='text',
     category_name: Literal['SELF_POST']='SELF_POST',
-    content: list[Content],
-    tags: list[Tag]=[],
+    content: List[Content],
+    tags: List[Tag]=[],
     title: str
 ) -> int:
     '''发表文本帖子
 
     参数:
         me (Me): 自身用户对象
         category_id (Literal[&#39;text&#39;], optional): 帖子画廊 ID `text`
         category_name (Literal[&#39;SELF_POST&#39;], optional): 帖子画廊名称 `SELF_POST`
-        content (list[Content]): 帖子内容
-        tags (list[Tag], optional): 帖子标签
+        content (List[Content]): 帖子内容
+        tags (List[Tag], optional): 帖子标签
         title (str): 帖子标题
 
     返回:
         int: 帖子 ID
     '''
     ...
 
@@ -531,34 +540,34 @@
 async def apost(
     me: 'Me',
     *,
     artists: Optional[str]=None,
     category_id: str,
     category_name: str,
     chart: Optional[Chart]=None,
-    content: list[Content],
+    content: List[Content],
     diff: Optional[Literal[0, 1, 2, 3, 4]]=None,
     level: Optional[int]=None,
     song: Optional[Union[CustomSong, ProvidedSong]]=None,
-    tags: Optional[list[Tag]]=None,
+    tags: Optional[List[Tag]]=None,
     title: Optional[str]=None
 ) -> int:
     '''发表帖子
 
     参数:
         me (Me): 自身用户对象
         artists (Optional[str], optional): 歌手
         category_id (str): 帖子画廊 ID
         category_name (str): 帖子画廊名称
         chart (Optional[Chart], optional): 谱面
-        content (list[Content]): 帖子内容
+        content (List[Content]): 帖子内容
         diff (Optional[Literal[0, 1, 2, 3, 4]], optional): 难度
         level (Optional[int], optional): 等级
         song (Optional[Union[CustomSong, ProvidedSong]], optional): 歌曲
-        tags (Optional[list[Tag]], optional): 帖子标签
+        tags (Optional[List[Tag]], optional): 帖子标签
         title (Optional[str], optional): 帖子标题
 
     返回:
         int: 帖子 ID
     '''
     ...
 
@@ -658,15 +667,15 @@
         '''社区帖子类
 
         参数:
             id (int): 社区帖子 ID
         '''
         self.id: int = id
         '''社区帖子 ID'''
-        self.__post: dict[str, Any] = {}
+        self.__post: Dict[str, Any] = {}
         '''社区帖子详细内容'''
         return
     
     # 谱面对象
     @property
     def chart(self) -> Chart:
         '''谱面对象'''
@@ -674,15 +683,15 @@
         if (chart := post.get('chart', None)) is not None:
             return Chart.normalize(chart)
         else:
             raise PostHasNoChartError(post)
     
     # 帖子标签
     @property
-    def tags(self) -> list[Tag]:
+    def tags(self) -> List[Tag]:
         '''帖子标签'''
         if (tags := self.__post.get('tags', None)) is not None:
             return [Tag(tag) for tag in tags]
         else:
             return []
     
     # 帖子内容
@@ -697,86 +706,86 @@
                 elif seg.get('type', None) == 'emoji':
                     result += f':{seg.get("data", "")}:'
                 elif seg.get('type', None) == 'br':
                     result += '\n'
         return result
     
     # 获取帖子基础信息
-    def get_basic(self) -> dict[str, Any]:
+    def get_basic(self) -> Dict[str, Any]:
         '''获取帖子基础信息
 
         返回:
-            dict[str, Any]: 基础信息
+            Dict[str, Any]: 基础信息
         '''
         response = Api(API['post']['basic']).get(params={'id': self.id,})
         return response.json()
     
     # 异步获取帖子基础信息
-    async def get_basic_async(self) -> dict[str, Any]:
+    async def get_basic_async(self) -> Dict[str, Any]:
         '''获取帖子基础信息
 
         返回:
-            dict[str, Any]: 基础信息
+            Dict[str, Any]: 基础信息
         '''
         response = await Api(API['post']['basic']).aget(params={'id': self.id,})
         if isinstance(response, Response):
             return response.json()
         else:
             return await response.json()
     
     # 获取帖子信息
-    def get_details(self) -> dict[str, Any]:
+    def get_details(self) -> Dict[str, Any]:
         '''获取帖子信息
 
         返回:
-            dict[str, Any]: 帖子详细信息
+            Dict[str, Any]: 帖子详细信息
         '''
         response = Api(API['post']['details']).get(params={'id': self.id,})
         if (post := response.json().get('post', None)) is not None:
             self.__post = dict(post)
         else:
             raise NoDataException('帖子信息')
         return self.__post
     
     # 异步获取帖子信息
-    async def get_details_async(self) -> dict[str, Any]:
+    async def get_details_async(self) -> Dict[str, Any]:
         '''获取帖子信息
 
         返回:
-            dict[str, Any]: 帖子详细信息
+            Dict[str, Any]: 帖子详细信息
         '''
         response = await Api(API['post']['details']).aget(params={'id': self.id,})
         if isinstance(response, Response):
             _data = response.json()
         else:
             _data = await response.json()
         
         if (post := _data.get('post', None)) is not None:
             self.__post = dict(post)
         else:
             raise NoDataException('帖子信息')
         return self.__post
     
     # 获取缓存信息
-    def __get_post_cache(self) -> dict[str, Any]:
+    def __get_post_cache(self) -> Dict[str, Any]:
         '''获取缓存信息
 
         返回:
-            dict[str, Any]: 缓存信息
+            Dict[str, Any]: 缓存信息
         '''
         if not self.__post:
             self.get_details()
         return self.__post
     
     # 异步获取缓存信息
-    async def __get_post_cache_async(self) -> dict[str, Any]:
+    async def __get_post_cache_async(self) -> Dict[str, Any]:
         '''获取缓存信息
 
         返回:
-            dict[str, Any]: 缓存信息
+            Dict[str, Any]: 缓存信息
         '''
         if not self.__post:
             await self.get_details_async()
         return self.__post
     
     # 获取歌曲信息对象
     def get_song(self) -> SongRes:
@@ -788,15 +797,15 @@
         post = self.__get_post_cache()
         if (song := post.get('song', None)) is None:
             raise PostHasNoSongError(post)
         
         if (type := song.get('type', None)) is None:
             raise TypeError('该帖子没有歌曲类型。')
         
-        result: dict[str, Union[bytes, None]] = {}
+        result: Dict[str, Union[bytes, None]] = {}
         if type == 'custom': # 自定义歌曲
             # 获取歌曲音频
             if (audio := song.get('audio', None)) is None:
                 result['audio'] = None
             else:
                 response = Api(audio).get()
                 result['audio'] = response.content
@@ -870,15 +879,15 @@
         post = await self.__get_post_cache_async()
         if (song := post.get('song', None)) is None:
             raise PostHasNoSongError(post)
         
         if (type := song.get('type', None)) is None:
             raise TypeError('该帖子没有歌曲类型。')
         
-        result: dict[str, Union[bytes, None]] = {}
+        result: Dict[str, Union[bytes, None]] = {}
         if type == 'custom': # 自定义歌曲
             # 获取歌曲音频
             if (audio := song.get('audio', None)) is None:
                 result['audio'] = None
             else:
                 response = await Api(audio).aget()
                 if isinstance(response, Response):
@@ -959,29 +968,29 @@
     
     # 获取帖子评论
     def get_comment(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取帖子评论
 
         参数:
             limit (int, optional): 展示出的评论数，默认为 20
             offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
 
         返回:
-            dict[str, Any]: 搜索结果
+            Dict[str, Any]: 搜索结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的评论总数
-                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                    "posts": ... # List[Dict[str, Any]] 列举出的评论
                 }
                 ```
         '''
         return get_list(
             category_name='POST_COMMENT',
             category_id=str(self.id),
             order=order,
@@ -991,65 +1000,65 @@
     
     # 异步获取帖子评论
     async def get_comment_async(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取帖子评论
 
         参数:
             limit (int, optional): 展示出的评论数，默认为 20
             offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
 
         返回:
-            dict[str, Any]: 搜索结果
+            Dict[str, Any]: 搜索结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的评论总数
-                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                    "posts": ... # List[Dict[str, Any]] 列举出的评论
                 }
                 ```
         '''
         return await get_list_async(
             category_name='POST_COMMENT',
             category_id=str(self.id),
             order=order,
             limit=limit,
             offset=offset
         )
     
     # 评论帖子
-    def comment(self, me: 'Me', content: list[Content]) -> int:
+    def comment(self, me: 'Me', content: List[Content]) -> int:
         '''评论帖子
 
         参数:
             me (Me): 自身用户对象
-            content (list[Content]): 评论内容
+            content (List[Content]): 评论内容
 
         返回:
             int: 评论 ID
         '''
         return post(
             me,
             category_id=str(self.id),
             category_name='POST_COMMENT',
             content=content
         )
     
     # 异步评论帖子
-    async def acomment(self, me: 'Me', content: list[Content]) -> int:
+    async def acomment(self, me: 'Me', content: List[Content]) -> int:
         '''评论帖子
 
         参数:
             me (Me): 自身用户对象
-            content (list[Content]): 评论内容
+            content (List[Content]): 评论内容
 
         返回:
             int: 评论 ID
         '''
         return await apost(
             me,
             category_id=str(self.id),
```

### Comparing `bestdori-api-1.1.1/bestdori/settings.py` & `bestdori-api-1.1.2/bestdori/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 '''`bestdori.settings` 设置项'''
 
-from enum import StrEnum
-from typing import TYPE_CHECKING, Union, Optional
+from enum import Enum
+from typing import TYPE_CHECKING, Dict, Union, Optional
 
 from http.cookies import SimpleCookie
 
 from .exceptions import NoCookiesError
 
 if TYPE_CHECKING:
     from .user import Me
 
-class AsyncClient(StrEnum):
+class AsyncClient(str, Enum):
     '''异步客户端'''
     HTTPX = 'httpx'
     AIO_HTTP = 'aiohttp'
 
-proxy: Optional[Union[dict[str, str], str]] = None
+proxy: Optional[Union[Dict[str, str], str]] = None
 '''代理服务器
 
 若想要使用代理，则必须设置该选项，
 因为 `bestdori` 将会在内部默认无视系统环境下的代理设置
 '''
 async_client: AsyncClient = AsyncClient.HTTPX
 '''异步客户端
```

### Comparing `bestdori-api-1.1.1/bestdori/songmeta.py` & `bestdori-api-1.1.2/bestdori/songmeta.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 '''`bestdori.songmeta`
 
 BanG Dream! 歌曲 Meta 相关操作'''
-from typing import Any, Literal
+from typing import Any, Dict, Literal
 
 from httpx import Response
 
 from .utils.utils import API
 from .utils.network import Api
 
 # 获取总歌曲 Meta 信息
-def get_all(index: Literal[5]=5) -> dict[str, dict[str, Any]]:
+def get_all(index: Literal[5]=5) -> Dict[str, Dict[str, Any]]:
     '''获取总歌曲 Meta 信息
 
     参数:
         index (Literal[5], optional): 指定获取哪种 `all.json`
             `5`: 获取所有已有歌曲 Meta 信息 `all.5.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总歌曲 Meta 信息
+        Dict[str, Dict[str, Any]]: 获取到的总歌曲 Meta 信息
     '''
     return Api(API['all']['meta'].format(index=index)).get().json()
 
 # 异步获取总歌曲 Meta 信息
-async def get_all_async(index: Literal[5]=5) -> dict[str, dict[str, Any]]:
+async def get_all_async(index: Literal[5]=5) -> Dict[str, Dict[str, Any]]:
     '''获取总歌曲 Meta 信息
 
     参数:
         index (Literal[5], optional): 指定获取哪种 `all.json`
             `5`: 获取所有已有歌曲 Meta 信息 `all.5.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总歌曲 Meta 信息
+        Dict[str, Dict[str, Any]]: 获取到的总歌曲 Meta 信息
     '''
     response = await Api(API['all']['meta'].format(index=index)).aget()
     if isinstance(response, Response):
         return response.json()
     else:
         return await response.json()
```

### Comparing `bestdori-api-1.1.1/bestdori/songs.py` & `bestdori-api-1.1.2/bestdori/songs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''`bestdori.songs`
 
 BanG Dream! 歌曲相关操作'''
-from typing import Any, Literal
+from typing import Any, Dict, List, Literal
 
 from aiohttp import ClientResponseError
 from httpx import Response, HTTPStatusError
 
 from .charts import Chart
 from .utils.utils import API, ASSETS
 from .utils.network import Api, Assets
@@ -13,40 +13,40 @@
 from .exceptions import (
     NoDataException,
     DiffNotExistError,
     SongNotExistError
 )
 
 # 获取总歌曲信息
-def get_all(index: Literal[0, 5, 7]=5) -> dict[str, dict[str, Any]]:
+def get_all(index: Literal[0, 5, 7]=5) -> Dict[str, Dict[str, Any]]:
     '''获取总歌曲信息
 
     参数:
         index (Literal[0, 5], optional): 指定获取哪种 `all.json`
             `0`: 仅获取所有已有歌曲 ID `all.0.json`
             `5`: 获取所有已有歌曲的简洁信息 `all.5.json`，默认为该项
             `7`: 获取所有已有歌曲的较为详细信息 `all.7.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总歌曲信息
+        Dict[str, Dict[str, Any]]: 获取到的总歌曲信息
     '''
     return Api(API['songs']['all'].format(index=index)).get().json()
 
 # 异步获取总歌曲信息
-async def get_all_async(index: Literal[0, 5, 7]=5) -> dict[str, dict[str, Any]]:
+async def get_all_async(index: Literal[0, 5, 7]=5) -> Dict[str, Dict[str, Any]]:
     '''获取总歌曲信息
 
     参数:
         index (Literal[0, 5], optional): 指定获取哪种 `all.json`
             `0`: 仅获取所有已有歌曲 ID `all.0.json`
             `5`: 获取所有已有歌曲的简洁信息 `all.5.json`，默认为该项
             `7`: 获取所有已有歌曲的较为详细信息 `all.7.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总歌曲信息
+        Dict[str, Dict[str, Any]]: 获取到的总歌曲信息
     '''
     response = await Api(API['songs']['all'].format(index=index)).aget()
     if isinstance(response, Response):
         return response.json()
     else:
         return await response.json()
 
@@ -114,24 +114,24 @@
         '''歌曲类
 
         参数:
             id (int): 歌曲 ID
         '''
         self.id: int = id
         '''歌曲 ID'''
-        self.__info: dict[str, Any] = {}
+        self.__info: Dict[str, Any] = {}
         '''歌曲信息'''
         return
     
     # 获取歌曲信息
-    def get_info(self) -> dict[str, Any]:
+    def get_info(self) -> Dict[str, Any]:
         '''获取歌曲信息
 
         返回:
-            dict[str, Any]: 歌曲详细信息
+            Dict[str, Any]: 歌曲详细信息
         '''
         try:
             response = Api(
                 API['songs']['info'].format(id=self.id)
             ).get()
         except HTTPStatusError as exception:
             if exception.response.status_code == 404:
@@ -139,19 +139,19 @@
             else:
                 raise exception
         
         self.__info = dict(response.json())
         return self.__info
     
     # 异步获取歌曲信息
-    async def get_info_async(self) -> dict[str, Any]:
+    async def get_info_async(self) -> Dict[str, Any]:
         '''获取歌曲信息
 
         返回:
-            dict[str, Any]: 歌曲详细信息
+            Dict[str, Any]: 歌曲详细信息
         '''
         try:
             response = await Api(
                 API['songs']['info'].format(id=self.id)
             ).aget()
         except HTTPStatusError as exception:
             if exception.response.status_code == 404:
@@ -199,27 +199,27 @@
         try:
             return next(filter(lambda x: x is not None, music_title))
         except StopIteration:
             raise NoDataException('歌曲名称')
     
     # 歌曲封面
     @property
-    def jacket(self) -> list[Jacket]:
+    def jacket(self) -> List[Jacket]:
         '''歌曲封面'''
         # 获取数据包序列号
         quotient, remainder = divmod(self.id, 10)
         if remainder == 0:
             index = self.id
         else:
             index = (quotient + 1) * 10
         
         info = self.__info
         if (jacket_image := info.get('jacketImage', None)) is None:
             raise NoDataException('歌曲封面资源')
-        jacket: list[Jacket] = []
+        jacket: List[Jacket] = []
         
         for image in jacket_image:
             jacket.append(Jacket(index, image, self.server))
         
         return jacket
     
     # 获取歌曲谱面
@@ -294,29 +294,29 @@
     
     # 获取歌曲评论
     def get_comment(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取歌曲评论
 
         参数:
             limit (int, optional): 展示出的评论数，默认为 20
             offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
 
         返回:
-            dict[str, Any]: 搜索结果
+            Dict[str, Any]: 搜索结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的评论总数
-                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                    "posts": ... # List[Dict[str, Any]] 列举出的评论
                 }
                 ```
         '''
         return get_list(
             category_name='SONG_COMMENT',
             category_id=str(self.id),
             order=order,
@@ -326,29 +326,29 @@
     
     # 异步获取歌曲评论
     async def get_comment_async(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取歌曲评论
 
         参数:
             limit (int, optional): 展示出的评论数，默认为 20
             offset (int, optional): 忽略前面的 `offset` 条评论，默认为 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 排序顺序，默认时间顺序
 
         返回:
-            dict[str, Any]: 搜索结果
+            Dict[str, Any]: 搜索结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的评论总数
-                    "posts": ... # list[dict[str, Any]] 列举出的评论
+                    "posts": ... # List[Dict[str, Any]] 列举出的评论
                 }
                 ```
         '''
         return await get_list_async(
             category_name='SONG_COMMENT',
             category_id=str(self.id),
             order=order,
```

### Comparing `bestdori-api-1.1.1/bestdori/upload.py` & `bestdori-api-1.1.2/bestdori/upload.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.1/bestdori/user.py` & `bestdori-api-1.1.2/bestdori/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''`bestdori.user`
 
 BanG Dream! 歌曲相关操作'''
 from http.cookies import SimpleCookie
-from typing import Any, Literal, Optional
+from typing import Any, Dict, Literal, Optional
 
 from httpx import Response
 
 from . import settings
 from .utils.utils import API
 from .utils.network import Api
 from .post import get_list, get_list_async
@@ -23,37 +23,37 @@
         '''用户类
 
         参数:
             username (str): 用户名
         '''        
         self.username: str = username
         '''用户名'''
-        self.__info: dict[str, Any] = {}
+        self.__info: Dict[str, Any] = {}
         '''用户信息'''
         return
     
     # 获取用户详细信息
-    def get_info(self) -> dict[str, Any]:
+    def get_info(self) -> Dict[str, Any]:
         '''获取用户详细信息
 
         返回:
-            dict[str, Any]: 用户详细信息
+            Dict[str, Any]: 用户详细信息
         '''
         response = Api(
             API['user']['info']
         ).get(params={'username': self.username})
         self.__info = dict(response.json())
         return self.__info
     
     # 异步获取用户详细信息
-    async def get_info_async(self) -> dict[str, Any]:
+    async def get_info_async(self) -> Dict[str, Any]:
         '''获取用户详细信息
 
         返回:
-            dict[str, Any]: 用户详细信息
+            Dict[str, Any]: 用户详细信息
         '''
         response = await Api(
             API['user']['info']
         ).aget(params={'username': self.username})
         if isinstance(response, Response):
             self.__info = dict(response.json())
         else:
@@ -62,85 +62,85 @@
     
     # 获取用户帖子
     def get_posts(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_DESC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取用户帖子
 
         参数:
             limit (int, optional): 展示出的帖子数，默认 20
             offset (int, optional): 忽略前面的 `offset` 个帖子，默认 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 帖子排序，默认时间倒序
 
         返回:
-            dict[str, Any]: 获取结果
+            Dict[str, Any]: 获取结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的帖子总数
-                    "posts": ... # list[dict[str, Any]] 列举出的帖子
+                    "posts": ... # List[Dict[str, Any]] 列举出的帖子
                 }
                 ```
         '''
         return get_list(
             username=self.username, limit=limit, offset=offset, order=order
         )
     
     # 异步获取用户帖子
     async def get_posts_async(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_DESC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取用户帖子
 
         参数:
             limit (int, optional): 展示出的帖子数，默认 20
             offset (int, optional): 忽略前面的 `offset` 个帖子，默认 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 帖子排序，默认时间倒序
 
         返回:
-            dict[str, Any]: 获取结果
+            Dict[str, Any]: 获取结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的帖子总数
-                    "posts": ... # list[dict[str, Any]] 列举出的帖子
+                    "posts": ... # List[Dict[str, Any]] 列举出的帖子
                 }
                 ```
         '''
         return await get_list_async(
             username=self.username, limit=limit, offset=offset, order=order
         )
     
     # 获取用户谱面
     def get_charts(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_DESC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取用户谱面
 
         参数:
             limit (int, optional): 展示出的谱面数，默认 20
             offset (int, optional): 忽略前面的 `offset` 个谱面，默认 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 谱面排序，默认时间倒序
 
         返回:
-            dict[str, Any]: 获取结果
+            Dict[str, Any]: 获取结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的谱面总数
-                    "posts": ... # list[dict[str, Any]] 列举出的谱面
+                    "posts": ... # List[Dict[str, Any]] 列举出的谱面
                 }
                 ```
         '''
         return get_list(
             username=self.username,
             category_name='SELF_POST',
             category_id='chart',
@@ -151,29 +151,29 @@
     
     # 异步获取用户谱面
     async def get_charts_async(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_DESC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取用户谱面
 
         参数:
             limit (int, optional): 展示出的谱面数，默认 20
             offset (int, optional): 忽略前面的 `offset` 个谱面，默认 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 谱面排序，默认时间倒序
 
         返回:
-            dict[str, Any]: 获取结果
+            Dict[str, Any]: 获取结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的谱面总数
-                    "posts": ... # list[dict[str, Any]] 列举出的谱面
+                    "posts": ... # List[Dict[str, Any]] 列举出的谱面
                 }
                 ```
         '''
         return await get_list_async(
             username=self.username,
             category_name='SELF_POST',
             category_id='chart',
@@ -184,29 +184,29 @@
     
     # 获取用户文本帖子
     def get_texts(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_DESC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取用户文本帖子
 
         参数:
             limit (int, optional): 展示出的帖子数，默认 20
             offset (int, optional): 忽略前面的 `offset` 个帖子，默认 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 帖子排序，默认时间倒序
 
         返回:
-            dict[str, Any]: 获取结果
+            Dict[str, Any]: 获取结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的帖子总数
-                    "posts": ... # list[dict[str, Any]] 列举出的帖子
+                    "posts": ... # List[Dict[str, Any]] 列举出的帖子
                 }
                 ```
         '''
         return get_list(
             username=self.username,
             category_name='SELF_POST',
             category_id='text',
@@ -217,29 +217,29 @@
     
     # 异步获取用户文本帖子
     async def get_texts_async(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_DESC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取用户文本帖子
 
         参数:
             limit (int, optional): 展示出的帖子数，默认 20
             offset (int, optional): 忽略前面的 `offset` 个帖子，默认 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 帖子排序，默认时间倒序
 
         返回:
-            dict[str, Any]: 获取结果
+            Dict[str, Any]: 获取结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的帖子总数
-                    "posts": ... # list[dict[str, Any]] 列举出的帖子
+                    "posts": ... # List[Dict[str, Any]] 列举出的帖子
                 }
                 ```
         '''
         return await get_list_async(
             username=self.username,
             category_name='SELF_POST',
             category_id='text',
@@ -250,29 +250,29 @@
     
     # 获取用户故事
     def get_storys(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_DESC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取用户故事
 
         参数:
             limit (int, optional): 展示出的故事数，默认 20
             offset (int, optional): 忽略前面的 `offset` 个故事，默认 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 故事排序，默认时间倒序
 
         返回:
-            dict[str, Any]: 获取结果
+            Dict[str, Any]: 获取结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的故事总数
-                    "posts": ... # list[dict[str, Any]] 列举出的故事
+                    "posts": ... # List[Dict[str, Any]] 列举出的故事
                 }
                 ```
         '''
         return get_list(
             username=self.username,
             category_name='SELF_POST',
             category_id='story',
@@ -283,29 +283,29 @@
     
     # 异步获取用户故事
     async def get_storys_async(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_DESC'
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         '''获取用户故事
 
         参数:
             limit (int, optional): 展示出的故事数，默认 20
             offset (int, optional): 忽略前面的 `offset` 个故事，默认 0
             order (Literal[&#39;TIME_DESC&#39;, &#39;TIME_ASC&#39;], optional): 故事排序，默认时间倒序
 
         返回:
-            dict[str, Any]: 获取结果
+            Dict[str, Any]: 获取结果
                 ```python
                 {
                     "result": ... # bool 是否有响应
                     "count": ... # int 搜索到的故事总数
-                    "posts": ... # list[dict[str, Any]] 列举出的故事
+                    "posts": ... # List[Dict[str, Any]] 列举出的故事
                 }
                 ```
         '''
         return await get_list_async(
             username=self.username,
             category_name='SELF_POST',
             category_id='story',
@@ -331,15 +331,15 @@
             password (str): 密码
         '''
         super().__init__(username)
         self.password: str = password
         '''密码'''
         self.__cookies: Optional[SimpleCookie] = None
         '''用户 Cookies'''
-        self.__me: dict[str, Any] = {}
+        self.__me: Dict[str, Any] = {}
         '''用户自我信息'''
         return
     
     # 用户登录
     @classmethod
     def login(cls, username: str, password: str) -> 'Me':
         '''用户登录
@@ -389,31 +389,31 @@
     def cookies(self) -> SimpleCookie:
         '''获取用户 Cookies'''
         if self.__cookies is None:
             raise ValueError(f'用户 {self.username} 未登录。')
         return self.__cookies
     
     # 获取用户自我信息
-    def me(self) -> dict[str, Any]:
+    def me(self) -> Dict[str, Any]:
         '''获取用户自我信息
 
         返回:
-            dict[str, Any]: 自我信息
+            Dict[str, Any]: 自我信息
         '''
         if len(self.__me) == 0:
             response = Api(API['user']['me']).get(cookies=self.cookies)
             self.__me = dict(response.json())
         return self.__me
     
     # 异步获取用户自我信息
-    async def ame(self) -> dict[str, Any]:
+    async def ame(self) -> Dict[str, Any]:
         '''获取用户自我信息
 
         返回:
-            dict[str, Any]: 自我信息
+            Dict[str, Any]: 自我信息
         '''
         if len(self.__me) == 0:
             response = await Api(API['user']['me']).aget(cookies=self.cookies)
             if isinstance(response, Response):
                 self.__me = dict(response.json())
             else:
                 self.__me = dict(await response.json())
```

### Comparing `bestdori-api-1.1.1/bestdori/utils/__init__.py` & `bestdori-api-1.1.2/bestdori/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 '''`bestdori.utils`
 
 杂项模块'''
-from typing import Literal, Any
+from typing import Literal, Any, Dict, Tuple
 
 from httpx import Response
 
 from .utils import API, RES,ASSETS
 from .network import Api, Res, Assets
 from bestdori.exceptions import (
     AssetsNotExistError
 )
 
 # 将十六进制颜色代码转换为 RGB 元组
-def hexto_rgb(hex: str) -> tuple[int, int, int]:
+def hexto_rgb(hex: str) -> Tuple[int, int, int]:
     '''将十六进制颜色代码转换为 RGB 元组
 
     参数:
         hex (str): 十六进制颜色代码
 
     返回:
-        tuple[int, int, int]: RGB 元组
+        Tuple[int, int, int]: RGB 元组
     '''
     if hex[0] == '#':
         hex = hex[1:]
     if len(hex) == 3:
         hex = hex[0] * 2 + hex[1] * 2 + hex[2] * 2
     rgb = tuple(int(hex[i:i+2], 16) for i in (0, 2, 4))
     if len(rgb) != 3:
@@ -77,92 +77,92 @@
     '''
     try:
         return await Assets(ASSETS['thumb']['degree'].format(degree_name=degree_name), server).aget()
     except AssetsNotExistError:
         raise AssetsNotExistError(f'称号 {degree_name}-{server}')
 
 # 获取总技能信息
-def get_skill_all(index: Literal[10]=10) -> dict[str, dict[str, Any]]:
+def get_skill_all(index: Literal[10]=10) -> Dict[str, Dict[str, Any]]:
     '''获取总技能信息
 
     参数:
         index (Literal[10], optional): 指定获取哪种 `all.json`
             `10`: 获取所有已有技能的信息 `all.5.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总技能信息
+        Dict[str, Dict[str, Any]]: 获取到的总技能信息
     '''
     return Api(API['all']['skills'].format(index=index)).get().json()
 
 # 异步获取总技能信息
-async def get_skill_all_async(index: Literal[10]=10) -> dict[str, dict[str, Any]]:
+async def get_skill_all_async(index: Literal[10]=10) -> Dict[str, Dict[str, Any]]:
     '''获取总技能信息
 
     参数:
         index (Literal[10], optional): 指定获取哪种 `all.json`
             `10`: 获取所有已有技能的信息 `all.5.json`
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总技能信息
+        Dict[str, Dict[str, Any]]: 获取到的总技能信息
     '''
     response = await Api(API['all']['skills'].format(index=index)).aget()
     if isinstance(response, Response): return response.json()
     return await response.json()
 
 # 获取总乐队信息
-def get_bands_all(index: Literal[1]=1) -> dict[str, dict[str, Any]]:
+def get_bands_all(index: Literal[1]=1) -> Dict[str, Dict[str, Any]]:
     '''获取总乐队信息
 
     参数:
         index (Literal[1], optional): 指定获取哪种 `all.json`
             `1`: 获取所有已有乐队的名称信息 `all.1.json`，默认为该项
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总乐队信息
+        Dict[str, Dict[str, Any]]: 获取到的总乐队信息
     '''
     return Api(API['bands']['all'].format(index=index)).get().json()
 
 # 异步获取总乐队信息
-async def get_bands_all_async(index: Literal[1]=1) -> dict[str, dict[str, Any]]:
+async def get_bands_all_async(index: Literal[1]=1) -> Dict[str, Dict[str, Any]]:
     '''获取总乐队信息
 
     参数:
         index (Literal[1], optional): 指定获取哪种 `all.json`
             `1`: 获取所有已有乐队的名称信息 `all.1.json`，默认为该项
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的总乐队信息
+        Dict[str, Dict[str, Any]]: 获取到的总乐队信息
     '''
     response = await Api(API['bands']['all'].format(index=index)).aget()
     if isinstance(response, Response): return response.json()
     return await response.json()
 
 # 获取主要乐队信息
-def get_bands_main(index: Literal[1]=1) -> dict[str, dict[str, Any]]:
+def get_bands_main(index: Literal[1]=1) -> Dict[str, Dict[str, Any]]:
     '''获取主要乐队信息
 
     参数:
         index (Literal[1], optional): 指定获取哪种 `main.json`
             `1`: 获取所有主要乐队的名称信息 `main.1.json`，默认为该项
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的主要乐队信息
+        Dict[str, Dict[str, Any]]: 获取到的主要乐队信息
     '''
     return Api(API['bands']['main'].format(index=index)).get().json()
 
 # 异步获取主要乐队信息
-async def get_bands_main_async(index: Literal[1]=1) -> dict[str, dict[str, Any]]:
+async def get_bands_main_async(index: Literal[1]=1) -> Dict[str, Dict[str, Any]]:
     '''获取主要乐队信息
 
     参数:
         index (Literal[1], optional): 指定获取哪种 `main.json`
             `1`: 获取所有主要乐队的名称信息 `main.1.json`，默认为该项
 
     返回:
-        dict[str, dict[str, Any]]: 获取到的主要乐队信息
+        Dict[str, Dict[str, Any]]: 获取到的主要乐队信息
     '''
     response = await Api(API['bands']['main'].format(index=index)).aget()
     if isinstance(response, Response): return response.json()
     return await response.json()
 
 # 获取乐队 logo
 def get_band_logo(
```

### Comparing `bestdori-api-1.1.1/bestdori/utils/network.py` & `bestdori-api-1.1.2/bestdori/utils/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''`bestdori.utils.network`
 
 向 Bestdori 发送请求相关模块'''
 from json import dumps
 from io import BufferedReader
 from http.cookies import SimpleCookie
-from typing import Any, Union, Literal, Optional, cast
+from typing import Any, Dict, Tuple, Union, Literal, Optional, cast
 
 from httpx import HTTPStatusError
 from aiohttp import ClientResponseError
 from aiohttp import ClientSession, ClientResponse
 from httpx import Client, Request, Response, AsyncClient
 
 from bestdori import settings
@@ -24,17 +24,17 @@
     '''向 Bestdori 发送 API 请求类
 
     参数:
         api (str): 请求的 API 地址
     '''
     api: str
     '''请求的 API 地址'''
-    headers: dict[str, str]
+    headers: Dict[str, str]
     '''请求头'''
-    _proxies: Optional[dict[str, str]] = None
+    _proxies: Optional[Dict[str, str]] = None
     '''代理服务器'''
     # 初始化
     def __init__(
         self,
         api: str
     ) -> None:
         '''初始化'''
@@ -60,26 +60,26 @@
     
     # 请求发送
     def _request(
         self,
         method: Literal['get', 'post'],
         *,
         cookies: Optional[SimpleCookie]=None,
-        params: Optional[dict[str, Any]]=None,
-        data: Optional[dict[str, Any]]=None,
-        files: Optional[dict[str, tuple[str, BufferedReader]]]=None
+        params: Optional[Dict[str, Any]]=None,
+        data: Optional[Dict[str, Any]]=None,
+        files: Optional[Dict[str, Tuple[str, BufferedReader]]]=None
     ) -> Response:
         '''请求发送
 
         参数:
             method (Literal[&#39;get&#39;, &#39;post&#39;]): API 调用方法
             cookies (Optional[Cookies], optional): Cookies
-            params (Optional[dict[str, Any]], optional): 调用参数
-            data (Optional[dict[str, Any]], optional): 调用参数，将以 `json` 字符串形式发送
-            files (Optional[dict[str, tuple[str, BufferedReader]]], optional): 发送文件参数
+            params (Optional[Dict[str, Any]], optional): 调用参数
+            data (Optional[Dict[str, Any]], optional): 调用参数，将以 `json` 字符串形式发送
+            files (Optional[Dict[str, Tuple[str, BufferedReader]]], optional): 发送文件参数
 
         返回:
             Response: 收到的响应
         '''
         # 构建一个请求体
         request = Request(
             method,
@@ -123,26 +123,26 @@
     
     # 异步请求发送
     async def _request_async(
         self,
         method: Literal['get', 'post'],
         *,
         cookies: Optional[SimpleCookie]=None,
-        params: Optional[dict[str, Any]]=None,
-        data: Optional[dict[str, Any]]=None,
-        files: Optional[dict[str, tuple[str, BufferedReader]]]=None
+        params: Optional[Dict[str, Any]]=None,
+        data: Optional[Dict[str, Any]]=None,
+        files: Optional[Dict[str, Tuple[str, BufferedReader]]]=None
     ) -> Union[Response, ClientResponse]:
         '''请求发送
 
         参数:
             method (Literal[&#39;get&#39;, &#39;post&#39;]): API 调用方法
             cookies (Optional[Cookies], optional): Cookies
-            params (Optional[dict[str, Any]], optional): 调用参数
-            data (Optional[dict[str, Any]], optional): 调用参数，将以 `json` 字符串形式发送
-            files (Optional[dict[str, tuple[str, BufferedReader]]], optional): 发送文件参数
+            params (Optional[Dict[str, Any]], optional): 调用参数
+            data (Optional[Dict[str, Any]], optional): 调用参数，将以 `json` 字符串形式发送
+            files (Optional[Dict[str, Tuple[str, BufferedReader]]], optional): 发送文件参数
 
         返回:
             Union[Response, ClientResponse]: 收到的响应
         '''
         if settings.async_client == settings.AsyncClient.HTTPX:
             # 构建一个请求体
             request = Request(
@@ -198,76 +198,76 @@
                         raise RequestException(self.api)
         return response
     
     def get(
         self,
         *,
         cookies: Optional[SimpleCookie]=None,
-        params: Optional[dict[str, Any]]=None
+        params: Optional[Dict[str, Any]]=None
     ) -> Response:
         '''发送 GET 请求
 
         参数:
             cookies (Optional[Cookies], optional): Cookies
-            params (Optional[dict[str, Any]], optional): 调用参数
+            params (Optional[Dict[str, Any]], optional): 调用参数
 
         返回:
             Response: 收到的响应
         '''
         return self._request('get', cookies=cookies, params=params)
     
     def post(
         self,
         *,
         cookies: Optional[SimpleCookie]=None,
-        data: Optional[dict[str, Any]]=None,
-        files: Optional[dict[str, tuple[str, BufferedReader]]]=None
+        data: Optional[Dict[str, Any]]=None,
+        files: Optional[Dict[str, Tuple[str, BufferedReader]]]=None
     ) -> Response:
         '''发送 POST 请求
 
         参数:
             cookies (Optional[Cookies], optional): Cookies
-            data (Optional[dict[str, Any]], optional): 调用参数，将以 `json` 字符串形式发送
-            files (Optional[dict[str, tuple[str, BufferedReader]]], optional): 发送文件参数
+            data (Optional[Dict[str, Any]], optional): 调用参数，将以 `json` 字符串形式发送
+            files (Optional[Dict[str, Tuple[str, BufferedReader]]], optional): 发送文件参数
 
         返回:
             Response: 收到的响应
         '''
         return self._request('post', cookies=cookies, data=data, files=files)
 
     async def aget(
         self,
         *,
         cookies: Optional[SimpleCookie]=None,
-        params: Optional[dict[str, Any]]=None
+        params: Optional[Dict[str, Any]]=None
     ) -> Union[Response, ClientResponse]:
         '''发送 GET 请求
 
         参数:
             cookies (Optional[Cookies], optional): Cookies
-            params (Optional[dict[str, Any]], optional): 调用参数
+            params (Optional[Dict[str, Any]], optional): 调用参数
 
         返回:
             Union[Response, ClientResponse]: 收到的响应
         '''
         return await self._request_async('get', cookies=cookies, params=params)
     
     async def apost(
         self,
         *,
         cookies: Optional[SimpleCookie]=None,
-        data: Optional[dict[str, Any]]=None,
-        files: Optional[dict[str, tuple[str, BufferedReader]]]=None
+        data: Optional[Dict[str, Any]]=None,
+        files: Optional[Dict[str, Tuple[str, BufferedReader]]]=None
     ) -> Union[Response, ClientResponse]:
         '''发送 POST 请求
 
         参数:
             cookies (Optional[Cookies], optional): Cookies
-            data (Optional[dict[str, Any]], optional): 调用参数，将以 `json` 字符串形式发送
-            files (Optional[dict[str, tuple[str, BufferedReader]]], optional): 发送文件参数
+            data (Optional[Dict[str, Any]], optional): 调用参数，将以 `json` 字符串形式发送
+            files (Optional[Dict[str, Tuple[str, BufferedReader]]], optional): 发送文件参数
 
         返回:
             Union[Response, ClientResponse]: 收到的响应
         '''
         return await self._request_async('post', cookies=cookies, data=data, files=files)
 
 # 获取 Bestdori 资源数据
@@ -278,15 +278,15 @@
         url (str): 请求的资源地址
         server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]): 资源所在服务器
     '''
     url: str
     '''请求的资源地址'''
     server: Literal['jp', 'en', 'tw', 'cn', 'kr', 'llsif']
     '''资源所在服务器'''
-    _proxies: Optional[dict[str, str]] = None
+    _proxies: Optional[Dict[str, str]] = None
     '''代理服务器'''
     # 初始化
     def __init__(
         self,
         url: str,
         server: Literal['jp', 'en', 'tw', 'cn', 'kr', 'llsif']
     ) -> None:
@@ -496,15 +496,15 @@
     '''获取 Bestdori res 资源数据
 
     参数:
         url (str): 请求的 res 资源地址
     '''
     url: str
     '''请求的资源地址'''
-    _proxies: Optional[dict[str, str]]=None
+    _proxies: Optional[Dict[str, str]]=None
     '''代理服务器'''
     # 初始化
     def __init__(
         self,
         url: str
     ) -> None:
         '''获取 Bestdori 资源数据
```

### Comparing `bestdori-api-1.1.1/bestdori/utils/utils.py` & `bestdori-api-1.1.2/bestdori/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.1/bestdori_api.egg-info/PKG-INFO` & `bestdori-api-1.1.2/bestdori_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bestdori-api
-Version: 1.1.1
+Version: 1.1.2
 Summary: Bestdori 的各种 API 调用整合，另外附带部分功能
 Home-page: https://github.com/WindowsSov8forUs/bestdori-api
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bestdori-api Version: 1.1.1 Summary: Bestdori
+Metadata-Version: 2.1 Name: bestdori-api Version: 1.1.2 Summary: Bestdori
 çåç§ API è°ç¨æ´åï¼å¦å¤éå¸¦é¨ååè½ Home-page: https://
 github.com/WindowsSov8forUs/bestdori-api Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
   ![bestdori-api logo](https://github.com/WindowsSov8forUs/bestdori-api/blob/
 main/logo.png) # Bestdori-api _â¨ [Bestdori](https://bestdori.com/) çåç§
          API è°ç¨æ´åï¼å¦å¤éå¸¦é¨ååè½ â¨_ **:warning:
         è¯¥é¡¹ç®ä»ç¶æ¥éæ´æ°ä¸ Debug ï¼ä½¿ç¨æ¶è¥éå° Bug
```

### Comparing `bestdori-api-1.1.1/bestdori_api.egg-info/SOURCES.txt` & `bestdori-api-1.1.2/bestdori_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bestdori-api-1.1.1/setup.py` & `bestdori-api-1.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='bestdori-api',
-    version='1.1.1',
+    version='1.1.2',
     author='WindowsSov8',
     author_email='qwertyuiop2333@hotmail.com',
     description='Bestdori 的各种 API 调用整合，另外附带部分功能',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/WindowsSov8forUs/bestdori-api',
     include_package_data=False,
@@ -18,11 +18,12 @@
     classifiers=[
         'Programming Language :: Python :: 3.8',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent'
     ],
     python_requires='>=3.8',
     install_requires=[
-        'httpx>=0.18.2',
-        'aiohttp>=3.7.4'
+        'httpx>=0.22.0',
+        'aiohttp>=3.8.1',
+        'typing_extensions>=4.5.0'
     ]
 )
```

