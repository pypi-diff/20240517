# Comparing `tmp/xconn-0.2.0.tar.gz` & `tmp/xconn-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xconn-0.2.0.tar", last modified: Mon May 13 13:12:19 2024, max compression
+gzip compressed data, was "xconn-0.2.1.tar", last modified: Thu May 16 22:15:40 2024, max compression
```

## Comparing `xconn-0.2.0.tar` & `xconn-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-13 13:12:19.511291 xconn-0.2.0/
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1107 2024-05-10 21:55:47.000000 xconn-0.2.0/LICENSE
--rw-r--r--   0 om26er    (1000) om26er    (1000)     3098 2024-05-13 13:12:19.511291 xconn-0.2.0/PKG-INFO
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      771 2024-05-08 19:52:19.000000 xconn-0.2.0/README.md
--rw-r--r--   0 om26er    (1000) om26er    (1000)     2509 2024-05-13 13:11:29.000000 xconn-0.2.0/pyproject.toml
--rw-r--r--   0 om26er    (1000) om26er    (1000)       38 2024-05-13 13:12:19.511291 xconn-0.2.0/setup.cfg
-drwxr-xr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-13 13:12:19.511291 xconn-0.2.0/xconn/
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      181 2024-05-08 19:52:19.000000 xconn-0.2.0/xconn/__init__.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     2173 2024-05-08 19:52:19.000000 xconn-0.2.0/xconn/__main__.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1834 2024-05-08 19:52:19.000000 xconn-0.2.0/xconn/acceptor.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1079 2024-05-08 19:52:19.000000 xconn-0.2.0/xconn/app.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      574 2024-05-08 19:52:19.000000 xconn-0.2.0/xconn/client.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      968 2024-05-08 19:52:19.000000 xconn-0.2.0/xconn/helpers.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      978 2024-05-08 19:52:19.000000 xconn-0.2.0/xconn/joiner.py
--rw-r--r--   0 om26er    (1000) om26er    (1000)     2374 2024-05-13 13:11:29.000000 xconn-0.2.0/xconn/realm.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1307 2024-05-08 19:52:19.000000 xconn-0.2.0/xconn/router.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1686 2024-05-08 19:52:19.000000 xconn-0.2.0/xconn/server.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     9772 2024-05-08 19:52:19.000000 xconn-0.2.0/xconn/session.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     8545 2024-05-08 19:52:19.000000 xconn-0.2.0/xconn/types.py
-drwxr-xr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-13 13:12:19.511291 xconn-0.2.0/xconn.egg-info/
--rw-r--r--   0 om26er    (1000) om26er    (1000)     3098 2024-05-13 13:12:19.000000 xconn-0.2.0/xconn.egg-info/PKG-INFO
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      403 2024-05-13 13:12:19.000000 xconn-0.2.0/xconn.egg-info/SOURCES.txt
--rw-rw-r--   0 om26er    (1000) om26er    (1000)        1 2024-05-13 13:12:19.000000 xconn-0.2.0/xconn.egg-info/dependency_links.txt
--rw-rw-r--   0 om26er    (1000) om26er    (1000)       46 2024-05-13 13:12:19.000000 xconn-0.2.0/xconn.egg-info/entry_points.txt
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      110 2024-05-13 13:12:19.000000 xconn-0.2.0/xconn.egg-info/requires.txt
--rw-rw-r--   0 om26er    (1000) om26er    (1000)        6 2024-05-13 13:12:19.000000 xconn-0.2.0/xconn.egg-info/top_level.txt
+drwxrwxr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-16 22:15:40.562036 xconn-0.2.1/
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1107 2024-05-10 21:55:47.000000 xconn-0.2.1/LICENSE
+-rw-r--r--   0 om26er    (1000) om26er    (1000)     3098 2024-05-16 22:15:40.562036 xconn-0.2.1/PKG-INFO
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      771 2024-05-08 19:52:19.000000 xconn-0.2.1/README.md
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     2509 2024-05-16 22:14:40.000000 xconn-0.2.1/pyproject.toml
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)       38 2024-05-16 22:15:40.562036 xconn-0.2.1/setup.cfg
+drwxrwxr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-16 22:15:40.558036 xconn-0.2.1/xconn/
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      181 2024-05-08 19:52:19.000000 xconn-0.2.1/xconn/__init__.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     2173 2024-05-16 21:52:06.000000 xconn-0.2.1/xconn/__main__.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     2100 2024-05-16 22:13:18.000000 xconn-0.2.1/xconn/acceptor.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1079 2024-05-08 19:52:19.000000 xconn-0.2.1/xconn/app.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      574 2024-05-08 19:52:19.000000 xconn-0.2.1/xconn/client.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      968 2024-05-08 19:52:19.000000 xconn-0.2.1/xconn/helpers.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      978 2024-05-08 19:52:19.000000 xconn-0.2.1/xconn/joiner.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     2500 2024-05-16 21:39:09.000000 xconn-0.2.1/xconn/realm.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1307 2024-05-08 19:52:19.000000 xconn-0.2.1/xconn/router.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1686 2024-05-08 19:52:19.000000 xconn-0.2.1/xconn/server.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     9772 2024-05-08 19:52:19.000000 xconn-0.2.1/xconn/session.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     8822 2024-05-16 22:13:18.000000 xconn-0.2.1/xconn/types.py
+drwxrwxr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-16 22:15:40.562036 xconn-0.2.1/xconn.egg-info/
+-rw-r--r--   0 om26er    (1000) om26er    (1000)     3098 2024-05-16 22:15:40.000000 xconn-0.2.1/xconn.egg-info/PKG-INFO
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      403 2024-05-16 22:15:40.000000 xconn-0.2.1/xconn.egg-info/SOURCES.txt
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)        1 2024-05-16 22:15:40.000000 xconn-0.2.1/xconn.egg-info/dependency_links.txt
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)       46 2024-05-16 22:15:40.000000 xconn-0.2.1/xconn.egg-info/entry_points.txt
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      110 2024-05-16 22:15:40.000000 xconn-0.2.1/xconn.egg-info/requires.txt
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)        6 2024-05-16 22:15:40.000000 xconn-0.2.1/xconn.egg-info/top_level.txt
```

### Comparing `xconn-0.2.0/LICENSE` & `xconn-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xconn-0.2.0/PKG-INFO` & `xconn-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xconn
-Version: 0.2.0
+Version: 0.2.1
 Summary: https://github.com/xconnio/xconn-python
 Author-email: Omer Akram <omer@thing.com>, Mahad Munir <mahad@xconn.io>
 License: MIT License
         
         Copyright (c) 2024 Simple Things Inc.
         Copyright (c) 2024 XConnIO Ltd.
         
