# Comparing `tmp/matrix_rssbot-0.1.1.tar.gz` & `tmp/matrix_rssbot-0.1.2.tar.gz`

## Comparing `matrix_rssbot-0.1.1.tar` & `matrix_rssbot-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/config.dist.ini
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/pantalaimon.example.conf
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/pantalaimon_first_login.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/rssbot-pantalaimon.service
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/rssbot.service
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/src/matrix_rssbot/__init__.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/src/matrix_rssbot/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/src/matrix_rssbot/classes/__init__.py
--rw-r--r--   0        0        0    20806 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/src/matrix_rssbot/classes/bot.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/src/matrix_rssbot/classes/logging.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/src/matrix_rssbot/classes/callbacks/__init__.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/src/matrix_rssbot/classes/callbacks/invite.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/src/matrix_rssbot/classes/callbacks/message.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/src/matrix_rssbot/classes/callbacks/roommember.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/src/matrix_rssbot/classes/callbacks/sync.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/src/matrix_rssbot/classes/commands/__init__.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/src/matrix_rssbot/classes/commands/addfeed.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/src/matrix_rssbot/classes/commands/botinfo.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/src/matrix_rssbot/classes/commands/help.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/src/matrix_rssbot/classes/commands/listfeeds.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/src/matrix_rssbot/classes/commands/newroom.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/src/matrix_rssbot/classes/commands/privacy.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/src/matrix_rssbot/classes/commands/processfeeds.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/src/matrix_rssbot/classes/commands/removefeed.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/src/matrix_rssbot/classes/commands/unknown.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/LICENSE
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/README.md
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/config.dist.ini
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/pantalaimon_first_login.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/rssbot.service
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/contrib/pantalaimon.example.conf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/src/matrix_rssbot/__init__.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/src/matrix_rssbot/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/src/matrix_rssbot/classes/__init__.py
+-rw-r--r--   0        0        0    18809 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/src/matrix_rssbot/classes/bot.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/src/matrix_rssbot/classes/logging.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/src/matrix_rssbot/classes/callbacks/__init__.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/src/matrix_rssbot/classes/callbacks/invite.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/src/matrix_rssbot/classes/callbacks/message.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/src/matrix_rssbot/classes/callbacks/roommember.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/src/matrix_rssbot/classes/callbacks/sync.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/src/matrix_rssbot/classes/commands/__init__.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/src/matrix_rssbot/classes/commands/addfeed.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/src/matrix_rssbot/classes/commands/botinfo.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/src/matrix_rssbot/classes/commands/help.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/src/matrix_rssbot/classes/commands/listfeeds.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/src/matrix_rssbot/classes/commands/privacy.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/src/matrix_rssbot/classes/commands/processfeeds.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/src/matrix_rssbot/classes/commands/removefeed.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/src/matrix_rssbot/classes/commands/unknown.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/README.md
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 matrix_rssbot-0.1.2/PKG-INFO
```

### Comparing `matrix_rssbot-0.1.1/config.dist.ini` & `matrix_rssbot-0.1.2/config.dist.ini`

 * *Files 6% similar despite different names*

```diff
@@ -65,8 +65,14 @@
 AccessToken = syt_yoursynapsetoken
 
 # The Matrix user ID of the bot (@local:domain.tld)
 # Only specify this if the bot fails to figure it out by itself
 #
 # UserID = @rssbot:matrix.local
 
+# The event type to use for sending messages
+# Can be either "text" or "notice"
+# Defaults to "notice", can be overridden using the `eventtype` command
+#
+# EventType = notice
+
 ###############################################################################
```

### Comparing `matrix_rssbot-0.1.1/src/matrix_rssbot/__main__.py` & `matrix_rssbot-0.1.2/src/matrix_rssbot/__main__.py`

 * *Files identical despite different names*

### Comparing `matrix_rssbot-0.1.1/src/matrix_rssbot/classes/bot.py` & `matrix_rssbot-0.1.2/src/matrix_rssbot/classes/bot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,35 @@
 import asyncio
-import functools
 
 from nio import (
     AsyncClient,
     AsyncClientConfig,
     WhoamiResponse,
     DevicesResponse,
     Event,
     Response,
     MatrixRoom,
     Api,
-    RoomMessagesError,
-    GroupEncryptionError,
-    EncryptionError,
     RoomMessageText,
     RoomSendResponse,
     SyncResponse,
-    RoomMessageNotice,
     JoinError,
     RoomLeaveError,
     RoomSendError,
-    RoomVisibility,
-    RoomCreateError,
-    RoomMessageMedia,
-    RoomMessageImage,
-    RoomMessageFile,
-    RoomMessageAudio,
-    DownloadError,
-    DownloadResponse,
-    ToDeviceEvent,
-    ToDeviceError,
-    RoomPutStateError,
     RoomGetStateError,
 )
 
 from typing import Optional, List
 from configparser import ConfigParser
 from datetime import datetime
 from io import BytesIO
