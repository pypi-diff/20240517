# Comparing `tmp/qbitrr2-4.6.6.tar.gz` & `tmp/qbitrr2-4.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbitrr2-4.6.6.tar", last modified: Fri May 17 08:51:20 2024, max compression
+gzip compressed data, was "qbitrr2-4.6.7.tar", last modified: Fri May 17 09:28:19 2024, max compression
```

## Comparing `qbitrr2-4.6.6.tar` & `qbitrr2-4.6.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:51:20.515415 qbitrr2-4.6.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-17 08:51:16.000000 qbitrr2-4.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-17 08:51:20.515415 qbitrr2-4.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-17 08:51:16.000000 qbitrr2-4.6.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-17 08:51:16.000000 qbitrr2-4.6.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:51:20.511415 qbitrr2-4.6.6/qBitrr/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-17 08:51:16.000000 qbitrr2-4.6.6/qBitrr/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   226108 2024-05-17 08:51:16.000000 qbitrr2-4.6.6/qBitrr/arss.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-17 08:51:16.000000 qbitrr2-4.6.6/qBitrr/bundled_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-05-17 08:51:16.000000 qbitrr2-4.6.6/qBitrr/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-17 08:51:16.000000 qbitrr2-4.6.6/qBitrr/env_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-17 08:51:16.000000 qbitrr2-4.6.6/qBitrr/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-17 08:51:16.000000 qbitrr2-4.6.6/qBitrr/ffprobe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26629 2024-05-17 08:51:16.000000 qbitrr2-4.6.6/qBitrr/gen_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-17 08:51:16.000000 qbitrr2-4.6.6/qBitrr/home_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-17 08:51:16.000000 qbitrr2-4.6.6/qBitrr/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8415 2024-05-17 08:51:16.000000 qbitrr2-4.6.6/qBitrr/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-17 08:51:16.000000 qbitrr2-4.6.6/qBitrr/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-17 08:51:16.000000 qbitrr2-4.6.6/qBitrr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:51:20.515415 qbitrr2-4.6.6/qBitrr2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-17 08:51:20.000000 qbitrr2-4.6.6/qBitrr2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-17 08:51:20.000000 qbitrr2-4.6.6/qBitrr2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 08:51:20.000000 qbitrr2-4.6.6/qBitrr2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-17 08:51:20.000000 qbitrr2-4.6.6/qBitrr2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-17 08:51:20.000000 qbitrr2-4.6.6/qBitrr2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 08:51:20.000000 qbitrr2-4.6.6/qBitrr2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-17 08:51:20.519415 qbitrr2-4.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 08:51:16.000000 qbitrr2-4.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:28:19.796818 qbitrr2-4.6.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-17 09:28:07.000000 qbitrr2-4.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-17 09:28:19.796818 qbitrr2-4.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-17 09:28:07.000000 qbitrr2-4.6.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-17 09:28:07.000000 qbitrr2-4.6.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:28:19.792818 qbitrr2-4.6.7/qBitrr/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-17 09:28:07.000000 qbitrr2-4.6.7/qBitrr/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   226108 2024-05-17 09:28:07.000000 qbitrr2-4.6.7/qBitrr/arss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-17 09:28:07.000000 qbitrr2-4.6.7/qBitrr/bundled_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-05-17 09:28:07.000000 qbitrr2-4.6.7/qBitrr/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-17 09:28:07.000000 qbitrr2-4.6.7/qBitrr/env_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-17 09:28:07.000000 qbitrr2-4.6.7/qBitrr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-17 09:28:07.000000 qbitrr2-4.6.7/qBitrr/ffprobe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26629 2024-05-17 09:28:07.000000 qbitrr2-4.6.7/qBitrr/gen_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-17 09:28:07.000000 qbitrr2-4.6.7/qBitrr/home_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-17 09:28:07.000000 qbitrr2-4.6.7/qBitrr/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-05-17 09:28:07.000000 qbitrr2-4.6.7/qBitrr/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-17 09:28:07.000000 qbitrr2-4.6.7/qBitrr/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-17 09:28:07.000000 qbitrr2-4.6.7/qBitrr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:28:19.792818 qbitrr2-4.6.7/qBitrr2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-17 09:28:19.000000 qbitrr2-4.6.7/qBitrr2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-17 09:28:19.000000 qbitrr2-4.6.7/qBitrr2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 09:28:19.000000 qbitrr2-4.6.7/qBitrr2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-17 09:28:19.000000 qbitrr2-4.6.7/qBitrr2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-17 09:28:19.000000 qbitrr2-4.6.7/qBitrr2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 09:28:19.000000 qbitrr2-4.6.7/qBitrr2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-17 09:28:19.796818 qbitrr2-4.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 09:28:07.000000 qbitrr2-4.6.7/setup.py
```

### Comparing `qbitrr2-4.6.6/LICENSE` & `qbitrr2-4.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.6/PKG-INFO` & `qbitrr2-4.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qBitrr2
-Version: 4.6.6
+Version: 4.6.7
 Summary: "A simple Python script to talk to qBittorrent and Arr's"
 Home-page: https://github.com/Feramance/qBitrr
 Author: Feramance
 Author-email: fera@fera.wtf
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Feramance/qBitrr/issues
 Project-URL: Source Code, https://github.com/Feramance/qBitrr
