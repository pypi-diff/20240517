# Comparing `tmp/moveread_dfy-0.1.2.tar.gz` & `tmp/moveread_dfy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_dfy-0.1.2.tar", last modified: Mon May 13 14:43:47 2024, max compression
+gzip compressed data, was "moveread_dfy-0.1.3.tar", last modified: Fri May 17 09:13:11 2024, max compression
```

## Comparing `moveread_dfy-0.1.2.tar` & `moveread_dfy-0.1.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-13 14:43:47.372851 moveread_dfy-0.1.2/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1227 2024-05-13 14:43:47.372851 moveread_dfy-0.1.2/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       50 2024-04-29 07:55:04.000000 moveread_dfy-0.1.2/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1056 2024-05-13 14:43:44.000000 moveread_dfy-0.1.2/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-13 14:43:47.372851 moveread_dfy-0.1.2/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-13 14:43:47.362851 moveread_dfy-0.1.2/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-13 14:43:47.362851 moveread_dfy-0.1.2/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-13 14:43:47.362851 moveread_dfy-0.1.2/src/moveread/dfy/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      155 2024-04-29 10:13:40.000000 moveread_dfy-0.1.2/src/moveread/dfy/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      310 2024-05-09 04:41:09.000000 moveread_dfy-0.1.2/src/moveread/dfy/__init__.pyi
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-13 14:43:47.372851 moveread_dfy-0.1.2/src/moveread/dfy/doer/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-07 14:51:57.000000 moveread_dfy-0.1.2/src/moveread/dfy/doer/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      140 2024-05-07 15:35:42.000000 moveread_dfy-0.1.2/src/moveread/dfy/doer/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1985 2024-05-12 16:19:17.000000 moveread_dfy-0.1.2/src/moveread/dfy/doer/_puller.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1297 2024-05-12 14:09:05.000000 moveread_dfy-0.1.2/src/moveread/dfy/doer/_pusher.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1015 2024-05-12 14:23:00.000000 moveread_dfy-0.1.2/src/moveread/dfy/doer/_run_connect.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-13 14:43:47.372851 moveread_dfy-0.1.2/src/moveread/dfy/integrations/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       28 2024-05-07 17:33:32.000000 moveread_dfy-0.1.2/src/moveread/dfy/integrations/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1866 2024-05-07 17:56:09.000000 moveread_dfy-0.1.2/src/moveread/dfy/integrations/core.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-13 14:43:47.372851 moveread_dfy-0.1.2/src/moveread/dfy/scripts/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-04-29 12:24:37.000000 moveread_dfy-0.1.2/src/moveread/dfy/scripts/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1535 2024-05-12 10:43:00.000000 moveread_dfy-0.1.2/src/moveread/dfy/scripts/api_cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      482 2024-05-12 10:50:26.000000 moveread_dfy-0.1.2/src/moveread/dfy/scripts/clientgen_cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1745 2024-05-07 17:15:46.000000 moveread_dfy-0.1.2/src/moveread/dfy/scripts/connect_cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3140 2024-05-12 14:35:12.000000 moveread_dfy-0.1.2/src/moveread/dfy/scripts/doer_cli.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-13 14:43:47.372851 moveread_dfy-0.1.2/src/moveread/dfy/server/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-08 07:12:36.000000 moveread_dfy-0.1.2/src/moveread/dfy/server/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      112 2024-05-07 10:08:12.000000 moveread_dfy-0.1.2/src/moveread/dfy/server/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3316 2024-05-13 12:55:43.000000 moveread_dfy-0.1.2/src/moveread/dfy/server/api.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      573 2024-05-12 09:12:38.000000 moveread_dfy-0.1.2/src/moveread/dfy/server/main.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      751 2024-05-12 10:41:22.000000 moveread_dfy-0.1.2/src/moveread/dfy/server/pgns.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4477 2024-05-13 12:52:26.000000 moveread_dfy-0.1.2/src/moveread/dfy/server/sdk.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2437 2024-05-13 12:47:37.000000 moveread_dfy-0.1.2/src/moveread/dfy/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-13 14:43:47.372851 moveread_dfy-0.1.2/src/moveread_dfy.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1227 2024-05-13 14:43:47.000000 moveread_dfy-0.1.2/src/moveread_dfy.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      995 2024-05-13 14:43:47.000000 moveread_dfy-0.1.2/src/moveread_dfy.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-13 14:43:47.000000 moveread_dfy-0.1.2/src/moveread_dfy.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      216 2024-05-13 14:43:47.000000 moveread_dfy-0.1.2/src/moveread_dfy.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      284 2024-05-13 14:43:47.000000 moveread_dfy-0.1.2/src/moveread_dfy.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-13 14:43:47.000000 moveread_dfy-0.1.2/src/moveread_dfy.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-17 09:13:11.597619 moveread_dfy-0.1.3/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1227 2024-05-17 09:13:11.597619 moveread_dfy-0.1.3/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       50 2024-04-29 07:55:04.000000 moveread_dfy-0.1.3/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1056 2024-05-17 09:13:09.000000 moveread_dfy-0.1.3/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-17 09:13:11.597619 moveread_dfy-0.1.3/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-17 09:13:11.587619 moveread_dfy-0.1.3/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-17 09:13:11.587619 moveread_dfy-0.1.3/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-17 09:13:11.587619 moveread_dfy-0.1.3/src/moveread/dfy/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      155 2024-04-29 10:13:40.000000 moveread_dfy-0.1.3/src/moveread/dfy/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      310 2024-05-09 04:41:09.000000 moveread_dfy-0.1.3/src/moveread/dfy/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-17 09:13:11.587619 moveread_dfy-0.1.3/src/moveread/dfy/doer/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-07 14:51:57.000000 moveread_dfy-0.1.3/src/moveread/dfy/doer/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      140 2024-05-07 15:35:42.000000 moveread_dfy-0.1.3/src/moveread/dfy/doer/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2424 2024-05-14 16:56:40.000000 moveread_dfy-0.1.3/src/moveread/dfy/doer/_puller.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1515 2024-05-14 14:28:20.000000 moveread_dfy-0.1.3/src/moveread/dfy/doer/_pusher.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1119 2024-05-14 12:50:44.000000 moveread_dfy-0.1.3/src/moveread/dfy/doer/_run_connect.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-17 09:13:11.597619 moveread_dfy-0.1.3/src/moveread/dfy/integrations/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       28 2024-05-07 17:33:32.000000 moveread_dfy-0.1.3/src/moveread/dfy/integrations/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2009 2024-05-14 17:12:01.000000 moveread_dfy-0.1.3/src/moveread/dfy/integrations/core.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-17 09:13:11.597619 moveread_dfy-0.1.3/src/moveread/dfy/scripts/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-04-29 12:24:37.000000 moveread_dfy-0.1.3/src/moveread/dfy/scripts/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1535 2024-05-12 10:43:00.000000 moveread_dfy-0.1.3/src/moveread/dfy/scripts/api_cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      482 2024-05-12 10:50:26.000000 moveread_dfy-0.1.3/src/moveread/dfy/scripts/clientgen_cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1745 2024-05-07 17:15:46.000000 moveread_dfy-0.1.3/src/moveread/dfy/scripts/connect_cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3837 2024-05-14 17:18:45.000000 moveread_dfy-0.1.3/src/moveread/dfy/scripts/doer_cli.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-17 09:13:11.597619 moveread_dfy-0.1.3/src/moveread/dfy/server/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-08 07:12:36.000000 moveread_dfy-0.1.3/src/moveread/dfy/server/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      112 2024-05-07 10:08:12.000000 moveread_dfy-0.1.3/src/moveread/dfy/server/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4224 2024-05-13 16:20:11.000000 moveread_dfy-0.1.3/src/moveread/dfy/server/api.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      573 2024-05-12 09:12:38.000000 moveread_dfy-0.1.3/src/moveread/dfy/server/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      751 2024-05-12 10:41:22.000000 moveread_dfy-0.1.3/src/moveread/dfy/server/pgns.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4477 2024-05-13 12:52:26.000000 moveread_dfy-0.1.3/src/moveread/dfy/server/sdk.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2437 2024-05-13 12:47:37.000000 moveread_dfy-0.1.3/src/moveread/dfy/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-17 09:13:11.597619 moveread_dfy-0.1.3/src/moveread_dfy.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1227 2024-05-17 09:13:11.000000 moveread_dfy-0.1.3/src/moveread_dfy.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      995 2024-05-17 09:13:11.000000 moveread_dfy-0.1.3/src/moveread_dfy.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-17 09:13:11.000000 moveread_dfy-0.1.3/src/moveread_dfy.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      216 2024-05-17 09:13:11.000000 moveread_dfy-0.1.3/src/moveread_dfy.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      284 2024-05-17 09:13:11.000000 moveread_dfy-0.1.3/src/moveread_dfy.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-17 09:13:11.000000 moveread_dfy-0.1.3/src/moveread_dfy.egg-info/top_level.txt
```

### Comparing `moveread_dfy-0.1.2/PKG-INFO` & `moveread_dfy-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-dfy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Moveread DFY data models and API
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-dfy.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: lazy-loader
 Requires-Dist: pydantic