-from pathlib import Path
-from contextlib import closing
 
-import base64
 import uuid
 import traceback
 import json
-import importlib.util
-import sys
-import traceback
 
 import markdown2
 import feedparser
 
 from .logging import Logger
 from .callbacks import RESPONSE_CALLBACKS, EVENT_CALLBACKS
 from .commands import COMMANDS
@@ -82,18 +60,27 @@
         """List of users allowed to use the bot.
 
         Returns:
             List[str]: List of user IDs. Defaults to [], which means all users are allowed.
         """
         try:
             return json.loads(self.config["RSSBot"]["AllowedUsers"])
-        except:
+        except Exception:
             return []
 
     @property
+    def event_type(self) -> str:
+        """Event type of outgoing messages.
+
+        Returns:
+            str: The event type of outgoing messages. Either "text" or "notice".
+        """
+        return self.config["Matrix"].get("EventType", "notice")
+
+    @property
     def display_name(self) -> str:
         """Display name of the bot user.
 
         Returns:
             str: The display name of the bot user. Defaults to "RSSBot".
         """
         return self.config["RSSBot"].get("DisplayName", "RSSBot")
@@ -276,23 +263,23 @@
                     {
                         "msgtype": "m.notice",
                         "body": f"You are not allowed to use this bot. Please contact {self.operator} for more information.",
                     },
                 )
             return
 
-        task = asyncio.create_task(self._event_callback(room, event))
+        asyncio.create_task(self._event_callback(room, event))
 
     async def _response_callback(self, response: Response):
         for response_type, callback in RESPONSE_CALLBACKS.items():
             if isinstance(response, response_type):
                 await callback(response, self)
 
     async def response_callback(self, response: Response):
-        task = asyncio.create_task(self._response_callback(response))
+        asyncio.create_task(self._response_callback(response))
 
     async def accept_pending_invites(self):
         """Accept all pending invites."""
 
         assert self.matrix_client, "Matrix client not set up"
 
         invites = self.matrix_client.invited_rooms
@@ -351,97 +338,14 @@
 
         response, _ = await self.matrix_client.upload(
             bio, content_type=mime, filename=filename, filesize=len(file)
         )
 
         return response.content_uri
 
-    async def send_image(
-        self, room: MatrixRoom, image: bytes, message: Optional[str] = None
-    ):
-        """Send an image to a room.
-
-        Args:
-            room (MatrixRoom|str): The room to send the image to.
-            image (bytes): The image to send.
-            message (str, optional): The message to send with the image. Defaults to None.
-        """
-
-        if isinstance(room, MatrixRoom):
-            room = room.room_id
-
-        self.logger.log(
-            f"Sending image of size {len(image)} bytes to room {room}", "debug"
-        )
-
-        bio = BytesIO(image)
-        img = Image.open(bio)
-        mime = Image.MIME[img.format]
-
-        (width, height) = img.size
-
-        self.logger.log(
-            f"Uploading - Image size: {width}x{height} pixels, MIME type: {mime}",
-            "debug",
-        )
-
-        content_uri = await self.upload_file(image, "image", mime)
-
-        self.logger.log("Uploaded image - sending message...", "debug")
-
-        content = {
-            "body": message or "",
-            "info": {
-                "mimetype": mime,
-                "size": len(image),
-                "w": width,
-                "h": height,
-            },
-            "msgtype": "m.image",
-            "url": content_uri,
-        }
-
-        status = await self.matrix_client.room_send(room, "m.room.message", content)
-
-        self.logger.log("Sent image", "debug")
-
-    async def send_file(
-        self, room: MatrixRoom, file: bytes, filename: str, mime: str, msgtype: str
-    ):
-        """Send a file to a room.
-
-        Args:
-            room (MatrixRoom|str): The room to send the file to.
-            file (bytes): The file to send.
-            filename (str): The name of the file.
-            mime (str): The MIME type of the file.
-        """
-
-        if isinstance(room, MatrixRoom):
-            room = room.room_id
-
-        self.logger.log(
-            f"Sending file of size {len(file)} bytes to room {room}", "debug"
-        )
-
-        content_uri = await self.upload_file(file, filename, mime)
-
-        self.logger.log("Uploaded file - sending message...", "debug")
-
-        content = {
-            "body": filename,
-            "info": {"mimetype": mime, "size": len(file)},
-            "msgtype": msgtype,
-            "url": content_uri,
-        }
-
-        status = await self.matrix_client.room_send(room, "m.room.message", content)
-
-        self.logger.log("Sent file", "debug")
-
     async def send_message(
         self,
         room: MatrixRoom | str,
         message: str,
         notice: bool = False,
         msgtype: Optional[str] = None,
     ):
