# Comparing `tmp/nonebot_plugin_steam_info-0.3.0.tar.gz` & `tmp/nonebot_plugin_steam_info-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_steam_info-0.3.0.tar", last modified: Fri May  3 14:26:02 2024, max compression
+gzip compressed data, was "nonebot_plugin_steam_info-1.0.0.tar", last modified: Fri May 17 15:02:11 2024, max compression
```

## Comparing `nonebot_plugin_steam_info-0.3.0.tar` & `nonebot_plugin_steam_info-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1062 2024-05-03 14:25:36.848723 nonebot_plugin_steam_info-0.3.0/LICENSE
--rw-r--r--   0        0        0     2560 2024-05-03 14:25:36.848723 nonebot_plugin_steam_info-0.3.0/README.md
--rw-r--r--   0        0        0    11166 2024-05-03 14:25:37.000723 nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/__init__.py
--rw-r--r--   0        0        0      209 2024-05-03 14:25:37.000723 nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/config.py
--rw-r--r--   0        0        0     6705 2024-05-03 14:25:37.000723 nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/data_source.py
--rw-r--r--   0        0        0    13658 2024-05-03 14:25:37.000723 nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/draw.py
--rw-r--r--   0        0        0      572 2024-05-03 14:25:37.000723 nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/models.py
--rw-r--r--   0        0        0      552 2024-05-03 14:25:37.000723 nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/res/busy.png
--rw-r--r--   0        0        0     1847 2024-05-03 14:25:37.000723 nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/res/friends_search.png
--rw-r--r--   0        0        0     8807 2024-05-03 14:25:37.000723 nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/res/gaming.png
--rw-r--r--   0        0        0     7467 2024-05-03 14:25:37.004723 nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/res/parent_status.png
--rw-r--r--   0        0        0     3409 2024-05-03 14:25:37.004723 nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/res/unknown_avatar.jpg
--rw-r--r--   0        0        0      533 2024-05-03 14:25:37.004723 nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/res/zzz_gaming.png
--rw-r--r--   0        0        0      536 2024-05-03 14:25:37.004723 nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/res/zzz_online.png
--rw-r--r--   0        0        0     1209 2024-05-03 14:25:37.004723 nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/steam.py
--rw-r--r--   0        0        0      580 2024-05-03 14:26:02.824605 nonebot_plugin_steam_info-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3027 1970-01-01 00:00:00.000000 nonebot_plugin_steam_info-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-17 15:01:46.905274 nonebot_plugin_steam_info-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2591 2024-05-17 15:01:46.905274 nonebot_plugin_steam_info-1.0.0/README.md
+-rw-r--r--   0        0        0    11775 2024-05-17 15:01:47.061274 nonebot_plugin_steam_info-1.0.0/nonebot_plugin_steam_info/__init__.py
+-rw-r--r--   0        0        0      209 2024-05-17 15:01:47.061274 nonebot_plugin_steam_info-1.0.0/nonebot_plugin_steam_info/config.py
+-rw-r--r--   0        0        0     8700 2024-05-17 15:01:47.061274 nonebot_plugin_steam_info-1.0.0/nonebot_plugin_steam_info/data_source.py
+-rw-r--r--   0        0        0    13784 2024-05-17 15:01:47.061274 nonebot_plugin_steam_info-1.0.0/nonebot_plugin_steam_info/draw.py
+-rw-r--r--   0        0        0     1041 2024-05-17 15:01:47.061274 nonebot_plugin_steam_info-1.0.0/nonebot_plugin_steam_info/models.py
+-rw-r--r--   0        0        0      552 2024-05-17 15:01:47.061274 nonebot_plugin_steam_info-1.0.0/nonebot_plugin_steam_info/res/busy.png
+-rw-r--r--   0        0        0     1847 2024-05-17 15:01:47.061274 nonebot_plugin_steam_info-1.0.0/nonebot_plugin_steam_info/res/friends_search.png
+-rw-r--r--   0        0        0     8807 2024-05-17 15:01:47.061274 nonebot_plugin_steam_info-1.0.0/nonebot_plugin_steam_info/res/gaming.png
+-rw-r--r--   0        0        0     7467 2024-05-17 15:01:47.061274 nonebot_plugin_steam_info-1.0.0/nonebot_plugin_steam_info/res/parent_status.png
+-rw-r--r--   0        0        0     3409 2024-05-17 15:01:47.061274 nonebot_plugin_steam_info-1.0.0/nonebot_plugin_steam_info/res/unknown_avatar.jpg
+-rw-r--r--   0        0        0      533 2024-05-17 15:01:47.061274 nonebot_plugin_steam_info-1.0.0/nonebot_plugin_steam_info/res/zzz_gaming.png
+-rw-r--r--   0        0        0      536 2024-05-17 15:01:47.061274 nonebot_plugin_steam_info-1.0.0/nonebot_plugin_steam_info/res/zzz_online.png
+-rw-r--r--   0        0        0     1565 2024-05-17 15:01:47.061274 nonebot_plugin_steam_info-1.0.0/nonebot_plugin_steam_info/steam.py
+-rw-r--r--   0        0        0      580 2024-05-17 15:02:11.617215 nonebot_plugin_steam_info-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3058 1970-01-01 00:00:00.000000 nonebot_plugin_steam_info-1.0.0/PKG-INFO
```

### Comparing `nonebot_plugin_steam_info-0.3.0/LICENSE` & `nonebot_plugin_steam_info-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.3.0/README.md` & `nonebot_plugin_steam_info-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Nonebot-Plugin-Steam-Info
 ✨ Steam 好友状态播报 NoneBot 插件 ✨
 
 ## 功能
 - [x] 绑定 Steam ID
 - [x] 群友状态变更播报
