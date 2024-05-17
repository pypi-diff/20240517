# Comparing `tmp/miservice_fork-2.4.4.tar.gz` & `tmp/miservice_fork-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miservice_fork-2.4.4.tar", last modified: Thu May 16 00:06:45 2024, max compression
+gzip compressed data, was "miservice_fork-2.5.0.tar", last modified: Fri May 17 04:29:37 2024, max compression
```

## Comparing `miservice_fork-2.4.4.tar` & `miservice_fork-2.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-16 00:06:45.508926 miservice_fork-2.4.4/
--rw-r--r--   0 hyi        (502) staff       (20)     1067 2023-03-11 14:21:43.000000 miservice_fork-2.4.4/LICENSE
--rw-r--r--   0 hyi        (502) staff       (20)      529 2024-05-16 00:06:45.508471 miservice_fork-2.4.4/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)     4587 2024-05-16 00:06:29.000000 miservice_fork-2.4.4/README.md
--rwxr-xr-x   0 hyi        (502) staff       (20)       96 2023-07-31 09:48:54.000000 miservice_fork-2.4.4/micli.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-16 00:06:45.503200 miservice_fork-2.4.4/miservice/
--rwxr-xr-x   0 hyi        (502) staff       (20)      178 2023-03-12 07:11:31.000000 miservice_fork-2.4.4/miservice/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)       95 2023-03-11 14:21:43.000000 miservice_fork-2.4.4/miservice/__main__.py
--rw-r--r--   0 hyi        (502) staff       (20)     7911 2024-05-16 00:06:29.000000 miservice_fork-2.4.4/miservice/cli.py
--rwxr-xr-x   0 hyi        (502) staff       (20)     5647 2023-10-23 08:06:30.000000 miservice_fork-2.4.4/miservice/miaccount.py
--rwxr-xr-x   0 hyi        (502) staff       (20)     3818 2024-01-07 08:08:03.000000 miservice_fork-2.4.4/miservice/miiocommand.py
--rwxr-xr-x   0 hyi        (502) staff       (20)    10620 2024-01-29 05:33:41.000000 miservice_fork-2.4.4/miservice/miioservice.py
--rw-r--r--   0 hyi        (502) staff       (20)     4264 2024-05-16 00:06:29.000000 miservice_fork-2.4.4/miservice/minaservice.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-16 00:06:45.507814 miservice_fork-2.4.4/miservice_fork.egg-info/
--rw-r--r--   0 hyi        (502) staff       (20)      529 2024-05-16 00:06:45.000000 miservice_fork-2.4.4/miservice_fork.egg-info/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)      424 2024-05-16 00:06:45.000000 miservice_fork-2.4.4/miservice_fork.egg-info/SOURCES.txt
--rw-r--r--   0 hyi        (502) staff       (20)        1 2024-05-16 00:06:45.000000 miservice_fork-2.4.4/miservice_fork.egg-info/dependency_links.txt
--rw-r--r--   0 hyi        (502) staff       (20)       46 2024-05-16 00:06:45.000000 miservice_fork-2.4.4/miservice_fork.egg-info/entry_points.txt
--rw-r--r--   0 hyi        (502) staff       (20)       21 2024-05-16 00:06:45.000000 miservice_fork-2.4.4/miservice_fork.egg-info/requires.txt
--rw-r--r--   0 hyi        (502) staff       (20)       10 2024-05-16 00:06:45.000000 miservice_fork-2.4.4/miservice_fork.egg-info/top_level.txt
--rw-r--r--   0 hyi        (502) staff       (20)       38 2024-05-16 00:06:45.508976 miservice_fork-2.4.4/setup.cfg
--rwxr-xr-x   0 hyi        (502) staff       (20)      919 2024-05-16 00:06:38.000000 miservice_fork-2.4.4/setup.py
+drwxrwxr-x   0 yihong    (1000) yihong    (1000)        0 2024-05-17 04:29:37.342739 miservice_fork-2.5.0/
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)     1067 2024-05-17 04:19:57.000000 miservice_fork-2.5.0/LICENSE
+-rw-r--r--   0 yihong    (1000) yihong    (1000)      529 2024-05-17 04:29:37.342739 miservice_fork-2.5.0/PKG-INFO
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)     4587 2024-05-17 04:19:57.000000 miservice_fork-2.5.0/README.md
+-rwxrwxr-x   0 yihong    (1000) yihong    (1000)       96 2024-05-17 04:19:57.000000 miservice_fork-2.5.0/micli.py
+drwxrwxr-x   0 yihong    (1000) yihong    (1000)        0 2024-05-17 04:29:37.342739 miservice_fork-2.5.0/miservice/
+-rwxrwxr-x   0 yihong    (1000) yihong    (1000)      178 2024-05-17 04:19:57.000000 miservice_fork-2.5.0/miservice/__init__.py
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)       95 2024-05-17 04:19:57.000000 miservice_fork-2.5.0/miservice/__main__.py
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)     7939 2024-05-17 04:27:59.000000 miservice_fork-2.5.0/miservice/cli.py
+-rwxrwxr-x   0 yihong    (1000) yihong    (1000)     5647 2024-05-17 04:19:57.000000 miservice_fork-2.5.0/miservice/miaccount.py
+-rwxrwxr-x   0 yihong    (1000) yihong    (1000)     3818 2024-05-17 04:19:57.000000 miservice_fork-2.5.0/miservice/miiocommand.py
+-rwxrwxr-x   0 yihong    (1000) yihong    (1000)    10620 2024-05-17 04:19:57.000000 miservice_fork-2.5.0/miservice/miioservice.py
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)     4496 2024-05-17 04:27:59.000000 miservice_fork-2.5.0/miservice/minaservice.py
+drwxrwxr-x   0 yihong    (1000) yihong    (1000)        0 2024-05-17 04:29:37.342739 miservice_fork-2.5.0/miservice_fork.egg-info/
+-rw-r--r--   0 yihong    (1000) yihong    (1000)      529 2024-05-17 04:29:37.000000 miservice_fork-2.5.0/miservice_fork.egg-info/PKG-INFO
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)      424 2024-05-17 04:29:37.000000 miservice_fork-2.5.0/miservice_fork.egg-info/SOURCES.txt
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)        1 2024-05-17 04:29:37.000000 miservice_fork-2.5.0/miservice_fork.egg-info/dependency_links.txt
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)       46 2024-05-17 04:29:37.000000 miservice_fork-2.5.0/miservice_fork.egg-info/entry_points.txt
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)       21 2024-05-17 04:29:37.000000 miservice_fork-2.5.0/miservice_fork.egg-info/requires.txt
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)       10 2024-05-17 04:29:37.000000 miservice_fork-2.5.0/miservice_fork.egg-info/top_level.txt
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)       38 2024-05-17 04:29:37.342739 miservice_fork-2.5.0/setup.cfg
+-rwxrwxr-x   0 yihong    (1000) yihong    (1000)      919 2024-05-17 04:29:20.000000 miservice_fork-2.5.0/setup.py
```

### Comparing `miservice_fork-2.4.4/LICENSE` & `miservice_fork-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.4.4/PKG-INFO` & `miservice_fork-2.5.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: miservice_fork
-Version: 2.4.4
+Version: 2.5.0
 Summary: XiaoMi Cloud Service fork from https://github.com/Yonsm/MiService
 Home-page: https://github.com/yihong0618/MiService
 Author: Yonsm, yihong0618
 Author-email: Yonsm@qq.com, zouzou0208@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: mutagen
 Requires-Dist: rich
