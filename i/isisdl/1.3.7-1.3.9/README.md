# Comparing `tmp/isisdl-1.3.7.tar.gz` & `tmp/isisdl-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isisdl-1.3.7.tar", last modified: Sun May  8 23:32:58 2022, max compression
+gzip compressed data, was "isisdl-1.3.9.tar", last modified: Fri Jun  3 16:28:30 2022, max compression
```

## Comparing `isisdl-1.3.7.tar` & `isisdl-1.3.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 emily     (1000) emily     (1000)        0 2022-05-08 23:32:58.345626 isisdl-1.3.7/
--rw-r--r--   0 emily     (1000) emily     (1000)    35149 2022-03-25 13:10:48.000000 isisdl-1.3.7/LICENSE
--rw-r--r--   0 emily     (1000) emily     (1000)      554 2022-05-08 23:32:58.345626 isisdl-1.3.7/PKG-INFO
--rw-r--r--   0 emily     (1000) emily     (1000)     3445 2022-05-03 21:55:30.000000 isisdl-1.3.7/README.md
--rw-r--r--   0 emily     (1000) emily     (1000)      414 2022-04-17 21:15:45.000000 isisdl-1.3.7/pyproject.toml
--rw-r--r--   0 emily     (1000) emily     (1000)      959 2022-05-08 23:32:58.345626 isisdl-1.3.7/setup.cfg
--rw-r--r--   0 emily     (1000) emily     (1000)      262 2022-03-25 13:10:48.000000 isisdl-1.3.7/setup.py
-drwxr-xr-x   0 emily     (1000) emily     (1000)        0 2022-05-08 23:32:58.342628 isisdl-1.3.7/src/
-drwxr-xr-x   0 emily     (1000) emily     (1000)        0 2022-05-08 23:32:58.343627 isisdl-1.3.7/src/isisdl/
--rw-r--r--   0 emily     (1000) emily     (1000)        0 2022-03-25 13:11:26.000000 isisdl-1.3.7/src/isisdl/__init__.py
--rw-r--r--   0 emily     (1000) emily     (1000)     3745 2022-05-03 20:39:18.000000 isisdl-1.3.7/src/isisdl/__main__.py
--rwxr-xr-x   0 emily     (1000) emily     (1000)      100 2022-04-17 21:15:45.000000 isisdl-1.3.7/src/isisdl/autorun.py
-drwxr-xr-x   0 emily     (1000) emily     (1000)        0 2022-05-08 23:32:58.344627 isisdl-1.3.7/src/isisdl/backend/
--rw-r--r--   0 emily     (1000) emily     (1000)        0 2022-03-25 13:10:48.000000 isisdl-1.3.7/src/isisdl/backend/__init__.py
--rw-r--r--   0 emily     (1000) emily     (1000)    19427 2022-05-01 13:41:19.000000 isisdl-1.3.7/src/isisdl/backend/config.py
--rw-r--r--   0 emily     (1000) emily     (1000)     4339 2022-05-01 13:47:23.000000 isisdl-1.3.7/src/isisdl/backend/crypt.py
--rw-r--r--   0 emily     (1000) emily     (1000)     9890 2022-04-22 18:59:05.000000 isisdl-1.3.7/src/isisdl/backend/database_helper.py
--rw-r--r--   0 emily     (1000) emily     (1000)    48036 2022-05-08 23:32:52.000000 isisdl-1.3.7/src/isisdl/backend/request_helper.py
--rw-r--r--   0 emily     (1000) emily     (1000)    10837 2022-04-20 10:30:06.000000 isisdl-1.3.7/src/isisdl/backend/status.py
--rw-r--r--   0 emily     (1000) emily     (1000)     8360 2022-05-01 16:28:28.000000 isisdl-1.3.7/src/isisdl/backend/sync_database.py
--rw-r--r--   0 emily     (1000) emily     (1000)    23172 2022-05-01 13:42:07.000000 isisdl-1.3.7/src/isisdl/compress.py
--rw-r--r--   0 emily     (1000) emily     (1000)    13797 2022-05-01 15:55:41.000000 isisdl-1.3.7/src/isisdl/settings.py
--rw-r--r--   0 emily     (1000) emily     (1000)    47576 2022-05-08 18:18:35.000000 isisdl-1.3.7/src/isisdl/utils.py
--rw-r--r--   0 emily     (1000) emily     (1000)       22 2022-05-08 23:32:52.000000 isisdl-1.3.7/src/isisdl/version.py
-drwxr-xr-x   0 emily     (1000) emily     (1000)        0 2022-05-08 23:32:58.344627 isisdl-1.3.7/src/isisdl.egg-info/
--rw-r--r--   0 emily     (1000) emily     (1000)      554 2022-05-08 23:32:57.000000 isisdl-1.3.7/src/isisdl.egg-info/PKG-INFO
--rw-r--r--   0 emily     (1000) emily     (1000)      674 2022-05-08 23:32:58.000000 isisdl-1.3.7/src/isisdl.egg-info/SOURCES.txt
--rw-r--r--   0 emily     (1000) emily     (1000)        1 2022-05-08 23:32:57.000000 isisdl-1.3.7/src/isisdl.egg-info/dependency_links.txt
--rw-r--r--   0 emily     (1000) emily     (1000)       48 2022-05-08 23:32:58.000000 isisdl-1.3.7/src/isisdl.egg-info/entry_points.txt
--rw-r--r--   0 emily     (1000) emily     (1000)        1 2022-03-25 13:12:03.000000 isisdl-1.3.7/src/isisdl.egg-info/not-zip-safe
--rw-r--r--   0 emily     (1000) emily     (1000)      206 2022-05-08 23:32:58.000000 isisdl-1.3.7/src/isisdl.egg-info/requires.txt
--rw-r--r--   0 emily     (1000) emily     (1000)        7 2022-05-08 23:32:58.000000 isisdl-1.3.7/src/isisdl.egg-info/top_level.txt
+drwxr-xr-x   0 emily     (1000) emily     (1000)        0 2022-06-03 16:28:30.329557 isisdl-1.3.9/
+-rw-r--r--   0 emily     (1000) emily     (1000)    35149 2022-03-25 13:10:48.000000 isisdl-1.3.9/LICENSE
+-rw-r--r--   0 emily     (1000) emily     (1000)      544 2022-06-03 16:28:30.329557 isisdl-1.3.9/PKG-INFO
+-rw-r--r--   0 emily     (1000) emily     (1000)     3723 2022-06-02 22:49:42.000000 isisdl-1.3.9/README.md
+-rw-r--r--   0 emily     (1000) emily     (1000)      414 2022-05-30 17:25:14.000000 isisdl-1.3.9/pyproject.toml
+-rw-r--r--   0 emily     (1000) emily     (1000)      959 2022-06-03 16:28:30.329557 isisdl-1.3.9/setup.cfg
+-rw-r--r--   0 emily     (1000) emily     (1000)      262 2022-03-25 13:10:48.000000 isisdl-1.3.9/setup.py
+drwxr-xr-x   0 emily     (1000) emily     (1000)        0 2022-06-03 16:28:30.327556 isisdl-1.3.9/src/
+drwxr-xr-x   0 emily     (1000) emily     (1000)        0 2022-06-03 16:28:30.328557 isisdl-1.3.9/src/isisdl/
+-rw-r--r--   0 emily     (1000) emily     (1000)        0 2022-03-25 13:11:26.000000 isisdl-1.3.9/src/isisdl/__init__.py
+-rw-r--r--   0 emily     (1000) emily     (1000)     4242 2022-06-03 15:12:15.000000 isisdl-1.3.9/src/isisdl/__main__.py
+-rwxr-xr-x   0 emily     (1000) emily     (1000)      100 2022-05-30 17:25:14.000000 isisdl-1.3.9/src/isisdl/autorun.py
+drwxr-xr-x   0 emily     (1000) emily     (1000)        0 2022-06-03 16:28:30.329557 isisdl-1.3.9/src/isisdl/backend/
+-rw-r--r--   0 emily     (1000) emily     (1000)        0 2022-03-25 13:10:48.000000 isisdl-1.3.9/src/isisdl/backend/__init__.py
+-rw-r--r--   0 emily     (1000) emily     (1000)    19427 2022-06-02 22:08:41.000000 isisdl-1.3.9/src/isisdl/backend/config.py
+-rw-r--r--   0 emily     (1000) emily     (1000)     4339 2022-06-02 22:09:00.000000 isisdl-1.3.9/src/isisdl/backend/crypt.py
+-rw-r--r--   0 emily     (1000) emily     (1000)     9890 2022-05-30 17:25:14.000000 isisdl-1.3.9/src/isisdl/backend/database_helper.py
+-rw-r--r--   0 emily     (1000) emily     (1000)    48991 2022-06-03 16:09:06.000000 isisdl-1.3.9/src/isisdl/backend/request_helper.py
+-rw-r--r--   0 emily     (1000) emily     (1000)    10837 2022-05-30 17:25:14.000000 isisdl-1.3.9/src/isisdl/backend/status.py
+-rw-r--r--   0 emily     (1000) emily     (1000)     8360 2022-06-02 22:09:00.000000 isisdl-1.3.9/src/isisdl/backend/sync_database.py
+-rw-r--r--   0 emily     (1000) emily     (1000)    23251 2022-06-03 15:12:50.000000 isisdl-1.3.9/src/isisdl/compress.py
+-rw-r--r--   0 emily     (1000) emily     (1000)    13731 2022-06-03 16:24:44.000000 isisdl-1.3.9/src/isisdl/settings.py
+-rw-r--r--   0 emily     (1000) emily     (1000)    47789 2022-06-03 15:12:50.000000 isisdl-1.3.9/src/isisdl/utils.py
+-rw-r--r--   0 emily     (1000) emily     (1000)       22 2022-06-02 22:49:42.000000 isisdl-1.3.9/src/isisdl/version.py
+drwxr-xr-x   0 emily     (1000) emily     (1000)        0 2022-06-03 16:28:30.328557 isisdl-1.3.9/src/isisdl.egg-info/
+-rw-r--r--   0 emily     (1000) emily     (1000)      544 2022-06-03 16:28:29.000000 isisdl-1.3.9/src/isisdl.egg-info/PKG-INFO
+-rw-r--r--   0 emily     (1000) emily     (1000)      674 2022-06-03 16:28:30.000000 isisdl-1.3.9/src/isisdl.egg-info/SOURCES.txt
+-rw-r--r--   0 emily     (1000) emily     (1000)        1 2022-06-03 16:28:30.000000 isisdl-1.3.9/src/isisdl.egg-info/dependency_links.txt
+-rw-r--r--   0 emily     (1000) emily     (1000)       48 2022-06-03 16:28:30.000000 isisdl-1.3.9/src/isisdl.egg-info/entry_points.txt
+-rw-r--r--   0 emily     (1000) emily     (1000)        1 2022-03-25 13:12:03.000000 isisdl-1.3.9/src/isisdl.egg-info/not-zip-safe
+-rw-r--r--   0 emily     (1000) emily     (1000)      206 2022-06-03 16:28:30.000000 isisdl-1.3.9/src/isisdl.egg-info/requires.txt
+-rw-r--r--   0 emily     (1000) emily     (1000)        7 2022-06-03 16:28:30.000000 isisdl-1.3.9/src/isisdl.egg-info/top_level.txt
```

### Comparing `isisdl-1.3.7/LICENSE` & `isisdl-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `isisdl-1.3.7/PKG-INFO` & `isisdl-1.3.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isisdl
-Version: 1.3.7
+Version: 1.3.9
 Summary: Download *everything* from ISIS - with *speed*
 Author: Emily Seebeck
 License: GPL3
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
@@ -13,10 +13,7 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Provides-Extra: testing
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `isisdl-1.3.7/README.md` & `isisdl-1.3.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 ### It is *fast*
 
 Once all files are downloaded it takes about 5s to synchronize your files with ISIS.
 
 ### It downloads *everything*
 
 All the files from all of your ISIS courses are found and downloaded. Also, if a link to a file is posted on the ISIS
