# Comparing `tmp/pyunfoldedcircleremote-0.7.1.tar.gz` & `tmp/pyunfoldedcircleremote-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyunfoldedcircleremote-0.7.1.tar", max compression
+gzip compressed data, was "pyunfoldedcircleremote-0.7.2.tar", max compression
```

## Comparing `pyunfoldedcircleremote-0.7.1.tar` & `pyunfoldedcircleremote-0.7.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-11-11 18:51:29.176913 pyunfoldedcircleremote-0.7.1/LICENSE
--rw-r--r--   0        0        0      119 2023-11-11 18:52:24.241472 pyunfoldedcircleremote-0.7.1/README.md
--rw-r--r--   0        0        0      604 2024-04-22 22:12:00.976251 pyunfoldedcircleremote-0.7.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-03 21:50:52.813920 pyunfoldedcircleremote-0.7.1/src/pyUnfoldedCircleRemote/__init__.py
--rw-r--r--   0        0        0      783 2024-04-21 21:46:12.575871 pyunfoldedcircleremote-0.7.1/src/pyUnfoldedCircleRemote/const.py
--rw-r--r--   0        0        0    66147 2024-04-22 22:12:06.194670 pyunfoldedcircleremote-0.7.1/src/pyUnfoldedCircleRemote/remote.py
--rw-r--r--   0        0        0     7345 2024-03-17 01:49:19.890767 pyunfoldedcircleremote-0.7.1/src/pyUnfoldedCircleRemote/remote_websocket.py
--rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 pyunfoldedcircleremote-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-11-11 18:51:29.176913 pyunfoldedcircleremote-0.7.2/LICENSE
+-rw-r--r--   0        0        0      119 2023-11-11 18:52:24.241472 pyunfoldedcircleremote-0.7.2/README.md
+-rw-r--r--   0        0        0      604 2024-05-17 17:17:27.690119 pyunfoldedcircleremote-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-03 21:50:52.813920 pyunfoldedcircleremote-0.7.2/src/pyUnfoldedCircleRemote/__init__.py
+-rw-r--r--   0        0        0      783 2024-04-21 21:46:12.575871 pyunfoldedcircleremote-0.7.2/src/pyUnfoldedCircleRemote/const.py
+-rw-r--r--   0        0        0    67891 2024-05-17 17:14:10.836759 pyunfoldedcircleremote-0.7.2/src/pyUnfoldedCircleRemote/remote.py
+-rw-r--r--   0        0        0     7345 2024-03-17 01:49:19.890767 pyunfoldedcircleremote-0.7.2/src/pyUnfoldedCircleRemote/remote_websocket.py
+-rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 pyunfoldedcircleremote-0.7.2/PKG-INFO
```

### Comparing `pyunfoldedcircleremote-0.7.1/LICENSE` & `pyunfoldedcircleremote-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyunfoldedcircleremote-0.7.1/pyproject.toml` & `pyunfoldedcircleremote-0.7.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyUnfoldedCircleRemote"
-version = "0.7.1"
+version = "0.7.2"
 description = "A python library to interact with the Unfolded Circle Remote"
 authors = ["Jack Powell <jackjpowell@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jackjpowell/py-unfolded-circle"
 packages = [{include = "pyUnfoldedCircleRemote", from = "src"}]
```

### Comparing `pyunfoldedcircleremote-0.7.1/src/pyUnfoldedCircleRemote/const.py` & `pyunfoldedcircleremote-0.7.2/src/pyUnfoldedCircleRemote/const.py`

 * *Files identical despite different names*

### Comparing `pyunfoldedcircleremote-0.7.1/src/pyUnfoldedCircleRemote/remote.py` & `pyunfoldedcircleremote-0.7.2/src/pyUnfoldedCircleRemote/remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -806,60 +806,95 @@
         async with (
             self.client() as session,
             session.get(self.url("system/update")) as response,
         ):
             await self.raise_on_error(response)
             information = await response.json()
             self._update_in_progress = information["update_in_progress"]
-            # self._next_update_check_date = information["next_check_date"]
             self._sw_version = information["installed_version"]
             self._automatic_updates = information["update_check_enabled"]
+            download_status = ""
             if "available" in information:
                 self._available_update = information["available"]
                 for update in self._available_update:
                     if update.get("channel") in ["STABLE", "TESTING"]:
                         if (
                             self._latest_sw_version == ""
                             or self._latest_sw_version < update.get("version")
                         ):
                             self._release_notes_url = update.get("release_notes_url")
                             self._latest_sw_version = update.get("version")
                             self._release_notes = update.get("description").get("en")
+                            download_status = update.get("download")
                     else:
                         self._latest_sw_version = self._sw_version
             else:
                 self._latest_sw_version = self._sw_version
+
+            if download_status in ("PENDING", "ERROR"):
+                try:
+                    # When download status is pending, the first request to system/update
+                    # will request the download of the latest firmware but will not install
+                    response = await self.update_remote()
+                except HTTPError:
+                    pass
             return information
 
     async def get_remote_force_update_information(self) -> bool:
         """Force a remote firmware update check."""
         async with (
             self.client() as session,
             session.put(self.url("system/update")) as response,
         ):
             await self.raise_on_error(response)
             information = await response.json()
             self._update_in_progress = information["update_in_progress"]
-            # self._next_update_check_date = information["next_check_date"]
             self._sw_version = information["installed_version"]
             self._automatic_updates = information["update_check_enabled"]
+            download_status = ""
             if "available" in information:
                 self._available_update = information["available"]
+                for update in self._available_update:
+                    if update.get("channel") in ["STABLE", "TESTING"]:
+                        if (
+                            self._latest_sw_version == ""
+                            or self._latest_sw_version < update.get("version")
+                        ):
+                            self._release_notes_url = update.get("release_notes_url")
+                            self._latest_sw_version = update.get("version")
+                            self._release_notes = update.get("description").get("en")
+                            download_status = update.get("download")
+                    else:
+                        self._latest_sw_version = self._sw_version
+            else:
+                self._latest_sw_version = self._sw_version
+
+            if download_status in ("PENDING", "ERROR"):
+                try:
+                    # When download status is pending, the first request to system/update
+                    # will request the download of the latest firmware but will not install
+                    response = await self.update_remote()
+                except HTTPError:
+                    pass
             return information
 
     async def update_remote(self) -> str:
         """Update Remote."""
         # WIP: Starts the latest firmware update."
         async with (
             self.client() as session,
             session.post(self.url("system/update/latest")) as response,
         ):
             await self.raise_on_error(response)
-            self._update_in_progress = True
             information = await response.json()
+            if information.get("state") == "DOWNLOAD":
+                self._update_in_progress = False
+
+            if information.get("state") == "START":
+                self._update_in_progress = True
             return information
 
     async def get_update_status(self) -> str:
         """Update remote status."""
         # WIP: Gets Update Status -- Only supports latest."
         async with (
             self.client() as session,
@@ -1262,14 +1297,15 @@
             self.get_remote_button_settings(),
             self.get_remote_sound_settings(),
             self.get_remote_haptic_settings(),
             self.get_remote_power_saving_settings(),
             self.get_activities(),
             self.get_remote_codesets(),
             self.get_docks(),
+            self.get_remote_wifi_info(),
         )
         await group
 
         await self.get_activity_groups()
 
         for activity_group in self.activity_groups:
             await activity_group.update()
```

### Comparing `pyunfoldedcircleremote-0.7.1/src/pyUnfoldedCircleRemote/remote_websocket.py` & `pyunfoldedcircleremote-0.7.2/src/pyUnfoldedCircleRemote/remote_websocket.py`

 * *Files identical despite different names*

### Comparing `pyunfoldedcircleremote-0.7.1/PKG-INFO` & `pyunfoldedcircleremote-0.7.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyUnfoldedCircleRemote
-Version: 0.7.1
+Version: 0.7.2
 Summary: A python library to interact with the Unfolded Circle Remote
 Home-page: https://github.com/jackjpowell/py-unfolded-circle
 License: MIT
 Author: Jack Powell
 Author-email: jackjpowell@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