+- [x] 群友游戏时间播报
 - [x] 主动查询群友状态
 
 ## 预览
 仿照了 Steam 好友列表的样式
 
 ![image](./preview.png)
 ![image](./preview_1.png)
```

### Comparing `nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/__init__.py` & `nonebot_plugin_steam_info-1.0.0/nonebot_plugin_steam_info/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
+import time
 import aiohttp
 import nonebot
 from io import BytesIO
 from pathlib import Path
 from nonebot.log import logger
 from PIL import Image as PILImage
-from typing import Union, Optional
 from nonebot.params import Depends
 from nonebot.params import CommandArg
 from nonebot import on_command, require
+from typing import Union, Optional, List, Dict
 from nonebot.adapters import Message, Event, Bot
 from nonebot.plugin import PluginMetadata, inherit_supported_adapters
 
 require("nonebot_plugin_alconna")
 require("nonebot_plugin_localstore")
 require("nonebot_plugin_apscheduler")
 
 import nonebot_plugin_localstore as store
 from nonebot_plugin_apscheduler import scheduler
 from nonebot_plugin_alconna import Text, Image, UniMessage, Target
 
 from .config import Config
-from .models import PlayerSummaries, Player
+from .models import ProcessedPlayer
 from .steam import get_steam_id, get_steam_users_info, STEAM_ID_OFFSET
 from .data_source import BindData, SteamInfoData, ParentData, DisableParentData
 from .draw import (
     check_font,
     fetch_avatar,
     image_to_bytes,
     draw_start_gaming,
@@ -108,31 +109,38 @@
                 if resp.status != 200:
                     raise ValueError(f"无法获取图片数据: {resp.status}")
                 return await resp.read()
 
     raise ValueError("无法获取图片数据")
 
 
-async def broadcast_steam_info(parent_id: str, steam_info: PlayerSummaries):
+async def broadcast_steam_info(parent_id: str, old_players: List[ProcessedPlayer], new_players: List[ProcessedPlayer]):
     if disable_parent_data.is_disabled(parent_id):
         return None
 
     bot = nonebot.get_bot()
 
-    play_data = steam_info_data.compare(parent_id, steam_info["response"])
+    play_data = steam_info_data.compare(old_players, new_players)
 
     msg = []
     for entry in play_data:
-        player: Player = entry["player"]
-        old_player: Player = entry.get("old_player")
+        player: ProcessedPlayer = entry["player"]
+        old_player: ProcessedPlayer = entry.get("old_player")
 
         if entry["type"] == "start":
             msg.append(f"{player['personaname']} 开始玩 {player['gameextrainfo']} 了")
         elif entry["type"] == "stop":
-            msg.append(f"{player['personaname']} 停止玩 {old_player['gameextrainfo']} 了")
+            time_start = old_player["game_start_time"]
+            time_stop = time.time()
+            hours = int((time_stop - time_start) / 3600)
+            minutes = int((time_stop - time_start) % 3600 / 60)
+            time_str = f"{hours} 小时 {minutes} 分钟" if hours > 0 else f"{minutes} 分钟"
+            msg.append(
+                f"{player['personaname']} 玩了 {time_str} {old_player['gameextrainfo']} 后不玩了"
+            )
         elif entry["type"] == "change":
             msg.append(
                 f"{player['personaname']} 停止玩 {old_player['gameextrainfo']}，开始玩 {player['gameextrainfo']} 了"
             )
         elif entry["type"] == "error":
             f"出现错误！{player['personaname']}\nNew: {player.get('gameextrainfo')}\nOld: {old_player.get('gameextrainfo')}"
         else:
@@ -140,63 +148,71 @@
 
     if msg == []:
         return None
 
     if config.steam_broadcast_type == "all":
         steam_status_data = [
             await simplize_steam_player_data(player, config.proxy, avatar_path)
-            for player in steam_info["response"]["players"]
+            for player in new_players
         ]
 
         parent_avatar, parent_name = parent_data.get(parent_id)
         image = draw_friends_status(parent_avatar, parent_name, steam_status_data)
         uni_msg = UniMessage([Text("\n".join(msg)), Image(raw=image_to_bytes(image))])
     elif config.steam_broadcast_type == "part":
-        images = [draw_start_gaming((await fetch_avatar(entry["player"], avatar_path, config.proxy)), entry["player"]["personaname"], entry["player"]["gameextrainfo"]) for entry in play_data if entry["type"] == "start"]
+        images = [
+            draw_start_gaming(
+                (await fetch_avatar(entry["player"], avatar_path, config.proxy)),
+                entry["player"]["personaname"],
+                entry["player"]["gameextrainfo"],
+            )
+            for entry in play_data
+            if entry["type"] == "start"
+        ]
         if images == []:
             uni_msg = UniMessage([Text("\n".join(msg))])
         else:
-            image = vertically_concatenate_images(images) if len(images) > 1 else images[0]
-            uni_msg = UniMessage([Text("\n".join(msg)), Image(raw=image_to_bytes(image))])
+            image = (
+                vertically_concatenate_images(images) if len(images) > 1 else images[0]
+            )
+            uni_msg = UniMessage(
+                [Text("\n".join(msg)), Image(raw=image_to_bytes(image))]
+            )
     else:
         uni_msg = UniMessage([Text("\n".join(msg))])
 
     await uni_msg.send(
         Target(parent_id, parent_id, True, False, "", bot.adapter.get_name()), bot
     )
 
-
-@nonebot.get_driver().on_bot_connect
-async def init_steam_info():
-    for parent_id in bind_data.content:
-        steam_ids = bind_data.get_all(parent_id)
-
-        steam_info = await get_steam_users_info(
-            steam_ids, config.steam_api_key, config.proxy
-        )
-
-        steam_info_data.update(parent_id, steam_info["response"])
-        steam_info_data.save()
-
-
 @scheduler.scheduled_job(
     "interval", minutes=config.steam_request_interval / 60, id="update_steam_info"
 )
+@nonebot.get_driver().on_bot_connect
 async def update_steam_info():
-    for parent_id in bind_data.content:
+    steam_ids = bind_data.get_all_steam_id()
+
+    steam_info = await get_steam_users_info(
+        steam_ids, config.steam_api_key, config.proxy
+    )
+
+    old_players_dict: Dict[str, List[ProcessedPlayer]] = {}
+
+    for parent_id in bind_data.content.keys():
         steam_ids = bind_data.get_all(parent_id)
+        old_players_dict[parent_id] = steam_info_data.get_players(steam_ids)
 
-        steam_info = await get_steam_users_info(
-            steam_ids, config.steam_api_key, config.proxy
-        )
+    steam_info_data.update_by_players(steam_info["response"]["players"])
+    steam_info_data.save()
 
-        await broadcast_steam_info(parent_id, steam_info)
+    for parent_id in bind_data.content.keys():
+        old_players = old_players_dict[parent_id]
+        new_players = steam_info_data.get_players(bind_data.get_all(parent_id))
 
-        steam_info_data.update(parent_id, steam_info["response"])
-        steam_info_data.save()
+        await broadcast_steam_info(parent_id, old_players, new_players)
 
 
 @bind.handle()
 async def bind_handle(
     event: Event, target: Target = Depends(get_target), cmd_arg: Message = CommandArg()
 ):
     parent_id = target.parent_id or target.id
```

### Comparing `nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/draw.py` & `nonebot_plugin_steam_info-1.0.0/nonebot_plugin_steam_info/draw.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             if resp.status != 200:
                 return Image.open(unknown_avatar_path)
             return Image.open(BytesIO(await resp.read()))
 
 
 async def fetch_avatar(player: Player, avatar_dir: Path, proxy: str = None) -> Image.Image:
     if avatar_dir is not None:
-        avatar_path = avatar_dir / f"avatar_{player['steamid']}.png"
+        avatar_path = avatar_dir / f"avatar_{player['steamid']}_{player['avatarhash']}.png"
 
         if avatar_path.exists():
             avatar = Image.open(avatar_path)
         else:
             avatar = await _fetch_avatar(player["avatarfull"], proxy)
 
             avatar.save(avatar_path)
@@ -276,14 +276,17 @@
         fill=fill[1],
     )
 
     return canvas
 
 
 def draw_gaming_friends_status(data: List[Dict[str, str]]) -> Image.Image:
+    # 排序数据，按照游戏名称字母表顺序排序
+    data.sort(key=lambda x: x["status"])
+
     canvas = Image.new(
         "RGB",
         (WIDTH, 64 + (MEMBER_AVATAR_SIZE + 16) * len(data) + 16),
         hex_to_rgb("1e2024"),
     )
 
     draw = ImageDraw.Draw(canvas)
```

### Comparing `nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/models.py` & `nonebot_plugin_steam_info-1.0.0/nonebot_plugin_steam_info/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,7 +23,30 @@
 
 class PlayerSummariesResponse(TypedDict):
     players: List[Player]
 
 
 class PlayerSummaries(TypedDict):
     response: PlayerSummariesResponse
+
+
+class ProcessedPlayer(TypedDict):
+    steamid: str
+    communityvisibilitystate: int
+    personaname: str
+    profileurl: str
+    avatar: str
+    avatarmedium: str
+    avatarfull: str
+    avatarhash: str
+    lastlogoff: int
+    personastate: int
+    realname: str
+    primaryclanid: str
+    timecreated: int
+    personastateflags: int
+
+    game_start_time: int  # Unix timestamp
+
+
+class PlayerSummariesProcessedResponse(TypedDict):
+    players: List[ProcessedPlayer]
```

### Comparing `nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/res/busy.png` & `nonebot_plugin_steam_info-1.0.0/nonebot_plugin_steam_info/res/busy.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/res/friends_search.png` & `nonebot_plugin_steam_info-1.0.0/nonebot_plugin_steam_info/res/friends_search.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/res/gaming.png` & `nonebot_plugin_steam_info-1.0.0/nonebot_plugin_steam_info/res/gaming.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/res/parent_status.png` & `nonebot_plugin_steam_info-1.0.0/nonebot_plugin_steam_info/res/parent_status.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/res/unknown_avatar.jpg` & `nonebot_plugin_steam_info-1.0.0/nonebot_plugin_steam_info/res/unknown_avatar.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/res/zzz_gaming.png` & `nonebot_plugin_steam_info-1.0.0/nonebot_plugin_steam_info/res/zzz_gaming.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.3.0/nonebot_plugin_steam_info/res/zzz_online.png` & `nonebot_plugin_steam_info-1.0.0/nonebot_plugin_steam_info/res/zzz_online.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.3.0/pyproject.toml` & `nonebot_plugin_steam_info-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-steam-info"
-version = "0.3.0"
+version = "1.0.0"
 description = "Default template for PDM package"
 authors = [
     { name = "zhaomaoniu", email = "2667292003@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.2.0",
     "nonebot-plugin-alconna>=0.37.0",
```

### Comparing `nonebot_plugin_steam_info-0.3.0/PKG-INFO` & `nonebot_plugin_steam_info-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-steam-info
-Version: 0.3.0
+Version: 1.0.0
 Summary: Default template for PDM package
 Author-Email: zhaomaoniu <2667292003@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: nonebot2>=2.2.0
 Requires-Dist: nonebot-plugin-alconna>=0.37.0
 Requires-Dist: aiohttp>=3.9.3
@@ -15,14 +15,15 @@
 
 # Nonebot-Plugin-Steam-Info
 ✨ Steam 好友状态播报 NoneBot 插件 ✨
 
 ## 功能
 - [x] 绑定 Steam ID
 - [x] 群友状态变更播报
+- [x] 群友游戏时间播报
 - [x] 主动查询群友状态
 
 ## 预览
 仿照了 Steam 好友列表的样式
 
 ![image](./preview.png)
 ![image](./preview_1.png)
```