-page, it will get downloaded. This only works, if the file is an actual file - not a download link to a file.
+page, it will get downloaded. This might work depending on the link. Links to Google Drive and TUBCloud supported, and
+there is planned support for youtube, prezi, doi and some more libraries.
 
-Links to Google Drive and TUBCloud are also supported.
+*Note*: If you have a specific url you would like to have downloaded, feel free to submit an issue.
 
 ### Compatibility
 
 `isisdl` will run on any python interpreter that is ≥ 3.8.
 
 If you do not have access to Python, there is also a standalone executable, which will run on any Linux distribution and
 Windows version (with their respective binaries).
@@ -46,31 +47,31 @@
 This is especially useful, if you either don't want to download all video files, but still be able to view them
 with `vlc` (see the `--stream` option), or if you want to start watching videos while the download is still running.
 
 ## Installation
 
 ### Linux
 
-The recommended installation is with pip:
-
 ```shell
 pip install isisdl
 ```
 
 If you are running an Arch based distro, the standalone executable of `isisdl` is also available in the AUR:
 
 ```shell
 yay -S isisdl
 ```
 
 ### Windows
 
-The recommended installation is by downloading the latest standalone executable from the [releases page]().
+The recommended installation is by downloading the latest standalone executable from
+[here](https://github.com/Emily3403/isisdl/releases/latest/download/isisdl-windows.exe).
 
-It does not rely on any installation or python version.
+There may be a Windows defender / smartscreen warning about this executable not being recognized. This is due to the fact
+that there are few Windows users. Simply ignore the warning. 
 
 ### Troubleshooting
 
 If you are having problems see the
 [troubleshoot guide](https://github.com/Emily3403/isisdl/wiki/Installation#help-my-install-isnt-working) for solutions.
 
 ## Additional options
@@ -86,13 +87,12 @@
 
 [//]: # (- `--subscribe`: Subscribes you to *all* publicly available courses)
 
 [//]: # (- `--unsubscribe`: Unsubscribes you from the courses you subscribed to.)
 
 ## Future Ideas
 
-
 ### Sharing of compressed videos
 
 Compressed videos could be saved and distributed from a central server. The access would be restricted, so there is no
 copyright infringement. If you want to participate in that you can soon™ request access.
```

### Comparing `isisdl-1.3.7/setup.cfg` & `isisdl-1.3.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `isisdl-1.3.7/src/isisdl/backend/config.py` & `isisdl-1.3.9/src/isisdl/backend/config.py`

 * *Files identical despite different names*

### Comparing `isisdl-1.3.7/src/isisdl/backend/crypt.py` & `isisdl-1.3.9/src/isisdl/backend/crypt.py`

 * *Files identical despite different names*

### Comparing `isisdl-1.3.7/src/isisdl/backend/database_helper.py` & `isisdl-1.3.9/src/isisdl/backend/database_helper.py`

 * *Files identical despite different names*

### Comparing `isisdl-1.3.7/src/isisdl/backend/request_helper.py` & `isisdl-1.3.9/src/isisdl/backend/request_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime
 from email.utils import parsedate_to_datetime
 from itertools import repeat, chain
 from pathlib import Path
 from queue import Queue
 from threading import Thread, Lock, current_thread
-from typing import Optional, Dict, List, Any, cast, Union, Iterable, DefaultDict, Tuple
+from typing import Optional, Dict, List, Any, cast, Union, Iterable, DefaultDict, Tuple, Set
 from urllib.parse import urlparse
 
 from requests import Session, Response
 from requests.adapters import HTTPAdapter
 from requests.exceptions import InvalidSchema
 
 from isisdl.backend.crypt import get_credentials
@@ -411,15 +411,15 @@
 
     def dump(self) -> MediaContainer:
         database_helper.add_pre_container(self)
         return self
 
     def string_dump(self) -> str:
         return f"Name: {sanitize_name(self._name, False)!r}\nCourse: {self.course!r}\nSize: {HumanBytes.format_str(self.size)}\n" \
-               f"Time: {datetime.fromtimestamp(self.time).strftime(datetime_str)}\nIs downloaded: {self.checksum is not None}\n"
+               f"Time: {datetime.fromtimestamp(self.time).strftime(datetime_str)}\nIs downloaded: {self.checksum is not None}\nPath: {self.path}\n"
 
     def __str__(self) -> str:
         if config.absolute_path_filename:
             return str(self.path)
 
         return sanitize_name(self._name, False)
 
@@ -457,15 +457,15 @@
             return
 
         if self.current_size is not None:
             return
 
         self.current_size = 0
 
-        if not self.should_download:
+        if not self.should_download and self.url != 'https://www.eecs.tu-berlin.de/fileadmin/f4/fkIVdokumente/studium/Plagiate/Merkblatt_Plagiate_Fak.IV_05-2020.pdf':
             self.current_size = self.size
             self._done = True
             return
 
         if is_stream:
             throttler.start_stream(self.path)
 
@@ -577,41 +577,14 @@
         if was_in_configuration is False and self.ok:
             os.makedirs(self.path(), exist_ok=True)
 
             if config.make_subdirs:
                 for item in MediaType.list_dirs():
                     os.makedirs(self.path(item), exist_ok=True)
 
-    def download_videos(self, s: SessionWithKey) -> List[PreMediaContainer]:
-        if config.download_videos is False:
-            return []
-
-        url = "https://isis.tu-berlin.de/lib/ajax/service.php"
-        # Thank you isia-tub for this data <3
-        video_data = [{
-            "methodname": "mod_videoservice_get_videos",
-            "args": {"courseid": self.course_id}
-        }]
-
-        videos_res = s.get_(url, params={"sesskey": s.key}, json=video_data)
-
-        if videos_res is None or not videos_res.ok:
-            return []
-
-        videos_json = videos_res.json()[0]
-
-        if videos_json["error"]:
-            return []
-
-        videos_json = videos_json["data"]["videos"]
-        video_urls = [item["url"] for item in videos_json]
-        video_names = [item["title"].strip() + item["fileext"] for item in videos_json]
-
-        return [PreMediaContainer(url, self, MediaType.video, name) for url, name in zip(video_urls, video_names)]
-
     def download_documents(self, helper: RequestHelper) -> List[PreMediaContainer]:
         content = helper.post_REST("core_course_get_contents", {"courseid": self.course_id})
         if content is None or isinstance(content, dict) and "exception" in content:
             return []
 
         content = cast(List[Dict[str, Any]], content)
         all_content: List[PreMediaContainer] = []
@@ -710,14 +683,15 @@
     session: SessionWithKey
     courses: List[Course]
     _courses: List[Course]
     _meta_info: Dict[str, str]
     course_id_mapping: Dict[int, Course] = {}
     _instance: Optional[RequestHelper] = None
     _instance_init: bool = False
+    _lock = Lock()
 
     def __init__(self, user: User, status: Optional[RequestHelperStatus] = None):
         if self._instance_init:
             return
 
         if status is not None:
             status.set_status(StatusOptions.authenticating)
@@ -792,31 +766,31 @@
 
         if response is None or not response.ok:
             return None
 
         return response.json()
 
     def download_content(self, status: Optional[RequestHelperStatus] = None) -> Dict[MediaType, List[MediaContainer]]:
-        exception_lock = Lock()
-
         if status is not None:
             status.set_total(len(self.courses))
 
         if enable_multithread:
             with ThreadPoolExecutor(discover_num_threads) as ex:
+                # Note the use of .map() instead of .submit(). This is done so in both cases the variable can be of type `Iterable`.
+                # If done with .submit() one would have to wrap the function call into a `Future` which is too cumbersome.
                 _mod_assign = ex.map(self._download_mod_assign, [0])
-                _document_containers = ex.map(self._download_documents, self.courses, repeat(exception_lock))
-                _video_containers = ex.map(self._download_videos, self.courses, repeat(exception_lock), repeat(status))
+                _video_containers = ex.map(self._download_videos, [0])
+                _document_containers = ex.map(self._download_documents, self.courses, repeat(status))
 
         else:
-            _mod_assign = iter([self._download_mod_assign()])
-            _document_containers = iter([self._download_documents(course, exception_lock) for course in self.courses])
-            _video_containers = iter([self._download_videos(course, exception_lock, status) for course in self.courses])
+            _mod_assign = iter([self._download_mod_assign(0)])
+            _video_containers = iter([self._download_videos(0)])
+            _document_containers = iter([self._download_documents(course, status) for course in self.courses])
 
-        pre_containers = [item for row in chain(_document_containers, _video_containers, _mod_assign) for item in row]
+        pre_containers = [item for row in filter(lambda x: x is not None, chain(_document_containers, _video_containers, _mod_assign)) for item in row]
         pre_containers = list({f"{item.course} {item.url}": item for item in pre_containers}.values())
         random.shuffle(pre_containers)
 
         if (num_cached := sum(pre_container.is_cached for pre_container in pre_containers)) != len(pre_containers):
             if status is not None:
                 status.set_total(len([item for item in pre_containers if not item.is_ready]))
                 status.count = num_cached
@@ -839,49 +813,84 @@
 
         for container in containers:
             mapping[container.media_type].append(container)
 
         return {typ: sorted(item, key=lambda x: x.time, reverse=True) for typ, item in mapping.items()}
 
     def _download_mod_assign(self, _: Any = None) -> List[PreMediaContainer]:
-        all_content = []
-        _assignments = self.post_REST("mod_assign_get_assignments", use_timeout=False)
-        if _assignments is None:
-            return []
+        try:
+            all_content = []
+            _assignments = self.post_REST("mod_assign_get_assignments", use_timeout=False)
+            if _assignments is None:
+                assignments = cast(Dict[str, Any], _assignments)
+
+                allowed_ids = {item.course_id for item in self.courses}
+                for _course in assignments["courses"]:
+                    if _course["id"] in allowed_ids:
+                        for assignment in _course["assignments"]:
+                            if "introattachments" not in assignment:
+                                continue
+
+                            for file in assignment["introattachments"]:
+                                file["filepath"] = assignment["name"]
+                                all_content.append(PreMediaContainer(
+                                    file["fileurl"], RequestHelper.course_id_mapping[_course["id"]], MediaType.document,
+                                    file["filename"], file["filepath"], file["filesize"], file["timemodified"])
+                                )
 
-        assignments = cast(Dict[str, Any], _assignments)
+                return all_content
 
-        allowed_ids = {item.course_id for item in self.courses}
-        for _course in assignments["courses"]:
-            if _course["id"] in allowed_ids:
-                for assignment in _course["assignments"]:
-                    if "introattachments" not in assignment:
-                        continue
-
-                    for file in assignment["introattachments"]:
-                        file["filepath"] = assignment["name"]
-                        all_content.append(PreMediaContainer(file["fileurl"], RequestHelper.course_id_mapping[_course["id"]], MediaType.document,
-                                                             file["filename"], file["filepath"], file["filesize"], file["timemodified"]))
+        except Exception as ex:
+            with self._lock:
+                generate_error_message(ex)
 
-        return all_content
+        return []
 
-    def _download_documents(self, course: Course, exception_lock: Lock) -> List[PreMediaContainer]:
+    def _download_videos(self, _: Any) -> List[PreMediaContainer]:
         try:
-            return course.download_documents(self)
+            if config.download_videos is False:
+                return []
+
+            url = "https://isis.tu-berlin.de/lib/ajax/service.php"
+            # Thank you isia-tub for discovering this service.
+            video_data = [{
+                "methodname": "mod_videoservice_get_videos",
+                "args": {"courseid": course.course_id},
+                "index": i
+            } for i, course in enumerate(self.courses)]
+
+            videos_res = self.session.get_(url, params={"sesskey": self.session.key}, json=video_data)
+
+            if videos_res is None or not videos_res.ok:
+                return []
+
+            res = []
+            for course, video in zip(self.courses, videos_res.json()):
+                if video["error"]:
+                    continue
+                assert course.course_id == video["data"]["courseid"]
+
+                videos_json = video["data"]["videos"]
+                video_urls = [item["url"] for item in videos_json]
+                video_names = [item["title"].strip() + item["fileext"] for item in videos_json]
+
+                res.extend([PreMediaContainer(url, course, MediaType.video, name) for url, name in zip(video_urls, video_names)])
+
+            return res
 
         except Exception as ex:
-            with exception_lock:
+            with self._lock:
                 generate_error_message(ex)
 
-    def _download_videos(self, course: Course, exception_lock: Lock, status: Optional[RequestHelperStatus] = None) -> List[PreMediaContainer]:
+    def _download_documents(self, course: Course, status: Optional[RequestHelperStatus] = None) -> List[PreMediaContainer]:
         try:
-            return course.download_videos(self.session)
+            return course.download_documents(self)
 
         except Exception as ex:
-            with exception_lock:
+            with self._lock:
                 generate_error_message(ex)
 
         finally:
             if status is not None:
                 status.done()
 
 
@@ -894,30 +903,16 @@
         if file.media_type == MediaType.corrupted:
             final_list.append(file)
         else:
             new_files.append(file)
 
     files = new_files
 
-    # First check for the same urls across the entire list
-    hard_link_conflicts: DefaultDict[str, List[MediaContainer]] = defaultdict(list)
-
-    for file in {file.path: file for file in files}.values():
-        hard_link_conflicts[file.download_url].append(file)
-
-    for conflict in hard_link_conflicts.values():
-        if len(conflict) != 1:
-            conflict.sort(key=lambda x: x.time)
-            conflict[0]._links.extend(conflict[1:])
-            final_list.append(conflict[0])
-            for item in conflict[0]._links:
-                files.remove(item)
-
     # Now check for files with the same size in each course
-    hard_link_conflicts = defaultdict(list)
+    hard_link_conflicts: DefaultDict[str, List[MediaContainer]] = defaultdict(list)
 
     for file in {file.path: file for file in files}.values():
         hard_link_conflicts[f"{file.course.course_id} {file._name} {file.size}"].append(file)
 
     for conflict in hard_link_conflicts.values():
         if len(conflict) != 1:
             conflict.sort(key=lambda x: x.time)
@@ -949,15 +944,37 @@
                 file.dump()
                 final_list.append(file)
 
         else:
             logger.assert_fail(f"conflict: {[{x: getattr(item, x) for x in item.__slots__} for item in conflict]}")
             continue
 
-    return final_list
+    # TODO: This takes too long.
+
+    # Finally filter the remaining files based on the url
+    hard_link_conflicts = defaultdict(list)
+
+    for file in {file.path: file for file in files}.values():
+        hard_link_conflicts[file.download_url].append(file)
+
+    conflict_urls: Set[str] = set()
+    new_files = []
+
+    for conflict in hard_link_conflicts.values():
+        if len(conflict) != 1:
+            conflict.sort(key=lambda x: x.time)
+            conflict[0]._links.extend(conflict[1:])
+            conflict_urls.add(conflict[0].url)
+            new_files.append(conflict[0])
+
+            final_list.append(conflict[0])
+            for item in conflict[0]._links:
+                final_list.remove(item)
+
+    return [file for file in final_list if file.url not in conflict_urls] + new_files
 
 
 class Downloader(Thread):
     q: Queue[MediaContainer]
     ret_q: Queue[int]
     thread_id: int
     status: DownloadStatus
```

### Comparing `isisdl-1.3.7/src/isisdl/backend/status.py` & `isisdl-1.3.9/src/isisdl/backend/status.py`

 * *Files identical despite different names*

### Comparing `isisdl-1.3.7/src/isisdl/backend/sync_database.py` & `isisdl-1.3.9/src/isisdl/backend/sync_database.py`

 * *Files identical despite different names*

### Comparing `isisdl-1.3.7/src/isisdl/compress.py` & `isisdl-1.3.9/src/isisdl/compress.py`

 * *Files 1% similar despite different names*

```diff
@@ -422,14 +422,15 @@
 
         log_strings = ["", "", "Summary of course size savings:", ""]
 
         for course_id, info in sorted(infos.items()):
             if info['num_processed'] == 0:
                 continue
 
+            # TODO: Indicate what the values mean
             out = f"{str(course_name_mapping[course_id]).ljust(max_course_name_len)} "
             out += f"{str(info['num_processed']).rjust(max_processed_file_len)} file{'s' if info['num_processed'] != 1 else ' '}  "
 
             if info['size_compressed']:
                 out += f"{calculate_efficiency(info['size_compressed'], info['total_size'] - info['size_skipped']) * 100:6.2f}%  "
             else:
                 out += "  ---    "
@@ -458,41 +459,41 @@
             popen = partial(subprocess.Popen, preexec_fn=lambda: os.setpgrp())
 
         for file in files:
             if stop_encoding:
                 stop_encoding = False
                 return
 
-            new_file_name = make_temp_filename(file)
+            tmp_file_name = make_temp_filename(file)
 
             if not file.path:
                 continue
 
             ffmpeg = popen([
                 "ffmpeg",
                 "-i", str(file.path),
                 "-y", "-loglevel", "warning", "-stats",
                 "-movflags", "use_metadata_tags", "-metadata", f"previous_size=\"{file.size}\"",
                 *ffmpeg_args,
                 "-x265-params", "log-level=0",
-                new_file_name
+                tmp_file_name
             ], stdin=subprocess.DEVNULL, stderr=subprocess.PIPE, universal_newlines=True)
             current_pid = ffmpeg.pid
 
             compress_status.start_thing(file, ffmpeg)
             ret_code = ffmpeg.wait()
 
             compress_status.done_thing(ret_code == 0)
 
             if ret_code == 0:
-                file.path.replace(new_file_name)
+                os.replace(tmp_file_name, file.path)
 
             else:
                 try:
-                    os.remove(new_file_name)
+                    os.remove(tmp_file_name)
                 except OSError:
                     pass
 
         stop_encoding = False
         compress_status.generate_final_message()
 
     except Exception as ex:
@@ -545,15 +546,15 @@
             continue
 
         if "bit_rate" not in vid_probe:
             continue
 
         content_and_score.append((con, int(vid_probe["bit_rate"])))
 
-    content = [item for item, _ in sorted(content_and_score, key=lambda pair: pair[1], reverse=False)]
+    content = [item for item, _ in sorted(content_and_score, key=lambda pair: pair[1], reverse=True)]
     compress_status = CompressStatus(content + inefficient_videos + already_h265, helper)
     compress_status.start()
 
     # Run the conversion in a separate thread so, if killed, it will still run
     compress_thread = Thread(target=compress, args=(content,))
     compress_thread.start()
     compress_thread.join()
@@ -561,8 +562,8 @@
 
 compress_status: Optional[CompressStatus] = None
 compress_thread: Optional[Thread] = None
 
 # TODO:
 #   Human readable for compression score
 #   Remote compression?
-#   Online ffprobe
+#   Hard links are not handled transparently
```

### Comparing `isisdl-1.3.7/src/isisdl/settings.py` & `isisdl-1.3.9/src/isisdl/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,14 @@
 # The name of the SQLite Database
 database_file_location = ".state.db"
 
 log_file_location = "isisdl.log"
 
 datetime_str = "%Y-%m-%d %H:%M:%S"
 
-# Fallback current database version
-current_database_version = 2
-
 # Settings for the lock
 lock_file_location = ".lock"
 enable_lock = True
 
 # Options for the `--subscribe` feature
 subscribed_courses_file_location = "subscribed_courses.json"
 subscribe_num_courses_to_subscribe_to = -1
```

### Comparing `isisdl-1.3.7/src/isisdl/utils.py` & `isisdl-1.3.9/src/isisdl/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,43 +35,45 @@
 import requests
 from packaging import version
 from packaging.version import Version, LegacyVersion
 from requests import Session
 
 from isisdl import settings
 from isisdl.backend.database_helper import DatabaseHelper
-from isisdl.settings import download_chunk_size, token_queue_download_refresh_rate, forbidden_chars, replace_dot_at_end_of_dir_name, force_filesystem
+from isisdl.settings import download_chunk_size, token_queue_download_refresh_rate, forbidden_chars, replace_dot_at_end_of_dir_name, force_filesystem, has_ffmpeg, fstype
 from isisdl.settings import working_dir_location, is_windows, checksum_algorithm, checksum_num_bytes, example_config_file_location, config_dir_location, database_file_location, status_time, \
     discover_num_threads, status_progress_bar_resolution, download_progress_bar_resolution, config_file_location, is_first_time, is_autorun, parse_config_file, lock_file_location, \
     enable_lock, error_directory_location, systemd_dir_location, master_password, is_testing, systemd_timer_file_location, systemd_service_file_location, export_config_file_location, \
     isisdl_executable, is_static, enable_multithread, subscribe_num_threads, subscribed_courses_file_location, error_text, token_queue_refresh_rate
 from isisdl.version import __version__
 
 if TYPE_CHECKING:
     from isisdl.backend.status import Status
     from isisdl.backend.request_helper import RequestHelper
 
 
 def get_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="isisdl", formatter_class=argparse.RawTextHelpFormatter, description="""
-    This program downloads all content from your ISIS profile.""")
+    This program downloads and synchronizes all of your ISIS content.""")
 
     parser.add_argument("-t", "--max-num-threads", help="The maximum number of threads to spawn (for downloading files)\n ", type=int, default=3, metavar="{num}")
     parser.add_argument("-d", "--download-rate", help="Limits the download rate to {num} MiB/s\n ", type=float, default=None, metavar="{num}")
 
     operations = parser.add_mutually_exclusive_group()
 
     operations.add_argument("-v", "--version", help="Print the version number and exit", action="store_true")
     operations.add_argument("--init", help="Guides you through the initial configuration and setup process.", action="store_true")
     operations.add_argument("--config", help="Guides you through additional configuration which focuses on what to download from ISIS.", action="store_true")
-    operations.add_argument("--sync", help="Synchronizes the local database with ISIS. Will delete not existent or corrupted entries.", action="store_true")
+    operations.add_argument("--sync", help="Do a full reset of the database, updating all file locations and urls.", action="store_true")
     operations.add_argument("--compress", help="Starts ffmpeg and will compress all downloaded videos.", action="store_true")
     operations.add_argument("--subscribe", help="Subscribes you to *all* ISIS courses publicly available.", action="store_true")
     operations.add_argument("--unsubscribe", help="Unsubscribes you from the courses you got subscribed by running `isisdl --subscribe`.", action="store_true")
-    operations.add_argument("--export-config", help=f"Exports the config to {export_config_file_location}", action="store_true")
+    if not is_windows:
+        operations.add_argument("--export-config", help=f"Exports the config to {export_config_file_location}.", action="store_true")
+
     operations.add_argument("--stream", help="Launches isisdl in streaming mode. Will watch for file accesses and download only those files.", action="store_true")
     operations.add_argument("--update", help="Checks if an update is available and installs it.", action="store_true")
     operations.add_argument("--delete-bad-urls", help="Deletes all urls deemed to be \"bad\" - meaning there is no content.", action="store_true")
 
     if is_testing:
         return parser.parse_known_args()[0]
 
@@ -623,15 +625,14 @@
 
     if "pip" in config.update_policy:
         ret = subprocess.call([sys.executable, "-m", "pip", "install", "--upgrade", "isisdl"])
 
     elif "github" in config.update_policy and is_static is False:
         ret = subprocess.call([sys.executable, "-m", "pip", "install", "git+https://github.com/Emily3403/isisdl"])
 
-    # TODO: test if this will work
     elif "github" in config.update_policy and is_static:
         with TemporaryDirectory() as tmp:
             assets = requests.get("https://api.github.com/repos/Emily3403/isisdl/releases/latest").json()["assets"]
             correct_name = "isisdl-windows.exe" if is_windows else "isisdl-linux.bin"
             for asset in assets:
                 if asset["name"] == correct_name:
                     break
@@ -1130,40 +1131,44 @@
         self.messages = Queue()
         self.done = Queue()
         self.generic_msg = {
             "username": User.sanitize_name(config.username),
             "OS": platform.system(),
             "OS_spec": distro.id(),
             "version": __version__,
+            "database_version": Config.default("database_version"),
+            "has_ffmpeg": has_ffmpeg,
+            "forbidden_chars": list(forbidden_chars),
+            "fstype": fstype,
             "is_static": is_static,
             "time": int(time.time()),
             "is_first_time": is_first_time,
         }
 
         super().__init__(daemon=True)
         self.start()
 
     def run(self) -> None:
-        while True:
-            item = self.messages.get()
-            self.s.post("http://49.12.42.246/isisdl/", json=item)
-            self.done.put(None)
+        try:
+            while True:
+                item = self.messages.get()
+                self.s.post("http://49.12.42.246/isisdl/", json=item)
+                self.done.put(None)
+        except Exception as ex:
+            generate_error_message(ex)
 
     def message(self, msg: Union[str, Dict[str, Any]]) -> None:
         if config.telemetry_policy is False or is_testing:
             return
 
         deliver = self.generic_msg.copy()
         deliver["message"] = msg
         self.messages.put(deliver)
 
     def assert_fail(self, msg: str) -> None:
-        if config.telemetry_policy is False or is_testing:
-            return
-
         self.message(f"Assertion failed: {msg}")
 
     def post(self, msg: Dict[str, Any]) -> None:
         if config.telemetry_policy is False or is_testing:
             return
 
         deliver = self.generic_msg.copy()
```

### Comparing `isisdl-1.3.7/src/isisdl.egg-info/PKG-INFO` & `isisdl-1.3.9/src/isisdl.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isisdl
-Version: 1.3.7
+Version: 1.3.9
 Summary: Download *everything* from ISIS - with *speed*
 Author: Emily Seebeck
 License: GPL3
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
@@ -13,10 +13,7 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Provides-Extra: testing
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `isisdl-1.3.7/src/isisdl.egg-info/SOURCES.txt` & `isisdl-1.3.9/src/isisdl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

