# Comparing `tmp/qbitrr2-4.6.1.tar.gz` & `tmp/qbitrr2-4.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbitrr2-4.6.1.tar", last modified: Thu May 16 09:50:00 2024, max compression
+gzip compressed data, was "qbitrr2-4.6.2.tar", last modified: Fri May 17 07:59:44 2024, max compression
```

## Comparing `qbitrr2-4.6.1.tar` & `qbitrr2-4.6.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:50:00.069096 qbitrr2-4.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-16 09:50:00.069096 qbitrr2-4.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:50:00.065096 qbitrr2-4.6.1/qBitrr/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/qBitrr/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   226108 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/qBitrr/arss.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/qBitrr/bundled_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/qBitrr/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/qBitrr/env_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/qBitrr/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/qBitrr/ffprobe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26629 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/qBitrr/gen_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/qBitrr/home_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/qBitrr/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/qBitrr/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/qBitrr/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/qBitrr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:50:00.069096 qbitrr2-4.6.1/qBitrr2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-16 09:50:00.000000 qbitrr2-4.6.1/qBitrr2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-16 09:50:00.000000 qbitrr2-4.6.1/qBitrr2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:50:00.000000 qbitrr2-4.6.1/qBitrr2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 09:50:00.000000 qbitrr2-4.6.1/qBitrr2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-16 09:50:00.000000 qbitrr2-4.6.1/qBitrr2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 09:50:00.000000 qbitrr2-4.6.1/qBitrr2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-16 09:50:00.069096 qbitrr2-4.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 09:49:54.000000 qbitrr2-4.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:59:44.737335 qbitrr2-4.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-17 07:59:40.000000 qbitrr2-4.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-17 07:59:44.737335 qbitrr2-4.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-17 07:59:40.000000 qbitrr2-4.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-17 07:59:40.000000 qbitrr2-4.6.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:59:44.733335 qbitrr2-4.6.2/qBitrr/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-17 07:59:40.000000 qbitrr2-4.6.2/qBitrr/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   226108 2024-05-17 07:59:40.000000 qbitrr2-4.6.2/qBitrr/arss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-17 07:59:40.000000 qbitrr2-4.6.2/qBitrr/bundled_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-17 07:59:40.000000 qbitrr2-4.6.2/qBitrr/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-17 07:59:40.000000 qbitrr2-4.6.2/qBitrr/env_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-17 07:59:40.000000 qbitrr2-4.6.2/qBitrr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-17 07:59:40.000000 qbitrr2-4.6.2/qBitrr/ffprobe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26629 2024-05-17 07:59:40.000000 qbitrr2-4.6.2/qBitrr/gen_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-17 07:59:40.000000 qbitrr2-4.6.2/qBitrr/home_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-17 07:59:40.000000 qbitrr2-4.6.2/qBitrr/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-05-17 07:59:40.000000 qbitrr2-4.6.2/qBitrr/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-17 07:59:40.000000 qbitrr2-4.6.2/qBitrr/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-17 07:59:40.000000 qbitrr2-4.6.2/qBitrr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 07:59:44.733335 qbitrr2-4.6.2/qBitrr2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-17 07:59:44.000000 qbitrr2-4.6.2/qBitrr2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-17 07:59:44.000000 qbitrr2-4.6.2/qBitrr2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 07:59:44.000000 qbitrr2-4.6.2/qBitrr2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-17 07:59:44.000000 qbitrr2-4.6.2/qBitrr2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-17 07:59:44.000000 qbitrr2-4.6.2/qBitrr2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 07:59:44.000000 qbitrr2-4.6.2/qBitrr2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-17 07:59:44.737335 qbitrr2-4.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 07:59:40.000000 qbitrr2-4.6.2/setup.py
```

### Comparing `qbitrr2-4.6.1/LICENSE` & `qbitrr2-4.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.1/PKG-INFO` & `qbitrr2-4.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qBitrr2
-Version: 4.6.1
+Version: 4.6.2
 Summary: "A simple Python script to talk to qBittorrent and Arr's"
 Home-page: https://github.com/Feramance/qBitrr
 Author: Feramance
 Author-email: fera@fera.wtf
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Feramance/qBitrr/issues
 Project-URL: Source Code, https://github.com/Feramance/qBitrr
```

### Comparing `qbitrr2-4.6.1/README.md` & `qbitrr2-4.6.2/README.md`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.1/pyproject.toml` & `qbitrr2-4.6.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 [tool.black]
 line-length = 99
 target-version = ['py38']
 
 [tool.poetry]
 name = "pypi-public"
-version = "4.6.1"
+version = "4.6.2"
 description = "A simple script to monitor qBit and communicate with Radarr and Sonarr"
 authors = ["Drapersniper", "Feramance"]
 readme = "README.md"
 repository = "https://github.com/Feramance/qBitrr"
 url = "https://pypi.org/simple/"
 
 [tool.autopep8]
```

### Comparing `qbitrr2-4.6.1/qBitrr/arss.py` & `qbitrr2-4.6.2/qBitrr/arss.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.1/qBitrr/config.py` & `qbitrr2-4.6.2/qBitrr/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         "-s",
         "-h",
         "--help",
     ]
 ):
     CONFIG = MyConfig(CONFIG_FILE, config=generate_doc())
     COPIED_TO_NEW_DIR = None
