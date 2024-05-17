# Comparing `tmp/nonebot_plugin_tsugu_bangdream_bot-0.1.2.tar.gz` & `tmp/nonebot_plugin_tsugu_bangdream_bot-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_tsugu_bangdream_bot-0.1.2.tar", last modified: Thu May 16 09:12:19 2024, max compression
+gzip compressed data, was "nonebot_plugin_tsugu_bangdream_bot-0.1.3.tar", last modified: Fri May 17 12:03:24 2024, max compression
```

## Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.2.tar` & `nonebot_plugin_tsugu_bangdream_bot-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1067 2024-05-16 09:11:54.024756 nonebot_plugin_tsugu_bangdream_bot-0.1.2/LICENSE
--rw-r--r--   0        0        0     6707 2024-05-16 09:11:54.024756 nonebot_plugin_tsugu_bangdream_bot-0.1.2/README.md
--rw-r--r--   0        0        0    36040 2024-05-16 09:11:54.024756 nonebot_plugin_tsugu_bangdream_bot-0.1.2/nonebot_plugin_tsugu_bangdream_bot/__init__.py
--rw-r--r--   0        0        0    13194 2024-05-16 09:11:54.024756 nonebot_plugin_tsugu_bangdream_bot-0.1.2/nonebot_plugin_tsugu_bangdream_bot/_commands.py
--rw-r--r--   0        0        0     7847 2024-05-16 09:11:54.024756 nonebot_plugin_tsugu_bangdream_bot-0.1.2/nonebot_plugin_tsugu_bangdream_bot/_utils.py
--rw-r--r--   0        0        0     1586 2024-05-16 09:11:54.024756 nonebot_plugin_tsugu_bangdream_bot-0.1.2/nonebot_plugin_tsugu_bangdream_bot/config.py
--rw-r--r--   0        0        0      569 2024-05-16 09:12:19.141057 nonebot_plugin_tsugu_bangdream_bot-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     7147 1970-01-01 00:00:00.000000 nonebot_plugin_tsugu_bangdream_bot-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-17 12:03:01.749841 nonebot_plugin_tsugu_bangdream_bot-0.1.3/LICENSE
+-rw-r--r--   0        0        0     6710 2024-05-17 12:03:01.749841 nonebot_plugin_tsugu_bangdream_bot-0.1.3/README.md
+-rw-r--r--   0        0        0    36185 2024-05-17 12:03:01.749841 nonebot_plugin_tsugu_bangdream_bot-0.1.3/nonebot_plugin_tsugu_bangdream_bot/__init__.py
+-rw-r--r--   0        0        0    13194 2024-05-17 12:03:01.749841 nonebot_plugin_tsugu_bangdream_bot-0.1.3/nonebot_plugin_tsugu_bangdream_bot/_commands.py
+-rw-r--r--   0        0        0     7847 2024-05-17 12:03:01.749841 nonebot_plugin_tsugu_bangdream_bot-0.1.3/nonebot_plugin_tsugu_bangdream_bot/_utils.py
+-rw-r--r--   0        0        0     1586 2024-05-17 12:03:01.749841 nonebot_plugin_tsugu_bangdream_bot-0.1.3/nonebot_plugin_tsugu_bangdream_bot/config.py
+-rw-r--r--   0        0        0      569 2024-05-17 12:03:24.965947 nonebot_plugin_tsugu_bangdream_bot-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     7150 1970-01-01 00:00:00.000000 nonebot_plugin_tsugu_bangdream_bot-0.1.3/PKG-INFO
```

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.2/LICENSE` & `nonebot_plugin_tsugu_bangdream_bot-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.2/README.md` & `nonebot_plugin_tsugu_bangdream_bot-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
-**nonebot-plugin-tsugu-bangdream-bot** 并无必填配置，但扔建议对部分配置进行添加。
+**nonebot-plugin-tsugu-bangdream-bot** 并无必填配置，但仍然建议对部分配置进行添加。
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | TSUGU_USE_EASY_BG | 否 | `False` | 是否使用简易背景，启用这将大幅提高速度，关闭将使部分界面效果更美观 |
 | TSUGU_COMPRESS | 否 | `False` | 是否压缩图片，启用会使图片质量下降，但是体积会减小，从而减少图片传输时所需的时间 |
 | TSUGU_BANDORI_STATION_TOKEN | 否 | `None` | BandoriStationToken, 用于发送车牌，可以去 [BandoriStation](https://github.com/maborosh/BandoriStation/wiki/API%E6%8E%A5%E5%8F%A3) 申请。缺失情况下，视为Tsugu车牌 |
 | TSUGU_REPLY | 否 | `False` | 消息是否回复用户 |
```

#### html2text {}

```diff
@@ -19,16 +19,16 @@
 pip pip install nonebot-plugin-tsugu-bangdream-bot pdm pdm add nonebot-plugin-
 tsugu-bangdream-bot poetry poetry add nonebot-plugin-tsugu-bangdream-bot conda
 conda install nonebot-plugin-tsugu-bangdream-bot æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
 é¨åè¿½å åå¥ plugins = ["nonebot-plugin-tsugu-bangdream-bot"] ## âï¸
 éç½® å¨ nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½®
 **nonebot-plugin-tsugu-bangdream-bot**
-å¹¶æ å¿å¡«éç½®ï¼ä½æå»ºè®®å¯¹é¨åéç½®è¿è¡æ·»å ã | éç½®é¡¹ |
-å¿å¡« | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| |
+å¹¶æ å¿å¡«éç½®ï¼ä½ä»ç¶å»ºè®®å¯¹é¨åéç½®è¿è¡æ·»å ã | éç½®é¡¹
+| å¿å¡« | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| |
 TSUGU_USE_EASY_BG | å¦ | `False` |
 æ¯å¦ä½¿ç¨ç®æèæ¯ï¼å¯ç¨è¿å°å¤§å¹æé«éåº¦ï¼å³é­å°ä½¿é¨åçé¢æææ´ç¾è§
 | | TSUGU_COMPRESS | å¦ | `False` |
 æ¯å¦åç¼©å¾çï¼å¯ç¨ä¼ä½¿å¾çè´¨éä¸éï¼ä½æ¯ä½ç§¯ä¼åå°ï¼ä»èåå°å¾çä¼ è¾æ¶æéçæ¶é´
 | | TSUGU_BANDORI_STATION_TOKEN | å¦ | `None` | BandoriStationToken,
 ç¨äºåéè½¦çï¼å¯ä»¥å» [BandoriStation](https://github.com/maborosh/
 BandoriStation/wiki/API%E6%8E%A5%E5%8F%A3)
```

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.2/nonebot_plugin_tsugu_bangdream_bot/__init__.py` & `nonebot_plugin_tsugu_bangdream_bot-0.1.3/nonebot_plugin_tsugu_bangdream_bot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, List, Tuple, Union, Optional
 
 from nonebot.log import logger
 from nonebot.adapters import Bot, Event, Message
-from nonebot.plugin import PluginMetadata, require
 from nonebot.params import RegexGroup, ArgPlainText
 from nonebot import on_regex, get_driver, get_plugin_config
+from nonebot.plugin import PluginMetadata, require, inherit_supported_adapters
 
 require("nonebot_plugin_alconna")
 
 from nonebot.typing import T_State
 from nonebot_plugin_alconna import load_builtin_plugin
 from nonebot_plugin_alconna import Command, Arparma, Extension, store_true
 from nonebot_plugin_alconna.uniseg import At, Text, Image, Reply, Segment, UniMessage
@@ -93,14 +93,26 @@
                 send = Reply(message_id) + send
             except:
                 pass
         return send
 
 config = get_plugin_config(Config)
 
+__plugin_meta__ = PluginMetadata(
+    name="nonebot-plugin-tsugu-bangdream-bot",
+    description="Koishi-Plugin-Tsugu-BanGDream-Bot 的 NoneBot2 实现",
+    usage="\n".join([f"{key}: {value}" for key, value in USAGES.items()]),
+    type="application",
+    homepage="https://github.com/WindowsSov8forUs/nonebot-plugin-tsugu-bangdream-bot",
+    config=Config,
+    supported_adapters=inherit_supported_adapters(
+        "nonebot_plugin_alconna", "nonebot_plugin_userinfo"
+    )
+)
+
 if "httpx" in get_driver().type:
     tsugu_api_async.settings.client = tsugu_api_async.settings.Client.HTTPX
 elif "aiohttp" in get_driver().type:
     tsugu_api_async.settings.client = tsugu_api_async.settings.Client.AIO_HTTP
 
 tsugu_api_async.settings.use_easy_bg = config.tsugu_use_easy_bg
 tsugu_api_async.settings.compress = config.tsugu_compress
@@ -1000,16 +1012,7 @@
     for _r in response:
         if isinstance(_r, str):
             segments.append(Text(_r))
         else:
             segments.append(Image(raw=_r))
     
     await gacha_simulate.finish(UniMessage(segments))
-
-__plugin_meta__ = PluginMetadata(
-    name="nonebot-plugin-tsugu-bangdream-bot",
-    description="Koishi-Plugin-Tsugu-BanGDream-Bot 的 NoneBot2 实现",
-    usage="\n".join([f"{key}: {value}" for key, value in USAGES.items()]),
-    type="application",
-    homepage="https://github.com/WindowsSov8forUs/nonebot-plugin-tsugu-bangdream-bot",
-    config=Config,
-)
```

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.2/nonebot_plugin_tsugu_bangdream_bot/_commands.py` & `nonebot_plugin_tsugu_bangdream_bot-0.1.3/nonebot_plugin_tsugu_bangdream_bot/_commands.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.2/nonebot_plugin_tsugu_bangdream_bot/_utils.py` & `nonebot_plugin_tsugu_bangdream_bot-0.1.3/nonebot_plugin_tsugu_bangdream_bot/_utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.2/nonebot_plugin_tsugu_bangdream_bot/config.py` & `nonebot_plugin_tsugu_bangdream_bot-0.1.3/nonebot_plugin_tsugu_bangdream_bot/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.2/pyproject.toml` & `nonebot_plugin_tsugu_bangdream_bot-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-tsugu-bangdream-bot"
-version = "0.1.2"
+version = "0.1.3"
 description = "Koishi-Plugin-Tsugu-BanGDream-Bot 的 NoneBot2 实现"
 authors = [
     { name = "WindowsSov8forUs", email = "qwertyuiop2333@hotmail.com" },
 ]
 dependencies = [
     "nonebot2>=2.2.1",
     "nonebot-plugin-alconna>=0.42.4",
```

### Comparing `nonebot_plugin_tsugu_bangdream_bot-0.1.2/PKG-INFO` & `nonebot_plugin_tsugu_bangdream_bot-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-tsugu-bangdream-bot
-Version: 0.1.2
+Version: 0.1.3
 Summary: Koishi-Plugin-Tsugu-BanGDream-Bot 的 NoneBot2 实现
 Author-Email: WindowsSov8forUs <qwertyuiop2333@hotmail.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: nonebot2>=2.2.1
 Requires-Dist: nonebot-plugin-alconna>=0.42.4
 Requires-Dist: tsugu-api-python>=1.1.7
@@ -88,15 +88,15 @@
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
-**nonebot-plugin-tsugu-bangdream-bot** 并无必填配置，但扔建议对部分配置进行添加。
+**nonebot-plugin-tsugu-bangdream-bot** 并无必填配置，但仍然建议对部分配置进行添加。
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | TSUGU_USE_EASY_BG | 否 | `False` | 是否使用简易背景，启用这将大幅提高速度，关闭将使部分界面效果更美观 |
 | TSUGU_COMPRESS | 否 | `False` | 是否压缩图片，启用会使图片质量下降，但是体积会减小，从而减少图片传输时所需的时间 |
 | TSUGU_BANDORI_STATION_TOKEN | 否 | `None` | BandoriStationToken, 用于发送车牌，可以去 [BandoriStation](https://github.com/maborosh/BandoriStation/wiki/API%E6%8E%A5%E5%8F%A3) 申请。缺失情况下，视为Tsugu车牌 |
 | TSUGU_REPLY | 否 | `False` | 消息是否回复用户 |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-tsugu-bangdream-bot Version: 0.1.2
+Metadata-Version: 2.1 Name: nonebot-plugin-tsugu-bangdream-bot Version: 0.1.3
 Summary: Koishi-Plugin-Tsugu-BanGDream-Bot ç NoneBot2 å®ç° Author-Email:
 WindowsSov8forUs
 hotmail.com> License: MIT Requires-Python: >=3.8 Requires-Dist: nonebot2>=2.2.1
 Requires-Dist: nonebot-plugin-alconna>=0.42.4 Requires-Dist: tsugu-api-
 python>=1.1.7 Requires-Dist: nonebot-plugin-userinfo>=0.2.4 Description-
 Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
@@ -26,16 +26,16 @@
 pip pip install nonebot-plugin-tsugu-bangdream-bot pdm pdm add nonebot-plugin-
 tsugu-bangdream-bot poetry poetry add nonebot-plugin-tsugu-bangdream-bot conda
 conda install nonebot-plugin-tsugu-bangdream-bot æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
 é¨åè¿½å åå¥ plugins = ["nonebot-plugin-tsugu-bangdream-bot"] ## âï¸
 éç½® å¨ nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½®
 **nonebot-plugin-tsugu-bangdream-bot**
-å¹¶æ å¿å¡«éç½®ï¼ä½æå»ºè®®å¯¹é¨åéç½®è¿è¡æ·»å ã | éç½®é¡¹ |
-å¿å¡« | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| |
+å¹¶æ å¿å¡«éç½®ï¼ä½ä»ç¶å»ºè®®å¯¹é¨åéç½®è¿è¡æ·»å ã | éç½®é¡¹
+| å¿å¡« | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| |
 TSUGU_USE_EASY_BG | å¦ | `False` |
 æ¯å¦ä½¿ç¨ç®æèæ¯ï¼å¯ç¨è¿å°å¤§å¹æé«éåº¦ï¼å³é­å°ä½¿é¨åçé¢æææ´ç¾è§
 | | TSUGU_COMPRESS | å¦ | `False` |
 æ¯å¦åç¼©å¾çï¼å¯ç¨ä¼ä½¿å¾çè´¨éä¸éï¼ä½æ¯ä½ç§¯ä¼åå°ï¼ä»èåå°å¾çä¼ è¾æ¶æéçæ¶é´
 | | TSUGU_BANDORI_STATION_TOKEN | å¦ | `None` | BandoriStationToken,
 ç¨äºåéè½¦çï¼å¯ä»¥å» [BandoriStation](https://github.com/maborosh/
 BandoriStation/wiki/API%E6%8E%A5%E5%8F%A3)
```

