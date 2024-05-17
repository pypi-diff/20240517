# Comparing `tmp/neon-phal-plugin-device-updater-0.2.0.tar.gz` & `tmp/neon-phal-plugin-device-updater-0.2.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-phal-plugin-device-updater-0.2.0.tar", last modified: Mon Apr 22 20:22:22 2024, max compression
+gzip compressed data, was "neon-phal-plugin-device-updater-0.2.1a1.tar", last modified: Fri May 17 20:01:40 2024, max compression
```

## Comparing `neon-phal-plugin-device-updater-0.2.0.tar` & `neon-phal-plugin-device-updater-0.2.1a1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:22:22.812146 neon-phal-plugin-device-updater-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-22 20:22:17.000000 neon-phal-plugin-device-updater-0.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-22 20:22:22.812146 neon-phal-plugin-device-updater-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-22 20:22:17.000000 neon-phal-plugin-device-updater-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:22:22.812146 neon-phal-plugin-device-updater-0.2.0/neon_phal_plugin_device_updater/
--rw-r--r--   0 runner    (1001) docker     (127)    23786 2024-04-22 20:22:17.000000 neon-phal-plugin-device-updater-0.2.0/neon_phal_plugin_device_updater/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:22:22.812146 neon-phal-plugin-device-updater-0.2.0/neon_phal_plugin_device_updater.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-22 20:22:22.000000 neon-phal-plugin-device-updater-0.2.0/neon_phal_plugin_device_updater.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-22 20:22:22.000000 neon-phal-plugin-device-updater-0.2.0/neon_phal_plugin_device_updater.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 20:22:22.000000 neon-phal-plugin-device-updater-0.2.0/neon_phal_plugin_device_updater.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-22 20:22:22.000000 neon-phal-plugin-device-updater-0.2.0/neon_phal_plugin_device_updater.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-22 20:22:22.000000 neon-phal-plugin-device-updater-0.2.0/neon_phal_plugin_device_updater.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-22 20:22:22.000000 neon-phal-plugin-device-updater-0.2.0/neon_phal_plugin_device_updater.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 20:22:22.812146 neon-phal-plugin-device-updater-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-22 20:22:17.000000 neon-phal-plugin-device-updater-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:01:40.269443 neon-phal-plugin-device-updater-0.2.1a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-17 20:01:37.000000 neon-phal-plugin-device-updater-0.2.1a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-17 20:01:40.269443 neon-phal-plugin-device-updater-0.2.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-17 20:01:37.000000 neon-phal-plugin-device-updater-0.2.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:01:40.265443 neon-phal-plugin-device-updater-0.2.1a1/neon_phal_plugin_device_updater/
+-rw-r--r--   0 runner    (1001) docker     (127)    24032 2024-05-17 20:01:37.000000 neon-phal-plugin-device-updater-0.2.1a1/neon_phal_plugin_device_updater/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:01:40.269443 neon-phal-plugin-device-updater-0.2.1a1/neon_phal_plugin_device_updater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-17 20:01:40.000000 neon-phal-plugin-device-updater-0.2.1a1/neon_phal_plugin_device_updater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-17 20:01:40.000000 neon-phal-plugin-device-updater-0.2.1a1/neon_phal_plugin_device_updater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 20:01:40.000000 neon-phal-plugin-device-updater-0.2.1a1/neon_phal_plugin_device_updater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-17 20:01:40.000000 neon-phal-plugin-device-updater-0.2.1a1/neon_phal_plugin_device_updater.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-17 20:01:40.000000 neon-phal-plugin-device-updater-0.2.1a1/neon_phal_plugin_device_updater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-17 20:01:40.000000 neon-phal-plugin-device-updater-0.2.1a1/neon_phal_plugin_device_updater.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 20:01:40.269443 neon-phal-plugin-device-updater-0.2.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-05-17 20:01:37.000000 neon-phal-plugin-device-updater-0.2.1a1/setup.py
```

### Comparing `neon-phal-plugin-device-updater-0.2.0/LICENSE.md` & `neon-phal-plugin-device-updater-0.2.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-device-updater-0.2.0/PKG-INFO` & `neon-phal-plugin-device-updater-0.2.1a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-device-updater
-Version: 0.2.0
+Version: 0.2.1a1
 Summary: Core Module Update Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-device-updater
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-device-updater-0.2.0/README.md` & `neon-phal-plugin-device-updater-0.2.1a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-device-updater-0.2.0/neon_phal_plugin_device_updater/__init__.py` & `neon-phal-plugin-device-updater-0.2.1a1/neon_phal_plugin_device_updater/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,21 +88,19 @@
     def initramfs_hash(self) -> Optional[str]:
         """
         Get the MD5 hash of the currently installed InitramFS
         """
         if not self._initramfs_hash:
             try:
                 Popen("mount_firmware", shell=True).wait(5)