@@ -471,19 +375,16 @@
 
         else:
             msgcontent = {
                 "msgtype": msgtype,
                 "content": message,
             }
 
-        content = None
-
-        if not content:
-            msgtype = "m.room.message"
-            content = msgcontent
+        msgtype = "m.room.message"
+        content = msgcontent
 
         method, path, data = Api.room_send(
             self.matrix_client.access_token,
             room.room_id,
             msgtype,
             content,
             uuid.uuid4(),
@@ -524,14 +425,30 @@
             self.logger.log(f"Could not get state for room {room}")
 
         for event in state.events:
             if event["type"] == event_type:
                 if state_key is None or event["state_key"] == state_key:
                     return event
 
+    async def get_event_type_for_room(self, room: MatrixRoom) -> str:
+        """Returns the event type to use for a room
+
+        Either the default event type or the event type set in the room's state
+
+        Args:
+            room (MatrixRoom): The room to get the event type for
+
+        Returns:
+            str: The event type to use
+        """
+        state = await self.get_state_event(room, "rssbot.event_type")
+        if state:
+            return state["content"]["event_type"]
+        return self.event_type
+
     async def process_room(self, room):
         self.logger.log(f"Processing room {room}", "debug")
 
         state = await self.get_state_event(room, "rssbot.feeds")
 
         if not state:
             feeds = []
@@ -554,24 +471,28 @@
 
             try:
                 feed_content = feedparser.parse(feed)
                 new_timestamp = timestamp
                 for entry in feed_content.entries:
                     try:
                         entry_time_info = entry.published_parsed
-                    except:
+                    except Exception:
                         entry_time_info = entry.updated_parsed
 
                     entry_timestamp = int(datetime(*entry_time_info[:6]).timestamp())
 
                     self.logger.log(f"Entry timestamp identified as {entry_timestamp}")
 
                     if entry_timestamp > timestamp:
                         entry_message = f"__{feed_content.feed.title}: {entry.title}__\n\n{entry.description}\n\n{entry.link}"
-                        await self.send_message(room, entry_message)
+                        await self.send_message(
+                            room,
+                            entry_message,
+                            (await self.get_event_type_for_room(room)) == "notice",
+                        )
                         new_timestamp = max(entry_timestamp, new_timestamp)
 
                 await self.send_state_event(
                     room, "rssbot.feed_state", {"timestamp": new_timestamp}, feed
                 )
             except Exception as e:
                 self.logger.log(f"Error processing feed at {feed}: {e}")
```

### Comparing `matrix_rssbot-0.1.1/src/matrix_rssbot/classes/logging.py` & `matrix_rssbot-0.1.2/src/matrix_rssbot/classes/logging.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 
 class Logger:
     LOG_LEVELS = ["trace", "debug", "info", "warning", "error", "critical"]
 
     def __init__(self, log_level: str = "warning"):
         if log_level not in self.LOG_LEVELS:
             raise ValueError(
-                f"Invalid log level {log_level}. Valid levels are {', '.join(self.LOG_LEVELS)}")
+                f"Invalid log level {log_level}. Valid levels are {', '.join(self.LOG_LEVELS)}"
+            )
 
         self.log_level = log_level
 
     def log(self, message: str, log_level: str = "info"):
         if log_level not in self.LOG_LEVELS:
             raise ValueError(
-                f"Invalid log level {log_level}. Valid levels are {', '.join(self.LOG_LEVELS)}")
+                f"Invalid log level {log_level}. Valid levels are {', '.join(self.LOG_LEVELS)}"
+            )
 
         if self.LOG_LEVELS.index(log_level) < self.LOG_LEVELS.index(self.log_level):
             return
 
         caller = inspect.currentframe().f_back.f_code.co_name
         timestamp = datetime.now().strftime("%Y-%m-%d %H:%M:%S:%f")
         print(f"[{timestamp}] - {caller} - [{log_level.upper()}] {message}")
```

### Comparing `matrix_rssbot-0.1.1/src/matrix_rssbot/classes/callbacks/message.py` & `matrix_rssbot-0.1.2/src/matrix_rssbot/classes/callbacks/message.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 from nio import MatrixRoom, RoomMessageText
 
 from datetime import datetime
 