-elif (not CONFIG_FILE.exists()) and (not CONFIG_PATH.exists()):
+elif (not CONFIG_FILE.exists()) or (not CONFIG_PATH.exists()):
     print(f"{file} has not been found")
 
     CONFIG_FILE = _write_config_file(docker=True)
     print(f"'{CONFIG_FILE.name}' has been generated")
     print('Rename it to "config.toml" then edit it and restart the container')
 
     sys.exit
```

### Comparing `qbitrr2-4.6.1/qBitrr/env_config.py` & `qbitrr2-4.6.2/qBitrr/env_config.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.1/qBitrr/errors.py` & `qbitrr2-4.6.2/qBitrr/errors.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.1/qBitrr/ffprobe.py` & `qbitrr2-4.6.2/qBitrr/ffprobe.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.1/qBitrr/gen_config.py` & `qbitrr2-4.6.2/qBitrr/gen_config.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.1/qBitrr/home_path.py` & `qbitrr2-4.6.2/qBitrr/home_path.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.1/qBitrr/logger.py` & `qbitrr2-4.6.2/qBitrr/logger.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.1/qBitrr/main.py` & `qbitrr2-4.6.2/qBitrr/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,27 +30,25 @@
 from qBitrr.ffprobe import FFprobeDownloader
 from qBitrr.home_path import HOME_PATH
 from qBitrr.logger import run_logs
 from qBitrr.utils import ExpiringSet, absolute_file_paths
 
 CHILD_PROCESSES = []
 
+logger = logging.getLogger(f"qBitrr")
 if ENABLE_LOGS:
     LOGS_FOLDER = HOME_PATH.joinpath("logs")
     LOGS_FOLDER.mkdir(parents=True, exist_ok=True)
     LOGS_FOLDER.chmod(mode=0o777)
     logfile = LOGS_FOLDER.joinpath("qBitrr.log")
     if pathlib.Path(logfile).is_file():
         logold = LOGS_FOLDER.joinpath("qBitrr.log.old")
         logfile.rename(logold)
     fh = logging.FileHandler(logfile)
-    logger = logging.getLogger(f"qBitrr")
     logger.addHandler(fh)
-else:
-    logger = logging.getLogger(f"qBitrr")
 run_logs(logger)
 
 
 class qBitManager:
     min_supported_version = VersionClass("4.3.9")
     soft_not_supported_supported_version = VersionClass("4.4.4")
     # max_supported_version = VersionClass("4.6.2")
@@ -58,27 +56,25 @@
 
     def __init__(self):
         self._name = "Manager"
         self.qBit_Host = CONFIG.get("qBit.Host", fallback="localhost")
         self.qBit_Port = CONFIG.get("qBit.Port", fallback=8105)
         self.qBit_UserName = CONFIG.get("qBit.UserName", fallback=None)
         self.qBit_Password = CONFIG.get("qBit.Password", fallback=None)
+        self.logger = logging.getLogger(f"qBitrr.{self._name}")
         if ENABLE_LOGS:
             LOGS_FOLDER = HOME_PATH.joinpath("logs")
             LOGS_FOLDER.mkdir(parents=True, exist_ok=True)
             LOGS_FOLDER.chmod(mode=0o777)
             logfile = LOGS_FOLDER.joinpath(self._name + ".log")
             if pathlib.Path(logfile).is_file():
                 logold = LOGS_FOLDER.joinpath(self._name + ".log.old")
                 logfile.rename(logold)
             fh = logging.FileHandler(logfile)
-            self.logger = logging.getLogger(f"qBitrr.{self._name}")
             self.logger.addHandler(fh)
-        else:
-            self.logger = logging.getLogger(f"qBitrr.{self._name}")
         run_logs(self.logger)
         self.logger.debug(
             "qBitTorrent Config: Host: %s Port: %s, Username: %s, Password: %s",
             self.qBit_Host,
             self.qBit_Port,
             self.qBit_UserName,
             self.qBit_Password,
```

### Comparing `qbitrr2-4.6.1/qBitrr/tables.py` & `qbitrr2-4.6.2/qBitrr/tables.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.1/qBitrr/utils.py` & `qbitrr2-4.6.2/qBitrr/utils.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.1/qBitrr2.egg-info/PKG-INFO` & `qbitrr2-4.6.2/qBitrr2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qBitrr2
-Version: 4.6.1
+Version: 4.6.2
 Summary: "A simple Python script to talk to qBittorrent and Arr's"
 Home-page: https://github.com/Feramance/qBitrr
 Author: Feramance
 Author-email: fera@fera.wtf
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Feramance/qBitrr/issues
 Project-URL: Source Code, https://github.com/Feramance/qBitrr
```

### Comparing `qbitrr2-4.6.1/qBitrr2.egg-info/requires.txt` & `qbitrr2-4.6.2/qBitrr2.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.1/setup.cfg` & `qbitrr2-4.6.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qBitrr2
-version = 4.6.1
+version = 4.6.2
 description = "A simple Python script to talk to qBittorrent and Arr's"
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Feramance/qBitrr
 author = Feramance
 author_email = fera@fera.wtf
 license = MIT
```