```

### Comparing `miservice_fork-2.4.4/README.md` & `miservice_fork-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.4.4/miservice/cli.py` & `miservice_fork-2.5.0/miservice/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,28 +72,28 @@
             return song_play_dict
 
 
 # TODO support more
 device_id_list = []
 
 
-async def miservice_pause(device_id):
+async def miservice_stop(device_id):
     """
     for ctrl + c exit
     """
     async with ClientSession() as session:
         env = os.environ
         account = MiAccount(
             session,
             env.get("MI_USER"),
             env.get("MI_PASS"),
             os.path.join(str(Path.home()), ".mi.token"),
         )
         mina_service = MiNAService(account)
-        await mina_service.player_pause(device_id)
+        await mina_service.player_stop(device_id)
     print("Stop")
 
 
 async def main(args):
     try:
         async with ClientSession() as session:
             env = os.environ
@@ -106,30 +106,31 @@
             result = ""
             mina_service = MiNAService(account)
             # TODO refactor this shit
             if args.split(" ")[0].strip() in [
                 "play",
                 "mina",
                 "pause",
+                "stop",
                 "loop",
                 "play_list",
                 "suno",
                 "suno_random",
             ]:
                 arg = args.split(" ")[0].strip()
                 result = await mina_service.device_list()
                 if not env.get("MI_DID"):
                     raise Exception("Please export MI_DID in your env")
                 device_id = find_device_id(result, env.get("MI_DID", ""))
                 # tricky add it to global
                 device_id_list.append(device_id)
                 args_list = args.split(" ")
                 if len(args_list) == 1:
-                    if args_list[0] == "pause":
-                        await mina_service.player_pause(device_id)
+                    if args_list[0] in ["pause", "stop"]:
+                        await mina_service.player_stop(device_id)
                     elif args_list[0] == "mina" and len(result) > 0:
                         print(result[0])
                     elif "suno" in args_list[0]:
                         song_dict = await get_suno_playlist()
                         print(song_dict)
                         song_urls = list(song_dict.keys())
                         if args_list[0] == "suno_random":
@@ -139,15 +140,15 @@
                             print("Will play suno trending list")
                         for song_url in song_urls:
                             title = song_dict[song_url]
                             print(f"Will play {song_url.strip()} title {title}")
                             await mina_service.play_by_url(device_id, song_url.strip())
                             duration = await _get_duration(song_url)
                             await asyncio.sleep(duration)
-                        await mina_service.player_pause(device_id)
+                        await mina_service.player_stop(device_id)
                     else:
                         print("Please provide a play URL")
                     return
                 # make device_id
                 if arg == "loop":
                     url = args_list[1]
                     await mina_service.play_by_url(device_id, url)
@@ -166,15 +167,15 @@
                         with open(file_name, encoding="utf8") as f:
                             lines = f.readlines()
                             for line in lines:
                                 print(f"Will play {line.strip()}")
                                 await mina_service.play_by_url(device_id, line.strip())
                                 duration = await _get_duration(line)
                                 await asyncio.sleep(duration)
-                        await mina_service.player_pause(device_id)
+                        await mina_service.player_stop(device_id)
                     except Exception as e:
                         print(e)
                         return
             else:
                 service = MiIOService(account)
                 result = await miio_command(
                     service, env.get("MI_DID"), args, sys.argv[0] + " "
@@ -208,15 +209,15 @@
             _LOGGER = logging.getLogger("miservice")
             _LOGGER.setLevel(level)
             _LOGGER.addHandler(logging.StreamHandler())
         try:
             asyncio.run(main(" ".join(argv[argi:])))
         except (KeyboardInterrupt, asyncio.exceptions.CancelledError) as e:
             device_id = device_id_list[0]
-            asyncio.run(miservice_pause(device_id))
+            asyncio.run(miservice_stop(device_id))
             print(str(e))
             pass
     else:
         usage()
 
 
 if __name__ == "__main__":
```

### Comparing `miservice_fork-2.4.4/miservice/miaccount.py` & `miservice_fork-2.5.0/miservice/miaccount.py`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.4.4/miservice/miiocommand.py` & `miservice_fork-2.5.0/miservice/miiocommand.py`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.4.4/miservice/miioservice.py` & `miservice_fork-2.5.0/miservice/miioservice.py`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.4.4/miservice/minaservice.py` & `miservice_fork-2.5.0/miservice/minaservice.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,22 @@
         return await self.ubus_request(
             deviceId,
             "player_play_operation",
             "mediaplayer",
             {"action": "pause", "media": "app_ios"},
         )
 
+    async def player_stop(self, deviceId):
+        return await self.ubus_request(
+            deviceId,
+            "player_play_operation",
+            "mediaplayer",
+            {"action": "stop", "media": "app_ios"},
+        )
+
     async def player_play(self, deviceId):
         return await self.ubus_request(
             deviceId,
             "player_play_operation",
             "mediaplayer",
             {"action": "play", "media": "app_ios"},
         )
```

### Comparing `miservice_fork-2.4.4/miservice_fork.egg-info/PKG-INFO` & `miservice_fork-2.5.0/miservice_fork.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: miservice_fork
-Version: 2.4.4
+Version: 2.5.0
 Summary: XiaoMi Cloud Service fork from https://github.com/Yonsm/MiService
 Home-page: https://github.com/yihong0618/MiService
 Author: Yonsm, yihong0618
 Author-email: Yonsm@qq.com, zouzou0208@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: mutagen
 Requires-Dist: rich
```

### Comparing `miservice_fork-2.4.4/setup.py` & `miservice_fork-2.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 
 
 from setuptools import setup
 
 setup(
     name="miservice_fork",
     description="XiaoMi Cloud Service fork from https://github.com/Yonsm/MiService",
-    version="2.4.4",
+    version="2.5.0",
     license="MIT",
     author="Yonsm, yihong0618",
     author_email="Yonsm@qq.com, zouzou0208@gmail.com",
     url="https://github.com/yihong0618/MiService",
     packages=["miservice"],
     scripts=["micli.py"],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=["aiohttp", "mutagen", "rich"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
```