-                with open(self.initramfs_real_path, "rb") as f:
-                    self._initramfs_hash = hashlib.md5(f.read()).hexdigest()
             except Exception as e:
                 LOG.error(e)
-                if isfile(self.initramfs_real_path):
-                    with open(self.initramfs_real_path, "rb") as f:
-                        self._initramfs_hash = hashlib.md5(f.read()).hexdigest()
+            if isfile(self.initramfs_real_path):
+                with open(self.initramfs_real_path, "rb") as f:
+                    self._initramfs_hash = hashlib.md5(f.read()).hexdigest()
         LOG.debug(f"hash={self._initramfs_hash}")
         return self._initramfs_hash
 
     @property
     def build_info(self) -> dict:
         """
         Get dict build information if available
@@ -279,14 +277,16 @@
         @return: String tag in `self.release_repo` corresponding to the newest
             valid release
         """
         include_prerelease = (track or self._default_branch) in ("dev", "beta")
 
         default_time = "2000-01-01T00:00:00Z"
         url = f'https://api.github.com/repos/{self.release_repo}/releases'
+        LOG.debug(f"Getting releases from {self.release_repo}. "
+                  f"prerelease={include_prerelease}")
         releases: list = requests.get(url).json()
         if not include_prerelease:
             releases = [r for r in releases if not r.get('prerelease', True)]
         installed_os = self.build_info.get("base_os", {}).get("name")
         if not installed_os:
             raise RuntimeError(f"Unable to determine installed OS from: "
                                f"{self.build_info}")
@@ -305,14 +305,15 @@
         """
         installed_os = self.build_info.get("base_os", {}).get("name")
         if not installed_os:
             raise RuntimeError(f"Unable to determine installed OS from: "
                                f"{self.build_info}")
         meta_url = (f"https://raw.githubusercontent.com/{self.release_repo}/"
                     f"{tag}/{installed_os}.yaml")
+        LOG.debug(f"Getting metadata from {meta_url}")
         resp = requests.get(meta_url)
         if not resp.ok:
             raise ValueError(f"Unable to get metadata for tag={tag}")
         meta_text = resp.text
         release_meta = yaml.safe_load(meta_text)
 
         return release_meta[0]
@@ -351,24 +352,28 @@
             return True
 
     def check_update_initramfs(self, message: Message):
         """
         Handle a request to check for initramfs updates
         @param message: `neon.check_update_initramfs` Message
         """
-        branch = message.data.get("track") or self._default_branch
+        track = message.data.get("track") or self._default_branch
+        track = "beta" if track in ("dev", "beta") else "stable"
         try:
             meta = self._get_gh_release_meta_from_tag(
-                self._get_gh_latest_release_tag(self._default_branch))
+                self._get_gh_latest_release_tag(track))
             update_available = meta['initramfs']['md5'] != self.initramfs_hash
         except Exception as e:
             LOG.exception(e)
-            update_available = self._legacy_check_initramfs_update_available(branch)
+            meta = dict()
+            update_available = self._legacy_check_initramfs_update_available(track)
         self.bus.emit(message.response({"update_available": update_available,
-                                        "track": branch}))
+                                        "new_meta": meta.get('initramfs'),
+                                        "current_hash": self.initramfs_hash,
+                                        "track": track}))
 
     def check_update_squashfs(self, message: Message):
         """
         Handle a request to check for squash updates
         @param message: `neon.check_update_squashfs` Message
         """
         track = message.data.get("track") or self._default_branch
```

### Comparing `neon-phal-plugin-device-updater-0.2.0/neon_phal_plugin_device_updater.egg-info/PKG-INFO` & `neon-phal-plugin-device-updater-0.2.1a1/neon_phal_plugin_device_updater.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-device-updater
-Version: 0.2.0
+Version: 0.2.1a1
 Summary: Core Module Update Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-device-updater
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-device-updater-0.2.0/setup.py` & `neon-phal-plugin-device-updater-0.2.1a1/setup.py`

 * *Files identical despite different names*