```

### Comparing `qbitrr2-4.6.6/README.md` & `qbitrr2-4.6.7/README.md`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.6/pyproject.toml` & `qbitrr2-4.6.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 [tool.black]
 line-length = 99
 target-version = ['py38']
 
 [tool.poetry]
 name = "pypi-public"
-version = "4.6.6"
+version = "4.6.7"
 description = "A simple script to monitor qBit and communicate with Radarr and Sonarr"
 authors = ["Drapersniper", "Feramance"]
 readme = "README.md"
 repository = "https://github.com/Feramance/qBitrr"
 url = "https://pypi.org/simple/"
 
 [tool.autopep8]
```

### Comparing `qbitrr2-4.6.6/qBitrr/arss.py` & `qbitrr2-4.6.7/qBitrr/arss.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.6/qBitrr/config.py` & `qbitrr2-4.6.7/qBitrr/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 elif (not CONFIG_FILE.exists()) or (not CONFIG_PATH.exists()):
     print(f"{file} has not been found")
 
     CONFIG_FILE = _write_config_file(docker=True)
     print(f"'{CONFIG_FILE.name}' has been generated")
     print('Rename it to "config.toml" then edit it and restart the container')
 
-    raise SystemExit
+    sys.exit(0)
 
 elif CONFIG_FILE.exists():
     CONFIG = MyConfig(CONFIG_FILE)
 else:
     with contextlib.suppress(
         Exception
     ):  # If file already exist or can't copy to APPDATA_FOLDER ignore the exception
```

### Comparing `qbitrr2-4.6.6/qBitrr/env_config.py` & `qbitrr2-4.6.7/qBitrr/env_config.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.6/qBitrr/errors.py` & `qbitrr2-4.6.7/qBitrr/errors.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.6/qBitrr/ffprobe.py` & `qbitrr2-4.6.7/qBitrr/ffprobe.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.6/qBitrr/gen_config.py` & `qbitrr2-4.6.7/qBitrr/gen_config.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.6/qBitrr/home_path.py` & `qbitrr2-4.6.7/qBitrr/home_path.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.6/qBitrr/logger.py` & `qbitrr2-4.6.7/qBitrr/logger.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.6/qBitrr/main.py` & `qbitrr2-4.6.7/qBitrr/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 from qBitrr.ffprobe import FFprobeDownloader
 from qBitrr.home_path import HOME_PATH
 from qBitrr.logger import run_logs
 from qBitrr.utils import ExpiringSet, absolute_file_paths
 
 CHILD_PROCESSES = []
 
-# if (not CONFIG_FILE.exists()) or (not CONFIG_PATH.exists()):
-#     raise SystemExit
+if (not CONFIG_FILE.exists()) or (not CONFIG_PATH.exists()):
+    sys.exit(0)
 logger = logging.getLogger(f"qBitrr")
 if ENABLE_LOGS:
     LOGS_FOLDER = HOME_PATH.joinpath("logs")
     LOGS_FOLDER.mkdir(parents=True, exist_ok=True)
     LOGS_FOLDER.chmod(mode=0o777)
     logfile = LOGS_FOLDER.joinpath("qBitrr.log")
     if pathlib.Path(logfile).is_file():
```

### Comparing `qbitrr2-4.6.6/qBitrr/tables.py` & `qbitrr2-4.6.7/qBitrr/tables.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.6/qBitrr/utils.py` & `qbitrr2-4.6.7/qBitrr/utils.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.6/qBitrr2.egg-info/PKG-INFO` & `qbitrr2-4.6.7/qBitrr2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qBitrr2
-Version: 4.6.6
+Version: 4.6.7
 Summary: "A simple Python script to talk to qBittorrent and Arr's"
 Home-page: https://github.com/Feramance/qBitrr
 Author: Feramance
 Author-email: fera@fera.wtf
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Feramance/qBitrr/issues
 Project-URL: Source Code, https://github.com/Feramance/qBitrr
```

### Comparing `qbitrr2-4.6.6/qBitrr2.egg-info/requires.txt` & `qbitrr2-4.6.7/qBitrr2.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.6/setup.cfg` & `qbitrr2-4.6.7/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qBitrr2
-version = 4.6.6
+version = 4.6.7
 description = "A simple Python script to talk to qBittorrent and Arr's"
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Feramance/qBitrr
 author = Feramance
 author_email = fera@fera.wtf
 license = MIT
```