+
 async def message_callback(room: MatrixRoom | str, event: RoomMessageText, bot):
     bot.logger.log(f"Received message from {event.sender} in room {room.room_id}")
 
     sent = datetime.fromtimestamp(event.server_timestamp / 1000)
     received = datetime.now()
     latency = received - sent
 
     if event.sender == bot.matrix_client.user_id:
         bot.logger.log("Message is from bot itself - ignoring", "debug")
 
     elif event.body.startswith("!rssbot") or event.body.startswith("* !rssbot"):
         await bot.process_command(room, event)
 
     elif event.body.startswith("!"):
-        bot.logger.log(f"Received {event.body} - might be a command, but not for this bot - ignoring", "debug")
+        bot.logger.log(
+            f"Received {event.body} - might be a command, but not for this bot - ignoring",
+            "debug",
+        )
 
     else:
-        bot.logger.log(f"Received regular message - ignoring", "debug")
+        bot.logger.log("Received regular message - ignoring", "debug")
 
     processed = datetime.now()
     processing_time = processed - received
 
-    bot.logger.log(f"Message processing took {processing_time.total_seconds()} seconds (latency: {latency.total_seconds()} seconds)", "debug")
+    bot.logger.log(
+        f"Message processing took {processing_time.total_seconds()} seconds (latency: {latency.total_seconds()} seconds)",
+        "debug",
+    )
```

### Comparing `matrix_rssbot-0.1.1/src/matrix_rssbot/classes/commands/addfeed.py` & `matrix_rssbot-0.1.2/src/matrix_rssbot/classes/commands/addfeed.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from nio.events.room_events import RoomMessageText
 from nio import RoomPutStateError
 from nio.rooms import MatrixRoom
 
 from datetime import datetime
-from urllib.request import urlopen
 
 import feedparser
 
 
 async def command_addfeed(room: MatrixRoom, event: RoomMessageText, bot):
     url = event.body.split()[2]
 
@@ -22,19 +21,20 @@
 
     feeds.append(url)
 
     feeds = list(set(feeds))
 
     try:
         feedparser.parse(url)
-    except:
+    except Exception as e:
         await bot.send_state_event(
             f"Could not access or parse feed at {url}. Please ensure that you got the URL right, and that it is actually an RSS/Atom feed.",
             True,
         )
+        bot.logger.log(f"Could not access or parse feed at {url}: {e}", "error")
 
     try:
         response1 = await bot.send_state_event(
             room,
             "rssbot.feed_state",
             {"timestamp": int(datetime.now().timestamp())},
             url,
@@ -46,22 +46,29 @@
                     room,
                     "Unable to put status events into this room. Please ensure I have the required permissions, then try again.",
                 )
 
             await bot.send_message(
                 room, "Unable to write feed state to the room. Please try again.", True
             )
+            bot.logger.log(
+                f"Error adding feed to room {room.room_id}: {response1.error}", "error"
+            )
             return
 
         response2 = await bot.send_state_event(room, "rssbot.feeds", {"feeds": feeds})
 
         if isinstance(response2, RoomPutStateError):
             await bot.send_message(
                 room, "Unable to write feed list to the room. Please try again.", True
             )
+            bot.logger.log(
+                f"Error adding feed to room {room.room_id}: {response2.error}", "error"
+            )
             return
 
         await bot.send_message(room, f"Added {url} to this room's feeds.", True)
-    except:
+    except Exception as e:
         await bot.send_message(
-            room, "Sorry, something went wrong. Please try again.", true
+            room, "Sorry, something went wrong. Please try again.", True
         )
+        bot.logger.log(f"Error adding feed to room {room.room_id}: {e}", "error")
```

### Comparing `matrix_rssbot-0.1.1/src/matrix_rssbot/classes/commands/help.py` & `matrix_rssbot-0.1.2/src/matrix_rssbot/classes/commands/help.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,11 +7,10 @@
 
 - !rssbot help - Show this message
 - !rssbot botinfo - Show information about the bot
 - !rssbot privacy - Show privacy information
 - !rssbot addfeed \<url\> - Bridges a new feed to the current room
 - !rssbot listfeeds - Lists all bridged feeds
 - !rssbot removefeed \<index|url\> - Removes a bridged feed given the numeric index from the listfeeds command or the URL of the feed
