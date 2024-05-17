# Comparing `tmp/qbitrr2-4.6.8.tar.gz` & `tmp/qbitrr2-4.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbitrr2-4.6.8.tar", last modified: Fri May 17 09:57:33 2024, max compression
+gzip compressed data, was "qbitrr2-4.6.9.tar", last modified: Fri May 17 10:59:06 2024, max compression
```

## Comparing `qbitrr2-4.6.8.tar` & `qbitrr2-4.6.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:57:33.583582 qbitrr2-4.6.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-17 09:57:29.000000 qbitrr2-4.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-17 09:57:33.583582 qbitrr2-4.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-17 09:57:29.000000 qbitrr2-4.6.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-17 09:57:29.000000 qbitrr2-4.6.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:57:33.579582 qbitrr2-4.6.8/qBitrr/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-17 09:57:29.000000 qbitrr2-4.6.8/qBitrr/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   226108 2024-05-17 09:57:29.000000 qbitrr2-4.6.8/qBitrr/arss.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-17 09:57:29.000000 qbitrr2-4.6.8/qBitrr/bundled_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-17 09:57:29.000000 qbitrr2-4.6.8/qBitrr/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-17 09:57:29.000000 qbitrr2-4.6.8/qBitrr/env_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-17 09:57:29.000000 qbitrr2-4.6.8/qBitrr/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-17 09:57:29.000000 qbitrr2-4.6.8/qBitrr/ffprobe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26629 2024-05-17 09:57:29.000000 qbitrr2-4.6.8/qBitrr/gen_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-17 09:57:29.000000 qbitrr2-4.6.8/qBitrr/home_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-17 09:57:29.000000 qbitrr2-4.6.8/qBitrr/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-05-17 09:57:29.000000 qbitrr2-4.6.8/qBitrr/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-17 09:57:29.000000 qbitrr2-4.6.8/qBitrr/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-17 09:57:29.000000 qbitrr2-4.6.8/qBitrr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:57:33.579582 qbitrr2-4.6.8/qBitrr2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-17 09:57:33.000000 qbitrr2-4.6.8/qBitrr2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-17 09:57:33.000000 qbitrr2-4.6.8/qBitrr2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 09:57:33.000000 qbitrr2-4.6.8/qBitrr2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-17 09:57:33.000000 qbitrr2-4.6.8/qBitrr2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-17 09:57:33.000000 qbitrr2-4.6.8/qBitrr2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 09:57:33.000000 qbitrr2-4.6.8/qBitrr2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-17 09:57:33.583582 qbitrr2-4.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 09:57:29.000000 qbitrr2-4.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:59:06.847455 qbitrr2-4.6.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-17 10:59:06.847455 qbitrr2-4.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:59:06.843455 qbitrr2-4.6.9/qBitrr/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/qBitrr/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   225987 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/qBitrr/arss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/qBitrr/bundled_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/qBitrr/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/qBitrr/env_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/qBitrr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/qBitrr/ffprobe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26629 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/qBitrr/gen_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/qBitrr/home_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/qBitrr/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/qBitrr/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/qBitrr/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/qBitrr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:59:06.847455 qbitrr2-4.6.9/qBitrr2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-17 10:59:06.000000 qbitrr2-4.6.9/qBitrr2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-17 10:59:06.000000 qbitrr2-4.6.9/qBitrr2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 10:59:06.000000 qbitrr2-4.6.9/qBitrr2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-17 10:59:06.000000 qbitrr2-4.6.9/qBitrr2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-17 10:59:06.000000 qbitrr2-4.6.9/qBitrr2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 10:59:06.000000 qbitrr2-4.6.9/qBitrr2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-17 10:59:06.851455 qbitrr2-4.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/setup.py
```

### Comparing `qbitrr2-4.6.8/LICENSE` & `qbitrr2-4.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.8/PKG-INFO` & `qbitrr2-4.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qBitrr2
-Version: 4.6.8
+Version: 4.6.9
 Summary: "A simple Python script to talk to qBittorrent and Arr's"
 Home-page: https://github.com/Feramance/qBitrr
 Author: Feramance
 Author-email: fera@fera.wtf
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Feramance/qBitrr/issues
 Project-URL: Source Code, https://github.com/Feramance/qBitrr