```

### Comparing `moveread_dfy-0.1.2/pyproject.toml` & `moveread_dfy-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-dfy"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Moveread DFY data models and API"
 dependencies = [
   "lazy-loader", "pydantic",
   "chess-pairings", "dslog",
```

### Comparing `moveread_dfy-0.1.2/src/moveread/dfy/doer/_puller.py` & `moveread_dfy-0.1.3/src/moveread/dfy/doer/_puller.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,19 +7,33 @@
 from haskellian import Left, either as E
 from dslog import Logger
 from kv.api import KV
 from q.api import WriteQueue
 from moveread.pipelines.dfy import Input
 from moveread.pipelines.input_validation import GameId
 from scoresheet_models import ModelID
-from ..types import Game
+from ..types import Game, Pairing
 
 def randomId(tournId: str, group: str, round: str, board: str) -> str:
   return f'{tournId}/{group}/{round}/{board}_{uuid4()}'
 
+def pairing_display(pairing: Pairing):
+  pair = pairing.root
+  if pair.tag == 'unpaired':
+    return 'Unpaired!?'
+  
+  s = f'{pair.white} - {pair.black}'
+  if pair.result is not None:
+    s += f' {pair.result}'
+  return s
+
+
+def title(pairing: Pairing, tournId: str, group: str, round: str, board: str) -> str:
+  return f'{tournId} {group}/{round}/{board} {pairing_display(pairing)}'
+
 async def puller(
   Qin: WriteQueue[Input], engine: Engine, *,
   online_images: KV[bytes], local_images: KV[bytes],
   tournId: str, model: ModelID, polling_interval: timedelta = timedelta(seconds=30),
   logger = Logger.rich().prefix('[PULLER]')
 ):
   @E.do()
@@ -28,15 +42,15 @@
       with Session(engine) as ses:
         stmt = select(Game).where(Game.tournId == tournId, Game.status == Game.Status.uploaded)
         games = ses.exec(stmt).all()
         for game in games:
           gameId = GameId(group=game.group, round=game.round, board=game.board)
           id = randomId(tournId, **gameId)
           urls = [img.url for img in game.imgs]
-          task = Input(gameId=gameId, model=model, imgs=urls)
+          task = Input(gameId=gameId, model=model, imgs=urls, title=title(game.pairing, tournId, **gameId))
           tasks = [online_images.copy(url, local_images, url).run() for url in urls]
           results = await asyncio.gather(*tasks)
           E.sequence(results).unsafe()
 
           logger(f'Inputting new task for "{id}":', task)
           (await Qin.push(id, task)).unsafe()
           game.status = Game.Status.doing
```

### Comparing `moveread_dfy-0.1.2/src/moveread/dfy/doer/_pusher.py` & `moveread_dfy-0.1.3/src/moveread/dfy/doer/_pusher.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 import asyncio
 from sqlalchemy import Engine
 from sqlmodel import select, Session
 from dslog import Logger
 from haskellian import either as E, Left
+from kv.api import KV
 from q.api import ReadQueue
-from moveread.pipelines.dfy import Result
+from moveread.core import CoreAPI
+from moveread.pipelines.dfy import Result, output_one
 from ..types import Game, PGN
 
 def exact_game(tournId: str, group: str, round: str, board: str):
   return Game.tournId == tournId, Game.group == group, Game.round == round, Game.board == board
 
 async def pusher(
   Qout: ReadQueue[Result], engine: Engine, *,
-  tournId: str,
+  tournId: str, output_core: CoreAPI, images: KV[bytes],
   logger = Logger.rich().prefix('[DFY PUSHER]')
 ):
   
   @E.do()
   async def push_one():
     id, result = (await Qout.read()).unsafe()
+    (await output_one(output_core, id, result, tournId=tournId, images=images)).unsafe()
     gid = result.gameId
     logger(f'Pushing result for {gid}')
     try:
       with Session(engine) as ses:
         stmt = select(Game).where(*exact_game(tournId, **gid))
         game = ses.exec(stmt).first()
         if game is None:
           logger(f'Game not found: {gid}', level='ERROR')
           return
 
-        game.pgn = PGN(moves=result.pgn)
+        game.pgn = PGN(moves=result.pgn, early=result.early)
         game.status = Game.Status.done
         ses.add(game)
         ses.commit()
     except Exception as e:
       Left(e).unsafe()
 
     (await Qout.pop(id)).unsafe()
```

### Comparing `moveread_dfy-0.1.2/src/moveread/dfy/doer/_run_connect.py` & `moveread_dfy-0.1.3/src/moveread/dfy/doer/_run_connect.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,31 +3,33 @@
 from sqlmodel import SQLModel
 from sqlalchemy import Engine
 from dslog import Logger
 from haskellian import promise as P
 from kv.api import KV
 from q.api import ReadQueue, WriteQueue
 from scoresheet_models import ModelID
+from moveread.core import CoreAPI
 from moveread.pipelines.dfy import Input, Result
 from ._puller import puller
 from ._pusher import pusher
 
 @P.run
 async def run_connect(
   Qin: WriteQueue[Input], Qout: ReadQueue[Result], *,
   engine: Engine, tournId: str, model: ModelID,
+  output_core: CoreAPI,
   local_images: KV[bytes], online_images: KV[bytes],
   logger = Logger.rich().prefix('[DFY]'),
   polling_interval = timedelta(seconds=30)
 ):
   
   SQLModel.metadata.create_all(engine)
 
   tasks = (
     puller(
       Qin, engine, tournId=tournId, polling_interval=polling_interval,
       model=model, logger=logger.prefix('[PULLER]'),
       online_images=online_images, local_images=local_images
     ),
-    pusher(Qout, engine, tournId=tournId, logger=logger.prefix('[PUSHER]'))
+    pusher(Qout, engine, output_core=output_core, images=local_images, tournId=tournId, logger=logger.prefix('[PUSHER]'))
   )
   await asyncio.gather(*tasks)
```

### Comparing `moveread_dfy-0.1.2/src/moveread/dfy/integrations/core.py` & `moveread_dfy-0.1.3/src/moveread/dfy/integrations/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Callable
 from uuid import uuid4
 from sqlmodel import Session
 from kv.api import KV
 from dslog import Logger
 from scoresheet_models import ModelID
 from moveread.core import CoreAPI, Game as CoreGame
-from ..types import Game, GameId, Image
+from ..types import Game, GameId, Image, Pairing, Paired
 
 def gameIdFn(game: CoreGame, tournId: str) -> GameId:
   if game.meta is None or game.meta.tournament is None:
-    return GameId(tournId=tournId, group='a', round=1, board=1)
+    return GameId(tournId=tournId, group='a', round='1', board='1')
   t = game.meta.tournament
-  return GameId(tournId=tournId, group=t.group or 'a', round=t.round or 1, board=t.board or 1)
+  return GameId(tournId=tournId, group=t.group or 'a', round=t.round or '1', board=t.board or '1')
 
 async def input_core(
   core: CoreAPI, session: Session,
   *, images: KV[bytes],
   gameId_fn: Callable[[CoreGame], GameId] | None = None,
-  tournId: str = 'llobregat',
+  tournId: str = 'llobregat23',
   num_games: int | None = None, shuffle: bool = True,
   logger = Logger.rich().prefix('[CORE INPUT]')
 ):
   """Input all images from `core` into `Qin` tasks
   - Actually, only images with `version == 0`
   - `model_fn`: determines the scoresheet model of each task
   - `state_fn`: determines an arbitrary tuple of JSON-serializable data to attach to each task
@@ -40,11 +40,13 @@
         id = str(imgId)
         url = f'{id}/original_{uuid4()}.jpg'
         img = (await core.blobs.read(image.url)).unsafe()
         (await images.insert(url, img)).unsafe()
         imgs.append(url)
 
     gid = gameId_fn(game)
-    g = Game(id=game.id, imgs=[Image(url=img, gameId=game.id) for img in imgs], **gid.dict())
+    g = Game(
+      index=int(gid['board']), pairing=Pairing(Paired(white='Magnus', black='Anish', tag='paired')),
+      imgs=[Image(url=img, descaled_url=img) for img in imgs], status=Game.Status.uploaded, **gid)
     session.add(g)
-    logger(f'Inputted game "{game.id}"')
+    logger(f'Inputted game "{gid}"')
   session.commit()
```

### Comparing `moveread_dfy-0.1.2/src/moveread/dfy/scripts/api_cli.py` & `moveread_dfy-0.1.3/src/moveread/dfy/scripts/api_cli.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.2/src/moveread/dfy/scripts/connect_cli.py` & `moveread_dfy-0.1.3/src/moveread/dfy/scripts/connect_cli.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.2/src/moveread/dfy/scripts/doer_cli.py` & `moveread_dfy-0.1.3/src/moveread/dfy/scripts/doer_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,60 +8,72 @@
   parser.add_argument('-b', '--base-path', required=True)
   parser.add_argument('-d', '--db', required=True, help='Database URL')
   parser.add_argument('-t', '--tournament', required=True, help='Tournament ID')
   parser.add_argument('-m', '--model', required=True, choices=MODEL_IDS, help='Model ID')
   parser.add_argument('--protocol', default='sqlite', required=False, choices=['sqlite', 'fs'], help='Protocol used in queues')
   parser.add_argument('--images', type=str, help='Local path to images')
   parser.add_argument('--blobs', type=str, help='Azure Blob connection string')
+  parser.add_argument('--core', type=str, help='Path to output core')
 
   args = parser.parse_args()
 
 
   import os
   from dslog import Logger
   input_path = os.path.join(os.getcwd(), args.input)
   output_path = os.path.join(os.getcwd(), args.output)
   base_path = os.path.join(os.getcwd(), args.base_path)
   proto = args.protocol
   db_url = args.db
   tournId = args.tournament
   images_path = os.path.join(os.getcwd(), args.images)
+  core_path = os.path.join(os.getcwd(), args.core)
   
   logger = Logger.click().prefix('[DFY]')
   logger(f'Running...')
   logger(f'- Tournament ID: "{tournId}"')
   logger(f'- Database URL: "{db_url}"')
   logger(f'- Images path: "{images_path}"')
+  logger(f'- Output core path: "{core_path}"')
 
   
   logger(f'- Queues protocol: "{proto}"')
   logger(f'- Input path: "{input_path}"')
   logger(f'- Internal path: "{base_path}"')
   logger(f'- Output path: "{output_path}"')
   
-  from kv.azure.blob import BlobKV
-  online_images = BlobKV[bytes].from_conn_str(args.blobs)
+
+  if args.blobs.startswith('.'):
+    from kv.fs import FilesystemKV
+    blobs = os.path.join(os.getcwd(), args.blobs)
+    online_images = FilesystemKV[bytes](blobs)
+    logger(f'- Local blobs: {blobs}')
   
-  logger(f'- Azure Blob account: {online_images.client.account_name}')
+  else:
+    from kv.azure.blob import BlobKV
+    online_images = BlobKV[bytes].from_conn_str(args.blobs)
+    logger(f'- Azure Blob account: {online_images.client.account_name}')
   
   from sqlmodel import create_engine
+  from kv.fs import FilesystemKV
   from moveread.dfy import run_connect
   from moveread.pipelines.dfy import run_local, input_queue, output_queue
   from multiprocessing import Process
-  from kv.fs import FilesystemKV
+  from moveread.core import CoreAPI
   local_images = FilesystemKV[bytes](images_path)
+  core = CoreAPI.at(core_path)
 
   Qin = input_queue(input_path, protocol=proto)
   Qout = output_queue(output_path, protocol=proto)
   engine = create_engine(db_url)
   ps = (
     Process(
       target=run_connect, args=(Qin, Qout), kwargs=dict(
         engine=engine, tournId=tournId, logger=logger.prefix('[I/O]'), model=args.model,
-        local_images=local_images, online_images=online_images
+        local_images=local_images, online_images=online_images, output_core=core
       )
     ),
     Process(
       target=run_local, args=(Qin, Qout), kwargs=dict(
         base_path=base_path, images=local_images,
         images_path=images_path, logger=logger
       )
@@ -72,19 +84,26 @@
   for p in ps:
     p.join()
 
 if __name__ == '__main__':
   import sys
   import os
   from dotenv import load_dotenv
-  os.chdir('/home/m4rs/mr-github/modes/moveread-dfy/infra/doer')
+  path = '/home/m4rs/mr-github/modes/moveread-dfy/infra/doer/local'
+  os.makedirs(path, exist_ok=True)
+  os.chdir(path)
   load_dotenv()
+
   SQL_CONN_STR = os.environ['SQL_CONN_STR']
+  # SQL_CONN_STR = 'sqlite:////home/m4rs/mr-github/modes/moveread-dfy/local-db/db.sqlite'
   BLOB_CONN_STR = os.environ['BLOB_CONN_STR']
+  # BLOB_CONN_STR = '../../../local-db/images'
+  blobs = ''
   args = f'-i queues/in -o queues/out -b queues/internal \
       -t llobregat23 -m llobregat23 \
       --db {SQL_CONN_STR} \
       --blobs {BLOB_CONN_STR} \
+      --core core \
       --images images'.replace('\n', '').split(' ')
   args = [arg for arg in args if arg]
   sys.argv.extend(args)
   main()
```

### Comparing `moveread_dfy-0.1.2/src/moveread/dfy/server/main.py` & `moveread_dfy-0.1.3/src/moveread/dfy/server/main.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.2/src/moveread/dfy/server/pgns.py` & `moveread_dfy-0.1.3/src/moveread/dfy/server/pgns.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.2/src/moveread/dfy/server/sdk.py` & `moveread_dfy-0.1.3/src/moveread/dfy/server/sdk.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.2/src/moveread/dfy/types.py` & `moveread_dfy-0.1.3/src/moveread/dfy/types.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.2/src/moveread_dfy.egg-info/PKG-INFO` & `moveread_dfy-0.1.3/src/moveread_dfy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-dfy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Moveread DFY data models and API
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-dfy.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: lazy-loader
 Requires-Dist: pydantic
```

### Comparing `moveread_dfy-0.1.2/src/moveread_dfy.egg-info/SOURCES.txt` & `moveread_dfy-0.1.3/src/moveread_dfy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