-- !rssbot newroom \<room name\> - Create a new room and invite yourself to it
 """
 
     await bot.send_message(room, body, True)
```

### Comparing `matrix_rssbot-0.1.1/src/matrix_rssbot/classes/commands/listfeeds.py` & `matrix_rssbot-0.1.2/src/matrix_rssbot/classes/commands/listfeeds.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from nio.events.room_events import RoomMessageText
-from nio import RoomPutStateError
 from nio.rooms import MatrixRoom
 
 async def command_listfeeds(room: MatrixRoom, event: RoomMessageText, bot):
     state = await bot.get_state_event(room, "rssbot.feeds")
 
     if (not state) or (not state["content"]["feeds"]):
-        message = f"There are currently no feeds associated with this room."
+        message = "There are currently no feeds associated with this room."
     else:
         message = "This room is currently bridged to the following feeds:\n\n"
 
         for key, value in enumerate(state["content"]["feeds"]):
             message += f"- {key}: {value}\n"
 
     await bot.send_message(room, message, True)
```

### Comparing `matrix_rssbot-0.1.1/src/matrix_rssbot/classes/commands/removefeed.py` & `matrix_rssbot-0.1.2/src/matrix_rssbot/classes/commands/removefeed.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from nio.events.room_events import RoomMessageText
-from nio import RoomPutStateError
 from nio.rooms import MatrixRoom
 
 async def command_removefeed(room: MatrixRoom, event: RoomMessageText, bot):
     identifier = event.body.split()[2]
 
     state = await bot.get_state_event(room, "rssbot.feeds")
 
     if (not state) or (not state["content"]["feeds"]):
         feeds = []
     else:
         feeds = state["content"]["feeds"]
         
     if identifier.isnumeric():
         try:
-            feed = feeds.pop(int(identifier))
+            feeds.pop(int(identifier))
         except IndexError:
             await bot.send_message(room, f"There is no feed with index {identifier}.")
             return
     else:
         try:
             feeds.remove(identifier)
         except ValueError:
-            await bot.send_message(room, f"There is no bridged feed with the provided URL.")
+            await bot.send_message(room, "There is no bridged feed with the provided URL.")
             return
 
     await bot.send_state_event(room, "rssbot.feeds", {"feeds": feeds})
```

### Comparing `matrix_rssbot-0.1.1/LICENSE` & `matrix_rssbot-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `matrix_rssbot-0.1.1/README.md` & `matrix_rssbot-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `matrix_rssbot-0.1.1/pyproject.toml` & `matrix_rssbot-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,45 +3,41 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project]
 name = "matrix-rssbot"
-version = "0.1.1"
+version = "0.1.2"
 
-authors = [
-  { name="Private.coffee Team", email="support@private.coffee" },
-]
+authors = [{ name = "Private.coffee Team", email = "support@private.coffee" }]
 
 description = "Simple RSS feed bridge for Matrix"
 readme = "README.md"
-license = { file="LICENSE" }
+license = { file = "LICENSE" }
 requires-python = ">=3.10"
 
-packages = [
-    "src/matrix_rssbot"
-]
+packages = ["src/matrix_rssbot"]
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-    "matrix-nio",
-    "pantalaimon",
+    "matrix-nio>=0.24.0",
     "setuptools",
     "markdown2",
     "feedparser",
-    ]
+    "future>=1.0.0",
+]
 
 [project.urls]
 "Homepage" = "https://git.private.coffee/PrivateCoffee/matrix-rssbot"
 "Bug Tracker" = "https://git.private.coffee/PrivateCoffee/matrix-rssbot/issues"
 
 [project.scripts]
 rssbot = "matrix_rssbot.__main__:main"
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/matrix_rssbot"]
+packages = ["src/matrix_rssbot"]
```

### Comparing `matrix_rssbot-0.1.1/PKG-INFO` & `matrix_rssbot-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: matrix-rssbot
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple RSS feed bridge for Matrix
 Project-URL: Homepage, https://git.private.coffee/PrivateCoffee/matrix-rssbot
 Project-URL: Bug Tracker, https://git.private.coffee/PrivateCoffee/matrix-rssbot/issues
 Author-email: "Private.coffee Team" <support@private.coffee>
 License: Copyright (c) 2024 Private.coffee Team <support@private.coffee>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,17 +26,17 @@
         SOFTWARE.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: feedparser
+Requires-Dist: future>=1.0.0
 Requires-Dist: markdown2
-Requires-Dist: matrix-nio
-Requires-Dist: pantalaimon
+Requires-Dist: matrix-nio>=0.24.0
 Requires-Dist: setuptools
 Description-Content-Type: text/markdown
 
 # Matrix-RSSBot
 
 [![Support Private.coffee!](https://shields.private.coffee/badge/private.coffee-support%20us!-pink?logo=coffeescript)](https://private.coffee)
 [![PyPI](https://shields.private.coffee/pypi/v/matrix-rssbot)](https://pypi.org/project/matrix-rssbot/)
```