```

### Comparing `qbitrr2-4.6.8/README.md` & `qbitrr2-4.6.9/README.md`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.8/pyproject.toml` & `qbitrr2-4.6.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 [tool.black]
 line-length = 99
 target-version = ['py38']
 
 [tool.poetry]
 name = "pypi-public"
-version = "4.6.8"
+version = "4.6.9"
 description = "A simple script to monitor qBit and communicate with Radarr and Sonarr"
 authors = ["Drapersniper", "Feramance"]
 readme = "README.md"
 repository = "https://github.com/Feramance/qBitrr"
 url = "https://pypi.org/simple/"
 
 [tool.autopep8]
```

### Comparing `qbitrr2-4.6.8/qBitrr/arss.py` & `qbitrr2-4.6.9/qBitrr/arss.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,22 +290,23 @@
             )
         self.file_extension_allowlist = re.compile(
             "|".join(self.file_extension_allowlist), re.DOTALL
         )
         self.client = client_cls(host_url=self.uri, api_key=self.apikey)
         if isinstance(self.client, SonarrAPI):
             self.type = "sonarr"
-            version_info = self.client.get_update()
-            self.version = version_parser.parse(version_info[0].get("version"))
-            self.logger.debug("%s version: %s", self._name, self.version.__str__())
         elif isinstance(self.client, RadarrAPI):
             self.type = "radarr"
+
+        try:
             version_info = self.client.get_update()
             self.version = version_parser.parse(version_info[0].get("version"))
             self.logger.debug("%s version: %s", self._name, self.version.__str__())
+        except Exception:
+            self.logger.debug("Failed to get version")
 
         if self.rss_sync_timer > 0:
             self.rss_sync_timer_last_checked = datetime(1970, 1, 1)
         else:
             self.rss_sync_timer_last_checked = None
         if self.refresh_downloads_timer > 0:
             self.refresh_downloads_timer_last_checked = datetime(1970, 1, 1)
```

### Comparing `qbitrr2-4.6.8/qBitrr/config.py` & `qbitrr2-4.6.9/qBitrr/config.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.8/qBitrr/env_config.py` & `qbitrr2-4.6.9/qBitrr/env_config.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.8/qBitrr/errors.py` & `qbitrr2-4.6.9/qBitrr/errors.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.8/qBitrr/ffprobe.py` & `qbitrr2-4.6.9/qBitrr/ffprobe.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.8/qBitrr/gen_config.py` & `qbitrr2-4.6.9/qBitrr/gen_config.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.8/qBitrr/home_path.py` & `qbitrr2-4.6.9/qBitrr/home_path.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.8/qBitrr/logger.py` & `qbitrr2-4.6.9/qBitrr/logger.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.8/qBitrr/main.py` & `qbitrr2-4.6.9/qBitrr/main.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.8/qBitrr/tables.py` & `qbitrr2-4.6.9/qBitrr/tables.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.8/qBitrr/utils.py` & `qbitrr2-4.6.9/qBitrr/utils.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.8/qBitrr2.egg-info/PKG-INFO` & `qbitrr2-4.6.9/qBitrr2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qBitrr2
-Version: 4.6.8
+Version: 4.6.9
 Summary: "A simple Python script to talk to qBittorrent and Arr's"
 Home-page: https://github.com/Feramance/qBitrr
 Author: Feramance
 Author-email: fera@fera.wtf
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Feramance/qBitrr/issues
 Project-URL: Source Code, https://github.com/Feramance/qBitrr
```

### Comparing `qbitrr2-4.6.8/qBitrr2.egg-info/requires.txt` & `qbitrr2-4.6.9/qBitrr2.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.8/setup.cfg` & `qbitrr2-4.6.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qBitrr2
-version = 4.6.8
+version = 4.6.9
 description = "A simple Python script to talk to qBittorrent and Arr's"
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Feramance/qBitrr
 author = Feramance
 author_email = fera@fera.wtf
 license = MIT
```