@@ -33,15 +33,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: websockets
-Requires-Dist: wampproto>=0.2.0
+Requires-Dist: wampproto>=0.2.1
 Requires-Dist: aiohttp
 Requires-Dist: uvloop
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 Requires-Dist: ruff; extra == "test"
```

### Comparing `xconn-0.2.0/README.md` & `xconn-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `xconn-0.2.0/pyproject.toml` & `xconn-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xconn"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   {name="Omer Akram", email="omer@thing.com"},
   {name="Mahad Munir", email="mahad@xconn.io"},
 ]
 description = "https://github.com/xconnio/xconn-python"
 readme = "README.md"
 license = {file = "LICENSE"}
 dependencies = [
   "websockets",
-  "wampproto>=0.2.0",
+  "wampproto>=0.2.1",
   "aiohttp",
   "uvloop",
 ]
 requires-python = ">=3.10"
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: MIT License",
```

### Comparing `xconn-0.2.0/xconn/__main__.py` & `xconn-0.2.1/xconn/__main__.py`

 * *Files identical despite different names*

### Comparing `xconn-0.2.0/xconn/acceptor.py` & `xconn-0.2.1/xconn/acceptor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import socket
 from typing import Sequence
 
 from aiohttp import web
-from wampproto import auth, acceptor
+from wampproto import auth, acceptor, serializers
 from websockets import ServerProtocol
 from websockets.sync.server import ServerConnection, Subprotocol
 
 from xconn import types, helpers
 
 
 class WebsocketsAcceptor:
@@ -39,13 +39,20 @@
     def __init__(self, authenticator: auth.IServerAuthenticator = None) -> None:
         self.authenticator = authenticator
 
     async def accept(self, ws: web.WebSocketResponse) -> types.AIOHttpBaseSession:
         serializer = helpers.get_serializer(ws.ws_protocol)
         a = acceptor.Acceptor(serializer=serializer, authenticator=self.authenticator)
 
+        if serializer is None or isinstance(serializer, serializers.JSONSerializer):
+            send_func = ws.send_str
+            receive_func = ws.receive_str
+        else:
+            send_func = ws.send_bytes
+            receive_func = ws.receive_bytes
+
         while not ws.closed:
-            msg = await ws.receive()
-            to_send, is_final = a.receive(msg.data)
-            await ws.send_bytes(to_send)
+            msg = await receive_func()
+            to_send, is_final = a.receive(msg)
+            await send_func(to_send)
             if is_final:
                 return types.AIOHttpBaseSession(ws, a.get_session_details(), serializer)
```

### Comparing `xconn-0.2.0/xconn/app.py` & `xconn-0.2.1/xconn/app.py`

 * *Files identical despite different names*

### Comparing `xconn-0.2.0/xconn/client.py` & `xconn-0.2.1/xconn/client.py`

 * *Files identical despite different names*

### Comparing `xconn-0.2.0/xconn/helpers.py` & `xconn-0.2.1/xconn/helpers.py`

 * *Files identical despite different names*

### Comparing `xconn-0.2.0/xconn/joiner.py` & `xconn-0.2.1/xconn/joiner.py`

 * *Files identical despite different names*

### Comparing `xconn-0.2.0/xconn/realm.py` & `xconn-0.2.1/xconn/realm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from asyncio import gather
 
 from wampproto import dealer, broker, messages
+from wampproto.types import SessionDetails
 
 from xconn import types
 
 
 class Realm:
     def __init__(self):
         super().__init__()
         self.dealer = dealer.Dealer()
         self.broker = broker.Broker()
 
         self.clients: dict[int, types.IAsyncBaseSession] = {}
 
     def attach_client(self, base: types.IAsyncBaseSession):
         self.clients[base.id] = base
-        self.dealer.add_session(base.id)
-        self.broker.add_session(base.id)
+
+        details = SessionDetails(base.id, base.realm, base.authid, base.authrole)
+        self.dealer.add_session(details)
+        self.broker.add_session(details)
 
     def detach_client(self, base: types.IAsyncBaseSession):
         del self.clients[base.id]
         self.broker.remove_session(base.id)
         self.dealer.remove_session(base.id)
 
     def stop(self):
```

### Comparing `xconn-0.2.0/xconn/router.py` & `xconn-0.2.1/xconn/router.py`

 * *Files identical despite different names*

### Comparing `xconn-0.2.0/xconn/server.py` & `xconn-0.2.1/xconn/server.py`

 * *Files identical despite different names*

### Comparing `xconn-0.2.0/xconn/session.py` & `xconn-0.2.1/xconn/session.py`

 * *Files identical despite different names*

### Comparing `xconn-0.2.0/xconn/types.py` & `xconn-0.2.1/xconn/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,14 +215,20 @@
     def __init__(
         self, ws: web.WebSocketResponse, session_details: joiner.SessionDetails, serializer: serializers.Serializer
     ):
         super().__init__()
         self.ws = ws
         self.session_details = session_details
         self._serializer = serializer
+        if serializer is None or isinstance(serializer, serializers.JSONSerializer):
+            self._send_func = ws.send_str
+            self._receive_func = ws.receive_str
+        else:
+            self._send_func = ws.send_bytes
+            self._receive_func = ws.receive_bytes
 
     @property
     def id(self) -> int:
         return self.session_details.session_id
 
     @property
     def realm(self) -> str:
@@ -237,18 +243,18 @@
         return self.session_details.authrole
 
     @property
     def serializer(self) -> serializers.Serializer:
         return self._serializer
 
     async def send(self, data: bytes):
-        await self.ws.send_bytes(data)
+        await self._send_func(data)
 
     async def receive(self) -> bytes:
-        return await self.ws.receive_bytes()
+        return await self._receive_func()
 
     async def send_message(self, msg: messages.Message):
         await self.send(self.serializer.serialize(msg))
 
     async def receive_message(self) -> messages.Message:
         return self.serializer.deserialize(await self.receive())
```

### Comparing `xconn-0.2.0/xconn.egg-info/PKG-INFO` & `xconn-0.2.1/xconn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xconn
-Version: 0.2.0
+Version: 0.2.1
 Summary: https://github.com/xconnio/xconn-python
 Author-email: Omer Akram <omer@thing.com>, Mahad Munir <mahad@xconn.io>
 License: MIT License
         
         Copyright (c) 2024 Simple Things Inc.
         Copyright (c) 2024 XConnIO Ltd.
         
@@ -33,15 +33,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: websockets
-Requires-Dist: wampproto>=0.2.0
+Requires-Dist: wampproto>=0.2.1
 Requires-Dist: aiohttp
 Requires-Dist: uvloop
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 Requires-Dist: ruff; extra == "test"
```

